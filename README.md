# 📊 **Data Warehousing Final Project**
**Analysis of Student Performance Factors in Education Data Mart**

**Contributors:**  
Advith Reddy Kunda, Neshma Kasamneni, Purna Chandra Shekar Reddy Gosala,  
**Raajitha Sai Bondada**, Sai Anirudh Mantha, Shyam Rishi Kashyap Sai Kalaparthy

---

## 📁 **Project Overview**
This project presents a dimensional data warehouse solution for analyzing factors that influence student performance. Using educational data from Kaggle, we built a **student performance data mart** integrating data for Math and Portuguese courses. The system supports multidimensional analytics, enabling insights across student demographics, attendance, school types, and academic outcomes.

---

## 📂 **Directory Structure**
├── README.md # Project documentation
├── ERD.png # Entity Relationship Diagram (optional)
├── data/
│ ├── student-mat.csv # Math dataset
│ └── student-por.csv # Portuguese dataset
├── sql/
│ ├── create_tables.sql # SQL scripts to create staging, dimension, and fact tables
│ ├── etl_process.sql # Data transformation and ETL logic
│ └── analysis_queries.sql # SQL queries used for analysis and reporting
└── reports/
└── DW_Final_Project.pdf # Full project report with diagrams and findings

yaml
Copy
Edit

---

## 🗃️ **Data Sources**
- **Source:** [Kaggle – Student Performance Dataset](https://www.kaggle.com/datasets/larsen0966/student-performance-data-set)  
- **Files Used:**  
  - `student-mat.csv` – Math course data  
  - `student-por.csv` – Portuguese course data  

---

## 🛠️ **Tech Stack**
- **Database:** Oracle SQL Developer  
- **ETL:** SQL-based extraction and transformation  
- **Modeling:** Star schema (Fact and Dimension tables)  
- **Tools:** SQL, ERD, CSV preprocessing  

---

## 🧱 **Dimensional Model**

### 🔸 **Fact Table: `STUDENT_PERFORMANCE_FACT`**
Stores academic metrics:
- `G1`, `G2`, `G3` – Grades for each period
- `ABSENCES` – Number of school absences
- Foreign keys: `SCHOOL_ID`, `STUDENT_ID`, `COURSE_ID`, `TIME_ID`

### 🔸 **Dimension Tables**
- `DIM_SCHOOL` – School ID and name  
- `DIM_STUDENT` – Student demographics (sex, age, address, family size)  
- `DIM_COURSE` – Course name (Math or Portuguese)  
- `DIM_TIME` – Academic year or term  

---

## 🔄 **ETL Process**
- **Extraction:** CSV files loaded into staging tables  
- **Transformation:** Data cleaning, standardization, and assigning IDs  
- **Loading:** Inserts into fact and dimension tables using joins/unions

---

## 📈 **Analytical Objectives**
- Investigate impact of absences, gender, and family size on student performance  
- Compare performance across courses and schools  
- Support data-driven educational interventions and decisions  

---

## 🧪 **Sample SQL Analysis**
- Average final grade by course and school  
- Impact of absenteeism on performance  
- Student performance by gender and age  
- Correlation between G1, G2, and G3

---

## 📚 **References**
- Marjanovic, O. (2010) – Data-Driven Decision Making in Education  
- Romero & Ventura (2013) – Educational Data Mining  
- Baker & Inventado (2014) – Learning Analytics  
