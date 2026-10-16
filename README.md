# Cyber-Threat-Detection-Security-Assessment-Platform
Real-time AI-powered network intrusion detection platform for live traffic monitoring, threat classification, risk assessment, and security analysis.
# 🛡️ Cyber Threat Detection & Security Assessment Platform

A real-time AI-powered cybersecurity platform for monitoring network traffic, detecting potential cyber threats, classifying network attacks using Machine Learning, and assessing security risks.

## 🚀 Overview

The Cyber Threat Detection & Security Assessment Platform is designed to automatically monitor network traffic and identify suspicious or malicious activity.

The system captures live network packets, creates network flows, extracts traffic features, and uses a trained Machine Learning model to classify the traffic. Detection results are then analyzed for risk and displayed on a live monitoring dashboard.

### Main Workflow

Live Network Traffic
        ↓
Scapy Packet Capture
        ↓
Flow Creation
        ↓
77 Network Features
        ↓
Machine Learning Model
        ↓
Threat Classification
        ↓
Risk Assessment
        ↓
Detection Event Storage
        ↓
FastAPI Backend
        ↓
Live Streamlit Dashboard

## ✨ Features

- 🔴 Real-time network traffic monitoring
- 📡 Automatic packet capture using Scapy
- 🔄 Network flow generation and analysis
- 📊 Extraction of 77 network traffic features
- 🤖 Machine Learning-based threat classification
- 🧠 Multiclass attack detection
- ⚠️ Risk-level assessment
- 💾 Automatic detection event logging
- 🚀 FastAPI REST API
- 🖥️ Live Streamlit dashboard
- 📈 Real-time detection statistics
- 📂 Optional CSV-based testing
- 🔍 Security assessment functionality
- 📄 Detection and security reports

## 🤖 Machine Learning

The platform uses a trained Random Forest multiclass classification model for network traffic classification.

The model works with 77 network-flow features.

### Supported Traffic / Attack Classes

- Benign
- Bot
- DDoS
- DoS GoldenEye
- DoS Hulk
- DoS Slowhttptest
- DoS slowloris
- FTP-Patator
- Heartbleed
- Infiltration
- PortScan
- SSH-Patator
- Web Attack – Brute Force
- Web Attack – SQL Injection
- Web Attack – XSS

> Model confidence represents the model's confidence in its classification. It should not be interpreted as a guaranteed probability that an attack is occurring.

## 🏗️ Project Structure

```text
IDS_Project/
│
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   │
│   ├── api/
│   │   ├── monitoring.py
│   │   ├── detection.py
│   │   ├── assessment.py
│   │   └── reports.py
│   │
│   ├── core/
│   │   └── risk_engine.py
│   │
│   ├── services/
│   │   ├── model_service.py
│   │   ├── feature_extractor.py
│   │   ├── traffic_monitor.py
│   │   └── security_scanner.py
│   │
│   └── data/
│       └── events.json
│
├── frontend/
│   └── app.py
│
├── ml/
│   ├── model_loader.py
│   └── detection.py
│
├── models/
│   └── ids_project_multiclass_model.pkl
│
├── dataset/
├── notebooks/
├── reports/
├── logs/
├── tests/
│
├── requirements.txt
├── .gitignore
└── README.md
