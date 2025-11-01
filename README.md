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
---

## Running the App

1) Ensure `trained_prompts_mc.csv` exists at:

   data/trained_prompts_mc.csv

2) Install packages:
   pip install -r requirements.txt

3) Run:
   python app.py

---
## Team 6 Prime — Contributors

| Member        | Role                                   |
|---------------|----------------------------------------|
| **Nathan**     | ML Pipeline / Backend Development      |
| **Bharath**    | ML + Rules Integration / Implementation |
| **Gokulan**    | System Integration + Quality Control   |
| **Krishnalaya**| Frontend + Visualisation               |
| **Keerthi**    | Data Analytics + Prompt Engineering    |
| **Gabel Nibu** | Documentation + Data Management        |



> Code development was led by **Nathan & Bharath**, while other members supported dataset creation, annotation, UI & documentation.

## Future Work

Plans for improvement include:
1) Expand labelled dataset for better generalisation
2) Experiment with additional classifiers
3) Explore transformer embeddings (e.g., SBERT)
4) Build larger keyword dictionary
5) Improve country-wise data balance
6) Multi-annotator agreement integration
7) Improve linguistic rule-based patterns and contextual cues

---

