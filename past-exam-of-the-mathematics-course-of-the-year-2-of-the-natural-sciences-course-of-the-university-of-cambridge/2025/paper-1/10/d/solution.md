<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

It is enough to choose an admissible parameter, without solving the minimizing equation. Take $a=V_0^2>0$ in the [Gaussian variational bound for an attractive Gaussian well](../../../../../gaussian-variational-bound-for-an-attractive-gaussian-well.md). The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives

$$
E_0\leq\frac{V_0^2}{2}-\frac{V_0^2}{\sqrt{1+V_0^2}}=-\frac{V_0^2}{2}+\varepsilon,
$$

where an explicit remainder is

$$
\varepsilon=V_0^2\left(1-\frac1{\sqrt{1+V_0^2}}\right)=\frac{V_0^4}{\sqrt{1+V_0^2}(\sqrt{1+V_0^2}+1)}.
$$

The denominator tends to $2$ as $V_0\to0$, proving $\varepsilon=O(V_0^4)$ in [Big O notation](../../../../../big-o-notation.md). More precisely the [binomial series](../../../../../binomial-series.md) gives

$$
\varepsilon=\frac12V_0^4-\frac38V_0^6+O(V_0^8),
$$

and therefore

$$
\boxed{E_0\leq-\frac12V_0^2+\varepsilon,\qquad\varepsilon=O(V_0^4).}
$$

This is an upper bound on the exact [ground state](../../../../../ground-state.md) energy, rather than an assertion that the leading coefficient of its exact weak-potential expansion is $-1/2$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
