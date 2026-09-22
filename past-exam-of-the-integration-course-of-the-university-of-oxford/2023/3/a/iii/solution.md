<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $(f_n)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md) in the [L2 space](../../../../../l2-space-is-a-hilbert-space.md) $L^2(\mathbb R)$, choosing measurable representatives. There is a subsequence $(f_{n_k})$ with

$$
\|f_{n_{k+1}}-f_{n_k}\|_2\leq2^{-k}\qquad(k\geq1).
$$

Write $d_k=f_{n_{k+1}}-f_{n_k}$ and $S_N=\sum_{k=1}^N|d_k|$. Repeated [Minkowski inequality](../../../../../minkowski-inequality.md) gives $\|S_N\|_2\leq\sum_{k=1}^N2^{-k}\leq1$. As $S_N^2$ increases pointwise, the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives

$$
\int_{\mathbb R}\left(\sum_{k=1}^{\infty}|d_k|\right)^2dm
=\lim_{N\to\infty}\int_{\mathbb R}S_N^2dm\leq1.
$$

Hence $S=\sum_k|d_k|$ is finite [almost everywhere](../../../../../almost-everywhere.md) and represents an [L2 function](../../../../../square-integrable-function.md). Define

$$
f=f_{n_1}+\sum_{k=1}^{\infty}d_k
$$

where the series converges, and set $f=0$ on the exceptional [Lebesgue null set](../../../../../lebesgue-null-set.md). It is a [measurable function](../../../../../measurable-function.md), and $|f|\leq|f_{n_1}|+S$ [almost everywhere](../../../../../almost-everywhere.md), so [Minkowski inequality](../../../../../minkowski-inequality.md) gives $f\in L^2(\mathbb R)$.

For fixed $k$, [Fatou's lemma](../../../../../fatou-s-lemma.md) applied to squares of finite tails and then [Minkowski inequality](../../../../../minkowski-inequality.md) give

$$
\|f-f_{n_k}\|_2^2
\leq\liminf_{M\to\infty}\left\|\sum_{j=k}^{M}d_j\right\|_2^2
\leq\left(\sum_{j=k}^{\infty}2^{-j}\right)^2=2^{2-2k}.
$$

Thus the subsequence converges to $f$ in [norm](../../../../../norm.md). Given $\varepsilon>0$, choose a sufficiently late $n_k$ with $\|f-f_{n_k}\|_2<\varepsilon/2$ and with $\|f_n-f_{n_k}\|_2<\varepsilon/2$ for every sufficiently large $n$, using the original [Cauchy sequence](../../../../../cauchy-sequence.md) property. The [triangle inequality](../../../../../triangle-inequality.md) then gives $\|f_n-f\|_2<\varepsilon$. Therefore

$$
\boxed{L^2(\mathbb R)\text{ is complete, hence a Banach space}.}
$$

This proves the needed instance of [completeness of Lp spaces](../../../../../completeness-of-lp-spaces.md) without assuming the result being proved.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
