# Part 2 Case 1(Charity Muigai)

# AI Hiring Bias Case Study: Amazon's Recruiting Tool

## Overview
This case study examines Amazon's AI recruiting tool that penalized female candidates, analyzing the bias sources and proposing comprehensive solutions for fair AI hiring systems.

## The Problem
Amazon's AI recruiting tool exhibited significant gender bias, systematically downgrading female candidates due to training on historically biased data from a male-dominated industry.

## Root Cause Analysis
**Primary Bias Source**: Biased training data
- 10+ years of historical resumes from male-dominated tech industry
- AI learned to replicate discriminatory hiring patterns
- Gender-coded language and experiences were penalized

## Solutions Framework

### 🔧 Technical Fixes
1. **Data Preprocessing**: Remove gendered language, augment with synthetic balanced data
2. **Algorithmic Debiasing**: Implement adversarial training and fairness constraints
3. **Human Oversight**: Structured blind review with diverse evaluation panels

### 📊 Fairness Metrics
- **Statistical Parity**: Equal selection rates across gender groups
- **Equalized Odds**: Consistent true/false positive rates
- **Outcome Tracking**: Monitor hiring, performance, and retention rates
- **Process Auditing**: Regular feature importance and intersectional analysis

## Key Takeaways
- Historical bias in training data perpetuates discrimination
- Multiple intervention points required (data, algorithms, process)
- Continuous monitoring essential for maintaining fairness
- Human oversight remains critical for ethical AI deployment

## Next Steps
1. Implement proposed technical solutions
2. Establish regular bias auditing schedule
3. Train hiring teams on fair AI practices
4. Monitor outcomes across all demographic groups

---
*This analysis provides a framework for identifying and addressing bias in AI hiring systems.*
# COMPAS Recidivism Bias Audit using AIF360

## 📌 Project Overview
This project performs a fairness audit on the COMPAS Recidivism Dataset using IBM's **AI Fairness 360 (AIF360)** toolkit. The goal is to identify and mitigate racial bias in predictive risk scores, specifically between African-American and Caucasian individuals.

## 📁 Files Included
- `COMPAS_Audit_AIF360.ipynb` — Jupyter notebook with full bias analysis, metrics, and visualization.
- `COMPAS_Bias_Audit_Report.docx` — A 300-word summary report of findings and mitigation strategies.
- `COMPAS_Bias_Audit_Report.pdf` — (Optional) PDF version of the report.
- `README.md` — This guide.

## 📊 Dataset
- **Source**: ProPublica COMPAS Risk Scores  
- **Link**: [https://www.propublica.org/datastore/dataset/compas-recidivism-risk-score-data-and-analysis](https://www.propublica.org/datastore/dataset/compas-recidivism-risk-score-data-and-analysis)
- **Protected Attribute**: Race (`African-American` vs `Caucasian`)

## ⚙️ Tools Used
- Python 3
- AIF360 (IBM)
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## 🧪 Steps Performed
1. Load and preprocess the COMPAS dataset using `CompasDataset`.
2. Compute baseline fairness metrics.
3. Apply **Reweighing** as a pre-processing bias mitigation technique.
4. Train a logistic regression model.
5. Evaluate fairness and accuracy metrics on test data.
6. Visualize disparities in outcomes like false positive rates.

## 📈 Key Findings
- African-American defendants have higher false positive rates.
- Reweighing reduces disparities while maintaining accuracy.

## ▶️ How to Run
1. Install dependencies:
    ```bash
    pip install aif360 scikit-learn matplotlib
    ```
2. Open `COMPAS_Audit_AIF360.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells step by step to see metrics and visualization.

## 📬 Contact
For questions or collaboration, reach out to the author or instructor.
