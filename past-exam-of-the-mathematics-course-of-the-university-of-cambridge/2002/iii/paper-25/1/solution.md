<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\theta(x)=\sum_{p\le x}\log p$ for the [Chebyshev theta function](../../../../../chebyshev-theta-function.md) and $\psi(x)=\sum_{n\le x}\Lambda(n)$ for the [Second Chebyshev function](../../../../../second-chebyshev-function.md), where $\Lambda$ is the [Von Mangoldt function](../../../../../von-mangoldt-function.md). We first establish the [Chebyshev estimate](../../../../../chebyshev-estimate.md). Every [prime](../../../../../prime-number.md) $n<p\le2n$ divides the [central binomial coefficient](../../../../../central-binomial-coefficient.md) $\binom{2n}{n}$, so

$$
\theta(2n)-\theta(n)\le\log\binom{2n}{n}\le2n\log2.
$$

Apply this at successive powers of two and use [monotonicity](../../../../../monotonic-function.md) to obtain $\theta(x)=O(x)$. Since

$$
\psi(x)=\sum_{r\ge1}\theta(x^{1/r}),
$$

the terms $r\ge2$ contribute $O(\sqrt x\log x)$ and therefore $\psi(x)=O(x)$. This [Chebyshev estimate from central binomial coefficients](../../../../../chebyshev-estimate-from-central-binomial-coefficients.md) is all the information about the distribution of [primes](../../../../../prime-number.md) needed here.

The [Von Mangoldt divisor identity](../../../../../von-mangoldt-divisor-identity.md) $\log n=\sum_{d\mid n}\Lambda(d)$ gives the [factorial proof of Mertens first theorem](../../../../../factorial-proof-of-mertens-first-theorem.md). With $N=\lfloor x\rfloor$, interchange the finite sums to obtain

$$
\log N!=\sum_{d\le x}\Lambda(d)\left\lfloor\frac xd\right\rfloor
=x\sum_{d\le x}\frac{\Lambda(d)}d+O(\psi(x)).
$$

Comparison of $\sum_{n\le N}\log n$ with $\int_1^N\log t\,dt$ gives $\log N!=N\log N-N+O(\log N)$. Dividing the preceding identity by $x$, using $N=x+O(1)$ and the [Chebyshev estimate](../../../../../chebyshev-estimate.md), gives

$$
\sum_{d\le x}\frac{\Lambda(d)}d=\log x+O(1).
$$

The contribution of higher [prime powers](../../../../../prime-power.md) is bounded independently of $x$, because

$$
\sum_p\sum_{r\ge2}\frac{\log p}{p^r}
=\sum_p\frac{\log p}{p(p-1)}
\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Thus the [Mertens first theorem](../../../../../mertens-first-theorem.md) is

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

For the [square-root logarithmic sum over primes](../../../../../square-root-logarithmic-sum-over-primes.md), apply [partial summation](../../../../../abel-s-summation-formula.md) to $A(t)$ with weight $(\log t)^{-1/2}$. The lower endpoint is understood as $A(2^-)=0$, so

$$
\sum_{p\le x}\frac{\sqrt{\log p}}p
=\frac{A(x)}{\sqrt{\log x}}
+\frac12\int_2^x\frac{A(t)}{t(\log t)^{3/2}}\,dt.
$$

The main terms are $\sqrt{\log x}$ and $\sqrt{\log x}-\sqrt{\log2}$. The bounded error in $A(t)$ produces a bounded integral, since $\int_2^\infty dt/(t(\log t)^{3/2})<\infty$. Therefore

$$
\boxed{\sum_{p\le x}\frac{\sqrt{\log p}}p=2\sqrt{\log x}+O(1).}
$$

Neither argument uses the [Prime number theorem](../../../../../prime-number-theorem.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
