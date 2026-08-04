# Data Quality Assessment Report

## Project

Motor Insurance Pricing Analytics

---

## Objective

The purpose of this assessment is to evaluate the quality of the motor insurance datasets before conducting exploratory analysis and predictive modelling.

The assessment focuses on identifying missing values, duplicate records, inconsistent data types, invalid values and potential data quality issues that may influence pricing decisions.

---

# Data Sources

## Frequency Dataset

Contains policy-level information including:

- Policy identifier
- Claim count
- Exposure
- Driver characteristics
- Vehicle characteristics
- Geographic information

Number of records:

**678,013**

---

## Severity Dataset

Contains individual claim payments linked to policies.

Number of records:

**26,639**

---

# Data Quality Checks

The following checks were performed:

- Dataset dimensions
- Variable data types
- Missing values
- Duplicate records
- Invalid values
- Range checks
- Consistency checks
- Outlier assessment

---

# Findings

# Findings

The data quality assessment indicates that the datasets are generally of high quality and suitable for actuarial pricing analysis.

Key findings include:

- No missing values were identified in either dataset.
- The frequency dataset contains no duplicate records.
- The severity dataset contains 255 duplicate records that require further investigation to determine whether they represent genuine duplicate observations or multiple claims with identical values.
- Policy exposure values are positive, with an average exposure of approximately 0.53 years.
- A small number of policies have exposure values greater than one year, which will be documented as a known characteristic of the dataset.
- Claim amounts exhibit a strongly right-skewed distribution with a small number of very large claims.
- Overall, the datasets demonstrate good completeness and consistency and are suitable for exploratory analysis and predictive modelling.

---

# Conclusion

# Conclusion

The datasets passed the initial data quality assessment and are considered suitable for actuarial pricing analysis.

Only minor data preparation is anticipated before modelling. Particular attention will be given to duplicate claim records, exposure values greater than one year, and the treatment of large claim amounts during exploratory data analysis.
