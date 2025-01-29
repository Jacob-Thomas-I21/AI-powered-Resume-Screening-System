**AI-Powered Resume Screening System**

📌 **Project Overview**

This project automates the resume screening process using Natural Language Processing (NLP) and Machine Learning (ML). The system extracts key information from resumes, ranks candidates based on job descriptions, and provides an AI-driven approach to hiring efficiency.

🚀 **Features**

Resume Parsing: Extracts structured information from PDF and DOCX resumes.

Text Preprocessing: Tokenization, stopword removal, Named Entity Recognition (NER).

Machine Learning Model: Classifies and ranks candidates based on job descriptions.

Web API: FastAPI/Flask-based API for integration with HR systems.

Streamlit Dashboard: User-friendly interface for resume uploads and ranking.

Deployment: Containerized with Docker and hosted on AWS/GCP.

## 📂 Project Structure

resume-screening/ 
├── data/               # Sample resumes and job descriptions 

├── models/             # Trained machine learning models 

├── notebooks/          # Jupyter notebooks for experimentation 

├── src/                # Source code 

│ ├── preprocessing.py  # Text preprocessing scripts 

│ ├── model.py          # ML model training and inference

│ ├── api.py            # FastAPI/Flask API 

│ ├── dashboard.py      # Streamlit front-end 

├── Dockerfile          # Docker containerization

├── requirements.txt    # Dependencies 

├── README.md           # Project documentation


📊**Technologies Used**

Programming Language: Python

NLP Libraries: SpaCy, NLTK, Transformers (BERT)

Machine Learning: Scikit-learn, TensorFlow/PyTorch

Web Framework: FastAPI/Flask

Front-end: Streamlit

Deployment: Docker, AWS/GCP

🛠️**Installation & Setup**

Prerequisites

Python 3.8+

Virtual environment (optional but recommended)

Docker (if deploying in containers)

Step 1: Clone the Repository

git clone https://github.com/yourusername/resume-screening.git
cd resume-screening

Step 2: Install Dependencies

pip install -r requirements.txt

Step 3: Run the Application

1. Preprocess the Data

python src/preprocessing.py

2. Train the Model

python src/model.py

3. Start the API

uvicorn src.api:app --reload

4. Launch the Dashboard

streamlit run src/dashboard.py

🐳 Docker Deployment

docker build -t resume-screening .
docker run -p 8000:8000 resume-screening

🔗**API Endpoints**

Method

Endpoint

Description

POST

/upload

Upload a resume for processing

GET

/rank

Retrieve ranked candidates

GET

/health

API health check

🛠️ **Future Enhancements**

Integration with ATS (Applicant Tracking Systems)

Advanced resume similarity scoring using BERT-based embeddings

Real-time job recommendations based on candidate profiles

🤝 **Contributing**

Pull requests are welcome! Please open an issue first to discuss major changes.

📜 **License**

This project is licensed under the MIT License.
