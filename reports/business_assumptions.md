
## Business Assumptions

# Purpose

This document outlines the principal business and statistical assumptions underpinning the motor insurance claim frequency modelling project. These assumptions provide the basis for developing, validating and interpreting the Poisson Generalized Linear Model (GLM).

# Portfolio Stability

The historical motor insurance portfolio is assumed to be broadly representative of future business. Policyholder behaviour, underwriting strategy and the external operating environment are assumed to remain sufficiently stable for historical claim experience to provide meaningful insight into future claim frequency.

# Independent Claim Events

Claim occurrences are assumed to be statistically independent. The occurrence of one policyholder's claim is not assumed to directly influence another policyholder's probability of making a claim.

# Appropriate Exposure Measurement

Policy exposure accurately reflects the period during which each policy was at risk. Exposure values were treated as the model offset to ensure claim frequencies were standardised across policies with different coverage durations.
# Poisson Distribution Assumption

Claim counts are assumed to follow a Poisson distribution where:

Claims are discrete events.
Events occur independently.
Expected claim frequency is proportional to policy exposure.
The probability of multiple claims occurring simultaneously is negligible.

These assumptions justify the use of a Poisson Generalized Linear Model for claim frequency modelling.

# Predictor Reliability

The explanatory variables used in the model are assumed to be accurate representations of the underlying policy characteristics. Data validation and preparation were performed to minimise inconsistencies before model development.

# Linear Relationship on the Log Scale

The model assumes that predictor variables have an approximately linear relationship with the logarithm of expected claim frequency after applying the log-link function.

# No Perfect Multicollinearity

Predictor variables are assumed not to exhibit perfect linear dependence. This ensures stable parameter estimation and meaningful interpretation of model coefficients.

# Data Quality

The modelling dataset is assumed to be sufficiently complete, accurate and representative following the data quality assessment, validation and preparation performed during the project.

# Business Interpretation

Model outputs are intended to support actuarial pricing decisions by estimating expected claim frequency rather than predicting individual policyholder behaviour with certainty.

# Practical Considerations

Although the Poisson GLM provides an interpretable and statistically robust framework for claim frequency modelling, real-world insurance portfolios may exhibit overdispersion, changing market conditions or evolving customer behaviour. These factors should be monitored during model deployment and may justify more advanced modelling approaches, such as the Negative Binomial GLM, where appropriate.

# Conclusion

The assumptions documented in this report provide the theoretical foundation for the modelling approach adopted in this project. Following data validation, feature preparation and model evaluation, the assumptions were considered sufficiently appropriate for developing an interpretable and business-relevant claim frequency model.