# Phase 1 – Extraction

## 1. Problem Statement 

We are building a **multi-feature intelligent platform** that solves real-world problems through automation, AI, and user-centric design.  
The system will focus on **core functional workflows** first (must-have use cases) and later add **wow-factor extras** (optional features) depending on time and resources.

---

### **2. Use Cases (Core vs Optional)**

**Core Use Cases (Must Deliver)**

1. **AI-Powered Chat Assistant** – Handles user queries, provides guidance, and processes requests via a simple UI.
2. **Smart Data Extraction Tool** – Pulls structured data from unstructured sources (text, PDFs, or images).
3. **Basic Analytics Dashboard** – Displays processed results in a clean, easy-to-read format.
4. **User Account System** – Simple login/registration to store preferences and past interactions.

**Optional Use Cases (Nice-to-Have)**

- **Voice Command Support** – Hands-free interaction for accessibility & speed.
- **Emotion-Based UI Customization** – Change UI themes or responses based on detected user mood.
- **Advanced Predictive Analytics** – Forecast trends or outcomes using AI models.
- **Multi-Platform Support** – Responsive design or mobile app extension.

---

### **3. Actor Mapping**

| Use Case                   | Actors                       | Triggers                       | Outcomes                           |
| -------------------------- | ---------------------------- | ------------------------------ | ---------------------------------- |
| AI Chat Assistant          | End User, Backend API        | User enters query in chat      | Relevant answer/solution provided  |
| Smart Data Extraction Tool | End User, Parsing Engine     | User uploads file/document     | Structured data output returned    |
| Analytics Dashboard        | End User, Database           | User accesses dashboard        | Visualized reports shown           |
| User Account System        | User, Authentication Service | Login/Register form submission | Account created / logged in        |
| Voice Command Support      | User, Speech-to-Text API     | User issues voice command      | Task executed without manual input |

---

### **4. Resource & Data Requirements**

- **APIs**: **OpenAI** API, Google Vision/Tesseract OCR, [ChartJS](https://www.chartjs.org/) and [D3.JS](https://d3js.org/) for visualization
- **Data**: Sample datasets or dummy user inputs for demo
- **Tech Stack (Might Change)**:
    - **Frontend**: React + Tailwind CSS (fast UI dev)
    - **Backend**: Node.js + Express
    - **Database**: MongoDB (fast setup & flexible schema)

---

### **5. Clarification Points for Faculty**

- Any tech stack restrictions?
- Is internet access guaranteed during the hackathon?
- Do optional features give bonus marks?
- Are we allowed to use pre-trained AI models?

---
