<h1 id="6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Partition a regular parameter into interest $\psi$ and nuisance $\lambda$. [Parameter orthogonality](../../../../../../orthogonal-statistical-parameters.md) means the cross-block of the expected [Fisher information matrix](../../../../../../fisher-information-matrix.md) vanishes:

$$
\boxed{I_{\psi\lambda}=\mathbb E[U_\psi U_\lambda^\top]=-\mathbb E\ell_{\psi\lambda}=0.}
$$

It is expected-information orthogonality, not a demand that every observed cross derivative be zero. To first order, the asymptotic normal distribution of the joint [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) has independent interest and nuisance blocks. Its efficient interest information simplifies from the Schur complement $I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}$ to $I_{\psi\psi}$.

For scalar interest, new nuisance coordinates $\eta$ can locally be chosen by the [local orthogonal nuisance reparametrization](../../../../../../local-orthogonal-nuisance-reparametrization.md)

$$
\partial_\psi\lambda(\psi,\eta)=-I_{\lambda\lambda}^{-1}I_{\lambda\psi}.
$$

Indeed the new interest score is $U_\psi+(\partial_\psi\lambda)^\top U_\lambda$, and its expected product with the transformed nuisance score is zero by this equation. Smoothness, nonsingular nuisance information and suitable initial coordinates provide the local ordinary-differential-equation construction. Simultaneous orthogonalization for several interest coordinates may face integrability constraints.

For normal location and variance $(\mu,\sigma^2)$, the cross information is zero: the location score is proportional to the centered observation and the variance score to its squared value minus its expectation, whose product has zero expectation by normal symmetry. This is a useful orthogonal parameterization. In general orthogonality reduces nuisance sensitivity and motivates adjusted profile constructions, but it implies neither exact estimator independence nor an exact nuisance-free conditional likelihood.

## ↑ Ancestors (11)

1. [V](../v.md)
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
