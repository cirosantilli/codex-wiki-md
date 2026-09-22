<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the approximants just chosen. The [weak type (1,1)](../../../../../../weak-type-1-1.md) bound gives

$$
\lambda\{S(g-f_n)>2^{-n}\}
\leq C\,2^n\|g-f_n\|_1\leq C2^{-n}.
$$

The [measures](../../../../../../measure.md) of these exceptional sets are summable. Indeed, the [measure](../../../../../../measure.md) of their union for $n\geq m$ is at most $C\sum_{n\geq m}2^{-n}\to0$. Hence their limsup is null; this is the [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md). Outside it, $S(g-f_n)\to0$.

Remove also the countable [null set](../../../../../../null-set.md) from part (b). At each remaining point and for every $n$, the estimate in part (a) yields

$$
\limsup_{r\downarrow0}|T_rg-T_0g|
\leq2S(g-f_n).
$$

Letting $n\to\infty$ makes the right side zero. Therefore

$$
\boxed{T_rg\longrightarrow T_0g\quad\text{almost everywhere as }r\downarrow0.}
$$

This proves [almost-everywhere convergence from weak-type domination](../../../../../../almost-everywhere-convergence-from-weak-type-domination.md). The argument uses countably many measurable exceptional sets and does not assume that a supremum over all real parameters is measurable.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
