# Customer Churn Prediction — Model Comparison

**Author:** Gabriele Giugliarelli  

This project compares multiple machine learning algorithms for predicting customer churn.  
Using a telecom-style dataset, it evaluates which models perform best and highlights why traditional ML methods often outperform deep learning on structured tabular data.

---

## Overview
- Cleaned and prepared a customer dataset (categorical encoding, scaling, splitting)  
- Trained and compared several models:
  - Logistic Regression  
  - Random Forest  
  - XGBoost  
  - A simple Deep Neural Network (DNN) for comparison  
- Evaluated models using Accuracy, Precision, Recall, F1-score, and ROC-AUC  

---

## Results
As expected, **classical machine learning models clearly outperformed deep learning** for this kind of structured (tabular) data:

| Model | Accuracy | AUC | Comment |
|--------|-----------|------|----------|
| Logistic Regression | ~0.80 | ~0.83 | Strong baseline, interpretable |
| Random Forest | ~0.80 | ~0.84 | Excellent performance and stability |
| XGBoost | ~0.80 | ~0.85 | Best overall performer |
| Deep Neural Network | ~0.71 | ~0.79 | Underperformed on tabular features |

**Conclusion:**  
Tree-based ensemble methods (Random Forest, XGBoost) handle mixed numerical and categorical variables efficiently and require less tuning than deep learning for structured datasets.  
The experiment confirms that classical machine learning models outperform neural networks when dealing with tabular data.
---

## Key Insights
- Short tenure, high monthly charges, and month-to-month contracts are the strongest churn predictors.  
- Feature engineering and proper preprocessing had a greater impact on performance than network depth.  
- Deep learning architectures may underperform on limited, non-sequential data unless extensive feature representation is applied.

---

## Tech Stack
Python · pandas · numpy · matplotlib · seaborn · scikit-learn · xgboost · PyTorch

---

## How to Run
You can open and run the notebook directly in **Google Colab**.  

---
## Contact
**GitHub:** [@giugliarelligabriele](https://github.com/giugliarelligabriele)
**LinkedIn:** [Gabriele Giugliarelli](https://www.linkedin.com/in/gabriele-giugliarelli)
