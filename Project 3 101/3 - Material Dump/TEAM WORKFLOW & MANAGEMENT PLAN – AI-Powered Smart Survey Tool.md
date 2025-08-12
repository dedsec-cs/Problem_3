# TEAM WORKFLOW & MANAGEMENT PLAN – AI-Powered Smart Survey Tool

---

## **1. Team Roles & Responsibilities**

We’ll have **clear ownership** so everyone knows their lane but can back each other up if needed.

|Role|Person|Responsibilities|
|---|---|---|
|**Tech Lead / Backend Lead**|You|API design, DB models, adaptive logic, integrations, code reviews|
|**Frontend Lead**|Dev 1|Survey Builder UI, Survey Runner, frontend API integration|
|**Integration Specialist**|Dev 2|WhatsApp API, translation, STT/TTS|
|**Dashboard & Data Lead**|Dev 3|Dashboard UI, paradata display, charts, supervisor tools|
|**QA & Docs Lead**|Dev 4|Testing, bug tracking, README, deployment scripts|
|**UX/UI Designer** _(optional if we have one)_|Dev 5|Styling, animations, accessibility|

**Golden Rule:** If your part is blocked, **help someone else before going idle**.

---

## **2. Communication Protocol**

We’ll use a **two-channel system** to avoid spam but keep info flowing.

- **WhatsApp Group** → Quick updates, urgent blockers, coordination.
- **GitHub Issues/Projects** → All tasks and progress tracking.
- **Google Meet / Discord** → Weekly sprint calls + daily standups.

---

## **3. Daily Stand-up (Max 10 Minutes)**

**Format:** Each member answers:

1. **Yesterday** – What I completed.
2. **Today** – What I’m working on.
3. **Blockers** – Any problems stopping me.

If blockers are found → Solve after the standup, not during.

---

## **4. Weekly Sprint Planning**

**When:** Every Monday evening  
**Agenda:**

1. Review previous week’s progress.
2. Assign new tasks from backlog.
3. Prioritize MVP features over extras.
4. Set **Friday mini-demo goal**.

**When:** Every Saturday morning (Review)

- Merge stable features to `dev`.
- Deploy staging build.
- Everyone tests and logs bugs in GitHub Issues.

---

## **5. Task Management Rules**

We’ll run **GitHub Projects (Kanban)** with 4 columns:

- **Backlog** → Not started yet.
- **In Progress** → Currently being worked on.
- **In Review** → PR waiting for code review.
- **Done** → Merged & deployed.

**Task Assignment Flow:**

- Open GitHub issue → Assign yourself → Move to “In Progress”.
- Once done → Open PR → Move to “In Review”.
- After review → Merge → Move to “Done”.

---

## **6. Coding Workflow**

**Branching Rules:**

- `main` → Stable, demo-ready only.
- `dev` → Integration branch for tested features.
- `feature/<name>` → One feature per branch.
- `hotfix/<name>` → Urgent fixes.

**Commit Guidelines:**

- Write small, meaningful commits:
    
    ```
    feat: added multilingual selection to survey runner
    fix: resolved CORS issue in backend API
    docs: updated setup guide in README
    ```
    
- Commit often, push daily.
    
**Code Reviews:**

- All PRs to `dev` require **at least 1 approval**.
- QA Lead runs feature on staging before merge to `main`.

---

## **7. Testing & QA Flow**

- **Every Friday** → Full team runs the app on staging.
    
- Use **checklists** for each feature:
    
    - Does it work?
    - Does it break other features?
    - Does it look good on mobile + desktop?
- Log bugs in GitHub Issues with steps to reproduce + screenshot.


---

## **8. Risk & Fallback Management**

- **If blocked > 24h** → Ping Tech Lead, reassign task.
- **If integration/API is failing** → Switch to mock data for MVP.
- **If feature isn’t demo-ready by Week 6** → Push to “future scope”.

---

## **9. Meeting Cadence**

|Day|Meeting|Duration|Purpose|
|---|---|---|---|
|Mon|Sprint Planning|30 min|Assign tasks, set goals|
|Tue–Fri|Standup|10 min|Status update, blockers|
|Sat|Review & Testing|45 min|Deploy to staging, test, log bugs|
|Sun|Optional catch-up|—|Self-paced dev time|

---

## **10. Hackathon Survival Rules**

- **Avoid Feature Creep** — No new features after Week 6.
- **Ship Small, Ship Often** — Push working code daily.
- **Demo > Perfection** — A working feature that looks 80% good is better than a broken 100% perfect idea.
- **Always Have a Fallback** — For every risky feature, have a simpler version ready.
