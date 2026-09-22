<h1 id="14e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $\lambda=N$ with $N\in\mathbb Z_{\geq0}$. Then

$$
f(t)=\frac{(t-1)^N}{t^{N+1}}.
$$

Take $\gamma_1$ to be a small positively oriented circle around $t=0$. For $\gamma_2$, start at $t=1$, travel to $-\infty$, and avoid the pole at zero by a fixed upper or lower detour. The endpoint factor vanishes at $t=1$, and the exponential controls $-\infty$.

The finite contour extracts the residue at zero:

$$
y_{\gamma_1}(z)
=2\pi i\,[t^N]\left(e^{zt}(t-1)^N\right).
$$

Only powers $z^0,\ldots,z^N$ occur, and the coefficient of $z^N$ is nonzero. Thus this solution is a polynomial of degree $N$ and, up to normalization, is the [Laguerre polynomial](../../../../../../laguerre-polynomial.md) $L_N(z)$:

$$
\boxed{y_1(z)\propto L_N(z)}.
$$

This also follows from the recurrence in part (i), because $a_{N+1}=0$ and every later coefficient vanishes.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
