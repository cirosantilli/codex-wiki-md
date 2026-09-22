<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative [submartingale](../../../../../../submartingale.md) $(M_k)_{0\leq k\leq n}$ and $M_n^*=\max_{0\leq k\leq n}M_k$, the weak form of the [Doob maximal inequality](../../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) is

$$
\boxed{u\,\mathbb P(M_n^*\geq u)\leq\mathbb E[M_n\mathbf1_{\{M_n^*\geq u\}}]\leq\mathbb E M_n\qquad(u>0).}
$$

To prove it, let $A_k$ be the event that $k$ is the first index with $M_k\geq u$. These events are disjoint, $A_k\in\mathcal F_k$, and their union is $A=\{M_n^*\geq u\}$. The [submartingale](../../../../../../submartingale.md) property gives $\mathbb E[M_n\mid\mathcal F_k]\geq M_k$. Multiplying by $\mathbf1_{A_k}$, taking expectations and summing yields $\mathbb E[M_n\mathbf1_A]\geq\sum_k\mathbb E[M_k\mathbf1_{A_k}]\geq u\mathbb P(A)$. Nonnegativity gives the second inequality.

The associated [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md), for $p>1$ and $M_n\in L^p$, is

$$
\boxed{\|M_n^*\|_p\leq\frac p{p-1}\|M_n\|_p.}
$$

Indeed $M_k\leq\mathbb E[M_n\mid\mathcal F_k]$, so conditional [Jensen inequality](../../../../../../jensen-s-inequality.md) first ensures finite $p$th moments for all $M_k$ and hence for the finite maximum. Integrating the weak inequality against $pu^{p-2}\,du$ and using the [Tonelli theorem](../../../../../../tonelli-theorem.md) gives

$$
\mathbb E(M_n^*)^p\leq\frac p{p-1}\mathbb E[M_n(M_n^*)^{p-1}]
\leq\frac p{p-1}\|M_n\|_p\|M_n^*\|_p^{p-1}.
$$

The last step is [Holder inequality](../../../../../../holder-inequality.md). Dividing, unless the maximum is zero, proves the stated norm bound. For an arbitrary [martingale](../../../../../../martingale-split.md), its absolute value is a nonnegative [submartingale](../../../../../../submartingale.md) by conditional [Jensen inequality](../../../../../../jensen-s-inequality.md), so both corresponding absolute-maximum bounds follow.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
