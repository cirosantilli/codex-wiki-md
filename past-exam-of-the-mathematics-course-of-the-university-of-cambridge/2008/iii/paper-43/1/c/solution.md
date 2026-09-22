<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $a+b/n=a(n+m-1)/n$, so iteration gives

$$
p_n=p_0a^n\frac{m(m+1)\cdots(m+n-1)}{n!}
=p_0\binom{m+n-1}{n}a^n.
$$

The negative-binomial series $\sum_{n\ge0}\binom{m+n-1}{n}a^n=(1-a)^{-m}$, valid for $0<a<1$, normalizes this to

$$
\boxed{p_n=\binom{m+n-1}{n}(1-a)^m a^n,\qquad n=0,1,\ldots.}
$$

This is the [negative binomial distribution](../../../../../../negative-binomial-distribution.md) counting failures before the $m$th success, with success probability $1-a$. The convention is specified because a negative-binomial variable is sometimes defined to count trials instead. Its count [expected value](../../../../../../expected-value.md) is $ma/(1-a)$, and the [Panjer recursion](../../../../../../panjer-recursion.md) begins at $g_0=(1-a)^m$. For $m=1$ this reduces to the failure-count [geometric distribution](../../../../../../geometric-distribution.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
