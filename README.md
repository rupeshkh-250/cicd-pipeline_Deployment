I built a complete CI/CD Pipeline for a Flask App. Whenever I push code, GitHub Actions automatically tests it and builds a Docker image.

**Live Status:** ✅ Pipeline GREEN

**Repo Link:** https://github.com/rupeshkh-250/cicd-pipeline_Deployment

## 🛠️ Tech Stack Used
- **Language:** Python 3.11
- **Framework:** Flask 2.3.3
- **Container:** Docker
- **CI/CD:** GitHub Actions
- **Server:** Ubuntu

## ⚙️ How CI/CD Works? (End-to-End Flow)
1.  **Code Push:** Developer writes code and pushes it to GitHub
2.  **Trigger:** `.github/workflows/deploy.yml` starts automatically
3.  **Checkout:** GitHub Actions checks out the code
4.  **Setup Python:** Python 3.11 is set up
5.  **Install & Test:** Requirements are installed and tests are run
6.  **Docker Build:** Docker Image is built from the Dockerfile
7.  **Success:** If everything passes, we get a Green Tick ✅

## 📁 Project Structure

cicd-pipeline_Deployment/
├── app.py
├── requirements.txt
├── Dockerfile
└── .github/
    └── workflows/
        └── deploy.yml
        
## 🐛 Errors I Fixed (Real Learning)
I faced 3 major errors in this project, which I fixed myself:

1.  **Python Version Error:** Python 3.9 is not supported on Ubuntu 26.04, so I upgraded to Python 3.11.
2.  **Flask / Werkzeug Mismatch:** Flask 2.0.3 was not compatible with the installed Werkzeug version, so I upgraded to Flask 2.3.3.
3.  **Dockerfile Not Found:** Windows had saved the file as `Dockerfile.txt`, so Docker could not find it. I removed the `.txt` extension and renamed it to `Dockerfile`.

## 🎯 What I Learned
- How an End-to-End CI/CD Pipeline works
- How to automate builds using GitHub Actions
- How to build a Docker Image from a Dockerfile
- How to debug and fix real production errors
