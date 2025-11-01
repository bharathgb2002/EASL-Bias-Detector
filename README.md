# EASL-LLM Bias Detector
A hybrid Machine Learning + Rule-based system to identify, classify and visualise bias in Large Language Model (LLM) responses.

This project was developed as part of CSE5PM — Assessment 3 at La Trobe University (Team: *6 Prime*).

---

## Project Overview
Reducing biases in AI systems is critical to ensure fairness and trust.  
Our project builds an Extended Active Selection Loop (EASL) that:
1) Collects prompts
2) Generates model responses
3) Human-annotates & labels bias
4) Trains a hybrid AI + rules classifier
5) Visualises patterns in bias

This tool can evaluate multiple LLMs and compare their bias profiles.

---

## Features
✔ Multi-label bias classification  
✔ Binary flag — *Biased / Not biased*  
✔ Supports rule-based + ML hybrid prediction  
✔ Human-verified annotation integration  
✔ Country, category + severity logging  
✔ Gradio UI for easy interaction  
✔ Supports CSV upload + saving new logs  
✔ Extensible framework to test ANY LLM  

---

## Tech Stack
| Component | Technology |
|----------|------------|
| UI | Gradio |
| ML Model | Logistic Regression (TF-IDF) |
| Data Handling | Pandas, NumPy |
| Visualisation | Matplotlib, PCA |
| Extras | TextBlob (sentiment) |
| Language | Python |
---

## Repository Structure
``` 
├── app.py                      # Gradio application
├── requirements.txt            # Dependencies
├── data/
│   └── trained_prompts_mc.csv  # Final labelled prompts
├── README.md                   # Documentation
``` 
---

## Team 6 Prime — Contributors

| Member | Role |
|--------|------|
| **Nathan** | ML Pipeline / Backend development |
| **Bharath** | ML + Rules integration / Project implementation |
| **Gokulan** | System Intergrater + Quality control |
| **Krishnalaya** | Frontend + Visualization |
| **Keerthi** | Data Anlytics+ Prompt Engineering |
| **Gabel Nibu** | Documentation + Data|

> Code development was led by **Nathan & Bharath**, while other members supported dataset creation, annotation, UI & documentation.

---

