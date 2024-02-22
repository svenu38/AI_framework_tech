# AI_framework_tech
HCAI
# 

# Analysis of Hospital Admission Data: Understanding Patient Stay Duration

## Overview
This project aims to analyze hospital admission data to gain insights into the factors influencing the duration of patient stays in hospitals. The dataset contains various features related to hospital admissions, including patient demographics, severity of illness, type of admission, and more. By exploring this data, we seek to understand patterns and trends that can help optimize hospital resources and improve patient care.

## Dataset Description
The dataset includes the following features:

- **case_id**: Unique ID for each case registered in the hospital.
- **Hospital_code**: Unique code assigned to each hospital.
- **Hospital_type_code**: Unique code indicating the type of hospital.
- **City_Code_Hospital**: City code where the hospital is located.
- **Hospital_region_code**: Code representing the region where the hospital is situated.
- **Available Extra Rooms in Hospital**: Number of extra rooms available in the hospital.
- **Department**: Department overseeing the case in the hospital.
- **Ward_Type**: Code representing the type of ward.
- **Ward_Facility_Code**: Code representing the facility of the ward.
- **Bed Grade**: Condition of the bed in the ward.
- **patientid**: Unique ID assigned to each patient.
- **City_Code_Patient**: City code of the patient.
- **Type of Admission**: Type of admission registered by the hospital.
- **Severity of Illness**: Severity of the illness recorded at the time of admission.
- **Visitors with Patient**: Number of visitors accompanying the patient.
- **Age**: Age of the patient.
- **Admission_Deposit**: Deposit amount made at the time of admission.
- **Stay**: Duration of stay in the hospital by the patient.

## Analysis Goals
- Explore the distribution of patient stay durations.
- Identify factors influencing the length of hospital stays.
- Build predictive models to estimate patient stay duration.
- Provide actionable insights for hospital administrators to optimize resources and improve patient care.

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Project Structure
- ``: Directory containing the dataset files.
- `dataset/exam.ipynb/`: Jupyter notebooks for data exploration, analysis, and modeling.
- `README.md`: Overview of the project, dataset description, analysis goals, and project structure.
- `requirements.txt`: List of Python packages required to run the project.

## Best Parameters and Model Performance

### Random Forest

After hyperparameter tuning, the best parameters for the Random Forest model were found to be:

- Number of Estimators: 200
- Minimum Samples Split: 5
- Minimum Samples Leaf: 2
- Maximum Features: 'sqrt'
- Maximum Depth: None
- Bootstrap: False

The model achieved a cross-validated score of 0.6282 with these parameters, indicating its performance in predicting patient stay duration.

## Best Parameters and Model Performance

### Decision Tree

After hyperparameter tuning, the best parameters for the Decision Tree model were found to be:

- Minimum Samples Split: 2
- Minimum Samples Leaf: 2
- Maximum Features: None
- Maximum Depth: None

The model achieved a cross-validated score of 0.4867 with these parameters, indicating its performance in predicting patient stay duration.

## Getting Started
1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Explore the Jupyter notebooks in the `exam.ipynb/` file to understand the analysis process.

## Contributors
- [venu siddapura govindaraju](https://github.com/svenu38/AI_framework_tech)
- [shilpa srinivasareddy] (https://github.com/shilpasrinivasareddy/AI_framework_tech)



