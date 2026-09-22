# Algebraic variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_variety)

An algebraic variety is a geometric space locally described by polynomial equations, together with its regular functions.

**Table of contents**

- [Rational map of algebraic varieties](#rational-map-of-algebraic-varieties)
- [Ring of rational functions on a reduced variety](#ring-of-rational-functions-on-a-reduced-variety)
  - [Local ring embeds in rational functions on incident components](#local-ring-embeds-in-rational-functions-on-incident-components)
- [Rational function on an algebraic variety](#rational-function-on-an-algebraic-variety)
- [Quasi-projective algebraic set](#quasi-projective-algebraic-set)
  - [Quasi-projective variety](#quasi-projective-variety)
- [Irreducible variety](#irreducible-variety)
- [Constructible subset of a variety](#constructible-subset-of-a-variety)
  - [Chevalley constructibility theorem](#chevalley-constructibility-theorem)
- [Rational point](#rational-point)
- [Smooth algebraic variety](#smooth-algebraic-variety)
  - [Smoothness of an algebraic variety](#smoothness-of-an-algebraic-variety)
- [Normalization of an algebraic variety](#normalization-of-an-algebraic-variety)
- [Closed subvariety](#closed-subvariety)
- [Algebraic curve](#algebraic-curve)
  - [Cissoid of Diocles](#cissoid-of-diocles)
  - [Integral projective curve](#integral-projective-curve)
  - [Nonsingular point of an algebraic curve](#nonsingular-point-of-an-algebraic-curve)
  - [Affine algebraic curve](#affine-algebraic-curve)
    - [Folium of Descartes](#folium-of-descartes)
  - [Cuspidal cubic](#cuspidal-cubic)
    - [Unique smooth flex of a cuspidal cubic](#unique-smooth-flex-of-a-cuspidal-cubic)
    - [Cusp with two isolated-point components](#cusp-with-two-isolated-point-components)
  - [Symmetric product of a curve](#symmetric-product-of-a-curve)
  - [Monomial curve](#monomial-curve)
    - [Monomial curve with exponents three, four and five](#monomial-curve-with-exponents-three-four-and-five)
  - [Rational parametrization of an algebraic curve](#rational-parametrization-of-an-algebraic-curve)
  - [Arithmetic genus](#arithmetic-genus)
    - [Genus of a complete-intersection space curve](#genus-of-a-complete-intersection-space-curve)
- [Prevariety](#prevariety)
- [Algebraic group](#algebraic-group)
  - [Isogeny](#isogeny)
  - [Multiplicative group scheme](#multiplicative-group-scheme)
  - [Multiplicative algebraic group](#multiplicative-algebraic-group)
  - [Algebraic group action](#algebraic-group-action)
  - [Dimension formula for an algebraic group homomorphism](#dimension-formula-for-an-algebraic-group-homomorphism)
  - [Constructible subgroup is closed](#constructible-subgroup-is-closed)
  - [Homomorphism of group varieties](#homomorphism-of-group-varieties)
  - [Abelian variety](abelian-variety.md)
    - [Prime-to-characteristic torsion of an abelian variety](abelian-variety.md#prime-to-characteristic-torsion-of-an-abelian-variety)
    - [Jacobian variety](abelian-variety.md#jacobian-variety)
      - [Torelli theorem](abelian-variety.md#torelli-theorem)
      - [Universal property of the Jacobian variety](abelian-variety.md#universal-property-of-the-jacobian-variety)
      - [Theta divisor](abelian-variety.md#theta-divisor)
        - [Riemann vanishing theorem](abelian-variety.md#riemann-vanishing-theorem)
          - [Theta pullback zero-divisor identity](abelian-variety.md#theta-pullback-zero-divisor-identity)
          - [Vector of Riemann constants](abelian-variety.md#vector-of-riemann-constants)
        - [Gauss map of a theta divisor](abelian-variety.md#gauss-map-of-a-theta-divisor)
          - [Branch locus of the theta Gauss map](abelian-variety.md#branch-locus-of-the-theta-gauss-map)
        - [Riemann singularity theorem](abelian-variety.md#riemann-singularity-theorem)
          - [Schur complement presentation of a theta singularity](abelian-variety.md#schur-complement-presentation-of-a-theta-singularity)
          - [Tangent cone to a theta divisor](abelian-variety.md#tangent-cone-to-a-theta-divisor)
        - [Theta autoduality of a Jacobian](abelian-variety.md#theta-autoduality-of-a-jacobian)
        - [Restriction of the theta divisor to an Abel curve](abelian-variety.md#restriction-of-the-theta-divisor-to-an-abel-curve)
        - [Determinant description of the theta divisor](abelian-variety.md#determinant-description-of-the-theta-divisor)
          - [Invertible cup-product direction for a line bundle on a curve](abelian-variety.md#invertible-cup-product-direction-for-a-line-bundle-on-a-curve)
          - [Evaluation determinant on a product of curves](abelian-variety.md#evaluation-determinant-on-a-product-of-curves)
            - [Torsion trivialization in a determinant quotient](abelian-variety.md#torsion-trivialization-in-a-determinant-quotient)
      - [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve)
        - [Derivative of the Abelian sum map](abelian-variety.md#derivative-of-the-abelian-sum-map)
          - [Repeated-point Abel differential formula](abelian-variety.md#repeated-point-abel-differential-formula)
    - [Curve generation criterion for an abelian variety](abelian-variety.md#curve-generation-criterion-for-an-abelian-variety)
    - [Dual abelian variety](abelian-variety.md#dual-abelian-variety)
      - [Weil pairing for an abelian variety](abelian-variety.md#weil-pairing-for-an-abelian-variety)
      - [Poincaré line bundle](abelian-variety.md#poincare-line-bundle)
    - [Mumford rigidity lemma](abelian-variety.md#mumford-rigidity-lemma)
    - [Invariant differential on a group scheme](abelian-variety.md#invariant-differential-on-a-group-scheme)
    - [Theorem of the Cube](abelian-variety.md#theorem-of-the-cube)
      - [Arithmetic cube identity for Weil heights](abelian-variety.md#arithmetic-cube-identity-for-weil-heights)
      - [Cohomological proof of the cube theorem for elliptic curves](abelian-variety.md#cohomological-proof-of-the-cube-theorem-for-elliptic-curves)
      - [Bilinear cross-effect of a line bundle on an abelian variety](abelian-variety.md#bilinear-cross-effect-of-a-line-bundle-on-an-abelian-variety)
      - [Theorem of the square](abelian-variety.md#theorem-of-the-square)
        - [Homomorphism associated to a line bundle on an abelian variety](abelian-variety.md#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)
          - [Line bundle translation stabilizer](abelian-variety.md#line-bundle-translation-stabilizer)
          - [Identity component of the Picard group](abelian-variety.md#identity-component-of-the-picard-group)
            - [Seesaw theorem](abelian-variety.md#seesaw-theorem)
- [Smooth algebraic curve](#smooth-algebraic-curve)
  - [Product dimension bound for sections on a curve](#product-dimension-bound-for-sections-on-a-curve)
- [Affine algebraic set](#affine-algebraic-set)
  - [Affineness from a unit-ideal principal affine cover](#affineness-from-a-unit-ideal-principal-affine-cover)
  - [Morphism of affine varieties](#morphism-of-affine-varieties)
  - [Coordinate ring of a product of affine varieties](#coordinate-ring-of-a-product-of-affine-varieties)
  - [Vanishing ideal](#vanishing-ideal)
  - [Coordinate ring](#coordinate-ring)
    - [Irreducibility and prime vanishing ideal](#irreducibility-and-prime-vanishing-ideal)
    - [Dominant morphism of affine varieties](#dominant-morphism-of-affine-varieties)
  - [Vanishing loci of ideal sums and intersections](#vanishing-loci-of-ideal-sums-and-intersections)
  - [Irreducible components of two intersecting complex hyperbolas](#irreducible-components-of-two-intersecting-complex-hyperbolas)
- [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)
  - [Sheaf of nonzero rational functions on an irreducible variety](#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety)
  - [Dimension from the function field](#dimension-from-the-function-field)
  - [Projective model of a finitely generated field](#projective-model-of-a-finitely-generated-field)
- [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)
  - [Morphism of algebraic curves](#morphism-of-algebraic-curves)
  - [Conic bundle](#conic-bundle)
    - [Conic discriminant](#conic-discriminant)
      - [Reduced singular fibres of a smooth conic bundle](#reduced-singular-fibres-of-a-smooth-conic-bundle)
  - [Generically finite morphism](#generically-finite-morphism)
  - [Isomorphic local rings determine isomorphic neighborhoods](#isomorphic-local-rings-determine-isomorphic-neighborhoods)
  - [Degree of a morphism of curves](#degree-of-a-morphism-of-curves)
  - [Algebraic quotient by a finite group](#algebraic-quotient-by-a-finite-group)
  - [Affine-target adjunction for varieties](#affine-target-adjunction-for-varieties)
  - [Ramification index of a morphism of curves](#ramification-index-of-a-morphism-of-curves)
  - [Fiber of a morphism](#fiber-of-a-morphism)
    - [Local fibre dimension](#local-fibre-dimension)
      - [Upper semicontinuity of local fibre dimension](#upper-semicontinuity-of-local-fibre-dimension)
    - [Fiber dimension theorem](#fiber-dimension-theorem)
      - [Dimension of image of a morphism](#dimension-of-image-of-a-morphism)
        - [Isolated fibre point forces dominance in equal dimensions](#isolated-fibre-point-forces-dominance-in-equal-dimensions)
      - [Generic equidimensionality of fibres](#generic-equidimensionality-of-fibres)
      - [Closed-fibre lower bound by finite normalization](#closed-fibre-lower-bound-by-finite-normalization)
    - [Scheme-theoretic fiber](#scheme-theoretic-fiber)
      - [Fibre of absolute Frobenius over a rational point of the affine line](#fibre-of-absolute-frobenius-over-a-rational-point-of-the-affine-line)
  - [Isomorphism of algebraic varieties](#isomorphism-of-algebraic-varieties)
  - [Finite morphism](#finite-morphism)
    - [Trace-dual module of a finite curve map](#trace-dual-module-of-a-finite-curve-map)
    - [Finite morphisms are proper](#finite-morphisms-are-proper)
- [Projective space](projective-space.md)
  - [Projective space represents invertible quotients](projective-space.md#projective-space-represents-invertible-quotients)
  - [Morphisms from projective space to smaller projective space are constant](projective-space.md#morphisms-from-projective-space-to-smaller-projective-space-are-constant)
  - [Dual projective space](projective-space.md#dual-projective-space)
    - [Projective dual variety](projective-space.md#projective-dual-variety)
      - [Projective biduality theorem](projective-space.md#projective-biduality-theorem)
  - [Projective coordinates over a local ring](projective-space.md#projective-coordinates-over-a-local-ring)
  - [Quaternionic projective space](projective-space.md#quaternionic-projective-space)
    - [Complex cobordism ring of the quaternionic projective plane](projective-space.md#complex-cobordism-ring-of-the-quaternionic-projective-plane)
    - [Complex inclusion into quaternionic projective space](projective-space.md#complex-inclusion-into-quaternionic-projective-space)
    - [Cohomology ring of quaternionic projective space](projective-space.md#cohomology-ring-of-quaternionic-projective-space)
  - [General linear position](projective-space.md#general-linear-position)
  - [Veronese map](projective-space.md#veronese-map)
  - [Top cohomology of projective space](projective-space.md#top-cohomology-of-projective-space)
  - [Cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space)
    - [Nonnegative hyperplane twist cohomology by restriction](projective-space.md#nonnegative-hyperplane-twist-cohomology-by-restriction)
    - [Infinite negative-twist sum with zero global sections](projective-space.md#infinite-negative-twist-sum-with-zero-global-sections)
    - [Global regular functions on projective space](projective-space.md#global-regular-functions-on-projective-space)
  - [Projective point](projective-space.md#projective-point)
    - [Homogeneous coordinate](projective-space.md#homogeneous-coordinate)
    - [Coordinate point](projective-space.md#coordinate-point)
  - [Projective plane](projective-space.md#projective-plane)
    - [Point-line duality](projective-space.md#point-line-duality)
      - [Dual arrangement of a planar point set](projective-space.md#dual-arrangement-of-a-planar-point-set)
        - [Good edge of a dual line arrangement](projective-space.md#good-edge-of-a-dual-line-arrangement)
          - [Safe edge of a dual line arrangement](projective-space.md#safe-edge-of-a-dual-line-arrangement)
            - [Bounded-radius propagation of edge defects](projective-space.md#bounded-radius-propagation-of-edge-defects)
        - [Euler defect identity for a projective line arrangement](projective-space.md#euler-defect-identity-for-a-projective-line-arrangement)
    - [Fano plane](projective-space.md#fano-plane)
      - [Fano plane duality group](projective-space.md#fano-plane-duality-group)
      - [Fano point-line stabilizer intersection](projective-space.md#fano-point-line-stabilizer-intersection)
  - [Projective linear transformation](projective-space.md#projective-linear-transformation)
  - [Projective variety](projective-space.md#projective-variety)
    - [Veronese surface](projective-space.md#veronese-surface)
    - [Projective embedding](projective-space.md#projective-embedding)
    - [Pole divisor avoiding a fiber](projective-space.md#pole-divisor-avoiding-a-fiber)
    - [Projective completion](projective-space.md#projective-completion)
      - [Homogenization (algebra)](projective-space.md#homogenization-algebra)
    - [Projective dimension theorem](projective-space.md#projective-dimension-theorem)
    - [Projective curve](projective-space.md#projective-curve)
      - [Rational normal curve](projective-space.md#rational-normal-curve)
      - [Smooth projective curve](projective-space.md#smooth-projective-curve)
        - [Two-affine cover of a smooth projective curve](projective-space.md#two-affine-cover-of-a-smooth-projective-curve)
        - [Genus of a smooth projective curve](projective-space.md#genus-of-a-smooth-projective-curve)
          - [Rationality of a smooth projective genus-zero curve](projective-space.md#rationality-of-a-smooth-projective-genus-zero-curve)
        - [Smooth plane cubic in characteristic three](projective-space.md#smooth-plane-cubic-in-characteristic-three)
        - [Smooth rational curve](projective-space.md#smooth-rational-curve)
        - [Local ring of a smooth algebraic curve](projective-space.md#local-ring-of-a-smooth-algebraic-curve)
          - [Local parameter on a smooth algebraic curve](projective-space.md#local-parameter-on-a-smooth-algebraic-curve)
        - [Extension of a rational map from a smooth projective curve](projective-space.md#extension-of-a-rational-map-from-a-smooth-projective-curve)
          - [Failure of rational-map extension on a singular curve](projective-space.md#failure-of-rational-map-extension-on-a-singular-curve)
    - [Homogeneous coordinate ring](projective-space.md#homogeneous-coordinate-ring)
    - [Product of projective varieties](projective-space.md#product-of-projective-varieties)
      - [Coordinate projection](projective-space.md#coordinate-projection)
      - [Segre embedding](projective-space.md#segre-embedding)
      - [Smooth quadric surface](projective-space.md#smooth-quadric-surface)
        - [Projection from a point on a smooth quadric](projective-space.md#projection-from-a-point-on-a-smooth-quadric)
        - [Picard group of a smooth affine quadric surface](projective-space.md#picard-group-of-a-smooth-affine-quadric-surface)
        - [Segre description of a smooth quadric surface](projective-space.md#segre-description-of-a-smooth-quadric-surface)
        - [Rulings of a smooth quadric surface](projective-space.md#rulings-of-a-smooth-quadric-surface)
          - [Disjoint curves on a smooth quadric surface](projective-space.md#disjoint-curves-on-a-smooth-quadric-surface)

## Rational map of algebraic varieties

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

A rational map is a [morphism of algebraic varieties](#morphism-of-algebraic-varieties) defined on a dense [open subset](topology.md#open-set), with representatives identified when they agree on a smaller dense [open subset](topology.md#open-set). For an integral source and a [separated variety](locally-ringed-space.md#separated-variety) as target, agreement on a dense open determines a morphism uniquely. This definition also permits nonprojective sources.

## Ring of rational functions on a reduced variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

For a possibly reducible [algebraic variety](algebraic-variety.md) $X$, take pairs $(U,f)$ with $U$ a dense open subset and $f$ a [regular function](locally-ringed-space.md#regular-function) on $U$. Identify pairs agreeing on a common dense open subset. Addition and multiplication on intersections make these classes a [ring](commutative-algebra.md#ring). For an [affine variety](#affine-algebraic-set) with reduced [coordinate ring](#coordinate-ring) $A$, this ring is its [total quotient ring](commutative-algebra.md#total-ring-of-fractions). For an [irreducible variety](#irreducible-variety), it is the [function field](#function-field-of-an-algebraic-variety). An [isomorphism](algebra.md#isomorphism) of dense open subsets induces an [isomorphism](algebra.md#isomorphism) of these rings.

### Local ring embeds in rational functions on incident components

↑ **Parent:** [Ring of rational functions on a reduced variety](#ring-of-rational-functions-on-a-reduced-variety)

Let $Y$ be the reduced union of the [irreducible components](algebraic-geometry.md#irreducible-component) of an [affine variety](#affine-algebraic-set) $X$ containing $P$. Removing all other components leaves an open neighbourhood of $P$ on which $X$ and $Y$ agree, so their [local rings](commutative-algebra.md#local-ring) at $P$ agree. In the [coordinate ring](#coordinate-ring) $B=k[Y]$, every denominator not vanishing at $P$ avoids all minimal primes: each component of $Y$ contains $P$. Such a denominator is a [non-zero-divisor](mathematics.md#non-zero-divisor). Consequently $B_{\mathfrak m_P}$ injects into the [total quotient ring](commutative-algebra.md#total-ring-of-fractions) $Q(B)=\operatorname{Rat}(Y)$. One cannot generally replace $Y$ by a single component through an intersection point.

## Rational function on an algebraic variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

On an integral algebraic variety, a rational function is an equivalence class of regular functions on nonempty open subsets, with equality on a common dense open subset. These form the function field $k(X)$. On an affine open $\operatorname{Spec}A$, this field is the fraction field of $A$.

// Target: geometry-and-topology.bigb

## Quasi-projective algebraic set

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

A locally closed [affine algebraic set](#affine-algebraic-set) in a [projective space](projective-space.md), equivalently an [open subset](topology.md#open-set) of a closed subset of [projective space](projective-space.md) cut out by homogeneous polynomials. Reducibility is allowed for an algebraic set; an [irreducible variety](#irreducible-variety) with such an embedding is a [quasi-projective variety](#quasi-projective-variety).

### Quasi-projective variety

↑ **Parent:** [Quasi-projective algebraic set](#quasi-projective-algebraic-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-projective_variety)

An [irreducible variety](#irreducible-variety) which admits a locally closed embedding into [projective space](projective-space.md). Open subsets of [affine varieties](#affine-algebraic-set) and [blowups of algebraic varieties](algebraic-geometry.md#blowing-up-algebraic-geometry) along closed centres give important examples.

## Irreducible variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

An [algebraic variety](algebraic-variety.md) whose underlying [topological space](topology.md#topological-space) with its [Zariski topology](algebraic-geometry.md#zariski-topology) is an [irreducible topological space](algebraic-geometry.md#irreducible-topological-space): it is nonempty and cannot be a union of two proper closed subsets. For a reduced affine variety, this is equivalent to its [coordinate ring](#coordinate-ring) being an [integral domain](commutative-algebra.md#integral-domain).

## Constructible subset of a variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

A constructible subset is a finite union of locally closed subsets in the [Zariski topology](algebraic-geometry.md#zariski-topology). A dense constructible subset contains a dense open subset. Constructibility alone is weaker than closedness, but a [constructible subgroup is closed](#constructible-subgroup-is-closed).

### Chevalley constructibility theorem

↑ **Parent:** [Constructible subset of a variety](#constructible-subset-of-a-variety)

The image of a morphism of algebraic varieties is constructible. This replaces the generally false assertion that all morphisms have closed image. Group structure adds the fact that a [constructible subgroup is closed](#constructible-subgroup-is-closed).

## Rational point

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

For an [algebraic variety](algebraic-variety.md) $X$ defined over a [field](algebra.md#field) $K$, a K-[rational point](#rational-point) is a morphism $\operatorname{Spec}K\to X$ over $K$. In affine coordinates it is a solution of the defining equations with every coordinate in $K$; in projective coordinates it is a nonzero coordinate vector over $K$, considered up to common nonzero scaling. The set is denoted $X(K)$. Over a [number field](algebraic-number-theory.md#number-field), having points over every completion need not imply having a [rational point](#rational-point); for genus-one coverings this failure is recorded by the [Tate–Shafarevich group](normalization-of-an-algebraic-curve.md#tate-shafarevich-group).

## Smooth algebraic variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

An algebraic variety is smooth over its ground field when its structural morphism is smooth. Over an algebraically closed field its local rings are regular; on an irreducible variety its tangent spaces all have the variety's [dimension of a scheme](locally-ringed-space.md#dimension-of-a-scheme).

### Smoothness of an algebraic variety

↑ **Parent:** [Smooth algebraic variety](#smooth-algebraic-variety)

Over a [perfect field](algebra.md#perfect-field), a point of an [algebraic variety](algebraic-variety.md) is smooth exactly when its [local ring](commutative-algebra.md#local-ring) is a [regular local ring](commutative-algebra.md#regular-local-ring). The [smooth locus of a variety](algebraic-geometry.md#smooth-locus-of-a-variety) is open; its closed complement is the [singular locus](algebraic-geometry.md#singular-locus).

## Normalization of an algebraic variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

The normalization of an integral [algebraic variety](algebraic-variety.md) is obtained by taking the integral closure of its affine coordinate rings in its [function field](#function-field-of-an-algebraic-variety). Its natural morphism is finite and birational, and its source is normal. For [Cartier divisors](cartier-divisor.md), [bigness under finite normalization](cartier-divisor.md#bigness-under-finite-normalization) compares section growth on the two varieties.

## Closed subvariety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

A closed subvariety is an integral closed subscheme of an [algebraic variety](algebraic-variety.md). It supplies the lower-dimensional loci on which positivity is tested by the [Nakai–Moishezon criterion](cartier-divisor.md#nakai-moishezon-criterion).

## Algebraic curve

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

An algebraic curve is a one-dimensional [algebraic variety](algebraic-variety.md). On a [smooth algebraic curve](#smooth-algebraic-curve), the local ring at every closed point is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), which allows orders of zeros and poles to be recorded as a [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve).

### Cissoid of Diocles

↑ **Parent:** [Algebraic curve](#algebraic-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cissoid_of_Diocles)

For $a>0$, this [algebraic curve](#algebraic-curve) can be constructed using a [circle](topology.md#circle) of [radius](topology.md#radius) $a$ centred at $(a,0)$ and its [tangent line](calculus.md#tangent-line) $x=2a$. On a ray from the origin, subtract the distance to its nonzero circle intersection from the distance to the line. The resulting radial distance is $r=2a\sin^2\theta/\cos\theta$, for $-\pi/2<\theta<\pi/2$. Thus a [parametric curve](topology.md#parametric-curve) for it is

$$
x=\frac{2at^2}{1+t^2},\qquad y=\frac{2at^3}{1+t^2},\qquad t\in\mathbb R.
$$

Eliminating $t$ gives the displayed cubic equation. It has a [cusp](algebraic-geometry.md#cusp-algebraic-geometry) at the origin, horizontal tangent direction there, and vertical [asymptote](topology.md#asymptote) $x=2a$. Its name honours [Diocles](mathematics.md#diocles-mathematician).

### Integral projective curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

An [algebraic curve](#algebraic-curve) which is projective, [reduced](commutative-algebra.md#reduced-ring) and [irreducible](representation-theory.md#irreducible-representation). Over an [algebraically closed field](algebra.md#algebraically-closed-field), its only [global regular functions](locally-ringed-space.md#global-regular-function) are constants and its [arithmetic genus](#arithmetic-genus) is $h^1(\mathcal O_C)\ge0$.

### Nonsingular point of an algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

For an affine plane [algebraic curve](#algebraic-curve) $F(x,y)=0$, a point over an [algebraic closure](algebra.md#algebraic-closure) is nonsingular when the displayed condition holds. Its [Zariski tangent space](algebraic-geometry.md#zariski-tangent-space) has dimension one, and a local coordinate can be chosen in the direction of a nonzero [partial derivative](multivariable-calculus.md#partial-derivative). A [smooth algebraic curve](#smooth-algebraic-curve) has all points nonsingular. Over a complete [local field](non-archimedean-analysis.md#local-field), the [Hensel lemma](non-archimedean-analysis.md#hensel-s-lemma) lifts a nonsingular residue point by solving for a coordinate with unit [partial derivative](multivariable-calculus.md#partial-derivative).

### Affine algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

An affine algebraic curve is an [affine variety](#affine-algebraic-set) of [Krull dimension](commutative-algebra.md#krull-dimension) one. An irreducible affine curve has a finitely generated one-dimensional domain as its [coordinate ring](#coordinate-ring). Quotienting this ring by a nonzero element gives a zero-dimensional [Noetherian ring](algebra.md#noetherian-ring), hence an [Artinian ring](algebra.md#artinian-ring). Consequently a nonzero regular function has finitely many zeros. No nonsingularity assumption is part of the definition.

#### Folium of Descartes

↑ **Parent:** [Affine algebraic curve](#affine-algebraic-curve)

For nonzero real $a$, the [folium of Descartes](#folium-of-descartes) is the [algebraic curve](#algebraic-curve) $x^3+y^3=3axy$, with [rational parametrization of an algebraic curve](#rational-parametrization-of-an-algebraic-curve)

$$
x=\frac{3at}{1+t^3},\qquad y=\frac{3at^2}{1+t^3},\qquad t\ne-1.
$$

It is symmetric about $y=x$ and has a node at the origin, with the coordinate axes as tangents. For $a>0$, $0\leq t<\infty$ traces a loop in the first quadrant, returning to the origin as $t\to\infty$. Its enclosed [area](differential-geometry.md#surface-area), by [Green's theorem](multivariable-calculus.md#green-theorem), is

$$
\frac12\int_0^\infty(xy'-yx')\,dt
=\frac{9a^2}{2}\int_0^\infty\frac{t^2\,dt}{(1+t^3)^2}=\frac{3a^2}{2}.
$$

The other branches approach the [asymptote](topology.md#asymptote) $x+y+a=0$ as $t\to-1$. Negative $a$ rotates the positive-$a$ picture through $\pi$.

### Cuspidal cubic

↑ **Parent:** [Algebraic curve](#algebraic-curve)

The projective [algebraic curve](#algebraic-curve) $D=\{y^2z=x^3\}\subset\mathbb P^2$ is an irreducible cubic with a [cusp](algebraic-geometry.md#cusp-algebraic-geometry) at $[0:0:1]$. In the chart $z=1$, its equation is $y^2=x^3$, with parametrization $(x,y)=(t^2,t^3)$. Its affine version $y^2=z^3$, used below, differs only by renaming a coordinate. At the point $[0:1:0]$, the chart $y=1$ gives $z=x^3$, which is smooth and exhibits its [unique smooth flex of a cuspidal cubic](#unique-smooth-flex-of-a-cuspidal-cubic).

#### Unique smooth flex of a cuspidal cubic

↑ **Parent:** [Cuspidal cubic](#cuspidal-cubic)

For $D=\{y^2z=x^3\}$, the determinant of the homogeneous [Hessian matrix](multivariable-calculus.md#hessian-matrix) is $24xy^2$. Its intersections with $D$ are the cusp $[0:0:1]$ and the smooth point $[0:1:0]$. The [Hessian criterion for a flex](algebraic-geometry.md#hessian-criterion-for-a-flex) therefore gives a unique smooth [flex](algebraic-geometry.md#inflection-point-of-an-algebraic-plane-curve), with tangent $z=0$ and contact order three. Consequently every pair consisting of a triple line and a cuspidal cubic meeting only at a smooth point is projectively equivalent to $(3\{z=0\},D)$.

#### Cusp with two isolated-point components

↑ **Parent:** [Cuspidal cubic](#cuspidal-cubic)

The algebraic set in $\mathbb A^3$ defined by

$$
xy=0,
\qquad y^2-z^3+xz=0,
\qquad x(x+y+2z+1)=0
$$

is the disjoint union of the cuspidal cubic $V(x,y^2-z^3)$ and the two reduced points $(-1,0,0)$ and $(1,0,-1)$. Its radical vanishing ideal is the intersection of the three corresponding prime ideals.

### Symmetric product of a curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

The [scheme](locally-ringed-space.md#scheme) $C^{(d)}$ parametrizes effective degree-$d$ [Cartier divisors](cartier-divisor.md) on a smooth [algebraic curve](#algebraic-curve). Near a [Cartier divisor](cartier-divisor.md) $\sum m_iP_i$, its completed local ring is a power-series ring in the elementary symmetric coordinates of $m_i$ local parameters at each $P_i$. It is therefore smooth of dimension $d$, even when the [characteristic of a field](algebra.md#characteristic-of-a-field) divides $d!$. For projective $C$ it is projective.

### Monomial curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

Over a [field](algebra.md#field) $k$, an affine curve parametrized by positive integer powers of one parameter. Its coordinate [ring](commutative-algebra.md#ring) is the subalgebra generated by those powers, and its defining [prime ideal](commutative-algebra.md#prime-ideal) is the kernel of $k[x_1,\ldots,x_n]\to k[t]$ sending $x_i$ to $t^{a_i}$. Equal exponent sums yield binomial relations. Studying those relations connects an additive semigroup of exponents to the geometry of the curve.

#### Monomial curve with exponents three, four and five

↑ **Parent:** [Monomial curve](#monomial-curve)

The kernel of $x\mapsto t^3$, $y\mapsto t^4$, $z\mapsto t^5$ is generated by $y^2-xz$, $yz-x^3$, $z^2-x^2y$. Reducing these three relations leaves a unique normal form $A_0(x)+A_1(x)y+A_2(x)z$: its images have distinct exponents modulo three. The curve [ring](commutative-algebra.md#ring) is therefore finite free of rank three over $k[x]$ and has dimension one. In a three-variable [polynomial ring](commutative-algebra.md#polynomial-ring) its [ideal](commutative-algebra.md#ideal) has height two, but its three independent quadratic initial forms force at least three generators. This is a concrete failure of generation by codimension many equations.

### Rational parametrization of an algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

A rational parametrization expresses the coordinates of an [algebraic curve](#algebraic-curve) as [rational functions](isolated-singularity.md#rational-function) of a parameter, with a rational inverse on a dense open subset. It identifies the [function field](#function-field-of-an-algebraic-variety) with $K(t)$ and the smooth projective [normalization of an algebraic curve](normalization-of-an-algebraic-curve.md) with the [projective line](finite-group-theory.md#projective-line). A nonconstant parametrizing map without an inverse is a weaker notion; even this cannot exist for an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) in characteristic zero.

### Arithmetic genus

↑ **Parent:** [Algebraic curve](#algebraic-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arithmetic_genus)

The [arithmetic genus](#arithmetic-genus) of a proper curve $C$ is $p_a(C)=1-\chi(C,\mathcal O_C)$. For an integral projective curve over an algebraically closed field, $H^0(C,\mathcal O_C)=k$, so $p_a=h^1\ge0$. Its finite normalization has $p_a(C)=g(C^\nu)+\operatorname{length}(\nu_*\mathcal O_{C^\nu}/\mathcal O_C)$. Hence [arithmetic genus](#arithmetic-genus) zero forces the curve to be smooth and rational.

#### Genus of a complete-intersection space curve

↑ **Parent:** [Arithmetic genus](#arithmetic-genus)

For a [projective complete intersection](locally-ringed-space.md#projective-complete-intersection) curve cut out by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of positive degrees $a,b$ in $\mathbb P^3_k$, the [Koszul resolution](homological-algebra.md#koszul-resolution) gives [Hilbert polynomial](algebraic-geometry.md#hilbert-polynomial) $ab\,m+ab(4-a-b)/2$. Hence its [arithmetic genus](#arithmetic-genus) is $1+ab(a+b-4)/2$. The same resolution shows $H^0(C,\mathcal O_C)=k$, and the [dimension of a scheme](locally-ringed-space.md#dimension-of-a-scheme) is one, so this genus equals $\dim_kH^1(C,\mathcal O_C)$. Smoothness and irreducibility of the curve are not required. For degrees five and seven, the value is $141$.

## Prevariety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

In the classical convention over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$, a prevariety is an [irreducible topological space](algebraic-geometry.md#irreducible-topological-space) with a [sheaf of rings](ringed-space.md#sheaf-of-rings) which has a finite [open cover](topology.md#open-cover) by [affine varieties](#affine-algebraic-set), with compatible local identifications. A prevariety need not be separated. A classical [algebraic variety](algebraic-variety.md) is a separated prevariety: its [diagonal morphism](locally-ringed-space.md#diagonal-morphism) has closed image. Some authors allow reducible prevarieties and varieties; the separation criterion and product construction remain the same under that convention.

## Algebraic group

↑ **Parent:** [Algebraic variety](algebraic-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_group)

A group variety is an [algebraic variety](algebraic-variety.md) whose multiplication and inversion are morphisms.

### Isogeny

↑ **Parent:** [Algebraic group](#algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isogeny)

An isogeny is a surjective [morphism](algebra.md#morphism) of [algebraic groups](#algebraic-group) with finite kernel. For [abelian varieties](abelian-variety.md) it is a finite surjective group morphism. An [isogeny of elliptic curves](normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) is its one-dimensional abelian-variety specialization.

### Multiplicative group scheme

↑ **Parent:** [Algebraic group](#algebraic-group)

The multiplicative group [scheme](locally-ringed-space.md#scheme) represents [units](algebra.md#unit-in-a-ring): its $R$-points are $R^\times$. Multiplication is specified by $t\mapsto t\otimes t$ on the coordinate [ring](commutative-algebra.md#ring). It is the [principal open subset](locally-ringed-space.md#principal-open-subscheme) $D(t)$ of the [affine line](locally-ringed-space.md#affine-line) and the one-dimensional split [algebraic torus](toric-geometry.md#algebraic-torus).

// Target: ringed-space.bigb

### Multiplicative algebraic group

↑ **Parent:** [Algebraic group](#algebraic-group)

The multiplicative [algebraic group](#algebraic-group) has $\mathbb G_m(K)=K^{\times}$, with multiplication as its [group operation](group.md#group-operation). Its coordinate ring is $K[z,z^{-1}]$. The [formal multiplicative group](normalization-of-an-algebraic-curve.md#formal-multiplicative-group) describes its law near the identity $z=1$.

### Algebraic group action

↑ **Parent:** [Algebraic group](#algebraic-group)

This is a group action whose action map $G\times V\to V$ is a morphism of varieties. Orbits are locally closed: constructibility gives a relatively open piece, and its translates cover the orbit. An orbit of an irreducible group is irreducible and open in its closure. These facts control degenerations of [quiver representations](algebra.md#representation-of-a-quiver).

### Dimension formula for an algebraic group homomorphism

↑ **Parent:** [Algebraic group](#algebraic-group)

The kernel is a closed identity fiber. The image is closed because a [constructible subgroup is closed](#constructible-subgroup-is-closed). Every nonempty fiber is a kernel translate, so the [fiber dimension theorem](#fiber-dimension-theorem) gives $\dim G=\dim\ker\varphi+\dim\operatorname{im}\varphi$, even for inseparable morphisms.

### Constructible subgroup is closed

↑ **Parent:** [Algebraic group](#algebraic-group)

Let $S$ be constructible in an [algebraic group](#algebraic-group), and $C=\overline S$. The closure is a subgroup. Choose a dense open $U\subseteq C$ contained in $S$. For every $c\in C$, the dense opens $U,cU$ intersect, giving $u=cv$ for $u,v\in S$. Hence $c=uv^{-1}\in S$ and $S=C$. The [Chevalley constructibility theorem](#chevalley-constructibility-theorem) therefore proves closedness of homomorphism images.

### Homomorphism of group varieties

↑ **Parent:** [Algebraic group](#algebraic-group)

A homomorphism of group varieties is a morphism of algebraic varieties that also preserves multiplication. It automatically preserves the identity and inversion.

### Abelian variety

↑ **Parent:** [Algebraic group](#algebraic-group)

[This section is present in another page, follow this link to view it.](abelian-variety.md)

## Smooth algebraic curve

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

A smooth algebraic curve is a one-dimensional [algebraic variety](algebraic-variety.md) whose [local ring](commutative-algebra.md#local-ring) at every point is regular.

This is the nonsingular subclass of [algebraic curves](#algebraic-curve).

### Product dimension bound for sections on a curve

↑ **Parent:** [Smooth algebraic curve](#smooth-algebraic-curve)

For nonzero finite-dimensional spaces $V,W$ of sections of two [line bundles](sheaf-of-modules.md#line-bundle) on a smooth integral curve over an algebraically closed field, their product span in sections of the tensor product satisfies this bound. At one point choose bases with strictly increasing orders of vanishing. Multiplying every first-space basis vector by the first second-space vector, and then the last first-space vector by the remaining second-space vectors, produces distinct increasing orders and hence independent sections. This proves the dimension inequality needed for the [Clifford inequality for curves](algebraic-geometry.md#clifford-inequality-for-curves).

## Affine algebraic set

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

An affine algebraic set is the common zero set $V(I)$ of an [ideal](commutative-algebra.md#ideal) in a polynomial ring over a field.

### Affineness from a unit-ideal principal affine cover

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

A classical [variety](algebraic-variety.md) is affine if finitely many global [regular functions](locally-ringed-space.md#regular-function) generate the [unit ideal](commutative-algebra.md#unit-ideal) and their nonvanishing opens are affine. [Localization of global sections on a principal open](sheaf-of-modules.md#localization-of-global-sections-on-a-principal-open) identifies their [coordinate rings](#coordinate-ring) with $A_{f_i}$, where $A=\Gamma(X,\mathcal O_X)$. Choose a finite-type subalgebra of $A$ containing the functions, their unit-ideal coefficients and numerators of generators of every $A_{f_i}$. Its affine variety has the same principal affine charts, whose [isomorphisms](algebra.md#isomorphism) glue globally. This avoids assuming finite generation of $A$ before affineness is known.

### Morphism of affine varieties

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

A map between [affine varieties](#affine-algebraic-set) is a morphism when its coordinate functions are restrictions of ambient [polynomials](polynomial.md). Pullback identifies these morphisms contravariantly with homomorphisms of their [coordinate rings](#coordinate-ring).

### Coordinate ring of a product of affine varieties

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

For [affine varieties](#affine-algebraic-set) $X,Y$ over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$, their [product in a category](category.md#product-category-theory) is affine, with [coordinate ring](#coordinate-ring) $A\otimes_k B$, where $A=k[X]$ and $B=k[Y]$. Presenting $A=k[x]/J$ and $B=k[y]/L$ identifies this ring with $k[x,y]/(J,L)$. If both varieties are irreducible, this is an [integral domain](commutative-algebra.md#integral-domain): express a nonzero tensor $F$ using linearly independent second factors. The points $x$ where its specialization $F_x$ is nonzero form a nonempty open subset of $X$. For two nonzero tensors $F,G$, choose $x$ in the intersection of these open subsets; then $F_xG_x\ne0$ in the domain $B$. The [Hilbert Nullstellensatz](algebraic-geometry.md#hilbert-nullstellensatz) identifies $(J,L)$ with the defining ideal of $X\times Y$. The universal property follows from the universal property of the [tensor product of modules](module-theory.md#tensor-product-of-modules) as a tensor product of commutative algebras.

### Vanishing ideal

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

The vanishing ideal of $X\subseteq k^n$ is

$$
I(X)=\{f\in k[x_1,\ldots,x_n]:f(x)=0\text{ for every }x\in X\}.
$$

### Coordinate ring

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coordinate_ring)

For an affine algebraic set $X\subseteq\mathbb A_k^n$, its coordinate ring is

$$
k[X]=k[x_1,\ldots,x_n]/I(X).
$$

The set $X$ is irreducible exactly when $k[X]$ is an [integral domain](commutative-algebra.md#integral-domain).

#### Irreducibility and prime vanishing ideal

↑ **Parent:** [Coordinate ring](#coordinate-ring)

For an affine algebraic set $X$ over an algebraically closed field,

$$
X\text{ is irreducible}
\quad\Longleftrightarrow\quad
I(X)\text{ is a prime ideal}.
$$

If $fg$ vanishes on $X$, then $X$ is the union of its intersections with $V(f)$ and $V(g)$. Conversely, a nontrivial decomposition into closed subsets supplies functions vanishing on each proper piece whose product vanishes on all of $X$.

#### Dominant morphism of affine varieties

↑ **Parent:** [Coordinate ring](#coordinate-ring)

A morphism $f:X\to Y$ of affine varieties is dominant when its image is [Zariski dense](algebraic-geometry.md#zariski-dense-subset) in $Y$. It is dominant exactly when the pullback homomorphism

$$
f^*:k[Y]\to k[X]
$$

is injective. When $X$ and $Y$ are irreducible, this injection extends to their function fields and gives $\dim X\geq\dim Y$.

This is the dense-image case of a [morphism of algebraic varieties](#morphism-of-algebraic-varieties).

### Vanishing loci of ideal sums and intersections

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

For ideals $I,J\subseteq k[x_1,\ldots,x_n]$,

$$
V(I+J)=V(I)\cap V(J),
\qquad
V(I\cap J)=V(I)\cup V(J).
$$

The second equality also follows from $V(IJ)=V(I)\cup V(J)$ and

$$
IJ\subseteq I\cap J.
$$

### Irreducible components of two intersecting complex hyperbolas

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

The algebraic set

$$
V(x^2+y^2-1,x^2-z^2-1)\subseteq\mathbb A_{\mathbb C}^3
$$

has the two irreducible components

$$
V(y-iz,x^2-z^2-1)
\quad\text{and}\quad
V(y+iz,x^2-z^2-1).
$$

Each is irreducible because the linear change $u=x-z$, $v=x+z$ identifies its [coordinate ring](#coordinate-ring) with

$$
\mathbb C[u,v]/(uv-1)\cong\mathbb C[u,u^{-1}],
$$

an [integral domain](commutative-algebra.md#integral-domain).

## Function field of an algebraic variety

↑ **Parent:** [Algebraic variety](algebraic-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_field_of_an_algebraic_variety)

The function field $k(X)$ of an irreducible [algebraic variety](algebraic-variety.md) consists of its [rational functions](isolated-singularity.md#rational-function).

### Sheaf of nonzero rational functions on an irreducible variety

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

For an irreducible [algebraic variety](algebraic-variety.md) $X$ with [function field](#function-field-of-an-algebraic-variety) $K$, this [sheaf of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups) assigns $K^*$ to every nonempty open set, with identity restriction maps, and assigns the trivial group to the empty set. Irreducibility ensures that any two nonempty open subsets meet, so these sections satisfy the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom). It is a [flasque sheaf](sheaf-of-modules.md#flasque-sheaf) and has zero higher [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology).

### Dimension from the function field

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

For an irreducible variety $X$ over a field $k$,

$$
\dim X=\operatorname{trdeg}_k k(X).
$$

Consequently birational irreducible varieties have the same dimension.

### Projective model of a finitely generated field

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

If $K/k$ is a finitely generated field extension, write $K=\operatorname{Frac}(A)$ for a finitely generated integral $k$-algebra $A$. The projective closure of the affine variety $\operatorname{Spec}A$ is an irreducible projective variety with function field $K$.

## Morphism of algebraic varieties

↑ **Parent:** [Algebraic variety](algebraic-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_algebraic_varieties)

A morphism of algebraic varieties is a map given locally by regular functions. A projective-coordinate formula defines a morphism wherever its homogeneous coordinate functions do not vanish simultaneously.

### Morphism of algebraic curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A [morphism of algebraic varieties](#morphism-of-algebraic-varieties) whose source and target are [algebraic curves](#algebraic-curve). A nonconstant morphism between [smooth projective curves](projective-space.md#smooth-projective-curve) is finite and surjective; its degree is the degree of the induced extension of [function fields](#function-field-of-an-algebraic-variety).

### Conic bundle

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conic_bundle)

A flat proper [morphism of algebraic varieties](#morphism-of-algebraic-varieties) whose geometric fibres are [plane conics](algebraic-geometry.md#plane-conic), usually presented as a quadratic equation in a [projective bundle](vector-bundle.md#projective-bundle) of relative dimension two. The generic fibre is normally required to be smooth; singular conics can occur in special fibres. A [conic bundle from a line on a smooth cubic surface](algebraic-geometry.md#conic-bundle-from-a-line-on-a-smooth-cubic-surface) has five reducible fibres over the [projective line](finite-group-theory.md#projective-line).

#### Conic discriminant

↑ **Parent:** [Conic bundle](#conic-bundle)

In characteristic different from two, a local equation for a [conic bundle](#conic-bundle) is $z^{\mathsf T}Mz=0$ with $M$ symmetric. A fibre is singular exactly when the [determinant](multilinear-algebra.md#determinant) vanishes. Changing the fibre coordinates multiplies that determinant by a nonzero square, so its zero locus is intrinsically defined even when the quadratic coefficients belong to twisting [line bundles](sheaf-of-modules.md#line-bundle).

##### Reduced singular fibres of a smooth conic bundle

↑ **Parent:** [Conic discriminant](#conic-discriminant)

Let the base be a [smooth algebraic curve](#smooth-algebraic-curve), the total surface be smooth, and the [field](algebra.md#field) be algebraically closed of characteristic different from two. At a rank-two singular fibre with kernel vector $v$, the fibre derivatives vanish at $[v]$. Smoothness requires $v^{\mathsf T}M'v\ne0$. The [adjugate matrix](linear-algebra.md#adjugate-matrix) is a nonzero multiple of $vv^{\mathsf T}$, so the determinant has a simple zero. At rank at most one, the projective kernel contains a line and the quadratic $v^{\mathsf T}M'v$ has a zero on it; that point would make the total surface singular. Thus every singular fibre is a pair of distinct [projective lines](finite-group-theory.md#projective-line) and its discriminant zero is simple.

### Generically finite morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A dominant [morphism of varieties](#morphism-of-algebraic-varieties) is generically finite when its extension of [function fields](#function-field-of-an-algebraic-variety) is finite. Its degree is the degree of this field extension. A dominant morphism between integral varieties of equal dimension is generically finite; over a suitable nonempty open subset of the target its fibers are finite.

### Isomorphic local rings determine isomorphic neighborhoods

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A $k$-algebra isomorphism between the local rings at closed points extends to a morphism on some neighborhoods: represent the images of finitely many affine coordinate generators by fractions, and shrink where their denominators are nonzero and their finitely many relations hold. Extend its inverse the same way. The two compositions agree with the identity as germs; finitely many coordinate equalities make them identities after shrinking again. Taking inverse images of these neighborhoods then gives mutually inverse actual neighborhood isomorphisms, not just a formal-completion isomorphism.

### Degree of a morphism of curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A nonconstant [morphism of algebraic varieties](#morphism-of-algebraic-varieties) $f:C\to D$ between smooth projective integral curves is finite, and its degree is the degree of the induced extension of [function fields](#function-field-of-an-algebraic-variety). It is also the degree of the pullback of a rational point, with ramification multiplicities and residue degrees included: locally the finite coordinate algebra is a torsion-free module over the target [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), hence free of its generic rank. For $D=\mathbb P^1$ and a [rational function](isolated-singularity.md#rational-function) defining $f$, the pullback of infinity is its pole [divisor](divisibility.md#divisor), so the total pole degree equals $\deg f$. A degree-one finite map to a normal curve is an isomorphism, since a finite integral algebra inside its unchanged function field equals the integrally closed target ring.

### Algebraic quotient by a finite group

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For an [affine variety](#affine-algebraic-set) with [coordinate ring](#coordinate-ring) $A$ acted on by a [finite group](group.md#finite-group) $G$, the affine quotient is $\operatorname{Spec}A^G$. Elements of $A$ satisfy monic orbit polynomials over $A^G$, so the quotient map is a [finite morphism](#finite-morphism). Over an [algebraically closed field](algebra.md#algebraically-closed-field), invariant functions separate finite orbits; in characteristic not dividing $|G|$, interpolate and average a function separating two orbits. The quotient fibres are consequently the orbits.

### Affine-target adjunction for varieties

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a classical [algebraic variety](algebraic-variety.md) $X$ and [affine variety](#affine-algebraic-set) $Y$, a homomorphism on the indicated rings gives a morphism by evaluating the images of affine coordinate generators at each point of $X$. The relations defining $Y$ remain zero. Local fractions pull back to local regular fractions, proving regularity; the [coordinate ring](#coordinate-ring) generators also prove uniqueness.

### Ramification index of a morphism of curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a nonconstant morphism between nonsingular curves and a local target [uniformizer](commutative-algebra.md#uniformizer) $t$ at the image of $P$, the index is the [order of vanishing](isolated-singularity.md#order-of-vanishing) of its pullback. Changing $t$ multiplies it by a local [unit in a ring](algebra.md#unit-in-a-ring) and does not change that order. This is a [valuation](algebra.md#valuation) definition and remains meaningful for inseparable morphisms.

### Fiber of a morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a [morphism of algebraic varieties](#morphism-of-algebraic-varieties) $f:X\to Y$ and $y\in Y$, the fiber is the inverse-image variety $X_y=f^{-1}(y)$.

For a point $y$, the underlying [fiber](function.md#fiber-of-a-function) is the inverse image $f^{-1}(y)$.

#### Local fibre dimension

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

The dimension of the [fibre of a morphism](#fiber-of-a-morphism) locally at its source point $x$: the maximum of the dimensions of the fibre's irreducible components through $x$. This differs from the [Krull dimension](commutative-algebra.md#krull-dimension) of the local ring at a nonclosed point.

##### Upper semicontinuity of local fibre dimension

↑ **Parent:** [Local fibre dimension](#local-fibre-dimension)

For a finite-type [morphism of schemes](locally-ringed-space.md#morphism-of-schemes), local fibre dimension is upper semicontinuous on the source, in the displayed sense. If the morphism is proper, the maximal fibre dimension is also upper semicontinuous on the target. Without properness a component of a large fibre can disappear from the source over a special point, so the target statement is not valid in that generality. [The Stacks Project: dimension of fibres](https://stacks.math.columbia.edu/tag/0B2H) distinguishes these statements.

#### Fiber dimension theorem

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

For a dominant morphism of irreducible varieties, generic fiber dimension is source dimension minus target dimension, and this dimension occurs over a nonempty open subset. In particular, constant fiber dimension $d$ gives source dimension equal to target dimension plus $d$. For algebraic groups the equal-dimensional components and coset fibers allow the same dimension formula componentwise.

##### Dimension of image of a morphism

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For an irreducible source, regard the [morphism of algebraic varieties](#morphism-of-algebraic-varieties) as dominant onto the closure of its image, with generic point $\eta$. The [fiber dimension theorem](#fiber-dimension-theorem) gives the displayed formula. A [proper morphism](locally-ringed-space.md#proper-morphism) has closed image, so the closure can then be omitted.

###### Isolated fibre point forces dominance in equal dimensions

↑ **Parent:** [Dimension of image of a morphism](#dimension-of-image-of-a-morphism)

Let $f:X\to Y$ be a [proper morphism](locally-ringed-space.md#proper-morphism) of irreducible [algebraic varieties](algebraic-variety.md) with equal dimension. If some fibre has an isolated point, its corresponding irreducible component has dimension zero. Apply the [fiber dimension theorem](#fiber-dimension-theorem) to $X\to f(X)$: $0\ge\dim X-\dim f(X)$. Thus the closed image has dimension $\dim Y$ and equals $Y$. The [incidence proof that a cubic surface contains a line](algebraic-geometry.md#incidence-proof-that-a-cubic-surface-contains-a-line) is an application; the entire witness fibre need not be finite.

##### Generic equidimensionality of fibres

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For a dominant [morphism of algebraic varieties](#morphism-of-algebraic-varieties) between irreducible varieties, there is a nonempty [Zariski-open subset](algebraic-geometry.md#zariski-open-set) of the target over which every fibre is nonempty and every irreducible component has the displayed dimension. Apply [Noether normalization](algebraic-geometry.md#noether-normalization) to affine source charts over the target [function field](#function-field-of-an-algebraic-variety) and clear denominators on the target to get a generic upper bound. Combine it with the closed-fibre lower bound in the [fiber dimension theorem](#fiber-dimension-theorem).

##### Closed-fibre lower bound by finite normalization

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For a surjective morphism of irreducible varieties, choose an affine neighborhood of the target point and a finite [Noether normalization](algebraic-geometry.md#noether-normalization) to affine space of target dimension $r$. On an affine source neighborhood the composite fibre is cut out by $r$ functions, so repeated [principal hypersurface dimension lemma](algebraic-geometry.md#principal-hypersurface-dimension-lemma) gives dimension at least source dimension minus $r$ on every component. The normalization fibre is finite. The original fibre is therefore an open-and-closed union of components of that composite fibre, proving the bound without assuming target smoothness. For a reducible source the bound must instead be applied using the dimension of each source component.

#### Scheme-theoretic fiber

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

For a morphism of schemes $f:X\to Y$ and a point $y\in Y$, the scheme-theoretic fiber is the fiber product $X\times_Y\operatorname{Spec}\kappa(y)$. It remembers multiplicities and nilpotents that the underlying set-theoretic inverse image cannot detect.

Its underlying [fiber](function.md#fiber-of-a-function) is enriched with local-ring and multiplicity information.

##### Fibre of absolute Frobenius over a rational point of the affine line

↑ **Parent:** [Scheme-theoretic fiber](#scheme-theoretic-fiber)

Over a [perfect field](algebra.md#perfect-field) $k$ of characteristic $p$, the [scheme-theoretic fiber](#scheme-theoretic-fiber) of the [Absolute Frobenius morphism](locally-ringed-space.md#absolute-frobenius-morphism) of $\mathbb A_k^1$ over a rational point $a$ is

$$
\operatorname{Spec}\bigl(k[t]\otimes_{k[t],\,t\mapsto t^p}k\bigr)
\cong\operatorname{Spec}k[t]/(t-a)^p.
$$

Its underlying space is one point, but its coordinate ring has a nonzero [nilpotent element](commutative-algebra.md#nilpotent), so the fibre is a length-$p$ [nonreduced scheme](locally-ringed-space.md#nonreduced-scheme).

### Isomorphism of algebraic varieties

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

An isomorphism of algebraic varieties is a [morphism](#morphism-of-algebraic-varieties) with a morphic inverse. It preserves all properties intrinsic to the variety.

### Finite morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_morphism)

A finite morphism is a morphism whose inverse image of every affine open set is affine and whose corresponding coordinate ring is finite as a module over the base coordinate ring. A nonconstant morphism between smooth projective curves is finite, and its degree is the number of points in a generic fiber counted with multiplicity.

#### Trace-dual module of a finite curve map

↑ **Parent:** [Finite morphism](#finite-morphism)

For a finite generically separable morphism between [smooth projective curves](projective-space.md#smooth-projective-curve), the [field trace](algebraic-number-theory.md#field-trace) on [rational differentials](algebraic-geometry.md#rational-differential-on-an-algebraic-curve) identifies the differential sheaf with the trace-dual module. Locally, for $A=k[[s]]\subset B=k[[u]]$ with $s=f(u)$, the trace-dual fractional ideal is $f'(u)^{-1}B$. Multiplying it by $ds=f'(u)du$ gives $Bdu$. For a monogenic finite extension with monic polynomial $P$, the identity $\operatorname{Tr}(g(u)/P'(u))=[T^{e-1}](g(T)\bmod P(T))$ proves the dual-module formula: the top-coefficient pairing on the basis $1,u,\ldots,u^{e-1}$ has invertible antitriangular matrix. Tensoring locally with an [invertible sheaf](sheaf-of-modules.md#line-bundle) yields $\pi_*(\mathcal M^\vee\otimes\Omega^1_C)\cong\mathcal H om(\pi_*\mathcal M,\Omega^1_D)$.

#### Finite morphisms are proper

↑ **Parent:** [Finite morphism](#finite-morphism)

A finite morphism is of finite type and separated: on affine charts the multiplication map $B\otimes_AB\to B$ is surjective and represents its closed diagonal. Each element of a finite algebra satisfies a monic equation by the determinant trick. In a valuative lifting problem, its image in the fraction field is therefore integral over the valuation ring and belongs to that ring, since valuation rings are integrally closed. This gives a lift, unique because the valuation ring embeds in its fraction field. The [valuative criterion for properness](locally-ringed-space.md#valuative-criterion-for-properness) proves properness.

## Projective space

↑ **Parent:** [Algebraic variety](algebraic-variety.md)

[This section is present in another page, follow this link to view it.](projective-space.md)

## ↑ Ancestors (5)

1. [Algebraic geometry](algebraic-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (42)

- [Affine chart of a variety](locally-ringed-space.md#affine-chart-of-a-variety)
- [Affine-target adjunction for varieties](#affine-target-adjunction-for-varieties)
- [Algebraic cotangent bundle](locally-ringed-space.md#algebraic-cotangent-bundle)
- [Algebraic curve](#algebraic-curve)
- [Algebraic group](#algebraic-group)
- [Algebraic set](algebraic-geometry.md#algebraic-set)
- [Algebraic surface](algebraic-geometry.md#algebraic-surface)
- [Chern class axioms in the Chow ring](algebraic-geometry.md#chern-class-axioms-in-the-chow-ring)
- [Closed subvariety](#closed-subvariety)
- [Cycle class map](algebraic-geometry.md#cycle-class-map)
- [Degree of an algebraic variety](algebraic-geometry.md#degree-of-an-algebraic-variety)
- [Dimension of a topological space by irreducible chains](algebraic-geometry.md#dimension-of-a-topological-space-by-irreducible-chains)
- [Equidimensional algebraic variety](algebraic-geometry.md#equidimensional-algebraic-variety)
- [Étale cohomology](algebraic-geometry.md#etale-cohomology)
- [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)
- [Hasse–Weil zeta function](analytic-number-theory.md#hasse-weil-zeta-function)
- [Intersection dimension bound on a smooth variety](algebraic-geometry.md#intersection-dimension-bound-on-a-smooth-variety)
- [Irreducible variety](#irreducible-variety)
- [Isolated fibre point forces dominance in equal dimensions](#isolated-fibre-point-forces-dominance-in-equal-dimensions)
- [Normal surface singularity](locally-ringed-space.md#normal-surface-singularity)
- [Normal variety](locally-ringed-space.md#normal-variety)
- [Normalization of an algebraic variety](#normalization-of-an-algebraic-variety)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-15.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-21.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-3.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#22i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-113.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#25h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#24g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#24g/solution)
- [Prevariety](#prevariety)
- [Projective bundle](vector-bundle.md#projective-bundle)
- [Rational point](#rational-point)
- [Ring of rational functions on a reduced variety](#ring-of-rational-functions-on-a-reduced-variety)
- [Separated variety](locally-ringed-space.md#separated-variety)
- [Sheaf of nonzero rational functions on an irreducible variety](#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety)
- [Singular locus](algebraic-geometry.md#singular-locus)
- [Smooth algebraic curve](#smooth-algebraic-curve)
- [Smoothness of an algebraic variety](#smoothness-of-an-algebraic-variety)
