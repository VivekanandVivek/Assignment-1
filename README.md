# Assignment-1
Assignment-1(Heart Disease Prediction using Linear Regression) of the Advanced Pattern Recognition, that illustrate the working of the linear regression with multiple independent variable.

# Assignment-1: Heart Disease Prediction using Linear Regression

This project implements a **Linear Regression model** using Python to predict the likelihood of heart disease based on patient health parameters.  
The dataset used is `cleaned_merged_heart_dataset.csv`.

---

##  Project Structure

```
├── cleaned_merged_heart_dataset.csv   # Dataset
├── linear_regression.py               # Main Python script
└── README.md                          # Project documentation
```

---

##  Dataset

The dataset contains various patient health attributes such as:
- `age` – Age of the patient  
- `sex` – Gender (1 = Male, 0 = Female)  
- `cp` – Chest pain type  
- `trestbps` – Resting blood pressure  
- `chol` – Serum cholesterol  
- `fbs` – Fasting blood sugar  
- `restecg` – Resting electrocardiographic results  
- `thalachh` – Maximum heart rate achieved  
- `exang` – Exercise-induced angina  
- `oldpeak` – ST depression induced by exercise  
- `slope` – Slope of the peak exercise ST segment  
- `ca` – Number of major vessels colored by fluoroscopy  
- `thal` – Thalassemia  
- `target` – Presence of heart disease (1 = Yes, 0 = No)

---

##  Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/VivekanandVivek/Assignment-1.git
   cd Assignment-1
   ```

2. **Create a virtual environment** (recommended)  
   ```bash
   python -m venv venv
   venv\Scripts\activate  # Windows
   venv/bin/activate #linux
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

*(Alternatively, just install scikit-learn & pandas manually)*  
```bash
pip install pandas scikit-learn
```

---

##  Usage

Run the Python script:

```bash
python linear_regression.py
```

It will:
- Train a **Linear Regression model**
- Predict heart disease on test data
- Print:
  - Mean Squared Error (MSE)
  - R² Score
  - Accuracy (based on threshold 0.5)

---

##  Example Output

```
Mean Squared Error: 0.19
R² Score: 0.24
Accuracy: 0.78
```

---

##  Model Evaluation

- **MSE (Mean Squared Error)**: Measures the average squared difference between predicted and actual values.  
- **R² Score**: Indicates how well the regression model explains variability in the target variable.  
- **Accuracy**: Since the target variable is binary (0 or 1), predictions are converted into classes (≥0.5 = 1, <0.5 = 0).

---

##  Technologies Used

- Python 3.12  
- Pandas  
- Scikit-learn  

---

##  Future Improvements

- Use Logistic Regression instead of Linear Regression (better suited for binary classification).  
- Perform feature scaling for improved model performance.  
- Add a confusion matrix and classification report for deeper evaluation.  

---

##  License

This project is licensed under the MIT License.
