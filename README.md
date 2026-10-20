# Alejandro Sousa

**Embedded Systems · Firmware · Electronics · HW/FW Integration · Testing & Validation**

Mechatronics engineering graduate based in Mexico, with a technical background in electronics. Engineering studies completed at Instituto Tecnológico Superior de Comalcalco; degree conferral in progress.

## About me

I work close to hardware: understanding the problem, choosing an architecture, integrating electronics and firmware, debugging unexpected behavior, and documenting what the system actually does.

My projects span wireless monitoring, embedded firmware, custom PCB design, power management, hardware–firmware integration and PLC automation. My work has progressed from integrating commercial modules into functional systems to designing compact product-oriented electronics at component level.

I am seeking an early-career role in embedded systems, electronics, hardware–firmware integration or test and validation. I am interested in applying this foundation to industrial, automotive and aerospace engineering teams while developing deeper technical skills.

## Selected engineering work

### P1 Rev B — Commercial Refrigeration Monitor

A product-oriented **retrofit condition-monitoring platform for commercial refrigeration**, developed from a real pilot need in a butcher-shop refrigeration environment. The system is intended to observe temperature, door state, power/battery condition and local events without taking control of the refrigerator or compressor.

**My contribution:** system architecture, component selection, schematic capture, four-layer PCB design in EasyEDA Pro, power/sensing/interface integration, preliminary mechanical integration in Fusion, engineering calculations and a structured pre-fabrication validation plan.

**Key decisions:** ESP32-C6 embedded core; single external USB-C for power, charging and native programming/service; BQ25186 LiPo charger/power path; TPS63802 buck-boost logic rail; external DS18B20 probe; low-power Hall sensing; RTC-backed timestamps; switched loads; 1.69-inch IPS display; local buzzer; dedicated L2 ground plane and L3 power distribution.

**Current status:** Rev B hardware architecture, schematic and four-layer PCB have reached the current pre-fabrication design milestone. Gerber/manufacturing review, first build, electrical bring-up, firmware, dedicated monitoring software, final enclosure and field validation remain next milestones.

<p align="center">
  <img src="https://raw.githubusercontent.com/alx-sousa/P1-Refrigeration-Monitor/main/docs/images/p1_revB_fusion_hero_iso.png" width="560" alt="P1 Rev B commercial refrigeration monitor conceptual PCB and display integration">
</p>

*Rev B conceptual PCB + display integration — design-stage view, fabrication pending.*

[Full project](https://github.com/alx-sousa/P1-Refrigeration-Monitor) · [Architecture](https://github.com/alx-sousa/P1-Refrigeration-Monitor/blob/main/docs/architecture.md) · [Validation plan](https://github.com/alx-sousa/P1-Refrigeration-Monitor/blob/main/docs/validation-plan.md)

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

### Additional hardware work

The [PCB Hardware Portfolio](https://github.com/alx-sousa/PCB-Hardware-Portfolio) contains a compact visual index of additional board designs, including the **DC Motor Controller with Encoder — REV A**. That project remains useful evidence of power-stage and motor-drive PCB work, but P1 Rev B is now the stronger representation of my current hardware-design level.

## Engineering toolkit

| Area | Project experience and tools |
|---|---|
| Embedded firmware | C/C++, Arduino framework, ESP32-C6, ESP32-S3, non-blocking and state-based logic |
| Interfaces and connectivity | GPIO, UART, I²C, SPI, ESP-NOW, Wi-Fi, BLE and RFID integration; depth varies by project |
| Electronics and PCB | EasyEDA Pro, schematic capture, two- and four-layer PCB layout, component selection, DRC, grounding, power management and interface protection |
| Hardware–firmware integration | Sensors, displays, local alarms, LiPo-powered nodes, USB service/programming and peripheral interfaces |
| Testing and documentation | Functional evaluation, debugging, test-result interpretation, validation planning and structured board bring-up procedures |
| Automation and control | Siemens S7-1200/S7-300, TIA Portal, STEP 7, Ladder, PID Compact, Factory I/O, instrumentation and pneumatics |
| Mechanical integration | Fusion 360 and SolidWorks for enclosure and assembly design |
| Development tools | Git, GitHub, Arduino IDE, VS Code and Cursor; basic Python and MATLAB |

## Earlier engineering projects

Academic and personal work also includes PLC-based tank-level control, PI/PID ball-position control, conveyor and pneumatic sequencing, stepper positioning, a servo-driven robotic arm, and mobile robots for maze navigation, line following and mini sumo.

These projects established my foundation in sensors, actuators, feedback control and system integration. They are summarized here as earlier work; detailed public case studies are not yet available.

## Current engineering direction

My planned progression is toward protected 24 V digital I/O, industrial remote I/O and communications, followed by CAN (Controller Area Network) nodes and automated hardware testing.

Longer-term learning goals include Python-based test tooling, Linux/SocketCAN and hardware-in-the-loop (HIL) test benches. These are future development areas, not completed projects or established competencies.
