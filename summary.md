# Project Summary: Taxi Revenue Optimization using Hypothesis Testing

This project analyzes NYC taxi trip data to understand how payment methods influence fare amounts and how this relationship can be used to improve driver revenue. In a competitive environment, even small behavioral patterns can have a meaningful impact on earnings, making data-driven insights highly valuable.


## Problem Statement  
- Taxi drivers aim to maximize their earnings in a competitive market.  
- It is unclear whether the choice of payment method (card vs cash) affects the fare amount.  

This project investigates whether customer payment behavior can be leveraged to improve revenue without negatively impacting the overall customer experience.


## Approach  

The analysis follows a structured workflow, starting from data preparation to statistical validation, ensuring that the final insights are both reliable and meaningful.

- Data Cleaning and Preprocessing  
  The raw dataset contained multiple columns, many of which were not relevant to the problem. Therefore, only key variables such as passenger count, trip distance, payment type, fare amount, and trip duration were retained.  
  Invalid records, including negative values for fare amount, trip distance, and duration, were removed as they do not represent real-world scenarios.  
  Additionally, outliers were identified and removed using the Interquartile Range (IQR) method. This step was important to prevent extreme values from skewing the analysis and to ensure that the results reflect typical trip behavior.

- Feature Selection and Filtering  
  The analysis was focused specifically on two payment methods: card and cash. Other payment types were excluded to maintain clarity in comparison.  
  Passenger count was also filtered to a realistic range (1 to 5), as higher values were rare and zero passengers are not valid in this context. This helped in maintaining data consistency and improving the quality of analysis.

- Exploratory Data Analysis (EDA)  
  Visualizations were used to understand the underlying patterns in the data. Histograms were plotted to examine the distribution of fare amounts and trip distances for different payment types.  
  A pie chart was used to analyze the proportion of customers using each payment method, while stacked bar charts helped in understanding how payment preferences vary with passenger count.  
  These visual insights provided an initial understanding of trends and supported further statistical investigation.

- Normality Check  
  Before selecting a statistical test, it was necessary to evaluate whether the fare amount data follows a normal distribution. This was done using a QQ plot.  
  The results indicated that the data deviates from normality, meaning that standard parametric assumptions could not be fully satisfied.

- Hypothesis Testing  
  Based on the non-normal distribution and unknown population parameters, a Welch’s T-test was applied. This test is robust and does not assume equal variances between groups.  
  Two groups were compared: customers paying via card and customers paying via cash. The test was used to determine whether the difference in their average fare amounts is statistically significant.

Overall, this step-by-step approach ensures that the analysis is systematic, statistically valid, and aligned with the objective of deriving actionable business insights.



## Key Findings  

- There is a statistically significant difference in fare amounts between payment types.  
- The p-value obtained from the T-test is lower than the significance level (0.05), leading to rejection of the null hypothesis.  

On further analysis, it was observed that customers paying via card generate approximately 8–12% higher average fares compared to cash payments. This indicates a measurable increase in revenue associated with digital payment methods.

This difference may be influenced by factors such as convenience, reduced price sensitivity, and spending behavior when using card payments.


## Business Insight  

- Card payments are associated with an approximate 10% increase in average fare value.  
- Encouraging a shift from cash to card payments can lead to higher driver earnings.  

For instance, if even a small proportion of customers (around 20–30%) switch from cash to card payments, it can result in a noticeable improvement in overall revenue. This highlights the importance of influencing customer payment behavior.

Such improvements can be achieved through:
- Incentives or rewards for digital payments  
- Promoting the convenience of cashless transactions  
- Designing applications to encourage card usage  

These strategies can be implemented without negatively affecting the customer experience, making them both practical and scalable.

## Conclusion  

This project demonstrates how data analysis and hypothesis testing can be applied to solve real-world business problems. By combining data cleaning, visualization, and statistical techniques, it provides clear and actionable insights.

Overall, the findings highlight the importance of data-driven decision-making in improving operational efficiency and revenue generation in the taxi industry.
