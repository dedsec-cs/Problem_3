# DEVELOPMENT PHASE PLAN – AI-Powered Smart Survey Tool

## **Phase A – Setup & Foundations (Week 1)**

**Goal:** Lock environment, repo, and basic infra before touching features.

**Tasks:**

- [ ] Create GitHub repo with `main`, `dev`, and `feature/*` branches.
- [ ] Add ESLint, Prettier, Husky pre-commit hooks.
- [ ] Create `/frontend` (React + Vite + Tailwind + shadcn/ui) and `/backend` (Node + Express) folders.
- [ ] Set up Firebase project for authentication.
- [ ] Set up MongoDB Atlas cluster and create survey DB schema skeleton.
- [ ] Create `.env.example` with API keys (WhatsApp, Google Translate, Whisper, Maps).
- [ ] Deploy empty frontend to Netlify and backend to Render (staging links ready).

**Output:**  
Running “Hello World” on both frontend & backend with connected DB.

---

## **Phase B – Core Backend APIs (Week 2–3)**

**Goal:** Get backend APIs ready for MVP features.

**Tasks:**

- [ ] **Auth Middleware** → Firebase JWT verification.
- [ ] **Survey CRUD API** → Create, read, update, delete surveys.
- [ ] **Response Submission API** → Accept responses, store in DB.
- [ ] **Adaptive Logic API** → Basic rules engine for skip/conditional flow.
- [ ] **Validation API** → Basic required-field + type checks.
- [ ] **Paradata Logger** → Time, GPS, device info logging.


**Output:**  
Postman-tested backend with working endpoints for surveys & responses.

---

## **Phase C – Core Frontend (Week 3–4)**

**Goal:** Build the no-code survey builder and survey runner (web).

**Tasks:**

- [ ] **Survey Builder UI** → Drag-drop form elements, link to question bank.
- [ ] **Question Bank Module** → Preloaded templates.
- [ ] **Survey Runner UI** → Render questions with multilingual text.
- [ ] **Validation UI** → Show inline errors.
- [ ] **Prepopulation Mock** → Auto-fill fields if ID matches sample data.
- [ ] Connect frontend to backend APIs.

**Output:**  
Full survey creation → survey running → response stored in DB.

**Demo Checkpoint 1:** End of Week 4 — First working web-based survey flow.

---

## **Phase D – Integrations (Week 5)**

**Goal:** Add multi-channel + multilingual capability.

**Tasks:**

- [ ] **WhatsApp API Integration** (Meta/Twilio) → Send survey link or questions.
- [ ] **Google Translate API** → Language switch for questions/answers.
- [ ] **Speech-to-Text (Whisper)** → Voice-to-text in chosen language.
- [ ] **Text-to-Speech (Google TTS)** → Read questions aloud.

**Output:**  
Survey working on both **web** and **WhatsApp** with multilingual support.

---

## **Phase E – Dashboard & Quality Control (Week 6)**

**Goal:** Give supervisors real-time visibility.

**Tasks:**

- [ ] **Completion Rate Display** → Percentage of finished surveys.
- [ ] **Enumerator Performance Table** → List with counts & average times.
- [ ] **Paradata Visualization** → Time spent, GPS map view.
- [ ] **Error Flag Panel** → AI/validation flags.
- [ ] **Real-Time Update via WebSockets**.

**Output:**  
Supervisors can monitor progress + quality in real-time.

**Demo Checkpoint 2:** End of Week 6 — MVP fully functional.

---

## **Phase F – Polish & Wow-Factor (Week 7)**

**Goal:** Make MVP shine for judges.

**Tasks:**

- [ ] Add animations, better styling (Framer Motion).
- [ ] Add AI auto-coding for open responses.
- [ ] Add live updating dashboard charts (Recharts/Chart.js).
- [ ] Add auto-language detection on start.
- [ ] Add light/dark theme toggle.

**Output:**  
Visually polished, AI-enhanced version of MVP.

---

## **Phase G – Demo Prep & Freeze (Week 8)**

**Goal:** Ensure smooth, risk-free demo.

**Tasks:**

- [ ] Final bug fixes.
- [ ] Write clean README & deployment guide.
- [ ] Record 2–3 min backup demo video.
- [ ] Load test with at least 20 concurrent survey runs.
- [ ] Prepare fallback scenarios (mock data, video demo).

**Output:**  
Judge-ready, stable, and visually impressive build.

**Demo Checkpoint 3:** End of Week 8 — Final presentation rehearsal.

---

## **Key Management Rules**

- [ ] **Daily stand-up**: 10 min max → blockers, priorities, updates.
- [ ] **Weekly code freeze for review** every Saturday.
- [ ] **Feature freeze at Week 6** — Weeks 7–8 are polish only.
- [ ] **Always test on staging before merge to main**.

