# TES prediction for stress

"TES prediction for stress" just a repo and code for what i and my friend learn for master


\# Synthetic College Student Lifestyle Dataset



\## Dataset Overview



| Attribute | Description |

|-----------|-------------|

| Dataset Name | Synthetic College Student Lifestyle Dataset |

| Purpose | Educational research, academic studies, and machine learning model development |

| Records | 300 synthetic student profiles |

| Features | 13 variables across 3 categories |

| Format | CSV (Comma-Separated Values) |

| File Size | ~45-50 KB |

| Encoding | UTF-8 |

| Ethical Status | Fully synthetic, no real student data |



\## Student Identification Features



| Feature | Type | Description | Format/Range |

|---------|------|-------------|--------------|

| `student\_id` | String | Unique synthetic identifier | `STU\_XXXX` |

| `name` | String | Synthetic full name | Faker-generated |



\## Academic Metrics



| Feature | Type | Range | Distribution | Description |

|---------|------|-------|--------------|-------------|

| `gpa` | Float | 2.0 - 4.0 | Normal (μ=3.2, σ=0.5) | Grade Point Average on 4.0 scale |

| `weekly\_study\_hours` | Float | 10 - 50 hours | Normal (μ=25, σ=8) | Total study hours per week |

| `assignments\_due\_this\_week` | Integer | 0 - 6 | Poisson (λ=2.5) | Assignments due in current week |

| `classes\_per\_week` | Integer | 12 - 25 hours | Uniform | Total class hours weekly |



\## Lifestyle Factors



| Feature | Type | Range | Distribution | Description |

|---------|------|-------|--------------|-------------|

| `sleep\_hours\_per\_night` | Float | 4 - 10 hours | Normal (μ=6.5, σ=1.2) | Average nightly sleep |

| `social\_events\_per\_week` | Float | 0 - 7 events | Modified Normal | Social activities attended |

| `exercise\_hours\_per\_week` | Float | 0 - 15 hours | Exponential (λ=3) | Physical exercise hours |

| `extracurricular\_hours` | Float | 0 - 10 hours | Exponential (λ=2) | Extracurricular activity hours |



\## Environmental Factors



| Feature | Type | Range | Distribution | Description |

|---------|------|-------|--------------|-------------|

| `part\_time\_job\_hours` | Integer | 0 - 25 hours | Conditional | Work hours (30% employed) |

| `commute\_time\_minutes` | Integer | 0 - 120 min | Exponential | Daily one-way commute |

| `financial\_stress\_level` | Float | 1 - 5 scale | Beta (α=2, β=5) | Self-reported financial stress |



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

\- \*\*Educational Research\*\*: Lifestyle-academic performance relationships

\- \*\*Machine Learning\*\*: Predictive model development

\- \*\*Academic Studies\*\*: Student behavior pattern analysis

\- \*\*Institutional Research\*\*: Analytics system prototyping



\### Analytical Applications

\- Correlation analysis between factors

\- Cluster analysis for behavior patterns

\- Regression modeling of performance predictors

\- Time management and workload studies



\## Limitations \& Ethical Considerations



\### Synthetic Nature

\*\*Note\*\*: This is computer-generated data and may not capture all real-world complexities.



| Limitation | Impact | Mitigation |

|------------|--------|------------|

| Generalized Patterns | May miss nuances | Based on aggregate research |

| Institutional Variation | One-size-fits-all | Customizable parameters |

| Cultural Factors | Limited representation | Research-informed ranges |



\### Ethical Usage Guidelines

\- \*\*No Real Data\*\*: All records are synthetically generated

\- \*\*Privacy Protection\*\*: No inference to real individuals possible

\- \*\*Appropriate Use\*\*: Research and development only

\- \*\*Production Warning\*\*: Validate with real data before deployment



\## Technical Specifications



\### File Structure

```

student\_id,name,gpa,weekly\_study\_hours,sleep\_hours\_per\_night,...

STU\_0001,John Smith,3.45,28.5,6.8,...

STU\_0002,Jane Doe,3.78,32.1,7.2,...

...

```



\### Data Types Summary

| Data Type | Features | Count |

|-----------|----------|-------|

| String | student\_id, name | 2 |

| Float | gpa, weekly\_study\_hours, sleep\_hours\_per\_night, social\_events\_per\_week, exercise\_hours\_per\_week, financial\_stress\_level, extracurricular\_hours | 7 |

| Integer | assignments\_due\_this\_week, classes\_per\_week, part\_time\_job\_hours, commute\_time\_minutes | 4 |



\## Sample Statistics



\### Descriptive Statistics

| Feature | Mean | Std Dev | Min | Max |

|---------|------|---------|-----|-----|

| GPA | 3.21 | 0.42 | 2.15 | 3.98 |

| Study Hours | 25.3 | 7.8 | 11.5 | 48.2 |

| Sleep Hours | 6.4 | 1.3 | 4.1 | 9.8 |



\### Correlation Matrix (Sample)

| Feature | GPA | Study Hours | Sleep | Social |

|---------|-----|-------------|-------|--------|

| GPA | 1.00 | 0.42 | 0.15 | 0.08 |

| Study Hours | 0.42 | 1.00 | -0.31 | -0.27 |

| Sleep Hours | 0.15 | -0.31 | 1.00 | 0.18 |

| Social Events | 0.08 | -0.27 | 0.18 | 1.00 |



\## Citation



When using this dataset, please acknowledge:



> "Synthetic College Student Lifestyle Dataset generated for educational research purposes using research-informed parameter distributions."



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

