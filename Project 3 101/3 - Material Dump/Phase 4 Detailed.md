# PHASE 4 – MVP PLAN (2-Month Hackathon)

**Goal:** Ship a working MVP early, avoid last-minute chaos, and have time left for polish + wow-factor.

---

## **1. Key Principles**

- **MVP First, Fancy Later** — Judge candy only happens after core is solid.
- **Parallel Tracks** — Frontend, backend, and integrations progress together.
- **Demo-Readiness Checkpoints** — We treat every major milestone like a mini-demo.
- **48-Hour Freeze Rule** — No risky changes right before demo.

---

## **2. Week-by-Week Timeline**

|Week|Goal|Deliverables|
|---|---|---|
|**Week 1**|**Foundation Setup**|GitHub repo, branch rules, linting, Husky hooks, basic folder structure, Firebase Auth integration, MongoDB Atlas setup.|
|**Week 2**|**Core Backend & Survey Data Models**|Survey CRUD API, Response API, Adaptive Logic (basic rules), Paradata schema.|
|**Week 3**|**Survey Builder (Frontend)**|Drag-drop UI, Question bank integration, Save to DB.|
|**Week 4**|**Survey Runner (Frontend)**|Multi-language text survey, Basic validation, Prepopulation mock. **DEMO CHECKPOINT 1** — First full survey from creation → response stored in DB.|
|**Week 5**|**Integrations**|WhatsApp survey delivery, Google Translate API, STT/TTS prototype.|
|**Week 6**|**Dashboard**|Completion rate, error flags, enumerator list, paradata display. **DEMO CHECKPOINT 2** — MVP with multi-channel, multi-language, dashboard live.|
|**Week 7**|**Polish & Optional Features**|Auto-coding with classification codes, styling improvements, mock analytics charts, animations.|
|**Week 8**|**Final Polish & Demo Prep**|Bug fixes, security checks, consent screen, README, deployment scripts, backup demo video. **DEMO CHECKPOINT 3** — Judge-ready build.|

---

## **3. Parallel Work Streams**

- **Backend Track**
    
    - Week 1–2: Auth, Survey CRUD, Response API
    - Week 3–4: Adaptive logic, validation, auto-coding
    - Week 5–6: Integrations layer, security & encryption
- **Frontend Track**
    
    - Week 1–2: Layout, theme setup, shared components
    - Week 3: Survey Builder
    - Week 4: Survey Runner (web)
    - Week 5–6: Dashboard, multi-language
- **Integration Track**
    
    - Week 4–5: WhatsApp + Translation API
    - Week 6: Speech APIs, Maps/GPS
- **QA & Docs Track**
    
    - Ongoing: Testing scripts, bug tracking, README updates
    - Week 7–8: Demo rehearsals, fallback scenarios

---

## **4. Demo-Readiness Checkpoints**

1. **Checkpoint 1 (End of Week 4)** — End-to-end survey on web works.
2. **Checkpoint 2 (End of Week 6)** — Multi-language + WhatsApp live + dashboard showing progress.
3. **Checkpoint 3 (End of Week 8)** — Polished, bug-free, judge-ready demo.

---

## **5. Testing Workflow**

- **Every Friday**: Team runs staging build together and logs bugs.
- **Every Monday**: Assign bug fixes & new tasks.
- **Tools**: Postman for API testing, Netlify staging URL for frontend, Render staging URL for backend.

---

## **6. MVP Core Feature List (Must Be Done by Week 6)**

- No-code survey creation with question bank
- Web-based survey runner with multi-language text
- WhatsApp delivery (working in sandbox)
- Adaptive questioning (basic rules)
- Real-time validation
- Response storage in MongoDB
- Dashboard with basic stats + paradata
- Consent capture & secure storage

---

## **7. Judge Prep Strategy**

- By **Week 7**, we’re only doing **polish, wow-factor features, and rehearsals**.
    
- Build a **short, punchy demo flow**:
    
    - 30s problem intro
    - 1 min live demo of MVP
    - 30s highlight of wow features
    - 30s impact/future vision


---

## **8. Safety Nets**

- **If WhatsApp API fails** → Show web survey and API logs.
- **If Speech APIs fail** → Keep text mode ready.
- **If DB fails** → Mock responses in local JSON and fake dashboard data.
- **If live demo internet fails** → Show pre-recorded demo video.
