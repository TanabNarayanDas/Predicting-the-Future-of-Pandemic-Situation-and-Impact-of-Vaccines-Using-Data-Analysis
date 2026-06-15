# Virus Spread Prediction and Vaccination Impact Analysis

## Project Overview

This project analyzes virus spread trends using historical COVID-19 data and applies various machine learning and statistical models to predict future infections. It also evaluates the impact of vaccination, vaccine effectiveness, booster doses, and mortality rates on disease transmission.

The project combines:

* Data visualization
* Linear Regression
* Logistic Growth Modeling
* Vaccination Impact Analysis
* Time-Series Validation
* Ridge Regression
* Mortality Prediction
* Geographic Visualization

---

## Features

### 1. Historical Data Visualization

* Visualizes daily virus cases.
* Uses line charts to identify infection trends over time.

### 2. Linear Regression Prediction

* Predicts future infection counts using:

  * SciPy Linear Regression
  * Scikit-Learn Linear Regression

### 3. Logistic Growth Modeling

* Models disease spread using a logistic growth curve.
* Estimates carrying capacity and infection growth rate.

### 4. Vaccination Impact Analysis

* Simulates how vaccination reduces virus transmission.
* Incorporates:

  * Vaccine effectiveness
  * Vaccination rate
  * Reduced infection growth rate

### 5. Moving Average Trend Analysis

* Calculates:

  * 7-Day Moving Average (MA)
  * 7-Day Exponential Moving Average (EMA)
* Helps smooth fluctuations in reported cases.

### 6. Time-Based Cross Validation

* Evaluates model performance using chronological splits.
* Calculates Mean Squared Error (MSE).

### 7. Ridge Regression

* Applies regularization to reduce overfitting.
* Compares performance with standard linear regression.

### 8. Booster Dose and Waning Immunity Model

* Simulates:

  * Declining vaccine effectiveness over time
  * Impact of booster vaccinations
* Adjusts virus growth rate dynamically.

### 9. Mortality Prediction

* Estimates mortality counts under:

  * No vaccination scenario
  * Vaccination and booster scenario

### 10. Country-Wise Death Visualization

* Generates an interactive world choropleth map.
* Displays death counts by country.

---

## Dataset

The project uses:

**country_wise_latest.csv**

Expected columns include:

| Column Name    | Description               |
| -------------- | ------------------------- |
| Country/Region | Country Name              |
| New cases      | Daily new confirmed cases |
| New recovered  | Daily recovered cases     |
| Deaths         | Total deaths              |

Dataset Source:
COVID-19 Country-wise Statistics Dataset

---

## Technologies Used

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Scikit-Learn
* Plotly

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/virus-spread-prediction.git

cd virus-spread-prediction
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn plotly
```

---

## Project Structure

```text
Virus-Spread-Prediction/
│
├── country_wise_latest.csv
├── virus_prediction.py
├── README.md
│
├── Visualizations
│   ├── Historical Spread
│   ├── Logistic Growth
│   ├── Vaccination Impact
│   ├── Heatmap Analysis
│   └── Country Death Map
│
└── Models
    ├── Linear Regression
    ├── Ridge Regression
    ├── Logistic Growth Model
    └── Vaccine Effectiveness Model
```

---

## Workflow

### Data Preparation

1. Load COVID-19 dataset
2. Create time index (`Days`)
3. Extract:

   * Cases
   * Recovered Cases
   * Vaccination Proxy Data

### Exploratory Analysis

* Historical spread visualization
* Trend smoothing using MA and EMA

### Predictive Modeling

#### Linear Regression

Predict future infections based on historical trends.

#### Logistic Growth Model

Model epidemic growth and saturation.

#### Vaccine-Aware Logistic Model

Adjust infection growth rate using vaccination effectiveness.

### Validation

* Time-Based Cross Validation
* Mean Squared Error Evaluation
* Ridge Regression Comparison

### Advanced Analysis

* Waning immunity simulation
* Booster dose effectiveness
* Mortality forecasting

### Visualization

* Trend plots
* Prediction curves
* Heatmaps
* Global death distribution maps

---

## Sample Outputs

### Historical Virus Spread

* Daily infection trend visualization.

### Virus Spread Prediction

* Actual vs Predicted Cases.

### Vaccination Impact

* Infection reduction due to vaccination.

### Heatmap Analysis

* Relationship between vaccine effectiveness and spread rate.

### Mortality Comparison

* Mortality with and without vaccination.

### Country-Wise Death Map

* Interactive global visualization using Plotly.

---

## Evaluation Metrics

The project uses:

### Mean Squared Error (MSE)

```text
MSE = (1/n) Σ(y_actual − y_predicted)²
```

Used to evaluate:

* Linear Regression
* Ridge Regression
* Time-Based Cross Validation

---

## Future Improvements

* Incorporate real vaccination datasets.
* Use ARIMA and LSTM models for forecasting.
* Add hospitalization prediction.
* Include age-group based analysis.
* Develop a real-time dashboard using Streamlit or Flask.
* Integrate live COVID-19 APIs.

---

## Conclusion

This project demonstrates how statistical modeling and machine learning techniques can be used to analyze virus spread patterns and evaluate vaccination strategies. By combining regression models, logistic growth analysis, booster effectiveness simulations, and geographic visualizations, the system provides insights into disease progression and public health interventions.

---

## Author

**Tanab Narayan Das**

Project: Virus Spread Prediction and Vaccination Impact Analysis

Year: 2026
