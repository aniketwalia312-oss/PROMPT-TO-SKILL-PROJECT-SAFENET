                                     # PROMPT-TO-SKILL-PROJECT-SAFENET

<div align="center">

# 🛡️ SAFENET
### AI-Powered Personal Safety, Emergency Detection & Autonomous Response Network

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688.svg?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/Frontend-React%2018-61DAFB.svg?logo=react&logoColor=black)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/UI-Tailwind%20CSS%203.4-38B2AC.svg?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Web Audio API](https://img.shields.io/badge/Acoustic-Web%20Audio%20API-FF6F00.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Gemini 2.5](https://img.shields.io/badge/AI%20Vision-Gemini%202.5%20Flash-4285F4.svg?logo=google&logoColor=white)](https://ai.google.dev/)

> **“When you can't react, your safety network can.”**

[Live Demo](https://safenet123.netlify.app/) • [Architecture](#-system-architecture) • [Features](#-core-capabilities) • [Quick Start](#-quick-start) • [API Specs](#-api-specifications)

</div>

---

## 📌 The Problem vs. The SAFENET Solution

| Challenge with Existing Apps | The SAFENET AI Solution |
| :--- | :--- |
| **Manual Panic Requirement**: Attacker prevents user from opening app. | **Zero-Touch Multi-Modal Triggers**: Acoustic scream NLP, custom voice codewords, dead-man timers, and motion impact sensors. |
| **Context-Blind SOS**: Sends just a bare GPS pin via SMS. | **Situational Incident Briefing**: Real-time synthesized dossier (vehicle plate, audio transcript, route deviation context, battery). |
| **Fastest Route vs. Safest Route**: Maps route pedestrians through unlit, isolated alleys. | **Predictive SafeRoute Engine**: Ranks routes by luminescence, crowd density, CCTV presence, and 24/7 safe havens. |
| **Unverified Strangers & Cabs**: Passengers enter unauthorized vehicles without records. | **Gemini Multimodal OCR**: Scans license plates and driver badges, logging encrypted snapshots to the cloud vault. |
| **Coercion Vulnerability**: Attacker forces victim to cancel SOS. | **Dual-PIN Protocol**: Master PIN (`1234`) disarms; Duress PIN (`9999`) covertly escalates to Level-3 Police Dispatch. |

---

## 🧠 System Architecture
                                  +-------------------------------------------------------------+
                                  |                           SAFENET                           |
                                  |   AI-Powered Personal Safety & Autonomous Response Network  |
                                  +-------------------------------------------------------------+
                                                                 |
                     +-------------------------------------------+-------------------------------------------+
                     |                                           |                                           |
     +-------------------------------+           +-------------------------------+           +-------------------------------+
     |     MULTIMODAL PERCEPTION     |           |     CONTEXT FUSION ENGINE     |           |    SAFETY POLICY ENGINE       |
     +-------------------------------+           +-------------------------------+           +-------------------------------+
     | - Realtime Speech (WebRTC/WS) |           | - Geo-telemetry & Deviations  |           | - Deterministic Rule Matrix   |
     | - Video & Image OCR (Gemini)  |           | - Historical Risk Zones       |           | - Anti-Hallucination Guard    |
     | - Acoustic Decibel Screams    |           | - Dead-Man Interval Watchdog  |           | - Action Idempotency Keys     |
     | - Inertial Drop/Impact Sensor |           | - Dynamic Threat Assessment   |           | - Duress vs Master PIN Auth   |
     +-------------------------------+           +-------------------------------+           +-------------------------------+
                                                                 |
                                         +-----------------------+-----------------------+
                                         |                                               |
                         +-------------------------------+               +-------------------------------+
                         |    EMERGENCY ORCHESTRATOR     |               |    REALTIME DISPATCH MESH     |
                         +-------------------------------+               +-------------------------------+
                         | - State Machine Manager       |               | - Twilio Voice / SMS Dispatch |
                         | - Live Expiring Session Gen   |               | - Live WebRTC / WS Audio Chat |
                         | - Chronological Audit Log     |               | - Firebase Cloud Push Alerts  |
                         | - Safe Haven Routing Engine   |               | - Trusted Circle Live Room    |
                         +-------------------------------+               +-------------------------------+

                         
---

## ⚡ Core Capabilities

### 1. 🎙️ Acoustic Distress & Scream Detection
- Listens continuously in a localized, circular RAM audio buffer using the **Web Audio API**.
- Monitors real-time ambient decibels ($\text{dB}$) and audio frequency spikes.
- Automatically triggers Level-2/3 emergency alerts if sudden distress screams or impact sounds ($>85\text{ dB}$) are detected.

### 2. 📸 Gemini Multimodal OCR Vehicle & Stranger Scanner
- Real-time camera capture for vehicle license plates, delivery agent badges, and driver IDs.
- Extracts registration text, validates against expected booking details, flags unregistered vehicles, and logs encrypted evidence to the Cloud Vault.

### 3. 🗺️ Predictive SafeRoute & Tactical Radar Map
- Calculates a dynamic **SafeScore ($0\text{–}100$)** considering street lighting, pedestrian crowd density, open 24/7 businesses, and community crime heatmaps.
- Identifies and routes toward the nearest verified **Safe Havens** (Police Kiosks, 24/7 Hospitals, Transit Hubs).

### 4. 🗣️ Realtime Conversational AI Voice Guardian
- Hands-free, low-latency conversational assistant powered by Web Speech Synthesis & Recognition.
- Gives calm, actionable instructions without encouraging physical confrontation.

### 5. 📞 Interactive Decoy Fake Incoming Call
- Realistic phone call simulation with real audio ringtones and dynamic conversational AI dialogue to provide an exit strategy from uncomfortable or threatening encounters.

### 6. 🔒 Anti-Coercion Dual-PIN Protocol
- **Master PIN (`1234`)**: Disarms the emergency protocol and resumes passive monitoring.
- **Duress PIN (`9999`)**: Simulates a standard UI dismissal to deceive an attacker while secretly dispatching a silent Level-3 alert with live audio and GPS telemetry.

### 7. 🧪 5-Scenario Interactive Simulation Controller
- 1-Click live testing suite for judges and reviewers to simulate:
  1. *Route Corridor Deviation*
  2. *Unanswered Dead-Man Check-in*
  3. *Silent Duress PIN Coercion*
  4. *Explicit Hold-to-SOS Trigger*
  5. *Multi-Factor Acoustic Scream in High-Risk Zone*

---

## 🛠️ Technology Stack

- **Frontend**: React 18, Tailwind CSS, Lucide Icons, Leaflet Maps, Web Audio API, Web Speech API, Canvas Confetti.
- **Backend API**: Python 3.11, FastAPI, SQLAlchemy, Pydantic v2, Uvicorn, WebSockets.
- **AI & Vision**: Google Gemini 2.5 Flash Multimodal Vision API, OpenAI Realtime API.
- **Telephony & Push**: Twilio Programmable Voice & SMS, Firebase Cloud Messaging (FCM).
- **Database & Cache**: PostgreSQL with PostGIS, Redis Pub/Sub.

---

## 🚀 Quick Start Guide

### Option 1: Standalone Single-File Launch (Zero-Dependency)
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/safenet-ai.git
   cd safenet-ai

   cd backend
python -m venv venv

# Windows
.\venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
cp .env.example .env

# Run FastAPI Server
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload

PORT=8000
DATABASE_URL=sqlite+aiosqlite:///./safenet.db
SECRET_KEY=your_super_secret_jwt_key_2026

# AI & Maps
OPENAI_API_KEY=your_openai_key
GOOGLE_MAPS_API_KEY=your_google_maps_key

# Telephony (Twilio - Sandbox enabled by default)
TWILIO_ACCOUNT_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE_NUMBER=+15005550006
ENABLE_SANDBOX_TELEPHONY=True
