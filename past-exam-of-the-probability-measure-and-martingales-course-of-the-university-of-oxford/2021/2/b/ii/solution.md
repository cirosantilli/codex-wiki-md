<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $B_n=\{X_n>a_n\}$. If $B_n$ occurs, the running maximum at time $n$ exceeds $a_n$, so $B_n\subseteq A_n$ and $\limsup_nB_n\subseteq A$.

For the reverse inclusion, fix an outcome for which only finitely many $B_n$ occur. Choose $N$ such that $X_m\leq a_m$ for every $m\geq N$. The finite prefix has a finite maximum $K=\max_{1\leq m<N}X_m$ when $N>1$; there is no prefix to check when $N=1$. Since $a_n\to\infty$, for every sufficiently large $n$ that prefix satisfies $K\leq a_n$. For the remaining indices $N\leq m\leq n$, the nondecreasing thresholds give

$$
X_m\leq a_m\leq a_n.
$$

Thus $\max_{m\leq n}X_m\leq a_n$ for every sufficiently large $n$, so only finitely many $A_n$ occur. Taking the contrapositive proves the reverse inclusion, and hence the pointwise [event](../../../../../event.md) equality

$$
\boxed{\limsup_n\{\max_{m\leq n}X_m>a_n\}
=\limsup_n\{X_n>a_n\}.}
$$

This [exceedance equivalence for increasing thresholds](../../../../../exceedance-equivalence-for-increasing-thresholds.md) is deterministic. Its proof uses both monotonicity of $a_n$ and divergence to $+\infty$; it does not require [independence](../../../../../independent-random-variables.md) or identical [probability distributions](../../../../../probability-distribution-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
