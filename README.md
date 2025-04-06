# 🤖 Automated Selection System Based on Personality Traits

A **smart hiring solution** built using **Flask + Machine Learning** to automate the initial candidate selection process based on **skills and personality traits**. Designed to streamline recruitment by evaluating resumes, testing personalities, and making data-driven decisions — all from a user-friendly web interface.

---

## 🌟 Key Features

### 1. 🌐 Web Application
- Built with **Flask** for a smooth user experience.
- Two types of candidate flows:  
  - 🧑‍🎓 *Junior*  
  - 👩‍💼 *Experienced*
- Secure **Sign Up** and **Login**.
- Candidates upload their **resume** and submit details for evaluation.

---

### 2. 📄 Resume Processing
- Utilizes **PyMuPDF (fitz)** and **Regular Expressions** to extract:
  - 📘 **Educational Qualifications**
  - 🛠️ **Skills**
- Matches extracted data against **predefined keywords** to map competencies.

---

### 3. 🧠 Candidate Assessment

#### ✅ Skill Competency
- Modeled using **Linear Regression** to score candidates on relevant skill areas.

#### 🧪 Personality Evaluation
- Based on the **Big Five Personality Traits**:
  - Openness  
  - Conscientiousness  
  - Extroversion  
  - Agreeableness  
  - Neuroticism  
- Assessed using a **Random Forest Classifier**.

---

### 4. 🗃️ Data Storage
- Candidate data is logged and organized into:
  - `candidate0.csv` → *Junior candidates*  
  - `candidate.csv` → *Experienced candidates*  
  - `final_candidate_dataset0.csv` → *Selected candidates*

---

### 5. 📬 Email Notifications
- **Automated email system** informs selected candidates.
- Emails are:
  - 🔒 Securely sent  
  - 🎯 Personalized  
  - ✅ Triggered based on selection criteria

---

### 6. ⚙️ Selection Logic
- Selection is based on **customizable thresholds** for:
  - Personality fit
  - Skill competency score
- Only candidates who meet both criteria are shortlisted.

---

### 7. 📈 Machine Learning Models
| Purpose            | Model Used             |
|--------------------|------------------------|
| Skill Assessment   | Linear Regression       |
| Personality Fit    | Random Forest Classifier|

Both models are trained to make accurate predictions on candidate suitability.

---

### 8. 🚀 Scalability & Extensibility
- Easily extensible for:
  - New job roles or departments
  - More nuanced resume parsing
  - Integration with HRMS/ATS platforms
- Modular structure supports threshold adjustments and future AI enhancements.

---

## 📦 Folder Structure

bash

├── app/

│   ├── templates/         # HTML templates (login, dashboard, etc.)

│   ├── static/            # CSS, JS, images

│   ├── models/            # ML models (regression.pkl, classifier.pkl)

│   ├── utils/             # Resume parser, personality scorer

│   ├── routes.py          # Flask routes and views

│   └── app.py             # Main Flask application

├── data/

│   ├── candidate0.csv

│   ├── candidate.csv

│   └── final_candidate_dataset0.csv

├── ml/

│   ├── train_models.py    # Training scripts

│   └── models.pkl

├── requirements.txt

├── README.md


---

## ✅ Tech Stack

- **Frontend:** HTML5, CSS3, Bootstrap  
- **Backend:** Python, Flask  
- **ML Models:** scikit-learn  
- **Resume Parsing:** PyMuPDF (fitz), RegEx  
- **Email Service:** smtplib  
- **Data Format:** CSV  

---


## 📈 Future Enhancements

- 📄 OCR-enabled resume processing (PDF/Word/Images)
- 🧬 NLP-based skill extraction using spaCy/BERT
- 📉 Dashboard analytics for recruiters (Power BI/Tableau)
- 🔁 Integration with job boards (LinkedIn, Indeed)
- 🔐 Role-based recruiter panel for shortlisting and feedback

---

## 📢 License

This project is licensed under the [MIT License](LICENSE).

---
