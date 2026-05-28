# **Project: CallMeMaybe Operator Efficiency Analysis**

This project focuses on data analysis to identify ineffective operators in the CallMeMaybe virtual phone service. Through Exploratory Data Analysis (EDA) and statistical testing, key metrics such as missed call rates, prolonged wait times, and the proportion of outgoing calls per operator are evaluated. The goal is to provide supervisors with information to improve operational efficiency and service quality.

**Objective**

The project is structured into the following main phases:

1. **Data Validation and Cleaning:** Prepare and validate the call and client datasets.
2. **Data Quality Analysis:** Evaluate data integrity and distribution.
3. **Exploratory Data Analysis:** Explore distributions, trends, and metrics by operator.
4. **Identification of Ineffective Operators:** Classify operators based on inefficiency criteria.
5. **Detailed Operator Analysis:** Delve into the performance of specific operators.
6. **Statistical Hypothesis Testing:** Validate statistically significant differences.
7. **Conclusions and Recommendations:** Synthesize findings and propose intervention strategies.

**🛠️ Technologies Used**

* **Python:** Primary language for data analysis.
* **Pandas:** For data manipulation, cleaning, and aggregation.
* **NumPy:** For numerical operations and array handling.
* **Matplotlib and Seaborn:** For data visualization, including distribution plots, boxplots, and per-operator analysis.
* **SciPy:** For conducting statistical tests (Mann-Whitney U test).
* **Jupyter Notebook:** Interactive environment for developing the analysis.

**Key Steps**

1. **Data Validation and Cleaning:**
   - Loaded the `telecom_dataset_new.csv` (call records) and `telecom_clients_us.csv` (client information) datasets.
   - Performed data cleaning, type conversion, and filtering by the relevant period.

2. **Data Quality Analysis:**
   - Evaluated the distribution of calls by operator, direction, and type.
   - Verified data integrity and identified outliers.

3. **Exploratory Data Analysis:**
   - Explored metrics such as call duration, wait times, and missed call rates.
   - Visualized distributions and temporal trends.

4. **Identification of Ineffective Operators:**
   - Defined criteria: high missed call rate, prolonged wait time, low proportion of outgoing calls.
   - Classified operators as effective or ineffective.

5. **Detailed Operator Analysis:**
   - Analyzed individual operator performance, including descriptive statistics.
   - Identified inefficiency patterns.

6. **Statistical Hypothesis Testing:**
   - Applied the Mann-Whitney U test to compare effective and ineffective groups.
   - Evaluated the statistical significance of differences.

7. **Conclusions and Recommendations:**
   - Synthesized findings and proposed prioritized intervention strategies.

**Results**

The analysis reveals that:

- **Data Quality:** Clean datasets with call records and clients, covering a specific period.
- **Ineffective Identification:** 505 operators (61.2% of the workforce) classified as ineffective, based on criteria of high loss, prolonged wait, inconsistency, and low output.
- **Key Findings:** Process risk (inconsistency) affects 206 operators; service risk (times) affects 206; severe risk (multiple issues) affects 147.
- **Top 10 Risk:** Operators with the highest inefficiency, dominated by extreme inconsistency and prolonged wait times (up to 1,007s).
- **Statistical Validation:** Mann-Whitney U test confirms significant differences (p ≈ 0.0000).
- **Recommendations:** Segmented strategy: immediate coaching for the top 10, group training for the 147 high-risk individuals, and audit for low output. Next steps include post-intervention monitoring and threshold adjustment.

**How to Run the Project**

1. Clone this repository to your local machine.
   ```bash
   git clone (https://github.com/ferchi4/Proyecto_spring_13)
   ```

2. Ensure you have the necessary dependencies installed:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy jupyter
   ```

3. Place the data files (`telecom_dataset_new.csv`, `telecom_clients_us.csv`) in the same directory as the notebook.

4. Open and execute the `Proy_Operadores.ipynb` file in Jupyter Notebook.
   ```bash
   jupyter notebook Proy_Operadores.ipynb
   ```
