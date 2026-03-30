# MES-MQTT-Simulation-Project
I built a mini MES pipeline where a simulated machine publishes operational data over MQTT, a consumer layer calculates downtime and OEE metrics, and a dashboard visualizes real-time manufacturing performance.


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
<img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/98117305-9adc-4968-a01e-753a22dd2255" />
<img width="1920" height="1080" alt="Screenshot (34)" src="https://github.com/user-attachments/assets/9ac157de-a2b7-4f4b-bf1e-7df3b9c84d6b" />
<img width="1920" height="1080" alt="Screenshot (35)" src="https://github.com/user-attachments/assets/41a810ff-9842-436a-a2dd-166e019b9193" />
