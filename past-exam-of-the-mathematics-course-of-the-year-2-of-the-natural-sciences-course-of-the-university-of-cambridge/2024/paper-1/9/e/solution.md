<h1 id="9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Impose $y=x$ before varying. Writing $\delta=\delta_1+\delta_2$, the restricted integrand is

$$
f_{\mathrm{line}}=\alpha(1+\beta x)+\alpha(\gamma_1+\gamma_2)(1+\beta x)\dot x+\frac\delta2\dot x^2.
$$

Its middle term is the [total derivative](../../../../../total-derivative.md) of $\alpha(\gamma_1+\gamma_2)(x+\beta x^2/2)$, so it can be dropped for fixed endpoints by part (b). The remaining [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $\delta\ddot x=\alpha\beta$. Integrating twice and imposing $x(0)=0$, $x(T)=S$ gives

$$
\boxed{x(t)=y(t)=\frac STt-\frac{\alpha\beta}{2(\delta_1+\delta_2)}t(T-t),\qquad0\leq t\leq T.}
$$

This is the unique [global minimizer](../../../../../global-minimizer.md) among paths on the specified line. To prove it, add any admissible [variation](../../../../../variation.md) $\eta$ with $\eta(0)=\eta(T)=0$. The change in fuel, after dropping the fixed [boundary term](../../../../../boundary-term.md), is

$$
F[x+\eta]-F[x]=\int_0^T[\alpha\beta\eta+\delta\dot x\dot\eta]dt+\frac\delta2\int_0^T\dot\eta^2dt=\frac\delta2\int_0^T\dot\eta^2dt\geq0.
$$

The first [integral](../../../../../integral-split.md) vanishes by [integration by parts](../../../../../integration-by-parts.md) and the equation for $x$. Equality forces $\eta=0$. No monotonicity or restriction to the segment between endpoints was imposed in the question; the minimizing coordinate can initially decrease for sufficiently large $T$.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
