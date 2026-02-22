# 🚀 RIFT – AI-Powered Autonomous CI/CD Healing System

## 📌 Overview

RIFT is an AI-powered autonomous CI/CD healing system that detects pipeline failures, analyzes error logs using Large Language Models (LLMs), generates intelligent fixes, and automatically pushes corrections back to the GitHub repository.

It reduces manual debugging effort and accelerates DevOps workflows by enabling self-healing pipelines.

---

## 🎯 Problem Statement

CI/CD pipelines commonly fail due to:

* Syntax errors
* Dependency issues
* Docker build failures
* Misconfigured workflows
* Runtime exceptions

Manual debugging consumes time and delays deployments.

RIFT automates detection, diagnosis, and resolution of such failures.

---

## 🧠 How It Works

1. Detects CI/CD pipeline failure
2. Collects and parses error logs
3. Sends logs to an LLM for reasoning
4. Generates corrected code or configuration
5. Creates a new branch
6. Commits the fix
7. Pushes changes to GitHub

---

## 🏗️ Project Structure

```
RIFT/
│
├── backend/
│   ├── agents.py
│   ├── docker_runner.py
│   ├── git_utils.py
│   ├── llm_client.py
│   ├── main.py
│   └── requirements.txt
│
├── frontend-react/
│   ├── public/
│   ├── src/
│   └── package.json
│
├── electron-app/
│   ├── main.js
│   ├── preload.js
│   └── package.json
│
└── README.md
```

---

## ⚙️ Tech Stack

* Python (Backend)
* React (Frontend)
* Electron (Desktop integration)
* GitHub API
* Docker
* NVIDIA LLM API / Ollama (local fallback)

---

## 🔐 Environment Variables

Create a `.env` file in the root directory and add:

```
GITHUB_TOKEN=your_github_personal_access_token
NVIDIA_API_KEY=your_nvidia_api_key
NVIDIA_BASE_URL=https://integrate.api.nvidia.com/v1
NVIDIA_MODEL=mistralai/mixtral-8x22b-instruct-v0.1
OLLAMA_BASE_URL=http://localhost:11434
OLLAMA_MODEL=llama3
```

---

## 🚀 Installation & Setup

### 1️⃣ Clone Repository

```
git clone https://github.com/soniyashaik29/CI-CD.git
cd CI-CD
```

### 2️⃣ Backend Setup

```
cd backend
pip install -r requirements.txt
python main.py
```

### 3️⃣ Frontend Setup

```
cd frontend-react
npm install
npm start
```

### 4️⃣ Electron App (Optional)

```
cd electron-app
npm install
npm start
```

---

## 🤖 Key Features

* Automated CI/CD failure detection
* AI-driven root cause analysis
* Intelligent fix generation
* Automatic branch creation and commit
* GitHub integration
* Docker-based testing
* Local LLM fallback support

---

## 🔮 Future Enhancements

* Automatic Pull Request creation
* Slack/Email notifications
* Multi-repository monitoring
* Kubernetes deployment support
* Advanced failure classification

---

## 📜 License

This project is currently not licensed.
All rights reserved by the repository owner.

---

## 👨‍💻 Author

Developed as part of the RIFT – Autonomous DevOps Intelligence System.

---

