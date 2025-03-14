### **Healthcare Stroke Prediction and Analysis**

This project aims to predict stroke occurrences based on various health parameters and demographic data. It includes a detailed **Healthcare Stroke Analysis Dashboard** that visualizes key insights and patterns in the dataset.

---

## **Project Overview**
Stroke is a serious medical condition that occurs when blood flow to the brain is interrupted. This project utilizes machine learning models to predict the likelihood of stroke based on risk factors such as age, glucose levels, smoking status, and medical history. Additionally, the interactive dashboard provides valuable insights for healthcare professionals and researchers.

---

## **Dataset Description**
The dataset contains multiple features related to health conditions and demographics, including:

- **age**: Age of the individual.  
- **gender**: Male, Female, or Other.  
- **hypertension**: Whether the individual has hypertension (1 = Yes, 0 = No).  
- **heart_disease**: Whether the individual has a history of heart disease (1 = Yes, 0 = No).  
- **ever_married**: Marital status (Yes/No).  
- **work_type**: Type of employment (Private, Self-employed, Govt job, etc.).  
- **Residence_type**: Urban or Rural.  
- **avg_glucose_level**: Average glucose level in the blood.  
- **bmi**: Body Mass Index.  
- **smoking_status**: Never smoked, Formerly smoked, or Currently smokes.  
- **stroke** (Target Variable): 1 = Stroke occurred, 0 = No stroke.  

---

## **Machine Learning Model**
The following steps were followed for building the predictive model:  

1. **Data Preprocessing:**  
   - Handled missing values using mean/mode imputation.  
   - Encoded categorical variables using **OneHotEncoder** to manage unseen data.  
   - Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to address class imbalance.  

2. **Model Training:**  
   - Implemented multiple models like **Random Forest**, **Logistic Regression**, and **XGBoost**.  
   - Tuned hyperparameters using GridSearchCV for optimal performance.  

3. **Evaluation Metrics:**  
   - ROC-AUC score, Precision, Recall, and F1-score were used to evaluate model performance.  

4. **Final Model Performance:**  
   - Achieved an improved **ROC-AUC score of 0.74** after applying **SMOTE** and **downsampling**.

---

## **Healthcare Stroke Analysis Dashboard**
The interactive dashboard visualizes crucial insights from the dataset, offering clear patterns and risk factors:

- **Stroke by Smoking Status:** Highlights stroke distribution among smokers and non-smokers.  
- **Age and Gender Analysis:** Reveals higher stroke cases in older individuals.  
- **Residence Type Impact:** Stroke cases are evenly distributed across **urban** and **rural** regions.  
- **Heart Disease by Work Type:** Private sector workers show a higher risk.  
- **Glucose and BMI Trends:** Elevated glucose levels correlate with higher stroke risk.  
- **Gender Analysis:** Females have higher hypertension rates, while males show more heart disease cases.

---

## **How to Run the Project**
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/healthcare-stroke-prediction.git
   cd healthcare-stroke-prediction
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Model Training Script:**
   ```bash
   python train_model.py
   ```

4. **Launch the Dashboard:**
   ```bash
   streamlit run dashboard.py
   ```

---

## **Technologies Used**
- **Python (pandas, numpy, scikit-learn)**  
- **SMOTE for handling class imbalance**  
- **Streamlit for interactive dashboard**  
- **Matplotlib & Seaborn for visualizations**  

---

## **Future Improvements**
- Integrate advanced feature engineering techniques.  
- Implement additional ML models for improved accuracy.  
- Enhance the dashboard for real-time data updates.

---

## **Contributing**
Contributions are welcome! Feel free to raise issues or submit pull requests.

---

## **Contact**
For queries or collaboration, reach out via [LinkedIn](https://www.linkedin.com/in/ramews14).
