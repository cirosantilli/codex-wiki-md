<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The head of the [Brownian snake](../../../../../../../brownian-snake.md) driven by $g$ is the centered [Gaussian process](../../../../../../../gaussian-process.md) $(Z_t)_{0\leq t\leq1}$ with [covariance function](../../../../../../../covariance-function.md) $\mathbb E[Z_sZ_t]=m_g(s,t)$. Part i shows that these [finite-dimensional distributions](../../../../../../../finite-dimensional-distribution.md) exist consistently. Moreover,

$$
\mathbb E[(Z_t-Z_s)^2]
=g(s)+g(t)-2m_g(s,t)=d_g(s,t).
$$

If $g$ has Hölder constant $L$, then $d_g(s,t)\leq2L|t-s|^\alpha$. The [absolute moment](../../../../../../../absolute-moment.md) formula for a centered [normal distribution](../../../../../../../normal-distribution.md) consequently gives, for every $p\geq2$,

$$
\mathbb E|Z_t-Z_s|^p\leq C_{p,L}|t-s|^{\alpha p/2}.
$$

The [Kolmogorov continuity theorem](../../../../../../../kolmogorov-continuity-theorem.md), with $p$ arbitrarily large, produces a modification that is $\gamma$-Hölder continuous for every $\gamma<\alpha/2$. Taking $\gamma=\alpha/2-\varepsilon$ proves the claim whenever $0<\varepsilon<\alpha/2$; for larger $\varepsilon$ the assertion is vacuous.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 220](../../../../paper-220-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
