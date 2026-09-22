<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $Q=G/H$ and write $M^H$ for the [invariant submodule](../../../../../invariant-submodule.md). The [five-term exact sequence in group cohomology](../../../../../five-term-exact-sequence-in-group-cohomology.md) associated with the [Lyndon–Hochschild–Serre spectral sequence](../../../../../lyndon-hochschild-serre-spectral-sequence.md) is

$$
0\longrightarrow H^1(Q,M^H)
\xrightarrow{\operatorname{inf}}H^1(G,M)
\xrightarrow{\operatorname{res}}H^1(H,M)^Q
\xrightarrow{d_2}H^2(Q,M^H)
\xrightarrow{\operatorname{inf}}H^2(G,M).
$$

The [inflation map in group cohomology](../../../../../inflation-map-in-group-cohomology.md) composes a cocycle on $Q$ with the quotient homomorphism $G\to Q$. The [restriction map in group cohomology](../../../../../restriction-map-in-group-cohomology.md) restricts a cocycle from $G$ to $H$. The quotient action on the middle term is, for $q=gH$ and a [one-cocycle](../../../../../one-cocycle.md) $f$,

$$
q\cdot[f]=\left[h\longmapsto g\cdot f(g^{-1}hg)\right].
$$

This is independent of the lift and of the representative at the level of [cohomology](../../../../../cohomology-split.md). Finally, the [transgression in group cohomology](../../../../../transgression-in-group-cohomology.md) extends a $Q$-invariant class on $H$ to a one-cochain on $G$; its coboundary is $H$-basic and descends to the two-cocycle on $Q$ representing $d_2[f]$. Changing the extension changes that cocycle by a [group coboundary](../../../../../group-coboundary.md).

For the application, choose free generators $x_1,\ldots,x_n$ of $F$ and normal generators $r_1,\ldots,r_n$ of $R$. Since a [finite nonabelian simple group](../../../../../finite-nonabelian-simple-group.md) $K$ is a [perfect group](../../../../../perfect-group.md), its abelianization is zero. The five-term sequence for $1\to R\to F\to K\to1$ with trivial coefficients contains

$$
0\longrightarrow\operatorname{Hom}(K,\mathbb Z)
\longrightarrow\operatorname{Hom}(F,\mathbb Z)
\xrightarrow{\operatorname{res}}\operatorname{Hom}(R,\mathbb Z)^K
\longrightarrow H^2(K,\mathbb Z)
\longrightarrow H^2(F,\mathbb Z).
$$

The first term is zero because $K$ is finite, and the last term is zero because a [free group](../../../../../free-group.md) has cohomological dimension one. It remains to prove that restriction is surjective.

The [invariant submodule](../../../../../invariant-submodule.md) of homomorphisms $R\to\mathbb Z$ is exactly

$$
\operatorname{Hom}(R/[F,R],\mathbb Z).
$$

The images of the relators $r_1,\ldots,r_n$ generate $R/[F,R]$, so such a homomorphism $\lambda$ is determined by the integer vector $b=(\lambda(r_1),\ldots,\lambda(r_n))^T$. Let $A$ be the [relator exponent-sum matrix](../../../../../relator-exponent-sum-matrix.md). This square integer matrix presents $K^{\mathrm{ab}}$, which is zero, so $A$ is a [unimodular matrix](../../../../../unimodular-matrix.md). There is therefore an integer vector $v$ satisfying $Av=b$. Define $\psi:F\to\mathbb Z$ by assigning to $x_i$ the $i$th entry of $v$. The definition of $A$ gives $\psi(r_j)=\lambda(r_j)$ for every $j$. Since the relator images generate $R/[F,R]$, the restriction of $\psi$ to $R$ equals $\lambda$. Restriction is surjective, exactness now gives

$$
\boxed{H^2(K,\mathbb Z)=0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
