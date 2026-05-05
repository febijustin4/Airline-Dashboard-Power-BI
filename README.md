# Airline Operations & Delay Intelligence Dashboard

> An interactive Power BI dashboard designed to analyze flight delays, cancellations, airline performance, and airport traffic using the US Flight Delays dataset.

---

## Project Objective

The objective of this project is to monitor airline operations and identify delay patterns by analyzing:

- Total flights operated
- Delayed flights
- Cancelled flights
- Airline performance
- Airport traffic
- Average arrival delay
- Average departure delay
- On-time performance

---

## Dataset Information

**Source:** Kaggle Flight Delays Dataset  
https://www.kaggle.com/datasets/usdot/flight-delays

### Tables Used

| Table Name | Description |
|------------|-------------|
| Flights | Contains flight operation details |
| Airlines | Airline information |
| Airports | Airport details |

---

## Tools & Technologies

- Power BI
- Power Query
- DAX
- Data Modeling

---

## Data Cleaning & Transformation

- Removed null values
- Checked data types
- Cleaned inconsistent records
- Prepared data for analysis in Power Query

---

## Data Modeling

Created relationships between:

- Flights table
- Airlines table
- Airports table

Used a star schema model for efficient reporting.

---

## DAX Measures


Total Flights = COUNT(flights[AIRLINE])

Total Delayed Flights = 
COUNTROWS(
    FILTER(flights, flights[ARRIVAL_DELAY] > 0)
)

Delay % = 
DIVIDE([Total Delayed Flights], [Total Flights])

Cancelled Flights = 
COUNTROWS(
    FILTER(flights, flights[CANCELLED] = 1)
)

## Project Workflow
-Data collection from Kaggle dataset
-Data cleaning and preprocessing
-Data modeling in Power BI
-Creating DAX measures
-Building interactive dashboards
-Generating insights for airline performance analysis

## Key Insights
Identified airlines with the highest delays
Analyzed cancellation trends across different airlines
Found busiest airports based on flight traffic
Measured average arrival and departure delays
Evaluated overall operational efficiency

## Dashboards

### Flight Dashboard

<img width="1263" height="708" alt="Screenshot 2026-05-04 151902" src="https://github.com/user-attachments/assets/a20c6179-0a7a-451b-bb30-9e6c4aa0334a" />

### Airline Dashboard

<img width="1257" height="708" alt="Screenshot 2026-05-04 151922" src="https://github.com/user-attachments/assets/f7886c70-6a09-47ff-a822-e45a708aab32" />

### Airport Dashboard

<img width="1263" height="679" alt="Screenshot 2026-05-04 151940" src="https://github.com/user-attachments/assets/59e776dc-872f-472a-9927-12561e56080f" />



### ⚙️ Connect with Me

<p align="center">
<a href="mailto:febijustin4@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/febi~justin/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
