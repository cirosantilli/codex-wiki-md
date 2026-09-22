<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If the [pole](../../../../../../pole.md) has order $k+1$, multiplying the [Laurent series](../../../../../../laurent-series.md) by $(z-a)^{k+1}$ gives a function $h$ with a holomorphic extension across $a$:

$$
h(z)=c_{-(k+1)}+c_{-k}(z-a)+\cdots+c_{-1}(z-a)^k+\cdots.
$$

Its coefficient of $(z-a)^k$ is exactly $c_{-1}$. The [Taylor series](../../../../../../taylor-series.md) coefficient formula gives $h^{(k)}(a)=k!c_{-1}$. Continuity of this derivative at $a$ therefore proves

$$
\boxed{\operatorname{res}(f,a)=\frac{h^{(k)}(a)}{k!}=\lim_{z\to a}\frac{h^{(k)}(z)}{k!}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
