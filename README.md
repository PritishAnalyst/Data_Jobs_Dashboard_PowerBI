<h1 align="center">Data Job Market Intelligence Dashboard</h1>

> Helping freshers and aspiring data professionals make smarter career decisions using real-world job data.

🎯 **Use Case:** Designed for students, career switchers, and job seekers new to data science—this dashboard answers the question:  
“What should I learn and which path pays off the most?”
<p align="center">
  <img src="assets\Dashboard 1 gif.gif" width="49%" />
  <img src="assets\Dashboard 2 gif.gif" width="49%" />
</p>

🗂️ **Dashboard File:** [Download Power BI File](/Data_Jobs_Dashboard_PowerBI.pbix) 


---

<h2 align="center"> 💡 What Problems Does This Dashboard Solve?</h2>


This dashboard was created to solve real struggles faced by **freshers and beginners in the data field**, such as:

- 🔎 **What are the top-paying roles in data?**  
  → Compare job titles by median yearly and hourly salary

- 🔎 **Which data jobs are most in demand?**  
  → See job count by role to identify hiring trends

- 🔎 **Which skills should I master to break into data?**  
  → View top in-demand high paying skills across job postings

- 🔎 **Where are these jobs located?**  
  → Use interactive maps and regional filters to spot high-opportunity zones

- 🔎 **Which platforms are best for finding data jobs?**  
  → Analyze hiring trends from job platforms like Indeed, LinkedIn, etc.


---

<h2 align="center">🔧 Data Process & Workflow</h2>


### 1. Data Preparation & ETL (Power Query)
- Imported real-world data on data-related job postings (titles, skills, salaries, regions, platforms, etc.)
- Cleaned and standardized columns to correct data types, handle blanks/nulls, and unify naming formats
- Created multiple **supporting dimension tables** using Power Query:
  - **Skill Table** for analyzing frequency of required skills
  - **Schedule Type Table** (e.g., Full Time, Internship, Contractor, etc.)
  - **Date Table** to support time intelligence (YTD trends, filters)
- Used **custom columns** and **conditional columns** to derive meaningful categories

<div style="display: flex; align-items: flex-start; gap: 20px;">

<!-- Text Section -->
<div style="flex: 1;">

### 2. Data Modeling (Power BI Data View)

- Designed a **star schema** with relationships between:
  - A central **Fact Table** (job postings)  
  - **Dimension tables** (skills, dates, schedule type, platforms, companies)
- Enforced referential integrity and optimized one-to-many relationships

</div>

<!-- Image Section -->
<div style="flex: 1;">
  <img src="assets\Screenshot 2025-07-19 115549.png" alt="Data Modeling Image" width="100%">
</div>

</div>


### 3. DAX & Measures
- Created a centralized **Measures Table** to maintain all calculated metrics
- Built advanced DAX measures for:
  - `Median Yearly Salary`, `Hourly Salary`, `Job Count`, `Skills per Job`
  - Percentage calculations: `% of Jobs`
- Used **CALCULATE**, **FILTER**, and **ALLSELECTED** to enable dynamic interactions in visuals

### 4. Parameterization
- Created **field parameters** and **numeric range parameters** to allow users to:
  - Toggle between salary metrics
  - Compare job count vs skill count


---

<h2 align="center">💡 Dashboard Pages Summary</h2>


### 📌 Page 1: Data Jobs Dashboard 

![Dashboard Preview](/assets/Power%20bi%20dashboard%201.png)


**Key Highlights:**
- **KPI Cards** for Job Count, Median Yearly & Hourly Salary, and Salary Rating
- **Line Chart** showing job count trends throughout 2024
- **Bar Chart** revealing the highest-paying job titles by median salary
- **Scatter Plot** comparing hourly vs. yearly salary across job roles
- **Interactive Table** listing Job Titles, Job Count, Median Salaries, and Job Trend mini-charts
- **Slicer** for selecting job titles
- **Drill-through Button** to jump to a job-specific deep-dive report

*Purpose: Quickly understand which roles dominate the market in terms of pay and volume, and how hiring fluctuates month-to-month.*

---

### 📌 Page 2: Job Title Drill Through

![Dashboard Preview](/assets/Job%20drill%20through%20dashboard.png)

This **contextual deep-dive page** gets triggered when a user selects a specific job title on Page 1.

**Key Highlights:**
- **Gauge Charts** for Yearly and Hourly Salary range of the selected role
- **Donut Charts** showing:
  - Work-from-home availability
  - Whether degree requirements or benefits are mentioned
- **Map Chart** for visualizing global job postings for the selected title
- **Bar Chart** of top hiring platforms
- **Treemap** showing distribution across different job schedule types

*Purpose: Help users analyze a specific role by understanding its salary range, job format, employer platforms, and global distribution.*

---

### 📌 Page 3: Data Jobs Dashboard 2.0 

![Dashboard Preview](/assets/Power%20bi%20dashboard%202.png)

**Key Highlights:**
- **KPI Cards** for Total Job Count, Average Skills per Job, Median Salaries
- **Bar Charts** showing:
  - Most in-demand skills (by Job Count or % share)
  - Salary comparison across job titles (Hourly or Yearly)
- **Toggle Buttons** to switch between:
  - Skill view: Job Count vs. Job Percentage
  - Salary view: Yearly vs. Hourly
- **Slicers** for job title and country selection
- **Clear Filter Button** for fast resets

*Purpose: Provide a quick-glance dashboard for users who want fast filtering and comparative analysis across roles and skills.*

---

---

## <h2 align="center">💡 Why It Matters ? </h2>

Many freshers are overwhelmed when entering the data world—they don’t know which skills matter, what roles pay well, or where to start.  
This dashboard acts as a **career compass**, helping them plan smartly based on **real-world job data**.

---


## 📫 Contact

 ### **Pritish Kumar Singh**  
If you'd like to connect, collaborate, or discuss improvements:

- 📧 Email: [pritishsinghprf@gmail.com](mailto:pritishsinghprf@gmail.com)
- 🔗 GitHub: [https://github.com/PritishAnalyst](https://github.com/PritishAnalyst)
- 🧑‍💼 LinkedIn: https://linkedin.com/in/pritish1298

