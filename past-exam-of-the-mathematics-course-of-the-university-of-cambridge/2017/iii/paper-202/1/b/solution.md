<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $N_2=\|M_\infty\|_2$ and $N_*=\|\sup_{t\geq0}|M_t|\|_2$. The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) ensures the existence of $M_\infty$ and yields $|M_\infty|\leq\sup_t|M_t|$ [almost surely](../../../../../../almost-sure-convergence.md). Hence $N_2\leq N_*$.

For a finite horizon $T$, the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) for the [submartingale](../../../../../../submartingale.md) $|M|$ gives

$$
\mathbb E\sup_{0\leq t\leq T}|M_t|^2\leq4\mathbb E|M_T|^2.
$$

The inequality does not require $M_0=0$. Send $T$ to infinity: the left side increases to $N_*^2$ by the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), and the right side tends to $4N_2^2$ by convergence in the [Lebesgue space](../../../../../../lp-space.md) $L^2$. Thus the [equivalent terminal and maximal norms for L2-bounded continuous martingales](../../../../../../equivalent-terminal-and-maximal-norms-for-l2-bounded-continuous-martingales.md) satisfy

$$
\boxed{\|M_\infty\|_2\leq\left\|\sup_{t\geq0}|M_t|\right\|_2\leq2\|M_\infty\|_2.}
$$

Both are genuine [norms](../../../../../../norm.md) on [L2-bounded continuous martingales](../../../../../../l2-bounded-continuous-martingale.md) modulo [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md): a zero terminal norm gives $M_t=\mathbb E[M_\infty\mid\mathcal F_t]=0$, first at rational times and then at all times by continuity. This proves that the two [norms](../../../../../../norm.md) are [equivalent norms](../../../../../../equivalent-norms.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
