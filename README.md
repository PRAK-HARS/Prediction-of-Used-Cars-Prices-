

---

# 🎯 **Prediction of Used Cars Prices**  

---

## 🚀 **Project Overview**  

In this project, we employ an **ensemble learning approach** for regression tasks using three state-of-the-art gradient boosting models:  
1. **XGBoost** 🌟  
2. **CatBoost** 🐱  
3. **LightGBM** 💡  

These models are combined using a **Voting Regressor** with optimized weights to maximize predictive performance.  

---

## ⚙️ **Approach & Methodology**  

### 🔹 **1. Model Selection**  
We chose the following models:  
- **XGBoost**: Fast, scalable, and efficient gradient boosting algorithm.  
- **CatBoost**: Handles categorical features seamlessly with robust performance.  
- **LightGBM**: Lightweight and optimized for large datasets with fast training speed.  

### 🔹 **2. Ensemble Learning**  
A **Voting Regressor** was used to combine predictions from the three models. Instead of equal weights, we optimized and fine-tuned the weights as follows:  

| Model         | Weight Assigned 🎚️      |  
|---------------|-------------------------|  
| **XGBoost**  | `2.9983`                |  
| **CatBoost** | `3.0023`                |  
| **LightGBM** | `2.9994`                |  

These weights ensure each model contributes proportionally to the final predictions.  

---

## 🛠️ **Workflow**  

1. 📊 **Data Preprocessing**  
   - Handled missing values.  
   - Feature scaling and dataset splitting into **training** and **testing** sets.  

2. 🔧 **Model Training**  
   - Trained XGBoost, CatBoost, and LightGBM individually on the preprocessed data.  

3. 🤝 **Voting Ensemble**  
   - Combined predictions using a weighted **Voting Regressor**.  

4. 📈 **Model Evaluation**  
   - Evaluated the ensemble model using ]**RMSE**.

---

## 💻 **Requirements**  

Ensure the following libraries are installed:  
```bash
pip install xgboost catboost lightgbm scikit-learn pandas numpy matplotlib
```

---

## 📊 **Results & Performance**  

The optimized **Voting Regressor** successfully combines the strengths of XGBoost, CatBoost, and LightGBM, yielding superior predictive performance compared to individual models.  

| **Metric**            | **Value** 📈   |  
|-----------------------|---------------|  
| Example: RMSE         | `63,278`  |

---

## 📝 **Code & Notebook**  

Explore the full implementation in the Jupyter Notebook:  
🔗 **`Missing_values.ipynb`**  
🔗 **`main.ipynb`**  

---

## 🎯 **Conclusion**  

By leveraging the power of ensemble learning with **weighted voting**, this approach enhances predictive accuracy and generalizes well on complex regression tasks.  

**Key Takeaway**: Combining the strengths of individual models often outperforms standalone techniques. 🌟  

---

## 🌟 **Future Work**  

- Experimenting with additional ensemble techniques (e.g., stacking, bagging).  
- Further hyperparameter tuning of individual models.  

---
