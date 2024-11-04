# Life-Expectancy-prediction
Life Expectancy Prediction through the use of an Epidemiological Database.

1- Introduction:
The database used to model Life Expectancy can be classified as an epidemiological and public health dataset on a global level, and it comprises the following variables:

Types of statistical variables:
Qualitative Nominal Variables: Country (object) and Status (object).
Quantitative Discrete Variables: Year (int64), Infant Deaths (int64), Measles (int64), and Deaths under five years (int64).
Quantitative Continuous Variables: Life Expectancy (float64), Adult Mortality (float64), Alcohol (float64), Percentage Expenditure (float64), Hepatitis B (float64), BMI (float64), Polio (float64), Total Expenditure (float64), Diphtheria (float64), HIV/AIDS (float64), GDP (float64), Population (float64), Thinness 1-19 years (float64), Thinness 5-9 years (float64), Income Composition of Resources (float64), and Schooling (float64).

2- Exploratory Data Analysis (EDA) and Data Cleaning:
The variables most strongly correlated with Life Expectancy are:

Adult Mortality
BMI (Body Mass Index)
Based on univariate and bivariate exploratory analysis, anomalous values (outliers) in the dependent variable, Life Expectancy, and the independent variable, Adult Mortality, were removed to eliminate secondary trends.

3- Life Expectancy Model:
A linear regression model was used, applying the Ordinary Least Squares (OLS) method.

4- Results:
In a preliminary test, the independent variable “Adult Mortality” was used without removing outliers. After running the model, the R-squared was 0.55, which is considerably lower compared to the model where outliers in Life Expectancy and Mortality were removed (R-squared = 0.86).

The filtered dataset without outliers increased the positive correlation between Life Expectancy and Adult Mortality, resulting in a more efficient predictive model. An R² of 0.86 indicates that the model is quite effective in predicting the values of the dependent variable, though it is not perfect, with 14% of the variability remaining unexplained by the model.
