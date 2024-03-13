# Imputation
As Donald B. Rubin Said 'Imputing one value for a missing datum cannot be correct in general, because we don’t know what value to impute with certainty (if we did, it wouldn’t be missing).'
Multiple Imputation, developed by Donald B. Rubin in the 1970s, emerged as a solution to practical problems with missing income data. Fritz Scheuren's work on a joint project with the Social Security Administration and the U.S. Census Bureau highlighted issues with hot deck imputation, leading to Rubin's idea of using multiple versions of the complete dataset.

Rubin's key insight was that single imputation for missing values could not be generally correct. He proposed creating multiple imputations to capture the uncertainty of missing data, a revolutionary departure from previous methods. The 1977 report outlined how to choose models and derive imputations, emphasizing the Bayesian framework for inference.

Rubin's original proposal focused on studying variation due to uncertainty in imputed values. Though met with skepticism, the methodological and statistical foundation was laid by Rubin in 1987, introducing Rubin's rules for combining repeated complete-data estimates. The report provided essential formulas and conditions for valid statistical inference under multiple imputation.

Tests for parameter combinations and technical improvements for degrees of freedom followed in the 1990s. Multiple imputation faced criticism in this period, with concerns about validity depending on subsequent analysis and bias in estimating variance. The tide turned around 2005, with multiple imputation becoming widely accepted and implemented in major statistical packages.

Today, multiple imputation is the benchmark against which newer methods are compared, marking a significant evolution and acceptance in dealing with missing data.[Stef van Buuren, *Flexible Imputation of Missing Data*](https://stefvanbuuren.name/fimd/)

![Alt Text](./img.png)

Image source: [Ranjit Lall, Thomas Robinson, Efficient Multiple Imputation for Diverse Data in Python and R: MIDASpy and rMIDAS, 2023](https://www.jstatsoft.org/article/view/v107i09)

The analysis of multiple imputation has been well-established for R and SPSS. However, Python users do not have direct access to the same functionality. In an effort to bridge this gap, I have attempted to develop Rubin's rules and analysis for multiple imputation in Python, aiming to establish it as the benchmark for imputations.
