# Heart Disease Analysis and Prediction

## Introduction

This project aims to analyze the **Cardiovascular Disease Dataset** to predict the likelihood of heart disease using various patient health metrics. The project is built using **Python** with popular data science libraries and Apache Spark for big data processing.

------------------------------------------------------------------------

## Project Structure

```bash
├── Data_Visualization.ipynb    # Data visualization and insights
├── modelling.ipynb            # Machine learning models implementation
├── Pre-processing.ipynb       # Data cleaning and preprocessing
└── README.md                  # Project documentation
```

------------------------------------------------------------------------

## Setup Environment

1. Clone the repository:
   ```bash
   git clone https://github.com/nguyenthanhdat-dnat/Cardio_Analysis_Prediction.git
   cd Cardio_Analysis_Prediction
   ```

2. Install required libraries:
   ```bash
   pip install pyspark pandas numpy matplotlib seaborn scikit-learn boto3 kagglehub
   ```

------------------------------------------------------------------------

## Dataset

- **Source**: Cardiovascular Disease dataset from Kaggle
- **Description**: The dataset includes the following key features:
  - `age_years`: Age of the patient (in years)
  - `gender`: Gender (1: Female, 2: Male)
  - `height`: Height in cm
  - `weight`: Weight in kg
  - `ap_hi`: Systolic blood pressure
  - `ap_lo`: Diastolic blood pressure
  - `cholesterol`: Cholesterol levels (1: Normal, 2: High, 3: Very high)
  - `gluc`: Glucose levels (1: Normal, 2: High, 3: Very high)
  - `smoke`: Smoking status (0: No, 1: Yes)
  - `alco`: Alcohol intake (0: No, 1: Yes)
  - `active`: Physical activity (0: No, 1: Yes)
  - `cardio`: Target variable - presence of heart disease (0: No, 1: Yes)

------------------------------------------------------------------------

## Analysis Process

1. **Data Preprocessing**
   - Removed invalid height values (< 100cm or > 220cm)
   - Filtered out unrealistic weight records (< 30kg or > 180kg)
   - Cleaned blood pressure readings (removed negative and extremely high values)
   - Calculated BMI from height and weight
   - Standardized age values to years

2. **Exploratory Data Analysis (EDA)**
   - Distribution analysis of numerical features
   - Boxplots comparing variables across cardio groups
   - Histogram comparisons for key metrics
   - Categorical variable analysis using countplots

3. **Machine Learning Modeling**
   - Feature engineering and scaling
   - Model implementation using PySpark ML
   - Train-test split (80-20)
   - Model evaluation and performance metrics

4. **Key Findings**
   - Correlation between blood pressure and heart disease
   - Impact of cholesterol levels on cardiovascular health
   - Age distribution patterns in heart disease cases

------------------------------------------------------------------------

## Visualization Examples

The project includes various visualizations:
- Boxplots comparing health metrics between healthy and cardiac patients
- Distribution plots for age, BMI, and blood pressure
- Count plots for categorical variables

------------------------------------------------------------------------

## Future Improvements

- [ ] Implement more advanced machine learning models
- [ ] Add real-time prediction capabilities
- [ ] Include feature importance analysis
- [ ] Develop a web interface for predictions

------------------------------------------------------------------------

## Author & Contributions

- **Author**: Nguyen Thanh Dat
- **GitHub**: [nguyenthanhdat-dnat](https://github.com/nguyenthanhdat-dnat)

Contributions are welcome through Pull Requests or Issues.