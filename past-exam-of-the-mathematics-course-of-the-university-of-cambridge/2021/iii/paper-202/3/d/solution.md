<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The supplied derivative identity and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give

$$
U_x(t,x)^2
\leq4U(t,x)\,\mathbb E[f'(x+B_{1-t})^2].
$$

Therefore

$$
\frac12\mathbb E\int_0^1\frac{U_x(t,W_t)^2}{U(t,W_t)}dt
\leq2\int_0^1\mathbb E[f'(W_t+B_{1-t})^2]dt.
$$

The sum $W_t+B_{1-t}$ is standard normal for every $t$, so the right side is $2\mathbb E f'(W_1)^2$. Part c proves the [Gaussian logarithmic Sobolev inequality](../../../../../../gaussian-logarithmic-sobolev-inequality.md)

$$
\boxed{
\mathbb E[f(W_1)^2\log f(W_1)^2]
\leq\mathbb E[f(W_1)^2]\log\mathbb E[f(W_1)^2]
+2\mathbb E[f'(W_1)^2].}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
