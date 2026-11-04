# Investigate a Dataset: Medical Appointment No-Shows

> Completed as part of **Udacity's Data Analyst Nanodegree Program**.

## Project Overview
This project explores why patients miss their medical appointments. It applies the full data analysis process (wrangling, exploration, visualization and conclusions) to a dataset of medical appointments in Brazil.

## Dataset
The **Medical Appointment No-Shows** dataset (Kaggle, May 2016) contains **110,527 appointments** and 14 columns, including:
- `Gender`, `Age`, `Neighbourhood`
- `ScheduledDay` and `AppointmentDay`
- `Scholarship` (enrolled in the Bolsa Família welfare program)
- Chronic conditions: `Hipertension`, `Diabetes`, `Alcoholism`, `Handcap`
- `SMS_received`: whether the patient received a reminder message
- `No-show`: **Yes** if the patient missed the appointment, **No** if they attended

The dataset is not included in this repository. It can be downloaded from Kaggle: *Medical Appointment No Shows* (`noshowappointments-kagglev2-may-2016.csv`).

## Research Questions
1. What is the overall distribution of no-shows vs. show-ups?
2. Does age affect the likelihood of a no-show?
3. What is the relationship between receiving an SMS reminder and attendance?
4. How do gender and SMS reminders together relate to attendance?
5. How do chronic health conditions relate to no-show rates?
6. Does the neighbourhood of the hospital affect no-show rates?

## Data Wrangling
- Checked data types, missing values and summary statistics (no missing values were found).
- Converted `ScheduledDay` and `AppointmentDay` from text to datetime.
- Removed one record with an invalid age of **-1**.
- Converted `PatientId` to text, since it is an identifier and not a number to calculate with.

## Exploratory Data Analysis
- **Descriptive statistics:** patients' ages range from 0 to 115, with a mean of about 37 years and an interquartile range of 18 to 55.
- **Statistical test:** a **Chi-Square test of independence** between `SMS_received` and `No-show`.
- **Visualizations:** a pie chart, box plots and stacked bar charts.

## Key Findings
- **About 20% of appointments were missed** (22,319 no-shows vs. 88,207 attended).
- **Age** distributions were similar for patients who attended and those who did not, so age does not appear to be a strong factor.
- **SMS reminders** were significantly associated with attendance (Chi-Square = 1766, p < 0.001).
- **Chronic conditions:** the share of patients with hypertension, diabetes and alcoholism differs between the no-show and show-up groups.
- **Neighbourhood:** most neighbourhoods have similar attendance rates, but one stands out with a clearly higher no-show rate.

## Limitations
- The dataset does not record **why** patients missed their appointments.
- The analysis is descriptive. The relationships found show **correlation, not causation**. For example, the link between SMS reminders and attendance may be affected by other factors, such as how far in advance the appointment was booked.

## Further Research
- Study the reasons behind no-shows to design targeted solutions.
- Analyze the time between booking and the appointment day, and its effect on attendance.
- Compare different reminder methods (calls vs. SMS).

## Tools
- Python, Jupyter Notebook
- Pandas and NumPy for data manipulation
- Matplotlib for visualization
- SciPy for the Chi-Square test

## Files
- `Investigate_a_Dataset.ipynb`: the full analysis, with code, charts and explanations.

---
**Jumanah Almatrood**
