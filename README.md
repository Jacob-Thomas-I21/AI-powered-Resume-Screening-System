**AI-Powered Resume Screening System**

**📌 Project Overview**
This project automates the resume screening process using Natural Language Processing (NLP) and Machine Learning (ML). The system extracts key information from resumes, ranks candidates based on job descriptions, and provides an AI-driven candidate shortlisting system.

**📊 Current Project Progress**

✅ Phase 1: Data Preprocessing (Completed)

 
 ✅ Step 1: Loaded Resume Dataset
 
 ✅ Step 2: Dropped Unnecessary Columns

 ✅ Step 3: Handled Missing Data

 ✅ Step 4: Cleaned Resume Text (Clean_Resume column)

 ✅ Phase 2: Feature Extraction (In Progress)

 ✅ Step 5: Tokenization & Stopword Removal

 ✅ Step 6: Skill Extraction (NER)
 
 ✅  Step 7: Convert Text to Numerical Vectors (TF-IDF / BERT) (Next)
 
 ⬜ Model Training & Resume Ranking (Upcoming)
 
 ⬜ API & Deployment (Final Phase)
 
**🚀 Features**

Resume Parsing – Extracts structured information from PDF & DOCX resumes.

Text Preprocessing – Tokenization, stopword removal, Named Entity Recognition (NER).

Skill Extraction – Identifies relevant skills (Python, Java, Machine Learning, etc.).

ML Model for Candidate Ranking – Uses TF-IDF/BERT embeddings to match resumes to job descriptions.

Web API & Dashboard – Built with FastAPI & Streamlit for real-world usability.

Deployment – Dockerized & deployable on AWS/GCP.

**📂 Project Structure**
resume-screening/
├── data/               # Sample resumes and job descriptions

├── models/             # Trained machine learning models

├── notebooks/          # Jupyter notebooks for experimentation

│   ├── data_processing.ipynb ✅ (Preprocessing, skill extraction & BERT embeddings)

│   ├── model_training.ipynb   # ML model training

│   ├── api_deployment.ipynb      # Deployment notebook

├── src/                # Source code

│   ├── preprocessing.py  # Text preprocessing scripts

│   ├── model.py         # ML model training & inference

│   ├── api.py           # FastAPI/Flask API

│   ├── dashboard.py      # Streamlit front-end

├── Dockerfile          # Docker containerization

├── requirements.txt     # Dependencies

├── README.md           # Project documentation

**Technologies Used**

Programming Language: Python

NLP Libraries: SpaCy, NLTK, Transformers (BERT)

Machine Learning: Scikit-learn, TensorFlow/PyTorch

Web Framework: FastAPI/Flask

Front-end: Streamlit

Deployment: Docker, AWS/GCP

**Installation & Setup**

📌**Prerequisites**

Python 3.8+
Virtual environment (optional but recommended)

Docker (if deploying in containers)

📌 **Step 1: Clone the Repository**

git clone https://github.com/yourusername/resume-screening.git

cd resume-screening

📌 **Step 2: Install Dependencies**

pip install -r requirements.txt

📌**Step 3: Run the Application**

**1️.Preprocess the Data**

python src/preprocessing.py

**2️.Train the Model**

python src/model.py

**3️.Start the API**

uvicorn src.api:app --reload

**4.Launch the Dashboard**


streamlit run src/dashboard.py

 **5.Docker Deployment**

docker build -t resume-screening .

docker run -p 8000:8000 resume-screening

**6.API Endpoints**

Method	Endpoint	Description

POST	/upload	Upload a resume for processing

GET	/rank	Retrieve ranked candidates

GET	/health	API health check

**Future Enhancements**

Integration with ATS (Applicant Tracking Systems)

Advanced resume similarity scoring using BERT-based embeddings

Real-time job recommendations based on candidate profiles

LLM-based Resume Analysis

**## License & Usage Restrictions**

 This project is NOT Open Source and is protected under a proprietary license.

**You are NOT allowed to:**

**Use, copy, modify, distribute, or resell this software without explicit permission from the author.
Train a competing AI model based on this repository.**

Permitted Uses (Only if you receive written approval):

Research and academic purposes.
Enterprise use with a purchased license.

For licensing inquiries, contact:

Email: jacobtjoshy@gmail.com

GitHub:Jacob-Thomas-I21

 **Unauthorized use, reproduction, or modification of this project may result in legal action.**

**Legal Notice**

This project is protected under international copyright laws.

Any unauthorized commercial use, reselling, or redistribution is strictly prohibited.
