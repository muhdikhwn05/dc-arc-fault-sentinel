# Dual-Domain (RF & Ultrasonic) Series DC Arc-Fault Sentinel ⚡

**Status:** Phase 1 (Proposal Submitted, Awaiting Grant)  
**Competition:** Global Sustainability Challenge (GSC) 2026-2027  
**Team:** OneSim  

## 📌 Project Overview
This project introduces a high-immunity fire prevention system for solar PV and battery storage. By cross-referencing radio frequency (RF) transients with ultrasonic acoustic emissions, this sentinel drastically reduces false positive arc-fault detections compared to traditional single-domain systems.

## 🛠️ Hardware Design

### System Schematic
*The analog front-end integrates a high-frequency current transformer and an ultrasonic transducer, feeding filtered signals into a Raspberry Pi Pico W.*

![Schematic Design](<img width="1072" height="732" alt="image" src="https://github.com/user-attachments/assets/34e58bf8-ff9b-44b2-9a66-bb6094cbd462" />
)

### PCB Layout
*Custom 2-layer PCB designed in KiCad, featuring bottom-layer ground copper pours for analog noise reduction.*

![PCB Layout](<img width="1543" height="757" alt="image" src="https://github.com/user-attachments/assets/c18ff75d-4414-4ecc-902c-34d89e2d2341" />)

![3D Render](<img width="882" height="436" alt="image" src="https://github.com/user-attachments/assets/331ae799-b342-4ee1-b606-c9efe6d8a02d" />
)


## 📂 Repository Structure
* `/Hardware` - KiCad project files, schematics, and custom component footprints.
* `/Firmware` - C/C++ source code for the Raspberry Pi Pico W.
* `/Docs` - GSC project proposal, block diagrams, and component datasheets.

## 🚀 Development Roadmap
- **Phase 1 (Current):** System architecture, KiCad schematic drafting, and GSC proposal submission.
- **Phase 2 (Pending Approval):** PCB fabrication, manual component soldering, and bench-testing the op-amp analog front-end.
- **Phase 3:** Pico W firmware development and dual-sensor polling integration.
