# Analyzing the Economic Impact of Gender Equality Across 190 Countries

## Project Overview
The project examines the relationship between gender equality and economic growth by analyzing data from nearly 190 countries. Using the Women, Business, and the Law (WBL) index, along with labor force participation and education levels as key variables, we aim to understand how these factors influence GDP.
Through exploratory data analysis, we investigate the extent to which improvements in gender equality correlate with economic performance. Our approach focuses on uncovering trends and relationships within the data without making predictive inferences. By employing Bayesian models, we analyze variations across countries and regions, allowing for a deeper understanding of the dynamics between equality, workforce participation, and education in shaping economic outcomes.
The insights gained from this study can contribute to a broader understanding of the critical role gender equality plays in fostering sustainable economic development. 

---

## Methodology
- **Dataset**:
  - Source: World Bank WBL 1.0 dataset (1971–2024).
  - Coverage: Data spans 190 economies, tracking changes in gender equality laws across 8 core themes.
  - Themes include: Mobility, Workplace, Pay, Marriage, Parenthood, Entrepreneurship, Assets, Pension.
  - Supplementary datasets: GDP growth rates, female labor force participation, and other socio-economic indicators.

- **Models**:
  1. **Generalized Linear Models (GLM)**:
     - Initial exploration to assess the direct impact of gender equality laws on GDP growth.
  2. **Multilevel Models**:
     - Accounting for regional and temporal heterogeneity.
     - Capturing differences between developed and developing economies.
  3. **Optional Extensions**:
     - Dynamic models to analyze lagged and cumulative effects of legal reforms.
     - Non-linear models if relationships deviate from linearity.

---

## Repository Structure
```plaintext
├── README.md                # Project overview
├── data/                    # Placeholder for datasets
├── scripts/                 # Analysis scripts
├── docs/                    # Documentation and plans
│   ├── project_plan.md      # Detailed project plan
│   ├── dataset_analysis.md  # Dataset analysis and research details
├── results/                 # Output results
