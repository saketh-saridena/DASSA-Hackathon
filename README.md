# CU Boulder DaSSA Hackathon 2 - Bad Cycle Classification

## Project Overview
This repository contains the code and documentation for my participation in the **CU Boulder DaSSA Hackathon 2**. The objective of the hackathon was to develop a classification model to predict **bad decoating cycles** in aluminum manufacturing, enabling timely maintenance and reducing business losses.

## Problem Statement
Aluminum decoating involves removing coatings, paints, and organic contaminants from aluminum scrap via thermal pyrolysis. Poor quality cycles lead to increased black dross, higher disposal costs, and operational inefficiencies. The **goal** was to classify cycles as **Good (0) or Bad (1)** based on various operational parameters, optimizing predictive maintenance scheduling.

### Key Considerations:
- **Downtime Costs:**  
  - If bad cycles are predicted accurately, maintenance takes **30 minutes** at a cost of **$16,000**.  
  - If bad cycles are not predicted, it takes **1 hour**, leading to a **$32,560** loss and extra labor costs of **$300/hr**.
- **Environmental Impact:** Poor metal quality increases black dross by **50kg per cycle**, with a disposal cost of **$60/kg**.

## Evaluation Metric
The **Area Under the Receiver Operating Characteristic Curve (AUC-ROC)** was used as the primary metric to evaluate model performance.

---

##  Repository Structure
```
├── Hackathon_final.ipynb         # Jupyter Notebook containing the full model pipeline
├── Hackathon_final.html          # Rendered HTML version of the notebook
├── Predicted_Test_Data_Final.csv # Final submission file for Kaggle
├── README.md                     
```

---

## Methodology

### 1️⃣ **Data Exploration**
- Analyzed data distributions and correlations.
- Identified missing values and anomalies.

### 2️⃣ **Data Preprocessing**
- Handled missing values.
- Normalized and transformed features.
- Engineered new features for better classification.

### 3️⃣ **Data Visualization**
- Created at least **5 unique visualizations** to understand data trends.
- Visualized the impact of cycle parameters on decoating quality.

### 4️⃣ **Feature Engineering**
- Derived meaningful features to improve model performance.
- Selected key features using correlation analysis.

### 5️⃣ **Modeling & Selection**
- Tried multiple classification models, including:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting (XGBoost)
- Used **hyperparameter tuning** to optimize the final model.

### 6️⃣ **Final Model & Predictions**
- The best model was selected based on **AUC-ROC**.
- Final predictions were saved in `Predicted_Test_Data_Final.csv` for submission.

---

## Results & Key Findings
- **Why this model?**  
  - The final model was chosen based on its high AUC-ROC score and ability to generalize well.
- **Metric Explanation:**  
  - AUC-ROC ensures better classification of bad cycles while minimizing false positives.
- **Visualization Insights:**  
  - Certain cycle parameters strongly influenced the likelihood of bad cycles.

---

## Hackathon Submission
As per the hackathon requirements, the final deliverables included:
- **GitHub Submission:** Uploaded all code and documentation.
- **PowerPoint Presentation:** Provided a structured presentation covering:
  - Data Exploration
  - Feature Engineering
  - Model Selection & Performance
  - Key Business Insights
- **Final Kaggle Submission:** Submitted predictions on **07:00 AM** deadline.

---

## Conclusion
This project successfully developed a predictive model to classify **bad decoating cycles**, helping **reduce operational costs, improve efficiency, and minimize environmental waste**. Future work could explore **real-time monitoring** and **deep learning techniques** for enhanced predictive maintenance.

**If you find this project useful, feel free to ⭐ the repo and fork it!**

---
