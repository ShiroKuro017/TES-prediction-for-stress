# TES prediction for stress

"TES prediction for stress" is just a repo and code for what my friend and I learn 



# Synthetic College Student Lifestyle Dataset

## Dataset Overview

**Dataset Name**: Synthetic College Student Lifestyle Dataset  
**Purpose**: Educational research, academic studies, and machine learning model development  
**Records**: 300 synthetic student profiles  
**Features**: 13 variables across 3 categories  
**Format**: CSV (Comma-Separated Values)  
**File Size**: ~45-50 KB  
**Encoding**: UTF-8  
**Ethical Status**: Fully synthetic, no real student data

## Student Identification Features

**student_id** (String)
- Unique synthetic identifier
- Format: `STU_XXXX`

**name** (String)
- Synthetic full name
- Faker-generated

## Academic Metrics

**gpa** (Float)
- Range: 2.0 - 4.0
- Distribution: Normal (μ=3.2, σ=0.5)
- Description: Grade Point Average on 4.0 scale

**weekly_study_hours** (Float)
- Range: 10 - 50 hours
- Distribution: Normal (μ=25, σ=8)
- Description: Total study hours per week

**assignments_due_this_week** (Integer)
- Range: 0 - 6
- Distribution: Poisson (λ=2.5)
- Description: Assignments due in current week

**classes_per_week** (Integer)
- Range: 12 - 25 hours
- Distribution: Uniform
- Description: Total class hours weekly

## Lifestyle Factors

**sleep_hours_per_night** (Float)
- Range: 4 - 10 hours
- Distribution: Normal (μ=6.5, σ=1.2)
- Description: Average nightly sleep

**social_events_per_week** (Float)
- Range: 0 - 7 events
- Distribution: Modified Normal
- Description: Social activities attended

**exercise_hours_per_week** (Float)
- Range: 0 - 15 hours
- Distribution: Exponential (λ=3)
- Description: Physical exercise hours

**extracurricular_hours** (Float)
- Range: 0 - 10 hours
- Distribution: Exponential (λ=2)
- Description: Extracurricular activity hours

## Environmental Factors

**part_time_job_hours** (Integer)
- Range: 0 - 25 hours
- Distribution: Conditional
- Description: Work hours (30% employed)

**commute_time_minutes** (Integer)
- Range: 0 - 120 min
- Distribution: Exponential
- Description: Daily one-way commute

**financial_stress_level** (Float)
- Range: 1 - 5 scale
- Distribution: Beta (α=2, β=5)
- Description: Self-reported financial stress

## Data Generation Methodology

### Research-Based Parameters
- **GPA Distributions**: Based on institutional academic data
- **Study Hours**: Aligned with national student surveys
- **Sleep Patterns**: Reflects college sleep studies
- **Financial Stress**: Derived from student wellness research

### Realistic Correlations
```
# Key relationships built into the data
study_sleep_corr ≈ -0.3
study_gpa_corr ≈ +0.4
social_study_tradeoff ≈ -0.25
```

## Intended Use Cases

### Primary Applications
- Educational Research: Lifestyle-academic performance relationships
- Machine Learning: Predictive model development
- Academic Studies: Student behavior pattern analysis
- Institutional Research: Analytics system prototyping

### Analytical Applications
- Correlation analysis between factors
- Cluster analysis for behavior patterns
- Regression modeling of performance predictors
- Time management and workload studies

## Limitations & Ethical Considerations

### Synthetic Nature
**Note**: This is computer-generated data and may not capture all real-world complexities.

**Generalized Patterns**
- Impact: May miss nuances
- Mitigation: Based on aggregate research

**Institutional Variation**
- Impact: One-size-fits-all
- Mitigation: Customizable parameters

**Cultural Factors**
- Impact: Limited representation
- Mitigation: Research-informed ranges

### Ethical Usage Guidelines
- No Real Data: All records are synthetically generated
- Privacy Protection: No inference to real individuals possible
- Appropriate Use: Research and development only
- Production Warning: Validate with real data before deployment

## Technical Specifications

### File Structure
```
student_id,name,gpa,weekly_study_hours,sleep_hours_per_night,...
STU_0001,John Smith,3.45,28.5,6.8,...
STU_0002,Jane Doe,3.78,32.1,7.2,...
```

### Data Types Summary
**String** (2 features)
- student_id, name

**Float** (7 features)
- gpa, weekly_study_hours, sleep_hours_per_night, social_events_per_week, exercise_hours_per_week, financial_stress_level, extracurricular_hours

**Integer** (4 features)
- assignments_due_this_week, classes_per_week, part_time_job_hours, commute_time_minutes

## Sample Statistics

### Descriptive Statistics
**GPA**
- Mean: 3.21
- Std Dev: 0.42
- Min: 2.15
- Max: 3.98

**Study Hours**
- Mean: 25.3
- Std Dev: 7.8
- Min: 11.5
- Max: 48.2

**Sleep Hours**
- Mean: 6.4
- Std Dev: 1.3
- Min: 4.1
- Max: 9.8

### Correlation Matrix (Sample)
**GPA**
- GPA: 1.00
- Study Hours: 0.42
- Sleep: 0.15
- Social: 0.08

**Study Hours**
- GPA: 0.42
- Study Hours: 1.00
- Sleep: -0.31
- Social: -0.27

**Sleep Hours**
- GPA: 0.15
- Study Hours: -0.31
- Sleep: 1.00
- Social: 0.18

**Social Events**
- GPA: 0.08
- Study Hours: -0.27
- Sleep: 0.18
- Social: 1.00

## Citation

When using this dataset, please acknowledge:

"Synthetic College Student Lifestyle Dataset generated for educational research purposes using research-informed parameter distributions."

## Files Included

- `student_lifestyle_dataset.csv` - Main dataset file
- `dataset_documentation.json` - Technical metadata
- `data_generation_script.py` - Generation code (optional)

## Support

This dataset is provided as-is for research and educational purposes. For methodological questions, refer to the accompanying documentation.

---

*Last Updated: 2025*  
*Dataset Version: 1.0*  
*Generated with: Python + Faker + Research Parameters*

