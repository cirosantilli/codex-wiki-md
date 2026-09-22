<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(Z_k,\mathcal F_k)_{0\leq k\leq n}$ be an [integrable](../../../../../../integrability.md) real [submartingale](../../../../../../submartingale.md), and put $Z_n^*=\max_{0\leq k\leq n}Z_k$. The refined [Doob maximal inequality](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) is

$$
\boxed{\lambda\,\mathbb P(Z_n^*\geq\lambda)
\leq\mathbb E[Z_n\mathbf1_{\{Z_n^*\geq\lambda\}}],\qquad\lambda>0.}
$$

In particular, for a nonnegative [submartingale](../../../../../../submartingale.md) the right-hand side is at most $\mathbb EZ_n$, giving the usual weak maximal bound.

For the proof, partition $A=\{Z_n^*\geq\lambda\}$ by its first crossing time: $A_k=\{Z_j<\lambda\ (j<k),\ Z_k\geq\lambda\}\in\mathcal F_k$. The [submartingale](../../../../../../submartingale.md) property gives $\mathbb E[Z_n\mid\mathcal F_k]\geq Z_k$, so

$$
\mathbb E[Z_n\mathbf1_{A_k}]
=\mathbb E[\mathbf1_{A_k}\mathbb E(Z_n\mid\mathcal F_k)]
\geq\mathbb E[Z_k\mathbf1_{A_k}]
\geq\lambda\mathbb P(A_k).
$$

Summing over the disjoint crossing events proves the refined inequality, including a possible crossing at time zero. No [independence](../../../../../../independent-random-variables.md) assumption is needed.

The strong form is the [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md). For $p>1$ and a nonnegative [submartingale](../../../../../../submartingale.md) with $Z_n\in L^p$,

$$
\boxed{\|Z_n^*\|_p\leq\frac p{p-1}\|Z_n\|_p.}
$$

Indeed, integrate the refined inequality against $p\lambda^{p-2}$ up to $K$. The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) and the [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\mathbb E[(Z_n^*\wedge K)^p]
\leq\frac p{p-1}\mathbb E[Z_n(Z_n^*\wedge K)^{p-1}].
$$

Apply the [Holder inequality](../../../../../../holder-inequality.md), divide by $\|Z_n^*\wedge K\|_p^{p-1}$ when it is nonzero, and let $K\to\infty$ by the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). For a [martingale](../../../../../../martingale-split.md) $M$, the process $|M_k|$ is a [submartingale](../../../../../../submartingale.md) by the [conditional Jensen inequality](../../../../../../conditional-jensen-inequality.md), giving the corresponding bound for $\max|M_k|$. On a bounded continuous-time interval the nonnegative, right-continuous version follows by applying these inequalities on refining finite time grids and taking limits.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
