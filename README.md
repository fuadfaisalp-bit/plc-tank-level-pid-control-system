# PLC Tank Level Control System using Siemens TIA Portal & Factory I/O

## Overview

This project demonstrates the implementation of a complete tank level control system using Siemens TIA Portal, PLCSIM, and Factory I/O.

The project progresses through three stages of industrial process control:

1. Manual Analog Valve Control
2. Automatic Level Control
3. PID-Based Closed Loop Control

The objective is to understand how analog signals are processed, how process variables are controlled, and how PID controllers are used in real industrial automation systems.

---

## Software Used

* Siemens TIA Portal
* Siemens S7-1500 PLC
* S7-PLCSIM
* Factory I/O

---

## Skills Demonstrated

* PLC Programming (LAD)
* Analog Input Processing
* Analog Output Control
* NORM_X Function
* SCALE_X Function
* Process Variable Scaling
* Comparator Instructions
* Automatic Level Control
* PID_Compact Configuration
* PID Tuning
* OB30 Cyclic Interrupt Programming
* Process Monitoring and Trace Analysis

---

# Phase 1 - Manual Valve Control

## Objective

Understand analog process behavior before implementing automatic control.

The tank level is manually controlled by changing the valve opening percentage. The raw analog level signal is converted into engineering units using NORM_X and SCALE_X.

### Features

* Manual analog valve control
* Raw analog value scaling
* Tank level percentage calculation
* High level alarm generation

---

### Factory I/O Tank Scene

![Factory IO Tank Scene](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_factoryio_tank_scene.png)

---

### Analog Valve Control Logic

![Analog Valve Control](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_analog_valve_control.png)

---

### NORM_X Scaling

![NORM\_X Scaling](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_norm_x_scaling.png)

---

### SCALE_X Scaling

![SCALE\_X Scaling](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_scale_x_scaling.png)

---

### Watch Table Monitoring

![Watch Table Monitoring](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_watch_table_monitoring.png)

---

### High Level Alarm Logic

![High Level Alarm Logic](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_high_level_alarm_logic.png)

---

### High Level Alarm Active

![High Level Alarm Active](Phase%201%20-%20Manual%20Valve%20Control/Screenshots/phase1_high_level_alarm_active.png)

---

### Demo Video

[Watch Demo](Phase%201%20-%20Manual%20Valve%20Control/Videos/demo.mp4)

---

# Phase 2 - Automatic Level Control

## Objective

Implement automatic filling and draining logic based on tank level thresholds.

The PLC automatically fills the tank when the level falls below the low limit and drains the tank when the level exceeds the high limit.

### Features

* Automatic filling
* Automatic draining
* Level-based decision making
* Process automation without PID

---

### Auto Fill Logic

![Auto Fill Logic](Phase%202%20-%20Automatic%20Level%20Control/Screenshots/phase2_auto_fill_logic.png)

---

### Auto Drain Logic

![Auto Drain Logic](Phase%202%20-%20Automatic%20Level%20Control/Screenshots/phase2_auto_drain_logic.png)

---

### Tank at Low Level

![Tank at Low Level](Phase%202%20-%20Automatic%20Level%20Control/Screenshots/phase2_factoryio_tank_at_low_level.png)

---

### Tank at High Level

![Tank at High Level](Phase%202%20-%20Automatic%20Level%20Control/Screenshots/phase2_factoryio_tank_at_high_level.png)

---

### Watch Table Auto Control

![Watch Table Auto Control](Phase%202%20-%20Automatic%20Level%20Control/Screenshots/phase2_watch_table_auto_control.png)

---

### Demo Video

[Watch Demo](Phase%202%20-%20Automatic%20Level%20Control/Videos/demo.mp4)

---

# Phase 3 - PID Control

## Objective

Implement closed-loop level control using Siemens PID_Compact technology object.

A potentiometer is used to adjust the setpoint in real time. The PID controller automatically regulates the valve position to maintain the desired tank level.

### Features

* PID_Compact Technology Object
* Dynamic Setpoint Control
* Closed Loop Level Control
* Automatic PID Tuning
* Trace Analysis
* OB30 Cyclic Interrupt Execution

---

### Factory I/O PID Operation

![Factory IO PID Operation](Phase%203%20-%20PID%20Control/Screenshots/phase3_factoryio_pid_operation.png)

---

### PID Program in OB30

![PID Program OB30](Phase%203%20-%20PID%20Control/Screenshots/phase3_pid_program_ob30.png)

---

### PID Parameters

![PID Parameters](Phase%203%20-%20PID%20Control/Screenshots/phase3_pid_parameters.png)

---

### PID Trace Analysis

![PID Trace Analysis](Phase%203%20-%20PID%20Control/Screenshots/phase3_pid_trace_analysis.png)

---

### Demo Video

[Watch Demo](Phase%203%20-%20PID%20Control/Videos/demo.mp4)

---

# Process Control Concepts Learned

### Process Variable (PV)

Tank Level (%)

### Setpoint (SP)

Desired Tank Level (%)

### Control Variable (CV)

Valve Opening (%)

### PID Performance Metrics

* Rise Time
* Settling Time
* Overshoot
* Oscillation

---

# Project Outcome

This project demonstrates the complete development of a process control system from manual operation to fully automated PID control.

The final PID implementation successfully maintains the tank level at the desired setpoint while automatically adjusting the valve position based on process conditions.

---

## Author

**Fuad Faisal**

Automation & Control Systems Engineer

PLC | SCADA | Industrial Automation | Process Control
