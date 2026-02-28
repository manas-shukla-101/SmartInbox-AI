# ⚡ SmartInbox AI: The Intelligent Email Gatekeeper

![GitHub stars](https://img.shields.io/github/stars/your-username/repo-name?style=for-the-badge&color=ffd700)
![GitHub forks](https://img.shields.io/github/forks/your-username/repo-name?style=for-the-badge&color=808080)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)
![Built with Python](https://img.shields.io/badge/Built%20with-LangFlow-blue?style=for-the-badge&logo=python)
![LLM](https://img.shields.io/badge/LLM-GPT--4o-orange?style=for-the-badge&logo=openai)
![Security](https://img.shields.io/badge/Security-Human--in--the--Loop-red?style=for-the-badge)

---

## 🌪️ The Problem
We receive **120+ emails daily**. 80% are noise. Traditional filters are "dumb"—they either miss sophisticated phishing or accidentally archive important client communications.

## 💡 The Solution: SmartInbox AI
An autonomous **Human-in-the-Loop (HITL)** orchestration that uses LLMs to think like a personal assistant. It doesn't just filter; it **reasons** through content to determine intent.

### 🛠️ The Tech Stack
* **Orchestration:** LangFlow / Flowise (LLM Workflow Builder)
* **Brain:** OpenAI GPT-4o Model
* **Integrations:** Gmail API (OAuth 2.0)
* **Logic:** Custom JSON Output Parsing & Conditional Routing

---

## 🎮 Live Visual Workflow

<div align="center">
  <img src="YOUR_GIF_OR_IMAGE_LINK_HERE" alt="Project Workflow Demo" width="900" style="border-radius: 10px; border: 2px solid #555;">
  <p><i>Real-time execution of the AI Agent analyzing and routing incoming traffic.</i></p>
</div>

---

## 🧠 Strategic Logic Flow

### 1. Ingestion & Analysis
The flow triggers on every new Gmail thread. The **Spam Analyzer Agent** extracts the intent, urgency, and sender credibility.

### 2. The Decision Engine
Using a **Routing Node**, the system forks into three distinct outcomes based on the AI's classification:

| Outcome | Action taken | Security Level |
| :--- | :--- | :--- |
| **🚨 Spam** | Prepares deletion message & **waits for human approval**. | High |
| **✅ Legitimate** | Marks as Read + Triggers an AI-generated draft reply. | Low |
| **⚠️ Fallback** | Keeps in Inbox for manual review (Safety Net). | Critical |

### 3. The "Human-in-the-Loop" Edge
Unlike basic scripts, this project features a **Wait for Approval** node. This demonstrates an understanding of **Enterprise AI Safety**—ensuring the AI never performs a destructive action (deletion) without a final human confirmation.

---

## 🚀 Quick Start (Importing the Flow)

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/manas-shukla-101/SmartInbox-AI.git](https://github.com/manas-shukla-101/SmartInbox-AI.git)
   ```
2. **Import JSON Configuration:**
   - Open your dashboard (LangFlow/Flowise).
   - Click Upload/Import and select the [SmartInbox AI](SmartInbox AI.json) file.
