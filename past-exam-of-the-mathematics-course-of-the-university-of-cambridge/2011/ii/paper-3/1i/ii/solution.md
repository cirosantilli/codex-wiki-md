<h1 id="1i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $m=(p-1)/2$ and let $O=1\cdot3\cdot5\cdots(p-2)$. The even residues $2,4,\ldots,p-1$ are precisely the negatives, in reverse order, of the odd residues $1,3,\ldots,p-2$. Hence their product is $(-1)^mO$ in the [finite field](../../../../../../finite-field.md) $\mathbb F_p$. Applying [Wilson theorem](../../../../../../wilson-s-theorem.md) gives

$$
-1\equiv(p-1)!=O\,((-1)^mO)=(-1)^mO^2\pmod p.
$$

The initial factor $1^2$ can be omitted, so

$$
\boxed{3^2\cdot5^2\cdots(p-2)^2\equiv(-1)^{m+1}=(-1)^{(p+1)/2}\pmod p.}
$$

For $p=3$ the product is empty and equals $1$, consistently with the formula.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1I](../../1i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
