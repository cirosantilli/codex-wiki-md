<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the natural [filtration](../../../../../../filtration-probability-theory.md) $\mathcal F_n=\sigma(Z_1,\ldots,Z_n)$, the sums form a [martingale](../../../../../../martingale-split.md). Put $v_n=\sum_{k\leq n}a_k^2$. [Independence](../../../../../../independent-random-variables.md) and the [characteristic function](../../../../../../characteristic-function.md) of a [standard normal random variable](../../../../../../standard-normal-random-variable.md) give

$$
\mathbb E e^{iuM_n}=e^{-u^2v_n/2}.
$$

If $M_n\to M_\infty$ [almost surely](../../../../../../almost-sure-convergence.md) with a finite limit, [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives convergence of these [characteristic functions](../../../../../../characteristic-function.md) to $\mathbb E e^{iuM_\infty}$. If $v_n\to\infty$, that limit would be $1$ at zero and $0$ at every nonzero $u$. A [characteristic function](../../../../../../characteristic-function.md) is continuous at zero: apply [dominated convergence](../../../../../../dominated-convergence-theorem.md) to $e^{iuM_\infty}$ as $u\to0$. This contradiction proves

$$
\boxed{\sum_{k=1}^\infty a_k^2<\infty.}
$$

This is also sufficient by the [L2-bounded martingale convergence theorem](../../../../../../l2-bounded-martingale-convergence-theorem.md), since $\mathbb EM_n^2=v_n$. Thus the [almost sure convergence criterion for an independent Gaussian series](../../../../../../almost-sure-convergence-criterion-for-an-independent-gaussian-series.md) is an equivalence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
