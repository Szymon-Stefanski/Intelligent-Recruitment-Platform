# Intelligent Recruitment Platform

## Project Vision
I'm creating this app for recruiters, especially from smaller companies that don’t have big HR systems.  
The goal is to make the recruitment process easier by automating some repetitive tasks like candidate matching.  
Right now, recruiters spend a lot of time reading resumes and trying to match them to job offers.  
My app will help by analyzing resumes, ranking candidates, and showing results in a simple dashboard.  
This way, recruiters can focus on talking to the best candidates instead of doing manual work.
I'm using Machine learning to help with matching candidates to job offers and ranking them automatically.

## Core Features (MVP)
- **Upload resumes** – recruiters can upload PDF or DOCX files.  
- **Analyze resumes** – extract skills, experience, and education.  
- **Match to job offers** – rank candidates according to how well they fit a job.  
- **Dashboard** – visualize candidates, scores, and job offers.  
- **Store data** – keep resumes and analysis results in a database.  

## System Architecture (High-Level)
- **Frontend** – React app for recruiters to upload resumes and view dashboard.  
- **Backend** – Django REST API handles uploads, stores data, and communicates with ML service.  
- **ML Service** – separate service that analyzes resumes and calculates matching scores.  
- **Database** – PostgreSQL stores resumes, job offers, and analysis results.  
- **Async tasks** – Celery handles long-running jobs like resume analysis.  
- **Communication** – frontend to backend via REST, backend to ML service via HTTP/async.  

## Engineering Principles
- Keep it simple stupid (KISS)  
- Don’t repeat yourself (DRY)  
- Test the important parts (testability)  
- Make it easy to scale (scalability)  
- Security basics (authentication, least privilege)  
- Separate concerns between components (separation of concerns)  
- Design APIs first (API-first / RESTful)  
