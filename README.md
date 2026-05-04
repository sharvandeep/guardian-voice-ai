RoadGuardian AI
Privacy-First Intelligent Road Accident Emergency Response System
🚨 About the Project

RoadGuardian AI is an AI-powered road safety and emergency response platform built for the IIT Madras Road Safety Hackathon 2026 (BIMSTEC Countries) under the RoadSoS Problem Statement.

In road accidents, victims often cannot unlock their phones, search for hospitals, call ambulances, or contact emergency services manually.

RoadGuardian AI solves this by using:

Voice-triggered emergency activation
Automatic crash detection
Smart accident severity analysis
Nearby emergency service discovery
Offline emergency fallback support

The system is designed to reduce response time during the Golden Hour — the most critical period immediately after a road accident.

🎯 Problem Statement

During road accidents:

Victims may be unconscious or injured
Phones may be locked
Internet may be unavailable
Immediate access to hospitals and ambulance services becomes difficult
Delay in emergency response can cost lives

Traditional emergency apps require manual interaction.

This is often impossible during real emergencies.

💡 Our Solution
RoadGuardian AI

A Privacy-First Voice + Crash Detection Emergency Rescue System

that automatically detects emergencies and provides:

Nearby trauma centre access
Ambulance support
Police station assistance
Vehicle towing / roadside rescue
Emergency contact alerts
Offline fallback support

without requiring manual phone usage.

🏆 Project Goal

To build a hands-free emergency rescue system that works even when users cannot interact with their device manually.

Main Objective
Reduce Emergency Response Time During the Golden Hour

This improves:

Faster medical attention
Faster ambulance dispatch
Better rescue coordination
Higher survival chances
🔥 Key Features
Core Emergency Features
🎙 Voice-Activated Emergency Trigger

Recognizes distress phrases like:

“Help me”
“Accident happened”
“Call ambulance”
“Police please”
“Emergency help”
🚗 Automatic Crash Detection

Detects accidents using:

Accelerometer spikes
Sudden speed drops
Device tilt abnormalities
Motion irregularities
GPS movement interruptions
📊 Smart Severity Detection

Classifies accidents into:

Minor
Moderate
Severe

This helps prioritize emergency response.

🏥 Nearby Trauma Centre Finder

Provides fast access to:

Hospitals
Trauma centres
Ambulance services

based on urgency and distance.

👮 Police Station Support

Quick access to:

Nearby police stations
Emergency law enforcement support

especially useful for highways and night accidents.

🔧 Vehicle Rescue Support

Supports:

Towing services
Roadside assistance
Breakdown rescue

A strong differentiator most teams miss.

📍 Emergency Contact Alerts

Automatically sends:

Live GPS location
Emergency type
Severity level
Help request message

through:

SMS
Emergency calls
Contact notifications
📶 Offline Fallback Mode

Works even without internet using:

SMS alerts
Cached nearby hospitals
Cached police stations
Emergency contact fallback

This is a major real-world advantage.

⚙ Core Concept

Traditional emergency apps work like this:

Unlock Phone → Open App → Search Help → Call Support

This wastes critical time.

RoadGuardian AI works like this:
Voice + Crash Detection → AI Analysis → Emergency Response

Fast. Automatic. Life-saving.

🏗 System Architecture
Mobile Device
        ↓
Continuous Low-Power Listening
        ↓
Wake Word Detection
        ↓
Voice Activity Detection
        ↓
Speech Recognition
        ↓
Crash Detection Engine
(Accelerometer + GPS + Motion Analysis)
        ↓
Severity Classification Engine
(Minor / Moderate / Severe)
        ↓
Intent Detection
        ↓
Emergency Decision Engine
        ↓
Location Intelligence Layer
        ↓
Nearby:
• Trauma Centres
• Ambulances
• Police Stations
• Vehicle Rescue Services
        ↓
Emergency Action Trigger
        ↓
Emergency Contacts + SOS Network
        ↓
Offline Backup Protocol
(SMS + Cached Emergency Data)
🧠 System Modules
1. Wake Word Detection

Continuously monitors audio for trigger phrases.

Example Triggers
Help me
Emergency help
Call ambulance
Requirements
Always-on listening
Low power usage
Fast response
Low false triggers
Privacy-first local processing
2. Voice Activity Detection (VAD)

Detects whether actual speech is present.

Purpose
Ignore background noise
Reduce unnecessary processing
Improve recognition accuracy
Save battery life
3. Offline Speech Recognition

Converts speech into text after trigger detection.

Tools Used
Vosk
Whisper
PocketSphinx

All processing happens locally on-device.

4. Crash Detection Engine

Detects physical accident signals.

Detection Signals
Impact force spikes
Sudden braking
Speed drops
Motion interruption
Device tilt changes

This makes the system stronger than voice-only solutions.

5. Severity Classification Engine

Classifies accident seriousness into:

Minor
Moderate
Severe
Severe Cases Trigger
Ambulance priority
Faster trauma centre selection
Emergency contact escalation
6. Intent Detection

Checks whether the spoken phrase is truly a distress request.

Example Distress Sentences
I am being attacked
Please help me
Call an ambulance

Implemented using:

Intent classifier
Small transformer model
Lightweight NLP model
On-device LLM
7. Location Intelligence Layer

Finds the nearest emergency support services.

Services Located
Trauma centres
Hospitals
Ambulances
Police stations
Towing services
Rescue providers

Priority is based on:

Distance
Arrival time
Severity level
8. Emergency Action System

Triggers immediate rescue actions.

Actions
Send SMS alerts
Share live GPS coordinates
Emergency phone calls
Loud alarm activation
Rescue notifications
Example Alert

Emergency alert from [User Name]
Possible road accident detected
Severity: Severe
Location: [GPS Coordinates]

9. Offline Backup Protocol

Used when internet is unavailable.

Offline Support Includes
SMS emergency alerts
Cached hospital database
Cached police station access
Emergency contact fallback
Minimal rescue workflow

Perfect for highways and rural areas.

💻 Technology Stack
AI / ML
Python
TensorFlow Lite
PyTorch
ONNX Runtime
Speech Processing
Vosk
Whisper
MFCC Audio Processing
Voice Activity Detection
Mobile Application
Android (Kotlin / Java)
Backend
Python FastAPI
SQLite / PostgreSQL
Maps + Location Services
Google Maps API

OR

OpenStreetMap APIs
Tools
GitHub
Docker
Edge AI Libraries
🌍 Final Vision

RoadGuardian AI is not just another emergency app.

It is an AI-powered:

Golden Hour Rescue Infrastructure

built to save lives by reducing the time between:

Accident Occurrence → Emergency Response
Mission
Faster Detection
Faster Rescue
Better Survival
