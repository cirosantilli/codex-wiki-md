<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $T(N)$ count pairs $n,n+2$ both [prime](../../../../../prime-number.md) with $n+2\leq N$. The [Selberg sieve](../../../../../selberg-sieve.md) replaces primality by the necessary condition that the polynomial $F(n)=n(n+2)$ have no small [prime](../../../../../prime-number.md) [divisor](../../../../../divisor.md). Its strength is a nonnegative quadratic majorant with optimizable [divisor](../../../../../divisor.md) weights; its limitation is that a sifted [integer](../../../../../integer.md) need not be [prime](../../../../../prime-number.md).

For a [prime](../../../../../prime-number.md) $p$, let $\nu(p)$ count the forbidden residues of $n$ modulo $p$. We have $\nu(2)=1$, since the two roots coincide modulo two, and $\nu(p)=2$ for every odd [prime](../../../../../prime-number.md), where the roots are zero and $-2$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) makes $\nu(d)$ multiplicative on [squarefree integers](../../../../../squarefree-integer.md). With $g(d)=\nu(d)/d$,

$$
\#\{n\leq N:d\mid F(n)\}=Ng(d)+O(\nu(d))
\qquad(d\text{ squarefree}).
$$

These local densities constitute the [sieve distribution](../../../../../sieve-distribution.md) for the twin-prime problem. Since $\sum_{p\leq z}g(p)=2\log\log z+O(1)$, it is a dimension-two sieve, which is why the expected upper bound has two logarithms in the denominator.

Let $P(R)=\prod_{p\leq R}p$ and choose real [Selberg sieve weights](../../../../../selberg-sieve-weights.md) $\lambda_d$ supported on squarefree $d\leq R$, with $\lambda_1=1$. If $\gcd(F(n),P(R))=1$, the only supported [divisor](../../../../../divisor.md) of $F(n)$ is one. Hence

$$
\mathbf1_{\gcd(F(n),P(R))=1}
\leq\left(\sum_{\substack{d\mid F(n)\\d\leq R}}\lambda_d\right)^2.
$$

Expanding and using the distribution of the polynomial roots gives

$$
S(N,R):=\#\{n\leq N:\gcd(F(n),P(R))=1\}
\leq NQ(\lambda)+O\left(\sum_{d,e\leq R}|\lambda_d\lambda_e|\nu([d,e])\right),
$$



$$
Q(\lambda)=\sum_{d,e\leq R}\lambda_d\lambda_e g([d,e]).
$$

Here $[d,e]$ denotes the [least common multiple](../../../../../least-common-multiple.md). The divisor-square support reaches $R^2$, although each individual weight is supported only to $R$; keeping these two levels distinct is essential for estimating the remainder.

The [Selberg sieve diagonalization](../../../../../selberg-sieve-diagonalization.md) solves the main-term minimization exactly. On [squarefree integers](../../../../../squarefree-integer.md) put

$$
k(r)=\prod_{p\mid r}(g(p)^{-1}-1),\qquad
w(r)=k(r)^{-1}=\prod_{p\mid r}\frac{g(p)}{1-g(p)},\qquad
Y_r=\sum_{\substack{d\leq R\\r\mid d}}g(d)\lambda_d.
$$

Multiplicativity gives

$$
g([d,e])=g(d)g(e)\sum_{r\mid(d,e)}k(r),
\qquad Q(\lambda)=\sum_{r\leq R}k(r)Y_r^2.
$$

Also, [Möbius inversion](../../../../../mobius-inversion-formula.md) gives $\sum_{r\leq R}\mu(r)Y_r=\lambda_1=1$. Therefore the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) proves

$$
Q(\lambda)\geq\frac1{G(R)},\qquad
G(R)=\sum_{\substack{r\leq R\\r\text{ squarefree}}}w(r),
$$

with equality at $Y_r=\mu(r)w(r)/G(R)$. Inverting the [divisor](../../../../../divisor.md) sums gives the optimizing weights

$$
\lambda_d=\frac{\mu(d)}{G(R)\prod_{p\mid d}(1-g(p))}
\sum_{\substack{m\leq R/d\\(m,d)=1\\m\text{ squarefree}}}w(m).
$$

In particular $\lambda_1=1$ and $Q(\lambda)=1/G(R)$.

