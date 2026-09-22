<h1 id="25k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [renewal process](../../../../../../renewal-process.md) has independent identically distributed, nonnegative, [almost surely](../../../../../../almost-sure-convergence.md) finite inter-arrival times $X_i$, epochs $S_0=0,S_n=\sum_{i=1}^nX_i$, and count $N(t)=\max\{n:S_n\leq t\}$. Allowing zero inter-arrivals is harmless provided $\mathbb P(X_1>0)>0$. The hypothesis $\mathbb E X_1>0$ ensures there is $\varepsilon>0$ with $p=\mathbb P(X_1\geq\varepsilon)>0$.

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) for the indicators gives $S_n\geq\varepsilon\sum_{i=1}^n\mathbf1_{X_i\geq\varepsilon}\to\infty$, so $N(t)$ is finite for finite $t$. Conversely every fixed $S_n$ is finite, so eventually $N(t)\geq n$. On their countable common [probability](../../../../../../probability.md)-one event, this proves $\boxed{N(t)\to\infty\text{ as }t\to\infty\text{ almost surely}}$.

For fixed $t$, put $L=\lfloor t/\varepsilon\rfloor$. The hinted comparison process has epochs $S_n'=\varepsilon\sum_{i=1}^n\mathbf1_{X_i\geq\varepsilon}\leq S_n$, hence $N(t)\leq N'(t)$. Equivalently,

$$
 \mathbb P(N(t)\geq n)\leq\mathbb P(\operatorname{Bin}(n,p)\leq L).
$$

If $p<1$, for $n>L$ this is bounded by $C_{t,p} n^L(1-p)^n$, by summing the first $L+1$ [binomial distribution](../../../../../../binomial-distribution.md). Thus $\sum_ne^{\theta n}\mathbb P(N(t)=n)<\infty$ for $0<\theta<-\log(1-p)$. If $p=1$, $N(t)\leq L$ deterministically. Therefore **a strictly positive exponential moment exists** for every fixed finite $t$, with the same allowed $\theta$ for all such $t$. Almost-sure finiteness of the inter-arrivals is implicit in a proper [renewal process](../../../../../../renewal-process.md); allowing an infinite inter-arrival with positive [probability](../../../../../../probability.md) would invalidate the divergence claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
