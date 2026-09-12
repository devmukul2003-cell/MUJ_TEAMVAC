# TeamVAC--- Autonomous Multi-Surface Cleaning Robot

## Hackathon Project --- MUJ HACKX 4.0

**Team:** Vac\
**Team ID:** 107\
**Problem Statement:** Wild Card Innovation Challenge\
**Theme:** Open Innovation

------------------------------------------------------------------------

## 1. Overview

Vac-Robo is an autonomous robotic cleaning system designed to extend
robotic cleaning beyond conventional floors to **vertical walls, glass,
stairs, and inclined surfaces**.

The project addresses a simple but important problem: floor-cleaning
robots are already common, while cleaning vertical and elevated surfaces
still requires significant manual effort and can involve safety risks.

Vac-Robo combines **vacuum-based adhesion, motorized mobility, cleaning,
sensing, and embedded control** into a single compact robotic platform.

> **One robot. Every surface.**

------------------------------------------------------------------------

## 2. Problem

Conventional robotic vacuum cleaners primarily operate on floors.
Cleaning walls, glass, stairs, and other elevated surfaces often remains
manual.

This creates three major challenges:

-   **Limited vertical reach** --- conventional robotic cleaners are
    designed mainly for floors.
-   **Manual risk and cost** --- elevated and vertical cleaning can be
    slow, labour-intensive, and unsafe.
-   **Limited multi-surface automation** --- intelligent cleaning has
    advanced significantly on floors, but autonomous multi-surface
    cleaning remains comparatively uncommon.

------------------------------------------------------------------------

## 3. Our Solution

Vac-Robo uses a **vacuum adhesion mechanism** to maintain contact with a
vertical surface while its drive system moves the robot.

The complete robot combines:

-   Vacuum adhesion
-   Motorized wheel assembly
-   Stabilization and suspension mechanisms
-   Cleaning mechanism
-   Embedded controller
-   Sensor-based navigation
-   Obstacle detection
-   Autonomous motion control

The current hardware platform has been physically built. The remaining
major development step is to move from direct/manual control to
**wireless autonomous control using a transmitter and receiver
architecture**.

------------------------------------------------------------------------

## 4. Current Development Status

### Hardware --- Completed

The physical robot has been assembled and the major mechanical and
electronic systems are in place.

The working system includes:

-   Wall-climbing body
-   Vacuum/suction system
-   Drive motors
-   Motor controllers/ESCs
-   ESP32-based control electronics
-   Battery power system
-   Cleaning/brush mechanism
-   Mechanical suspension/stabilization
-   3D-printed mechanical components

### Control --- Final Development Stage

The robot is currently controllable through the ESP32.

The next step is to implement:

**Transmitter → Wireless communication → Receiver ESP32 → Motor/actuator
control**

This will eliminate the need for a direct wired control connection and
provide the foundation for autonomous operation.

------------------------------------------------------------------------

## 5. Automation Architecture

The planned control architecture is:

``` text
┌──────────────────────┐
│   TRANSMITTER ESP32  │
│                      │
│ • User commands      │
│ • Joystick/buttons   │
│ • Speed control      │
└──────────┬───────────┘
           │
           │ Wireless
           ▼
┌──────────────────────┐
│    RECEIVER ESP32    │
│                      │
│ • Receives commands  │
│ • Processes commands │
│ • Safety handling    │
└──────────┬───────────┘
           │
     ┌─────┴─────┐
     ▼           ▼
┌──────────┐ ┌──────────────┐
│ Drive    │ │ Vacuum /     │
│ Motors   │ │ Cleaning     │
│ ESC      │ │ System       │
└──────────┘ └──────────────┘
```

The receiver will act as the robot's main control node. The transmitter
will send movement and system commands wirelessly.

------------------------------------------------------------------------

## 6. Technical Approach

### Mechanical System

The mechanical design focuses on maintaining stable contact with a
surface while allowing the robot to move.

Key elements include:

-   Vacuum adhesion mechanism
-   Linear actuator/suspension mechanism
-   Motorized wheel modules
-   Stabilization system
-   Compact modular body
-   Cleaning assembly

### Smart Systems

The planned intelligent control system includes:

