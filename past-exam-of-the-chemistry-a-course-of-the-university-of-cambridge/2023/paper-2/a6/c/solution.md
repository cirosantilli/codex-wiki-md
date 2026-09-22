<h1 id="a6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [uniform-binding multilayer adsorption model](../../../../../uniform-binding-multilayer-adsorption-model.md), $\theta_j$ describes sites of **exactly** height $j$, not the fraction whose height is at least $j$. At equilibrium the upward and downward fluxes on each adjacent pair of heights balance:

$$
k_a p\theta_{j-1}=k_d\theta_j,\qquad j\geq1.
$$

For completeness, stationarity alone gives a height-independent probability current; the reflecting boundary at height zero sets that current to zero. This justifies pairwise balance for a normalizable equilibrium distribution.

Writing $x=K_{\rm ads}p$ gives the recurrence $\theta_j=x\theta_{j-1}$. Successive substitution then yields

$$
\theta_1=x\theta_0,\qquad \theta_2=x^2\theta_0,\qquad
\boxed{\theta_j=x^j\theta_0=(K_{\rm ads}p)^j\theta_0}.
$$

An equilibrium [geometric distribution](../../../../../geometric-distribution.md) of unbounded heights requires $0\leq x<1$. The first-layer-only [Langmuir adsorption model](../../../../../langmuir-adsorption-model.md) instead truncates the allowed heights at one, which changes the normalization and removes this convergence restriction.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [A6](../../a6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
