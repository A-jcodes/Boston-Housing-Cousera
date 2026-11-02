# Boston Housing Analysis

Statistical analysis of the Boston housing dataset (U.S. Census Service) for the IBM Statistics with Python course. The goal is to give a housing agency's management clear insights into what drives median home values.

## Dataset

506 areas in the Boston region, 13 variables, no missing values. Key variables:

| Variable | Meaning |
|---|---|
| MEDV | Median value of owner occupied homes ($1000s) |
| CHAS | Borders the Charles River (1 = yes, 0 = no) |
| AGE | Share of owner occupied units built before 1940 |
| NOX | Nitric oxide concentration (parts per 10 million) |
| INDUS | Share of non retail business acres per town |
| DIS | Weighted distance to five Boston employment centres |
| PTRATIO | Pupil to teacher ratio |

## Methods

Descriptive statistics, boxplots, bar plot, scatter plot and histogram, followed by five tests at a significance level of 0.05: Levene's test, Welch's t test, one way ANOVA, Pearson correlation and simple linear regression (OLS).

## Key Findings

1. **Charles River:** Areas bordering the river have significantly higher home values, averaging about $28,400 against $22,100 elsewhere (Welch's t test, p = 0.004).
2. **Housing age:** Home values differ significantly across age groups (ANOVA, F = 36.4, p < 0.001). Areas with the most pre 1940 homes have the lowest median, about $18,200, against $24,800 in the newest group.
3. **Pollution and industry:** Nitric oxide and industrial land share a strong positive relationship (r = 0.76, p < 0.001).
4. **Distance to jobs:** Each extra unit of distance from employment centres adds about $1,090 to home value (p < 0.001), but distance explains little of the overall variation (R squared = 0.062).

## Tools

Python, pandas, matplotlib, seaborn, SciPy, statsmodels

## Files

- `boston_housing_analysis.ipynb`: full notebook with code, charts and interpretations
