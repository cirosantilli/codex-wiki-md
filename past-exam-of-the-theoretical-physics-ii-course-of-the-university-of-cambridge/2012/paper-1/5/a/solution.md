<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Split the [time-evolution operator](../../../../../time-evolution-operator.md) into $N$ factors with $\epsilon=T/N$, and insert $N-1$ [position](../../../../../position.md) [completeness relations](../../../../../resolution-of-the-identity.md) between them. Each factor is evaluated by inserting [momentum](../../../../../momentum-split.md) states normalized by $\langle x|p\rangle=(2\pi\hbar)^{-1/2}e^{ipx/\hbar}$:

$$
\begin{aligned}
\langle x_{j+1}|e^{-i\epsilon p^2/(2m\hbar)}|x_j\rangle
&=\int_{\mathbb R}\frac{dp}{2\pi\hbar}
\exp\left[\frac{ip(x_{j+1}-x_j)}{\hbar}
-\frac{i\epsilon p^2}{2m\hbar}\right]\\
&=\sqrt{\frac{m}{2\pi i\hbar\epsilon}}\,
\exp\left[\frac{im(x_{j+1}-x_j)^2}{2\hbar\epsilon}\right].
\end{aligned}
$$

Multiplying the $N$ kernels and integrating the intermediate [positions](../../../../../position.md) produces the stated time-sliced [path integral](../../../../../path-integral.md), including its $N/2$ normalization power. For a [free particle](../../../../../free-particle.md) this [Gaussian](../../../../../normal-distribution.md) short-time kernel is exact, so the convolution identity already holds at finite $N$. Oscillatory [integrals](../../../../../integral-split.md) are defined with a vanishing convergence regulator, consistently fixing the square-root phase.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
