<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work on $\mathbb R$ with [Lebesgue measure](../../../../../../lebesgue-measure.md). Without a uniform $L^p$ bound, use

$$
\boxed{f_n=n^{-1}1_{[0,n^q]}.}
$$

It has $\|f_n\|_q=1$ and $\|f_n\|_r=n^{q/r-1}\leq1$, with $1/r=0$ for $r=\infty$. Each function still belongs to $L^p\cap L^r$, but its $L^p$ norm is unbounded. For every fixed $\varepsilon>0$, its level set above $\varepsilon$ is eventually empty, defeating any positive uniform $M$.

Without a uniform $L^r$ bound, use instead

$$
\boxed{g_n=n\,1_{[0,n^{-q}]}.}
$$

Now $\|g_n\|_q=1$ and $\|g_n\|_p=n^{1-q/p}\leq1$, but for any fixed $\varepsilon>0$ the high-amplitude level set has measure $n^{-q}\to0$. These give the two distinct failures of the [nonvanishing level-set bound between three Lp norms](../../../../../../nonvanishing-level-set-bound-between-three-lp-norms.md) when either control is removed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
