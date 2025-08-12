# **PHASE 1 – EXTRACTION**

**Goal:** Break down the problem into beginner-friendly English, map out actors/triggers/outcomes, identify all core & optional features, required data/APIs, and prep questions for mentors.

---

## **1. Problem in Plain English**

We’re building a **Government-grade AI-powered survey system** for MoSPI that can:

- Create surveys without coding (even from plain text prompts).
- Deliver them through **multiple channels** — WhatsApp, phone calls, AI avatars, web/mobile.
- Speak and understand **multiple languages** (text + voice).
- **Pre-fill answers** from existing data using unique IDs.
- **Adapt questions in real-time** based on AI logic and responses.
- **Validate and code answers automatically** while the survey is being filled.
- Store responses securely in **structured formats**.
- Track and analyze **enumerator performance and data quality**.

---

## **2. Core Use Cases (Must-Haves for MVP)**

| ID   | Use Case                          | Actor(s)           | Trigger                   | Outcome                                                    |
| ---- | --------------------------------- | ------------------ | ------------------------- | ---------------------------------------------------------- |
| UC1  | No-code survey creation           | Survey admin       | Admin logs into dashboard | Creates a new survey via drag-and-drop or prompt input     |
| UC2  | Access standardized question bank | Admin              | Admin building survey     | Pre-loaded question templates ready for use                |
| UC3  | Multi-channel survey delivery     | System, Respondent | Survey is published       | User can respond via WhatsApp, IVR, avatar, or web         |
| UC4  | Multilingual text & voice         | Respondent, AI     | Survey starts             | Respondent interacts in their preferred language           |
| UC5  | Data prepopulation                | System             | Unique ID provided        | Fields auto-filled from linked datasets                    |
| UC6  | AI-driven adaptive questioning    | System             | Mid-survey                | Next question adjusts based on responses                   |
| UC7  | Real-time validation              | System             | Respondent answers        | Flags errors/inconsistencies instantly                     |
| UC8  | Auto-coding of responses          | System             | Response submitted        | Coded per classification standards (NCO/NIC/ISIC)          |
| UC9  | Dashboard monitoring              | Supervisor/Admin   | Anytime                   | View progress, quality metrics, and enumerator performance |
| UC10 | Paradata capture                  | System             | Survey in progress        | Logs time, GPS, device, mode, and pauses                   |
| UC11 | Consent capture & compliance      | System, Respondent | Start of survey           | Consent recorded and stored securely                       |
| UC12 | Secure storage                    | System             | Response received         | Data encrypted and stored in SQL/NoSQL                     |

---

## **3. Optional / Wow-Factor Features (Future Scope or Judge Bonus)**

|ID|Feature|Actor(s)|Outcome|
|---|---|---|---|
|OPT1|Integrated self-service chatbot|Respondent|Can complete survey without enumerator|
|OPT2|OCR for document scanning|Enumerator|Extracts data from ID cards, documents|
|OPT3|Real-time analytics dashboard|Admin|Instant visualization of survey results|
|OPT4|Biometric/facial recognition|Respondent|Verify identity before survey|
|OPT5|AI summarization of open responses|System|Summarizes qualitative data instantly|
|OPT6|Offline mode|Enumerator|Survey works without internet, syncs later|

---

## **4. Actors**

- **Respondent** – Person answering the survey.
- **Enumerator** – Field agent facilitating the survey.
- **Survey Admin** – Creates and manages surveys.
- **Supervisor** – Monitors survey progress and quality.
- **AI/Backend System** – Handles adaptive logic, validation, and data storage.

---

## **5. Triggers**

- Survey creation event by admin.
- Survey distribution event via channels.
- Respondent starts answering.
- Unique ID match found (triggers prepopulation).
- AI detects inconsistent answer (triggers flag).
- Supervisor views dashboard.

---

## **6. Expected Outcomes**

- Functional prototype with multi-channel, multilingual survey execution.
- AI-based adaptive and validation features.
- Structured and secure data storage.
- Quality monitoring dashboard.
- Consent & privacy compliance.

---

## **7. Required Data & APIs**

- **Datasets:**
    
    - NSS sample questionnaires.
    - Local Government Directory (LGD) codes for geotagging.
    - Open Census/SECC socio-economic datasets for prepopulation.

- **APIs:**
    
    - WhatsApp Business API (Twilio/Meta).
    - IVR API (Exotel/Plivo/Twilio Voice).
    - Translation API (Google Cloud Translate, IndicTrans, Microsoft Translator).
    - Speech-to-Text & Text-to-Speech (Google STT/TTS, OpenAI Whisper).
    - Map/GPS APIs (Google Maps, OpenStreetMap).
    - Classification codes API or static datasets.
    - Secure auth (Firebase Auth or Keycloak).


---

## **8. Clarification Questions for Mentors**

1. **Deployment** – Can we use public cloud for prototype hosting?
2. **Data Access** – Will we get real LGD/Census datasets or must we simulate them?
3. **WhatsApp API** – Will a sandbox account be provided?
4. **Voice Support** – Is basic prototype enough or must it be production-ready?
5. **Offline Mode** – Is it required in MVP?
6. **AI Model Rules** – Can we use external APIs like OpenAI, or must models be local for privacy?
7. **Security** – Any mandatory compliance standards (e.g., ISO, NIC infra)?

---

✅ With this, Phase 1 is **fully complete** — our team now has:

- Clear understanding of the problem.
- Explicit MVP vs. optional features.
- Actors, triggers, and outcomes mapped.
- API/data needs.
- Mentor question list to de-risk early.
