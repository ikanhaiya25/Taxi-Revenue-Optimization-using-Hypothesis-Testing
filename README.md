
# Taxi-Revenue-Optimization-using-Hypothesis-Testing
The study specifically compares two common payment methods card and cash to identify whether one leads to higher average fares.

### Objective

The primary objective of this project is to examine the relationship between payment type and fare amount using statistical techniques. By applying hypothesis testing, the project aims to determine whether the difference in fares between card and cash payments is statistically significant.

⸻

### Methodology

1. Data Cleaning and Preprocessing

The dataset initially contained multiple columns, out of which only relevant features were selected. Invalid values such as negative fares, trip distances, and durations were removed. Additionally, outliers were handled using the Interquartile Range (IQR) method to ensure the reliability of the analysis.

2. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand patterns in the data. This included:
	•	Distribution of fare amounts and trip distances
	•	Comparison of payment types
	•	Passenger count analysis across different payment methods

These visualizations helped identify trends and supported further statistical testing.

3. Statistical Analysis

To determine the appropriate test, the distribution of fare amounts was examined using a QQ plot, which indicated that the data does not follow a normal distribution.

As a result, a Welch’s T-test was applied to compare the mean fare amounts between card and cash payments. This test is suitable when population variance is unknown and sample sizes may differ.

⸻

### Key Findings

The results of the hypothesis test showed that the p-value is lower than the significance level (0.05). Therefore, the null hypothesis was rejected, indicating that there is a statistically significant difference in fare amounts between the two payment methods.

It was observed that customers paying via card tend to have higher average fares compared to those paying with cash.

⸻

### Business Insight

The findings suggest that encouraging customers to use card payments can potentially increase driver revenue. This insight can be useful for taxi platforms and drivers when designing strategies to promote digital payments without negatively impacting customer experience.

⸻

### Tech Stack

	•	Python
	•	Pandas
	•	NumPy
	•	Matplotlib
	•	SciPy
	•	Statsmodels

  ## How to Run
  Install the required libraries:
  
	pip install -r requirements.txt

  ## 	Open the Jupyter Notebook:
  	jupyter notebook

  ## Conclusion

This project demonstrates how data analysis and hypothesis testing can be used to extract meaningful business insights. By combining data cleaning, visualization, and statistical testing, the analysis provides a clear understanding of how payment behavior influences revenue in the taxi industry.
