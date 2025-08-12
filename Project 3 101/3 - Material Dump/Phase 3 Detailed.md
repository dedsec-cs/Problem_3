## Phase 3 – Tech Blueprint 

### **1. Development Philosophy**

- **MVP shipped by Week 3** → So even if half the team vanishes, we still have a working product to show.
- **Incremental upgrades every 2 weeks** → Each sprint adds stability + features.
- **Parallel work tracks** → Backend, frontend, AI/ML, UI/UX, Testing run at the same time.
- **Early testing & feedback loops** → Deploy MVP early so we catch issues before they snowball.

---

### **2. Upgraded Tech Stack (Scalable but Still Beginner-Friendly)**

**Frontend**

- React.js + Tailwind CSS
- ShadCN/UI for beautiful, fast prebuilt components
- React Router for navigation
- Axios for API requests

**Backend**

- Node.js + Express
- Multer for uploads
- OpenAI API for AI chat
- Tesseract.js for OCR (Phase 1) → Upgrade to Google Vision API if needed
- JWT for authentication
- Socket.IO for real-time features (optional wow-factor)

**Database**

- MongoDB Atlas
- Mongoose ORM

**DevOps**

- GitHub Actions for auto-deploy
- Netlify (frontend) + Render/Vercel (backend) hosting
- Postman for API testing

---

### **3. Core Modules (Same Structure, More Time for Depth)**

**Module 1 – Auth & User Management** _(Week 1–2)_

- JWT auth
- Roles & permissions (user/admin)
- User profile system

**Module 2 – AI Chat Assistant** _(Week 1–3)_

- Core AI responses via OpenAI
- Context memory per session
- Upgrade with domain-specific prompt engineering

**Module 3 – Data Extraction Engine** _(Week 2–4)_

- OCR with Tesseract.js
- File parsing & text cleanup
- Optional: Auto-categorization of extracted data

**Module 4 – Analytics Dashboard** _(Week 3–5)_

- Live data visualizations via [ChartJS](https://www.chartjs.org/) and [D3.JS](https://d3js.org/) 
- Filter/search functions
- Export to CSV/PDF

**Module 5 – Wow-Factors (Optional)** _(Week 5–8)_

- Voice Command Support
- Emotion-based UI themes
- Real-time collaboration view (Socket.IO)
- Mobile app wrapper via Capacitor

---

### **4. 8-Week Sprint Plan**

**Week 1–2 (Sprint 1)** → Backend + Frontend Skeletons

- Backend API structure & DB connection
- React pages & routing setup
- Auth system done


**Week 3–4 (Sprint 2)** → MVP Feature Completion

- AI Chat working end-to-end
- Data extraction functional
- Basic dashboard live

**Week 5–6 (Sprint 3)** → Feature Expansion + Polish

- Add dashboard filters/export
- Improve AI prompts for accuracy
- UI/UX refinements

**Week 7 (Sprint 4)** → Wow-Factor Features

- Add at least 1 optional big feature (voice/emotion UI)
- Mobile PWA optimization

**Week 8** → Final Testing & Demo Prep

- Full bug hunt
- Stress testing
- Polished presentation & dry run

**Person 1 (Lead Dev / Backend AI)** – System architecture, AI integration, OCR  
**Person 2 (Frontend Lead)** – UI structure, component design, dashboard visuals  
**Person 3 (Backend Auth & Data)** – Auth, DB schema, analytics APIs  
**Person 4 (Feature Enhancer)** – Optional features, mobile/PWA, socket events  
**Person 5 (QA & Product Manager)** – Weekly testing, Kanban updates, presentation


---

