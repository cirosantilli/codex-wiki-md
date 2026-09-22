<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Doob maximal inequality for a nonnegative submartingale](../../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) states that, for a nonnegative [submartingale](../../../../../../../submartingale.md) $(M_j)_{0\leq j\leq N}$ and $u>0$,

$$
u\,\mathbb P\!\left(\max_{0\leq j\leq N}M_j\geq u\right)\leq\mathbb EM_N.
$$

For completeness, partition the crossing event according to its first crossing time $j$. On that event $M_j\geq u$, while $\mathbb E[M_N\mid\mathcal F_j]\geq M_j$. Summing the corresponding expectations over $j$ proves $u\mathbb P(\max M_j\geq u)\leq\mathbb E[M_N\mathbf1_{\{\max M_j\geq u\}}]\leq\mathbb EM_N$.

If $q>p$, the exponential $r^{S_j}$, with $r=q/p>1$, is increasing as a function of $S_j$. Apply the inequality to the [martingale](../../../../../../../martingale-split.md) from part (a), with $u=r^k$:

$$
\mathbb P\!\left(\max_{0\leq j\leq N}S_j\geq k\right)
\leq r^{-k}\mathbb EZ_N=(p/q)^k.
$$

Letting $N\to\infty$ and using continuity of [probability measures](../../../../../../../probability-measure.md) on increasing events gives

$$
\boxed{\mathbb P\!\left(\sup_{n\geq0}S_n\geq k\right)\leq(p/q)^k,\qquad k\geq1.}
$$

The same event is obtained if the supremum excludes time zero, since $k\geq1$. If $p\geq q$, the right side is at least one and the bound is automatic; the nontrivial [Doob maximal inequality](../../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) argument is for $q>p$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
