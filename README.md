# 🦁 BEAST SEVAI - PS-01
## Autonomous Tamil Voice Agent for E-Sevai

> A Tamil-first autonomous agent that converts a citizen's Tamil voice request
> into an automated E-Sevai application workflow.

### 🌐 Live Demo
https://beast-sevai-ps-01.vercel.app

### 💻 GitHub Repository
https://github.com/hidhayaafnan786-rgb/beast-sevai-ps-01

---

## 📌 Problem

Many Tamil-speaking citizens, especially in rural areas, face difficulties
using online government service portals because of language barriers and
complex application procedures.

Common challenges include:

- English-heavy online interfaces
- Difficulty understanding application steps
- Travel to nearby E-Sevai centres
- Long waiting times
- Additional assistance/form-filling charges
- Complex workflows for different certificates

---

## 💡 Solution

**BEAST SEVAI** is a Tamil-first autonomous agent designed to simplify
government certificate applications.

The user can simply say:

> "Enakku income certificate venum"

The system converts the voice request into an automated workflow:

**Tamil Voice → Intent Detection → Browser Automation → Verification
→ Form Filling → Human Confirmation → Payment → Document Delivery**

---

## 🚀 PS-01 Requirements Implemented

### 1. Browser Use ✅

Implemented using **Puppeteer** in `server.js`.

Capabilities include:

- Browser launch
- Portal navigation
- Automated form interaction
- Page navigation
- Screenshots
- Progress logging

### 2. MCP Servers ✅

The project includes MCP-based modules for:

- Tamil Voice / Speech-to-Text
- Payment processing
- WhatsApp document delivery

### 3. APIs & Connectors ✅

The architecture supports:

- Aadhaar verification
- E-Sevai services
- Payment gateway integration
- WhatsApp document delivery

> Note: Some integrations are implemented as mock/demo connectors and are
> structured to be replaced with production APIs.

### 4. Goal-to-Achievement Workflow ✅

```text
Tamil Voice Input
        ↓
Intent Planner
        ↓
Browser Automation
        ↓
Verification
        ↓
Automatic Form Filling
        ↓
Human Confirmation
        ↓
Payment
        ↓
Document Delivery

## 🧠 Progress & Human-in-Loop
- Progress Checker: Live green terminal logs on Vercel
- Auto-recovery: Retry logic on fail
- Human Confirmation: Required before ₹60 payment

## ▶️ How to Run
npm install
node server.js
Frontend: vercel --prod