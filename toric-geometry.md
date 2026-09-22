# Toric geometry

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toric_geometry)

Toric geometry studies algebraic varieties containing an [algebraic torus](#algebraic-torus) as a dense open subset, with the torus action extended to the whole variety. Rational polyhedral fans translate their geometry into lattice combinatorics.

**Table of contents**

- [Lattice in toric geometry](#lattice-in-toric-geometry)
  - [Basis of a toric lattice](#basis-of-a-toric-lattice)
- [Toric scheme over a base ring](#toric-scheme-over-a-base-ring)
  - [Semistable infinite chain from a toric fan](#semistable-infinite-chain-from-a-toric-fan)
    - [Cyclic formal quotient of the infinite toric chain](#cyclic-formal-quotient-of-the-infinite-toric-chain)
- [Algebraic torus](#algebraic-torus)
  - [Maximal algebraic torus](#maximal-algebraic-torus)
    - [Rational maximal torus](#rational-maximal-torus)
      - [Elliptic maximal torus](#elliptic-maximal-torus)
  - [Character lattice of an algebraic torus](#character-lattice-of-an-algebraic-torus)
    - [Algebraic torus character](#algebraic-torus-character)
  - [Cocharacter lattice of an algebraic torus](#cocharacter-lattice-of-an-algebraic-torus)
- [Fan in toric geometry](#fan-in-toric-geometry)
  - [Infinite fan in toric geometry](#infinite-fan-in-toric-geometry)
  - [Normal fan of a polytope](#normal-fan-of-a-polytope)
  - [Cone in toric geometry](#cone-in-toric-geometry)
    - [Face of a polyhedral cone](#face-of-a-polyhedral-cone)
      - [Ray of a fan](#ray-of-a-fan)
    - [Dual cone](#dual-cone)
      - [Face duality for polyhedral cones](#face-duality-for-polyhedral-cones)
      - [Affine semigroup of a rational cone](#affine-semigroup-of-a-rational-cone)
        - [Gordan lemma](#gordan-lemma)
        - [Hilbert basis of a rational cone](#hilbert-basis-of-a-rational-cone)
    - [Simplicial polyhedral cone](#simplicial-polyhedral-cone)
  - [Complete fan](#complete-fan)
    - [Star of a cone in a fan](#star-of-a-cone-in-a-fan)
    - [Simplex fan](#simplex-fan)
  - [Fan subdivision](#fan-subdivision)
    - [Star subdivision](#star-subdivision)
      - [Toric blowup along an orbit closure](#toric-blowup-along-an-orbit-closure)
      - [Toric blowup at a torus-fixed point](#toric-blowup-at-a-torus-fixed-point)
        - [Ample divisor after blowing up a torus-fixed point](#ample-divisor-after-blowing-up-a-torus-fixed-point)
        - [Blowup of affine space at the origin](#blowup-of-affine-space-at-the-origin)
      - [Toric resolution of singularities](#toric-resolution-of-singularities)
        - [Two minimal toric resolutions of a four-ray threefold cone](#two-minimal-toric-resolutions-of-a-four-ray-threefold-cone)
        - [Multiplicity descent in toric desingularization](#multiplicity-descent-in-toric-desingularization)
        - [Hirzebruch–Jung resolution](#hirzebruch-jung-resolution)
        - [Self-intersection formula for a toric surface divisor](#self-intersection-formula-for-a-toric-surface-divisor)
          - [Toric contraction of a minus-one curve](#toric-contraction-of-a-minus-one-curve)
  - [Product fan](#product-fan)
  - [Fan of the affine line](#fan-of-the-affine-line)
  - [Fan of the projective line](#fan-of-the-projective-line)
- [Toric variety](#toric-variety)
  - [Complete three-ray toric surfaces with at most one singular point](#complete-three-ray-toric-surfaces-with-at-most-one-singular-point)
  - [Toric surface](#toric-surface)
  - [Weighted projective space](#weighted-projective-space)
    - [Well-formed weighted projective space](#well-formed-weighted-projective-space)
      - [Class-group generator of a well-formed weighted projective space](#class-group-generator-of-a-well-formed-weighted-projective-space)
        - [Divisorial section ring of a well-formed weighted projective space](#divisorial-section-ring-of-a-well-formed-weighted-projective-space)
    - [Weighted projective plane](#weighted-projective-plane)
      - [Divisor class and Picard groups of a weighted projective plane](#divisor-class-and-picard-groups-of-a-weighted-projective-plane)
  - [Projective toric variety of a lattice polytope](#projective-toric-variety-of-a-lattice-polytope)
  - [Affine toric variety](#affine-toric-variety)
    - [Cyclic quotient surface singularity](#cyclic-quotient-surface-singularity)
      - [Four-ray completion criterion for a cyclic quotient surface singularity](#four-ray-completion-criterion-for-a-cyclic-quotient-surface-singularity)
    - [Dense torus of an affine toric variety](#dense-torus-of-an-affine-toric-variety)
    - [Coordinate ring of an affine toric variety](#coordinate-ring-of-an-affine-toric-variety)
    - [Diagonal cyclic quotient singularity of order three](#diagonal-cyclic-quotient-singularity-of-order-three)
  - [Orbit-cone correspondence](#orbit-cone-correspondence)
    - [Monomial support face of a toric point](#monomial-support-face-of-a-toric-point)
    - [Complement of an affine toric face chart](#complement-of-an-affine-toric-face-chart)
    - [Orbit closure in a toric variety](#orbit-closure-in-a-toric-variety)
      - [Monomial zero locus in an affine toric variety](#monomial-zero-locus-in-an-affine-toric-variety)
    - [Torus-invariance of the singular locus of a toric variety](#torus-invariance-of-the-singular-locus-of-a-toric-variety)
  - [Proper toric variety](#proper-toric-variety)
  - [Smoothness criterion for a toric variety](#smoothness-criterion-for-a-toric-variety)
  - [Hirzebruch surface](#hirzebruch-surface)
    - [Negative section of a Hirzebruch surface](#negative-section-of-a-hirzebruch-surface)
    - [Fiber class of a Hirzebruch surface](#fiber-class-of-a-hirzebruch-surface)
      - [Multiples of a fiber on the first Hirzebruch surface](#multiples-of-a-fiber-on-the-first-hirzebruch-surface)
  - [Toric morphism](#toric-morphism)
    - [No nonconstant toric morphism from the projective plane to the product of projective lines](#no-nonconstant-toric-morphism-from-the-projective-plane-to-the-product-of-projective-lines)
  - [Rational map of toric varieties from a lattice homomorphism](#rational-map-of-toric-varieties-from-a-lattice-homomorphism)
  - [Toric divisor](#toric-divisor)
    - [Principal divisor on a toric variety](#principal-divisor-on-a-toric-variety)
    - [Toric divisor class sequence](#toric-divisor-class-sequence)
    - [Lattice polytope of a toric divisor](#lattice-polytope-of-a-toric-divisor)
  - [Cox construction](#cox-construction)
    - [Toric irrelevant ideal](#toric-irrelevant-ideal)
    - [Cox ring](#cox-ring)
    - [Geometric quotient](#geometric-quotient)

## Lattice in toric geometry

↑ **Parent:** [Toric geometry](toric-geometry.md)

A toric lattice is a finite-rank [free abelian group](group-theory.md#free-abelian-group) $N$, embedded as a discrete full-rank subgroup of $N_{\mathbb R}=N\otimes_{\mathbb Z}\mathbb R$. Its dual is $M=\operatorname{Hom}(N,\mathbb Z)$. This lattice of integral vectors is distinct from an order-theoretic [lattice](mathematical-logic.md#lattice). It supplies the integral structure for [toric cones](#cone-in-toric-geometry) and their dual monomials.

### Basis of a toric lattice

↑ **Parent:** [Lattice in toric geometry](#lattice-in-toric-geometry)

A lattice basis $v_1,\ldots,v_n$ expresses each vector of the [toric lattice](#lattice-in-toric-geometry) uniquely as $\sum_i a_iv_i$ with $a_i\in\mathbb Z$. Relative to any fixed integral basis, vectors form another lattice basis exactly when their determinant is $\pm1$. A primitive vector is one whose integer span is saturated; it can be completed to such a basis by the Euclidean algorithm.

## Toric scheme over a base ring

↑ **Parent:** [Toric geometry](toric-geometry.md)

Given a dual pair of free lattices $N,M$ and a rational fan, glue $\operatorname{Spec}A[\sigma^\vee\cap M]$ over common-face charts. The monoid [rings](commutative-algebra.md#ring) are [semigroup algebras](algebra.md#semigroup-algebra). A lattice map respecting cones gives a [toric morphism](#toric-morphism). This construction works over a [commutative ring](commutative-algebra.md#commutative-ring) $A$, including $\mathbb Z$, and also for an [infinite fan in toric geometry](#infinite-fan-in-toric-geometry).

// Target: toric-geometry.bigb

### Semistable infinite chain from a toric fan

↑ **Parent:** [Toric scheme over a base ring](#toric-scheme-over-a-base-ring)

Take rays $(i,1)$ and cones generated by consecutive rays in $\mathbb Z^2$. Their dual generators $(1,-i)$ and $(-1,i+1)$ give $x_i=tq^{-i}$, $y_i=t^{-1}q^{i+1}$. Adjacent charts glue by $x_{i+1}=y_i^{-1}$, $y_{i+1}=x_i y_i^2$. The fibre $q=0$ is a chain of [projective lines](finite-group-theory.md#projective-line): each component has two affine-line charts joined by reciprocal coordinates, and consecutive components meet at one node. Inverting $q$ identifies all charts with the [multiplicative group scheme](algebraic-geometry.md#multiplicative-group-scheme) over $\mathbb Z[q,q^{-1}]$. The local node algebra is free over $\mathbb Z[q]$, with [basis](vector-space.md#basis) $1,x_i^a,y_i^b$ for $a,b\geq1$, so the morphism is flat.

// Target: toric-geometry.bigb

#### Cyclic formal quotient of the infinite toric chain

↑ **Parent:** [Semistable infinite chain from a toric fan](#semistable-infinite-chain-from-a-toric-fan)

The lattice shear $(a,b)\mapsto(a+mb,b)$ shifts the chain charts by $m$ and preserves $q$. On the dense torus it acts as $(t,q)\mapsto(q^mt,q)$. For $m\geq3$, translates of each chart of the [formal completion of a scheme](ringed-space.md#formal-completion-of-a-scheme) along $q=0$ are disjoint. Glue $m$ representative formal charts cyclically by the adjacent-chart formulas to obtain a [formal scheme](ringed-space.md#formal-scheme) quotient. The two branch opens of each chart are disjoint because $D(x_i)\cap D(y_i)=D(q)$ is empty on the formal support. The quotient fibre is an $m$-gon of [projective lines](finite-group-theory.md#projective-line), and the quotient map is locally an [isomorphism](algebra.md#isomorphism) on each translated chart. Invariant morphisms descend uniquely through this gluing.

// Target: ringed-space.bigb

## Algebraic torus

↑ **Parent:** [Toric geometry](toric-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_torus)

An algebraic torus of dimension $n$ is an algebraic group isomorphic over the base field to $(\mathbb G_m)^n$. Its character and cocharacter lattices are dual free abelian groups $M$ and $N$.

### Maximal algebraic torus

↑ **Parent:** [Algebraic torus](#algebraic-torus)

A maximal algebraic torus is an [algebraic torus](#algebraic-torus) maximal among the tori contained in an [algebraic group](algebraic-geometry.md#algebraic-group). In a connected [reductive algebraic group](lie-theory.md#reductive-group), all maximal algebraic tori are conjugate. A [Borel subgroup](lie-theory.md#borel-subgroup) contains maximal algebraic tori, and its [unipotent radical](lie-theory.md#unipotent-radical) gives a decomposition $B=T\ltimes U$.

#### Rational maximal torus

↑ **Parent:** [Maximal algebraic torus](#maximal-algebraic-torus)

A [maximal algebraic torus](#maximal-algebraic-torus) $T$ is rational for $F$ when $F(T)=T$. Rationality does not require every point of $T$ to be fixed: the finite group $T^F$ is its rational-point group. Similarly a rational [Borel subgroup](lie-theory.md#borel-subgroup) or [parabolic subgroup](lie-theory.md#parabolic-subgroup) means an $F$-stable algebraic subgroup.

##### Elliptic maximal torus

↑ **Parent:** [Rational maximal torus](#rational-maximal-torus)

A [rational maximal torus](#rational-maximal-torus) is elliptic when it is contained in no proper rational [parabolic subgroup](lie-theory.md#parabolic-subgroup). This definition allows the split central torus of the ambient group; an absolute absence of every split subtorus is not the right condition when the centre is nontrivial.

### Character lattice of an algebraic torus

↑ **Parent:** [Algebraic torus](#algebraic-torus)

The character lattice $M=\operatorname{Hom}(T,\mathbb G_m)$ of an [algebraic torus](#algebraic-torus) is the free abelian group of algebraic group homomorphisms from $T$ to the multiplicative group.

#### Algebraic torus character

↑ **Parent:** [Character lattice of an algebraic torus](#character-lattice-of-an-algebraic-torus)

An algebraic torus character is a morphism of algebraic groups $T\to\mathbb G_m$. For a split torus with character lattice $M$, these are precisely the Laurent monomials $\chi^m$, with $\chi^{m+m'}=\chi^m\chi^{m'}$.

// Target: algebra.bigb

### Cocharacter lattice of an algebraic torus

↑ **Parent:** [Algebraic torus](#algebraic-torus)

The cocharacter lattice $N=\operatorname{Hom}(\mathbb G_m,T)$ is dual to the [character lattice of an algebraic torus](#character-lattice-of-an-algebraic-torus) under composition:

$$
\langle m,n\rangle\in\operatorname{Hom}(\mathbb G_m,\mathbb G_m)\cong\mathbb Z.
$$

## Fan in toric geometry

↑ **Parent:** [Toric geometry](toric-geometry.md)

A [fan in toric geometry](#fan-in-toric-geometry) is a finite collection of rational strongly convex [cones in toric geometry](#cone-in-toric-geometry) in a real [vector space](vector-space.md) with a [lattice](mathematical-logic.md#lattice), closed under taking [faces of a polyhedral cone](#face-of-a-polyhedral-cone), such that the intersection of two cones is a face of each. A fan determines a [toric variety](#toric-variety).

A fan $\Sigma$ in $N_{\mathbb R}$ is a finite collection of strictly convex rational polyhedral cones closed under taking faces, such that the intersection of two cones is a face of each.

### Infinite fan in toric geometry

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

An infinite rational fan allows infinitely many [cones in toric geometry](#cone-in-toric-geometry) while retaining the face and intersection axioms of a [fan in toric geometry](#fan-in-toric-geometry). Gluing its affine monoid charts constructs a possibly non-quasi-compact [toric scheme over a base ring](#toric-scheme-over-a-base-ring). Finiteness of the collection is unnecessary for the chart gluing, though it is needed for finite-type conclusions.

// Target: toric-geometry.bigb

### Normal fan of a polytope

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

The normal cone of a face $F$ of a polytope consists of linear functionals whose minimum is attained on all of $F$. These cones form the inward normal fan, complete in the dual of the polytope's affine span. For a full-dimensional [lattice polytope](mathematical-optimization.md#lattice-polytope), it is a complete rational fan in the full dual space.

// Target: geometry-and-topology.bigb

### Cone in toric geometry

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

A [cone in toric geometry](#cone-in-toric-geometry) is a [convex cone](mathematical-optimization.md#convex-cone) generated by finitely many [lattice](mathematical-logic.md#lattice) vectors and containing no nonzero [linear subspace](vector-space.md#vector-subspace). Such cones are the pieces of a [fan in toric geometry](#fan-in-toric-geometry).

A cone in toric geometry is the nonnegative real span of finitely many lattice vectors. It is rational when those generators lie in a lattice and strictly convex when it contains no nonzero linear subspace.

#### Face of a polyhedral cone

↑ **Parent:** [Cone in toric geometry](#cone-in-toric-geometry)

A face of a polyhedral cone $C$ is $C\cap\ker\ell$ for a linear functional nonnegative on $C$. Every [convex face](mathematical-optimization.md#face-of-a-convex-set) of a polyhedral cone is exposed in this way. Faces include the whole cone and its lineality space, and are closed under intersection.

// Target: geometry-and-topology.bigb

##### Ray of a fan

↑ **Parent:** [Face of a polyhedral cone](#face-of-a-polyhedral-cone)

A [ray of a fan](#ray-of-a-fan) is a one-dimensional cone in a [fan in toric geometry](#fan-in-toric-geometry). It has the form $\mathbb R_{\geq0}v$, where $v$ is a primitive [lattice](mathematical-logic.md#lattice) vector, and occurs as a [face of a polyhedral cone](#face-of-a-polyhedral-cone).

A ray of a fan is a one-dimensional cone. It has a unique primitive lattice generator $v_\rho$ pointing along it.

#### Dual cone

↑ **Parent:** [Cone in toric geometry](#cone-in-toric-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_cone)

For a cone $\sigma\subseteq N_{\mathbb R}$, its dual cone is

$$
\sigma^\vee=\{m\in M_{\mathbb R}:\langle m,v\rangle\geq0\text{ for all }v\in\sigma\}.
$$

##### Face duality for polyhedral cones

↑ **Parent:** [Dual cone](#dual-cone)

For a closed polyhedral cone $C$, the maps $\tau\mapsto C^\vee\cap\tau^\perp$ and $\nu\mapsto C\cap\nu^\perp$ give inverse order-reversing bijections on faces. Choose a exposing functional in the relative interior of the dual face. The bipolar identity and an exposing functional for the original face show that applying the maps twice returns that face.

// Target: geometry-and-topology.bigb

##### Affine semigroup of a rational cone

↑ **Parent:** [Dual cone](#dual-cone)

For a rational cone $\sigma$, the lattice points $\sigma^\vee\cap M$ form a finitely generated additive monoid.

###### Gordan lemma

↑ **Parent:** [Affine semigroup of a rational cone](#affine-semigroup-of-a-rational-cone)

The lattice points of a rational polyhedral cone form a finitely generated additive monoid. Choose lattice generators for the cone. Subtracting integer parts of nonnegative coefficients leaves a lattice point in their bounded fundamental parallelepiped; its finitely many lattice points, together with the chosen generators, generate the monoid. This supplies finite generation of the [coordinate ring of an affine toric variety](#coordinate-ring-of-an-affine-toric-variety).

// Target: geometry-and-topology.bigb

###### Hilbert basis of a rational cone

↑ **Parent:** [Affine semigroup of a rational cone](#affine-semigroup-of-a-rational-cone)

The Hilbert basis is the unique minimal generating set of the additive monoid of lattice points in a pointed rational cone.

#### Simplicial polyhedral cone

↑ **Parent:** [Cone in toric geometry](#cone-in-toric-geometry)

A polyhedral cone is simplicial when its primitive ray generators are linearly independent. A smooth cone in a lattice must be simplicial, but simpliciality alone does not make its ray generators part of a lattice basis.

### Complete fan

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

A fan is complete when the union of all its cones is the whole ambient real vector space. A [toric variety](#toric-variety) is proper exactly when its fan is complete.

#### Star of a cone in a fan

↑ **Parent:** [Complete fan](#complete-fan)

For a cone $\tau\in\Sigma$, its star is the fan in the quotient by $\operatorname{span}(\tau)$ formed from the images of all cones $\sigma$ containing $\tau$ as a face.

#### Simplex fan

↑ **Parent:** [Complete fan](#complete-fan)

In dimension $d$, the fan whose rays are generated by $e_1,\ldots,e_d,-\sum_ie_i$ and whose cones are generated by proper subsets of those rays is complete. It is the fan of [projective space](projective-space.md) $\mathbb P^d$.

### Fan subdivision

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

A subdivision of a fan replaces its cones by smaller cones with the same support and compatible intersections. It induces a proper birational [toric morphism](#toric-morphism).

#### Star subdivision

↑ **Parent:** [Fan subdivision](#fan-subdivision)

This operation is a [fan subdivision](#fan-subdivision). A star subdivision inserts a ray through a lattice point in a cone and subdivides every cone containing that point. It induces a proper birational [toric morphism](#toric-morphism).

##### Toric blowup along an orbit closure

↑ **Parent:** [Star subdivision](#star-subdivision)

On a smooth [toric variety](#toric-variety), the [blowup](algebraic-geometry.md#blowing-up-algebraic-geometry) along the [orbit closure in a toric variety](#orbit-closure-in-a-toric-variety) of a cone generated by part of a [lattice basis](#basis-of-a-toric-lattice) $v_1,\ldots,v_k$ is the [star subdivision](#star-subdivision) at their sum. Locally the center has ideal $(x_1,\ldots,x_k)$; its blowup charts adjoin $x_j/x_i$, producing precisely these subdivided cones. This extends the [toric blowup at a torus-fixed point](#toric-blowup-at-a-torus-fixed-point) to invariant centers of any codimension.

##### Toric blowup at a torus-fixed point

↑ **Parent:** [Star subdivision](#star-subdivision)

If a smooth maximal cone is generated by a lattice basis $e_1,\ldots,e_n$, its star subdivision through $e_1+\cdots+e_n$ is the fan of the blowup at the corresponding torus-fixed point.

###### Ample divisor after blowing up a torus-fixed point

↑ **Parent:** [Toric blowup at a torus-fixed point](#toric-blowup-at-a-torus-fixed-point)

For an ample invariant divisor $D$ and the blowup $\pi$ of a torus-fixed smooth point in dimension at least two, $c\pi^*D-E$ is ample for sufficiently large integers $c$. In the subdivided cone, its local characters are $cm_\sigma+u_i$, where $u_i$ is dual to the omitted ray generator. The new strict inequalities have gap one on the omitted ray and grow linearly with $c$ elsewhere, proving the claim by the [toric ampleness criterion](cartier-divisor.md#toric-ampleness-criterion).

###### Blowup of affine space at the origin

↑ **Parent:** [Toric blowup at a torus-fixed point](#toric-blowup-at-a-torus-fixed-point)

The blowup of $\mathbb A^n$ at the origin is the total space of the tautological line bundle $\mathcal O_{\mathbb P^{n-1}}(-1)$. Its exceptional divisor is the zero section $\mathbb P^{n-1}$, and projection to the direction of a line gives the bundle map to $\mathbb P^{n-1}$.

##### Toric resolution of singularities

↑ **Parent:** [Star subdivision](#star-subdivision)

A toric resolution of singularities is obtained by subdividing a fan until every cone is generated by part of a lattice basis. The resulting smooth toric variety maps properly and birationally to the original one.

###### Two minimal toric resolutions of a four-ray threefold cone

↑ **Parent:** [Toric resolution of singularities](#toric-resolution-of-singularities)

For this [toric cone](#cone-in-toric-geometry), one smooth [fan subdivision](#fan-subdivision) has maximal cones $abc,acd$ and no exceptional divisors. Another has $abd,bce,cde,dbe$, with $e=a+c=(b+c+d)/2$. Its only exceptional divisor is a [projective plane](projective-space.md#projective-plane), since the quotient fan at $e$ has the three rays $\bar b,\bar c,\bar d$ with sum zero and unimodular neighboring cones. Both subdivisions admit no proper smooth coarsening. Their common smooth refinement is obtained from the first by adding $e$ in $ac$ and then $w=a+e$ in $ae$, and from the second by adding $w=b+d$ in $bd$. Each step is a [toric blowup along an orbit closure](#toric-blowup-along-an-orbit-closure).

###### Multiplicity descent in toric desingularization

↑ **Parent:** [Toric resolution of singularities](#toric-resolution-of-singularities)

First make a [toric fan](#fan-in-toric-geometry) simplicial by compatible rational subdivisions. In a nonregular simplicial cone, choose a nonregular face minimal under inclusion. Its half-open fundamental parallelepiped contains a nonzero point of the [toric lattice](#lattice-in-toric-geometry) $w=\sum_i\alpha_iv_i$, with every $0<\alpha_i<1$: a zero coefficient would put it in a regular proper face and force all coefficients to be integers. A [star subdivision](#star-subdivision) at the primitive point on this ray replaces a generator by $w$ and multiplies the affected lattice determinant by a number strictly between zero and one. The maximum multiplicity and the number of maximal cones realizing it decrease lexicographically, giving a finite [toric resolution of singularities](#toric-resolution-of-singularities).

<h6 id="hirzebruch-jung-resolution">Hirzebruch–Jung resolution</h6>

↑ **Parent:** [Toric resolution of singularities](#toric-resolution-of-singularities)

For the [cyclic quotient surface singularity](#cyclic-quotient-surface-singularity) $\frac1r(1,q)$, expand $r/q=[b_1,\ldots,b_s]^-$ with $b_i\ge2$. In the quotient lattice, start with $v_0=(0,1)$, $v_1=(1,q)/r$, and set $v_{i+1}=b_iv_i-v_{i-1}$. The last vector is $(1,0)$, each consecutive pair is a lattice basis, and subdivision by these rays is a resolution. Its exceptional chain has self-intersections $-b_i$. None is a minus-one curve, so the resolution is minimal. All coefficients are two exactly for $q=r-1$.

// Target: geometry-and-topology.bigb

###### Self-intersection formula for a toric surface divisor

↑ **Parent:** [Toric resolution of singularities](#toric-resolution-of-singularities)

In a smooth complete toric surface, if consecutive primitive rays are $u,w,v$ and $u+v=aw$, then the invariant divisor $D_w$ has $D_w^2=-a$. A ray introduced inside a cone by a smooth subdivision has $a>0$, so its divisor has negative self-intersection.

###### Toric contraction of a minus-one curve

↑ **Parent:** [Self-intersection formula for a toric surface divisor](#self-intersection-formula-for-a-toric-surface-divisor)

A compact invariant curve with consecutive rays $u,v,w$ on a smooth toric surface contracts torically to a smooth point exactly when $u+w=v$, equivalently when its self-intersection is $-1$. Deleting $v$ then reverses a [toric blowup at a torus-fixed point](#toric-blowup-at-a-torus-fixed-point).

// Target: geometry-and-topology.bigb

### Product fan

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

The product of fans $\Sigma_1\subseteq N_{1,\mathbb R}$ and $\Sigma_2\subseteq N_{2,\mathbb R}$ consists of the cones $\sigma_1\times\sigma_2$. Its [toric variety](#toric-variety) is $X_{\Sigma_1}\times X_{\Sigma_2}$.

### Fan of the affine line

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

The fan $\{0,\mathbb R_{\geq0}\}$ in $\mathbb R$ defines the affine line $\mathbb A^1$.

### Fan of the projective line

↑ **Parent:** [Fan in toric geometry](#fan-in-toric-geometry)

The fan $\{0,\mathbb R_{\geq0},\mathbb R_{\leq0}\}$ defines the [complex projective line](algebraic-topology.md#complex-projective-line) $\mathbb P^1$.

## Toric variety

↑ **Parent:** [Toric geometry](toric-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toric_variety)

A toric variety $X_\Sigma$ is obtained by gluing the affine toric varieties associated with the cones of a fan $\Sigma$. It contains an [algebraic torus](#algebraic-torus) as a dense open orbit.

### Complete three-ray toric surfaces with at most one singular point

↑ **Parent:** [Toric variety](#toric-variety)

Two neighboring smooth cones can be normalized so that the three rays are $(1,0),(0,1),(-1,-r)$, with $r\geq1$. Completeness forces the negative sign and their primitive relation has weights $(1,r,1)$. Thus these surfaces are precisely the [weighted projective planes](#weighted-projective-plane) $\mathbb P(1,1,r)$. For $r=1$ the surface is the [projective plane](projective-space.md#projective-plane); for $r>1$ its unique singularity is the [cyclic quotient surface singularity](#cyclic-quotient-surface-singularity) $\frac1r(1,1)$.

### Toric surface

↑ **Parent:** [Toric variety](#toric-variety)

A toric surface is a two-dimensional normal [toric variety](#toric-variety), described by a [toric fan](#fan-in-toric-geometry) in a rank-two [toric lattice](#lattice-in-toric-geometry). Primitive consecutive rays bound its affine charts; those charts are smooth exactly when the two ray generators form a [lattice basis](#basis-of-a-toric-lattice).

### Weighted projective space

↑ **Parent:** [Toric variety](#toric-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weighted_projective_space)

The weighted projective space is $\operatorname{Proj}k[z_0,\ldots,z_n]$ with $\deg z_i=w_i>0$. Over an algebraically closed field of characteristic zero it is the [geometric quotient](#geometric-quotient) of punctured affine space by $\lambda\cdot z_i=\lambda^{w_i}z_i$. For well-formed weights, these weights also grade its [Cox ring](#cox-ring).

// Target: geometry-and-topology.bigb

#### Well-formed weighted projective space

↑ **Parent:** [Weighted projective space](#weighted-projective-space)

A [weighted projective space](#weighted-projective-space) with positive integer weights $q_0,\ldots,q_n$ is well-formed when the greatest common divisor of the weights with any one weight omitted is one. The quotient [toric lattice](#lattice-in-toric-geometry) $N=\mathbb Z^{n+1}/\mathbb Z(q_0,\ldots,q_n)$ is free and the images of the coordinate vectors are primitive [toric rays](#ray-of-a-fan). Its fan contains the cones on all proper subsets of these rays.

##### Class-group generator of a well-formed weighted projective space

↑ **Parent:** [Well-formed weighted projective space](#well-formed-weighted-projective-space)

The [toric divisor class sequence](#toric-divisor-class-sequence) identifies the [divisor class group](algebraic-geometry.md#divisor-class-group) with $\mathbb Z$ via $(a_i)\mapsto\sum q_ia_i$. Choose integers $a_i$ with $\sum q_ia_i=1$; then $D=\sum a_iF_i$ represents its positive generator $H$. This is an ample [Q-Cartier divisor](algebraic-geometry.md#q-cartier-divisor): for $\ell=\operatorname{lcm}(q_i)$ the local Cartier data of $\ell D$ on the chart omitting ray $j$ is $m_j=(\ell/q_j)e_j-\ell(a_i)$, which satisfies the strict [toric ampleness criterion](cartier-divisor.md#toric-ampleness-criterion). The generator need not itself be a [Cartier divisor](cartier-divisor.md); for example the positive generator on $\mathbb P(1,1,2)$ has Cartier index two.

###### Divisorial section ring of a well-formed weighted projective space

↑ **Parent:** [Class-group generator of a well-formed weighted projective space](#class-group-generator-of-a-well-formed-weighted-projective-space)

With $D=\sum a_iF_i$ and $\sum q_ia_i=1$, the dual [toric lattice](#lattice-in-toric-geometry) is $M=\{m\in\mathbb Z^{n+1}:\sum q_im_i=0\}$. A [torus character](fourier-analysis.md#characters-of-a-real-torus) $\chi^m$ is a section of $rD$ exactly when $b_i=m_i+ra_i\geq0$. The vector $b$ has weighted degree $\sum q_ib_i=r$, and the correspondence $\chi^m\mapsto X^b$ is bijective on bases in every degree and respects multiplication. This gives the displayed graded-ring isomorphism, even when $D$ is a non-Cartier [Weil divisor](algebraic-geometry.md#weil-divisor).

#### Weighted projective plane

↑ **Parent:** [Weighted projective space](#weighted-projective-space)

This is a two-dimensional [weighted projective space](#weighted-projective-space). The weighted projective plane $\mathbb P(a,b,c)$ is the quotient of $\mathbb A^3\setminus\{0\}$ by $\lambda\mathbin{\cdot}(x,y,z)=(\lambda^ax,\lambda^by,\lambda^cz)$. It is generally singular but is a proper toric surface.

##### Divisor class and Picard groups of a weighted projective plane

↑ **Parent:** [Weighted projective plane](#weighted-projective-plane)

For coprime positive integers $a,b$,

$$
\operatorname{Cl}(\mathbb P(1,a,b))\cong\mathbb Z,
\qquad
\operatorname{Pic}(\mathbb P(1,a,b))\cong\mathbb Z,
$$

and the natural map identifies the Picard group with $ab\mathbb Z$ inside the class group. The plane is smooth exactly when $a=b=1$.

### Projective toric variety of a lattice polytope

↑ **Parent:** [Toric variety](#toric-variety)

For a [lattice polytope](mathematical-optimization.md#lattice-polytope) $\Delta$, form the semigroup of lattice points $(m,l)$ with $l\ge0$ and $m\in l\Delta$, using only $(0,0)$ in degree zero. Its semigroup algebra is graded by $l$, and its [Proj construction](ringed-space.md#proj-construction) gives $\mathbb P_\Delta$. The chart at a lattice vertex $v$ is $\operatorname{Spec}k[\operatorname{cone}(\Delta-v)\cap M]$; these charts give the [normal fan of a polytope](#normal-fan-of-a-polytope) construction. For a polytope of smaller dimension, use its intrinsic affine lattice after translation.

// Target: geometry-and-topology.bigb

### Affine toric variety

↑ **Parent:** [Toric variety](#toric-variety)

For a rational strongly convex cone $\sigma\subseteq N_{\mathbb R}$, the affine toric variety is

$$
U_\sigma=\operatorname{Spec}\mathbb C[\sigma^\vee\cap M].
$$

#### Cyclic quotient surface singularity

↑ **Parent:** [Affine toric variety](#affine-toric-variety)

For $r>1$ and $\gcd(r,q)=1$, the quotient of $\mathbb A^2$ by $(x,y)\mapsto(\zeta x,\zeta^q y)$ is a cyclic quotient surface singularity. Its toric model uses the first-quadrant cone in $\mathbb Z^2+\mathbb Z(1,q)/r$. Conversely, every singular full-dimensional affine toric surface over an algebraically closed field of characteristic zero has this form. Smooth cones and cones with a torus factor require separate treatment.

// Target: geometry-and-topology.bigb

##### Four-ray completion criterion for a cyclic quotient surface singularity

↑ **Parent:** [Cyclic quotient surface singularity](#cyclic-quotient-surface-singularity)

The [cyclic quotient surface singularity](#cyclic-quotient-surface-singularity) $\frac1r(q,1)$ is the only singular point of a complete four-ray [toric surface](#toric-surface) exactly under the displayed condition. Normalize the three smooth cones to the consecutive rays $(a,-1),(1,0),(0,1),(-1,b)$. The singular cone has determinant $1-ab=r$, so $ab=1-r$. In the basis $(-1,b),(0,-1)$, its other generator is $-a(-1,b)+r(0,-1)$, giving quotient parameter $a\bmod r$. Thus $a=\pm s$ for a positive divisor $s$ of $r-1$. Conversely these rays construct the surface. Exchanging the two axes replaces $q$ by $q^{-1}$; replacing a factor by its complementary factor preserves the criterion under this equivalence.

#### Dense torus of an affine toric variety

↑ **Parent:** [Affine toric variety](#affine-toric-variety)

For a strongly convex rational cone $\sigma$, the group generated by $S=\sigma^\vee\cap M$ is $M$. Inverting its finitely many monomial generators gives $k[M]$, so $\operatorname{Spec}k[M]$ is a dense open [algebraic torus](#algebraic-torus) in $\operatorname{Spec}k[S]$. The map $\chi^m\mapsto\chi^m\otimes\chi^m$ extends torus multiplication to the entire variety.

// Target: geometry-and-topology.bigb

#### Coordinate ring of an affine toric variety

↑ **Parent:** [Affine toric variety](#affine-toric-variety)

The coordinate ring of $U_\sigma$ is generated by the characters $\chi^m$ for lattice points $m\in\sigma^\vee\cap M$, with multiplication $\chi^m\chi^{m'}=\chi^{m+m'}$.

#### Diagonal cyclic quotient singularity of order three

↑ **Parent:** [Affine toric variety](#affine-toric-variety)

The cone generated by $(1,0)$ and $(-1,3)$ has semigroup ring

$$
\mathbb C[t_2,t_1t_2,t_1^2t_2,t_1^3t_2]
\cong\mathbb C[x,y]^{\mu_3},
$$

where $\mu_3$ acts diagonally with weight one. Inserting the ray through $(0,1)$ resolves it, with one exceptional curve of self-intersection $-3$.

### Orbit-cone correspondence

↑ **Parent:** [Toric variety](#toric-variety)

The orbit-cone correspondence assigns to every cone $\sigma\in\Sigma$ a torus orbit of codimension $\dim\sigma$. In particular, maximal cones correspond to torus-fixed points.

#### Monomial support face of a toric point

↑ **Parent:** [Orbit-cone correspondence](#orbit-cone-correspondence)

At a point $p$ of $\operatorname{Spec}k[C\cap M]$, the exponents $m$ with $\chi^m(p)\ne0$ form a [semigroup face](algebra.md#face-of-an-additive-monoid). They are the lattice points of one face of $C$. Points with that same support face form a single algebraic torus orbit: their nonzero monomial evaluations extend to homomorphisms from the lattice generated by the face into $k^*$, and restriction from the full torus is surjective.

// Target: mathematical-optimization.bigb

#### Complement of an affine toric face chart

↑ **Parent:** [Orbit-cone correspondence](#orbit-cone-correspondence)

If $\tau\preceq\sigma$, choose $m\in\sigma^\vee\cap M$ with $\tau=\sigma\cap m^\perp$. Then $U_\tau=D(\chi^m)\subset U_\sigma$. Its complement is the union of orbit closures indexed by faces of $\sigma$ that are not faces of $\tau$.

// Target: geometry-and-topology.bigb

#### Orbit closure in a toric variety

↑ **Parent:** [Orbit-cone correspondence](#orbit-cone-correspondence)

For $\sigma\in\Sigma$, the closure of its torus orbit is

$$
V(\sigma)=\overline{O(\sigma)}
=\bigcup_{\tau\supseteq\sigma}O(\tau).
$$

Thus orbit-closure inclusion reverses face inclusion.

##### Monomial zero locus in an affine toric variety

↑ **Parent:** [Orbit closure in a toric variety](#orbit-closure-in-a-toric-variety)

On the orbit of a face $\tau\preceq\sigma$, the monomial $\chi^\mu$, with $\mu\in\sigma^\vee\cap M$, vanishes exactly when $\mu\notin\tau^\perp$. Its reduced zero locus is consequently the union of those orbit closures. The principal subscheme need not be reduced: $V(x^2)$ and $V(x)$ have the same support but different ideals.

// Target: geometry-and-topology.bigb

#### Torus-invariance of the singular locus of a toric variety

↑ **Parent:** [Orbit-cone correspondence](#orbit-cone-correspondence)

The action of the [algebraic torus](#algebraic-torus) on a [toric variety](#toric-variety) is by automorphisms, and automorphisms preserve regular local rings. The smooth and singular loci are therefore unions of torus orbits.

### Proper toric variety

↑ **Parent:** [Toric variety](#toric-variety)

A toric variety is proper exactly when its [fan](#fan-in-toric-geometry) is [complete](#complete-fan).

### Smoothness criterion for a toric variety

↑ **Parent:** [Toric variety](#toric-variety)

An affine toric chart associated with a cone $\sigma$ is smooth exactly when the primitive ray generators of $\sigma$ extend to a lattice basis. For a two-dimensional cone generated by $u,v$, this is equivalent to $|\det(u,v)|=1$.

### Hirzebruch surface

↑ **Parent:** [Toric variety](#toric-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hirzebruch_surface)

The Hirzebruch surface is the ruled surface

$$
\mathbb F_k=\mathbb P_{\mathbb P^1}(\mathcal O\oplus\mathcal O(k)).
$$

It is the smooth toric surface with rays $(1,0),(0,1),(-1,k),(0,-1)$.

#### Negative section of a Hirzebruch surface

↑ **Parent:** [Hirzebruch surface](#hirzebruch-surface)

The negative section $S\subset\mathbb F_k$ has self-intersection $S^2=-k$. Together with a fiber $F$ of the ruling, it generates the Picard group and satisfies $F^2=0$ and $S\mathbin{\cdot}F=1$.

#### Fiber class of a Hirzebruch surface

↑ **Parent:** [Hirzebruch surface](#hirzebruch-surface)

The fiber class $F$ is the divisor class of a fiber of $\mathbb F_k\to\mathbb P^1$. Its complete linear system gives the ruling.

##### Multiples of a fiber on the first Hirzebruch surface

↑ **Parent:** [Fiber class of a Hirzebruch surface](#fiber-class-of-a-hirzebruch-surface)

For a toric fiber divisor $F$ on $\mathbb F_1$,

$$
h^0(\mathbb F_1,\mathcal O(kF))=
\begin{cases}k+1,&k\geq0,\\0,&k<0.
\end{cases}
$$

The bundles $\mathcal O(kF)$ are basepoint-free for $k\geq0$ but never ample, since $F^2=0$.

### Toric morphism

↑ **Parent:** [Toric variety](#toric-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toric_morphism)

A lattice homomorphism that maps each cone of one fan into a cone of another induces an equivariant morphism of the corresponding toric varieties.

#### No nonconstant toric morphism from the projective plane to the product of projective lines

↑ **Parent:** [Toric morphism](#toric-morphism)

Every fan morphism from the fan of $\mathbb P^2$ to the fan of $\mathbb P^1$ is zero: the three source ray images sum to zero, while each adjacent pair must lie in one half-line. Composing a fan morphism to the product fan of $\mathbb P^1\times\mathbb P^1$ with both projections therefore makes it zero.

### Rational map of toric varieties from a lattice homomorphism

↑ **Parent:** [Toric variety](#toric-variety)

A lattice homomorphism always gives a homomorphism of dense algebraic tori and hence a rational map of their toric compactifications. It extends across the orbit of a source cone exactly when that cone maps into one cone of the target fan.

### Toric divisor

↑ **Parent:** [Toric variety](#toric-variety)

Each ray $\rho$ of a fan determines a torus-invariant prime divisor $D_\rho$. Integer combinations of these divisors encode line bundles and maps from a toric variety.

#### Principal divisor on a toric variety

↑ **Parent:** [Toric divisor](#toric-divisor)

For a character $\chi^m$ of the dense torus,

$$
\operatorname{div}(\chi^m)=\sum_\rho\langle m,v_\rho\rangle D_\rho.
$$

#### Toric divisor class sequence

↑ **Parent:** [Toric divisor](#toric-divisor)

For a toric variety whose rays span $N_{\mathbb R}$, the divisor class group is computed by

$$
0\longrightarrow M\longrightarrow\mathbb Z^{\Sigma(1)}
\longrightarrow\operatorname{Cl}(X_\Sigma)\longrightarrow0,
$$

where $m\mapsto(\langle m,v_\rho\rangle)_\rho$.

#### Lattice polytope of a toric divisor

↑ **Parent:** [Toric divisor](#toric-divisor)

For an invariant divisor $D=\sum_\rho a_\rho D_\rho$, its lattice polytope is

$$
P_D=\{m\in M_{\mathbb R}:\langle m,v_\rho\rangle\geq-a_\rho\text{ for every }\rho\}.
$$

Its lattice points index torus-character sections of the associated [line bundle](ringed-space.md#line-bundle).

### Cox construction

↑ **Parent:** [Toric variety](#toric-variety)

The Cox construction presents a toric variety as a quotient of an open subset of affine space by a quasitorus determined by its divisor class group.

#### Toric irrelevant ideal

↑ **Parent:** [Cox construction](#cox-construction)

In the [Cox ring](#cox-ring) $S=k[z_\rho]$, the irrelevant ideal is generated by $\prod_{\rho\notin\sigma(1)}z_\rho$ as $\sigma$ runs over maximal cones. The [Cox construction](#cox-construction) takes the quotient of $\operatorname{Spec}S\setminus V(B_\Sigma)$ by the diagonalizable group whose character group is the divisor class group.

// Target: geometry-and-topology.bigb

#### Cox ring

↑ **Parent:** [Cox construction](#cox-construction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cox_ring)

The Cox ring of a toric variety is the polynomial ring with one variable $x_\rho$ for each ray, graded by the divisor class group through $\deg x_\rho=[D_\rho]$.

#### Geometric quotient

↑ **Parent:** [Cox construction](#cox-construction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_quotient)

A geometric quotient $X\to X/G$ has fibers equal to group orbits and carries precisely the invariant regular functions locally on the quotient.

## ↑ Ancestors (5)

1. [Algebraic geometry](algebraic-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
