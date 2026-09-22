<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Parameters $\psi$ and $\lambda$ are [orthogonal parameters](../../../../../../orthogonal-statistical-parameters.md) if the cross block of the expected [Fisher information matrix](../../../../../../fisher-information-matrix.md) is zero throughout the relevant parameter region:

$$
I_{\psi\lambda}=\mathbb E_\theta[\ell_\psi\ell_\lambda^T]=-\mathbb E_\theta\ell_{\psi\lambda}=0.
$$

This is a statement about expected information, not a requirement that every observed cross derivative vanish. For regular [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md), $\sqrt n(\widehat\theta-\theta)$ has limiting [covariance](../../../../../../covariance.md) equal to the inverse per-observation [Fisher information matrix](../../../../../../fisher-information-matrix.md). Block diagonality therefore gives asymptotically [independent](../../../../../../independent-random-variables.md) fitted interest and [nuisance parameters](../../../../../../nuisance-parameter.md). The efficient information $I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}$ reduces to $I_{\psi\psi}$ at an orthogonal parametrization, although nuisance estimation can still matter at higher orders.

For scalar interest and nuisance, retain $\psi$ and write the old nuisance as $\lambda=\lambda(\psi,\eta)$. The transformed cross information is $\lambda_\eta(I_{\psi\lambda}+\lambda_\psi I_{\lambda\lambda})$. Hence an orthogonal nuisance coordinate can locally be found from

$$
\boxed{\lambda_\psi=-I_{\psi\lambda}/I_{\lambda\lambda},\qquad I_{\lambda\lambda}>0,}
$$

subject to local solvability and a nonsingular coordinate change. Global coordinates need not follow from this local construction. For the [normal distribution](../../../../../../normal-distribution.md) with separately varying mean and [variance](../../../../../../variance-split.md) parameters $(\mu,v)$, the scores are $(Y-\mu)/v$ and $-1/(2v)+(Y-\mu)^2/(2v^2)$; their product has zero [expectation](../../../../../../expected-value.md) by symmetry. Thus the per-observation information is diagonal with entries $1/v$ and $1/(2v^2)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
