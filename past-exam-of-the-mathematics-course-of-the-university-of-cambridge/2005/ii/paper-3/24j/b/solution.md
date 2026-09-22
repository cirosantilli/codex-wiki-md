<h1 id="24j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Completeness means that every norm-Cauchy sequence has a limit belonging to the same [Lp space](../../../../../../lp-space.md), with $\|f_n-f\|_p\to0$. To prove it, choose a subsequence $f_{n_j}$ with $\|f_{n_{j+1}}-f_{n_j}\|_p\leq2^{-j}$. The functions

$$
H_N=|f_{n_1}|+\sum_{j=1}^N|f_{n_{j+1}}-f_{n_j}|
$$

have $p$-norm bounded by $\|f_{n_1}\|_p+1$, by [Minkowski inequality](../../../../../../minkowski-inequality.md). They increase to $H$, and [Fatou's lemma](../../../../../../fatou-s-lemma.md) gives $\int H^p\leq(\|f_{n_1}\|_p+1)^p$. Thus $H$ is finite almost everywhere, so the subsequence telescopes absolutely there to a measurable limit $f$ with $|f|\leq H$ and $f\in L^p$.

The same argument on the tails gives $\|f-f_{n_j}\|_p\leq\sum_{k\geq j}2^{-k}\to0$. Given $\epsilon$, choose such a subsequence term beyond the Cauchy threshold and use $\|f_n-f\|_p\leq\|f_n-f_{n_j}\|_p+\|f_{n_j}-f\|_p$. This proves convergence of the full sequence and **completeness for every $1\leq p<\infty$**, on an arbitrary measure space.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24J](../../24j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
