<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) in its $L^1$-bounded form says that a [martingale](../../../../../../martingale-split.md) with $\sup_n\mathbb E|M_n|<\infty$ has an integrable limit $M_\infty$ and

$$
\boxed{M_n\longrightarrow M_\infty\quad\text{almost surely},\qquad
\mathbb E|M_\infty|\leq\sup_n\mathbb E|M_n|.}
$$

The norm bound on the limit follows from [Fatou lemma](../../../../../../fatou-s-lemma.md). Boundedness in $L^1$ by itself does not imply [convergence in L1](../../../../../../convergence-in-l1.md). The [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) gives the stronger conclusion: if $(M_n)$ is [uniformly integrable](../../../../../../uniform-integrability.md), then $M_n\to M_\infty$ both [almost surely](../../../../../../almost-sure-convergence.md) and in [L1 norm](../../../../../../l1-norm.md), and $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$. Conversely, [convergence in L1](../../../../../../convergence-in-l1.md) implies [uniform integrability](../../../../../../uniform-integrability.md).

For the distinction, the [fair-coin doubling martingale](../../../../../../fair-coin-doubling-martingale.md) $M_n=2^n\mathbf1_{\{\text{first }n\text{ tosses are heads}\}}$ has [expectation](../../../../../../expected-value.md) one for every $n$ but converges [almost surely](../../../../../../almost-sure-convergence.md) to zero. Its [L1 norm](../../../../../../l1-norm.md) remains one, so its convergence is not in [L1 norm](../../../../../../l1-norm.md). These two formulations specify exactly which hypothesis is needed in part (d).

## ↑ Ancestors (11)

1. [A](../a.md)
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
