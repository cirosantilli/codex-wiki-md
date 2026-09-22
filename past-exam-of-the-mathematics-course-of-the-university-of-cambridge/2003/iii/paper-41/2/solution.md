<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [conditional likelihood](../../../../../conditional-likelihood.md) is the conditional density of the observed data given a chosen statistic, viewed as a function of the parameter. Conditioning can eliminate a nuisance parameter if the statistic is sufficient for it within the relevant family. The conditioning statistic need not be ancillary; conditioning can also discard some information about the parameter of interest.

For the canonical family, let $T_1=\sum_i\tau_1(Y_i)$ and $s=n^{-1}\sum_i\tau_2(Y_i)$. Normalization of the density gives the [cumulant-generating function](../../../../../cumulant-generating-function.md) of one nuisance statistic:

$$
K_{\psi,\lambda}(t)=\log\mathbb E_{\psi,\lambda}e^{t\tau_2(Y_i)}=d(\psi,\lambda+t)-d(\psi,\lambda).
$$

For the sample mean $S$, it is $K_S(t)=n[d(\psi,\lambda+t/n)-d(\psi,\lambda)]$. Differentiation gives $d_\lambda=\mathbb E\tau_2(Y_i)$ and $d_{\lambda\lambda}=\operatorname{Var}(\tau_2(Y_i))$.

Assume an interior saddle with positive curvature and the usual smooth nonlattice density conditions. Define $\widehat\lambda_\psi$ by

$$
d_\lambda(\psi,\widehat\lambda_\psi)=s.
$$

This is the constrained [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) of $\lambda$ with $\psi$ held fixed. The exponential tilt parameter for one summand is $\widehat t=\widehat\lambda_\psi-\lambda$. Tilting puts the sample mean at $s$, where its tilted density has leading normal value $\sqrt{n/[2\pi d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)]}$. Undoing the tilt gives the [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md)

$$
\widehat f_S(s;\psi,\lambda)=\left[\frac{n}{2\pi d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)}\right]^{1/2}\exp\left\{n[d(\psi,\widehat\lambda_\psi)-d(\psi,\lambda)-(\widehat\lambda_\psi-\lambda)s]\right\}.
$$

This is the density of the mean, not the sum; their factors differ by $n$.

The sample [log-likelihood](../../../../../log-likelihood.md) is $\ell(\psi,\lambda)=\psi T_1+n\lambda s-nd(\psi,\lambda)-\sum_iQ(Y_i)$. Conditional on $S=s$, the factor involving $\lambda$ is constant on the conditioning surface, so the conditional distribution is free of $\lambda$. Subtracting the saddlepoint log-density from the joint log-likelihood now cancels all the original nuisance terms:

$$
\ell(\psi,\lambda)-\log\widehat f_S(s;\psi,\lambda)=\ell(\psi,\widehat\lambda_\psi)+\frac12\log d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)-\frac12\log\frac n{2\pi}.
$$

The final term, and any conditioning-coordinate factor, are data-only constants. Thus the [saddlepoint conditional likelihood adjustment](../../../../../saddlepoint-conditional-likelihood-adjustment.md) is

$$
\boxed{\ell_c(\psi)\approx\ell(\psi,\widehat\lambda_\psi)+\frac12\log|d_{\lambda\lambda}(\psi,\widehat\lambda_\psi)|.}
$$

The absolute-value notation agrees with the question; positive variance makes it unnecessary in this regular setting. The sign of this correction is positive, because a nuisance-statistic density with inverse-square-root curvature has been divided out. A lattice-valued statistic requires the corresponding mass approximation, and a boundary or zero-variance saddle is outside the stated regular density calculation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
