<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Selberg upper-bound sieve](../../../../../selberg-upper-bound-sieve.md) replaces the [indicator function](../../../../../indicator-function.md) of a sifted set by the square of a divisor sum. If the real [Selberg sieve weights](../../../../../selberg-sieve-weights.md) satisfy $\lambda_1=1$, then

$$
\boldsymbol1_{(F(n),P(z))=1}
\le\left(\sum_{\substack{d\mid F(n)\\d\mid P(z)}}\lambda_d\right)^2,
\qquad P(z)=\prod_{p\le z}p.
$$

When $F(n)$ has no forbidden [prime factors](../../../../../prime-factor.md), the divisor sum is exactly one; otherwise its square is still nonnegative. Taking the weights to vanish for $d>z$ controls the error in summing this majorant. The main term is a positive [quadratic form](../../../../../quadratic-form.md) that can be diagonalized and minimized explicitly. This optimization, together with a bound for the remainder, is the central idea of the [Selberg sieve](../../../../../selberg-sieve.md).

For [twin primes](../../../../../twin-prime.md), take $F(n)=n(n+2)$ and let $\rho(d)$ be the number of its [roots](../../../../../root-of-a-root-system.md) modulo a [squarefree integer](../../../../../squarefree-integer.md) $d$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) makes $\rho$ a [multiplicative arithmetic function](../../../../../multiplicative-function.md), with $\rho(2)=1$ and $\rho(p)=2$ for odd [primes](../../../../../prime-number.md). Thus the [polynomial root density in a sieve](../../../../../polynomial-root-density-in-a-sieve.md) is $g(d)=\rho(d)/d$, and

$$
\#\{n\le x:d\mid F(n)\}=xg(d)+r_d,\qquad |r_d|\le\rho(d).
$$

Summing the majorant gives

$$
S(x,z):=\#\{n\le x:(F(n),P(z))=1\}
\le xQ(\lambda)+O\left(\left(\sum_{d\le z}|\lambda_d|\rho(d)\right)^2\right),
$$

where $Q(\lambda)=\sum_{d,e\le z}\lambda_d\lambda_e g([d,e])$, with all indices [squarefree](../../../../../squarefree-integer.md). Here $\rho([d,e])\le\rho(d)\rho(e)$ controls the error.

We carry out the [Selberg sieve diagonalization](../../../../../selberg-sieve-diagonalization.md). Put

$$
h(r)=\prod_{p\mid r}\left(\frac1{g(p)}-1\right),\qquad
h(1)=1,\qquad
y_r=\sum_{\substack{d\le z\\r\mid d}}\lambda_dg(d).
$$

For [squarefree integers](../../../../../squarefree-integer.md) $d,e$, [multiplicativity](../../../../../multiplicativity-of-an-arithmetic-function.md) gives

$$
g([d,e])=g(d)g(e)\sum_{r\mid(d,e)}h(r),
\qquad Q(\lambda)=\sum_{r\le z}h(r)y_r^2.
$$

The identity behind the first equality is $\prod_{p\mid(d,e)}[1+h(p)]=1/g((d,e))$. [Möbius inversion](../../../../../mobius-inversion-formula.md) gives $\lambda_1=\sum_r\mu(r)y_r=1$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) therefore implies

$$
1\le\left(\sum_{r\le z}h(r)y_r^2\right)
\left(\sum_{r\le z}\frac{\mu(r)^2}{h(r)}\right).
$$

Define $G(z)=\sum_{r\le z,\ r\text{ squarefree}}1/h(r)$. Equality is attained at $y_r=\mu(r)/(h(r)G(z))$, giving **$\min Q=1/G(z)$**. Inverting again, the optimizing [Selberg sieve weights](../../../../../selberg-sieve-weights.md) are

$$
\lambda_d=\frac{\mu(d)}{g(d)h(d)G(z)}G_d(z/d),\qquad
G_d(v)=\sum_{\substack{m\le v\\(m,d)=1\\m\text{ squarefree}}}\frac1{h(m)}.
$$

