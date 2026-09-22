<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $a>1$. Continuity ensures $M_{T_a}=a$ when $T_a<\infty$, even though the defining inequality is strict. Before that infimum the process is at most $a$. Thus $M^{T_a}$ is a bounded nonnegative [local martingale](../../../../../../local-martingale.md) and hence a true [martingale](../../../../../../martingale-split.md), with expectation one. For deterministic $t$,

$$
1=\mathbb E M_{t\wedge T_a}=a\,\mathbb P(T_a\leq t)+\mathbb E[M_t\mathbf1_{\{T_a>t\}}].
$$

The stopped process converges to $a$ on $\{T_a<\infty\}$ and to zero on its complement. It is bounded by $a$, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives $1=a\mathbb P(T_a<\infty)$. The crossing event is exactly $\{\sup_{t\geq0}M_t>a\}$. Therefore

$$
\boxed{\mathbb P(T_a<\infty)=\mathbb P\left(\sup_{t\geq0}M_t>a\right)=a^{-1}.}
$$

This is the [maximal identity for a continuous nonnegative local martingale tending to zero](../../../../../../maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero.md). It also shows there is no atom at a level greater than one. The tail tends to one as $a\downarrow1$, so the overall maximum has no atom at its lower endpoint either.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
