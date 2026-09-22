<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Selberg upper-bound sieve](../../../../../selberg-upper-bound-sieve.md) replaces an exact but long inclusion-exclusion expansion by a short nonnegative square, and then minimizes its main term. For an interval $\mathcal A=(a,a+x]\cap\mathbb Z$, the count of multiples of every [integer](../../../../../integer.md) $d$ is

$$
|\mathcal A_d|=\left\lfloor\frac{a+x}d\right\rfloor-\left\lfloor\frac ad\right\rfloor
=\frac xd+r_d,\qquad |r_d|\le1.
$$

Crucially the remainder bound is independent of $a$.

Let $P(z)=\prod_{p\le z}p$ and take real weights $\lambda_d$, supported on [squarefree](../../../../../squarefree-integer.md) $d\le z$, with $\lambda_1=1$. If $(n,P(z))=1$, the sum of these weights over [divisors](../../../../../divisor.md) of $n$ is just one; for all other $n$ its square is nonnegative. Thus

$$
\mathbf1_{(n,P(z))=1}\le\left(\sum_{d\mid n}\lambda_d\right)^2.
$$

Expanding and counting common multiples gives

$$
S(\mathcal A,z)\le xQ(\lambda)+\left(\sum_{d\le z}|\lambda_d|\right)^2,
\qquad Q(\lambda)=\sum_{d,e\le z}\frac{\lambda_d\lambda_e}{[d,e]}.
$$

This separates the local density $1/[d,e]$ from a uniform interval error. The weights will be chosen to minimize $Q$.

The [Euler totient function](../../../../../euler-totient-function.md) identity $(d,e)=\sum_{r\mid d,\ r\mid e}\varphi(r)$ yields the [Selberg sieve diagonalization](../../../../../selberg-sieve-diagonalization.md)

$$
Q(\lambda)=\sum_{r\le z}\varphi(r)y_r^2,
\qquad y_r=\sum_{\substack{d\le z\\r\mid d}}\frac{\lambda_d}{d}.
$$

Only [squarefree](../../../../../squarefree-integer.md) $r$ occur. Inverting this finite triangular sum by [Möbius inversion](../../../../../mobius-inversion-formula.md) gives

$$
\frac{\lambda_d}d=\sum_{\substack{r\le z\\d\mid r}}\mu(r/d)y_r,
\qquad1=\lambda_1=\sum_{r\le z}\mu(r)y_r.
$$

Write $G(z)=\sum_{r\le z}\mu(r)^2/\varphi(r)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $1\le G(z)Q(\lambda)$, with equality at $y_r=\mu(r)/(\varphi(r)G(z))$. The inverse formula then produces the optimal [Selberg sieve weights](../../../../../selberg-sieve-weights.md)

$$
\lambda_d=\mu(d)\frac{d}{\varphi(d)}\frac{G_d(z/d)}{G(z)},
\qquad G_d(v)=\sum_{\substack{\ell\le v\\(\ell,d)=1}}\frac{\mu(\ell)^2}{\varphi(\ell)},
\qquad Q(\lambda)=\frac1{G(z)}.
$$

The constraints are satisfied, since the diagonal transformation is invertible and $\sum_r\mu(r)y_r=1$.

We need the leading constant, not just $G(z)\gg\log z$. Here is an elementary proof of the [Selberg sieve denominator asymptotic](../../../../../selberg-sieve-denominator-asymptotic.md). For $g(n)=\mu(n)^2/\varphi(n)$ define the [multiplicative arithmetic function](../../../../../multiplicative-function.md) $h$ by

$$
h(p)=\frac1{p(p-1)},\qquad h(p^2)=-\frac1{p(p-1)},\qquad h(p^j)=0\quad(j\ge3).
$$

Checking the prime-local factors shows $g=h*(n\mapsto1/n)$. Also $\sum_n|h(n)|\log(2n)<\infty$: the local factors for absolute values differ from one by $O(p^{-2})$, and their logarithmic first moments sum $O((\log p)/p^2)$. The signed local sums are all one, so [absolute convergence](../../../../../absolute-convergence.md) gives $\sum_nh(n)=1$. Using the [harmonic number](../../../../../harmonic-number.md) estimate,

$$
G(z)=\sum_{d\le z}h(d)H_{\lfloor z/d\rfloor}
=\sum_{d\le z}h(d)\log(z/d)+O(1)=\log z+O(1).
$$

For the last equality, $\sum|h(d)|\log d$ is bounded and $\log z\sum_{d>z}|h(d)|\le\sum_{d>z}|h(d)|\log d$ is bounded too.

The [optimal Selberg weights have modulus at most one](../../../../../optimal-selberg-weights-have-modulus-at-most-one.md). To prove this here, for [squarefree](../../../../../squarefree-integer.md) $d$ use $d/\varphi(d)=\sum_{e\mid d}1/\varphi(e)$. The product $(d/\varphi(d))G_d(z/d)$ is the sum of $1/\varphi(e\ell)$ over $e\mid d$, $\ell\le z/d$, $(\ell,d)=1$, with $\ell$ [squarefree](../../../../../squarefree-integer.md). All $e\ell$ are distinct [squarefree integers](../../../../../squarefree-integer.md) at most $z$, and so these are a subset of the terms of $G(z)$. The displayed weight formula now gives $|\lambda_d|\le1$. Consequently

$$
S(\mathcal A,z)\le\frac{x}{G(z)}+z^2.
$$

Every [prime](../../../../../prime-number.md) in the interval exceeding $z$ survives the sieve; at most $z$ smaller [primes](../../../../../prime-number.md) must be restored. Choose $z=\lfloor\sqrt x/(\log x)^2\rfloor$. Then

$$
\log z=\tfrac12\log x-2\log\log x+o(1),\qquad
z+z^2=o(x/\log x),
$$

and the [uniform interval bound from optimal Selberg weights](../../../../../uniform-interval-bound-from-optimal-selberg-weights.md) follows:

$$
\pi(a+x)-\pi(a)\le\frac{x}{G(z)}+z^2+z
=\left(2+O\left(\frac{\log\log x}{\log x}\right)\right)\frac{x}{\log x}.
$$

All constants are independent of $a$. Given $\varepsilon>0$, make the absolute error in the coefficient smaller than $\varepsilon/2$ by choosing $x_0(\varepsilon)$ large enough. **Uniformly for every $a>0$ and $x>x_0(\varepsilon)$,**

$$
\boxed{\pi(a+x)-\pi(a)<(2+\varepsilon)\frac{x}{\log x}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