In particular $\lambda_1=1$. Since $G_d(z/d)\le G(z)$,

$$
|\lambda_d|\le\frac1{g(d)h(d)}
=\prod_{p\mid d}\frac1{1-g(p)}\le d.
$$

The last inequality holds separately at $p=2$, $p=3$, and $p\ge5$. Together with $\rho(d)\le d$, this crude bound already makes the remainder $O(z^6)$, because $\sum_{d\le z}d^2=O(z^3)$.

We also need a lower bound for $G(z)$; we prove it rather than presuppose a sieve asymptotic. For odd [squarefree integers](../../../../../squarefree-integer.md) $r$,

$$
\frac1{h(r)}=\prod_{p\mid r}\frac2{p-2}\ge\frac{2^{\omega(r)}}r,
$$

where $\omega(r)$ counts distinct [prime factors](../../../../../prime-factor.md). Put $y=\sqrt z$ and $L(y)=\sum_{a\le y,\ a\text{ odd}}1/a=\tfrac12\log y+O(1)$. The total weight $1/(ab)$ of odd pairs $a,b\le y$ is $L(y)^2$. Exclude pairs for which $a$ has a square [prime factor](../../../../../prime-factor.md), $b$ has a square [prime factor](../../../../../prime-factor.md), or $a,b$ have a common [prime factor](../../../../../prime-factor.md). For each of these three categories the total weight is at most $L(y)^2\sum_{p\text{ odd}}p^{-2}$: for example, the weighted count of odd multiples of $p^2$ is $p^{-2}L(y/p^2)\le p^{-2}L(y)$, and the common-factor category uses $p^{-1}L(y/p)$ for each variable. Moreover,

$$
\sum_{p\text{ odd}}p^{-2}
\le\sum_{m\ge1}(2m+1)^{-2}
\le\frac19+\int_1^\infty\frac{dt}{(2t+1)^2}
=\frac5{18}.
$$

Hence the remaining odd [coprime](../../../../../coprime-integers.md) [squarefree](../../../../../squarefree-integer.md) pairs have weight at least $L(y)^2/6$. Their products $r=ab\le z$ are [squarefree](../../../../../squarefree-integer.md), and $2^{\omega(r)}$ counts all ordered [coprime](../../../../../coprime-integers.md) factorizations of $r$. This proves the [elementary lower bound for the twin-prime sieve denominator](../../../../../elementary-lower-bound-for-the-twin-prime-sieve-denominator.md):

$$
G(z)\ge\sum_{\substack{r\le z\\r\text{ odd and squarefree}}}\frac{2^{\omega(r)}}r
\ge\frac{L(\sqrt z)^2}{6}\gg(\log z)^2.
$$

If $p>z$ and both $p,p+2$ are [primes](../../../../../prime-number.md), $F(p)$ survives the sieve. The at most $z$ smaller values are the only exceptions. Thus, with $T(x)=\#\{p\le x:p,p+2\text{ prime}\}$ and $z=x^{1/10}$, the [twin-prime upper bound from a quadratic sieve](../../../../../twin-prime-upper-bound-from-a-quadratic-sieve.md) becomes

$$
T(x)\le S(x,z)+z\ll\frac{x}{(\log z)^2}+z^6+z,
\qquad\boxed{T(x)\ll\frac{x}{(\log x)^2}.}
$$

Finally [partial summation](../../../../../abel-s-summation-formula.md) gives

$$
\sum_{\substack{p\le X\\p,p+2\text{ prime}}}\frac1p
=\frac{T(X)}X+\int_2^X\frac{T(t)}{t^2}\,dt.
$$

The integral over $[3,\infty)$ is bounded by a constant times $\int_3^\infty dt/(t(\log t)^2)<\infty$. The nonnegative partial sums are therefore bounded and increasing. Thus **the reciprocal [series](../../../../../series-mathematics.md) over the smaller members of twin-prime pairs converges**, a form of [Brun's theorem](../../../../../brun-s-theorem.md). The upper bound does not assert that infinitely many [twin primes](../../../../../twin-prime.md) exist.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
