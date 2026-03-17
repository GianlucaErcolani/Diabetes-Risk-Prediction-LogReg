# Diabetes Risk Prediction project

The goal of this project is to build a classification model using **Logistic Regression** to predict whether a patient has diabetes based on specific clinical diagnostic measurements. This project covers the full analytical pipeline, from data exploration and feature scaling to model evaluation using ROC curves.

### Project Structure

* `Logistic regression-Diabetes dataset.py`: Python script containing the complete workflow:
    * **Data Exploration (EDA)**: Inspection of statistical distributions and feature relationships using histograms and pairplots.
    * **Data Preprocessing**: Feature scaling using `StandardScaler` to normalize the clinical variables.
    * **Predictive Modeling**: Implementation of a Logistic Regression classifier.
    * **Performance Evaluation**: Detailed analysis using Confusion Matrix, Accuracy, Sensitivity (Recall), and Specificity metrics.
    * **Threshold Analysis**: Visualization of the **ROC Curve** (Receiver Operating Characteristic) to evaluate the model's diagnostic ability across different thresholds.
* `requirements.txt`: List of Python libraries required (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn).

### Dataset

**Input variables (Clinical Markers):**
* `Pregnancies`: Number of times pregnant.
* `Glucose`: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.
* `BloodPressure`: Diastolic blood pressure (mm Hg).
* `SkinThickness`: Triceps skin fold thickness (mm).
* `Insulin`: 2-Hour serum insulin (mu U/ml).
* `BMI`: Body mass index (weight in kg/(height in m)^2).
* `DiabetesPedigreeFunction`: A function which scores likelihood of diabetes based on family history.
* `Age`: Age (years).

**Output variable (Target):**
* `Outcome`: Class variable (0 = No Diabetes, 1 = Diabetes).

### Results
The model demonstrated strong diagnostic performance on the test set:
* **Accuracy**: ~82%
* **Sensitivity (Recall)**: ~61% (Ability to correctly identify patients with diabetes)
* **Specificity**: ~93% (Ability to correctly identify healthy patients)

The project includes an **ROC Curve** visualization to assist in selecting the optimal classification threshold for medical diagnosis.
