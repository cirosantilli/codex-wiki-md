<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $\Re s>1$, the [Euler products](../../../../../euler-product.md) are

$$
\boxed{\zeta(s)=\prod_p(1-p^{-s})^{-1},\qquad
L(s,\chi)=\prod_p(1-\chi(p)p^{-s})^{-1}.}
$$

The [Dirichlet character](../../../../../dirichlet-character.md) is completely multiplicative, and [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) expands each finite product into the terms of the corresponding [Dirichlet series](../../../../../dirichlet-series.md) supported on those primes. Absolute convergence permits passage to all primes. More strongly, the absolutely convergent [Euler product](../../../../../euler-product.md) logarithm gives

$$
L(s,\chi)=\exp\left(\sum_p\sum_{m\ge1}\frac{\chi(p)^m}{m p^{ms}}\right)\ne0,
$$

since the sum of absolute values is bounded by $\sum_{n\ge2}\sum_{m\ge1}n^{-m\Re s}/m<\infty$.

We prove [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../../../nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one.md), including real [Dirichlet characters](../../../../../dirichlet-character.md). If $\chi$ is nonprincipal modulo $q$, periodicity and the given [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) bound $A_\chi(x)=\sum_{n\le x}\chi(n)$ by $q$. [Partial summation](../../../../../abel-s-summation-formula.md) gives

$$
L(s,\chi)=s\int_1^\infty A_\chi(x)x^{-s-1}\,dx,
$$

which is holomorphic for $\Re s>0$ by locally uniform convergence, including after differentiation. The [principal Dirichlet character](../../../../../principal-dirichlet-character.md) instead has

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s}),
$$

with a simple pole at one.

For a nonreal [Dirichlet character](../../../../../dirichlet-character.md), consider $P(s)=\prod_{\chi\bmod q}L(s,\chi)$. For real $\sigma>1$, its [Euler product](../../../../../euler-product.md) logarithm is

$$
\log P(\sigma)=\sum_{p\nmid q}\sum_{m\ge1}
\frac{\sum_\chi\chi(p^m)}{m p^{m\sigma}}\ge0.
$$

The given character inversion with $a=1$ makes each inner sum either $\varphi(q)$ or zero, so $P(\sigma)\ge1$. If $L(1,\chi)=0$ for a nonreal [Dirichlet character](../../../../../dirichlet-character.md), then $L(1,\overline\chi)=0$ as well, since their values at real $s$ are conjugate. These are two distinct factors. All nonprincipal factors are holomorphic at one, and only the principal factor has a simple pole. Their two zeros would force $P(\sigma)\to0$, a contradiction.

For a real nonprincipal [Dirichlet character](../../../../../dirichlet-character.md), suppose $L(1,\chi)=0$. Then $G(s)=\zeta(s)L(s,\chi)$ is holomorphic throughout $\Re s>0$: the supplied continuation of the [Riemann zeta function](../../../../../riemann-zeta-function.md) has no other pole there, and the zero cancels the pole at one. On $\Re s>1$ its [Dirichlet series](../../../../../dirichlet-series.md) has coefficients

$$
g_n=\sum_{d\mid n}\chi(d)\ge0.
$$

To check the sign explicitly, for a [prime power](../../../../../prime-power.md) $p^j$ the local sum is $j+1$ if $\chi(p)=1$, is $1$ for even $j$ and $0$ for odd $j$ if $\chi(p)=-1$, and is $1$ if $\chi(p)=0$. Multiplication over [prime factors](../../../../../prime-factor.md) proves nonnegativity and $g_{m^2}\ge1$. Also $g_n\le\tau(n)$, so termwise derivatives at $s=2$ are justified by absolute convergence:

$$
(-1)^jG^{(j)}(2)=\sum_n\frac{g_n(\log n)^j}{n^2}\ge0.
$$

The disc $|s-2|<2$ lies in $\Re s>0$. Its [Taylor series](../../../../../taylor-series.md) therefore converges at $s=1/2$, and [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
G(1/2)=\sum_{j\ge0}\frac{(3/2)^j}{j!}\sum_n\frac{g_n(\log n)^j}{n^2}
=\sum_n\frac{g_n}{n^{1/2}}\ge\sum_{m\ge1}\frac1m=\infty.
$$

This contradicts holomorphy at $1/2$. It is the positive-coefficient argument behind the [Landau theorem for a Dirichlet series with nonnegative coefficients](../../../../../landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients.md), proved here rather than invoked. Thus $L(1,\chi)\ne0$ for every nonprincipal [Dirichlet character](../../../../../dirichlet-character.md).

It remains to detect the primes. For real $\sigma>1$, the [Euler product](../../../../../euler-product.md) logarithm satisfies

$$
\log L(\sigma,\chi)=\sum_p\frac{\chi(p)}{p^\sigma}+O(1),
$$

uniformly as $\sigma\downarrow1$: terms with $m\ge2$ are bounded in absolute value by $\sum_{n\ge2}\sum_{m\ge2}n^{-m}/m<\infty$. For a nonprincipal [Dirichlet character](../../../../../dirichlet-character.md), a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) of $L$ exists near one by the nonvanishing just proved. On a short real interval it differs from the [Euler product](../../../../../euler-product.md) logarithm by a fixed multiple of $2\pi i$, so the prime sum stays bounded. For the [principal Dirichlet character](../../../../../principal-dirichlet-character.md), the simple pole instead gives

$$
\sum_p\chi_0(p)p^{-\sigma}=\log\frac1{\sigma-1}+O_q(1).
$$

Applying the supplied [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) for a reduced residue class $a$ now yields

$$
\sum_{p\equiv a\pmod q}p^{-\sigma}
=\frac1{\varphi(q)}\sum_\chi\overline{\chi(a)}\sum_p\chi(p)p^{-\sigma}
=\frac1{\varphi(q)}\log\frac1{\sigma-1}+O_q(1).
$$

The right side tends to infinity, whereas a finite set of primes would give a bounded left side. Therefore **every residue class coprime to $q$ contains infinitely many primes**, proving the [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
