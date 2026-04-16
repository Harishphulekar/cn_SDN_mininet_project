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
### 2. Create Virtual Environment (Python 3.8 recommended)
    python3.8 -m venv ryu-env38
    source ryu-env38/bin/activate
### 3. Install Dependencies
    pip install "pip<23"
    pip install "setuptools<58"
    pip install wheel
    pip install eventlet==0.30.2
    pip install ryu
    
---

## How To Run

### 1. Run Ryu Controller
    ryu-manager flow_analyzer.py
### 2. Start Mininet
    sudo mn --topo single,3 --controller remote
### 3. Generate Traffic
    pingall


## Result 
