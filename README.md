# Guardian Voice AI

Privacy-First Voice-Activated Distress Alert System

A safety-focused AI system that allows users to trigger emergency alerts through voice commands even when their phone is locked or offline. The system processes voice locally on the device to maintain privacy and reduce response time.

---

## Project Goal

The goal of Guardian Voice AI is to provide a **hands-free emergency alert mechanism** that works in critical situations when users cannot unlock their device or interact with it manually.

The system continuously listens for predefined distress phrases and automatically sends alerts to emergency contacts.

Key objectives:

• Reduce the time required to notify emergency contacts  
• Work without internet connectivity  
• Preserve user privacy through on-device AI processing  
• Provide a voice-first emergency interface  

---

## Key Features

- Voice activated emergency alerts
- Works when device is locked
- Works offline
- On-device AI processing (no cloud)
- Automatic SMS / emergency call trigger
- Location sharing with contacts
- Privacy-first architecture

---

## Core Concept

Traditional emergency apps require the user to unlock their device and manually trigger help.

Guardian Voice AI solves this problem by enabling:

Voice → AI detection → Emergency alert

The system continuously listens for a **distress phrase** such as:

"Help me"  
"I am in danger"  
"Call the police"

When detected with high confidence, the system automatically sends alerts.

---

## System Architecture

The system follows a multi-stage AI pipeline.

Microphone  
↓  
Wake Word Detection  
↓  
Voice Activity Detection  
↓  
Speech Recognition  
↓  
Intent Detection  
↓  
Emergency Action Trigger

---

## 1. Wake Word Detection

The first stage continuously monitors incoming audio for a trigger phrase.

Example phrases:

"Help me"  
"Emergency help"

This is done using **keyword spotting models**.

Keyword spotting is a speech processing technique used to detect specific words or phrases from continuous audio streams and trigger actions in voice systems. :contentReference[oaicite:2]{index=2}

Requirements:

• Always-on listening  
• Low power consumption  
• Very fast response time  
• Low false triggers  

---

## 2. Voice Activity Detection

This stage determines if speech is actually present in the audio stream.

Purpose:

• Ignore background noise  
• Reduce processing load  
• Improve accuracy

---

## 3. Speech Recognition (Offline)

Once the wake phrase is detected, the system converts the speech into text.

Possible tools:

Vosk  
Whisper Tiny  
PocketSphinx  

All processing runs locally on the device.

---

## 4. Intent Detection

The system analyzes the spoken phrase to determine if the user is in distress.

Example phrases classified as distress:

"I am being attacked"  
"Please help me"  
"Call an ambulance"

This can be implemented using:

Small transformer model  
Intent classifier  
On-device LLM

---

## 5. Emergency Action System

If the distress intent is confirmed, the system triggers emergency actions.

Possible actions:

Send SMS to emergency contacts  
Share location coordinates  
Trigger loud alarm  
Call emergency number

Example alert message:

"Emergency alert from [User Name]. Possible distress detected. Location: [GPS coordinates]"

---

## Technology Stack

AI / ML

Python  
TensorFlow Lite  
PyTorch  
ONNX  

Speech Processing

Vosk  
Whisper  
MFCC audio processing  

Mobile Application

Android (Kotlin / Java)

Tools

GitHub  
Docker  
Edge AI libraries  

---

## Repository Structure
