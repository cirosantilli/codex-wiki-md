<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) is

$$
A^*Ax=A^*y.
$$

[Landweber iteration](../../../../../../landweber-iteration.md) is the stationary iteration

$$
\boxed{
x_{n+1}=x_n+\gamma A^*(y-Ax_n)
=(I-\gamma A^*A)x_n+\gamma A^*y}.
$$

A sufficient step-size condition is

$$
\boxed{0<\gamma<\frac2{\lVert A\rVert^2}}.
$$

If $y\in\mathcal D(A^\dagger)$ and $x_0\in(\ker A)^\perp$, then

$$
\boxed{x_n\longrightarrow A^\dagger y}.
$$

For an arbitrary initial iterate, its null-space component is unchanged and the limit is

$$
\boxed{A^\dagger y+P_{\ker A}x_0.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
