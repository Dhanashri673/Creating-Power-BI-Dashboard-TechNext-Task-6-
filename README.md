# Creating-Power-BI-Dashboard-TechNext-Task-6

# Objective:

# * To design a complete data analysis workflow that:

Stores and organizes data in a SQL database.

Extracts and transforms data using SQL queries.

Connects SQL output to Power BI.

Builds an interactive dashboard to identify projects and departments at risk of being over budget or underperforming.


# Project Workflow

# 1.Database Setup

Installed Microsoft SQL Server Express 2022 as the database engine.

Installed SQL Server Management Studio (SSMS) for database management and query execution.

Created a new database named project.

# 2.Data Ingestion

Imported multiple CSV files into SQL Server using the Import Flat File feature:

employees

departments

completed_projects

upcoming_projects

project_assignments

projects (additional project details)

headshots (employee profile images)

# 3.SQL Query Development

Performed exploratory queries using SELECT statements to review data in each table.

 # Joins & Relationships:

Linked employees with departments via department_id.

Linked employees to projects via project_assignments using employee_id and project_id.

# Combining Project Tables:

Merged upcoming_projects and completed_projects using UNION ALL.

Added a status column to distinguish between “Upcoming” and “Completed” projects.

Created a Common Table Expression (CTE) project_status to hold combined project data.

# Built a final consolidated query (Big Table) combining:

Employee details (ID, name, job title, salary)

Department information

Project name, status, and budget.

# 4.Power BI Integration

Opened Power BI Desktop and selected SQL Server as the data source.

Connected using server details from SQL Server properties.

Used the SQL query (Big Table) as the main dataset for Power BI.

# 5.Dashboard Development

Designed an interactive dashboard with:

Employee Info Section – Displays name, job title, salary, and headshots.

Department Overview – Shows which departments are profitable or over budget.

Project Status Tracking – Highlights upcoming vs. completed projects.

Filters & Slicers – Allows filtering by department, project, or employee.

# Key Learnings & Skills Applied

Database Management: Installing and configuring SQL Server, creating databases, importing data.

SQL Techniques: SELECT, JOIN, UNION ALL, CTEs, aliases, and filtering.

Data Visualization: Creating interactive dashboards in Power BI connected directly to a SQL database.

End-to-End Workflow: From raw data to an analytical dashboard, demonstrating real-world data analysis processes.

# Outcome

# A fully functional Power BI dashboard that provides:

Real-time insights into departmental budgets.

Identification of at-risk projects.

Detailed employee and project-level information for better decision-making.
