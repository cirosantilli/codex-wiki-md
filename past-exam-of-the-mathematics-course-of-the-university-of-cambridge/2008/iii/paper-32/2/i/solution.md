<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $G=\operatorname{Gal}(F/K)$ and fix a [prime ideal](../../../../../../prime-ideal.md) $\mathfrak q$ above $\mathfrak p$. Suppose there is another prime $\mathfrak r$ above $\mathfrak p$ outside the $G$-orbit of $\mathfrak q$. Distinct nonzero [prime ideals](../../../../../../prime-ideal.md) in the [ring of integers](../../../../../../ring-of-integers.md) are distinct [maximal ideals](../../../../../../maximal-ideal.md), hence pairwise comaximal. The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) supplies $a\in\mathcal O_F$ satisfying $a\equiv0\pmod{\mathfrak r}$ and $a\equiv1\pmod{\sigma\mathfrak q}$ for every $\sigma\in G$. Its [field norm](../../../../../../field-norm.md) is

$$
b=N_{F/K}(a)=\prod_{\sigma\in G}\sigma(a)\in\mathcal O_K.
$$

The factor $a$ puts $b$ in $\mathfrak r$, hence in $\mathfrak r\cap\mathcal O_K=\mathfrak p$. But every $\sigma(a)$ is congruent to $1$ modulo $\mathfrak q$, since $a\equiv1\pmod{\sigma^{-1}\mathfrak q}$. Thus $b\equiv1\pmod{\mathfrak q}$, contradicting $b\in\mathfrak p\subset\mathfrak q$. This proves [transitivity of the Galois action on primes](../../../../../../transitivity-of-the-galois-action-on-primes.md) without any unramified hypothesis.

Let $D=\operatorname{Stab}_G(\mathfrak q)$ be the [decomposition group](../../../../../../decomposition-group.md) and $H=\operatorname{Gal}(F/L)$. Transitivity identifies the primes of $F$ above $\mathfrak p$ with the [coset](../../../../../../coset.md) space $G/D$. Two such primes contract to the same prime in $L$ exactly when they are in the same $H$-orbit: apply the transitivity just proved to the [Galois extension](../../../../../../finite-galois-extension.md) $F/L$. Therefore [primes in an intermediate field as double cosets](../../../../../../primes-in-an-intermediate-field-as-double-cosets.md) gives

$$
\boxed{\#\{\mathfrak l\subset\mathcal O_L:\mathfrak l\mid\mathfrak p\}=|H\backslash G/D|=|D\backslash G/H|.}
$$

The second equality follows by inversion of representatives. It allows one to count $D$-orbits on the embeddings of $L$ into $F$, represented by $G/H$. If $H$ is normal, this simplifies to $[G:HD]$; the double-coset formulation also handles nonnormal intermediate fields.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
