<div align="center">

# 🌾 KisanKonnect — किसान कनेक्ट

**Voice-First AI Platform for India's Smallholder Farmers**

*किसान की आवाज़, AI की ताकत — The farmer's voice, powered by AI*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-3.0-brightgreen.svg)](https://github.com/asthamosmi-arch/KisanKonnect)
[![Status](https://img.shields.io/badge/Status-Active%20Development-blue.svg)](https://github.com/asthamosmi-arch/KisanKonnect)
[![Hackathon](https://img.shields.io/badge/Moonshot%20Awards-2026-gold.svg)](https://moonshot.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen.svg)](CONTRIBUTING.md)

[🌐 Live Demo](#) · [📖 Docs](#documentation) · [🗺️ Roadmap](#roadmap) · [🤝 Contribute](#contributing)

</div>

---

## 📋 Table of Contents

- [Overview](#overview)
- [The Problem](#the-problem)
- [Our Solution](#our-solution)
- [Current Status](#current-implementation-status)
- [Features](#features)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [AI Modules](#ai-modules)
- [Roadmap](#roadmap)
- [Responsible AI](#responsible-ai)
- [Contributing](#contributing)
- [About the Developer](#about-the-developer)
- [License](#license)

---

## Overview

KisanKonnect is an **open-source, AI-powered digital companion** for India's smallholder farmers. It helps farmers make better agricultural decisions through **multilingual voice interaction**, practical crop guidance, and offline-friendly technology.

The platform addresses a critical gap: while India has 600 million farmers, most agricultural knowledge and government information is only available in English and requires digital literacy that most rural farmers do not have.

> **KisanKonnect's vision:** Make agricultural knowledge as accessible as a phone call — in the farmer's own language, on any device, even on 2G connectivity.

---

## The Problem

India's farmers face a compounding information crisis:

| Problem | Scale | Impact |
|---------|-------|--------|
| Language barrier | 82% of farmers cannot access English-language resources | Late crop disease detection, wrong treatment |
| Information asymmetry | Real-time Mandi prices unavailable to most farmers | Selling 30–40% below fair market rate |
| Scheme awareness gap | Complex application processes in bureaucratic language | ₹1.5 lakh crore in govt schemes unclaimed annually |
| Weather alert delays | Rural areas receive alerts hours after urban areas | Crop losses from unprepared weather events |
| Digital literacy barrier | Most agricultural apps require reading and typing | Excludes the farmers who need help most |

These are not isolated problems — they compound each other and systematically disadvantage the people who grow food for 1.4 billion Indians.

---

## Our Solution

KisanKonnect is built on a single core insight: **if a farmer cannot read, give them a tool that does not require reading.**

### Design Principles

- **Voice-first** — primary interface is a microphone button, not a text field
- **Language-native** — Hindi, Bhojpuri, Maithili with real speech recognition
- **Offline-capable** — critical features cached for 2G/3G environments
- **Honest about AI** — confidence indicators, disclaimers, human oversight guidance
- **Open source** — anyone can contribute, extend, or deploy

### Four Core Modules

| Module | What it does | Status |
|--------|-------------|--------|
| 🌿 **Crop Disease Diagnosis** | Voice/text query → AI identifies disease + treatment in Hindi | ✅ Implemented (Claude AI) |
| 📊 **Mandi Price Intelligence** | Real-time market prices with buy/sell advisory | 🔧 Prototype (sample data) |
| 🌦 **Weather + Crop Calendar** | Hyperlocal forecasts + crop-stage irrigation advice | 🔧 Prototype (sample data) |
| 🏛 **Government Scheme Advisor** | Eligibility matching + step-by-step guidance | ✅ Implemented (static data) |

---

## Current Implementation Status

> **We believe in radical transparency about what is built vs. what is planned.**

### ✅ Implemented and Working

- **Real voice recognition** — Web Speech API in Hindi, Bhojpuri, Maithili, English
- **Real AI advisory** — Claude AI (Anthropic) for crop disease diagnosis and guidance
- **Hindi Text-to-Speech** — SpeechSynthesis API speaks AI responses aloud
- **Community Voice Feed** — Farmers can post voice queries and receive AI analysis
- **Government Schemes** — PM-KISAN, PMFBY, KCC, Soil Health Card with static data
- **Farm Diary** — Local storage diary for tracking farming activities
- **Dark/Light mode** — Full theme switching
- **Accessibility** — ARIA labels, skip links, keyboard navigation
- **Offline-first UI** — App shell works without internet

### 🔧 Prototype (Demo Data)

- **Mandi Prices** — Sample data shown. AGMARKNET API integration is a future milestone.
- **Weather** — Sample weather data shown. IMD/OpenWeatherMap integration is planned.
- **ISRO Satellite Panel** — Illustrative NDVI/soil moisture values. Real satellite data integration is a future milestone.

### 🗺️ Future Roadmap

See the [Roadmap](#roadmap) section for planned features.

---

## Features

### 🎙️ Voice-First Interaction
Record crop problems by voice in your local language. KisanAI listens, understands, and responds — all in Hindi. No typing, no reading required.

### 🤖 KisanAI Crop Advisory (Real AI)
Powered by Claude AI (Anthropic). Ask any farming question and receive:
- Disease/pest identification with confidence percentage
- Specific treatment with product names, doses, and timing
- Prevention advice
- Satellite indicator context (illustrative)
- Always includes: "Verify with your local KVK before applying"

### 🌾 Community Feed
A voice-based community where farmers share crop problems and receive AI analysis. Features:
- Voice note recording and playback simulation
- AI analysis of each query
- Helpful/upvote system
- Share functionality

### 📊 Mandi Price Tracker *(Prototype)*
Sample market price data with:
- Price ticker for major crops
- Nearby mandi comparison table
- Trend indicators (up/down)
- AI buy/sell recommendation based on MSP comparison

### 🌦 Weather + Crop Calendar *(Prototype)*
Sample weather data with:
- 7-day forecast
- AI-generated crop advisory based on weather
- Crop calendar with activity reminders
- Irrigation scheduling

### 🏛 Government Scheme Advisor
Comprehensive coverage of major schemes:
- PM-KISAN (₹6,000/year income support)
- PMFBY (crop insurance up to ₹2 lakh)
- Kisan Credit Card (4% interest credit)
- Soil Health Card (free soil testing)

Each scheme includes eligibility info, benefits, required documents, and application guidance.

### 🛰️ ISRO Satellite Panel *(Illustrative Prototype)*
Dashboard showing:
- NDVI vegetation health index
- Soil moisture percentage
- SAR crop stress indicator
- 30-day NDVI trend
- Live satellite pass information

*Note: Values are illustrative. Real integration with ISRO LISS-IV and RISAT-2B SAR data is a future milestone.*

### 📔 Farm Diary
Personal farming journal with local storage:
- Date-stamped entries
- Tag system for organization
- Persistent across sessions

### 🌐 Multilingual Support
- Hindi (हिंदी) — primary
- Bhojpuri (भोजपुरी)
- Maithili (मैथिली)
- English

---

## Architecture

```
┌─────────────────────────────────────────────────────┐
│                KisanKonnect Frontend                │
│           (Progressive Web App — HTML/CSS/JS)       │
├──────────────┬──────────────┬───────────────────────┤
│  Voice Layer │   AI Layer   │    Data Layer         │
│              │              │                       │
│ Web Speech   │ Claude API   │ LocalStorage (diary)  │
│ API (input)  │ (Anthropic)  │ Static JSON (schemes) │
│              │              │                       │
│ SpeechSynth  │ Prompt       │ Sample data (mandi,   │
│ API (output) │ Engineering  │ weather) — prototype  │
└──────────────┴──────────────┴───────────────────────┘

                    FUTURE ARCHITECTURE
┌─────────────────────────────────────────────────────┐
│                   Backend API                       │
│              (Python FastAPI — planned)             │
├──────────────┬──────────────┬───────────────────────┤
│  Data APIs   │ Satellite    │   AI/ML Pipeline      │
│              │              │                       │
│ AGMARKNET    │ ISRO LISS-IV │ Custom multilingual   │
│ (mandi live) │ RISAT-2B SAR │ agricultural LLM      │
│ IMD weather  │ Resourcesat  │ (training roadmap)    │
│ PM-KISAN API │ NDVI engine  │                       │
└──────────────┴──────────────┴───────────────────────┘
```

### AI Modules (Current + Planned)

| Module | Current State | Technology |
|--------|--------------|------------|
| Crop Health Assistant | ✅ Real AI | Claude AI |
| Community Knowledge | ✅ Real AI | Claude AI |
| Market Intelligence | 🔧 Prototype | Sample data |
| Weather Advisor | 🔧 Prototype | Sample data |
| Government Scheme Assistant | ✅ Static | JSON data |
| Satellite Analysis | 🔧 Illustrative | Future: ISRO APIs |
| Farm Planning Assistant | 🗺️ Planned | Future milestone |
| Soil Guidance Assistant | 🗺️ Planned | Future milestone |
| Water Management Assistant | 🗺️ Planned | Future milestone |

---

## Tech Stack

### Current (v3.0)

| Layer | Technology | Notes |
|-------|-----------|-------|
| Frontend | HTML5, CSS3, Vanilla JavaScript | No framework — max compatibility |
| Voice Input | Web Speech API | Built into Chrome/Edge/Safari |
| AI Advisory | Anthropic Claude API | `claude-sonnet-4-6` model |
| Voice Output | SpeechSynthesis API | Hindi TTS built into browsers |
| Fonts | Baloo 2, Noto Sans Devanagari, DM Sans | Google Fonts |
| Storage | localStorage | Farm diary, settings |
| Design | CSS Custom Properties, Glassmorphism | Mobile-first |

### Planned (Roadmap)

| Layer | Technology |
|-------|-----------|
| Backend | Python 3.11 + FastAPI |
| Database | PostgreSQL |
| Cache | Redis |
| Weather | IMD / OpenWeatherMap API |
| Mandi | AGMARKNET Government API |
| Satellite | ISRO NRSC Data Portal |
| Deployment | Docker + cloud hosting |
| Mobile | PWA → React Native (future) |

---

## Getting Started

### Prerequisites

- Any modern web browser (Chrome recommended for full Web Speech API support)
- Internet connection (for Claude AI advisory)
- Microphone (for voice features)

### Quick Start

```bash
# Clone the repository
git clone https://github.com/asthamosmi-arch/KisanKonnect.git
cd KisanKonnect

# Option 1: Open directly
open KisanKonnect_v3.html

# Option 2: Serve locally (recommended)
python -m http.server 8080
# Then visit: http://localhost:8080/KisanKonnect_v3.html

# Option 3: Using Node
npx serve .
```

### AI Features Setup

The app calls the Anthropic Claude API for real AI advisory. For the API to work:

**Option A — Direct (for personal use/demo):**
Add your Anthropic API key in `KisanKonnect_v3.html`:
```javascript
headers: {
  "Content-Type": "application/json",
  "x-api-key": "YOUR_API_KEY_HERE",   // ← add this line
  "anthropic-version": "2023-06-01"
}
```

**Option B — Backend proxy (recommended for production):**
Set up a simple FastAPI proxy (see `backend/` folder — coming soon) that holds the API key server-side.

> **Security note:** Never expose your API key in client-side code in a public deployment.

### Browser Support

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| Core UI | ✅ | ✅ | ✅ | ✅ |
| AI Advisory | ✅ | ✅ | ✅ | ✅ |
| Voice Input (Speech API) | ✅ | ⚠️ Limited | ✅ | ✅ |
| Hindi TTS | ✅ | ⚠️ Limited | ✅ | ✅ |
| Dark Mode | ✅ | ✅ | ✅ | ✅ |

---

## Responsible AI

KisanKonnect takes responsible AI seriously, especially in an agricultural context where wrong advice can cause real harm.

### Our Commitments

**1. Confidence Indicators**
Every AI diagnosis shows a confidence percentage. Low-confidence results are flagged differently from high-confidence ones.

**2. Mandatory Disclaimers**
Every AI response includes: *"Verify with your local Krishi Vigyan Kendra (KVK) before applying."* This is non-negotiable.

**3. Prototype Transparency**
Features using sample data are clearly labeled with a `⚠️ Prototype` badge. Live features show a `● Live` badge. Users always know what is real vs. demo.

**4. Human Oversight**
The app explicitly positions AI as a first-line advisor, not a replacement for agricultural extension officers, KVK staff, or licensed agronomists.

**5. Privacy**
- Voice is processed locally by the browser's Web Speech API — not sent to our servers
- AI queries go to Anthropic's API — governed by their privacy policy
- No personal farming data is stored on external servers

**6. Explainable Recommendations**
AI responses always include reasoning, not just answers. Farmers understand *why* a treatment is recommended.

---

## Roadmap

### Phase 1 — Current (v3.0) ✅
- [x] Voice-first UI with Web Speech API
- [x] Real AI advisory via Claude
- [x] Hindi TTS
- [x] Community voice feed
- [x] Government schemes (static data)
- [x] Farm diary with local storage
- [x] Dark/light mode
- [x] Accessibility (ARIA, skip links)

### Phase 2 — Near Term 🔧
- [ ] Backend API (Python FastAPI)
- [ ] Live weather integration (IMD / OpenWeatherMap)
- [ ] Live Mandi prices (AGMARKNET API)
- [ ] PWA — installable on mobile home screen
- [ ] Offline mode with service worker
- [ ] WhatsApp Bot integration

### Phase 3 — Medium Term 🗺️
- [ ] ISRO satellite data integration (LISS-IV NDVI)
- [ ] Android native app (React Native)
- [ ] IVR integration (phone call access for feature phones)
- [ ] Language expansion: Marathi, Tamil, Telugu, Punjabi
- [ ] Pilot testing: 50–200 farmers in Bihar and UP

### Phase 4 — Long Term 🔭
- [ ] Custom multilingual agricultural LLM trained on KisanKonnect dataset
- [ ] IoT sensor integration (soil, weather stations)
- [ ] Satellite crop health mapping at village level
- [ ] Blockchain-based farmer identity and credit scoring
- [ ] Scale to 10+ Indian languages

---

## Contributing

KisanKonnect is open source and welcomes contributions. Here's how to get involved:

### Ways to Contribute

- 🐛 **Bug reports** — open an issue with reproduction steps
- 💡 **Feature suggestions** — open a discussion
- 🌐 **Translations** — help add more Indian languages
- 🎨 **Design** — UI/UX improvements
- 💻 **Code** — see open issues labeled `good first issue`
- 📖 **Documentation** — improve guides and comments

### Development Setup

```bash
git clone https://github.com/asthamosmi-arch/KisanKonnect.git
cd KisanKonnect
# No build step needed — open HTML directly
```

### Code Style

- Vanilla JavaScript — no frameworks (max compatibility for rural devices)
- CSS Custom Properties for theming
- Comments in English
- Hindi strings kept in UI only
- Every AI-powered feature must include a disclaimer

### Commit Convention

```
feat: add live weather API integration
fix: speech recognition stops after 30 seconds
docs: update installation guide
a11y: add ARIA labels to scheme cards
```

---

## About the Developer

**Astha Mosmi**
B.A. Program (Computer Applications + Economics), Year I
Maitreyi College, Vasant Kunj, New Delhi — 110021
📧 asthamosmi@gmail.com

KisanKonnect is a solo project built over six weeks while studying full time. It grew out of a simple observation: the people who grow food for a billion Indians have the least access to the knowledge that could help them grow it better.

**Submitted to Moonshot Awards 2026 — AI for Good category**

---

## License

MIT License — free to use, build upon, and distribute.

See [LICENSE](LICENSE) for full text.

---

<div align="center">

*"जब किसान मज़बूत होगा, तब भारत मज़बूत होगा।"*
*When the farmer is strong, India is strong.*

**⭐ Star this repo if you believe technology should speak every farmer's language.**

</div>
