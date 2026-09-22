<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

A 95 percent [confidence set](../../../../../confidence-region.md) is a measurable data-dependent set $C(X_1,\ldots,X_n)$ whose repeated-sampling coverage satisfies $\mathbb P_\theta\{\theta\in C(X_1,\ldots,X_n)\}\ge0.95$ for every parameter value, with equality for an exact 95 percent procedure. The parameter is fixed; the set is random. This is not a posterior probability statement about the parameter after the data have been observed.

For independent [normal random variables](../../../../../gaussian-random-variable.md) of known variance, $\overline X\sim N(\mu,\sigma^2/n)$, so $(\overline X-\mu)/(\sigma/\sqrt n)$ has the standard [normal distribution](../../../../../normal-distribution.md). The supplied quantile gives the exact [confidence interval](../../../../../confidence-interval.md)

$$
\boxed{\left[\overline X-1.960\frac\sigma{\sqrt n},\ \overline X+1.960\frac\sigma{\sqrt n}\right].}
$$

Its deterministic length is $3.920\sigma/\sqrt n$. Requiring this to be at most $\varepsilon$ gives

$$
\boxed{n\ge\frac{(3.920)^2\sigma^2}{\varepsilon^2},\qquad n_{\min}=\max\!\left(1,\left\lceil\frac{(3.920)^2\sigma^2}{\varepsilon^2}\right\rceil\right).}
$$

Among fixed-length intervals based equivariantly on the sample mean, the centred interval has greatest coverage: an interval of a given length captures most mass of a symmetric unimodal [normal distribution](../../../../../normal-distribution.md) when centred on its mean. Thus the width calculation is sharp for the usual fixed-length normal-mean construction.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
