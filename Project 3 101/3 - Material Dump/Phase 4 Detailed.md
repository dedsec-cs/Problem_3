## Phase 4 – MVP Plan 

### **🎯 MVP Goal**

Deliver a working, demo-ready product in **3 weeks** that:

- Has **all core modules functional**
    
- Can run on any laptop with internet access
    
- Looks clean enough for a faculty demo
    
- Can survive if one feature fails during judging
    

---

## **1. MVP Feature Set (No More, No Less)**

✅ **Auth & User Management**

- Register/Login
    
- JWT-based authentication
    
- User profiles with basic info
    

✅ **AI Chat Assistant**

- Accepts text queries & returns OpenAI responses
    
- Handles at least 5 pre-defined query types
    
- Simple UI with chat bubbles
    

✅ **Data Extraction Tool**

- Upload PDFs or images
    
- OCR to extract text
    
- Show extracted content in a preview box
    

✅ **Analytics Dashboard**

- Displays charts/tables from extracted or chat data
    
- At least 2 types of visualizations (bar chart, pie chart)
    
- Basic filtering (date/category)
    

---

## **2. 3-Week MVP Sprint Plan**

### **Week 1 – Skeleton & Core Setup**

**Frontend**

- React + Tailwind setup
    
- Page routing (Login, Chat, Dashboard)
    
- Basic UI layout
    

**Backend**

- Node.js + Express setup
    
- MongoDB Atlas connection
    
- Auth endpoints done (register, login, JWT middleware)
    

**Milestone:** Auth module working E2E (login → dashboard redirect)

---

### **Week 2 – Core Features Integration**

**Frontend**

- Chat UI component linked to backend
    
- File upload UI for OCR
    
- Placeholder charts with dummy data
    

**Backend**

- AI Chat endpoint integrated with OpenAI API
    
- OCR endpoint functional with Tesseract.js
    
- Dashboard API to serve processed data
    

**Milestone:** Chat, file upload, and dashboard pages fetch live backend data

---

### **Week 3 – MVP Completion & First Demo**

**Frontend**

- Polish UI with ShadCN/UI components
    
- Make dashboard charts interactive
    
- Implement basic filtering
    

**Backend**

- Store extracted text in MongoDB
    
- Return stored data for dashboard queries
    
- Add error handling + basic logging
    

**Milestone:** **Full MVP ready** — Auth → Chat → Data extraction → Dashboard works end-to-end

---

## **3. Division of Labor (First 3 Weeks)**

**You (Lead Dev)** – Backend architecture, AI Chat integration, OCR backend  
**Person 2** – Frontend skeleton, Chat UI, integration with backend  
**Person 3** – Auth backend + frontend forms, MongoDB schema setup  
**Person 4** – Dashboard backend APIs, Chart.js visualizations  
**Person 5** – Testing each module as it’s built, dummy data creation, slide prep

---

## **4. Parallel Work Streams**

We’ll keep **frontend & backend completely separate** until Week 2 mid-point.  
This means:

- Frontend team uses dummy JSON for UI
    
- Backend team uses Postman to test APIs
    
- Merge only after both are stable
    

---

## **5. MVP Demo Strategy**

- Show **end-to-end flow** in under 3 minutes
    
- Avoid live coding — run a **pre-filled demo**
    
- Keep backup screenshots in case internet fails
    
- Make sure at least 3 team members can run the demo locally
    

---
Now We Have:-
- Locked MVP features
- 3-week timeline with milestones
- Role assignments for MVP
- Parallel work method to avoid merge chaos
- Demo plan for early validation