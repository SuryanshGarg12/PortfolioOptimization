# Portfolio Optimization with Robust Covariance and CVaR Constraints

This repository implements the research paper: 
**"Portfolio Optimization with Robust Covariance and Conditional Value-at-Risk Constraints"** by Qiqin Zhou (Cornell University), arXiv:2406.00610.

## 🧠 Overview

This project explores various methods to estimate robust covariance matrices and optimize portfolios under Conditional Value-at-Risk (CVaR) constraints. The goal is to construct portfolios that are both stable and capable of handling extreme market conditions.

Implemented techniques include:

- **Ledoit-Wolf Shrinkage Estimator**
- **Gerber Robust Covariance Matrix**
- **CVaR-constrained Minimum Variance Portfolios**

---

## 📁 Repository Structure

```
.
├── BasePortfolio.ipynb           # Benchmark: Exp. Sample & Std Gerber
├── ledoit_wolf.ipynb             # Ledoit-Wolf covariance estimator
├── GerberMethod.ipynb            # Gerber covariance (Std & MAD)
├── Untitled3.ipynb               # 1-CVaR and 2-CVaR portfolio optimization
├── 2406.00610v1.pdf              # Research paper reference
└── README.md                     # This file
```

---

## 📊 Data

- **Universe**: 55 Indian stocks (top 5 market-cap from each of 11 sectors)
- **Time Range**: Jan 2012 – Jan 2022
- **Sampling Frequency**: Weekly
---

## 🔧 Techniques & Models

### Covariance Estimators

- **Exponentially Weighted Sample Covariance**
- **Ledoit-Wolf Shrinkage Covariance**
- **Gerber Covariance Matrix**:
  - Based on significant co-movements
  - Thresholds using:
    - Standard Deviation (Std)
    - Median Absolute Deviation (MAD)
---


## 📦 Requirements

```bash
pip install numpy pandas matplotlib seaborn scikit-learn cvxpy
```

---

## 📚 References

1. Jobson, J. D., & Korkie, B. (1980). *Estimation for Markowitz Efficient Portfolios*. Journal of the American Statistical Association, 75(371), 544–554.
2. Frost, P. A., & Savarino, J. E. (1988). *For better performance: Constrain portfolio weights*. Journal of Portfolio Management, 15(1), 29–34.
3. Ledoit, O., & Wolf, M. (2003). *Improved estimation of the covariance matrix of stock returns with an application to portfolio selection*. Journal of Empirical Finance, 10(5), 603–621.
4. Ledoit, O., & Wolf, M. (2004). *Honey, I Shrunk the Sample Covariance Matrix*. The Journal of Portfolio Management, 30(4), 110–119.
5. Rousseeuw, P. J. (1984). *Least Median of Squares Regression*. Journal of the American Statistical Association, 79(388), 871–880.
6. López de Prado, M. (2019). *A Robust Estimator of the Efficient Frontier*. Available at SSRN: https://ssrn.com/abstract=3469961.
7. Gerber, S., Markowitz, H. M., Ernst, P. A., et al. (2022). *The Gerber Statistic: A Robust Co-Movement Measure for Portfolio Optimization*. The Journal of Portfolio Management, 48(3), 87–102.
8. Rockafellar, R. T., & Uryasev, S. (2000). *Optimization of Conditional Value-at-Risk*. The Journal of Risk, 2, 21–41.
9. Alexander, G. J., & Baptista, A. M. (2004). *A comparison of VaR and CVaR constraints on portfolio selection with the mean-variance model*. Management Science, 50(9), 1261–1273.
10. Zhou, Q. (2024). *Portfolio Optimization with Robust Covariance and Conditional Value-at-Risk Constraints*. arXiv:2406.00610. https://arxiv.org/abs/2406.00610

---
