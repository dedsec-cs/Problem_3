# **PHASE 3 – TECH BLUEPRINT (Overkill Edition)**

**Goal:** Build a bulletproof technical foundation so we ship **fast**, **without bugs**, and **without team collisions** — while impressing judges with solid architecture and pro workflows.
## **1. Tech Stack – Locked, Fast, and Scalable**

We’re balancing **MVP speed** with **future scalability** so nothing breaks under demo pressure.

|Layer|Tech|Why We’re Choosing It|
|---|---|---|
|**Frontend Framework**|**React 18 + Vite**|Vite’s hot reload is insanely fast, React is proven and beginner-friendly.|
|**UI Styling**|**Tailwind CSS + shadcn/ui**|Rapid styling, prebuilt accessible components, dark mode support.|
|**Backend Framework**|**Node.js 20 + Express**|Fast setup, easy API development, massive package ecosystem.|
|**Database**|**MongoDB Atlas**|Handles dynamic survey schemas; cloud-based, no server setup.|
|**Authentication**|**Firebase Auth**|Simple setup, supports email, phone OTP, and social logins.|
|**Hosting (Frontend)**|**Netlify**|Auto-deploy from GitHub, instant rollbacks.|
|**Hosting (Backend)**|**Render**|Continuous deploy from GitHub, free SSL, staging + prod.|
|**Messaging API**|**WhatsApp Cloud API** (Meta)|Direct government-grade channel; fallback: Twilio Sandbox.|
|**Translation API**|**Google Cloud Translate API**|Supports 100+ languages including Indic.|
|**Speech-to-Text**|**OpenAI Whisper API**|Accurate transcription for multiple languages.|
|**Text-to-Speech**|**Google Cloud TTS**|Clear voice output in multiple languages.|
|**Maps/GPS**|**Google Maps API + LGD Codes Dataset**|Location tagging and administrative mapping.|
|**Analytics**|**Chart.js / Recharts**|For dashboards and data visualization.|
|**Version Control**|**GitHub**|Central repo with protected branches.|
|**Dev Tools**|**Postman, ESLint, Prettier, Husky Hooks**|For API testing and code quality enforcement.|

---

## **2. Detailed System Architecture**

```
          ┌─────────────────── FRONTEND ────────────────────┐
          │ React + Tailwind + shadcn/ui                     │
          │ - Survey Builder (no-code UI)                    │
          │ - Survey Runner (web, multi-language)            │
          │ - Dashboard (progress, quality, paradata)        │
          └───────────────┬──────────────────────────────────┘
                          │ REST + WebSocket (Realtime Flags)
          ┌───────────────▼────────────────┐
          │         BACKEND (Express)       │
          │ - Auth via Firebase Middleware  │
          │ - Survey CRUD API               │
          │ - Response Handling             │
          │ - AI Adaptive Logic Layer       │
          │ - Data Validation Engine        │
          │ - Auto-Coding Engine            │
          │ - Paradata Capture              │
          │ - WebSocket Event Push          │
          └───────────────┬────────────────┘
          ┌───────────────┼─────────────────────────────────────┐
          │                │                                     │
  ┌───────▼───────┐ ┌──────▼──────────┐ ┌────────────────────────▼────────────┐
  │ MongoDB Atlas │ │ Firebase Auth   │ │ External APIs                        │
  │ - Surveys     │ │ - User Mgmt     │ │ - WhatsApp API (Meta)                 │
  │ - Responses   │ │ - Session Mgmt  │ │ - Google Translate (Multilingual)     │
  │ - Paradata    │ │                 │ │ - Whisper (Speech-to-Text)            │
  │ - User Roles  │ │                 │ │ - Google TTS                          │
  └───────────────┘ └─────────────────┘ │ - Google Maps / LGD Codes             │
                                        └───────────────────────────────────────┘
```

---

## **3. Repo & Branch Management (Merge Chaos Prevention)**

**Repo Setup:**

- **main** → Production-ready code only.
- **dev** → Integration branch for QA-tested features.
- **feature/*** → One branch per feature (e.g., `feature/survey-builder`).
- **hotfix/*** → For urgent demo bugs.
- **docs/*** → Documentation updates.

**Branching Workflow:**

1. `git checkout -b feature/your-feature-name`
2. Work locally → **Commit small, descriptive messages**.
3. Push to origin → Open PR to `dev`.
4. Peer review → Merge to `dev` after review.
5. QA team tests in staging → Merge `dev` → `main`.

---

## **4. Code Quality & Commit Rules**

- **ESLint + Prettier** → Auto-format + lint before commit.
- **Husky pre-commit hooks** → Blocks bad code from entering repo.
- **Commit Message Format**:
    
    ```
    feat: added multilingual survey selection
    fix: resolved API CORS issue
    docs: updated README for deployment
    ```
    

---

## **5. Deployment Strategy**

- **Staging Environment**:
    
    - Netlify (frontend) → staging branch.
    - Render (backend) → staging instance.
- **Production Environment**:
    
    - Netlify (frontend) → main branch auto-deploy.
    - Render (backend) → main branch auto-deploy.

---

## **6. Testing Workflow**

- **Unit Tests**: Jest for backend, React Testing Library for frontend.
- **Integration Tests**: Postman collections for API endpoints.
- **Manual QA**: Every Friday — entire team tests staging build together.
- **Demo Freeze Rule**: No merges to main 48 hours before final demo.

---

## **7. Parallel Dev Tracks (First 3 Weeks)**

|Track|Tasks|Owner|
|---|---|---|
|**Backend API**|Auth, Survey CRUD, Response API, Adaptive Logic|You|
|**Frontend Builder**|Drag-drop builder, question bank integration|Dev 1|
|**Frontend Runner**|Multi-language rendering, validation, prepopulation mock|Dev 2|
|**Integrations**|WhatsApp, translation, speech APIs|Dev 3|
|**Dashboard**|Metrics, paradata view, enumerator list|Dev 4|
|**QA & Docs**|Setup lint, tests, README, deployment scripts|Dev 5|

---

## **8. Risk Mitigation Rules**

- **If API fails** → Mock data for demo.
- **If WhatsApp fails** → Use web runner for demo, show API logs as proof.
- **If speech-to-text fails** → Fall back to text input with translation.
- **If adaptive AI fails** → Use rule-based branching.

---

## **9. Judge-Friendly Extras We’ll Prep Early**

- Clean UI (dark/light theme toggle).
- Live dashboard during demo.
- Real paradata sample in the dashboard.
- Clear README + deployment link.
- Short 1–2 min demo video as backup.

---

This **Overkill Phase 3** now has:

- Locked **stack**.
- Full **architecture diagram**.
- Strict **branching & code rules**.
- **Parallel work plan** to maximize time.
- Risk fallbacks so **nothing breaks on demo day**.
