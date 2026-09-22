<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [marginal statistical likelihood](../../../../../marginal-likelihood-from-a-nuisance-free-statistic.md) uses a statistic whose marginal sampling distribution depends on the parameter of interest but does not involve the [nuisance parameter](../../../../../nuisance-parameter.md). It integrates out other observed coordinates. A [profile likelihood](../../../../../profile-likelihood.md) instead keeps the full data and, for every fixed interest parameter, fits the [nuisance parameter](../../../../../nuisance-parameter.md) by maximizing the full [likelihood](../../../../../likelihood-function.md). Profiling supplies a [likelihood](../../../../../likelihood-function.md) function but usually not a normalized sampling [probability density function](../../../../../probability-density-function.md). Here the marginalization is of data coordinates; Bayesian model evidence averages parameters against a prior and is a separate construction.

Use shape-rate notation for the [gamma distribution](../../../../../gamma-distribution.md). The independent sums have $X\sim\operatorname{Gamma}(m,\psi\lambda)$ and $Y\sim\operatorname{Gamma}(n,\lambda)$, so their [joint probability density](../../../../../joint-probability-density.md) for $x,y>0$ is

$$
f_{X,Y}(x,y)=\frac{\psi^m\lambda^{m+n}}{\Gamma(m)\Gamma(n)}x^{m-1}y^{n-1}e^{-\lambda(\psi x+y)}.
$$

For $x=tu$, $y=u$ the absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is u. Therefore

$$
f_{T,U}(t,u)=\frac{\psi^m\lambda^{m+n}}{\Gamma(m)\Gamma(n)}t^{m-1}u^{m+n-1}e^{-\lambda(1+\psi t)u},\qquad t,u>0.
$$

Integrate u using the gamma integral $\int_0^\infty u^{m+n-1}e^{-bu}du=\Gamma(m+n)b^{-(m+n)}$. The lambda factors cancel, leaving

$$
\boxed{f_T(t)=\frac{\Gamma(m+n)}{\Gamma(m)\Gamma(n)}\frac{\psi^m t^{m-1}}{(1+\psi t)^{m+n}},\qquad t>0.}
$$

Thus T gives a nuisance-free marginal [likelihood](../../../../../likelihood-function.md). Discarding only terms independent of psi, its logarithm is

$$
\boxed{\ell_m(\psi;t)=m\log\psi-(m+n)\log(1+\psi t).}
$$

The factor t in the logarithm is required, as in the original PDF.

The full [log-likelihood](../../../../../log-likelihood.md) is $m\log\psi+(m+n)\log\lambda-\lambda(\psi x+y)+c(x,y)$. Its lambda derivative vanishes uniquely at

$$
\boxed{\widehat\lambda_\psi=\frac{m+n}{\psi x+y}.}
$$

The second derivative in lambda is negative. Substituting this maximum gives $\ell_p(\psi)=m\log\psi-(m+n)\log(\psi x+y)+c'(x,y)$. Since $\psi x+y=y(1+\psi t)$, it agrees with $\ell_m(\psi;t)$ up to a psi-independent constant. This proves the [Gamma-ratio marginal and profile likelihood identity](../../../../../gamma-ratio-marginal-and-profile-likelihood-identity.md). Their common maximizer is $\widehat\psi=m/(nt)=my/(nx)$, if an interest-parameter estimate is also wanted.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
