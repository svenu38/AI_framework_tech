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

# Model Performance and Hyperparameter Tuning

## Splitting the Dataset into Training and Testing Sets
- **Training set size:** 251,034
- **Testing set size:** 62,759

## Handling Class Imbalance (SMOTE)
### Class distribution before balancing:
- **21-30:** 69,138
- **11-20:** 61,789
- **31-40:** 43,345
- **51-60:** 27,471
- **0-10:** 18,548
- **41-50:** 9,204
- **71-80:** 8,141
- **More than 100 Days:** 5,226
- **81-90:** 3,836
- **91-100:** 2,194
- **61-70:** 2,142

### Class distribution after SMOTE:
- **31-40:** 69,138
- **0-10:** 69,138
- **21-30:** 69,138
- **81-90:** 69,138
- **11-20:** 69,138
- **51-60:** 69,138
- **61-70:** 69,138
- **More than 100 Days:** 69,138
- **71-80:** 69,138
- **91-100:** 69,138
- **41-50:** 69,138

## Model Performance Before Hyperparameter Tuning

### Random Forest Model
- **Accuracy:** 0.409
- **Precision:** 0.391
- **Recall:** 0.409
- **F1-score:** 0.386

### Logistic Regression Model
- **Accuracy:** 0.184
- **Precision:** 0.158
- **Recall:** 0.184
- **F1-score:** 0.150

### Decision Tree Model
- **Accuracy:** 0.300
- **Precision:** 0.304
- **Recall:** 0.300
- **F1-score:** 0.302



## Best Parameters and Model Performance

### Random Forest Model
- **Best Parameters:** {'n_estimators': 200, 'min_samples_split': 5, 'min_samples_leaf': 2, 'max_features': 'sqrt', 'max_depth': None, 'bootstrap': False}
- **Best Score:** 0.623

### Decision Tree Model
- **Best Parameters:** {'min_samples_split': 2, 'min_samples_leaf': 2, 'max_features': None, 'max_depth': None}
- **Best Score:** 0.481

## Explanation
- The Random Forest model's performance significantly improved after hyperparameter tuning, achieving an accuracy of 0.623, indicating better generalization and capturing more patterns in the data.
- Similarly, the Decision Tree model also showed improvement with an accuracy of 0.481 after tuning, though not as high as the Random Forest model.
- Despite hyperparameter tuning not being mentioned for Logistic Regression, its poor performance suggests the need for further analysis or more sophisticated techniques.

## Conclusion
Hyperparameter tuning played a crucial role in enhancing the Random Forest and Decision Tree models' performance, significantly improving their accuracy and overall predictive capability. Further refinement may be necessary, especially for the Logistic Regression model, to achieve better results.





## Getting Started
1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Explore the Jupyter notebooks in the `exam.ipynb/` file to understand the analysis process.

## Contributors
- [venu siddapura govindaraju](https://github.com/svenu38/AI_framework_tech)
- [shilpa srinivasareddy] (https://github.com/shilpasrinivasareddy/AI_framework_tech)

- Abhishek 
- abdelelreheman



