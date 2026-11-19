# Dual-Modal (RF & Ultrasonic) DC Arc-Fault Prevention System with IoT Diagnostics ⚡

**Status:** Phase 1 (Proposal Submitted, Awaiting Grant)  
**Competition:** Global Sustainability Challenge (GSC) 2026-2027  
**Team:** OneSim (Ikhwan(leader), Fadhli, Khairul Alif, Akif, Umar)

## 📌 Project Overview
This project introduces a high-immunity fire prevention system engineered for commercial rooftop PV installations (≤1000 V DC) and battery storage. By cross-referencing radio frequency (RF) transients with ultrasonic acoustic emissions, this sentinel drastically reduces false positive arc-fault detections caused by inverter switching noise. 

An integrated **Raspberry Pi Pico W** provides real-time **IoT web telemetry**. It utilizes an asymmetric dual-core architecture: Core 0 handles safety-critical 5 kHz sampling and trip logic (<5 ms response time), while Core 1 hosts an IoT HTTP server to broadcast diagnostic data and trigger remote alerts to a web dashboard.

## 🗺️ System Architecture (Macro & Micro View)
*The macro view demonstrates integration at the PV combiner box, while the micro view details the custom PCB connections including the SCT-013 clamp and TCT40-16R ultrasonic receiver.*

![System Architecture Diagram](https://github.com/user-attachments/assets/28eb077f-e75d-4dfe-8e3b-76a3b07b4801)
## 🛠️ Hardware Design

### System Schematic
*The analog front-end integrates a high-frequency current transformer and an ultrasonic transducer, feeding filtered signals into a Raspberry Pi Pico W.*

![Schematic Design](https://github.com/user-attachments/assets/34e58bf8-ff9b-44b2-9a66-bb6094cbd462)


### PCB Layout
*Custom 2-layer PCB designed in KiCad, featuring bottom-layer ground copper pours for analog noise reduction.*

![PCB Layout](https://github.com/user-attachments/assets/c18ff75d-4414-4ecc-902c-34d89e2d2341)

![3D Render](https://github.com/user-attachments/assets/23c5da36-6c99-4939-9fa2-7eb2c159f4b4)


## 📂 Repository Structure
* `/Hardware` - KiCad project files, schematics, and custom component footprints.
* `/Firmware` - C/C++ source code for the Raspberry Pi Pico W.
* `/Docs` - GSC project proposal, block diagrams, and component datasheets.

## 🚀 Development Roadmap
- **Phase 1 (Current):** System architecture, KiCad schematic drafting, and GSC proposal submission.
- **Phase 2 (Pending Approval):** PCB fabrication, manual component soldering, and bench-testing the op-amp analog front-end.
- **Phase 3:** Pico W firmware development and dual-sensor polling integration.
