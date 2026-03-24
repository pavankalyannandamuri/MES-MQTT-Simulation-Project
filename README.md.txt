# MES MQTT Simulation Project

## Overview
This project simulates a Manufacturing Execution System (MES) pipeline using MQTT and Node-RED.

## Architecture
Machine Simulator → MQTT (Mosquitto) → MES Logic → Dashboard

## Features
- Machine simulation (state, count, temperature)
- MQTT publish/subscribe communication
- Real-time OEE calculation
- Dashboard visualization

## Technologies Used
- Node-RED
- Mosquitto (MQTT broker)
- JavaScript (function nodes)

## MQTT Topics
plant1/line1/machine01/state  
plant1/line1/machine01/count  
plant1/line1/machine01/temp  

## OEE Calculation
- Availability = Runtime / (Runtime + Downtime)
- Performance = Actual Rate / Ideal Rate
- Quality = Good / Total
- OEE = A × P × Q

## How to Run
1. Start Mosquitto
2. Run Node-RED
3. Import flows.json
4. Deploy
5. Open dashboard

## Learning Outcome
- MQTT event-driven architecture
- MES data modeling
- Real-time analytics