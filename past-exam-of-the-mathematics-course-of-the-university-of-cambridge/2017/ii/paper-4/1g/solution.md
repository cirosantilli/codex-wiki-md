<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Expand the finite [Euler product](../../../../../euler-product.md) into [geometric series](../../../../../geometric-series.md). By [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md), it is the sum of $1/n$ over positive [integers](../../../../../integer.md) whose [prime factors](../../../../../prime-factor.md) do not exceed $x$, and hence contains every term up to $m=\lfloor x\rfloor$. The [harmonic sum](../../../../../harmonic-sum.md) satisfies

$$
\prod_{p\leq x}(1-p^{-1})^{-1}\geq\sum_{n=1}^m\frac1n>\int_1^{m+1}\frac{dt}{t}=\log(m+1)>\log x.
$$

The last inequality uses $m+1>x$, including when $x$ is an [integer](../../../../../integer.md). For each [prime number](../../../../../prime-number.md) $p$,

$$
0<-\log(1-p^{-1})-p^{-1}=\sum_{j=2}^\infty\frac1{jp^j}<\frac1{2p(p-1)}.
$$

The [telescoping series](../../../../../telescoping-series.md) over all [integers](../../../../../integer.md) $n\geq2$ bounds the sum of these remainders by $\frac12\sum_{n\geq2}[n(n-1)]^{-1}=1/2$. Taking [logarithms](../../../../../logarithm.md) of the product bound therefore gives

$$
\boxed{\sum_{p\leq x}\frac1p>\log\log x-\frac12,\qquad c=-\frac12.}
$$

This explicit constant suffices; no asymptotic theorem about the distribution of [prime numbers](../../../../../prime-number.md) is needed.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
