# Student Performance Analysis - EDA Project

## Project Description

This project conducts an Exploratory Data Analysis (EDA) on student academic performance to identify and understand the key factors that influence educational outcomes. Through comprehensive statistical analysis, this study examines how demographic characteristics, socioeconomic indicators, and educational interventions correlate with student achievement across math, reading, and writing assessments.

The analysis employs comparative methodologies and statistical testing to uncover actionable insights that can inform educational policy and intervention strategies at the institutional level.

---

## Table of Contents

- [Dataset Overview](#dataset-overview)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)

---

## Dataset Overview

The dataset contains student performance records with the following attributes:

| Variable | Description |
|----------|-------------|
| **gender** | Student's gender |
| **race/ethnicity** | Student's racial or ethnic group |
| **parental level of education** | Highest level of education attained by a parent |
| **lunch** | Type of lunch received (standard or free/reduced) |
| **test preparation course** | Completion status of test preparation course |
| **math score** | Numerical score in mathematics |
| **reading score** | Numerical score in reading |
| **writing score** | Numerical score in writing |

**Data Quality:** The dataset is clean with no missing values, making it ready for immediate analysis.

---

## Methodology

The analysis followed a systematic approach:

1. **Feature Engineering**
   - Created an average score metric by combining math, reading, and writing scores
   - Provided a single performance indicator for each student

2. **Comparative Analysis**
   - Calculated average scores across different categorical groups
   - Computed percentage differences to quantify performance gaps

3. **Statistical Testing**
   - Applied ANOVA (Analysis of Variance) tests
   - Determined statistical significance of observed differences
   - Validated that findings were not due to random chance

---

## Key Findings

The analysis revealed three primary factors with statistically significant impacts on student performance:

### 1. Test Preparation Course
- **Impact:** Students who completed the course scored **11.73% higher** on average
- **Significance:** Statistically significant with medium effect size
- **Implication:** Strong evidence for the effectiveness of structured test preparation

### 2. Lunch Type (Socioeconomic Indicator)
- **Impact:** Students receiving free lunch scored **12% lower** on average compared to those with standard lunch
- **Significance:** Statistically significant
- **Implication:** Suggests correlation between socioeconomic status and academic performance

### 3. Parental Education Level
- **Impact:** **16.64% score difference** between highest and lowest parental education levels
- **Significance:** Clear and substantial relationship
- **Implication:** Strong intergenerational educational influence

---

## Recommendations

Based on the findings, the following actionable recommendations are proposed:

### 1. Expand Test Preparation Access
- Make the test preparation course mandatory or strongly incentivized
- Consider reducing course fees to improve accessibility
- Track participation rates and outcomes

### 2. Investigate Socioeconomic Factors
- Conduct deeper analysis into the lunch type correlation
- Examine family socioeconomic status more comprehensively
- Assess nutritional quality and its potential impact on performance
- Consider additional support services for economically disadvantaged students

### 3. Targeted Support Programs
- Develop specialized academic support for students whose parents have lower education levels
- Create parent engagement workshops to build capacity for supporting student learning
- Provide educational resources and guidance for parents
- Establish mentorship or tutoring programs

---

## Technologies Used

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib/Seaborn** - Data visualization
- **SciPy/Statsmodels** - Statistical testing (ANOVA)

---

## Getting Started

### Prerequisites
```bash
python 3.x
pandas
numpy
matplotlib
seaborn
scipy
```

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/student-performance-eda.git

# Navigate to project directory
cd student-performance-eda

# Install required packages
pip install -r requirements.txt
```

### Usage
```bash
# Run the analysis notebook
jupyter notebook student_performance_analysis.ipynb

# Or run the Python script
python analysis.py
```

---

## Project Structure
```
student-performance-eda/
│
├── data/
│   └── student_performance.csv
├── notebooks/
│   └── student_performance_analysis.ipynb
├── src/
│   └── analysis.py
├── visualizations/
│   └── plots/
├── README.md
└── requirements.txt
```

---

## Conclusion

This EDA successfully identified and quantified key factors influencing student academic performance. The findings provide evidence-based insights that can guide institutional decision-making, resource allocation, and the development of targeted intervention programs to improve educational outcomes for all students.

---

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions or collaboration opportunities, please open an issue in the repository.

---

*This analysis was conducted as part of an academic project to demonstrate exploratory data analysis techniques and statistical inference methods.*