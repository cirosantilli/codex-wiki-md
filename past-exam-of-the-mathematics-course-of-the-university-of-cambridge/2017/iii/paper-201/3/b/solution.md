<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $1<p<\infty$, the [Lp martingale convergence theorem](../../../../../../lp-martingale-convergence-theorem.md) states that a [martingale](../../../../../../martingale-split.md) with $\sup_n\mathbb E|M_n|^p<\infty$ has a limit $M_\infty\in L^p$ such that

$$
\boxed{M_n\to M_\infty\text{ almost surely},\qquad
\|M_n-M_\infty\|_p\to0.}
$$

Moreover, $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$ and $\mathbb E|M_\infty|^p\leq\sup_n\mathbb E|M_n|^p$. To see why $p>1$ matters, the [Doob Lp maximal inequality](../../../../../../doob-lp-maximal-inequality.md) gives an integrable dominating variable $(\sup_n|M_n|)^p$. The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) first supplies the almost-sure limit, then the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) supplies convergence in the [Lp norm](../../../../../../lp-norm.md). This maximal estimate is unavailable at $p=1$ in the required form.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
