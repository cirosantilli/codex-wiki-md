# Homology (mathematics)

↑ **Parent:** [Algebraic topology](algebraic-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homology_(mathematics))

Homology assigns abelian groups $H_i(X)$ to a space, measuring cycles modulo boundaries in each dimension.

**Table of contents**

- [Borel-Moore homology](#borel-moore-homology)
- [Generalized homology theory](#generalized-homology-theory)
  - [Represented homology theory](#represented-homology-theory)
- [Null-homologous cycle](#null-homologous-cycle)
- [Primitive homology class](#primitive-homology-class)
- [Acyclic space](#acyclic-space)
- [Homology of a directed union](#homology-of-a-directed-union)
  - [Countability of the homology of an open Euclidean subset](#countability-of-the-homology-of-an-open-euclidean-subset)
- [Reduced homology](#reduced-homology)
- [Homology group](#homology-group)
  - [Zeroth homology group](#zeroth-homology-group)
  - [Homology class](#homology-class)
- [Functoriality of homology](#functoriality-of-homology)
  - [Homotopy invariance of homology](#homotopy-invariance-of-homology)
    - [Singular prism operator](#singular-prism-operator)
- [First homology](#first-homology)
- [Singular homology](#singular-homology)
  - [Singular chain complex](#singular-chain-complex)
  - [Small singular chains for an open cover](#small-singular-chains-for-an-open-cover)
  - [Local coefficient system](#local-coefficient-system)
    - [Orientation local system](#orientation-local-system)
  - [Betti number](#betti-number)
    - [Poincaré polynomial](#poincare-polynomial)
  - [Singular chain](#singular-chain)
    - [Singular chain group](#singular-chain-group)
  - [Singular simplex](#singular-simplex)
- [Intersection form](#intersection-form)
  - [Rank-one intersection form and the projective-plane cohomology ring](#rank-one-intersection-form-and-the-projective-plane-cohomology-ring)
  - [Positive index of the intersection form](#positive-index-of-the-intersection-form)
  - [Intersection form of a product of two closed oriented surfaces](#intersection-form-of-a-product-of-two-closed-oriented-surfaces)
  - [Unimodular intersection pairing](#unimodular-intersection-pairing)
  - [Novikov additivity](#novikov-additivity)
  - [Intersection pairing](#intersection-pairing)
    - [Intersection matrix](#intersection-matrix)
    - [Coordinate sphere intersection basis](#coordinate-sphere-intersection-basis)
    - [Half-lives-half-dies theorem](#half-lives-half-dies-theorem)
  - [Degree constraint from intersection forms](#degree-constraint-from-intersection-forms)
  - [Real de Rham intersection form in dimension four](#real-de-rham-intersection-form-in-dimension-four)
    - [Signature of the intersection form from harmonic duality](#signature-of-the-intersection-form-from-harmonic-duality)
- [Integral homology](#integral-homology)
- [Homology of a sphere](#homology-of-a-sphere)
  - [Homology of an equatorial sphere complement](#homology-of-an-equatorial-sphere-complement)
- [Degree of a continuous mapping](#degree-of-a-continuous-mapping)
  - [Mod-two degree of a map between closed manifolds](#mod-two-degree-of-a-map-between-closed-manifolds)
  - [Nonzero degree from a sphere obstructs manifold products](#nonzero-degree-from-a-sphere-obstructs-manifold-products)
  - [Degrees of maps of the zero-sphere](#degrees-of-maps-of-the-zero-sphere)
  - [Relative mapping degree](#relative-mapping-degree)
    - [Graph intersection formula for mapping degree](#graph-intersection-formula-for-mapping-degree)
    - [Quotient-sphere degree identity](#quotient-sphere-degree-identity)
  - [Local degree of a continuous map](#local-degree-of-a-continuous-map)
    - [Local degrees of arbitrary integer value](#local-degrees-of-arbitrary-integer-value)
    - [Degree as a sum of local degrees](#degree-as-a-sum-of-local-degrees)
  - [Degree under suspension](#degree-under-suspension)
    - [Sphere maps of arbitrary integer degree](#sphere-maps-of-arbitrary-integer-degree)
  - [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)
    - [Cup-power obstruction to nonzero degree](#cup-power-obstruction-to-nonzero-degree)
    - [Arbitrary-degree maps to a surface of genus two](#arbitrary-degree-maps-to-a-surface-of-genus-two)
    - [Collapse map of degree one onto a sphere](#collapse-map-of-degree-one-onto-a-sphere)
    - [Surjective degree-zero sphere-to-torus map](#surjective-degree-zero-sphere-to-torus-map)
    - [Multiplicativity of mapping degree](#multiplicativity-of-mapping-degree)
    - [Homotopy invariance of mapping degree](#homotopy-invariance-of-mapping-degree)
    - [Degree does not classify general manifold maps](#degree-does-not-classify-general-manifold-maps)
    - [Degree by integration of a pullback volume form](#degree-by-integration-of-a-pullback-volume-form)
    - [Spherical degree by area pullback](#spherical-degree-by-area-pullback)
    - [Degree-one maps between closed oriented surfaces](#degree-one-maps-between-closed-oriented-surfaces)
    - [Prime-degree sphere map forces primary torsion](#prime-degree-sphere-map-forces-primary-torsion)
    - [Degrees of maps factoring through real projective space](#degrees-of-maps-factoring-through-real-projective-space)
  - [Antipodal map](#antipodal-map)
    - [Fixed-point-free sphere maps are homotopic to the antipodal map](#fixed-point-free-sphere-maps-are-homotopic-to-the-antipodal-map)
    - [Odd map between spheres](#odd-map-between-spheres)
      - [Cohomological obstruction to separately odd sphere multiplication](#cohomological-obstruction-to-separately-odd-sphere-multiplication)
      - [Odd maps pull back the real tautological line bundle](#odd-maps-pull-back-the-real-tautological-line-bundle)
    - [Invariant primitive under a finite group action](#invariant-primitive-under-a-finite-group-action)
      - [Top-degree differential forms on even-dimensional real projective space are exact](#top-degree-differential-forms-on-even-dimensional-real-projective-space-are-exact)
  - [Degree of a Euclidean homeomorphism](#degree-of-a-euclidean-homeomorphism)
  - [Degree of a factor swap](#degree-of-a-factor-swap)
- [Relative homology](#relative-homology)
  - [Relative homology of a surface modulo disjoint circles](#relative-homology-of-a-surface-modulo-disjoint-circles)
  - [Relative homology class](#relative-homology-class)
  - [Relative chain complex](#relative-chain-complex)
    - [Relative cycle](#relative-cycle)
    - [Relative simplicial chain complex](#relative-simplicial-chain-complex)
  - [Long exact sequence in relative homology](#long-exact-sequence-in-relative-homology)
  - [Relative homology of a simplex and its boundary](#relative-homology-of-a-simplex-and-its-boundary)
  - [Good pair](#good-pair)
    - [Collapsing a pair theorem](#collapsing-a-pair-theorem)
      - [Collapsing a simple closed curve on a surface](#collapsing-a-simple-closed-curve-on-a-surface)
        - [Homology after collapsing a nonseparating surface curve](#homology-after-collapsing-a-nonseparating-surface-curve)
        - [Homology after collapsing a separating surface curve](#homology-after-collapsing-a-separating-surface-curve)
- [Excision theorem](#excision-theorem)
- [Exact sequence](#exact-sequence)
  - [Long exact sequence](#long-exact-sequence)
- [Commutative diagram](#commutative-diagram)
- [Chain complex](#chain-complex)
  - [Hopf trace identity](#hopf-trace-identity)
  - [Differential of a chain complex](#differential-of-a-chain-complex)
  - [Reversed dual chain complex](#reversed-dual-chain-complex)
  - [Graded Hom complex of chain complexes](#graded-hom-complex-of-chain-complexes)
    - [Sign conjugation for the tensor-Hom identification](#sign-conjugation-for-the-tensor-hom-identification)
  - [Tensor product of chain complexes](#tensor-product-of-chain-complexes)
    - [Koszul sign rule](#koszul-sign-rule)
  - [Disk chain complex](#disk-chain-complex)
  - [Sphere chain complex](#sphere-chain-complex)
  - [Double complex](#double-complex)
    - [Double cochain complex](#double-cochain-complex)
      - [Two spectral sequences of a bounded double complex](#two-spectral-sequences-of-a-bounded-double-complex)
      - [Total cochain complex](#total-cochain-complex)
  - [Koszul complex](#koszul-complex)
    - [Self-duality of the Koszul complex](#self-duality-of-the-koszul-complex)
    - [Koszul acyclicity criterion in a Noetherian local ring](#koszul-acyclicity-criterion-in-a-noetherian-local-ring)
    - [Koszul complex with module coefficients](#koszul-complex-with-module-coefficients)
    - [Koszul homology](#koszul-homology)
      - [Koszul homotopy for multiplication by a generator](#koszul-homotopy-for-multiplication-by-a-generator)
    - [Koszul complex on central ring elements](#koszul-complex-on-central-ring-elements)
  - [Augmented chain complex](#augmented-chain-complex)
  - [Chain group](#chain-group)
  - [Chain subcomplex](#chain-subcomplex)
  - [Boundary operator](#boundary-operator)
  - [Cellular chain complex](#cellular-chain-complex)
    - [Cellular chain group](#cellular-chain-group)
    - [Cellular chain](#cellular-chain)
    - [Cellular cycle](#cellular-cycle)
      - [Cellular boundary](#cellular-boundary)
    - [Cellular chains of a product of finite CW complexes](#cellular-chains-of-a-product-of-finite-cw-complexes)
    - [Homology of a torus with two parallel circles collapsed](#homology-of-a-torus-with-two-parallel-circles-collapsed)
    - [Cellular homology theorem](#cellular-homology-theorem)
    - [Cellular cochain complex](#cellular-cochain-complex)
      - [Cellular cohomology](#cellular-cohomology)
        - [One-cell bound on next-degree cohomology](#one-cell-bound-on-next-degree-cohomology)
        - [Coprime two-cell attachments to a circle](#coprime-two-cell-attachments-to-a-circle)
    - [Cellular boundary formula](#cellular-boundary-formula)
  - [Chain cycle](#chain-cycle)
  - [Chain boundary](#chain-boundary)
  - [Chain coefficient](#chain-coefficient)
  - [Chain map](#chain-map)
    - [Quasi-isomorphism](#quasi-isomorphism)
      - [Prime coefficient detection of quasi-isomorphisms](#prime-coefficient-detection-of-quasi-isomorphisms)
    - [Induced map on homology](#induced-map-on-homology)
    - [Chain homotopy](#chain-homotopy)
      - [Contracting homotopy](#contracting-homotopy)
      - [Cochain homotopy](#cochain-homotopy)
      - [Small simplex theorem](#small-simplex-theorem)
  - [Mapping cone (homological algebra)](#mapping-cone-homological-algebra)
    - [Mapping cone acyclicity criterion](#mapping-cone-acyclicity-criterion)
  - [Short exact sequence of chain complexes](#short-exact-sequence-of-chain-complexes)
    - [Long exact sequence in homology](#long-exact-sequence-in-homology)
      - [Connecting homomorphism](#connecting-homomorphism)
        - [Relative homology connecting homomorphism](#relative-homology-connecting-homomorphism)
        - [Bockstein homomorphism](#bockstein-homomorphism)
          - [Bockstein on infinite real projective space](#bockstein-on-infinite-real-projective-space)
          - [Bockstein factorization through integral cohomology](#bockstein-factorization-through-integral-cohomology)
            - [Degree-one Bockstein square identity](#degree-one-bockstein-square-identity)
            - [Bockstein square-zero identity](#bockstein-square-zero-identity)
              - [Bockstein cohomology](#bockstein-cohomology)
          - [Integral Bockstein homomorphism](#integral-bockstein-homomorphism)
          - [Bockstein isomorphism for a three-dimensional lens space](#bockstein-isomorphism-for-a-three-dimensional-lens-space)
            - [Bockstein linking invariant of a three-dimensional lens space](#bockstein-linking-invariant-of-a-three-dimensional-lens-space)
          - [Bockstein homology](#bockstein-homology)
          - [Long exact sequence from a coefficient sequence](#long-exact-sequence-from-a-coefficient-sequence)
          - [Bockstein derivation rule](#bockstein-derivation-rule)
  - [Elementary decomposition of a finite free chain complex](#elementary-decomposition-of-a-finite-free-chain-complex)
  - [Detection of integral acyclicity modulo primes](#detection-of-integral-acyclicity-modulo-primes)
- [Universal coefficient theorem for homology](#universal-coefficient-theorem-for-homology)
  - [Rational homology](#rational-homology)
- [Simplicial homology](#simplicial-homology)
  - [Simplicial cycle](#simplicial-cycle)
  - [Simplicial chain complex](#simplicial-chain-complex)
    - [Simplicial cone chain contraction](#simplicial-cone-chain-contraction)
  - [Euler characteristic](#euler-characteristic)
    - [Odd-dimensional closed manifolds have zero Euler characteristic](#odd-dimensional-closed-manifolds-have-zero-euler-characteristic)
    - [Euler characteristics of closed oriented four-manifolds](#euler-characteristics-of-closed-oriented-four-manifolds)
    - [Ordinary vertex in a nonconcurrent great-circle arrangement](#ordinary-vertex-in-a-nonconcurrent-great-circle-arrangement)
    - [Euler formula for a sphere](#euler-formula-for-a-sphere)
    - [Euler characteristic of a product](#euler-characteristic-of-a-product)
    - [Euler characteristic under a finite covering](#euler-characteristic-under-a-finite-covering)
    - [Euler characteristic of an odd-dimensional closed manifold](#euler-characteristic-of-an-odd-dimensional-closed-manifold)
    - [Euler-Poincare formula](#euler-poincare-formula)
  - [Barycentric subdivision](#barycentric-subdivision)
    - [Iterated barycentric subdivision](#iterated-barycentric-subdivision)
    - [Mesh of a simplicial complex](#mesh-of-a-simplicial-complex)
    - [Barycentric subdivision of a tetrahedron](#barycentric-subdivision-of-a-tetrahedron)
- [Local homology](#local-homology)
  - [Local homology from a link](#local-homology-from-a-link)
  - [Fixed barycentre of the barycentric tetrahedral two-skeleton](#fixed-barycentre-of-the-barycentric-tetrahedral-two-skeleton)
- [Intersection form of a 4-manifold](#intersection-form-of-a-4-manifold)
- [Universal coefficient theorem](#universal-coefficient-theorem)

## Borel-Moore homology

↑ **Parent:** [Homology (mathematics)](homology.md)

For a locally compact space, replace finite [singular chains](#singular-chain) by chains for which every compact subset meets the images of only finitely many simplices with nonzero coefficients. The [boundary operator](#boundary-operator) preserves this local finiteness, giving the Borel-Moore chain complex and its [homology](homology.md). On a compact space it reduces to ordinary singular homology. A noncompact manifold has a locally finite [fundamental class](cohomology.md#fundamental-class), with its [orientation local system](#orientation-local-system) when necessary. The chain groups and homology are zero in negative degrees.

## Generalized homology theory

↑ **Parent:** [Homology (mathematics)](homology.md)

A [generalized homology theory](#generalized-homology-theory) obeys the homotopy, exactness, suspension and wedge axioms, without imposing the ordinary dimension axiom. A [represented homology theory](#represented-homology-theory) is obtained by taking [stable homotopy groups](algebraic-topology.md#stable-homotopy-group) after a [smash product of spectra](algebraic-topology.md#smash-product-of-spectra).

### Represented homology theory

↑ **Parent:** [Generalized homology theory](#generalized-homology-theory)

A [topological spectrum](algebraic-topology.md#spectrum-topology) $E$ represents the reduced [generalized homology theory](#generalized-homology-theory) $\widetilde E_k(X)=\pi_k(E\wedge\Sigma^\infty X)$ on [based spaces](algebraic-topology.md#based-space), where the [smash product of spectra](algebraic-topology.md#smash-product-of-spectra) is derived. It is covariant in $X$.

## Null-homologous cycle

↑ **Parent:** [Homology (mathematics)](homology.md)

An element of a [cycle module](algebra.md#cycle-module) is null-homologous when it represents zero in [homology](homology.md), equivalently when it lies in the image of the [boundary operator](#boundary-operator). A closed submanifold bounding a submanifold one dimension higher is null-homologous.

## Primitive homology class

↑ **Parent:** [Homology (mathematics)](homology.md)

A positive-degree class whose reduced [homology](homology.md) diagonal vanishes. In a torsion-free [homology](homology.md) Hopf algebra, powers of an even primitive class have binomial diagonals. Dualizing that diagonal produces the multiplication of a [divided power algebra](commutative-algebra.md#divided-power-algebra).

## Acyclic space

↑ **Parent:** [Homology (mathematics)](homology.md)

A nonempty space is acyclic with the chosen coefficients if its reduced homology vanishes in every degree. Equivalently it has the [homology](homology.md) of a point. It need not be contractible.

## Homology of a directed union

↑ **Parent:** [Homology (mathematics)](homology.md)

Suppose $X=\bigcup_aX_a$ is directed by inclusion and every compact subset of $X$ lies in some $X_a$. Every finite [singular chain](#singular-chain) then lies in one $X_a$, so $C_*(X)=\varinjlim_aC_*(X_a)$. Exactness of [filtered colimits](module-theory.md#filtered-colimit-of-modules) gives

$$
H_i(X)\cong\varinjlim_aH_i(X_a).
$$

### Countability of the homology of an open Euclidean subset

↑ **Parent:** [Homology of a directed union](#homology-of-a-directed-union)

Every open subset $U\subseteq\mathbb R^N$ is the directed union of finite unions of closed rational cubes contained in $U$. Every compact subset of $U$ lies in one such finite polyhedron, whose homology is finitely generated. The [homology of a directed union](#homology-of-a-directed-union) therefore expresses each $H_i(U;\mathbb Z)$ as a direct limit over a countable family of countable groups, so it is countable.

## Reduced homology

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_homology)

Reduced homology modifies degree zero so that a one-point space has zero homology in every degree. For a nonempty space, $\widetilde H_k(X)=H_k(X)$ when $k>0$, while $H_0(X)\cong\widetilde H_0(X)\oplus\mathbb Z$.

## Homology group

↑ **Parent:** [Homology (mathematics)](homology.md)

A homology group is one of the [abelian groups](group.md#abelian-group) produced by a [homology](homology.md) theory. Its elements are [homology classes](#homology-class), represented in singular homology by cycles modulo boundaries.

### Zeroth homology group

↑ **Parent:** [Homology group](#homology-group)

The zeroth homology group is the free [abelian group](group.md#abelian-group) on the [path components](geometry-and-topology.md#path-component) of $X$. In particular, if $X$ has finitely many path components, then

$$
H_0(X;\mathbb Z)\cong\mathbb Z^{\#\pi_0(X)}.
$$

### Homology class

↑ **Parent:** [Homology group](#homology-group)

A homology class is an equivalence class of [chain cycles](#chain-cycle) modulo [chain boundaries](#chain-boundary) in a [chain complex](#chain-complex).

## Functoriality of homology

↑ **Parent:** [Homology (mathematics)](homology.md)

A [continuous map](topology.md#continuous-map) $f:X\to Y$ induces homomorphisms $f_*:H_n(X)\to H_n(Y)$ satisfying $(g\circ f)_*=g_*\circ f_*$ and $(\operatorname{id}_X)_*=\operatorname{id}_{H_n(X)}$.

### Homotopy invariance of homology

↑ **Parent:** [Functoriality of homology](#functoriality-of-homology)

[Homotopic](algebraic-topology.md#homotopy) maps induce the same homomorphism on every [homology group](#homology-group). Consequently, [homotopy equivalent](algebraic-topology.md#homotopy-inverse) spaces have isomorphic homology groups.

#### Singular prism operator

↑ **Parent:** [Homotopy invariance of homology](#homotopy-invariance-of-homology)

Triangulate $\Delta^q\times I$ by the simplices with vertices $(v_0,0),\ldots,(v_i,0),(v_i,1),\ldots,(v_q,1)$ and coefficients $(-1)^i$. Composing with a [homotopy](algebraic-topology.md#homotopy) between f and g gives a degree-one map P on [singular chains](#singular-chain). Shared faces cancel; the remaining faces give the displayed [chain homotopy](#chain-homotopy) identity. Hence homotopic maps induce the same map on [singular homology](#singular-homology).

## First homology

↑ **Parent:** [Homology (mathematics)](homology.md)

The first homology group $H_1(X)$ is the group of one-dimensional cycles modulo boundaries. For a path-connected space it is the [abelianization](group-theory.md#abelianization) of the [fundamental group](algebraic-topology.md#fundamental-group).

## Singular homology

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_homology)

Singular homology forms a [chain complex](#chain-complex) from formal sums of continuous maps from standard simplices into a [topological space](topology.md#topological-space). Its homology groups are invariant under [homotopy](algebraic-topology.md#homotopy).

### Singular chain complex

↑ **Parent:** [Singular homology](#singular-homology)

The [chain complex](#chain-complex) whose degree-$n$ group is freely generated over $R$ by the [singular simplices](#singular-simplex) $\sigma:\Delta^n\to X$. Its boundary is the alternating sum of restrictions to codimension-one faces. The [homology](homology.md) of this complex is [singular homology](#singular-homology).

### Small singular chains for an open cover

↑ **Parent:** [Singular homology](#singular-homology)

For an open cover, take the subcomplex generated by singular simplices whose images lie in single cover members. Repeated [barycentric subdivision](#barycentric-subdivision) makes each finite singular chain small, and the standard subdivision chain homotopy shows that inclusion induces homology isomorphisms. For a two-set cover, the short exact sequence of these small chains gives the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence); excising the complement of one open set from the pair with the other set gives its equivalent relative-homology formulation.

### Local coefficient system

↑ **Parent:** [Singular homology](#singular-homology)

A local coefficient system assigns an Abelian group or module to each point, with compatible transport isomorphisms along paths depending only on homotopy relative endpoints. Equivalently it is a functor from the fundamental groupoid. On a connected manifold it is described by a representation of the [fundamental group](algebraic-topology.md#fundamental-group) after fixing one fiber.

#### Orientation local system

↑ **Parent:** [Local coefficient system](#local-coefficient-system)

Its fiber at $x$ is $H_n(M,M\setminus\{x\};\mathbb Z)\cong\mathbb Z$. Transport changes its generator by the sign of local orientation along the path. For a connected nonorientable manifold, its degree-zero cohomology is zero, because no nonzero integer is invariant under sign reversal, whereas its degree-zero homology is $\mathbb Z/2$, the coinvariants under that reversal.

### Betti number

↑ **Parent:** [Singular homology](#singular-homology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Betti_number)

A Betti number is the dimension of a real [singular homology](#singular-homology) group; on a smooth manifold it is also the dimension of the corresponding [de Rham cohomology](differential-form.md#de-rham-cohomology) group. For a finite-dimensional cohomology group on a closed Riemannian manifold, it equals the dimension of its space of harmonic representatives. Betti numbers can increase under a finite cover, so equality is a separate hypothesis, not a general covering-space theorem.

<h4 id="poincare-polynomial">Poincaré polynomial</h4>

↑ **Parent:** [Betti number](#betti-number)

For a space with finite-dimensional [homology](homology.md) over a specified field and only finitely many nonzero [Betti numbers](#betti-number), this polynomial records their graded dimensions. Its value at one is the total [Betti number](#betti-number), and its value at minus one is the [Euler characteristic](#euler-characteristic). The [Künneth theorem](cohomology.md#kunneth-theorem) gives $P_{M\times N}(t)=P_M(t)P_N(t)$ over a field. For integer [homology](homology.md) ranks, use the rational [Betti numbers](#betti-number).

### Singular chain

↑ **Parent:** [Singular homology](#singular-homology)

A singular $n$-chain is a finite formal integer linear combination of [singular simplices](#singular-simplex). Its support is contained in a compact subset of the ambient space.

#### Singular chain group

↑ **Parent:** [Singular chain](#singular-chain)

The singular chain group is the free [abelian group](group.md#abelian-group) on all continuous maps $\Delta^q\to X$, the [singular simplices](#singular-simplex). In particular it is free even when the set of simplices is infinite. This freeness makes applying $\operatorname{Hom}(C_q(X),-)$ to a short exact coefficient sequence exact.

### Singular simplex

↑ **Parent:** [Singular homology](#singular-homology)

A singular $n$-simplex in a space $X$ is a [continuous map](topology.md#continuous-map) $\sigma:\Delta^n\to X$ from the standard $n$-simplex. Its alternating restrictions to the faces form its [boundary](#boundary-operator).

## Intersection form

↑ **Parent:** [Homology (mathematics)](homology.md)

For an oriented compact manifold of dimension $4k$, the intersection form is the bilinear pairing on middle-dimensional homology obtained by representing classes by transverse cycles and counting their signed intersection points. On an oriented four-manifold it is equivalently the cup-product pairing on $H^2$ evaluated on the fundamental class.

The [intersection form of a 4-manifold](#intersection-form-of-a-4-manifold) is the four-dimensional case of this middle-dimensional intersection pairing.

### Rank-one intersection form and the projective-plane cohomology ring

↑ **Parent:** [Intersection form](#intersection-form)

For a simply connected closed four-manifold with second [Betti number](#betti-number) one, [Poincare duality](cohomology.md#poincare-duality) and the [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology) make $H_2$ torsion-free of rank one. The integral [intersection form](#intersection-form) is unimodular, so its one-by-one matrix is $[1]$ or $[-1]$. Hence the square of a generator $u\in H^2$ generates $H^4$, giving the displayed [cohomology ring](cohomology.md#cohomology-ring). This is a ring isomorphism; it need not preserve a preassigned orientation class.

### Positive index of the intersection form

↑ **Parent:** [Intersection form](#intersection-form)

For a closed oriented [smooth four-manifold](topology.md#smooth-four-manifold), $b_2^+$ is the dimension of a maximal positive-definite subspace of its real [intersection form](#intersection-form). A [symplectic form](symplectic-geometry.md#symplectic-form) forces $b_2^+\geq1$, because its [cohomology class](cohomology.md#cohomology-class) has positive square. Reversing orientation exchanges the positive and negative indices.

### Intersection form of a product of two closed oriented surfaces

↑ **Parent:** [Intersection form](#intersection-form)

Here $H$ is the hyperbolic form with matrix $\begin{pmatrix}0&1\\1&0\end{pmatrix}$. The degree-two cohomology consists of the two factor orientation classes and $4gh$ products of degree-one classes. The factor classes pair once and have zero squares. In symplectic bases $a_i,b_i$ and $c_j,d_j$, $(a_ic_j)(b_kd_l)=-\delta_{ik}\delta_{jl}\omega_1\omega_2$ and $(a_id_j)(b_kc_l)=\delta_{ik}\delta_{jl}\omega_1\omega_2$. Each pair $(i,j)$ contributes two hyperbolic forms; the fiber classes contribute one more. The sign in the first formula comes from interchanging two odd-degree factors.

### Unimodular intersection pairing

↑ **Parent:** [Intersection form](#intersection-form)

An integral [intersection form](#intersection-form) on a finite-rank free [abelian group](group.md#abelian-group) $L$ is unimodular if its adjoint $x\mapsto\lambda(x,-)$ is an [isomorphism](algebra.md#isomorphism) to the integral dual. In an integral basis, this is equivalent to the pairing matrix having determinant $1$ or $-1$, not merely nonzero determinant. For example, [projective lines generate a unimodular intersection form](algebraic-topology.md#projective-lines-generate-a-unimodular-intersection-form) on the [Complex projective plane](algebraic-topology.md#complex-projective-plane), with matrix $(1)$ in its complex [orientation](algebraic-topology.md#orientation-of-a-simplex).

### Novikov additivity

↑ **Parent:** [Intersection form](#intersection-form)

When compact oriented four-manifolds are glued along an entire closed boundary three-manifold, the [signature](linear-algebra.md#signature-of-a-quadratic-form) of the result is the sum of their [intersection form](#intersection-form) signatures. It applies to $X_0\cup_{\partial X_0}(-X_1)$ with the difference of the two signatures. Gluing along only part of a boundary can require a correction; that is a different situation.

### Intersection pairing

↑ **Parent:** [Intersection form](#intersection-form)

An intersection pairing counts signed intersections of transverse representatives of complementary [homology classes](#homology-class), using one relative representative when the [manifold](topology.md#topological-manifold) has boundary. With $\mathbb F_2$ coefficients it is defined without [orientation](algebraic-topology.md#orientation-of-a-simplex) choices. [Poincare-Lefschetz duality](cohomology.md#lefschetz-duality) makes this a [perfect pairing](linear-algebra.md#perfect-pairing) for compact [manifolds](topology.md#topological-manifold).

#### Intersection matrix

↑ **Parent:** [Intersection pairing](#intersection-pairing)

The intersection matrix records an [intersection pairing](#intersection-pairing) on chosen classes. Its nonsingularity proves [linear independence](vector-space.md#linear-independence): a relation between the classes, paired with each class in turn, gives a vector in the matrix's kernel.

#### Coordinate sphere intersection basis

↑ **Parent:** [Intersection pairing](#intersection-pairing)

In the product $(S^{2d})^{2\ell}$, for $d,\ell\ge1$, vary the factors indexed by an $\ell$-element subset $I$ and fix points in the other factors. Orient the resulting [submanifold](differential-geometry.md#submanifold) $S_I$ in increasing factor order. These [homology classes](#homology-class) form an integral middle-dimensional basis by the [Künneth theorem](cohomology.md#kunneth-theorem). Complementary subsets give a transverse intersection at one point, with positive sign since all factor dimensions are even. For noncomplementary subsets some factor is fixed in both representatives; moving that point makes them disjoint. In particular every basis class has zero [self-intersection number](algebraic-geometry.md#self-intersection-number). Complementary pairs give hyperbolic blocks in the [intersection form](#intersection-form).

#### Half-lives-half-dies theorem

↑ **Parent:** [Intersection pairing](#intersection-pairing)

For a compact [three-manifold](topology.md#3-manifold) $W$, let $L=\ker(H_1(\partial W;\mathbb F_2)\to H_1(W;\mathbb F_2))$. The boundary [intersection pairing](#intersection-pairing) satisfies $L^\perp=L$: the [long exact sequence in relative homology](#long-exact-sequence-in-relative-homology) identifies $L$ with boundaries of relative surfaces, and the boundary-interior adjoint identity identifies its orthogonal complement with the same kernel. Hence $2\dim L=\dim H_1(\partial W;\mathbb F_2)$. This also implies that a closed surface with odd first mod-two [Betti number](#betti-number), such as $\mathbb{RP}^2$, cannot be the entire boundary of a compact [three-manifold](topology.md#3-manifold).

### Degree constraint from intersection forms

↑ **Parent:** [Intersection form](#intersection-form)

For a map $f:M\to N$ of connected closed oriented four-manifolds, naturality of the [cup product](cohomology.md#cup-product) gives

$$
Q_M(f^*u,f^*v)=(\deg f)Q_N(u,v).
$$

When $\deg f\ne0$, nondegeneracy makes $f^*:H^2(N;\mathbb Q)\to H^2(M;\mathbb Q)$ injective. Consequently the target [intersection form](#intersection-form), multiplied by the [mapping degree](#degree-of-a-continuous-mapping), must embed into the source form. For equal second [Betti numbers](#betti-number), a matrix $P$ for pullback satisfies $P^{\mathsf T}Q_MP=(\deg f)Q_N$; taking determinants often rules out nonzero degrees. In particular, a two-dimensional indefinite source form cannot realize a nonzero multiple of a two-dimensional definite target form.

### Real de Rham intersection form in dimension four

↑ **Parent:** [Intersection form](#intersection-form)

On a compact oriented [smooth manifold](differential-geometry.md#smooth-manifold) $N$ of dimension four without boundary, set $Q([\alpha],[\beta])=\int_N\alpha\wedge\beta$ for closed real two-forms. The [Stokes theorem](calculus.md#stokes-theorem) makes the expression independent of representatives, and the even degrees make it symmetric. It is the real [de Rham cohomology](differential-form.md#de-rham-cohomology) version of the [intersection form](#intersection-form). The [Hodge decomposition theorem](differential-form.md#hodge-decomposition-theorem) and [Hodge star operator](differential-form.md#hodge-star-operator) express it as $Q(h,k)=(h,*k)_{L^2}$ on harmonic representatives.

#### Signature of the intersection form from harmonic duality

↑ **Parent:** [Real de Rham intersection form in dimension four](#real-de-rham-intersection-form-in-dimension-four)

On a closed oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension four, the [Hodge star operator](differential-form.md#hodge-star-operator) preserves harmonic two-forms and splits them into orthogonal spaces $\mathcal H^+$ and $\mathcal H^-$ with eigenvalues $+1$ and $-1$. The [real de Rham intersection form in dimension four](#real-de-rham-intersection-form-in-dimension-four) equals the positive $L^2$ [inner product](linear-algebra.md#inner-product) on $\mathcal H^+$ and its negative on $\mathcal H^-$. It is nondegenerate, since $Q(h,*h)=\|h\|_2^2$. Its [signature pair](linear-algebra.md#signature-pair-of-a-real-symmetric-bilinear-form) is $(\dim\mathcal H^+,\dim\mathcal H^-)$.

## Integral homology

↑ **Parent:** [Homology (mathematics)](homology.md)

Integral homology is [homology](homology.md) with coefficients in $\mathbb Z$. It retains both the free and [torsion](group-theory.md#torsion-subgroup) parts of each homology group.

## Homology of a sphere

↑ **Parent:** [Homology (mathematics)](homology.md)

For $n>0$,

$$
H_i(S^n;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,n,\\
0,&\text{otherwise}.
\end{cases}
$$

Writing $S^n$ as two contractible hemispheres whose intersection deformation retracts to $S^{n-1}$ gives the calculation inductively through the [Mayer–Vietoris theorem](algebraic-topology.md#mayer-vietoris-sequence).

### Homology of an equatorial sphere complement

↑ **Parent:** [Homology of a sphere](#homology-of-a-sphere)

For the standard coordinate inclusion of [spheres](geometry-and-topology.md#sphere), write points as $(u,v)\in\mathbb R^{m+1}\times\mathbb R^{n-m}$, with $v\ne0$ in the complement. The map $(u,v)\mapsto(u,v/\lVert v\rVert)$ is a [homeomorphism](topology.md#homeomorphism) to $B^{m+1}_{\mathrm{open}}\times S^{n-m-1}$, with inverse $(u,w)\mapsto(u,\sqrt{1-\lVert u\rVert^2}w)$. Contracting the ball factor proves the displayed [homotopy equivalence](algebraic-topology.md#homotopy-equivalence). In codimension one there are two contractible components, so integral $H_0$ is $\mathbb Z^2$; in higher codimension the only nonzero [homology groups](#homology-group) are $H_0=\mathbb Z$ and $H_{n-m-1}=\mathbb Z$.

## Degree of a continuous mapping

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degree_of_a_continuous_mapping)

For a map $f:S^m\to S^m$, the degree is the integer by which $f_*$ multiplies a chosen generator of $H_m(S^m;\mathbb Z)$. It is invariant under [homotopy](algebraic-topology.md#homotopy).

### Mod-two degree of a map between closed manifolds

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

For a map $f:M\to N$ between closed connected $n$-manifolds, the mod-two degree is defined by $f_*[M]_2=\deg_2(f)[N]_2$. Every manifold has a mod-two orientation class, so no orientability assumption is needed. It is invariant under [homotopy](algebraic-topology.md#homotopy). A nonsurjective map has mod-two degree zero: mapping the fundamental classes into the local relative homology at a missed target point makes the source contribution zero but leaves the target local generator nonzero.

### Nonzero degree from a sphere obstructs manifold products

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

Suppose a map $S^m\to M$ of closed connected oriented manifolds has nonzero [mapping degree](#degree-of-a-continuous-mapping). A product decomposition with $0<k<m$ would have oriented closed factors: an orientation-reversing loop in either factor, with the other coordinate fixed, would reverse the product orientation. Pull back their top [orientation classes](cohomology.md#fundamental-class) to obtain $\alpha\in H^k(M;\mathbb Z)$ and $\beta\in H^{m-k}(M;\mathbb Z)$ with $\alpha\smile\beta$ a generator of $H^m(M;\mathbb Z)$. Both pullbacks to the sphere vanish in their intermediate degrees, contradicting the nonzero-degree pullback of their product.

### Degrees of maps of the zero-sphere

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

Define [mapping degree](#degree-of-a-continuous-mapping) for $S^0$ using its rank-one [reduced homology](#reduced-homology) group $\widetilde H_0(S^0;\mathbb Z)$. Its generator is the difference of its two points. The four maps of that two-point set consist of the identity, the interchange, and two constant maps; their degree multipliers are $1,-1,0,0$. Thus [sphere maps of arbitrary integer degree](#sphere-maps-of-arbitrary-integer-degree) require positive [sphere](geometry-and-topology.md#sphere) dimension.

### Relative mapping degree

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

For a map of oriented disk pairs, the multiplier on top [relative homology](#relative-homology) is its relative [mapping degree](#degree-of-a-continuous-mapping). Naturality of the [connecting homomorphism](#connecting-homomorphism) identifies it with the [mapping degree](#degree-of-a-continuous-mapping) of the boundary map.

#### Graph intersection formula for mapping degree

↑ **Parent:** [Relative mapping degree](#relative-mapping-degree)

For a smooth map of disk pairs whose [graph of a function](function.md#graph-of-a-function) is transverse to the zero slice, orient the graph by its domain. With the tangent space of the zero slice ordered before that of the graph, the local [smooth intersection number](differential-geometry.md#smooth-intersection-number) at a zero is $\operatorname{sgn}\det DF$. Summing these signs gives the relative [mapping degree](#degree-of-a-continuous-mapping) and hence the boundary [mapping degree](#degree-of-a-continuous-mapping). Reversing the order of these two $m$-dimensional tangent spaces changes the sign by $(-1)^m$.

#### Quotient-sphere degree identity

↑ **Parent:** [Relative mapping degree](#relative-mapping-degree)

Collapsing the boundary identifies the top [relative homology](#relative-homology) of a disk pair with the top [reduced homology](#reduced-homology) of its quotient [sphere](geometry-and-topology.md#sphere). Together with the boundary [connecting homomorphism](#connecting-homomorphism), this shows that the induced quotient map and the boundary map have the same [mapping degree](#degree-of-a-continuous-mapping), using the corresponding orientations.

### Local degree of a continuous map

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

Let $f:M\to N$ be a [continuous map](topology.md#continuous-map) between oriented $d$-dimensional [manifolds](topology.md#topological-manifold), with $d\geq1$. Suppose $x$ is an isolated point of the fiber over $y=f(x)$. Choose an open neighborhood $U$ with $U\cap f^{-1}(y)=\{x\}$. The map of pairs

$$
(U,U\setminus\{x\})\longrightarrow(N,N\setminus\{y\})
$$

induces a map between rank-one degree-$d$ [local homology](#local-homology) groups. Relative to the [local orientation of a manifold](cohomology.md#local-orientation-of-a-manifold), this map is multiplication by an integer, the local degree. [Excision](#excision-theorem) makes it independent of the neighborhood. A [smooth map between manifolds](differential-geometry.md#smooth-map-between-manifolds) with invertible derivative at $x$ has local degree $\operatorname{sign}\det Df_x$, by the [inverse function theorem](calculus.md#inverse-function-theorem) and the chosen orientations.

#### Local degrees of arbitrary integer value

↑ **Parent:** [Local degree of a continuous map](#local-degree-of-a-continuous-map)

In dimension two, $z\mapsto z^k$ for positive $k$ has local degree $k$ at zero, and $z\mapsto\overline z^{\,|k|}$ has degree $k$ for negative $k$. The proper map $z\mapsto|z|^2\in\mathbb C$ has isolated zero fiber and local degree zero, since its image misses every nearby nonreal target. These proper maps extend to the two-sphere. Taking their product with the identity of $\mathbb R^{n-2}$ realizes the same local degrees in every dimension $n\geq2$. In dimension one an isolated local degree is restricted to $0,1,-1$.

#### Degree as a sum of local degrees

↑ **Parent:** [Local degree of a continuous map](#local-degree-of-a-continuous-map)

For a [continuous map](topology.md#continuous-map) $f:M\to N$ of closed connected oriented $d$-dimensional [manifolds](topology.md#topological-manifold), suppose $f^{-1}(y)=\{x_1,\ldots,x_s\}$ is finite. Then

$$
\deg f=\sum_{j=1}^s\deg_{x_j}f.
$$

By [excision](#excision-theorem), the degree-$d$ [relative homology](#relative-homology) group $H_d(M,M\setminus f^{-1}(y);\mathbb Z)$ is the direct sum of the local groups at $x_j$. The [fundamental class](cohomology.md#fundamental-class) maps to the tuple of local orientation generators. Mapping this tuple to $H_d(N,N\setminus\{y\};\mathbb Z)$ adds their local degrees. Naturality identifies the result with the image of $(\deg f)[N]$. If the fiber is empty, the same argument gives degree zero.

### Degree under suspension

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

If $f:S^m\to S^m$, then its suspension $\Sigma f:S^{m+1}\to S^{m+1}$ has the same degree. This follows from naturality of the suspension isomorphism in reduced homology.

#### Sphere maps of arbitrary integer degree

↑ **Parent:** [Degree under suspension](#degree-under-suspension)

Every integer $m$ is the [mapping degree](#degree-of-a-continuous-mapping) of a [continuous map](topology.md#continuous-map) $S^n\to S^n$ in every dimension $n\geq1$. Start with the [circle](topology.md#circle) map $z\mapsto z^m$, whose argument winds $m$ times, and use [degree under suspension](#degree-under-suspension) repeatedly. Negative $m$ reverses the winding, and $m=0$ is constant before suspending. The [degrees of maps of the zero-sphere](#degrees-of-maps-of-the-zero-sphere) are a genuine exceptional case.

### Degree of a map between oriented manifolds

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

For a map $f:M\to N$ between closed connected oriented $d$-manifolds, its degree is the integer determined by $f_*[M]=(\deg f)[N]$ in top-dimensional homology.

#### Cup-power obstruction to nonzero degree

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

Let $M,N$ be closed connected oriented manifolds of the same dimension, and suppose $a^r$ generates the top integral [cohomology](cohomology.md) of $N$. If every class of degree $|a|$ on $M$ has zero rth [cup power](cohomology.md#cup-power), every [continuous map](topology.md#continuous-map) $f:M\to N$ has [mapping degree](#degree-of-a-continuous-mapping) zero. Indeed, $f^*(a^r)=(f^*a)^r=0$, and evaluation on the [fundamental class](cohomology.md#fundamental-class) gives $\deg f=0$. For $S^2\times S^4\to\mathbb{CP}^3$, the degree-two class is a multiple of the sphere class $u$, whose square vanishes.

#### Arbitrary-degree maps to a surface of genus two

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For $k>0$, an epimorphism $\pi_1(\Sigma_2)\to\mathbb Z/k$ gives a connected $k$-sheeted cover. Its Euler characteristic is $-2k$, hence its genus is $k+1$, and the lifted orientation gives degree $k$. For negative $k$ compose the $|k|$-sheeted cover with an orientation-reversing homeomorphism of the target. For $k=0$ take a constant map from the torus.

#### Collapse map of degree one onto a sphere

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

Choose an oriented embedded closed disc in a closed oriented positive-dimensional manifold and collapse its complement to a point. A target point away from the collapsed value has one preimage with local degree $+1$, proving global degree one by the [degree as a sum of local degrees](#degree-as-a-sum-of-local-degrees).

#### Surjective degree-zero sphere-to-torus map

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

On the unit two-sphere this formula maps onto the torus: every torus point has arguments corresponding to $x,y\in[-1/2,1/2]$, and $x^2+y^2\leq1/2$ leaves a real $z$ on the sphere. Scaling both arguments continuously to zero is a null-homotopy, so the degree is zero. Surjectivity alone does not force nonzero degree.

#### Multiplicativity of mapping degree

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For maps of oriented connected [closed manifolds](differential-geometry.md#closed-manifold) of the same dimension, apply functoriality of [homology](homology.md) to $f_*[M]=(\deg f)[N]$ and $g_*[N]=(\deg g)[L]$. The composite coefficient is their product. This recovers the multiplication of signed sheet counts for compositions of finite [covering maps](algebraic-topology.md#covering-space).

#### Homotopy invariance of mapping degree

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For maps between oriented connected [closed manifolds](differential-geometry.md#closed-manifold) of the same dimension, a [homotopy](algebraic-topology.md#homotopy) induces equal maps on top-dimensional [homology](homology.md), hence equal coefficients on the [fundamental class](cohomology.md#fundamental-class). For smooth maps and a smooth homotopy, the [degree by integration of a pullback volume form](#degree-by-integration-of-a-pullback-volume-form) gives another proof: the [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) on the homotopy cylinder makes the difference of endpoint pullback integrals zero because the target top form is closed. This is an obstruction to extending a degree-one sphere identity over a ball.

#### Degree does not classify general manifold maps

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

Although [topological degree](geometry-and-topology.md#topological-degree) classifies maps $S^n\to S^n$ up to [homotopy](algebraic-topology.md#homotopy), it is not a complete invariant for other manifolds. On the [torus](topology.md#torus), the identity and the integer shear $\begin{pmatrix}1&1\\0&1\end{pmatrix}$ both have degree one, but induce distinct maps on $H_1(T^2;\mathbb Z)$ and cannot be homotopic.

#### Degree by integration of a pullback volume form

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For a smooth map $f:M\to N$ between oriented connected [closed manifolds](differential-geometry.md#closed-manifold) of the same dimension, a normalized [volume form](differential-form.md#volume-form) on the target gives $\deg f=\int_Mf^*\omega$. The formula agrees with the [degree as a sum of local degrees](#degree-as-a-sum-of-local-degrees). A change of normalized top-form adds an exact form by top-dimensional [de Rham cohomology](differential-form.md#de-rham-cohomology), whose pullback has zero integral by [Stokes theorem](calculus.md#stokes-theorem).

#### Spherical degree by area pullback

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For a smooth map between oriented unit [spheres](geometry-and-topology.md#sphere), integrate the pullback of the target [area form](differential-form.md#area-form). Localizing a normalized top-degree form near a [regular value](differential-geometry.md#regular-value), and using [Stokes theorem](calculus.md#stokes-theorem) to discard exact-form differences, identifies this integral with the [degree as a sum of local degrees](#degree-as-a-sum-of-local-degrees).

#### Degree-one maps between closed oriented surfaces

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

A [degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds) equal to one makes the pullback on degree-one [cohomology](cohomology.md) injective by the [Poincare duality pairing](cohomology.md#poincare-duality-pairing). Thus a degree-one map of closed oriented surfaces requires $2h\leq2g$. Conversely, collapse the extra handles in $\Sigma_h\#\Sigma_{g-h}$ onto a point. The retained oriented disc shows that this map has degree one.

#### Prime-degree sphere map forces primary torsion

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

If $S^n\to N$ has prime degree $p$ and $N$ is a closed connected oriented $n$-manifold, every [integral homology](#integral-homology) group of $N$ in degrees strictly between zero and $n$ is a finite $p$-primary [abelian group](group.md#abelian-group). Consequently one power of $p$ annihilates all these groups. The proof combines [Poincare duality](cohomology.md#poincare-duality) over each field $\mathbb F_q$, $q\ne p$, with the [universal coefficient theorem for homology](#universal-coefficient-theorem-for-homology) and finite generation.

#### Degrees of maps factoring through real projective space

↑ **Parent:** [Degree of a map between oriented manifolds](#degree-of-a-map-between-oriented-manifolds)

For $n\geq2$, a self-map of $S^n$ factoring through [Real projective space](algebraic-topology.md#real-projective-space) $\mathbb{RP}^n$ has degree zero when $n$ is even, and can have exactly the even degrees when $n$ is odd. In the odd case the first map lifts through the double covering and the covering has degree two. The dimension-one exception allows every integer, since $\mathbb{RP}^1\cong S^1$.

### Antipodal map

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antipodal_map)

The antipodal map $x\mapsto-x$ on $S^m$ has degree $(-1)^{m+1}$.

#### Fixed-point-free sphere maps are homotopic to the antipodal map

↑ **Parent:** [Antipodal map](#antipodal-map)

If a continuous map $f:S^d\to S^d$ has no fixed point, the formula $H_t(x)=((1-t)f(x)-tx)/\|(1-t)f(x)-tx\|$ is a [homotopy](algebraic-topology.md#homotopy) from $f$ to the [antipodal map](#antipodal-map). The denominator could vanish only at $t=1/2$ and $f(x)=x$, which is excluded. The [homotopy invariance of mapping degree](#homotopy-invariance-of-mapping-degree) therefore gives $\deg f=(-1)^{d+1}$.

#### Odd map between spheres

↑ **Parent:** [Antipodal map](#antipodal-map)

An odd map between [spheres](geometry-and-topology.md#sphere) is a [continuous map](topology.md#continuous-map) $f:S^n\to S^m$ satisfying $f(-x)=-f(x)$. Thus it is equivariant for the two [antipodal maps](#antipodal-map). It descends to a [continuous map](topology.md#continuous-map) of [Real projective spaces](algebraic-topology.md#real-projective-space).

##### Cohomological obstruction to separately odd sphere multiplication

↑ **Parent:** [Odd map between spheres](#odd-map-between-spheres)

Suppose a [continuous map](topology.md#continuous-map) $g:S^n\times S^n\to S^n$ changes sign on negating either input. Its quotient $\bar g:\mathbb{RP}^n\times\mathbb{RP}^n\to\mathbb{RP}^n$ pulls back the [real tautological line bundle](fiber-bundle.md#real-tautological-line-bundle) to the [tensor product of vector bundles](fiber-bundle.md#tensor-product-of-vector-bundles) $p_1^*\gamma_n\otimes p_2^*\gamma_n$. The fiber map sends $(s x)\otimes(t y)$ to $st g(x,y)$. The [First Stiefel–Whitney class of a tensor product of real line bundles](fiber-bundle.md#first-stiefel-whitney-class-of-a-tensor-product-of-real-line-bundles) consequently gives $\bar g^*a=a_1+a_2$. The [Künneth theorem](cohomology.md#kunneth-theorem) and the [mod-two cohomology ring of real projective space](algebraic-topology.md#mod-two-cohomology-ring-of-real-projective-space) imply

$$
(a_1+a_2)^{n+1}=0\quad\text{in }\mathbb F_2[a_1,a_2]/(a_1^{n+1},a_2^{n+1}).
$$

Every interior [binomial coefficient](combinatorics.md#binomial-coefficient) in row $n+1$ must be even. By [binomial coefficients with even interior terms](combinatorics.md#binomial-coefficients-with-even-interior-terms), $n=2^k-1$ for some $k\geq0$. This is a necessary condition, not an assertion of existence in every such dimension.

##### Odd maps pull back the real tautological line bundle

↑ **Parent:** [Odd map between spheres](#odd-map-between-spheres)

For an [odd map between spheres](#odd-map-between-spheres) $f:S^n\to S^m$ and its quotient $\bar f$, there is an [isomorphism](algebra.md#isomorphism) $\gamma_n\cong\bar f^*\gamma_m$ of [real tautological line bundles](fiber-bundle.md#real-tautological-line-bundle). With $x$ a unit vector, send $t x$ to $t f(x)$; replacing $x$ by $-x$ and $t$ by $-t$ gives the same vector. This proves both linearity on fibers and well-definedness. Therefore $\bar f^*w_1(\gamma_m)=w_1(\gamma_n)$. The [mod-two cohomology ring of real projective space](algebraic-topology.md#mod-two-cohomology-ring-of-real-projective-space) then implies $n\leq m$, since a vanishing $(m+1)$st power must pull back to a vanishing power.

#### Invariant primitive under a finite group action

↑ **Parent:** [Antipodal map](#antipodal-map)

Let a [finite group](group.md#finite-group) $G$ act smoothly on a [smooth manifold](differential-geometry.md#smooth-manifold), and suppose that a $G$-invariant [differential form](differential-form.md) $\omega$ is an [exact differential form](differential-form.md#exact-differential-form), say $\omega=d\eta$. Averaging gives the invariant primitive

$$
\bar\eta=\frac1{|G|}\sum_{g\in G}g^*\eta,
\qquad d\bar\eta=\omega.
$$

If the action is free, invariant forms descend uniquely through the resulting [covering map](algebraic-topology.md#covering-space).

##### Top-degree differential forms on even-dimensional real projective space are exact

↑ **Parent:** [Invariant primitive under a finite group action](#invariant-primitive-under-a-finite-group-action)

For the double covering $\pi:S^{2n}\to\mathbb{RP}^{2n}$ and the [antipodal map](#antipodal-map) $a$, every pulled-back top form satisfies $a^*\pi^*\omega=\pi^*\omega$. Since $\deg a=-1$, its integral over the sphere is its own negative and hence vanishes. It is therefore exact on the sphere. Averaging a primitive under $a$ and descending it proves that $\omega$ is exact on real projective space.

### Degree of a Euclidean homeomorphism

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

A Euclidean homeomorphism is a [proper map](cohomology.md#proper-map) and extends to its [one-point compactification](topology.md#alexandroff-extension) $S^n$. Its degree is the [degree of a continuous mapping](#degree-of-a-continuous-mapping) of this extension, and belongs to $\{1,-1\}$. A linear isomorphism has degree equal to the sign of its determinant.

### Degree of a factor swap

↑ **Parent:** [Degree of a continuous mapping](#degree-of-a-continuous-mapping)

The factor swap $\mathbb R^m\times\mathbb R^n\to\mathbb R^n\times\mathbb R^m$ has degree $(-1)^{mn}$. Moving an oriented basis of the first factor past one of the second requires $mn$ transpositions.

## Relative homology

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Relative_homology)

The relative chain complex is $C_*(X,A)=C_*(X)/C_*(A)$, and its homology is the relative homology $H_*(X,A)$. A pair $A\subseteq U\subseteq X$ produces a long exact sequence for the triple.

### Relative homology of a surface modulo disjoint circles

↑ **Parent:** [Relative homology](#relative-homology)

Let $A$ be a nonempty union of disjoint embedded circles in a closed oriented [topological surface](topology.md#topological-surface) $\Sigma_g$, and let $c$ be the number of components after cutting along them. [Excision](#excision-theorem) and [Poincare-Lefschetz duality](cohomology.md#lefschetz-duality) identify the [relative homology](#relative-homology) with the complementary-degree [cohomology](cohomology.md) of the cut surface. Its components have boundary, so the relative groups are free, with the displayed ranks; $H_0$ and higher groups vanish. The rank of the circle classes in $H_1(\Sigma_g)$ is $|\pi_0(A)|+1-c$. For a single circle these groups detect whether its class is zero, but for genus at least two cannot distinguish a disk boundary from an essential separating circle.

### Relative homology class

↑ **Parent:** [Relative homology](#relative-homology)

A relative homology class is represented by a [singular chain](#singular-chain) whose boundary lies in $A$. Two representatives give the same class when their difference is a [boundary operator](#boundary-operator) image plus a chain in $A$. Thus a path with endpoints in $A$ can represent a class even when its endpoints are different.

### Relative chain complex

↑ **Parent:** [Relative homology](#relative-homology)

For a subspace $A\subseteq X$, the relative chain complex is the [quotient group](group-theory.md#quotient-group) in each degree,

$$
C_k(X,A)=C_k(X)/C_k(A),
$$

with [boundary operator](#boundary-operator) $[c]\mapsto[\partial c]$. This is well defined because $C_*(A)$ is a [chain subcomplex](#chain-subcomplex) of $C_*(X)$.

#### Relative cycle

↑ **Parent:** [Relative chain complex](#relative-chain-complex)

A relative cycle for $A\subset B$ is a chain $b\in C_n(B)$ whose boundary lies in $A$. Equivalently its coset is a [homological cycle](#chain-cycle) in $C_*(B,A)$. Unlike an absolute cycle, its boundary need not be zero. It represents a [relative homology class](#relative-homology-class).

#### Relative simplicial chain complex

↑ **Parent:** [Relative chain complex](#relative-chain-complex)

If $L$ is a [simplicial subcomplex](algebraic-topology.md#simplicial-subcomplex) of $K$, then

$$
C_k(K,L)=C_k(K)/C_k(L).
$$

Its homology is the simplicial [relative homology](#relative-homology) $H_k(K,L)$.

### Long exact sequence in relative homology

↑ **Parent:** [Relative homology](#relative-homology)

For a pair $A\subseteq X$, the [short exact sequence of chain complexes](#short-exact-sequence-of-chain-complexes) $0\to C_*(A)\to C_*(X)\to C_*(X,A)\to0$ induces

$$
\cdots\to H_n(A)\to H_n(X)\to H_n(X,A)\xrightarrow{\partial}H_{n-1}(A)\to\cdots.
$$

### Relative homology of a simplex and its boundary

↑ **Parent:** [Relative homology](#relative-homology)

For $n\geq1$,

$$
H_k(\Delta^n,\partial\Delta^n;\mathbb Z)
\cong
\begin{cases}
\mathbb Z,&k=n,\\
0,&k\ne n.
\end{cases}
$$

In the [relative simplicial chain complex](#relative-simplicial-chain-complex), every proper face vanishes, leaving one generator in degree $n$ and zero chain groups in all other degrees.

### Good pair

↑ **Parent:** [Relative homology](#relative-homology)

A pair $(X,A)$ is good when $A$ is closed and is a deformation retract of some neighborhood in $X$. Such a pair satisfies the hypotheses needed to compare relative homology with the reduced homology of a quotient.

#### Collapsing a pair theorem

↑ **Parent:** [Good pair](#good-pair)

For a good pair $(X,A)$, the quotient map induces natural isomorphisms

$$
H_q(X,A)\cong\widetilde H_q(X/A).
$$

##### Collapsing a simple closed curve on a surface

↑ **Parent:** [Collapsing a pair theorem](#collapsing-a-pair-theorem)

A simple closed curve in a [closed orientable surface](topology.md#closed-orientable-surface) has an annular [collar neighbourhood](differential-geometry.md#collar-neighbourhood), so its collapse is governed by the [collapsing a pair theorem](#collapsing-a-pair-theorem). In the [long exact sequence in relative homology](#long-exact-sequence-in-relative-homology), the decisive map is $H_1(A;\mathbb Z)\to H_1(\Sigma_g;\mathbb Z)$, sending the [circle](topology.md#circle) generator to its [homology class](#homology-class). That class is zero for a separating curve and a [primitive homology class](#primitive-homology-class) for a nonseparating curve. The two possibilities lead to [homology after collapsing a separating surface curve](#homology-after-collapsing-a-separating-surface-curve) and [homology after collapsing a nonseparating surface curve](#homology-after-collapsing-a-nonseparating-surface-curve).

###### Homology after collapsing a nonseparating surface curve

↑ **Parent:** [Collapsing a simple closed curve on a surface](#collapsing-a-simple-closed-curve-on-a-surface)

For genus $g\geq1$, collapse a nonseparating simple closed curve on a [closed orientable surface](topology.md#closed-orientable-surface). Its [homology class](#homology-class) is primitive, as a curve meeting it transversely once detects by the [intersection pairing on an oriented surface](cohomology.md#intersection-pairing-on-an-oriented-surface). The [long exact sequence in relative homology](#long-exact-sequence-in-relative-homology) therefore gives $H_0=\mathbb Z$, $H_1=\mathbb Z^{2g-1}$, $H_2=\mathbb Z$, and zero higher groups for the quotient. Geometrically it has the [homotopy type](algebraic-topology.md#homotopy-type) $\Sigma_{g-1}\vee S^1$.

###### Homology after collapsing a separating surface curve

↑ **Parent:** [Collapsing a simple closed curve on a surface](#collapsing-a-simple-closed-curve-on-a-surface)

Collapse a separating simple closed curve on a [closed orientable surface](topology.md#closed-orientable-surface) of genus $g$. If its two sides have genera $g_1,g_2$, the quotient is homeomorphic to $\Sigma_{g_1}\vee\Sigma_{g_2}$. Its [integral homology](#integral-homology) is $\mathbb Z$ in degree zero, $\mathbb Z^{2g}$ in degree one, $\mathbb Z^2$ in degree two, and zero above degree two. In [relative homology](#relative-homology), the [circle](topology.md#circle) maps to zero in $H_1(\Sigma_g)$, and the second relative group fits into a split sequence $0\to\mathbb Z\to H_2(\Sigma_g,A)\to\mathbb Z\to0$. The two collapsed sides retain independent [fundamental classes](cohomology.md#fundamental-class).

## Excision theorem

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Excision_theorem)

Excision identifies relative homology after removing a subspace whose closure lies in the interior of the subspace being quotiented. It makes local homology computable in an arbitrarily small neighborhood.

## Exact sequence

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exact_sequence)

An exact sequence has the image of each map equal to the kernel of the next.

### Long exact sequence

↑ **Parent:** [Exact sequence](#exact-sequence)

A long exact sequence is a sequence of [abelian groups](group.md#abelian-group) or [modules](module-theory.md#module-mathematics) with arbitrarily many consecutive maps, for which the image of every map equals the kernel of the next. A [short exact sequence of cochain complexes](algebra.md#short-exact-sequence-of-cochain-complexes) yields a long exact sequence of their [cohomology](cohomology.md), with [connecting homomorphisms](#connecting-homomorphism) increasing degree by one. The exact sequences of [relative cohomology](cohomology.md#relative-cohomology) and the [Bockstein homomorphism](#bockstein-homomorphism) are examples.

## Commutative diagram

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutative_diagram)

A commutative diagram is a diagram of objects and morphisms in which every two directed paths with the same endpoints define the same morphism.

## Chain complex

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chain_complex)

A chain complex is a sequence of abelian groups or modules and homomorphisms $d_i:C_i\to C_{i-1}$ satisfying $d_{i-1}d_i=0$. Its homology is $H_i(C)=\ker d_i/\operatorname{im}d_{i+1}$.

### Hopf trace identity

↑ **Parent:** [Chain complex](#chain-complex)

For an endomorphism of a finite-dimensional bounded [chain complex](#chain-complex) over a [field](algebra.md#field), the alternating chain trace equals the alternating trace on [homology](homology.md). Split each chain space into boundaries, representatives for [homology](homology.md), and a complement mapping isomorphically to the preceding boundaries. The chain-map relation makes the traces on the first and third summands cancel in successive degrees, leaving the [homology](homology.md) traces. Over a [field](algebra.md#field) the induced [cohomology](cohomology.md) maps are dual and have the same traces. This identity turns the absence of diagonal simplex contributions into a vanishing [Lefschetz number](algebraic-topology.md#lefschetz-number).

### Differential of a chain complex

↑ **Parent:** [Chain complex](#chain-complex)

The [chain differential](#boundary-operator) of a homological [chain complex](#chain-complex) is a family of group or module homomorphisms $\partial_n:C_n\to C_{n-1}$ satisfying $\partial_{n-1}\partial_n=0$. The identity implies $\operatorname{im}\partial_{n+1}\subset\ker\partial_n$, so the quotient $H_n=\ker\partial_n/\operatorname{im}\partial_{n+1}$ is defined. In a graded complex over $\mathbb Z[U]$, the [chain differential](#boundary-operator) can have degree $-1$ while $U$ has degree $-2$, with $\partial(Ux)=U\partial x$.

### Reversed dual chain complex

↑ **Parent:** [Chain complex](#chain-complex)

The reversed [dual module](module-theory.md#dual-module) of a [chain complex](#chain-complex) becomes a [chain complex](#chain-complex) with the unsigned precomposition differential above. A functional on $C_{-i}$ is sent to a functional on $C_{1-i}$, lowering the reversed degree by one.

### Graded Hom complex of chain complexes

↑ **Parent:** [Chain complex](#chain-complex)

A graded [Hom functor](algebra.md#hom-functor) construction consists of maps shifting degree by $j$. One homological convention is $d_M f=f d_C+(-1)^{j-1}d_{C'}f$. Its degree-zero cycles are [chain maps](#chain-map), and its degree-zero boundaries are null-homotopic [chain maps](#chain-map), so its zeroth [homology](homology.md) is the module of [chain homotopy](#chain-homotopy) classes. This convention differs by degree-dependent signs from the alternative convention $d'f-(-1)^jfd$.

#### Sign conjugation for the tensor-Hom identification

↑ **Parent:** [Graded Hom complex of chain complexes](#graded-hom-complex-of-chain-complexes)

For finite free total [chain complexes](#chain-complex), evaluation identifies the underlying graded [tensor product](linear-algebra.md#tensor-product) $X\otimes C'$ with the [graded Hom complex of chain complexes](#graded-hom-complex-of-chain-complexes), where $X$ is the [reversed dual chain complex](#reversed-dual-chain-complex). Under the precomposition-first Hom differential, conjugation by the sign $(-1)^{j(j-1)/2}$ makes this a chain isomorphism. The identity $\rho(j)-\rho(j-1)=j-1$ works for every integer degree. If the grading is unbounded and only degreewise finite, products on the Hom side need not equal direct sums on the tensor side.

### Tensor product of chain complexes

↑ **Parent:** [Chain complex](#chain-complex)

The [tensor product](linear-algebra.md#tensor-product) of homologically graded [chain complexes](#chain-complex) has differential $D(x_p\otimes y)=dx_p\otimes y+(-1)^p x_p\otimes dy$. The sign makes the two mixed terms in $D^2$ cancel. Total degree is the sum of the two degrees.

#### Koszul sign rule

↑ **Parent:** [Tensor product of chain complexes](#tensor-product-of-chain-complexes)

Interchanging homogeneous objects of degrees $p$ and $q$ introduces $(-1)^{pq}$. In particular, moving a degree-minus-one differential past a degree-$p$ factor introduces $(-1)^p$. This convention produces the differential on the [tensor product of chain complexes](#tensor-product-of-chain-complexes).

### Disk chain complex

↑ **Parent:** [Chain complex](#chain-complex)

For $n\geq1$, the [chain complex](#chain-complex) with copies of $R$ in degrees $n,n-1$ and identity differential. It is acyclic; a map from it chooses an arbitrary degree-$n$ element and its boundary.

### Sphere chain complex

↑ **Parent:** [Chain complex](#chain-complex)

The [chain complex](#chain-complex) with $R$ in a single degree $n$ and zero differential. A map from it into a complex chooses a cycle in degree $n$.

### Double complex

↑ **Parent:** [Chain complex](#chain-complex)

A double complex has modules $C_{p,q}$ and differentials lowering either index, each squaring to zero and anticommuting with the other. The total [chain complex](#chain-complex) has term $\bigoplus_{p+q=i}C_{p,q}$ and differential the sum of the two differentials. For the tensor product of two [chain complexes](#chain-complex), a sign $(-1)^p$ on the second differential ensures anticommutation. If the double complex is in the first quadrant and one direction has [homology](homology.md) only in degree zero, its total [homology](homology.md) is computed by the surviving degree-zero complex. Applying this twice to two [free resolutions](algebra.md#free-resolution) proves the balanced calculation of the [Tor functor](algebra.md#tor-functor).

#### Double cochain complex

↑ **Parent:** [Double complex](#double-complex)

Two degree-raising differentials square to zero and anticommute. If an initial convention uses commuting differentials, introduce a sign in one of them before forming the [total cochain complex](#total-cochain-complex).

##### Two spectral sequences of a bounded double complex

↑ **Parent:** [Double cochain complex](#double-cochain-complex)

Filtering the [total cochain complex](#total-cochain-complex) by each index yields two [spectral sequences](algebra.md#spectral-sequence). One first takes vertical cohomology and the other horizontal cohomology; boundedness ensures both converge to total cohomology.

##### Total cochain complex

↑ **Parent:** [Double cochain complex](#double-cochain-complex)

The total differential is $d_h+d_v$ for anticommuting differentials. For a [double cochain complex](#double-cochain-complex) bounded in both indices, both index filtrations are finite and have the same total [cohomology](cohomology.md) as abutment.

### Koszul complex

↑ **Parent:** [Chain complex](#chain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koszul_complex)

The Koszul complex on $f_1,\ldots,f_r$ has term $K_i=\bigwedge^iR^r$ and differential $\partial(e_{j_1}\wedge\cdots\wedge e_{j_i})=\sum_a(-1)^{a-1}f_{j_a}e_{j_1}\wedge\cdots\wedge\widehat{e_{j_a}}\wedge\cdots\wedge e_{j_i}$. Its degree-zero [homology](homology.md) is $R/(f_1,\ldots,f_r)$. For a [regular sequence](commutative-algebra.md#regular-sequence) it is exact in positive degrees, hence a [Koszul resolution](algebra.md#koszul-resolution) of that quotient. The variables of a [polynomial ring](commutative-algebra.md#polynomial-ring) form a [regular sequence](commutative-algebra.md#regular-sequence), so this resolves the coefficient [field](algebra.md#field) in length equal to the number of variables.

#### Self-duality of the Koszul complex

↑ **Parent:** [Koszul complex](#koszul-complex)

The perfect exterior pairing in complementary degrees identifies the dual of a [Koszul complex](#koszul-complex) with its degree reversal, with suitable differential signs. For a [regular sequence](commutative-algebra.md#regular-sequence), its [Koszul resolution](algebra.md#koszul-resolution) consequently gives $\operatorname{Ext}_R^i(R/(f),R)=0$ except in degree $r$, where it is $R/(f)$.

#### Koszul acyclicity criterion in a Noetherian local ring

↑ **Parent:** [Koszul complex](#koszul-complex)

Let $(R,\mathfrak m)$ be a [Noetherian local ring](algebra.md#noetherian-local-ring), let $M$ be nonzero and finitely generated, and let every $f_i$ lie in $\mathfrak m$. Then positive [Koszul homology](#koszul-homology) vanishes exactly when $f$ is a [regular sequence on a module](module-theory.md#regular-sequence-on-a-module) $M$. The [mapping cone](#mapping-cone-homological-algebra) exact sequence proves the forward implication by induction; surjectivity of the last generator on earlier homology and the [Nakayama lemma](mathematics.md#nakayama-lemma) prove the converse.

#### Koszul complex with module coefficients

↑ **Parent:** [Koszul complex](#koszul-complex)

Tensor the finite free [Koszul complex](#koszul-complex) on $f_1,\ldots,f_r$ with the module $M$. For a [regular sequence on a module](module-theory.md#regular-sequence-on-a-module), its positive [Koszul homology](#koszul-homology) vanishes. If the sequence is regular on $R$, this complex instead computes $\operatorname{Tor}^R(R/(f),M)$ for arbitrary $M$.

#### Koszul homology

↑ **Parent:** [Koszul complex](#koszul-complex)

Koszul homology is the homology of the [Koszul complex with module coefficients](#koszul-complex-with-module-coefficients). Its degree-zero term is $M/(f)M$, and its positive terms record failures of regularity. Each generator acts trivially on homology by the [Koszul homotopy for multiplication by a generator](#koszul-homotopy-for-multiplication-by-a-generator).

##### Koszul homotopy for multiplication by a generator

↑ **Parent:** [Koszul homology](#koszul-homology)

Exterior multiplication $h_j(u)=e_j\wedge u$ is a [chain homotopy](#chain-homotopy) between multiplication by $f_j$ and zero on a [Koszul complex](#koszul-complex). A linear combination of these homotopies is a [contracting homotopy](#contracting-homotopy) when the generators span the unit ideal.

#### Koszul complex on central ring elements

↑ **Parent:** [Koszul complex](#koszul-complex)

For a possibly noncommutative ring and central $t_i$, the formal exterior basis gives free [bimodules](module-theory.md#bimodule) with differential $d(e_{i_1}\wedge\cdots\wedge e_{i_k})=\sum_a(-1)^{a-1}t_{i_a}e_{i_1}\wedge\cdots\widehat{e_{i_a}}\cdots\wedge e_{i_k}$. Centrality makes this a bimodule differential. Pairwise cancellation proves $d^2=0$.

### Augmented chain complex

↑ **Parent:** [Chain complex](#chain-complex)

An augmented [chain complex](#chain-complex) includes an augmentation $\varepsilon:C_0\to\mathbb Z$ with $\varepsilon d_1=0$. For a nonempty [simplicial complex](algebraic-topology.md#simplicial-complex), the augmentation sends every vertex to $1$ and the augmented homology in degree zero is its [reduced homology](#reduced-homology).

### Chain group

↑ **Parent:** [Chain complex](#chain-complex)

The chain group $C_i$ is the group in degree $i$ of a [chain complex](#chain-complex). Its elements are $i$-chains.

### Chain subcomplex

↑ **Parent:** [Chain complex](#chain-complex)

A chain subcomplex $D_\bullet\subseteq C_\bullet$ consists of subgroups $D_i\leq C_i$ preserved by the [boundary operator](#boundary-operator): $\partial(D_i)\subseteq D_{i-1}$.

### Boundary operator

↑ **Parent:** [Chain complex](#chain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boundary_operator)

The boundary operator of a [chain complex](#chain-complex) is its degree-minus-one differential $\partial:C_i\to C_{i-1}$. The identity $\partial^2=0$ says that every [chain boundary](#chain-boundary) is a [chain cycle](#chain-cycle).

### Cellular chain complex

↑ **Parent:** [Chain complex](#chain-complex)

For a CW complex, $C_n^{\mathrm{cell}}(X)=H_n(X^n,X^{n-1})$ is freely generated by the oriented $n$-cells. Connecting maps of skeleton pairs define its differential.

#### Cellular chain group

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

For a [CW complex](algebraic-topology.md#cw-complex), the qth [cellular chain group](#cellular-chain-group) is the relative [homology group](#homology-group) of successive skeleta, a [free abelian group](group-theory.md#free-abelian-group) with one generator for each q-cell. The attaching maps determine the [cellular boundary](#cellular-boundary), and the resulting [cellular chain complex](#cellular-chain-complex) computes [singular homology](#singular-homology).

#### Cellular chain

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

A finite linear combination, with coefficients in $R$, of the oriented $n$-cells of a [CW complex](algebraic-topology.md#cw-complex).

#### Cellular cycle

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

A [cellular chain](#cellular-chain) whose cellular boundary is zero.

##### Cellular boundary

↑ **Parent:** [Cellular cycle](#cellular-cycle)

A [cellular chain](#cellular-chain) that is the boundary of a chain one dimension higher. The chain-complex identity $d_nd_{n+1}=0$ makes every cellular boundary a [cellular cycle](#cellular-cycle); their quotient is [cellular homology](#cellular-chain-complex).

#### Cellular chains of a product of finite CW complexes

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

The product cells of finite [CW complexes](algebraic-topology.md#cw-complex) give the [tensor product](linear-algebra.md#tensor-product) of their [cellular chain complexes](#cellular-chain-complex). The boundary formula is the displayed signed product rule. The sign comes from moving the outward normal of the second factor past the $p$ oriented tangent directions of the first factor. This is the cellular counterpart of the [Eilenberg–Zilber theorem](cohomology.md#eilenberg-zilber-theorem).

#### Homology of a torus with two parallel circles collapsed

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

Collapse two distinct parallel circles of a [torus](topology.md#torus) to two separate points. Cutting between the circles gives two annuli, each of which becomes a two-sphere with the two collapsed points as its poles. The resulting [CW complex](algebraic-topology.md#cw-complex) has two vertices, two edges connecting them, and two two-cells with zero cellular boundary. Its homology is as displayed, with all higher groups zero; it is homotopy equivalent to $S^1\vee S^2\vee S^2$.

#### Cellular homology theorem

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

For a [CW complex](algebraic-topology.md#cw-complex), the [homology](homology.md) of its [cellular chain complex](#cellular-chain-complex) naturally equals its [singular homology](#singular-homology). The relative groups of successive skeleton pairs, free on the cells in the corresponding dimension and zero in other dimensions, yield this identification through their connecting maps.

#### Cellular cochain complex

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

For a [CW complex](algebraic-topology.md#cw-complex), applying $\operatorname{Hom}(-,A)$ to its integral [cellular chain complex](#cellular-chain-complex) gives a cochain complex. The differential is precomposition with the cellular boundary. For finitely many cells it is represented by the transpose of the boundary matrix, reduced in the coefficient group when appropriate.

##### Cellular cohomology

↑ **Parent:** [Cellular cochain complex](#cellular-cochain-complex)

The [cohomology](cohomology.md) of the [cellular cochain complex](#cellular-cochain-complex) naturally agrees with singular cohomology. A [CW complex](algebraic-topology.md#cw-complex) with no odd cells has zero cellular differentials and free integral cohomology on its even cells, although its [cup product](cohomology.md#cup-product) still requires a separate computation.

###### One-cell bound on next-degree cohomology

↑ **Parent:** [Cellular cohomology](#cellular-cohomology)

If an $n$-dimensional [CW complex](algebraic-topology.md#cw-complex) is extended by exactly one cell in dimension $n+1$, then its cellular [cochain](cohomology.md#singular-cochain) group in that degree is the coefficient [field](algebra.md#field) $k$. Regardless of how many higher cells are attached, the [cohomology](cohomology.md) is a quotient of a subspace of that one-dimensional group. This gives the displayed bound. Finiteness of the higher cell sets is unnecessary for this particular conclusion.

###### Coprime two-cell attachments to a circle

↑ **Parent:** [Cellular cohomology](#cellular-cohomology)

The cellular boundary $\mathbb Z^2\to\mathbb Z$ is $(m,n)$, with kernel $\mathbb Z$ and zero cokernel when the degrees are coprime. The [van Kampen theorem](algebraic-topology.md#seifert-van-kampen-theorem) gives trivial fundamental group. The [Hurewicz theorem](algebraic-topology.md#hurewicz-theorem) supplies a map from the sphere representing a homology generator, and the [homological Whitehead theorem](algebraic-topology.md#homological-whitehead-theorem) makes it a homotopy equivalence. For degrees $2,3$ the space cannot be homeomorphic to a sphere: an embedded circle in a sphere bounds its two complementary regions, so both characteristic boundary maps would have degree of absolute value one.

#### Cellular boundary formula

↑ **Parent:** [Cellular chain complex](#cellular-chain-complex)

The coefficient of an $(n-1)$-cell in the cellular boundary of an $n$-cell is the degree of the attaching map after collapsing the complement of that $(n-1)$-cell to obtain a map $S^{n-1}\to S^{n-1}$.

### Chain cycle

↑ **Parent:** [Chain complex](#chain-complex)

An element of a [chain group](#chain-group) is a cycle when its [boundary operator](#boundary-operator) kills it. A cycle need not itself be a [chain boundary](#chain-boundary). The [homology group](#homology-group) $H_n(C)$ identifies cycles whose difference is a [chain boundary](#chain-boundary).

### Chain boundary

↑ **Parent:** [Chain complex](#chain-complex)

An element of a [chain group](#chain-group) is a boundary when it is the image of a higher-degree element under the [boundary operator](#boundary-operator). Since $\partial^2=0$, every boundary is a [chain cycle](#chain-cycle). Thus $H_n(C)=Z_n(C)/B_n(C)$, and a [chain cycle](#chain-cycle) represents zero in [homology](homology.md) exactly when it is a boundary.

### Chain coefficient

↑ **Parent:** [Chain complex](#chain-complex)

The coefficients of a chain are the scalars multiplying its basis simplices.

### Chain map

↑ **Parent:** [Chain complex](#chain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chain_map)

A chain map $f:C\to C'$ is a family $f_i:C_i\to C'_i$ satisfying $d'_if_i=f_{i-1}d_i$.

#### Quasi-isomorphism

↑ **Parent:** [Chain map](#chain-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-isomorphism)

A [chain map](#chain-map) inducing isomorphisms on all [homology groups](#homology-group). The same definition applies to a map of [cochain complexes](algebra.md#cochain-complex) using [cohomology groups](cohomology.md#cohomology-group). A quasi-isomorphism need not be an isomorphism in each degree.

##### Prime coefficient detection of quasi-isomorphisms

↑ **Parent:** [Quasi-isomorphism](#quasi-isomorphism)

Let $f$ be a [chain map](#chain-map) between degreewise finitely generated [free abelian groups](group-theory.md#free-abelian-group). If its reduction modulo every [prime number](number-theory.md#prime-number) is a [quasi-isomorphism](#quasi-isomorphism), the [mapping cone acyclicity criterion](#mapping-cone-acyclicity-criterion) makes $M(f)\otimes\mathbb F_p$ acyclic. The [short exact sequence of chain complexes](#short-exact-sequence-of-chain-complexes) $0\to M\xrightarrow{p}M\to M\otimes\mathbb F_p\to0$ implies that multiplication by $p$ is an [isomorphism](algebra.md#isomorphism) on every $H_i(M)$. These are [finitely generated abelian groups](group.md#finitely-generated-abelian-group). Their free summands would make multiplication by $p$ fail to be surjective, and any nonzero finite summand would make it fail to be injective for a prime dividing its order. Thus $H_i(M)=0$ and $f$ is a [quasi-isomorphism](#quasi-isomorphism). Degreewise finite generation is essential to this argument.

#### Induced map on homology

↑ **Parent:** [Chain map](#chain-map)

A chain map sends cycles to cycles and boundaries to boundaries, and therefore induces $f_*:H_i(C)\to H_i(C')$ by $[x]\mapsto[f_i(x)]$.

#### Chain homotopy

↑ **Parent:** [Chain map](#chain-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chain_homotopy)

Chain maps $f,g:C\to C'$ are chain homotopic when there are maps $h_i:C_i\to C'_{i+1}$ such that

$$
f_i-g_i=d'_{i+1}h_i+h_{i-1}d_i.
$$

Chain-homotopic maps induce the same map on homology.

##### Contracting homotopy

↑ **Parent:** [Chain homotopy](#chain-homotopy)

A contracting homotopy on a [chain complex](#chain-complex) is a degree-one map $h$ whose displayed identity makes the identity chain-homotopic to zero. It implies that all homology vanishes. The converse is not valid for arbitrary complexes of modules.

##### Cochain homotopy

↑ **Parent:** [Chain homotopy](#chain-homotopy)

For cochain maps $f,g:C^\bullet\to D^\bullet$, a cochain homotopy is a family $K:C^q\to D^{q-1}$ satisfying

$$
f-g=dK+Kd.
$$

Cochain-homotopic maps induce the same map on [cohomology](cohomology.md).

##### Small simplex theorem

↑ **Parent:** [Chain homotopy](#chain-homotopy)

For an open cover $\mathcal U$ of $X$, singular chains generated by simplices lying inside one member of $\mathcal U$ form a subcomplex chain-homotopy equivalent to the full singular chain complex. Repeated barycentric subdivision makes chains small.

### Mapping cone (homological algebra)

↑ **Parent:** [Chain complex](#chain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mapping_cone_(homological_algebra))

For a chain map $f:C\to C'$, one mapping-cone convention takes $M(f)_i=C_{i-1}\oplus C'_i$ with a differential combining $d,d'$ and $f$. Its short exact sequence with $C'$ and a shift of $C$ produces a long exact sequence in homology.

#### Mapping cone acyclicity criterion

↑ **Parent:** [Mapping cone (homological algebra)](#mapping-cone-homological-algebra)

For a [chain map](#chain-map) $f:C\to D$, use $M_i=C_{i-1}\oplus D_i$ and $d(x,y)=(d_Cx,(-1)^if(x)+d_Dy)$. The [chain map](#chain-map) identity makes $d^2=0$. The [short exact sequence of chain complexes](#short-exact-sequence-of-chain-complexes) $0\to D\to M\to C_{*-1}\to0$ has [connecting homomorphism](#connecting-homomorphism) $(-1)^if_*$ in degree $i$. Its [long exact sequence in homology](#long-exact-sequence-in-homology) shows that the [homology](homology.md) of $M$ vanishes precisely when every $f_*$ is an [isomorphism](algebra.md#isomorphism).

### Short exact sequence of chain complexes

↑ **Parent:** [Chain complex](#chain-complex)

A degreewise short exact sequence $0\to A\to B\to C\to0$ of chain complexes induces a long exact sequence of homology groups through the connecting homomorphisms.

#### Long exact sequence in homology

↑ **Parent:** [Short exact sequence of chain complexes](#short-exact-sequence-of-chain-complexes)

The connecting map sends a homology class in the quotient complex to the class obtained by lifting a representative, applying the middle differential, and identifying the result in the subcomplex.

##### Connecting homomorphism

↑ **Parent:** [Long exact sequence in homology](#long-exact-sequence-in-homology)

The connecting homomorphism is the degree-shifting map produced by the lift-and-boundary construction in a long exact sequence.

###### Relative homology connecting homomorphism

↑ **Parent:** [Connecting homomorphism](#connecting-homomorphism)

A relative cycle is represented by a [singular chain](#singular-chain) $b$ whose boundary lies in $A$. Define $\delta[\bar b]=[\partial b]$. If a representative changes by $\partial c+a$ with $a\in C_n(A)$, its boundary changes by $\partial a$, an $A$-boundary. Thus the map is well-defined and additive. Its image is exactly the kernel of $H_{n-1}(A)\to H_{n-1}(B)$: a cycle in $A$ dies in $B$ precisely when it is the boundary of a relative cycle lifted to $B$. This proves the corresponding exactness in the [long exact sequence in relative homology](#long-exact-sequence-in-relative-homology) directly.

###### Bockstein homomorphism

↑ **Parent:** [Connecting homomorphism](#connecting-homomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bockstein_homomorphism)

The Bockstein homomorphism is the connecting homomorphism associated with a short exact sequence of coefficient groups. For $0\to\mathbb Z/n\to\mathbb Z/n^2\to\mathbb Z/n\to0$, it has degree $-1$ on homology and degree $+1$ on cohomology.

###### Bockstein on infinite real projective space

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

For the coefficient sequence $0\to\mathbb Z_2\to\mathbb Z_4\to\mathbb Z_2\to0$, the [Bockstein homomorphism](#bockstein-homomorphism) on [infinite-dimensional real projective space](algebraic-topology.md#infinite-dimensional-real-projective-space) is zero from an even degree and an isomorphism from an odd degree. In [cellular cohomology](#cellular-cohomology), lift the mod-two generator to $1\in\mathbb Z_4$. The coboundary is zero in even degree and two in odd degree; identifying two with the image of $1\in\mathbb Z_2$ gives the formula.

###### Bockstein factorization through integral cohomology

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

The [Bockstein homomorphism](#bockstein-homomorphism) for $0\to\mathbb Z/n\to\mathbb Z/n^2\to\mathbb Z/n\to0$, with injection $[a]\mapsto[na]$, is coefficient reduction $\rho$ after the [integral Bockstein homomorphism](#integral-bockstein-homomorphism). The commuting maps of coefficient sequences prove this by naturality of the [connecting homomorphism](#connecting-homomorphism).

###### Degree-one Bockstein square identity

↑ **Parent:** [Bockstein factorization through integral cohomology](#bockstein-factorization-through-integral-cohomology)

Reduction $\rho$ of the [integral Bockstein homomorphism](#integral-bockstein-homomorphism) associated to $0\to\mathbb Z\xrightarrow{2}\mathbb Z\to\mathbb F_2\to0$ equals the [cup product](cohomology.md#cup-product) square on degree-one classes. One can see this on an ordered two-simplex: lift the values of a mod-two one-cocycle to zero or one. The half-coboundary is one precisely when both consecutive edge values are one, giving the cup-square cocycle.

###### Bockstein square-zero identity

↑ **Parent:** [Bockstein factorization through integral cohomology](#bockstein-factorization-through-integral-cohomology)

Exactness of the integral coefficient sequence gives $\widehat\beta\rho=0$. The [Bockstein factorization through integral cohomology](#bockstein-factorization-through-integral-cohomology) therefore gives $\beta^2=\rho\widehat\beta\rho\widehat\beta=0$, for every modulus $n\geq2$, including composite moduli.

###### Bockstein cohomology

↑ **Parent:** [Bockstein square-zero identity](#bockstein-square-zero-identity)

The degree-one [Bockstein homomorphism](#bockstein-homomorphism) makes modulo-$n$ [cohomology](cohomology.md) into a [cochain complex](algebra.md#cochain-complex). Its cohomology is the Bockstein cohomology. For prime $n$ this is a graded vector space; for composite $n$ it is a graded $\mathbb Z/n$-module. For $\mathbb{RP}^3$ at modulus two, its only nonzero groups are $\mathbb F_2$ in degrees zero and three. This is the cohomological counterpart of [Bockstein homology](#bockstein-homology).

###### Integral Bockstein homomorphism

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

The integral Bockstein is the [connecting homomorphism](#connecting-homomorphism) of $0\to\mathbb Z\xrightarrow{n}\mathbb Z\to\mathbb Z/n\to0$. Lift a modulo-$n$ cocycle to an integral cochain $a$; write its coboundary as $\delta a=nb$. Then $\widehat\beta[a]=[b]$. Its image is the subgroup of integral [cohomology](cohomology.md) killed by $n$.

###### Bockstein isomorphism for a three-dimensional lens space

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

For the three-dimensional [lens space](knot-theory.md#lens-space) $L(p)$, the integral coefficient sequence shows that the integral connecting map $H^1(L(p);\mathbb F_p)\to H^2(L(p);\mathbb Z)$ is an isomorphism between groups of order $p$. Reduction modulo $p$ is also an isomorphism in degree two, so their composite Bockstein is an isomorphism.

###### Bockstein linking invariant of a three-dimensional lens space

↑ **Parent:** [Bockstein isomorphism for a three-dimensional lens space](#bockstein-isomorphism-for-a-three-dimensional-lens-space)

For a generator $a\in H^1(L(p);\mathbb F_p)$, [Poincare duality](cohomology.md#poincare-duality) and the [Bockstein isomorphism for a three-dimensional lens space](#bockstein-isomorphism-for-a-three-dimensional-lens-space) make $t(a)$ nonzero. Replacing $a$ by $na$ multiplies $t(a)$ by $n^2$. An orientation-reversing homotopy equivalence multiplies the evaluation by $-1$, so its existence forces $n^2=-1$ in $\mathbb F_p$ for some $n$.

###### Bockstein homology

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

When the homological Bockstein satisfies $\beta^2=0$, it makes $H_*(C\otimes\mathbb Z/n)$ into a chain complex. Its homology is the Bockstein homology $\beta H_*(C;n)$.

###### Long exact sequence from a coefficient sequence

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

A short exact sequence of coefficient groups $0\to A\to B\to C\to0$ induces a natural long exact sequence

$$
\cdots\to H^i(X;A)\to H^i(X;B)\to H^i(X;C)
\xrightarrow{\delta}H^{i+1}(X;A)\to\cdots.
$$

The connecting map is a [Bockstein homomorphism](#bockstein-homomorphism).

###### Bockstein derivation rule

↑ **Parent:** [Bockstein homomorphism](#bockstein-homomorphism)

For the modulo-$m$ cohomological [Bockstein homomorphism](#bockstein-homomorphism),

$$
\beta(x\smile y)=\beta(x)\smile y+(-1)^{|x|}x\smile\beta(y).
$$

This follows by lifting cocycles to integral cochains and applying the graded Leibniz rule for the coboundary before dividing by $m$.

### Elementary decomposition of a finite free chain complex

↑ **Parent:** [Chain complex](#chain-complex)

Over the principal ideal domain $\mathbb Z$, [Smith normal form](algebra.md#smith-normal-form) decomposes a chain complex of finitely generated free modules into direct sums of one-term complexes $\mathbb Z$ and two-term complexes

$$
0\longrightarrow\mathbb Z\xrightarrow{m}\mathbb Z\longrightarrow0.
$$

The one-term summands record free homology, the summands with $m>1$ record cyclic torsion, and those with $m=1$ are acyclic.

### Detection of integral acyclicity modulo primes

↑ **Parent:** [Chain complex](#chain-complex)

If a chain complex of finitely generated free abelian groups has zero homology after tensoring with $\mathbb F_p$ for every prime $p$, then its integral homology vanishes. The [universal coefficient theorem for homology](#universal-coefficient-theorem-for-homology) detects a free summand modulo every prime and detects a nonzero finite summand modulo any prime dividing its order.

## Universal coefficient theorem for homology

↑ **Parent:** [Homology (mathematics)](homology.md)

For an abelian coefficient group $G$, there is a split short exact sequence

$$
0\to H_i(X;\mathbb Z)\otimes G
\to H_i(X;G)
\to\operatorname{Tor}(H_{i-1}(X;\mathbb Z),G)\to0.
$$

For $G=\mathbb Q$, the Tor term vanishes.

This is the homology case of the [universal coefficient theorem](#universal-coefficient-theorem); its cohomology case uses Hom and Ext rather than tensor product and Tor.

### Rational homology

↑ **Parent:** [Universal coefficient theorem for homology](#universal-coefficient-theorem-for-homology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_homology)

Rational homology satisfies

$$
H_i(X;\mathbb Q)\cong H_i(X;\mathbb Z)\otimes_\mathbb Z\mathbb Q.
$$

It records the free rank of integral homology and discards torsion.

## Simplicial homology

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplicial_homology)

Simplicial homology computes homology from the boundary maps between free abelian groups generated by oriented simplices.

### Simplicial cycle

↑ **Parent:** [Simplicial homology](#simplicial-homology)

A simplicial cycle is a simplicial chain with zero boundary. Its homology class is unchanged on addition of a boundary; in the [Mayer–Vietoris sequence](algebraic-topology.md#mayer-vietoris-sequence), splitting a cycle between two subcomplexes constructs the connecting map.

### Simplicial chain complex

↑ **Parent:** [Simplicial homology](#simplicial-homology)

The simplicial chain group $C_n(K)$ is freely generated by oriented $n$-simplices, subject to reversal of orientation changing sign. Its boundary is

$$
\partial[v_0\cdots v_n]
=\sum_{i=0}^n(-1)^i[v_0\cdots\widehat v_i\cdots v_n].
$$

#### Simplicial cone chain contraction

↑ **Parent:** [Simplicial chain complex](#simplicial-chain-complex)

In an [augmented chain complex](#augmented-chain-complex) of a simplex with vertices $v_0,\ldots,v_n$, put $s(1)=[v_0]$ and $s[v_{i_0},\ldots,v_{i_q}]=[v_0,v_{i_0},\ldots,v_{i_q}]$ when $v_0$ is absent, and zero when it is present. Direct expansion of the [boundary operator](#boundary-operator) gives $ds+sd=1$. This proves that every positive-degree [chain cycle](#chain-cycle) is a [chain boundary](#chain-boundary), without invoking [cellular homology](#cellular-chain-complex).

### Euler characteristic

↑ **Parent:** [Simplicial homology](#simplicial-homology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_characteristic)

For a finite complex,

$$
\chi(X)=\sum_i(-1)^i\dim_\mathbb QH_i(X;\mathbb Q).
$$

#### Odd-dimensional closed manifolds have zero Euler characteristic

↑ **Parent:** [Euler characteristic](#euler-characteristic)

Use [Poincare duality](cohomology.md#poincare-duality) with coefficients in $\mathbb F_2$, valid also without orientability. The ranks in complementary degrees agree, and their signs in the alternating sum are opposite. They therefore cancel in pairs. Euler characteristic is independent of the coefficient field, giving the stated integer equality.

#### Euler characteristics of closed oriented four-manifolds

↑ **Parent:** [Euler characteristic](#euler-characteristic)

[Poincare duality](cohomology.md#poincare-duality) gives the displayed formula for connected closed oriented four-manifolds. Every integer occurs. A [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds) of $r$ copies of the [Complex projective plane](algebraic-topology.md#complex-projective-plane) and $s$ copies of $S^1\times S^3$ has Euler characteristic $2+r-2s$, because the summand characteristics are three and zero. Given any integer $h$, choose $s$ large enough that $r=h-2+2s\geq0$; when both counts are zero use $S^4$. If simple connectivity is additionally required, the possible values instead begin at two, since $b_1=0$; connected sums of projective planes realize every such value.

#### Ordinary vertex in a nonconcurrent great-circle arrangement

↑ **Parent:** [Euler characteristic](#euler-characteristic)

A finite set of distinct [great circles](geometry-and-topology.md#great-circle) not all passing through a common antipodal pair has a vertex lying on exactly two circles. Its cells are spherical polygons with at least three edges: a digon would have antipodal endpoints, and every circle's defining hemisphere would then have to contain both endpoints, forcing a common axis. With $V-E+F=2$ and $3F\leq2E$, the graph has a vertex of valence less than six. Valences are even and at least four, so one is exactly four. Central projection identifies this with an ordinary intersection in a real projective line arrangement. If affine line intersections are counted only at finite points, parallel-line configurations require a separate qualification.

#### Euler formula for a sphere

↑ **Parent:** [Euler characteristic](#euler-characteristic)

For a finite cell decomposition of the [sphere](geometry-and-topology.md#sphere) into polygonal faces, the numbers of vertices, edges and faces satisfy the displayed formula. Triangulating faces preserves $V-E+F$ because each added diagonal adds one edge and one face. This is the spherical form of [Euler formula for a connected planar graph](graph-theory.md#euler-formula-for-a-connected-planar-graph), where the plane's exterior face is included.

#### Euler characteristic of a product

↑ **Parent:** [Euler characteristic](#euler-characteristic)

For finite CW complexes, the product cell structure has one $(p+q)$-cell for every pair consisting of a $p$-cell and a $q$-cell. Taking the alternating cell count gives

$$
\chi(X\times Y)=\chi(X)\chi(Y).
$$

#### Euler characteristic under a finite covering

↑ **Parent:** [Euler characteristic](#euler-characteristic)

If $p:X\to Y$ is a finite covering of degree $d$ between spaces having finite CW type, then

$$
\chi(X)=d\chi(Y).
$$

A lifted CW structure has exactly $d$ cells above each cell of the base.

#### Euler characteristic of an odd-dimensional closed manifold

↑ **Parent:** [Euler characteristic](#euler-characteristic)

Every closed odd-dimensional manifold has Euler characteristic zero. For an orientable manifold this follows by pairing complementary Betti numbers using [Poincare duality](cohomology.md#poincare-duality); the general case follows from the orientable double cover and [Euler characteristic under a finite covering](#euler-characteristic-under-a-finite-covering).

#### Euler-Poincare formula

↑ **Parent:** [Euler characteristic](#euler-characteristic)

If a finite simplicial complex has $f_i$ simplices of dimension $i$, then

$$
\chi(X)=\sum_i(-1)^if_i.
$$

Writing $C_i=Z_i\oplus$ a lift of $B_{i-1}$ and $Z_i=H_i\oplus B_i$ makes the boundary dimensions cancel in the alternating sum.

### Barycentric subdivision

↑ **Parent:** [Simplicial homology](#simplicial-homology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barycentric_subdivision)

The vertices of the barycentric subdivision of a simplicial complex are its nonempty faces, and its simplices are strict chains of faces.

#### Iterated barycentric subdivision

↑ **Parent:** [Barycentric subdivision](#barycentric-subdivision)

The iterated barycentric subdivisions are defined recursively by $K^{(0)}=K$ and $K^{(r+1)}=(K^{(r)})'$.

#### Mesh of a simplicial complex

↑ **Parent:** [Barycentric subdivision](#barycentric-subdivision)

For a geometrically realized simplicial complex, its mesh is

$$
\mu(K)=\sup_{\sigma\in K}\operatorname{diam}|\sigma|.
$$

If $K$ has dimension $n$, barycentric subdivision satisfies

$$
\mu(K')\leq\frac{n}{n+1}\mu(K),
$$

so $\mu(K^{(r)})\to0$.

#### Barycentric subdivision of a tetrahedron

↑ **Parent:** [Barycentric subdivision](#barycentric-subdivision)

The barycentric subdivision of a tetrahedron has f-vector

$$
(f_0,f_1,f_2,f_3)=(15,50,60,24).
$$

Its two-skeleton therefore has Euler characteristic $15-50+60=25$ and homology $H_0\cong\mathbb Z$, $H_1=0$, and $H_2\cong\mathbb Z^{24}$.

## Local homology

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_homology)

The local homology at $x\in X$ is $H_i(X,X\setminus\{x\})$. It is preserved by homeomorphisms and, in a simplicial complex, is computed from the reduced homology of the local link.

### Local homology from a link

↑ **Parent:** [Local homology](#local-homology)

If a neighborhood of $x$ is a cone on a compact link $L$, excision and the long exact sequence of the cone pair give

$$
H_i(X,X\setminus\{x\})\cong\widetilde H_{i-1}(L).
$$

### Fixed barycentre of the barycentric tetrahedral two-skeleton

↑ **Parent:** [Local homology](#local-homology)

In the two-skeleton of a barycentrically subdivided tetrahedron, the vertex corresponding to the whole tetrahedron has link equal to the connected 1-skeleton of the subdivided boundary, with 14 vertices and 36 edges. Its local $H_2$ therefore has rank $36-14+1=23$. Every other point has smaller local rank, so every self-homeomorphism fixes this vertex.

## Intersection form of a 4-manifold

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_form_of_a_4-manifold)

The [intersection form of a 4-manifold](#intersection-form-of-a-4-manifold) is the middle-dimensional signed-intersection pairing of an oriented compact four-manifold. On a closed manifold it can equivalently be defined on second cohomology by evaluating the cup product on the fundamental class. The general [intersection form](#intersection-form) also applies to higher dimensions.

## Universal coefficient theorem

↑ **Parent:** [Homology (mathematics)](homology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universal_coefficient_theorem)

The [universal coefficient theorem](#universal-coefficient-theorem) relates homology or cohomology with different coefficient groups through tensor and Tor, or Hom and Ext, respectively. The [universal coefficient theorem for homology](#universal-coefficient-theorem-for-homology) is its tensor-Tor sequence; the [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology) is its Hom-Ext sequence.

## ↑ Ancestors (5)

1. [Algebraic topology](algebraic-topology.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (171)

- [Acyclic space](#acyclic-space)
- [Alexander module of a space](algebraic-topology.md#alexander-module-of-a-space)
- [Borel-Moore homology](#borel-moore-homology)
- [Cellular approximation theorem](algebraic-topology.md#cellular-approximation-theorem)
- [Cellular homology theorem](#cellular-homology-theorem)
- [Chain boundary](#chain-boundary)
- [Classification of compact surfaces](topology.md#classification-of-compact-surfaces)
- [Cohomological Künneth theorem over a field](cohomology.md#cohomological-kunneth-theorem-over-a-field)
- [Cohomology](cohomology.md)
- [Connective generalized homology detects simply connected equivalences](algebraic-topology.md#connective-generalized-homology-detects-simply-connected-equivalences)
- [Double complex](#double-complex)
- [Double of a manifold](topology.md#double-of-a-manifold)
- [Finite CW approximation from bounded homology](algebraic-topology.md#finite-cw-approximation-from-bounded-homology)
- [Finite type CW approximation](algebraic-topology.md#finite-type-cw-approximation)
- [First Betti-number bound from polynomial fundamental-group growth](geometric-group-theory.md#first-betti-number-bound-from-polynomial-fundamental-group-growth)
- [Graded Hom complex of chain complexes](#graded-hom-complex-of-chain-complexes)
- [Group homology](group-theory.md#group-homology)
- [Haken sum](topology.md#haken-sum)
- [Homological algebra](algebra.md#homological-algebra)
- [Homological degree of a smooth complex plane curve](algebraic-geometry.md#homological-degree-of-a-smooth-complex-plane-curve)
- [Homological monodromy](algebraic-topology.md#homological-monodromy)
- [Homological transfer for a finite covering](algebraic-topology.md#homological-transfer-for-a-finite-covering)
- [Homological Whitehead theorem](algebraic-topology.md#homological-whitehead-theorem)
- [Homology after attaching a Möbius band to the real projective plane](algebraic-topology.md#homology-after-attaching-a-mobius-band-to-the-real-projective-plane)
- [Homology comparison proof of Freudenthal suspension](algebraic-topology.md#homology-comparison-proof-of-freudenthal-suspension)
- [Homology cross product](cohomology.md#homology-cross-product)
- [Homology group](#homology-group)
- [Homology obstruction to carrying surface curves onto one another](algebraic-topology.md#homology-obstruction-to-carrying-surface-curves-onto-one-another)
- [Homology of the complement of a smooth conic](algebraic-geometry.md#homology-of-the-complement-of-a-smooth-conic)
- [Homotopy groups of the stunted projective space through degree nine](algebraic-topology.md#homotopy-groups-of-the-stunted-projective-space-through-degree-nine)
- [Homotopy invariance of mapping degree](#homotopy-invariance-of-mapping-degree)
- [Homotopy sphere](cohomology.md#homotopy-sphere)
- [Homotopy type](algebraic-topology.md#homotopy-type)
- [Hopf band](knot-theory.md#hopf-band)
- [Hopf projection of a product smash quotient](algebraic-topology.md#hopf-projection-of-a-product-smash-quotient)
- [Hopf trace identity](#hopf-trace-identity)
- [Hurewicz theorem modulo a Serre class](algebraic-topology.md#hurewicz-theorem-modulo-a-serre-class)
- [Infinite cyclic cover associated to an epimorphism](algebraic-topology.md#infinite-cyclic-cover-associated-to-an-epimorphism)
- [Integral cohomology of an odd-sphere loop space](algebraic-topology.md#integral-cohomology-of-an-odd-sphere-loop-space)
- [Integral homology](#integral-homology)
- [Integral homology of the loop space of a sphere](algebraic-topology.md#integral-homology-of-the-loop-space-of-a-sphere)
- [Integral homology of two real projective planes](differential-geometry.md#integral-homology-of-two-real-projective-planes)
- [James reduced product](algebraic-topology.md#james-reduced-product)
- [Kernel cover of a real projective plane wedged with a circle](algebraic-topology.md#kernel-cover-of-a-real-projective-plane-wedged-with-a-circle)
- [Koszul complex](#koszul-complex)
- [Left derived functor](algebra.md#left-derived-functor)
- [Linking form of a branched cover](knot-theory.md#linking-form-of-a-branched-cover)
- [Loop-space homology](algebraic-topology.md#loop-space-homology)
- [Manin symbol](modular-function.md#manin-symbol)
- [Mapping cone acyclicity criterion](#mapping-cone-acyclicity-criterion)
- [Mapping cone exact sequence](algebraic-topology.md#mapping-cone-exact-sequence)
- [Mapping torus](algebraic-topology.md#mapping-torus)
- [Mapping-torus homology from Mayer–Vietoris](algebraic-topology.md#mapping-torus-homology-from-mayer-vietoris)
- [Milnor–Moore theorem](algebraic-topology.md#milnor-moore-theorem)
- [Moore space (algebraic topology)](algebraic-topology.md#moore-space-algebraic-topology)
- [Morse chain complex](differential-geometry.md#morse-chain-complex)
- [Morse-Smale complex](differential-geometry.md#morse-smale-complex)
- [Multiplicativity of mapping degree](#multiplicativity-of-mapping-degree)
- [Naturality of the cap product](cohomology.md#naturality-of-the-cap-product)
- [Nonseparating curve](geometry-and-topology.md#nonseparating-curve)
- [Null-homologous cycle](#null-homologous-cycle)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-13.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-16.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-16.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-26.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-26.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-27.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-17.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-17.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-13.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-18.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-18.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-22.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-22.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-16.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-16.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-16.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-16.md#4/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-20.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#21h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-16.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-16.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-16.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-55.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-14.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#18h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-15.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-127.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#19i/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-114.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-114.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#21g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#25g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-151.md#2/solution)
- [Perfect Morse function](differential-geometry.md#perfect-morse-function)
- [Poincare duality pairing](cohomology.md#poincare-duality-pairing)
- [Poincaré polynomial](#poincare-polynomial)
- [Pontryagin product on loop-space homology](algebraic-topology.md#pontryagin-product-on-loop-space-homology)
- [Pontryagin ring](algebraic-topology.md#pontryagin-ring)
- [Pontryagin ring of an odd-sphere loop space](algebraic-topology.md#pontryagin-ring-of-an-odd-sphere-loop-space)
- [Primitive homology class](#primitive-homology-class)
- [Rational homotopy theory](algebraic-topology.md#rational-homotopy-theory)
- [Rational Whitehead theorem](algebraic-topology.md#rational-whitehead-theorem)
- [Reidemeister torsion](algebraic-topology.md#reidemeister-torsion)
- [Relative homology of a fibration over a sphere](algebraic-topology.md#relative-homology-of-a-fibration-over-a-sphere)
- [Relative Hurewicz theorem](algebraic-topology.md#relative-hurewicz-theorem)
- [Seifert-matrix presentation of the Alexander module](knot-theory.md#seifert-matrix-presentation-of-the-alexander-module)
- [Serre class](group.md#serre-class)
- [Serre class of finitely generated abelian groups](group.md#serre-class-of-finitely-generated-abelian-groups)
- [Serre finiteness theorem for homotopy groups](algebraic-topology.md#serre-finiteness-theorem-for-homotopy-groups)
- [Singular chain complex](#singular-chain-complex)
- [Surjective rational Hurewicz homomorphism gives a wedge of spheres](algebraic-topology.md#surjective-rational-hurewicz-homomorphism-gives-a-wedge-of-spheres)
- [Three-sphere bundle over the four-sphere](fiber-bundle.md#three-sphere-bundle-over-the-four-sphere)
- [Tor functor](algebra.md#tor-functor)
- [Tower proof of the loop theorem](topology.md#tower-proof-of-the-loop-theorem)
- [Universal cover of a closed three-manifold with finite fundamental group](algebraic-topology.md#universal-cover-of-a-closed-three-manifold-with-finite-fundamental-group)
