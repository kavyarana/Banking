Banking

1. Problem Statement
Vehicle loan defaults cause significant financial losses for institutions, leading to stricter
underwriting and higher rejection rates. The aim of this project was to identify the factors influencing
loan defaults and to develop a predictive framework to estimate potential defaulters. This study
combines data preparation, exploratory analysis, and predictive modeling to provide a complete
solution.

2. Data Preparation (Excel)
The project began with a raw dataset containing 41 attributes. The data was imported into Excel for
initial cleaning and preprocessing.
Data Cleaning:
- Removed duplicate records to ensure data integrity.
- Standardized column names for consistency across the project's different tools.
- Handled missing values by replacing them with the median for numerical attributes and the mode
for categorical attributes.
- Verified the consistency of values across all attributes to prepare the data for visualization and
modeling.
After cleaning, the final dataset was exported for further analysis in Tableau and Python.

3. Exploratory Data Analysis (Tableau)
Using the cleaned data, I created 13 worksheets in Tableau to perform a thorough exploratory data
analysis (EDA). The goal was to visualize and understand the key relationships and patterns within
the data.
- Target Distribution: I analyzed the overall default rate, which was found to be approximately
21.71%.
- Default by Business Categories: I created visualizations to show defaults by Branch, Supplier, and
Manufacturer, identifying which specific categories had the highest default rates.
- Demographics: I explored default trends based on Age, noting a peak in defaults among
applicants in their late 20s and early 30s. I also analyzed the Employment Type of applicants,
finding a higher default tendency among the self-employed.
- Credit History: I investigated credit history metrics like Primary and Secondary Loan Details,
Credit Bureau Score Distribution, New Accounts in Last Six Months, Defaults in Last Six Months,
and Loan Inquiries. This analysis provided the foundation for my predictive modeling.
- ID Proof: I examined the distribution of different ID Proof Types used by customers.

4. Dashboarding (Tableau)
I built two interactive dashboards to present the insights from my worksheets clearly and effectively.
- Dashboard 1 (Executive Summary): Focused on high-level findings, including the Target
Distribution, Defaults by Branch, Supplier, and Manufacturer, and Demographic charts. This
dashboard provides a quick, strategic overview for stakeholders.
- Dashboard 2 (Credit History Dive): Dedicated to a detailed analysis of credit-related attributes,
including Primary Loans, Secondary Loans, New Credit History, Default Credit History, and
Inquiries.
Interactivity was added through filters and a structured layout to enhance the user experience and
enable a clear, guided storytelling of the data. Consistent formatting was used, with red
representing defaulters and blue representing non-defaulters.

5. Predictive Modeling (Python)
After visualizing the data, I used Python to build and evaluate a predictive model.
Model: A Logistic Regression model was applied to predict loan default.
Evaluation: The model's performance was evaluated using a Confusion Matrix, which was then
summarized in a text box and added to a dashboard in Tableau.
Confusion Matrix Results
Predicted No Default (0) Predicted Default (1)
Actual No Default (0) 1000 (True Negatives) 50 (False Positives)
Actual Default (1) 200 (False Negatives) 150 (True Positives)

6. Key Findings
Credit History: My analysis found that while Credit Bureau Score and Delinquent Accounts in the
Last Six Months are significant predictors of default, other credit history factors, such as New
Accounts and Inquiries, showed a very weak to non-existent correlation. Specifically:
- NEW.ACCTS.IN.LAST.SIX.MONTHS showed a very weak negative correlation with a score of
-0.03.
0.18.
- DELINQUENT.ACCTS.IN.LAST.SIX.MONTHS showed a weak positive correlation with a score of
- NO.OF_INQUIRIES showed a very weak positive correlation with a score of 0.04.
Inquiries: Customers with multiple loan inquiries show a higher risk of default.
Demographics: Certain employment categories (e.g., self-employed) and younger age groups
showed higher default tendencies.

7. Conclusion
This project successfully combined Excel (data cleaning), Tableau (EDA and dashboards), and
Python (predictive modeling and validation) to provide a comprehensive solution to the problem of
vehicle loan default. The insights gained from the analysis can help financial institutions refine their
loan approval process, better identify high-risk customers, and ultimately reduce losses from loan
defaults. Future work should focus on improving the predictive model to reduce false negatives.
