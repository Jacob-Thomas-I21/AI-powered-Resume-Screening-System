# AI-Powered Resume Screening System

## 📌 Project Overview
This project automates the resume screening process using Natural Language Processing (NLP) and Machine Learning (ML). The system extracts key information from resumes, ranks candidates based on job descriptions, and provides an AI-driven candidate shortlisting system.

---

## 📊 Current Project Progress

✅ Phase 1: Data Preprocessing (Completed)

✅ Step 1: Loaded Resume Dataset  
✅ Step 2: Dropped Unnecessary Columns  
✅ Step 3: Handled Missing Data  
✅ Step 4: Cleaned Resume Text (Clean_Resume column)

✅ Phase 2: Feature Extraction (Completed)

✅ Step 5: Tokenization & Stopword Removal  
✅ Step 6: Skill Extraction (NER)  
✅ Step 7: Convert Text to Numerical Vectors (SBERT)  

✅ Model Training & Resume Ranking (Completed)  
✅ API & Deployment (In Progress)

---

## 🚀 Features

✅ Resume Parsing – Extracts structured information from PDF & DOCX resumes.  
✅ Text Preprocessing – Tokenization, stopword removal, Named Entity Recognition (NER).  
✅ Skill Extraction – Identifies relevant skills (Python, Java, Machine Learning, etc.).  
✅ AI Model for Candidate Ranking – Uses SBERT embeddings + MLP + XGBoost to match resumes to job descriptions.  
✅ Deployment Ready – Prepares FastAPI service for real-time predictions.  

---

## 📂 Project Structure

resume-screening/ 

├── data/ # Sample resumes and job descriptions 

├── models/ # Trained machine learning models

├── notebooks/ # Jupyter notebooks for experimentation

│ ├── data_processing.ipynb ✅ (Preprocessing, skill extraction & SBERT embeddings)

│ ├── model_training.ipynb # ML model training

│ ├── api_deployment.ipynb # Deployment notebook

├── src/ # Source code 

│ ├── preprocessing.py # Text preprocessing scripts

│ ├── model.py # ML model training & inference

│ ├── api.py # FastAPI API 

│ ├── dashboard.py # Streamlit front-end 

├── Dockerfile # Docker containerization

├── requirements.txt # Dependencies

├── README.md # Project documentation


---

## **Technologies Used**

✅ Programming Language: Python  
✅ NLP Libraries: SpaCy, NLTK, Sentence Transformers  
✅ Machine Learning: Scikit-learn, TensorFlow, XGBoost  
✅ Deployment: FastAPI, Docker, AWS/GCP

---

## 📌 Installation & Setup

### **Prerequisites**
- Python 3.8+
- Virtual environment (optional but recommended)
- Docker (if deploying in containers)

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/yourusername/resume-screening.git
cd resume-screening

Step 2: Install Dependencies

pip install -r requirements.txt

📌 New Process - Add/Change Job Description
🆕 Adding or Updating Job Description

    Run the new script:

    python update_job_description.py

    Paste the new job description when prompted.
    This will: ✅ Save job_description.csv
    ✅ Precompute & save job_embedding.npy
    ✅ Precompute & save job_skills.pkl

🔄 What to Do After Updating Job Description?

    Re-run Data Preprocessing for All Resumes:

python data_preprocessing,_skill_extraction_&_sbert_embeddings.py

Retrain the Models:

    python resume_match_deployment.py

📌 Process for New Resumes (Same Job Description)

    Add new resumes to your folder.
    Re-run:

    python data_preprocessing,_skill_extraction_&_sbert_embeddings.py
    python resume_match_deployment.py

📌 Process for New Resumes (Single Prediction After Deployment)

    After deployment, if a single new resume arrives, you don’t need to retrain the entire model.
    Use:

    python predict_resume_match.py /path/to/new_resume.pdf

    This loads existing models and gives a result immediately.

📌 Running the API

Once fully trained and processed, you can run:

uvicorn api:app --reload

This serves the AI as a REST API for real-time predictions.
📌 License & Usage Restrictions

This project is NOT Open Source and is protected under a proprietary license.

You are NOT allowed to:

    Use, copy, modify, distribute, or resell this software without explicit permission from the author.
    Train a competing AI model based on this repository.

Permitted Uses (Only if you receive written approval):

    Research and academic purposes.
    Enterprise use with a purchased license.

For licensing inquiries, contact:

    Email: jacobtjoshy@gmail.com
    GitHub: Jacob-Thomas-I21

Unauthorized use, reproduction, or modification of this project may result in legal action.

Legal Notice This project is protected under international copyright laws.
Any unauthorized commercial use, reselling, or redistribution is strictly prohibited.
**Legal Notice**

This project is protected under international copyright laws.

Any unauthorized commercial use, reselling, or redistribution is strictly prohibited.
