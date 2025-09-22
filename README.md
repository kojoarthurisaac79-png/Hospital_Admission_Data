This project analyzes a hospital admission dataset using MySQL.
The goal is to practice SQL queries for real-world scenarios such as patient outcomes, disease conditions, comorbidities, and hospital resource use.

The dataset includes 14,620 rows with multiple clinical and demographic columns such as:
	•	Patient ID (Mrd_No)
	•	Admission & Discharge details (d.o.a, d.o.d, duration of year, duration of intensive unit stay)
	•	Demographics (age, gender, rural/urban)
	•	Clinical parameters (hb, tlc, glucose, urea, creatinine, bnp)
	•	Conditions (heart_failure, dm, htn, acs, stemi, aki, etc.)
	•	Outcomes (Discharged, Expiry, DAMA)



	•	Practice SQL fundamentals and intermediate queries.
	•	Explore real-world hospital dataset analysis.
	•	Answer common business-style questions like:
	•	Which gender had more admissions?
	•	What is the average age of admitted patients?
	•	How many patients were admitted with heart failure?
	•	What is the outcome distribution of patients (Discharged, Expired, DAMA)?
	•	What is the average ICU stay by outcome?



 Tools Used
	•	MySQL Workbench – to run SQL queries
	•	GitHub Desktop – for version control
	•	VS Code – to view/edit .sql files

SELECT COUNT(*) AS total_admissions
FROM hdhi_admission_data;

SELECT gender, COUNT(*) AS total
FROM hdhi_admission_data
GROUP BY gender;

SELECT COUNT(*) AS heart_failure_cases
FROM hdhi_admission_data
WHERE heart_failure = 1;

Insights from Queries
	•	Total admissions: 14,620
	•	Most patients admitted were male
	•	Significant number of patients with hypertension & diabetes
	•	Discharged is the most common outcome
	•	ICU stay duration varies greatly based on outcome


This project is part of my SQL learning journey. Feedback and suggestions are welcome!
