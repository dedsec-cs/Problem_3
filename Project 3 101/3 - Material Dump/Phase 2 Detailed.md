# PHASE 2 – DEEP ANALYSIS

**Goal:** Choose the smartest, safest, and most impactful features to actually build in the hackathon.
## **1. Impact vs Effort Prioritization**

|ID|Feature|Impact|Effort|Decision|
|---|---|---|---|---|
|UC1|No-code survey creation|High|High|✅ Keep – core, but start with simple drag-drop builder|
|UC2|Standardized question bank|High|Low|✅ Keep – easy boost for speed|
|UC3|Multi-channel delivery|High|Medium|✅ Keep – WhatsApp + Web for MVP, mock IVR/avatar|
|UC4|Multilingual text & voice|High|Medium|✅ Keep – text multilingual now, voice later|
|UC5|Data prepopulation|Medium|High|⚠ Keep – use mock data for MVP to avoid API delays|
|UC6|AI adaptive questioning|High|Medium|✅ Keep – simple rules-based now, AI LLM later|
|UC7|Real-time validation|High|Medium|✅ Keep – basic form validation + simple AI checks|
|UC8|Auto-coding responses|Medium|Medium|✅ Keep – static mapping tables for MVP|
|UC9|Monitoring dashboard|High|Medium|✅ Keep – minimal metrics (completion rate, flags)|
|UC10|Paradata capture|Medium|Low|✅ Keep – log timestamps, GPS, device|
|UC11|Consent capture & compliance|High|Low|✅ Keep – must have for gov project|
|UC12|Secure storage|High|Low|✅ Keep – Firebase/Atlas encryption|

**Optional Features (Future Scope / Judge Candy):**

|ID|Feature|Impact|Effort|Decision|
|---|---|---|---|---|
|OPT1|Self-service chatbot|Medium|High|❌ Drop now|
|OPT2|OCR for docs|Medium|High|❌ Drop now|
|OPT3|Real-time analytics|Medium|Medium|⚠ Keep if time permits|
|OPT4|Biometric verification|Low|High|❌ Drop now|
|OPT5|AI summarization|Medium|Medium|⚠ Keep if API ready|
|OPT6|Offline mode|High|High|❌ Drop – risky for hackathon timeframe|

---

## **2. Dependencies (What Must Happen Before What)**

|Dependent Feature|Depends On|
|---|---|
|UC5 Data prepopulation|Dataset/API integration ready|
|UC6 Adaptive questioning|Basic survey creation done|
|UC7 Real-time validation|Survey form functional|
|UC8 Auto-coding|Survey response capture working|
|UC9 Dashboard|Survey + paradata capture functional|

---

## **3. Kill or Postpone Risky Features**

- **Offline Mode** → Skip for MVP; too complex for short timeframe.
- **Biometric Verification** → High complexity, low core relevance.
- **OCR Document Scanning** → Requires extra pipeline & libs, skip for MVP.
- **Avatar/Full Voice Support** → Mock for demo, build text fully.

---

## **4. MVP Lock – “Definition of Done” Per Feature**

|Feature|Definition of Done|
|---|---|
|No-code survey creation|Admin can create/edit survey using drag-drop or form wizard|
|Question bank|Preloaded set of at least 20 gov-standard questions|
|Multi-channel|Survey works on web and WhatsApp sandbox|
|Multilingual (text)|User chooses language at start, all questions auto-translated|
|Prepopulation (mock)|Auto-fill at least 3 fields when ID entered|
|Adaptive questioning|Conditional skip logic or simple AI rules|
|Real-time validation|Blocks submission on missing/invalid answers|
|Auto-coding|Stores coded values in DB for at least 2 question types|
|Dashboard|Shows completion %, error flags, enumerator list|
|Paradata capture|Logs timestamps, GPS, and device type|
|Consent & compliance|Records a Yes/No consent before survey start|
|Secure storage|Data encrypted at rest & in transit|

---

## **5. MVP Build Order (Execution Logic)**

1. **Backend foundation** (Auth, DB schema, API endpoints).
2. **Survey creation** (drag-drop + question bank).
3. **Survey rendering on web** (basic form logic).
4. **Multi-language support** (start with 2–3 languages).
5. **WhatsApp integration** (parallel dev track).
6. **Validation + adaptive logic**.
7. **Prepopulation mock + auto-coding**.
8. **Dashboard + paradata logging**.
9. **Security, consent, polish**.
