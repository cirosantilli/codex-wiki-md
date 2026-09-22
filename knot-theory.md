# Knot theory

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_theory)

Knot theory studies embeddings of circles in three-dimensional manifolds and their higher-dimensional analogues.

**Table of contents**

- [Knot invariant](#knot-invariant)
- [Knot](#knot)
  - [Oriented knot](#oriented-knot)
  - [Unknot](#unknot)
  - [Connected sum of knots](#connected-sum-of-knots)
    - [Prime decomposition of knots](#prime-decomposition-of-knots)
    - [Composite knot](#composite-knot)
    - [Prime knot](#prime-knot)
    - [Splitting sphere of a knot](#splitting-sphere-of-a-knot)
      - [Decomposing sphere system for a knot](#decomposing-sphere-system-for-a-knot)
        - [Prime-ball exchange lemma](#prime-ball-exchange-lemma)
  - [Torus knot](#torus-knot)
    - [Torus knots are prime](#torus-knots-are-prime)
    - [Trefoil knot](#trefoil-knot)
  - [Satellite knot](#satellite-knot)
    - [Pattern of a satellite knot](#pattern-of-a-satellite-knot)
      - [Winding number of a satellite pattern](#winding-number-of-a-satellite-pattern)
    - [Cable knot](#cable-knot)
    - [Satellite formula for the Levine-Tristram signature](#satellite-formula-for-the-levine-tristram-signature)
    - [Satellite formula for the Alexander polynomial](#satellite-formula-for-the-alexander-polynomial)
    - [Whitehead double](#whitehead-double)
  - [Seifert surface](#seifert-surface)
    - [Hopf band](#hopf-band)
    - [Seifert hypersurface](#seifert-hypersurface)
    - [Seifert algorithm](#seifert-algorithm)
      - [Seifert circle](#seifert-circle)
    - [Seifert genus](#seifert-genus)
      - [Additivity of Seifert genus](#additivity-of-seifert-genus)
    - [Seifert form](#seifert-form)
      - [Seifert matrix](#seifert-matrix)
        - [Seifert-matrix presentation of the Alexander module](#seifert-matrix-presentation-of-the-alexander-module)
        - [Alexander polynomial](#alexander-polynomial)
          - [Conway polynomial (knot theory)](#conway-polynomial-knot-theory)
            - [Conway-normalized Alexander polynomial](#conway-normalized-alexander-polynomial)
          - [Alexander breadth bound on Seifert genus](#alexander-breadth-bound-on-seifert-genus)
            - [Full-degree irreducible Alexander polynomial implies a prime knot](#full-degree-irreducible-alexander-polynomial-implies-a-prime-knot)
          - [Alexander polynomial realization theorem](#alexander-polynomial-realization-theorem)
          - [Alexander module of a knot](#alexander-module-of-a-knot)
            - [Alexander module of a connected sum](#alexander-module-of-a-connected-sum)
          - [Alexander matrix](#alexander-matrix)
            - [Kauffman state of a knot diagram](#kauffman-state-of-a-knot-diagram)
          - [Knot determinant](#knot-determinant)
        - [Levine-Tristram signature](#levine-tristram-signature)
          - [Signature of a knot](#signature-of-a-knot)
            - [Alternating diagram signature formula](#alternating-diagram-signature-formula)
      - [Algebraic concordance of knots](#algebraic-concordance-of-knots)
        - [Metabolic Seifert form](#metabolic-seifert-form)
        - [Algebraic concordance group over a field](#algebraic-concordance-group-over-a-field)
          - [Isometric structure](#isometric-structure)
            - [Witt group of isometric structures](#witt-group-of-isometric-structures)
              - [Primary component of an isometric structure](#primary-component-of-an-isometric-structure)
          - [P-adic algebraic-concordance obstruction](#p-adic-algebraic-concordance-obstruction)
  - [Knot exterior](#knot-exterior)
    - [Nontrivial knot exteriors have incompressible boundary](#nontrivial-knot-exteriors-have-incompressible-boundary)
    - [Knot group](#knot-group)
      - [Two-generator knot groups have cyclic Alexander modules](#two-generator-knot-groups-have-cyclic-alexander-modules)
      - [Dehn presentation of a knot group](#dehn-presentation-of-a-knot-group)
        - [Alexander numbering](#alexander-numbering)
      - [Wirtinger presentation](#wirtinger-presentation)
        - [Wirtinger generator](#wirtinger-generator)
    - [Meridian of a knot](#meridian-of-a-knot)
    - [Infinite cyclic cover of a knot exterior](#infinite-cyclic-cover-of-a-knot-exterior)
  - [Alternating knot](#alternating-knot)
  - [Knot diagram](#knot-diagram)
    - [Crossing change](#crossing-change)
      - [Unknotting crossing](#unknotting-crossing)
    - [Gauss code](#gauss-code)
      - [Oriented smoothing permutation of a Gauss code](#oriented-smoothing-permutation-of-a-gauss-code)
    - [Reduced knot diagram](#reduced-knot-diagram)
    - [Alternating knot diagram](#alternating-knot-diagram)
    - [Tait conjectures](#tait-conjectures)
    - [Crossing number of a knot](#crossing-number-of-a-knot)
      - [Tait crossing-number theorem](#tait-crossing-number-theorem)
    - [Reidemeister move](#reidemeister-move)
  - [Twist knot](#twist-knot)
  - [Figure-eight knot](#figure-eight-knot)
    - [Figure-eight knot group](#figure-eight-knot-group)
- [Knot concordance](#knot-concordance)
  - [Slice knot](#slice-knot)
    - [Slice disk](#slice-disk)
      - [Ribbon disk](#ribbon-disk)
        - [Ribbon knot](#ribbon-knot)
    - [Slice genus](#slice-genus)
      - [Levine-Tristram signature bound on the slice genus](#levine-tristram-signature-bound-on-the-slice-genus)
  - [Doubly slice knot](#doubly-slice-knot)
    - [Double slice genus](#double-slice-genus)
- [Two-fold branched cover of a knot](#two-fold-branched-cover-of-a-knot)
  - [Linking form of a branched cover](#linking-form-of-a-branched-cover)
- [Amphichiral knot](#amphichiral-knot)
- [Arf invariant of a knot](#arf-invariant-of-a-knot)
- [Twist-spun knot](#twist-spun-knot)
  - [Zeeman theorem on twist-spun knots](#zeeman-theorem-on-twist-spun-knots)
- [Surface knot](#surface-knot)
  - [Banded-unlink diagram](#banded-unlink-diagram)
- [Stevedore knot](#stevedore-knot)
- [Seifert longitude](#seifert-longitude)
  - [Preferred longitude of an unknot](#preferred-longitude-of-an-unknot)
- [Link](#link)
  - [Link invariant](#link-invariant)
  - [Split link](#split-link)
    - [Split link diagram](#split-link-diagram)
  - [Borromean rings](#borromean-rings)
    - [Borromean link group](#borromean-link-group)
  - [Multivariable Alexander polynomial](#multivariable-alexander-polynomial)
  - [Link exterior](#link-exterior)
  - [Hopf link](#hopf-link)
    - [Zero surgery on the Hopf link](#zero-surgery-on-the-hopf-link)
  - [Unlink](#unlink)
  - [Linking number](#linking-number)
  - [Link isotopy](#link-isotopy)
    - [Mirror of a link](#mirror-of-a-link)
  - [Writhe](#writhe)
  - [Link diagram](#link-diagram)
    - [Alternating link diagram](#alternating-link-diagram)
      - [Reduced alternating link diagram](#reduced-alternating-link-diagram)
    - [Adequate link diagram](#adequate-link-diagram)
    - [Turaev surface](#turaev-surface)
    - [Tait graph](#tait-graph)
    - [Skein relation](#skein-relation)
      - [Oriented smoothing](#oriented-smoothing)
    - [Writhe of a link diagram](#writhe-of-a-link-diagram)
    - [Tangle](#tangle)
      - [Tangle category](#tangle-category)
      - [Mutation (knot theory)](#mutation-knot-theory)
    - [Kauffman bracket](#kauffman-bracket)
      - [Kauffman bracket skein module](#kauffman-bracket-skein-module)
        - [Relative Kauffman bracket skein module](#relative-kauffman-bracket-skein-module)
      - [Kauffman bracket breadth bound](#kauffman-bracket-breadth-bound)
        - [Jones polynomial breadth bound for a disconnected diagram](#jones-polynomial-breadth-bound-for-a-disconnected-diagram)
      - [Temperley-Lieb diagram algebra](#temperley-lieb-diagram-algebra)
        - [Jones-Wenzl idempotent](#jones-wenzl-idempotent)
          - [Jones-Wenzl partial trace](#jones-wenzl-partial-trace)
          - [Reduced Temperley-Lieb skein theory](#reduced-temperley-lieb-skein-theory)
            - [Jones-Wenzl color](#jones-wenzl-color)
            - [Semisimplicity of the reduced Temperley-Lieb category](#semisimplicity-of-the-reduced-temperley-lieb-category)
            - [Fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors)
              - [Dimension-weighted fusion resolution](#dimension-weighted-fusion-resolution)
              - [Hopf pairing of Jones-Wenzl colors](#hopf-pairing-of-jones-wenzl-colors)
          - [Jones-Wenzl twist eigenvalue](#jones-wenzl-twist-eigenvalue)
        - [Bracket trace on the three-strand Temperley-Lieb algebra](#bracket-trace-on-the-three-strand-temperley-lieb-algebra)
      - [Bracket smoothing state](#bracket-smoothing-state)
      - [Jones polynomial](#jones-polynomial)
        - [Jones unknot detection problem](#jones-unknot-detection-problem)
        - [Signed Jones evaluation at minus one](#signed-jones-evaluation-at-minus-one)
        - [Jones polynomial of a mirror](#jones-polynomial-of-a-mirror)
        - [Jones polynomial evaluation at one](#jones-polynomial-evaluation-at-one)
        - [Jones polynomial of a split union](#jones-polynomial-of-a-split-union)
        - [Jones polynomial of a connected sum](#jones-polynomial-of-a-connected-sum)
        - [Jones polynomial skein relation](#jones-polynomial-skein-relation)
        - [Unreduced Jones polynomial](#unreduced-jones-polynomial)
  - [Torus link](#torus-link)
  - [Framed link](#framed-link)
    - [Surface framing](#surface-framing)
    - [Seifert framing](#seifert-framing)
    - [Dehn surgery on a framed link](#dehn-surgery-on-a-framed-link)
      - [Integer surgery coefficient](#integer-surgery-coefficient)
      - [Surgery trace](#surgery-trace)
        - [Surgery linking matrix](#surgery-linking-matrix)
        - [Kirby calculus](#kirby-calculus)
          - [Jones polynomial surgery invariant](#jones-polynomial-surgery-invariant)
          - [Kirby diagram](#kirby-diagram)
          - [Slam-dunk move](#slam-dunk-move)
      - [Lens space](#lens-space)
        - [Genus-one gluing model of a lens space](#genus-one-gluing-model-of-a-lens-space)
        - [Oriented classification of lens spaces](#oriented-classification-of-lens-spaces)
- [Colored link](#colored-link)
  - [Kirby color](#kirby-color)
    - [Gauss sums of Jones-Wenzl colors](#gauss-sums-of-jones-wenzl-colors)
      - [Nonvanishing of Kirby stabilization factors](#nonvanishing-of-kirby-stabilization-factors)
    - [Kirby color handle-slide identity](#kirby-color-handle-slide-identity)
- [Dehn surgery](#dehn-surgery)
  - [Dehn filling](#dehn-filling)
    - [Fundamental theorem of Dehn surgery](#fundamental-theorem-of-dehn-surgery)
      - [Unit surface-framed surgery realizes a Dehn twist](#unit-surface-framed-surgery-realizes-a-dehn-twist)
    - [Fiber-curve surgery](#fiber-curve-surgery)
    - [Rational Dehn surgery](#rational-dehn-surgery)
    - [Annulus-quotient model of Dehn filling](#annulus-quotient-model-of-dehn-filling)
- [Fibered knot](#fibered-knot)
  - [Homological monodromy of a genus-one fibered knot](#homological-monodromy-of-a-genus-one-fibered-knot)
  - [Nielsen–Thurston classification](#nielsen-thurston-classification)
    - [Periodic surface homeomorphism](#periodic-surface-homeomorphism)
    - [Pseudo-Anosov map](#pseudo-anosov-map)
    - [Anosov homeomorphism](#anosov-homeomorphism)
    - [Hyperbolization of a pseudo-Anosov mapping torus](#hyperbolization-of-a-pseudo-anosov-mapping-torus)
- [Seifert fibered space](#seifert-fibered-space)
  - [Vertical surface in a Seifert fibered space](#vertical-surface-in-a-seifert-fibered-space)
  - [Horizontal surface in a Seifert fibered space](#horizontal-surface-in-a-seifert-fibered-space)
  - [Seifert fiber](#seifert-fiber)
  - [Seifert fibrations of real projective 3-space](#seifert-fibrations-of-real-projective-3-space)
- [Splice of knots](#splice-of-knots)
  - [Zero surgery on a connected sum as a splice](#zero-surgery-on-a-connected-sum-as-a-splice)
- [Turaev torsion](#turaev-torsion)
  - [Homology orientation](#homology-orientation)
  - [Euler structure](#euler-structure)
  - [Turaev-torsion Dehn-filling formula](#turaev-torsion-dehn-filling-formula)
- [Satellite knot as a splice](#satellite-knot-as-a-splice)

## Knot invariant

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_invariant)

A knot invariant assigns the same value to isotopic [knots](#knot). Examples include the [knot group](#knot-group), [Alexander polynomial of a knot](#alexander-polynomial), [Seifert genus](#seifert-genus), [knot signature](#signature-of-a-knot) and [Jones polynomial](#jones-polynomial). Different [knot invariants](#knot-invariant) can retain different information: isomorphic [knot groups](#knot-group) do not alone imply isotopic [knots](#knot).

## Knot

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_(mathematics))

A knot is a smooth embedding $S^1\hookrightarrow S^3$, considered up to ambient isotopy.

### Oriented knot

↑ **Parent:** [Knot](#knot)

An oriented knot is a [knot](#knot) together with a choice of orientation on its embedded circle.

### Unknot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unknot)

The unknot is the knot bounding a smoothly embedded disk in $S^3$.

### Connected sum of knots

↑ **Parent:** [Knot](#knot)

The connected sum removes a short unknotted arc from each of two oriented knots and joins the four endpoints by an orientation-compatible pair of arcs.

The ambient three-sphere is also joined by [connected sum](differential-geometry.md#connected-sum-of-oriented-manifolds), while the two knot arcs join inside it.

#### Prime decomposition of knots

↑ **Parent:** [Connected sum of knots](#connected-sum-of-knots)

Every nontrivial oriented [knot](#knot) is a finite [connected sum of knots](#connected-sum-of-knots) of [prime knots](#prime-knot), uniquely up to permutation and oriented [link isotopy](#link-isotopy). Existence follows by induction from [additivity of Seifert genus](#additivity-of-seifert-genus). For uniqueness, compare complete [decomposing sphere systems for a knot](#decomposing-sphere-system-for-a-knot) and remove their intersection [circles](topology.md#circle) by the [prime-ball exchange lemma](#prime-ball-exchange-lemma). Once a prime ball is disjoint from both systems, its factor can be removed from both; induction then matches all factors.

#### Composite knot

↑ **Parent:** [Connected sum of knots](#connected-sum-of-knots)

A composite knot is a connected sum of two nontrivial knots.

#### Prime knot

↑ **Parent:** [Connected sum of knots](#connected-sum-of-knots)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_knot)

A prime knot is a nontrivial knot that is not a [composite knot](#composite-knot).

#### Splitting sphere of a knot

↑ **Parent:** [Connected sum of knots](#connected-sum-of-knots)

A splitting sphere meets a knot transversely in two points. It is trivial when one of the resulting one-string tangles is boundary-parallel in its three-ball; otherwise it exhibits a nontrivial connected-sum decomposition.

##### Decomposing sphere system for a knot

↑ **Parent:** [Splitting sphere of a knot](#splitting-sphere-of-a-knot)

A finite collection of disjoint [splitting spheres of a knot](#splitting-sphere-of-a-knot) encodes a [connected sum of knots](#connected-sum-of-knots). Cut along every [sphere](geometry-and-topology.md#sphere) and fill each spherical boundary with a [three-ball](topology.md#three-ball) containing a straight arc joining its two marked endpoints. The resulting oriented [knots](#knot) are the factors. The system is complete when its nontrivial factors are [prime knots](#prime-knot).

###### Prime-ball exchange lemma

↑ **Parent:** [Decomposing sphere system for a knot](#decomposing-sphere-system-for-a-knot)

In a complete [decomposing sphere system for a knot](#decomposing-sphere-system-for-a-knot), a disk inside a prime-factor ball that meets the knotted arc once cuts its factor into a [connected sum of knots](#connected-sum-of-knots). One side must be an [unknot](#unknot). Replacing the ball by the side carrying the prime factor therefore preserves the unordered factor list. A disk missing the arc cuts off an empty ball and gives the same conclusion. After a small transverse perturbation, such a replacement removes an innermost intersection [circle](topology.md#circle) with another sphere system. If a chosen innermost disk contains both marked points, another innermost disk, or its complementary disk when it is the only intersection, contains neither. Iterating produces a prime-factor ball disjoint from both systems. The replacement changes only the location of a joining arc in the intervening punctured ball; capping the other boundaries still recovers the same oriented factors.

### Torus knot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torus_knot)

For coprime integers $p,q$, the torus knot $T_{p,q}$ winds $p$ times meridionally and $q$ times longitudinally on an unknotted torus in $S^3$.

#### Torus knots are prime

↑ **Parent:** [Torus knot](#torus-knot)

For coprime p,q with absolute values at least two, the [knot group](#knot-group) is $\langle a,b\mid a^p=b^q\rangle$. Its nontrivial central element $z=a^p=b^q$ maps nontrivially to the abelianization. A meridian $a^ub^v$, where $qu+pv=1$, has infinite order in the quotient $C_{|p|}*C_{|q|}$. A composite [knot](#knot) [group](group.md) would be an [amalgamated free product](algebraic-topology.md#amalgamated-free-product) of proper factors over its meridian subgroup, whose center lies in that subgroup. Then z would be a meridian power, contradicting the infinite order of the meridian modulo z.

// Target: geometric-group-theory.bigb

#### Trefoil knot

↑ **Parent:** [Torus knot](#torus-knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trefoil_knot)

The trefoil is the torus knot $T_{2,3}$. It has [Seifert genus](#seifert-genus) one, [crossing number of a knot](#crossing-number-of-a-knot) three, and [Alexander polynomial of a knot](#alexander-polynomial) $t-1+t^{-1}$ up to a unit.

### Satellite knot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Satellite_knot)

A satellite knot $P(K)$ is obtained by embedding a patterned solid torus into a tubular neighborhood of a companion knot $K$.

#### Pattern of a satellite knot

↑ **Parent:** [Satellite knot](#satellite-knot)

A pattern is a knot $P$ inside a solid torus. Embedding that torus as a tubular neighborhood of $K$ produces the satellite $P(K)$.

##### Winding number of a satellite pattern

↑ **Parent:** [Pattern of a satellite knot](#pattern-of-a-satellite-knot)

The winding number is the integer represented by the pattern in the first homology of the solid torus, equivalently its algebraic intersection number with a meridional disk.

#### Cable knot

↑ **Parent:** [Satellite knot](#satellite-knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cable_knot)

The $(p,q)$-cable of $K$ uses the $(p,q)$ torus knot as a pattern in a tubular neighborhood of $K$.

#### Satellite formula for the Levine-Tristram signature

↑ **Parent:** [Satellite knot](#satellite-knot)

For a pattern of winding number $w$,

$$
\sigma_\omega(P(K))=\sigma_\omega(P(U))+\sigma_{\omega^w}(K)
$$

whenever the relevant [signatures](#levine-tristram-signature) are defined by nonsingular forms. The usual averaged convention extends the identity through roots.

#### Satellite formula for the Alexander polynomial

↑ **Parent:** [Satellite knot](#satellite-knot)

If a satellite knot has pattern $P$, companion $K$, and winding number $w$, then

$$
\Delta_{P(K)}(t)\doteq\Delta_{P(U)}(t)\Delta_K(t^w).
$$

#### Whitehead double

↑ **Parent:** [Satellite knot](#satellite-knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Whitehead_double)

A Whitehead double is the satellite formed with the Whitehead pattern, which has winding number zero and whose image on the unknot is an unknot. The [Satellite formula for the Alexander polynomial](#satellite-formula-for-the-alexander-polynomial) therefore gives $\Delta(t)\doteq1$ for every untwisted Whitehead double.

### Seifert surface

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seifert_surface)

A Seifert surface for an oriented knot $K$ is a compact connected oriented surface $F\subset S^3$ with oriented boundary $\partial F=K$.

#### Hopf band

↑ **Parent:** [Seifert surface](#seifert-surface)

A Hopf band is an annulus with one full twist whose boundary is a [Hopf link](#hopf-link). Plumbing it with another band adds a generator to the first [homology](homology.md) of a [Seifert surface](#seifert-surface). Its core has self-[linking number](#linking-number) $1$ or $-1$, depending on the twisting convention.

#### Seifert hypersurface

↑ **Parent:** [Seifert surface](#seifert-surface)

A Seifert hypersurface for an oriented codimension-two submanifold is an oriented codimension-one submanifold having it as boundary. For a closed oriented surface in $S^4$, an integral meridional map from the complement to the circle, with angular behavior near the surface, supplies a [Seifert hypersurface](#seifert-hypersurface) by taking a [regular value](differential-geometry.md#regular-value).

#### Seifert algorithm

↑ **Parent:** [Seifert surface](#seifert-surface)

Apply the [oriented smoothing](#oriented-smoothing) to every crossing of an oriented [knot diagram](#knot-diagram), fill the resulting [Seifert circles](#seifert-circle) by disjoint disks at suitable heights, and reconnect them by twisted bands at the original crossings. The boundary is the original [knot](#knot). If the connected surface has $s$ disks and $c$ bands, its [Euler characteristic](homology.md#euler-characteristic) is $s-c$ and its [genus](topology.md#genus-of-a-surface) is $(1-s+c)/2$.

##### Seifert circle

↑ **Parent:** [Seifert algorithm](#seifert-algorithm)

A Seifert circle is a component of the crossing-free diagram obtained by [oriented smoothing](#oriented-smoothing) at every crossing. These circles bound the disks used in the [Seifert algorithm](#seifert-algorithm).

#### Seifert genus

↑ **Parent:** [Seifert surface](#seifert-surface)

The Seifert genus is the smallest genus of a [Seifert surface](#seifert-surface) for the knot.

It minimizes the genus over all choices of [Seifert surface](#seifert-surface).

##### Additivity of Seifert genus

↑ **Parent:** [Seifert genus](#seifert-genus)

The [Seifert genus](#seifert-genus) is additive under [connected sum of knots](#connected-sum-of-knots):

$$
g_s(K\mathbin{\#}J)=g_s(K)+g_s(J).
$$

The upper bound comes from boundary-connected-summing minimal [Seifert surfaces](#seifert-surface), while the reverse inequality follows by cutting any Seifert surface for the connected sum along a splitting sphere.

#### Seifert form

↑ **Parent:** [Seifert surface](#seifert-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seifert_form)

For oriented curves $x,y$ on a Seifert surface, the Seifert form is

$$
\theta_F([x],[y])=\operatorname{lk}(x^+,y),
$$

where $x^+$ is a positive normal push-off of $x$.

##### Seifert matrix

↑ **Parent:** [Seifert form](#seifert-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seifert_matrix)

A Seifert matrix represents the [Seifert form](#seifert-form) in an integral basis of $H_1(F)$. Its skew-symmetrization $A-A^T$ represents the intersection form of the surface and is unimodular.

###### Seifert-matrix presentation of the Alexander module

↑ **Parent:** [Seifert matrix](#seifert-matrix)

Cut a [knot exterior](#knot-exterior) along a [Seifert surface](#seifert-surface) and stack copies to form its [infinite cyclic cover](#infinite-cyclic-cover-of-a-knot-exterior). Linking-dual generators for the [homology](homology.md) of the cut-open piece give the positive and negative inclusion [matrices](vector-space.md#matrix) $V$ and $V^T$ in row convention. The gluing relations therefore have [matrix](vector-space.md#matrix) $tV-V^T$. The H0 gluing map is multiplication by $t-1$ and is injective, so these relations present the entire [Alexander module of a knot](#alexander-module-of-a-knot). Its order is the determinant, up to a Laurent unit.

###### Alexander polynomial

↑ **Parent:** [Seifert matrix](#seifert-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander_polynomial)

Up to multiplication by a unit $\pm t^n$, the Alexander polynomial is

$$
\Delta_K(t)=\det(tA-A^T).
$$

It satisfies $\Delta_K(t^{-1})\doteq\Delta_K(t)$ and $\Delta_K(1)=\pm1$.

###### Conway polynomial (knot theory)

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

The Conway polynomial is normalized by $\nabla_U=1$ for the [unknot](#unknot), zero for a split [unlink](#unlink) with more than one component, and the [skein relation](#skein-relation) $\nabla_{L_+}-\nabla_{L_-}=z\nabla_{L_0}$. For a [knot](#knot), the symmetric [Alexander polynomial](#alexander-polynomial) with value one at $t=1$ is $\Delta_K(t)=\nabla_K(t^{1/2}-t^{-1/2})$. This fixes the Laurent-unit ambiguity of the [Seifert-matrix presentation of the Alexander module](#seifert-matrix-presentation-of-the-alexander-module).

###### Conway-normalized Alexander polynomial

↑ **Parent:** [Conway polynomial (knot theory)](#conway-polynomial-knot-theory)

The symmetric [Alexander polynomial](#alexander-polynomial) normalized by the [Conway polynomial](#conway-polynomial-knot-theory) is uniquely fixed for a [knot](#knot). Its sign matters in the [signed Jones evaluation at minus one](#signed-jones-evaluation-at-minus-one), whereas the [knot determinant](#knot-determinant) retains only the absolute value.

###### Alexander breadth bound on Seifert genus

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

A minimal-[genus](topology.md#genus-of-a-surface) [Seifert surface](#seifert-surface) has a $2g_s(K)$-by-$2g_s(K)$ [Seifert matrix](#seifert-matrix) $V$. Each entry of $tV-V^T$ has degree at most one, so its [determinant](linear-algebra.md#determinant) has [breadth of a Laurent polynomial](polynomial.md#breadth-of-a-laurent-polynomial) at most $2g_s(K)$. This lower bound on [Seifert genus](#seifert-genus) need not be sharp: an untwisted [Whitehead double](#whitehead-double) can have [Alexander polynomial of a knot](#alexander-polynomial) $1$ and positive [Seifert genus](#seifert-genus).

###### Full-degree irreducible Alexander polynomial implies a prime knot

↑ **Parent:** [Alexander breadth bound on Seifert genus](#alexander-breadth-bound-on-seifert-genus)

Assume $g_s(K)>0$. A nontrivial [connected sum of knots](#connected-sum-of-knots) has positive genus summands, and [additivity of Seifert genus](#additivity-of-seifert-genus) applies. Its [Alexander polynomial of a knot](#alexander-polynomial) is the product of the summand [polynomials](polynomial.md). If the [polynomial](polynomial.md) is irreducible, one summand has unit [polynomial](polynomial.md); the other must then have [polynomial](polynomial.md) breadth $2g_s(K)$, exceeding twice its strictly smaller genus. This contradicts the [Alexander breadth bound on Seifert genus](#alexander-breadth-bound-on-seifert-genus). Irreducibility without the full-degree hypothesis alone does not imply primeness.

###### Alexander polynomial realization theorem

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

Every Laurent polynomial $f(t)\in\mathbb Z[t^{\pm1}]$ satisfying $f(t^{-1})=f(t)$ and $f(1)=1$ is the [Alexander polynomial of a knot](#alexander-polynomial) up to multiplication by a unit $\pm t^k$.

###### Alexander module of a knot

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

The Alexander module is the first integral homology of the [infinite cyclic cover of a knot exterior](#infinite-cyclic-cover-of-a-knot-exterior). Its deck transformation makes it a module over $\mathbb Z[t^{\pm1}]$, and its first elementary ideal determines the [Alexander polynomial of a knot](#alexander-polynomial).

###### Alexander module of a connected sum

↑ **Parent:** [Alexander module of a knot](#alexander-module-of-a-knot)

Boundary-connected-summing [Seifert surfaces](#seifert-surface) gives a block-diagonal [Seifert matrix](#seifert-matrix), because basis curves in the separated summands have zero linking. The [Seifert-matrix presentation of the Alexander module](#seifert-matrix-presentation-of-the-alexander-module) is block diagonal too. Thus the Alexander [modules](module-theory.md#module-mathematics) form a direct sum and their [Alexander polynomials of a knot](#alexander-polynomial) multiply up to a unit.

###### Alexander matrix

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

Given a presentation $\langle x_1,\ldots,x_n\mid r_1,\ldots,r_m\rangle$ of a knot group, apply abelianization to the [Fox derivatives](geometric-group-theory.md#fox-calculus) $\partial r_j/\partial x_i$. The resulting matrix over $\mathbb Z[t^{\pm1}]$ is an Alexander matrix; suitable maximal minors recover the [Alexander polynomial of a knot](#alexander-polynomial).

###### Kauffman state of a knot diagram

↑ **Parent:** [Alexander matrix](#alexander-matrix)

For a reduced knot diagram with two adjacent starred regions, a Kauffman state chooses one corner at every crossing so that every unstarred region contains exactly one chosen corner. Terms in a determinant expansion of a Dehn-presentation [Alexander matrix](#alexander-matrix) correspond bijectively to these states.

###### Knot determinant

↑ **Parent:** [Alexander polynomial](#alexander-polynomial)

The knot determinant is $|\Delta_K(-1)|=|\det(A+A^T)|$. It is also the order of the first homology of the two-fold cover of $S^3$ branched over $K$.

###### Levine-Tristram signature

↑ **Parent:** [Seifert matrix](#seifert-matrix)

For $\omega\in S^1\setminus\{1\}$, the Levine-Tristram signature is the signature of the Hermitian matrix

$$
H_\omega=(1-\omega)A+(1-\overline\omega)A^T.
$$

It is locally constant away from unit roots of the [Alexander polynomial of a knot](#alexander-polynomial).

At $\omega=-1$, this becomes the [signature of a knot](#signature-of-a-knot).

###### Signature of a knot

↑ **Parent:** [Levine-Tristram signature](#levine-tristram-signature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Signature_of_a_knot)

The knot signature is the [signature](linear-algebra.md#signature-of-a-quadratic-form) of the symmetrized [Seifert matrix](#seifert-matrix). Equivalently it is the [signature](linear-algebra.md#signature-of-a-quadratic-form) of the double [branched covering](algebraic-topology.md#branched-covering) of $B^4$ over a pushed-in [Seifert surface](#seifert-surface). At $\omega=-1$ it agrees with the [Levine-Tristram signature](#levine-tristram-signature). It is additive under [connected sum of knots](#connected-sum-of-knots), changes sign under reflection, and obeys $|\sigma(K)|\leq2g_4(K)$. State the ambient [orientation](algebraic-topology.md#orientation-of-a-simplex) and push-off convention when assigning a sign.

###### Alternating diagram signature formula

↑ **Parent:** [Signature of a knot](#signature-of-a-knot)

For a reduced connected [alternating knot diagram](#alternating-knot-diagram), its [knot signature](#signature-of-a-knot) is $s_A(D)-c_+(D)-1$, where $s_A$ counts circles in the all-$A$ [bracket smoothing state](#bracket-smoothing-state) and $c_+$ counts positive crossings. The convention is that the $A$-smoothing at a positive braid crossing is the [oriented smoothing](#oriented-smoothing), and a positive [trefoil knot](#trefoil-knot) has [knot signature](#signature-of-a-knot) $-2$. Reversing the global [knot signature](#signature-of-a-knot) convention negates the formula.

##### Algebraic concordance of knots

↑ **Parent:** [Seifert form](#seifert-form)

Two Seifert forms are algebraically concordant when their difference is metabolic. Stable equivalence classes form the algebraic concordance group.

###### Metabolic Seifert form

↑ **Parent:** [Algebraic concordance of knots](#algebraic-concordance-of-knots)

A nonsingular Seifert form on a $2g$-dimensional space is metabolic when it vanishes on a $g$-dimensional subspace called a metabolizer.

The metabolizer is a half-dimensional subspace on which the [Seifert form](#seifert-form) restricts to zero.

###### Algebraic concordance group over a field

↑ **Parent:** [Algebraic concordance of knots](#algebraic-concordance-of-knots)

The algebraic concordance group over a field $F$ is the Witt group of nonsingular Seifert forms over $F$, modulo metabolic forms.

###### Isometric structure

↑ **Parent:** [Algebraic concordance group over a field](#algebraic-concordance-group-over-a-field)

An isometric structure consists of a finite-dimensional vector space $V$, a nonsingular symmetric bilinear form $Q$, and a $Q$-isometry $T$ with the required nondegeneracy at $\pm1$. Metabolic isometric structures are quotiented out to form $\mathcal W_F$.

###### Witt group of isometric structures

↑ **Parent:** [Isometric structure](#isometric-structure)

The Witt group of isometric structures identifies two [isometric structures](#isometric-structure) when their orthogonal difference is metabolic.

###### Primary component of an isometric structure

↑ **Parent:** [Witt group of isometric structures](#witt-group-of-isometric-structures)

For an irreducible symmetric Laurent polynomial $\delta$, the primary component is

$$
V_\delta=\ker\delta(T)^N
$$

for sufficiently large $N$. Distinct symmetric primary components are orthogonal, so restriction defines a projection $\mathcal W_F\to\mathcal W_F^\delta$.

###### P-adic algebraic-concordance obstruction

↑ **Parent:** [Algebraic concordance group over a field](#algebraic-concordance-group-over-a-field)

Extending an algebraic-concordance class from $\mathbb Q$ to a p-adic field $\mathbb Q_p$ detects torsion invisible over the real numbers. For $p\equiv3\pmod4$, an odd-dimensional second-residue form generates the order-four part of the local Witt group.

### Knot exterior

↑ **Parent:** [Knot](#knot)

The knot exterior is $E_K=S^3\setminus\operatorname{int}\nu K$, where $\nu K$ is an open tubular neighborhood of the knot. It is homotopy equivalent to the [knot complement](#knot-exterior) $S^3\setminus K$.

#### Nontrivial knot exteriors have incompressible boundary

↑ **Parent:** [Knot exterior](#knot-exterior)

A [sphere](geometry-and-topology.md#sphere) in a [knot](#knot) exterior bounds a ball on the side not containing the [knot](#knot), so the exterior is irreducible. A compression disk for its boundary [torus](topology.md#torus) would cut the exterior to a manifold with [sphere](geometry-and-topology.md#sphere) boundary; irreducibility makes that manifold a ball, and reversing the compression gives a solid [torus](topology.md#torus) exterior. Its meridian disk has boundary a preferred [knot](#knot) longitude, so adjoining the boundary annulus gives a spanning disk for the [knot](#knot), which is then an [unknot](#unknot). The [Loop theorem](topology.md#loop-theorem) therefore makes the peripheral fundamental [group](group.md) injective for every nontrivial [knot](#knot). In particular its [knot](#knot) [group](group.md) contains an injected copy of the [torus](topology.md#torus) [group](group.md) and cannot be cyclic.

#### Knot group

↑ **Parent:** [Knot exterior](#knot-exterior)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_group)

The knot group is the [fundamental group](algebraic-topology.md#fundamental-group) of the [knot exterior](#knot-exterior).

##### Two-generator knot groups have cyclic Alexander modules

↑ **Parent:** [Knot group](#knot-group)

The abelianization of a [knot group](#knot-group) is infinite cyclic. Nielsen changes of a two-generator free basis reduce its exponent vector to $(1,0)$. In the cyclic-cover [cellular chain complex](homology.md#cellular-chain-complex), the first boundary is then $(t-1,0)$, whose kernel is a free rank-one Laurent [module](module-theory.md#module-mathematics). Quotienting by the lifted relator boundaries gives a [cyclic module](module-theory.md#cyclic-module), regardless of the number of relators. A noncyclic [Alexander module](#alexander-module-of-a-knot) therefore obstructs every two-generator knot-group presentation.

##### Dehn presentation of a knot group

↑ **Parent:** [Knot group](#knot-group)

Give every region of a [knot diagram](#knot-diagram) a generator and set the generator of the unbounded region to the identity. At a crossing, reading the four incident regions cyclically gives a relation $a b^{-1}c d^{-1}=1$, with the cyclic order reversed if the opposite convention is chosen. These relations form the Dehn presentation of the knot group.

###### Alexander numbering

↑ **Parent:** [Dehn presentation of a knot group](#dehn-presentation-of-a-knot-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alexander_numbering)

An Alexander numbering assigns an integer to every region of an oriented link diagram so that crossing an oriented arc from right to left increases the integer by one. Under abelianization, a Dehn region generator with number $m$ maps to $t^m$.

##### Wirtinger presentation

↑ **Parent:** [Knot group](#knot-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wirtinger_presentation)

A Wirtinger presentation has one meridional generator for every arc of a [knot diagram](#knot-diagram) and one conjugacy relator at every crossing. For a connected diagram one crossing relator is redundant, giving a deficiency-one presentation of the [knot group](#knot-group).

###### Wirtinger generator

↑ **Parent:** [Wirtinger presentation](#wirtinger-presentation)

A Wirtinger generator is the [meridian of a knot](#meridian-of-a-knot) associated with an arc of a [knot diagram](#knot-diagram) between successive undercrossings. The overpassing meridian conjugates the incoming meridian to the outgoing meridian, with exponent determined by the crossing sign.

#### Meridian of a knot

↑ **Parent:** [Knot exterior](#knot-exterior)

A meridian is an oriented simple closed curve on the boundary of a [knot exterior](#knot-exterior) that bounds a disk in the removed tubular neighborhood and has [linking number](#linking-number) one with the knot.

Viewed inside the removed tubular neighborhood, this is a [meridian of a solid torus](topology.md#meridian-of-a-solid-torus).

#### Infinite cyclic cover of a knot exterior

↑ **Parent:** [Knot exterior](#knot-exterior)

The infinite cyclic cover corresponds to the kernel of the abelianization $\pi_1(E_K)\to\mathbb Z$. Its deck group is generated by $t$, so its cellular chains and homology are modules over $\mathbb Z[t^{\pm1}]$.

### Alternating knot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alternating_knot)

An [alternating knot](#alternating-knot) is a [knot](#knot) admitting an [alternating knot diagram](#alternating-knot-diagram). A nonalternating diagram can still represent an alternating knot; the property of the knot is existential over its diagrams.

### Knot diagram

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_diagram)

A knot diagram is a generic projection of a [knot](#knot) to a plane together with overcrossing and undercrossing information at every double point.

#### Crossing change

↑ **Parent:** [Knot diagram](#knot-diagram)

A crossing change exchanges the overpassing and underpassing strands at one crossing of a [knot diagram](#knot-diagram). It generally changes the [knot](#knot); unlike a [Reidemeister move](#reidemeister-move), it is not an [isotopy](differential-geometry.md#isotopy). Two oriented band moves realize a crossing change as a genus-one [knot cobordism](geometry-and-topology.md#knot-cobordism).

##### Unknotting crossing

↑ **Parent:** [Crossing change](#crossing-change)

An unknotting crossing is a crossing whose [crossing change](#crossing-change) converts a [knot](#knot) into the [unknot](#unknot). It gives a genus-one [knot cobordism](geometry-and-topology.md#knot-cobordism) to the [unknot](#unknot), and hence [slice genus](#slice-genus) at most one after capping with a disk in $B^4$.

#### Gauss code

↑ **Parent:** [Knot diagram](#knot-diagram)

A Gauss code records the successive crossings encountered when traversing an oriented [knot diagram](#knot-diagram). Each crossing label occurs twice; overpassing/underpassing data and crossing signs make the code sufficient to recover its [Wirtinger presentation](#wirtinger-presentation) and smoothing counts. Labels are arbitrary and cyclic starting points represent the same traversal.

##### Oriented smoothing permutation of a Gauss code

↑ **Parent:** [Gauss code](#gauss-code)

Number the $2n$ visits along an oriented [knot diagram](#knot-diagram), and let $\tau$ exchange the two visits to each crossing. At an [oriented smoothing](#oriented-smoothing), an incoming strand follows the outgoing strand of the other visit. Thus the cycles of the displayed [permutation](combinatorics.md#permutation) are exactly the [Seifert circles](#seifert-circle). Their count $s$ gives the [Seifert algorithm](#seifert-algorithm) genus $(1-s+n)/2$ without requiring a separate drawing of the smoothed diagram.

#### Reduced knot diagram

↑ **Parent:** [Knot diagram](#knot-diagram)

A knot diagram is reduced when it has no nugatory crossing, equivalently no crossing can be isolated from the rest of the diagram by a circle meeting the diagram only at that crossing.

#### Alternating knot diagram

↑ **Parent:** [Knot diagram](#knot-diagram)

An alternating knot diagram alternates between overcrossings and undercrossings while traversing its component.

A [knot](#knot) admitting such a diagram is an [alternating knot](#alternating-knot).

#### Tait conjectures

↑ **Parent:** [Knot diagram](#knot-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tait_conjectures)

The Tait conjectures concern reduced [alternating knot diagrams](#alternating-knot-diagram): they minimize the [crossing number of a knot](#crossing-number-of-a-knot), have an invariant diagram [writhe](#writhe), and are related by flypes. These formerly conjectural assertions are now theorems; the first is the [Tait crossing-number theorem](#tait-crossing-number-theorem).

#### Crossing number of a knot

↑ **Parent:** [Knot diagram](#knot-diagram)

The crossing number $c(K)$ is the least number of crossings in any [knot diagram](#knot-diagram) of $K$.

##### Tait crossing-number theorem

↑ **Parent:** [Crossing number of a knot](#crossing-number-of-a-knot)

Every reduced alternating diagram of a link has the minimum possible number of crossings. This result is one of the former Tait conjectures.

It is the minimum-crossing assertion among the [Tait conjectures](#tait-conjectures).

#### Reidemeister move

↑ **Parent:** [Knot diagram](#knot-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reidemeister_move)

The three Reidemeister moves are local changes of a link diagram that create or remove a kink, create or remove two opposite crossings, or slide one strand past a crossing. Two diagrams represent isotopic links exactly when they are related by planar isotopy and finitely many Reidemeister moves.

### Twist knot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Twist_knot)

A twist knot is obtained by closing two strands with a clasp after inserting a row of half-twists. Every nontrivial twist knot has [Seifert genus](#seifert-genus) one; a standard reduced alternating diagram with $m$ crossings in the twist region has $m+2$ crossings.

### Figure-eight knot

↑ **Parent:** [Knot](#knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Figure-eight_knot)

The figure-eight knot is the unique knot of [crossing number of a knot](#crossing-number-of-a-knot) four. It is prime, alternating, and has [Alexander polynomial of a knot](#alexander-polynomial) $-t+3-t^{-1}$ up to a unit.

#### Figure-eight knot group

↑ **Parent:** [Figure-eight knot](#figure-eight-knot)

The [fundamental group](algebraic-topology.md#fundamental-group) of the [figure-eight knot](#figure-eight-knot) complement has the displayed two-generator one-relator presentation. It follows from the [Artin automorphism of a braid](group.md#artin-automorphism-of-a-braid) for $(\sigma_1\sigma_2^{-1})^2$ by eliminating the third meridian from its fixed-generator presentation.

## Knot concordance

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knot_concordance)

Two knots are concordant when they cobound a smoothly embedded annulus in $S^3\times[0,1]$. Connected sum makes concordance classes into an abelian group.

### Slice knot

↑ **Parent:** [Knot concordance](#knot-concordance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slice_knot)

A slice knot bounds a smooth properly embedded disk in the four-ball $B^4$.

#### Slice disk

↑ **Parent:** [Slice knot](#slice-knot)

A slice disk is a smooth proper embedding $D^2\hookrightarrow B^4$ whose boundary is the knot in $S^3=\partial B^4$.

##### Ribbon disk

↑ **Parent:** [Slice disk](#slice-disk)

A ribbon disk is a slice disk whose radial Morse function has no interior local maxima. It can be built from disks by attaching bands.

###### Ribbon knot

↑ **Parent:** [Ribbon disk](#ribbon-disk)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ribbon_knot)

A ribbon knot is the boundary of a [ribbon disk](#ribbon-disk).

#### Slice genus

↑ **Parent:** [Slice knot](#slice-knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slice_genus)

The slice genus is the smallest genus of a smooth compact connected oriented surface properly embedded in $B^4$ with boundary $K$.

##### Levine-Tristram signature bound on the slice genus

↑ **Parent:** [Slice genus](#slice-genus)

For every unit complex number $\omega$ at which the signature form is nonsingular,

$$
2g_4(K)\geq|\sigma_\omega(K)|.
$$

### Doubly slice knot

↑ **Parent:** [Knot concordance](#knot-concordance)

A knot is doubly slice when it is the equatorial cross-section of an unknotted smooth two-sphere in $S^4$.

#### Double slice genus

↑ **Parent:** [Doubly slice knot](#doubly-slice-knot)

The double slice genus is the smallest genus of an unknotted closed orientable surface in $S^4$ whose transverse equatorial cross-section is $K$.

## Two-fold branched cover of a knot

↑ **Parent:** [Knot theory](knot-theory.md)

The two-fold branched cover of a knot is the double cover of $S^3$ branched along the knot. Its first homology has a nonsingular linking form and, when finite, has order $\det K$.

Away from the knot this is a two-sheeted [covering space](algebraic-topology.md#covering-space); at the knot it has the standard local model of a [branched covering](algebraic-topology.md#branched-covering).

### Linking form of a branched cover

↑ **Parent:** [Two-fold branched cover of a knot](#two-fold-branched-cover-of-a-knot)

For a rational homology three-sphere $Y$, the linking form is the nonsingular pairing

$$
\lambda_Y:\operatorname{Tor}H_1(Y)\times\operatorname{Tor}H_1(Y)\to\mathbb Q/\mathbb Z.
$$

Reversing the orientation of $Y$ negates this form.

Here the paired elements lie in the [torsion subgroup](group-theory.md#torsion-subgroup) of first [homology](homology.md).

## Amphichiral knot

↑ **Parent:** [Knot theory](knot-theory.md)

An amphichiral knot is ambient-isotopic to its mirror. Positive and negative amphichirality distinguish whether the symmetry preserves or reverses the knot orientation.

## Arf invariant of a knot

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arf_invariant_of_a_knot)

The Arf invariant is a $\mathbb Z/2$-valued concordance invariant obtained from the quadratic refinement of the mod-two intersection form on a Seifert surface.

## Twist-spun knot

↑ **Parent:** [Knot theory](knot-theory.md)

An $m$-twist spin removes a trivial arc from a knot and spins the resulting knotted arc around the boundary of a three-ball in $S^4$, inserting $m$ full twists during one revolution.

The result is a [surface knot](#surface-knot) with domain a two-sphere.

### Zeeman theorem on twist-spun knots

↑ **Parent:** [Twist-spun knot](#twist-spun-knot)

Zeeman's theorem says that the complement of an $m$-twist spin fibers over the circle with fiber the punctured $m$-fold cyclic branched cover of the original knot. In particular, the $1$- and $-1$-twist spins are unknotted.

This identifies the complement structure of a [twist-spun knot](#twist-spun-knot).

## Surface knot

↑ **Parent:** [Knot theory](knot-theory.md)

A surface knot is a smooth embedding of a closed connected surface in a four-manifold. In the narrow standard usage, a 2-knot is an embedded two-sphere in $S^4$.

It extends the embedding viewpoint of [knot theory](knot-theory.md) to two-dimensional domains.

### Banded-unlink diagram

↑ **Parent:** [Surface knot](#surface-knot)

A banded-unlink diagram consists of an unlink $U$ and disjoint bands whose simultaneous surgery produces another unlink. Capping the lower and upper unlinks by disks and tracing the band surgeries constructs a surface in $S^4$.

## Stevedore knot

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stevedore_knot_(mathematics))

The Stevedore knot $6_1$ is a ribbon knot with Alexander polynomial $2t^2-5t+2$ up to a unit.

## Seifert longitude

↑ **Parent:** [Knot theory](knot-theory.md)

The Seifert longitude is the zero-linking parallel of a knot on the boundary of its tubular neighborhood. It is the framing induced by a [Seifert surface](#seifert-surface).

### Preferred longitude of an unknot

↑ **Parent:** [Seifert longitude](#seifert-longitude)

The exterior of an [unknot](#unknot) is a [solid torus](topology.md#solid-torus). Inclusion of its boundary kills exactly the primitive [Seifert longitude](#seifert-longitude), so every essential simple closed curve bounding a disk in that exterior is isotopic, as an unoriented curve, to that longitude. The bounding disk need not avoid other link components.

## Link

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Link_(knot_theory))

A link is a smooth embedding of a finite disjoint union of circles in $S^3$, considered up to ambient isotopy. A one-component link is a [knot](#knot).

### Link invariant

↑ **Parent:** [Link](#link)

A [link](#link) invariant assigns the same value to [links](#link) related by [link isotopy](#link-isotopy). The [Jones polynomial](#jones-polynomial) applies to oriented [links](#link), while its bracket precursor retains a framing dependence. An invariant need not distinguish all [link](#link) types.

### Split link

↑ **Parent:** [Link](#link)

A split [link](#link) admits an embedded [sphere](geometry-and-topology.md#sphere) in its complement with nonempty portions of the [link](#link) on both sides. A split diagram admits a simple closed curve in the projection [sphere](geometry-and-topology.md#sphere) separating nonempty portions of the diagram. A split diagram always represents a split [link](#link); the converse need not hold for an arbitrary diagram.

#### Split link diagram

↑ **Parent:** [Split link](#split-link)

A split diagram has two nonempty parts separated by a simple closed curve disjoint from the diagram. For a two-component [link](#link), this is equivalent to disconnectedness of its projection graph. An [alternating link diagram](#alternating-link-diagram) representing a split [link](#link) cannot have a connected projection graph, as its Jones value at minus one detects a nonzero spanning-tree count.

### Borromean rings

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borromean_rings)

The Borromean rings are a three-component [link](#link) whose components are unknotted, which is nontrivial although removing any one component leaves an unlink. Its complement has a complete finite-volume [hyperbolic three-manifold](topology.md#hyperbolic-three-manifold) structure obtained from two regular ideal octahedra.

#### Borromean link group

↑ **Parent:** [Borromean rings](#borromean-rings)

With [group commutator](group.md#group-commutator) convention $[a,b]=a^{-1}b^{-1}ab$, the displayed [group presentation](geometric-group-theory.md#group-presentation) describes the [fundamental group](algebraic-topology.md#fundamental-group) of the [Borromean rings](#borromean-rings) complement. Its [abelianization](group-theory.md#abelianization) is $\mathbb Z^3$, since each relator is a [group commutator](group.md#group-commutator) and hence imposes no abelian relation. It embeds discretely in the [Gaussian Bianchi group](topological-group.md#gaussian-bianchi-group) by sending the meridians to $\begin{pmatrix}1&1\\0&1\end{pmatrix}$, $\begin{pmatrix}1&0\\2i&1\end{pmatrix}$ and $\begin{pmatrix}i&1\\2i&2-i\end{pmatrix}$.

### Multivariable Alexander polynomial

↑ **Parent:** [Link](#link)

For a [link](#link) with at least two components, this polynomial is the greatest common divisor of the appropriate maximal minors of an abelianized [Alexander matrix](#alexander-matrix), with one variable per oriented component meridian. It is defined up to multiplication by a signed monomial. For a deficiency-one presentation with $g$ generators and $g-1$ relators, use its $(g-1)$-row minors. This normalization gives one for a [Hopf link](#hopf-link).

### Link exterior

↑ **Parent:** [Link](#link)

The exterior of a [link](#link) is the complement of the interior of a closed [tubular neighborhood](differential-geometry.md#tubular-neighborhood) of the entire [link](#link). Its boundary consists of one [torus](topology.md#torus) per component; its [first homology](homology.md#first-homology) has the component meridians as a free basis.

### Hopf link

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf_link)

The Hopf link consists of two [unknots](#unknot) with [linking number](#linking-number) $\pm1$. Each component is a [meridian of a knot](#meridian-of-a-knot) of the other.

#### Zero surgery on the Hopf link

↑ **Parent:** [Hopf link](#hopf-link)

The [Hopf link](#hopf-link) exterior is $T^2\times I$. Each component's [Seifert longitude](#seifert-longitude) is the other's meridian. Filling the two boundary tori along these longitudes therefore attaches solid tori with meridians intersecting once on a common torus, recovering the standard genus-one splitting of the [three-sphere](geometry-and-topology.md#three-sphere). Merely specifying two linked [unknots](#unknot) without specifying their link type does not force this answer.

### Unlink

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unlink)

An unlink is a link whose components bound pairwise disjoint embedded disks in $S^3$.

### Linking number

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linking_number)

The linking number of two disjoint oriented closed curves in $S^3$ is the signed intersection number of one curve with a [Seifert surface](#seifert-surface) for the other. In an oriented diagram it is half the signed sum of crossings between the two components.

### Link isotopy

↑ **Parent:** [Link](#link)

A link isotopy is an [isotopy](differential-geometry.md#isotopy) of the ambient three-sphere carrying one link to another. It preserves the number and individual knot types of the components.

Here [ambient isotopy](differential-geometry.md#ambient-isotopy) is applied to the embedded [link](#link) inside the three-sphere.

#### Mirror of a link

↑ **Parent:** [Link isotopy](#link-isotopy)

Apply an orientation-reversing [homeomorphism](topology.md#homeomorphism) of $S^3$ to a [link](#link) and transport its component orientations. Reflection through the projection plane produces a [link diagram](#link-diagram) by switching every crossing.

### Writhe

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Writhe)

For an oriented closed curve, geometric [writhe](#writhe) is the signed crossing number averaged over generic viewing directions. For an individual [link diagram](#link-diagram), [writhe of a link diagram](#writhe-of-a-link-diagram) is its signed crossing sum. Both depend on geometry or projection rather than only the [link isotopy](#link-isotopy) class.

### Link diagram

↑ **Parent:** [Link](#link)

A link diagram is a generic planar projection of a [link](#link) with overcrossing and undercrossing data.

#### Alternating link diagram

↑ **Parent:** [Link diagram](#link-diagram)

A [link](#link) diagram is alternating if overpassing and underpassing crossings alternate along every component. Its checkerboard smoothing choices are consistent across all crossings of a connected projection. An [alternating knot diagram](#alternating-knot-diagram) is the one-component case.

##### Reduced alternating link diagram

↑ **Parent:** [Alternating link diagram](#alternating-link-diagram)

A reduced alternating [link](#link) diagram is an [alternating link diagram](#alternating-link-diagram) with no nugatory crossing. Its [Tait graph](#tait-graph) and dual have no loops, so it is an [adequate link diagram](#adequate-link-diagram). If connected, its [Jones polynomial](#jones-polynomial) breadth equals its crossing count.

// Target: module-theory.bigb

#### Adequate link diagram

↑ **Parent:** [Link diagram](#link-diagram)

A diagram is A-adequate if changing a single smoothing of its all-A state joins two different state [circles](topology.md#circle), and B-adequate analogously. It is adequate if both conditions hold. In an adequate diagram the top and bottom degree terms of the [Kauffman bracket](#kauffman-bracket) arise uniquely from these two states. Reduced alternating diagrams are adequate because their [Tait graphs](#tait-graph) and duals have no loop edges.

#### Turaev surface

↑ **Parent:** [Link diagram](#link-diagram)

Replace each crossing of a diagram by a saddle joining its A smoothing above the projection [sphere](geometry-and-topology.md#sphere) to its B smoothing below; cap the upper and lower state [circles](topology.md#circle). For a connected classical [link diagram](#link-diagram) this constructs a connected closed orientable [surface](topology.md#topological-surface). Its Euler characteristic is $s_A+s_B-c(D)$, so $s_A+s_B\leq c(D)+2$. For an alternating diagram the [surface](topology.md#topological-surface) has genus zero.

#### Tait graph

↑ **Parent:** [Link diagram](#link-diagram)

Choose a checkerboard coloring of the complementary regions of a [link diagram](#link-diagram). The Tait graph has one vertex for each black region and one edge through each crossing joining its adjacent black regions. The other coloring gives its planar dual. For a connected [alternating link diagram](#alternating-link-diagram), all-A and all-B smoothing [circles](topology.md#circle) correspond to the regions of its two checkerboard colors; one-circle smoothing states correspond to [spanning trees](combinatorics.md#spanning-tree).

#### Skein relation

↑ **Parent:** [Link diagram](#link-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skein_relation)

A skein relation relates the invariants of [link diagrams](#link-diagram) agreeing outside a disk and differing by a positive crossing, a negative crossing, and a smoothing within it. Its signs and normalization determine the particular invariant convention.

##### Oriented smoothing

↑ **Parent:** [Skein relation](#skein-relation)

The oriented smoothing replaces a crossing by two disjoint arcs whose orientations agree with the four oriented ends. It is the zero-resolution in an oriented [skein relation](#skein-relation).

#### Writhe of a link diagram

↑ **Parent:** [Link diagram](#link-diagram)

The writhe is the sum of the signs of all crossings in an oriented link diagram. It changes under the first [Reidemeister move](#reidemeister-move) and is unchanged under the second and third moves.

Diagram writhe depends on the chosen projection; averaging it over projection directions gives the geometric [writhe](#writhe).

#### Tangle

↑ **Parent:** [Link diagram](#link-diagram)

A tangle is a proper embedding of arcs and circles in a three-ball with prescribed arc endpoints on its boundary. A two-string tangle has four boundary endpoints.

##### Tangle category

↑ **Parent:** [Tangle](#tangle)

Objects are finite words of strand orientations. Morphisms are boundary-fixed ambient-isotopy classes of oriented [tangles](#tangle) in a slab, composed by stacking compatible boundary words; horizontal juxtaposition is the [tensor product](linear-algebra.md#tensor-product). Cups, caps, identity strands and crossings generate the category. Ordinary unframed isotopy includes all three [Reidemeister moves](#reidemeister-move); framed variants impose different first-move relations.

##### Mutation (knot theory)

↑ **Parent:** [Tangle](#tangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutation_(knot_theory))

A Conway mutation cuts a link along a sphere meeting it in four points, rotates the enclosed two-string tangle through $180^\circ$, and reglues it.

#### Kauffman bracket

↑ **Parent:** [Link diagram](#link-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kauffman_bracket)

The Kauffman bracket is the unoriented diagram invariant determined by resolving each crossing into its two smoothings and replacing every additional disjoint circle by the loop factor $-A^2-A^{-2}$. It is invariant under the second and third [Reidemeister moves](#reidemeister-move).

##### Kauffman bracket skein module

↑ **Parent:** [Kauffman bracket](#kauffman-bracket)

For an oriented 3-manifold, take the linear span of [isotopy](differential-geometry.md#isotopy) classes of [framed links](#framed-link), including the empty [link](#link), and impose the local bracket smoothing relation and the trivial-circle relation with factor $-A^2-A^{-2}$. Fixing framed boundary endpoints gives its relative version. Gluing manifolds or stacking cylinders induces maps between skein [modules](module-theory.md#module-mathematics); framed [isotopy](differential-geometry.md#isotopy), rather than unframed Reidemeister-I invariance, is built into this construction.

###### Relative Kauffman bracket skein module

↑ **Parent:** [Kauffman bracket skein module](#kauffman-bracket-skein-module)

The relative skein [module](module-theory.md#module-mathematics) fixes finitely many framed endpoints on the boundary of a 3-manifold and uses properly embedded framed tangles with those endpoints. Local [Kauffman bracket](#kauffman-bracket) relations are imposed away from the boundary. Gluing compatible endpoint sets composes tangles; a rectangle cylinder with n endpoints on each horizontal side gives the [Temperley-Lieb diagram algebra](#temperley-lieb-diagram-algebra).

##### Kauffman bracket breadth bound

↑ **Parent:** [Kauffman bracket](#kauffman-bracket)

A state with $k$ B smoothings has at most $s_A+k$ [circles](topology.md#circle), so its largest A exponent is at most $c(D)+2s_A-2$. The dual argument bounds the smallest exponent below by $-c(D)-2s_B+2$. For a connected [link diagram](#link-diagram), the [Turaev surface](#turaev-surface) inequality bounds the resulting breadth by $4c(D)$. For a connected [reduced alternating diagram](#reduced-alternating-link-diagram), adequacy prevents cancellation at both extremes and planar [Euler characteristic](homology.md#euler-characteristic) gives equality. A disconnected projection needs the additional term in the [Jones polynomial breadth bound for a disconnected diagram](#jones-polynomial-breadth-bound-for-a-disconnected-diagram).

###### Jones polynomial breadth bound for a disconnected diagram

↑ **Parent:** [Kauffman bracket breadth bound](#kauffman-bracket-breadth-bound)

Here $n$ is the crossing count and $k$ is the number of connected components of the planar [link diagram](#link-diagram), not necessarily the number of [link](#link) components. The all-$A$ and all-$B$ state counts satisfy $s_A+s_B\leq n+2k$, by summing the [Turaev surface](#turaev-surface) [Euler characteristic](homology.md#euler-characteristic) bound over projection components. The [Kauffman bracket breadth bound](#kauffman-bracket-breadth-bound) and $t=A^{-4}$ give the displayed bound. It is sharp for an [unlink](#unlink) diagram with $n=0$, whose [Jones polynomial](#jones-polynomial) has [breadth of a Laurent polynomial](polynomial.md#breadth-of-a-laurent-polynomial) $k-1$.

##### Temperley-Lieb diagram algebra

↑ **Parent:** [Kauffman bracket](#kauffman-bracket)

The Temperley-Lieb diagram algebra is generated by planar cap-cup [tangles](#tangle), with composition by stacking and each closed circle replaced by $\delta$. Its local relations $e_i^2=\delta e_i$ and $e_ie_{i+1}e_i=e_i$ make the second and third [Reidemeister moves](#reidemeister-move) direct algebraic identities for $R_i=A I+A^{-1}e_i$ when $\delta=-A^2-A^{-2}$.

###### Jones-Wenzl idempotent

↑ **Parent:** [Temperley-Lieb diagram algebra](#temperley-lieb-diagram-algebra)

The Jones-Wenzl [idempotent](commutative-algebra.md#idempotent) has identity-diagram coefficient one, satisfies $f_n^2=f_n$, and annihilates each adjacent cap-cup generator on either side. With $\delta=-A^2-A^{-2}$ and $\Delta_0=1$, $\Delta_1=\delta$, $\Delta_n=\delta\Delta_{n-1}-\Delta_{n-2}$, it is constructed recursively by $f_n=F-(\Delta_{n-2}/\Delta_{n-1})Fe_{n-1}F$, where $F=f_{n-1}\otimes1$. The required denominators must be nonzero. Its closed bracket trace is $\Delta_n=(-1)^n[n+1]$.

###### Jones-Wenzl partial trace

↑ **Parent:** [Jones-Wenzl idempotent](#jones-wenzl-idempotent)

Close the last strand of the projector recursion. Closing $f_{n-1}\otimes1$ gives $\delta f_{n-1}$, while closing its cap-cup correction gives $f_{n-1}$. The coefficient is $\delta-\Delta_{n-2}/\Delta_{n-1}=\Delta_n/\Delta_{n-1}$. Iteration proves $\operatorname{tr}(f_n)=\Delta_n$ and supplies the normalization needed to split the two [fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors) channels in $f_{n-1}\otimes1$.

###### Reduced Temperley-Lieb skein theory

↑ **Parent:** [Jones-Wenzl idempotent](#jones-wenzl-idempotent)

At $A=e^{\pi i/(2r)}$, $r\geq3$, the projector $f_{r-1}$ exists but its closed trace is zero. Quotient by the skein ideal generated by this projector. The surviving simple colors are $0,\ldots,r-2$, with nonzero [quantum dimensions](category-theory.md#quantum-dimension) $d_j=(-1)^j\sin((j+1)\pi/r)/\sin(\pi/r)$. This truncation prevents zero-trace channels from interfering with nondegenerate fusion and surgery normalization.

###### Jones-Wenzl color

↑ **Parent:** [Reduced Temperley-Lieb skein theory](#reduced-temperley-lieb-skein-theory)

A surviving color denotes $j$ parallel framed strands equipped with the [Jones-Wenzl idempotent](#jones-wenzl-idempotent) $f_j$. Its closed trace is its [quantum dimension](category-theory.md#quantum-dimension). The [semisimplicity of the reduced Temperley-Lieb category](#semisimplicity-of-the-reduced-temperley-lieb-category) identifies these colors with the simple objects; their [tensor products](linear-algebra.md#tensor-product) decompose according to [fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors).

###### Semisimplicity of the reduced Temperley-Lieb category

↑ **Parent:** [Reduced Temperley-Lieb skein theory](#reduced-temperley-lieb-skein-theory)

The [Jones-Wenzl idempotent](#jones-wenzl-idempotent) recursion decomposes $f_j\otimes1$ into the orthogonal $f_{j+1}$ and $f_{j-1}$ channels. The [Jones-Wenzl partial trace](#jones-wenzl-partial-trace) supplies the nonzero scalar normalizing the cap-cup channel. At the highest surviving color the $f_{r-1}$ channel is zero. Induction therefore decomposes every tensor power into the surviving colors. A planar matching between different projected colors has a turnback on the larger side and vanishes; between equal colors only the identity matching remains. Their [endomorphism](algebra.md#endomorphism) spaces are consequently one-dimensional, and the resulting finite [matrix](vector-space.md#matrix) blocks split. Taking direct sums and splitting these [idempotents](commutative-algebra.md#idempotent) produces a [semisimple category](category-theory.md#semisimple-category), supplying the complete resolutions needed in [fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors) and the [Kirby color handle-slide identity](#kirby-color-handle-slide-identity).

###### Fusion of Jones-Wenzl colors

↑ **Parent:** [Reduced Temperley-Lieb skein theory](#reduced-temperley-lieb-skein-theory)

In the reduced theory the product of colors a and b decomposes with multiplicity one into colors c satisfying $|a-b|\leq c\leq\min(a+b,2r-4-a-b)$ and $a+b+c$ even. These rules follow by iterating $1\otimes j=(j-1)\oplus(j+1)$, with color $r-1$ set to zero. The closure traces give $d_ad_b=\sum_cN_{ab}^cd_c$, and self-duality makes the multiplicities symmetric in all three colors.

###### Dimension-weighted fusion resolution

↑ **Parent:** [Fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors)

In the reduced Jones-Wenzl theory, bend a fixed self-dual color a in the mutually inverse inclusion/projection maps of $c\subset b\otimes a$, obtaining $U_c^b:b\to c\otimes a$ and $V_c^b:c\otimes a\to b$. Cyclic closure trace and straightening cups and caps give $V_c^bU_c^b=(d_c/d_b)1_b$. Completeness of the normalized maps for all b then proves the weighted resolution. The dimensions are nonzero in the reduced theory. This local identity gives the precise weight preservation in the [Kirby color handle-slide identity](#kirby-color-handle-slide-identity).

###### Hopf pairing of Jones-Wenzl colors

↑ **Parent:** [Fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors)

The full bracket of a zero-framed [Hopf link](#hopf-link) colored i and j is the displayed pairing. Its normalized [matrix](vector-space.md#matrix) is the finite sine transform with parity signs. Sine orthogonality gives $H^2=\mathcal D^2I$, where $\mathcal D^2=\sum_jd_j^2=r/(2\sin^2(\pi/r))$. Thus the pairing is nondegenerate in the reduced theory.

###### Jones-Wenzl twist eigenvalue

↑ **Parent:** [Jones-Wenzl idempotent](#jones-wenzl-idempotent)

A positive framing twist on an n-strand Jones-Wenzl cable has n positive individual curls and $n(n-1)$ braid crossings. Each curl contributes $-A^3$, and each braid crossing contributes $A$ because its turnback term annihilates the [Jones-Wenzl idempotent](#jones-wenzl-idempotent). Their product is the displayed scalar. This is the colored framing factor used in surgery invariants.

###### Bracket trace on the three-strand Temperley-Lieb algebra

↑ **Parent:** [Temperley-Lieb diagram algebra](#temperley-lieb-diagram-algebra)

Close a three-strand planar [tangle](#tangle) and evaluate its reduced [Kauffman bracket](#kauffman-bracket). The basis $1,e_1,e_2,e_1e_2,e_2e_1$ has the displayed trace values, with the last value also valid for $e_2e_1$. Writing braid generators as $A1+A^{-1}e_i$ turns knot-polynomial computations into a five-dimensional algebra calculation.

##### Bracket smoothing state

↑ **Parent:** [Kauffman bracket](#kauffman-bracket)

A bracket smoothing state chooses one of the two unoriented smoothings at every crossing of a [link diagram](#link-diagram). Its weight is $A^{a-b}\delta^{s-1}$ in the reduced [Kauffman bracket](#kauffman-bracket), where $a,b$ count the smoothing types and $s$ counts resulting circles. The all-$A$ and all-$B$ states choose the same smoothing type at every crossing.

##### Jones polynomial

↑ **Parent:** [Kauffman bracket](#kauffman-bracket)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jones_polynomial)

The Jones polynomial is obtained from the [Kauffman bracket](#kauffman-bracket) of an oriented diagram by the writhe normalization

$$
V_L(t)=(-A^3)^{-w(D)}\langle D\rangle\big|_{t=A^{-4}}.
$$

###### Jones unknot detection problem

↑ **Parent:** [Jones polynomial](#jones-polynomial)

This asks whether the [Jones polynomial](#jones-polynomial) equal to one characterizes the [unknot](#unknot) among [knots](#knot). A zero [breadth of a Laurent polynomial](polynomial.md#breadth-of-a-laurent-polynomial) makes $V_K$ a [monomial](polynomial.md#monomial); the identities $V_K(1)=1$ and $V'_K(1)=0$ then force that monomial to be one. Thus using Jones breadth as a strictly positive complexity for nontrivial [knots](#knot) requires this detection property. To prove the [derivative](calculus.md#derivative) identity, differentiate the [Jones polynomial skein relation](#jones-polynomial-skein-relation) at one for a crossing change in a [knot](#knot). Both crossed diagrams have value one, while the smoothed two-component [link](#link) has value minus two by [Jones polynomial evaluation at one](#jones-polynomial-evaluation-at-one), so $V'_{K_+}(1)=V'_{K_-}(1)$. Crossing changes reduce to the [unknot](#unknot), whose [derivative](calculus.md#derivative) is zero. The corresponding [Alexander polynomial](#alexander-polynomial) detection property is false, as nontrivial untwisted [Whitehead doubles](#whitehead-double) demonstrate. The Jones question is discussed in [research on closed four-strand braids](https://arxiv.org/abs/2402.02553).

###### Signed Jones evaluation at minus one

↑ **Parent:** [Jones polynomial](#jones-polynomial)

Use the [Conway-normalized Alexander polynomial](#conway-normalized-alexander-polynomial). Choosing $t^{1/2}=i$ in the [Jones polynomial skein relation](#jones-polynomial-skein-relation) gives $V_{L_+}(-1)-V_{L_-}(-1)=-2iV_{L_0}(-1)$. The quantities $(-1)^{\ell-1}\nabla_L(2i)$ obey the same relation, because smoothing changes the component count by one. Their [unlink](#unlink) values agree, so crossing-change induction proves equality for every [link](#link). For a [knot](#knot), the sign is one and $\nabla_K(2i)=\Delta_K(-1)$. This proves the signed identity, not only equality of [knot determinants](#knot-determinant).

###### Jones polynomial of a mirror

↑ **Parent:** [Jones polynomial](#jones-polynomial)

Reflecting a [link diagram](#link-diagram) interchanges its two bracket smoothings and negates its [writhe of a link diagram](#writhe-of-a-link-diagram). This replaces $A$ by $A^{-1}$ in the normalized [Kauffman bracket](#kauffman-bracket), hence $t$ by $t^{-1}$. A [knot](#knot) whose [Jones polynomial](#jones-polynomial) differs from its reciprocal cannot be an [amphichiral knot](#amphichiral-knot).

###### Jones polynomial evaluation at one

↑ **Parent:** [Jones polynomial](#jones-polynomial)

For a nonempty [link](#link) with $\ell$ components, the [Jones polynomial skein relation](#jones-polynomial-skein-relation) at $t=1$ makes a crossing change preserve the value. Crossing changes turn the [link](#link) into an [unlink](#unlink) with the same number of components. Repeated [Jones polynomial of a split union](#jones-polynomial-of-a-split-union) gives the formula. In particular the [Jones polynomial](#jones-polynomial) is never the zero [polynomial](polynomial.md).

###### Jones polynomial of a split union

↑ **Parent:** [Jones polynomial](#jones-polynomial)

Placing the two [link diagrams](#link-diagram) in disjoint disks keeps all state [circles](topology.md#circle) separate. The reduced [Kauffman bracket](#kauffman-bracket) therefore acquires one extra loop factor $-A^2-A^{-2}$. Correcting [writhe of a link diagram](#writhe-of-a-link-diagram) and setting $t=A^{-4}$ gives the displayed formula. It concerns a [split link](#split-link), not an arbitrary union of linked components.

###### Jones polynomial of a connected sum

↑ **Parent:** [Jones polynomial](#jones-polynomial)

For [knots](#knot), matching [bracket smoothing states](#bracket-smoothing-state) across a [connected sum of knots](#connected-sum-of-knots) joins one state [circle](topology.md#circle) from each side. Their total [circle](topology.md#circle) count is therefore the sum of the two counts minus one. The reduced [Kauffman bracket](#kauffman-bracket) state weights multiply, and [writhe of a link diagram](#writhe-of-a-link-diagram) adds, proving the formula.

###### Jones polynomial skein relation

↑ **Parent:** [Jones polynomial](#jones-polynomial)

Resolve the two crossings in a [skein relation](#skein-relation) using the [Kauffman bracket](#kauffman-bracket), then correct by the [writhe of a link diagram](#writhe-of-a-link-diagram). The other smoothing cancels, leaving the displayed coefficient of the [oriented smoothing](#oriented-smoothing). This relation and the value one on the [unknot](#unknot) determine the [Jones polynomial](#jones-polynomial): crossing changes give descending diagrams, which are [unlinks](#unlink), while the smoothing terms have fewer crossings.

###### Unreduced Jones polynomial

↑ **Parent:** [Jones polynomial](#jones-polynomial)

Use the [Kauffman bracket](#kauffman-bracket) assigning the empty diagram value $1$ and a disjoint circle factor $-A^2-A^{-2}$. Correct by the [writhe of a link diagram](#writhe-of-a-link-diagram) and substitute $t=A^{-4}$. Relative to the [Jones polynomial](#jones-polynomial) normalized to be $1$ on the [unknot](#unknot), this unreduced invariant has an additional factor $-(t^{1/2}+t^{-1/2})$. For a nonempty $l$-component [link](#link), its value at $t=1$ is $(-2)^l$.

### Torus link

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torus_link)

The torus link $T_{p,q}$ lies on an unknotted torus and winds $p$ times meridionally and $q$ times longitudinally. It has $\gcd(p,q)$ components; distinct components of the positively oriented $T_{n,n}$ have [linking number](#linking-number) one.

### Framed link

↑ **Parent:** [Link](#link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Framed_link)

A framed link is a link together with a homotopy class of nonzero normal vector field on every component. Relative to the [Seifert framing](#seifert-framing), each component framing is encoded by an integer.

#### Surface framing

↑ **Parent:** [Framed link](#framed-link)

A surface framing pushes a curve in the direction tangent to an oriented [topological surface](topology.md#topological-surface) containing it and normal to the curve. For a [two-handle](topology.md#two-handle) attached along a curve on a boundary [topological surface](topology.md#topological-surface), this specifies the attaching annulus.

#### Seifert framing

↑ **Parent:** [Framed link](#framed-link)

The Seifert framing pushes a knot in the direction tangent to a [Seifert surface](#seifert-surface) and normal to its boundary. The knot and its push-off then have [linking number](#linking-number) zero.

#### Dehn surgery on a framed link

↑ **Parent:** [Framed link](#framed-link)

Integral Dehn surgery removes a tubular neighborhood of every component and reglues a solid torus so that its meridian follows the slope specified by the framing.

The framing specifies the integer slope in this special case of [Dehn surgery](#dehn-surgery).

##### Integer surgery coefficient

↑ **Parent:** [Dehn surgery on a framed link](#dehn-surgery-on-a-framed-link)

Relative to the [meridian of a knot](#meridian-of-a-knot) $\mu$ and [Seifert longitude](#seifert-longitude) $\lambda$, an integer surgery coefficient $n$ means that the filling [meridian of a solid torus](topology.md#meridian-of-a-solid-torus) is identified with $n\mu+\lambda$.

##### Surgery trace

↑ **Parent:** [Dehn surgery on a framed link](#dehn-surgery-on-a-framed-link)

The surgery trace $W(L)$ is obtained from $B^4$ by attaching one two-handle along every component of a framed link $L\subset S^3$. Its boundary is the three-manifold produced by surgery on $L$.

###### Surgery linking matrix

↑ **Parent:** [Surgery trace](#surgery-trace)

The surgery linking matrix has the framing coefficients on its diagonal and pairwise linking numbers off the diagonal. It represents the [intersection form](homology.md#intersection-form) on the second homology of the surgery trace, presents the first homology of its boundary, and has kernel isomorphic to the boundary's second homology.

###### Kirby calculus

↑ **Parent:** [Surgery trace](#surgery-trace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kirby_calculus)

Kirby calculus changes framed-link diagrams by handle slides and creation or cancellation of standard handle pairs without changing the represented four-manifold up to diffeomorphism.

###### Jones polynomial surgery invariant

↑ **Parent:** [Kirby calculus](#kirby-calculus)

For an m-component integral framed surgery [link](#link), normalize its full colored bracket by the displayed expression, where $\sigma(L)$ is the signature of its linking [matrix](vector-space.md#matrix). The [Kirby color handle-slide identity](#kirby-color-handle-slide-identity) handles slides; $p_+p_-=\mathcal D^2$ cancels disjoint plus- or minus-one-framed unknots. [Kirby calculus](#kirby-calculus) therefore makes this an oriented 3-manifold invariant. This convention has $\tau_r(S^3)=1$.

// Target: module-theory.bigb

###### Kirby diagram

↑ **Parent:** [Kirby calculus](#kirby-calculus)

A Kirby diagram depicts a [handle decomposition](topology.md#handle-decomposition) of a four-dimensional [manifold](topology.md#topological-manifold) using a [framed link](#framed-link) for the two-handles and dotted circles for the one-handles. The framing specifies the attaching normal directions; it controls the resulting [intersection form](homology.md#intersection-form) and the boundary [Dehn surgery](#dehn-surgery).

###### Slam-dunk move

↑ **Parent:** [Kirby calculus](#kirby-calculus)

If a [meridian of a knot](#meridian-of-a-knot) component in a surgery [link](#link) links only one other component, filling it with coefficient $b\ne0$ removes it and replaces the other coefficient $a$ by $a-1/b$. This gives the negative continued-fraction chain description of rational [Dehn filling](#dehn-filling).

##### Lens space

↑ **Parent:** [Dehn surgery on a framed link](#dehn-surgery-on-a-framed-link)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lens_space)

For coprime integers $p>0$ and $q$, the lens space $L(p,q)$ is the quotient of $S^3\subset\mathbb C^2$ by $(z_1,z_2)\mapsto(e^{2\pi i/p}z_1,e^{2\pi iq/p}z_2)$. Equivalently, it is obtained by an appropriate rational surgery on the unknot.

###### Genus-one gluing model of a lens space

↑ **Parent:** [Lens space](#lens-space)

The quotient model of a [lens space](#lens-space) splits into two [solid tori](topology.md#solid-torus). In the boundary angle lattice $\mathbb Z^2+\mathbb Z(1/p,q/p)$, choose $\mu_1=(0,1)$ and $\lambda_1=(1/p,q/p)$. The other meridian is $(1,0)=-q\mu_1+p\lambda_1$. A second column completing this primitive slope to a determinant-one matrix specifies a gluing map after reversing one boundary-basis convention. Different completions differ by a meridional [Dehn twist](topology.md#dehn-twist) extending across the second solid torus, so they give the same [three-manifold](topology.md#3-manifold).

###### Oriented classification of lens spaces

↑ **Parent:** [Lens space](#lens-space)

With a consistent surgery orientation convention, $L(p,q)$ and $L(p,q')$ are orientation-preservingly related by a [homeomorphism](topology.md#homeomorphism) exactly when $q'\equiv q^{\pm1}\pmod p$. An orientation-reversing [homeomorphism](topology.md#homeomorphism) instead requires $q'\equiv-q^{\pm1}\pmod p$.

## Colored link

↑ **Parent:** [Knot theory](knot-theory.md)

A colored link assigns each component a color. In the trivial coloring all components have the same color, so a doubly slice realization uses one unknotted surface component.

### Kirby color

↑ **Parent:** [Colored link](#colored-link)

The Kirby color is the weighted sum of annular closures of the surviving [Jones-Wenzl idempotents](#jones-wenzl-idempotent) at a root of unity. Its weights are their closed bracket traces. The [fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors) gives $a\Omega=d_a\Omega$ in the annular fusion ring. Inserting the corresponding fusion resolutions along a band gives the [Kirby color handle-slide identity](#kirby-color-handle-slide-identity), the central ingredient of surgery invariance.

#### Gauss sums of Jones-Wenzl colors

↑ **Parent:** [Kirby color](#kirby-color)

These sums are the evaluations of the plus- and minus-one-framed unknots with [Kirby color](#kirby-color). Twist balancing and the fusion-dimension identity give $H(\theta_jd_j)_j=p_+(\theta_j^{-1}d_j)_j$. Conjugating this identity and using $H^2=\mathcal D^2I$ proves $p_+p_-=\mathcal D^2$, so neither stabilization factor vanishes.

##### Nonvanishing of Kirby stabilization factors

↑ **Parent:** [Gauss sums of Jones-Wenzl colors](#gauss-sums-of-jones-wenzl-colors)

Let $H$ be the real [Hopf pairing of Jones-Wenzl colors](#hopf-pairing-of-jones-wenzl-colors) [matrix](vector-space.md#matrix), $d$ the dimension vector and $T$ the diagonal [matrix](vector-space.md#matrix) of [Jones-Wenzl twist eigenvalues](#jones-wenzl-twist-eigenvalue). Twist balancing on the [fusion of Jones-Wenzl colors](#fusion-of-jones-wenzl-colors) gives $HTd=p_+T^{-1}d$, using $\sum_i d_iN_{ij}^k=d_jd_k$. Complex conjugation gives $HT^{-1}d=p_-Td$. Apply $H$ again and use finite sine orthogonality, $H^2=\mathcal D^2I$. Since $Td\ne0$, the displayed identity follows. Thus both factors used to normalize the [Jones polynomial surgery invariant](#jones-polynomial-surgery-invariant) are nonzero.

#### Kirby color handle-slide identity

↑ **Parent:** [Kirby color](#kirby-color)

The bracket of a framed [link](#link) with every surgery component colored by the [Kirby color](#kirby-color) is unchanged by a [handle slide](topology.md#handle-slide). For a fixed self-dual color a choose inclusion/projection maps $i_c:c\to b\otimes a$, $p_c:b\otimes a\to c$ with $p_ci_c=1_c$ and $\sum_ci_cp_c=1_{b\otimes a}$. Bend the a strand to form $U_c^b:b\to c\otimes a$ and $V_c^b:c\otimes a\to b$. Closing the diagrams gives $V_c^bU_c^b=(d_c/d_b)1_b$. Completeness of these dual fusion maps therefore gives $\sum_b d_bU_c^bV_c^b=d_c1_{c\otimes a}$. Resolve the strand meeting a slide band into these channels. Moving the band across the colored loop bends its maps into U and V, and this weighted identity replaces the old loop-color sum by precisely the new Kirby coefficient $d_c$. The exterior ribbon diagrams agree by [isotopy](differential-geometry.md#isotopy). Summing the sliding color with its own Kirby weight proves the full identity, including its carried band framing.

## Dehn surgery

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dehn_surgery)

[Dehn surgery](#dehn-surgery) removes tubular neighborhoods of a [link](#link) in a three-dimensional [manifold](topology.md#topological-manifold) and performs [Dehn filling](#dehn-filling) on their boundary tori with specified primitive meridian slopes. [Dehn surgery on a framed link](#dehn-surgery-on-a-framed-link) is the integral-slope special case.

### Dehn filling

↑ **Parent:** [Dehn surgery](#dehn-surgery)

Let $X$ be a three-manifold with a torus boundary component and let $\alpha$ be a primitive slope on that torus. The Dehn filling $X(\alpha)$ glues in a solid torus whose meridian is identified with $\alpha$.

#### Fundamental theorem of Dehn surgery

↑ **Parent:** [Dehn filling](#dehn-filling)

Every closed connected orientable [three-manifold](topology.md#3-manifold) is obtained by integer [Dehn surgery](#dehn-surgery) on a finite [framed link](#framed-link) in the [three-sphere](geometry-and-topology.md#three-sphere). Compare a [Heegaard splitting](topology.md#heegaard-splitting) with a standard splitting of the sphere, factor their gluing difference using the [Lickorish-Dehn theorem](topology.md#lickorish-dehn-theorem), and realize each twist by unit surgery on a distinct level of a collar of the splitting surface.

##### Unit surface-framed surgery realizes a Dehn twist

↑ **Parent:** [Fundamental theorem of Dehn surgery](#fundamental-theorem-of-dehn-surgery)

Put a simple closed curve in a surface collar and use its [surface framing](#surface-framing). Filling its deleted tubular neighborhood along $\mu\pm\lambda$ inserts one full positive or negative twist of the annulus between the collar levels. Thus surgery of coefficient $\pm1$ changes the gluing by a [Dehn twist](topology.md#dehn-twist) or its inverse. The exact sign depends on the orientations of the seam and normal direction.

#### Fiber-curve surgery

↑ **Parent:** [Dehn filling](#dehn-filling)

Let a [knot](#knot) lie in a fiber of a [mapping torus](algebraic-topology.md#mapping-torus) of an oriented [topological surface](topology.md#topological-surface). Surgery with coefficient $-1$ relative to its [surface framing](#surface-framing) replaces the monodromy by its composition with a [right-handed Dehn twist](topology.md#right-handed-dehn-twist). Coefficient $+1$ gives the inverse twist. The composition side depends on the choice of seam and time orientation; the existence of the new [fiber bundle](fiber-bundle.md) does not.

#### Rational Dehn surgery

↑ **Parent:** [Dehn filling](#dehn-filling)

For a null-homologous [knot](#knot), choose a [meridian of a knot](#meridian-of-a-knot) $\mu$ and [Seifert longitude](#seifert-longitude) $\lambda$. Rational surgery with relatively prime numerator $p$ and denominator $q$ fills the [knot exterior](#knot-exterior) along $p\mu+q\lambda$. A negative [continued fraction](number-theory.md#continued-fraction) for $p/q$ replaces this operation by integer surgery on a chain of meridians, using [slam-dunk moves](#slam-dunk-move).

#### Annulus-quotient model of Dehn filling

↑ **Parent:** [Dehn filling](#dehn-filling)

Let two parallel curves $\beta_1,\beta_2$ cut a torus boundary into annuli $A_1,A_2$, and let a slope $\alpha$ meet each $\beta_i$ once. Identifying $A_1$ with $A_2$ by an orientation-reversing map fixing their boundary and matching the two arcs of $\alpha$ produces the same manifold as the Dehn filling $X(\alpha)$. A collar of the boundary turns the quotient region into the solid torus attached by the filling.

## Fibered knot

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fibered_knot)

A fibered knot is a knot whose exterior fibers over the circle, with fiber a compact surface whose boundary is the knot longitude. Its exterior is the [mapping torus](algebraic-topology.md#mapping-torus) of the fiber monodromy.

### Homological monodromy of a genus-one fibered knot

↑ **Parent:** [Fibered knot](#fibered-knot)

For a genus-one fibered knot, the fiber is a once-punctured torus and its monodromy acts on first homology by a matrix $M\in SL_2(\mathbb Z)$. Up to a Laurent unit, the one-variable Alexander polynomial is

$$
\det(tI-M)=t^2-\operatorname{tr}(M)t+1.
$$

<h3 id="nielsen-thurston-classification">Nielsen–Thurston classification</h3>

↑ **Parent:** [Fibered knot](#fibered-knot)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nielsen–Thurston_classification)

The Nielsen–Thurston classification says that an orientation-preserving surface homeomorphism is periodic, reducible, or pseudo-Anosov. For a once-punctured torus, the three cases correspond to $|\operatorname{tr}M|<2$, $|\operatorname{tr}M|=2$, and $|\operatorname{tr}M|>2$ for its action $M\in SL_2(\mathbb Z)$ on first homology.

#### Periodic surface homeomorphism

↑ **Parent:** [Nielsen–Thurston classification](#nielsen-thurston-classification)

A periodic surface homeomorphism has a positive power equal to the identity. A mapping class is periodic when it has such a representative. Allowing motion of boundary circles is a different convention from requiring every [isotopy](differential-geometry.md#isotopy) to fix the boundary pointwise.

#### Pseudo-Anosov map

↑ **Parent:** [Nielsen–Thurston classification](#nielsen-thurston-classification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudo-Anosov_map)

A pseudo-Anosov homeomorphism preserves two transverse measured foliations and stretches one while contracting the other by the same factor greater than one. Unlike the [Anosov homeomorphism](#anosov-homeomorphism) case, the foliations may have singularities.

#### Anosov homeomorphism

↑ **Parent:** [Nielsen–Thurston classification](#nielsen-thurston-classification)

An Anosov surface homeomorphism has nonsingular invariant expanding and contracting foliations. In the closed orientable surface setting it occurs on the [torus](topology.md#torus), with a hyperbolic integral linear model.

#### Hyperbolization of a pseudo-Anosov mapping torus

↑ **Parent:** [Nielsen–Thurston classification](#nielsen-thurston-classification)

The interior of the mapping torus of a pseudo-Anosov homeomorphism of a compact surface with boundary admits a complete finite-volume hyperbolic metric. Periodic monodromy instead gives a Seifert fibered mapping torus, while reducible monodromy gives a manifold containing an essential torus.

## Seifert fibered space

↑ **Parent:** [Knot theory](knot-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seifert_fibered_space)

A Seifert fibered space is a three-manifold decomposed into circles so that every fiber has a standard fibered solid-torus neighborhood. The quotient is a two-dimensional orbifold, whose cone points correspond to exceptional fibers.

### Vertical surface in a Seifert fibered space

↑ **Parent:** [Seifert fibered space](#seifert-fibered-space)

A vertical surface is a union of [Seifert fibers](#seifert-fiber) over an arc or a closed curve in the base [orbifold](geometry-and-topology.md#orbifold). Typical connected examples are an [annulus](topology.md#annulus-mathematics) and a [torus](topology.md#torus).

### Horizontal surface in a Seifert fibered space

↑ **Parent:** [Seifert fibered space](#seifert-fibered-space)

A horizontal surface is a properly embedded [topological surface](topology.md#topological-surface) transverse to every [Seifert fiber](#seifert-fiber). Its projection to the base [orbifold](geometry-and-topology.md#orbifold) is an orbifold covering. The covering degree is its intersection number with a regular [Seifert fiber](#seifert-fiber).

### Seifert fiber

↑ **Parent:** [Seifert fibered space](#seifert-fibered-space)

A Seifert fiber is one of the circles of a [Seifert fibered space](#seifert-fibered-space). A regular fiber has a product neighborhood; an exceptional fiber has a fibered [solid torus](topology.md#solid-torus) neighborhood with multiplicity greater than one.

### Seifert fibrations of real projective 3-space

↑ **Parent:** [Seifert fibered space](#seifert-fibered-space)

The Hopf circle action on $S^3$ descends through the antipodal quotient to a free circle action on $\mathbb{RP}^3$, giving a Seifert fibration over $S^2$ with no exceptional fibers. The weighted action

$$
e^{it}(z_1,z_2)=(e^{it}z_1,e^{3it}z_2)
$$

also descends and, after dividing by its generic order-two kernel, gives a fibration over $S^2$ with one exceptional fiber of multiplicity three.

## Splice of knots

↑ **Parent:** [Knot theory](knot-theory.md)

The splice of knots $K_i\subset Y_i$ is obtained by gluing their exteriors so that the meridian of each knot is identified, up to the orientation signs, with the longitude of the other. Thus the gluing exchanges meridians and longitudes.

### Zero surgery on a connected sum as a splice

↑ **Parent:** [Splice of knots](#splice-of-knots)

Let $Y_1'=X_1(\lambda_1)$ and orient its filling core $K_1'$ so that its longitude is $\mu_1$. Then zero surgery on $K_1\mathbin\#K_2$ is the splice of $(Y_1',K_1')$ and $(Y_2,K_2)$. Cutting the connected-sum exterior along its decomposing annulus and applying the [annulus-quotient model of Dehn filling](#annulus-quotient-model-of-dehn-filling) identifies $\lambda_1$ with $\lambda_2$ and $\mu_1$ with $\mu_2$, which is exactly the splice gluing.

## Turaev torsion

↑ **Parent:** [Knot theory](knot-theory.md)

Turaev torsion is a sign-refined form of Reidemeister torsion for manifolds and chain complexes. For a knot exterior with meridian $\mu$ and first Betti number one, its group-ring normalization satisfies

$$
\tau(X_K)\doteq\frac{\Delta_K}{1-[\mu]}.
$$

The refinement resolves sign and normalization choices present in [Reidemeister torsion](algebraic-topology.md#reidemeister-torsion).

### Homology orientation

↑ **Parent:** [Turaev torsion](#turaev-torsion)

A homology orientation chooses an orientation of the real vector space $\bigoplus_iH_i(M;\mathbb R)$. It fixes the sign in refined [Turaev torsion](#turaev-torsion).

### Euler structure

↑ **Parent:** [Turaev torsion](#turaev-torsion)

An Euler structure fixes the lift ambiguity in refined [Turaev torsion](#turaev-torsion). Changing it can multiply the torsion by an element of the [first homology group](homology.md#first-homology).

### Turaev-torsion Dehn-filling formula

↑ **Parent:** [Turaev torsion](#turaev-torsion)

If filling a boundary torus along a slope produces $Y$ and the filling core represents $h\in H_1(Y)$, then, up to the standard torsion unit,

$$
\tau(Y)\doteq\frac{i_*\tau(X)}{1-h}.
$$

Equivalently, $i_*\tau(X)\doteq(1-h)\tau(Y)$.

## Satellite knot as a splice

↑ **Parent:** [Knot theory](knot-theory.md)

Let $P$ be a knot in the exterior of an unknot $U$. Splicing the exterior of a companion $C$ to the $U$-boundary of the two-component exterior exchanges their peripheral curves and leaves the $P$-boundary. Meridian filling that remaining boundary gives $S^3$, and its filling core is the satellite $P(C)$.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Surface knot](#surface-knot)
