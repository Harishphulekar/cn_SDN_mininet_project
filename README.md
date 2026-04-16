# Multi-Switch Flow Table Analyzer (SDN Project)

## Problem Statement
Analyze flow tables in SDN switches and display rule usage by identifying ACTIVE and UNUSED flow rules dynamically.



## Objective
This project demonstrates:
- Controller–switch interaction using SDN
- Flow rule monitoring and analysis
- Identification of ACTIVE vs UNUSED flow entries
- Dynamic updates of flow statistics



## Technologies Used
- Mininet (Network Emulator)
- Ryu Controller (SDN Controller)
- OpenFlow Protocol (v1.3)
- Python



## System Architecture
Mininet (Hosts + Switches) → OpenFlow Switch → Ryu Controller → Flow Analyzer Module → Output



## Setup Instructions

### 1. Install Mininet
    sudo apt update
    sudo apt install mininet -y
