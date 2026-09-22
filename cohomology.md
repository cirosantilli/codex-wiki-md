# Cohomology

↑ **Parent:** [Algebraic topology](algebraic-topology.md)

Cohomology is the contravariant counterpart of [homology](homology.md), formed from cochains and coboundaries. A coefficient ring equips it with the [cup product](#cup-product) and hence with a graded ring structure.

**Table of contents**

- [Gysin homomorphism](#gysin-homomorphism)
- [Generalized cohomology theory](#generalized-cohomology-theory)
  - [Represented cohomology theory](#represented-cohomology-theory)
  - [Multiplicative generalized cohomology theory](#multiplicative-generalized-cohomology-theory)
  - [Atiyah-Hirzebruch spectral sequence](#atiyah-hirzebruch-spectral-sequence)
    - [Homological Atiyah-Hirzebruch spectral sequence](#homological-atiyah-hirzebruch-spectral-sequence)
- [Cohomology groups do not determine homotopy type](#cohomology-groups-do-not-determine-homotopy-type)
- [Singular cohomology](#singular-cohomology)
  - [Singular cochain](#singular-cochain)
    - [Cochain pullback](#cochain-pullback)
- [Cohomology operation](#cohomology-operation)
  - [Stable cohomology operation](#stable-cohomology-operation)
    - [Comparison of stable maps and cohomology operations](#comparison-of-stable-maps-and-cohomology-operations)
    - [Integral generator signs constrain Steenrod comparisons](#integral-generator-signs-constrain-steenrod-comparisons)
    - [Steenrod algebra](#steenrod-algebra)
      - [Admissible sequence of Steenrod squares](#admissible-sequence-of-steenrod-squares)
        - [Excess of an admissible Steenrod sequence](#excess-of-an-admissible-steenrod-sequence)
      - [Adem relations](#adem-relations)
      - [Steenrod square](#steenrod-square)
      - [Cartan formula (algebraic topology)](#cartan-formula-algebraic-topology)
      - [Steenrod reduced power](#steenrod-reduced-power)
        - [Steenrod powers on quaternionic projective space](#steenrod-powers-on-quaternionic-projective-space)
- [Reduced cohomology](#reduced-cohomology)
- [Equivariant cohomology](#equivariant-cohomology)
  - [Borel construction](#borel-construction)
- [Cohomology group](#cohomology-group)
  - [Cohomology class](#cohomology-class)
- [Integral cohomology](#integral-cohomology)
- [Relative cohomology](#relative-cohomology)
  - [Long exact cohomology sequence of a pair](#long-exact-cohomology-sequence-of-a-pair)
- [Induced map on cohomology](#induced-map-on-cohomology)
  - [Homotopy invariance of cohomology](#homotopy-invariance-of-cohomology)
  - [Realization of top-dimensional cohomology by a sphere map](#realization-of-top-dimensional-cohomology-by-a-sphere-map)
- [Universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology)
  - [First cohomology of the countably punctured plane](#first-cohomology-of-the-countably-punctured-plane)
- [Alexander duality](#alexander-duality)
  - [Mod-two homology of a submanifold complement](#mod-two-homology-of-a-submanifold-complement)
  - [Complement homology of a compact codimension-zero submanifold](#complement-homology-of-a-compact-codimension-zero-submanifold)
- [Compactly supported cohomology](#compactly-supported-cohomology)
  - [Top compactly supported cohomology from orientation signs](#top-compactly-supported-cohomology-from-orientation-signs)
  - [Compactly supported cohomology of Euclidean space](#compactly-supported-cohomology-of-euclidean-space)
  - [Compact-support comparison with a one-point compactification](#compact-support-comparison-with-a-one-point-compactification)
  - [Proper map](#proper-map)
- [Cap product](#cap-product)
  - [Naturality of the cap product](#naturality-of-the-cap-product)
  - [Fundamental class](#fundamental-class)
    - [Local orientation of a manifold](#local-orientation-of-a-manifold)
    - [R-fundamental class](#r-fundamental-class)
    - [Poincare duality](#poincare-duality)
      - [Poincaré duality for noncompact manifolds](#poincare-duality-for-noncompact-manifolds)
      - [Rational cohomology injectivity of a nonzero-degree map](#rational-cohomology-injectivity-of-a-nonzero-degree-map)
      - [Third homology of a closed oriented four-manifold](#third-homology-of-a-closed-oriented-four-manifold)
      - [Poincare duality with the orientation local system](#poincare-duality-with-the-orientation-local-system)
        - [Second homology of a closed nonorientable three-manifold](#second-homology-of-a-closed-nonorientable-three-manifold)
      - [Intersection pairing on an oriented surface](#intersection-pairing-on-an-oriented-surface)
      - [Mod-two Poincare duality](#mod-two-poincare-duality)
      - [Euler characteristic parity in dimensions congruent to two modulo four](#euler-characteristic-parity-in-dimensions-congruent-to-two-modulo-four)
        - [Every even integer is the Euler characteristic of a closed oriented six-manifold](#every-even-integer-is-the-euler-characteristic-of-a-closed-oriented-six-manifold)
      - [Cohomological pushforward between closed oriented manifolds](#cohomological-pushforward-between-closed-oriented-manifolds)
      - [Poincare duality pairing](#poincare-duality-pairing)
        - [Even rank of middle cohomology in dimension four k plus two](#even-rank-of-middle-cohomology-in-dimension-four-k-plus-two)
      - [Cohomological injectivity of a map of invertible degree](#cohomological-injectivity-of-a-map-of-invertible-degree)
      - [Lefschetz duality](#lefschetz-duality)
        - [Mod-two handle duality](#mod-two-handle-duality)
      - [Poincare dual](#poincare-dual)
        - [Compactly supported dual of a compact submanifold](#compactly-supported-dual-of-a-compact-submanifold)
      - [Cap-product support lemma for a two-set cover](#cap-product-support-lemma-for-a-two-set-cover)
      - [Cohomological injectivity of a degree-one map](#cohomological-injectivity-of-a-degree-one-map)
      - [Homology sphere](#homology-sphere)
        - [Simply connected closed three-manifolds are homology spheres](#simply-connected-closed-three-manifolds-are-homology-spheres)
        - [Homotopy sphere](#homotopy-sphere)
          - [Topological generalized Poincare theorem](#topological-generalized-poincare-theorem)
- [Cup product](#cup-product)
  - [Cup power](#cup-power)
  - [Cohomological cross product](#cohomological-cross-product)
  - [Cup length](#cup-length)
  - [Relative cup product](#relative-cup-product)
    - [Nilpotence from a contractible subcomplex cover](#nilpotence-from-a-contractible-subcomplex-cover)
    - [Vanishing cup product from an open cover](#vanishing-cup-product-from-an-open-cover)
  - [Graded commutativity of the cup product](#graded-commutativity-of-the-cup-product)
  - [Exterior product in cohomology](#exterior-product-in-cohomology)
  - [Cohomology ring](#cohomology-ring)
    - [Degree-one cup-square obstruction to ring isomorphism](#degree-one-cup-square-obstruction-to-ring-isomorphism)
    - [Cohomology ring of a product of two spheres](#cohomology-ring-of-a-product-of-two-spheres)
      - [Cohomology ring of a product of unequal-dimensional spheres](#cohomology-ring-of-a-product-of-unequal-dimensional-spheres)
      - [Cup square after a diagonal sphere attachment](#cup-square-after-a-diagonal-sphere-attachment)
    - [Mod-p cup-square obstruction to a homotopy equivalence](#mod-p-cup-square-obstruction-to-a-homotopy-equivalence)
    - [Cohomology ring of a closed oriented surface](#cohomology-ring-of-a-closed-oriented-surface)
- [Künneth theorem](#kunneth-theorem)
  - [Cohomology cross product](#cohomology-cross-product)
  - [Cohomological Künneth theorem over a field](#cohomological-kunneth-theorem-over-a-field)
  - [Integral cohomological Künneth theorem for finite cell complexes](#integral-cohomological-kunneth-theorem-for-finite-cell-complexes)
  - [Diagonal-degree obstruction to a symmetric sphere retraction](#diagonal-degree-obstruction-to-a-symmetric-sphere-retraction)
  - [Homology cross product](#homology-cross-product)
    - [Eilenberg–Zilber theorem](#eilenberg-zilber-theorem)
  - [Integral Künneth torsion polynomial](#integral-kunneth-torsion-polynomial)

## Gysin homomorphism

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gysin_homomorphism)

For an oriented proper smooth map $f:M^m\to N^n$ of oriented [manifolds](topology.md#topological-manifold), the [Gysin homomorphism](#gysin-homomorphism) is a degree-shifting pushforward $f_!:H^k(M)\to H^{k+n-m}(N)$, defined using [Poincare duality](#poincare-duality) and the appropriate pushforward on homology. For an oriented sphere bundle it is integration along the fiber and participates in the [Gysin sequence of a sphere bundle](fiber-bundle.md#gysin-sequence-of-a-sphere-bundle). Oriented embeddings give the corresponding Thom-class construction.

## Generalized cohomology theory

↑ **Parent:** [Cohomology](cohomology.md)

A generalized cohomology theory assigns graded groups contravariantly to suitable topological pairs, with homotopy invariance, excision and a natural long exact sequence for each pair. It omits the dimension axiom of ordinary [cohomology](cohomology.md), so its coefficient groups at a point can occur in degrees other than zero. A multiplicative theory also has compatible external and relative [cup products](#cup-product).

### Represented cohomology theory

↑ **Parent:** [Generalized cohomology theory](#generalized-cohomology-theory)

A [topological spectrum](algebraic-topology.md#spectrum-topology) $E$ represents the reduced [generalized cohomology theory](#generalized-cohomology-theory) $\widetilde E^q(X)=[\Sigma^\infty X,\Sigma^qE]_{\mathrm{st}}$. For an [Omega-spectrum](algebraic-topology.md#omega-spectrum) this equals $[X,E_q]_*$, taking $E_q=\Omega^{-q}E_0$ for negative $q$. It is contravariant in $X$.

### Multiplicative generalized cohomology theory

↑ **Parent:** [Generalized cohomology theory](#generalized-cohomology-theory)

A [generalized cohomology theory](#generalized-cohomology-theory) with natural unital cup products compatible with relative groups, suspension, and the cohomology axioms. Its coefficient groups form a graded ring. Thom orientations make the cohomology of a bundle's [Thom space](fiber-bundle.md#thom-space) a shifted module over the cohomology of the base.

// Target: geometry-and-topology.bigb

### Atiyah-Hirzebruch spectral sequence

↑ **Parent:** [Generalized cohomology theory](#generalized-cohomology-theory)

The skeletal filtration of a CW complex gives this spectral sequence, with differential of bidegree $(r,1-r)$ in cohomological grading. For a finite complex the filtration is finite and convergence is bounded. In a multiplicative theory the associated graded product is the ordinary cohomology product with coefficients in the theory's coefficient ring.

#### Homological Atiyah-Hirzebruch spectral sequence

↑ **Parent:** [Atiyah-Hirzebruch spectral sequence](#atiyah-hirzebruch-spectral-sequence)

The skeletal filtration of a [CW complex](algebraic-topology.md#cw-complex) and the [cofiber sequences of spectra](algebraic-topology.md#cofiber-sequence-of-spectra) of its cell attachments produce

$$
E^2_{p,q}=\widetilde H_p(X;\pi_qE)\Longrightarrow\widetilde E_{p+q}(X),\qquad d_r:E^r_{p,q}\to E^r_{p-r,q+r-1}.
$$

For a [connective spectrum](algebraic-topology.md#connective-spectrum) it is first quadrant and converges in each fixed total degree. Its reduced version has no contribution from the basepoint summand.

## Cohomology groups do not determine homotopy type

↑ **Parent:** [Cohomology](cohomology.md)

The [torus](topology.md#torus) and the [wedge sum](topology.md#wedge-sum) $S^1\vee S^1\vee S^2$ both have integral cohomology $\mathbb Z,\mathbb Z^2,\mathbb Z$ in degrees zero, one and two. Their fundamental groups differ: the torus has $\mathbb Z^2$, while the wedge has the nonabelian free group on two generators. Thus even compact finite cell complexes can have the same additive cohomology without being homotopy equivalent.

## Singular cohomology

↑ **Parent:** [Cohomology](cohomology.md)

For a [topological space](topology.md#topological-space) $X$ and [abelian group](group.md#abelian-group) $A$, singular cohomology is the [cohomology](cohomology.md) of the [cochain complex](algebra.md#cochain-complex) $C^n(X;A)=\operatorname{Hom}(C_n(X;\mathbb Z),A)$, where $C_n$ is the [singular chain group](homology.md#singular-chain-group). Its differential is dual to the singular boundary. This theory has [relative cohomology](#relative-cohomology), [long exact sequences](homology.md#long-exact-sequence) and the [Excision theorem](homology.md#excision-theorem). On spaces that are not locally contractible it can differ from [Čech cohomology](ringed-space.md#cech-cohomology).

### Singular cochain

↑ **Parent:** [Singular cohomology](#singular-cohomology)

A singular $n$-cochain with coefficients in an [abelian group](group.md#abelian-group) $A$ is a homomorphism from the [singular chain group](homology.md#singular-chain-group) $C_n(X;\mathbb Z)$ to $A$. It is specified by its values on all singular simplices, without a finite-support restriction. Its [coboundary](algebra.md#coboundary) evaluates on the alternating sum of the faces. The resulting [cochain complex](algebra.md#cochain-complex) computes [singular cohomology](#singular-cohomology).

#### Cochain pullback

↑ **Parent:** [Singular cochain](#singular-cochain)

For a [continuous map](topology.md#continuous-map) $f:X\to Y$, precomposition with the induced map on [singular chains](homology.md#singular-chain) sends a [singular cochain](#singular-cochain) on $Y$ to one on $X$. It commutes with the [coboundary](algebra.md#coboundary) and induces the [induced map on cohomology](#induced-map-on-cohomology).

## Cohomology operation

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cohomology_operation)

A cohomology operation is a [natural transformation](category.md#natural-transformation) between cohomology functors. Thus for every continuous map $f$, its pullback commutes with the operation: $\theta(f^*a)=f^*\theta(a)$. This makes operations additional invariants of [homotopy equivalence](algebraic-topology.md#homotopy-equivalence), beyond the additive groups and their [cup products](#cup-product).

### Stable cohomology operation

↑ **Parent:** [Cohomology operation](#cohomology-operation)

A cohomology operation is stable if it commutes with the [suspension isomorphism](algebraic-topology.md#suspension-isomorphism) on [reduced cohomology](#reduced-cohomology). Ordinary [cup products](#cup-product) become zero on a suspension, but stable operations can still connect its nonzero classes. The [Steenrod squares](#steenrod-square) and [Steenrod reduced powers](#steenrod-reduced-power) are examples.

#### Comparison of stable maps and cohomology operations

↑ **Parent:** [Stable cohomology operation](#stable-cohomology-operation)

For cellular [Omega-spectra](algebraic-topology.md#omega-spectrum) $D,E$, natural degree-preserving additive operations $D^*\to E^*$ commuting with suspension are compatible families $[D_j,E_j]_*$ by the [Yoneda lemma](category.md#yoneda-lemma). Since $D\simeq\operatorname{hocolim}_j\Sigma^{-j}\Sigma^\infty D_j$, the [Milnor exact sequence for maps of spectra](algebraic-topology.md#milnor-exact-sequence-for-maps-of-spectra) realizes every such family. Its kernel consists precisely of [hyperphantom maps of spectra](algebraic-topology.md#hyperphantom-map-of-spectra). Thus operations determine stable maps only modulo that kernel.

#### Integral generator signs constrain Steenrod comparisons

↑ **Parent:** [Stable cohomology operation](#stable-cohomology-operation)

Suppose two integral cohomology groups of a space are free of rank one. An integral isomorphism can send each chosen generator only to itself or its negative. After reduction modulo $p$, naturality of a [Steenrod reduced power](#steenrod-reduced-power) between those groups therefore permits its coefficient to change only by a sign, even though an abstract vector-space change of basis could rescale by any nonzero field element. At $p=5$, coefficients one and two cannot be related by signs, so they obstruct an integral [homotopy equivalence](algebraic-topology.md#homotopy-equivalence). This constraint is stronger than comparing the isolated mod-five Steenrod modules with arbitrary bases.

#### Steenrod algebra

↑ **Parent:** [Stable cohomology operation](#stable-cohomology-operation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steenrod_algebra)

The Steenrod algebra organizes stable mod-$p$ [cohomology operations](#cohomology-operation). At $p=2$ it is generated by the [Steenrod squares](#steenrod-square); at an odd prime it is generated by the [Steenrod reduced powers](#steenrod-reduced-power) and [Bockstein homomorphism](homology.md#bockstein-homomorphism). Cohomology is a module over this algebra, and every continuous map induces a homomorphism preserving its action.

##### Admissible sequence of Steenrod squares

↑ **Parent:** [Steenrod algebra](#steenrod-algebra)

An index sequence obeying the displayed inequalities represents an admissible product $\operatorname{Sq}^{i_1}\cdots\operatorname{Sq}^{i_r}$. Its degree increment is the sum of the indices. The [Adem relations](#adem-relations) rewrite every square monomial in terms of admissible ones, whose [Steenrod excess](#excess-of-an-admissible-steenrod-sequence) controls universal instability.

###### Excess of an admissible Steenrod sequence

↑ **Parent:** [Admissible sequence of Steenrod squares](#admissible-sequence-of-steenrod-squares)

The excess measures the minimum degree on which an admissible Steenrod monomial can be nonzero. Strict excess below $n$ picks out polynomial generators in the mod-two [cohomology](cohomology.md) of $K(\mathbb Z/2,n)$; equality can correspond to a square, rather than a new generator.

##### Adem relations

↑ **Parent:** [Steenrod algebra](#steenrod-algebra)

These mod-two identities rewrite nonadmissible products of [Steenrod squares](#steenrod-square). For example, $\operatorname{Sq}^1\operatorname{Sq}^1=0$, $\operatorname{Sq}^1\operatorname{Sq}^2=\operatorname{Sq}^3$, and $\operatorname{Sq}^1\operatorname{Sq}^3=0$. In general the sum ranges over $0\leq t\leq\lfloor a/2\rfloor$ and coefficients are reduced modulo two.

##### Steenrod square

↑ **Parent:** [Steenrod algebra](#steenrod-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steenrod_square)

The Steenrod squares are natural operations

$$
\operatorname{Sq}^i:H^n(X;\mathbb F_2)\to H^{n+i}(X;\mathbb F_2).
$$

For a degree-one class $x$, $\operatorname{Sq}^1x=x^2$, and $\operatorname{Sq}^1$ agrees with the mod-two Bockstein.

##### Cartan formula (algebraic topology)

↑ **Parent:** [Steenrod algebra](#steenrod-algebra)

The Cartan product formula says that total [Steenrod squares](#steenrod-square) and total [Steenrod reduced powers](#steenrod-reduced-power) preserve the [cup product](#cup-product):

$$
\operatorname{Sq}^k(ab)=\sum_{i+j=k}\operatorname{Sq}^i(a)\operatorname{Sq}^j(b),
\qquad
P^k(ab)=\sum_{i+j=k}P^i(a)P^j(b).
$$

It is named after Henri Cartan and is distinct from [Cartan's magic formula](differential-form.md#cartan-s-magic-formula) for the [Lie derivative of a differential form](differential-form.md#lie-derivative-of-a-differential-form), named after Élie Cartan.

##### Steenrod reduced power

↑ **Parent:** [Steenrod algebra](#steenrod-algebra)

For odd prime $p$, the reduced powers are natural [stable cohomology operations](#stable-cohomology-operation). They satisfy $P^0=1$, the [Cartan formula](#cartan-formula-algebraic-topology), and the instability conditions $P^i a=0$ for $2i>|a|$ and $P^i a=a^p$ for $|a|=2i$. In particular, a degree-two class has $P^1x=x^p$ and no higher nonzero reduced power. Stability lets these operations detect distinctions between suspensions whose additive cohomology and cup products agree.

###### Steenrod powers on quaternionic projective space

↑ **Parent:** [Steenrod reduced power](#steenrod-reduced-power)

Choose the degree-four generator with pullback $u\mapsto x^2$ under the [complex inclusion into quaternionic projective space](projective-space.md#complex-inclusion-into-quaternionic-projective-space). On infinite complex projective space, the [Cartan formula](#cartan-formula-algebraic-topology) gives $P^i(x^{2k})=\binom{2k}{i}x^{2k+i(p-1)}$. Injectivity of the infinite-space pullback proves the displayed formula for [quaternionic projective space](projective-space.md#quaternionic-projective-space). Restriction to $\mathbb{HP}^n$ sets powers above $n$ to zero. Coefficients are reduced modulo the odd prime $p$; the exponent is an integer because $p-1$ is even.

## Reduced cohomology

↑ **Parent:** [Cohomology](cohomology.md)

For a based space, reduced cohomology removes the coefficient-ring summand coming from the basepoint. In nonnegative degrees it is the kernel of restriction $H^*(X;R)\to H^*(\{x_0\};R)$. It agrees with ordinary [cohomology](cohomology.md) in positive degrees and admits the [suspension isomorphism](algebraic-topology.md#suspension-isomorphism) and exact sequences for based cofibrations.

## Equivariant cohomology

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivariant_cohomology)

The Borel version of equivariant cohomology is the ordinary [cohomology](cohomology.md) of the [Borel construction](#borel-construction). It retains information about both the space and its [group action](group-theory.md#group-action). For a point it is the cohomology of the [classifying space](fiber-bundle.md#classifying-space); for a free action with the usual bundle hypotheses it is the cohomology of the orbit space.

### Borel construction

↑ **Parent:** [Equivariant cohomology](#equivariant-cohomology)

For a [group action](group-theory.md#group-action) on $X$ and a contractible free $G$-space $EG$, the diagonal orbit space $EG\times_GX$ maps to the [classifying space](fiber-bundle.md#classifying-space) $BG$ with fibre $X$. It defines [equivariant cohomology](#equivariant-cohomology). When $X\to X/G$ is a principal $G$-bundle, the map $EG\times_GX\to X/G$ has contractible fibre $EG$ and gives a [homotopy equivalence](algebraic-topology.md#homotopy-equivalence) for spaces of CW type. Freeness without the bundle hypotheses should not be substituted for this assertion for arbitrary topological groups.

## Cohomology group

↑ **Parent:** [Cohomology](cohomology.md)

A degree-$q$ cohomology group is the quotient of degree-$q$ cocycles by coboundaries in a [cochain complex](algebra.md#cochain-complex). Topological cohomology groups arise from singular or cellular cochains. Their direct sum carries the [cohomology ring](#cohomology-ring) structure when equipped with the [cup product](#cup-product).

### Cohomology class

↑ **Parent:** [Cohomology group](#cohomology-group)

The equivalence class of a [cocycle](algebra.md#cocycle) in a [cochain complex](algebra.md#cochain-complex), where adding a [coboundary](algebra.md#coboundary) leaves its class unchanged.

## Integral cohomology

↑ **Parent:** [Cohomology](cohomology.md)

Integral cohomology is [cohomology](cohomology.md) with integer coefficients, $H^*(X;\mathbb Z)$. Its [cup product](#cup-product) makes it a graded [cohomology ring](#cohomology-ring), retaining torsion and integral information that can disappear after changing coefficients to a [field](algebra.md#field).

## Relative cohomology

↑ **Parent:** [Cohomology](cohomology.md)

Relative cohomology is the [cohomology](cohomology.md) of cochains on $X$ vanishing on chains in $A$. A pair has a natural [long exact sequence in cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology), and [excision](homology.md#excision-theorem) identifies relative groups for suitable neighborhood pairs.

### Long exact cohomology sequence of a pair

↑ **Parent:** [Relative cohomology](#relative-cohomology)

For an inclusion $A\subseteq X$, the restriction [cochain map](algebra.md#cochain-map) fits into an [exact triangle](algebra.md#exact-triangle-in-a-derived-category) with the relative [cochain complex](algebra.md#cochain-complex). Its [cohomology](cohomology.md) gives $\cdots\to H^i(X,A)\to H^i(X)\to H^i(A)\xrightarrow{\delta}H^{i+1}(X,A)\to\cdots$. The same construction with derived sections of a [sheaf](algebraic-geometry.md#sheaf-mathematics) complex gives relative [hypercohomology](ringed-space.md#hypercohomology) and is natural under restrictions of pairs.

## Induced map on cohomology

↑ **Parent:** [Cohomology](cohomology.md)

A continuous map $f:X\to Y$ induces a pullback $f^*:H^q(Y;R)\to H^q(X;R)$. It preserves sums and [cup products](#cup-product), and $(g\circ f)^*=f^*\circ g^*$.

### Homotopy invariance of cohomology

↑ **Parent:** [Induced map on cohomology](#induced-map-on-cohomology)

Homotopic continuous maps induce the same map on [cohomology](cohomology.md). In particular, a [homotopy equivalence](algebraic-topology.md#homotopy-equivalence) induces an isomorphism of [cohomology rings](#cohomology-ring).

### Realization of top-dimensional cohomology by a sphere map

↑ **Parent:** [Induced map on cohomology](#induced-map-on-cohomology)

If $X$ is a CW complex of dimension at most $n$, every class $a\in H^n(X;\mathbb Z)$ has the form

$$
a=f^*u
$$

for some map $f:X\to S^n$ and generator $u\in H^n(S^n;\mathbb Z)$. Cellular obstruction theory constructs $f$ on the top cells; there are no cells of larger dimension that could obstruct the extension.

## Universal coefficient theorem for cohomology

↑ **Parent:** [Cohomology](cohomology.md)

This is the cohomological form of the [universal coefficient theorem](homology.md#universal-coefficient-theorem), with Ext and Hom terms rather than the homological tensor and Tor terms.

For an abelian coefficient group $G$, cohomology fits into a split short exact sequence

$$
0\to\operatorname{Ext}(H_{n-1}(X;\mathbb Z),G)
\to H^n(X;G)
\to\operatorname{Hom}(H_n(X;\mathbb Z),G)\to0.
$$

### First cohomology of the countably punctured plane

↑ **Parent:** [Universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology)

The connected open set $X=\mathbb R^2\setminus\{(n,0):n\geq1\}$ retracts onto a locally finite graph having one independent loop around each puncture. Hence $H_1(X;\mathbb Z)\cong\bigoplus_{n\geq1}\mathbb Z$, while the [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) gives

$$
H^1(X;\mathbb Z)\cong\operatorname{Hom}\left(\bigoplus_{n\geq1}\mathbb Z,\mathbb Z\right)\cong\prod_{n\geq1}\mathbb Z,
$$

an uncountable group.

## Alexander duality

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander_duality)

For a compact locally contractible subspace $A\subseteq S^n$, Alexander duality gives

$$
\widetilde H^q(S^n\setminus A;R)\cong\widetilde H_{n-q-1}(A;R).
$$

### Mod-two homology of a submanifold complement

↑ **Parent:** [Alexander duality](#alexander-duality)

For a closed connected $k$-manifold smoothly embedded in $S^n$, with $k<n$ and $n\geq1$, its complement has

$$
\widetilde H_i(S^n\setminus M;\mathbb F_2)\cong H_{i+k+1-n}(M;\mathbb F_2)\quad(0\leq i\leq n-2),
$$

and zero reduced homology for $i\geq n-1$, where negative-index groups are zero. The [Thom isomorphism theorem](fiber-bundle.md#thom-isomorphism-theorem) for the normal bundle and the pair's exact sequence give this formula. The top ambient [fundamental class](#fundamental-class) maps isomorphically to the fundamental class of $M$, canceling the exceptional top term.

### Complement homology of a compact codimension-zero submanifold

↑ **Parent:** [Alexander duality](#alexander-duality)

A compact smooth $n$-manifold with nonempty boundary embedded in $S^n$ is a proper compact locally contractible subset. [Alexander duality](#alexander-duality) therefore expresses the [reduced homology](homology.md#reduced-homology) of its complement by the reduced [cohomology](cohomology.md) of the abstract manifold. Thus these groups do not depend on its particular [smooth embedding](differential-geometry.md#smooth-embedding).

## Compactly supported cohomology

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compactly_supported_cohomology)

Compactly supported cohomology is the cohomology of cochains vanishing outside a compact subset. Equivalently,

$$
H_c^*(X)\cong\varinjlim_{K\subseteq X\text{ compact}}H^*(X,X\setminus K).
$$

### Top compactly supported cohomology from orientation signs

↑ **Parent:** [Compactly supported cohomology](#compactly-supported-cohomology)

For a connected n-manifold without boundary, a finite good cover presents its top [compactly supported cohomology](#compactly-supported-cohomology) by one generator per disc and relations $u_i=\pm u_j$ on overlaps. This follows from the compact-support [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence) and vanishing above dimension n. The overlap graph is connected, so the group is cyclic. Coherent local [orientations](algebraic-topology.md#orientation-of-a-simplex) give $\mathbb Z$; an orientation-reversing loop gives $\mathbb Z/2$.

### Compactly supported cohomology of Euclidean space

↑ **Parent:** [Compactly supported cohomology](#compactly-supported-cohomology)

For a nonnegative integer $d$ and an [abelian group](group.md#abelian-group) $A$,

$$
H_c^q(\mathbb R^d;A)\cong\begin{cases}A,&q=d,\\0,&q\ne d.\end{cases}
$$

The [one-point compactification](topology.md#alexandroff-extension) is the [sphere](geometry-and-topology.md#sphere) $S^d$, and it is locally contractible at the added point. Apply the [compact-support comparison with a one-point compactification](#compact-support-comparison-with-a-one-point-compactification) and the [reduced cohomology](#reduced-cohomology) of a sphere. In dimension zero the compactification is $S^0$, giving the same formula.

### Compact-support comparison with a one-point compactification

↑ **Parent:** [Compactly supported cohomology](#compactly-supported-cohomology)

If the [one-point compactification](topology.md#alexandroff-extension) $X^+$ is Hausdorff and has a basis of contractible neighbourhoods at the added point, then

$$
H_c^*(X;A)\cong\widetilde H^*(X^+;A).
$$

The [Excision theorem](homology.md#excision-theorem) identifies $H^*(X,X\setminus K)$ with $H^*(X^+,X^+\setminus K)$. The contractible neighbourhoods form a cofinal family of the complements of compact $K$, and their pair [long exact sequences](homology.md#long-exact-sequence) identify each relative group naturally with [reduced cohomology](#reduced-cohomology). Passing to the [direct limit](module-theory.md#direct-limit-of-abelian-groups) gives the comparison. Local contractibility matters for [singular cohomology](#singular-cohomology); the [Hawaiian earring](topology.md#hawaiian-earring) illustrates its failure.

### Proper map

↑ **Parent:** [Compactly supported cohomology](#compactly-supported-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_map)

A continuous map is proper when inverse images of compact sets are compact. Proper maps induce contravariant maps on compactly supported cohomology.

## Cap product

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cap_product)

The cap product pairs a homology class and a cohomology class to lower degree:

$$
H_p(X;R)\otimes H^k(X;R)\longrightarrow H_{p-k}(X;R).
$$

### Naturality of the cap product

↑ **Parent:** [Cap product](#cap-product)

For a [singular simplex](homology.md#singular-simplex) $\sigma$ of dimension $n$ and a degree-$p$ [cochain](#singular-cochain), use $\sigma\frown\alpha=\alpha(\sigma|[v_0,\ldots,v_p])\sigma|[v_p,\ldots,v_n]$, setting the result to zero if $p>n$. A [continuous map](topology.md#continuous-map) $f$ commutes with both face restrictions, and the [pullback](category.md#pullback-category-theory) cochain evaluates by composing with $f$. Therefore $f_*(\sigma\frown f^*\alpha)=(f\circ\sigma)\frown\alpha$ already on chains. Passing to [homology](homology.md) and [cohomology](cohomology.md) proves the displayed [cap product](#cap-product) identity.

### Fundamental class

↑ **Parent:** [Cap product](#cap-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_class)

For an oriented closed connected $d$-manifold, the fundamental class is the unique generator of $H_d(M;\mathbb Z)$ that restricts to the orientation generator in every local homology group.

#### Local orientation of a manifold

↑ **Parent:** [Fundamental class](#fundamental-class)

A local $R$-orientation of a $d$-manifold $M$ at $x$ is a generator of the rank-one $R$-module $H_d(M,M\setminus\{x\};R)$. An $R$-orientation is a locally coherent choice of such a generator at every point.

#### R-fundamental class

↑ **Parent:** [Fundamental class](#fundamental-class)

An $R$-fundamental class of a closed $d$-manifold is a class in $H_d(M;R)$ whose image in every local homology group $H_d(M,M\setminus\{x\};R)$ is a generator. These local images form an $R$-orientation.

#### Poincare duality

↑ **Parent:** [Fundamental class](#fundamental-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincare_duality)

For a closed oriented $d$-manifold, cap product with the fundamental class gives isomorphisms

$$
H^k(M;R)\cong H_{d-k}(M;R).
$$

<h5 id="poincare-duality-for-noncompact-manifolds">Poincaré duality for noncompact manifolds</h5>

↑ **Parent:** [Poincare duality](#poincare-duality)

Cap product with the locally finite [fundamental class](#fundamental-class) of an $n$-manifold without boundary gives the displayed duality, including a possibly nontrivial [orientation local system](homology.md#orientation-local-system) $\mathcal O_M$. It is the noncompact version of [Poincare duality](#poincare-duality); for a compact manifold [Borel-Moore homology](homology.md#borel-moore-homology) is ordinary homology. Locally it is the relative fundamental-class calculation in an oriented coordinate ball; compatibility on overlaps and the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence) give the global statement. Since the chain complex of locally finite homology is zero in negative degrees, this duality implies $H^k(M;\mathbb Z)=0$ for $k>n$.

##### Rational cohomology injectivity of a nonzero-degree map

↑ **Parent:** [Poincare duality](#poincare-duality)

For a [continuous map](topology.md#continuous-map) $f:M\to N$ of nonzero [mapping degree](homology.md#degree-of-a-continuous-mapping) between closed connected oriented manifolds of the same dimension, $f^*:H^q(N;\mathbb Q)\to H^q(M;\mathbb Q)$ is injective in every degree. Pair a nonzero class $a$ with a complementary class $b$ using [Poincare duality](#poincare-duality). Naturality gives $\langle f^*a\smile f^*b,[M]\rangle=(\deg f)\langle a\smile b,[N]\rangle\ne0$, so $f^*a\ne0$. Over coefficients of positive characteristic the argument requires that the degree remain nonzero in that field.

##### Third homology of a closed oriented four-manifold

↑ **Parent:** [Poincare duality](#poincare-duality)

For a connected closed oriented four-manifold, [Poincare duality](#poincare-duality) identifies $H_3$ with $H^1$. The [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) identifies $H^1$ with $\operatorname{Hom}(H_1,\mathbb Z)$ because $H_0=\mathbb Z$ has zero Ext. Consequently $H_3$ is torsion-free and its rank equals that of $H_1$.

##### Poincare duality with the orientation local system

↑ **Parent:** [Poincare duality](#poincare-duality)

For a closed connected manifold, cap product with $[M]\in H_n(M;\mathcal O_M)$ gives the displayed isomorphism. The ordinary integral theorem results when the orientation system is trivial. Modulo two the sign representation is always trivial, so duality holds without an orientability assumption. In particular a nonorientable connected closed $n$-manifold has $H_n(M;\mathbb Z)=0$ and $H^n(M;\mathbb Z)=\mathbb Z/2$.

###### Second homology of a closed nonorientable three-manifold

↑ **Parent:** [Poincare duality with the orientation local system](#poincare-duality-with-the-orientation-local-system)

Zero [Euler characteristic](homology.md#euler-characteristic) and $H_3=0$ give free rank $b_1-1$. The [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) identifies $H^3(M;\mathbb Z)=\mathbb Z/2$ with $\operatorname{Ext}(H_2(M;\mathbb Z),\mathbb Z)$, so the only torsion in $H_2$ is one copy of $\mathbb Z/2$. In particular $b_1\geq1$.

##### Intersection pairing on an oriented surface

↑ **Parent:** [Poincare duality](#poincare-duality)

Represent one-dimensional [homology classes](homology.md#homology-class) on a closed oriented [topological surface](topology.md#topological-surface) by transverse oriented curves and sum their signed crossing points. This gives a [bilinear form](linear-algebra.md#bilinear-form) that is skew-symmetric. A symplectic handle basis has matrix $\begin{pmatrix}0&I_g\\-I_g&0\end{pmatrix}$, which is unimodular. In particular, a class detected with intersection $1$ or $-1$ by another integral class is a [primitive homology class](homology.md#primitive-homology-class): the detecting homomorphism splits its rank-one subgroup.

##### Mod-two Poincare duality

↑ **Parent:** [Poincare duality](#poincare-duality)

For a closed $n$-dimensional [manifold](topology.md#topological-manifold), [Poincare duality](#poincare-duality) holds over $\mathbb F_2$ without an [orientation](algebraic-topology.md#orientation-of-a-simplex) assumption. The mod-two [fundamental class](#fundamental-class) exists because orientation signs disappear. The resulting complementary-degree [intersection pairing](homology.md#intersection-pairing) is a [perfect pairing](linear-algebra.md#perfect-pairing).

##### Euler characteristic parity in dimensions congruent to two modulo four

↑ **Parent:** [Poincare duality](#poincare-duality)

For a closed oriented [manifold](topology.md#topological-manifold) of dimension $4r+2$, [Poincare duality](#poincare-duality) pairs all rational [Betti numbers](homology.md#betti-number) except the middle one, making their total contribution to the [Euler characteristic](homology.md#euler-characteristic) even. The middle cohomology degree is odd, so its nondegenerate [Poincare duality pairing](#poincare-duality-pairing) is an [alternating bilinear form](linear-algebra.md#alternating-bilinear-form) and has even dimension. Hence the Euler characteristic is even. Nonorientable manifolds can have odd Euler characteristic, as [Real projective space](algebraic-topology.md#real-projective-space) of even dimension demonstrates.

###### Every even integer is the Euler characteristic of a closed oriented six-manifold

↑ **Parent:** [Euler characteristic parity in dimensions congruent to two modulo four](#euler-characteristic-parity-in-dimensions-congruent-to-two-modulo-four)

Take a [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) of $r$ copies of [Complex projective space](algebraic-topology.md#complex-projective-space) $\mathbb {CP}^3$ and $s$ copies of $S^3\times S^3$, with the empty sum interpreted as $S^6$. Their [Euler characteristics](homology.md#euler-characteristic) are four, zero and two, respectively. Removing a six-ball subtracts one from the Euler characteristic and gluing along its boundary $S^5$ subtracts zero, so each connected sum subtracts two. The result is $2+2r-2s$. For any even integer $n$, choose $r=\max(n/2-1,0)$ and $s=\max(1-n/2,0)$.

##### Cohomological pushforward between closed oriented manifolds

↑ **Parent:** [Poincare duality](#poincare-duality)

For a map between closed oriented manifolds of the same dimension, [Poincare duality](#poincare-duality) turns homological pushforward into a degree-preserving map on [cohomology](cohomology.md). It is adjoint to pullback under the duality pairing: $\langle f^!a\smile b,[N]\rangle=\langle a\smile f^*b,[M]\rangle$. If $f$ has degree $d$, nondegeneracy gives $f^!f^*=d\,\mathrm{id}$. Maps of different dimensions require the corresponding degree shift.

##### Poincare duality pairing

↑ **Parent:** [Poincare duality](#poincare-duality)

For a closed oriented $d$-dimensional [manifold](topology.md#topological-manifold) over a [field](algebra.md#field) $F$, the [cup product](#cup-product) pairing

$$
H^q(M;F)\times H^{d-q}(M;F)\to F,\qquad (a,b)\mapsto\langle a\smile b,[M]_F\rangle
$$

is a [perfect pairing](linear-algebra.md#perfect-pairing) between complementary degrees. The [cap product](#cap-product) with the [fundamental class](#fundamental-class) is an [isomorphism](algebra.md#isomorphism) by [Poincare duality](#poincare-duality), and the [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) over $F$ identifies the complementary [cohomology](cohomology.md) with the full [dual space](linear-algebra.md#dual-space) of the resulting [homology](homology.md). Evaluation is therefore a perfect pairing. Taking the top-degree part of the same formula defines a nondegenerate [bilinear form](linear-algebra.md#bilinear-form) on the full graded [cohomology](cohomology.md). A boundary requires relative groups and [Poincare-Lefschetz duality](#lefschetz-duality) instead.

###### Even rank of middle cohomology in dimension four k plus two

↑ **Parent:** [Poincare duality pairing](#poincare-duality-pairing)

For a closed oriented manifold, the rational middle-dimensional cup-product pairing is nondegenerate by [Poincare duality](#poincare-duality). Its degree is odd, so graded commutativity makes it skew-symmetric. A nondegenerate skew-symmetric form has even dimension. In particular a closed oriented six-manifold cannot have a rank-one third cohomology group.

// Target: algebra.bigb

##### Cohomological injectivity of a map of invertible degree

↑ **Parent:** [Poincare duality](#poincare-duality)

If $f:M\to N$ is a map between closed connected oriented manifolds of the same dimension and its degree is nonzero in a coefficient field $F$, then $f^*:H^*(N;F)\to H^*(M;F)$ is injective. For a nonzero class $a$, [Poincare duality](#poincare-duality) supplies $b$ with $\langle a\smile b,[N]\rangle\ne0$, and naturality gives

$$
\langle f^*a\smile f^*b,[M]\rangle=(\deg f)\langle a\smile b,[N]\rangle\ne0.
$$

##### Lefschetz duality

↑ **Parent:** [Poincare duality](#poincare-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lefschetz_duality)

For a compact oriented $n$-manifold $W$ with boundary, cap product with its relative [fundamental class](#fundamental-class) gives

$$
H^q(W;R)\cong H_{n-q}(W,\partial W;R),\qquad H^q(W,\partial W;R)\cong H_{n-q}(W;R).
$$

###### Mod-two handle duality

↑ **Parent:** [Lefschetz duality](#lefschetz-duality)

Reverse a [handle decomposition](topology.md#handle-decomposition) of a compact $n$-dimensional [manifold](topology.md#topological-manifold). Absolute $k$-handles become relative $(n-k)$-handles based on the boundary. The absolute boundary matrices count [attaching sphere](topology.md#attaching-sphere)-[belt sphere](topology.md#belt-sphere) intersections; the corresponding relative matrices are their transposes over $\mathbb F_2$. The absolute [chain complex](homology.md#chain-complex) is thus the complementary-degree dual of the relative [chain complex](homology.md#chain-complex). The [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) proves [Poincare-Lefschetz duality](#lefschetz-duality) without an [orientation](algebraic-topology.md#orientation-of-a-simplex) hypothesis.

##### Poincare dual

↑ **Parent:** [Poincare duality](#poincare-duality)

For an oriented codimension-$r$ closed submanifold $Y\subset M$, its Poincare dual is the class in $H^r(M)$ whose cup-product evaluation against any complementary class equals intersection with $Y$.

###### Compactly supported dual of a compact submanifold

↑ **Parent:** [Poincare dual](#poincare-dual)

For a compact oriented submanifold without boundary in an oriented [manifold](topology.md#topological-manifold), the normal [Thom class](fiber-bundle.md#thom-class) gives a [compactly supported cohomology](#compactly-supported-cohomology) class dual to its pushed-forward [fundamental class](#fundamental-class). It is independent of the [tubular neighborhood](differential-geometry.md#tubular-neighborhood) and its ordinary-cohomology image vanishes on the complement of the submanifold. A noncompact submanifold closed only as a subset generally has its dual in ordinary cohomology, using locally finite homology instead.

##### Cap-product support lemma for a two-set cover

↑ **Parent:** [Poincare duality](#poincare-duality)

If a closed oriented manifold is covered by two open sets and a positive-degree cohomology class restricts to zero on both, then its cap product with the fundamental class vanishes in every degree strictly below the top. A chain proof uses the small simplex theorem and replaces the two restricted cocycles by coboundaries.

##### Cohomological injectivity of a degree-one map

↑ **Parent:** [Poincare duality](#poincare-duality)

A degree-one map $f:M\to N$ between closed connected oriented manifolds of the same dimension induces an injection $f^*:H^*(N;R)\to H^*(M;R)$. The wrong-way map defined using [Poincare duality](#poincare-duality) is a left inverse by the projection formula and $f_*[M]=[N]$.

##### Homology sphere

↑ **Parent:** [Poincare duality](#poincare-duality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homology_sphere)

An integral homology $d$-sphere is a space with the same integral homology as $S^d$. Removing one point from a closed oriented integral homology sphere produces an acyclic space by the long exact sequence of the pair and the local orientation isomorphism in degree $d$.

###### Simply connected closed three-manifolds are homology spheres

↑ **Parent:** [Homology sphere](#homology-sphere)

A simply connected closed three-dimensional [manifold](topology.md#topological-manifold) is orientable, since its orientation monodromy factors through its trivial [fundamental group](algebraic-topology.md#fundamental-group). Its first integral homology is the [abelianization](group-theory.md#abelianization) of that fundamental group and is zero. The [universal coefficient theorem for cohomology](#universal-coefficient-theorem-for-cohomology) gives $H^1(M;\mathbb Z)=0$, and [Poincare duality](#poincare-duality) gives $H_2=0$, $H_3=\mathbb Z$. Connectedness gives $H_0=\mathbb Z$, and duality gives zero homology above dimension three. Thus it is an integral [homology sphere](#homology-sphere), without needing any homeomorphism classification.

###### Homotopy sphere

↑ **Parent:** [Homology sphere](#homology-sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homotopy_sphere)

A [homotopy](algebraic-topology.md#homotopy) [sphere](geometry-and-topology.md#sphere) is a closed [manifold](topology.md#topological-manifold) with the [homotopy type](algebraic-topology.md#homotopy-type) of a [sphere](geometry-and-topology.md#sphere) of the same dimension. In dimensions at least two, a closed [simply connected](algebraic-topology.md#simply-connected-space) [integral homology sphere](#homology-sphere) is a [homotopy](algebraic-topology.md#homotopy) [sphere](geometry-and-topology.md#sphere): successive applications of the [Hurewicz theorem](algebraic-topology.md#hurewicz-theorem) produce a map from the [sphere](geometry-and-topology.md#sphere) inducing an [isomorphism](algebra.md#isomorphism) on integral [homology](homology.md), and the [homological Whitehead theorem](algebraic-topology.md#homological-whitehead-theorem) makes it a [homotopy equivalence](algebraic-topology.md#homotopy-equivalence). The [topological generalized Poincare theorem](#topological-generalized-poincare-theorem) identifies its topological type, while prescribed smooth structures require a separate question.

###### Topological generalized Poincare theorem

↑ **Parent:** [Homotopy sphere](#homotopy-sphere)

Every closed [topological manifold](topology.md#topological-manifold) with the [homotopy type](algebraic-topology.md#homotopy-type) of $S^d$ is homeomorphic to $S^d$. This is a classification theorem about [homeomorphisms](topology.md#homeomorphism), and does not assert a [diffeomorphism](geometry-and-topology.md#diffeomorphism) between prescribed smooth structures. It is the precise final step needed after proving that a cone link is a [simply connected](algebraic-topology.md#simply-connected-space) [integral homology sphere](#homology-sphere) in the [manifold criterion for a suspension](algebraic-topology.md#manifold-criterion-for-a-suspension).

## Cup product

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cup_product)

The cup product is a natural bilinear operation $H^p(X;R)\times H^q(X;R)\to H^{p+q}(X;R)$. It is graded-commutative: $a\smile b=(-1)^{pq}b\smile a$.

### Cup power

↑ **Parent:** [Cup product](#cup-product)

For a [cohomology class](#cohomology-class) $a$, its rth cup power is its r-fold product in the [cohomology ring](#cohomology-ring). Naturality gives $f^*(a^r)=(f^*a)^r$. A nilpotent class has some positive cup power zero; the nilpotence order is preserved by ring isomorphisms and can obstruct a [homotopy equivalence](algebraic-topology.md#homotopy-equivalence) or a nonzero [mapping degree](homology.md#degree-of-a-continuous-mapping).

### Cohomological cross product

↑ **Parent:** [Cup product](#cup-product)

The cross product takes classes on two factors to a class on their product. Its multiplication rule has the [graded tensor product](commutative-algebra.md#graded-tensor-product) sign: $(a\times b)(c\times d)=(-1)^{|b||c|}(ac)\times(bd)$. The [Künneth theorem](#kunneth-theorem) makes these products an additive basis when the integral cohomology of the finite cell complexes is torsion-free.

### Cup length

↑ **Parent:** [Cup product](#cup-product)

The largest number of positive-degree [cohomology classes](#cohomology-class) whose [cup product](#cup-product) is nonzero, with a specified coefficient ring $R$; it can be infinite. It is zero if there is no nonzero positive-degree class. The [vanishing cup product from an open cover](#vanishing-cup-product-from-an-open-cover) argument implies that [Lusternik–Schnirelmann category](algebraic-topology.md#lusternik-schnirelmann-category) is at least cup length plus one. For [Complex projective space](algebraic-topology.md#complex-projective-space) $\mathbb{CP}^r$, its integral cup length is $r$.

### Relative cup product

↑ **Parent:** [Cup product](#cup-product)

For open subsets $U,V$ of a [topological space](topology.md#topological-space) $Y$, the relative [cup product](#cup-product) gives

$$
H^p(Y,U;R)\otimes H^q(Y,V;R)\longrightarrow H^{p+q}(Y,U\cup V;R).
$$

Compatibility with the maps to absolute [cohomology](cohomology.md) identifies its image with the ordinary cup product. More generally the construction requires an excisive pair of subsets. The open-set case can be proved using subdivision to compute on chains subordinate to the open cover.

#### Nilpotence from a contractible subcomplex cover

↑ **Parent:** [Relative cup product](#relative-cup-product)

If a pointed CW complex is covered by $l$ contractible subcomplexes containing the basepoint, every reduced class lifts to a relative class for each appropriate subcomplex. Their [relative cup product](#relative-cup-product) lies in $h^*(X,\bigcup_jA_j)=h^*(X,X)=0$, so every product of $l$ reduced classes vanishes. The conclusion also holds if $X$ is path connected. Without either condition a two-point space covered by its two points is a counterexample in ordinary degree-zero cohomology.

#### Vanishing cup product from an open cover

↑ **Parent:** [Relative cup product](#relative-cup-product)

Let $U_1,\ldots,U_k$ be an open cover of $Y$, and suppose $\alpha_i\in H^{d_i}(Y;R)$ restricts to zero on $U_i$. The pair [long exact sequence](homology.md#long-exact-sequence) lifts each $\alpha_i$ to $H^{d_i}(Y,U_i;R)$. Their [relative cup product](#relative-cup-product) lies in $H^{\sum d_i}(Y,\bigcup_iU_i;R)=H^{\sum d_i}(Y,Y;R)=0$, so $\alpha_1\smile\cdots\smile\alpha_k=0$. This proves characteristic-class products vanish from local trivializations without cancelling possible zero divisors in the coefficient ring.

### Graded commutativity of the cup product

↑ **Parent:** [Cup product](#cup-product)

Homogeneous cohomology classes satisfy

$$
a\smile b=(-1)^{|a||b|}b\smile a.
$$

In particular, an odd-degree class has square killed by two, and its square vanishes whenever two is invertible in the coefficient ring.

### Exterior product in cohomology

↑ **Parent:** [Cup product](#cup-product)

For projections $p_X:X\times Y\to X$ and $p_Y:X\times Y\to Y$, the exterior product is

$$
a\times b=p_X^*a\smile p_Y^*b.
$$

The same definition gives $H^p(X,A;R)\otimes H^q(Y;R)\to H^{p+q}(X\times Y,A\times Y;R)$.

### Cohomology ring

↑ **Parent:** [Cup product](#cup-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cohomology_ring)

The cohomology ring is the graded ring whose multiplication is the [cup product](#cup-product). It records intersection information that the graded cohomology groups alone do not detect.

#### Degree-one cup-square obstruction to ring isomorphism

↑ **Parent:** [Cohomology ring](#cohomology-ring)

The property that every degree-one element has square zero is invariant under a graded ring isomorphism. Over $\mathbb F_2$ it distinguishes the [cohomology ring of a torus](topology.md#cohomology-ring-of-a-torus) from the [mod-two cohomology ring of an inversion mapping torus](algebraic-topology.md#mod-two-cohomology-ring-of-an-inversion-mapping-torus) of dimension at least two.

#### Cohomology ring of a product of two spheres

↑ **Parent:** [Cohomology ring](#cohomology-ring)

For positive $n$, let $x,y$ be the pullbacks of the orientation classes from the two factors. Then $x^2=y^2=0$, $xy$ generates degree $2n$, and $yx=(-1)^nxy$. When $n$ is even, every graded ring automorphism restricts on $H^n$ to a signed permutation matrix; when $n$ is odd the ring admits every matrix in $GL_2(\mathbb Z)$.

##### Cohomology ring of a product of unequal-dimensional spheres

↑ **Parent:** [Cohomology ring of a product of two spheres](#cohomology-ring-of-a-product-of-two-spheres)

For positive unequal dimensions $p,q$, let $u,v$ be the pullbacks of the integral orientation classes of the factors. The [Künneth theorem](#kunneth-theorem) gives the free abelian basis $1,u,v,uv$, with degrees $0,p,q,p+q$. The products satisfy $u^2=v^2=0$ and $vu=(-1)^{pq}uv$, by naturality and [graded commutativity of the cup product](#graded-commutativity-of-the-cup-product). In particular, for $p=2,q=4$, the [cohomology ring](#cohomology-ring) is $\mathbb Z[u,v]/(u^2,v^2)$, with degrees two and four.

##### Cup square after a diagonal sphere attachment

↑ **Parent:** [Cohomology ring of a product of two spheres](#cohomology-ring-of-a-product-of-two-spheres)

For even $n\ge2$, attach an $(n+1)$-cell to $S^n\times S^n$ along the diagonal. The [cellular chain complex](homology.md#cellular-chain-complex) has boundary $(1,1)$ for the new cell. The degree-$n$ [cohomology](cohomology.md) generator restricts to $a-b$, and the top generator restricts to $ab$. Naturality of the [cup product](#cup-product) therefore gives $u^2=-2v$, since $(a-b)^2=-2ab$. Thus the resulting [cohomology ring](#cohomology-ring) is $\mathbb Z[u,v]/(u^2+2v,uv,v^2)$, with $|u|=n$ and $|v|=2n$. This distinguishes the attachment from a wedge of spheres, whose positive-degree products vanish.

#### Mod-p cup-square obstruction to a homotopy equivalence

↑ **Parent:** [Cohomology ring](#cohomology-ring)

Two finite [CW complexes](algebraic-topology.md#cw-complex) can have isomorphic integral [cohomology rings](#cohomology-ring) but different cohomology rings modulo $p$. For example, attaching a three-cell of degree $p$ to the projective line in $\mathbb{CP}^2$ preserves the nonzero square of the degree-two class modulo $p$, whereas the corresponding [Moore space](algebraic-topology.md#moore-space-algebraic-topology) wedged with $S^4$ has zero square. The spaces therefore cannot be [homotopy equivalent](algebraic-topology.md#homotopy-inverse).

#### Cohomology ring of a closed oriented surface

↑ **Parent:** [Cohomology ring](#cohomology-ring)

Choose degree-one classes $\alpha_i,\beta_i$ dual to a symplectic basis of one-cycles and let $\omega$ generate $H^2(\Sigma_g;\mathbb Z)$. The only nonzero products of positive-degree basis elements are

$$
\alpha_i\smile\beta_j=\delta_{ij}\omega,
\qquad
\beta_j\smile\alpha_i=-\delta_{ij}\omega.
$$

<h2 id="kunneth-theorem">Künneth theorem</h2>

↑ **Parent:** [Cohomology](cohomology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Künneth_theorem)

For chain complexes of free modules over a principal ideal domain $R$, the Künneth theorem gives a natural split short exact sequence

$$
0\to\bigoplus_{i+j=n}H_i(C)\otimes_RH_j(D)\to H_n(C\otimes_RD)\to\bigoplus_{i+j=n-1}\operatorname{Tor}_1^R(H_i(C),H_j(D))\to0,
$$

although the splitting is not natural. Over a field the Tor term vanishes, and the cohomological cross product gives $H^*(X\times Y;k)\cong H^*(X;k)\otimes_kH^*(Y;k)$ as graded rings under standard finiteness hypotheses.

### Cohomology cross product

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

For classes on $X$ and $Y$, apply the [induced maps on cohomology](#induced-map-on-cohomology) of the coordinate projections and take their [cup product](#cup-product) on $X\times Y$. The result has degree $|a|+|b|$. On a [tensor product](linear-algebra.md#tensor-product) of graded rings, the sign rule $(a\otimes b)(c\otimes d)=(-1)^{|b||c|}ac\otimes bd$ makes this a ring homomorphism.

<h3 id="cohomological-kunneth-theorem-over-a-field">Cohomological Künneth theorem over a field</h3>

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

If $k$ is a [field](algebra.md#field) and $H^*(F;k)$ has finite total dimension, the [cohomology cross product](#cohomology-cross-product) gives the displayed graded-ring [isomorphism](algebra.md#isomorphism) for arbitrary spaces. Over a [field](algebra.md#field), every chain complex splits into its [homology](homology.md) with zero differential and contractible summands. The [Eilenberg–Zilber theorem](#eilenberg-zilber-theorem) thus replaces the fiber chain complex by a bounded finite-dimensional complex; dualizing its tensor product with $C_*(X;k)$ gives a finite direct sum of shifted cochain complexes of $X$. Its cohomology is the displayed tensor product. Finiteness prevents the infinite-product obstruction that can occur for two infinite discrete spaces. The standard product formula and its finiteness hypothesis are discussed in [https://pi.math.cornell.edu/~hatcher/AT/ATch3.pdf,](https://pi.math.cornell.edu/~hatcher/AT/ATch3.pdf,) Theorem 3.15.

<h3 id="integral-cohomological-kunneth-theorem-for-finite-cell-complexes">Integral cohomological Künneth theorem for finite cell complexes</h3>

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

For finite cell complexes, the cohomological cross product gives a split, but not naturally split, short exact sequence $0\to\bigoplus_{p+q=n}H^p(X;\mathbb Z)\otimes H^q(Y;\mathbb Z)\to H^n(X\times Y;\mathbb Z)\to\bigoplus_{p+q=n+1}\operatorname{Tor}_1(H^p(X;\mathbb Z),H^q(Y;\mathbb Z))\to0$. The Tor degree is $n+1$ for cohomology, unlike the $n-1$ shift in the homological version. If one factor's cohomology is free, the Tor term vanishes and the resulting ring is the [graded tensor product](commutative-algebra.md#graded-tensor-product).

### Diagonal-degree obstruction to a symmetric sphere retraction

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

For $d\geq1$ and $n>1$, no factor-permutation-invariant map $f:(S^d)^n\to S^d$ restricts to the identity on the diagonal. The [Künneth theorem](#kunneth-theorem) makes the degree-$d$ [cohomology](cohomology.md) a direct sum of $n$ copies of $\mathbb Z$. Symmetry forces $f^*\alpha=a\sum_i u_i$ for one integer $a$. Pulling back to the diagonal multiplies this coefficient by $n$, so the identity restriction would give $na=1$. The contradiction uses integral coefficients and applies in both even and odd sphere dimensions.

### Homology cross product

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

The singular-chain product induces this natural pairing on [homology](homology.md). Composing it with multiplication of a loop space gives the [Pontryagin product on loop-space homology](algebraic-topology.md#pontryagin-product-on-loop-space-homology). This is different from the vector [cross product](vector-space.md#cross-product).

<h4 id="eilenberg-zilber-theorem">Eilenberg–Zilber theorem</h4>

↑ **Parent:** [Homology cross product](#homology-cross-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eilenberg–Zilber_theorem)

The [singular chain complex](homology.md#singular-chain-complex) of a product is naturally chain-homotopy equivalent to the [tensor product](linear-algebra.md#tensor-product) of the factors' chain complexes. The shuffle map and the front-face/back-face map implement the equivalence. It is the chain-level input to the [Künneth theorem](#kunneth-theorem).

<h3 id="integral-kunneth-torsion-polynomial">Integral Künneth torsion polynomial</h3>

↑ **Parent:** [Künneth theorem](#kunneth-theorem)

For spaces whose integral [cohomology](cohomology.md) has only free and $\mathbb Z/2$ summands, let $F$ encode free ranks and $T$ count order-two summands by degree. An additively split integral [Künneth theorem](#kunneth-theorem) gives $F_{A\times B}=F_AF_B$ and the displayed rule for $T$. The $t^{-1}$ term is the cohomological degree shift of the [Tor functor](algebra.md#tor-functor) contribution. The formula requires this torsion type and the usual finite-type hypotheses.

## ↑ Ancestors (5)

1. [Algebraic topology](algebraic-topology.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (160)

- [Bockstein cohomology](homology.md#bockstein-cohomology)
- [Cellular cohomology](homology.md#cellular-cohomology)
- [Chevalley–Eilenberg cochains of a graded Lie algebra](lie-algebra.md#chevalley-eilenberg-cochains-of-a-graded-lie-algebra)
- [Cochain homotopy](homology.md#cochain-homotopy)
- [Cochain map](algebra.md#cochain-map)
- [Cohomological pushforward between closed oriented manifolds](#cohomological-pushforward-between-closed-oriented-manifolds)
- [Cohomology class of a cooriented submanifold](fiber-bundle.md#cohomology-class-of-a-cooriented-submanifold)
- [Cohomology ring of a Hopf attachment with a sphere summand](algebraic-topology.md#cohomology-ring-of-a-hopf-attachment-with-a-sphere-summand)
- [Cohomology sheaf](ringed-space.md#cohomology-sheaf)
- [Cohomology-sheaf exact sequence](ringed-space.md#cohomology-sheaf-exact-sequence)
- [Cohomology suspension](algebraic-topology.md#cohomology-suspension)
- [Compact first-cohomology obstruction to a Lagrangian fibration](symplectic-geometry.md#compact-first-cohomology-obstruction-to-a-lagrangian-fibration)
- [Complement homology of a compact codimension-zero submanifold](#complement-homology-of-a-compact-codimension-zero-submanifold)
- [Connected sum of oriented manifolds](differential-geometry.md#connected-sum-of-oriented-manifolds)
- [Costalk](ringed-space.md#costalk)
- [Cup-power obstruction to nonzero degree](homology.md#cup-power-obstruction-to-nonzero-degree)
- [Cup square after a diagonal sphere attachment](#cup-square-after-a-diagonal-sphere-attachment)
- [de Rham cohomology of a finite quotient](differential-form.md#de-rham-cohomology-of-a-finite-quotient)
- [Degree-one maps between closed oriented surfaces](homology.md#degree-one-maps-between-closed-oriented-surfaces)
- [Diagonal-degree obstruction to a symmetric sphere retraction](#diagonal-degree-obstruction-to-a-symmetric-sphere-retraction)
- [Differential graded algebra](commutative-algebra.md#differential-graded-algebra)
- [Equivariant cohomology](#equivariant-cohomology)
- [Excess of an admissible Steenrod sequence](#excess-of-an-admissible-steenrod-sequence)
- [Ext functor](algebra.md#ext-functor)
- [First Chern class of a tensor product of complex line bundles](complex-geometry.md#first-chern-class-of-a-tensor-product-of-complex-line-bundles)
- [Formal space](algebraic-topology.md#formal-space)
- [Generalized cohomology theory](#generalized-cohomology-theory)
- [Graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule)
- [Grauert base change theorem](ringed-space.md#grauert-base-change-theorem)
- [Group cohomology commutes with finite direct sums](group-theory.md#group-cohomology-commutes-with-finite-direct-sums)
- [Gysin ring splitting for an odd-dimensional sphere bundle](fiber-bundle.md#gysin-ring-splitting-for-an-odd-dimensional-sphere-bundle)
- [Homological algebra](algebra.md#homological-algebra)
- [Homotopy invariance of cohomology](#homotopy-invariance-of-cohomology)
- [Hopf invariant](algebraic-topology.md#hopf-invariant)
- [Hopf trace identity](homology.md#hopf-trace-identity)
- [Hypercohomology](ringed-space.md#hypercohomology)
- [Infinite-dimensional real projective space](algebraic-topology.md#infinite-dimensional-real-projective-space)
- [Integral Bockstein homomorphism](homology.md#integral-bockstein-homomorphism)
- [Integral cohomology](#integral-cohomology)
- [Integral Künneth torsion polynomial](#integral-kunneth-torsion-polynomial)
- [Intersection complex](algebraic-topology.md#intersection-complex)
- [Intersection-complex support and cosupport axioms](algebraic-topology.md#intersection-complex-support-and-cosupport-axioms)
- [Inversion mapping torus of a torus](algebraic-topology.md#inversion-mapping-torus-of-a-torus)
- [K3 intersection lattice](complex-geometry.md#k3-intersection-lattice)
- [Leray-Hirsch theorem](fiber-bundle.md#leray-hirsch-theorem)
- [Local basis criterion for Leray-Hirsch classes](fiber-bundle.md#local-basis-criterion-for-leray-hirsch-classes)
- [Long exact cohomology sequence of a pair](#long-exact-cohomology-sequence-of-a-pair)
- [Long exact sequence](homology.md#long-exact-sequence)
- [Minimal model of a wedge of simply connected spheres](algebraic-topology.md#minimal-model-of-a-wedge-of-simply-connected-spheres)
- [Mod-p cohomology ring of a cyclic group](group-theory.md#mod-p-cohomology-ring-of-a-cyclic-group)
- [Mod-two cohomology ring of the antipodal two-sphere mapping torus](algebraic-topology.md#mod-two-cohomology-ring-of-the-antipodal-two-sphere-mapping-torus)
- [Mod-two intersection pairing of the Klein bottle](topology.md#mod-two-intersection-pairing-of-the-klein-bottle)
- [Moduli space of Ricci-flat K3 metrics](complex-geometry.md#moduli-space-of-ricci-flat-k3-metrics)
- [Naturality of the cap product](#naturality-of-the-cap-product)
- [One-cell bound on next-degree cohomology](homology.md#one-cell-bound-on-next-degree-cohomology)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-22.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-18.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-18.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-21.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-21.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-22.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-22.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-57.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-16.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-5.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#5/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#5/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-12.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-15.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-18.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-142.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-142.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-142.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151.md#4/solution)
- [Periodic group cohomology from a free sphere action](group-theory.md#periodic-group-cohomology-from-a-free-sphere-action)
- [Poincare duality pairing](#poincare-duality-pairing)
- [Pontryagin class](geometry-and-topology.md#pontryagin-class)
- [Pontryagin ring of an odd-sphere loop space](algebraic-topology.md#pontryagin-ring-of-an-odd-sphere-loop-space)
- [Projective bundle formula for complex vector bundles](fiber-bundle.md#projective-bundle-formula-for-complex-vector-bundles)
- [Proper base change for sheaves](ringed-space.md#proper-base-change-for-sheaves)
- [Rank bound for a nonsingular complex bilinear map](linear-algebra.md#rank-bound-for-a-nonsingular-complex-bilinear-map)
- [Rational homotopy type](algebraic-topology.md#rational-homotopy-type)
- [Rational model of a collapsed complex projective subspace](algebraic-topology.md#rational-model-of-a-collapsed-complex-projective-subspace)
- [Rational polynomial differential forms](algebraic-topology.md#rational-polynomial-differential-forms)
- [Rationalization of a topological space](algebraic-topology.md#rationalization-of-a-topological-space)
- [Reduced cohomology](#reduced-cohomology)
- [Relative cohomology](#relative-cohomology)
- [Relative cup product](#relative-cup-product)
- [Relative homology of a surface modulo disjoint circles](homology.md#relative-homology-of-a-surface-modulo-disjoint-circles)
- [Representability of cohomology by Eilenberg–MacLane spaces](algebraic-topology.md#representability-of-cohomology-by-eilenberg-maclane-spaces)
- [Retraction onto a punctured oriented surface](topology.md#retraction-onto-a-punctured-oriented-surface)
- [Second Chern class of a tensor product of rank-two bundles](fiber-bundle.md#second-chern-class-of-a-tensor-product-of-rank-two-bundles)
- [Singular cohomology](#singular-cohomology)
- [Spectral sequence](algebra.md#spectral-sequence)
- [Stiefel–Whitney obstruction to a diagonal projective immersion](fiber-bundle.md#stiefel-whitney-obstruction-to-a-diagonal-projective-immersion)
- [Stunted real projective space](algebraic-topology.md#stunted-real-projective-space)
- [Sullivan minimal model](algebraic-topology.md#sullivan-minimal-model)
- [Sullivan minimal-model classification](algebraic-topology.md#sullivan-minimal-model-classification)
- [Sullivan model of the connected sum of two complex projective planes](algebraic-topology.md#sullivan-model-of-the-connected-sum-of-two-complex-projective-planes)
- [Surjective rational Hurewicz homomorphism gives a wedge of spheres](algebraic-topology.md#surjective-rational-hurewicz-homomorphism-gives-a-wedge-of-spheres)
- [Total cochain complex](homology.md#total-cochain-complex)
