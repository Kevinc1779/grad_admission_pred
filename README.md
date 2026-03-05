# Graduate Admissions Prediction Using Regression (R)

This project analyzes factors influencing graduate school admission probability using regression modeling in R. The goal is to understand which academic metrics most strongly influence admission chances and build a statistical model to estimate admission probability.

## Dataset

The dataset contains **400 graduate school applicants** with the following variables:

- GRE score
- TOEFL score
- University rating
- Statement of Purpose (SOP)
- Letter of Recommendation strength (LOR)
- Undergraduate GPA (CGPA)
- Chance of admission (response variable)

The dataset was analyzed using exploratory data analysis and regression modeling.

## Project Workflow

The analysis followed these steps:

1. Data loading and preprocessing
2. Exploratory Data Analysis (EDA)
3. Summary statistics for key variables
4. Distribution visualization using histograms
5. Scatter plot analysis of predictors vs admission chance
6. Correlation analysis
7. Simple linear regression for each predictor
8. Multiple linear regression model construction
9. Model reduction based on statistical significance
10. Generation of confidence intervals and prediction intervals

## Model Development

Initial regression models were built for each independent variable individually.

Correlation analysis showed that the strongest relationships with admission chance were:

- **CGPA (0.873)**
- **GRE (0.803)**
- **TOEFL (0.792)**

A full multiple regression model was constructed using all predictors:

GRE + TOEFL + Urate + SOP + LOR + CGPA

Statistical testing indicated that **University Rating and SOP were not significant predictors**, so a reduced model was constructed.

### Final Regression Model

The final model includes:

- GRE
- TOEFL
- LOR
- CGPA

## Results

The reduced regression model achieved:

- **R² ≈ 0.798**
- **Adjusted R² ≈ 0.796**

This indicates the model explains approximately **80% of the variability in admission probability**.

Among all predictors:

- **CGPA was the strongest individual predictor**
- GRE and TOEFL also showed strong positive relationships with admission chance.

The model was then used to generate:

- **95% confidence intervals**
- **95% prediction intervals**

for predicted admission probabilities.


## Tools Used

- R
- RMarkdown
- Linear Regression
- Correlation Analysis
- Statistical Modeling

## Key Insights

- Undergraduate GPA (CGPA) is the strongest predictor of graduate admission probability.
- GRE and TOEFL scores significantly improve prediction accuracy.
- A reduced regression model can maintain predictive performance while simplifying interpretation.
