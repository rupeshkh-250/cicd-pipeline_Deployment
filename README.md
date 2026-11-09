# 🚀 End-to-End CI/CD Pipeline Deployment

![GitHub Actions](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-green)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![Python](https://img.shields.io/badge/Python-3.11-yellow)
![Flask](https://img.shields.io/badge/Flask-2.3.3-red)

## 📌 Project Overview
Maine ek Flask App ke liye complete CI/CD Pipeline banaya hai. Jab bhi main code push karta hu, GitHub Actions automatically test karke Docker image build karta hai.

**Live Status:** ✅ Pipeline GREEN

**Repo Link:** https://github.com/rupeshkh-250/cicd-pipeline_Deployment

## 🛠️ Tech Stack Used
- **Language:** Python 3.11
- **Framework:** Flask 2.3.3
- **Container:** Docker
- **CI/CD:** GitHub Actions
- **Server:** Ubuntu

## ⚙️ How CI/CD Works? (End-to-End Flow)

1.  **Code Push:** Developer code likh ke GitHub pe push karta hai
2.  **Trigger:** `.github/workflows/deploy.yml` automatically start ho jata hai
3.  **Checkout:** GitHub Actions code ko checkout karta hai
4.  **Setup Python:** Python 3.11 setup hota hai
5.  **Install & Test:** Requirements install hote hai aur test run hota hai
6.  **Docker Build:** Dockerfile se Docker Image build hota hai
7.  **Success:** Sab pass hone pe Green Tick ✅ milta hai

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
