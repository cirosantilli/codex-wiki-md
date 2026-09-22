<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix a positive integer $q$ and an integer $a$ [coprime](../../../../../coprime-integers.md) to $q$. We use [Dirichlet characters](../../../../../dirichlet-character.md) modulo $q$, extended by [zero](../../../../../zero-of-a-function.md) on integers not [coprime](../../../../../coprime-integers.md) to $q$, and write $\chi_0$ for the [principal Dirichlet character](../../../../../principal-dirichlet-character.md). For a [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md), the sum over one complete period is [zero](../../../../../zero-of-a-function.md). Its partial sums $A_\chi(u)=\sum_{n\le u}\chi(n)$ are therefore $O(q)$. [Partial summation](../../../../../abel-s-summation-formula.md) gives

$$
L(s,\chi)=s\int_1^\infty A_\chi(u)u^{-s-1}\,du,\qquad\Re s>0.
$$

The integral converges locally uniformly there, so these [Dirichlet L-functions](../../../../../dirichlet-l-function.md) are [holomorphic](../../../../../complex-differentiability-at-a-point.md) at one. On the other hand,

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../../../pole.md) at one, with [residue](../../../../../residue.md) $\varphi(q)/q$.

The assumed [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../../../nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one.md) for real [Dirichlet characters](../../../../../dirichlet-character.md) also excludes vanishing for nonreal ones. To prove this, form the [product over all Dirichlet characters](../../../../../product-over-all-dirichlet-characters.md)

$$
\mathcal F(\sigma)=\prod_{\chi\bmod q}L(\sigma,\chi),\qquad\sigma>1.
$$

Use the [logarithm](../../../../../logarithm.md) supplied by the absolutely convergent [Euler product](../../../../../euler-product.md). The [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) yields

$$
\log\mathcal F(\sigma)
=\sum_{p\nmid q}\sum_{m\ge1}\frac{\sum_\chi\chi(p)^m}{mp^{m\sigma}}
=\varphi(q)\sum_{\substack{p\nmid q,\ m\ge1\\p^m\equiv1\pmod q}}\frac1{mp^{m\sigma}}\ge0.
$$

Thus $\mathcal F(\sigma)\ge1$. If a nonreal [Dirichlet character](../../../../../dirichlet-character.md) $\chi$ had $L(1,\chi)=0$, its distinct conjugate $\overline\chi$ would also have a [zero](../../../../../zero-of-a-function.md) there, since $L(1,\overline\chi)=\overline{L(1,\chi)}$. These two [zeros](../../../../../zero-of-a-function.md) would outweigh the single [pole](../../../../../pole.md) of the principal factor; all other factors are bounded near one. It would follow that $\mathcal F(\sigma)\to0$ as $\sigma\downarrow1$, contradicting the lower bound. Together with the assumption for real [Dirichlet characters](../../../../../dirichlet-character.md), this proves $L(1,\chi)\ne0$ for every [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md).

The first-degree part of the [Euler product](../../../../../euler-product.md) [logarithm](../../../../../logarithm.md) gives

$$
\log L(\sigma,\chi)=\sum_p\frac{\chi(p)}{p^\sigma}+O(1),\qquad\sigma\downarrow1.
$$

The omitted terms are bounded uniformly, since $\sum_p\sum_{m\ge2}(mp^{m\sigma})^{-1}\ll\sum_p p^{-2}<\infty$. For each nonprincipal factor, its [logarithm](../../../../../logarithm.md) remains bounded: choose a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) near the now established nonzero value $L(1,\chi)$; the Euler-product branch differs from it by a fixed integral multiple of $2\pi i$ on a sufficiently small real interval. For the principal factor,

$$
\log L(\sigma,\chi_0)=\log\frac1{\sigma-1}+O_q(1).
$$

Applying [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) again gives

$$
\varphi(q)\sum_{p\equiv a\,\mathrm{mod}\,q}\frac1{p^\sigma}
=\sum_{\chi\bmod q}\overline{\chi(a)}\log L(\sigma,\chi)+O_q(1)
=\log\frac1{\sigma-1}+O_q(1).
$$

The right side diverges as $\sigma\downarrow1$, so the [arithmetic progression](../../../../../arithmetic-progression.md) contains infinitely many [primes](../../../../../prime-number.md). This proves [Dirichlet's theorem on arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md): **every reduced [residue class](../../../../../residue-class.md) modulo $q$ contains infinitely many [primes](../../../../../prime-number.md)**. The argument also covers $q=1$ and $q=2$, when there need not be a nonreal character.

For the sharper statement about [reciprocal primes in a fixed arithmetic progression](../../../../../reciprocal-primes-in-a-fixed-arithmetic-progression.md), use the given [prime-counting function](../../../../../prime-counting-function.md) asymptotic with $q$ fixed:

$$
\pi(x;q,a)\sim\frac{\operatorname{li}(x)}{\varphi(q)}
\sim\frac{x}{\varphi(q)\log x}.
$$

The second equivalence follows by [integration by parts](../../../../../integration-by-parts.md) in the [logarithmic integral function](../../../../../logarithmic-integral-function.md). [Partial summation](../../../../../abel-s-summation-formula.md) yields

$$
H(x):=\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p
=\frac{\pi(x;q,a)}x+\int_2^x\frac{\pi(t;q,a)}{t^2}\,dt.
$$

For any $\varepsilon>0$, choose a fixed $T$ so large that the relative error in $\pi(t;q,a)$ is at most $\varepsilon$ for $t\ge T$. The initial integral is a constant, while the remaining integral lies between

$$
\frac{1-\varepsilon}{\varphi(q)}\bigl(\log\log x-\log\log T\bigr)
\quad\text{and}\quad
\frac{1+\varepsilon}{\varphi(q)}\bigl(\log\log x-\log\log T\bigr).
$$

The boundary term is $O_q(1/\log x)$. Divide by $\log\log x$, let $x\to\infty$, and then let $\varepsilon\downarrow0$. We obtain

$$
\boxed{\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p
\sim\frac{\log\log x}{\varphi(q)}.}
$$

Only a relative asymptotic is deduced from the given information; an additive $O(1)$ error, or uniformity for a growing modulus $q$, would require additional estimates.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
