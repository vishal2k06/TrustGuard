# TrustGuard

## Privacy-First Identity Trust Framework for Secure Digital Banking

### Overview

TrustGuard is a risk-based identity trust platform designed to strengthen digital banking security by continuously validating user identities throughout a session. Unlike traditional authentication methods that verify users only during login, TrustGuard continuously evaluates contextual and behavioral signals to detect suspicious activities and trigger adaptive authentication only when required.

The solution primarily focuses on preventing **Account Takeover (ATO)** while also addressing risks associated with **new device usage, behavioral anomalies, and suspicious account recovery attempts**.

---

## Problem Statement

Modern banking systems are increasingly vulnerable to identity-based attacks due to stolen credentials, unauthorized devices, and abnormal user behavior. Static authentication methods such as passwords and OTPs are often insufficient to detect these threats in real time.

TrustGuard aims to provide a privacy-first, continuous identity verification framework that enhances security while maintaining a seamless user experience.

---

## Proposed Solution

TrustGuard continuously monitors:

- Login behavior
- Device information
- Login location
- Account recovery requests
- User activity patterns

These signals are processed to generate a **Trust Score** for every user session.

The platform also maintains an **Identity Trust Graph** that maps relationships between users, devices, IP addresses, and account activities to identify suspicious patterns and potential account takeover attempts.

Based on the calculated Trust Score, the system performs adaptive authentication:

- Low Risk → Access Granted
- Medium Risk → OTP Verification
- High Risk → Additional Verification
- Critical Risk → Block Access & Generate Alert

---

## Key Features

- Continuous Identity Validation
- Dynamic Trust Score Calculation
- Identity Trust Graph
- Adaptive Authentication
- New Device Detection
- Behavioral Risk Analysis
- Suspicious Account Recovery Detection
- Security Monitoring Dashboard

---

## Workflow

1. User initiates login or account recovery.
2. Device and contextual information are collected.
3. Trust Score is calculated.
4. Identity Trust Graph analyzes relationships.
5. Risk level is determined.
6. Adaptive authentication is triggered.
7. Security dashboard displays alerts and logs.

---

## Technology Stack

### Frontend
- Next.js
- React
- Tailwind CSS

### Backend
- FastAPI
- Python

### Database
- PostgreSQL

### Graph Analysis
- NetworkX (Prototype)
- Neo4j (Future Scope)

### Security & Analytics
- JWT Authentication
- Isolation Forest
- Rule-Based Risk Engine

### Deployment
- Docker

---

## Project Structure

```
trustguard/
│
├── frontend/
├── backend/
├── docs/
├── README.md
└── requirements.txt
```

---

## Current Status

This repository contains the initial project architecture and documentation prepared for the **PSB Hackathon Series 2026 – Cybersecurity & Fraud Domain**.

The prototype implementation is currently under development.

---

## Future Enhancements

- Machine Learning-based Trust Score
- Real-time Fraud Detection
- Advanced Identity Graph Analytics
- Explainable Risk Analysis
- Enterprise Security Dashboard
- Multi-channel Banking Integration

---

## Team

**Team Name:** Inglorious

### Members

- Vishal M
- Team Member 2

---

## License

This project is developed for the **PSB Hackathon Series 2026** as an academic prototype.
