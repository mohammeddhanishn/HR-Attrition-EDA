# HR Analytics: Employee Attrition EDA

An exploratory data analysis of employee records to understand how attrition varies across age groups, departments, job roles, overtime, satisfaction, work-life balance, and business travel.

## 1. Business Question

Which employee groups show higher attrition in this dataset, and what workforce patterns should HR investigate to support retention?

## 2. Dataset

- **Dataset:** HR Analytics (`HR_Analytics-4.csv`)
- **Size:** 1,480 rows and 37 columns before cleaning; 1,478 rows after removing 2 duplicate rows.
- **Content:** Employee demographics, department and job details, compensation, satisfaction ratings, tenure, overtime, travel, and attrition status.
- **Source:** The notebook loads a local CSV file, but the dataset source URL is not recorded in the notebook. Add the original public dataset link here before publishing: **[Add dataset source URL]**.
- **Data file:** Add `HR_Analytics-4.csv` to this repository if its license permits, or update the notebook to download/read it from the source above. Do not leave the notebook pointing to a local computer path.

## 3. Tools Used

- Python 3
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook

## 4. Steps Followed

1. Loaded the employee dataset with Pandas and checked its shape, columns, data types, and summary statistics.
2. Checked missing values and duplicate records. The notebook fills the 61 missing `YearsWithCurrManager` values with the median (3 years) and removes 2 duplicate rows.
3. Removed constant or non-informative columns: `EmployeeCount`, `Over18`, and `StandardWorkingHours`.
4. Compared attrition across employee groups and created visualizations for age group, gender, department, job role, business travel, job satisfaction, overtime, monthly income, and work-life balance. A correlation chart explores numeric feature relationships.

## 5. Key Insights

Based on the notebook's cleaned data and group-level comparisons:

1. **Overall attrition:** 239 of 1,478 employees left, an attrition rate of about **16.17%**.
2. **Age:** Employees aged 18–25 had the highest age-group attrition rate at about **36.6%**. The 36–45 group had the lowest rate at about **9.1%**.
3. **Overtime:** Attrition was about **31.0%** among employees working overtime, compared with **10.3%** among those not working overtime.
4. **Department:** Sales had the highest department attrition rate (about **25.2%**), followed by Human Resources (about **23.1%**). Operations had the lowest rate (about **8.3%**).
5. **Job role:** Sales Representatives had the highest job-role attrition rate (about **40.5%**); Research Directors had the lowest (about **2.5%**).
6. **Satisfaction:** Attrition was highest among employees with job satisfaction level 1 (about **23.1%**) and lowest at level 4 (about **11.2%**).
7. **Work-life balance:** The lowest work-life balance rating (1) corresponded to the highest rate in this comparison (about **30.9%**).

These are associations in this dataset and do not establish that any one factor causes employees to leave. HR could investigate workload and retention conditions among overtime workers, younger employees, and sales roles.

## 6. Screenshots or Output

Charts and analysis outputs are included in the Jupyter Notebook. Keep the notebook outputs saved before committing it. For a more visual repository landing page, add selected chart images under `images/` and link them here.

## 7. How to Run or Open

1. Clone or download this repository.
2. Install the required packages:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. Place `HR_Analytics-4.csv` in the project folder (or update the notebook to use the dataset's public source URL).
4. Open and run `Sales Data Analysis with Python. Project 1 (3).ipynb` in Jupyter Notebook or JupyterLab.

**Before uploading:** Update the notebook's CSV path. It currently points to a file path on the author's computer, which will not work for other users. A relative path such as `pd.read_csv("HR_Analytics-4.csv")` will work when the CSV is in the repository folder.

## 8. Author

- **Name:** Mohammed Dhanish N
- **Program / project:** Project 1 — Data Analysis with Python (EDA)
