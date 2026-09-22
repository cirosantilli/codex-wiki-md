<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Selberg upper-bound sieve](../../../../../selberg-upper-bound-sieve.md) replaces a difficult coprimality indicator by a nonnegative square whose coefficients can be optimized. Let $P(z)=\prod_{p\le z}p$, and suppose a finite sequence has divisibility counts

$$
A_d=Xg(d)+r_d\qquad(d\mid P(z)),
$$

where $g$ is multiplicative on [squarefree integers](../../../../../squarefree-integer.md) and $0<g(p)<1$. Choose real [Selberg sieve weights](../../../../../selberg-sieve-weights.md) $\lambda_1=1$ supported on $d\mid P(z)$ with $d\le R$. If an entry has no [prime](../../../../../prime-number.md) factor in $P(z)$, its only weighted divisor is $1$, so its indicator is bounded above by the square of the divisor sum. Summing gives

$$
S\le\sum_{d,e\le R}\lambda_d\lambda_e A_{[d,e]}
=XQ(\lambda)+O\left(\sum_{d,e\le R}|\lambda_d\lambda_e r_{[d,e]}|\right),
$$

where $Q(\lambda)=\sum_{d,e}\lambda_d\lambda_e g([d,e])$. This is an upper bound regardless of the signs of the weights.

Here is the optimization. On the permitted [squarefree integers](../../../../../squarefree-integer.md) put

$$
h(r)=\prod_{p\mid r}\frac{1-g(p)}{g(p)},\qquad k(r)=h(r)^{-1},\qquad
Y_r=\sum_{r\mid d}\lambda_dg(d).
$$

The identity

$$
g([d,e])=g(d)g(e)\sum_{r\mid(d,e)}h(r)
$$

can be checked one [prime](../../../../../prime-number.md) at a time: a [prime](../../../../../prime-number.md) in both $d$ and $e$ gives the factor $1+h(p)=1/g(p)$. Thus

$$
Q(\lambda)=\sum_rh(r)Y_r^2.
$$

Finite [Möbius inversion](../../../../../mobius-inversion-formula.md) gives $\lambda_dg(d)=\sum_{d\mid r}\mu(r/d)Y_r$, and in particular the condition $\lambda_1=1$ becomes $\sum_r\mu(r)Y_r=1$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) now yields

$$
Q(\lambda)\ge\frac1{J(R,z)},\qquad
J(R,z)=\sum_{\substack{r\le R\\r\mid P(z)}}k(r).
$$

Equality is attained by $Y_r=\mu(r)k(r)/J$. Inverting again gives the explicit optimizing weights

$$
\lambda_d=\mu(d)\prod_{p\mid d}(1-g(p))^{-1}\,
\frac{\displaystyle\sum_{\substack{v\le R/d\\v\mid P(z)\\(v,d)=1}}k(v)}{J(R,z)}.
$$

They satisfy $|\lambda_d|\le1$. To see this, multiply out $\prod_{p\mid d}(1-g(p))^{-1}=\sum_{e\mid d}k(e)$. The numerator becomes the sum of $k(ev)$ over distinct permitted integers $ev\le R$ with $e\mid d$ and $(v,d)=1$, a subset of the terms in $J$. We therefore have a main term $X/J$ and a controllable remainder. This proves the basic [Selberg sieve diagonalization](../../../../../selberg-sieve-diagonalization.md) and the useful bound on the weights, rather than merely asserting an optimized density.

Apply it to the polynomial $F(n)=n(n+2)$ for $1\le n\le N$. If $\omega(d)$ is the number of roots of $F$ modulo squarefree $d$, the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives

$$
\omega(2)=1,\qquad \omega(p)=2\ (p>2),\qquad
A_d=\frac{\omega(d)}dN+O(\omega(d)).
$$

Use $g(d)=\omega(d)/d$, $R=z=N^{1/8}$, and sieve the indices for which $F(n)$ has no [prime](../../../../../prime-number.md) factor at most $z$. The local weights are

$$
k(2)=1,\qquad k(p)=\frac2{p-2}\quad(p>2).
$$

We claim $J(z,z)\gg(\log z)^2$. The following truncated-product argument supplies the necessary lower bound. Put $w=z^{1/8}$, and consider all [squarefree integers](../../../../../squarefree-integer.md) on the [primes](../../../../../prime-number.md) at most $w$, with total weight

$$
W=\prod_{p\le w}(1+k(p))=\prod_{p\le w}(1-g(p))^{-1}.
$$

Give such an integer $d$ [probability](../../../../../probability.md) $k(d)/W$. [Prime](../../../../../prime-number.md) inclusion is independent with [probability](../../../../../probability.md) $g(p)$, so

$$
\mathbb E[\log d]=\sum_{p\le w}g(p)\log p=2\log w+O(1)=\tfrac14\log z+O(1),
$$

by the [Mertens first theorem](../../../../../mertens-first-theorem.md), absorbing the [prime](../../../../../prime-number.md) $2$ separately. For sufficiently large $z$, this is at most $\tfrac12\log z$. The [Markov inequality](../../../../../markov-inequality.md) shows that at least half of $W$ lies on $d\le z$, all of which are terms in $J(z,z)$.

Moreover, [partial summation](../../../../../abel-s-summation-formula.md) applied to the [Mertens first theorem](../../../../../mertens-first-theorem.md) gives

$$
\sum_{p\le w}\frac1p=\log\log w+B+O(1/\log w).
$$

Indeed it is $A(w)/\log w+\int_2^w A(t)/(t(\log t)^2)\,dt$, and the contribution of $A(t)-\log t=O(1)$ has a finite limiting constant with tail $O(1/\log w)$. Expanding the logarithm of $W$ now gives

$$
\log W=2\sum_{3\le p\le w}\frac1p+O(1)=2\log\log w+O(1).
$$

The error is bounded since $\sum_p p^{-2}<\infty$. Consequently $W\asymp(\log w)^2\asymp(\log z)^2$, proving the claim. The exponent two reflects the two forbidden classes at almost every [prime](../../../../../prime-number.md).

For the remainder use $|\lambda_d|\le1$ and the simple bound $\omega([d,e])\le[d,e]\le de$. Hence

$$
\sum_{d,e\le z}|\lambda_d\lambda_e r_{[d,e]}|\ll\sum_{d,e\le z}de\ll z^4.
$$

The number of surviving indices is therefore

$$
S\ll\frac{N}{(\log z)^2}+z^4.
$$

Every pair of [primes](../../../../../prime-number.md) $p,p+2$ with $p>z$ survives, since both its [prime](../../../../../prime-number.md) factors exceed $z$. The exceptional pairs with $p\le z$ number at most $z$. With $z=N^{1/8}$ we obtain

$$
\boxed{\#\{p\le N:p\text{ and }p+2\text{ prime}\}\ll\frac{N}{(\log N)^2}+N^{1/2}+N^{1/8}\ll\frac{N}{(\log N)^2}.}
$$

This is the [twin-prime upper bound from a quadratic sieve](../../../../../twin-prime-upper-bound-from-a-quadratic-sieve.md). The method constructs a majorant and bounds the sifted set; it does not give a positive lower bound for twin [primes](../../../../../prime-number.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
