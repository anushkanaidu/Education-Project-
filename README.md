# Education project.

Purpose: This project explores how socioeconomic factors relate to average student performance on standardized tests (ACT/SAT) across U.S. schools.

---
## Project Overview

This project explores the question: How do socioeconomic factors relate to average student performance on the ACT or SAT exams across U.S. schools?

In this analysis, we use two datasets, one from EdGap.org and another from the National Center for Education Statistics (NCES).

The EdGap_data.xlsx file includes 2016 data on school's average ACT/SAT scores and several socioeconomic variables such as household income, unemployment rate, adult education level, and family structure.
The ccd_sch_029_1617_w_1a_11212017.csv dataset provides school level details like name, type, level, and location.

We will:

- Explore, clean, and merge the datasets
- Handle missing or inconsistent values
- Visualize relationships between socioeconomic indicators and ACT/SAT performance
- Identify which factors show the strongest association with student performance
  
By the end of this project, we will understand how economic and social conditions influence educational outcomes across different school communities in the United States.

---
## Repository Structure

Weather-project/

    ├── weather/                # Core project folder

    ├── code/                   # Jupyter notebooks and Python scripts
    
    ├── data/                   # Raw and processed data
    
    ├── License                 # Project license
    
    ├── Weather Report.pdf      # Generated report and visualizations
    
    ├── requirements.txt        # Dependencies
    
    └── README.md               # Project documentation 

---
## Data

In this analysis, we use two datasets, one from [**EdGap.org**](https://www.edgap.org/#5/37.892/-95.977) and another from the [**National Center for Education Statistics (NCES)**](https://nces.ed.gov/ccd/pubschuniv.asp).
The [EdGap_data.xlsx](https://github.com/brian-fischer/DATA-5100/blob/main/EdGap_data.xlsx) file includes 2016 data on school's average ACT/SAT scores and several socioeconomic variables such as household income, unemployment rate, adult education level, and family structure.  
The [ccd_sch_029_1617_w_1a_11212017.csv](https://www.dropbox.com/s/lkl5nvcdmwyoban/ccd_sch_029_1617_w_1a_11212017.csv?dl=1) dataset provides school level details like name, type, level, and location.

---
## Requirements

To run the code, install the following:

pandas

numpy

matplotlib

seaborn

scikit-learn

statsmodels

---
## Analysis

The analysis for this project is done in one notebook: **`weather/code/Notebook_education.ipynb`**.  
**Follow the steps below to reproduce the results.**

1. Explore the Data – Review the datasets to understand the key socioeconomic variables related to ACT/SAT performance.

2. Visualize Relationships – Create pair plots and heat maps to see how factors like unemployment, education level, and free/reduced lunch rates relate to test scores.

3. Build Models 
- Start with a simple linear regression using household income.
- Add a quadratic term to test for non-linear patterns.
- Use multiple regression to include all socioeconomic factors.
- Create a reduced model using only significant predictors: unemployment, adult education, and free/reduced lunch percentage.

4. Compare Models – Check model accuracy using R², RMSE, and MAE. The reduced model explained about 63% of the variation in ACT/SAT scores, performing nearly as well as the full model.

5. Validate Results – Review the residual plot to confirm that the model fits well and meets regression assumptions.

6. Findings - Summarize the findings and indicate which socioeconomic factors are the strongest predictors of student test performance
---

**Note:**  
Run the cells from top to bottom in the notebook. Each step depends on the previous one.

---
## Findings

This project studied how socioeconomic factors affect average ACT/SAT scores in U.S. schools.

- The results showed a strong connection between community conditions and student performance on ACT/SAT scores.
- Schools in areas with: Lower unemployment rates, more adults with college degrees and fewer students receiving free lunch
tend to have higher average test scores.
- The reduced multiple linear regression model, using only these three predictors, explained about 62.8% of the variation in ACT/SAT scores (R² = 0.628).
- This reduced model performed as well as the full model, showing that these three factors are the most important predictors of student achievement.
- Overall, the analysis suggests that communities with stronger economic and educational support systems help students perform better on standardized tests, showing how socioeconomic conditions shape educational outcomes.
  
---
## Authors
**Anushka Naidu Maddisetty** – (https://github.com/anushkanaidu)

---

## License
This project is licensed under the **MIT License** – see the ([LICENSE](https://github.com/anushkanaidu/Weather-project/blob/main/weather/License)) file for details.

---

## Acknowledgements
**Tools and Libraries Used:**  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Seaborn](https://seaborn.pydata.org/)  
- [Matplotlib](https://matplotlib.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)  
- [Statsmodels](https://www.statsmodels.org/stable/index.html)  

**Data Source:**  
- [EdGap.org – Education Opportunity Project](https://edopportunity.org/)  
- [National Center for Education Statistics (NCES)](https://nces.ed.gov/)  

**Inspiration and Guidance:**  
- Seattle University **DATA-5100 (Foundations of Data Science)** project template.  
- Course instructor and peers for feedback and support.
