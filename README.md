# End-to-end Drop-Out Project

## Introduction

Student performance is a key indicator for educational institutions to assess the quality of their services. With the increasing diversity of study programs and specialization levels, analyzing student outcomes has become essential for understanding trends among new generations and improving institutional strategies. This project leverages machine learning to classify and predict whether a student is likely to graduate, drop out, or remain enrolled, providing actionable insights for early intervention.

## Scope

**Goal:**  
The primary objective is to explore and understand the available data, apply machine learning algorithms for student outcome classification, and enhance predictive performance through model selection and optimization. The project specifically focuses on predicting the `Target` variable, categorizing students as 'Graduate', 'Dropout', or 'Enrolled'.

**Dataset:**  
The [dataset](https://www.mdpi.com/2306-5729/7/11/146) was compiled by Valentim Realinho, Jorge Machado, Luís Baptista, and Mónica V. Martins from the Research Center for Endogenous Resource Valorization at the [Polytechnic Institute of Portalegre](https://www.ipportalegre.pt/pt/). It includes information on undergraduate students from various nationalities.

**Project Steps:**
1. Setup and Feature Inspection
2. Exploratory Data Analysis (EDA)
3. Data Preparation
4. Machine Learning Model Deployment
5. Fine-tuning
6. Evaluation and Conclusions

### Prerequisites

- Python 3.8+
- Main libraries: pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn, joblib, etc.

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/antoniomacu/End-to-end-Drop-Out-Project.git
   cd Drop-Out-Project-v2
   ```

2. Install required packages.

### Running the Project

Open and run the cells in `Dropout Project.ipynb` to follow the analysis step by step. All code and plots are in the notebook.

---

## Results

- The final model is an **XGBoost pipeline**, selected after thorough comparison and optimization.
- **Performance:**
  - **Training F1-score:** 82.9%
  - **Test F1-score:** 70.4%
- The model performs strongly for the 'Graduate' and 'Dropout' classes.
- The 'Enrolled' class remains challenging due to class imbalance, even after mitigation attempts.
- Error analysis shows most misclassifications are in the 'Enrolled' class.

---

## Conclusion

In this project, the [dataset](https://www.mdpi.com/2306-5729/7/11/146) from the Polytechnic Institute of Portalegre was deeply analyzed to develop and evaluate a machine learning model for predicting student outcomes: dropout, graduation, or continued enrollment.

- Through preprocessing, feature selection, and model comparison, an **XGBoost pipeline** was chosen, delivering robust performance in classifying outcomes, particularly for 'Graduate' and 'Dropout'.
- **Key metrics:** 82.9% F1-score on training, 70.4% on test data.
- The primary challenge remains the accurate classification of 'Enrolled' students, linked to class imbalance, as revealed in both EDA and error analysis.
- Future improvements could involve more advanced techniques for class balancing, enhanced feature engineering, or testing alternative algorithms.

This project highlights the value of data-driven methods for identifying at-risk students, enabling educational institutions to implement timely interventions and improve learning outcomes.

---

## Acknowledgements

- [Dataset Source](https://www.mdpi.com/2306-5729/7/11/146): Valentim Realinho, Jorge Machado, Luís Baptista, Mónica V. Martins (Research Center for Endogenous Resource Valorization, Polytechnic Institute of Portalegre)

---
## Contact

For questions or suggestions, please contact [antoniomacu](https://github.com/antoniomacu).
