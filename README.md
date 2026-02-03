# PLC-Delta-Robot-Control
This project involves the PLC-based control of a Delta Robot used for high-speed pick-and-place operations. The system includes motion coordination, safety interlocks, and object detection via sensors

## 🎬 System Demonstration
![Delta Robot Demo](Delta.gif)

## 💻 PLC Program Architecture

The control software is structured using a hierarchical state-machine and modular motion control blocks.

### 🔁 Main State Machine

The system operates using defined machine states:
- **Reset_State** – System reset
- **Resetting_State** – System reset and homing checks  
- **Idle_State** – Waiting for start command  
- **Starting_State** – Pre-start checks and robot enable  
- **Running_State** – Normal automatic pick-and-place operation  
- **Stopping_State** – Controlled stop sequence  
- **Aborting_State** – Emergency or fault stop handling  
- **Manual_State** – Manual mode  

---

### Robot Motion Program 

Handles all robot-related motion coordination.

Submodules:

- **R1_Servo_Ctrl** – Servo enable, status monitoring, and motion permission  
- **R1_Robot_Init** – Robot initialization and homing sequence  
- **R1_Automatic** – Automatic pick-and-place
## 🔒 Note on Source Code

The full PLC program is not publicly available due to academic project restrictions.  
However, system architecture, control strategy, and engineering approach are documented here to demonstrate technical competence.
