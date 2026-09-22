<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the sign convention in which a [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md) satisfies

$$
\Delta_{\mathbf r}G(\mathbf r,\mathbf r')=\delta^{(2)}(\mathbf r-\mathbf r')
$$

in the sense of [distributions](../../../../../distribution-mathematical-analysis.md). It is a [harmonic function](../../../../../harmonic-function.md) away from the source. Writing $\rho=|\mathbf r-\mathbf r'|$, the radial equation is $(\rho G')'=0$, so $G=A\log\rho+B$. The [divergence theorem](../../../../../divergence-theorem.md) on a small circle about the source fixes its total flux:

$$
1=\int_{\rho<\varepsilon}\Delta G\,d^2r
=\int_{\rho=\varepsilon}\partial_\rho G\,ds
=\frac A\varepsilon(2\pi\varepsilon)=2\pi A.
$$

Consequently

$$
\boxed{G(\mathbf r,\mathbf r')=\frac1{2\pi}\log|\mathbf r-\mathbf r'|+B}.
$$

The arbitrary constant is a [harmonic function](../../../../../harmonic-function.md). For the alternative convention $-\Delta G=\delta^{(2)}$, the logarithm has the opposite sign; subsequent [Green's function](../../../../../green-s-function-split.md) formulas must use that convention consistently.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
