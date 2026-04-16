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

---

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

---

## Result 

### 1)Hosts with 0% packet loss.
<img width="757" height="540" alt="ss1" src="https://github.com/user-attachments/assets/3a004b58-1dde-4190-8cf0-7f6dad075df9" />

### 2)Flow Table Before Traffic Generation 
<img width="1098" height="161" alt="ss2" src="https://github.com/user-attachments/assets/7c38fafd-484b-4f6e-bb5f-2c0a13bf3b02" />

### 3)Flow Table After Traffic Generation
<img width="1451" height="372" alt="ss3" src="https://github.com/user-attachments/assets/9fcccc41-8946-43df-a9e5-2a530ad14dfc" />

### 4)Ryu Controller Packet-In Logs
<img width="1022" height="503" alt="ss4" src="https://github.com/user-attachments/assets/7277632c-6917-46f6-982a-c9801cefee8a" />

### 5)Flow Table Analyzer Output (Active vs Unused Rules)
<img width="1223" height="821" alt="ss5" src="https://github.com/user-attachments/assets/5231114b-1feb-4324-9ce8-a7d2d083cd1e" />

----

