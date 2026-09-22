<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $a=\sqrt[3]{2}$ and $\zeta=\zeta_3$. The polynomial $X^3-2$ is irreducible over $\mathbb Q$ by the [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at $2$, so $[\mathbb Q(a):\mathbb Q]=3$. This field is real and cannot contain the nonreal $\zeta$. Adjoining $\zeta$ gives a quadratic extension and hence $[F:\mathbb Q]=6$. Since $F$ is the [splitting field](../../../../../../splitting-field.md) of $X^3-2$, its [Galois group](../../../../../../galois-group.md) acts faithfully on $a,\zeta a,\zeta^2a$ and has order six. Consequently

$$
\operatorname{Gal}(F/\mathbb Q)\simeq S_3.
$$

For a prime $\mathfrak q$ over a rational prime $p$, its [absolute residue degree](../../../../../../absolute-residue-degree.md) is the order of the cyclic [quotient group](../../../../../../quotient-group.md) $D_{\mathfrak q}/I_{\mathfrak q}$ from part (i). If that degree were six, then $D_{\mathfrak q}$, a subgroup of $S_3$, would have order at least six, so $D_{\mathfrak q}=S_3$ and $I_{\mathfrak q}=1$. This would make $S_3$ cyclic, a contradiction. The argument applies also at ramified primes. Thus

$$
\boxed{\text{No prime of }F\text{ has absolute residue degree }6.}
$$

For the second request printed with the same subpart label, work over $E=\mathbb Q(\zeta)$. The [Galois group](../../../../../../galois-group.md) of $F/E$ is cyclic of order three, with generator $\sigma(a)=\zeta a$ and $\sigma(\zeta)=\zeta$. The [ideal norm](../../../../../../ideal-norm.md) of $(\zeta+3)$ is seven, since

$$
(\zeta+3)(\zeta^2+3)=7.
$$

In its [residue field](../../../../../../residue-field.md) we have $\zeta\equiv-3\equiv4\pmod{\mathfrak p_1}$. The polynomial $X^3-2$ has no root in $\mathbb F_7$, because its cube residues are $0,1,6$. It is therefore irreducible there. Its discriminant $-108$ is a unit at $\mathfrak p_1$. To check the local index condition, the [trace pairing](../../../../../../trace-pairing.md) matrix of $1,a,a^2$ has this unit determinant. For any integral element $b$ of $F$, its traces against these three basis elements are integral; solving with this invertible matrix shows that its basis coefficients are integral locally. Thus the relative [ring of integers](../../../../../../ring-of-integers.md) equals $\mathcal O_E[a]$ at $\mathfrak p_1$. The relative [Kummer-Dedekind theorem](../../../../../../kummer-dedekind-theorem.md) gives one unramified prime above $\mathfrak p_1$, of [residue degree](../../../../../../residue-degree.md) three.

Use [arithmetic Frobenius](../../../../../../frobenius-automorphism.md), characterized by $b\mapsto b^7$ on this [residue field](../../../../../../residue-field.md). As $a^3=2$,

$$
a^7=4a\equiv\zeta a\pmod{\mathfrak q}.
$$

The three possible images $a,\zeta a,\zeta^2a$ remain distinct modulo $\mathfrak q$, since $a$ is nonzero and $1,4,2$ are distinct modulo seven. This congruence therefore identifies the actual automorphism uniquely:

$$
\boxed{\operatorname{Frob}_{\mathfrak p_1}(a)=\zeta_3a,\qquad
\operatorname{Frob}_{\mathfrak p_1}(\zeta_3)=\zeta_3.}
$$

The geometric Frobenius convention would give its inverse. Since $F/E$ is abelian, the arithmetic element is independent of the choice of prime above $\mathfrak p_1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
