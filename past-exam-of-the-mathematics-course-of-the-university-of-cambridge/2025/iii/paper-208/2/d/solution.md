<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Subtract a constant so that $f(0)=0$, and write $m=\mathbb Ef(Y)$, $V=\operatorname{Var}f(Y)$, and $A=\mathbb E f'(Y)^2$. The supplied identity applied to $f$ and $f^2$ gives

$$
m=\mathbb E[\operatorname{sgn}(Y)f'(Y)],
\qquad
\mathbb Ef(Y)^2=2\mathbb E[\operatorname{sgn}(Y)f(Y)f'(Y)].
$$

By [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), $m^2\leq A$ and

$$
V=\mathbb Ef^2-m^2
\leq2\sqrt{(V+m^2)A}-m^2.
$$

**Thus $V+m^2\leq2\sqrt{(V+m^2)A}$, so $V+m^2\leq4A$ and in particular $V\leq4A$. Therefore the standard Laplace distribution has $C_P(Y)\leq4$.**

## ↑ Ancestors (11)

1. [D](../d.md)
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
