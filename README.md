# 🏥 Healthcare Appointment No-Show Prediction  

### Predicting Patient Appointment Attendance Using Machine Learning


Missed medical appointments (No-Shows) are a major problem in the healthcare industry. When patients fail to attend scheduled appointments, hospitals experience:

Revenue loss

Inefficient resource utilization

Increased waiting times

Reduced patient satisfaction

This project builds a machine learning model to predict whether a patient will attend or miss a scheduled appointment using historical data.

The goal is to help healthcare providers take proactive measures such as targeted reminders and optimized scheduling.

🎯 Business Objective

The primary objective of this project is:

To predict whether a patient will show up for their appointment based on demographic, medical, and scheduling features.

By identifying high-risk patients in advance, healthcare providers can:

Send reminder notifications

Adjust scheduling strategies

Improve operational efficiency

Reduce financial losses due to no-shows

📊 Dataset Description

The dataset contains historical medical appointment records. Each row represents one appointment.

Target Variable:

No-show

Yes → Patient did not attend

No → Patient attended

Key Features:

Patient ID

Appointment ID

Gender

Age

Neighbourhood

Scholarship (Financial support)

Hypertension

Diabetes

Alcoholism

Handicap

SMS Received

Scheduled Day

Appointment Day

🛠 Tools & Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

Jupyter Notebook

🔍 Data Preprocessing

The following preprocessing steps were performed:

Removed irrelevant columns (Patient ID, Appointment ID)

Converted date columns into datetime format

Created a new feature: Waiting Days

Calculated as the difference between Appointment Day and Scheduled Day

Handled categorical variables using encoding techniques

Checked for missing values

Split dataset into features (X) and target variable (y)

Performed train-test split (80% training, 20% testing)

📈 Exploratory Data Analysis (EDA)

Exploratory analysis was conducted to understand patterns in the dataset.

Key Observations:

Younger patients showed slightly higher no-show rates.

Patients who did not receive SMS reminders were more likely to miss appointments.

Longer waiting periods increased the probability of no-show.

Certain neighborhoods had higher no-show frequency.

Visualizations Used:

Count plots

Distribution plots

Correlation heatmap

Boxplots

Bar charts

EDA helped identify important variables that influence attendance behavior.

🤖 Model Building

The following machine learning models were implemented:

Logistic Regression

Decision Tree

Random Forest

The dataset was split into training and testing sets to evaluate model performance.

📊 Model Evaluation

Models were evaluated using:

Accuracy

Precision

Recall

F1 Score

Confusion Matrix

ROC-AUC Score

Example Results (Update with your actual values):
Model	Accuracy	F1 Score	ROC-AUC
Logistic Regression	0.78	0.75	0.80
Random Forest	0.82	0.80	0.85

Random Forest performed better compared to Logistic Regression in terms of overall accuracy and ROC-AUC score.

🔎 Key Insights

Patients with longer waiting days are more likely to miss appointments.

SMS reminders significantly reduce no-show probability.

Age is an important predictor.

Financial aid (Scholarship) shows some influence on attendance behavior.

💼 Business Impact

This predictive model can help healthcare providers:

Identify high-risk patients before appointment date

Send targeted SMS reminders

Optimize appointment scheduling

Reduce operational inefficiencies

Improve patient satisfaction

If deployed in a real hospital system, this model could significantly reduce revenue loss due to missed appointments.

---

##  Project Files & Download Links

-  **Jupyter Notebook** – Model development and evaluation:  
  [View or Download Notebook](https://github.com/bindurag1807/Healthcare-Appointment-No-Show-Prediction/blob/main/Healthcare%20Appointment%20no%20show%20prediction%20.ipynb)

-  **Power BI Dashboard (.pbix)** – Interactive insights and visualizations:  
  [View or Download Dashboard](https://github.com/bindurag1807/Healthcare-Appointment-No-Show-Prediction/blob/main/Healthcare%20appointemnet%20no%20show%20prediction.pbix)

---

##  Dashboard Features

The included Power BI dashboard showcases:
-  Overall attendance vs. no-show rates  
-  High-risk patient analysis  
-  Impact of SMS reminders on no-shows  
-  Model performance metrics (Precision, Recall, F1 Score, Accuracy) visualized clearly

---

##  Results Summary

| Metric           | Value         |
|------------------|---------------|
| Model Accuracy   | 77.44%        |
| F1 Score         | 0.87          |
| Reminder Impact  | Slight reduction in no-show rate when SMS reminders were sent |

