<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real [random variables](../../../../../../random-variable-split.md) with finite [second moments](../../../../../../second-moment.md), the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) is

$$
\boxed{|\mathbb E[Y_1Y_2]|^2\leq\mathbb E[Y_1^2],\mathbb E[Y_2^2].}
$$

The product is integrable because $2|Y_1Y_2|\leq Y_1^2+Y_2^2$. If $\mathbb E[Y_2^2]=0$, then $Y_2=0$ almost surely and the result is immediate. Otherwise the nonnegative [expectation](../../../../../../expected-value.md) of a square gives, for every real $t$,

$$
0\leq\mathbb E[(Y_1-tY_2)^2]=\mathbb E[Y_1^2]-2t\mathbb E[Y_1Y_2]+t^2\mathbb E[Y_2^2].
$$

Choose $t=\mathbb E[Y_1Y_2]/\mathbb E[Y_2^2]$. The resulting inequality is exactly the claimed [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Equality holds precisely when $Y_1$ is a constant multiple of $Y_2$ almost surely in this nondegenerate case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
