<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\alpha,\beta>0$, integrating the [Weibull distribution](../../../../../../../weibull-distribution.md) [probability density function](../../../../../../../probability-density-function.md) gives

$$
G(x)=1-e^{-x^\alpha/\beta}\quad(x\geq0).
$$

The [inverse transform sampling](../../../../../../../inverse-transform-sampling.md) method takes $U$ uniform on $(0,1)$ and solves $G(X)=U$. Hence

$$
\boxed{X=\{-\beta\log(1-U)\}^{1/\alpha}.}
$$

Since $1-U$ is also uniform, $\{-\beta\log U\}^{1/\alpha}$ is an equivalent implementation. For any $x\geq0$, the resulting event $X\leq x$ has [probability](../../../../../../../probability.md) $G(x)$, verifying its distribution.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
