# 🤖 Maze-Navigating mBot  
<img width="316" height="192" alt="image" src="https://github.com/user-attachments/assets/13d45b6f-ca9a-475a-8841-606ab64ec030" />
<img width="493" height="337" alt="image" src="https://github.com/user-attachments/assets/196ec2d1-42f5-43ea-ba35-84d8fae837ac" />

The mBot is an **autonomous robot** designed to navigate a maze while completing waypoint challenges. It integrates **custom sensor circuits, real-time control algorithms, and Arduino-based firmware** to traverse mazes efficiently and respond to colored waypoints.  

---

🌟 **Features**  

🚀 **Autonomous Navigation**  
Uses **ultrasonic and IR sensors** for obstacle detection and wall-following, with proportional control for smooth, straight-line movement.  

🎨 **Color-Based Waypoint Detection**  
Custom RGB LED + LDR sensor circuit identifies waypoint colors, triggering the robot to execute precise turn commands.  

⚙️ **Actuation & Output**  
Includes a **catapult mechanism** for object interaction and a **buzzer** that signals maze completion.  

🛠️ **Hardware Architecture**  

| Component       | Role |
|-----------------|------|
| Arduino Uno     | Runs navigation firmware, reads sensor inputs, and controls motors & actuators |
| Ultrasonic Sensor | Detects walls and obstacles for proportional navigation |
| IR Sensor       | Provides backup obstacle detection when ultrasonic readings are unavailable |
| RGB + LDR Sensor | Detects waypoint colors to determine turning actions |
| Motors & Encoders | Drive wheels, provide odometry feedback for precise motion |
| Buzzer & Catapult | Provide end-of-maze celebration and object manipulation |

---

💡 **Firmware Overview**  

**Arduino Uno**  
- Executes low-level movement commands and actuator control  
- Reads ultrasonic and IR sensors for obstacle detection  
- Processes LDR readings to detect waypoint colors  
- Implements proportional control and nudging for accurate maze traversal  
- Integrates catapult and buzzer actuation at specific waypoints  

---

🎯 **Mission Scenario**  
- Navigate maze without bumping into walls  
- Stop at waypoints and decode color signals 🎨  
- Execute corresponding turn or action at each waypoint  
- Celebrate at the end of the maze with buzzer activation 🔔  

---

⚡ **Design Highlights**  
- **Custom IR & Color Sensor Circuits:** Designed emitter-detector circuits and optimized LED biasing for reliable readings  
- **Proportional Control Algorithm:** Ensures smooth straight-line navigation  
- **Iterative Calibration:** Fine-tuned sensor readings and actuator responses for consistent performance  

---

📝 **Installation & Setup**  
1. Assemble mBot chassis and attach sensors per wiring diagram 🔌  
2. Flash Arduino Uno firmware for navigation, sensor reading, and actuator control  
3. Calibrate IR and RGB sensors for local lighting conditions  
4. Place mBot at maze start and run autonomous navigation routine 🚀  

---

🌍 **Potential Applications**  
- Autonomous maze-solving and obstacle navigation training  
- Embedded systems and robotics education  
- Prototyping sensor-driven robotic behaviors in constrained environments  
