<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $y$ be a stationary [function](../../../../../function-split.md) and perturb it to $y_\varepsilon=y+\varepsilon\eta$, where $\eta$ is smooth and $\eta(a)=\eta(b)=0$. These perturbations preserve the prescribed endpoint values. Differentiate the [functional](../../../../../functional.md) at $\varepsilon=0$:

$$
\delta I=\left.\frac{dI[y_\varepsilon]}{d\varepsilon}\right|_{\varepsilon=0}=\int_a^b(F_y\eta+F_{y'}\eta')\,dx.
$$

By [integration by parts](../../../../../integration-by-parts.md),

$$
\delta I=[F_{y'}\eta]_a^b+\int_a^b\left(F_y-\frac d{dx}F_{y'}\right)\eta\,dx.
$$

The boundary term vanishes. The remaining [integral](../../../../../integral-split.md) must vanish for every such $\eta$, so the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\frac{\partial F}{\partial y}-\frac d{dx}\left(\frac{\partial F}{\partial y'}\right)=0.}
$$

It is a necessary stationarity condition; deciding whether the stationary path is a minimum requires additional information.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
