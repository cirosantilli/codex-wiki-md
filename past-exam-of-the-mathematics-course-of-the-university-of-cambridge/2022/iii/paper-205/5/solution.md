<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For disjoint nonempty index sets $A$ and $B$, partition the mean and covariance conformably. The [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) is

$$
Z_A\mid Z_B=z_B
\sim N\left(
\mu_A+\Sigma_{0,A B}\Sigma_{0,B B}^{-1}(z_B-\mu_B),
\Sigma_{0,A A}-\Sigma_{0,A B}\Sigma_{0,B B}^{-1}\Sigma_{0,B A}
\right).
$$

If the sets overlap, the shared coordinates are fixed and this formula applies to $A\setminus B$.

Partition $\Omega_0$ into the $A$ and $A^c$ blocks. The block-inverse formula identifies the displayed conditional covariance with

$$
\operatorname{Var}(Z_A\mid Z_{A^c})
=(\Omega_{0,A,A})^{-1}.
$$

For $A=\{j,k\}$, inversion of the two-by-two precision block gives

$$
\operatorname{Cov}(Z_j,Z_k\mid Z_{-jk})
=-\frac{\Omega_{0,jk}}
{\Omega_{0,jj}\Omega_{0,kk}-\Omega_{0,jk}^2}.
$$

The denominator is positive, so the conditional covariance vanishes exactly when $\Omega_{0,jk}=0$. A Gaussian pair is independent exactly when it is uncorrelated, proving

$$
Z_j\mathrel{\perp\!\!\!\perp}Z_k\mid Z_{-jk}
\quad\Longleftrightarrow\quad
\Omega_{0,jk}=0.
$$

Profiling the Gaussian likelihood over $\mu$ gives $\widehat\mu=\bar X$. Apart from constants and a positive factor, the negative log-likelihood for the [precision matrix](../../../../../precision-matrix.md) is

$$
-\log\det\Omega+\operatorname{tr}(S\Omega).
$$

Its derivative is $-\Omega^{-1}+S$, so the unpenalized minimizer is $S^{-1}$. The [Graphical Lasso](../../../../../graphical-lasso.md) solves

$$
\widehat\Omega_\lambda
\in\operatorname*{argmin}_{\Omega\succ0}
\left\{-\log\det\Omega+\operatorname{tr}(S\Omega)
+\lambda\sum_{j\ne k}|\Omega_{jk}|\right\},
$$

with some conventions also penalizing the diagonal.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
