# obulezi-approximation-r
R implementation and benchmarking suite for the Obulezi Approximation: an $O(n^{-3})$ log-Taylor expansion for high-precision Bayesian posterior expectations.
# Obulezi Approximation: An $O(n^{-3})$ Log-Taylor Expansion for Bayesian Posterior Expectations

[![R Version](https://img.shields.io/badge/R-%E2%89%A5%204.0-blue.svg)](https://www.r-project.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository provides the official R implementation and replication benchmarking suite for the **Obulezi Approximation**, a non-linear log-Taylor series expansion that elevates analytical Bayesian integration to an $O(n^{-3})$ relative error rate. 

By explicitly incorporating functional log-gradient interaction vectors ($\boldsymbol{v}^*$) and pure posterior kernel kurtosis cumulants ($\mathcal{K}_{\text{kernel}}^*$) at the shifted mode ($\hat{\boldsymbol{\theta}}^*$), the proposed method addresses the small-sample ($n \le 25$) truncation errors inherent in standard Lindley $O(n^{-1})$ and Tierney–Kadane $O(n^{-2})$ Laplace approximations.

---

## 📁 Repository Structure

```text
├── script for independent gamma priors.R  # Bivariate Weibull model (p=2) under independent Gamma priors
├── script for alternative priors.R        # Prior invariance suite (e.g., Correlated Bivariate Log-Normal)
├── higher dimension script.R              # 4D Bayesian Logistic Regression (p=4, M=500 MC replications)
├── LICENSE                                # MIT License
└── README.md                              # Repository documentation