These weights have $|\lambda_d|\leq1$, which supplies a simple rigorous remainder estimate. Indeed, multiply the inner sum by $\prod_{p\mid d}(1-g(p))^{-1}=\sum_{e\mid d}w(e)$. The terms are $w(em)$ for distinct [squarefree integers](../../../../../squarefree-integer.md) $em\leq R$ with $e\mid d$ and $(m,d)=1$, hence form a subset of the sum defining $G(R)$. Since $\nu([d,e])\leq\nu(d)\nu(e)$ and $\nu(d)\leq\tau(d)$,

$$
\sum_{d,e\leq R}|\lambda_d\lambda_e|\nu([d,e])
\leq\left(\sum_{d\leq R}\nu(d)\right)^2
\ll R^2\log^2(2R).
$$

Thus

$$
S(N,R)\leq\frac N{G(R)}+O(R^2\log^2(2R)).
$$

For this sieve $w(2)=1$ and $w(p)=2/(p-2)$ for odd [primes](../../../../../prime-number.md). Here is a direct proof that $G(R)\asymp\log^2R$, sufficient for the upper bound. Put

$$
W(z)=\prod_{p\leq z}(1+w(p))=\prod_{p\leq z}(1-g(p))^{-1}.
$$

The [Mertens theorem for reciprocal primes](../../../../../mertens-second-theorem.md) implies $W(z)\asymp\log^2z$, by taking logarithms and using the convergence of $\sum_pg(p)^2$. Give each [divisor](../../../../../divisor.md) $d\mid P(z)$ probability $w(d)/W(z)$. Its expected logarithm is

$$
\mathbb E(\log d)=\sum_{p\leq z}\frac{w(p)}{1+w(p)}\log p
=\sum_{p\leq z}g(p)\log p=2\log z+O(1),
$$

by the [Mertens first theorem](../../../../../mertens-first-theorem.md). With $z=R^{1/8}$ this is at most $\frac13\log R$ for large $R$. The [Markov inequality](../../../../../markov-inequality.md) shows that at least two thirds of the total product weight has $d\leq R$. These terms occur in $G(R)$, so $G(R)\gg W(R^{1/8})\gg\log^2R$. Conversely $G(R)\leq W(R)\ll\log^2R$, proving the claim without treating an untruncated [Euler product](../../../../../euler-product.md) as a truncated [divisor](../../../../../divisor.md) sum.

Choose, for example, $R=N^{1/4}$. Any twin-prime pair with smaller member greater than $R$ survives this sieve; pairs with smaller member at most $R$ contribute at most $O(R)$. Consequently

$$
\boxed{T(N)\leq\frac N{G(N^{1/4})}
+O(N^{1/2}\log^2N+N^{1/4})
\ll\frac N{(\log N)^2}.}
$$

The chosen level is deliberately enough to prove the correct logarithmic order; sharper level and remainder analyses improve the numerical upper-bound constant.

The local correction factor also explains the conjectured main-term constant. Relative to two independent primality conditions, the singular series is

$$
\mathfrak S=\prod_p\frac{1-\nu(p)/p}{(1-1/p)^2}
=2\prod_{p>2}\left(1-\frac1{(p-1)^2}\right)=2C_2.
$$

The [twin-prime constant](../../../../../twin-prime-constant.md) $C_2$ is positive and convergent because its logarithm has an absolutely convergent tail. The factor two at $p=2$ records that only one parity is allowed, while each odd-prime factor records the two distinct forbidden residues. The [Hardy–Littlewood twin-prime asymptotic conjecture](../../../../../hardy-littlewood-twin-prime-asymptotic-conjecture.md) predicts

$$
T(N)\sim2C_2\int_2^N\frac{dt}{(\log t)^2}
\sim\frac{2C_2N}{(\log N)^2}.
$$

This is a conjecture, not a consequence of the upper-bound calculation.

The [parity problem in sieve theory](../../../../../parity-problem.md) is the obstruction to reversing the argument. The nonnegative square majorizes all survivors, including composites with sufficiently large [prime factors](../../../../../prime-factor.md); small-divisor information does not isolate the desired prime-factor parity or force both factors to be [prime](../../../../../prime-number.md). Therefore the [Selberg sieve](../../../../../selberg-sieve.md) establishes the correct upper-bound scale and the arithmetic local factors, but by itself does not prove a positive lower bound for twin [primes](../../../../../prime-number.md), their infinitude, or the conjectured asymptotic.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
