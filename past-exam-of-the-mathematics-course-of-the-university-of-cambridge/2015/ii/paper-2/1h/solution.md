<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

The [Euler totient function](../../../../../euler-totient-function.md) counts integers $1\leq a\leq n$ with $\gcd(a,n)=1$. The [Möbius function](../../../../../mobius-function.md) has $\mu(1)=1$, is zero when a prime square divides $n$, and equals $(-1)^r$ when $n$ is a product of $r$ distinct primes. Consequently

$$
\sum_{d\mid n}\mu(d)=\begin{cases}1&n=1,\\0&n>1,\end{cases}
$$

because for $n>1$ the sum over squarefree divisors is $(1-1)^r$.

The [Möbius inversion formula](../../../../../mobius-inversion-formula.md) is **$g(n)=\sum_{d\mid n}\mu(d)f(n/d)$**. Substituting the divisor sum defining $f$ and collecting the coefficient of $g(e)$ gives

$$
\sum_{d\mid n}\mu(d)f(n/d)=\sum_{e\mid n}g(e)\sum_{d\mid n/e}\mu(d)=g(n).
$$

This proof uses only finite sums, so no convergence hypothesis is needed.

Classifying $1,\ldots,n$ by their greatest common divisor with $n$ gives $\sum_{d\mid n}\varphi(d)=n$: the class with greatest common divisor $n/d$ contains exactly $\varphi(d)$ integers. Applying the [Möbius inversion formula](../../../../../mobius-inversion-formula.md) yields

$$
\boxed{\varphi(n)=\sum_{d\mid n}\mu(d)\frac nd=n\prod_{p\mid n}(1-p^{-1}).}
$$

The [Riemann zeta function](../../../../../riemann-zeta-function.md) is $\zeta(s)=\sum_{n\geq1}n^{-s}$ for $\operatorname{Re}s>1$. [Absolute convergence](../../../../../absolute-convergence.md) justifies multiplication of [Dirichlet series](../../../../../dirichlet-series.md). The divisor identity for the [Möbius function](../../../../../mobius-function.md) gives $\sum\mu(n)n^{-s}=1/\zeta(s)$ there. For $\operatorname{Re}s>2$ both factors below converge absolutely, and their [Dirichlet convolution](../../../../../dirichlet-convolution.md) is the [Euler totient function](../../../../../euler-totient-function.md):

$$
\boxed{\frac{\zeta(s-1)}{\zeta(s)}=\sum_{n=1}^{\infty}\frac{\varphi(n)}{n^s}.}
$$

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
