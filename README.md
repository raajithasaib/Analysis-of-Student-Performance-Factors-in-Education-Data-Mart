📊 Data Warehousing Final Project
Analysis of Student Performance Factors in Education Data Mart

Contributors:
Advith Reddy Kunda, Neshma Kasamneni, Purna Chandra Shekar Reddy Gosala,
Raajitha Sai Bondada, Sai Anirudh Mantha, Shyam Rishi Kashyap Sai Kalaparthy

📁 Project Overview
This project presents a dimensional data warehouse solution for analyzing factors that influence student performance. Using educational data from Kaggle, we built a student performance data mart integrating data for Math and Portuguese courses. The system supports multidimensional analytics, enabling insights across student demographics, attendance, school types, and academic outcomes.

📂 Directory Structure
text
Copy
Edit
├── README.md                # Project documentation
├── ERD.png                  # Entity Relationship Diagram (optional)
├── data/
│   ├── student-mat.csv      # Math dataset
│   └── student-por.csv      # Portuguese dataset
├── sql/
│   ├── create_tables.sql    # SQL scripts to create staging, dimension, and fact tables
│   ├── etl_process.sql      # Data transformation and ETL logic
│   └── analysis_queries.sql # SQL queries used for analysis and reporting
└── reports/
    └── DW_Final_Project.pdf # Full project report with diagrams and findings
🗃️ Data Sources
Source: Kaggle - Student Performance Dataset

Files Used:

student-mat.csv – Math course data

student-por.csv – Portuguese course data

🛠️ Tech Stack
Database: Oracle SQL Developer

ETL: Manual SQL-based extraction and transformation

Modeling: Star schema with fact and dimension tables

Tools: SQL, ERD modeling, data preprocessing in CSV format

🧱 Dimensional Model
Fact Table: STUDENT_PERFORMANCE_FACT
Stores academic metrics such as:

G1, G2, G3 (Grades)

Absences

Linked via foreign keys to School, Student, Course, and Time dimensions

Dimension Tables:
DIM_SCHOOL: School ID and name

DIM_STUDENT: Student demographic info (Sex, Age, Address, Family size)

DIM_COURSE: Course identifiers and names

DIM_TIME: Academic year mapping

🔄 ETL Process
Extraction: Raw CSV files loaded into staging tables

Transformation: Standardization, deduplication, course labeling

Loading: Data inserted into dimension and fact tables using SQL joins and unions

📈 Analytical Goals
Explore impact of demographics and attendance on student performance

Analyze performance across courses and schools

Support decision-making for targeted educational interventions

📊 Sample SQL Analysis Queries
Average grades by school

Impact of absences on final grades

Comparison between Math and Portuguese performance

Gender-based performance trends

📑 References
Marjanovic, O. (2010) – Data-driven decision making in education

Romero, C. & Ventura, S. (2013) – Educational data mining

Baker, R. S., & Inventado, P. S. (2014) – Predictive modeling in learning analytics
