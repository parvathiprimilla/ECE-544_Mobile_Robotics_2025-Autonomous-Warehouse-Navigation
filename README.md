# ECE 544 – Mobile Robotics  
## Autonomous Warehouse Navigation

This repository contains code and materials for an **Autonomous Warehouse Navigation** project completed as part of **ECE 544 – Mobile Robotics**, a university course.

---

## Project Context

This repository is a **fork of the original project repository** created for a **group-based university course project**.  
It is maintained here **for academic reference, personal learning, experimentation, and portfolio purposes**.

All original authorship and credit from the upstream repository are fully preserved.

---

## Autonomous Warehouse Navigation

This project contains a complete simulation setup for a mobile robot operating in a warehouse environment using **ROS** and **Gazebo**. The system integrates mapping, localization, and navigation components to enable autonomous motion in a structured indoor environment.

Key capabilities include:
- SLAM using Gmapping
- Localization using AMCL
- Autonomous navigation with `move_base`
- URDF-based robot modeling
- Simulation in a custom Gazebo warehouse world

---

## 👥 Team Contributions

This project was completed as a collaborative university course effort.  
Individual contributions are listed below for clarity and transparency.

### **Parvathi Primilla**
🔧 **Technical Contributions:**
- Implemented **SLAM-based mapping pipelines** for accurate environment representation
- Configured the **ROS navigation stack** to enable autonomous path planning and execution
- Developed and integrated **sensor fusion techniques** to improve localization and navigation reliability
- Played a key role in **system-level debugging, testing, and launch file development** to ensure seamless integration of perception, localization, and navigation modules

👥 **Project Impact:**  
This project provided hands-on experience in translating theoretical robotics concepts into a fully functional autonomous system. My work emphasized system robustness, integration, and performance validation in a realistic warehouse environment.  
This fork is maintained to support experimentation, learning, and portfolio demonstration.

---

### **Hemanth Katikala Muniraj**
🔧 **Technical Contributions:**
- Built and optimized the **robot model using URDF**
- Designed a realistic **Gazebo-based warehouse simulation**
- Integrated multiple sensors and debugged **TF transformations and ROS topics**
- Used teleoperation for **SLAM-based mapping** and **AMCL** for localization
- Configured autonomous navigation using `move_base` and 2D Nav Goals

👥 **Collaboration:**  
We jointly contributed to debugging, testing, and launch file development to ensure stable and reliable system performance.

---


## 📁 Project Structure

```
Final/
├── launch/                  # ROS launch files for various components
├── meshes/                  # 3D model files (e.g., sensors)
├── urdf/                    # Robot URDF and xacro descriptions
├── model/                   # Gazebo model configuration files
├── Map/                     # Predefined map (YAML and PGM)
└── worlds/                  # Gazebo world file
```

## 🚀 Launch Instructions

Make sure you have ROS (preferably Noetic) installed and sourced.

```bash
cd Final
roslaunch launch/world.launch             # Launch the Gazebo world
roslaunch launch/robot_description.launch # Load robot description
roslaunch launch/gmapping_demo.launch     # Run SLAM using Gmapping
roslaunch launch/localization.launch      # Run localization (AMCL)
roslaunch launch/navigation.launch        # Start move_base navigation
```

## 🧰 Dependencies

- ROS (Noetic)
- Gazebo (compatible with your ROS version)
- `gmapping`, `amcl`, `move_base`, and other navigation stack packages

## 🗺️ Map

The map is located in the `Map/` directory and is used for localization and navigation.

## 🧪 World

The custom Gazebo world is defined in `worlds/Warehouse1.world`.

---

## Usage & Attribution

This repository is shared **for academic reference, personal learning, and portfolio demonstration purposes only**.

The project was developed as part of a collaborative university course effort.  
All original credit and authorship are acknowledged.  
No claim of sole ownership is made.

If you are a student or researcher interested in similar work, please use this repository as a **reference** rather than a redistributable software package.
