# NHANES: Questions & Analysis

### Question 1: "Is there an association between marital status (married or not married) and education level (bachelor’s degree or higher vs. less than a bachelor’s degree)?"

- Test: Chi-square test (Chosen due to both variables being categorical).
- Preparation: Recoded `DMDMARTZ` and `DMDEDUC2` into binary categories.
- Results: Calculated chi-square statistic and p-value, followed by a bar plot visualizing the distribution. The data indicates that regardless of marital status, individuals tend to hold a bachelor's degree or higher.

### Question 2: "Is there a difference in the mean sedentary behavior time between those who are married and those who are not married?"

- Test: T-test (Chosen due to variables being continuous and categorical).
- Preparation: Cleaned `PAD680` by removing placeholder values (`7777`, `9999`) and recoded marital status.
- Result: Mean values and t-test results were visually displayed and showed that the observed effect or difference is statistically significant.

### Question 3: "How do age and marital status affect systolic blood pressure?"

- Test: ANOVA (Chosen due to being more than 2 variables).
- Preparation: Defined the OLS model with the correct 'data' argument.
- Result: Reported F-statistic and p-values for interpreting age and marital status’s influence on blood pressure. The graph indicates little to no correlation between marital status and systolic blood pressure. However, it reveals a trend of increasing systolic blood pressure with age.

### Question 4: "Is there a correlation between self-reported weight and minutes of sedentary behavior?"

- Test: Pearson’s correlation coefficient (Chosen due to both variables being continuous).
- Preparation: Cleaned `WHD020` and `PAD680` for outliers (`7777`, `9999`).
- Result: Displayed correlation coefficient and p-value. The graph indicates that there is a weak correlation between self-reported weight and minutes of sedentary behavior but the correlation is statistically significant.

### Question 5 (Creative Analysis): "Is there a difference in the mean sedentary behavior time between education status?"

- Test: T-test (Chosen due to variables being continuous and categorical).
- Preparation: Cleaned `PAD680` by removing placeholder values (`7777`, `9999`) and recoded data for education status `DMDEDUC2` into binary category.
- Results: Mean values and t-test results displayed that the observed effect or difference is statistically significant at any reasonable significance level but there is little to no difference between sedentary behavior time and education status.
