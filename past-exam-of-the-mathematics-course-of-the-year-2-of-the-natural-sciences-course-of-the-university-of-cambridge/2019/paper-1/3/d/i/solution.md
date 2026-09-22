<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose $y_a=x$ and $y_b=x^3-x$, satisfying the left and right conditions respectively. Their [Wronskian](../../../../../../wronskian.md) is

$$
W(x)=x(3x^2-1)-(x^3-x)=2x^3.
$$

Part (a) therefore supplies the valid kernel

$$
\boxed{G_0(x,z)=\begin{cases}\dfrac{x(z^3-z)}{2z^3},&0\leq x\leq z,\\[4pt]\dfrac{x^3-x}{2z^2},&z\leq x\leq1,\end{cases}\qquad0<z<1.}
$$

It is continuous at the source, its first [derivative](../../../../../../derivative.md) has jump one, and it vanishes at both endpoints. However, it is not unique: $x^3-x$ is a nonzero homogeneous solution satisfying both stated endpoint conditions. Thus $G_0+(x^3-x)h(z)$ has the same defining properties for any suitable $h$.

This is a [nonunique Green kernel at a singular endpoint with two vanishing modes](../../../../../../nonunique-green-kernel-at-a-singular-endpoint-with-two-vanishing-modes.md). Choosing $y_a=x^3$ instead also gives a valid kernel, corresponding to the stronger selection $y(x)/x\to0$ at the left endpoint. The original problem states no such selection, so the family must be acknowledged.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
