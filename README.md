# Internship-task-12---Power-BI-Data-Transformation-using-Power-Query

## Objective
The objective of this task is to demonstrate practical skills in cleaning, transforming,
and preparing real-world data using Power Query in Power BI before building dashboards.

## Tools Used
- Primary: Power BI Desktop
- Alternative: Excel Power Query

## Dataset Used
- HR Employee Attrition Dataset

## Step-by-Step Transformation Process

### Step 1: Data Import
- Imported the CSV file into Power BI using **Get Data**
- Opened **Power Query Editor** by selecting *Transform Data*

### Step 2: Remove Unwanted Columns
- Removed columns with no analytical value:
  - EmployeeCount
  - Over18
  - StandardHours

### Step 3: Rename Columns
- Renamed technical column names to business-friendly names  
- Example: `MonthlyIncome` → `Monthly Income`

### Step 4: Handle Missing Values
- Identified null values using column filters
- Removed rows where critical fields were missing:
  - Age
  - Department
  - JobRole
  - Attrition
  - Gender
- Replaced missing numerical values with median values
- Replaced missing categorical values with `"Unknown"`

### Step 5: Change Data Types
- Corrected column data types to ensure accurate calculations:
  - Age → Whole Number
  - Monthly Income → Decimal Number
  - Attrition → Text
  - Date fields → Date

### Step 6: Create Conditional Columns
- Created **Age Group** column:
  - Young (<25)
  - Mid (25–40)
  - Senior (>40)
- Created **Salary Band** column:
  - Low
  - Medium
  - High

### Step 7: Apply Changes
- Closed Power Query Editor
- Applied all transformations to the data model

### Visualizations Created

### Visual 1: Employee Count by Department
- Chart Type: Bar Chart
- X-axis: Employee Count
- Y-axis: Department

### Visual 2: Average Monthly Income by Age Group
- Chart Type: Column Chart
- X-axis: Age Group
- Y-axis: Average Monthly Income

### Visual 3: Attrition Breakdown
- Chart Type: Pie Chart
- Shows Attrition vs Non-Attrition

## Final Outcome
- Cleaned and transformed raw HR data
- Created business-ready columns
- Built meaningful visuals
- Demonstrated real-world data preparation skills


