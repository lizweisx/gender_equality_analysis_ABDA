# Applied Bayesian Data Analysis: Gender Equality and Economic Growth

## Project Overview
This project explores the impact of gender equality laws on economic growth using Bayesian models, focusing on mechanisms like female labor participation and education. It includes a comparison of outcomes across regions and economic levels.

### Objectives: 

1. Quantify the impact of gender equality laws on GDP growth. 
1. Identify pathways linking gender-equal laws to economic outcomes (e.g., labor force participation, education). 
1. Analyze heterogeneity in these effects across regions and income levels.

---

## Research Questions
1. **Does legal gender equality promote economic growth (e.g., GDP growth rate)?**
2. **What are the key mechanisms through which gender-equal laws affect GDP?**
   - Female labor force participation: Do laws encourage more women to enter the workforce?
   - Social welfare improvements: How does gender equality enhance education and health outcomes?
3. **Do the effects of gender equality laws vary by region or economic context?**
   - How do developed and developing countries differ in their responses to gender-equal laws?

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
