# 🤖 ABB RobotStudio: Vision-Guided Pick & Place Simulation

This project demonstrates a fully automated industrial robotic cell developed using **ABB RobotStudio** and the **RAPID** programming language. The simulation showcases a "Pick & Place" workflow where a robot uses vision-guided logic to organize randomized objects.

---

## ✨ Key Features

* **Vision System Integration:** Simulated camera feedback to detect object position ($X, Y, Z$) and rotation in real-time.
* **Dynamic Pick-and-Place:** Handles objects generated in randomized locations and orientations.
* **Vacuum Gripper Control:** Implementation of smart components to simulate suction physics and vacuum activation.
* **Orientation Sync:** The robot dynamically calculates and adjusts its tool orientation to match the workpiece rotation.
* **Automated Packaging:** Systematic placement of picked items into a structured box/container.

---

## 🚀 Technologies & Tools

* **ABB RAPID:** Industrial robot programming (logic, motion, and I/O).
* **RobotStudio:** 3D simulation and offline programming (OLP).
* **Smart Components:** For simulating physics, sensors, and the vacuum tool.
* **Virtual Controller:** Used to run the simulated RAPID code.

---

## 📂 Project Workflow (Logic)

1.  **Scanning:** The robot waits at a home position until the vision sensor identifies a new workpiece on the workspace.
2.  **Data Acquisition:** The system retrieves the target's coordinates and orientation from the simulated vision system.
3.  **Pick Sequence:** The robot performs an approach move, activates the **Vacuum Gripper** via Digital Output (DO), and secures the object.
4.  **Transport:** Collision-free path execution from the source area to the destination box.
5.  **Place & Reset:** The object is released at the designated slot, and the robot returns to the scanning phase.

---

## 🛠 Skills & Competencies

* **Industrial Robot Programming:** Writing structured RAPID code for production cycles.
* **Cell Design:** Building 3D robotic environments with conveyors, tools, and sensors.
* **Signal Handling:** Managing Digital I/O for sensor-actor synchronization.
* **Problem Solving:** Handling randomized inputs to ensure system robustness.
