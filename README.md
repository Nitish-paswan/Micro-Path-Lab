# Micro-Path-Lab
MICRO PATH is a modern, responsive, bilingual (English/Hindi) pathology lab and tele-triage web platform featuring voice-to-text queries, lab report vaults, doctor consultation, and doorstep sample collection.

https://nitish-paswan.github.io/Micro-Path-Lab/
visit website
## 🌟 Key Features

### 1. Complete Bilingual System (English & हिंदी)
- One-click global language switcher (`[English] | [हिंदी]`).
- Instant state-preserving DOM updates (form inputs remain intact when toggling languages).
- Localized validation feedback and clinical terms.

### 2. Dual-Mode "Ask a Doctor" (Voice + Text)
- **Speech-to-Text (STT):** Integrated Web Speech API (`SpeechRecognition`) supporting both Indian English (`en-IN`) and Hindi (`hi-IN`).
- **Editable Transcripts:** Patients can review and edit recognized speech before submitting.
- **Text-to-Speech (TTS):** "Listen" button allowing visually impaired or elderly patients to hear doctor responses read aloud.

### 3. Pathology & Diagnostic Suite
- Test catalog covering CBC, HbA1c, Liver Function (LFT), Kidney Function (KFT), Lipid, Thyroid, Urine Routine, and Microbiology.
- Comprehensive test cards specifying sample type (Serum, EDTA, Urine), fasting/prep instructions, turnaround time (TAT), and live pricing.
- Real-time search by test name, category, or health condition.

### 4. Doorstep Phlebotomy & Report Vault
- **Home Sample Collection:** Online booking system with cold-chain protocol advisories and slot booking.
- **Report Upload System:** Supports PDF, JPG, and PNG uploads with instant tracking reference generation (`MP-REP-XXXXX`).

### 5. Multi-Role Control Centers
- **Patient Dashboard:** Tracks query statuses, appointment confirmations, and past uploaded lab files.
- **Doctor Dashboard:** Triage queue with workflow statuses (`New`, `In Review`, `Replied`, `Closed`), audio query playback, and dictation tools for replies.
- **Admin Panel:** Dynamic price management, emergency contact config (Phone, WhatsApp, Timings), and staff oversight.

---

## 🛡️ Medical Safety & Disclaimers

> **IMPORTANT CLINICAL NOTICE**
> 
> MICRO PATH is designed for pathology service coordination, triage assistance, and administrative workflow management. 
> 
> - **No Autonomous Diagnosis:** The platform does not generate automated or AI-based diagnoses. All medical assessments require review by an authorized medical professional.
> - **Emergency Protocol:** In acute or life-threatening emergencies, patients must not wait for online replies. Direct contact with local emergency medical services (e.g., 112 / 108 / 911) or immediate transit to the nearest emergency department is strictly advised.

---

## 🛠️ Tech Stack

- **Frontend:** Semantic HTML5, Vanilla JavaScript (ES6+), Modern CSS3 (CSS Grid, Flexbox, Custom Properties).
- **Styling / Icons:** Tailwind CSS / FontAwesome Icons.
- **Browser APIs:** 
  - `webkitSpeechRecognition` / `SpeechRecognition` (Voice Input)
  - `window.speechSynthesis` (Audio Output)
  - `FileReader API` (Client-side Report File Previews)
  - `localStorage` (Session simulation & state persistence)

---

## 📁 Suggested Folder Structure

```text
micro-path/
├── index.html              # Main application single-page layout
├── README.md               # Project documentation
├── LICENSE                 # MIT License file
├── assets/
│   ├── css/
│   │   └── style.css       # Custom styles & animation overrides
│   ├── js/
│   │   ├── app.js          # Core app controller & state
│   │   ├── voice.js        # Web Speech API & TTS wrappers
│   │   ├── i18n.js         # English & Hindi translation dictionaries
│   │   └── storage.js      # LocalStorage & mock data layer
│   └── images/
│       ├── logo.svg        # MICRO PATH vector branding
│       └── hero-bg.jpg     # Clinical banner visuals
