# End-to-End Student Drop-Out Prediction Project

**Executive Summary:**  
This project uses real student data and advanced machine learning to predict whether students will graduate, drop out, or remain enrolled. By combining thorough data exploration, robust modeling, and hyperparameter optimization, the resulting XGBoost pipeline achieves strong predictive performance and provides actionable insights for early intervention in higher education.

---

## **Project Overview**

**Goal:**  
Predict student outcomes—'Graduate', 'Dropout', or 'Enrolled'—using demographic, academic, and socioeconomic features.

**Why it matters:**  
Early identification of at-risk students enables universities to deploy targeted support, reduce dropout rates, and improve educational outcomes.

**Your Role:**  
All analysis, modeling, and reporting performed by [Antonio Martín Acuña](https://github.com/antoniomacu).

---

## **Dataset**

- Source: Valentim Realinho, Jorge Machado, Luís Baptista, Mónica V. Martins (Research Center for Endogenous Resource Valorization, Polytechnic Institute of Portalegre)
- Undergraduate student records with demographic, academic, and economic variables.

---

## **Project Steps**

1. **Setup and Feature Inspection**
2. **Exploratory Data Analysis (EDA)**
3. **Data Preparation & Preprocessing**
4. **Model Training & Evaluation**
5. **Hyperparameter Tuning** (RandomSearch, GridSearch, Optuna)
6. **Error Analysis & Model Persistence**

---

## **Key Results**

- **Best Model:** XGBoost Pipeline (after SMOTE and optimization)
- **Performance:**
  - Training F1-score: **82.9%**
  - Test F1-score: **70.4%**
  - Highest accuracy for 'Graduate' and 'Dropout'
  - 'Enrolled' remains challenging due to class imbalance (see notebook for error analysis)
- **Business Value:**  
  Enables early warning for student support teams to proactively address potential dropouts.

- **Sample Visualizations:**  
  _See notebook for:_
    - Confusion matrix (test set)
    - Feature importance
    - ROC-AUC curves
    - Error profiles

---

## **Reproducibility**

- Python 3.8+
- Main libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `matplotlib`, `seaborn`, `joblib`, `optuna`, `imblearn`
- All code in the notebook is modular, with random seeds set for reproducibility.
- Final model is saved as `best_model.joblib` for easy deployment.

---

## **Getting Started**

```bash
git clone https://github.com/antoniomacu/End-to-end-Drop-Out-Project.git
cd End-to-end-Drop-Out-Project
# Install requirements using pip or conda as needed
```

Open and run the notebook `Dropout Project.ipynb` to follow the entire workflow with code, plots, and commentary.

---

## **Conclusion & Future Work**

- The XGBoost pipeline provides robust classification of student outcomes.
- Primary challenge: Improving recall for the 'Enrolled' class.
- **Future directions:**  
  - Explore more advanced class balancing techniques
  - Enhanced feature engineering
  - Test additional algorithms or interpretability tools (e.g., SHAP)

---

## **Acknowledgements**

- **Dataset Source:** Valentim Realinho, Jorge Machado, Luís Baptista, Mónica V. Martins (Research Center for Endogenous Resource Valorization, Polytechnic Institute of Portalegre)

---

## **Contact**

- **GitHub:** [antoniomacu](https://github.com/antoniomacu)
- **LinkedIn:** [Antonio Martín Acuña](https://www.linkedin.com/in/antonio-mart%C3%ADn-acu%C3%B1a/)
- _Questions or suggestions welcome!_

---
## Contact

For questions or suggestions, please contact:
- GitHub: [antoniomacu](https://github.com/antoniomacu)
- LinkedIn: [Antonio Martín Acuña](https://www.linkedin.com/in/antonio-mart%C3%ADn-acu%C3%B1a-328793208/)
