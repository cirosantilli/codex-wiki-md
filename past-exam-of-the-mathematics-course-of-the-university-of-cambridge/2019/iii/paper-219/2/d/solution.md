<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Conditional independence](../../../../../../conditional-independence.md) gives

$$
P(m\mid d_1,\ldots,d_S)
\propto P(m)\prod_{s=1}^SP(d_s\mid m),
\qquad S=N_{\rm sat}.
$$

For each satellite, [Bayes' theorem](../../../../../../bayes-theorem.md) gives $P(d_s\mid m)\propto P(m\mid d_s)/P(m)$. Therefore

$$
P(m\mid\mathbf d)\propto
P(m)^{1-S}\prod_{s=1}^SP(m\mid d_s).
$$

If $\widehat p_0(m)$ is a [kernel density estimator](../../../../../../kernel-density-estimation.md) for the simulated marginal masses and $\widehat p_s(m)$ estimates the posterior based on satellite $s$, then

$$
\boxed{
\widehat{\bar m}=
\frac{\int m\,\widehat p_0(m)^{1-S}
\prod_{s=1}^S\widehat p_s(m)\,dm}
{\int \widehat p_0(m)^{1-S}
\prod_{s=1}^S\widehat p_s(m)\,dm}.}
$$

The one-dimensional integrals can be evaluated by [numerical integration](../../../../../../numerical-integration.md) on a common mass grid.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
