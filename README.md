# Graduate Admissions Prediction Using Regression

This project analyzes factors influencing graduate school admission probability using statistical modeling in R. The analysis explores relationships between academic metrics and admission outcomes, then builds regression models to predict admission chances.

## Dataset

The dataset contains information about graduate school applicants, including academic scores and recommendation metrics.

Variables included:

- GRE score
- TOEFL score
- University rating
- Statement of Purpose (SOP)
- Letter of Recommendation strength (LOR)
- Undergraduate GPA (CGPA)
- Chance of admission (response variable)

The dataset contains **400 applicant records**.

## Objectives

The goals of this analysis were:

- Explore relationships between academic variables and admission probability
- Identify the most important predictors of admission chances
- Build regression models to estimate admission probability
- Evaluate model performance using statistical metrics

## Methods

The following statistical techniques were used:

- Exploratory Data Analysis (EDA)
- Correlation analysis
- Simple linear regression
- Multiple linear regression
- Model selection using statistical significance
- Confidence and prediction interval estimation

## Model Development

Initial models evaluated each variable individually using simple linear regression.

Key findings:

- **CGPA showed the strongest relationship with admission chance**
- **GRE and TOEFL also had strong predictive power**

Final reduced model included:

- GRE
- TOEFL
- LOR
- CGPA

## Results

The final regression model achieved:

- **R² ≈ 0.80**
- All selected predictors were statistically significant (p < 0.05)

This indicates the model explains approximately **80% of the variation in admission probability**.


## Tools Used

- R
- RMarkdown
- Linear Regression
- Statistical Modeling
- Data Visualization

## Key Insights

- CGPA is the strongest predictor of graduate admission probability
- GRE and TOEFL scores also significantly influence admission chances
- A reduced regression model can maintain strong predictive power while simplifying interpretation

## Future Improvements

Possible improvements include:

- Testing nonlinear models
- Applying regularized regression methods (Ridge/Lasso)
- Incorporating additional applicant features
- Cross-validation for stronger model validation
