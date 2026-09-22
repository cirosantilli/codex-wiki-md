<h1 id="9f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Finiteness of the [moment-generating function](../../../../../../moment-generating-function.md) on an open neighborhood of zero gives its differentiability there. Using the permitted interchange of differentiation and [expectation](../../../../../../expected-value.md),

$$
M_X'(t)=\mathbb E[Xe^{tX}],\qquad M_X''(t)=\mathbb E[X^2e^{tX}].
$$

Hence $M_X(0)=1$, $M_X'(0)=\mu$ and $M_X''(0)=s^2$. The second-order [Taylor expansion](../../../../../../taylor-expansion.md) with its Peano remainder gives

$$
\boxed{M_X(t)=1+\mu t+\frac12s^2t^2+o(t^2)}.
$$

Here $s^2$ is the raw second moment, not the [variance](../../../../../../variance-split.md): $\operatorname{Var}(X)=s^2-\mu^2$. This distinction matters before specializing to a centered variable.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
