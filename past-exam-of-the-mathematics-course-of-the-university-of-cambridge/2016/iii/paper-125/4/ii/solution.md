<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Galois cohomology](../../../../../../galois-cohomology.md) records the obstruction to choosing Galois-invariant division points. Let $G_K=\operatorname{Gal}(\overline K/K)$ be the [absolute Galois group](../../../../../../absolute-galois-group.md) and give its algebraic-point modules the discrete topology. A continuous $1$-cocycle with values in a [Galois module](../../../../../../galois-module.md) $M$ is a function $c:G_K\to M$ satisfying

$$
c_{\sigma\tau}=c_\sigma+\sigma c_\tau.
$$

A [group coboundary](../../../../../../group-coboundary.md) has the form $c_\sigma=\sigma a-a$. Quotienting cocycles by coboundaries defines $H^1(K,M)$. For the finite module $E[m]$ these cocycles have finite image and factor through finite data; continuity is essential because $G_K$ is a [profinite group](../../../../../../profinite-group.md).

In characteristic zero, multiplication by $m\geq2$ on the algebraic points of an [elliptic curve](../../../../../../elliptic-curve.md) is surjective, with kernel $E[m]\cong(\mathbb Z/m\mathbb Z)^2$. The short exact sequence of Galois modules

$$
0\longrightarrow E[m]\longrightarrow E(\overline K)\xrightarrow{[m]}E(\overline K)\longrightarrow0
$$

gives the [Kummer exact sequence of an elliptic curve](../../../../../../kummer-exact-sequence-of-an-elliptic-curve.md)

$$
\boxed{0\longrightarrow E(K)/mE(K)\xrightarrow{\delta}H^1(K,E[m])\longrightarrow H^1(K,E)[m]\longrightarrow0.}
$$

Explicitly, choose $Q$ with $mQ=P$ and set $\delta(P)_\sigma=\sigma Q-Q$. Changing $Q$ by an $m$-torsion point changes the cocycle by a coboundary. The class vanishes exactly when a suitable choice of $Q$ is Galois-fixed, that is, when $P\in mE(K)$. This proves the injection directly and identifies its arithmetic meaning.

The entire group $H^1(K,E[m])$ need not be finite. For example, [Kummer theory](../../../../../../kummer-theory.md) gives $H^1(K,\mu_m)=K^*/K^{*m}$, which has classes supported on arbitrarily many different primes. The finite part needed for the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) comes from a ramification restriction on the image of $\delta$.

Choose a finite set $S$ of places containing the archimedean places, the primes dividing $m$ and all primes of [bad reduction of an elliptic curve](../../../../../../bad-reduction-of-an-elliptic-curve.md). At a finite place $v\notin S$, the curve has good reduction and $m$ is invertible in its valuation ring. The elliptic curve extends to a smooth proper group scheme, and $[m]$ on that model is finite etale. A point $P\in E(K_v)$ extends to an integral section by properness. Its division-point fibre is consequently finite etale over the valuation ring. Over the maximal unramified extension it has a point, so the Kummer cocycle restricts trivially to the [inertia group](../../../../../../inertia-group.md). The module $E[m]$ itself is unramified there for the same reason. Thus

$$
\delta(E(K)/mE(K))\subseteq H^1_S(K,E[m]),
$$

where $H^1_S$ denotes classes unramified outside $S$.

Here is a proof that this restricted group is finite. Take a finite Galois extension $L/K$ containing all coordinates of $E[m]$ and the $m$th roots of unity, and enlarge $S$ by its ramified primes. Over $L$ the module is trivial and, after choosing a basis, is isomorphic to $\mu_m^2$. [Hilbert theorem 90](../../../../../../hilbert-s-theorem-90.md) and the multiplicative Kummer sequence therefore give

$$
H^1(L,E[m])\cong(L^*/L^{*m})^2.
$$

For [unramified Kummer classes with bounded prime support](../../../../../../unramified-kummer-classes-with-bounded-prime-support.md), a class unramified outside $S_L$ has valuations divisible by $m$ at every prime outside $S_L$: the valuation of an $m$th root in an unramified extension is integral. Consequently both coordinates lie in

$$
L(S_L,m)=\{[a]\in L^*/L^{*m}:v_{\mathfrak p}(a)\equiv0\pmod m\text{ for }\mathfrak p\notin S_L\}.
$$

To show this set finite, write the outside-$S_L$ divisor of $a$ as $mD$. The ideal class of $D$ belongs to the $m$-torsion of the [ideal class group](../../../../../../ideal-class-group.md) of the ring of $S_L$-integers. This gives the exact sequence

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/(\mathcal O_{L,S_L}^{\times})^m
\longrightarrow L(S_L,m)
\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[m]
\longrightarrow0.
$$

The last map is onto: if $mD$ is principal in the $S_L$-ideal group, a generator represents a class with outside valuations divisible by $m$. The kernel consists exactly of [S-units](../../../../../../s-unit.md) modulo $m$th powers. The [Dirichlet unit theorem](../../../../../../dirichlet-s-unit-theorem.md), with the finitely many inverted primes adjoined, makes the [S-unit group](../../../../../../s-unit-group.md) finitely generated; the [ideal class group](../../../../../../ideal-class-group.md) is finite, and localization only quotients it. Both ends of the sequence are therefore finite.

Finally, the [inflation-restriction exact sequence](../../../../../../inflation-restriction-exact-sequence.md) bounds the kernel of restriction from $H^1(K,E[m])$ to $H^1(L,E[m])$ by the finite group $H^1(\operatorname{Gal}(L/K),E[m])$. The unramified subgroup has finite image, contained in $L(S_L,m)^2$, and finite kernel, so it is finite. The Kummer injection now proves

$$
\boxed{E(K)/mE(K)\text{ is finite for every }m\geq2.}
$$

This is the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md), proved without first assuming finite generation of $E(K)$.

For computation one refines the unramified group by local solvability. The [Selmer group of an elliptic curve](../../../../../../n-selmer-group.md) consists of classes whose restriction at every completion lies in the corresponding local Kummer image. It is finite and sits in

$$
0\longrightarrow E(K)/mE(K)\longrightarrow\operatorname{Sel}_m(E/K)\longrightarrow\operatorname{Sha}(E/K)[m]\longrightarrow0,
$$

where the [Tate–Shafarevich group](../../../../../../tate-shafarevich-group.md) $\operatorname{Sha}$ measures classes in $H^1(K,E)$ that become trivial at every completion. Thus locally soluble descent equations can give an upper bound without every class coming from a rational point. No finiteness assumption on the whole Tate-Shafarevich group is needed for the weak theorem. Combining the finite quotient with the [height descent lemma](../../../../../../height-descent-lemma.md) from the height essay yields the full [Mordell-Weil theorem](../../../../../../mordell-weil-group.md). Replacing multiplication by $m$ with a smaller isogeny gives the same cohomological framework for [two-isogeny descent](../../../../../../two-isogeny-descent.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
