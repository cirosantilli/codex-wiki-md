<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $R=\lVert X_{(L)}-x\rVert_\infty$ and $\delta_0=(2L/(nM))^{1/d}$. If $\delta_0\geq1$, the claim follows from $R\leq1$. Otherwise, for $\delta\geq\delta_0$, part (c) gives

$$
\mathbb P(R>\delta)
\leq\frac4{nM\delta^d}leq\frac2L.
$$

The [tail-sum formula](../../../../../../tail-sum-formula.md) then yields

$$
\boxed{\mathbb ER
\leq\delta_0+\int_{\delta_0}^1\mathbb P(R>\delta)\,d\delta
\leq\left(\frac{2L}{nM}\right)^{1/d}+\frac2L.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
