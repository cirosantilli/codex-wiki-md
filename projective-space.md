# Projective space

↑ **Parent:** [Algebraic variety](algebraic-geometry.md#algebraic-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_space)

Projective space $\mathbb P^n$ is the set of one-dimensional subspaces of a vector space of dimension $n+1$, written in homogeneous coordinates $[x_0:\cdots:x_n]$.

**Table of contents**

- [Projective space represents invertible quotients](#projective-space-represents-invertible-quotients)
- [Morphisms from projective space to smaller projective space are constant](#morphisms-from-projective-space-to-smaller-projective-space-are-constant)
- [Dual projective space](#dual-projective-space)
  - [Projective dual variety](#projective-dual-variety)
    - [Projective biduality theorem](#projective-biduality-theorem)
- [Projective coordinates over a local ring](#projective-coordinates-over-a-local-ring)
- [Quaternionic projective space](#quaternionic-projective-space)
  - [Complex cobordism ring of the quaternionic projective plane](#complex-cobordism-ring-of-the-quaternionic-projective-plane)
  - [Complex inclusion into quaternionic projective space](#complex-inclusion-into-quaternionic-projective-space)
  - [Cohomology ring of quaternionic projective space](#cohomology-ring-of-quaternionic-projective-space)
- [General linear position](#general-linear-position)
- [Veronese map](#veronese-map)
- [Top cohomology of projective space](#top-cohomology-of-projective-space)
- [Cohomology of twisting sheaves on projective space](#cohomology-of-twisting-sheaves-on-projective-space)
  - [Nonnegative hyperplane twist cohomology by restriction](#nonnegative-hyperplane-twist-cohomology-by-restriction)
  - [Infinite negative-twist sum with zero global sections](#infinite-negative-twist-sum-with-zero-global-sections)
  - [Global regular functions on projective space](#global-regular-functions-on-projective-space)
- [Projective point](#projective-point)
  - [Homogeneous coordinate](#homogeneous-coordinate)
  - [Coordinate point](#coordinate-point)
- [Projective plane](#projective-plane)
  - [Point-line duality](#point-line-duality)
    - [Dual arrangement of a planar point set](#dual-arrangement-of-a-planar-point-set)
      - [Good edge of a dual line arrangement](#good-edge-of-a-dual-line-arrangement)
        - [Safe edge of a dual line arrangement](#safe-edge-of-a-dual-line-arrangement)
          - [Bounded-radius propagation of edge defects](#bounded-radius-propagation-of-edge-defects)
      - [Euler defect identity for a projective line arrangement](#euler-defect-identity-for-a-projective-line-arrangement)
  - [Fano plane](#fano-plane)
    - [Fano plane duality group](#fano-plane-duality-group)
    - [Fano point-line stabilizer intersection](#fano-point-line-stabilizer-intersection)
- [Projective linear transformation](#projective-linear-transformation)
- [Projective variety](#projective-variety)
  - [Veronese surface](#veronese-surface)
  - [Projective embedding](#projective-embedding)
  - [Pole divisor avoiding a fiber](#pole-divisor-avoiding-a-fiber)
  - [Projective completion](#projective-completion)
    - [Homogenization (algebra)](#homogenization-algebra)
  - [Projective dimension theorem](#projective-dimension-theorem)
  - [Projective curve](#projective-curve)
    - [Rational normal curve](#rational-normal-curve)
    - [Smooth projective curve](#smooth-projective-curve)
      - [Two-affine cover of a smooth projective curve](#two-affine-cover-of-a-smooth-projective-curve)
      - [Genus of a smooth projective curve](#genus-of-a-smooth-projective-curve)
        - [Rationality of a smooth projective genus-zero curve](#rationality-of-a-smooth-projective-genus-zero-curve)
      - [Smooth plane cubic in characteristic three](#smooth-plane-cubic-in-characteristic-three)
      - [Smooth rational curve](#smooth-rational-curve)
      - [Local ring of a smooth algebraic curve](#local-ring-of-a-smooth-algebraic-curve)
        - [Local parameter on a smooth algebraic curve](#local-parameter-on-a-smooth-algebraic-curve)
      - [Extension of a rational map from a smooth projective curve](#extension-of-a-rational-map-from-a-smooth-projective-curve)
        - [Failure of rational-map extension on a singular curve](#failure-of-rational-map-extension-on-a-singular-curve)
  - [Homogeneous coordinate ring](#homogeneous-coordinate-ring)
  - [Product of projective varieties](#product-of-projective-varieties)
    - [Coordinate projection](#coordinate-projection)
    - [Segre embedding](#segre-embedding)
    - [Smooth quadric surface](#smooth-quadric-surface)
      - [Projection from a point on a smooth quadric](#projection-from-a-point-on-a-smooth-quadric)
      - [Picard group of a smooth affine quadric surface](#picard-group-of-a-smooth-affine-quadric-surface)
      - [Segre description of a smooth quadric surface](#segre-description-of-a-smooth-quadric-surface)
      - [Rulings of a smooth quadric surface](#rulings-of-a-smooth-quadric-surface)
        - [Disjoint curves on a smooth quadric surface](#disjoint-curves-on-a-smooth-quadric-surface)

## Projective space represents invertible quotients

↑ **Parent:** [Projective space](projective-space.md)

With the quotient convention, [projective space](projective-space.md) represents the [functor](category.md#functor) of surjections from a rank-$n+1$ [free sheaf](ringed-space.md#free-sheaf) to a [line bundle](ringed-space.md#line-bundle), modulo isomorphisms of the target compatible with the map. On an affine base the target may be a nontrivial rank-one [projective module](module-theory.md#projective-module), so a tuple of elements generating the unit ideal is only the description when that target is trivial. Where the image of the $i$th basis vector generates the target, divide the other images by it to get the usual affine coordinates. Infinitesimal variations of the quotient form $\mathcal H om(\ker q,\mathcal L)$ and give the [Euler sequence](algebraic-geometry.md#euler-sequence).

## Morphisms from projective space to smaller projective space are constant

↑ **Parent:** [Projective space](projective-space.md)

A nonconstant morphism $\mathbb P^m\to\mathbb P^n$ with $m>n$ would have a positive-dimensional [fiber of a morphism](algebraic-geometry.md#fiber-of-a-morphism) by the [fiber dimension theorem](algebraic-geometry.md#fiber-dimension-theorem). A target hyperplane avoiding its image point meets the positive-dimensional projective image, so its pullback is a nonempty divisor in $\mathbb P^m$ disjoint from that fibre. Every positive-dimensional projective subvariety meets every hypersurface: on its affine cone, a homogeneous equation cuts a positive-dimensional zero set containing a nonzero cone point. This contradiction proves constancy.

## Dual projective space

↑ **Parent:** [Projective space](projective-space.md)

Hyperplanes in $\mathbb P(V)$ are kernels of nonzero linear functionals modulo scalar multiplication. Their parameter space is therefore $\mathbb P(V^*)$, of the same dimension. In particular lines in a [projective plane](#projective-plane) are parametrized by another [projective plane](#projective-plane).

### Projective dual variety

↑ **Parent:** [Dual projective space](#dual-projective-space)

For an irreducible [projective variety](#projective-variety) $Y\subset\mathbb P(V)$, its projective dual is the closure of hyperplanes containing the embedded tangent space at some smooth point of $Y$. Over the [complex numbers](complex-analysis.md#complex-number), biduality gives $(Y^*)^*=Y$. For a nondegenerate smooth curve in characteristic zero, the dual is an irreducible hypersurface; a general point corresponds to one ordinary tangency. Its defining incidence space consists of a point on the curve and a hyperplane containing its tangent line.

#### Projective biduality theorem

↑ **Parent:** [Projective dual variety](#projective-dual-variety)

Over the [complex numbers](complex-analysis.md#complex-number), an irreducible [projective variety](#projective-variety) is recovered by applying [projective dual variety](#projective-dual-variety) twice. In its conormal incidence variety, pairs $(y,H)$ with $H$ tangent at $y$ become pairs $(H,y)$ under exchange of the two projective factors. At general smooth pairs, differentiating the incidence equation shows that the hyperplane defined by $y$ is tangent to the dual variety at $H$. Closure gives the same conormal variety with the factors exchanged, proving biduality. This is why the branch hypersurface of the [Gauss map of a theta divisor](abelian-variety.md#gauss-map-of-a-theta-divisor) determines a nonhyperelliptic canonical curve.

## Projective coordinates over a local ring

↑ **Parent:** [Projective space](projective-space.md)

For a [local ring](commutative-algebra.md#local-ring) $A$, every map from $\operatorname{Spec}A$ into [projective space](projective-space.md) lands in one standard chart: the inverse image of a chart containing the closed point is the whole spectrum. This gives [homogeneous coordinates](#homogeneous-coordinate) with at least one unit entry, unique up to a common [unit](algebra.md#unit-in-a-ring). For a nonlocal ring, coordinates may instead merely generate the unit ideal, and general maps can involve a nontrivial [invertible sheaf](ringed-space.md#line-bundle) quotient.

## Quaternionic projective space

↑ **Parent:** [Projective space](projective-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quaternionic_projective_space)

Quaternionic projective space is the space of right quaternionic lines in $\mathbb H^{n+1}$. It is $S^{4n+3}$ modulo the right action of unit [quaternions](algebra.md#quaternion), with one cell in each dimension $0,4,\ldots,4n$. It is a compact smooth manifold of real dimension $4n$; $\mathbb{HP}^1\cong S^4$. The [quaternionic tautological line bundle](fiber-bundle.md#quaternionic-tautological-line-bundle) and its [sphere bundle](fiber-bundle.md#sphere-bundle) give the multiplication in its [cohomology ring of quaternionic projective space](#cohomology-ring-of-quaternionic-projective-space).

### Complex cobordism ring of the quaternionic projective plane

↑ **Parent:** [Quaternionic projective space](#quaternionic-projective-space)

For the [quaternionic tautological line bundle](fiber-bundle.md#quaternionic-tautological-line-bundle) regarded as a complex rank-two bundle, take $q=c_2^{MU}$. Its ordinary image generates degree-four integral cohomology, and its square generates degree eight. The [Atiyah-Hirzebruch spectral sequence](cohomology.md#atiyah-hirzebruch-spectral-sequence) collapses because the cells have dimensions $0,4,8$ and the coefficients are even. The classes $1,q,q^2$ lift a free basis of the associated graded module, and $q^3=0$ because the theory is connective and the space has dimension eight.

### Complex inclusion into quaternionic projective space

↑ **Parent:** [Quaternionic projective space](#quaternionic-projective-space)

Coordinate inclusion of complex vectors sends a complex line to its quaternionic span. If two such vectors span the same quaternionic line, a nonzero complex coordinate forces their scalar ratio to be complex, so this map is injective. The pulled-back [quaternionic tautological line bundle](fiber-bundle.md#quaternionic-tautological-line-bundle) splits as $L\oplus\overline L$ with complex first [Chern classes](algebraic-geometry.md#chern-class) $-x,x$. Its top [Chern class](algebraic-geometry.md#chern-class), and thus [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle), is $-x^2$. With $u$ the negative Euler generator, $i^*u=x^2$ and $i^*(u^k)=x^{2k}$. The map on infinite projective spaces is injective on cohomology; a finite inclusion loses the degrees with $2k>n$.

### Cohomology ring of quaternionic projective space

↑ **Parent:** [Quaternionic projective space](#quaternionic-projective-space)

The cell structure gives one integral cohomology generator in each degree divisible by four through $4n$. The [Gysin sequence of a sphere bundle](fiber-bundle.md#gysin-sequence-of-a-sphere-bundle) for the [quaternionic tautological line bundle](fiber-bundle.md#quaternionic-tautological-line-bundle) makes multiplication by its [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle) an isomorphism between successive such degrees. Choose $u$ to be the negative of that Euler class; its powers generate the displayed [cohomology ring](cohomology.md#cohomology-ring).

## General linear position

↑ **Parent:** [Projective space](projective-space.md)

Points in $\mathbb P^n$ are in general linear position when no $k+1$ of them lie in a projective subspace of dimension less than $k$ for $k\leq n$. Equivalently, every selection of at most $n+1$ representing vectors is [linearly independent](vector-space.md#linear-independence).

## Veronese map

↑ **Parent:** [Projective space](projective-space.md)

The degree-$d$ Veronese map sends a projective point to the list of all degree-$d$ monomials in its homogeneous coordinates. It embeds $\mathbb P^n$ into a higher-dimensional projective space.

## Top cohomology of projective space

↑ **Parent:** [Projective space](projective-space.md)

For a field $k$,

$$
H^n(\mathbb P_k^n,\mathcal O(-n-1))\cong k.
$$

This nonvanishing obstructs affine covers of $\mathbb P_k^n$ having only $n$ members.

## Cohomology of twisting sheaves on projective space

↑ **Parent:** [Projective space](projective-space.md)

For every integer $d$, the cohomology of a [twisting sheaf on projective space](ringed-space.md#twisting-sheaf-on-projective-space) is

$$
H^q(\mathbb P_k^n,\mathcal O(d))\cong
\begin{cases}
k[x_0,\ldots,x_n]_d,&q=0\text{ and }d\geq0,\\
k[x_0,\ldots,x_n]_{-d-n-1}^*,&q=n\text{ and }d\leq-n-1,\\
0,&\text{otherwise}.
\end{cases}
$$

Thus all intermediate cohomology vanishes. The top line follows from [Serre duality](ringed-space.md#serre-duality) and $\omega_{\mathbb P^n}\cong\mathcal O(-n-1)$.

### Nonnegative hyperplane twist cohomology by restriction

↑ **Parent:** [Cohomology of twisting sheaves on projective space](#cohomology-of-twisting-sheaves-on-projective-space)

For $m\ge0$, these [sheaf cohomology](ringed-space.md#sheaf-cohomology) dimensions follow from the vanishing for $\mathcal O$ and the [hyperplane exact sequence for twisting sheaves](ringed-space.md#hyperplane-exact-sequence-for-twisting-sheaves). Induct on dimension and then on $m$ in $0\to\mathcal O(m-1)\to\mathcal O(m)\to i_*\mathcal O_{\mathbf P^{n-1}}(m)\to0$. The [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology) gives higher-degree vanishing and the recurrence $h^0_n(m)-h^0_n(m-1)=\binom{n-1+m}{n-1}$. Starting with $h^0_n(0)=1$ yields the formula; the corresponding homogeneous monomials form a basis of global sections.

### Infinite negative-twist sum with zero global sections

↑ **Parent:** [Cohomology of twisting sheaves on projective space](#cohomology-of-twisting-sheaves-on-projective-space)

On the [projective line](finite-group-theory.md#projective-line), an infinite direct sum of copies of $\mathcal O(-1)$ is a [quasi-coherent sheaf](ringed-space.md#quasi-coherent-sheaf) but not a [coherent sheaf](ringed-space.md#coherent-sheaf): at any point its residue-vector-space dimension is infinite. Its [global sections](ringed-space.md#global-section) vanish because each summand has no sections, and sections commute with [direct sums](vector-space.md#direct-sum) for the finite two-chart equalizer. Its [direct image sheaf](ringed-space.md#direct-image-sheaf) on $\operatorname{Spec}k$ is consequently zero and coherent. This shows that a nonaffine direct image can lose information needed to detect coherence.

### Global regular functions on projective space

↑ **Parent:** [Cohomology of twisting sheaves on projective space](#cohomology-of-twisting-sheaves-on-projective-space)

The only [regular functions](ringed-space.md#regular-function) defined on all of a nonempty [projective space](projective-space.md) over a [field](algebra.md#field) $k$ are the constants:

$$
\Gamma(\mathbb P_k^n,\mathcal O)=H^0(\mathbb P_k^n,\mathcal O)=k.
$$

For $\mathbb P^1$, this also follows by gluing $k[t]$ and $k[t^{-1}]$ inside $k[t,t^{-1}]$: their intersection is $k$.

## Projective point

↑ **Parent:** [Projective space](projective-space.md)

A projective point is an equivalence class $[x_0:\cdots:x_n]$ of nonzero coordinate vectors under multiplication by a nonzero scalar.

### Homogeneous coordinate

↑ **Parent:** [Projective point](#projective-point)

The homogeneous coordinates $[x_0:\cdots:x_n]$ of a [projective point](#projective-point) are defined only up to simultaneous multiplication by a nonzero scalar.

### Coordinate point

↑ **Parent:** [Projective point](#projective-point)

A coordinate point of $\mathbb P^n$ is represented by a standard basis vector, so exactly one of its homogeneous coordinates is nonzero.

## Projective plane

↑ **Parent:** [Projective space](projective-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_plane)

The projective plane is the two-dimensional [projective space](projective-space.md) $\mathbb P^2$.

### Point-line duality

↑ **Parent:** [Projective plane](#projective-plane)

A point $[a:b:c]$ of the [projective plane](#projective-plane) corresponds to the dual line $aX+bY+cZ=0$. A line given by those coefficients corresponds back to the point $[a:b:c]$. Incidence is reversed: $p\in\ell$ if and only if $\ell^*\in p^*$. Thus collinear point triples become concurrent line triples, preserving the essential combinatorics of [incidence geometry](combinatorics.md#incidence-geometry).

#### Dual arrangement of a planar point set

↑ **Parent:** [Point-line duality](#point-line-duality)

Dualize a noncollinear finite point set in the [real projective plane](differential-geometry.md#real-projective-plane) to projective lines. Their intersection vertices and consecutive line segments form an embedded graph. A vertex incident to $k$ lines has graph degree $2k$ and corresponds to a primal line containing $k$ points. [Ordinary lines](combinatorics.md#ordinary-line) correspond to degree-four vertices. The faces are polygons with at least three sides.

##### Good edge of a dual line arrangement

↑ **Parent:** [Dual arrangement of a planar point set](#dual-arrangement-of-a-planar-point-set)

A [good dual-arrangement edge](#good-edge-of-a-dual-line-arrangement) has degree-six endpoints and two triangular adjacent faces. Other edges are bad. The [Euler defect identity for a projective line arrangement](#euler-defect-identity-for-a-projective-line-arrangement) bounds the number of bad edges by $16t_2$: charge them to degree-four or higher-degree vertices and to nontriangular faces. This turns a count of [ordinary lines](combinatorics.md#ordinary-line) into quantitative control of local triangular geometry.

###### Safe edge of a dual line arrangement

↑ **Parent:** [Good edge of a dual line arrangement](#good-edge-of-a-dual-line-arrangement)

A [safe dual-arrangement edge](#safe-edge-of-a-dual-line-arrangement) is one for which every edge on a path of length at most two from either endpoint is a [good dual-arrangement edge](#good-edge-of-a-dual-line-arrangement). This stronger local condition supplies a two-cell-thick triangular strip. Only a bounded multiple of the original bad edges can be unsafe: trace a shortest path to the first bad edge and reverse it through degree-six intermediate vertices.

###### Bounded-radius propagation of edge defects

↑ **Parent:** [Safe edge of a dual line arrangement](#safe-edge-of-a-dual-line-arrangement)

In an embedded arrangement graph, an edge whose fixed-radius neighbourhood meets a bad edge can be charged to the first such edge along a shortest path. All intervening edges are [good dual-arrangement edges](#good-edge-of-a-dual-line-arrangement), so their endpoints have bounded degree. The number of possible reversed paths is bounded in terms of the fixed radius alone. Therefore thickening a defect set by a fixed radius preserves an $O(t_2)$ edge count.

##### Euler defect identity for a projective line arrangement

↑ **Parent:** [Dual arrangement of a planar point set](#dual-arrangement-of-a-planar-point-set)

Let $t_k$ count vertices where $k$ lines meet and $f_j$ count faces with $j$ sides in a nonpencil projective line arrangement. Using [Euler characteristic](homology.md#euler-characteristic) one, $v=\sum t_k$, $e=\sum kt_k$, and $2e=\sum jf_j$ gives $t_2=3+\sum_{k\ge4}(k-3)t_k+\sum_{j\ge4}(j-3)f_j$. Thus few double vertices control both high-multiplicity vertices and nontriangular faces. Discarding the face term gives the usual arrangement form of the ordinary-line inequality.

### Fano plane

↑ **Parent:** [Projective plane](#projective-plane)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fano_plane)

The Fano plane is the [projective plane](#projective-plane) over the [finite field](algebra.md#finite-field) $\mathbb F_2$. It has seven points and seven lines, each line contains three points, and two distinct lines meet in one point. A line-point incidence matrix $N$ therefore satisfies $NN^{\mathsf T}=2I+J$, making it invertible over the real numbers and useful for the [transplantation theorem](riemannian-geometry.md#transplantation-theorem).

#### Fano plane duality group

↑ **Parent:** [Fano plane](#fano-plane)

Adjoin the [inverse-transpose automorphism](finite-group-theory.md#inverse-transpose-automorphism) to the collineation group of the [Fano plane](#fano-plane). Its maximal subgroups other than the collineation group are unordered incident-pair stabilizers, unordered nonincident-pair stabilizers and Sylow 7-normalizers, of orders 16, 12 and 42.

#### Fano point-line stabilizer intersection

↑ **Parent:** [Fano plane](#fano-plane)

There are 21 incident point-line pairs and 28 nonincident pairs in the [Fano plane](#fano-plane), with $GL_3(2)$ transitive on each type. [Orbit-stabilizer theorem](group-theory.md#orbit-stabilizer-theorem) gives the two orders as $168/21=8$ and $168/28=6$.

## Projective linear transformation

↑ **Parent:** [Projective space](projective-space.md)

An invertible linear map of the underlying vector space induces a projective linear transformation of $\mathbb P^n$; scalar multiples induce the same transformation.

## Projective variety

↑ **Parent:** [Projective space](projective-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_variety)

A projective variety is a closed algebraic subvariety of some projective space.

### Veronese surface

↑ **Parent:** [Projective variety](#projective-variety)

The complete system of quadratic forms maps $\mathbb P^2$ to a smooth surface of degree four in $\mathbb P^5$. The six coordinates are $x_0^2,x_0x_1,x_0x_2,x_1^2,x_1x_2,x_2^2$. It occurs as a degree-two image of a [K3 surface](complex-geometry.md#k3-surface) and, after taking a projective cone, in the plane-quintic exception to the [K3 linear system dichotomies](complex-geometry.md#k3-linear-system-dichotomies).

### Projective embedding

↑ **Parent:** [Projective variety](#projective-variety)

A projective embedding realizes a variety as a closed subvariety of [projective space](projective-space.md). A [very ample line bundle](ringed-space.md#very-ample-line-bundle) gives such an embedding through its global sections.

### Pole divisor avoiding a fiber

↑ **Parent:** [Projective variety](#projective-variety)

Suppose a nonconstant [morphism of varieties](algebraic-geometry.md#morphism-of-algebraic-varieties) $f:X\to Z$ has fiber $Y$ over $z_0$, where $X$ is normal, connected and projective. Choose an affine neighborhood $U$ of $z_0$ and a regular function on $U$ nonconstant on $f(X)\cap U$. Its pullback is a nonconstant rational function on $X$, so its pole [Weil divisor](algebraic-geometry.md#weil-divisor) is nonzero. A pole-free rational function on a normal variety is regular, and global regular functions on a connected [projective variety](#projective-variety) are constant. The pole divisor avoids $f^{-1}(U)$, hence avoids $Y$. No projectivity assumption on $Z$ is needed.

### Projective completion

↑ **Parent:** [Projective variety](#projective-variety)

A projective completion of an [affine variety](algebraic-geometry.md#affine-algebraic-set) $X$ is a [projective variety](#projective-variety) containing $X$ as a dense open subvariety. Homogenizing affine defining equations and taking their projective zero set gives the projective closure, although it may add singularities at infinity.

#### Homogenization (algebra)

↑ **Parent:** [Projective completion](#projective-completion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homogenization_(algebra))

The homogenization of a polynomial $f(x_1,\ldots,x_n)$ of total degree $d$ is the homogeneous polynomial

$$
F(X_1,\ldots,X_n,Z)=Z^df(X_1/Z,\ldots,X_n/Z).
$$

Its projective zero set is the [projective closure](#projective-completion) of the affine hypersurface defined by $f$.

### Projective dimension theorem

↑ **Parent:** [Projective variety](#projective-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_dimension_theorem)

If projective varieties $X,Y\subseteq\mathbb P^n$ have dimensions $r,s$ and $r+s\geq n$, then $X\cap Y$ is nonempty and every component has dimension at least $r+s-n$.

### Projective curve

↑ **Parent:** [Projective variety](#projective-variety)

A [projective curve](#projective-curve) is a projective [algebraic curve](algebraic-geometry.md#algebraic-curve). A projective curve is a one-dimensional [projective variety](#projective-variety).

#### Rational normal curve

↑ **Parent:** [Projective curve](#projective-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_normal_curve)

A rational normal curve in $\mathbb P^n$ is the image of the degree-$n$ [Veronese map](#veronese-map) from $\mathbb P^1$. After projective changes of coordinates it has parametrization

$$
[S:T]\longmapsto[S^n:S^{n-1}T:\cdots:T^n].
$$

#### Smooth projective curve

↑ **Parent:** [Projective curve](#projective-curve)

A [smooth projective curve](#smooth-projective-curve) is a nonsingular [projective curve](#projective-curve). A smooth projective curve is a nonsingular projective variety of dimension one.

##### Two-affine cover of a smooth projective curve

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

A nonconstant rational function on a [smooth projective curve](#smooth-projective-curve) extends to a [finite morphism](algebraic-geometry.md#finite-morphism) to the [projective line](finite-group-theory.md#projective-line). The inverse images of its two standard affine charts are [affine varieties](algebraic-geometry.md#affine-algebraic-set) covering the curve. The resulting [Čech cochain complex](ringed-space.md#cech-cochain-complex) has only degrees zero and one, so every [coherent sheaf](ringed-space.md#coherent-sheaf) has zero [sheaf cohomology](ringed-space.md#sheaf-cohomology) in degrees at least two.

##### Genus of a smooth projective curve

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

For a [smooth projective curve](#smooth-projective-curve) with $H^0(C,\mathcal O_C)=k$, its genus is $\dim_kH^1(C,\mathcal O_C)$, equivalently $\dim_kH^0(C,\Omega^1_C)$ by [Serre duality](ringed-space.md#serre-duality). It equals the [arithmetic genus](algebraic-geometry.md#arithmetic-genus) $1-\chi(\mathcal O_C)$. Without the condition on constants, the general [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) instead uses $\chi(\mathcal O_C)=h^0(\mathcal O_C)-h^1(\mathcal O_C)$.

###### Rationality of a smooth projective genus-zero curve

↑ **Parent:** [Genus of a smooth projective curve](#genus-of-a-smooth-projective-curve)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), choose a point $P$ on the [smooth projective curve](#smooth-projective-curve). The [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) gives $\dim L(P)=2$: the complementary [canonical divisor](algebraic-geometry.md#canonical-divisor) term has negative degree. A nonconstant function in $L(P)$ has exactly one simple pole, so it defines a degree-one [morphism of algebraic curves](algebraic-geometry.md#morphism-of-algebraic-curves) to the [projective line](finite-group-theory.md#projective-line). A degree-one map between [smooth projective curves](#smooth-projective-curve) is an [isomorphism](algebra.md#isomorphism). The existence of a rational point is essential over a field which is not algebraically closed.

##### Smooth plane cubic in characteristic three

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

Over the algebraic closure of $\mathbb F_3$, the displayed cubic is smooth. Its three partial derivatives are $Z^2$, $2YZ$, and $Y^2+2XZ$; their simultaneous vanishing would give $Z=Y=0$, and the equation would then give $X=0$, impossible in projective space. Its affine equation $y^2=x^3-x$ is irreducible because the odd-degree polynomial on the right is not a square in the rational function field.

##### Smooth rational curve

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

Over an algebraically closed field, a smooth projective rational curve is isomorphic to $\mathbb P^1$. Its [line bundles](ringed-space.md#line-bundle) are determined by degree, its degree-zero [line bundle](ringed-space.md#line-bundle) is trivial, and $H^1(\mathbb P^1,\mathcal O)=0$. An integral projective curve of [arithmetic genus](algebraic-geometry.md#arithmetic-genus) zero is automatically smooth and rational by the normalization genus formula.

##### Local ring of a smooth algebraic curve

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

At every point of a [smooth algebraic curve](algebraic-geometry.md#smooth-algebraic-curve), the [local ring](commutative-algebra.md#local-ring) is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring). Its valuation measures the [order of vanishing](isolated-singularity.md#order-of-vanishing) of a [rational function](isolated-singularity.md#rational-function) at that point.

###### Local parameter on a smooth algebraic curve

↑ **Parent:** [Local ring of a smooth algebraic curve](#local-ring-of-a-smooth-algebraic-curve)

At a point of a [smooth algebraic curve](algebraic-geometry.md#smooth-algebraic-curve), its [local ring](commutative-algebra.md#local-ring) is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring). A local parameter is a generator $t$ of its [maximal ideal](commutative-algebra.md#maximal-ideal), equivalently an element of [valuation](algebra.md#valuation) one. It measures the order of a [zero of a function](polynomial.md#zero-of-a-function) or [pole](isolated-singularity.md#pole) by expressing functions as powers of $t$ times units. Over the complex numbers its analytic counterpart is a [local coordinate](complex-analysis.md#local-coordinate) vanishing simply at the point. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) in a [Weierstrass equation of an elliptic curve](normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve), $t=-x/y$ is the standard parameter at the identity.

##### Extension of a rational map from a smooth projective curve

↑ **Parent:** [Smooth projective curve](#smooth-projective-curve)

Every [rational map](algebraic-geometry.md#rational-map-of-projective-varieties) from a [smooth projective curve](#smooth-projective-curve) to a [projective variety](#projective-variety) extends uniquely to a [morphism](algebraic-geometry.md#morphism-of-algebraic-varieties). At a missing point, the [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) of the curve lets one divide homogeneous coordinates by their smallest valuation, leaving regular coordinates of which at least one is a unit.

###### Failure of rational-map extension on a singular curve

↑ **Parent:** [Extension of a rational map from a smooth projective curve](#extension-of-a-rational-map-from-a-smooth-projective-curve)

Let $\nu:\widetilde C\to C$ be the [normalization of a nodal curve](normalization-of-an-algebraic-curve.md#normalization-of-a-nodal-curve). Its rational inverse $C\dashrightarrow\widetilde C$ cannot extend over the node: the two branches give two distinct points of $\widetilde C$, whereas a morphism can assign only one image to the node.

### Homogeneous coordinate ring

↑ **Parent:** [Projective variety](#projective-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homogeneous_coordinate_ring)

For $X=V_+(I)\subseteq\mathbb P^n$, the homogeneous coordinate ring is the [graded ring](commutative-algebra.md#graded-ring) $k[x_0,\ldots,x_n]/I$.

### Product of projective varieties

↑ **Parent:** [Projective variety](#projective-variety)

The product of projective varieties is projective via the Segre embedding. Dimensions add under products, and the product of smooth varieties is smooth.

#### Coordinate projection

↑ **Parent:** [Product of projective varieties](#product-of-projective-varieties)

The coordinate projections from a product send $(x,y)$ to $x$ and $y$, respectively. For products of [projective varieties](#projective-variety), they are [morphisms](algebraic-geometry.md#morphism-of-algebraic-varieties).

#### Segre embedding

↑ **Parent:** [Product of projective varieties](#product-of-projective-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Segre_embedding)

The Segre embedding sends

$$
([x_0:\cdots:x_m],[y_0:\cdots:y_n])
\longmapsto [x_iy_j]_{i,j}
$$

and realizes $\mathbb P^m\times\mathbb P^n$ as a [projective variety](#projective-variety).

#### Smooth quadric surface

↑ **Parent:** [Product of projective varieties](#product-of-projective-varieties)

A [smooth quadric surface](#smooth-quadric-surface) is a smooth two-dimensional [quadric hypersurface](algebraic-geometry.md#quadric-algebraic-geometry). Over an [algebraically closed field](algebra.md#algebraically-closed-field) of [characteristic](algebra.md#characteristic-of-a-field) other than two, every smooth quadric surface in $\mathbb P^3$ becomes

$$
V(x_0x_3-x_1x_2),
$$

after a [projective linear transformation](#projective-linear-transformation). The [Segre embedding](#segre-embedding) identifies it with $\mathbb P^1\times\mathbb P^1$.

##### Projection from a point on a smooth quadric

↑ **Parent:** [Smooth quadric surface](#smooth-quadric-surface)

For $X=\{x_0x_1=x_2x_3\}$ and $P=[1:0:0:1]$, the displayed map is defined on $X\setminus\{P\}$. Its fibre over $[u:v:w]$ has equation $(u-v)\lambda+uw=0$ on an affine line. Away from $u=v$ the fibre is one reduced point. On that line it is empty except at $[0:0:1]$ and $[1:1:0]$, where it is a punctured ruling line, hence an affine line. The two exceptional lines are the [rulings of a smooth quadric surface](#rulings-of-a-smooth-quadric-surface) through $P$.

##### Picard group of a smooth affine quadric surface

↑ **Parent:** [Smooth quadric surface](#smooth-quadric-surface)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), remove a smooth hyperplane conic $C$ from a [smooth quadric surface](#smooth-quadric-surface) $Q$. The [rulings of a smooth quadric surface](#rulings-of-a-smooth-quadric-surface) generate $\operatorname{Pic}(Q)=\mathbb Z^2$, and $C$ has class $(1,1)$. [Picard-group localization on a smooth variety](ringed-space.md#picard-group-localization-on-a-smooth-variety) gives the quotient by $\mathbb Z(1,1)$. The restricted ruling bundle $\mathcal O_Q(1,0)$ is a generator, exhibiting a nontrivial [line bundle](ringed-space.md#line-bundle) on an affine surface.

##### Segre description of a smooth quadric surface

↑ **Parent:** [Smooth quadric surface](#smooth-quadric-surface)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), a smooth four-variable projective quadratic equation can be written $x_0x_3-x_1x_2=0$, including in characteristic two. Its quadratic form splits into two hyperbolic planes: choose an isotropic vector and its paired vector, adjust the latter to be isotropic, and repeat on the orthogonal complement. In characteristic two, smoothness forces the alternating polar form in dimension four to have full rank, since a positive-dimensional radical has a nonzero isotropic vector over the algebraically closed field and would give a singular point. The [Segre embedding](#segre-embedding) $([s_0:s_1],[t_0:t_1])\mapsto[s_0t_0:s_0t_1:s_1t_0:s_1t_1]$ then gives the [isomorphism](algebra.md#isomorphism). Each matrix of coordinates has rank one, which supplies the inverse pair of projective factors.

##### Rulings of a smooth quadric surface

↑ **Parent:** [Smooth quadric surface](#smooth-quadric-surface)

Under $Q\cong\mathbb P^1\times\mathbb P^1$, the fibres of the two [coordinate projections](#coordinate-projection) are the two rulings of the [smooth quadric surface](#smooth-quadric-surface). Two distinct fibres in one ruling are disjoint [projective lines](finite-group-theory.md#projective-line), while one fibre from each ruling meets in one point.

###### Disjoint curves on a smooth quadric surface

↑ **Parent:** [Rulings of a smooth quadric surface](#rulings-of-a-smooth-quadric-surface)

For distinct $p,q\in\mathbb P^1$, the curves $\mathbb P^1\times\{p\}$ and $\mathbb P^1\times\{q\}$ are disjoint, smooth, and projective.

## ↑ Ancestors (6)

1. [Algebraic variety](algebraic-geometry.md#algebraic-variety)
2. [Algebraic geometry](algebraic-geometry.md)
3. [Geometry and topology](geometry-and-topology.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (49)

- [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve)
- [Blowing up (algebraic geometry)](algebraic-geometry.md#blowing-up-algebraic-geometry)
- [Canonical bundle of projective space](ringed-space.md#canonical-bundle-of-projective-space)
- [Canonical-form transition on projective space](ringed-space.md#canonical-form-transition-on-projective-space)
- [Complex tautological line bundle](fiber-bundle.md#complex-tautological-line-bundle)
- [Cotangent Euler sequence in homogeneous coordinates](algebraic-geometry.md#cotangent-euler-sequence-in-homogeneous-coordinates)
- [Cubic surface](algebraic-geometry.md#cubic-surface)
- [Finite global generation on a quasi-compact scheme](ringed-space.md#finite-global-generation-on-a-quasi-compact-scheme)
- [Genus bound for a nonplanar degree-five curve](algebraic-geometry.md#genus-bound-for-a-nonplanar-degree-five-curve)
- [Global regular functions on projective space](#global-regular-functions-on-projective-space)
- [Hyperplane divisor](cartier-divisor.md#hyperplane-divisor)
- [Laurent-monomial description of top cohomology on projective space](ringed-space.md#laurent-monomial-description-of-top-cohomology-on-projective-space)
- [Length-two criterion for a very ample linear system](algebraic-geometry.md#length-two-criterion-for-a-very-ample-linear-system)
- [Line bundle](ringed-space.md#line-bundle)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-56.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-15.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-18.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-23.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-89.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-21.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-16.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-20.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-20.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#24i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-113.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#24f/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#24g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-113.md#1/c/solution)
- [Plücker coordinates](differential-geometry.md#plucker-coordinates)
- [Projective bundle](fiber-bundle.md#projective-bundle)
- [Projective complete intersection](ringed-space.md#projective-complete-intersection)
- [Projective coordinates over a local ring](#projective-coordinates-over-a-local-ring)
- [Projective embedding](#projective-embedding)
- [Projective plane](#projective-plane)
- [Projective space represents invertible quotients](#projective-space-represents-invertible-quotients)
- [Projective special linear group](group-theory.md#projective-special-linear-group)
- [Projective tangent plane](algebraic-geometry.md#projective-tangent-plane)
- [Projective twistor space](general-relativity.md#projective-twistor-space)
- [Quasi-projective algebraic set](algebraic-geometry.md#quasi-projective-algebraic-set)
- [Quasi-projective variety](algebraic-geometry.md#quasi-projective-variety)
- [Real conic without real rational points](algebraic-geometry.md#real-conic-without-real-rational-points)
- [Simplex fan](toric-geometry.md#simplex-fan)
- [Smooth morphism](ringed-space.md#smooth-morphism)
- [Smooth projective surface](algebraic-geometry.md#smooth-projective-surface)
- [Very ample line bundle](ringed-space.md#very-ample-line-bundle)
