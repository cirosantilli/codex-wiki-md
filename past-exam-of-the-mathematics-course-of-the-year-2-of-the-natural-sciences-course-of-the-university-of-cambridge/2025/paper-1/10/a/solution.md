<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take nonzero real trial functions $y$ with $y,y'$ [square-integrable](../../../../../square-integrable-function.md) and sufficient decay for [integration by parts](../../../../../integration-by-parts.md). For a compactly supported [variation](../../../../../variation.md) $y\mapsto y+\varepsilon\eta$, the [first variations](../../../../../first-variation.md) are

$$
\delta F=2\int_{\mathbb R}(y'\eta'-V_0e^{-x^2}y\eta)\,dx=2\int_{\mathbb R}(-y''-V_0e^{-x^2}y)\eta\,dx,\qquad\delta G=2\int_{\mathbb R}y\eta\,dx.
$$

The [quotient rule](../../../../../quotient-rule.md) for the [functional](../../../../../functional.md) then yields

$$
\delta\Lambda=\frac2{G[y]}\int_{\mathbb R}\left[-y''-V_0e^{-x^2}y-\Lambda[y]y\right]\eta\,dx.
$$

By the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md), stationarity for all such $\eta$ is equivalent to

$$
-y''-V_0e^{-x^2}y=\Lambda[y]y.
$$

Conversely, multiplying a decaying [eigenfunction](../../../../../eigenfunction.md) equation by $y$ and using [integration by parts](../../../../../integration-by-parts.md) gives $F[y]=EG[y]$, so its [Rayleigh quotient](../../../../../rayleigh-quotient.md) equals $E$ and its [first variation](../../../../../first-variation.md) vanishes. Thus the stationary values of the [functional](../../../../../functional.md) are the energy [eigenvalues](../../../../../eigenvalue.md). The word "extrema" in the question includes stationary points here: higher [eigenfunctions](../../../../../eigenfunction.md) can be saddle points of the unrestricted [Rayleigh quotient](../../../../../rayleigh-quotient.md).

The [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives

$$
\boxed{E_0=\inf_{y\ne0}\Lambda[y],\qquad E_0\leq\Lambda[y_T].}
$$

Choose an admissible trial family, calculate its [Rayleigh quotient](../../../../../rayleigh-quotient.md), and minimize over its parameters to obtain the best upper bound within that family. Equality holds for the exact [ground state](../../../../../ground-state.md); a restricted family generally gives only an upper bound.

## ↑ Ancestors (13)

1. [A](../a.md)
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
