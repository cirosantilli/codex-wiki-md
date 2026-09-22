# Group cohomology

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_cohomology)

Group cohomology studies a [group](group.md) through cochain complexes built from its actions on abelian groups. In degree one, $H^1(G,M)$ identifies one-cocycles $c:G\to M$ modulo one-coboundaries.

**Table of contents**

- [Cellular free resolution from a contractible universal cover](#cellular-free-resolution-from-a-contractible-universal-cover)
- [Integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group)
  - [Stallings-Swan theorem](#stallings-swan-theorem)
- [Poincare duality group](#poincare-duality-group)
  - [Normal finitely presented subgroups of three-dimensional duality groups](#normal-finitely-presented-subgroups-of-three-dimensional-duality-groups)
  - [Classification of two-dimensional Poincare duality groups](#classification-of-two-dimensional-poincare-duality-groups)
  - [Strebel infinite-index subgroup theorem](#strebel-infinite-index-subgroup-theorem)
  - [Extension rule for Poincare duality groups](#extension-rule-for-poincare-duality-groups)
  - [Finite-index invariance of Poincare duality for torsion-free groups](#finite-index-invariance-of-poincare-duality-for-torsion-free-groups)
- [Mod-p cohomology ring of a cyclic group](#mod-p-cohomology-ring-of-a-cyclic-group)
- [Dimension shifting in group cohomology](#dimension-shifting-in-group-cohomology)
- [Tate cohomology of a finite group](#tate-cohomology-of-a-finite-group)
- [Continuous cochains with topological coefficients](#continuous-cochains-with-topological-coefficients)
- [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)
  - [Cyclic cohomology of a regular lattice](#cyclic-cohomology-of-a-regular-lattice)
  - [Herbrand quotient](#herbrand-quotient)
    - [Herbrand quotient of a finite module](#herbrand-quotient-of-a-finite-module)
    - [Herbrand quotient of the local multiplicative group](#herbrand-quotient-of-the-local-multiplicative-group)
- [Corestriction map in group cohomology](#corestriction-map-in-group-cohomology)
- [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)
  - [Cohomology continuity at closed subgroups](#cohomology-continuity-at-closed-subgroups)
  - [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)
    - [Trivial coefficients detect the cohomological dimension of a pro-p group](#trivial-coefficients-detect-the-cohomological-dimension-of-a-pro-p-group)
    - [Characteristic p Galois dimension bound](#characteristic-p-galois-dimension-bound)
- [Nonabelian first cohomology](#nonabelian-first-cohomology)
- [Periodic group cohomology](#periodic-group-cohomology)
  - [Cohomology ring of a finite cyclic group over its prime field](#cohomology-ring-of-a-finite-cyclic-group-over-its-prime-field)
  - [Periodic group cohomology from a free sphere action](#periodic-group-cohomology-from-a-free-sphere-action)
- [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)
  - [Group cohomology commutes with finite direct sums](#group-cohomology-commutes-with-finite-direct-sums)
  - [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group)
    - [Second cohomology of a rank-two free abelian group with truncated group-ring coefficients](#second-cohomology-of-a-rank-two-free-abelian-group-with-truncated-group-ring-coefficients)
- [Coinduced module](#coinduced-module)
  - [Shapiro's lemma](#shapiro-s-lemma)
    - [Hom functor adjunction for a coinduced module](#hom-functor-adjunction-for-a-coinduced-module)
- [Conjugation module of a group ring](#conjugation-module-of-a-group-ring)
  - [Group cohomology of a conjugation module](#group-cohomology-of-a-conjugation-module)
- [Integral cohomology of a finite cyclic group](#integral-cohomology-of-a-finite-cyclic-group)
  - [Periodic resolution of a finite cyclic group](#periodic-resolution-of-a-finite-cyclic-group)
- [Group extension](#group-extension)
  - [Torsion-free finite extension of a lattice](#torsion-free-finite-extension-of-a-lattice)
  - [Split group extension](#split-group-extension)
    - [Section normal form for a split group extension](#section-normal-form-for-a-split-group-extension)
  - [Equivalent group extensions](#equivalent-group-extensions)
  - [Fiber product of groups](#fiber-product-of-groups)
    - [Mihailova subgroup](#mihailova-subgroup)
  - [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)
    - [Integral central extensions of a rank-two free abelian group](#integral-central-extensions-of-a-rank-two-free-abelian-group)
    - [Extension cocycle](#extension-cocycle)
- [Group cocycle](#group-cocycle)
  - [One-cocycle](#one-cocycle)
    - [Galois 1-cocycle](#galois-1-cocycle)
    - [Crossed homomorphism](#crossed-homomorphism)
      - [Principal crossed homomorphism](#principal-crossed-homomorphism)
  - [Two-cocycle](#two-cocycle)
    - [Normalized two-cocycle](#normalized-two-cocycle)
- [Group coboundary](#group-coboundary)
- [Group cochain](#group-cochain)
- [Long exact sequence in group cohomology](#long-exact-sequence-in-group-cohomology)
- [Finite-group cohomology is annihilated by the group order](#finite-group-cohomology-is-annihilated-by-the-group-order)
  - [Restriction-corestriction identity in group cohomology](#restriction-corestriction-identity-in-group-cohomology)
- [Mac Lane exact sequence for a free presentation](#mac-lane-exact-sequence-for-a-free-presentation)
- [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)
  - [Cyclic-extension shift of group-ring cohomology](#cyclic-extension-shift-of-group-ring-cohomology)
  - [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)
    - [Inflation-restriction exact sequence](#inflation-restriction-exact-sequence)
    - [Inflation map in group cohomology](#inflation-map-in-group-cohomology)
    - [Restriction map in group cohomology](#restriction-map-in-group-cohomology)
    - [Transgression in group cohomology](#transgression-in-group-cohomology)
  - [Integral cohomology of the dihedral group of order ten](#integral-cohomology-of-the-dihedral-group-of-order-ten)

## Cellular free resolution from a contractible universal cover

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a connected [CW complex](algebraic-topology.md#cw-complex) $X$ with contractible [universal cover](algebraic-topology.md#universal-cover), let $\Gamma=\pi_1(X)$ and $R=\mathbb Z\Gamma$. Lift each cell once and transport its orientation by [deck transformations](algebraic-topology.md#deck-transformation). Its translates form an $R$-basis of the cellular chains of the cover. The augmentation sends every vertex to one, and contractibility makes the augmented chain complex an exact [free resolution](homological-algebra.md#free-resolution) of the trivial module $\mathbb Z$. An $R$-linear cochain with trivial coefficient action is constant on each orbit of lifts, identifying $\operatorname{Hom}_R(C_*(\widetilde X),\mathbb Z)$ with the [cellular cohomology](homology.md#cellular-cohomology) complex of $X$. Consequently $H^i(X;\mathbb Z)=\operatorname{Ext}_R^i(\mathbb Z,\mathbb Z)$. The same argument with singular simplex lifts works for spaces with a contractible universal cover.

## Integral cohomological dimension of a group

↑ **Parent:** [Group cohomology](group-cohomology.md)

The integral cohomological dimension is the least length of a [projective resolution](homological-algebra.md#projective-resolution) of the trivial [group ring](commutative-algebra.md#group-ring) module $\mathbb Z$, equivalently the largest degree in which [group cohomology](group-cohomology.md) with some module can be nonzero. A group containing torsion has infinite integral cohomological dimension. For $\mathbb Z^r$ the dimension is $r$, realized by its [torus](topological-surface.md#torus) classifying space and detected by its top cohomology.

### Stallings-Swan theorem

↑ **Parent:** [Integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group)

A group has integral [cohomological dimension](#integral-cohomological-dimension-of-a-group) at most one precisely when it is a [free group](geometric-group-theory.md#free-group), including the trivial free group in dimension zero. This result concerns integral coefficients; a rational dimension-one statement has different conclusions.

## Poincare duality group

↑ **Parent:** [Group cohomology](group-cohomology.md)

A Poincare duality group of dimension $n$ has a finite-length resolution of the trivial [group ring](commutative-algebra.md#group-ring) module $\mathbb Z$ by [finitely generated projective modules](module-theory.md#finite-projective-module), and $H^k(G,\mathbb ZG)$ vanishes except in degree $n$, where it is infinite cyclic as an abelian group. The top module $D$ can have an orientation-sign action. Reversing the dual projective resolution gives $H^k(G,V)\cong\operatorname{Tor}^{\mathbb ZG}_{n-k}(D,V)$, equivalently $H_{n-k}(G,D\otimes V)$ with the appropriate diagonal action. Untwisted duality requires trivial orientation action. In positive dimension $H^0(G,\mathbb ZG)=0$, since a finitely supported invariant element cannot exist for an infinite group.

### Normal finitely presented subgroups of three-dimensional duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

Let $N$ be a normal [finitely presented group](geometric-group-theory.md#finitely-presented-group) inside a dimension-three [Poincare duality group](#poincare-duality-group) $G$, with $G/N$ containing an element of infinite order. Then $N$ is either a [free group](geometric-group-theory.md#free-group) or a dimension-two [Poincare duality group](#poincare-duality-group). The [Strebel infinite-index subgroup theorem](#strebel-infinite-index-subgroup-theorem) gives $\operatorname{cd}N\leq2$. If the dimension is two, take the preimage of an infinite cyclic subgroup of the quotient. The [cyclic-extension shift of group-ring cohomology](#cyclic-extension-shift-of-group-ring-cohomology) gives dimension three, forcing this preimage to have finite index by Strebel. Its duality then gives $H^*(N;\mathbb ZN)$ concentrated in degree two with top group $\mathbb Z$. The quotient is virtually cyclic, and surface automorphism realization gives a finite-index surface mapping-torus group.

### Classification of two-dimensional Poincare duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

Every integral dimension-two [Poincare duality group](#poincare-duality-group) is the [fundamental group](algebraic-topology.md#fundamental-group) of a closed aspherical [topological surface](topological-surface.md). Orientable examples are the torus and closed surfaces of genus at least two. Nonorientable aspherical closed surfaces supply the orientation-twisted examples.

### Strebel infinite-index subgroup theorem

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

An infinite-index subgroup of an integral dimension-$d$ [Poincare duality group](#poincare-duality-group) has integral [cohomological dimension](#integral-cohomological-dimension-of-a-group) at most $d-1$. No finiteness assumption on the subgroup is needed for this inequality. In dimension three it places every infinite-index subgroup in cohomological dimension at most two.

### Extension rule for Poincare duality groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

For an extension with kernel a dimension-$n$ [Poincare duality group](#poincare-duality-group) and quotient a dimension-$q$ [Poincare duality group](#poincare-duality-group), apply the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) to the ambient group ring. Kernel cohomology is concentrated in degree $n$ and is a regular quotient module with a rank-one orientation twist. Quotient cohomology is then concentrated in degree $q$ with underlying group $\mathbb Z$. The extension resolution supplies finiteness and gives cohomological dimension at most $n+q$, proving duality in that dimension. Orientation actions need not be trivial.

### Finite-index invariance of Poincare duality for torsion-free groups

↑ **Parent:** [Poincare duality group](#poincare-duality-group)

For a [torsion-free group](group.md#torsion-free-group) $G$ and [finite-index subgroup](group.md#finite-index-subgroup) $H$, $G$ is a [Poincare duality group](#poincare-duality-group) of dimension $n$ if and only if $H$ is. Finite-index induction and coinduction of $\mathbb ZH$ coincide and give $\mathbb ZG$, so [Shapiro's lemma](#shapiro-s-lemma) identifies their group-ring cohomology as abelian groups. The finite-index finiteness and cohomological-dimension lemmas supply finite projective resolutions. Without torsion-freeness of $G$ the converse fails: $\mathbb Z\times C_2$ contains the index-two $PD^1$ subgroup $\mathbb Z$ but has infinite integral cohomological dimension.

## Mod-p cohomology ring of a cyclic group

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a prime $p$, a classifying [Eilenberg–MacLane space](homotopy.md#eilenberg-maclane-space) for $C_p$ is the infinite lens space $S^\infty/C_p$, using scalar multiplication by a primitive $p$th root on the complex-coordinate sphere. Its contractible [universal cover](algebraic-topology.md#universal-cover) is $S^\infty$. The standard two-periodic free resolution has differentials $g-1$ and $1+g+\cdots+g^{p-1}$, both zero after applying [cochains](cohomology.md#singular-cochain) with trivial $\mathbb F_p$ coefficients. Thus every [cohomology](cohomology.md) degree has dimension one. If $p=2$, the ring is $\mathbb F_2[t]$, $|t|=1$. If $p$ is odd, it is $\Lambda(a)\otimes\mathbb F_p[b]$, with $|a|=1$, $|b|=2$: graded commutativity gives $a^2=0$ and the periodicity class $b$ induces the degree-two isomorphisms. The [Künneth theorem](cohomology.md#kunneth-theorem) gives two copies of these generators for $C_p\times C_p$; the dimension in degree $d$ is $d+1$ for every $p$.

## Dimension shifting in group cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

Embed a [module](module-theory.md#module-mathematics) $M$ over the [group ring](commutative-algebra.md#group-ring) $\mathbb Z[G]$ in a module $I$ with vanishing positive [group cohomology](group-cohomology.md), and write $M'=I/M$. The connecting map in the long exact [group cohomology](group-cohomology.md) sequence of $0\to M\to I\to M'\to0$ is an isomorphism $H^r(G,M')\to H^{r+1}(G,M)$ for $r\geq1$, since the groups involving $I$ on both sides vanish. For a finite [group](group.md) and a module $I$ with vanishing [Tate cohomology of a finite group](#tate-cohomology-of-a-finite-group) in every degree, the same argument shifts every Tate degree. Repeating this construction transports computations to a convenient resolution.

## Tate cohomology of a finite group

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a finite [group](group.md) $G$, Tate cohomology joins [group cohomology](group-cohomology.md) and [group homology](group-theory.md#group-homology) through the norm map $N_G=\sum_{g\in G}g$. For $r\geq1$ it equals ordinary [group cohomology](group-cohomology.md); for $r\leq-2$ it equals $H_{-r-1}(G,M)$. The middle terms are $\widehat H^0(G,M)=M^G/N_GM$ and $\widehat H^{-1}(G,M)=\ker(N_G)/I_GM$, where $I_GM$ is generated by $gm-m$. For the trivial module $\mathbb Z$, $\widehat H^{-2}(G,\mathbb Z)=G^{\mathrm{ab}}$. With multiplicative coefficients the norm is the product of the translates.

## Continuous cochains with topological coefficients

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a [topological group module](module-theory.md#topological-group-module), use continuous maps with pointwise addition and the inhomogeneous group-cohomology differential. The kernel modulo the image defines continuous [group cohomology](group-cohomology.md) as an abelian group. With general topological coefficients the quotient topology need not be Hausdorff; the cohomology here is the algebraic quotient of continuous cocycles by continuous coboundaries. With trivial discrete coefficients in a [prime field](algebra.md#prime-field), its first cohomology is the space of continuous [group homomorphisms](group-theory.md#group-homomorphism) to that field's additive group.

## Tate cohomology of a cyclic group

↑ **Parent:** [Group cohomology](group-cohomology.md)

For $G=\langle\sigma\rangle$, set $D=\sigma-1$ and $N=\sum_{g\in G}g$. The two periodic groups are $M^G/NM$ and $\ker N/DM$. A short exact sequence of modules gives a six-term periodic exact sequence. For multiplicative modules the norm operator is a product and $D(x)=\sigma(x)/x$.

### Cyclic cohomology of a regular lattice

↑ **Parent:** [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)

Let $G$ be cyclic and let $R[G]$ carry the regular [permutation action](group-action.md). Invariants are constant coefficient vectors, which are the images of the norm operator. A vector with coefficient sum zero is the difference of a vector and its cyclic translate, by successively solving the coordinate differences. Thus the norm [group kernel](group-theory.md#kernel-of-a-group-homomorphism) equals $(\sigma-1)R[G]$. Both cyclic [Tate cohomology](#tate-cohomology-of-a-finite-group) [groups](group.md) vanish. This applies to $R=\mathbb Z$ and $R=\mathbb Z_p$, and to finite [direct sums](vector-space.md#direct-sum) of regular lattices.

### Herbrand quotient

↑ **Parent:** [Tate cohomology of a cyclic group](#tate-cohomology-of-a-cyclic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Herbrand_quotient)

When the two indicated groups are finite, their size ratio is multiplicative on short exact sequences. It is one for finite modules and therefore unchanged by finite-index modifications. A trivial integral module $\mathbb Z$ has quotient $|G|$, while an induced regular lattice $\mathbb Z_p[G]$ has both Tate groups zero and quotient one. These facts permit norm-index calculations without explicitly finding every norm.

#### Herbrand quotient of a finite module

↑ **Parent:** [Herbrand quotient](#herbrand-quotient)

For a finite [module](module-theory.md#module-mathematics) acted on by a cyclic [group](group.md), write $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The two [Tate cohomology](#tate-cohomology-of-a-finite-group) [group](group.md) sizes are $|\ker D|/|NM|$ and $|\ker N|/|DM|$. The equalities $|NM|=|M|/|\ker N|$ and $|DM|=|M|/|\ker D|$ show that these sizes are equal. The exact-sequence multiplication rule for the [Herbrand quotient](#herbrand-quotient) consequently makes it unchanged by finite-index modifications of lattices.

#### Herbrand quotient of the local multiplicative group

↑ **Parent:** [Herbrand quotient](#herbrand-quotient)

For a cyclic extension of [p-adic fields](non-archimedean-analysis.md#p-adic-field), sufficiently deep [principal units](non-archimedean-analysis.md#principal-unit) are equivariantly isomorphic to an additive lattice by the [p-adic logarithm](non-archimedean-analysis.md#p-adic-logarithm). The [normal basis theorem](galois-theory.md#normal-basis-theorem) makes its [Herbrand quotient](#herbrand-quotient) one. Passing across finite unit quotients preserves it. The valuation exact sequence with quotient $\mathbb Z$ therefore gives the displayed formula.

## Corestriction map in group cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

For an open finite-index subgroup $U$ of a [profinite group](topological-group.md#profinite-group) $G$ and a discrete $G$-module $M$, cohomological transfer gives $\operatorname{Cor}_U^G:H^q(U,M)\to H^q(G,M)$. In degree zero it is the sum over cosets, or the norm for multiplicative coefficients. It is transitive and satisfies $\operatorname{Cor}\operatorname{Res}=[G:U]$ and the cup-product projection formula.

## Continuous cohomology of a profinite group

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a [profinite group](topological-group.md#profinite-group) and a discrete module with continuous action, continuous cohomology is computed by continuous cochains. On a compact domain these cochains have finite image. Positive-degree classes become zero on a sufficiently small open subgroup and hence are torsion by restriction followed by corestriction.

### Cohomology continuity at closed subgroups

↑ **Parent:** [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)

For a closed subgroup $P$ of a [profinite group](topological-group.md#profinite-group) $G$ and a discrete $G$-module $M$, restriction gives $H^q(P,M)=\varinjlim_{U\supseteq P,\ U\ \mathrm{open}}H^q(U,M)$. Thus a class restricting to zero on $P$ already restricts to zero on one such open subgroup. The property follows by extending continuous finite-image cochains and their identities to a sufficiently small open neighborhood of $P$.

### Cohomological dimension at a prime

↑ **Parent:** [Continuous cohomology of a profinite group](#continuous-cohomology-of-a-profinite-group)

The value $\operatorname{cd}_p(G)$ is the least $n$ such that all cohomology in degrees greater than $n$ vanishes for every discrete $p$-primary torsion module. Vanishing in degree $n+1$ for all such modules suffices by dimension shifting. Dimension does not increase on closed subgroups. For a field, use its [absolute Galois group](galois-theory.md#absolute-galois-group).

#### Trivial coefficients detect the cohomological dimension of a pro-p group

↑ **Parent:** [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)

For a [pro-p group](topological-group.md#pro-p-group) $P$, vanishing of $H^{n+1}(P,\mathbb F_p)$ implies vanishing in that degree for every discrete $p$-primary module. Finite such modules have composition factors equal to the trivial module $\mathbb F_p$, so the long exact sequence gives the result by induction. General modules are unions of finite stable submodules, and continuous cohomology commutes with filtered unions. Dimension shifting gives $\operatorname{cd}_p(P)\le n$. The converse is immediate from the definition.

#### Characteristic p Galois dimension bound

↑ **Parent:** [Cohomological dimension at a prime](#cohomological-dimension-at-a-prime)

A field of characteristic $p$ satisfies $\operatorname{cd}_p(K)\le1$. The Artin-Schreier sequence and vanishing of positive-degree cohomology of the additive separable-closure module yield the bound. It concerns discrete $p$-primary modules; it does not assert that the $p$-primary [Brauer group](associative-algebra.md#brauer-group) vanishes.

## Nonabelian first cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a group $G$ acting by automorphisms on a possibly noncommutative group $B$, $H^1(G,B)$ is the pointed set of maps satisfying $c_{\sigma\tau}=c_\sigma\sigma(c_\tau)$ modulo $c_\sigma\mapsto b c_\sigma\sigma(b)^{-1}$. It classifies twisting of a reference action. It need not be an abelian group.

## Periodic group cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a finite group, the usual integral notion asks for a class $\Delta\in H^n(G;\mathbb Z)$ whose [cup product](cohomology.md#cup-product) gives the displayed isomorphisms for every coefficient module $M$ and every $i>0$. The analogous claim for just trivial coefficients over a fixed field is weaker and should be stated as such. A free cohomologically orientation-preserving sphere action supplies that field-coefficient version through [periodic group cohomology from a free sphere action](#periodic-group-cohomology-from-a-free-sphere-action).

### Cohomology ring of a finite cyclic group over its prime field

↑ **Parent:** [Periodic group cohomology](#periodic-group-cohomology)

The alternating resolution maps $g-1$ and $1+g+\cdots+g^{p-1}$ for a [cyclic group](group.md#cyclic-group) $C_p$ become zero after applying homomorphisms to its trivial [prime field](algebra.md#prime-field) module. Thus there is one class in every degree. A two-step shift of the resolution represents a degree-two periodicity class $u$. For odd $p$, a degree-one class $v$ squares to zero by graded commutativity, and

$$
H^*(BC_p;\mathbb F_p)=\Lambda_{\mathbb F_p}(v)\otimes\mathbb F_p[u],\qquad |v|=1,\ |u|=2.
$$

One can take $u=\beta(v)$ for the [Bockstein homomorphism](homology.md#bockstein-homomorphism). For $p=2$ the two maps agree over $\mathbb F_2[C_2]$, so a one-step shift gives $H^*(BC_2;\mathbb F_2)=\mathbb F_2[v]$ with $|v|=1$. The [Künneth theorem](cohomology.md#kunneth-theorem) then gives dimension $i+1$ in degree $i$ for $B(C_p\times C_p)$, obstructing [periodic group cohomology](#periodic-group-cohomology) and hence such a free sphere action.

### Periodic group cohomology from a free sphere action

↑ **Parent:** [Periodic group cohomology](#periodic-group-cohomology)

Suppose a finite group acts freely on $S^{n-1}$ and trivially on its integral [cohomology](cohomology.md). The [Borel construction](cohomology.md#borel-construction) gives a sphere fibration over $BG$ whose total space is homotopy equivalent to the $(n-1)$-dimensional quotient. Its [Serre spectral sequence](homotopy.md#serre-spectral-sequence) has just two rows with trivial local coefficients. Transgressing the fibre generator gives $\Delta$; the sole differential is multiplication by it up to sign. For $i>0$, both the source and target terms have total degrees above $n-1$, so their surviving kernel and cokernel must vanish. Hence multiplication by $\Delta$ gives period $n$ in positive-degree cohomology over any field.

## Projective-resolution definition of group cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

Choose a [projective resolution](homological-algebra.md#projective-resolution) $P_\bullet\to\mathbb Z$ of the trivial $\mathbb ZG$-module. For a $\mathbb ZG$-module $M$, [group cohomology](group-cohomology.md) is

$$
H^n(G,M)=H^n\!\left(\operatorname{Hom}_{\mathbb ZG}(P_\bullet,M)\right)
=\operatorname{Ext}_{\mathbb ZG}^n(\mathbb Z,M).
$$

Different [projective resolutions](homological-algebra.md#projective-resolution) give naturally isomorphic groups.

### Group cohomology commutes with finite direct sums

↑ **Parent:** [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)

For $\mathbb ZG$-modules $M_1,M_2$,

$$
H^n(G,M_1\oplus M_2)\cong H^n(G,M_1)\oplus H^n(G,M_2),
$$

because the [Hom functor](homological-algebra.md#hom-functor) into a finite [direct sum](vector-space.md#direct-sum) splits degree by degree and taking [cohomology](cohomology.md) preserves that splitting.

### Koszul resolution for a rank-two free abelian group

↑ **Parent:** [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)

For $G=\langle x,y\mid xy=yx\rangle$, the trivial $\mathbb ZG$-module has the free resolution

$$
0\longrightarrow\mathbb ZG\xrightarrow{\binom{1-y}{x-1}}(\mathbb ZG)^2
\xrightarrow{(x-1\quad y-1)}\mathbb ZG\longrightarrow\mathbb Z\longrightarrow0.
$$

#### Second cohomology of a rank-two free abelian group with truncated group-ring coefficients

↑ **Parent:** [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group)

If $G\cong\mathbb Z^2$, $I$ is the augmentation ideal, and $M=\mathbb ZG/I^2$, then

$$
H^2(G,M)\cong M/IM\cong\mathbb Z.
$$

The quotient map $M\to\mathbb ZG/I\cong\mathbb Z$ induces an isomorphism in second cohomology.

## Coinduced module

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a subgroup $K\leq G$ and a $\mathbb ZK$-module $X$, the coinduced module is

$$
\operatorname{Coind}_K^G X=\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X),
\qquad (g f)(r)=f(rg).
$$

<h3 id="shapiro-s-lemma">Shapiro's lemma</h3>

↑ **Parent:** [Coinduced module](#coinduced-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shapiro's_lemma)

[Shapiro's lemma](#shapiro-s-lemma) gives a natural isomorphism

$$
H^n\!\left(G,\operatorname{Coind}_K^G X\right)\cong H^n(K,X).
$$

It follows by applying the [Hom functor adjunction for a coinduced module](#hom-functor-adjunction-for-a-coinduced-module) to a [projective resolution](homological-algebra.md#projective-resolution) and observing that restriction from $G$ to $K$ preserves [projective modules](module-theory.md#projective-module).

#### Hom functor adjunction for a coinduced module

↑ **Parent:** [Shapiro's lemma](#shapiro-s-lemma)

For a $\mathbb ZG$-module $P$ and a $\mathbb ZK$-module $X$,

$$
\operatorname{Hom}_{\mathbb ZG}\!\left(P,\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X)\right)
\cong\operatorname{Hom}_{\mathbb ZK}(P,X).
$$

Evaluation at $1\in G$ gives the forward map. If $a:P\to X$ is $\mathbb ZK$-linear, its inverse sends $a$ to $p\mapsto(r\mapsto a(rp))$.

## Conjugation module of a group ring

↑ **Parent:** [Group cohomology](group-cohomology.md)

The [group ring](commutative-algebra.md#group-ring) $\mathbb ZG$ becomes a $\mathbb ZG$-module under the [conjugation action](group-action.md#conjugation-action) $g\cdot x=gxg^{-1}$. Its basis splits into [conjugacy classes](group-action.md#conjugacy-class), and the span of the class of $x$ is the permutation module on $G/C_G(x)$.

### Group cohomology of a conjugation module

↑ **Parent:** [Conjugation module of a group ring](#conjugation-module-of-a-group-ring)

For a [finite group](group.md#finite-group) $G$ and representatives $g_i$ of its [conjugacy classes](group-action.md#conjugacy-class), [Shapiro's lemma](#shapiro-s-lemma) gives

$$
H^n(G,\mathbb ZG_{\mathrm{conj}})
\cong\bigoplus_iH^n(C_G(g_i),\mathbb Z).
$$

## Integral cohomology of a finite cyclic group

↑ **Parent:** [Group cohomology](group-cohomology.md)

For the trivial action of the [finite cyclic group](group.md#finite-cyclic-group) $C_m$ on $\mathbb Z$,

$$
H^0(C_m,\mathbb Z)=\mathbb Z,
\qquad H^{2k+1}(C_m,\mathbb Z)=0,
\qquad H^{2k}(C_m,\mathbb Z)=\mathbb Z/m\mathbb Z
$$

for $k\geq1$. The [periodic resolution of a finite cyclic group](#periodic-resolution-of-a-finite-cyclic-group) proves this directly.

### Periodic resolution of a finite cyclic group

↑ **Parent:** [Integral cohomology of a finite cyclic group](#integral-cohomology-of-a-finite-cyclic-group)

If $C_m=\langle t\rangle$ and $N=1+t+\cdots+t^{m-1}$, a [free resolution](homological-algebra.md#free-resolution) of the trivial $\mathbb ZC_m$-module alternates multiplication by $t-1$ and $N$. Applying $\operatorname{Hom}_{\mathbb ZC_m}(-,\mathbb Z)$ for the trivial action alternates the zero map and multiplication by $m$.

## Group extension

↑ **Parent:** [Group cohomology](group-cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_extension)

A group extension of $G$ by an abelian $G$-module $A$ is a [short exact sequence](module-theory.md#short-exact-sequence)

$$
1\longrightarrow A\longrightarrow E\longrightarrow G\longrightarrow1
$$

whose conjugation action on $A$ is the specified $G$-action.

### Torsion-free finite extension of a lattice

↑ **Parent:** [Group extension](#group-extension)

For a specified [finite group](group.md#finite-group) action on $A=\mathbb Z^n$, extensions are classified by $e\in H^2(Q,A)$. For an element $q$ of prime order $p$, a lift $g$ satisfies $g^p=a\in A^q$; changing the lift changes $a$ by $N_qv=(1+q+\cdots+q^{p-1})v$. Thus the extension is torsion-free precisely when every restriction to a prime-order cyclic subgroup is nonzero in $A^q/N_qA$. Any finite-order element has a prime-order power, so this tests all torsion. An arbitrary finite quotient must not be confused with faithful holonomy on a maximal translation lattice.

### Split group extension

↑ **Parent:** [Group extension](#group-extension)

A [group extension](#group-extension) is split when its quotient homomorphism admits a group-homomorphic section. Equivalently, the middle group is a [semidirect product](group-theory.md#semidirect-product) of the kernel by the quotient.

#### Section normal form for a split group extension

↑ **Parent:** [Split group extension](#split-group-extension)

If a [group homomorphism](group-theory.md#group-homomorphism) section $i:G/N\to G$ satisfies $\pi i=\mathrm{id}$, then each $g\in G$ has a unique form $i(q)n$ with $q\in G/N$ and $n\in N$: take $q=\pi(g)$ and $n=i(q)^{-1}g$. Thus $(q,n)\mapsto i(q)n$ is a bijection. It is a homomorphism for the ordinary [direct product of groups](group-theory.md#direct-product-of-groups) exactly when the section image centralizes $N$. In general it describes a [semidirect product](group-theory.md#semidirect-product) with a nontrivial conjugation action.

### Equivalent group extensions

↑ **Parent:** [Group extension](#group-extension)

Two extensions of $G$ by the same $G$-module $M$ are equivalent when an isomorphism between their middle groups commutes with the inclusions of $M$ and the projections to $G$. Splitness is preserved under this equivalence.

### Fiber product of groups

↑ **Parent:** [Group extension](#group-extension)

For homomorphisms $E\to H$ and $G\to H$, their fiber product is

$$
E\times_HG=\{(e,g)\in E\times G:\pi(e)=f(g)\}.
$$

It is a subgroup of $E\times G$. Pulling a [group extension](#group-extension) back along $G\to H$ uses this fiber product as its middle group.

#### Mihailova subgroup

↑ **Parent:** [Fiber product of groups](#fiber-product-of-groups)

For a [finite group presentation](geometric-group-theory.md#finite-group-presentation) $H=\langle x_1,\ldots,x_m\mid r_1,\ldots,r_n\rangle$, let $F$ be the free group on its generators and $\pi:F\to H$. The corresponding [fiber product of groups](#fiber-product-of-groups) is generated by $(x_i,x_i)$ and $(1,r_j)$. Conjugation by the diagonal pairs supplies every pair $(1,r)$ with $r$ in the [normal closure](group-theory.md#normal-closure) of the relators, and $(u,v)=(u,u)(1,u^{-1}v)$ proves the generating claim. Membership of $(1,w)$ is equivalent to $w=1$ in $H$, so this finitely generated subgroup can have undecidable membership even though $F\times F$ has soluble word problem.

### Second group cohomology classifies group extensions

↑ **Parent:** [Group extension](#group-extension)

Equivalence classes of [group extensions](#group-extension) of $G$ by an abelian $G$-module $A$ correspond to $H^2(G,A)$. A section $s:G\to E$ produces the [extension cocycle](#extension-cocycle)

$$
c(g,h)=s(g)s(h)s(gh)^{-1},
$$

and changing the section changes $c$ by a [group coboundary](#group-coboundary).

#### Integral central extensions of a rank-two free abelian group

↑ **Parent:** [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)

With a fixed identification of the kernel with $\mathbb Z$ and quotient with $\mathbb Z^2$, these central [group extensions](#group-extension) are classified by $n\in\mathbb Z$. Choose lifts $x,y$ of the quotient generators; their commutator is $z^n$ and is unchanged by central changes of lifts. Every element has unique normal form $z^my^bx^a$, proving this invariant is complete. A cocycle representative is $c((a,b),(c,d))=nad$, whose cocycle identity follows from bilinearity. Its extension multiplication is $(a,b,m)(c,d,l)=(a+c,b+d,m+l+nad)$. The zero parameter gives $\mathbb Z^3$ and parameter one gives the integer Heisenberg group. The [Koszul resolution for a rank-two free abelian group](#koszul-resolution-for-a-rank-two-free-abelian-group) independently computes $H^2(\mathbb Z^2,\mathbb Z)\cong\mathbb Z$.

#### Extension cocycle

↑ **Parent:** [Second group cohomology classifies group extensions](#second-group-cohomology-classifies-group-extensions)

An extension cocycle is the [two-cocycle](#two-cocycle) obtained from a section of a [group extension](#group-extension). It measures the failure of the section to be a [group homomorphism](group-theory.md#group-homomorphism).

## Group cocycle

↑ **Parent:** [Group cohomology](group-cohomology.md)

A group cocycle is an element of the kernel of the coboundary map in the standard cochain complex computing [group cohomology](group-cohomology.md).

### One-cocycle

↑ **Parent:** [Group cocycle](#group-cocycle)

For a $G$-module $M$, a one-cocycle is a map $f:G\to M$ satisfying $f(gh)=f(g)+g\cdot f(h)$.

#### Galois 1-cocycle

↑ **Parent:** [One-cocycle](#one-cocycle)

A continuous one-cocycle for a Galois group acting on an abelian module $M$ is a map satisfying the displayed identity. Cocycles modulo maps $\sigma\mapsto\sigma u-u$ form $H^1(K,M)$ in [Galois cohomology](galois-theory.md#galois-cohomology). For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), choosing $mQ=P$ gives the cocycle $\sigma\mapsto\sigma Q-Q$ in $E[m]$, which represents the [Kummer map of an elliptic curve](normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve).

#### Crossed homomorphism

↑ **Parent:** [One-cocycle](#one-cocycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crossed_homomorphism)

A crossed homomorphism from $G$ to a $G$-module $M$ is a map $f:G\to M$ satisfying

$$
f(gh)=f(g)+g\cdot f(h).
$$

Thus crossed homomorphisms are precisely [one-cocycles](#one-cocycle).

##### Principal crossed homomorphism

↑ **Parent:** [Crossed homomorphism](#crossed-homomorphism)

For $m\in M$, the map $g\mapsto g\cdot m-m$ is a principal crossed homomorphism. It is the [group coboundary](#group-coboundary) of the zero-cochain $m$, so first [group cohomology](group-cohomology.md) is the quotient of crossed homomorphisms by principal crossed homomorphisms.

### Two-cocycle

↑ **Parent:** [Group cocycle](#group-cocycle)

For a $G$-module $M$, a two-cocycle is a map $c:G\times G\to M$ satisfying

$$
g\cdot c(h,k)-c(gh,k)+c(g,hk)-c(g,h)=0.
$$

#### Normalized two-cocycle

↑ **Parent:** [Two-cocycle](#two-cocycle)

A two-cocycle is normalized when $c(1,g)=c(g,1)=0$ in additive notation, or $c(1,g)=c(g,1)=1$ in multiplicative notation.

## Group coboundary

↑ **Parent:** [Group cohomology](group-cohomology.md)

A group coboundary is a cochain in the image of the preceding coboundary map. Quotienting [group cocycles](#group-cocycle) by group coboundaries gives [group cohomology](group-cohomology.md).

## Group cochain

↑ **Parent:** [Group cohomology](group-cohomology.md)

An inhomogeneous group $n$-cochain with values in a $G$-module $M$ is a function $G^n\to M$. The standard alternating [group coboundary](#group-coboundary) turns these groups into the cochain complex whose cohomology is $H^n(G,M)$.

## Long exact sequence in group cohomology

↑ **Parent:** [Group cohomology](group-cohomology.md)

A [short exact sequence](module-theory.md#short-exact-sequence) $0\to M_1\to M_2\to M_3\to0$ of $G$-modules induces a natural long exact sequence

$$
0\to H^0(G,M_1)\to H^0(G,M_2)\to H^0(G,M_3)
\to H^1(G,M_1)\to\cdots.
$$

It follows by applying the cochain functor and the long exact cohomology sequence of a short exact sequence of cochain complexes.

## Finite-group cohomology is annihilated by the group order

↑ **Parent:** [Group cohomology](group-cohomology.md)

If $G$ is finite and $n>0$, multiplication by $|G|$ annihilates $H^n(G,M)$. Indeed, restriction to the trivial subgroup is zero in positive degree, while the restriction-corestriction composite is multiplication by $|G|$.

### Restriction-corestriction identity in group cohomology

↑ **Parent:** [Finite-group cohomology is annihilated by the group order](#finite-group-cohomology-is-annihilated-by-the-group-order)

For a subgroup $K\leq G$, restriction followed by corestriction acts on group cohomology as the sum over coset translates. For $K$ trivial, inner automorphisms act trivially on cohomology, so this sum is multiplication by $|G|$.

## Mac Lane exact sequence for a free presentation

↑ **Parent:** [Group cohomology](group-cohomology.md)

For a free presentation $G=F/R$ and a $\mathbb ZG$-module $M$, restriction of derivations to $R$ gives an exact sequence

$$
H^1(F,M)\longrightarrow\operatorname{Hom}_G(R/[R,R],M)
\longrightarrow H^2(G,M)\longrightarrow0.
$$

It follows by applying $\operatorname{Hom}_{\mathbb ZG}(-,M)$ to the presentation relation sequence.

<h2 id="lyndon-hochschild-serre-spectral-sequence">Lyndon–Hochschild–Serre spectral sequence</h2>

↑ **Parent:** [Group cohomology](group-cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lyndon–Hochschild–Serre_spectral_sequence)

For a [normal subgroup](group-theory.md#normal-subgroup) $H\triangleleft G$, quotient $Q=G/H$, and a $G$-module $M$, the Lyndon–Hochschild–Serre spectral sequence has

$$
E_2^{p,q}=H^p(Q,H^q(H,M))\Longrightarrow H^{p+q}(G,M).
$$

### Cyclic-extension shift of group-ring cohomology

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

If $N$ has a finite resolution by finitely generated projective modules, restriction of the semidirect-product group ring gives a direct sum of copies of $\mathbb ZN$, indexed by the integers. On its kernel cohomology the cyclic generator shifts those copies, possibly twisting each copy by an automorphism. Invariants are zero because elements have finite support; coinvariants identify with a single copy. The two-column [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) therefore gives the displayed isomorphism of abelian groups. A group with such a finite resolution and cohomological dimension $d$ has $H^d(N;\mathbb ZN)\ne0$, so the cyclic extension has dimension $d+1$.

### Five-term exact sequence in group cohomology

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

The low-degree edge maps of the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence) give

$$
0\to H^1(Q,M^H)\xrightarrow{\mathrm{inf}}H^1(G,M)
\xrightarrow{\mathrm{res}}H^1(H,M)^Q
\xrightarrow{d_2}H^2(Q,M^H)
\xrightarrow{\mathrm{inf}}H^2(G,M).
$$

#### Inflation-restriction exact sequence

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

For a normal subgroup $N$ of $G$ and a $G$-module $M$, the low-degree exact sequence begins $0\to H^1(G/N,M^N)\to H^1(G,M)\to H^1(N,M)^{G/N}\to H^2(G/N,M^N)$. The first map inflates cocycles along $G\to G/N$; the second restricts them. If the restriction is trivial, subtract a coboundary to make the cocycle vanish on $N$ and descend to the quotient. Thus for a finite Galois extension, the kernel of restriction on [Galois cohomology](galois-theory.md#galois-cohomology) with finite coefficients is finite.

#### Inflation map in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

Inflation composes a cocycle on the quotient $Q=G/H$ with the quotient map $G\to Q$ and regards its values in the invariant submodule $M^H$ as values in $M$.

#### Restriction map in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

Restriction sends a cocycle on $G$ to its restriction to a subgroup $H$. If $H$ is normal, its image in $H^1(H,M)$ is fixed by the induced $G/H$-action.

#### Transgression in group cohomology

↑ **Parent:** [Five-term exact sequence in group cohomology](#five-term-exact-sequence-in-group-cohomology)

The transgression $d_2:H^1(H,M)^Q\to H^2(Q,M^H)$ is the first differential crossing from the vertical to the horizontal edge of the [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence). If a representative on $H$ is extended to a cochain on $G$, its coboundary descends to the representing two-cocycle on $Q$.

### Integral cohomology of the dihedral group of order ten

↑ **Parent:** [Lyndon–Hochschild–Serre spectral sequence](#lyndon-hochschild-serre-spectral-sequence)

For the dihedral group $D_{10}=C_5\rtimes C_2$,

$$
H^n(D_{10},\mathbb Z)\cong
\begin{cases}
\mathbb Z,&n=0,\\
0,&n\text{ odd},\\
\mathbb Z/2,&n\equiv2\pmod4,\\
\mathbb Z/10,&n>0\text{ and }n\equiv0\pmod4.
\end{cases}
$$

The Lyndon–Hochschild–Serre spectral sequence proves this from the inversion action of $C_2$ on $H^2(C_5,\mathbb Z)$.

## ↑ Ancestors (5)

1. [Group theory](group-theory.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (18)

- [Classifying space of a discrete group](fiber-bundle.md#classifying-space-of-a-discrete-group)
- [Continuous cochains with topological coefficients](#continuous-cochains-with-topological-coefficients)
- [Dimension shifting in group cohomology](#dimension-shifting-in-group-cohomology)
- [Finite groups cannot act freely on Euclidean space](group-action.md#finite-groups-cannot-act-freely-on-euclidean-space)
- [Galois cohomology](galois-theory.md#galois-cohomology)
- [Group coboundary](#group-coboundary)
- [Group cocycle](#group-cocycle)
- [Integral cohomological dimension of a group](#integral-cohomological-dimension-of-a-group)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-2.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-125.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-151.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-125.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-343.md#4/b/solution)
- [Principal crossed homomorphism](#principal-crossed-homomorphism)
- [Projective-resolution definition of group cohomology](#projective-resolution-definition-of-group-cohomology)
- [Tate cohomology of a finite group](#tate-cohomology-of-a-finite-group)
