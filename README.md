# logistic-regression-theory-and-practice
A complete, hands-on walkthrough of logistic regression — from mathematical foundations and manual implementation to scikit-learn modeling, with in-depth coverage of regularisation, feature scaling, class imbalance, and model interpretation.

## Introduction

## Why Logistic Regression?

Logistic regression is the workhorse of **binary classification**—the task of predicting whether an observation belongs to class 0 or class 1.  
Despite its name, it is **not** a regression algorithm for continuous targets; rather, it models the *probability* of class membership using a logistic (sigmoid) curve.

* **Intuition**  
  - Linear regression lets predicted values wander from $-\infty$ to $+\infty$.  
  - Classification, however, demands outputs bounded in $[0,1]$ so they can be interpreted as probabilities.  
  - Logistic regression achieves this by passing a linear combination of features through the sigmoid function:
    $$
      \hat{p} = \sigma(z) = \frac{1}{1 + e^{-z}},\quad 
      \text{where } z = \beta_0 + \beta_1x_1 + \dots + \beta_kx_k.
    $$

* **Why start here?**  
  - It is **interpretable**: coefficients translate into *odds ratios* that non-technical stakeholders grasp.  
  - It scales gracefully from a single predictor to thousands of sparse features.  
  - Many modern classifiers (neural nets, transformers) still end with a logistic layer for binary outputs.


* **What you’ll learn in this notebook**  
  1. The mathematical foundations: likelihood, log-odds, and cross-entropy loss.  
  2. A from-scratch NumPy implementation using gradient descent.  
  3. A production-ready approach with `scikit-learn`.
  4. Practical tips: handling class imbalance, feature scaling, regularisation, and model interpretation.

By mastering logistic regression, you build a solid springboard to more advanced classification techniques while retaining a firm grasp on the underlying statistics.

📖 Medium Article (x minutes read): 

---
Max Wienandts
- LinkedIn: https://www.linkedin.com/in/max-wienandts/
- Medium: https://medium.com/@maxwienandts
- GitHub: https://github.com/MaxWienandts
- Buy me a coffee: https://www.paypal.com/donate/?hosted_button_id=2F444HZGJBNX6
