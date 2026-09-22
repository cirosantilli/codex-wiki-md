<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $e_j$ be the [coordinate vectors](../../../../../coordinate-vector.md) and define finitely supported vectors

$$
v_k=2^{-k}\sum_{j=2^k}^{2^{k+1}-1}e_j,\qquad k=0,1,\ldots.
$$

Each $v_k$ belongs to $\ell^1$, and $\|v_k\|_\infty=2^{-k}$. Hence $\sum_kv_k$ is absolutely convergent for the [supremum norm](../../../../../supremum-norm.md). Its [partial sums](../../../../../partial-sum.md) converge uniformly in $\ell^\infty$ to the sequence $v$ whose entries on the $k$th block all equal $2^{-k}$. But every block contributes one to its $\ell^1$ sum:

$$
\sum_j|v_j|=\sum_{k=0}^{\infty}2^k2^{-k}=\infty.
$$

Thus $v\notin\ell^1$. Any supremum-[norm](../../../../../norm.md) limit in $\ell^1$ would have the same coordinates as $v$, an impossibility. The [partial sums](../../../../../partial-sum.md) are Cauchy and have no limit in the space. Therefore **$(\ell^1,\|\cdot\|_\infty)$ is not Banach**, and the displayed [series](../../../../../series-mathematics.md) is the required absolutely convergent but nonconvergent [series](../../../../../series-mathematics.md) in that space.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
