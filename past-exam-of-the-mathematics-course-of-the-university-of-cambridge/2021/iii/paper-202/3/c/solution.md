<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The backward heat equation and [Itô formula](../../../../../../ito-s-lemma.md) give

$$
dM_t=U_x(t,W_t)\,dW_t,
\qquad
d[M]_t=U_x(t,W_t)^2dt.
$$

Moreover $M_1=f(W_1)^2$ and $M_0=\mathbb E f(W_1)^2$. Substitution into part a yields

$$
\boxed{
\mathbb E[f(W_1)^2\log f(W_1)^2]
=\mathbb E[f(W_1)^2]\log\mathbb E[f(W_1)^2]
+\frac12\mathbb E\int_0^1\frac{U_x(t,W_t)^2}{U(t,W_t)}\,dt.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
