<h1 id="5j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [weighted least squares](../../../../../../weighted-least-squares.md) objective is

$$
Q(b)=(Y-Xb)^TW(Y-Xb).
$$

Its gradient is

$$
\nabla_bQ(b)=-2X^TW(Y-Xb).
$$

Since $W$ is positive diagonal and $X$ has full column rank, $X^TWX$ is positive definite. The unique stationary point is therefore the unique minimizer:

$$
\boxed{\operatorname*{arg\,min}_{b\in\mathbb R^p}Q(b)
=(X^TWX)^{-1}X^TWY}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5J](../../5j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
