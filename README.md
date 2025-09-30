🤖 Research Assistant – AI-Powered Knowledge Tool









---

Navigation Menu

Sign in

Code

Issues

Pull Requests

Actions

Projects

Wiki

Security

Insights



---

🌟 Overview

A full-stack AI-powered research assistant built with Spring Boot (backend) and a Chrome Extension (frontend) for simplifying research, summarization, and note management.

Java • Spring Boot • Chrome Extensions • AI API Integration • Docker


---

🌟 Key Features

Feature	Description

📚 Text Summarization	Generate concise summaries from long research text
💡 Suggestions & Insights	AI-powered recommendations for related topics
📝 Research Notes	Save, edit, and manage notes locally
🔍 Search & Filter	Quickly search across saved research data
⚡ Spring Boot Backend	REST APIs for AI integration & text processing
🎨 Frontend (Chrome Extension)	Side-panel UI for summarization and note-taking
🐳 Docker Ready	Containerized backend for easy deployment



---

📂 Repository Structure

Research-Assistant/
├── backend/ (Spring Boot API)
│   ├── controller/         # REST Controllers
│   ├── service/            # Business logic, AI integration
│   ├── model/              # DTOs and entities
│   └── ResearchAssistantApplication.java
│
├── frontend/ (Chrome Extension)
│   ├── manifest.json       # Extension configuration
│   ├── sidepanel.html      # UI for summarization & notes
│   ├── background.js       # Event handlers
│   ├── content.js          # Page integration
│   └── assets/             # Icons & static files
│
├── dockerfile              # Backend container config
├── docker-compose.yml      # Multi-service setup (optional)
└── README.md


---

🚀 Quick Start

1. Run Backend (Spring Boot API)

Option A: With Docker (Recommended)

git clone https://github.com/adityamanurkar/Research-Assistant-Springboot-Ai.git
cd Research-Assistant-Springboot-Ai
docker build -t research-assistant .
docker run -p 8080:8080 research-assistant

Option B: Local (Maven)

git clone https://github.com/adityamanurkar/Research-Assistant-Springboot-Ai.git
cd Research-Assistant-Springboot-Ai
mvn spring-boot:run

Backend available at 👉 http://localhost:8080


---

2. Run Frontend (Chrome Extension)

git clone https://github.com/adityamanurkar/Research-Assistant-Springboot-Ai-FrontEnd.git

1. Open Chrome → Extensions → Manage Extensions


2. Enable Developer mode


3. Click Load unpacked → Select cloned Research-Assistant-Springboot-Ai-FrontEnd folder


4. Open any webpage → Click extension → Summarize text or take notes!




---

📚 API Documentation

Base URL: http://localhost:8080/api/v1/

🔥 Core Endpoints

Summarization API

POST /api/v1/summarize
Body: { "text": "Long input text..." }
Response: { "summary": "Concise summary..." }

Suggestions API

POST /api/v1/suggest
Body: { "text": "Research topic..." }
Response: { "topics": ["Topic 1", "Topic 2", "Further reading..."] }

Health Check

GET /api/v1/health
Response: { "status": "UP" }


---

🏗️ Architecture

Research Assistant
├── Backend (Spring Boot)
│   ├── REST Endpoints
│   ├── AI Integration Service (LLM/Google API)
│   └── Optional persistence layer
└── Frontend (Chrome Extension)
    ├── Side Panel UI
    ├── Notes Management
    └── Summarization Trigger


---

🔧 Configuration

Environment Variables

Create a .env or add to system environment:

AI_API_KEY=your_api_key_here
SERVER_PORT=8080


---

🧪 Development & Testing

# Run unit tests
mvn test

# Build project
mvn clean package

Frontend testing is manual (via Chrome extension reload).


---

🤝 Contributing

We welcome contributions!

1. Fork & clone repo


2. Create feature branch

git checkout -b feature/amazing-feature


3. Commit changes & run tests


4. Open a pull request 🎉




---

📄 License

This project is licensed under the MIT License – see the LICENSE file.


---

🙏 Acknowledgments

Spring Boot

Chrome Extensions API

Google AI APIs



---

⭐ Star this repository if you find it useful!


---
