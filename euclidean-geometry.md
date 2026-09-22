# Euclidean geometry

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_geometry)

[Euclidean geometry](euclidean-geometry.md) describes flat [Euclidean space](normed-vector-space.md#euclidean-norm) using [lengths](physics.md#length), [angles](geometry-and-topology.md#angle), and [rigid motions](#rigid-transformation). A coordinate realization uses points $x,y\in\mathbb R^n$, [Euclidean distance](topological-analysis.md#euclidean-distance)

$$
d(x,y)=\sqrt{\sum_{i=1}^n(x_i-y_i)^2},
$$

and [angles](geometry-and-topology.md#angle) determined by the [dot product](inner-product.md#dot-product). The coordinate axes are a convenience: [translations](geometry-and-topology.md#translation-geometry) and [rotations](riemannian-geometry.md#rotation-mathematics) change coordinates while preserving these measurements. This makes [Euclidean geometry](euclidean-geometry.md) useful for comparing figures and converting measurements along different directions into a single distance.

In the [Euclidean plane](geometry-and-topology.md#euclidean-plane), through a point outside a line there is exactly one parallel line. This is a standard equivalent formulation of the [parallel postulate](#parallel-postulate). Euclid's fifth postulate in the [Elements](#euclid-s-elements) instead describes when two lines meet using the interior [angles](geometry-and-topology.md#angle) made by a crossing line.[Euclid, Elements I, Postulate 5](https://mathcs.clarku.edu/~djoyce/elements/bookI/post5.html) The assumption has consequences we often take for granted: a [triangle](#triangle)'s interior [angles](geometry-and-topology.md#angle) sum to $\pi$, and [similar triangles](#similar-triangle) can differ in size while keeping their [angles](geometry-and-topology.md#angle). Comparing with [spherical geometry](geometry-and-topology.md#spherical-geometry) reveals that these are properties of a particular geometry.

As a computed example, the diagonal from $(0,0)$ to $(4,3)$ in a [rectangle](#rectangle) has [length](physics.md#length) $\sqrt{4^2+3^2}=5$. The [Pythagorean theorem](#pythagorean-theorem) explains why perpendicular contributions add as squares. If the directions cease to meet at a [right angle](#right-angle), the [law of cosines](#law-of-cosines) supplies the missing [angle](geometry-and-topology.md#angle)-dependent term. The beauty is that a single distance formula unites geometric constructions, coordinate calculations, and [orthogonality](inner-product.md#orthogonal-vectors) in [linear algebra](linear-algebra.md).

Make the assumptions visible: in a [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system) with [orthogonal](inner-product.md#orthogonal-vectors) axes and the same [length](physics.md#length) unit on each axis, take $A=(0,0)$, $B=(4,0)$ and $C=(0,3)$. The [vectors](vector-space.md#vector) $B-A=(4,0)$ and $C-A=(0,3)$ have [dot product](inner-product.md#dot-product) zero, establishing a [right angle](#right-angle) at $A$ before using the [Pythagorean theorem](#pythagorean-theorem). A sketch that merely looks like a [right triangle](#right-triangle) supplies no such guarantee. Likewise, an image stretched horizontally and vertically by different amounts can distort both [lengths](physics.md#length) and [angles](geometry-and-topology.md#angle); a displayed shape and the assumptions defining it must be kept separate.

For a less origin-dependent measurement, take $P=(1,2)$ and $Q=(5,5)$. Their displacement [vector](vector-space.md#vector) is $Q-P=(4,3)$, so their [Euclidean distance](topological-analysis.md#euclidean-distance) is again $5$. Its [Euclidean norm](normed-vector-space.md#euclidean-norm) records the direct separation, whereas travelling first horizontally and then vertically covers [length](physics.md#length) $4+3=7$. This connects measuring a diagonal to locating two positions from a [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system). A [translation](geometry-and-topology.md#translation-geometry) changes where the positions are recorded without changing their separation; a [rotation](riemannian-geometry.md#rotation-mathematics) changes the component values without changing the [Euclidean norm](normed-vector-space.md#euclidean-norm).

**Table of contents**

- [Straightedge and compass construction](straightedge-and-compass-construction.md)
  - [Constructible polygon](straightedge-and-compass-construction.md#constructible-polygon)
    - [Constructible regular polygon](straightedge-and-compass-construction.md#constructible-regular-polygon)
      - [Gauss-Wantzel theorem](straightedge-and-compass-construction.md#gauss-wantzel-theorem)
- [Dihedral angle](#dihedral-angle)
  - [Torsion angle](#torsion-angle)
- [Sylvester-Gallai theorem](#sylvester-gallai-theorem)
- [Geometric scale factor](#geometric-scale-factor)
- [Perpendicular lines](#perpendicular-lines)
- [Cone (geometry)](#cone-geometry)
  - [Optimal cylinder inscribed in a cone](#optimal-cylinder-inscribed-in-a-cone)
- [Collinearity](#collinearity)
- [Quadric surface](#quadric-surface)
  - [Parabolic cylinder](#parabolic-cylinder)
  - [Distance extrema on a real quadratic surface](#distance-extrema-on-a-real-quadratic-surface)
    - [Distance extrema on a central plane section of an ellipsoid](#distance-extrema-on-a-central-plane-section-of-an-ellipsoid)
  - [Hyperbolic cylinder](#hyperbolic-cylinder)
  - [Elliptic cylinder](#elliptic-cylinder)
  - [Signature transition from an ellipsoid to an elliptic cylinder and a one-sheet hyperboloid](#signature-transition-from-an-ellipsoid-to-an-elliptic-cylinder-and-a-one-sheet-hyperboloid)
  - [Elliptic cone](#elliptic-cone)
- [Center (geometry)](#center-geometry)
- [Distance between parallel lines](#distance-between-parallel-lines)
- [Square grid](#square-grid)
- [Parallel postulate](#parallel-postulate)
- [Euclid's Elements](#euclid-s-elements)
- [Congruence (geometry)](#congruence-geometry)
  - [Geometric congruence class](#geometric-congruence-class)
- [Right circular conical surface](#right-circular-conical-surface)
- [Euclidean group](#euclidean-group)
- [Geometric locus](#geometric-locus)
- [Hypercube](#hypercube)
  - [Orthogonality of hypercube body diagonals](#orthogonality-of-hypercube-body-diagonals)
- [Centroid](#centroid)
  - [Integral of an affine function over a simplex](#integral-of-an-affine-function-over-a-simplex)
- [Polygon](#polygon)
  - [Dodecagon](#dodecagon)
  - [Regular star polygon](#regular-star-polygon)
  - [Cyclic polygon](#cyclic-polygon)
  - [Shoelace formula](#shoelace-formula)
  - [Kernel of a polygon](#kernel-of-a-polygon)
  - [Polygon inequality](#polygon-inequality)
  - [Semiperimeter](#semiperimeter)
  - [Perimeter of a polygon](#perimeter-of-a-polygon)
  - [Pentagon](#pentagon)
  - [Hexagon](#hexagon)
    - [Regular hexagon](#regular-hexagon)
  - [Vertex of a polygon](#vertex-of-a-polygon)
  - [Side of a polygon](#side-of-a-polygon)
  - [Diagonal of a polygon](#diagonal-of-a-polygon)
  - [Quadrilateral](#quadrilateral)
    - [Convex quadrilateral](#convex-quadrilateral)
    - [Rectangle](#rectangle)
      - [Square](#square)
        - [Square lamina](#square-lamina)
        - [Unit square](#unit-square)
    - [Parallelogram](#parallelogram)
    - [Bretschneider's formula](#bretschneider-s-formula)
- [Point group](#point-group)
  - [Neumann's principle](#neumann-s-principle)
  - [Molecular symmetry](#molecular-symmetry)
    - [Symmetry coordinate](#symmetry-coordinate)
    - [D infinity h molecular point group](#d-infinity-h-molecular-point-group)
    - [C4v molecular point group](#c4v-molecular-point-group)
    - [Symmetry operation](#symmetry-operation)
    - [Molecular point group](#molecular-point-group)
    - [C2h molecular point group](#c2h-molecular-point-group)
    - [C3v molecular point group](#c3v-molecular-point-group)
    - [D6h molecular point group](#d6h-molecular-point-group)
    - [Td molecular point group](#td-molecular-point-group)
      - [Methane normal-mode representation](#methane-normal-mode-representation)
    - [Infrared and Raman mutual exclusion](#infrared-and-raman-mutual-exclusion)
    - [Molecular character reduction](#molecular-character-reduction)
    - [Symmetry-closed orbital basis](#symmetry-closed-orbital-basis)
    - [Ih molecular point group](#ih-molecular-point-group)
    - [D4h molecular point group](#d4h-molecular-point-group)
    - [D3h molecular point group](#d3h-molecular-point-group)
    - [D2d molecular point group](#d2d-molecular-point-group)
    - [C2v molecular point group](#c2v-molecular-point-group)
    - [Molecular symmetry operation](#molecular-symmetry-operation)
  - [D2h point group](#d2h-point-group)
  - [C2v point group](#c2v-point-group)
  - [Crystallographic restriction theorem](#crystallographic-restriction-theorem)
- [Wallpaper group](#wallpaper-group)
- [Elliptic paraboloid](#elliptic-paraboloid)
  - [Volume and centroid of a parabolic cup](#volume-and-centroid-of-a-parabolic-cup)
  - [Paraboloid sector surface measures](#paraboloid-sector-surface-measures)
  - [Maximal cylinder and box in an elliptic paraboloid](#maximal-cylinder-and-box-in-an-elliptic-paraboloid)
- [Double circular cone](#double-circular-cone)
  - [Intersection plane of parallel congruent double cones](#intersection-plane-of-parallel-congruent-double-cones)
- [Geometric packing](#geometric-packing)
  - [Triangular lattice packing of discs](#triangular-lattice-packing-of-discs)
  - [Sphere packing](#sphere-packing)
    - [Hard-sphere model](#hard-sphere-model)
    - [Simple-cubic sphere packing](#simple-cubic-sphere-packing)
  - [Circle packing](#circle-packing)
    - [Descartes' circle theorem](#descartes-circle-theorem)
    - [Alternating-radius square circle packing](#alternating-radius-square-circle-packing)
  - [Packing fraction](#packing-fraction)
- [Euclidean ray](#euclidean-ray)
  - [Injectivity of sums on two distinct rays](#injectivity-of-sums-on-two-distinct-rays)
  - [Open planar sector](#open-planar-sector)
- [Hyperbolic paraboloid](#hyperbolic-paraboloid)
- [Right circular cone](#right-circular-cone)
- [Straight line](#straight-line)
  - [Direction vector](#direction-vector)
  - [Slope](#slope)
  - [Secant line](#secant-line)
  - [Parametric equation of a straight line](#parametric-equation-of-a-straight-line)
- [Polyhedron](#polyhedron)
  - [Bicapped square antiprism](#bicapped-square-antiprism)
  - [Pentagonal bipyramid](#pentagonal-bipyramid)
  - [Truncated octahedron](#truncated-octahedron)
  - [Prism (geometry)](#prism-geometry)
    - [Minimum deviation of a prism](#minimum-deviation-of-a-prism)
      - [Prism sweep under different rotation conventions](#prism-sweep-under-different-rotation-conventions)
    - [Hexagonal prism](#hexagonal-prism)
  - [Edge of a polyhedron](#edge-of-a-polyhedron)
  - [Interior dihedral angle of a convex polyhedron](#interior-dihedral-angle-of-a-convex-polyhedron)
  - [Pyramid](#pyramid)
    - [Square pyramid](#square-pyramid)
  - [Octahedron](#octahedron)
  - [Parallelepiped](#parallelepiped)
    - [Rectangular parallelepiped](#rectangular-parallelepiped)
  - [Pentagonal prism](#pentagonal-prism)
  - [Tetrahedron](#tetrahedron)
    - [Tetrahedron membership via scalar triple products](#tetrahedron-membership-via-scalar-triple-products)
    - [Tetrahedron centroid-to-midpoint sum of squares](#tetrahedron-centroid-to-midpoint-sum-of-squares)
    - [Incenter of a tetrahedron](#incenter-of-a-tetrahedron)
    - [Circumcenter of a tetrahedron](#circumcenter-of-a-tetrahedron)
    - [Regular tetrahedron](#regular-tetrahedron)
    - [Sphere center from three tetrahedron face distances](#sphere-center-from-three-tetrahedron-face-distances)
    - [Opposite edges of a tetrahedron](#opposite-edges-of-a-tetrahedron)
      - [Tetrahedron volume under sliding opposite edges](#tetrahedron-volume-under-sliding-opposite-edges)
      - [Orthogonal opposite edges of a tetrahedron](#orthogonal-opposite-edges-of-a-tetrahedron)
  - [Platonic solid](#platonic-solid)
    - [Regular icosahedron](#regular-icosahedron)
    - [Cube](#cube)
    - [Dodecahedron](#dodecahedron)
  - [Archimedean solid](#archimedean-solid)
    - [Icosidodecahedron](#icosidodecahedron)
- [Pythagorean theorem](#pythagorean-theorem)
  - [Pythagorean equation](#pythagorean-equation)
  - [Pythagorean triple](#pythagorean-triple)
    - [Berggren tree](#berggren-tree)
    - [Primitive Pythagorean triple](#primitive-pythagorean-triple)
    - [Euclid's formula for Pythagorean triples](#euclid-s-formula-for-pythagorean-triples)
    - [Primitive Pythagorean parametrization](#primitive-pythagorean-parametrization)
- [Voronoi diagram](#voronoi-diagram)
- [Sphere](#sphere)
  - [Tangent spheres](#tangent-spheres)
  - [Equator](#equator)
  - [Meridian of a sphere](#meridian-of-a-sphere)
  - [Volume enclosed by a sphere](#volume-enclosed-by-a-sphere)
  - [Spherical wedge](#spherical-wedge)
  - [Circle of intersection of two spheres](#circle-of-intersection-of-two-spheres)
  - [Spherical shell](#spherical-shell)
  - [Product of two spheres](#product-of-two-spheres)
    - [Simultaneous antipodal quotient of two spheres](#simultaneous-antipodal-quotient-of-two-spheres)
  - [Surface measure on a sphere](#surface-measure-on-a-sphere)
  - [Antipodal pair](#antipodal-pair)
  - [Apollonius sphere](#apollonius-sphere)
  - [Hemisphere](#hemisphere)
    - [Maximum-volume cuboid in a hemisphere](#maximum-volume-cuboid-in-a-hemisphere)
    - [Open hemisphere](#open-hemisphere)
      - [General-position hemisphere count](#general-position-hemisphere-count)
      - [Gale hemisphere lemma](#gale-hemisphere-lemma)
  - [Great circle](#great-circle)
    - [Regions of a general-position great-circle arrangement](#regions-of-a-general-position-great-circle-arrangement)
  - [Gnomonic projection](#gnomonic-projection)
  - [Unit sphere as a regular level set](#unit-sphere-as-a-regular-level-set)
  - [Two-sphere](#two-sphere)
  - [Three-sphere](#three-sphere)
  - [Solid angle](#solid-angle)
    - [Steradian](#steradian)
    - [Solid angle of a circular cone](#solid-angle-of-a-circular-cone)
    - [Solid angle of a disk](#solid-angle-of-a-disk)
    - [Angular average](#angular-average)
- [Triangle](#triangle)
  - [Apollonius's theorem](#apollonius-s-theorem)
  - [Median of a triangle](#median-of-a-triangle)
  - [Heron's formula](#heron-s-formula)
  - [Circumradius](#circumradius)
  - [Incenter](#incenter)
  - [Angle bisector theorem](#angle-bisector-theorem)
  - [Fermat point](#fermat-point)
  - [Law of sines](#law-of-sines)
  - [Orthocenter](#orthocenter)
  - [Isosceles triangle](#isosceles-triangle)
  - [Similar triangle](#similar-triangle)
  - [Incircle of a triangle](#incircle-of-a-triangle)
    - [Inradius](#inradius)
  - [Circumcircle](#circumcircle)
  - [Law of cosines](#law-of-cosines)
  - [Acute triangle](#acute-triangle)
  - [Equilateral triangle](#equilateral-triangle)
  - [Right triangle](#right-triangle)
    - [Leg of a right triangle](#leg-of-a-right-triangle)
    - [Hypotenuse](#hypotenuse)
- [Trapezoid](#trapezoid)
- [Triangular prism](#triangular-prism)
- [Borsuk conjecture](#borsuk-conjecture)
  - [Kahn-Kalai counterexample to the Borsuk conjecture](#kahn-kalai-counterexample-to-the-borsuk-conjecture)
    - [Quadratic sign-vector diameter formula](#quadratic-sign-vector-diameter-formula)
    - [Borsuk counterexample in dimension 1325](#borsuk-counterexample-in-dimension-1325)
    - [Balanced cut-vector distance formula](#balanced-cut-vector-distance-formula)
  - [Volumetric covering bound](#volumetric-covering-bound)
- [Unit disk](#unit-disk)
- [Cyclic quadrilateral](#cyclic-quadrilateral)
  - [Brahmagupta's formula](#brahmagupta-s-formula)
- [Locus (mathematics)](#locus-mathematics)
- [Conic section](#conic-section)
  - [Conic type discriminant](#conic-type-discriminant)
  - [Degenerate conic](#degenerate-conic)
  - [Directrix of a conic](#directrix-of-a-conic)
  - [Focus of a conic](#focus-of-a-conic)
  - [Eccentricity of a conic](#eccentricity-of-a-conic)
  - [Semilatus rectum](#semilatus-rectum)
  - [Parabola](#parabola)
    - [Vertex of a parabola](#vertex-of-a-parabola)
  - [Hyperbola](#hyperbola)
    - [Rectangular hyperbola](#rectangular-hyperbola)
    - [Hyperbolic parametrization of a hyperbola](#hyperbolic-parametrization-of-a-hyperbola)
    - [Focal-distance identity for a hyperbola](#focal-distance-identity-for-a-hyperbola)
  - [Ellipse](#ellipse)
    - [Steiner inellipse](#steiner-inellipse)
    - [Affine image of a circle](#affine-image-of-a-circle)
    - [Semi-major and semi-minor axes](#semi-major-and-semi-minor-axes)
    - [Ellipse perimeter expansion near a circle](#ellipse-perimeter-expansion-near-a-circle)
    - [Nondegenerate ellipse](#nondegenerate-ellipse)
      - [Parity and upper bound for transverse ellipse intersections](#parity-and-upper-bound-for-transverse-ellipse-intersections)
    - [Focal line](#focal-line)
- [Ellipsoid](#ellipsoid)
  - [Nearest points to the origin on a positive-definite ellipsoid](#nearest-points-to-the-origin-on-a-positive-definite-ellipsoid)
  - [Solid ellipsoid](#solid-ellipsoid)
    - [Cartesian second moment of a solid ellipsoid](#cartesian-second-moment-of-a-solid-ellipsoid)
  - [John ellipsoid](#john-ellipsoid)
    - [John contact decomposition](#john-contact-decomposition)
    - [John position](#john-position)
  - [Coordinate-projection atlas of an ellipsoid](#coordinate-projection-atlas-of-an-ellipsoid)
  - [Two-chart smooth atlas of an ellipsoid](#two-chart-smooth-atlas-of-an-ellipsoid)
  - [Spheroid](#spheroid)
    - [Prolate spheroid](#prolate-spheroid)
      - [Intersection of a prolate spheroid and a concentric sphere](#intersection-of-a-prolate-spheroid-and-a-concentric-sphere)
- [Perpendicular bisector](#perpendicular-bisector)
  - [Circumcenter](#circumcenter)
- [Skew lines](#skew-lines)
  - [Distance between skew lines](#distance-between-skew-lines)
- [Circles of Apollonius](#circles-of-apollonius)
- [Right angle](#right-angle)
- [Rigid transformation](#rigid-transformation)
  - [Point reflection](#point-reflection)
- [Thales's theorem](#thales-s-theorem)
- [Regular polygon](#regular-polygon)
  - [Area of a regular octagon](#area-of-a-regular-octagon)
- [Spherical cap](#spherical-cap)
  - [Mass of a spherical cap with height-proportional density](#mass-of-a-spherical-cap-with-height-proportional-density)
  - [Curved area of a spherical cap](#curved-area-of-a-spherical-cap)
  - [Volume of a spherical cap](#volume-of-a-spherical-cap)
  - [Spherical cap area upper bound](#spherical-cap-area-upper-bound)
- [Lattice polygon](#lattice-polygon)
- [Isoperimetric inequality](#isoperimetric-inequality)
  - [Planar isoperimetric inequality](#planar-isoperimetric-inequality)
    - [Maximum-area circular segment with fixed arc length and chord](#maximum-area-circular-segment-with-fixed-arc-length-and-chord)
    - [Hurwitz proof of the planar isoperimetric inequality](#hurwitz-proof-of-the-planar-isoperimetric-inequality)
    - [Circle equality in the planar isoperimetric inequality](#circle-equality-in-the-planar-isoperimetric-inequality)

## Straightedge and compass construction

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

[This section is present in another page, follow this link to view it.](straightedge-and-compass-construction.md)

## Dihedral angle

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dihedral_angle)

The [dihedral angle](#dihedral-angle) measures the angle between two intersecting planes. Molecular [torsion angles](#torsion-angle) use an oriented four-atom convention to specify a related signed angle.

### Torsion angle

↑ **Parent:** [Dihedral angle](#dihedral-angle)

For four consecutively bonded atoms A–B–C–D, the [torsion angle](#torsion-angle) is the signed dihedral between planes A–B–C and B–C–D. State the viewing and sign convention when comparing projections.

## Sylvester-Gallai theorem

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

## Geometric scale factor

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

The ratio between corresponding lengths of two geometrically similar figures. Multiplying every length by $t>0$ multiplies areas by $t^2$ and volumes by $t^3$. For [integer](integer.md)-sided [triangles](#triangle), choosing a [positive integer](integer.md#positive-integer) scale factor preserves [integer](integer.md) side lengths.

## Perpendicular lines

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

Two intersecting [straight lines](#straight-line) are perpendicular if their angle is $90^\circ$. Their [direction vectors](#direction-vector) have zero [dot product](inner-product.md#dot-product).

## Cone (geometry)

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cone)

A geometric cone joins a fixed [point](geometry-and-topology.md#point-geometry) to points of a [plane curve](algebraic-geometry.md#plane-curve) by straight [lines](#straight-line). A circular cone uses a [circle](topology.md#circle) as that curve; its solid version includes the enclosed circular cross-sections. For a right circular cone of height $h$ and base radius $R$, the cross-section radius varies linearly along the axis, and its [volume](geometry-and-topology.md#volume) is $\pi R^2h/3$ by [integration](integral.md). An [elliptic cone](#elliptic-cone) allows elliptical cross-sections. The construction differs from the abstract [topological cone](algebraic-topology.md#cone-topology), which does not specify lengths or angles.

### Optimal cylinder inscribed in a cone

↑ **Parent:** [Cone (geometry)](#cone-geometry)

For a coaxial cylinder standing on the base of a right circular [cone](#cone-geometry) of height $h>0$ and semi-vertical [angle](geometry-and-topology.md#angle) $0<\alpha<\pi/2$, similar triangles give radius $r=(h-x)\tan\alpha$ at cylinder height $x$. Its [volume](geometry-and-topology.md#volume) is $V=\pi x(h-x)^2\tan^2\alpha$. Differentiation gives $V'=\pi\tan^2\alpha(h-x)(h-3x)$, so the unique positive-volume [maximum](set.md#maximum-of-a-subset-of-a-total-order) has $x=h/3$ and occupies $4/9$ of the cone's [volume](geometry-and-topology.md#volume). Its curved [surface area](differential-geometry.md#surface-area) is instead $A=2\pi x(h-x)\tan\alpha$, maximized at $x=h/2$. Changing the optimized quantity changes the optimal shape, even though the geometric constraint is identical.

## Collinearity

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Collinearity)

Points are collinear when they lie on a single [line](#straight-line). Two [vectors](vector-space.md#vector) are collinear when their [linear span](vector-space.md#linear-span) has [dimension](vector-space.md#dimension-vector-space) at most one. For a nonzero vector $v$, this means that the other vector is $\lambda v$ for some [scalar](vector-space.md#scalar) $\lambda$. This algebraic convention includes the zero vector; the directional use of “parallel” sometimes assumes both vectors are nonzero.

## Quadric surface

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A quadric surface in three-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm) is the zero set of a real [polynomial](polynomial.md) of degree two. Its quadratic part can be written with a [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$, since the [antisymmetric matrix](linear-algebra.md#skew-symmetric-matrix) part contributes zero to $x^TAx$. An [orthogonal diagonalization](linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) and a [translation](geometry-and-topology.md#translation-geometry) expose its geometry: examples include an [ellipsoid](#ellipsoid), an [elliptic cone](#elliptic-cone), and a [hyperboloid](differential-geometry.md#hyperboloid). This affine geometric description allows singular surfaces such as a cone's vertex.

### Parabolic cylinder

↑ **Parent:** [Quadric surface](#quadric-surface)

A [quadric surface](#quadric-surface) obtained by extending a [parabola](#parabola) along a fixed direction outside its plane. For example, $x=c-y^2/(4c)$ with arbitrary $z$ is a parabolic cylinder parallel to the $z$ axis. Each cross-section of fixed $z$ has vertex $(c,0)$ and focus $(0,0)$ in its $xy$ plane. It occurs as a coordinate surface in [parabolic cylindrical coordinates](multivariable-calculus.md#parabolic-cylindrical-coordinates).

### Distance extrema on a real quadratic surface

↑ **Parent:** [Quadric surface](#quadric-surface)

For a real [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$, every stationary squared distance $x^Tx$ on $x^TAx=1$ occurs in a positive-[eigenvalue](linear-operator-theory.md#eigenvalue) [eigenspace](linear-operator-theory.md#eigenspace). The [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) equation is $x=\Lambda Ax$; multiplying by $x^T$ gives $\Lambda=|x|^2>0$, hence $Ax=|x|^{-2}x$. If $A$ is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix), the nearest and farthest squared distances are $1/\lambda_{\max}$ and $1/\lambda_{\min}$. With a repeated [eigenvalue](linear-operator-theory.md#eigenvalue), the stationary set may contain an entire sphere within its [eigenspace](linear-operator-theory.md#eigenspace). For an indefinite or singular form the surface may be unbounded, and a stationary point need not be a global extremum.

#### Distance extrema on a central plane section of an ellipsoid

↑ **Parent:** [Distance extrema on a real quadratic surface](#distance-extrema-on-a-real-quadratic-surface)

Let $A$ be a real [positive-definite matrix](quadratic-form.md#positive-definite-matrix) and let the columns of $U$ be an [orthonormal basis](inner-product.md#orthonormal-basis) of a two-dimensional [linear subspace](vector-space.md#vector-subspace) in three-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm). Points in that central plane are $x=Uq$, with $|x|^2=|q|^2$. Restricting the [ellipsoid](#ellipsoid) $x^TAx=1$ gives $q^T(U^TAU)q=1$. The compressed [matrix](vector-space.md#matrix) $U^TAU$ is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix), and its extreme [eigenvalues](linear-operator-theory.md#eigenvalue) give the distance formulas in the title by the [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient). The two extremal axes are the images under $U$ of the corresponding [eigenvectors](linear-operator-theory.md#eigenvector). This restriction reduces a problem with two [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) to a two-dimensional [quadratic form](quadratic-form.md).

### Hyperbolic cylinder

↑ **Parent:** [Quadric surface](#quadric-surface)

For $a,b>0$, this [quadric surface](#quadric-surface) is independent of its third coordinate and is formed by translating a [hyperbola](#hyperbola) along that direction. Its two connected components correspond to $u\geq a$ and $u\leq-a$. In [elliptic cylindrical coordinates](multivariable-calculus.md#elliptic-cylindrical-coordinates), fixing a generic angular coordinate selects a half-branch of such a cylinder because the signs of both planar coordinates are fixed by that angular value.

### Elliptic cylinder

↑ **Parent:** [Quadric surface](#quadric-surface)

For $a,b>0$, an elliptic cylinder is a [quadric surface](#quadric-surface) with the displayed equation in suitable [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system), independent of the third coordinate. It is formed by translating an [ellipse](#ellipse) parallel to a line perpendicular to its plane. The generator direction is the zero-eigenvalue direction of its quadratic part, while the transverse semiaxes are $a,b$. It is circular if $a=b$.

### Signature transition from an ellipsoid to an elliptic cylinder and a one-sheet hyperboloid

↑ **Parent:** [Quadric surface](#quadric-surface)

After an [orthogonal diagonalization](linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix), the sign of the third coefficient classifies the displayed [quadric surface](#quadric-surface). If $C>0$, it is an [ellipsoid](#ellipsoid) with semiaxes $A^{-1/2},B^{-1/2},C^{-1/2}$. If $C=0$, it is an elliptic cylinder parallel to the $w$ axis, with elliptical transverse section. If $C<0$, it is a [one-sheet hyperboloid](differential-geometry.md#one-sheet-hyperboloid) with axis $w$ and waist ellipse $Au^2+Bv^2=1$. The continuous limit $C\to0$ sends the associated axial length scale to infinity. Repeated positive eigenvalues make the corresponding principal-axis choices nonunique within their eigenspace, without changing the surface.

### Elliptic cone

↑ **Parent:** [Quadric surface](#quadric-surface)

An elliptic cone is a real [quadric surface](#quadric-surface) consisting of the two nappes $u=\pm\sqrt{(bv^2+cw^2)/a}$, joined at the vertex. Its intersections with planes $u=u_0\ne0$ are [ellipses](#ellipse). It is the zero level of an indefinite [quadratic form](quadratic-form.md) of [signature](quadratic-form.md#signature-of-a-quadratic-form) $(1,2)$. Changing the level to a positive value produces a [two-sheeted hyperboloid](differential-geometry.md#two-sheeted-hyperboloid); changing it to a negative value produces a [one-sheet hyperboloid](differential-geometry.md#one-sheet-hyperboloid), when the positive coefficient is assigned to the axial coordinate $u$.

## Center (geometry)

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

The center of a [circle](topology.md#circle) or [sphere](#sphere) is the unique point $\mathbf c$ at the fixed positive [radius](topology.md#radius) $R$ from every point of that [circle](topology.md#circle) or [sphere](#sphere). In [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system), its equation is $|\mathbf x-\mathbf c|^2=R^2$. In the [complex plane](complex-analysis.md#complex-plane), a [circle](topology.md#circle) has equation $|z-c|^2=R^2$; [completing the square](polynomial.md#completing-the-square) identifies $c$ as its center. For example, $|z+b|^2=R^2$ has center $-b$.

## Distance between parallel lines

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

For two parallel [lines](#straight-line) $\mathbf a_1+s\mathbf v$ and $\mathbf a_2+t\mathbf v$ in three-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm), with $\mathbf v\ne0$ and $\mathbf d=\mathbf a_2-\mathbf a_1$, their shortest distance is

$$
\boxed{d=\left\|\mathbf d-\frac{\mathbf d\cdot\mathbf v}{\mathbf v\cdot\mathbf v}\mathbf v\right\|=\frac{\|\mathbf d\times\mathbf v\|}{\|\mathbf v\|}.}
$$

Every joining displacement is $\mathbf d+(t-s)\mathbf v$. Its component perpendicular to $\mathbf v$ is fixed, and its parallel component can be cancelled by a suitable $t-s$. The [Pythagorean theorem](#pythagorean-theorem) proves that this perpendicular component has the shortest [Euclidean norm](normed-vector-space.md#euclidean-norm). The [cross product](vector-space.md#cross-product) expression follows from $\|\mathbf d\times\mathbf v\|=\|\mathbf d\|\|\mathbf v\|\sin\theta$. For coincident [lines](#straight-line) the distance is zero. The perpendicular-component formula also applies in any finite-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm), where a three-dimensional [cross product](vector-space.md#cross-product) need not be available.

## Square grid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

Two equally spaced families of perpendicular [lines](#straight-line) partitioning the [Euclidean plane](geometry-and-topology.md#euclidean-plane) into congruent [squares](#square). A general [affine map](geometry-and-topology.md#affine-map) can turn this grid into [parallelograms](#parallelogram), or collapse directions if its [linear part of an affine map](geometry-and-topology.md#linear-part-of-an-affine-map) is not [injective](algebra.md#injective-function).

## Parallel postulate

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallel_postulate)

In the [Euclidean plane](geometry-and-topology.md#euclidean-plane), precisely one line through a point outside a given line is parallel to it. This formulation is equivalent to Euclid's fifth postulate within the usual axioms of plane geometry.

<h2 id="euclid-s-elements">Euclid's Elements</h2>

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid's_Elements)

## Congruence (geometry)

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Congruence_(geometry))

Figures are [congruent](#congruence-geometry) when a [rigid motion](#rigid-transformation) maps one onto the other, preserving all [Euclidean distances](topological-analysis.md#euclidean-distance).

### Geometric congruence class

↑ **Parent:** [Congruence (geometry)](#congruence-geometry)

## Right circular conical surface

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

This [surface](topological-surface.md) consists of rays from a vertex $\mathbf a$ whose directions make a fixed angle $\beta$ with a unit axis [vector](vector-space.md#vector) $\widehat{\mathbf n}$. The displayed equation follows from the [dot product](inner-product.md#dot-product) formula for that angle. For $0<\beta<\pi$, $\beta\ne\pi/2$, it gives one circular nappe; $\beta=\pi/2$ gives a [plane](geometry-and-topology.md#plane), and $\beta=0,\pi$ gives a degenerate ray. Squaring the equation produces both nappes, so the unsquared sign distinguishes them. [Generalized angular momentum in a radial monopole field](momentum.md#generalized-angular-momentum-in-a-radial-monopole-field) confines particle directions to such a surface.

## Euclidean group

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_group)

The [Euclidean group](#euclidean-group) $E(n)=O(n)\ltimes\mathbb R^n$ is the [group](group.md) of all [isometries](riemannian-geometry.md#isometry) $x\mapsto Ax+b$ of [Euclidean space](normed-vector-space.md#euclidean-norm), with $A$ an [orthogonal matrix](linear-algebra.md#orthogonal-matrix). Its orientation-preserving [subgroup](group.md#subgroup) is $SE(n)=SO(n)\ltimes\mathbb R^n$, the [semidirect product](group-theory.md#semidirect-product) of the [special orthogonal group](linear-algebra.md#special-orthogonal-group) with translations. The [Euclidean motion of Euclidean three-space](differential-geometry.md#euclidean-motion-of-euclidean-three-space) and the [proper Euclidean motion of Euclidean three-space](differential-geometry.md#proper-euclidean-motion-of-euclidean-three-space) are the respective three-dimensional instances.

## Geometric locus

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A [geometric locus](#geometric-locus) is the [set](set.md) of points satisfying a specified geometric or algebraic condition in an ambient space. For example, points at a fixed positive distance $r$ from $p$ form a [circle](topology.md#circle) in the plane and a [sphere](#sphere) in three dimensions. In the [complex plane](complex-analysis.md#complex-plane), $|z-z_0|=r$ has Cartesian equation $(x-\operatorname{Re}z_0)^2+(y-\operatorname{Im}z_0)^2=r^2$, proving the [circle](topology.md#circle) description. A locus can also be a union, such as $x(y-1)=0$, which consists of two lines; domain restrictions in the original equation must be retained when simplifying it.

## Hypercube

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypercube)

A hypercube is the Cartesian product of $n$ equal-length closed intervals in [Euclidean space](normed-vector-space.md#euclidean-norm). The centered cube $[-1,1]^n$ has $2^n$ vertices, each with coordinates in $\{-1,1\}$. Antipodal vertices determine $2^{n-1}$ body diagonals.

### Orthogonality of hypercube body diagonals

↑ **Parent:** [Hypercube](#hypercube)

Two sign-vector vertices of a centered [hypercube](#hypercube) differing in $h$ coordinates have [dot product](inner-product.md#dot-product) $n-2h$. Thus their body diagonals can be [orthogonal](inner-product.md#orthogonal-vectors) only in even dimension. A collection of mutually [orthogonal](inner-product.md#orthogonal-vectors) nonzero diagonals has at most $n$ members; achieving $n$ is equivalent to the existence of a [Hadamard matrix](vector-space.md#hadamard-matrix) of order $n$. For unoriented lines the angle is determined by $|n-2h|/n$, while oriented vertex vectors retain the sign of their [dot product](inner-product.md#dot-product).

## Centroid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Centroid)

### Integral of an affine function over a simplex

↑ **Parent:** [Centroid](#centroid)

For a nondegenerate $d$-dimensional [simplex](algebraic-topology.md#simplex) $S$ with vertices $v_0,\ldots,v_d$ and an [affine function](vector-space.md#affine-function) $f$, the integral equals the volume times the value at the [centroid](#centroid) $c=(v_0+\cdots+v_d)/(d+1)$. To prove this, write $x=\sum_i\lambda_i(x)v_i$ in a [barycentric coordinate system](algebraic-topology.md#barycentric-coordinate-system). On the standard simplex, symmetry permuting the vertices gives equal integrals of all $\lambda_i$; since $\sum_i\lambda_i=1$, each is $\operatorname{vol}(S)/(d+1)$. An invertible [affine map](geometry-and-topology.md#affine-map) transfers this result to any simplex. Affineness gives $f(x)=\sum_i\lambda_i(x)f(v_i)$, so [linearity of integration](integral.md#linearity-of-integration) proves the formula. For a tetrahedron the factor is one quarter. The rule is exact for affine integrands; a nonlinear integrand generally needs additional moments.

## Polygon

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polygon)

### Dodecagon

↑ **Parent:** [Polygon](#polygon)

### Regular star polygon

↑ **Parent:** [Polygon](#polygon)

A regular star polygon $\{p/q\}$ joins every $q$-th vertex of a regular $p$-gon. When $\gcd(p,q)=1$, this traces one closed polygonal circuit.

### Cyclic polygon

↑ **Parent:** [Polygon](#polygon)

### Shoelace formula

↑ **Parent:** [Polygon](#polygon)

For a simple [polygon](#polygon) with cyclically ordered [vertices of a polygon](#vertex-of-a-polygon) $(x_i,y_i)$, its signed area is $\tfrac12\sum_i(x_i y_{i+1}-x_{i+1}y_i)$, with indices read cyclically. Reversing the traversal changes the sign; taking the absolute value gives the area. Each summand is a two-dimensional [determinant](multilinear-algebra.md#determinant).

### Kernel of a polygon

↑ **Parent:** [Polygon](#polygon)

### Polygon inequality

↑ **Parent:** [Polygon](#polygon)

Positive [real number](arithmetic.md#real-number) lengths $a_1,\ldots,a_k$, with $k\ge3$, are the sides of a nondegenerate [polygon](#polygon) exactly when $2\max_i a_i<\sum_i a_i$. Necessity follows from the [triangle inequality](topological-analysis.md#triangle-inequality): the longest side must be shorter than the path formed by the remaining sides.

### Semiperimeter

↑ **Parent:** [Polygon](#polygon)

The semiperimeter is half the [perimeter](inverse-problem.md#perimeter). For a [triangle](#triangle) with side lengths $a,b,c$, it is $s=(a+b+c)/2$.

### Perimeter of a polygon

↑ **Parent:** [Polygon](#polygon)

The [sum](arithmetic.md#sum) of the lengths of its [sides of a polygon](#side-of-a-polygon). For a [triangle](#triangle) with side lengths $a,b,c$, the [perimeter of a polygon](#perimeter-of-a-polygon) is $a+b+c$.

### Pentagon

↑ **Parent:** [Polygon](#polygon)

A [polygon](#polygon) with five sides and five vertices. A regular pentagon has equal sides and angles; its [symmetry group](group-action.md#symmetry-group) is the order-ten [dihedral group](finite-group-theory.md#dihedral-group), consisting of five rotations and five reflections. Each reflection axis passes through a vertex and the midpoint of the opposite edge.

### Hexagon

↑ **Parent:** [Polygon](#polygon)

A [polygon](#polygon) with six sides and six vertices. A regular [hexagon](#hexagon) has equal sides and angles, with each interior angle equal to $2\pi/3$. Its [symmetry group](group-action.md#symmetry-group) consists of six rotations and six reflections, forming a [dihedral group](finite-group-theory.md#dihedral-group) of order twelve.

#### Regular hexagon

↑ **Parent:** [Hexagon](#hexagon)

### Vertex of a polygon

↑ **Parent:** [Polygon](#polygon)

A [vertex of a polygon](#vertex-of-a-polygon) is an endpoint where consecutive [sides of a polygon](#side-of-a-polygon) meet.

### Side of a polygon

↑ **Parent:** [Polygon](#polygon)

A [side of a polygon](#side-of-a-polygon) is a [line segment](convex-set.md#line-segment) joining two consecutive [vertices of a polygon](#vertex-of-a-polygon) in its boundary.

### Diagonal of a polygon

↑ **Parent:** [Polygon](#polygon)

A [diagonal of a polygon](#diagonal-of-a-polygon) joins two [vertices of a polygon](#vertex-of-a-polygon) that are not endpoints of the same [side of a polygon](#side-of-a-polygon). A [square](#square) has two [diagonals of a polygon](#diagonal-of-a-polygon), forming a two-element [group orbit](group-action.md#orbit-group-theory) under its [dihedral group](finite-group-theory.md#dihedral-group) of symmetries.

### Quadrilateral

↑ **Parent:** [Polygon](#polygon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadrilateral)

#### Convex quadrilateral

↑ **Parent:** [Quadrilateral](#quadrilateral)

#### Rectangle

↑ **Parent:** [Quadrilateral](#quadrilateral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rectangle)

A Euclidean [polygon](#polygon) with four sides and four right angles. Opposite sides are parallel and have equal lengths. A rectangle is a [square](#square) exactly when its adjacent side lengths agree.

##### Square

↑ **Parent:** [Rectangle](#rectangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square)

A [rectangle](#rectangle) with all four side lengths equal. It is a regular four-sided [polygon](#polygon). Rotations and translations preserve this definition; its sides need not be parallel to the coordinate axes.

###### Square lamina

↑ **Parent:** [Square](#square)

A square frame formed by removing a concentric square hole from a larger [square](#square). If outer and inner sides are [positive integers](integer.md#positive-integer) $a>b$ with the same [integer parity](integer.md#parity-mathematics), the border has [integer](integer.md) thickness $t=(a-b)/2$ and contains $a^2-b^2=4t(b+t)$ unit tiles.

###### Unit square

↑ **Parent:** [Square](#square)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_square)

The [unit square](#unit-square) here is the [Cartesian product](set-theory.md#cartesian-product) $[0,1]\times[0,1]$ in the [Euclidean plane](geometry-and-topology.md#euclidean-plane), a [square](#square) of side length one.

#### Parallelogram

↑ **Parent:** [Quadrilateral](#quadrilateral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallelogram)

A parallelogram is the [convex set](convex-set.md) with vertices $p,p+u,p+v,p+u+v$ for two linearly independent planar vectors $u,v$. Its opposite edges are parallel and its centre $p+(u+v)/2$ gives central symmetry. Its area is $|\det[u,v]|$, so an invertible linear map changes its area by the absolute value of that map's [determinant](multilinear-algebra.md#determinant). These facts make parallelograms convenient convex bodies for two-dimensional applications of the [Minkowski convex body theorem](algebraic-number-theory.md#minkowski-s-theorem).

<h4 id="bretschneider-s-formula">Bretschneider's formula</h4>

↑ **Parent:** [Quadrilateral](#quadrilateral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bretschneider's_formula)

For a quadrilateral with side lengths $a,b,c,d$, semiperimeter $s$, area $K$, and opposite angles $A,C$,

$$
K^2=(s-a)(s-b)(s-c)(s-d)-abcd\cos^2\frac{A+C}{2}.
$$

The second term vanishes exactly when $A+C=\pi$, which is the cyclicity condition for a nondegenerate convex quadrilateral.

## Point group

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Point_group)

The [point group](#point-group) of a Euclidean crystallographic group is the group of its orthogonal linear parts, equivalently its quotient by the translation subgroup. It preserves the translation [Euclidean lattice](fourier-analysis.md#euclidean-lattice). In an arbitrary dimension it is a finite orthogonal group; for a [plane crystallographic group](#wallpaper-group) this lattice preservation restricts the allowed rotation orders.

<h3 id="neumann-s-principle">Neumann's principle</h3>

↑ **Parent:** [Point group](#point-group)

A physical property [tensor](multilinear-algebra.md#tensor) must be invariant under every symmetry operation of the material's [point group](#point-group). For a polar rank-$r$ [tensor](multilinear-algebra.md#tensor), $T_{i_1\ldots i_r}=R_{i_1j_1}\cdots R_{i_rj_r}T_{j_1\ldots j_r}$. Taking $R=-I$ proves that an odd-rank polar [tensor](multilinear-algebra.md#tensor) vanishes in a centrosymmetric material. A susceptibility of order $n$ has rank $n+1$, so local bulk even-order electric-dipole response is forbidden there. The name refers to [Franz Ernst Neumann](physicist.md#franz-ernst-neumann).

### Molecular symmetry

↑ **Parent:** [Point group](#point-group)

The spatial [symmetry](physics.md#symmetry-physics) of a fixed molecular geometry. Its [point group](#point-group) acts on atomic positions, orbitals and vibrational coordinates; these actions need not have the same [group representation](representation-theory.md#group-representation).

#### Symmetry coordinate

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

A linear combination of atomic displacements adapted to an [irreducible representation](representation-theory.md#irreducible-representation) of a [molecular point group](#molecular-point-group). [Symmetry coordinates](#symmetry-coordinate) reduce the [dynamical matrix](wave-equation.md#dynamical-matrix) into independent symmetry blocks; several coordinates in the same block can still mix.

#### D infinity h molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The [molecular point group](#molecular-point-group) of a centrosymmetric linear [molecule](molecule.md). Longitudinal coordinates have $\Sigma$ symmetry; their behaviour under inversion about the [inversion centre](physics.md#inversion-centre) supplies the $g$ or $u$ label, and a vertical reflection supplies the sign on a $\Sigma$ representation.

#### C4v molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The eight-operation [molecular point group](#molecular-point-group) of an ideal square pyramid. Its polar-vector components transform as $A_1$ for the principal-axis coordinate and $E$ for the transverse pair. Symmetric quadratic functions also contain $B_1$ and $B_2$, allowing [Raman spectroscopy](optics.md#raman-spectroscopy) activity beyond the [infrared](optics.md#infrared) modes.

#### Symmetry operation

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

A transformation that preserves a specified structure, including the chemical identity of sites in a [molecule](molecule.md). Rotations, reflections, inversion and improper rotations can occur in a [molecular point group](#molecular-point-group). The associated action on [atomic orbitals](chemistry.md#atomic-orbital) also changes their orientations and signs, which must be included when computing a [character of a representation](representation-theory.md#character-of-a-representation).

#### Molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The [point group](#point-group) of orthogonal spatial transformations that preserve a fixed [molecular geometry](molecule.md#molecular-geometry), including the positions and chemical identities of all nuclei. Changing a conformation can change the [molecular point group](#molecular-point-group) even when the molecular connectivity is unchanged. Its [group representations](representation-theory.md#group-representation) on [atomic orbitals](chemistry.md#atomic-orbital) depend on orbital signs and rotations as well as the permutation of centres.

#### C2h molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The [molecular point group](#molecular-point-group) containing identity, one twofold rotation, an [inversion centre](physics.md#inversion-centre) and a mirror plane perpendicular to the twofold axis. Its four operations are $E,C_2,i,\sigma_h$. An extended anti conformation of [hexa-1,5-diyne](chemical-substance.md#hexa-1-5-diyne) provides an example; changing the conformation can change the [symmetry](physics.md#symmetry-physics).

#### C3v molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The six-operation molecular [point group](#point-group) with a threefold proper rotation axis and three vertical mirror planes. Its [rotational symmetry number](molecule.md#rotational-symmetry-number) is three because mirror operations do not count as proper spatial rotations.

#### D6h molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The 24-operation molecular [point group](#point-group) of a regular planar hexagon with equivalent sites. Its [irreducible representations](representation-theory.md#irreducible-representation) have inversion labels $g,u$; polar-vector components transform as $A_{2u}$ for $z$ and $E_{1u}$ for $(x,y)$.

#### Td molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The 24-operation molecular [point group](#point-group) of an ideal regular [tetrahedron](#tetrahedron), including improper operations. Its [irreducible representations](representation-theory.md#irreducible-representation) are $A_1,A_2,E,T_1,T_2$, with dimensions $1,1,2,3,3$. The polar-vector representation is $T_2$, the axial-vector representation is $T_1$, and symmetric quadratic functions transform as $A_1+E+T_2$.

##### Methane normal-mode representation

↑ **Parent:** [Td molecular point group](#td-molecular-point-group)

The 15 Cartesian displacements of tetrahedral methane have characters $(15,0,-1,-1,3)$ on classes $(E,8C_3,3C_2,6S_4,6\sigma_d)$. Removing translations $T_2$ and rotations $T_1$ gives $(9,0,1,-1,3)$ and the stated decomposition. There are nine vibrational coordinates in four frequency families.

#### Infrared and Raman mutual exclusion

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

In a centrosymmetric molecule, a fundamental vibration cannot be both electric-dipole [infrared](optics.md#infrared) active and ordinary [Raman spectroscopy](optics.md#raman-spectroscopy) active. Dipole components are odd under inversion; polarizability components are even. This selection rule concerns modes, not accidental numerical equality of unrelated frequencies.

#### Molecular character reduction

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

For a finite molecular [point group](#point-group), the multiplicity of irrep $\lambda$ in a representation with character $\chi$ is $n_\lambda=|G|^{-1}\sum_C |C|\chi(C)\chi_\lambda(C)^*$. The sum is over [conjugacy classes](group-action.md#conjugacy-class).

#### Symmetry-closed orbital basis

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

An orbital set whose span is invariant under every [molecular symmetry operation](#molecular-symmetry-operation). Completeness here means closure of the chosen representation space; it does not mean that a finite orbital set spans the entire electronic Hilbert space.

#### Ih molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The full icosahedral molecular [point group](#point-group), including inversion, with 120 operations. Its single-valued orbital [irreducible representations](representation-theory.md#irreducible-representation) have dimensions 1, 3, 3, 4 and 5 in each inversion parity.

#### D4h molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The sixteen-element molecular [point group](#point-group) of an ideal square with a horizontal mirror plane. Inversion distinguishes gerade and ungerade [irreducible representations](representation-theory.md#irreducible-representation).

#### D3h molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The twelve-element molecular [point group](#point-group) of an ideal trigonal bipyramid. Reflection in its equatorial plane distinguishes primed and double-primed [irreducible representations](representation-theory.md#irreducible-representation).

#### D2d molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

An eight-element molecular [point group](#point-group) with classes $E,2S_4,C_2,2C_2^\prime,2\sigma_d$. The vector representation decomposes as $B_2+E$.

#### C2v molecular point group

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

The four-element molecular [point group](#point-group) with one twofold axis and two mirror planes containing that axis. [Water](chemical-substance.md#water) has this symmetry at its equilibrium bent geometry.

#### Molecular symmetry operation

↑ **Parent:** [Molecular symmetry](#molecular-symmetry)

A rotation, reflection, inversion or improper rotation that carries a fixed molecular geometry into an indistinguishable configuration. Products of such operations must also be symmetries.

### D2h point group

↑ **Parent:** [Point group](#point-group)

A molecular [point group](#point-group) containing identity, three mutually perpendicular twofold rotations, inversion, and three mirror reflections. In the conventional axis labelling, $z\sim B_{1u}$, $y\sim B_{2u}$ and $x\sim B_{3u}$; $yz\sim B_{3g}$ and $xz\sim B_{2g}$. The symmetry of a perpendicular atomic $p$ orbital includes its sign reversal when an operation reverses its axis, in addition to any permutation of atomic centres.

### C2v point group

↑ **Parent:** [Point group](#point-group)

A molecular [point group](#point-group) with identity, one twofold axis, and two mirror planes containing that axis. With the twofold axis along $z$, its one-dimensional irreducible representations have Cartesian bases $z\sim A_1$, $x\sim B_1$, and $y\sim B_2$. For [formaldehyde](chemical-substance.md#formaldehyde) in the $xz$ plane, the vibrational representation is $3A_1+2B_1+B_2$.

### Crystallographic restriction theorem

↑ **Parent:** [Point group](#point-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crystallographic_restriction_theorem)

A rotation preserving a rank-two [lattice](mathematical-logic.md#lattice) has order $1,2,3,4$ or $6$. In a lattice basis its matrix is integral, while its trace is $2\cos\theta$. The only integral values in $[-2,2]$ are $-2,-1,0,1,2$, which give precisely those rotation orders. Finiteness of a symmetry group alone would not impose this restriction.

## Wallpaper group

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wallpaper_group)

A [plane crystallographic group](#wallpaper-group) is a discrete group of Euclidean plane isometries with compact quotient. Its translation subgroup is a rank-two [lattice](mathematical-logic.md#lattice), and the quotient by translations is its finite [point group](#point-group). This separates the periodic translational geometry from the finite rotational and reflection symmetries.

## Elliptic paraboloid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

An elliptic paraboloid is a smooth bowl-shaped quadratic surface with elliptical horizontal sections. In the circular case $A=B$, it is a [surface of revolution](differential-geometry.md#surface-of-revolution). For $z=x^2+y^2$, polar coordinates give the parametrization $(r\cos\theta,r\sin\theta,r^2)$ and upward [vector area element](differential-geometry.md#vector-area-element) $(-2r^2\cos\theta,-2r^2\sin\theta,r)\,dr\,d\theta$. A band between two positive heights has two boundary circles and no cap.

### Volume and centroid of a parabolic cup

↑ **Parent:** [Elliptic paraboloid](#elliptic-paraboloid)

The solid $0\leq z\leq h$, $x^2+y^2\leq az$, with $a,h>0$, has horizontal slice area $\pi az$. Thus its [volume](geometry-and-topology.md#volume) is $\int_0^h\pi az\,dz=\pi ah^2/2$. For a positive constant [mass density](fluid-mechanics.md#density), rotational symmetry puts its [centre of mass](classical-mechanics.md#center-of-mass) on the vertical axis, and

$$
\bar z=\frac{\int_0^h z(\pi az)dz}{\int_0^h\pi az\,dz}=\frac{2h}{3}.
$$

The curved [surface area](differential-geometry.md#surface-area), excluding the horizontal opening, is $\pi a^2[(1+4h/a)^{3/2}-1]/6$. Parametrizing the [elliptic paraboloid](#elliptic-paraboloid) by $(r\cos\theta,r\sin\theta,r^2/a)$ gives the [area element of a surface](differential-geometry.md#area-element-of-a-surface) $r\sqrt{1+4r^2/a^2}\,dr\,d\theta$, with $0\leq r\leq\sqrt{ah}$, proving this last formula. It is also a translated and reflected specialization of [paraboloid sector surface measures](#paraboloid-sector-surface-measures).

### Paraboloid sector surface measures

↑ **Parent:** [Elliptic paraboloid](#elliptic-paraboloid)

For $h,R>0$ and $0<\alpha\leq2\pi$, the curved sector $z=h(1-r^2/R^2)$, $0\leq r\leq R$, $0\leq\theta\leq\alpha$ has [volume](geometry-and-topology.md#volume) $\alpha hR^2/4$ beneath it. Its [surface area](differential-geometry.md#surface-area) is

$$
A=\frac{\alpha R^4}{12h^2}\left[\left(1+\frac{4h^2}{R^2}\right)^{3/2}-1\right].
$$

To derive this, parametrize the [surface](topological-surface.md) by $(r\cos\theta,r\sin\theta,h(1-r^2/R^2))$. The upward [vector area element](differential-geometry.md#vector-area-element) is $(2hr^2\cos\theta/R^2,2hr^2\sin\theta/R^2,r)\,dr\,d\theta$; its magnitude integrates to the stated [surface area](differential-geometry.md#surface-area). Its integral gives the [vector area](differential-geometry.md#vector-area)

$$
\mathbf S=\left(\frac{2hR}{3}\sin\alpha,\frac{2hR}{3}(1-\cos\alpha),\frac{\alpha R^2}{2}\right).
$$

In the shallow limit $h/R\to0$, the [surface area](differential-geometry.md#surface-area) is $\alpha R^2/2+\alpha h^2/2+O(h^4/R^2)$, approaching the area of its planar sector projection.

### Maximal cylinder and box in an elliptic paraboloid

↑ **Parent:** [Elliptic paraboloid](#elliptic-paraboloid)

For the rotational [elliptic paraboloid](#elliptic-paraboloid) $z=H(1-(x^2+y^2)/R^2)$ above $z=0$, allow inscribed shapes to touch the boundary. A coaxial [cylinder](geometry-and-topology.md#cylinder-geometry) of radius $r$ and height $h$ obeys $h+Hr^2/R^2=H$. Applying a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) to $\pi r^2h$ gives $h=Hr^2/R^2$, hence $h=H/2$ and $r=R/\sqrt2$.

A centred [rectangular parallelepiped](#rectangular-parallelepiped) with horizontal side lengths $a,b$ and height $c$ obeys $c+H(a^2+b^2)/(4R^2)=H$. The [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) equations for $abc$ give $a=b$ and $c=Ha^2/(2R^2)$, hence $a=b=R,c=H/2$. These yield the displayed maximal volumes; both positive stationary shapes are interior optima among the dimension variables, while their degenerate boundary shapes have zero volume. The cylinder's volume is $\pi/2$ times the box's. If strict containment in the open region is required, these are suprema approached by slightly smaller shapes rather than attained maxima.

## Double circular cone

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

The union of the two infinite lateral conical sheets meeting at a common vertex is a double circular cone. The displayed example has axis $z$ and semi-angle $\pi/4$. It is smooth away from the vertex, where its defining [gradient](multivariable-calculus.md#gradient) is nonzero. A [right circular cone](#right-circular-cone) truncated on one side is a related bounded solid; this surface includes both axial directions and has no base disks.

### Intersection plane of parallel congruent double cones

↑ **Parent:** [Double circular cone](#double-circular-cone)

Let two [double circular cones](#double-circular-cone) have vertices $a_1,a_2$, common unit axis $n$, and semi-angle $0<\alpha<\pi/2$. Put $Q=\cos^2\alpha\,I-nn^T$ and $b=a_1-a_2\ne0$. Their equations are $(x-a_i)^TQ(x-a_i)=0$. Subtracting cancels the common quadratic term, so every intersection point satisfies

$$
(Qb)\cdot\left(x-\frac{a_1+a_2}{2}\right)=0.
$$

Since $Q$ has eigenvalues $\cos^2\alpha$ perpendicular to $n$ and $-\sin^2\alpha$ along $n$, $Qb\ne0$. Thus the intersection is contained in a plane, possibly with an empty intersection. Its unit normal is $Qb/|Qb|$, with $|Qb|^2=|b|^2\cos^4\alpha+(n\cdot b)^2(1-2\cos^2\alpha)$. Degenerate endpoint semi-angles can make the normal vanish and must be treated separately.

## Geometric packing

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

Placement of geometric objects without interior overlap. A [packing fraction](#packing-fraction) measures how much area or [volume](geometry-and-topology.md#volume) they occupy. [Circle packing](#circle-packing) and [sphere packing](#sphere-packing) are examples.

### Triangular lattice packing of discs

↑ **Parent:** [Geometric packing](#geometric-packing)

A triangular array with nearest-centre spacing $2r$ has primitive cell area $2\sqrt3r^2$. Dividing the disc area $\pi r^2$ by that area gives packing fraction $\pi/(2\sqrt3)\simeq0.9069$.

### Sphere packing

↑ **Parent:** [Geometric packing](#geometric-packing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sphere_packing)

Arrangement of [spheres](#sphere) without interior overlap. The occupied [volume](geometry-and-topology.md#volume) fraction is its [packing fraction](#packing-fraction); it depends on the spatial arrangement and on the radii.

#### Hard-sphere model

↑ **Parent:** [Sphere packing](#sphere-packing)

A model assigning nonoverlapping [spheres](#sphere) to particles; contacts express geometric constraints. A crystallographic sublattice need not be physically close-packed even when its [Bravais lattice](quantum-scattering.md#bravais-lattice) is face-centred cubic.

#### Simple-cubic sphere packing

↑ **Parent:** [Sphere packing](#sphere-packing)

Equal spheres of radius $r$ occupy the sites of a cubic lattice of spacing $2r$. A cell contains one sphere, so its [packing fraction](#packing-fraction) is $(4\pi r^3/3)/(2r)^3=\pi/6$. This is an ideal arranged deposit rather than a claim about all settling suspensions.

### Circle packing

↑ **Parent:** [Geometric packing](#geometric-packing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circle_packing)

Arrangement of [circles](topology.md#circle) in a plane without interior overlap. The covered area fraction is its [packing fraction](#packing-fraction). Equal-radius square packing has fraction $\pi/4$.

#### Descartes' circle theorem

↑ **Parent:** [Circle packing](#circle-packing)

Four mutually [tangent circles](topology.md#tangent-circles) with signed curvatures $k_i$ satisfy $(k_1+k_2+k_3+k_4)^2=2(k_1^2+k_2^2+k_3^2+k_4^2)$. Curvature is the reciprocal of the [radius](topology.md#radius), with an enclosing [circle](topology.md#circle) assigned negative curvature. Given three curvatures, solving the [quadratic equation](polynomial.md#quadratic-equation) gives $k_4=k_1+k_2+k_3\pm2\sqrt{k_1k_2+k_2k_3+k_3k_1}$, providing the two completions of the configuration.

#### Alternating-radius square circle packing

↑ **Parent:** [Circle packing](#circle-packing)

Place equal numbers of radii $r_1,r_2$ on alternating sites of a square nearest-neighbour lattice of spacing $d$. Nonoverlap requires $d\ge\max(r_1+r_2,\sqrt2r_1,\sqrt2r_2)$. A two-circle cell has area $2d^2$, giving the displayed [packing fraction](#packing-fraction). Its maximum within this geometry occurs at large-to-small radius ratio $1+\sqrt2$ and is $\pi(1-1/\sqrt2)$; smaller interstitial circles leave unused space, while larger ones force the large-circle lattice apart.

### Packing fraction

↑ **Parent:** [Geometric packing](#geometric-packing)

Occupied area or [volume](geometry-and-topology.md#volume) divided by the corresponding total area or [volume](geometry-and-topology.md#volume) of a [geometric packing](#geometric-packing). For a periodic packing, it is the total object area or [volume](geometry-and-topology.md#volume) within a repeat cell divided by the cell measure. It is distinct from the number fraction of objects of a given size.

## Euclidean ray

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A Euclidean ray from the origin with direction $v\ne0$ is the geometric half-line $\{tv:t\geq0\}$. Points in the strictly positive quadrant lie on rays with positive slope.

### Injectivity of sums on two distinct rays

↑ **Parent:** [Euclidean ray](#euclidean-ray)

If finite point sets $P,Q$ lie on two distinct [Euclidean rays](#euclidean-ray) in a plane, the map $(p,q)\mapsto p+q$ is [injective](algebra.md#injective-function) because the two direction vectors are [linearly independent](vector-space.md#linear-independence). Thus $|P+Q|=|P||Q|$. If all points are nonzero and the rays have positive slope, every sum lies in the [open planar sector](#open-planar-sector) between those rays.

### Open planar sector

↑ **Parent:** [Euclidean ray](#euclidean-ray)

The open planar sector between two distinct [Euclidean rays](#euclidean-ray) of positive slope consists of nonzero points whose directions lie strictly between their directions. Sectors between consecutive members of an ordered collection of [Euclidean rays](#euclidean-ray) are disjoint.

## Hyperbolic paraboloid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A hyperbolic paraboloid is a saddle-shaped quadric such as $z=xy$. Its graph parametrization $(x,y,xy)$ has [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) $-1/(1+x^2+y^2)^2$ and is regular everywhere. It is not a hyperboloid: their quadratic equations have different forms.

## Right circular cone

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A right circular cone has an axis through its apex and the centre of its circular base. With the axis chosen as the $z$ axis, its solid interior is $0\leq z\leq h$, $x^2+y^2\leq(z\tan\alpha)^2$, where $0<\alpha<\pi/2$ is the semi-angle. Its closed boundary includes both the lateral surface and the base [Euclidean disk](topology.md#disk-mathematics).

## Straight line

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)

A straight line in [Euclidean space](normed-vector-space.md#euclidean-norm) is the set $L=\{x_0+tv:t\in\mathbb R\}$, for a fixed point $x_0$ and nonzero direction [vector](vector-space.md#vector) $v$. Two distinct points determine one such line.

### Direction vector

↑ **Parent:** [Straight line](#straight-line)

A nonzero [vector](vector-space.md#vector) $d$ is a direction vector of a [line](#straight-line) if the [line](#straight-line) has a parametrization $r=p+td$, $t\in\mathbb R$, for some point $p$. Replacing $d$ by a nonzero [scalar multiple](vector-space.md#scalar-multiple) describes the same [line](#straight-line); dividing by its [Euclidean norm](normed-vector-space.md#euclidean-norm) gives a [unit vector](vector-space.md#unit-vector) in one of the two orientations. A [cross product](vector-space.md#cross-product) of two nonparallel [normal vectors](differential-geometry.md#normal-vector) supplies a direction vector for the intersection of their [planes](geometry-and-topology.md#plane).

### Slope

↑ **Parent:** [Straight line](#straight-line)

In Cartesian coordinates, the [slope](#slope) of a nonvertical [straight line](#straight-line) is its vertical change divided by its horizontal change. The graph $y=mx+c$ has [slope](#slope) $m$; a vertical [straight line](#straight-line) has no finite [slope](#slope). For a [tangent line](calculus.md#tangent-line) to a [differentiable function](analysis.md#differentiable-function), the [slope](#slope) is the [derivative](calculus.md#derivative).

### Secant line

↑ **Parent:** [Straight line](#straight-line)

A [secant line](#secant-line) is a [straight line](#straight-line) passing through two distinct points of a [curve](topology.md#curve). For a graph $y=f(x)$ at $x=a$ and $x=a+h$, its [slope](#slope) is the [difference quotient](calculus.md#difference-quotient) $(f(a+h)-f(a))/h$. As the second point approaches the first, a limiting [secant line](#secant-line) can give the [tangent line](calculus.md#tangent-line).

### Parametric equation of a straight line

↑ **Parent:** [Straight line](#straight-line)

A [straight line](#straight-line) through a point $a$ in nonzero direction $t$ is the set of vectors $r=a+st$ for real parameter $s$. If $|t|=1$, changes in the parameter equal signed distances along the line. Two such lines intersect exactly when their two parameter formulas give a common vector for some choice of their parameters.

## Polyhedron

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polyhedron)

A polyhedron is a three-dimensional solid assembled from polygonal faces meeting along edges and vertices.

### Bicapped square antiprism

↑ **Parent:** [Polyhedron](#polyhedron)

A ten-vertex cage formed by adding one cap over each square face of a square antiprism. Each axial cap is joined to four vertices in its nearer square; adjacent squares are rotated relative to each other. It is the usual idealized ten-vertex [closo cluster](molecule.md#closo-cluster) skeleton.

### Pentagonal bipyramid

↑ **Parent:** [Polyhedron](#polyhedron)

A seven-vertex [polyhedron](#polyhedron) consisting of a five-membered equatorial ring and two axial vertices, each joined to every ring vertex. Removing an equatorial vertex leaves the six-vertex pentagonal-pyramidal skeleton used for some [nido clusters](molecule.md#nido-cluster).

### Truncated octahedron

↑ **Parent:** [Polyhedron](#polyhedron)

The Archimedean solid obtained by truncating an [octahedron](#octahedron), with eight hexagonal faces and six square faces. In an fcc nanocrystal the analogous shape can expose both $\{111\}$ and $\{100\}$ [facets](convex-set.md#facet); the relative [facet](convex-set.md#facet) areas need not equal those of the regular Archimedean solid.

### Prism (geometry)

↑ **Parent:** [Polyhedron](#polyhedron)

A [polyhedron](#polyhedron) with two congruent parallel polygonal bases whose corresponding vertices are joined by parallel edges. A right prism has edges between the bases perpendicular to their planes. The optical use of a transparent prism is a separate application of this geometric shape.

#### Minimum deviation of a prism

↑ **Parent:** [Prism (geometry)](#prism-geometry)

For a homogeneous [optical prism](geometrical-optics.md#prism-optics) in the same medium on both sides, the minimum transmitted-ray deviation occurs for a symmetric path: the two internal refraction angles equal half its apex angle $A$. The expression requires $n\sin(A/2)\leq1$; equality is a grazing limiting path.

##### Prism sweep under different rotation conventions

↑ **Parent:** [Minimum deviation of a prism](#minimum-deviation-of-a-prism)

For a prism in air with fixed apex angle $A$, Snell's law gives $r_1=\arcsin(\sin i/n)$, $r_2=A-r_1$ and $e=\arcsin(n\sin r_2)$. The exit angle $e$ is relative to the moving exit-face normal; the deviation $D$ is relative to the incoming beam. Rotating the prism while keeping the incident beam fixed changes the laboratory outgoing direction by $\Delta D$. Steering the incoming beam while fixing the prism instead changes it by $\Delta e$. These are distinct experiments; emergence and total-internal-reflection conditions must also be checked.

#### Hexagonal prism

↑ **Parent:** [Prism (geometry)](#prism-geometry)

A prism with two hexagonal faces and six quadrilateral side faces. Its twelve vertices and eighteen edges provide an alternating [aluminium](chemical-substance.md#aluminium)–[oxygen](chemical-substance.md#oxygen) cage model when the graph is coloured bipartitely.

### Edge of a polyhedron

↑ **Parent:** [Polyhedron](#polyhedron)

A line segment along which two faces of a [polyhedron](#polyhedron) meet. A [rectangular parallelepiped](#rectangular-parallelepiped) has twelve edges, four parallel to each of its three side directions.

### Interior dihedral angle of a convex polyhedron

↑ **Parent:** [Polyhedron](#polyhedron)

At an edge of a convex [polyhedron](#polyhedron), its interior dihedral angle is the angle of the wedge inside the solid, measured in a [plane](geometry-and-topology.md#plane) perpendicular to the edge. If the two incident faces have outward [unit normal vectors](differential-geometry.md#unit-normal) $\hat{\mathbf n}_1,\hat{\mathbf n}_2$, then their normal angle is supplementary to the interior angle. Thus $\cos\theta=-\hat{\mathbf n}_1\cdot\hat{\mathbf n}_2$. Equivalently, subtract from each vector pointing into one face its [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the common edge; the angle between the resulting inward face directions is the interior angle. This distinguishes an interior angle from the acute angle convention for two unoriented [planes](geometry-and-topology.md#plane).

### Pyramid

↑ **Parent:** [Polyhedron](#polyhedron)

A pyramid is a [polyhedron](#polyhedron) with a [polygon](#polygon) as its base and triangular faces joining the base edges to one apex outside the base plane. If its base area is $A$ and perpendicular height is $h$, its [volume](geometry-and-topology.md#volume) is $Ah/3$. At height $z$ above the base, similarity gives cross-sectional area $A(1-z/h)^2$. Integrating this area from $0$ to $h$ proves the formula.

#### Square pyramid

↑ **Parent:** [Pyramid](#pyramid)

A square pyramid has a square base. If the base edge has length $a$ and all four lateral edges have length $\ell>a/\sqrt2$, the apex lies above the base center. The center-to-vertex distance is $a/\sqrt2$, so the [Pythagorean theorem](#pythagorean-theorem) gives $h=\sqrt{\ell^2-a^2/2}$. Its [volume](geometry-and-topology.md#volume) is $a^2h/3$. When all eight edges have the same length $a$, this reduces to $a^3/(3\sqrt2)$.

### Octahedron

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Octahedron)

An [octahedron](#octahedron) is a [polyhedron](#polyhedron) with eight faces. The regular [octahedron](#octahedron) has six vertices, twelve equal edges and eight equilateral triangular faces. One realization has vertices $\pm\mathbf e_1,\pm\mathbf e_2,\pm\mathbf e_3$; two vertices are adjacent exactly when they are not an opposite pair. Its edge graph is the [octahedral graph](graph-theory.md#octahedral-graph).

### Parallelepiped

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parallelepiped)

A [parallelepiped](#parallelepiped) is a [polyhedron](#polyhedron) with six [parallelogram](#parallelogram) faces in three opposite pairs. Three generating [vectors](vector-space.md#vector) determine its edges; the [absolute value](real-analysis.md#absolute-value) of their [determinant](multilinear-algebra.md#determinant) gives its volume in orthonormal Cartesian coordinates.

#### Rectangular parallelepiped

↑ **Parent:** [Parallelepiped](#parallelepiped)

A rectangular parallelepiped is a [parallelepiped](#parallelepiped) whose three edge directions at each vertex are mutually perpendicular. Its faces are [rectangles](#rectangle); if its edge lengths are $a,b,c$, its [volume](geometry-and-topology.md#volume) is $abc$. A [cube](#cube) is the special case $a=b=c$.

### Pentagonal prism

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pentagonal_prism)

A pentagonal prism has two pentagonal bases and five quadrilateral side faces, with three edges meeting at every vertex. Radial projection from an interior point gives a spherical polygon decomposition with five quadrilaterals and two pentagons.

### Tetrahedron

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tetrahedron)

A tetrahedron is the three-dimensional [simplex](algebraic-topology.md#simplex), with four vertices, six edges, and four triangular faces.

#### Tetrahedron membership via scalar triple products

↑ **Parent:** [Tetrahedron](#tetrahedron)

Let $D=\mathbf a\cdot(\mathbf b\times\mathbf c)>0$. The [reciprocal basis](multilinear-algebra.md#reciprocal-basis) gives the coordinates of any [position vector](classical-mechanics.md#position-vector) as

$$
\alpha=\frac{\mathbf r\cdot(\mathbf b\times\mathbf c)}D,\qquad
\beta=\frac{\mathbf r\cdot(\mathbf c\times\mathbf a)}D,\qquad
\gamma=\frac{\mathbf r\cdot(\mathbf a\times\mathbf b)}D.
$$

The point lies in the closed [tetrahedron](#tetrahedron) with vertices $0,\mathbf a,\mathbf b,\mathbf c$ exactly when $\alpha,\beta,\gamma\geq0$ and $\alpha+\beta+\gamma\leq1$. Indeed, these conditions express it as a [convex combination](convex-set.md#convex-combination) of the four vertices, with fourth weight $1-\alpha-\beta-\gamma$. They also describe the intersection of the four inward [half-spaces](geometry-and-topology.md#half-space) bounded by its faces. Strict inequalities characterize its interior.

#### Tetrahedron centroid-to-midpoint sum of squares

↑ **Parent:** [Tetrahedron](#tetrahedron)

Place the [centroid](#centroid) of a [tetrahedron](#tetrahedron) at the origin, so its four vertex vectors satisfy $r_1+r_2+r_3+r_4=0$. Midpoints of opposite edges have opposite vectors, hence equal distances from the centroid. For the three opposite-edge pairs, choose midpoint vectors $(r_1+r_j)/2$, $j=2,3,4$. Expanding their squared lengths and using $\sum_{j=2}^4r_j=-r_1$ gives

$$
\sum_{j=2}^4\left|\frac{r_1+r_j}{2}\right|^2=\frac14\sum_{i=1}^4|r_i|^2.
$$

The argument uses no regularity or equal-edge assumption on the tetrahedron.

#### Incenter of a tetrahedron

↑ **Parent:** [Tetrahedron](#tetrahedron)

The center of the sphere tangent to all four faces is the positive face-area-weighted combination of the opposite vertices. If $V$ is the [volume](geometry-and-topology.md#volume) and $S$ the total face area, its distance from each face is $3V/S$. Indeed its weight for vertex $A$ is $S_A/S$ and the corresponding altitude is $3V/S_A$, so their product is the common distance. Positive weights place it inside the [tetrahedron](#tetrahedron).

#### Circumcenter of a tetrahedron

↑ **Parent:** [Tetrahedron](#tetrahedron)

For independent edge vectors $u=B-A$, $v=C-A$, $w=D-A$, the displacement $x=O-A$ solves $x\cdot u=|u|^2/2$, $x\cdot v=|v|^2/2$, $x\cdot w=|w|^2/2$. The reciprocal cross-product basis gives the displayed formula. Its squared distances to all four vertices are equal. It need not lie inside the [tetrahedron](#tetrahedron).

#### Regular tetrahedron

↑ **Parent:** [Tetrahedron](#tetrahedron)

A [tetrahedron](#tetrahedron) whose six edges have equal length; its four faces are [equilateral triangles](#equilateral-triangle).

#### Sphere center from three tetrahedron face distances

↑ **Parent:** [Tetrahedron](#tetrahedron)

For a positively oriented [basis](vector-space.md#basis) $\mathbf a,\mathbf b,\mathbf c$, put $\tau=\mathbf a\cdot(\mathbf b\times\mathbf c)>0$. The center of an interior [sphere](#sphere) at distance $r$ from each of the three [tetrahedron](#tetrahedron) face planes through the origin has the displayed expression. The three inward [unit vectors](vector-space.md#unit-vector) are the normalized [cross products](vector-space.md#cross-product) $\mathbf b\times\mathbf c$, $\mathbf c\times\mathbf a$, $\mathbf a\times\mathbf b$. Taking [inner products](inner-product.md) with these vectors solves three independent signed-distance equations. Reversing some signs instead produces centers on exterior sides. Existence of a sphere contained in the full [tetrahedron](#tetrahedron) also requires clearance from the fourth face.

#### Opposite edges of a tetrahedron

↑ **Parent:** [Tetrahedron](#tetrahedron)

Two edges of a tetrahedron are opposite when they share no vertex. The six edges split into three opposite pairs.

##### Tetrahedron volume under sliding opposite edges

↑ **Parent:** [Opposite edges of a tetrahedron](#opposite-edges-of-a-tetrahedron)

Place one pair of opposite [tetrahedron](#tetrahedron) vertices on the line $b+\lambda a$ and the other pair on $d+\mu c$, with fixed nonzero direction [vectors](vector-space.md#vector) $a,c$. Let $\Delta=d-b$ and let $\delta\lambda,\delta\mu$ be the parameter differences within the two pairs. The [scalar triple product](multilinear-algebra.md#scalar-triple-product) of the three edge vectors from one vertex gives the displayed [volume](geometry-and-topology.md#volume). Terms parallel to $a$ or $c$ vanish in the triple product, leaving only $\Delta\cdot(a\times c)$. Sliding either pair along its own line while preserving its separation leaves this volume unchanged. When the two lines are [skew lines](#skew-lines), it can also be written $V=d_\perp\ell_1\ell_2|\sin\alpha|/6$, where $d_\perp$ is their shortest distance, $\ell_1,\ell_2$ the two edge lengths and $\alpha$ their direction angle. Intersecting or parallel lines give zero volume because all four vertices are coplanar.

##### Orthogonal opposite edges of a tetrahedron

↑ **Parent:** [Opposite edges of a tetrahedron](#opposite-edges-of-a-tetrahedron)

Place one vertex of a [tetrahedron](#tetrahedron) at the origin and denote the other vertex vectors by $a,b,c$. Orthogonality of two pairs of [opposite edges of a tetrahedron](#opposite-edges-of-a-tetrahedron) forces $a\cdot b=a\cdot c=b\cdot c$. It follows that the third pair is orthogonal too. The three sums of squared lengths of opposite edges all equal $|a|^2+|b|^2+|c|^2-2a\cdot b$. This gives a [dot product](inner-product.md#dot-product) test for the special geometry without solving for the face planes.

### Platonic solid

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Platonic_solid)

A Platonic solid is a convex polyhedron whose faces are congruent regular polygons and whose vertex figures are all alike.

#### Regular icosahedron

↑ **Parent:** [Platonic solid](#platonic-solid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_icosahedron)

A [regular icosahedron](#regular-icosahedron) is a [Platonic solid](#platonic-solid) with twenty equilateral triangular faces, twelve vertices and thirty edges. Five faces meet at each vertex. Its orientation-preserving [rotational symmetry](linear-algebra.md#rotational-symmetry) has order sixty: the [orbit-stabilizer theorem](group-action.md#orbit-stabilizer-theorem) gives twenty faces times the three [rotations](riemannian-geometry.md#rotation-mathematics) stabilizing a chosen face.

#### Cube

↑ **Parent:** [Platonic solid](#platonic-solid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cube)

A [Platonic solid](#platonic-solid) with six square faces, twelve edges and eight vertices. Its [rotational symmetry group of a cube](group-action.md#rotational-symmetry-group-of-a-cube) has order 24; including orientation-reversing isometries gives the order-48 [symmetry group of a cube](group-action.md#symmetry-group-of-a-cube).

#### Dodecahedron

↑ **Parent:** [Platonic solid](#platonic-solid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dodecahedron)

The regular dodecahedron is the [Platonic solid](#platonic-solid) with 12 regular pentagonal faces, 20 vertices, and 30 edges.

### Archimedean solid

↑ **Parent:** [Polyhedron](#polyhedron)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Archimedean_solid)

An Archimedean solid is a convex uniform polyhedron with regular polygonal faces and equivalent vertices, allowing more than one type of face.

#### Icosidodecahedron

↑ **Parent:** [Archimedean solid](#archimedean-solid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Icosidodecahedron)

The icosidodecahedron has 20 triangular and 12 pentagonal faces, with the faces alternating around each of its 30 vertices. It can be obtained by cutting a [dodecahedron](#dodecahedron) through the midpoints of its edges.

## Pythagorean theorem

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pythagorean_theorem)

For a [right triangle](#right-triangle) in [Euclidean geometry](euclidean-geometry.md) with perpendicular side [lengths](physics.md#length) $a,b>0$ and [hypotenuse](#hypotenuse) $c$, the [Pythagorean theorem](#pythagorean-theorem) states

$$
a^2+b^2=c^2.
$$

Geometrically, the [area](differential-geometry.md#surface-area) of the [square](#square) on the [hypotenuse](#hypotenuse) equals the sum of the [areas](differential-geometry.md#surface-area) of the [squares](#square) on the other two sides. Euclid's [Elements](#euclid-s-elements), Book I, Proposition 47 states this [area](differential-geometry.md#surface-area) equality; Proposition 48 states its converse: a [triangle](#triangle) satisfying the equality has a [right angle](#right-angle) opposite side $c$.[Euclid, Elements I.47](https://mathcs.clarku.edu/~djoyce/elements/bookI/propI47.html)[Euclid, Elements I.48](https://mathcs.clarku.edu/~djoyce/elements/bookI/propI48.html)

For $a=3$ and $b=4$, we compute $c=\sqrt{9+16}=5$. The [triangle](#triangle) has [area](differential-geometry.md#surface-area) $ab/2=6$, and its side [lengths](physics.md#length) form a [Pythagorean triple](#pythagorean-triple). Conversely, a [triangle](#triangle) measured to have sides $3,4,5$ must have a [right angle](#right-angle) between the sides $3$ and $4$. This makes the equality both a calculation tool and a test for perpendicularity.

The three [squares](#square) in the next figure have [areas](differential-geometry.md#surface-area) $3^2=9$, $4^2=16$ and $5^2=25$ in squared [length](physics.md#length) units. These are different from the central [right triangle](#right-triangle)'s [area](differential-geometry.md#surface-area) $3\cdot4/2=6$. The [Pythagorean theorem](#pythagorean-theorem) adds the [areas](differential-geometry.md#surface-area) of the attached [squares](#square), not their side [lengths](physics.md#length) and not the [area](differential-geometry.md#surface-area) of the [triangle](#triangle). The [square](#square) on the [hypotenuse](#hypotenuse) is tilted, but a [rotation](riemannian-geometry.md#rotation-mathematics) preserves its [area](differential-geometry.md#surface-area). This makes the formula visible without suggesting that the [hypotenuse](#hypotenuse) has to align with an axis.

<a id="image-squares-on-a-3-4-5-right-triangle-have-areas-9-plus-16-25-the-triangle-itself-has-area-6"></a>
![](pythagorean-square-areas.png)

**[Figure 1](#image-squares-on-a-3-4-5-right-triangle-have-areas-9-plus-16-25-the-triangle-itself-has-area-6). Squares on a 3-4-5 right triangle have areas $9+16=25$; the triangle itself has area $6$**.

Historically, [Euclid's Elements](#euclid-s-elements) records an organized proof of the [Pythagorean theorem](#pythagorean-theorem) as an equality of [areas](differential-geometry.md#surface-area), rather than the modern equation between numbers representing [lengths](physics.md#length). Its placement in Book I makes it available before the treatment of [similar triangles](#similar-triangle) in Book VI. This is evidence of how the result was established within that text; the name [Pythagorean theorem](#pythagorean-theorem) alone does not establish who first discovered or proved it. The precise historical anchor here is the surviving proposition, rather than an unsupported story of a single inventor.[Euclid, Elements I.47, statement and proof](https://mathcs.clarku.edu/~djoyce/elements/bookI/propI47.html)

The dissection below makes the general identity tangible. Both outer [squares](#square) have side $a+b$ and contain the same four [congruent](#congruence-geometry) [right triangles](#right-triangle). In the first arrangement, their [hypotenuses](#hypotenuse) bound a [square](#square) of side $c$: adjacent acute [angles](geometry-and-topology.md#angle) together make a [right angle](#right-angle). In the second, the uncovered regions are [squares](#square) of sides $a$ and $b$. Subtracting the same total [triangle](#triangle) [area](differential-geometry.md#surface-area) from equal outer [areas](differential-geometry.md#surface-area) gives

$$
c^2=(a+b)^2-4\frac{ab}{2}=a^2+b^2.
$$

For the pictured dimensions, the shared uncovered [area](differential-geometry.md#surface-area) is $49-24=25=9+16$.

<a id="image-rearranging-four-congruent-3-4-5-right-triangles-proves-that-the-uncovered-square-areas-satisfy-25-9-plus-16"></a>
![](pythagorean-area-dissection.png)

**[Figure 2](#image-rearranging-four-congruent-3-4-5-right-triangles-proves-that-the-uncovered-square-areas-satisfy-25-9-plus-16). Rearranging four congruent 3-4-5 right triangles proves that the uncovered square areas satisfy $25=9+16$**.

The same mechanism survives in [inner product spaces](inner-product.md#inner-product-space): for [orthogonal](inner-product.md#orthogonal-vectors) [vectors](vector-space.md#vector) $u,v$, expanding the [inner product](inner-product.md) gives $\|u+v\|^2=\|u\|^2+\|v\|^2$. This is why [orthogonal projection](hilbert-space.md#orthogonal-projection) separates a squared distance into independent contributions. The familiar [right triangle](#right-triangle) is the simplest picture of a much more reusable principle.

### Pythagorean equation

↑ **Parent:** [Pythagorean theorem](#pythagorean-theorem)

The equation $a^2+b^2=c^2$. Its [positive integer](integer.md#positive-integer) solutions are [Pythagorean triples](#pythagorean-triple); [primitive Pythagorean triples](#primitive-pythagorean-triple) are those with no common factor greater than 1.

### Pythagorean triple

↑ **Parent:** [Pythagorean theorem](#pythagorean-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pythagorean_triple)

A Pythagorean triple consists of three positive [integers](integer.md) satisfying $x^2+y^2=z^2$. It is primitive when their [greatest common divisor](divisibility.md#greatest-common-divisor) is one. Reducing their [square numbers](integer.md#square-number) modulo $3$ shows that at least one leg is divisible by $3$; reducing modulo $4$ shows that both legs cannot be odd.

#### Berggren tree

↑ **Parent:** [Pythagorean triple](#pythagorean-triple)

A rooted ternary tree that generates every primitive [Pythagorean triple](#pythagorean-triple) from $(3,4,5)$ by three fixed linear transformations. Keeping a consistent leg convention gives each primitive triple once; multiplying its sides then supplies all nonprimitive triples.

#### Primitive Pythagorean triple

↑ **Parent:** [Pythagorean triple](#pythagorean-triple)

A [Pythagorean triple](#pythagorean-triple) $(a,b,c)$ whose coordinates have [greatest common divisor](divisibility.md#greatest-common-divisor) 1. Its two legs have opposite [integer parity](integer.md#parity-mathematics), and every [Pythagorean triple](#pythagorean-triple) is a unique [positive integer](integer.md#positive-integer) multiple of a [primitive Pythagorean triple](#primitive-pythagorean-triple) up to the ordering of its legs.

<h4 id="euclid-s-formula-for-pythagorean-triples">Euclid's formula for Pythagorean triples</h4>

↑ **Parent:** [Pythagorean triple](#pythagorean-triple)

The formulas $a=m^2-n^2$, $b=2mn$, $c=m^2+n^2$ give a [Pythagorean triple](#pythagorean-triple) for [integers](integer.md) $m>n>0$, because $(m^2-n^2)^2+(2mn)^2=(m^2+n^2)^2$. They give a [primitive Pythagorean triple](#primitive-pythagorean-triple) exactly when $m,n$ are [coprime](divisibility.md#coprime-integers) and have opposite [integer parity](integer.md#parity-mathematics). Every [primitive Pythagorean triple](#primitive-pythagorean-triple) arises this way after possibly exchanging the legs; scaling gives the nonprimitive triples.

#### Primitive Pythagorean parametrization

↑ **Parent:** [Pythagorean triple](#pythagorean-triple)

Every primitive [Pythagorean triple](#pythagorean-triple), after exchanging its legs, has this form with $m>n>0$, $\gcd(m,n)=1$ and opposite parity. Its area is $mn(m-n)(m+n)$. The factors $m,n,m-n,m+n$ are pairwise coprime, because $m\pm n$ are odd. Conversely these conditions give a primitive triple. The parametrization follows by factoring the relatively prime integers $(c+b)/2$ and $(c-b)/2$ when $a$ is the even leg.

## Voronoi diagram

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Voronoi_diagram)

Given sites in a [Euclidean space](normed-vector-space.md#euclidean-norm), the Voronoi cell of a site is the set of points at least as close to it as to every other site. The Voronoi diagram is the subdivision formed by all of these cells.

## Sphere

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sphere)

A sphere is the set of points at one fixed positive [Euclidean distance](topological-analysis.md#euclidean-distance) from a center.

### Tangent spheres

↑ **Parent:** [Sphere](#sphere)

Two distinct [spheres](#sphere) are externally tangent when their center distance equals the sum of their [radii](topology.md#radius). They are internally tangent when it equals the absolute difference of their [radii](topology.md#radius). At the point of contact they have the same tangent plane.

### Equator

↑ **Parent:** [Sphere](#sphere)

For a [sphere](#sphere) with a chosen polar axis, its equator is the [great circle](#great-circle) in the plane through its center perpendicular to that axis. On the unit [sphere](#sphere) in [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) it is $\theta=\pi/2$. Like every [great circle](#great-circle), it is a [geodesic](riemannian-geometry.md#geodesic).

### Meridian of a sphere

↑ **Parent:** [Sphere](#sphere)

A [great circle](#great-circle) passing through a chosen pair of antipodal poles, or the pole-to-pole half of that circle at fixed longitude. In [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system), a fixed azimuth selects such a half-circle. Meridians are special cases of a [meridian of a surface of revolution](differential-geometry.md#meridian-of-a-surface-of-revolution) and are [geodesics](riemannian-geometry.md#geodesic) of the [sphere](#sphere).

### Volume enclosed by a sphere

↑ **Parent:** [Sphere](#sphere)

The solid ball inside a radius-$a$ [sphere](#sphere) has [volume](geometry-and-topology.md#volume) $4\pi a^3/3$. One derivation integrates concentric shell area: $V=\int_0^a4\pi r^2dr$. The sphere itself is the boundary surface; its area is $4\pi a^2$, a different dimensional quantity.

### Spherical wedge

↑ **Parent:** [Sphere](#sphere)

A [spherical wedge](#spherical-wedge) is the portion of a solid [sphere](#sphere) between two meridional half-planes meeting at a dihedral angle $\beta$, with $0<\beta<2\pi$. Put the common axis along $z$ and its azimuthal bisector along $x$. For radius $a$, use [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) $0\leq r\leq a$, $0\leq\theta\leq\pi$, $-\beta/2\leq\varphi\leq\beta/2$. Its [volume](geometry-and-topology.md#volume) is $2\beta a^3/3$.

For constant [mass density](fluid-mechanics.md#density), reflection symmetries put the [centre of mass](classical-mechanics.md#center-of-mass) on the bisector. The first moment is

$$
\int_Vx\,dV=\left(\int_0^a r^3\,dr\right)
\left(\int_0^\pi\sin^2\theta\,d\theta\right)
\left(\int_{-\beta/2}^{\beta/2}\cos\varphi\,d\varphi\right)
=\frac{\pi a^4}{4}\sin\frac\beta2.
$$

Dividing by [volume](geometry-and-topology.md#volume) gives $\bar x=3\pi a\sin(\beta/2)/(8\beta)$. It decreases from the limiting value $3\pi a/16$ for an infinitesimal wedge to zero for a full sphere.

The curved boundary is a [spherical lune](geometry-and-topology.md#spherical-lune). Its outward [vector area](differential-geometry.md#vector-area) is $\pi a^2\sin(\beta/2)\mathbf e_x$. Indeed, its $x$ component has the same angular integrals as the first moment, multiplied by $a^2$; the other components cancel by symmetry. Its scalar [surface area](differential-geometry.md#surface-area) is $2\beta a^2$, which is generally different from the magnitude of its [vector area](differential-geometry.md#vector-area).

### Circle of intersection of two spheres

↑ **Parent:** [Sphere](#sphere)

Two [spheres](#sphere) with centres $a,b$ and positive radii $p,q$ intersect in a nondegenerate [circle](topology.md#circle) exactly under the displayed strict triangle inequalities. Put $d=|b-a|$. Subtracting $|r-a|^2=p^2$ and $|r-b|^2=q^2$ gives its plane,

$$
2(b-a)\cdot r=p^2-q^2+|b|^2-|a|^2.
$$

The circle centre is $a+\ell(b-a)/d$, where $\ell=(p^2-q^2+d^2)/(2d)$, and its squared radius is $p^2-\ell^2$. This is positive exactly under the strict inequalities. Equality gives internal or external tangency; coincident equal [spheres](#sphere) have an entire sphere in common rather than a unique intersection circle.

### Spherical shell

↑ **Parent:** [Sphere](#sphere)

A spherical shell is the region between two concentric [spheres](#sphere). A thin mass shell at radius $r$, thickness $dr$ and [mass density](fluid-mechanics.md#density) $\rho(r)$ has mass $4\pi r^2\rho(r)\,dr$ to first order. Decomposing a spherical body into such shells makes the [spherical shell theorem](mathematical-physics.md#spherical-shell-theorem) applicable to its [gravitational potential energy](energy.md#gravitational-energy).

### Product of two spheres

↑ **Parent:** [Sphere](#sphere)

The [Cartesian product](set-theory.md#cartesian-product) $S^p\times S^q$ has one cell in each of dimensions $0,p,q,p+q$, counting the two middle cells separately when $p=q$. For positive $p,q$, its integral [cohomology ring](cohomology.md#cohomology-ring) has generators $a,b$ of degrees $p,q$, with $a^2=b^2=0$ and $ba=(-1)^{pq}ab$. The class $ab$ is a product orientation class. This follows from the [Künneth theorem](cohomology.md#kunneth-theorem).

#### Simultaneous antipodal quotient of two spheres

↑ **Parent:** [Product of two spheres](#product-of-two-spheres)

For positive $p,q$, quotient $S^p\times S^q$ by $(x,y)\mapsto(-x,-y)$. This is a free double [covering space](algebraic-topology.md#covering-space) action. Its [closed manifold](smooth-manifold.md#closed-manifold) quotient is orientable exactly when $p+q$ is even, because the product [mapping degree](homology.md#degree-of-a-continuous-mapping) is $(-1)^{p+q+2}$. If $p,q\ge2$, the product is [simply connected](algebraic-topology.md#simply-connected-space) and the quotient has [fundamental group](algebraic-topology.md#fundamental-group) $\mathbb Z/2$. For $p=q=2$, the quotient has integral [cohomology groups](cohomology.md#cohomology-group) $\mathbb Z$ in degrees $0,4$, $\mathbb Z/2$ in degrees $2,3$, and zero elsewhere. Every positive-degree [cup product](cohomology.md#cup-product) is zero. These conclusions follow from [Poincare duality](cohomology.md#poincare-duality), the [Euler characteristic under a finite covering](homology.md#euler-characteristic-under-a-finite-covering), and the [universal coefficient theorem for cohomology](cohomology.md#universal-coefficient-theorem-for-cohomology).

### Surface measure on a sphere

↑ **Parent:** [Sphere](#sphere)

Surface area is the two-dimensional measure induced on the unit [sphere](#sphere) in three dimensions. It is invariant under orthogonal rotations. It is not the restriction of ambient three-dimensional [Lebesgue measure](measure-theory.md#lebesgue-measure), under which the [sphere](#sphere) has measure zero. Normalizing by the [sphere](#sphere) area gives a [probability measure](probability-space.md#probability-measure).

### Antipodal pair

↑ **Parent:** [Sphere](#sphere)

On a [sphere](#sphere) centred at the origin, an antipodal pair is the unordered pair $\{x,-x\}$. The [antipodal map](homology.md#antipodal-map) exchanges its two points.

### Apollonius sphere

↑ **Parent:** [Sphere](#sphere)

For distinct points and $0<\lambda<1$, the distance-ratio locus is a sphere with center $(\mathbf a-\lambda^2\mathbf b)/(1-\lambda^2)$ and radius $\lambda|\mathbf a-\mathbf b|/(1-\lambda^2)$. Completing the square proves this formula. It encloses $\mathbf a$ but excludes $\mathbf b$, because their distances to the center are $\lambda R$ and $R/\lambda$. It is the zero-potential locus of two opposite-sign point charges with magnitude ratio $\lambda$. Equal magnitudes instead give a plane.

### Hemisphere

↑ **Parent:** [Sphere](#sphere)

A hemisphere is either half of a sphere cut by a plane through its center. Its curved surface has area $2\pi r^2$. Closing that surface with its equatorial disk encloses a half-ball of volume $2\pi r^3/3$. The curved surface and enclosed solid have distinct roles in surface-cost and volume calculations.

#### Maximum-volume cuboid in a hemisphere

↑ **Parent:** [Hemisphere](#hemisphere)

For a closed [hemisphere](#hemisphere) of [radius](topology.md#radius) $a>0$, take a [rectangular parallelepiped](#rectangular-parallelepiped) with a face on the flat base, base half-widths $x,y>0$ and height $z>0$. Its curved-boundary constraint is $x^2+y^2+z^2=a^2$ and its [volume](geometry-and-topology.md#volume) is $4xyz$. A [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) gives $x=y=z=a/\sqrt3$, yielding the displayed maximum. The full edge lengths are $2a/\sqrt3,2a/\sqrt3,a/\sqrt3$.

This bound remains valid when arbitrary orientations are allowed. Write a cuboid's half-edge lengths as $u_1,u_2,u_3$, its center components in its orthonormal edge basis as $v_i$, and the vertical unit-vector components as $n_i$. Containment above the base plane requires $\sum n_iv_i\geq\sum|n_i|u_i$. Hence $|v_j|\geq u_j$ for at least one $j$: otherwise every contributing term would be strictly smaller than its required bound. Its farthest vertex has squared distance

$$
\sum_i u_i^2+\sum_i v_i^2+2\sum_i u_i|v_i|
\geq\sum_{i\ne j}u_i^2+4u_j^2.
$$

Containment in the sphere bounds the right side by $a^2$. The [arithmetic-geometric mean inequality](mathematical-optimization.md#arithmetic-geometric-mean-inequality) then gives $2u_1u_2u_3\leq a^3/(3\sqrt3)$, so the full [volume](geometry-and-topology.md#volume) $8u_1u_2u_3$ cannot exceed the displayed value. The constructed cuboid attains it. With strict containment and no boundary contact, the same value is a supremum.

#### Open hemisphere

↑ **Parent:** [Hemisphere](#hemisphere)

For a nonzero vector $u$, the open hemisphere of $S^d$ with direction $u$ is $\{x\in S^d:u\cdot x>0\}$. Its boundary is excluded, so opposite [open hemispheres](#open-hemisphere) are disjoint.

##### General-position hemisphere count

↑ **Parent:** [Open hemisphere](#open-hemisphere)

Choose $N$ points of $S^d$ such that every $d+1$ of their position vectors are [linearly independent](vector-space.md#linear-independence). Any equatorial hyperplane then contains at most $d$ points. If $N-d\geq2r-1$, at least one of each opposite pair of [open hemispheres](#open-hemisphere) contains $r$ points. Such configurations exist: take distinct real parameters $t_i$ and normalize $(1,t_i,\ldots,t_i^d)$; the [Vandermonde determinant](galois-theory.md#vandermonde-determinant) proves the required independence. This weaker one-of-two guarantee already suffices for the topological lower bound in [Lovász theorem on Kneser graphs](graph-theory.md#lovasz-theorem-on-kneser-graphs).

##### Gale hemisphere lemma

↑ **Parent:** [Open hemisphere](#open-hemisphere)

For integers $n=2k+d$ with $k\geq1$ and $d\geq0$, there are $n$ labelled points of $S^d$ such that every [open hemisphere](#open-hemisphere) contains at least $k$ of them. The normalized vectors $(-1)^i(1,t_i,\ldots,t_i^d)$ for increasing $t_i$ give a signed [moment curve](fourier-analysis.md#moment-curve) construction. A nonzero [polynomial](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $d$ cannot have enough sign changes for fewer than $k$ positive alternating sample values. Zero sample values can be perturbed negatively by a [Lagrange interpolation polynomial](interpolation.md#lagrange-polynomial). Labels allow repeated positions when $d=0$.

### Great circle

↑ **Parent:** [Sphere](#sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Great_circle)

A great circle is the intersection of a [sphere](#sphere) with a plane through its centre. Its shorter arcs are [geodesics](riemannian-geometry.md#geodesic) of the round [sphere](#sphere); celestial meridians and the equator are examples.

#### Regions of a general-position great-circle arrangement

↑ **Parent:** [Great circle](#great-circle)

For $N\geq1$ [great circles](#great-circle) on a [sphere](#sphere), with no coincident circles or triple intersection, the number of open regions is $R_N=N(N-1)+2$. The first circle gives two regions. Each subsequent circle meets the previous $n-1$ circles at $2(n-1)$ distinct points and is divided into that many arcs, each splitting a previous region. Summing the increments proves the formula. If the circles are $a_i\cdot x=0$, each region has one fixed sign vector $(\operatorname{sgn}(a_i\cdot x))_i$. Conversely a realized strict sign vector has a connected region: its cone is an intersection of open [half-spaces](geometry-and-topology.md#half-space), and radial projection of line segments connects any two points.

### Gnomonic projection

↑ **Parent:** [Sphere](#sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gnomonic_projection)

The gnomonic projection intersects rays from a [sphere](#sphere)’s centre with a tangent plane. If $\mathbf b$ is its unit normal and $\mathbf e,\mathbf n$ are tangent basis vectors, a direction $\mathbf s$ maps to $f(\mathbf s\cdot\mathbf e,\mathbf s\cdot\mathbf n)/(\mathbf s\cdot\mathbf b)$. It maps [great circle](#great-circle) arcs to straight lines and is singular at the tangent-plane horizon.

### Unit sphere as a regular level set

↑ **Parent:** [Sphere](#sphere)

The unit sphere $S^n\subseteq\mathbb R^{n+1}$ is the regular level set $\lVert x\rVert^2=1$. Its tangent space is

$$
T_xS^n=x^\perp=\{v\in\mathbb R^{n+1}:x\mathbin\cdot v=0\}.
$$

### Two-sphere

↑ **Parent:** [Sphere](#sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Two-sphere)

The two-sphere is the two-dimensional [sphere](#sphere) embedded in three-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm).

### Three-sphere

↑ **Parent:** [Sphere](#sphere)

The three-sphere is the unit sphere in four-dimensional [Euclidean space](normed-vector-space.md#euclidean-norm):

$$
S^3=\{x\in\mathbb R^4:\lVert x\rVert=1\}.
$$

Identifying $\mathbb R^4$ with $\mathbb C^2$ realizes it as $\{(z_1,z_2):|z_1|^2+|z_2|^2=1\}$.

### Solid angle

↑ **Parent:** [Sphere](#sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solid_angle)

A [solid angle](#solid-angle) measures how much of the surrounding directions a region occupies, as seen from a specified point $O$. Draw a [sphere](#sphere) of [radius](topology.md#radius) $R$ centered at $O$ and mark where those directions meet its surface. If the marked patch has [surface area](differential-geometry.md#surface-area) $A_R$, then

$$
\boxed{\Omega=\frac{A_R}{R^2}.}
$$

A [Euclidean similarity](geometry-and-topology.md#euclidean-similarity) scales both $A_R$ and $R^2$ by the same factor, so the chosen [radius](topology.md#radius) does not affect the answer. On the unit [two-sphere](#two-sphere), the numerical value is simply the patch's [surface area](differential-geometry.md#surface-area). Unlike an [angle](geometry-and-topology.md#angle) drawn in one plane, a [solid angle](#solid-angle) measures coverage in two angular directions.

For example, the full [sphere](#sphere) has [surface area](differential-geometry.md#surface-area) $4\pi R^2$ and hence [solid angle](#solid-angle) $4\pi$ [steradians](#steradian). A [hemisphere](#hemisphere) occupies $2\pi$ [steradians](#steradian). Three mutually perpendicular coordinate planes divide the directions into eight congruent pieces, so each octant occupies $4\pi/8=\pi/2$ [steradians](#steradian). A [solid angle](#solid-angle) of one [steradian](#steradian) therefore covers $1/(4\pi)\approx7.96\%$ of all directions, rather than one full turn.

This makes a geometric question answer a collection question. For an ideal [point emitter](radiometry.md#point-emitter) with [isotropy](continuum-mechanics.md#isotropy), equal [solid angles](#solid-angle) carry equal [radiant flux](radiometry.md#radiant-flux). A detector accepting directions of total [solid angle](#solid-angle) $\Omega$ intercepts the fraction $\Omega/(4\pi)$ of that emitted [radiant flux](radiometry.md#radiant-flux), before losses. With direction-dependent [radiant intensity](radiometry.md#radiant-intensity) $I$, the accepted [radiant flux](radiometry.md#radiant-flux) is instead $\int I\,d\Omega$. The [solid angle of a disk](#solid-angle-of-a-disk) below gives an exact example where the familiar [inverse-square law](physics.md#inverse-square-law) is only a distant-source approximation.

#### Steradian

↑ **Parent:** [Solid angle](#solid-angle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steradian)

A [steradian](#steradian) is the [solid angle](#solid-angle) subtended at a [sphere](#sphere)'s center by a patch of [surface area](differential-geometry.md#surface-area) $R^2$. The whole [sphere](#sphere) subtends $4\pi\,\mathrm{sr}$. In the [SI](physics.md#international-system-of-units), the [steradian](#steradian) has unit one; retaining its symbol identifies a [solid angle](#solid-angle), just as [radians](geometry-and-topology.md#radian) identify an [angle](geometry-and-topology.md#angle). A [dimensionless quantity](physics.md#dimensionless-quantity) still needs its physical meaning specified.[Version 4.01, June 2026; English §2.3.3, printed pp. 132–133, and §2.3.4, Table 4, printed pp. 133–134, notes (b)–(c): radian and steradian definitions and unit-one convention](physics-bibliography.md#the-international-system-of-units-si-ninth-edition-si-brochure)

#### Solid angle of a circular cone

↑ **Parent:** [Solid angle](#solid-angle)

A [right circular cone](#right-circular-cone) with vertex $O$ selects all directions within a half-opening [angle](geometry-and-topology.md#angle) $\theta$ of its axis. Here $\theta$ is measured from the axis to a boundary direction, so the full opening in a meridian plane is $2\theta$. For $0\leq\theta\leq\pi$, interpret the selected directions as a [spherical cap](#spherical-cap); for $\theta>\pi/2$, this is a region larger than a [hemisphere](#hemisphere).

The [spherical coordinate system](multivariable-calculus.md#spherical-coordinate-system) gives the [area element](differential-geometry.md#area-element-of-a-surface) $dA=R^2\sin\alpha\,d\alpha\,d\phi$ on the [sphere](#sphere). Dividing by $R^2$ and integrating over the cap yields

$$
d\Omega=\sin\alpha\,d\alpha\,d\phi,\qquad
\Omega=\int_0^{2\pi}\int_0^\theta\sin\alpha\,d\alpha\,d\phi
=2\pi(1-\cos\theta).
$$

The factor $\sin\alpha$ matters: a thin angular strip near a pole contains fewer directions than an equally wide strip near the equator. Treating equal intervals of both [spherical coordinates](multivariable-calculus.md#spherical-coordinate-system) as equal [solid angles](#solid-angle) would overcount the polar directions.

<a id="image-one-set-of-directions-cuts-similar-spherical-caps-from-spheres-of-different-radii"></a>
![](solid-angle-cone-and-spherical-cap.png)

**[Figure 3](#image-one-set-of-directions-cuts-similar-spherical-caps-from-spheres-of-different-radii). One set of directions cuts similar spherical caps from spheres of different radii**. Original geometric construction with half-opening [angle](geometry-and-topology.md#angle) $45^\circ$. Left: a meridian section of two concentric [spheres](#sphere); rotating each blue arc about the dotted axis gives its cap. Right: the corresponding patch on the unit [sphere](#sphere). The patch is curved, and its [surface area](differential-geometry.md#surface-area), rather than the volume inside the cone, determines the [solid angle](#solid-angle).

At $\theta=45^\circ$, the [solid angle](#solid-angle) is $\pi(2-\sqrt2)\approx1.8403$ [steradians](#steradian), or about $14.64\%$ of all directions. At $\theta=90^\circ$ it is $2\pi$ [steradians](#steradian), and at $180^\circ$ it is $4\pi$ [steradians](#steradian). For a small $\theta$ measured in [radians](geometry-and-topology.md#radian), the [Taylor series](calculus.md#taylor-series) $\cos\theta=1-\theta^2/2+O(\theta^4)$ gives the [small-angle approximation](geometry-and-topology.md#small-angle-approximation) $\Omega\approx\pi\theta^2$. Doubling a narrow half-opening [angle](geometry-and-topology.md#angle) therefore approximately quadruples its coverage.

#### Solid angle of a disk

↑ **Parent:** [Solid angle](#solid-angle)

Consider a flat circular [disk](topology.md#disk-mathematics) of [radius](topology.md#radius) $a>0$, with its center a perpendicular distance $d>0$ from the viewpoint $O$. The line from $O$ to its center is normal to the [disk](topology.md#disk-mathematics). Its rim defines a [right circular cone](#right-circular-cone) with $\tan\theta=a/d$ and $\cos\theta=d/\sqrt{d^2+a^2}$. The [solid angle of a circular cone](#solid-angle-of-a-circular-cone) immediately gives

$$
\boxed{\Omega=2\pi\left(1-\frac{d}{\sqrt{d^2+a^2}}\right).}
$$

For $a=d$, this is the same $45^\circ$ half-opening example: about $1.8403$ [steradians](#steradian). Both the [radius](topology.md#radius) and distance enter; doubling both leaves the [solid angle](#solid-angle) unchanged.

A useful local version applies to a small surface patch of [area](differential-geometry.md#surface-area) $dA$, at distance $r$ from $O$. If $\psi$ is the [angle](geometry-and-topology.md#angle) between its [unit normal](differential-geometry.md#unit-normal) and the line to $O$, its unsigned geometric contribution is

$$
d\Omega=\frac{|\cos\psi|\,dA}{r^2}.
$$

The numerator is the [projected area](radiometry.md#projected-area). For a visible patch, perpendicular projection followed by radial projection onto a small piece of a [sphere](#sphere) gives this formula. Integrating counts the directions once provided no direction encounters multiple counted patches. For an opaque detector, use its unoccluded face. At grazing view, the [projected area](radiometry.md#projected-area) tends to zero.

For this on-axis [disk](topology.md#disk-mathematics), a ring of [radius](topology.md#radius) $\rho$ has $r=\sqrt{d^2+\rho^2}$ and $|\cos\psi|=d/r$. Its [polar coordinates](multivariable-calculus.md#polar-coordinates) gives $dA=\rho\,d\rho\,d\phi$, so the same answer follows directly from the [surface integral](multivariable-calculus.md#surface-integral):

$$
\Omega=2\pi\int_0^a\frac{d\,\rho}{(d^2+\rho^2)^{3/2}}\,d\rho
=2\pi\left(1-\frac{d}{\sqrt{d^2+a^2}}\right).
$$

The changing distance and obliquity are both already accounted for; an extra detector-wide cosine factor would count the projection twice.

<a id="image-the-exact-solid-angle-of-an-on-axis-circular-detector-approaches-a-hemisphere-at-close-range"></a>
![](solid-angle-disk-detector-and-distance.png)

**[Figure 4](#image-the-exact-solid-angle-of-an-on-axis-circular-detector-approaches-a-hemisphere-at-close-range). The exact solid angle of an on-axis circular detector approaches a hemisphere at close range**. Left: a meridian section, drawn with $a=d$. Right: the geometric acceptance fraction $\Omega/(4\pi)$ for a [point emitter](radiometry.md#point-emitter) with [isotropy](continuum-mechanics.md#isotropy), compared with the distant-source approximation $a^2/(4d^2)$. These are calculated geometric curves, not measured detector efficiencies. The dashed approximation is displayed outside its accurate range to show how it overestimates acceptance.

For $d\gg a$, the [Taylor series](calculus.md#taylor-series) of $(1+a^2/d^2)^{-1/2}$ gives

$$
\Omega=\frac{\pi a^2}{d^2}+O\!\left(\frac{a^4}{d^4}\right).
$$

Thus the accepted fraction of an ideal [point emitter](radiometry.md#point-emitter)'s isotropic output is approximately $A/(4\pi d^2)$, where $A=\pi a^2$. This is the geometry behind the [inverse-square law](physics.md#inverse-square-law) for a small detector. At fixed $a$, however, taking $d\to0^+$ gives $\Omega\to2\pi$, so the accepted fraction approaches $1/2$ rather than diverging.

For a chosen numerical example, let $a=1\,\mathrm{cm}$ and $d=5\,\mathrm{cm}$. The exact [solid angle](#solid-angle) is approximately $0.122015$ [steradians](#steradian), giving an acceptance fraction $0.00970966$. An ideal [point emitter](radiometry.md#point-emitter) with [isotropy](continuum-mechanics.md#isotropy) and total [radiant flux](radiometry.md#radiant-flux) $1\,\mathrm{mW}$ would therefore send **about $9.71\,\mathrm{\mu W}$ onto the disk**. The distant-source approximation gives $10.0\,\mathrm{\mu W}$, about $3.0\%$ high. This calculation assumes unobstructed propagation and counts incident [radiant flux](radiometry.md#radiant-flux); [photon absorption](quantum-mechanics.md#photon-absorption), detector response, and any [optical attenuator](optical-instrument.md#optical-attenuator) require separate factors.

#### Angular average

↑ **Parent:** [Solid angle](#solid-angle)

The normalized [angular average](#angular-average) is over the unit [sphere](#sphere), with [solid angle](#solid-angle) measure $d\Omega$. Rotational symmetry gives $\langle e^i\rangle_\Omega=0$, $\langle e^ie^j\rangle_\Omega=\delta^{ij}/3$, and $\langle e^ie^je^ke^\ell\rangle_\Omega=(\delta^{ij}\delta^{k\ell}+\delta^{ik}\delta^{j\ell}+\delta^{i\ell}\delta^{jk})/15$. The constants follow by contracting indices and using $e^ie_i=1$. These identities extract [photon angular temperature moments](cosmic-microwave-background-anisotropy.md#photon-angular-temperature-moments). For normalized [spherical harmonics](analysis.md#spherical-harmonic), $\int Y_{\ell m}^*Y_{\ell' m'}\,d\Omega=\delta_{\ell\ell'}\delta_{mm'}$; their [angular average](#angular-average) instead has an extra factor $1/(4\pi)$.

## Triangle

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangle)

A [triangle](#triangle) is the [convex hull](convex-set.md#convex-hull) of three noncollinear [points](geometry-and-topology.md#point-geometry): the three vertices must not lie on one [line](#straight-line). Its boundary consists of the three joining [line segments](convex-set.md#line-segment); depending on context, "[triangle](#triangle)" can mean this boundary or the filled region it encloses. Here a [triangle](#triangle)'s [area](differential-geometry.md#surface-area) refers to the filled region. The noncollinearity assumption excludes a collapsed shape with zero [area](differential-geometry.md#surface-area), for which ordinary interior [angles](geometry-and-topology.md#angle) are not defined.

For example, the positions $(0,0)$, $(4,0)$ and $(0,3)$ form a [right triangle](#right-triangle) with a [right angle](#right-angle) at the origin. Taking the side of [length](physics.md#length) $4$ as its base gives perpendicular height $3$, so its [area](differential-geometry.md#surface-area) is $4\cdot3/2=6$. The height is measured at a [right angle](#right-angle) to the chosen base; it is not generally the [length](physics.md#length) of another side. In this example it happens to be a side because the [triangle](#triangle) is a [right triangle](#right-triangle).

By contrast, side [lengths](physics.md#length) $3,4,6$ define a valid [triangle](#triangle): each side is shorter than the sum of the other two, as required by the strict [triangle inequality](topological-analysis.md#triangle-inequality). But $3^2+4^2=25\ne36=6^2$, so this is not a [right triangle](#right-triangle) and the [Pythagorean theorem](#pythagorean-theorem) cannot calculate its longest side from the other two. The [law of cosines](#law-of-cosines) instead gives the opposite interior [angle](geometry-and-topology.md#angle) $C$ through

$$
\cos C=\frac{3^2+4^2-6^2}{2\cdot3\cdot4}=-\frac{11}{24},\qquad C\approx117.28^\circ.
$$

This example separates the definition of a [triangle](#triangle) from the additional assumption of a [right angle](#right-angle).

Every [triangle](#triangle) in the [Euclidean plane](geometry-and-topology.md#euclidean-plane) has interior [angles](geometry-and-topology.md#angle) summing to $\pi$ [radians](geometry-and-topology.md#radian), a result proved in [Euclid's Elements](#euclid-s-elements) I.32.[Euclid, Elements I.32](https://mathcs.clarku.edu/~djoyce/elements/bookI/propI32.html) It lets two measured [angles](geometry-and-topology.md#angle) determine the third, and underlies the angle-angle criterion for [similar triangles](#similar-triangle). The qualification "[Euclidean plane](geometry-and-topology.md#euclidean-plane)" matters: the earlier [spherical triangle](geometry-and-topology.md#spherical-triangle) demonstrates a different sum.

<h3 id="apollonius-s-theorem">Apollonius's theorem</h3>

↑ **Parent:** [Triangle](#triangle)

### Median of a triangle

↑ **Parent:** [Triangle](#triangle)

A median joins a [vertex of a polygon](#vertex-of-a-polygon) to the midpoint of the opposite side of a [triangle](#triangle). For side lengths $a,b,c$, the median to the side of length $c$ has length $m_c=\tfrac12\sqrt{2a^2+2b^2-c^2}$, by [Apollonius's theorem](#apollonius-s-theorem).

<h3 id="heron-s-formula">Heron's formula</h3>

↑ **Parent:** [Triangle](#triangle)

For a [triangle](#triangle) with side lengths $a,b,c$ and [semiperimeter](#semiperimeter) $s=(a+b+c)/2$, its [area](differential-geometry.md#surface-area) is $A=\sqrt{s(s-a)(s-b)(s-c)}$. This expresses the [area](differential-geometry.md#surface-area) using only the three side lengths.

### Circumradius

↑ **Parent:** [Triangle](#triangle)

The [radius](topology.md#radius) of a [triangle](#triangle)'s circumscribed [circle](topology.md#circle), whose center is the [circumcenter](#circumcenter). For side lengths $a,b,c$ and [area](differential-geometry.md#surface-area) $A$, it satisfies $R=abc/(4A)$.

### Incenter

↑ **Parent:** [Triangle](#triangle)

The intersection of a [triangle](#triangle)'s internal [angle bisectors](geometry-and-topology.md#angle-bisector). It is the center of the circle tangent to all three sides, and its distance to any side is the [inradius](#inradius).

### Angle bisector theorem

↑ **Parent:** [Triangle](#triangle)

An internal [angle bisector](geometry-and-topology.md#angle-bisector) of a [triangle](#triangle) divides the opposite side in the ratio of the two adjacent sides. If $AD$ bisects the [angle](geometry-and-topology.md#angle) at $A$ in [triangle](#triangle) $ABC$, then $BD/DC=AB/AC$. Comparing the [areas](differential-geometry.md#surface-area) of [triangles](#triangle) $ABD$ and $ACD$ proves this: their shared altitude gives the ratio $BD/DC$, while their equal included [angles](geometry-and-topology.md#angle) give $AB/AC$.

### Fermat point

↑ **Parent:** [Triangle](#triangle)

### Law of sines

↑ **Parent:** [Triangle](#triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_sines)

In a nondegenerate [triangle](#triangle), let $a,b,c$ be the side lengths opposite the interior [angles](geometry-and-topology.md#angle) $A,B,C$. Its [area](differential-geometry.md#surface-area) $K$ satisfies $2K=bc\sin A=ca\sin B=ab\sin C$. Division by $abc>0$ proves the law of sines. The area formula itself follows by taking the magnitude of the [cross product](vector-space.md#cross-product) of two edge vectors. Unlike the [law of cosines](#law-of-cosines), this relation alone may leave an ambiguity between two supplementary angles when two sides and a nonincluded angle are given.

### Orthocenter

↑ **Parent:** [Triangle](#triangle)

The common intersection of a [triangle](#triangle)'s three altitude lines. Each line passes through a vertex and is [orthogonal](inner-product.md#orthogonal-vectors) to the opposite side. The intersection can lie inside or outside the triangle, or at its right-angle vertex. An [orthogonal projection onto an intercept plane](geometry-and-topology.md#orthogonal-projection-onto-an-intercept-plane) supplies a concrete three-dimensional construction of one.

### Isosceles triangle

↑ **Parent:** [Triangle](#triangle)

An isosceles [triangle](#triangle) has two equal sides. Its [angles](geometry-and-topology.md#angle) opposite those sides are equal: reflecting the triangle across the bisector of the angle between the equal sides exchanges them and fixes the opposite side as a set. A [triangle](#triangle) formed by two [radii](topology.md#radius) of one [circle](topology.md#circle) is therefore isosceles.

### Similar triangle

↑ **Parent:** [Triangle](#triangle)

Two [triangles](#triangle) are similar if a [Euclidean similarity](geometry-and-topology.md#euclidean-similarity) maps one onto the other. Their corresponding [angles](geometry-and-topology.md#angle) agree, and corresponding side [lengths](physics.md#length) have a common positive ratio.

Specify the correspondence first: $A$ matches $A'$, $B$ matches $B'$ and $C$ matches $C'$. For [similar triangles](#similar-triangle), the common scale factor $k>0$ satisfies

$$
\frac{|A'B'|}{|AB|}=\frac{|B'C'|}{|BC|}=\frac{|C'A'|}{|CA|}=k.
$$

The [ratios](arithmetic.md#ratio) compare matching sides in the same order. A [Euclidean similarity](geometry-and-topology.md#euclidean-similarity) can also move, turn or reflect the [triangle](#triangle); its orientation on the page is irrelevant. In the [Euclidean plane](geometry-and-topology.md#euclidean-plane), matching just two interior [angles](geometry-and-topology.md#angle) is enough: their sums force the third to match, and equal corresponding [angles](geometry-and-topology.md#angle) force the side [ratios](arithmetic.md#ratio) to agree. This is the angle-angle (AA) criterion for [similar triangles](#similar-triangle). Matching just one [angle](geometry-and-topology.md#angle) is insufficient.

Scale the [right triangle](#right-triangle) with vertices $(0,0)$, $(4,0)$ and $(0,3)$ by $k=2$. Its new vertices are $(0,0)$, $(8,0)$ and $(0,6)$, and its side [lengths](physics.md#length) are $6,8,10$. The matching side [ratios](arithmetic.md#ratio) are $6/3=8/4=10/5=2$. Both [triangles](#triangle) have a [right angle](#right-angle) and the same two other interior [angles](geometry-and-topology.md#angle), approximately $36.87^\circ$ and $53.13^\circ$. However, their [areas](differential-geometry.md#surface-area) are $3\cdot4/2=6$ and $6\cdot8/2=24$: doubling [lengths](physics.md#length) multiplies [area](differential-geometry.md#surface-area) by four.

<a id="image-similar-3-4-5-and-6-8-10-right-triangles-side-lengths-multiply-by-2-while-area-multiplies-by-2-2-4"></a>
![](similar-triangle-scaling.png)

**[Figure 5](#image-similar-3-4-5-and-6-8-10-right-triangles-side-lengths-multiply-by-2-while-area-multiplies-by-2-2-4). Similar 3-4-5 and 6-8-10 right triangles: side lengths multiply by $2$, while area multiplies by $2^2=4$**.

Generally, a [Euclidean similarity](geometry-and-topology.md#euclidean-similarity) multiplies both a base and its perpendicular height by $k$, so the [area](differential-geometry.md#surface-area) becomes $\tfrac12(kb)(kh)=k^2\tfrac12bh$. This explains why an enlarged drawing needs four times as much surface when each [length](physics.md#length) doubles. It also enables indirect measurement: under assumptions of level ground, vertical objects and parallel light rays, an object of height $3$ casting a shadow of [length](physics.md#length) $4$ provides a [right triangle](#right-triangle). Another object's shadow of [length](physics.md#length) $8$ gives a [similar triangle](#similar-triangle) and height $3(8/4)=6$. The shared [angles](geometry-and-topology.md#angle) justify the inference; visual resemblance alone does not.

[Euclid's Elements](#euclid-s-elements) VI, Definition 1 describes similarity using corresponding [angles](geometry-and-topology.md#angle) and proportional sides. VI.4 establishes the implication from matching [angles](geometry-and-topology.md#angle) to matching side [ratios](arithmetic.md#ratio), while VI.19 states the squared relation between side [ratios](arithmetic.md#ratio) and [areas](differential-geometry.md#surface-area). These are documented ancient formulations of the principles used above, without establishing a first discoverer.[Euclid, Elements VI, Definition 1](https://mathcs.clarku.edu/~djoyce/elements/bookVI/defVI1.html)[Euclid, Elements VI.4](https://mathcs.clarku.edu/~djoyce/elements/bookVI/propVI4.html)[Euclid, Elements VI.19](https://mathcs.clarku.edu/~djoyce/elements/bookVI/propVI19.html)

### Incircle of a triangle

↑ **Parent:** [Triangle](#triangle)

The [incircle of a triangle](#incircle-of-a-triangle) is the [circle](topology.md#circle) inside the [triangle](#triangle) tangent to all three sides. Its center is the intersection of two internal angle bisectors; its radius is $r=\Delta/s$, where $\Delta$ is the area and $s$ the semiperimeter. To prove it is the largest contained [circle](topology.md#circle), let any candidate have center $P$, radius $\rho$ and distances $d_i\geq\rho$ from the three side lines. Splitting the [triangle](#triangle) into three [triangles](#triangle) with vertex $P$ gives $\Delta=\frac12\sum_i\ell_i d_i\geq s\rho$. The tangent [circle](topology.md#circle) attains equality, proving maximality. For a [right triangle](#right-triangle) with legs $a,b$ and hypotenuse $c$, $r=(a+b-c)/2$, since $r=ab/(a+b+c)$ and $a^2+b^2=c^2$.

#### Inradius

↑ **Parent:** [Incircle of a triangle](#incircle-of-a-triangle)

The inradius is the [radius](topology.md#radius) of an [incircle](#incircle-of-a-triangle). For a [triangle](#triangle) of [area](differential-geometry.md#surface-area) $A$ and [semiperimeter](#semiperimeter) $s$, it is $r=A/s$: joining the [incenter](#incenter) to the three vertices partitions the [triangle](#triangle) into three [triangles](#triangle) with common altitude $r$.

### Circumcircle

↑ **Parent:** [Triangle](#triangle)

The [circumcircle](#circumcircle) of a nondegenerate [triangle](#triangle) is the unique [circle](topology.md#circle) through its three vertices. Its center is the [circumcenter](#circumcenter), found by intersecting two [perpendicular bisectors](#perpendicular-bisector); equality of distances to all three vertices proves existence, and subtracting the squared-distance equations proves uniqueness. For a [right triangle](#right-triangle), the midpoint of its hypotenuse is equidistant from all vertices, so its circumradius is half the hypotenuse length.

### Law of cosines

↑ **Parent:** [Triangle](#triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_cosines)

For a [triangle](#triangle) with side lengths $a,b,c$ and angle $C$ opposite $c$, the law of cosines states

$$
c^2=a^2+b^2-2ab\cos C.
$$

### Acute triangle

↑ **Parent:** [Triangle](#triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acute_triangle)

An acute triangle has all three interior angles strictly smaller than a right angle.

### Equilateral triangle

↑ **Parent:** [Triangle](#triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equilateral_triangle)

An equilateral triangle has three equal side lengths.

### Right triangle

↑ **Parent:** [Triangle](#triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Right_triangle)

A right triangle has one interior angle equal to a right angle.

#### Leg of a right triangle

↑ **Parent:** [Right triangle](#right-triangle)

#### Hypotenuse

↑ **Parent:** [Right triangle](#right-triangle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypotenuse)

The [hypotenuse](#hypotenuse) is the side opposite the [right angle](#right-angle) in a [right triangle](#right-triangle). Its [length](physics.md#length) $c$ is determined by the [Pythagorean theorem](#pythagorean-theorem).

## Trapezoid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trapezoid)

A trapezium is a quadrilateral with at least one pair of parallel opposite sides.

## Triangular prism

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangular_prism)

A triangular prism is the orthogonal [Cartesian product](set-theory.md#cartesian-product) of a [triangle](#triangle) with a [line segment](convex-set.md#line-segment).

## Borsuk conjecture

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borsuk_conjecture)

The Borsuk conjecture asserted that every bounded subset of $\mathbb R^d$ with positive diameter can be partitioned into $d+1$ subsets of strictly smaller diameter. It is false in sufficiently high dimension.

### Kahn-Kalai counterexample to the Borsuk conjecture

↑ **Parent:** [Borsuk conjecture](#borsuk-conjecture)

Kahn and Kalai represented uniform subsets by quadratic sign vectors so that diameter pairs correspond to one forbidden intersection size. The [Frankl-Wilson theorem](extremal-set-theory.md#frankl-wilson-theorem) bounds each smaller-diameter part, forcing exponentially many parts while the ambient dimension grows only quadratically.

#### Quadratic sign-vector diameter formula

↑ **Parent:** [Kahn-Kalai counterexample to the Borsuk conjecture](#kahn-kalai-counterexample-to-the-borsuk-conjecture)

Take $N=4p-1$, $|A|=|B|=2p-1$ and sign [vectors](vector-space.md#vector) $u_A=2\mathbf1_A-\mathbf1$. The [Frobenius inner product](inner-product.md#frobenius-inner-product) of two outer products is $(u_A\cdot u_B)^2$, proving the formula. The squared [Euclidean distance](topological-analysis.md#euclidean-distance) is largest precisely when $|A\cap B|=p-1$, where the inner product is minus one. The common diagonal can be deleted, leaving an isometric representation in dimension $\binom N2$ if off-diagonal coordinates are multiplied by $\sqrt2$. The [Frankl-Wilson theorem](extremal-set-theory.md#frankl-wilson-theorem) then bounds each smaller-[diameter](topological-analysis.md#diameter) class.

#### Borsuk counterexample in dimension 1325

↑ **Parent:** [Kahn-Kalai counterexample to the Borsuk conjecture](#kahn-kalai-counterexample-to-the-borsuk-conjecture)

Use the [balanced cut-vector distance formula](#balanced-cut-vector-distance-formula) with $p=13$. There are $\binom{51}{25}=247959266474052$ distinct cuts. A subset of strictly smaller [diameter](topological-analysis.md#diameter) contains no pair with side intersection thirteen, so deleting their shared coordinate one and applying the [Frankl-Wilson theorem](extremal-set-theory.md#frankl-wilson-theorem) bounds its size by $\binom{51}{12}=158753389900$. At least 1562 smaller-diameter parts are needed, exceeding $1325+1$. The cut vectors occupy an [affine hyperplane](vector-space.md#affine-hyperplane) in $\mathbb R^{1326}$, which identifies isometrically with $\mathbb R^{1325}$ and gives the stated explicit counterexample.

#### Balanced cut-vector distance formula

↑ **Parent:** [Kahn-Kalai counterexample to the Borsuk conjecture](#kahn-kalai-counterexample-to-the-borsuk-conjecture)

Represent a balanced partition of $[4p]$ by the zero-one vector recording which unordered pairs lie across its cut. Complementary subsets represent the same cut; choose the representative containing coordinate one. Two such cuts differ on the pairs crossing the [symmetric difference](set.md#symmetric-difference) of their sides, giving the displayed distance. Its maximum is $4p^2$, attained exactly when $t=p$. Every cut has $4p^2$ occupied coordinates, so the vectors lie in an [affine hyperplane](vector-space.md#affine-hyperplane) of dimension at most $\binom{4p}{2}-1$.

### Volumetric covering bound

↑ **Parent:** [Borsuk conjecture](#borsuk-conjecture)

The unit ball in $\mathbb R^n$ can be covered by at most $9^n$ balls of radius $1/4$. A maximal $1/4$-separated set supplies the centres, and disjoint radius-$1/8$ balls around them fit inside the ball of radius $9/8$.

## Unit disk

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_disk)

The open unit disk in the [Euclidean plane](euclidean-geometry.md) is

$$
\{(x,y)\in\mathbb R^2:x^2+y^2<1\}.
$$

## Cyclic quadrilateral

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_quadrilateral)

A cyclic quadrilateral has all four vertices on one circle. Among quadrilaterals with fixed cyclically ordered side lengths, a cyclic quadrilateral has maximal area.

<h3 id="brahmagupta-s-formula">Brahmagupta's formula</h3>

↑ **Parent:** [Cyclic quadrilateral](#cyclic-quadrilateral)

## Locus (mathematics)

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locus_(mathematics))

A locus is the [set](set.md) of [points](geometry-and-topology.md#point-geometry) satisfying specified geometric conditions. A [circle](topology.md#circle) is the locus at fixed [Euclidean distance](topological-analysis.md#euclidean-distance) from a point; an [ellipse](#ellipse) is the locus with fixed sum of distances to its [foci of a conic](#focus-of-a-conic).

## Conic section

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conic_section)

A conic section is obtained by intersecting a [plane](geometry-and-topology.md#plane) with a [double circular cone](#double-circular-cone). Cuts away from the vertex produce an [ellipse](#ellipse), a [parabola](#parabola) or a [hyperbola](#hyperbola); a perpendicular cut is the [circle](topology.md#circle) case of an [ellipse](#ellipse). A cut through the vertex can instead produce a [degenerate conic](#degenerate-conic). One simple surface therefore connects several familiar [plane curves](algebraic-geometry.md#plane-curve).[Precalculus 2e, §10.1, Writing Equations of Ellipses in Standard Form, Figure 2](mathematics-bibliography.md#precalculus-2e-by-jay-abramson/10-1-the-ellipse)

Consider the original family

$$
z^2=x^2+y^2,\qquad z=1+mx.
$$

Substituting the [plane equation](geometry-and-topology.md#cartesian-equation-of-a-plane) into the [double circular cone](#double-circular-cone) equation gives

$$
(1-m^2)x^2+y^2-2mx-1=0.
$$

Thus $m=0$ gives a [circle](topology.md#circle), $m=3/5$ an [ellipse](#ellipse), $m=1$ a [parabola](#parabola), and $m=7/5$ a [hyperbola](#hyperbola). The last cut meets both sheets of the [double circular cone](#double-circular-cone), producing its two branches. These parameters specify a mathematical family, rather than measurements of a physical object.

<a id="image-circle-ellipse-parabola-and-hyperbola-from-four-cuts-of-one-double-circular-cone"></a>
![](conic-sections-double-cone-plane-cuts.png)

**[Figure 6](#image-circle-ellipse-parabola-and-hyperbola-from-four-cuts-of-one-double-circular-cone). Circle, ellipse, parabola and hyperbola from four cuts of one double circular cone**. Original three-dimensional intersections of $z^2=x^2+y^2$ with $z=1+mx$. The cone meshes and planes are finite displayed patches. The [circle](topology.md#circle) can look elliptical in the perspective view; its intrinsic geometry is circular.

The [Cartesian coordinate system](linear-algebra.md#cartesian-coordinate-system) descriptions of these curves are second-degree equations

$$
Ax^2+Bxy+Cy^2+Dx+Ey+F=0.
$$

A [rotation](riemannian-geometry.md#rotation-mathematics) and a [translation](geometry-and-topology.md#translation-geometry) expose their principal directions and offsets. The [conic type discriminant](#conic-type-discriminant) identifies the ordinary nondegenerate real type, while a separate [degenerate conic](#degenerate-conic) check prevents confusing two crossing [straight lines](#straight-line) with a [hyperbola](#hyperbola).

This is useful because a difficult-looking equation can be understood through a small set of geometric features: [foci of a conic](#focus-of-a-conic), [directrices of a conic](#directrix-of-a-conic), [eccentricity of a conic](#eccentricity-of-a-conic) and the [semi-major and semi-minor axes](#semi-major-and-semi-minor-axes). The same [ellipse](#ellipse) can be traced by a constant-length string or parametrized by $x=a\cos t$, $y=b\sin t$. These are different descriptions of one curve, with different advantages for construction and calculation.

### Conic type discriminant

↑ **Parent:** [Conic section](#conic-section)

For a second-degree equation $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$, the number $\Delta_2=B^2-4AC$ is the [discriminant of a binary quadratic form](number-theory.md#discriminant-of-a-binary-quadratic-form) associated with its quadratic part. For a nonempty, nondegenerate real [conic section](#conic-section), a negative value gives an [ellipse](#ellipse), zero a [parabola](#parabola), and a positive value a [hyperbola](#hyperbola). It is invariant under a [rotation](riemannian-geometry.md#rotation-mathematics) of orthonormal coordinates.[Precalculus 2e, §10.4, Identifying Conics without Rotating Axes and Using the Discriminant to Identify a Conic](mathematics-bibliography.md#precalculus-2e-by-jay-abramson/10-4-rotation-of-axes)

A short explanation uses the [symmetric matrix](linear-algebra.md#symmetric-matrix)

$$
H=\begin{pmatrix}A&B/2\\B/2&C\end{pmatrix},\qquad \Delta_2=-4\det H.
$$

An [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $R$ changes this matrix to $R^{\mathsf T}HR$, whose [determinant](multilinear-algebra.md#determinant) equals $\det H$. The [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) then removes the mixed term. Equal-sign, opposite-sign and one-zero [eigenvalues](linear-operator-theory.md#eigenvalue) give the three types after the remaining linear terms and offsets are considered.

The qualification matters. The equations $x^2+y^2=0$, $y^2=0$ and $xy=0$ describe a [point](geometry-and-topology.md#point-geometry), a repeated [straight line](#straight-line), and two crossing [straight lines](#straight-line), respectively. Their quadratic discriminants have the signs expected of ellipse, parabola and hyperbola types, but all three are [degenerate conics](#degenerate-conic). Also, $x^2+y^2=-1$ has an [empty set](set.md#empty-set) of real solutions despite its negative quadratic discriminant.

### Degenerate conic

↑ **Parent:** [Conic section](#conic-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degenerate_conic)

For $Ax^2+Bxy+Cy^2+Dx+Ey+F=0$, the homogeneous quadratic coefficient matrix is

$$
Q=\begin{pmatrix}A&B/2&D/2\\B/2&C&E/2\\D/2&E/2&F\end{pmatrix}.
$$

The conic is degenerate when $Q$ is a [singular matrix](linear-algebra.md#singular-matrix). Examples over the [real numbers](arithmetic.md#real-number) include the point $x^2+y^2=0$, the repeated line $y^2=0$, and the two [straight lines](#straight-line) in $xy=0$. The real solution set alone need not reveal the algebraic distinction: $x^2+y^2=-1$ has no real points, but its matrix is nonsingular. This determinant test is different from the [conic type discriminant](#conic-type-discriminant), which only uses the quadratic part in $x,y$.

### Directrix of a conic

↑ **Parent:** [Conic section](#conic-section)

A [directrix of a conic](#directrix-of-a-conic) is the fixed line in its focus-directrix description: distance to the [focus of a conic](#focus-of-a-conic) is a constant multiple of distance to this line. For a [parabola](#parabola) the multiple is one. The [directrix of a conic](#directrix-of-a-conic) belongs to the geometry of the [conic section](#conic-section), rather than being a tangent or an asymptote.

### Focus of a conic

↑ **Parent:** [Conic section](#conic-section)

In the focus-directrix description of a noncircular [conic section](#conic-section), the focus is the fixed point $F$ for which every point $X$ of the curve satisfies $|X-F|=e\,\operatorname{dist}(X,L)$, where $L$ is a [directrix of a conic](#directrix-of-a-conic) and $e$ is the [eccentricity of a conic](#eccentricity-of-a-conic). For $y^2=4ax$ with $a>0$, the [focus of a conic](#focus-of-a-conic) is $(a,0)$, the [directrix of a conic](#directrix-of-a-conic) is $x=-a$, and $e=1$.

### Eccentricity of a conic

↑ **Parent:** [Conic section](#conic-section)

The parameter $e\geq0$ in a focus-centred [polar coordinates](multivariable-calculus.md#polar-coordinates) equation $r=\ell/(1-e\cos\theta)$ for a [conic section](#conic-section). It distinguishes an [ellipse](#ellipse) ($e<1$), a [parabola](#parabola) ($e=1$), and a [hyperbola](#hyperbola) ($e>1$).

For a noncircular [conic section](#conic-section), the [eccentricity of a conic](#eccentricity-of-a-conic) is the constant ratio

$$
e=\frac{\operatorname{dist}(X,F)}{\operatorname{dist}(X,L)},
$$

where $F$ is a [focus of a conic](#focus-of-a-conic), $L$ the corresponding [directrix of a conic](#directrix-of-a-conic), and $X$ a point on the curve. For an [ellipse](#ellipse) with [semi-major axis](celestial-mechanics.md#semi-major-axis) $a$ and distance $c$ from the focal [midpoint](convex-set.md#midpoint) to either [focus of a conic](#focus-of-a-conic), $e=c/a=\sqrt{1-b^2/a^2}$. Its [circle](topology.md#circle) case has $e=0$; a finite directrix does not give that circle through the displayed ratio. The circle is the limit as $c\to0$ and its [directrices of a conic](#directrix-of-a-conic) move arbitrarily far away.

The [eccentricity of a conic](#eccentricity-of-a-conic) is intrinsic to the cutting [plane](geometry-and-topology.md#plane), and is not generally its slope in a chosen three-dimensional drawing. For the family $z=1+mx$ in [conic section](#conic-section), with $0<m<1$, completing the square gives

$$
(1-m^2)\left(x-\frac{m}{1-m^2}\right)^2+y^2=\frac1{1-m^2}.
$$

A [displacement](classical-mechanics.md#displacement) $dx$ along this [plane](geometry-and-topology.md#plane) has [Euclidean norm](normed-vector-space.md#euclidean-norm) $\sqrt{1+m^2}|dx|$. Thus the intrinsic semiaxis ratio satisfies $b^2/a^2=(1-m^2)/(1+m^2)$, giving

$$
e=\frac{\sqrt2m}{\sqrt{1+m^2}}.
$$

For $m=3/5$, this is $3/\sqrt{17}$, rather than $3/5$. This normalization separates the curve's geometry from a distorted projection of it onto the $xy$ plane.

### Semilatus rectum

↑ **Parent:** [Conic section](#conic-section)

The distance from a focus to a [conic section](#conic-section) along a line perpendicular to its symmetry axis. In focus-centred [polar coordinates](multivariable-calculus.md#polar-coordinates), an [ellipse](#ellipse) may be written $r(1-e\cos\theta)=\ell$, where $e$ is its [eccentricity of a conic](#eccentricity-of-a-conic).

### Parabola

↑ **Parent:** [Conic section](#conic-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parabola)

A parabola is a [plane curve](algebraic-geometry.md#plane-curve) whose points are equally distant from a focus and a directrix. In suitable coordinates it has equation $y=ax^2$, with $a\ne0$. Its quadratic geometry can also describe a [contour deformation](complex-analysis.md#contour-deformation) through a [saddle point](analysis.md#saddle-point).

For example, take a [focus of a conic](#focus-of-a-conic) at $(1,0)$ and a [directrix of a conic](#directrix-of-a-conic) $x=-1$. Equality of squared [Euclidean distances](topological-analysis.md#euclidean-distance) gives $(x-1)^2+y^2=(x+1)^2$, hence $y^2=4x$. The point $(1,2)$ has distance $2$ to both the focus and the directrix. Its [eccentricity of a conic](#eccentricity-of-a-conic) is one. Unlike an [ellipse](#ellipse), a [parabola](#parabola) is unbounded and has only one matched focus-directrix description.

#### Vertex of a parabola

↑ **Parent:** [Parabola](#parabola)

For a [parabola](#parabola) described by the [function graph](function.md#graph-of-a-function) $y=a(x-h)^2+k$, with nonzero $a$ in the [real numbers](arithmetic.md#real-number), its [vertex of a parabola](#vertex-of-a-parabola) is the [point](geometry-and-topology.md#point-geometry) $(h,k)$. This point gives its [minimum](set.md#minimum-of-a-subset-of-a-total-order) or [maximum](set.md#maximum-of-a-subset-of-a-total-order) value of $y$ in these coordinates.

### Hyperbola

↑ **Parent:** [Conic section](#conic-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbola)

A hyperbola is a [conic section](#conic-section) with two unbounded branches. In suitable coordinates its equation is $x^2/a^2-y^2/b^2=1$ with $a,b>0$. The unit hyperbola is parametrized by $x=\cosh t$, $y=\sinh t$ on its right branch, relating it to the [hyperbolic functions](calculus.md#hyperbolic-function).

For example, $x^2/9-y^2/16=1$ has [foci of a conic](#focus-of-a-conic) at $(\pm5,0)$, because $5^2=3^2+4^2$. Its focal-distance difference has absolute value $6$, while its [eccentricity of a conic](#eccentricity-of-a-conic) is $5/3>1$. At the point $(3,0)$, the focal distances are $8$ and $2$, verifying that difference. The [asymptotes](topology.md#asymptote) are $y=\pm4x/3$; a distant point approaches those directions while remaining on one of the two branches. The focal-distance difference, rather than a constant sum, distinguishes this [hyperbola](#hyperbola) from an [ellipse](#ellipse).

#### Rectangular hyperbola

↑ **Parent:** [Hyperbola](#hyperbola)

A [hyperbola](#hyperbola) whose two asymptotes are perpendicular. After a suitable choice of coordinates it has equation $xy=c$ for a nonzero constant $c$. In the form $x^2/a^2-y^2/b^2=1$, it is rectangular exactly when $a=b$.

#### Hyperbolic parametrization of a hyperbola

↑ **Parent:** [Hyperbola](#hyperbola)

For nonzero real $a,b$, the identity $\cosh^2t-\sinh^2t=1$ eliminates the parameter. The additional condition $x/a=\cosh t\geq1$ is essential: the parametrization traces only the branch with the sign of $a$. Every point of that branch is obtained by $t=\operatorname{arsinh}(y/b)$. Its vertex is $(a,0)$ and its asymptotes are $y=\pm(b/a)x$. An algebraic equation alone would also include the opposite branch, which this real parametrization never reaches.

#### Focal-distance identity for a hyperbola

↑ **Parent:** [Hyperbola](#hyperbola)

For $x^2/a^2-y^2/b^2=1$, let $c=\sqrt{a^2+b^2}$ and place the [foci of a conic](#focus-of-a-conic) at $(\pm c,0)$. On the right branch write $x=a\cosh t$, $y=b\sinh t$. Direct expansion gives

$$
d_-^2=(x+c)^2+y^2=(c\cosh t+a)^2,\qquad
d_+^2=(x-c)^2+y^2=(c\cosh t-a)^2.
$$

Since $c>a>0$, both square roots are positive and $d_--d_+=2a$. On the reflected left branch the signed difference reverses, while its absolute value stays $2a$. This proves the constant-difference characterization of a [hyperbola](#hyperbola) and keeps track of which branch a [hyperbolic function](calculus.md#hyperbolic-function) parametrization covers.

### Ellipse

↑ **Parent:** [Conic section](#conic-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ellipse)

An ellipse is the [locus](#locus-mathematics) of [points](geometry-and-topology.md#point-geometry) whose [Euclidean distances](topological-analysis.md#euclidean-distance) from two fixed [foci of a conic](#focus-of-a-conic) have constant sum $2a$. If the distance between the [foci of a conic](#focus-of-a-conic) is $d<2a$, the [semi-major and semi-minor axes](#semi-major-and-semi-minor-axes) are $a$ and $\sqrt{4a^2-d^2}/2$. Writing $c=d/2$ gives the conventional relation $b^2=a^2-c^2$.[Precalculus 2e, §10.1, ellipse definition and Deriving the Equation of an Ellipse Centered at the Origin, Figure 5](mathematics-bibliography.md#precalculus-2e-by-jay-abramson/10-1-the-ellipse)

For an original calculation, choose $a=5$, $b=3$, and hence $c=4$. The [ellipse](#ellipse)

$$
\boxed{\frac{x^2}{25}+\frac{y^2}{9}=1}
$$

has [foci of a conic](#focus-of-a-conic) $F_-=(-4,0)$ and $F_+=(4,0)$. The point $P=(3,12/5)$ lies on it since $9/25+16/25=1$. Its focal distances are

$$
|P-F_-|=\frac{37}5,\qquad |P-F_+|=\frac{13}5,\qquad |P-F_-|+|P-F_+|=10.
$$

Its [eccentricity of a conic](#eccentricity-of-a-conic) is $e=4/5$. The matching [directrix of a conic](#directrix-of-a-conic) for $F_+$ is $x=a/e=25/4$, and the perpendicular distance from $P$ to that [straight line](#straight-line) is $13/4$. Therefore the ratio of focal distance to directrix distance is $(13/5)/(13/4)=4/5$, agreeing with $e$.

<a id="image-one-ellipse-has-a-constant-focal-distance-sum-and-a-constant-focus-directrix-ratio"></a>
![](ellipse-focal-distances-and-directrix.png)

**[Figure 7](#image-one-ellipse-has-a-constant-focal-distance-sum-and-a-constant-focus-directrix-ratio). One ellipse has a constant focal-distance sum and a constant focus-directrix ratio**. Original example with semiaxes $5,3$, foci at $(\pm4,0)$, and $P=(3,12/5)$. The left triangle represents a taut closed-loop construction; the right panel uses one matched focus and directrix. All lengths are in the same arbitrary unit.

The constant sum can be turned into a construction. Fix a pin at each [focus of a conic](#focus-of-a-conic) and pull a closed string loop taut with a pencil. In this example the segment between the pins has length $8$, so a loop of length $18$ leaves $10$ for the two pencil-to-pin segments. Moving the pencil while keeping that loop taut traces the [ellipse](#ellipse). This is a geometric prediction from the length constraint, not an assertion about a measured drawing.

The parametrization $x=5\cos t$, $y=3\sin t$ maps the [unit circle](complex-analysis.md#complex-unit-circle) onto this [ellipse](#ellipse). It makes plotting easy, but is an [affine map](geometry-and-topology.md#affine-map) rather than an [isometry](riemannian-geometry.md#isometry): horizontal and vertical lengths have different scale factors. An [ellipse](#ellipse) is not a [circle](topology.md#circle) under the original [Euclidean metric](riemannian-metric.md#euclidean-metric) merely because this map exists. Its two semiaxes and [eccentricity of a conic](#eccentricity-of-a-conic) retain the metric information lost by that equivalence.

A useful proof outline begins with $|X-F_-|+|X-F_+|=2a$. Isolate one [square root](algebra.md#square-root), square, and then repeat; the resulting [quadratic equation](polynomial.md#quadratic-equation) is $x^2/a^2+y^2/(a^2-c^2)=1$. Since $a>c$, the quantities isolated before squaring have the required signs, so the reverse implication introduces no extra branch. The condition $a>c$ is essential: at equality the focal-distance locus becomes the [line segment](convex-set.md#line-segment) between the [foci of a conic](#focus-of-a-conic).

#### Steiner inellipse

↑ **Parent:** [Ellipse](#ellipse)

The Steiner inellipse of a nondegenerate [triangle](#triangle) is the unique [ellipse](#ellipse) of largest [area](differential-geometry.md#surface-area) contained in the [triangle](#triangle). Its center is the [centroid](#centroid), and it touches each side at its midpoint.

#### Affine image of a circle

↑ **Parent:** [Ellipse](#ellipse)

Let a radius-$R$ [circle](topology.md#circle) have center $c\in\mathbb R^2$, and apply the real [affine map](geometry-and-topology.md#affine-map) $y=Mx+b$. If $M$ is invertible, substitute $x-c=M^{-1}(y-Mc-b)$ into $|x-c|^2=R^2$ to obtain the displayed [ellipse](#ellipse). Its center is $Mc+b$ and its semiaxes are $R$ times the two [singular values](linear-algebra.md#singular-value) of $M$, as follows from the [singular value decomposition](linear-algebra.md#singular-value-decomposition). A rotation or reflection preserves both semiaxes and hence gives another circle. If $M$ has rank one, the image is a segment; rank zero gives one point. This real-plane description also handles maps that stretch real and imaginary coordinates differently and are not holomorphic complex maps.

#### Semi-major and semi-minor axes

↑ **Parent:** [Ellipse](#ellipse)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semi-major_and_semi-minor_axes)

The [semi-major and semi-minor axes](#semi-major-and-semi-minor-axes) are the larger and smaller half-axis lengths of an [ellipse](#ellipse). In principal-axis coordinates the [ellipse](#ellipse) has equation $x^2/a^2+y^2/b^2=1$ with $a\ge b>0$. The same terminology is used for a [hyperbola](#hyperbola) $x^2/a^2-y^2/b^2=1$, where $a$ is half its transverse axis and $b$ half its conjugate axis. Orbital semiaxes apply these geometric quantities to [conic sections](#conic-section).

#### Ellipse perimeter expansion near a circle

↑ **Parent:** [Ellipse](#ellipse)

For an [ellipse](#ellipse) with semiaxes $1,x$, the perimeter integral has integrand $\sqrt{1-t\cos^2\theta}$. The uniformly convergent [binomial series](sequence-and-series.md#binomial-series) near $t=0$ permits termwise integration. Integrals of $\cos^2\theta$ and $\cos^4\theta$ over a full period give the displayed first corrections. The same coefficients follow from the [Frobenius method](complex-analysis.md#frobenius-method) for the transformed perimeter equation.

#### Nondegenerate ellipse

↑ **Parent:** [Ellipse](#ellipse)

A nondegenerate ellipse has two positive semiaxis lengths. It is a smooth closed curve rather than a point or line segment.

##### Parity and upper bound for transverse ellipse intersections

↑ **Parent:** [Nondegenerate ellipse](#nondegenerate-ellipse)

Parametrize one [ellipse](#ellipse) as $\gamma(t)=c+A(\cos t,\sin t)$ and substitute it into the quadratic equation $Q=0$ of the other. At a [transverse intersection](smooth-manifold.md#transverse-intersection), $g(t)=Q(\gamma(t))$ has a simple zero, so its sign changes. Periodicity makes the number of zeros even. The function is a [trigonometric polynomial](fourier-series.md#trigonometric-polynomial) of degree at most two, so multiplication by $z^2$, with $z=e^{it}$, gives a nonzero polynomial of degree at most four. Hence there are at most four distinct intersection points. Coincident ellipses are excluded by transversality.

#### Focal line

↑ **Parent:** [Ellipse](#ellipse)

The focal line of an [ellipse](#ellipse) is the straight line through its two foci.

## Ellipsoid

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ellipsoid)

An ellipsoid is a level set $(x-c)^TA(x-c)=1$ for a real symmetric [positive-definite matrix](quadratic-form.md#positive-definite-matrix) $A$. Its principal axes are the orthonormal eigenvectors of $A$, and an eigenvalue $\lambda$ gives semi-axis length $1/\sqrt\lambda$.

### Nearest points to the origin on a positive-definite ellipsoid

↑ **Parent:** [Ellipsoid](#ellipsoid)

For a [positive-definite symmetric matrix](linear-algebra.md#symmetric-positive-definite-matrix) $A$, the [ellipsoid](#ellipsoid) $x^TAx=1$ has nearest points to the origin exactly at $x=\lambda_{\max}^{-1/2}u$, where $u$ ranges over [unit vectors](vector-space.md#unit-vector) in the largest-[eigenvalue](linear-operator-theory.md#eigenvalue) [eigenspace](linear-operator-theory.md#eigenspace). Indeed, the [spectral theorem for real symmetric matrices](linear-algebra.md#spectral-theorem-for-real-symmetric-matrices) gives $x^TAx\leq\lambda_{\max}|x|^2$, with equality precisely in that [eigenspace](linear-operator-theory.md#eigenspace). A simple largest [eigenvalue](linear-operator-theory.md#eigenvalue) gives two opposite nearest points; multiplicity $m>1$ gives a scaled $(m-1)$-sphere of nearest points.

### Solid ellipsoid

↑ **Parent:** [Ellipsoid](#ellipsoid)

The interior bounded by an [ellipsoid](#ellipsoid) is a solid ellipsoid. Positive coordinate dilations multiply its [symplectic capacity](symplectic-geometry.md#symplectic-capacity) by the square of the dilation factor.

#### Cartesian second moment of a solid ellipsoid

↑ **Parent:** [Solid ellipsoid](#solid-ellipsoid)

For the [solid ellipsoid](#solid-ellipsoid) $D=\{x^2/a^2+y^2/b^2+z^2/c^2\le1\}$ with positive semi-axes, set $x=au$, $y=bv$, $z=cw$. The [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) of this inverse coordinate map is $abc$, and $D$ becomes the unit ball. Symmetry gives $\int_{B_1}u^2\,dV=\frac13\int_{B_1}r^2\,dV=4\pi/15$, proving the displayed moment. The other two moments follow by interchanging the semi-axes; mixed moments vanish by reflection symmetry.

### John ellipsoid

↑ **Parent:** [Ellipsoid](#ellipsoid)

The [John ellipsoid](#john-ellipsoid) of a convex body is its inscribed [ellipsoid](#ellipsoid) of largest volume. For the [unit ball](normed-vector-space.md#unit-ball) $K$ of a $d$-dimensional [normed vector space](normed-vector-space.md), change coordinates so that this [ellipsoid](#ellipsoid) is the [Euclidean unit ball](normed-vector-space.md#euclidean-unit-ball). The resulting coordinates are called [John position](#john-position). In these coordinates the [John contact decomposition](#john-contact-decomposition) implies $B_2^d\subseteq K\subseteq\sqrt d B_2^d$, or $\|x\|_E\leq |x|\leq\sqrt d\|x\|_E$.

#### John contact decomposition

↑ **Parent:** [John ellipsoid](#john-ellipsoid)

For a centrally symmetric convex body in [John position](#john-position), there are contact points $u_j\in\partial K\cap S^{d-1}$ and positive weights $c_j$ such that $\sum_jc_j u_j\otimes u_j=I$. Taking the [trace](linear-algebra.md#matrix-trace) gives $\sum_jc_j=d$. A supporting hyperplane at $u_j$ shows $|\langle u_j,x\rangle|\leq\|x\|_K$.

Here is the maximum-volume argument for the decomposition. If $I$ were outside the [convex cone](convex-set.md#convex-cone) generated by the contact matrices, a [separating hyperplane](statistical-learning.md#separating-hyperplane) would give a [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$ with $\operatorname{tr}A>0$ and $\langle Au,u\rangle\leq0$ at every contact. Subtract a small positive multiple of $I$ so these inequalities become strict while the [trace](linear-algebra.md#matrix-trace) remains positive. The [support function](convex-set.md#support-function) of $(I+tA)B_2^d$ is $|(I+tA)v|$. It decreases below $1$ near all contact directions for small positive $t$; away from them, the strict gap $h_K(v)>1$ preserves containment. Its volume increases, since $\det(I+tA)=1+t\operatorname{tr}A+O(t^2)$, a contradiction. The cone is closed because its generators have [trace](linear-algebra.md#matrix-trace) $1$ and form a [compact set](topology.md#compact-space); finite-dimensional [convexity](real-analysis.md#convex-function) gives a finite decomposition.

#### John position

↑ **Parent:** [John ellipsoid](#john-ellipsoid)

A centrally symmetric convex body is in [John position](#john-position) when its [John ellipsoid](#john-ellipsoid) is the [Euclidean unit ball](normed-vector-space.md#euclidean-unit-ball).

### Coordinate-projection atlas of an ellipsoid

↑ **Parent:** [Ellipsoid](#ellipsoid)

For nonzero real $a_i$, scale the ambient coordinates by $q_i=a_i r_i$. On the half where $\varepsilon q_i>0$, omitting $q_i$ is a [manifold chart](differential-geometry.md#manifold-chart) onto the [open unit ball](normed-vector-space.md#open-unit-ball); its inverse restores $q_i=\varepsilon\sqrt{1-\sum_{j\ne i}q_j^2}$. These $2(n+1)$ charts form a [smooth atlas](differential-geometry.md#smooth-atlas) of the [ellipsoid](#ellipsoid), including for negative $a_i$.

### Two-chart smooth atlas of an ellipsoid

↑ **Parent:** [Ellipsoid](#ellipsoid)

If $D=\operatorname{diag}(a_1,\ldots,a_{n+1})$ is invertible, $x\mapsto Dx$ sends the [ellipsoid](#ellipsoid) $\sum_i a_i^2x_i^2=1$ to the unit [sphere](#sphere). On $u=(v,s)\in S^n$, the two [stereographic projections](riemann-surfaces.md#stereographic-projection) $v/(1-s)$ and $v/(1+s)$ omit opposite poles and have inverses $(2w/(1+|w|^2),\pm(|w|^2-1)/(1+|w|^2))$, with the sign chosen for the appropriate pole. Their overlap transition is $w\mapsto w/|w|^2$, smooth and involutive on $\mathbb R^n\setminus\{0\}$. Composing their inverses with $D^{-1}$ gives a two-chart [smooth atlas](differential-geometry.md#smooth-atlas) of the ellipsoid. Its [subspace topology](topology.md#subspace-topology) is [Hausdorff](topology.md#hausdorff-space) and has a [second-countable space](topology.md#second-countable-space) topology, so it is a [smooth manifold](smooth-manifold.md). For $n=0$ the overlap is empty and each chart is a point.

### Spheroid

↑ **Parent:** [Ellipsoid](#ellipsoid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spheroid)

A [spheroid](#spheroid) is an [ellipsoid](#ellipsoid) of revolution obtained by rotating an [ellipse](#ellipse) about a principal axis. Rotation about the shorter axis gives an [oblate spheroid](galaxy.md#oblate-spheroid); rotation about the longer axis gives a [prolate spheroid](#prolate-spheroid). Thus the oblate form is a member of the general family.

#### Prolate spheroid

↑ **Parent:** [Spheroid](#spheroid)

A [prolate spheroid](#prolate-spheroid) is an [ellipsoid](#ellipsoid) with two equal shorter semiaxes and a longer symmetry-axis semiaxis. Its meridional section is an [ellipse](#ellipse) rotated about its major axis. In the coordinates $R^2/(\lambda+\alpha)+z^2/(\lambda+\beta)=1$ with $\beta>\alpha$, a fixed regular $\lambda$ has equatorial radius $\sqrt{\lambda+\alpha}$ and polar radius $\sqrt{\lambda+\beta}$; its focal separation is independent of $\lambda$, giving a confocal family.

##### Intersection of a prolate spheroid and a concentric sphere

↑ **Parent:** [Prolate spheroid](#prolate-spheroid)

For the [prolate spheroid](#prolate-spheroid) $u^2/a^2+(v^2+w^2)/b^2=1$ with $a>b>0$, intersect the concentric [sphere](#sphere) $u^2+v^2+w^2=R^2$. When $b<R<a$, subtraction gives two [circles](topology.md#circle) in the perpendicular planes

$$
u=\pm a\sqrt{\frac{R^2-b^2}{a^2-b^2}},\qquad v^2+w^2=\frac{b^2(a^2-R^2)}{a^2-b^2}.
$$

Their centers lie on the long principal axis and the line through the centers is normal to both planes. At $R=b$ the circles merge into the equator; at $R=a$ they shrink to the two polar vertices. There is no intersection for $R<b$ or $R>a$.

## Perpendicular bisector

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perpendicular_bisector)

The perpendicular bisector of a line segment is the line through its midpoint at a right angle to the segment.

### Circumcenter

↑ **Parent:** [Perpendicular bisector](#perpendicular-bisector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circumcenter)

The circumcenter of a nondegenerate triangle is the common intersection of its three [perpendicular bisectors](#perpendicular-bisector). It is equidistant from the three vertices and is the center of the triangle's circumcircle.

## Skew lines

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skew_lines)

Skew lines are two lines in three-dimensional Euclidean space that are neither parallel nor intersecting.

### Distance between skew lines

↑ **Parent:** [Skew lines](#skew-lines)

For lines $\mathbf a_1+\lambda\mathbf u_1$ and $\mathbf a_2+\mu\mathbf u_2$ with $\mathbf u_1\times\mathbf u_2\ne0$, their shortest distance is

$$
\frac{|(\mathbf a_2-\mathbf a_1)\mathbin\cdot(\mathbf u_1\times\mathbf u_2)|}{|\mathbf u_1\times\mathbf u_2|}.
$$

## Circles of Apollonius

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circles_of_Apollonius)

An Apollonius circle is the locus of points whose distances from two fixed points have a prescribed positive ratio different from one. Ratio one gives the perpendicular bisector.

## Right angle

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Right_angle)

A right angle is an angle of $\pi/2$ radians; two nonzero vectors meet at a right angle exactly when their inner product is zero.

## Rigid transformation

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rigid_transformation)

A rigid motion preserves Euclidean distances and therefore preserves angles, lengths, and curvatures.

### Point reflection

↑ **Parent:** [Rigid transformation](#rigid-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Point_reflection)

<h2 id="thales-s-theorem">Thales's theorem</h2>

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thales's_theorem)

An angle subtended by a diameter of a circle is right; conversely, the hypotenuse of a right triangle inscribed in a circle is a diameter.

## Regular polygon

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_polygon)

A regular polygon has equal side lengths and equal interior angles. Its vertices on a circle are scaled and rotated roots of unity.

### Area of a regular octagon

↑ **Parent:** [Regular polygon](#regular-polygon)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Area_of_a_regular_octagon)

A regular octagon of side length s has area 2(1+sqrt(2))s^2.

## Spherical cap

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spherical_cap)

A spherical cap is the part of a sphere cut off by a plane.

### Mass of a spherical cap with height-proportional density

↑ **Parent:** [Spherical cap](#spherical-cap)

For a solid [spherical cap](#spherical-cap) $r^2+z^2\leq R^2$, $z\geq c$, where $0\leq c\leq R$ and the [mass density](fluid-mechanics.md#density) is $\rho=kz$ with $k\geq0$, a [volume integral](multivariable-calculus.md#volume-integral) in [cylindrical coordinates](multivariable-calculus.md#cylindrical-coordinate-system) gives

$$
M=\pi k\int_c^Rz(R^2-z^2)\,dz=\frac{\pi k}{4}(R^2-c^2)^2.
$$

Here the height is measured from the centre of the [sphere](#sphere), rather than from the bottom of the cap. Specifying that origin matters for a nonuniform [mass density](fluid-mechanics.md#density).

### Curved area of a spherical cap

↑ **Parent:** [Spherical cap](#spherical-cap)

For a [sphere](#sphere) of [radius](topology.md#radius) $R>0$, the [spherical cap](#spherical-cap) above $z=R-h$, with $0\leq h\leq2R$, has curved [surface area](differential-geometry.md#surface-area) $2\pi Rh$. On the surface use $r(z)=\sqrt{R^2-z^2}$. The [surface of revolution](differential-geometry.md#surface-of-revolution) area element is $2\pi r\sqrt{1+(dr/dz)^2}\,dz=2\pi R\,dz$. Integrating from $R-h$ to $R$ proves the formula. It includes only the spherical surface; if the planar closing disk is required, add $\pi(2Rh-h^2)$. The coordinate expression is interpreted by a [limit](calculus.md#limit-of-a-function) at a pole.

### Volume of a spherical cap

↑ **Parent:** [Spherical cap](#spherical-cap)

For a solid [spherical cap](#spherical-cap) of height $0\leq h\leq2R$ cut from a [sphere](#sphere) of [radius](topology.md#radius) $R$,

$$
\boxed{V=\pi h^2\left(R-\frac h3\right).}
$$

Centre the [sphere](#sphere) at the origin with the cap on the side $z\geq R-h$. Its cross-section at height $z$ is a [circle](topology.md#circle) of squared [radius](topology.md#radius) $R^2-z^2$. A [volume integral](multivariable-calculus.md#volume-integral) in [cylindrical coordinates](multivariable-calculus.md#cylindrical-coordinate-system) gives

$$
V=\int_{R-h}^{R}\int_0^{2\pi}\int_0^{\sqrt{R^2-z^2}}r\,dr\,d\phi\,dz=\pi\int_{R-h}^{R}(R^2-z^2)\,dz=\pi h^2(R-h/3).
$$

The formula includes caps larger than a [hemisphere](#hemisphere), when $h>R$, and the whole solid [sphere](#sphere), when $h=2R$. For the retained region $z\geq-d$ with $0<d<R$, set $h=R+d$ to obtain $V=\pi(2R^3/3+R^2d-d^3/3)$. Multiplying by uniform [mass density](fluid-mechanics.md#density) gives its [mass](classical-mechanics.md#mass).

### Spherical cap area upper bound

↑ **Parent:** [Spherical cap](#spherical-cap)

On the [unit sphere](topology.md#unit-sphere) $S^{n-1}$, let $D_\rho$ be a [spherical cap](#spherical-cap) of angular radius $0<\rho<\pi/2$. If $\sin\rho\geq1/\sqrt n$, its [surface area](differential-geometry.md#surface-area) is at most $s_{n-1}\sin^n\rho$. This includes $\rho\geq\pi/4$ for every $n\geq2$. The bound follows by comparing the cap-area derivative with the derivative of $\sin^n\rho$ and checking the two endpoint values.

## Lattice polygon

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lattice_polygon)

A lattice polygon has all vertices in the integer lattice; triangulation shows that its area is a half-integer.

## Isoperimetric inequality

↑ **Parent:** [Euclidean geometry](euclidean-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isoperimetric_inequality)

The [isoperimetric inequality](#isoperimetric-inequality) bounds enclosed volume in terms of boundary size. In the plane it gives $4\pi A\leq L^2$, with equality for disks; higher-dimensional forms bound the boundary area of a region of prescribed volume.

### Planar isoperimetric inequality

↑ **Parent:** [Isoperimetric inequality](#isoperimetric-inequality)

This is the planar case of the [isoperimetric inequality](#isoperimetric-inequality). Every bounded planar domain with a sufficiently regular boundary of length $L$ and area $A$ satisfies

$$
4\pi A\leq L^2.
$$

Equality holds exactly for circular domains.

#### Maximum-area circular segment with fixed arc length and chord

↑ **Parent:** [Planar isoperimetric inequality](#planar-isoperimetric-inequality)

Fix two attachments a distance $2a$ apart on a straight line and a simple fence of length $2l$ in one half-plane, with $a<l<\pi a/2$. There is a unique $\theta\in(0,\pi/2)$ satisfying $l/a=\theta/\sin\theta$: its derivative has numerator $\sin\theta-\theta\cos\theta>0$, since that numerator starts at zero and has derivative $\theta\sin\theta>0$. A radius-$R$ minor circular arc with half-angle $\theta$ then has the required chord and length. Its graph is $y=\sqrt{R^2-x^2}-\sqrt{R^2-a^2}$, for $-a\leq x\leq a$, and sector-minus-triangle geometry gives the displayed area.

To prove global maximality, attach the complementary major arc of this circle, lying in the opposite half-plane, to any competing fence. The resulting closed curve has perimeter $2l+(2\pi R-2l)=2\pi R$. Its enclosed area is the competitor's area plus a fixed major-segment area. The [planar isoperimetric inequality](#planar-isoperimetric-inequality) bounds the total by $\pi R^2$, with equality only for a circle. Subtracting that fixed added area proves the minor arc is the unique maximizing shape on the chosen side. The same arc follows from the [Beltrami identity](analysis.md#beltrami-identity) for the area-minus-length functional.

#### Hurwitz proof of the planar isoperimetric inequality

↑ **Parent:** [Planar isoperimetric inequality](#planar-isoperimetric-inequality)

Parametrize a positively oriented closed [plane curve](algebraic-geometry.md#plane-curve) at constant [arc length](riemannian-geometry.md#arc-length) speed on $[0,2\pi]$, and let $c_n$ be its complex-position [Fourier coefficients](fourier-series.md#fourier-coefficient). [Green's theorem](multivariable-calculus.md#green-theorem) and [Parseval's identity](fourier-analysis.md#parseval-identity) give $A=\pi\sum_n n|c_n|^2$ and $L^2/(4\pi^2)=\sum_n n^2|c_n|^2$. Since $n\leq n^2$ for integers, the [planar isoperimetric inequality](#planar-isoperimetric-inequality) follows. Equality leaves only the constant and positive first harmonic, a translated circle.

#### Circle equality in the planar isoperimetric inequality

↑ **Parent:** [Planar isoperimetric inequality](#planar-isoperimetric-inequality)

Equality in the Cauchy-Schwarz and periodic Wirtinger bounds makes the arclength boundary parametrization a first harmonic with orthogonal equal-length coefficient vectors. The boundary is therefore a circle, and the enclosed domain is a disc.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (21)

- [Algebraic number theory](algebraic-number-theory.md)
- [Borsuk-Ulam theorem](algebraic-topology.md#borsuk-ulam-theorem)
- [Complex number](complex-analysis.md#complex-number)
- [Differential geometry](differential-geometry.md)
- [Euclidean geometry](euclidean-geometry.md)
- [Fermat number](number-theory.md#fermat-number)
- [Geometry and topology](geometry-and-topology.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2.md#14f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2020/paper-1.md#1/a/i/solution)
- [Point-mass gravitational lens](gravitational-lensing.md#point-mass-gravitational-lens)
- [Pythagorean theorem](#pythagorean-theorem)
- [Rotation (mathematics)](riemannian-geometry.md#rotation-mathematics)
- [Rotational invariance of the Laplacian](multivariable-calculus.md#rotational-invariance-of-the-laplacian)
- [Spherical geometry](geometry-and-topology.md#spherical-geometry)
- [Triangle group](group.md#triangle-group)
- [Trigonometric function](geometry-and-topology.md#trigonometric-function)
- [Unit disk](#unit-disk)
- [Vacuum conservation of specific intensity](radiometry.md#vacuum-conservation-of-specific-intensity)
