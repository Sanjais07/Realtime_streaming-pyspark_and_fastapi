# 🏥 SNR Hospitals Real-Time Booking and Analytics Dashboard

## 👨‍💻 Project By
- **Sanjai S**

## 📌 Abstract
In modern healthcare environments, efficient room availability management is vital. This project implements a **real-time hospital room booking and monitoring dashboard** using:

- **FastAPI** (Backend Server)
- **Streamlit** (Interactive Dashboard)
- **Apache Spark** (Real-Time Analytics)

The system provides:
- Live room status updates
- Manual booking through the dashboard
- Real-time analytics of booking activities

Its lightweight, real-time architecture makes it adaptable for real-world hospital scenarios.

---

## 📖 Table of Contents
1. [Introduction](#introduction)
2. [Background Study](#background-study)
3. [Problem Statement](#problem-statement)
4. [Gaps Identified](#gaps-identified)
5. [Materials and Methods](#materials-and-methods)
6. [Experiment and Results](#experiment-and-results)
7. [Conclusion and Future Work](#conclusion-and-future-work)
8. [References](#references)

---

## 🩺 Introduction
Hospitals require dynamic bed/room availability tracking. Traditional systems lack real-time interactivity. This system offers:
- Live updates from a backend server
- Manual booking capability
- Booking activity history
- Real-time data analytics

---

## 📚 Background Study
Technologies used:
- ⚡ **FastAPI** – Lightweight API server
- 📊 **Streamlit** – Interactive dashboard UI
- 🔥 **Apache Spark** – Fast real-time analytics engine

Modern microservice-based design allows easy deployment and maintenance, unlike older monolithic systems.

---

## ❓ Problem Statement
**Design and implement a lightweight, real-time, interactive hospital room management system** that supports:
- Live room status monitoring
- Manual room booking
- Historical activity logging
- Real-time analytics

---

## 🕳️ Gaps Identified
Existing systems face issues like:
- No real-time updates
- Non-intuitive interfaces
- Heavy deployment requirements
- Poor analytics
- No manual override for bookings

**This project solves these using modern, lightweight technologies.**

---

## 🧪 Materials and Methods

### 🔧 Tools & Technologies
- **FastAPI** – Backend server
- **Streamlit** – Web dashboard
- **Apache Spark** – Real-time analytics
- **Python 3**
- **Ubuntu 22.04 (VirtualBox)**

### 🏗️ System Architecture

| Component | Description |
|----------|-------------|
| `hospital_server.py` | FastAPI backend serving random room booking updates |
| `hospital_client.py` | Streamlit frontend dashboard for monitoring & booking |
| `hospital_spark_analytics.py` | Spark script analyzing booking data in real-time |

### 🔁 Methodology
- FastAPI sends room booking updates every few seconds
- Streamlit client:
  - Fetches and displays live data
  - Allows manual bookings via sidebar form
  - Tracks all updates (auto & manual) with timestamps
- Spark script performs live string analysis on updates

---

## 🔍 Experiment and Results

### 🧪 Setup
- OS: Ubuntu 22.04 (VirtualBox)
- Python 3.10
- Commands to run:
  ```bash
  uvicorn hospital_server:app --reload
  streamlit run hospital_client.py
  python3 hospital_spark_analytics.py

## Output:
![Screenshot 2025-04-27 232724](https://github.com/user-attachments/assets/5d18dfdd-b139-46ec-9c39-483b2199c0b8)
![Screenshot 2025-04-27 232738](https://github.com/user-attachments/assets/bbb14475-614e-4f0d-98d2-01676768e266)
![Screenshot 2025-04-27 232818](https://github.com/user-attachments/assets/741f0240-fc10-4db2-b868-911708447a07)
![Screenshot 2025-04-27 232838](https://github.com/user-attachments/assets/62014bfd-8fbd-4ad0-be69-1e7bef82e929)
![Screenshot 2025-04-27 232852](https://github.com/user-attachments/assets/cd9a35d5-c47d-43fe-86ce-de4eb4e840ca)
![Screenshot 2025-04-27 232906](https://github.com/user-attachments/assets/be39372b-b7d6-4abe-b524-fc54196169a4)





