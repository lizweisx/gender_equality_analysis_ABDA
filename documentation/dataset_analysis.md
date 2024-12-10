# **Dataset Analysis**

### **Ⅰ. Dataset Overview**

- **Source**: WBL 1.0[Data](https://wbl.worldbank.org/en/wbl-data), developed by the World Bank, covering data from 1971 to 2024, covering 190 economies.
- **Indicators**:
  - 8 core themes: Mobility, Workspace, Pay, Marriage, Parenthood, Entrepreneurship, Assets, Pension.
  - 35 binary questions (e.g., Yes/No).
- **Scoring Rules**:
  - Each question is scored (e.g., Yes = points).
  - Scores are averaged for each theme, and the overall WBL score is the mean of all 8 themes.
  - The maximum score is 100, indicating full legal gender equality.

### **Ⅱ. Dataset Advantages**

- Long time span (1971–2024), wide coverage (190 economies), structured with 8 themes and 35 questions.
- Simple, intuitive indicators focused on legal frameworks, making it easy for modeling and interpretation.

### **Ⅲ. Dataset Issues**

- **Simple scoring mechanism**: All questions are equally weighted, ignoring differences in importance (e.g., "freedom to choose residence" vs. "maternity leave days").
- **Discrete design**: Most questions are binary (Yes/No), leading to concentrated scores and limited granularity for detailed analysis.

### **Ⅳ. Research Questions**

- Does legal gender equality promote economic growth (e.g., GDP growth rate)?
- Possible mechanisms linking gender-equal laws to GDP:
  1. **Female labor force participation**: How do laws encourage women to join the workforce? 
  2. **Social welfare effects**: How does gender equality improve education and health, driving long-term growth?
- Are the effects of gender-equal laws on GDP different across economies with varying legal and economic contexts?

### **Ⅴ. Why Bayesian Models?**

- **Capturing heterogeneity**: Bayesian multilevel models quantify differences in the effects of gender-equal laws across economies (e.g., cultural or economic differences).
- **Dynamic analysis**: Gender-equal laws may have delayed effects on economic outcomes; Bayesian models incorporate time dimensions.
- **Pathway analysis**: Bayesian models can test mechanisms (e.g., female labor force participation, education,...) through which laws influence GDP.

### **Ⅵ. Model Framework**

1. **Extended Linear Regression Models**: To analyze the direct impact of gender-equal laws on GDP.
2. **Multilevel Regression Models**:
   - Grouping by economy/region (e.g., developed vs. developing countries).
   - Controlling for year effects (tt).
   - Adding variables like ZitZ_{it} (e.g., 0/1 for developing countries).
3. **Time-related Models**:
   - **Lagged Effects**: Analyzing how last year’s legal score affects current GDP.
   - **Cumulative Effects**: Evaluating the long-term impacts of laws on GDP growth.

### **Ⅶ. Related Datasets to Include**

- [**GDP growth (annual %) - | Data**](https://data.worldbank.org/indicator/NY.GDP.MKTP.KD.ZG?end=2023&locations=Z7%3B&start=2000&view=chart&year=2000)
- [**Labor force, female (% of total labor force) | Data**](https://data.worldbank.org/indicator/SL.TLF.TOTL.FE.ZS)
- [**School enrollment, tertiary, female (% gross) | Data**](https://data.worldbank.org/indicator/SE.TER.ENRR.FE)
- [**Wage and salaried workers, female (% of female employment) (modeled ILO estimate) | Data**](https://data.worldbank.org/indicator/SL.EMP.WORK.FE.ZS)
- [**Life expectancy at birth, female (years) | Data**](https://data.worldbank.org/indicator/SP.DYN.LE00.FE.IN)



### **Research question:**

How do legal rights for women, particularly in areas like mobility, pay and workspace protections influence women’s economic participation, overall economic development and regional differences and what barriers prevent countries from implementing these reforms?

### **Tasks:**

1. Examine the most impactful legal indicators 
2. Analyse their effects on women’s economic outcomes -> by GLM or non-linear model, depending on data distribution
3. Compare outcomes across regions or income levels ->by Multilevel model
4. Investigate barriers to reform 
5. Explore the broader economic implications of better legal rights for women ->how to achieve?

### **Models:** 

(just an idea to use the model for the tasks) *need to do a proper study tho.

**Generalized Linear Models (GLM):** To predict the likelihood of a country having higher women’s economic participation based on its legal scores.

**Hierarchical/Multilevel Models:** To model how legal rights influence women’s economic outcomes, while accounting for country-specific and regional-level variations.

**Mixture models:** To identify clusters of countries with similar legal frameworks and predicting economic outcomes for women based on their cluster membership. 

**Non-linear models:** To model the non-linear relationship between legal reforms (like pay or marriage laws) and women’s economic outcomes, especially to expect diminishing returns or thresholds. 