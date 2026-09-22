<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Poincaré inequality in probability theory](../../../../../../poincare-inequality-in-probability-theory.md) to $g=e^{\lambda f/2}$. Since $\lVert\nabla f\rVert\leq1$,

$$
F(\lambda)-F(\lambda/2)^2
\leq C_P(X)\frac{\lambda^2}{4}F(\lambda).
$$

Hence

$$
F(\lambda)\leq
\left(1-\frac{\lambda^2C_P(X)}4\right)^{-1}
F(\lambda/2)^2.
$$

Iterating this estimate $m$ times yields

$$
F(\lambda)\leq
\prod_{k=0}^{m-1}
\left(1-\frac{\lambda^2C_P(X)}{4^{k+1}}\right)^{-2^k}
F(\lambda/2^m)^{2^m},
$$

valid under the stated bound on $\lambda$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
