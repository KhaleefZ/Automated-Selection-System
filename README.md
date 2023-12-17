# Automated-Selection-System- Based on Personality Traits

This project is an automated selection system for candidates based on their skills and personality traits. The system involves a web application built using Flask, where candidates can sign up, log in, and submit their details, including a resume. The system analyzes the resume to extract skills and education information.

Key Components:

1. *Web Application:*
   - Users can sign up and log in.
   - Two types of candidates are considered: junior and experienced.
   - Candidates submit their details, including a resume.

2. *Resume Processing:*
   - Resumes are processed to extract skills and education information using PyMuPDF (fitz) and regular expressions.
   - Skills and education keywords are predefined.

3. *Candidate Assessment:*
   - Candidates are assessed based on a personality test (Openness, Conscientiousness, Extroversion, Agreeableness, Neuroticism).
   - Skill competency is evaluated.

4. *Data Storage:*
   - Candidate data is stored in CSV files (candidate0.csv and candidate.csv for junior and experienced candidates, respectively).

5. *Automated Hiring:*
   - Linear Regression is used to assess skill competency.
   - Random Forest Classifier is used to assess personality.
   - A threshold-based approach is employed for hiring decisions.

6. *Email Notifications:*
   - Successful candidates receive email notifications.
   - The emails are personalized and inform candidates about their selection for the next round.

7. *Scalability and Extension:*
   - The project supports both junior and experienced candidate types.
   - The selection criteria can be adjusted by modifying thresholds or incorporating additional features.

8. *Machine Learning Models:*
   - Linear Regression for skill competency assessment.
   - Random Forest Classifier for personality assessment.

9. *Final Results:*
   - Successful candidates are recorded in the final_candidate_dataset0.csv file.
   - Email notifications are sent to hired candidates.

Note: This project aims to automate the initial candidate selection process based on a combination of skills and personality assessments. The code demonstrates how to implement a web application, integrate resume processing, apply machine learning models for assessment, and notify candidates about their selection results.
