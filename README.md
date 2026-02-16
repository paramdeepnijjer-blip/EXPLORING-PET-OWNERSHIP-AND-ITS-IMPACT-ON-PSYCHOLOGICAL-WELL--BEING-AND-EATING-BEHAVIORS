# 🐾 Exploring Pet Ownership and Its Impact on Psychological Well-Being and Eating Behaviors

**Statistical Consulting Capstone Project | MacEwan University | April 2025**

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![RMarkdown](https://img.shields.io/badge/RMarkdown-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)
![Statistics](https://img.shields.io/badge/Statistics-FF6F00?style=for-the-badge&logo=google-scholar&logoColor=white)

---

## 📋 Project Overview

This capstone project investigates the complex relationship between pet ownership, emotional attachment to pets, and mental health outcomes—specifically focusing on eating disorder risk, depression, anxiety, and mood disturbances. Contrary to popular belief that pets universally improve well-being, this study reveals nuanced and sometimes counterintuitive findings.

### 🎯 Key Research Questions

1. **Is pet ownership associated with disordered eating behaviors?** (Drive for Thinness, Body Dissatisfaction, Bulimia)
2. **Does pet ownership affect psychological well-being?** (Depression, Anxiety, Positive/Negative Mood, Loneliness)
3. **How does pet attachment relate to mental health outcomes?**
4. **Does pet attachment correlate with eating disorder risk?**
5. **Do psychological factors mediate the relationship between pet ownership and eating behaviors?**

---

## 🔍 Key Findings

### Unexpected Results

Contrary to the hypothesis that pet ownership would be protective:

- **Pet owners reported HIGHER levels of disordered eating behaviors**
  - Drive for Thinness (p < 0.001)
  - Body Dissatisfaction (p < 0.001)
  - Bulimia (p = 0.004)

- **Stronger pet attachment correlated with INCREASED psychological distress**
  - Depression (r = 0.221, p < 0.001)
  - Anxiety (r = 0.304, p < 0.001)
  - Negative Mood (r = 0.208, p < 0.001)

### Protective Effects

Pet ownership was associated with some benefits:
- **Lower depression scores** (p = 0.006)
- **Lower anxiety scores** (p < 0.001)
- **Reduced negative mood** (p = 0.013)

### Mediation Analysis

**Depression and negative mood partially mediated** the relationship between pet ownership and eating disorder risk:
- Indirect effect through depression: β = 1.34 (p = 0.026)
- Indirect effect through negative mood: β = 1.14 (p = 0.023)
- Total effect: β = 6.30 (p < 0.001)

---

## 📊 Dataset

### Sample Characteristics
- **N = 645 participants** (after cleaning from original 686)
- **Survey method**: Online self-report questionnaire
- **Demographics**:
  - Age: M = 20.32, SD = 4.71 (range: 17-47)
  - Gender: 77.4% female, 18.5% male, 4.1% other/non-binary
  - Pet ownership: 58.6% owners, 41.4% non-owners

### Variables Measured

**Disordered Eating (EDI-3 subscales)**
- Drive for Thinness (DT)
- Body Dissatisfaction (BD)
- Bulimia (B)
- Composite: EDRC_Raw

**Psychological Well-Being**
- Beck Depression Inventory (BDI)
- Beck Anxiety Inventory (BAI)
- Positive and Negative Affect Schedule (PANAS)
- UCLA Loneliness Scale (RULS-6)

**Pet Variables**
- Pet ownership status
- Pet type (dog, cat, other)
- Lexington Attachment to Pets Scale (LAPS)

**Demographics**
- Age, Gender, Ethnicity
- Sexual Orientation, Marital Status, Education
- Living Situation

---

## 📈 Statistical Methods

### Analytical Techniques

1. **ANOVA** - Group differences between pet owners and non-owners
2. **Linear Regression** - Predictive relationships
3. **Correlation Analysis** - Strength and direction of associations
4. **Mediation Analysis** (lavaan package) - Indirect effects through psychological variables
5. **Independent Samples t-tests** - Comparing dog vs. cat owners

### Model Validation
- Normality testing (Shapiro-Wilk test, Q-Q plots)
- Homogeneity of variance (Levene's Test)
- Multicollinearity assessment (VIF)
- Residual diagnostics

---

## 🗂️ Repository Structure

```
pet-ownership-mental-health/
├── README.md                              # This file
├── Param_FINAL_STAT_496_REPORT_.Rmd      # Full R Markdown analysis
├── ParamFINALSTAT496REPORT.pdf           # Complete written report (24 pages)
├── STAT 496 Final Presentation.pptx      # Presentation slides
├── data/
│   └── CLEAN_DATA.xlsx                    # Cleaned dataset (N=645)
├── figures/                               # Key visualizations
│   ├── churn_by_contract.png
│   ├── correlation_matrix.png
│   ├── mediation_diagram.png
│   └── anova_results.png
└── LICENSE                                # MIT License
```

---

## 🚀 Getting Started

### Prerequisites
```r
# Required R packages
install.packages(c(
  "tidyverse",    # Data manipulation and visualization
  "lavaan",       # Mediation analysis
  "psych",        # Psychometric analysis
  "ggplot2",      # Advanced visualizations
  "readxl",       # Excel file import
  "knitr",        # Report generation
  "rmarkdown"     # Document creation
))
```

### Running the Analysis

1. **Clone the repository**
```bash
git clone https://github.com/paramdeepnijjer-bliip/pet-ownership-mental-health.git
cd pet-ownership-mental-health
```

2. **Load data**
```r
library(readxl)
data <- read_excel("data/CLEAN_DATA.xlsx")
```

3. **Open and run the R Markdown file**
```r
# In RStudio
rmarkdown::render("Param_FINAL_STAT_496_REPORT_.Rmd")
```

---

## 📑 Report Sections

The 24-page comprehensive report includes:

### 1. Abstract & Introduction
- Research context and motivation
- Literature review on pet ownership and mental health
- Study objectives and hypotheses

### 2. Methods
- Study design (cross-sectional, observational)
- Participant recruitment and eligibility
- Measures and instruments (EDI-3, BDI, BAI, PANAS, LAPS)
- Statistical procedures
- Ethical considerations

### 3. Results (6 Research Questions)
- **RQ1**: Pet ownership and disordered eating behaviors
- **RQ2**: Pet ownership and EDRC composite score
- **RQ3**: Pet ownership and psychological well-being
- **RQ4**: Pet attachment and psychological indicators
- **RQ5**: Pet attachment and eating disorder risk
- **RQ6**: Mediation analysis (depression & negative mood)

### 4. Discussion
- Interpretation of counterintuitive findings
- Comparison with existing literature
- Clinical and practical implications
- Study limitations
- Future research directions

### 5. Appendices
- Distribution histograms for all variables
- Q-Q plots and normality tests
- Residual diagnostics
- Complete statistical output

---

## 💡 Clinical Implications

### For Mental Health Professionals

1. **Screen for pet attachment quality** - High attachment may signal emotional over-reliance
2. **Consider pet-related stress** - Financial burden, caregiving responsibility, grief/loss
3. **Evaluate social support networks** - Pets may substitute for human connections
4. **Assess coping strategies** - Reliance on pets may reflect maladaptive regulation

### For Future Research

1. **Longitudinal studies** - Establish directionality (does distress lead to pet ownership, or vice versa?)
2. **Moderators to explore**:
   - Socioeconomic status and financial strain
   - Caregiving burden
   - Quality vs. quantity of human social support
   - Attachment style (anxious, avoidant, secure)
3. **Contextual factors**:
   - Pet care costs
   - Living situation constraints
   - Life transitions and stressors

---

## 📊 Key Visualizations

### Churn Rate by Pet Attachment
![Pet Attachment Distribution](figures/pet_attachment_boxplot.png)

### Correlation Matrix
![Correlation Matrix](figures/correlation_heatmap.png)

### Mediation Model
![Mediation Diagram](figures/mediation_model.png)

*(Figures to be added from PDF extraction)*

---

## 🎓 Academic Context

**Course**: STAT 496 - Applied Statistics Consulting Project  
**Institution**: MacEwan University  
**Program**: B.Sc. Applied Statistics  
**Instructor**: Dr. Su  
**Date**: April 4, 2025  

### Project Scope

This was a **full-cycle statistical consulting project** involving:
- Client communication and needs assessment
- Research question formulation
- Data cleaning and validation
- Comprehensive statistical analysis
- Written report and presentation delivery
- Interpretation and recommendations for stakeholders

---

## 🔬 Statistical Rigor

### Strengths
- ✅ Large sample size (N = 645)
- ✅ Validated psychometric instruments (EDI-3, BDI, BAI, LAPS)
- ✅ Multiple analytical approaches (ANOVA, regression, mediation)
- ✅ Comprehensive diagnostic checks
- ✅ Transparent reporting of limitations

### Limitations
- ⚠️ Cross-sectional design (no causality)
- ⚠️ Self-report bias
- ⚠️ Unmeasured confounders (SES, caregiving burden)
- ⚠️ Convenience sampling (online survey)
- ⚠️ Limited generalizability (university-aged sample)

---

## 📚 References

**Key Literature Cited**:

1. Ståhl, A., et al. (2023). Pet and owner personality and mental wellbeing associate with attachment to cats and dogs. *iScience, 26*(12), 108423.

2. Marcial-Modesto, D., et al. (2023). Pet ownership and mental health in United States adults during COVID-19. *Frontiers in Psychology, 14*, 1217059.

3. Lass-Hennemann, J., et al. (2022). The relationship between attachment to pets and mental health: The shared link via attachment to humans. *BMC Psychiatry, 22*, 586.

4. National Institutes of Health (2022). The power of pets: Health benefits of human-animal interactions. NIH News in Health.

---

## 👤 Author

**Paramdeep Nijjer**  
B.Sc. Applied Statistics | MacEwan University  
Data Analyst | Machine Learning Enthusiast

- 📧 Email: [paramdeep.nijjer@gmail.com]
- 💼 LinkedIn: [https://www.linkedin.com/in/paramdeepnijjer/]
- 🐙 GitHub: [@paramdeepnijjer-bliip](https://github.com/paramdeepnijjer-bliip)

---

## 🤝 Acknowledgments

- **Dr. Su** - Faculty advisor and course instructor
- **Study participants** - 645 individuals who completed the survey
- **MacEwan University** - STAT 496 course support
- **R Community** - Open-source statistical software

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Key Takeaway

> **"Pet ownership is not universally protective for mental health. The relationship is complex, context-dependent, and may reflect underlying emotional vulnerabilities rather than causing them. Strong pet attachment can signal both comfort-seeking and psychological distress."**

---

## 📞 Contact & Collaboration

Interested in collaborating or have questions about the methodology?  
Feel free to open an issue or reach out directly!

**⭐ Star this repository if you found the research interesting!**

---

*Last Updated: February 2026*
