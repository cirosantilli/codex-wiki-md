<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [profile likelihood](../../../../../profile-likelihood.md) for the parameter of interest replaces the [nuisance parameter](../../../../../nuisance-parameter.md) by its constrained best fit: $L_p(\psi)=\sup_\lambda L(\psi,\lambda)$, with $\ell_p(\psi)=\ell(\psi,\widehat\lambda_\psi)$. It is not in general a normalized sampling density. A [conditional likelihood](../../../../../conditional-likelihood.md) instead uses the sampling law conditional on a statistic carrying the nuisance dependence. In the canonical [exponential family](../../../../../exponential-family-split.md) here, conditioning on $S$ removes $\lambda$ because the factor involving $\lambda$ is constant over the conditioning fibre.

Let $\bar T_1=n^{-1}\sum_i\tau_1(y_i)$ and let the observed $S$ equal $s$. For the [cumulant-generating function](../../../../../cumulant-generating-function.md) of $\tau_2(Y)$ at fixed $\psi$,

$$
K(t)=d(\psi,\lambda+t)-d(\psi,\lambda).
$$

The saddlepoint solves $K'(\widehat t)=s$, equivalently $d_\lambda(\psi,\widehat\lambda_\psi)=s$ with $\widehat\lambda_\psi=\lambda+\widehat t$. This is also the constrained [likelihood](../../../../../likelihood-function.md) equation, since $\ell_\lambda=n(s-d_\lambda)$. Assume an interior saddle, $d_{\lambda\lambda}>0$, and the usual smooth nonlattice conditions under which $S$ has a density. [Exponential tilting](../../../../../exponential-tilting.md) to $\widehat\lambda_\psi$ makes $s$ the tilted mean. A local [normal approximation](../../../../../normal-approximation.md) gives tilted density $\{n/(2\pi d_{\lambda\lambda}(\psi,\widehat\lambda_\psi))\}^{1/2}$ at that mean; undoing the tilt gives the [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md)

$$
\boxed{\widehat f_S(s;\psi,\lambda)=\left[\frac{n}{2\pi d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)}\right]^{1/2}
\exp\left\{n\left[d(\psi,\widehat\lambda_\psi)-d(\psi,\lambda)-(\widehat\lambda_\psi-\lambda)s\right]\right\}.}
$$

The factor $n^{1/2}$ is for the [sample mean](../../../../../sample-mean.md), rather than the sum. A transform-based derivation gives the same expression by expanding $K$ to second order at its stationary point.

The joint [log-likelihood](../../../../../log-likelihood.md) is $n\psi\bar T_1+n\lambda s-nd(\psi,\lambda)-\sum_iQ(y_i)$. Subtracting $\log\widehat f_S(s;\psi,\lambda)$ cancels every appearance of the original $\lambda$, leaving

$$
\widehat\ell_c(\psi)=n\psi\bar T_1+n\widehat\lambda_\psi s-nd(\psi,\widehat\lambda_\psi)-\sum_iQ(y_i)
+\frac12\log d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)-\frac12\log\frac n{2\pi}.
$$

Any change from the ambient density to a conditional density on $S=s$ contributes only a data-dependent [Jacobian determinant](../../../../../jacobian-determinant.md). Thus, up to a constant [independent](../../../../../independent-random-variables.md) of $\psi$, the [saddlepoint conditional likelihood adjustment](../../../../../saddlepoint-conditional-likelihood-adjustment.md) is

$$
\boxed{\widehat\ell_c(\psi)=\ell_p(\psi)+B(\psi),\qquad B(\psi)=\frac12\log d_{\lambda\lambda}(\psi,\widehat\lambda_\psi).}
$$

Equivalently $B=\tfrac12\log j_{\lambda\lambda}(\psi,\widehat\lambda_\psi)$ up to the constant $-\tfrac12\log n$, where $j_{\lambda\lambda}=nd_{\lambda\lambda}$ is the nuisance [observed information](../../../../../observed-fisher-information.md). The adjustment has a positive sign. The printed exponential-family form alone does not guarantee a density for $S$: for example a continuous $Y$ can have $\tau_2(Y)=\mathbf1_{\{Y>0\}}$. In a lattice case one must approximate the probability mass of the sum instead; the displayed density calculation uses the regular continuous interpretation.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
