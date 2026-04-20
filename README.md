
# Healthcare Appointment Attendance Analysis

## Project Overview

This project analyses patient appointment attendance and no-show behaviour using the Brazil Medical Appointment No-Show dataset.

The objective was to identify patterns linked to missed appointments and explore actions that may improve attendance rates and scheduling efficiency.

---

## Business Problem

Missed medical appointments can lead to:

- unused clinic capacity  
- longer waiting lists  
- lower operational efficiency  
- delayed patient treatment  
- lost revenue opportunities  

This analysis focuses on understanding who misses appointments and whether reminders improve attendance.

---

## Tools Used

- **SQL (SQLite)** – data cleaning and analysis  
- **Power BI** – dashboard development  
- **Excel** – supporting preparation work  
- **Power Query** – data reshaping and transformation  

---

## Dataset

- **Source:** Public Kaggle dataset  
- **Records:** 100K+ appointment records  
- **Region:** Brazil healthcare appointments  

Main fields included:

- Patient age  
- Gender  
- Scheduled date  
- Appointment date  
- SMS reminder status  
- Chronic conditions  
- No-show status  

---

## Data Preparation

The dataset was cleaned and transformed before reporting.

### Key Steps

- Standardised date formats  
- Created age bands for segmentation  
- Relabelled no-show fields into clear attendance status  
- Converted binary condition flags into readable labels  
- Calculated waiting days between booking and appointment  
- Reshaped condition columns for easier reporting  

---

## Example SQL Logic

```sql
SELECT SMS_Status,
       COUNT(*) AS total_appointments
FROM noshow_cleaned
GROUP BY SMS_Status;


## Dashboard Features

The Power BI dashboard includes:

- Total appointments KPI
- No-shows by age group
- Attendance by chronic condition
- Gender attendance comparison
- SMS reminder analysis
- Interactive filters and slicers

---

## Key Findings

- Working-age adults recorded the highest number of missed appointments.
- Patients who received SMS reminders had fewer no-shows.
- Female patients represented a larger share of attended appointments.
- Older patients had stronger attendance rates than younger groups.
- Hypertension was the most common chronic condition in the dataset.

## Recommendations

- Continue and expand SMS reminder programs.
- Add follow-up reminders closer to appointment dates.
- Focus no-show reduction efforts on higher-risk age groups.
- Review waiting times and scheduling delays.
- Monitor repeat no-show behaviour for targeted intervention.