-   Sensor-based navigation
-   Obstacle detection
-   Autonomous motion control
-   Adhesion monitoring
-   Future AI-based debris/object recognition

### Electronics & Embedded Control

The system uses ESP32-based embedded control.

The ESP32 handles communication and control signals for the robot's:

-   Drive system
-   Vacuum system
-   Cleaning system
-   Sensors
-   Future autonomous functions

------------------------------------------------------------------------

## 7. Key Innovation

Vac-Robo is not simply a robotic vacuum cleaner.

Its main innovation is the combination of:

**Cleaning + Vacuum Adhesion + Multi-Surface Mobility + Intelligent
Control**

This allows the same robotic platform to target surfaces that
conventional floor-cleaning robots cannot easily reach.

------------------------------------------------------------------------

## 8. Feasibility

The concept is based on established technologies that can be integrated
into a single robotic platform.

The project research references work on:

-   Glass and façade-cleaning robots
-   Wall-climbing mechanisms
-   Vacuum-based adhesion
-   Adhesion-aware control
-   Coverage path planning
-   Multi-surface robotic mobility

The project presentation also identifies service robotics and
professional robotics as growing markets, supporting the potential for
robotic cleaning solutions beyond conventional floor cleaning.

------------------------------------------------------------------------

## 9. Applications

Vac-Robo can potentially be adapted for:

-   Residential walls and windows
-   Commercial buildings
-   Glass façades
-   Hotels
-   Hospitals
-   Shopping malls
-   Industrial cleaning
-   Elevated or difficult-to-access surfaces

------------------------------------------------------------------------

## 10. Future Development

After completing the transmitter/receiver system, development will focus
on progressively increasing autonomy:

### Phase 1 --- Wireless Control

-   ESP32 transmitter
-   ESP32 receiver
-   Wireless command transmission
-   Drive and vacuum control

### Phase 2 --- Sensor Integration

-   Distance/obstacle sensing
-   Adhesion monitoring
-   Surface detection

### Phase 3 --- Autonomous Navigation

-   Automatic movement
-   Obstacle avoidance
-   Surface coverage planning

### Phase 4 --- Intelligent Cleaning

-   AI-assisted debris recognition
-   Adaptive cleaning
-   Automated coverage optimization

### Phase 5 --- Full Autonomous Operation

The long-term goal is for Vac-Robo to receive a cleaning task and
perform the required movement and cleaning with minimal human
intervention.

------------------------------------------------------------------------

## 11. Impact

Vac-Robo aims to reduce the need for manual cleaning of
difficult-to-access surfaces.

Expected benefits include:

-   Improved cleaning safety
-   Reduced dependence on manual elevated cleaning
-   Reduced labour requirements for repetitive cleaning
-   Increased accessibility of robotic cleaning
-   A reusable platform for multi-surface cleaning applications

------------------------------------------------------------------------

## 12. Research Basis

The project research includes academic work on glass/façade-cleaning
robots, wall-climbing mechanisms, adhesion-aware control, dynamic
modelling, coverage path planning, and vacuum-suction adhesion.

Market research included service robotics and professional service
robotics forecasts.

Full citations, DOIs, and report links are maintained in the project
documentation.

------------------------------------------------------------------------

## 13. Team

### Team Vac

**Team ID:** 107

The team is developing Vac-Robo as an open-innovation robotics project
for MUJ HACKX 4.0.

------------------------------------------------------------------------

## 14. Project Status

**Mechanical System:** ✅ Built\
**Electronic System:** ✅ Built\
**Motor Control:** ✅ Working\
**Vacuum/Adhesion System:** ✅ Built\
**ESP32 Control:** ✅ Working\
**Wireless Transmitter:** 🔄 In Development\
**Wireless Receiver:** 🔄 In Development\
**Autonomous Navigation:** 🔜 Next Stage\
**Full Autonomous Cleaning:** 🔜 Future Stage

------------------------------------------------------------------------

## 15. Conclusion

Vac-Robo aims to take robotic cleaning from **"floor only" to
"multi-surface."**

The physical robot has already been developed. The current focus is on
completing the wireless transmitter/receiver control system and then
building progressively toward autonomous navigation and intelligent
cleaning.

**Vac-Robo --- One robot. Every surface.**
