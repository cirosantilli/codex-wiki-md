<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $a_0\in A$. Right multiplication by $a_0$ injects $A^2$ into $A^3$, so

$$
|A^2|\leq|A^3|\leq K|A|.
$$

Apply part i with anchor $A^{-1}$, $B=A$, and $C=A^2$. Since inversion preserves cardinality,

$$
|A|\,|AA^{-1}A^{-1}|
\leq |A^{-1}A^{-1}|\,|A^{-1}A^{-1}A^{-1}|
=|A^2|\,|A^3|
\leq K^2|A|^2.
$$

Therefore $|AA^{-1}A^{-1}|\leq K^2|A|$.

Apply part i again, now with anchor $A$, $B=A^2$, and $C=A^{-1}A^{-1}$. This gives

$$
|A|\,|A^4|
\leq|AA^{-1}A^{-1}|\,|A^3|
\leq K^3|A|^2.
$$

**Thus $|A^4|\leq K^3|A|$. Since $K\geq1$, this proves the requested [fourfold product bound from small tripling](../../../../../../fourfold-product-bound-from-small-tripling.md) $|A^4|\leq K^4|A|$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
