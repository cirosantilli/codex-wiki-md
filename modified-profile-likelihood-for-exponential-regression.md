# Modified profile likelihood for exponential regression

↑ **Parent:** [Modified profile likelihood](modified-profile-likelihood.md)

For independent [exponential distributions](exponential-distribution.md) with means $\lambda e^{\psi x_i}$ and a nonconstant fixed design, put $A(\psi)=\sum_iY_ie^{-\psi x_i}$. The constrained [maximum-likelihood estimate](maximum-likelihood-estimator.md) is $\widetilde\lambda_\psi=A(\psi)/n$ and the [profile log-likelihood](profile-log-likelihood.md) is $\ell_p(\psi)=-n\log[A(\psi)/n]-\psi\sum_i x_i-n$. Use the [ancillary statistic](ancillary-statistic.md) $a_i=\log Y_i-\log\widehat\lambda-\widehat\psi x_i$ to specify sample coordinates. At fixed $\widehat\psi,a$, the [Jacobian determinant](jacobian-determinant.md) $\partial\widetilde\lambda_\psi/\partial\widehat\lambda=\widetilde\lambda_\psi/\widehat\lambda$, while $j_{\lambda\lambda}(\psi,\widetilde\lambda_\psi)=n/\widetilde\lambda_\psi^2$. Therefore the [modified profile likelihood](modified-profile-likelihood.md) satisfies

$$
\ell_m(\psi)=\ell_p(\psi)-\tfrac12\log j_{\lambda\lambda}-\log\left|\frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}\right|=\ell_p(\psi)+\log\widehat\lambda-\tfrac12\log n.
$$

The adjustment is independent of $\psi$. Keeping only the [observed information](observed-fisher-information.md) adjustment would miss this cancellation.

## ↑ Ancestors (11)

1. [Modified profile likelihood](modified-profile-likelihood.md)
2. [Profile likelihood](profile-likelihood.md)
3. [Likelihood function](likelihood-function.md)
4. [Maximum-likelihood estimator](maximum-likelihood-estimator.md)
5. [Maximum likelihood estimation](maximum-likelihood-estimation.md)
6. [Statistical modelling](statistical-modelling-split.md)
7. [Statistical model](statistical-model-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/2/solution.md)
