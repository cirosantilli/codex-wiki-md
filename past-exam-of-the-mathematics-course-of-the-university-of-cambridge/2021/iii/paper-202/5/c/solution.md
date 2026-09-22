<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
h(y)=g'(g^{-1}(y)).
$$

Differentiating and using the scale equation gives

$$
h'(y)=\frac{g''(x)}{g'(x)}=-2b(x),
\qquad x=g^{-1}(y).
$$

Since $b$ is bounded, $h$ has global [Lipschitz continuity](../../../../../../lipschitz-continuity.md). Thus

$$
dY_t=h(Y_t)dW_t
$$

has a pathwise unique strong solution by the standard Lipschitz existence-and-uniqueness theorem for a [stochastic differential equation](../../../../../../stochastic-differential-equation.md). Applying the deterministic inverse $g^{-1}$ gives a strong solution $X$, and uniqueness of $Y$ gives pathwise uniqueness of $X$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
