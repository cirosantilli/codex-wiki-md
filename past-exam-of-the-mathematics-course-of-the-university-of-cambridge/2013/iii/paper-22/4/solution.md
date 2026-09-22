<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Kummer theory](../../../../../kummer-theory.md) studies extracting roots through Galois actions, and on an [elliptic curve](../../../../../elliptic-curve.md) the corresponding operation is division of points. The bridge is a cocycle: different Galois conjugates of a chosen division point differ by torsion. Controlling the ramification of these cocycles is what proves the [Weak Mordell-Weil theorem](../../../../../weak-mordell-weil-theorem.md).

Classically, for a characteristic-zero field $K$, the sequence

$$
1\longrightarrow\mu_m\longrightarrow\overline K^{\times}\xrightarrow{\ z\mapsto z^m\ }\overline K^{\times}\longrightarrow1
$$

is exact. [Hilbert's theorem 90](../../../../../hilbert-s-theorem-90.md) gives $H^1(K,\overline K^{\times})=0$, so [Galois cohomology](../../../../../galois-cohomology.md) identifies

$$
H^1(K,\mu_m)\cong K^{\times}/(K^{\times})^m.
$$

The class of $a$ is represented by $\sigma\mapsto\sigma(\sqrt[m]{a})/\sqrt[m]{a}$. If $\mu_m\subset K$, the module is constant and these are continuous characters into $\mu_m$; the associated fields are cyclic Kummer extensions of degree dividing $m$. Several such classes give abelian extensions of exponent dividing $m$. Without the roots-of-unity hypothesis the cohomological description still holds, but the action on $\mu_m$ must not be discarded.

For an [elliptic curve](../../../../../elliptic-curve.md) over a [number field](../../../../../number-field.md) $K$, multiplication by $m\ge2$ gives the [exact sequence](../../../../../exact-sequence.md) of Galois modules

$$
0\longrightarrow E[m]\longrightarrow E(\overline K)\xrightarrow{[m]}E(\overline K)\longrightarrow0.
$$

The map is onto because it is a nonconstant isogeny over an algebraically closed field. For $P\in E(K)$ choose $Q\in E(\overline K)$ with $mQ=P$, and set

$$
\delta_m(P)_\sigma=\sigma Q-Q\in E[m].
$$

It satisfies $\delta(P)_{\sigma\tau}=\delta(P)_\sigma+\sigma\delta(P)_\tau$, the [Galois 1-cocycle](../../../../../galois-1-cocycle.md) identity. Changing $Q$ by a [torsion point of an elliptic curve](../../../../../torsion-point-of-an-elliptic-curve.md) changes the cocycle by a coboundary. If the class is zero, a corresponding change of $Q$ makes it Galois-fixed, so $P\in mE(K)$. Conversely a rational division point gives the zero class. Thus the [Kummer map of an elliptic curve](../../../../../kummer-map-of-an-elliptic-curve.md) is injective on the quotient, and the cohomology sequence gives

$$
\boxed{0\longrightarrow E(K)/mE(K)\xrightarrow{\delta_m}H^1(K,E[m])\longrightarrow H^1(K,E)[m]\longrightarrow0.}
$$

This is the [Kummer exact sequence of an elliptic curve](../../../../../kummer-exact-sequence-of-an-elliptic-curve.md). The last group parametrizes the appropriate torsor classes. It is important that the entire middle group need not be finite; an unrestricted Kummer class can ramify at arbitrarily many primes.

The [Weak Mordell-Weil theorem](../../../../../weak-mordell-weil-theorem.md) states **$E(K)/mE(K)$ is finite for every [number field](../../../../../number-field.md) $K$ and every $m\ge1$**. The case $m=1$ is trivial. To prove the remaining cases, choose a finite set $S$ containing the primes of bad reduction and the primes dividing $m$. At a prime outside $S$, the [elliptic curve](../../../../../elliptic-curve.md) extends to a smooth proper [group scheme](../../../../../group-scheme.md) over the valuation ring, and $[m]$ is finite étale. Properness extends a local [rational point](../../../../../rational-point.md) to a section; its division fibre is a finite étale torsor over that ring. Therefore its Kummer class is unramified. This is [unramified division torsors at good primes](../../../../../unramified-division-torsors-at-good-primes.md), and shows that $\delta_m(E(K))$ lies in [first Galois cohomology unramified outside a finite set](../../../../../first-galois-cohomology-unramified-outside-a-finite-set.md).

Let $L=K(E[m])$, enlarged if necessary to contain $\mu_m$, and include in $S$ the finitely many primes ramified in $L/K$. This is a finite Galois extension. Over $L$ the torsion module is constant, isomorphic to $(\mathbb Z/m\mathbb Z)^2$, and so to two copies of $\mu_m$. Restricting a cocycle to $G_L$ therefore reduces it to two classical Kummer classes unramified outside the primes above $S$. Such a class is represented by $a\in L^{\times}$ satisfying

$$
v_{\mathfrak p}(a)\equiv0\pmod m\qquad(\mathfrak p\notin S_L).
$$

Write this power-class group as $L(S_L,m)$. The implication follows locally because, away from residue characteristic dividing $m$, the valuation of an unramified $m$th-root extension must be divisible by $m$.

Its finiteness comes from two standard arithmetic finiteness results, rather than from an assertion that all of $L^{\times}/(L^{\times})^m$ is finite. The valuations outside $S_L$ associate to $a$ an ideal whose $m$th power is principal. There is an [exact sequence](../../../../../exact-sequence.md)

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/(\mathcal O_{L,S_L}^{\times})^m\longrightarrow L(S_L,m)\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[m]\longrightarrow0.
$$

The left group is finite by the finite generation of the [S-unit group](../../../../../s-unit-group.md), and the right group is finite by [finiteness of the ideal class group](../../../../../finiteness-of-the-ideal-class-group.md). This proves [finiteness of S-unramified Kummer classes](../../../../../finiteness-of-s-unramified-kummer-classes.md). Hence there are only finitely many restricted cocycles over $L$. The kernel of restriction from $K$ is contained in $H^1(\operatorname{Gal}(L/K),E[m])$, which is finite because both group and module are finite. The restricted cohomology group over $K$ is therefore finite, and its injected subgroup $E(K)/mE(K)$ is finite too. This completes a [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../../../kummer-theoretic-proof-of-the-weak-mordell-weil-theorem.md).

For arithmetic computation one adds local conditions. The [Selmer group of an elliptic curve](../../../../../n-selmer-group.md) consists of classes in $H^1(K,E[m])$ whose restriction at every completion $K_v$ lies in the image of the corresponding local Kummer map. They are unramified outside the same finite set, so this group is finite. The failure of a everywhere locally soluble torsor to have a global point is measured by the [Tate–Shafarevich group](../../../../../tate-shafarevich-group.md), defined as the kernel of the local restriction map on $H^1(K,E)$. The resulting [exact sequence](../../../../../exact-sequence.md) is

$$
0\longrightarrow E(K)/mE(K)\longrightarrow\operatorname{Sel}^{(m)}(E/K)\longrightarrow\operatorname{Sha}(E/K)[m]\longrightarrow0.
$$

Thus the [Selmer group of an elliptic curve](../../../../../n-selmer-group.md) gives a computable upper bound for the quotient; actual [rational points](../../../../../rational-point.md) supply lower bounds. Equality need not follow just from local solubility. Finiteness of this fixed torsion subgroup does not prove finiteness of the whole [Tate–Shafarevich group](../../../../../tate-shafarevich-group.md).

Finally, weak finiteness alone is not finite generation: the additive group $\mathbb Q$ has trivial quotients by multiplication and is not finitely generated. The additional ingredient for the [Mordell-Weil theorem](../../../../../mordell-weil-group.md) is [height descent](../../../../../height-descent-lemma.md). Choose representatives $P_i$ of $E(K)/mE(K)$ and write $P=P_i+mQ$. The quadratic growth of the [canonical height of an elliptic curve](../../../../../canonical-height-of-an-elliptic-curve.md), together with bounds for translation by the finitely many $P_i$, makes $Q$ have smaller height whenever $P$ is sufficiently large. [Northcott theorem](../../../../../northcott-theorem.md) gives only finitely many points of bounded height, and repeated descent yields a finite generating set. This explains the roles of [Kummer theory](../../../../../kummer-theory.md), local information and heights without conflating the weak and full theorems.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
