<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md), choose a prime $\ell$ with

$$
\ell\equiv1\pmod r.
$$

The [cyclotomic field](../../../../../../cyclotomic-field.md) $E=\mathbb Q(\zeta_\ell)$ is Galois over $\mathbb Q$, and

$$
\operatorname{Gal}(E/\mathbb Q)
\cong(\mathbb Z/\ell\mathbb Z)^\times
\cong C_{\ell-1},
$$

where the last group is cyclic because the multiplicative group of a finite field is cyclic.

The cyclic group $C_{\ell-1}$ has a unique subgroup $H$ of order $(\ell-1)/r$. By the [Galois correspondence](../../../../../../galois-correspondence.md), its fixed field $L=E^H$ satisfies

$$
\operatorname{Gal}(L/\mathbb Q)
\cong \operatorname{Gal}(E/\mathbb Q)/H
\cong C_r.
$$

Normality follows because $H$ lies in an abelian group. Thus every $r>1$ occurs as the Galois group of a finite extension of $\mathbb Q$. This is the [cyclic Galois extension of the rational numbers of every finite degree](../../../../../../cyclic-galois-extension-of-the-rational-numbers-of-every-finite-degree.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
