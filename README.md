#  Chilean College Admissions Descriptive/Diagnostic Analysis.
## Description
This project focuses on analyzing the Chilean college admissions dataset and exploring various factors related to demographics, income levels, education, and test scores. The analysis involves data cleaning, transformation, and visualization to derive meaningful insights.

The Column Descriptions of the CSV:
•MRUN: Application number.

•DOB: date of birth.

•Gender: Male or Female

•Family size: number of people that live with the student.

•How many in your family work: number of people that work within the family.

•Income level: categorical variable representing monthly income, as detailed in the next Table: 
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/ea71f2bb-4df9-4fea-8647-abe3b02c56b0)

•Level education father/mother: categorical variable representing the maximum level of
education attained by the parents, as detailed in the next table:
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/c1d6e0bb-ca16-40e3-9488-da147b725ff7)

•High School Type: The type of Highschool student is from i.e. 2-Public, 3-voucher, 4-Private.

•Scores: NEM, LYC, MATE, HYCS, CIEN scores of applicants.

## These are the steps that were followed to conduct the analysis and derive the insights:

### Data Cleaning and Transformation
Separated Demographics data into columns using text-to-columns with a delimiter.
Converted the data into a table for better organization and analysis.
Filtered irrelevant, wrong, or duplicated data, such as DOB with 0 and income level zero.

### Age Calculation
Computed the current age of each student using their date of birth (DOB) in the DMMYYYY format using the DATEDIF function.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/3f92bd31-1fcd-4bb5-88d7-b3353577208a)

### Median Monthly Income Analysis
Calculated the median monthly income for each income level, considering the middle point for each range.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/ff0b7d09-fa78-4695-b704-84127a90028f)

### Relation between Income and Parent's Education Level
Analyzed the relationship between the median monthly income per family member and the level of education of the father and mother using a pivot table.
Identified that education levels were proportional to median monthly income, with fluctuations and a peak at level 9.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/ca4592dd-6f6e-452b-b47e-15ef22713034)

### Effect of Family Size on NEM Score
Used a pivot table to explore the effect of the number of family members on the NEM score.
Found that the NEM scores remained steady with minimal fluctuations, reaching their highest average scores at 1 and 11 family members.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/86a91af6-dfa5-44d1-bc96-32e796bbdd8b)

### Impact of Parent's Education Level on Test Scores
Computed the average scores between Math (MATE) and Language (LYC) based on the mother's and father's education levels.
Analyzed that the mother's scores had a bigger effect than the father's on the average scores, particularly with the increase in income.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/3f2186aa-8730-4173-b7e8-433e54087f0e)
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/7bbba7aa-90f3-4e2f-b549-c8aee87118cd)

### Effect of Income Level on Test Scores
Examined the effect of the level of income on NEM, MATE, CIEN, HYC, and LYC average scores.
Observed a steady increase with fluctuations, reaching their peak at specific income levels.
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/939fe451-27c3-457f-8ff5-b2f519a21ef7)

### Relationship between High School Type and Income Level
Explored the relationship between high school types (HST) and income levels.
Identified that students with income levels 1 and 2 predominantly opted for public schools (HST-2), while higher-income students preferred private schools (HST-4).
![image](https://github.com/JeevanBhargav/Chilean-college-admissions-case./assets/130612387/73205c33-ee59-498e-99f2-72c1fbff71f0)

## Conclusion
Through the analysis of the Chilean college admissions dataset, several insights were gained regarding the relationship between income, education, family size, and test scores. The findings suggest a correlation between higher education levels and median monthly income, as well as the impact of family size on the NEM scores. The influence of parents' education levels on test scores was also examined, revealing a stronger effect from the mother's education level. Additionally, the analysis highlighted the association between income levels and test scores, as well as the preference for different high school types based on income levels.





