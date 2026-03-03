# VisionPilot – A Gemini-Powered Universal Visual Control Agent

VisionPilot is a multimodal AI agent that becomes the user’s hands on screen.

It observes screenshots, interprets UI visually using Gemini models via Vertex AI, and generates structured executable actions to automate workflows across any application — without relying on DOM or APIs.

---

##  Elevator Pitch

VisionPilot sees your screen, understands your intent, and takes action like a human — across any application.

---

##  What It Does

- Accepts screenshot input
- Interprets UI elements visually using Gemini 1.5
- Understands user intent in natural language
- Outputs structured JSON action plans
- Executes actions via browser or desktop automation
- Works without DOM access

Example instruction:

> “Log into Kaggle and open my latest notebook.”

VisionPilot:
1. Detects login button
2. Types credentials
3. Navigates dashboard
4. Opens notebook



##  Architecture

User Screen  
→ Screenshot Capture  
→ Cloud Run Backend  
→ Cloud Storage  
→ Vertex AI (Gemini Vision)  
→ Structured Action Plan  
→ Execution Engine (Playwright / Desktop Runtime)

---

##  Built With

- Python 3.11
- FastAPI
- Google GenAI SDK
- Gemini 1.5 
- Vertex AI
- Cloud Run
- Cloud Storage
- Playwright
- Docker

---

##  Repository Structure
visionpilot-gemini-agent/
│
├── backend/
│ ├── main.py
│ ├── gemini_agent.py
│ ├── action_executor.py
│ ├── schemas.py
│ └── requirements.txt
│
├── extension/
│
├── desktop_runtime/
│
├── infra/
│ └── deploy.sh
│
├── Dockerfile
└── README.md
