📌 Overview
This project focuses on building a machine learning model to predict whether a person is likely to donate blood again. Accurate predictions can help health organizations target the right individuals and improve the efficiency of blood donation drives.

We also visualize patterns in the data using Power BI, and apply SMOTE to deal with class imbalance in the dataset.

📊 Dataset
File: blood.csv
Rows: 748
Columns:

Recency: Months since last donation

Frequency: Total number of donations

Monetary: Total donated blood (in c.c.)

Time: Months since first donation

Class: Target (1 = likely to donate again, 0 = not likely)

🔧 Project Workflow
Data Preprocessing

Loaded CSV

Checked missing values

Explored summary statistics

Visualization

Histograms and correlation heatmap (Python)

Interactive Power BI dashboard

Modeling

Logistic Regression

Decision Tree

Random Forest (with SMOTE)

XGBoost (with SMOTE)

Evaluated using accuracy, confusion matrix, precision, recall, and F1-score

Class Imbalance Handling

Used SMOTE (Synthetic Minority Over-sampling Technique) to oversample minority class

🧪 Results
Model	Accuracy	Notes
Logistic Regression	76%	Weak on minority class (1)
Decision Tree	63%	Low recall overall
Random Forest + SMOTE	75.4%	Balanced performance
XGBoost + SMOTE	76.3%	Best performance overall

📈 Power BI Dashboard
The dashboard includes:

Pie chart of predicted donor classes

Bar chart of average feature values by predicted class

Filters for interactive exploration

Cards showing key metrics (e.g., total donors, % likely to donate)

🛠 Technologies Used
Python (pandas, scikit-learn, seaborn, matplotlib, xgboost)

Power BI (for interactive dashboards)

SMOTE (from imblearn)

🚀 Future Improvements
Include age, blood type, and health records

Add donor engagement metrics (email opens, clinic visits)

Build a web dashboard with Streamlit

Deploy model for real-time use

📁 Folder Structure
cpp
Copy
Edit
📦 Personalized_Healthcare_Recommendations/
├── blood.csv
├── Personalized_Healthcare_Recommendations.ipynb
├── dashboard.pbix  (optional Power BI file)
├── README.md
└── requirements.txt
