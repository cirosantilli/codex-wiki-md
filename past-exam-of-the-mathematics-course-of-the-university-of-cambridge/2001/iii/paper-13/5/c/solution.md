<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose a nontrivial finite [group](../../../../../../group-split.md) acts freely on $\mathbb R^n$ by [homeomorphisms](../../../../../../homeomorphism.md). Choose a nonidentity element of finite order $m$, a prime $p$ dividing $m$, and the power of that element with exponent $m/p$. It has order $p$, so a subgroup $C_p$ also acts freely.

Let $M=\mathbb R^n/C_p$. A finite free action is properly discontinuous: around any point choose mutually disjoint neighborhoods of the finitely many orbit points, then intersect their inverse translates to obtain an evenly covered neighborhood. Thus $M$ is an $n$-[manifold](../../../../../../topological-manifold.md) with [universal cover](../../../../../../universal-cover.md) $\mathbb R^n$, which is contractible. The [group](../../../../../../group-split.md)-[cohomology](../../../../../../cohomology-split.md) argument of Question 2 applies even if no cell structure has been chosen: [singular simplices](../../../../../../singular-simplex.md) in $M$ lift to the cover, their lifts form free deck-[group](../../../../../../group-split.md) orbits, and the augmented [singular chains](../../../../../../singular-chain.md) of the contractible cover form an exact [free resolution](../../../../../../free-resolution.md). Therefore

$$
H^i(M;\mathbb Z)\cong
\operatorname{Ext}_{\mathbb Z[C_p]}^i(\mathbb Z,\mathbb Z).
$$

We calculate the right-hand side explicitly. Write $R=\mathbb Z[C_p]$, let $t$ generate $C_p$, and set $N=1+t+\cdots+t^{p-1}$. The [periodic resolution of a finite cyclic group](../../../../../../periodic-resolution-of-a-finite-cyclic-group.md) is

$$
\cdots\xrightarrow{\,t-1\,}R\xrightarrow{\,N\,}R
\xrightarrow{\,t-1\,}R\xrightarrow{\varepsilon}\mathbb Z\longrightarrow0.
$$

Its exactness can be seen in coefficients. For $r=\sum_{j=0}^{p-1}a_jt^j$, $(t-1)r=0$ exactly when all $a_j$ are equal, giving $\ker(t-1)=\mathbb ZN=\operatorname{im}N$. Also $Nr=\varepsilon(r)N$, so $\ker N=\ker\varepsilon$. If $\varepsilon(r)=0$, then

$$
r=\sum_{j=1}^{p-1}a_j(t^j-1)
=(t-1)\sum_{j=1}^{p-1}a_j(1+t+\cdots+t^{j-1}).
$$

Hence $\ker N=\ker\varepsilon=(t-1)R$, proving exactness everywhere.

Apply $\operatorname{Hom}_R(-,\mathbb Z)$ with the trivial action. Multiplication by $t-1$ induces zero, and multiplication by $N$ induces multiplication by $p$. The [cochain complex](../../../../../../cochain-complex.md) is therefore

$$
\mathbb Z\xrightarrow{0}\mathbb Z\xrightarrow{p}\mathbb Z
\xrightarrow{0}\mathbb Z\xrightarrow{p}\cdots.
$$

Its positive even-degree [cohomology](../../../../../../cohomology-split.md) is

$$
H^{2j}(M;\mathbb Z)\cong\mathbb Z/p\mathbb Z
\quad(j\geq1),
$$

while its positive odd-degree [cohomology](../../../../../../cohomology-split.md) is zero.

This contradicts the dimension of the quotient [manifold](../../../../../../topological-manifold.md). The noncompact form of [Poincaré duality for noncompact manifolds](../../../../../../poincare-duality-for-noncompact-manifolds.md), with the [orientation local system](../../../../../../orientation-local-system.md) when needed, is

$$
H^i(M;\mathbb Z)\cong
H_{n-i}^{\mathrm{BM}}(M;\mathcal O_M).
$$

Here [Borel-Moore homology](../../../../../../borel-moore-homology.md) is the [homology](../../../../../../homology-split.md) of locally finite chains. Its negative-degree chain groups are zero, so $H^i(M;\mathbb Z)=0$ for $i>n$, whether or not $M$ is [orientable](../../../../../../orientable-surface.md). Taking any $2j>n$ contradicts the displayed [cyclic group](../../../../../../cyclic-group.md) calculation. Thus

$$
\boxed{\text{a finite group acting freely on }\mathbb R^n
\text{ must be trivial}.}
$$

This proves [finite groups cannot act freely on Euclidean space](../../../../../../finite-groups-cannot-act-freely-on-euclidean-space.md) for general [homeomorphisms](../../../../../../homeomorphism.md); it does not assume that the action consists of affine maps or isometries.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
