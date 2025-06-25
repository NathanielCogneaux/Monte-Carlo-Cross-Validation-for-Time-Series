# Monte Carlo Cross-Validation for Time Series

In traditional bootstrap methods, a key question is whether to sample with or without replacement. When it comes to Monte Carlo Cross-Validation for time series (i.e., randomized sliding walk-forward windows), I found that there was no readily available implementation of a **without-replacement** variant that integrates well with the scikit-learn framework, so I'm working on one!

This approach is particularly useful when your dataset is limited and you want more diverse validation splits than standard time series cross-validation allows, while still **avoiding repeated or heavily overlapping out-of-sample sets**. 

The goal is to implement a variant of Monte Carlo Time Series Cross-Validation that:
- Samples **without replacement**,
- **Minimizes overlap** between out-of-sample windows,
- Ensures **broad and diverse coverage** of the dataset,
- Remains compatible with the scikit-learn interface.

Stay tuned, testing and refinements will follow!
