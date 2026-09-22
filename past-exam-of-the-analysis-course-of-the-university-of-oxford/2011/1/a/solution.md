<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [series](../../../../series-mathematics.md) $\sum_{n\geq1}x_n$ converges in $X$ when its [partial sums](../../../../partial-sum.md) $s_N=\sum_{n=1}^Nx_n$ converge in [norm](../../../../norm.md) to an element of $X$. It is absolutely convergent when $\sum_n\|x_n\|<\infty$.

If $X$ is complete, then

$$
\|s_M-s_N\|\leq\sum_{n=N+1}^M\|x_n\|\longrightarrow0
$$

for an absolutely convergent [series](../../../../series-mathematics.md). Its [partial sums](../../../../partial-sum.md) are Cauchy and therefore converge.

Conversely suppose every absolutely convergent [series](../../../../series-mathematics.md) converges. Given a [Cauchy sequence](../../../../cauchy-sequence.md) $(z_n)$, choose a subsequence $(z_{n_k})$ with $\|z_{n_{k+1}}-z_{n_k}\|\leq2^{-k}$. The [series](../../../../series-mathematics.md)

$$
z_{n_1}+\sum_{k=1}^{\infty}(z_{n_{k+1}}-z_{n_k})
$$

is absolutely convergent. Its [partial sums](../../../../partial-sum.md) are precisely the subsequence, which therefore converges to some $z\in X$. A [Cauchy sequence](../../../../cauchy-sequence.md) with a convergent subsequence converges to that same limit: estimate $\|z_n-z\|$ by $\|z_n-z_{n_k}\|+\|z_{n_k}-z\|$. Hence

$$
\boxed{X\text{ is Banach}\iff\text{every absolutely convergent series in }X\text{ converges}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
