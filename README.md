Employee Performance Analytics using NumPy

1. Project Overview
- This project analyzes employee performance using pure NumPy.
- The goal was to build a complete analytics workflow without using pandas.
- The project focuses on vectorization, boolean masking, percentiles, and numerical analysis.
- It simulates a real-world HR analytics scenario.

2. Objective of the Project
- Generate a realistic employee dataset using NumPy
- Measure employee productivity and efficiency
- Identify top, average, and at-risk employees
- Perform department-wise performance analysis
- Use NumPy-only logic without relying on high-level abstractions

3. Dataset Description
- The dataset is synthetically generated using NumPy.
- Each row represents one employee.
- Total employees: 200
- Total departments: 4

Employee attributes included:
- Employee ID
- Department ID
- Monthly hours worked
- Tasks completed
- Quality score
- Monthly salary
- Absenteeism days

4. Data Generation
- Data was generated using NumPy random functions.
- Realistic ranges were used for all numerical values.
- A fixed random seed was used to ensure reproducibility.
- All columns were created using vectorized operations.

5. Feature Engineering
The following performance metrics were created from raw data:

- Productivity Score
  - Calculated as tasks completed divided by hours worked.
  - Measures how efficiently an employee completes tasks.

- Efficiency Score
  - Productivity score adjusted using normalized quality score.
  - Combines output quantity and quality.

- Performance Index
  - Final composite score.
  - Penalizes absenteeism to reflect real-world performance impact.

6. Performance Categorization
- Employees were categorized using percentile-based thresholds.
- Percentiles were used instead of fixed cutoffs to ensure fairness.

Categories used:
- Top Performers: Top 20 percent
- Average Performers: Middle 60 percent
- At-Risk Employees: Bottom 20 percent

Techniques applied:
- NumPy percentiles
- Boolean masking
- Vectorized conditional logic

7. Department-wise Analysis
- NumPy does not provide a built-in groupby function.
- Department-level analysis was implemented using boolean masking.
- Vectorized aggregation was used for performance calculation.

The analysis includes:
- Average performance score per department
- Identification of the best-performing department
- Count of top performers in each department

8. Key Insights
- Employee performance follows a balanced 20–60–20 distribution.
- Department 4 has the highest average performance score.
- Department 3 has the highest number of top-performing employees.
- Percentile-based evaluation avoids bias caused by absolute thresholds.

9. Tools and Technologies Used
- Python
- NumPy
- Jupyter Notebook
- Pandas was not used in this project.

10. How to Run the Project
- Clone or download the repository.
- Install required dependencies using:
  pip install -r requirements.txt
- Open the Jupyter notebook:
  jupyter notebook notebooks/employee_performance_analysis.ipynb

11. What I Learned
- Writing efficient NumPy code using vectorization.
- Using boolean masking instead of Python loops.
- Applying percentiles for fair performance evaluation.
- Performing group-level analysis without pandas.
- Translating numerical results into business insights.

12. Conclusion
- This project demonstrates how NumPy alone can be used for real-world analytics.
- It strengthens core numerical computing and analytical thinking skills.
- The project is suitable for portfolio presentation and interview discussion.
