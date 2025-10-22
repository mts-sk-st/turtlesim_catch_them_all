# 🐢 Turtlesim Catch Them All (ROS2)

A ROS2 project where a main turtle chases and catches randomly spawned turtles in the Turtlesim simulator.  
Implemented in **both Python and C++** to demonstrate cross-language ROS2 development.

---

## 📖 Overview

The goal is to:
- Spawn turtles one by one in the Turtlesim environment.
- Control the main turtle to catch the nearest one.
- Remove turtles once they are caught.

The project demonstrates:
- ROS2 **topics**, **services**, and **custom messages**.
- Writing ROS2 nodes in **Python** and **C++**.
- Organizing a multi-package ROS2 workspace.

---

## 📂 Repository Structure
```code 
turtlesim_catch_them_all/
|
│── my_robot_bringup/         # Launch & config files      # Shared bringup
│── my_robot_interfaces/      # Custom messages & services # Shared interfaces
|
|── python_version/
│   └── turtlesim_catch_them_all/ # Python nodes (controller, spawner)
│
├── cpp_version/
│  └── turtlesim_project_cpp/    # C++ nodes (controller, spawner)
│
├── README.md
```
## 🚀 Features
- **Custom ROS2 messages** (`Turtle.msg`, `TurtleArray.msg`)  
- **Custom ROS2 service** (`CatchTurtle.srv`)  
- **Spawner node**: publishes new turtles at random positions  
- **Controller node**: moves the main turtle to catch the nearest one  
- **Cross-language implementation**: Python and C++ versions

```
## ▶️ Run Instructions
### Python & C++ :
```bash 
ros2 launch my_robot_bringup turtlesim_catch_them_all.launch.xml
```

## 📊 Comparison: Python vs C++

| Feature                  | Python Implementation | C++ Implementation |
|---------------------------|-----------------------|--------------------|
| Ease of writing           | ✅ Faster prototyping | ⚡ High performance |
| Code readability          | 🟢 Very clear         | 🟡 More verbose     |
| Execution speed           | 🟡 Slower             | 🟢 Faster           |
| ROS2 ecosystem support    | ✅ Widely used        | ✅ Widely used      |

## 📸 Demo
![Turtlesim Demo](/docs/demo.gif)

### Python & C++ implementations of the turtle-catching game in ROS2
 ---

## 📚 Learning Outcomes
- Practiced **ROS2 node development** in both Python and C++.

- Learned to define and use **custom messages and services.**

- Gained experience in **multi-package workspace organization.**

- Showcased ability to **translate logic across languages.**
