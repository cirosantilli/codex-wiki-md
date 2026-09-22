<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $r=(p-1)/2$, $O=1\cdot3\cdots(p-2)$ and $E=2\cdot4\cdots(p-1)$. The residues $p-2,p-4,\ldots,p-2r$ are exactly the odd factors of $O$, in reverse order. Hence

$$
O\equiv(-1)^rE\pmod p,
\qquad OE=(p-1)!\equiv-1\pmod p
$$

by [Wilson's theorem](../../../../../../wilson-s-theorem.md). It follows that the [odd-residue squared product modulo a prime](../../../../../../odd-residue-squared-product-modulo-a-prime.md) is

$$
\boxed{1^2\cdot3^2\cdots(p-2)^2=O^2\equiv(-1)^{r+1}=(-1)^{(p+1)/2}\pmod p.}
$$

Thus it is $-1$ for $p\equiv1\pmod4$ and $1$ for $p\equiv3\pmod4$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
