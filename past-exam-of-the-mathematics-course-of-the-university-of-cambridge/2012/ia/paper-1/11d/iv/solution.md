<h1 id="11d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**No: there need not be even one orbit tending to zero.** Partition the domain into the disjoint intervals

$$
I_j=\left(\frac1{j+1},\frac1j\right]\cap(0,1),\qquad j=1,2,\ldots,
$$

and, for the unique $j$ with $x\in I_j$, define

$$
\boxed{f(x)=\frac12\left(x+\frac1{j+1}\right).}
$$

The left endpoint is strictly below $x$, so $0<f(x)<x$. Moreover $f(x)>1/(j+1)$ and $f(x)\leq x\leq1/j$, so $f(x)$ remains in the same interval. For every iterate,

$$
\boxed{f^n(x)=\frac1{j+1}+2^{-n}\left(x-\frac1{j+1}\right)\longrightarrow\frac1{j+1}>0.}
$$

Every starting point belongs to some finite-index interval, so this proves the claim for all $x\in(0,1)$. The open left endpoints matter: an orbit approaches a boundary but never crosses it. This is [discontinuous trapping of decreasing iterates](../../../../../../discontinuous-trapping-of-decreasing-iterates.md), not a violation of the [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md); each orbit does converge, just to a positive value where continuity fails.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
