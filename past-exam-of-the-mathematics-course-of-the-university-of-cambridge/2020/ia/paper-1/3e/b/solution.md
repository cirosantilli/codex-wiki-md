<h1 id="3e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<\varepsilon<e^{-1}$, set $u=\log(1/x)$. The ordinary [change of variables formula](../../../../../../change-of-variables-formula.md) gives

$$
\int_\varepsilon^{e^{-1}}
\frac{dx}{x(\log(1/x))^\theta}
=\int_1^{\log(1/\varepsilon)}u^{-\theta}\,du.
$$

Taking $\varepsilon\downarrow0$ is exactly the defining [limit](../../../../../../limit-of-a-function.md) of the [improper integral](../../../../../../improper-integral.md). By the [improper power integral](../../../../../../improper-power-integral.md), it converges for $\theta>1$, and

$$
\boxed{\int_0^{e^{-1}}
\frac{dx}{x(\log(1/x))^\theta}
=\int_1^\infty u^{-\theta}\,du
=\frac1{\theta-1}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3E](../../3e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
