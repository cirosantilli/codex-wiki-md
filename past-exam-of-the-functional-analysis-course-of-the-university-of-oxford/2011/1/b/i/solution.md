<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Q_N$ be truncation to the first $N$ coordinates in $\ell^1$. For $x\in\ell^1$, boundedness of $T$ and absolute convergence give

$$
(T-TQ_N)x=\sum_{n>N}x_nTe_n,\qquad
\|(T-TQ_N)x\|_1\leq\sup_{n>N}\|Te_n\|_1\,\|x\|_1.
$$

Applying the difference to each $e_n$ with $n>N$ gives the reverse bound on the [operator norm](../../../../../operator-norm.md). Hence

$$
\boxed{\|T-TQ_N\|=\sup_{n>N}\|Te_n\|_1.}
$$

The stated condition makes this tend to zero. Each $TQ_N$ has finite rank, so part (a)(ii) proves [compactness](../../../../../compact-space.md). Thus the condition is **sufficient** on $\ell^1$.

For failure of necessity, set $Tx=(\sum_{n\geq1}x_n)e_1$. The sum defines a bounded [linear functional](../../../../../linear-functional.md) on $\ell^1$, so $T$ is a bounded rank-one operator and therefore [compact](../../../../../compact-space.md). But $Te_n=e_1$ for every $n$, so $\|Te_n\|_1=1$. Thus **[compactness](../../../../../compact-space.md) need not make the basis images tend to zero on $\ell^1$**.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the functional analysis course of the University of Oxford](../../../../split.md)
6. [Functional analysis course of the University of Oxford](../../../../../functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
