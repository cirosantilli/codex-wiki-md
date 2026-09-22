<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\vartheta(x)=\sum_{p\le x}\log p$ and $\psi(x)=\sum_{n\le x}\Lambda(n)$ for the two [Chebyshev functions](../../../../../chebyshev-function.md), and $\pi(x)$ for the [prime-counting function](../../../../../prime-counting-function.md). If $m<p\le2m$, the [prime](../../../../../prime-number.md) $p$ divides the central [binomial coefficient](../../../../../binomial-coefficient.md) $\binom{2m}{m}$. Consequently

$$
\vartheta(2m)-\vartheta(m)\le\log\binom{2m}{m}\le2m\log2.
$$

Sum this inequality over dyadic integers $m=1,2,4,\ldots,2^{k-1}$. It gives $\vartheta(2^k)\le2^{k+1}\log2$. [Monotonicity](../../../../../monotonic-function.md), with $2^{k-1}<x\le2^k$, gives $\vartheta(x)=O(x)$ for real $x\ge2$. This is the [Chebyshev estimate from central binomial coefficients](../../../../../chebyshev-estimate-from-central-binomial-coefficients.md); no information about the distribution of [primes](../../../../../prime-number.md) beyond [unique factorization](../../../../../unique-factorization-in-an-integral-domain.md) has been used.

Split the [primes](../../../../../prime-number.md) at $\sqrt x$. For $p>\sqrt x$, $\log p>\tfrac12\log x$, so

$$
\pi(x)\le\sqrt x+\frac{2\vartheta(x)}{\log x}.
$$

Since $\sqrt x=O(x/\log x)$,

$$
\boxed{\pi(x)=O\left(\frac{x}{\log x}\right).}
$$

We also need $\psi(x)=O(x)$. The contributions of higher [prime powers](../../../../../prime-power.md) satisfy

$$
\psi(x)=\sum_{k\ge1}\vartheta(x^{1/k})=\vartheta(x)+O(\sqrt x\log x)=O(x),
$$

because only $k\le\log x/\log2$ contribute, and $\vartheta(x^{1/k})\ll\sqrt x$ for $k\ge2$.

The [Von Mangoldt divisor identity](../../../../../von-mangoldt-divisor-identity.md) is $\log n=\sum_{d\mid n}\Lambda(d)$, which follows by factoring $n$ into [prime powers](../../../../../prime-power.md). Summing it for $n\le M$, with $M$ a positive integer, gives

$$
\log(M!)=\sum_{d\le M}\Lambda(d)\left\lfloor\frac Md\right\rfloor
=M\sum_{d\le M}\frac{\Lambda(d)}d+O(\psi(M)).
$$

The bound already proved makes the last error $O(M)$. Integral comparison for $\sum_{n\le M}\log n$, or the [Stirling formula](../../../../../stirling-formula.md), gives $\log(M!)=M\log M-M+O(\log M)$. Therefore

$$
\sum_{d\le M}\frac{\Lambda(d)}d=\log M+O(1).
$$

The contribution from higher [prime powers](../../../../../prime-power.md) is uniformly bounded:

$$
\sum_p\sum_{k\ge2}\frac{\log p}{p^k}=\sum_p\frac{\log p}{p(p-1)}\le\sum_{n\ge2}\frac{\log n}{n(n-1)}<\infty.
$$

Subtract it, and replace $M$ by $\lfloor x\rfloor$, to obtain the [Mertens first theorem](../../../../../mertens-first-theorem.md)

$$
\boxed{A(x):=\sum_{p\le x}\frac{\log p}{p}=\log x+O(1).}
$$

Now fix $\delta>0$. Apply [partial summation](../../../../../abel-s-summation-formula.md) to $A(t)$ and $f(t)=(\log t)^{-1-\delta}$. With the lower endpoint interpreted as $2^-$, so that the [prime](../../../../../prime-number.md) $2$ is included, this gives

$$
\sum_{p\le x}\frac1{p(\log p)^\delta}
=\frac{A(x)}{(\log x)^{1+\delta}}+(1+\delta)\int_2^x\frac{A(t)}{t(\log t)^{2+\delta}}\,dt.
$$

The boundary term tends to zero, and the integral converges, since $A(t)\ll\log t$ and $\int_2^\infty dt/(t(\log t)^{1+\delta})<\infty$. Thus **the series converges for every positive $\delta$**. Keeping the main term of $A(t)$ also gives the useful [logarithmically weighted reciprocal-prime tail](../../../../../logarithmically-weighted-reciprocal-prime-tail.md)

$$
\boxed{\sum_{p>x}\frac1{p(\log p)^\delta}=\frac1{\delta(\log x)^\delta}+O_\delta\left(\frac1{(\log x)^{1+\delta}}\right).}
$$

Indeed, subtract the finite partial sum from the limiting integral: the boundary contributes $-(\log x)^{-\delta}$ and the main integral contributes $(1+\delta)(\log x)^{-\delta}/\delta$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
