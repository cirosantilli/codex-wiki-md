<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

An [arithmetic function](../../../../../arithmetic-function.md) $f$ is [multiplicative](../../../../../multiplicative-function.md) if $f(mn)=f(m)f(n)$ whenever $m$ and $n$ are [coprime integers](../../../../../coprime-integers.md). If $g(n)=\sum_{d\mid n}f(d)$ and $(m,n)=1$, every positive [integer divisor](../../../../../divisor.md) of $mn$ is uniquely $d_1d_2$ with $d_1\mid m$ and $d_2\mid n$. Hence

$$
g(mn)=\sum_{d_1\mid m}\sum_{d_2\mid n}f(d_1d_2)
=\left(\sum_{d_1\mid m}f(d_1)\right)
 \left(\sum_{d_2\mid n}f(d_2)\right)
=g(m)g(n),
$$

so $g$ is [multiplicative](../../../../../multiplicative-function.md).

The [Möbius function](../../../../../mobius-function.md) is defined by $\mu(1)=1$, $\mu(n)=0$ if the [square](../../../../../square-number.md) of a [prime number](../../../../../prime-number.md) divides $n$, and $\mu(n)=(-1)^r$ if $n$ is a product of $r$ distinct [prime numbers](../../../../../prime-number.md). Coprime integers have disjoint sets of [prime factors](../../../../../prime-factor.md), so this definition immediately gives $\mu(mn)=\mu(m)\mu(n)$ when $(m,n)=1$.

For $n=p_1^{a_1}\cdots p_r^{a_r}>1$, only the [square-free](../../../../../square-free-integer.md) divisors contribute, and therefore

$$
\sum_{d\mid n}\mu(d)=\prod_{j=1}^r(1-1)=0.
$$

For $n=1$ the sum is $1$. Thus $\mathbf 1*\mu=\varepsilon$ in the language of [Dirichlet convolution](../../../../../dirichlet-convolution.md). Convolving $g=\mathbf 1*f$ with $\mu$ gives the [Möbius inversion formula](../../../../../mobius-inversion-formula.md)

$$
f(n)=(\mu*g)(n)=\sum_{e\mid n}\mu(e)g(n/e).
$$

If $f(n)=n$, its [divisor sum](../../../../../divisor-sum.md) is the [sum-of-divisors function](../../../../../sum-of-divisors-function.md). Conversely, if $g(n)=n$, [Möbius inversion](../../../../../mobius-inversion-formula.md) gives

$$
f(n)=\sum_{e\mid n}\mu(e)\frac ne=\varphi(n),
$$

using the standard divisor identity for the [Euler totient function](../../../../../euler-totient-function.md). Therefore the two requested answers are

$$
\boxed{g(n)=\sigma_1(n),\qquad f(n)=\varphi(n).}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
