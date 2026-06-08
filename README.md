# IoT-Based Smart Lock System

A complete IoT smart lock system with cloud-based authentication 
and a React Native mobile app for secure remote control.

## Features
- Remote lock/unlock control via mobile app
- Three-factor authentication: username/password + device ID + admin approval gate
- Real-time access logging — captures user identity, timestamp, and action on every lock event
- Admin authorization workflow — new users remain inactive until admin explicitly approves access
- Full auditable trail available on admin dashboard

## Hardware Used
- ESP8266 NodeMCU
- Solenoid lock / servo motor

## Tech Stack
- Embedded C (Arduino framework)
- React Native (mobile app)
- Hostinger (cloud backend)
- REST API

## How It Works
1. User sends lock/unlock command from the React Native app
2. App authenticates using username, password, and registered device ID
3. Request only processed if admin has approved the user account
4. Lock state changes and the event is logged to the cloud in real time
5. Admin can view full access history from the dashboard
