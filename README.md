# Diabetes-prediction-app-
A machine learning web app that predicts diabetes based on health metrics like glucose, BMI, insulin, and more. Built with Random Forest and Gradio, it displays prediction confidence with visuals and offers risk categories and tips. Developed for a scholarship competition.

#  Diabetes Prediction App (ML + Gradio)

A machine learning web application that predicts whether a person is diabetic based on key health indicators. It also displays the prediction confidence using a bar chart and provides health risk categories with tips. Built by Patrick Ayisi and team as a scholarship competition capstone.

---

##  Features

- Predicts diabetes using Random Forest Classifier
- Interactive UI using Gradio
- Confidence chart (prediction probability)
- Feature engineering for enhanced model performance
- Risk category tagging
- Custom health tips based on input data

---

##  Model Overview

- **Algorithm**: RandomForestClassifier
- **Best Params**: `n_estimators=300`, `max_depth=20`, `min_samples_split=10`, `min_samples_leaf=2`
- **Tuning**: GridSearchCV
- **Accuracy**: ~77.9%
- **Balanced with**: PowerSMOTE (to handle class imbalance)

---

##  Features Used

- Pregnancies  
- Glucose  
- Blood Pressure  
- Skin Thickness  
- Insulin  
- BMI  
- Diabetes Pedigree Function  
- Age  
- Engineered:  
    - BMI × Age  
    - Glucose ÷ (BMI + 1)  
    - Pregnancy ÷ (Age + 1)

---

##  Interface Preview

![Gradio UI](images/app_screenshot.png)  
<img width="1570" height="851" alt="image" src="https://github.com/user-attachments/assets/adfe2a1d-73a5-45c1-bd5a-f046295f3c87" />

---

##  Try It Out

You can run the app in Google Colab (with Gradio interface):  
[🔗 Launch App on Colab](your_colab_link_here)

---

##  Sample Input

| Feature         | Value |
|----------------|-------|
| Pregnancies     | 2     |
| Glucose         | 140   |
| Blood Pressure  | 70    |
| Skin Thickness  | 25    |
| Insulin         | 100   |
| BMI             | 33.6  |
| Diabetes Pedigree Function | 0.45 |
| Age             | 29    |

---

##  How to Run

```bash
# Clone repo
git clone https://github.com/yourusername/diabetes-prediction-app.git
cd diabetes-prediction-app

# Install dependencies
pip install -r requirements.txt

# Run app
python app.py
