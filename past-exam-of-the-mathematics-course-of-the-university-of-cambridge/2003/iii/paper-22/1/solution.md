<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\vartheta(x)=\sum_{p\le x}\log p$ for the [Chebyshev theta function](../../../../../chebyshev-theta-function.md) and $\psi(x)=\sum_{p^j\le x}\log p$ for the [Second Chebyshev function](../../../../../second-chebyshev-function.md). Throughout, $p$ denotes a [prime](../../../../../prime-number.md) and all [logarithms](../../../../../logarithm.md) are natural. Each [prime](../../../../../prime-number.md) $n<p\le2n$ divides the central [binomial coefficient](../../../../../binomial-coefficient.md), so

$$
\vartheta(2n)-\vartheta(n)\le\log\binom{2n}{n}\le2n\log2.
$$

Apply this at $n=1,2,4,\ldots,2^{r-1}$ and telescope: $\vartheta(2^r)\le(2^{r+1}-2)\log2$. Bounding a general $x$ by the next power of two proves $\vartheta(x)=O(x)$. Splitting the [prime-counting function](../../../../../prime-counting-function.md) at $\sqrt x$ now gives

$$
\pi(x)\le\sqrt x+\frac2{\log x}\vartheta(x),
\qquad\boxed{\pi(x)=O(x/\log x).}
$$

This is the required [Chebyshev estimate from central binomial coefficients](../../../../../chebyshev-estimate-from-central-binomial-coefficients.md), with no use of a [prime](../../../../../prime-number.md) asymptotic.

The higher [prime powers](../../../../../prime-power.md) also satisfy

$$
\psi(x)=\sum_{1\le j\le\log x/\log2}\vartheta(x^{1/j})
=\vartheta(x)+O(\sqrt x\log x)=O(x).
$$

For an [integer](../../../../../integer.md) $N$, the [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) of a [factorial](../../../../../factorial.md) gives

$$
\log N!=\sum_{p^j\le N}\left\lfloor\frac N{p^j}\right\rfloor\log p
=N\sum_{p^j\le N}\frac{\log p}{p^j}+O(\psi(N)).
$$

The [Stirling formula](../../../../../stirling-formula.md), or integral comparison for $\log t$, says $\log N!=N\log N-N+O(\log N)$. After division by $N$ we obtain $\sum_{p^j\le N}(\log p)/p^j=\log N+O(1)$. Moreover

$$
0\le\sum_{p}\sum_{j\ge2}\frac{\log p}{p^j}
=\sum_p\frac{\log p}{p(p-1)}
\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Subtract this bounded contribution and replace $N$ by $\lfloor x\rfloor$. The [factorial proof of Mertens first theorem](../../../../../factorial-proof-of-mertens-first-theorem.md) therefore yields

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

For fixed $\lambda>1$, apply [partial summation](../../../../../abel-s-summation-formula.md) to $A(t)$ and $f(t)=(\log t)^{\lambda-1}$:

$$
\sum_{p\le x}\frac{(\log p)^\lambda}{p}
=A(x)(\log x)^{\lambda-1}
-(\lambda-1)\int_2^x A(t)\frac{(\log t)^{\lambda-2}}t\,dt.
$$

The main contribution is

$$
(\log x)^\lambda-\frac{\lambda-1}{\lambda}(\log x)^\lambda+O(1)
=\frac1\lambda(\log x)^\lambda+O(1).
$$

The bounded error in $A(t)$ contributes $O((\log x)^{\lambda-1})$ at the endpoint and in the integral, since $\int_2^x(\log t)^{\lambda-2}dt/t=O_\lambda((\log x)^{\lambda-1})$. Thus the [positive logarithmic moments of reciprocal primes](../../../../../positive-logarithmic-moments-of-reciprocal-primes.md) satisfy

$$
\boxed{\sum_{p\le x}\frac{(\log p)^\lambda}{p}
=\frac1\lambda(\log x)^\lambda+O_\lambda((\log x)^{\lambda-1}).}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
