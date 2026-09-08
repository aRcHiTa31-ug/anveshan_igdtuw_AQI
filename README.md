# 🌍 AQI Prediction Using Machine Learning

A machine learning-based system for **Air Quality Index (AQI) prediction** using historical air pollution and meteorological data. The project compares multiple regression models and applies **Genetic Algorithm (GA)** for feature selection and **Differential Evolution (DE)** for hyperparameter optimization.

---

## 📌 Project Overview

Air pollution is a major environmental and public-health concern. Accurate AQI prediction can help authorities and individuals anticipate poor air-quality conditions and take preventive measures.

This project develops and evaluates several machine learning models for predicting AQI using historical air-quality data from India.

The study focuses on **Ahmedabad** and investigates whether intelligent feature selection and hyperparameter optimization can improve prediction performance.

---

## 🎯 Objectives

* Predict AQI using historical air-quality data.
* Compare different machine learning regression algorithms.
* Identify the most important features for AQI prediction.
* Use **Genetic Algorithm (GA)** for feature selection.
* Use **Differential Evolution (DE)** for hyperparameter optimization.
* Evaluate models using standard regression metrics.
* Identify the best-performing model for AQI prediction.

---

## 📊 Dataset

**Dataset:** Air Quality Data in India (2015–2020)

**Source:** Kaggle

The dataset contains historical air-quality measurements collected from monitoring stations across India.

For this project, the analysis focuses on **Ahmedabad**.

### Major Features

The dataset includes pollutants and environmental variables such as:

* PM2.5
* PM10
* NO
* NO₂
* NOx
* NH₃
* CO
* SO₂
* O₃
* Benzene
* Toluene
* Xylene
* Other relevant air-quality parameters

The target variable is:

**AQI — Air Quality Index**

---

## 🔄 Methodology

The overall workflow of the project is:

```text
Raw Dataset
     ↓
Data Cleaning & Preprocessing
     ↓
Missing Value Handling
     ↓
Exploratory Data Analysis
     ↓
Feature Selection using Genetic Algorithm
     ↓
Train-Test Split
     ↓
Machine Learning Models
     ↓
Hyperparameter Optimization using Differential Evolution
     ↓
Model Evaluation
     ↓
Best AQI Prediction Model
```

---

## 🤖 Machine Learning Models

The following regression models were evaluated:

### 1. Random Forest

An ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

### 2. XGBoost

A gradient boosting algorithm that builds an ensemble of decision trees sequentially and is highly effective for structured/tabular datasets.

### 3. Gradient Boosting

An ensemble technique that combines weak learners sequentially, with each new model attempting to correct the errors of previous models.

### 4. Stacking Regressor

A meta-learning approach that combines predictions from multiple base models to produce a final prediction.

---

## 🧬 Feature Selection — Genetic Algorithm

A **Genetic Algorithm (GA)** was used to identify an effective subset of features.

The GA works by:

1. Representing feature subsets as chromosomes.
2. Evaluating each feature subset using a fitness function.
3. Selecting better-performing solutions.
4. Applying crossover and mutation.
5. Repeating the process across generations.
6. Selecting the feature subset with the best performance.

This helps reduce unnecessary features while retaining the information most useful for AQI prediction.

---

## ⚙️ Hyperparameter Optimization — Differential Evolution

**Differential Evolution (DE)** was used to optimize model hyperparameters.

Instead of manually selecting hyperparameters, DE searches through the parameter space to identify combinations that improve model performance.

This optimization was applied to improve the predictive performance of the machine learning models.

---

## 📈 Evaluation Metrics

The models were evaluated using:

### R² Score

Measures how well the model explains the variation in the target variable.

Higher values indicate better performance.

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted AQI values.

Lower values are better.

### Root Mean Squared Error (RMSE)

Measures the square root of the average squared prediction error.

Lower values indicate better performance.

---

## 🏆 Results

Among the evaluated models, **Random Forest achieved the best performance**.

### Best Result

| Model             |  R² Score |
| ----------------- | --------: |
| **Random Forest** | **0.863** |

The Random Forest model achieved an **R² score of approximately 0.863**, indicating that it explained around **86.3% of the variance** in AQI in the evaluated dataset.

The complete experimental results and comparisons are available in the project files.

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Libraries

* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost

### Optimization Techniques

* Genetic Algorithm
* Differential Evolution

### Development Environment

* Jupyter Notebook / Google Colab
* GitHub

---

## 📁 Project Structure

```text
AQI-Prediction/
│
├── README.md
├── main.py
├── requirements.txt
│
├── Results.md
│
├── notebooks/
│   └── AQI_Prediction.ipynb
│
├── images/
│   ├── correlation_heatmap.png
│   ├── feature_importance.png
│   └── model_comparison.png
│
└── .gitignore
```

> Dataset files are not included in the repository if they are too large or subject to external dataset licensing. The dataset can be obtained from its original source.

---

## 🚀 Installation

Clone the repository:

```bash
git clone <your-github-repository-url>
cd AQI-Prediction
```

Create a virtual environment (optional):

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the main Python file:

```bash
python main.py
```

Alternatively, open the Jupyter Notebook:

```bash
jupyter notebook
```

and run the cells sequentially.

---

## 📊 Key Findings

* Machine learning models can effectively capture relationships between pollutant concentrations and AQI.
* Feature selection can reduce the number of input variables while maintaining useful predictive information.
* Hyperparameter optimization can improve model performance compared with default model configurations.
* Among the tested models, **Random Forest produced the strongest predictive performance**, with an R² score of approximately **0.863**.

---

## 🔮 Future Improvements

Possible future improvements include:

* Incorporating real-time air-quality data.
* Developing a web-based AQI prediction dashboard.
* Adding time-series models such as LSTM and GRU.
* Incorporating weather and meteorological information.
* Testing the models on additional Indian cities.
* Deploying the best-performing model as an API.
* Developing an early-warning system for severe air pollution events.

---

## 👩‍💻 Author

**Pihu**

B.Tech — Electronics & Communication Engineering (AI)

Indira Gandhi Delhi Technical University for Women (IGDTUW)

---

## 📄 License

This project is intended for **educational and research purposes**.
