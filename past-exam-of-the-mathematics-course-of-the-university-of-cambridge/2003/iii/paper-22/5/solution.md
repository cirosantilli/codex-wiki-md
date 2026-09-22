<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix a modulus $q$ and a [residue class](../../../../../residue-class.md) $a$ with $(a,q)=1$. The [Dirichlet characters](../../../../../dirichlet-character.md) modulo $q$ are the one-dimensional [characters of a representation](../../../../../character-of-a-representation.md) of $(\mathbb Z/q\mathbb Z)^\times$, extended by zero on nonunits. Let $\chi_0$ be the [principal Dirichlet character](../../../../../principal-dirichlet-character.md).

For every [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md) the [partial sums](../../../../../partial-sum.md) $\sum_{n\le u}\chi(n)$ are bounded: the sum over a full period is zero, and a remaining incomplete period has bounded length. [Partial summation](../../../../../abel-s-summation-formula.md) therefore continues its [Dirichlet L-function](../../../../../dirichlet-l-function.md) holomorphically to $\Re s>0$ by

$$
L(s,\chi)=s\int_1^\infty\left(\sum_{n\le u}\chi(n)\right)u^{-s-1}\,du.
$$

This shows in particular that it has no [pole](../../../../../pole.md) at one. By contrast

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../../../pole.md) there. We use the stipulated nonvanishing $L(1,\chi)\ne0$ for every real [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md), and establish the remaining nonvanishing as follows.

For real $\sigma>1$, take the [product over all Dirichlet characters](../../../../../product-over-all-dirichlet-characters.md). The [Euler product](../../../../../euler-product.md) [logarithms](../../../../../logarithm.md) and [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) give

$$
\log\prod_{\chi\bmod q}L(\sigma,\chi)
=\sum_{p\nmid q}\sum_{j\ge1}\frac{\sum_\chi\chi(p)^j}{jp^{j\sigma}}
=\varphi(q)\sum_{p\nmid q}\sum_{\substack{j\ge1\\p^j\equiv1\pmod q}}\frac1{jp^{j\sigma}}\ge0.
$$

Thus this product is real and at least one. If a nonreal [Dirichlet character](../../../../../dirichlet-character.md) had $L(1,\chi)=0$, [complex conjugation](../../../../../complex-conjugation.md) would also give $L(1,\overline\chi)=0$. These are distinct factors. Two zeros and only one possible simple [pole](../../../../../pole.md) force the whole product to tend to zero as $\sigma\downarrow1$, contradicting the lower bound. Hence **all [nonprincipal Dirichlet characters](../../../../../nonprincipal-dirichlet-character.md) have $L(1,\chi)\ne0$**, under the given real-character assumption.

For $\sigma>1$, [absolute convergence](../../../../../absolute-convergence.md) of each [Euler product](../../../../../euler-product.md) gives

$$
\log L(\sigma,\chi)
=\sum_{p\nmid q}\frac{\chi(p)}{p^\sigma}+O(1),
$$

with bounded remainder as $\sigma\downarrow1$: the terms of prime-power exponent at least two have total modulus at most $\sum_{n\ge2}1/(n(n-1))$. Since a nonprincipal $L$ defines a [holomorphic function](../../../../../holomorphic-function.md) that is nonzero near one, its Euler-product [logarithm](../../../../../logarithm.md) differs from a local [holomorphic logarithm](../../../../../holomorphic-logarithm.md) by a fixed [integer](../../../../../integer.md) multiple of $2\pi i$ on a short real interval. It is therefore bounded there. For the [principal Dirichlet character](../../../../../principal-dirichlet-character.md) the [pole](../../../../../pole.md) instead gives

$$
\log L(\sigma,\chi_0)=\log\frac1{\sigma-1}+O_q(1).
$$

Apply the [Dirichlet character](../../../../../dirichlet-character.md) orthogonality relation at each [prime](../../../../../prime-number.md). The [prime-character sum near one](../../../../../prime-character-sum-near-one.md) yields

$$
\sum_{p\equiv a\pmod q}p^{-\sigma}
=\frac1{\varphi(q)}\sum_{\chi\bmod q}\overline{\chi(a)}\log L(\sigma,\chi)+O_q(1)
=\frac1{\varphi(q)}\log\frac1{\sigma-1}+O_q(1).
$$

This tends to infinity. A finite set of [primes](../../../../../prime-number.md) would have a bounded sum as $\sigma\downarrow1$, so **every [coprime](../../../../../coprime-integers.md) [residue class](../../../../../residue-class.md) contains infinitely many [primes](../../../../../prime-number.md)**. This proves the [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) from the specified assumption. In fact it proves divergence of the corresponding reciprocal-prime series and gives [Dirichlet density](../../../../../dirichlet-density.md) $1/\varphi(q)$.

Finally, for real $s>1$ each [prime](../../../../../prime-number.md) satisfies

$$
p^{-s}=s\int_p^\infty t^{-s-1}\,dt.
$$

The integrands are nonnegative, so [Tonelli theorem](../../../../../tonelli-theorem.md) permits summation inside the integral. At a fixed $t$, exactly $\pi(t,q,a)$ [primes](../../../../../prime-number.md) from the [residue class](../../../../../residue-class.md) have entered. Therefore

$$
\boxed{\sum_{p\equiv a\pmod q}\frac1{p^s}
=s\int_1^\infty\frac{\pi(t,q,a)}{t^{s+1}}\,dt.}
$$

Both sides are finite, since they are bounded respectively by $\sum_{n\ge2}n^{-s}$ and $s\int_1^\infty t^{-s}\,dt$. The values of a counting function at its isolated jump endpoints do not change this integral.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
