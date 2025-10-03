# TES prediction for stress

"TES prediction for stress" just a repo and code for what i and my friend learn for master



\# Synthetic College Student Lifestyle Dataset



\## Dataset Overview



\*\*Dataset Name\*\*: Synthetic College Student Lifestyle Dataset  

\*\*Purpose\*\*: Educational research, academic studies, and machine learning model development  

\*\*Records\*\*: 300 synthetic student profiles  

\*\*Features\*\*: 13 variables across 3 categories  

\*\*Format\*\*: CSV (Comma-Separated Values)  

\*\*File Size\*\*: ~45-50 KB  

\*\*Encoding\*\*: UTF-8  

\*\*Ethical Status\*\*: Fully synthetic, no real student data



\## Student Identification Features



\*\*student\_id\*\* (String)

\- Unique synthetic identifier

\- Format: `STU\_XXXX`



\*\*name\*\* (String)

\- Synthetic full name

\- Faker-generated



\## Academic Metrics



\*\*gpa\*\* (Float)

\- Range: 2.0 - 4.0

\- Distribution: Normal (μ=3.2, σ=0.5)

\- Description: Grade Point Average on 4.0 scale



\*\*weekly\_study\_hours\*\* (Float)

\- Range: 10 - 50 hours

\- Distribution: Normal (μ=25, σ=8)

\- Description: Total study hours per week



\*\*assignments\_due\_this\_week\*\* (Integer)

\- Range: 0 - 6

\- Distribution: Poisson (λ=2.5)

\- Description: Assignments due in current week



\*\*classes\_per\_week\*\* (Integer)

\- Range: 12 - 25 hours

\- Distribution: Uniform

\- Description: Total class hours weekly



\## Lifestyle Factors



\*\*sleep\_hours\_per\_night\*\* (Float)

\- Range: 4 - 10 hours

\- Distribution: Normal (μ=6.5, σ=1.2)

\- Description: Average nightly sleep



\*\*social\_events\_per\_week\*\* (Float)

\- Range: 0 - 7 events

\- Distribution: Modified Normal

\- Description: Social activities attended



\*\*exercise\_hours\_per\_week\*\* (Float)

\- Range: 0 - 15 hours

\- Distribution: Exponential (λ=3)

\- Description: Physical exercise hours



\*\*extracurricular\_hours\*\* (Float)

\- Range: 0 - 10 hours

\- Distribution: Exponential (λ=2)

\- Description: Extracurricular activity hours



\## Environmental Factors



\*\*part\_time\_job\_hours\*\* (Integer)

\- Range: 0 - 25 hours

\- Distribution: Conditional

\- Description: Work hours (30% employed)



\*\*commute\_time\_minutes\*\* (Integer)

\- Range: 0 - 120 min

\- Distribution: Exponential

\- Description: Daily one-way commute



\*\*financial\_stress\_level\*\* (Float)

\- Range: 1 - 5 scale

\- Distribution: Beta (α=2, β=5)

\- Description: Self-reported financial stress



\## Data Generation Methodology



\### Research-Based Parameters

\- \*\*GPA Distributions\*\*: Based on institutional academic data

\- \*\*Study Hours\*\*: Aligned with national student surveys

\- \*\*Sleep Patterns\*\*: Reflects college sleep studies

\- \*\*Financial Stress\*\*: Derived from student wellness research



\### Realistic Correlations

```

\# Key relationships built into the data

study\_sleep\_corr ≈ -0.3

study\_gpa\_corr ≈ +0.4

social\_study\_tradeoff ≈ -0.25

```



\## Intended Use Cases



\### Primary Applications

\- Educational Research: Lifestyle-academic performance relationships

\- Machine Learning: Predictive model development

\- Academic Studies: Student behavior pattern analysis

\- Institutional Research: Analytics system prototyping



\### Analytical Applications

\- Correlation analysis between factors

\- Cluster analysis for behavior patterns

\- Regression modeling of performance predictors

\- Time management and workload studies



\## Limitations \& Ethical Considerations



\### Synthetic Nature

\*\*Note\*\*: This is computer-generated data and may not capture all real-world complexities.



\*\*Generalized Patterns\*\*

\- Impact: May miss nuances

\- Mitigation: Based on aggregate research



\*\*Institutional Variation\*\*

\- Impact: One-size-fits-all

\- Mitigation: Customizable parameters



\*\*Cultural Factors\*\*

\- Impact: Limited representation

\- Mitigation: Research-informed ranges



\### Ethical Usage Guidelines

\- No Real Data: All records are synthetically generated

\- Privacy Protection: No inference to real individuals possible

\- Appropriate Use: Research and development only

\- Production Warning: Validate with real data before deployment



\## Technical Specifications



\### File Structure

```

student\_id,name,gpa,weekly\_study\_hours,sleep\_hours\_per\_night,...

STU\_0001,John Smith,3.45,28.5,6.8,...

STU\_0002,Jane Doe,3.78,32.1,7.2,...

```



\### Data Types Summary

\*\*String\*\* (2 features)

\- student\_id, name



\*\*Float\*\* (7 features)

\- gpa, weekly\_study\_hours, sleep\_hours\_per\_night, social\_events\_per\_week, exercise\_hours\_per\_week, financial\_stress\_level, extracurricular\_hours



\*\*Integer\*\* (4 features)

\- assignments\_due\_this\_week, classes\_per\_week, part\_time\_job\_hours, commute\_time\_minutes



\## Sample Statistics



\### Descriptive Statistics

\*\*GPA\*\*

\- Mean: 3.21

\- Std Dev: 0.42

\- Min: 2.15

\- Max: 3.98



\*\*Study Hours\*\*

\- Mean: 25.3

\- Std Dev: 7.8

\- Min: 11.5

\- Max: 48.2



\*\*Sleep Hours\*\*

\- Mean: 6.4

\- Std Dev: 1.3

\- Min: 4.1

\- Max: 9.8



\### Correlation Matrix (Sample)

\*\*GPA\*\*

\- GPA: 1.00

\- Study Hours: 0.42

\- Sleep: 0.15

\- Social: 0.08



\*\*Study Hours\*\*

\- GPA: 0.42

\- Study Hours: 1.00

\- Sleep: -0.31

\- Social: -0.27



\*\*Sleep Hours\*\*

\- GPA: 0.15

\- Study Hours: -0.31

\- Sleep: 1.00

\- Social: 0.18



\*\*Social Events\*\*

\- GPA: 0.08

\- Study Hours: -0.27

\- Sleep: 0.18

\- Social: 1.00



\## Citation



When using this dataset, please acknowledge:



"Synthetic College Student Lifestyle Dataset generated for educational research purposes using research-informed parameter distributions."



\## Files Included



\- `student\_lifestyle\_dataset.csv` - Main dataset file

\- `dataset\_documentation.json` - Technical metadata

\- `data\_generation\_script.py` - Generation code (optional)



\## Support



This dataset is provided as-is for research and educational purposes. For methodological questions, refer to the accompanying documentation.



---



\*Last Updated: 2025\*  

\*Dataset Version: 1.0\*  

\*Generated with: Python + Faker + Research Parameters\*

