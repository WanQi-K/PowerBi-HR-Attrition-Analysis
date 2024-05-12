# PowerBi-HR-Attrition-Analysis

IBM HR Dashboard Analysis on Employee Attrition
As someone new to Power BI, I was eager to apply my growing data analysis skills to a real-world challenge: employee retention. Understanding the factors influencing employee departures and identifying high-risk groups is crucial for any organization seeking to build a stable and engaged workforce. Hence, I retrieved the dataset from Kaggle on IBM HR Dataset, a publicly available here (https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
Problem Statement: Unveiling the Drivers of Turnover
Understanding why employees leave is crucial for developing effective retention strategies. This analysis aims to identify the primary drivers of employee attrition and pinpoint specific employee groups with higher turnover rates and provide recommendations to counter this issue.

# Building the Dashboard: A Data-Driven Approach

Before developing the dashboard, I ensured the data is complete and cleaned out any duplicates data in PowerBi. Next, in order to make the data digestible, I organized it into subcategories like demographics, compensation, and job attributes. Attrition rates were quantified, allowing for calculations and analysis. DAX formulas were employed to create meaningful categories and measures were crafted to analyze attrition rate, average working years, and employee headcount.
For example, to quantity the Years In Current Role Category, below DAX function is used :

YearsInCurrentRole_Category = 
SWITCH(
    TRUE(),
    'HR-Employee-Attrition'[YearsInCurrentRole]<5,"Less than 5 Years",
    'HR-Employee-Attrition'[YearsInCurrentRole]>=5 && 'HR-Employee-Attrition'[YearsInCurrentRole]<10,"5-10 Years",
    "More than 10 Years"
    )
    
The interactive dashboard includes key features:
•	Dynamic Parameters: Users can explore multiple metrics within a single graph for a holistic view.
•	Interactive Slicers: The dashboard empowers users to filter based on specific criteria for a deeper dive.
•	Accessible Insights: An "information button" on each page unveils key takeaways.
Actionable Insights: Addressing the Retention Gap

The analysis yielded valuable insights with significant implications for HR strategies:
1.	New Hire Retention Gap: The data revealed the highest attrition rate among employees with less than five years of service. This highlights a need to improve on onboarding programs, performance reviews, and employee engagement initiatives.
2.	Stock Options Matter: A significant drop in attrition was observed among employees with stock options. This suggests that stock options should be a key consideration for future compensation and benefits plans.
3.	Engagement is Key: Job involvement emerged as the most crucial factor impacting retention. Disengaged employees were 2.24 times more likely to leave. Implementing measures to enhance engagement, challenge, and skill development can potentially significantly improve retention.

   
# Wrapping It Up
This project demonstrates the power of Power BI in transforming HR data into actionable insights. By fostering a data-driven culture, HR teams can gain a deeper understanding of their workforce, leading to a more engaged and productive employee pool.

What are your thoughts on leveraging data analytics for employee retention? Share your insights in the comments below!

**Reach out to me : kwanqi.yt@gmail.com**

