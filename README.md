# HR Attrition in IBM

## Executive Summary

This project analyzes IBM HR attrition using Kaggle data to identify trends, key factors influencing attrition, and build predictive models. We followed the CRISP-DM methodology for data mining and evaluated models to improve IBM HR's strategic decision-making.

## Data Overview

- **Source:** Kaggle HR Attrition dataset
- **Records:** 1,470 employees, 33 attributes
- **Key Features:** Age, Monthly Income, Job Role, Work-life Balance, Overtime, Attrition Status

## Data Preprocessing

- Removed missing values (e.g., `Date_of_Termination`)
- Used **Variance Inflation Factor (VIF)** for feature selection
- Applied **SMOTE** to handle class imbalance
- Final dataset: 2,418 observations, 25 attributes

## Exploratory Data Analysis (EDA)

<table>
<tr>
<td align="center"><img src="https://github.com/user-attachments/assets/4172c10e-5d71-4eaa-a81f-05a9c55f8634" width="45%"></td>
<td align="center"><img src="https://github.com/user-attachments/assets/802f2df5-c46b-4568-b4aa-d035761db0ab" width="45%"></td>
</tr>
<tr>
<td align="center"><img src="https://github.com/user-attachments/assets/7f5f98a8-f250-4bb2-90bf-e5c0f8ea8451" width="45%"></td>
<td align="center"><img src="https://github.com/user-attachments/assets/d87bbb6a-db53-4908-9fd8-8fb611af522d" width="45%"></td>
</tr>
</table>


- **Attrition Rate:** 16% of employees left, primarily under age 40.
- **Overtime:** No significant impact on attrition.
- **Distance from Home:** Employees farther from work showed higher attrition.
- **Departmental Trends:** HR & Sales had higher attrition compared to R&D.
- **Gender & Salary Disparity:** Female employees in senior roles had higher attrition.

  

## Predictive Modeling

We applied **Naïve Bayes, Decision Tree, and Random Forest** for classification:

| Model           | Accuracy  | Sensitivity | Specificity | Cost ($) |
|----------------|-----------|------------|------------|---------|
| Random Forest  | 89.62%    | 92%        | 87.11%     | 2,735   |
| Naïve Bayes    | 79.86%    | 77.97%     | 81.58%     | 7,360   |
| Decision Tree  | 76.71%    | 79.34%     | 74.02%     | 7,917   |

### Best Model: **Random Forest**
- **Highest accuracy (89.62%)** and lowest cost ($2,735).
- **Key Influencing Factors:** Monthly Income, Overtime, Job Level, Work-Life Balance.

## Conclusions & Recommendations

- **Address Salary Disparities:** Reduce gender pay gaps to retain top talent.
- **Improve Work-Life Balance:** Especially in HR & Sales departments.
- **Optimize Hiring & Training Costs:** Use the Random Forest model to predict attrition risks and allocate HR resources efficiently.


