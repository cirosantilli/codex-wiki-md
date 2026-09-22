<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For parameter of interest $\psi$ and nuisance parameter $\lambda$, the [profile likelihood](../../../../../../profile-likelihood.md) has log form $\ell_p(\psi)=\ell(\psi,\widehat\lambda_\psi)$, where $\widehat\lambda_\psi$ is the constrained nuisance maximum. Profiling optimizes over the nuisance dimension but does not account for its local volume or conditioning geometry. The [modified profile likelihood](../../../../../../modified-profile-likelihood.md) corrects this loss.

Use ancillary sample coordinates $(\widehat\psi,\widehat\lambda,a)$, and let $j_{\lambda\lambda}(\psi,\widehat\lambda_\psi)=-\ell_{\lambda\lambda}$ be the nuisance block of [observed information](../../../../../../observed-fisher-information.md). Holding $\widehat\psi,a$ fixed, put $D(\psi)=|\partial\widehat\lambda_\psi/\partial\widehat\lambda|$. The [Barndorff-Nielsen modified profile likelihood](../../../../../../modified-profile-likelihood.md) is, up to data-only factors,

$$
\boxed{\ell_m(\psi)=\ell_p(\psi)-\frac12\log|j_{\lambda\lambda}(\psi,\widehat\lambda_\psi)|-\log D(\psi).}
$$

This combines a nuisance-information determinant and a data-coordinate [Jacobian determinant](../../../../../../jacobian-determinant.md). Implicit differentiation of $\ell_\lambda(\psi,\widehat\lambda_\psi)=0$ gives $\partial\widehat\lambda_\psi/\partial\widehat\lambda=j_{\lambda\lambda}^{-1}\ell_{\lambda;\widehat\lambda}$, so equivalently

$$
\ell_m(\psi)=\ell_p(\psi)+\frac12\log|j_{\lambda\lambda}|-\log|\ell_{\lambda;\widehat\lambda}|.
$$

The semicolon denotes differentiation in the varying sample coordinate, rather than a parameter derivative. This form also explains the positive adjustment in Question 2: in that canonical conditional problem the mixed sample derivative is data-only, leaving the positive half-log curvature. The adjustment sign cannot be copied between unrelated constructions without tracking their Jacobians.

In an appropriate orthogonal nuisance formulation, the [Cox-Reid adjusted profile likelihood](../../../../../../cox-reid-adjusted-profile-likelihood.md) uses $\ell_p-\tfrac12\log|j_{\lambda\lambda}|$. It is a useful simpler adjustment, but discarding $D$ is not universally legitimate. For normal data with interest $\sigma^2$ and nuisance $\mu$, the constrained and full nuisance fits both equal $\bar X$, so $D=1$ and $j_{\mu\mu}=n/\sigma^2$. Thus

$$
\ell_m(\sigma^2)=-\frac{n-1}{2}\log\sigma^2-\frac{\sum_i(X_i-\bar X)^2}{2\sigma^2}+\text{constant},
$$

recovering the residual degrees of freedom and fitted variance $\sum_i(X_i-\bar X)^2/(n-1)$. These adjustments target nuisance-related bias and higher-order likelihood inference; they are approximations to conditional or marginal constructions, not an assertion that profiling has become an exact full sampling density.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
