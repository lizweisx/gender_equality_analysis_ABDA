# Project plan

**Project Duration**: 2024.12.04 - 2025.3.14

| **Phase**          | **Dates**               | **Tasks**                                                    |
| ------------------ | ----------------------- | ------------------------------------------------------------ |
| Pre-Holiday Phase  | 2024.12.04 - 2024.12.18 | **Data Preparation**<br/>-(Completed) Finalize research questions <br/> - Data cleaning and exploration <br/> - Descriptive statistics and initial visualizations. <br/> |
| Holiday Phase      | 2024.12.19 - 2025.1.6   | **Model Development**<br/>- Implementation of GLM or non-linear models.<br/>- Implementation of multilevel models.<br/>- (Optional)Lagged effect or cumulative effect analysis. |
| Post-Holiday Phase | 2025.1.7 - 2025.1.22    | **Results Analysis**<br/>- Regional and income-level heterogeneity analysis. <br/> \-Testing pathways through which gender equality laws influence GDP. <br/> \- Generating visualizations for results. |
| Presentation Prep  | 2025.1.23 - 2025.1.27   | -                                                            |
| Presentation       | 2025.1.28-2025.1.29     | -                                                            |
| Report Writing     | 2025.1.30-2025.3.14     | -                                                            |

### **Details for Each Phase**

#### **Pre-Holiday Phase** (15 days) -> **Data Preparation**

1. **Finalize Research Questions (Completed)**:
2. **Data Cleaning and Exploration**:
   - Check dataset integrity and remove missing or anomalous values:
     - Ensure alignment of key indicators (e.g., WBL indices and GDP data).
     - Handle missing or inconsistent values in the time-series data.
   - Write scripts to clean the data and save it in organized formats (e.g., `.csv` or `.RData`).
3. **Descriptive Statistics and Initial Visualizations**:
   - Generate basic statistics for each variable (e.g., mean, median, standard deviation).
   - Create distribution plots for key variables, such as histograms or time-series graphs for WBL indices and GDP growth.
   - Investigate potential patterns or correlations:
     - Use scatter plots to visualize the preliminary relationship between GDP growth and WBL indices.
     - Plot gender equality trends across regions or income levels.

#### **Holiday Phase** (19 days) -> Model Development

1. **Implementation of GLM or Non-linear Models**:

   - **Objective**: Test the direct effect of gender equality laws on GDP growth.

   - Steps:
     - Define dependent variables (e.g., GDP growth rate) and independent variables (e.g., WBL indices).
     - Write GLM model code.
     - If nonlinear relationships are detected, try implementing nonlinear models (e.g., polynomial regression or logarithmic transformations).

2. **Implementation of Multilevel Models**:

   - **Objective**: Analyze heterogeneity across different countries or regions.

   - Steps:
     - Group data by country or region to create hierarchical models.
     - Use brms to build multilevel models:
       - Fixed effects: WBL indices.
       - Random effects: Country or region.
     - Validate model convergence (check posterior distributions and diagnostic metrics).

3. **Lagged Effect or Cumulative Effect Analysis (Optional)**:

   - **Objective**: Explore the lagged or long-term effects of gender equality laws.

   - Steps:
     - Create lagged variables (e.g., WBL indices from the previous year or two years ago).
     - Test the predictive power of lagged variables on GDP.
     - Build cumulative effect models to evaluate the overall economic impact of years of legislative changes.

#### **Post-Holiday Phase** (16 days) -> **Results Analysis**

1. **Regional and Income-level Heterogeneity Analysis**:

   - **Objective**: Investigate the differential effects of gender equality laws across regions or income levels.

   - Steps:
     - Create regional or income-level grouping variables (e.g., low-income/middle-income/high-income countries).
     - Add interaction terms (e.g., `WBL × Income Level`) to multilevel models.
     - Visualize regional disparities using forest plots or grouped effect charts.

2. **Testing Pathways through Which Gender Equality Laws Influence GDP**:

   - **Objective**: Validate how gender equality affects GDP through intermediary variables such as labor force participation or education.

   - Steps:
     - Identify mediating variables (e.g., female labor force participation, educational attainment).
     - Build mediation models:
       - Step 1: WBL → Mediating variable.
       - Step 2: Mediating variable → GDP growth.
     - Assess direct, indirect, and total effects.

3. **Generating Visualizations for Results**:

   - **Objective**: Clearly present research findings.

   - Steps:
     - Create time-series trend plots to show the long-term impacts of gender equality on GDP.
     - Plot regression analysis results (e.g., confidence intervals and effect sizes in forest plots).
     - Optionally create interactive visualizations using tools like `shiny` or `plotly`.

