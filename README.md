# AI Lead Qualifier Bot (n8n + Gemini)

An automated AI-driven lead scoring workflow built using Google Forms, Sheets, n8n, and Google Gemini (via API). Classifies leads as **Hot**, **Warm**, or **Cold**, and writes the result back to Google Sheets.

---

## 🔧 Tech Stack

- 🧠 Google Gemini (LLM API)
- 📝 Google Forms + Google Sheets
- ⚙️ n8n (Open Source Automation Tool)
- 🧾 REST API, JSON, Regex

---

## 📈 Workflow Overview

1. ✅ Lead submits Google Form  
2. ✅ Form is connected to Google Sheets  
3. ✅ n8n Trigger detects new row  
4. ✅ Gemini receives form data and replies with classification  
5. ✅ Function Node extracts score and lead level  
6. ✅ Original Google Sheet row is updated with:
   - `lead_score`: Full Gemini output
   - `lead_level`: Extracted value (Hot, Warm, Cold)

---

## 🧪 AI Prompt Example

> You are an AI lead qualifier. Analyze this lead's info:
>
> - Service: Automation / Bots  
> - Budget: £500–£1000  
> - Timeline: Immediately  
> - Message: I want an automatic chatbot.
>
> Classify this lead as Hot, Warm, or Cold. Explain your reasoning briefly.

---

## 💾 How to Deploy

1. Clone repo  
2. Import JSON into n8n  
3. Set up environment variables for API keys  
4. Connect Google Sheets + Gemini  
5. Activate workflow

---

## 📬 Future Upgrades

- Gmail alerts for Hot leads  
- CRM push (HubSpot, Notion, etc.)  
- GPT-based rewriter for follow-up emails  

---

## 👤 Built by Krrish Gupta  
Part of my automation portfolio. Feel free to fork or collaborate!
