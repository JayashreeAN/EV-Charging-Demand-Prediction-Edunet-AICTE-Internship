# EV Charging Demand Prediction

This project was developed during the **AICTE – Edunet Internship (July–Aug 2025)**. The goal is to predict future electric vehicle (EV) adoption trends across counties in Washington State using machine learning and deploy the results through an interactive web app.

---

## Objective

To forecast electric vehicle (EV) demand over the next 36 months using historical registration data, enabling better insights for EV infrastructure planning.

---

## Problem Statement

Using a real-world dataset from the Washington State Department of Licensing (DOL), this project aims to:

- Predict the number of electric vehicles (EVs) in future months.
- Analyze growth trends based on vehicle types (BEVs, PHEVs).
- Compare EV adoption across counties using historical monthly registration data (2017–2024).

---

## Tools & Technologies

- **Language**: Python 3.12.8  
- **Libraries**: pandas, numpy, matplotlib, scikit-learn, joblib, streamlit  
- **Environments**: Google Colab, Kaggle, VS Code, Jupyter Notebook

---

## Methodology

1. **Data Preprocessing**  
   - Cleaned raw dataset and engineered time-series features like lag values, percent change, and growth slope  
   - Encoded categorical columns (county names)

2. **Model Training**  
   - Trained a Random Forest Regressor using scikit-learn  
   - Target variable: `Electric Vehicle (EV) Total`

3. **Model Saving**  
   - Saved the trained model using `joblib` as `forecasting_ev_model.pkl`

4. **Web App Development**  
   - Built an interactive dashboard using **Streamlit** (`app.py`)  
   - User selects a county to view 3-year EV adoption forecast  
   - Supports comparison of EV growth across up to 3 counties

5. **Visualization**  
   - Displayed historical and forecasted EV trends using Matplotlib  
   - Showed percentage growth insights across selected regions

---

## Running the Project

1. Clone the repository and open the folder in Visual Studio Code:
git clone [https://github.com/JayashreeAN/EV-Charging-Demand-Prediction-Edunet-AICTE-Internship.git](https://github.com/JayashreeAN/EV-Charging-Demand-Prediction-Edunet-AICTE-Internship.git)

cd EV-Charging-Demand-Prediction-Edunet-AICTE-Internship

2. (Optional) Create and activate a virtual environment:
python -m venv venv
.\venv\Scripts\activate   # for Windows 

3. Install the required dependencies:
pip install -r requirements.txt

4. Run the Streamlit application:  
streamlit run app.py

```

The web app will launch in your browser, allowing you to forecast EV adoption per county and compare regional trends.

---

## 📦 Project Files

| File Name                        | Description                                |
|----------------------------------|--------------------------------------------|
| Dataset.csv                      | Raw vehicle registration data              |
| Preprocessed_EV_data.csv         | Cleaned and feature-engineered dataset     |
| forecasting_ev_model.pkl         | Trained regression model                   |
| app.py                           | Streamlit web application script           |
| requirements.txt                 | Python dependencies                        |
| EV_Charging_Demand_Prediction.ipynb | Jupyter notebook for EDA + model training |

---

## Developed By

**Jayashree N**  
Artificial Intelligence & Data Science  
AICTE – Edunet Internship 2025
```
