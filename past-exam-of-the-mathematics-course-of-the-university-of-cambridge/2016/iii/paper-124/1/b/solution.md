<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Möbius function](../../../../../../mobius-function.md) has $\mu(1)=1$, $\mu(n)=0$ when $n$ is divisible by a [prime](../../../../../../prime-number.md) square, and $\mu(n)=(-1)^r$ when $n$ is a product of $r$ distinct [primes](../../../../../../prime-number.md). The [Riemann zeta function](../../../../../../riemann-zeta-function.md) is initially the [Dirichlet series](../../../../../../dirichlet-series.md) $\zeta(s)=\sum_{n\ge1}n^{-s}$ for $\sigma=\Re s>1$. Both this [Dirichlet series](../../../../../../dirichlet-series.md) and $\sum\mu(n)n^{-s}$ have [absolute convergence](../../../../../../absolute-convergence.md), because $|\mu(n)|\le1$ and $\sum n^{-\sigma}<\infty$.

For a finite set of [primes](../../../../../../prime-number.md) $p\le y$, multiplication of absolutely convergent [geometric series](../../../../../../geometric-series.md) and [unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) give

$$
\prod_{p\le y}(1-p^{-s})^{-1}=\sum_{\substack{n\ge1\\p\mid n\Rightarrow p\le y}}n^{-s}.
$$

Every omitted integer has a [prime factor](../../../../../../prime-factor.md) exceeding $y$, so it exceeds $y$. The difference from $\zeta(s)$ has absolute value at most $\sum_{n>y}n^{-\sigma}\to0$. This proves the [Euler product](../../../../../../euler-product.md), with the product interpreted as the limit of its finite products:

$$
\boxed{\zeta(s)=\prod_p(1-p^{-s})^{-1}\qquad(\Re s>1).}
$$

For the reciprocal identity, [absolute convergence](../../../../../../absolute-convergence.md) justifies multiplying and regrouping the two [Dirichlet series](../../../../../../dirichlet-series.md) by their product index. Their [Dirichlet convolution](../../../../../../dirichlet-convolution.md) coefficient at $m$ is

$$
\sum_{d\mid m}\mu(d)=\begin{cases}1,&m=1,\\(1-1)^r=0,&m>1\text{ with }r\text{ distinct prime factors}.
\end{cases}
$$

The coefficient calculation uses only the [squarefree integers](../../../../../../squarefree-integer.md) dividing $m$. Consequently **the reciprocal identity is an identity of absolutely convergent series**:

$$
\boxed{\zeta(s)\sum_{n=1}^{\infty}\frac{\mu(n)}{n^s}=1\qquad(\Re s>1).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
