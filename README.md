# Alejandro Sousa

**Embedded Systems · Firmware · Electronics · HW/FW Integration · Testing & Validation**

Mechatronics engineering graduate based in Mexico, with a technical background in electronics. Engineering studies completed at Instituto Tecnológico Superior de Comalcalco; degree conferral in progress.

## About me

I work close to hardware: understanding the problem, choosing an architecture, integrating electronics and firmware, debugging unexpected behavior, and documenting what the system actually does.

My projects span wireless monitoring, embedded firmware, custom PCB design, motor-control hardware and PLC automation. My work has progressed from integrating commercial modules into a functional system to designing power and interface circuits at component level.

I am seeking an early-career role in embedded systems, electronics, hardware–firmware integration or test and validation. I am interested in applying this foundation to industrial, automotive and aerospace engineering teams while developing deeper technical skills.

## Selected engineering work

### Autonomous IoT Monitoring

A wireless proximity-monitoring and local-alert system developed in response to a technical request from the DTI department of Hospital General Dr. Desiderio G. Rosado Carbajal in Comalcalco, Mexico.

**My contribution:** project coordination, C++ firmware for ESP32-C6 nodes, electronics integration, functional testing and technical documentation within the project team. After delivery, I continued the receiver redesign independently.

**Key decisions:** the wearable communicates independently with the area and exit receivers through ESP-NOW. Each receiver evaluates received signal strength (RSSI) locally, using an exponential moving average (EMA) and hysteresis to balance stability against response delay. Local alarms do not depend on cloud telemetry. RSSI supports proximity decisions rather than exact distance measurement.

**V1 outcome:** built, evaluated and delivered to the hospital by the team. Historical aggregate test results and their limitations are documented in the repository; raw trial datasets are not published.

**REV 2.0 status:** custom two-layer receiver PCB and enclosure CAD developed around a removable XIAO ESP32-S3 and external PN532 reader. Fabrication, firmware porting and physical validation remain pending; component matching still requires closure before assembly.

<p align="center">
  <img src="https://raw.githubusercontent.com/alx-sousa/Autonomous-IoT-Monitoring/main/docs/images/rev2/rev2-final-enclosure-cad.png" width="520" alt="REV 2.0 receiver enclosure CAD; physical fabrication pending">
</p>

*REV 2.0 enclosure CAD — design-stage view.*

[Full project](https://github.com/alx-sousa/Autonomous-IoT-Monitoring) · [V1 evaluation](https://github.com/alx-sousa/Autonomous-IoT-Monitoring/blob/main/docs/testing.md) · [Validation status](https://github.com/alx-sousa/Autonomous-IoT-Monitoring/blob/main/docs/validation.md)

The project repository includes block-level firmware documentation and sanitized historical V1 source snapshots for technical review; deployment-specific configuration remains private.

### DC Motor Controller with Encoder — REV A

A personal hardware project for a 12 V geared DC motor with an incremental Hall encoder. I developed it to practice designing the power and motor-drive stages from individual components.

**My contribution:** component selection, schematic capture, two-layer PCB layout in EasyEDA Pro, design-rule checks and mechanical integration review in Fusion 360.

**Key decisions:** protected 12 V input, TPS54302 buck conversion, DRV8871 motor drive, an intended 3.3 V encoder interface and a removable ESP32-C6 Super Mini. The layout separates functional blocks and includes ground pours, stitching vias and exposed-pad thermal vias.

**Current result:** schematic and routing completed, design-rule checks (DRC) reported as passed, and 3D integration reviewed. These are design-stage checks; prototype fabrication, electrical bring-up, motor/encoder measurements and closed-loop firmware remain pending.

The exact encoder's electrical compatibility and the controller module's power-path behavior remain verification items before system operation.

<p align="center">
  <img src="https://raw.githubusercontent.com/alx-sousa/DC-Motor-Controller-Encoder/main/docs/images/rev-a/pcb-3d-perspective.png" width="520" alt="REV A motor-controller PCB render; fabrication and electrical testing pending">
</p>

*REV A PCB render — design-stage view.*

[Full project](https://github.com/alx-sousa/DC-Motor-Controller-Encoder) · [Design decisions](https://github.com/alx-sousa/DC-Motor-Controller-Encoder/blob/main/docs/design-decisions.md) · [Planned bring-up](https://github.com/alx-sousa/DC-Motor-Controller-Encoder/blob/main/docs/bring-up-plan.md)

[PCB Hardware Portfolio](https://github.com/alx-sousa/PCB-Hardware-Portfolio) provides a compact visual index of these board designs.

## Engineering toolkit

| Area | Project experience and tools |
|---|---|
| Embedded firmware | C/C++, Arduino framework, ESP32-C6, ESP32-S3, non-blocking and state-based logic |
| Interfaces and connectivity | GPIO, UART, I²C, SPI, ESP-NOW, Wi-Fi, BLE and RFID integration; depth varies by project |
| Electronics and PCB | EasyEDA Pro, schematic capture, two-layer layout, component selection, DRC, power routing, grounding and thermal considerations |
| Hardware–firmware integration | Sensors, displays, local alarms, LiPo-powered nodes and peripheral interfaces |
| Testing and documentation | Functional evaluation, debugging, test-result interpretation and planned board bring-up procedures |
| Automation and control | Siemens S7-1200/S7-300, TIA Portal, STEP 7, Ladder, PID Compact, Factory I/O, instrumentation and pneumatics |
| Mechanical integration | Fusion 360 and SolidWorks for enclosure and assembly design |
| Development tools | Git, GitHub, Arduino IDE, VS Code and Cursor; basic Python and MATLAB |

## Earlier engineering projects

Academic and personal work also includes PLC-based tank-level control, PI/PID ball-position control, conveyor and pneumatic sequencing, stepper positioning, a servo-driven robotic arm, and mobile robots for maze navigation, line following and mini sumo.

These projects established my foundation in sensors, actuators, feedback control and system integration. They are summarized here as earlier work; detailed public case studies are not yet available.

## Current engineering direction

My planned progression is toward protected 24 V digital I/O, industrial remote I/O and communications, followed by CAN (Controller Area Network) nodes and automated hardware testing.

Longer-term learning goals include Python-based test tooling, Linux/SocketCAN and hardware-in-the-loop (HIL) test benches. These are future development areas, not completed projects or established competencies.
