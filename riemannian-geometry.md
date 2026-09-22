# Riemannian geometry

↑ **Parent:** [Differential geometry](differential-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemannian_geometry)

Riemannian geometry studies smooth manifolds equipped with smoothly varying inner products on tangent spaces.

**Table of contents**

- [Minimal submanifold](#minimal-submanifold)
- [Ricci soliton](#ricci-soliton)
  - [Steady gradient Ricci soliton scalar identity](#steady-gradient-ricci-soliton-scalar-identity)
- [Riemannian Hessian](#riemannian-hessian)
- [Spectral geometry](#spectral-geometry)
  - [Wave trace](#wave-trace)
    - [Duistermaat-Guillemin trace formula](#duistermaat-guillemin-trace-formula)
  - [Weyl law](#weyl-law)
  - [Spectral zeta function](#spectral-zeta-function)
    - [Zero-mode correction to the spectral zeta value](#zero-mode-correction-to-the-spectral-zeta-value)
  - [Heat trace](#heat-trace)
    - [Euler characteristic from the heat trace of a bordered surface](#euler-characteristic-from-the-heat-trace-of-a-bordered-surface)
  - [Spectrum of the Laplacian on a sphere](#spectrum-of-the-laplacian-on-a-sphere)
    - [Ambient restriction formula for the spherical Laplacian](#ambient-restriction-formula-for-the-spherical-laplacian)
  - [Isospectral manifolds](#isospectral-manifolds)
    - [Compact isospectral sets of closed surfaces](#compact-isospectral-sets-of-closed-surfaces)
    - [Tetra and Didi](#tetra-and-didi)
    - [Finiteness of isospectral hyperbolic surfaces](#finiteness-of-isospectral-hyperbolic-surfaces)
    - [Sunada theorem](#sunada-theorem)
      - [Sunada orbital heat-trace formula](#sunada-orbital-heat-trace-formula)
      - [Sunada unitary equivalence without a finite heat trace](#sunada-unitary-equivalence-without-a-finite-heat-trace)
      - [Intersection test for nonisometric finite covers](#intersection-test-for-nonisometric-finite-covers)
        - [Generic isolation of lifted simple geodesics](#generic-isolation-of-lifted-simple-geodesics)
        - [Cycle intersections count intersections of lifted curves](#cycle-intersections-count-intersections-of-lifted-curves)
      - [Cone-torus construction of genus-four Sunada surfaces](#cone-torus-construction-of-genus-four-sunada-surfaces)
        - [Lambert quadrilateral construction of a cone torus](#lambert-quadrilateral-construction-of-a-cone-torus)
      - [Triangle cover construction for Sunada surfaces](#triangle-cover-construction-for-sunada-surfaces)
        - [Reflection intertwining of triangle-cover coset actions](#reflection-intertwining-of-triangle-cover-coset-actions)
      - [Curvature markers distinguishing finite-cover quotients](#curvature-markers-distinguishing-finite-cover-quotients)
      - [Area separation of convergent Sunada families](#area-separation-of-convergent-sunada-families)
      - [Binary family of nonhomeomorphic Sunada quotients](#binary-family-of-nonhomeomorphic-sunada-quotients)
    - [Transplantation theorem](#transplantation-theorem)
      - [Orthogonalization of a transplantation matrix](#orthogonalization-of-a-transplantation-matrix)
      - [Seven-triangle Dirichlet transplantation](#seven-triangle-dirichlet-transplantation)
      - [Four-tile mixed-boundary transplantation between a disk and a nonorientable surface](#four-tile-mixed-boundary-transplantation-between-a-disk-and-a-nonorientable-surface)
      - [Eight-tile Neumann transplantation across orientability](#eight-tile-neumann-transplantation-across-orientability)
      - [Pure Neumann reflection transplantation preserves Euler characteristic](#pure-neumann-reflection-transplantation-preserves-euler-characteristic)
      - [Transplantation by reflection parity](#transplantation-by-reflection-parity)
      - [Propeller domains](#propeller-domains)
    - [Spectral rigidity](#spectral-rigidity)
      - [Wolpert generic spectral rigidity theorem](#wolpert-generic-spectral-rigidity-theorem)
- [Riemannian manifold](#riemannian-manifold)
  - [Cartan-Ambrose-Hicks theorem](#cartan-ambrose-hicks-theorem)
  - [Classification of complete positive constant-curvature manifolds](#classification-of-complete-positive-constant-curvature-manifolds)
  - [Locally symmetric Riemannian manifold](#locally-symmetric-riemannian-manifold)
    - [Jacobi fields in a locally symmetric Riemannian manifold](#jacobi-fields-in-a-locally-symmetric-riemannian-manifold)
  - [Boundary normal coordinates](#boundary-normal-coordinates)
  - [Simple Riemannian manifold](#simple-riemannian-manifold)
    - [Geodesic scattering relation](#geodesic-scattering-relation)
      - [Boundary distance determines geodesic scattering](#boundary-distance-determines-geodesic-scattering)
    - [Boundary distance function](#boundary-distance-function)
  - [Homogeneous Riemannian manifold](#homogeneous-riemannian-manifold)
    - [Two-point homogeneous Riemannian manifold](#two-point-homogeneous-riemannian-manifold)
      - [Unit tangent transitivity characterizes two-point homogeneity](#unit-tangent-transitivity-characterizes-two-point-homogeneity)
    - [Completeness of homogeneous Riemannian manifolds](#completeness-of-homogeneous-riemannian-manifolds)
  - [Conical singularity](#conical-singularity)
  - [Killing-Yano tensor](#killing-yano-tensor)
    - [Killing-Yano two-form](#killing-yano-two-form)
      - [Square of a Killing-Yano two-form](#square-of-a-killing-yano-two-form)
  - [Killing tensor](#killing-tensor)
    - [Rank-two Killing tensor](#rank-two-killing-tensor)
      - [Quadratic geodesic first integral](#quadratic-geodesic-first-integral)
  - [Spin manifold](#spin-manifold)
    - [Spinor bundle](#spinor-bundle)
    - [Spin structure](#spin-structure)
      - [Spin-c structure](#spin-c-structure)
    - [Spinor field](#spinor-field)
      - [Dirac operator](#dirac-operator)
        - [Chiral phase of the round-sphere Dirac operator](#chiral-phase-of-the-round-sphere-dirac-operator)
          - [Degree-one compression of a chiral sphere phase](#degree-one-compression-of-a-chiral-sphere-phase)
        - [Atiyah-Singer index theorem](#atiyah-singer-index-theorem)
          - [Getzler rescaling](#getzler-rescaling)
        - [Twisted Dirac operator](#twisted-dirac-operator)
          - [Lichnerowicz formula for a twisted Dirac operator](#lichnerowicz-formula-for-a-twisted-dirac-operator)
        - [Equivariant index theorem](#equivariant-index-theorem)
  - [Induced metric](#induced-metric)
- [Riemannian surface](#riemannian-surface)
- [Arc length](#arc-length)
  - [Length of a curve](#length-of-a-curve)
  - [Riemannian distance](#riemannian-distance)
    - [Riemannian distance induces the manifold topology](#riemannian-distance-induces-the-manifold-topology)
    - [Distance splitting through a small geodesic sphere](#distance-splitting-through-a-small-geodesic-sphere)
    - [Minimizing geodesic](#minimizing-geodesic)
      - [A minimizing broken geodesic has no corner](#a-minimizing-broken-geodesic-has-no-corner)
      - [Cut locus](#cut-locus)
        - [Riemannian cut point](#riemannian-cut-point)
          - [Cut and conjugate times in round real projective space](#cut-and-conjugate-times-in-round-real-projective-space)
          - [Cut-point dichotomy for complete Riemannian manifolds](#cut-point-dichotomy-for-complete-riemannian-manifolds)
- [Riemannian product](#riemannian-product)
  - [Product Laplacian eigenspace decomposition](#product-laplacian-eigenspace-decomposition)
    - [Isospectral stabilization by a small flat torus](#isospectral-stabilization-by-a-small-flat-torus)
- [Isometry](#isometry)
  - [Isometry group](#isometry-group)
    - [Finite orientation-preserving plane isometry groups are cyclic](#finite-orientation-preserving-plane-isometry-groups-are-cyclic)
    - [Isometry dimensions in dimension three](#isometry-dimensions-in-dimension-three)
    - [Isometry group of a Riemannian quotient](#isometry-group-of-a-riemannian-quotient)
    - [Myers-Steenrod theorem](#myers-steenrod-theorem)
    - [Fixed point of a finite Euclidean isometry group](#fixed-point-of-a-finite-euclidean-isometry-group)
  - [Fixed-point set](#fixed-point-set)
  - [Euclidean isometry](#euclidean-isometry)
    - [Rigidity of a scalene triangle](#rigidity-of-a-scalene-triangle)
    - [Rotation (mathematics)](#rotation-mathematics)
    - [Translation subgroup](#translation-subgroup)
      - [Translation lattice](#translation-lattice)
    - [Frieze group](#frieze-group)
    - [Glide reflection](#glide-reflection)
    - [Finite reflection decomposition of a Euclidean isometry](#finite-reflection-decomposition-of-a-euclidean-isometry)
      - [Reflection length of a Euclidean orthogonal map](#reflection-length-of-a-euclidean-orthogonal-map)
  - [Isometric embedding](#isometric-embedding)
    - [Isometric extension](#isometric-extension)
- [Geodesic](#geodesic)
  - [Conjugate points](#conjugate-points)
  - [Local extension of geodesic velocity](#local-extension-of-geodesic-velocity)
  - [Liouville metric geodesic integral](#liouville-metric-geodesic-integral)
  - [Spacelike geodesic](#spacelike-geodesic)
  - [Closed geodesic](#closed-geodesic)
    - [Primitive closed geodesic](#primitive-closed-geodesic)
  - [Uniqueness of a closed geodesic on a negatively curved cylinder](#uniqueness-of-a-closed-geodesic-on-a-negatively-curved-cylinder)
  - [Pregeodesic](#pregeodesic)
    - [Null pregeodesic](#null-pregeodesic)
  - [Geodesic convexity](#geodesic-convexity)
  - [Geodesic segment](#geodesic-segment)
  - [Distance minimizers on a punctured sphere](#distance-minimizers-on-a-punctured-sphere)
  - [Geodesic variation](#geodesic-variation)
    - [Deviation vector](#deviation-vector)
    - [Realization of Jacobi fields by geodesic variations](#realization-of-jacobi-fields-by-geodesic-variations)
  - [Geodesic triangle](#geodesic-triangle)
  - [Surface covariant derivative](#surface-covariant-derivative)
    - [Surface tangent projector](#surface-tangent-projector)
      - [Sphere surface derivative identities](#sphere-surface-derivative-identities)
    - [Surface gradient](#surface-gradient)
    - [Surface divergence](#surface-divergence)
      - [Surface divergence theorem for a tangent field](#surface-divergence-theorem-for-a-tangent-field)
  - [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)
    - [Differential of the exponential map at zero](#differential-of-the-exponential-map-at-zero)
    - [Convex normal neighbourhood](#convex-normal-neighbourhood)
    - [Geodesic flow](#geodesic-flow)
      - [Geodesic hyperbolicity from negative Gaussian curvature](#geodesic-hyperbolicity-from-negative-gaussian-curvature)
      - [Generalized thermostat on a Riemannian surface](#generalized-thermostat-on-a-riemannian-surface)
        - [Linearized transverse equation for a surface thermostat](#linearized-transverse-equation-for-a-surface-thermostat)
        - [Gaussian thermostat](#gaussian-thermostat)
          - [Divergence of a Gaussian thermostat](#divergence-of-a-gaussian-thermostat)
      - [Magnetic flow on a Riemannian surface](#magnetic-flow-on-a-riemannian-surface)
        - [Contact rigidity of a zero-flux Anosov magnetic flow](#contact-rigidity-of-a-zero-flux-anosov-magnetic-flow)
      - [Geodesic Hamiltonian](#geodesic-hamiltonian)
    - [Domain of the exponential map](#domain-of-the-exponential-map)
      - [Exponential map of the punctured plane](#exponential-map-of-the-punctured-plane)
    - [Normal neighbourhood](#normal-neighbourhood)
      - [Radial distance in a normal neighbourhood](#radial-distance-in-a-normal-neighbourhood)
        - [Radial vector field in a normal neighbourhood](#radial-vector-field-in-a-normal-neighbourhood)
      - [Injectivity radius](#injectivity-radius)
      - [Geodesic normal coordinates](#geodesic-normal-coordinates)
        - [Christoffel symbols vanish at the center of normal coordinates](#christoffel-symbols-vanish-at-the-center-of-normal-coordinates)
        - [Geodesic sphere](#geodesic-sphere)
        - [Radial Christoffel-symbol criterion for geodesic coordinates](#radial-christoffel-symbol-criterion-for-geodesic-coordinates)
    - [Geodesic polar coordinates](#geodesic-polar-coordinates)
      - [Radial Riccati equation for distance spheres](#radial-riccati-equation-for-distance-spheres)
      - [Geodesic circle](#geodesic-circle)
        - [Close geodesic circles intersect twice](#close-geodesic-circles-intersect-twice)
      - [Gauss's lemma (Riemannian geometry)](#gauss-s-lemma-riemannian-geometry)
        - [Jacobi equation in geodesic polar coordinates](#jacobi-equation-in-geodesic-polar-coordinates)
          - [One-dimensional Rauch comparison inequality](#one-dimensional-rauch-comparison-inequality)
          - [Area of a geodesic polar ball with nonpositive curvature](#area-of-a-geodesic-polar-ball-with-nonpositive-curvature)
          - [Area of a small geodesic polar ball under an upper curvature bound](#area-of-a-small-geodesic-polar-ball-under-an-upper-curvature-bound)
  - [Complete geodesic](#complete-geodesic)
    - [Maximal geodesic](#maximal-geodesic)
      - [Extendible geodesic](#extendible-geodesic)
    - [Geodesic completeness](#geodesic-completeness)
      - [Upward stability of Riemannian completeness](#upward-stability-of-riemannian-completeness)
      - [Compact-core completeness for a Euclidean end](#compact-core-completeness-for-a-euclidean-end)
      - [Geodesic incompleteness](#geodesic-incompleteness)
        - [Curvature-blowup criterion for inextendibility of a surface](#curvature-blowup-criterion-for-inextendibility-of-a-surface)
          - [Incomplete surface z equals r to three halves](#incomplete-surface-z-equals-r-to-three-halves)
      - [Hopf-Rinow theorem](#hopf-rinow-theorem)
        - [Hopf-Rinow lemma](#hopf-rinow-lemma)
        - [Radial continuation proof of Hopf-Rinow](#radial-continuation-proof-of-hopf-rinow)
  - [Line in a Riemannian manifold](#line-in-a-riemannian-manifold)
    - [Disconnected at infinity](#disconnected-at-infinity)
      - [A line from disconnection at infinity](#a-line-from-disconnection-at-infinity)
  - [Tangency invariance of an ambient-surface geodesic](#tangency-invariance-of-an-ambient-surface-geodesic)
    - [Cylindrical-helix tangency construction](#cylindrical-helix-tangency-construction)
- [Energy of a curve](#energy-of-a-curve)
  - [Fixed-endpoint variation of a curve](#fixed-endpoint-variation-of-a-curve)
  - [First variation of geodesic energy](#first-variation-of-geodesic-energy)
  - [Variation vector field](#variation-vector-field)
    - [Riemannian index form](#riemannian-index-form)
      - [Riccati factorization of the Riemannian index form](#riccati-factorization-of-the-riemannian-index-form)
      - [Jacobi fields form the radical of the fixed-endpoint index form](#jacobi-fields-form-the-radical-of-the-fixed-endpoint-index-form)
      - [Conjugate-point criterion for the Riemannian index form](#conjugate-point-criterion-for-the-riemannian-index-form)
        - [Loss of geodesic minimality beyond a conjugate point](#loss-of-geodesic-minimality-beyond-a-conjugate-point)
      - [Sine index-form bound for positive Ricci curvature](#sine-index-form-bound-for-positive-ricci-curvature)
      - [Second variation of geodesic energy](#second-variation-of-geodesic-energy)
        - [Instability of a closed geodesic in positive even-dimensional curvature](#instability-of-a-closed-geodesic-in-positive-even-dimensional-curvature)
      - [Second variation of Riemannian arc length](#second-variation-of-riemannian-arc-length)
        - [Moving-endpoint second variation of Riemannian arc length](#moving-endpoint-second-variation-of-riemannian-arc-length)
- [Christoffel symbol](#christoffel-symbol)
  - [Christoffel trace identity](#christoffel-trace-identity)
  - [Christoffel symbols of a diagonal spherical spacetime metric](#christoffel-symbols-of-a-diagonal-spherical-spacetime-metric)
- [Geodesic equation](#geodesic-equation)
  - [Geodesic coordinate grid](#geodesic-coordinate-grid)
    - [Constant-angle geodesic coordinate grids are locally flat](#constant-angle-geodesic-coordinate-grids-are-locally-flat)
  - [Unparametrized geodesic equation](#unparametrized-geodesic-equation)
    - [Timelike length and energy have the same geodesic images](#timelike-length-and-energy-have-the-same-geodesic-images)
  - [Geodesic Lagrangian](#geodesic-lagrangian)
  - [Ambient acceleration criterion for a surface geodesic](#ambient-acceleration-criterion-for-a-surface-geodesic)
    - [Constant speed of an affinely parametrized geodesic](#constant-speed-of-an-affinely-parametrized-geodesic)
  - [Normal section of a surface](#normal-section-of-a-surface)
  - [Affine parameter](#affine-parameter)
- [Geodesic polygon](#geodesic-polygon)
- [Schur's lemma (Riemannian geometry)](#schur-s-lemma-riemannian-geometry)
- [Complete manifold](#complete-manifold)

## Minimal submanifold

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)

A minimal submanifold has vanishing [mean curvature](second-fundamental-form.md#mean-curvature) vector, equivalently zero first variation of volume for compactly supported normal variations. A [minimal surface](second-fundamental-form.md#minimal-surface) is its two-dimensional case. A [calibrated submanifold](differential-geometry.md#calibrated-submanifold) satisfies the stronger property of minimizing volume in its relative homology class.

// Target: general-relativity.bigb

## Ricci soliton

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ricci_soliton)

A [Riemannian metric](differential-geometry.md#riemannian-metric) satisfying the displayed equation for a [vector field](calculus.md#vector-field) $X$ and constant $\lambda$. A gradient Ricci soliton has $X=\nabla f$; it is steady when $\lambda=0$.

### Steady gradient Ricci soliton scalar identity

↑ **Parent:** [Ricci soliton](#ricci-soliton)

For $\operatorname{Ric}+\nabla^2 f=0$, the [contracted Bianchi identity](general-relativity.md#contracted-bianchi-identity) and the commutation identity $\Delta\nabla f=\nabla\Delta f+\operatorname{Ric}(\nabla f)$ imply $\nabla R=2\operatorname{Ric}(\nabla f)$. Meanwhile $\nabla|\nabla f|^2=-2\operatorname{Ric}(\nabla f)$, so their sum is constant on every [connected component](geometry-and-topology.md#connected-component).

## Riemannian Hessian

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)

The symmetric covariant two-tensor defined using the [Levi-Civita connection](general-relativity.md#levi-civita-connection) by $\operatorname{Hess}_g f(X,Y)=X(Yf)-(\nabla_XY)f$. Its negative [metric trace](linear-algebra.md#metric-trace) is the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) applied to $f$. Along a [geodesic](#geodesic) it gives the second derivative of $f$.

## Spectral geometry

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_geometry)

[Spectral geometry](#spectral-geometry) studies which properties of a [Riemannian manifold](#riemannian-manifold) can be recovered from the [spectrum](linear-operator-theory.md#spectrum-functional-analysis) of geometric [differential operators](analysis.md#differential-operator), especially the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator). Explicit [spherical harmonics](analysis.md#spherical-harmonic), [Fourier series](fourier-series.md) on a [flat torus](second-fundamental-form.md#flat-torus), and [isospectral manifolds](#isospectral-manifolds) illustrate three different aspects of the problem.

### Wave trace

↑ **Parent:** [Spectral geometry](#spectral-geometry)

For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) $P$ on a [closed manifold](differential-geometry.md#closed-manifold), the [wave trace](#wave-trace) is the [distribution](distribution-theory.md#distribution-mathematical-analysis) $\sum_j e^{it\sqrt{\lambda_j}}$, counting [multiplicities](polynomial.md#multiplicity-mathematics). The series is interpreted after testing against smooth compactly supported functions, rather than as an ordinarily convergent sum. Its singularities relate the spectrum to the [length spectrum](geometry-and-topology.md#length-spectrum) of [closed geodesics](#closed-geodesic), through the [Duistermaat-Guillemin trace formula](#duistermaat-guillemin-trace-formula).

#### Duistermaat-Guillemin trace formula

↑ **Parent:** [Wave trace](#wave-trace)

For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) on a [closed manifold](differential-geometry.md#closed-manifold), the singular support of the [wave trace](#wave-trace) lies in zero together with signed lengths of [closed geodesics](#closed-geodesic). Under the clean fixed-set hypotheses, its singularity at a periodic-geodesic length has an expansion determined by the [geodesic flow](#geodesic-flow) and its linearized return map. In particular, when the relevant leading coefficient does not vanish through cancellation, that length is determined by the spectrum. The inclusion of singular supports alone does not justify an unconditional recovery of every [geodesic](#geodesic) length.

### Weyl law

↑ **Parent:** [Spectral geometry](#spectral-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weyl_law)

For the positive scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) on a closed $d$-dimensional [Riemannian manifold](#riemannian-manifold), the number of [eigenvalues](linear-operator-theory.md#eigenvalue) at most $\lambda$, counted with multiplicity, has the displayed leading asymptotic. The exponent determines the dimension and the coefficient determines the total volume of the [Riemannian metric](differential-geometry.md#riemannian-metric). There is an analogous result with fixed [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) or [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) on a compact smooth domain.

### Spectral zeta function

↑ **Parent:** [Spectral geometry](#spectral-geometry)

For a nonnegative elliptic operator $L$ on a [closed manifold](differential-geometry.md#closed-manifold), sum its positive [eigenvalues](linear-operator-theory.md#eigenvalue) with multiplicity. The defining series converges in a right half-plane. If $n_0=\dim\ker L$ and $K(t)=\operatorname{Tr}(e^{-tL})$ is the [heat trace](#heat-trace), then

$$
\zeta_L(s)=\frac1{\Gamma(s)}\int_0^\infty t^{s-1}(K(t)-n_0)\,dt.
$$

Subtracting finitely many terms of the short-time [heat kernel expansion](diffusion-equation.md#heat-kernel-expansion) gives a [meromorphic continuation](complex-analysis.md#meromorphic-continuation). Zero eigenvalues must be excluded: assigning them a nonexistent inverse power does not define the spectral zeta function.

#### Zero-mode correction to the spectral zeta value

↑ **Parent:** [Spectral zeta function](#spectral-zeta-function)

For a Laplace-type operator on a [closed manifold](differential-geometry.md#closed-manifold), let $a_{t^0}$ be the constant coefficient of its full [heat trace](#heat-trace) expansion. In the [Mellin transform](analysis.md#mellin-transform) defining the [spectral zeta function](#spectral-zeta-function), the reduced trace has constant coefficient $a_{t^0}-\dim\ker L$. Its contribution is $(a_{t^0}-\dim\ker L)/s$, and $1/\Gamma(s)=s+O(s^2)$ proves the identity. For the scalar [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) on a closed surface, $a_{t^0}=\int R\,dV/(24\pi)$ and $\dim\ker L$ is the number of connected components. In particular, a connected sphere has value $-2/3$ and a connected flat torus has value $-1$.

### Heat trace

↑ **Parent:** [Spectral geometry](#spectral-geometry)

For the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) on a closed compact [Riemannian manifold](#riemannian-manifold), the [heat trace](#heat-trace) is $Z_M(t)=\sum_j e^{-t\lambda_j}=\int_M K_M(t,x,x)\,dV(x)$. It records every [eigenvalue](linear-operator-theory.md#eigenvalue) with multiplicity. In a finite free isometric quotient it equals $|U|^{-1}\sum_{u\in U}\int_NK_N(t,x,ux)\,dV(x)$. The orbital integrals form a [class function](representation-theory.md#class-function) of the ambient finite isometry group, so [Gassmann equivalence](representation-theory.md#gassmann-equivalence) gives equal quotient [heat traces](#heat-trace) and hence [Sunada theorem](#sunada-theorem).

#### Euler characteristic from the heat trace of a bordered surface

↑ **Parent:** [Heat trace](#heat-trace)

For a compact smooth [Riemannian surface](#riemannian-surface) with smooth boundary and a pure [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) or pure [Neumann boundary condition](differential-equation.md#neumann-boundary-condition), the constant coefficient in the [heat trace](#heat-trace) is

$$
\frac1{12\pi}\left(\int_MK\,dA+\int_{\partial M}\kappa\,ds\right)=\frac{\chi(M)}6.
$$

The equality is the [Gauss-Bonnet theorem](differential-geometry.md#gauss-bonnet-theorem). Thus such [isospectral manifolds](#isospectral-manifolds) have the same [Euler characteristic](homology.md#euler-characteristic). A [simply connected](algebraic-topology.md#simply-connected-space) compact connected bordered surface is a disk with $\chi=1$, whereas a nonorientable surface with $c\geq1$ crosscaps and $b\geq1$ boundary components has $\chi=2-c-b\leq0$. These cannot be isospectral in this setting. Corners and mixed [boundary conditions](differential-equation.md#boundary-condition) contribute additional heat coefficients, so the smooth pure-boundary-condition hypothesis is essential.

### Spectrum of the Laplacian on a sphere

↑ **Parent:** [Spectral geometry](#spectral-geometry)

For the unit $S^d$ and the nonnegative [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator), the [eigenvalues](linear-operator-theory.md#eigenvalue) are $\ell(\ell+d-1)$, with multiplicities $\binom{\ell+d}{d}-\binom{\ell+d-2}{d}$ for $\ell\geq0$. The [eigenfunctions](linear-operator-theory.md#eigenfunction) are restrictions of degree-$\ell$ [harmonic polynomials](partial-differential-equation.md#harmonic-polynomial). The [harmonic decomposition of homogeneous polynomials](partial-differential-equation.md#harmonic-decomposition-of-homogeneous-polynomials) and the [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) prove completeness.

#### Ambient restriction formula for the spherical Laplacian

↑ **Parent:** [Spectrum of the Laplacian on a sphere](#spectrum-of-the-laplacian-on-a-sphere)

For a smooth ambient function near the unit [sphere](geometry-and-topology.md#sphere), the [chain rule](calculus.md#chain-rule) along the [great circles](geometry-and-topology.md#great-circle) $\gamma_i(t)=p\cos t+e_i\sin t$ gives $(F\circ\gamma_i)''(0)=D^2F(e_i,e_i)-DF(p)$. Sum over an [orthonormal basis](linear-algebra.md#orthonormal-basis) of the [tangent space](differential-geometry.md#tangent-space) and supplement it by the radial vector $p$. The [geodesic trace formula for the Laplace-Beltrami operator](differential-geometry.md#geodesic-trace-formula-for-the-laplace-beltrami-operator) then gives the displayed formula, evaluated at radius one. In particular a degree-$\ell$ [harmonic polynomial](partial-differential-equation.md#harmonic-polynomial) restricts to a [spherical harmonic](analysis.md#spherical-harmonic) with positive [eigenvalue](linear-operator-theory.md#eigenvalue) $\ell(\ell+d-1)$.

### Isospectral manifolds

↑ **Parent:** [Spectral geometry](#spectral-geometry)

Two [Riemannian manifolds](#riemannian-manifold) are isospectral for a specified [differential operator](analysis.md#differential-operator) if their [eigenvalues](linear-operator-theory.md#eigenvalue), counted with multiplicities and with the same [boundary conditions](differential-equation.md#boundary-condition), agree. [Riemannian isometries](differential-geometry.md#riemannian-isometry) preserve the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) [spectrum](linear-operator-theory.md#spectrum-functional-analysis), but the converse can fail. The [transplantation theorem](#transplantation-theorem) and the [Sunada theorem](#sunada-theorem) give systematic constructions.

#### Compact isospectral sets of closed surfaces

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

For a fixed [closed](topology.md#closed-set) orientable [Riemannian surface](#riemannian-surface), the smooth metrics with a specified scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) spectrum form a [compact](topology.md#compact-space) set modulo [diffeomorphisms](geometry-and-topology.md#diffeomorphism), in the smooth topology. This is a [compactness](topology.md#compact-space) assertion, not uniqueness or finiteness of the number of [Riemannian isometry](differential-geometry.md#riemannian-isometry) classes. It restricts geometric degeneration within an isospectral set and uses more information than the leading [heat invariants](diffusion-equation.md#heat-invariants) alone. The theorem was established in [the 1988 compactness paper](https://doi.org/10.1016/0022-1236(88)90071-7).

#### Tetra and Didi

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

A pair of closed orientable flat three-manifolds with equal scalar [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) spectra but different first [Betti numbers](homology.md#betti-number), respectively one and zero. Consequently they are not [homeomorphic](topology.md#local-homeomorphism). They cannot be isospectral for the [Hodge Laplacian](differential-form.md#hodge-laplacian) on one-forms, whose zero-eigenvalue multiplicity is the first [Betti number](homology.md#betti-number). This shows why the spectrum on functions must not be silently replaced by the spectra on all differential forms.

#### Finiteness of isospectral hyperbolic surfaces

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

For a fixed closed [hyperbolic surface](geometry-and-topology.md#hyperbolic-surface), there are only finitely many [isometry](#isometry) classes with its [Laplacian](calculus.md#laplacian) spectrum. The [Selberg trace formula](geometry-and-topology.md#selberg-trace-formula) gives a common discrete [length spectrum](geometry-and-topology.md#length-spectrum) and common positive [hyperbolic systole](geometry-and-topology.md#hyperbolic-systole). [Mumford's compactness theorem](geometry-and-topology.md#mumford-s-compactness-theorem) confines this family to a compact subset of [moduli space](geometry-and-topology.md#moduli-space). If distinct members accumulated, choose nearby markings at an accumulation point and use [finite length coordinates for hyperbolic surfaces](geometry-and-topology.md#finite-length-coordinates-for-hyperbolic-surfaces). Each of these finitely many lengths converges while remaining in one discrete spectrum, so it is eventually constant. The length coordinates then force eventual equality, a contradiction. This finiteness theorem is weaker than the [Wolpert generic spectral rigidity theorem](#wolpert-generic-spectral-rigidity-theorem).

#### Sunada theorem

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

Suppose a finite [group](group.md) $G$ acts by [Riemannian isometries](differential-geometry.md#riemannian-isometry) on a compact [Riemannian manifold](#riemannian-manifold) $M$, and [Gassmann equivalent](representation-theory.md#gassmann-equivalence) subgroups $H_1,H_2$ act freely. The quotient manifolds $H_i\backslash M$ have equal [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) spectra. For an [eigenfunction](linear-operator-theory.md#eigenfunction) space $E$, the quotient multiplicity is $|H_i|^{-1}\sum_{h\in H_i}\operatorname{tr}(h|E)$, and the equality follows by summing its [character of a representation](representation-theory.md#character-of-a-representation) over [conjugacy classes](group-theory.md#conjugacy-class). Nonconjugacy inside $G$ alone does not guarantee that the quotients are nonisometric.

##### Sunada orbital heat-trace formula

↑ **Parent:** [Sunada theorem](#sunada-theorem)

For a finite [subgroup](group.md#subgroup) $U$ of a [group](group.md) $T$ of [Riemannian isometries](differential-geometry.md#riemannian-isometry) of a [closed manifold](differential-geometry.md#closed-manifold) $N$, assume $U$ acts freely and define $I_t(g)=\int_N H_N(t,x,gx)\,dV(x)$. Invariance of the [Riemannian heat kernel](diffusion-equation.md#riemannian-heat-kernel) and change of variables show that $I_t$ is a [class function](representation-theory.md#class-function) on $T$. For $U\le T$, the [heat kernel on a finite isometric quotient](diffusion-equation.md#heat-kernel-on-a-finite-isometric-quotient) and integration over a [fundamental domain](group-theory.md#fundamental-domain) give the displayed [heat trace](#heat-trace) formula. Grouping by [conjugacy classes](group-theory.md#conjugacy-class) proves equality for [Gassmann equivalent](representation-theory.md#gassmann-equivalence) [subgroups](group.md#subgroup). More generally the same argument allows fixed points of $T$ outside the freely acting [subgroups](group.md#subgroup); only the quotient under consideration must be smooth.

##### Sunada unitary equivalence without a finite heat trace

↑ **Parent:** [Sunada theorem](#sunada-theorem)

A finite isometry group decomposes $L^2(N)$ into its irreducible representation factors $V_\rho$ and multiplicity Hilbert spaces $\mathcal H_\rho$. The Laplacian commutes with the group, so it acts as the identity on each representation factor. The averaging projection gives $\dim V_\rho^{U_i}=|U_i|^{-1}\sum_{u\in U_i}\chi_\rho(u)$. For [Gassmann equivalent](representation-theory.md#gassmann-equivalence) subgroups these dimensions agree. Choosing unitary identifications of the invariant finite-dimensional factors therefore intertwines the quotient Laplacians, even when a noncompact covering manifold has no finite [heat trace](#heat-trace).

##### Intersection test for nonisometric finite covers

↑ **Parent:** [Sunada theorem](#sunada-theorem)

Let two finite locally isometric covers carry uniquely length-identified primitive closed [geodesics](#geodesic) $\alpha_i,\beta_i$. If their geometric intersection numbers differ, the covering surfaces are not [isometric](#isometry), because an [isometry](#isometry) preserves both lengths and intersections. For base simple curves intersecting once, lift components correspond to cycles of their [monodromy permutations](algebraic-topology.md#monodromy-permutation). Their intersection number is the number of sheets common to the two cycles. This distinguishes covers even when every individual permutation has the same cycle type in both actions, as in [Gassmann equivalence](representation-theory.md#gassmann-equivalence).

###### Generic isolation of lifted simple geodesics

↑ **Parent:** [Intersection test for nonisometric finite covers](#intersection-test-for-nonisometric-finite-covers)

In a finite hyperbolic covering, primitive lifts of a primitive closed [geodesic](#geodesic) correspond to cycles of its [monodromy permutation](algebraic-topology.md#monodromy-permutation); an $r$-cycle gives length $r\ell(\gamma)$. In a real-analytic family of compact [hyperbolic surfaces](geometry-and-topology.md#hyperbolic-surface) or hyperbolic cone orbifolds, a prescribed multiple of a simple curve's length can be isolated generically from unrelated lifted lengths. To exclude an identity of length functions, pinch the simple curve: only its peripheral powers can have length tending to zero, while intersecting curves are long by the [collar lemma](geometry-and-topology.md#collar-lemma). The countably many remaining length equalities have empty interior, so the [Baire category theorem](topological-analysis.md#baire-category-theorem) supplies a parameter avoiding them. Only finitely many closed geodesics lie below a fixed local length bound; thus the isolation persists in an open parameter neighbourhood. This makes cycle-intersection information an intrinsic obstruction to an [isometry](#isometry), rather than an invariant of a chosen covering map alone.

###### Cycle intersections count intersections of lifted curves

↑ **Parent:** [Intersection test for nonisometric finite covers](#intersection-test-for-nonisometric-finite-covers)

If two simple base [geodesics](#geodesic) meet once, their lift components correspond to the cycles $C,D$ of their [monodromy permutations](algebraic-topology.md#monodromy-permutation). A lifted crossing belongs to the sheet labels common to both cycles, giving the displayed geometric intersection count. When their relevant lifted lengths identify these components independently of the covering map, different multisets of intersection counts obstruct an [isometry](#isometry) between the covering surfaces.

##### Cone-torus construction of genus-four Sunada surfaces

↑ **Parent:** [Sunada theorem](#sunada-theorem)

Take a hyperbolic torus with a single cone point of angle $2\pi/7$. Its [orbifold fundamental group](geometry-and-topology.md#orbifold-fundamental-group) is $\langle a,d\mid[d,a]^7=1\rangle$. An epimorphism to $\mathrm{PSL}(3,2)$ whose commutator has exact order $7$ has torsion-free kernel. The point and line stabilizers have index $7$ and order $24$, hence avoid all nontrivial cone stabilizers. Their quotient covers are smooth surfaces with [Euler characteristic](homology.md#euler-characteristic) $7(-6/7)=-6$, so have [genus](topology.md#genus-of-a-surface) $4$. Their equal coset [permutation characters](representation-theory.md#permutation-character) give equal [heat traces](#heat-trace) by the [Sunada theorem](#sunada-theorem). Nonisometry still requires a geometric distinction, such as the [intersection test for nonisometric finite covers](#intersection-test-for-nonisometric-finite-covers).

###### Lambert quadrilateral construction of a cone torus

↑ **Parent:** [Cone-torus construction of genus-four Sunada surfaces](#cone-torus-construction-of-genus-four-sunada-surfaces)

A [Lambert quadrilateral](geometry-and-topology.md#lambert-quadrilateral) with acute angle $\pi/14$ and sides $x,y$ incident to the opposite right-angle vertex satisfies the displayed relation. Reflect four copies around that vertex to make a symmetric hyperbolic quadrilateral whose four corner angles are $\pi/14$. Identifying opposite sides yields a torus with one cone angle $2\pi/7$. The two central axis loops have lengths $2x,2y$ and meet once at right angles. Cutting along one loop gives a pair of pants with two equal geodesic boundaries and the cone point; reglue the boundaries with a [Fenchel–Nielsen twist](geometry-and-topology.md#fenchel-nielsen-twist) to obtain the two-parameter cone-torus family. Its seven-sheeted torsion-free covers have genus four.

##### Triangle cover construction for Sunada surfaces

↑ **Parent:** [Sunada theorem](#sunada-theorem)

Let a finite [group](group.md) $T$ be generated by elements of exact orders $p,q$ whose product has exact order $r$, with $p^{-1}+q^{-1}+r^{-1}<1$. The epimorphism from the [hyperbolic triangle group](geometric-group-theory.md#hyperbolic-triangle-group) sending its generators to these elements has torsion-free kernel. Its quotient of the [hyperbolic plane](geometry-and-topology.md#hyperbolic-plane) is a closed surface with a $T$ action. A subgroup acts freely precisely when it meets no conjugate of a nonidentity power of the three elliptic generators. Free [almost conjugate subgroups](representation-theory.md#gassmann-equivalence) give [isospectral manifolds](#isospectral-manifolds) by the [Sunada theorem](#sunada-theorem).

###### Reflection intertwining of triangle-cover coset actions

↑ **Parent:** [Triangle cover construction for Sunada surfaces](#triangle-cover-construction-for-sunada-surfaces)

Write triangle-group generators as products $a=s_1s_2$, $b=s_2s_3$ of adjacent side reflections. Conjugation by $s_2$ sends both to their inverses. A sheet relabelling satisfying the displayed two permutation identities therefore lifts this base reflection to an [orientation-reversing isometry](differential-geometry.md#orientation-reversing-riemannian-isometry) between the two hyperbolic covers. Thus nonconjugate subgroups in the orientation-preserving finite group can still give isometric covers.

##### Curvature markers distinguishing finite-cover quotients

↑ **Parent:** [Sunada theorem](#sunada-theorem)

For a finite isometric group action on a closed [Riemannian surface](#riemannian-surface), choose a disk in the free locus whose translates are disjoint. Modify the [Riemannian metric](differential-geometry.md#riemannian-metric) there, and identically on its translates, by small supported changes with three distinguished high [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) maxima. Give their heights distinct values occurring nowhere else, arrange them as a tight noncollinear cluster, and keep separate clusters far apart. Such markers can be made by local conformal bump functions controlling curvature and its derivatives. Every quotient [isometry](#isometry) must send an entire labelled cluster to another. After identifying the marked disks with the original one, an [isometry](#isometry) fixes its three noncollinear points and is therefore the identity locally. If $p_i:M\to U_i\backslash M$ are free finite quotients, any quotient [isometry](#isometry) $F$ consequently makes $F\circ p_1=p_2\circ t$ on an open disk for some element $t$ of the original group. Two local isometries agreeing on an open set agree on the connected surface, by propagation along geodesics. The equality therefore holds globally and implies $tU_1t^{-1}\subseteq U_2$, hence equality for equal subgroup orders. Nonconjugate equal-order subgroups thus have nonisometric quotients for this marked invariant metric; constant curvature is not required.

##### Area separation of convergent Sunada families

↑ **Parent:** [Sunada theorem](#sunada-theorem)

Suppose a fixed pair of [Gassmann equivalent](representation-theory.md#gassmann-equivalence) finite covers of a compact two-dimensional orbifold has isometric limiting hyperbolic metrics. Choose nearby orbifold-smooth [nowhere locally homogeneous metrics](differential-geometry.md#nowhere-locally-homogeneous-metric) and rescale them to the displayed distinct areas. Scaling by a positive constant multiplies area by that constant in dimension two, preserves local rigidity, and preserves convergence when the constants tend to one. [Sunada theorem](#sunada-theorem) supplies equal spectra within each pair. Local rigidity forces any quotient isometry to descend to the identity on the base; nonconjugate covering subgroups therefore exclude within-pair isometry. Distinct areas exclude all cross-pair isometries and spectra, because the leading [heat trace](#heat-trace) coefficient is area divided by $4\pi t$. Fixed markings of the two isometric limiting covers give convergence to the same metric. The existence of those isometric limits is an additional geometric input, not a consequence of [Gassmann equivalence](representation-theory.md#gassmann-equivalence) alone.

##### Binary family of nonhomeomorphic Sunada quotients

↑ **Parent:** [Sunada theorem](#sunada-theorem)

Choose distinct odd primes and take products of the [nonisomorphic Gassmann equivalent regular subgroups](representation-theory.md#nonisomorphic-gassmann-equivalent-regular-subgroups), selecting one of the two groups at each prime. Product conjugacy-class counts give $2^n$ [Gassmann equivalent](representation-theory.md#gassmann-equivalence) [subgroups](group.md#subgroup) of the same finite product of symmetric groups. Their [fundamental groups](algebraic-topology.md#fundamental-group) are distinguished by whether the unique Sylow [subgroup](group.md#subgroup) at each chosen prime is abelian. The [closed-manifold realization of a finitely presented fundamental group](algebraic-topology.md#closed-manifold-realization-of-a-finitely-presented-fundamental-group) and [Sunada theorem](#sunada-theorem) therefore produce $2^n$ pairwise nonhomeomorphic, and hence nonisometric, isospectral closed four-manifolds. Gassmann equivalence alone, without a topology distinction, does not imply nonhomeomorphism.

#### Transplantation theorem

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

For two assemblies of congruent Euclidean tiles, let $M_s,N_s$ encode the gluing or boundary reflection at each labelled face. An invertible constant matrix $C$ satisfying $CM_s=N_sC$ carries tile restrictions of [Laplacian eigenfunctions](partial-differential-equation.md#laplacian-eigenfunction) bijectively to those on the second assembly. Boundary values satisfy $M_su=u$ and outward [normal derivatives](differential-geometry.md#normal-derivative) satisfy $M_sv=-v$, so the intertwining identities preserve matching and [boundary conditions](differential-equation.md#boundary-condition). Use diagonal $-1$ for a [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) and $+1$ for a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition).

##### Orthogonalization of a transplantation matrix

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Suppose an invertible real matrix $C$ intertwines symmetric orthogonal tile-reflection matrices: $CM_s=N_sC$. Then $C^TC$ commutes with every $M_s$, so its positive inverse square root does too. The [polar decomposition of an invertible real matrix](linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix) therefore gives an orthogonal matrix $O=C(C^TC)^{-1/2}$ satisfying $OM_s=N_sO$. On a disjoint union of congruent tiles, $O$ preserves both the $L^2$ [inner product](linear-algebra.md#inner-product) and [Dirichlet energy](differential-geometry.md#dirichlet-energy). The intertwining identities preserve the face trace conditions defining the assembled [Sobolev space](sobolev-space.md), so $O$ gives a [unitary equivalence](vector-space.md#unitary-equivalence) of the assembled [Laplacians](calculus.md#laplacian).

##### Seven-triangle Dirichlet transplantation

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Take seven copies of a scalene [triangle](geometry-and-topology.md#triangle), with sides labelled $a,b,c$ opposite its three vertices, and reflect adjacent copies across their glued side. For the first [planar domain](geometry-and-topology.md#planar-domain), the glued pairs are $a:(2,3),(6,7)$, $b:(4,6),(5,7)$, $c:(1,5),(3,7)$; for the second they are $a:(1,3),(5,7)$, $b:(2,6),(3,7)$, $c:(4,5),(6,7)$. Both coloured trees have central tile $7$. For triangles sufficiently close to equilateral the interiors do not overlap. If its three angles are distinct and between $\pi/4$ and $\pi/2$, the only reentrant vertices are the original central vertices, with angles four times the corresponding triangle angles. They force any proposed [isometry](#isometry) to preserve the labelled central triangle, which is incompatible with the different attachments on its arms.

For the spectral proof index the nonzero vectors and covectors of $\mathbb F_2^3$ by $1,\ldots,7$, using binary coordinates. The [Fano plane](projective-space.md#fano-plane) incidence matrix is $B_{y,x}=\mathbf1_{y\cdot x=0}$. It satisfies $B^TB=2I+J$, so is invertible, and intertwines the point and line permutations of each of the three elementary transvections. Put $D=\operatorname{diag}(1,1,-1,1,-1,-1,1)$. The signed reflection matrices for the [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) are $-DP_sD$ and $-DQ_sD$, hence $C=DBD$ intertwines them. Its polar orthogonal factor gives a [unitary equivalence](vector-space.md#unitary-equivalence) of the [Dirichlet Laplacians](partial-differential-equation.md#dirichlet-laplacian), preserving both the $L^2$ [inner product](linear-algebra.md#inner-product) and the Dirichlet energy of the piecewise functions. This produces a three-parameter family of noncongruent isospectral [planar domains](geometry-and-topology.md#planar-domain).

##### Four-tile mixed-boundary transplantation between a disk and a nonorientable surface

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Take four congruent octagonal [regular polygons](geometry-and-topology.md#regular-polygon) with four alternate sides labelled $a,b,c,d$. The intervening sides have [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). Pair equal face parameters in the positive reference boundary direction. The complete gluing data are

$$
\begin{array}{c|c|c|c|c}
\text{face}&\text{pairs in }D&\text{Dirichlet tiles in }D&\text{pairs in }B&\text{Dirichlet tiles in }B\\ \hline
a&23&\varnothing&13&\varnothing\\
b&12&\varnothing&12&\varnothing\\
c&01&\{2,3\}&02&\{1,3\}\\
d&\varnothing&\{1,3\}&01,\ 23&\varnothing
\end{array}
$$

All unpaired labelled faces not in a Dirichlet column also have [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). Encode these rules by [signed permutation matrices](vector-space.md#signed-permutation-matrix), using a positive swap for a paired interface and diagonal $-1$ or $+1$ for an unpaired [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) or [Neumann boundary condition](differential-equation.md#neumann-boundary-condition). The four-by-four [Hadamard matrix](vector-space.md#hadamard-matrix) $C$ above satisfies $CM_s=N_sC$ for every label. Explicitly, if its columns are $h_0,h_1,h_2,h_3$, applying $N_a,N_b,N_c,N_d$ gives respectively $(h_0,h_1,h_3,h_2)$, $(h_0,h_2,h_1,h_3)$, $(h_1,h_0,-h_2,-h_3)$, and $(h_0,-h_1,h_2,-h_3)$, which are exactly the columns of the corresponding $CM_s$. On every intervening face the face matrix is the identity.

Since $C^TC=4I$, the [orthogonal matrix](linear-algebra.md#orthogonal-matrix) $C/2$ preserves the $L^2$ [inner product](linear-algebra.md#inner-product) and the sum of Dirichlet energies. Its intertwining relations map matching [Sobolev traces](sobolev-space.md#trace-operator) and zero Dirichlet traces bijectively to those of the other assembly. It therefore preserves the [quadratic form](linear-algebra.md#quadratic-form) domains and the forms themselves. The associated [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator) are unitarily equivalent, proving equality of all [eigenvalues](linear-operator-theory.md#eigenvalue) with their [multiplicities](polynomial.md#multiplicity-mathematics) for the specified [mixed boundary conditions](differential-equation.md#mixed-boundary-condition).

The [topology of disk tiles glued along disjoint boundary arcs](topology.md#topology-of-disk-tiles-glued-along-disjoint-boundary-arcs) shows that $D$, whose gluing [graph](graph.md) is $0,1,2,3$ in a path, is a [closed disc](topology.md#closed-disc) and is [simply connected](algebraic-topology.md#simply-connected-space) and [orientable](differential-geometry.md#orientable-surface). The gluing [graph](graph.md) of $B$ has edges $13,12,02,01,23$; it is connected with two independent cycles, so $\chi(B)=-1$ and $\pi_1(B)\cong F_2$. Its odd cycle $1,2,3,1$ makes it a [nonorientable surface](topology.md#non-orientable-surface). Each assembled surface has nonempty polygonal boundary. This explicitly realizes isospectrality between a simply-connected orientable bordered surface and a nonorientable, non-simply-connected one. The boundary corners and [mixed boundary conditions](differential-equation.md#mixed-boundary-condition) are essential qualifications; it does not contradict the [Euler characteristic from the heat trace of a bordered surface](#euler-characteristic-from-the-heat-trace-of-a-bordered-surface) for smooth boundaries and pure boundary conditions.

##### Eight-tile Neumann transplantation across orientability

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Take eight congruent hexagonal tiles with three pairwise nonadjacent distinguished faces. On tile indices modulo eight let $\sigma(j)=1-j$, $t(j)=-j$, and use $u_1(j)=3j$ for one assembly and $u_2(j)=3j+4$ for the other. Pair faces by reflection and leave fixed faces, and the three remaining faces, with [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). If $Re_j=e_{j+1}$, the displayed matrix intertwines all three face actions: its circulant coefficients satisfy $c_r=c_{-r}=c_{3r+4}$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are $1+(-1)^k+4\cos(\pi k/4)$, which are nonzero for $0\leq k\leq7$. The [transplantation theorem](#transplantation-theorem) gives equal spectra. The second gluing graph is [bipartite](graph-theory.md#bipartite-graph), with parts $\{0,5,6,7\}$ and $\{1,2,3,4\}$, so it is [orientable](differential-geometry.md#orientable-surface). The first has the odd cycle $1,3,6,2,7,1$ and is nonorientable. Both graphs are connected with eight vertices and ten edges, and their bordered surfaces retract up to homotopy to the graphs. Both have [Euler characteristic](homology.md#euler-characteristic) $-2$ and [fundamental groups](algebraic-topology.md#fundamental-group) free of rank three. Neither is [simply connected](algebraic-topology.md#simply-connected-space).

##### Pure Neumann reflection transplantation preserves Euler characteristic

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Consider assemblies of congruent polygonal tiles with same-labelled faces paired by reflection and pure [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) on unpaired faces. An invertible intertwiner for all face [permutation matrices](vector-space.md#permutation-matrix) preserves the [Euler characteristic](homology.md#euler-characteristic). The number of tiles is the dimension of the representation. For each face label the number of edge classes is $(n+\operatorname{tr}M_s)/2$. For each vertex label the number of vertex classes is the number of orbits of the subgroup generated by incident-face involutions, hence the dimension of its invariant vectors. Intertwining preserves all these numbers. Summing the vertex and edge counts proves equal $V-E+F$, including boundary corners. This argument uses genuine permutation matrices; signed matrices encoding mixed [boundary conditions](differential-equation.md#boundary-condition) do not give the same topological count.

##### Transplantation by reflection parity

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

Reflection across a cut splits [Laplacian eigenfunctions](partial-differential-equation.md#laplacian-eigenfunction) into odd and even parts. The odd restriction has a [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) on the cut; the even restriction has a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) there. The displayed matrix intertwines the two-tile swap with $\operatorname{diag}(-1,1)$. A connected uniform-Dirichlet rectangle of width $2a$ is therefore isospectral to the disjoint union of width-$a$ rectangles with all-Dirichlet and three-Dirichlet/one-Neumann conditions. This illustrates why changing boundary conditions can conceal connectedness in the [spectrum](linear-operator-theory.md#spectrum-functional-analysis).

##### Propeller domains

↑ **Parent:** [Transplantation theorem](#transplantation-theorem)

A propeller domain consists of seven congruent reflected triangles: one central triangle and three arms of two triangles each. There are different coloured gluing patterns whose [Dirichlet Laplacian](partial-differential-equation.md#dirichlet-laplacian) and [Neumann Laplacian](partial-differential-equation.md#neumann-laplacian) spectra agree by the [transplantation theorem](#transplantation-theorem). Varying the three side lengths of a scalene triangle in a suitable open region gives three parameters; the central triangle is identifiable from the three reflex corners, allowing a direct nonisometry proof.

#### Spectral rigidity

↑ **Parent:** [Isospectral manifolds](#isospectral-manifolds)

A class of metrics is spectrally rigid if equality of their specified [spectra](linear-operator-theory.md#spectrum-functional-analysis) forces the metrics to be isometric, or, in a deformation version, if continuous isospectral deformations are trivial. The [spectrum of a flat torus](second-fundamental-form.md#spectrum-of-a-flat-torus) determines every two-dimensional [flat torus](second-fundamental-form.md#flat-torus) up to [isometry](#isometry). The [Wolpert generic spectral rigidity theorem](#wolpert-generic-spectral-rigidity-theorem) is a generic, rather than universal, uniqueness statement.

##### Wolpert generic spectral rigidity theorem

↑ **Parent:** [Spectral rigidity](#spectral-rigidity)

For closed [hyperbolic surfaces](geometry-and-topology.md#hyperbolic-surface) of genus $g\geq2$, there is a closed proper real-analytic exceptional subset of [Teichmüller space](complex-analysis.md#teichmuller-space) such that a surface outside it is determined up to [isometry](#isometry) by its unmarked [length spectrum](geometry-and-topology.md#length-spectrum), equivalently its [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) [spectrum](linear-operator-theory.md#spectrum-functional-analysis). The analytic part of the proof controls possible spectral matchings using finite determining length data; the geometric part recognizes persistent matchings as changes of marking, using the [collar lemma](geometry-and-topology.md#collar-lemma) and variations of [Fenchel–Nielsen coordinates](geometry-and-topology.md#fenchel-nielsen-coordinates). Orientation reversal remains invisible to the spectrum.

## Riemannian manifold

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemannian_manifold)

A Riemannian manifold is a smooth manifold equipped with a smoothly varying positive-definite inner product on each tangent space.

### Cartan-Ambrose-Hicks theorem

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartan–Ambrose–Hicks_theorem)

A linear [isometry](#isometry) between tangent spaces of complete simply connected [Riemannian manifolds](#riemannian-manifold) extends to a global [isometry](#isometry) when parallel transport along corresponding broken [geodesics](#geodesic) identifies their [Riemann curvature tensors](general-relativity.md#riemann-curvature-tensor). In particular, complete simply connected manifolds of the same dimension and constant [sectional curvature](second-fundamental-form.md#sectional-curvature) are isometric: their curvature tensors are determined by that common constant and their [Riemannian metrics](differential-geometry.md#riemannian-metric). This is the constant-curvature form often called Cartan's theorem.

### Classification of complete positive constant-curvature manifolds

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

For a connected complete [Riemannian manifold](#riemannian-manifold) of dimension $n\geq2$ and constant [sectional curvature](second-fundamental-form.md#sectional-curvature) $k>0$, its complete simply connected [universal cover](algebraic-topology.md#universal-cover) is the round [sphere](geometry-and-topology.md#sphere) of radius $k^{-1/2}$. This is the constant-curvature case of [Cartan-Ambrose-Hicks theorem](#cartan-ambrose-hicks-theorem). Thus the manifold is a quotient by a finite group of [isometries](#isometry) acting freely. In even dimension, the determinant embeds this group in $\{1,-1\}$: every determinant-one orthogonal transformation in odd ambient dimension has eigenvalue one and therefore a fixed point. The only possible nonidentity element is the antipodal involution, giving [Real projective space](algebraic-topology.md#real-projective-space). In odd dimensions, free cyclic scalar actions on complex unit spheres instead produce [lens spaces](knot-theory.md#lens-space).

### Locally symmetric Riemannian manifold

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

A [Riemannian manifold](#riemannian-manifold) is locally symmetric when its [Riemann curvature tensor](general-relativity.md#riemann-curvature-tensor) is parallel for the [Levi-Civita connection](general-relativity.md#levi-civita-connection). Along a [geodesic](#geodesic), [parallel transport](fiber-bundle.md#parallel-transport) then conjugates the [Jacobi curvature operator](general-relativity.md#jacobi-curvature-operator) at the initial point to the operator at every later point. Thus its [eigenvalues](linear-operator-theory.md#eigenvalue) stay constant. The condition is local and does not assert that global point reflections extend to isometries of the whole manifold.

#### Jacobi fields in a locally symmetric Riemannian manifold

↑ **Parent:** [Locally symmetric Riemannian manifold](#locally-symmetric-riemannian-manifold)

Diagonalize the self-adjoint [Jacobi curvature operator](general-relativity.md#jacobi-curvature-operator) at the initial point and transport its orthonormal eigenbasis parallel along the [geodesic](#geodesic). The [Jacobi field](general-relativity.md#jacobi-field) equation reduces to $j_i''+\lambda_i j_i=0$. For zero initial position and initial derivative $b_i$, the solution is $b_i\sin(\sqrt{\lambda_i}t)/\sqrt{\lambda_i}$ when $\lambda_i>0$, $b_it$ when $\lambda_i=0$, and $b_i\sinh(\sqrt{-\lambda_i}t)/\sqrt{-\lambda_i}$ when $\lambda_i<0$. Only positive eigenvalues contribute [conjugate points](#conjugate-points), at $t=k\pi/\sqrt{\lambda_i}$. At a common zero the multiplicity is the sum of the contributing eigenspace dimensions. The displayed convention uses the curvature operator positive on a positively curved plane; reversing the tensor convention also reverses its tensor formula.

### Boundary normal coordinates

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

The map $(x,r)\mapsto\exp_x(r\nu_{\mathrm{in}})$ gives a collar in which the metric has this form. Two metrics with the same induced boundary metric can be identified by their normal collars, fixing the boundary and matching full tangent-space metrics there. To extend the local identification globally, interpolate the metrics, form their smoothly varying collars, and extend the resulting collar isotopy velocity by a cutoff. The time-dependent vector field vanishes on the boundary and agrees with that velocity near it, so its global flow gives the desired boundary-fixing diffeomorphism.

### Simple Riemannian manifold

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

A compact manifold with boundary is simple when the boundary is strictly convex and any two points are joined by a unique geodesic depending smoothly on the endpoints, without conjugate points. Geodesics exit in finite time. These properties make off-diagonal boundary distance derivatives and the [geodesic scattering relation](#geodesic-scattering-relation) well behaved.

#### Geodesic scattering relation

↑ **Parent:** [Simple Riemannian manifold](#simple-riemannian-manifold)

For an inward unit boundary vector, the geodesic scattering relation returns the next boundary point and its outgoing unit velocity. On outward vectors it can be extended using the first backward exit, giving an involution on the full boundary unit bundle, with tangential vectors fixed. Exit time is separate lens data; on a simple manifold it equals boundary distance between the endpoint pair.

##### Boundary distance determines geodesic scattering

↑ **Parent:** [Geodesic scattering relation](#geodesic-scattering-relation)

With the full boundary metric fixed, first variation gives $d_xd_g(w)=-\langle v_{\rm in},w\rangle$ and $d_yd_g(z)=\langle v_{\rm out},z\rangle$ for tangential endpoint variations. These covectors recover the tangential parts of both unit velocities. Their normal components follow from unit length and the inward/outward sign, so equal boundary distances give equal scattering relations. Without a fixed boundary metric, the bundle identification must first be gauged by a boundary-fixing diffeomorphism.

#### Boundary distance function

↑ **Parent:** [Simple Riemannian manifold](#simple-riemannian-manifold)

The boundary distance is the intrinsic distance between boundary points. Its infinitesimal limit along boundary curves recovers the induced metric on the boundary tangent bundle. It does not directly fix the normal and mixed metric components, which can be changed by boundary-fixing diffeomorphisms.

### Homogeneous Riemannian manifold

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

A [Riemannian manifold](#riemannian-manifold) is homogeneous when its [isometry](#isometry) group acts transitively on points. For example, a [Lie group](lie-theory.md#lie-group) with a [left-invariant metric](lie-theory.md#left-invariant-metric) is homogeneous under left translations. Homogeneity gives the same local metric-ball geometry at every point, which yields the [completeness of homogeneous Riemannian manifolds](#completeness-of-homogeneous-riemannian-manifolds). It does not imply two-point homogeneity: that stronger property also controls directions and pairs at equal distance.

#### Two-point homogeneous Riemannian manifold

↑ **Parent:** [Homogeneous Riemannian manifold](#homogeneous-riemannian-manifold)

A connected [Riemannian manifold](#riemannian-manifold) is two-point homogeneous if its [isometry](#isometry) group is transitive on ordered pairs at each fixed [Riemannian distance](#riemannian-distance). The equal-distance condition is necessary because [isometries](#isometry) preserve distance. Round spheres and Euclidean spaces are examples. The [unit tangent transitivity characterizes two-point homogeneity](#unit-tangent-transitivity-characterizes-two-point-homogeneity) lemma shows that this pair condition is equivalent to transitivity on the [unit tangent bundle](fiber-bundle.md#unit-tangent-bundle).

##### Unit tangent transitivity characterizes two-point homogeneity

↑ **Parent:** [Two-point homogeneous Riemannian manifold](#two-point-homogeneous-riemannian-manifold)

For a connected [Riemannian manifold](#riemannian-manifold), two-point homogeneity is equivalent to the [isometry](#isometry) group being transitive on the [unit tangent bundle](fiber-bundle.md#unit-tangent-bundle). One direction follows by taking short equal-length radial [geodesic](#geodesic) segments: the [Gauss lemma](#gauss-s-lemma-riemannian-geometry) identifies their distance, and injectivity of the [exponential map](#exponential-map-riemannian-geometry) identifies the initial directions after the endpoints are matched. Conversely, unit tangent transitivity implies point homogeneity, hence completeness. The [Hopf-Rinow theorem](#hopf-rinow-theorem) supplies minimizing [geodesics](#geodesic) for arbitrary equal-distance pairs. Matching their initial unit tangent vectors and using uniqueness of the [geodesic equation](#geodesic-equation) matches their other endpoints.

#### Completeness of homogeneous Riemannian manifolds

↑ **Parent:** [Homogeneous Riemannian manifold](#homogeneous-riemannian-manifold)

In a [homogeneous Riemannian manifold](#homogeneous-riemannian-manifold), choose $r>0$ so that one closed metric ball $\overline B(o,r)$ is compact. Such a ball exists from local compactness and the metric topology. Every radius-$r$ ball is isometric to it. A [Cauchy sequence](real-analysis.md#cauchy-sequence) eventually lies in one such compact ball, has a convergent subsequence, and therefore converges. This proves metric completeness; the [Hopf-Rinow theorem](#hopf-rinow-theorem) gives [geodesic completeness](#geodesic-completeness) and minimizing [geodesics](#geodesic) between points.

### Conical singularity

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

A conical singularity is a failure of smoothness at the apex of a metric cone. If $\vartheta$ has period $P$, small circles have circumference-to-radius ratio $aP$. The two-dimensional apex is smooth precisely when this equals $2\pi$. [Euclidean black-hole regularity condition](general-relativity.md#euclidean-black-hole-regularity-condition) applies this test to the imaginary-time and radial plane.

### Killing-Yano tensor

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)

A Killing-Yano tensor is a [differential form](differential-form.md) satisfying the displayed equation for the [Levi-Civita connection](general-relativity.md#levi-civita-connection). Its [covariant derivative](general-relativity.md#covariant-derivative) is totally antisymmetric. Contraction with the velocity of an affinely parametrized [geodesic](#geodesic) gives a form that is carried by [parallel transport](fiber-bundle.md#parallel-transport) along that [geodesic](#geodesic). This differs from a [Killing tensor](#killing-tensor), which is symmetric.

#### Killing-Yano two-form

↑ **Parent:** [Killing-Yano tensor](#killing-yano-tensor)

For a Killing-Yano two-form, $\nabla_aY_{bc}$ is a [differential three-form](differential-form.md#differential-three-form). Along a [geodesic](#geodesic) with velocity $v$, the covector $w_c=Y_{bc}v^b$ is carried by [parallel transport](fiber-bundle.md#parallel-transport), since $v^av^b\nabla_aY_{bc}=0$.

##### Square of a Killing-Yano two-form

↑ **Parent:** [Killing-Yano two-form](#killing-yano-two-form)

The square is a [rank-two Killing tensor](#rank-two-killing-tensor). It is symmetric because it pairs the covectors $Y_{a\cdot}$ and $Y_{b\cdot}$ using the metric. Along every affinely parametrized [geodesic](#geodesic), its contraction $K(v,v)$ is the squared norm of the carried by [parallel transport](fiber-bundle.md#parallel-transport) covector $Y(v,\cdot)$. [Metric compatibility](fiber-bundle.md#metric-compatibility) makes that norm constant, proving the [Killing tensor](#killing-tensor) equation. On a [Riemannian manifold](#riemannian-manifold) this tensor is positive semidefinite.

### Killing tensor

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Killing_tensor)

A Killing tensor is a symmetric covariant tensor satisfying the displayed equation for the [Levi-Civita connection](general-relativity.md#levi-civita-connection). Its contraction with $r$ copies of a [geodesic](#geodesic) velocity is constant along every affinely parametrized [geodesic](#geodesic). The converse follows because the resulting symmetric derivative is determined by its homogeneous polynomial on tangent vectors. Rank one recovers the [Killing vector field](general-relativity.md#killing-vector-field) after metric duality.

#### Rank-two Killing tensor

↑ **Parent:** [Killing tensor](#killing-tensor)

A symmetric two-tensor satisfying this equation gives a [quadratic geodesic first integral](#quadratic-geodesic-first-integral). Examples include the [Riemannian metric](differential-geometry.md#riemannian-metric), symmetric products of metric-dual [Killing vector fields](general-relativity.md#killing-vector-field), and the [square of a Killing-Yano two-form](#square-of-a-killing-yano-two-form).

##### Quadratic geodesic first integral

↑ **Parent:** [Rank-two Killing tensor](#rank-two-killing-tensor)

A quadratic [homogeneous polynomial](algebra.md#homogeneous-polynomial) in the fibre variables of the [cotangent bundle](symplectic-geometry.md#cotangent-bundle) is a first integral of the [geodesic Hamiltonian](#geodesic-hamiltonian) exactly when its symmetric lowered coefficients form a [rank-two Killing tensor](#rank-two-killing-tensor). For $v=g^{-1}p$, the [Poisson bracket](classical-mechanics.md#poisson-bracket) is $\{K,H\}=\nabla_{(a}K_{bc)}v^av^bv^c$, so the equivalence follows by comparing cubic coefficients at every point.

### Spin manifold

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_manifold)

A spin manifold is an oriented Riemannian manifold whose orthonormal frame bundle lifts from $SO(n)$ to its double cover $\operatorname{Spin}(n)$. Such a lift defines a spinor bundle.

#### Spinor bundle

↑ **Parent:** [Spin manifold](#spin-manifold)

A chosen [spin structure](#spin-structure) on a [spin manifold](#spin-manifold) defines the complex spinor bundle associated to the spin representation. In dimension $2m$ its [vector bundle rank](fiber-bundle.md#rank-of-a-vector-bundle) is $2^m$. Its [chirality matrix](algebra.md#chirality-matrix) is $\Gamma=i^mc(e^1)\cdots c(e^{2m})$ in the negative [Clifford multiplication](algebra.md#clifford-multiplication) convention. It satisfies $\Gamma^2=1$ and anticommutes with each $c(e^i)$, giving $S=S^+\oplus S^-$ and an odd [Dirac operator](#dirac-operator). In odd dimension there is no such canonical chiral splitting of the irreducible spinor bundle.

#### Spin structure

↑ **Parent:** [Spin manifold](#spin-manifold)

A spin structure is a consistent choice of lifting oriented orthonormal frame changes to their spin double cover, permitting globally defined [spinor fields](#spinor-field). For a spatial circle in a [worldsheet](string-theory.md#worldsheet), the two choices give periodic and antiperiodic fermions, hence the [Ramond sector](string-theory.md#ramond-sector) and [Neveu–Schwarz sector](string-theory.md#neveu-schwarz-sector). Local field equations do not choose the global spin structure.

##### Spin-c structure

↑ **Parent:** [Spin structure](#spin-structure)

A Spin-c structure on an oriented rank-$n$ real [vector bundle](fiber-bundle.md#vector-bundle) is a lift of its oriented frame bundle to $\operatorname{Spin}^c(n)=(\operatorname{Spin}(n)\times U(1))/\{(1,1),(-1,-1)\}$. Its [determinant line bundle](fiber-bundle.md#determinant-line-bundle) is associated with $[s,z]\mapsto z^2$; its [First Chern class](complex-geometry.md#first-chern-class) reduces modulo two to the second [Stiefel–Whitney class](fiber-bundle.md#stiefel-whitney-class). When such structures exist, their isomorphism classes form an affine space over $H^2$; tensoring by a complex line bundle of first Chern class $h$ changes the determinant class by $2h$. On a closed oriented three-manifold they always exist. On a four-manifold, the determinant class is characteristic: $\langle c_1(\mathfrak s),v\rangle\equiv v\cdot v\pmod2$.

#### Spinor field

↑ **Parent:** [Spin manifold](#spin-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spinor_field)

A spinor field is a section of a spinor bundle. Clifford multiplication by tangent vectors acts fiberwise on spinor fields.

##### Dirac operator

↑ **Parent:** [Spinor field](#spinor-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_operator)

The Dirac operator is the first-order elliptic operator obtained by composing the spin connection with Clifford multiplication. On an even-dimensional compact spin manifold it exchanges positive and negative chirality spinors.

###### Chiral phase of the round-sphere Dirac operator

↑ **Parent:** [Dirac operator](#dirac-operator)

For the oriented round unit two-sphere, positive and negative [spinor bundles](#spinor-bundle) have degrees $-1,+1$. Its [Dirac operator](#dirac-operator) has $D^2=C+1/4$ on their homogeneous sections, where $C$ is the angular-momentum [Casimir operator](semisimple-lie-algebra.md#casimir-element); the [eigenvalues](linear-operator-theory.md#eigenvalue) of $D$ are the nonzero integers. Therefore the chiral phase is a unitary between the two L2 chiral spaces, commuting with $SU(2)$. For a smooth function $f$, $[D,f]=c(df)$ is bounded. The sign-operator resolvent integral expresses its phase commutator as a norm-convergent integral of compact resolvent products bounded by a constant times $(1+t^2)^{-1}$. Thus it intertwines multiplication by every continuous function modulo compacts. Its full graded phase is self-adjoint; the chiral phase is the component relevant to nonzero compressed indices.

###### Degree-one compression of a chiral sphere phase

↑ **Parent:** [Chiral phase of the round-sphere Dirac operator](#chiral-phase-of-the-round-sphere-dirac-operator)

Let $P$ project onto a degree-one equivariant line bundle on the complex-oriented round two-sphere, and let $V$ be its positive-to-negative chiral [Dirac operator](#dirac-operator) phase. The compressed map has parametrix $PV^*P$ modulo compacts. Its domain bundle has degree zero and its target degree two. Their [homogeneous line-bundle representations on the two-sphere](ringed-space.md#homogeneous-line-bundle-representations-on-the-two-sphere) are respectively $E_0\oplus E_2\oplus E_4\oplus\cdots$ and $E_2\oplus E_4\oplus\cdots$, so the [equivariant Fredholm index](functional-analysis.md#equivariant-fredholm-index) is the trivial representation and the ordinary index is one. Reversing chirality negates the index. Compressing the full self-adjoint phase instead gives ordinary index zero.

###### Atiyah-Singer index theorem

↑ **Parent:** [Dirac operator](#dirac-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Atiyah–Singer_index_theorem)

For a [Twisted Dirac operator](#twisted-dirac-operator) on a closed even-dimensional [spin manifold](#spin-manifold), the theorem identifies its analytic [Fredholm index](functional-analysis.md#fredholm-index) with the integral of the top-degree part of the [A-hat form](geometry-and-topology.md#a-hat-form) times the [Chern character](algebraic-topology.md#chern-character). This is one geometric specialization of the general theorem for [elliptic differential operators](distribution-theory.md#elliptic-differential-operator), which expresses the analytic index in terms of the topological class of the [principal symbol](partial-differential-equation.md#principal-symbol-of-a-partial-differential-equation). The heat proof pairs all positive [eigenvalues](linear-operator-theory.md#eigenvalue) by the odd [Dirac operator](#dirac-operator), leaving only the index in the [supertrace](quantum-mechanics.md#supertrace); [Getzler rescaling](#getzler-rescaling) computes its local limit from curvature.

###### Getzler rescaling

↑ **Parent:** [Atiyah-Singer index theorem](#atiyah-singer-index-theorem)

Getzler rescaling combines the change $x\mapsto\sqrt t\,x$ in [geodesic normal coordinates](#geodesic-normal-coordinates) with the [Clifford algebra](algebra.md#clifford-algebra) filtration, assigning degree one to a derivative and to a Clifford generator and degree minus one to a coordinate. The associated graded [Clifford algebra](algebra.md#clifford-algebra) is the [exterior algebra](linear-algebra.md#exterior-algebra). This is useful because the spinor [supertrace](quantum-mechanics.md#supertrace) annihilates every Clifford monomial except the top-degree one. Applied to the [Lichnerowicz formula for a twisted Dirac operator](#lichnerowicz-formula-for-a-twisted-dirac-operator), it retains a quadratic curvature model, whose [heat kernel](diffusion-equation.md#heat-kernel) is computed by a Gaussian ansatz; all terms of smaller rescaling degree disappear from the local index limit. Thus the cancellations in a supersymmetric heat trace can be computed before solving the complete curved heat equation.

###### Twisted Dirac operator

↑ **Parent:** [Dirac operator](#dirac-operator)

On a [spin manifold](#spin-manifold), tensor the [spinor bundle](#spinor-bundle) $S$ with a [Hermitian vector bundle](fiber-bundle.md#hermitian-vector-bundle) $W$ carrying a [unitary connection](fiber-bundle.md#unitary-connection). Composing the induced tensor-product [connection on a vector bundle](fiber-bundle.md#connection-vector-bundle) with [Clifford multiplication](algebra.md#clifford-multiplication) defines the twisted Dirac operator. In even dimension it maps $S^+\otimes W$ to $S^-\otimes W$ and conversely. On a [closed manifold](differential-geometry.md#closed-manifold) its chiral restriction $D_W^+:H^1(S^+\otimes W)\to L^2(S^-\otimes W)$ is a [Fredholm operator](functional-analysis.md#fredholm-operator).

###### Lichnerowicz formula for a twisted Dirac operator

↑ **Parent:** [Twisted Dirac operator](#twisted-dirac-operator)

At the centre of [geodesic normal coordinates](#geodesic-normal-coordinates), expand the square of the [Twisted Dirac operator](#twisted-dirac-operator). The diagonal terms give the [rough Laplacian](fiber-bundle.md#rough-laplacian); the off-diagonal terms are $\sum_{i<j}c(e^i)c(e^j)[\nabla_i,\nabla_j]$. The tensor-product [vector-bundle curvature](fiber-bundle.md#curvature-form) is the sum of spin curvature and $F^W$. Substituting spin curvature $\frac14\sum_{a,b}\langle R(e_i,e_j)e_a,e_b\rangle c(e^a)c(e^b)$ and using the [Clifford algebra](algebra.md#clifford-algebra) relations yields the scalar term $\operatorname{Scal}/4$: the four-generator contribution vanishes by the algebraic [Bianchi identity](fiber-bundle.md#bianchi-identity) and the contracted terms are the [scalar curvature](second-fundamental-form.md#scalar-curvature). This proves the displayed identity at every point.

###### Equivariant index theorem

↑ **Parent:** [Dirac operator](#dirac-operator)

An equivariant index theorem expresses the supertrace of a symmetry on the kernel and cokernel of an elliptic operator as an integral of local characteristic data over the symmetry's fixed-point set.

### Induced metric

↑ **Parent:** [Riemannian manifold](#riemannian-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Induced_metric)

An immersion into a Riemannian manifold inherits a metric by taking ambient inner products of tangent vectors. For a parametrized curve $\mathbf r(u)$ in Euclidean space, the induced metric coefficient is $g=\partial_u\mathbf r\cdot\partial_u\mathbf r$.

## Riemannian surface

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemannian_surface)

A Riemannian surface is a two-dimensional smooth manifold equipped with a smoothly varying inner product on each tangent plane.

## Arc length

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arc_length)

The arc length of a regular curve $\gamma:[a,b]\to M$ is

$$
L(\gamma)=\int_a^b|\dot\gamma(t)|\,dt.
$$

### Length of a curve

↑ **Parent:** [Arc length](#arc-length)

For a piecewise smooth [curve](topology.md#curve), $L(\alpha)=\int\|\alpha^{\prime}(t)\|dt$ in an ambient Euclidean space, or the corresponding [Riemannian metric](differential-geometry.md#riemannian-metric) norm on a manifold. This is invariant under regular monotone reparametrization.

### Riemannian distance

↑ **Parent:** [Arc length](#arc-length)

The distance induced by a connected Riemannian manifold is the infimum of the lengths of piecewise smooth curves joining two points:

$$
d_g(p,q)=\inf_{\gamma:p\leadsto q}L_g(\gamma).
$$

#### Riemannian distance induces the manifold topology

↑ **Parent:** [Riemannian distance](#riemannian-distance)

In a relatively [compact](topology.md#compact-space) coordinate ball the [Riemannian metric](differential-geometry.md#riemannian-metric) norm is bounded above and below by positive multiples of the Euclidean norm. A coordinate segment gives the upper distance bound. A path leaving the ball has a positive lower length bound before its first exit; paths staying in it have the Euclidean displacement lower bound. Consequently distinct points have positive [Riemannian distance](#riemannian-distance), and the resulting [metric topology](topological-analysis.md#metric-topology) equals the manifold topology. Connectedness makes the distance finite because [smooth manifolds](differential-geometry.md#smooth-manifold) are locally path [connected](geometry-and-topology.md#connected-space).

#### Distance splitting through a small geodesic sphere

↑ **Parent:** [Riemannian distance](#riemannian-distance)

In a connected [Riemannian manifold](#riemannian-manifold), choose a small compact [geodesic sphere](#geodesic-sphere) around $p$ with $0<r<d(p,q)$. Minimize $d(\cdot,q)$ on this sphere. Every path from $p$ to $q$ crosses it, so an almost-minimizing path has length at least $r+\min_{S_r(p)}d(\cdot,q)$. The [triangle inequality](topological-analysis.md#triangle-inequality) gives the reverse bound, yielding the displayed equality. No global completeness is needed.

#### Minimizing geodesic

↑ **Parent:** [Riemannian distance](#riemannian-distance)

A minimizing geodesic realizes the Riemannian distance between its endpoints. A geodesic segment is locally minimizing, but need not remain globally minimizing beyond a cut point.

##### A minimizing broken geodesic has no corner

↑ **Parent:** [Minimizing geodesic](#minimizing-geodesic)

At an interior junction of two unit-speed [geodesic](#geodesic) segments, let $u$ be the incoming and $v$ the outgoing tangent. Choose points close to the junction in a common [convex normal neighbourhood](#convex-normal-neighbourhood). Moving the junction with velocity $z$ changes the sum of the two segment lengths by $\langle u-v,z\rangle$, using the [first variation of geodesic energy](#first-variation-of-geodesic-energy) or the [Gauss lemma](#gauss-s-lemma-riemannian-geometry). If $u\ne v$, choose $z=v-u$ to reduce length. Hence a length-minimizing broken [geodesic](#geodesic) has matching tangents and is one smooth [geodesic](#geodesic).

// Target: riemannian-geometry.bigb

##### Cut locus

↑ **Parent:** [Minimizing geodesic](#minimizing-geodesic)

On a complete connected [Riemannian manifold](#riemannian-manifold), let $c(v)$ for a unit tangent vector $v$ be the supremum of times for which $t\mapsto\exp_p(tv)$ minimizes [Riemannian distance](#riemannian-distance) from $p$. The cut locus consists of the endpoints $\exp_p(c(v)v)$ with $c(v)<\infty$. Radial minimization fails beyond this first cut time; distance spheres can cease to be smooth there.

###### Riemannian cut point

↑ **Parent:** [Cut locus](#cut-locus)

For a unit-speed [geodesic](#geodesic) $\gamma(t)=\exp_p(tv)$, a finite cut time $c(v)$ is the last time to which its segment from $p$ minimizes [Riemannian distance](#riemannian-distance). Its endpoint is the Riemannian cut point along that geodesic. It lies in the [cut locus](#cut-locus); it need not be a [cut point](geometry-and-topology.md#cut-point) in the topological sense. The segment up to the cut time still minimizes by continuity of distance.

###### Cut and conjugate times in round real projective space

↑ **Parent:** [Riemannian cut point](#riemannian-cut-point)

In unit-curvature [Real projective space](algebraic-topology.md#real-projective-space) of dimension at least two, [Riemannian distance](#riemannian-distance) is $d([v],[u])=\arccos|\langle v,u\rangle|$ for unit lifts. A unit-speed [geodesic](#geodesic) has lift $\cos t\,v+\sin t\,w$, with $w$ unit and perpendicular to $v$, and therefore ceases to minimize after $\pi/2$. Its normal [Jacobi fields](general-relativity.md#jacobi-field) with zero initial value are $\sin t$ times [parallel vector fields along a curve](fiber-bundle.md#parallel-vector-field-along-a-curve), giving first [conjugate point](calculus-of-variations.md#conjugate-point) at time $\pi$. The two times differ in every direction.

###### Cut-point dichotomy for complete Riemannian manifolds

↑ **Parent:** [Riemannian cut point](#riemannian-cut-point)

A [Riemannian cut point](#riemannian-cut-point) along a [geodesic](#geodesic) in a complete [Riemannian manifold](#riemannian-manifold) is either its first [conjugate point](calculus-of-variations.md#conjugate-point) or the endpoint of another minimizing [geodesic](#geodesic) from the initial point. To prove this, approach the cut time from above and choose minimizing geodesics to the later endpoints using the [Hopf-Rinow theorem](#hopf-rinow-theorem). A subsequence of their initial unit vectors converges. If its limit is the original initial vector and the cut endpoint is not conjugate, the [inverse function theorem](calculus.md#inverse-function-theorem) for the [Riemannian exponential map](#exponential-map-riemannian-geometry) identifies the two geodesics locally and contradicts the shorter length of the chosen minimizers. A conjugate point earlier than the cut time is excluded by the negative [Riemannian index form](#riemannian-index-form) direction obtained by extending an endpoint-vanishing [Jacobi field](general-relativity.md#jacobi-field) by zero and perturbing its endpoint corner.

## Riemannian product

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)

For Riemannian manifolds $(M,g)$ and $(N,h)$, the product metric on $M\times N$ is $g\oplus h$. Its Levi-Civita connection and curvature split by factors, so its Ricci and scalar curvatures are the corresponding sums.

This equips a [product manifold](differential-geometry.md#product-manifold) with the direct-sum [Riemannian metric](differential-geometry.md#riemannian-metric).

### Product Laplacian eigenspace decomposition

↑ **Parent:** [Riemannian product](#riemannian-product)

For [closed manifolds](differential-geometry.md#closed-manifold) with the product [Riemannian metric](differential-geometry.md#riemannian-metric), the [positive Laplace-Beltrami operator](differential-geometry.md#positive-laplace-beltrami-operator) is the sum of the two factor operators. Products of their [orthonormal eigenbases](linear-operator-theory.md#orthonormal-eigenbasis) form a complete basis, and [eigenvalues](linear-operator-theory.md#eigenvalue) add. Hence the product [eigenspace](linear-operator-theory.md#eigenspace) at $\lambda$ is the displayed finite orthogonal sum of [tensor products](linear-algebra.md#tensor-product). The discrete assertion requires a discrete spectral setting.

#### Isospectral stabilization by a small flat torus

↑ **Parent:** [Product Laplacian eigenspace decomposition](#product-laplacian-eigenspace-decomposition)

Two [isospectral manifolds](#isospectral-manifolds) remain isospectral after taking a [Riemannian product](#riemannian-product) with the same [closed](topology.md#closed-set) factor: [eigenvalues](linear-operator-theory.md#eigenvalue) add, with [multiplicities](polynomial.md#multiplicity-mathematics) given by the [product Laplacian eigenspace decomposition](#product-laplacian-eigenspace-decomposition). For nonisometric [closed](topology.md#closed-set) connected factors $M_1,M_2$, choose $\varepsilon<\delta<\min_i\operatorname{inj}(M_i)$. Every [closed](topology.md#closed-set) product [geodesic](#geodesic) of length less than $\delta$ has constant projection to $M_i$, since a nonconstant [closed geodesic](#closed-geodesic) shorter than the [injectivity radius](#injectivity-radius) is impossible. The short coordinate [geodesics](#geodesic) of the small [flat torus](second-fundamental-form.md#flat-torus) span exactly its tangent factor at every point. Any product [Riemannian isometry](differential-geometry.md#riemannian-isometry) must preserve that intrinsically defined [smooth distribution](differential-geometry.md#distribution-differential-geometry) and its [orthogonal complement](hilbert-space.md#orthogonal-complement), hence restrict to an [isometry](#isometry) of the original factors. Thus these products are still nonisometric. Taking $M_i$ to be four-dimensional [tori](topology.md#torus) proves the higher-dimensional stabilization statement without assuming a cancellation theorem for arbitrary products.

## Isometry

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isometry)

An isometry between [metric spaces](topological-analysis.md#metric-space) preserves every distance. A Riemannian isometry preserves the Riemannian metric and therefore distances, angles, geodesics, and intrinsic curvature.

### Isometry group

↑ **Parent:** [Isometry](#isometry)

The [isometry group](#isometry-group) of a [metric space](topological-analysis.md#metric-space) consists of its bijective [isometries](#isometry), with composition as the group operation. For a [Riemannian metric](differential-geometry.md#riemannian-metric), these are the [diffeomorphisms](geometry-and-topology.md#diffeomorphism) preserving the [metric tensor](general-relativity.md#metric-tensor). Right translations of a [right-invariant Riemannian metric](lie-theory.md#right-invariant-riemannian-metric) supply a faithful subgroup isomorphic to the underlying [Lie group](lie-theory.md#lie-group).

#### Finite orientation-preserving plane isometry groups are cyclic

↑ **Parent:** [Isometry group](#isometry-group)

A finite [group](group.md) of orientation-preserving [isometries](#isometry) of the [Euclidean plane](geometry-and-topology.md#euclidean-plane) or [hyperbolic plane](geometry-and-topology.md#hyperbolic-plane) is a [cyclic group](group.md#cyclic-group). Take one orbit and its unique minimum-radius enclosing disc. Every group element preserves the orbit and therefore the disc's centre. The orientation-preserving stabilizer of a point acts as planar rotations, so the group embeds in the circle group. In a nontrivial finite subgroup, the least positive rotation angle generates all angles by division with remainder, proving cyclicity. Orientation reversal changes the conclusion: reflection groups need not be cyclic.

#### Isometry dimensions in dimension three

↑ **Parent:** [Isometry group](#isometry-group)

For a connected three-dimensional [Riemannian manifold](#riemannian-manifold), the [Myers-Steenrod theorem](#myers-steenrod-theorem) bounds the dimension of its isometry group by six. Dimension five cannot occur: isotropy embeds in $O(3)$, whose Lie subalgebras have dimensions zero, one or three. A five-dimensional action would require three-dimensional isotropy and a two-dimensional orbit; full rotational isotropy has no invariant tangent two-plane. The maximal dimension six forces transitivity and isotropy, hence constant sectional curvature. Each of the six listed dimensions is attained by a suitable metric.

#### Isometry group of a Riemannian quotient

↑ **Parent:** [Isometry group](#isometry-group)

For a complete simply connected [Riemannian manifold](#riemannian-manifold) $X$ and a free properly discontinuous deck group $\Gamma$, each isometry of $X/\Gamma$ lifts to an isometry of $X$ normalizing $\Gamma$. Conversely such a normalizing isometry descends; two lifts differ by a deck transformation. This proves the formula, including orientation-reversing isometries if the full normalizer is used.

#### Myers-Steenrod theorem

↑ **Parent:** [Isometry group](#isometry-group)

The isometry group of a smooth connected [Riemannian manifold](#riemannian-manifold) is a finite-dimensional [Lie group](lie-theory.md#lie-group), and its action is smooth. An isometry is determined by its value and derivative at one point, since it preserves the exponential map and continuation along geodesics. The stabilizer embeds in $O(n)$, giving dimension at most $n(n+1)/2$. For a [compact manifold](differential-geometry.md#compact-manifold) the isometry group is compact.

#### Fixed point of a finite Euclidean isometry group

↑ **Parent:** [Isometry group](#isometry-group)

A finite [group](group.md) of [Euclidean isometries](#euclidean-isometry) has a common [fixed point](function.md#fixed-point): average any orbit. Each [isometry](#isometry) is an [affine map](geometry-and-topology.md#affine-map) and therefore preserves this finite affine average; applying a [group](group.md) element merely permutes the orbit terms. To see that an isometry is affine, subtract its value at zero and use the [polarization identity](linear-algebra.md#polarization-identity) to show that the resulting map preserves inner products. Images of a standard [orthonormal basis](linear-algebra.md#orthonormal-basis) then determine a linear orthogonal map.

### Fixed-point set

↑ **Parent:** [Isometry](#isometry)

The fixed-point set of a map $f:M\to M$ is $M^f=\{x:f(x)=x\}$. For an isometry of a Riemannian manifold, each smooth component of the fixed-point set is totally geodesic.

### Euclidean isometry

↑ **Parent:** [Isometry](#isometry)

A Euclidean isometry has the form $\mathbf x\mapsto\mathbf a+R\mathbf x$, where $R$ is orthogonal. It preserves inner products of displacement vectors, distances, angles, and arc length.

#### Rigidity of a scalene triangle

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)

The vertex [set](set.md) of a triangle with three distinct side lengths has trivial setwise [stabilizer subgroup](group-theory.md#stabilizer-subgroup) in the plane [isometry group](#isometry-group). Each vertex is characterized by the unordered pair of lengths of its incident edges, so a setwise-preserving [Euclidean isometry](#euclidean-isometry) fixes every vertex. An [isometry](#isometry) fixing three noncollinear plane points is the identity: squared [Euclidean distances](topological-analysis.md#euclidean-distance) to them determine every other point, since subtracting two of the [Euclidean distance](topological-analysis.md#euclidean-distance) equations gives two independent linear equations. For example, $(0,0),(1,0),(0,2)$ have side lengths $1,2,\sqrt5$.

#### Rotation (mathematics)

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)

In [Euclidean geometry](geometry-and-topology.md#euclidean-geometry), a rotation about the origin is an orientation-preserving orthogonal [linear map](vector-space.md#linear-map), represented by an element of the [special orthogonal group](linear-algebra.md#special-orthogonal-group). About another center $a$, the map has form $x\mapsto a+R(x-a)$. In three dimensions a nonidentity rotation fixes an axis.

#### Translation subgroup

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)

The translation subgroup of a group of [Euclidean isometries](#euclidean-isometry) consists of its [translations](geometry-and-topology.md#translation-geometry). It is a [normal subgroup](group-theory.md#normal-subgroup), because conjugation by $x\mapsto Ax+b$ takes translation by $v$ to translation by $Av$. Its vectors form an additive subgroup of Euclidean space; for a [plane crystallographic group](geometry-and-topology.md#wallpaper-group) they form a rank-two [translation lattice](#translation-lattice).

##### Translation lattice

↑ **Parent:** [Translation subgroup](#translation-subgroup)

A translation lattice is the additive group generated by linearly independent vectors $v_1,\ldots,v_r$ in a Euclidean space. It defines a [discrete subgroup](topological-group.md#discrete-subgroup) of [translations](geometry-and-topology.md#translation-geometry). A full-rank translation lattice has a compact parallelepiped as a fundamental region and therefore a [cocompact group action](geometric-group-theory.md#cocompact-group-action). This geometric usage is distinct from an order-theoretic lattice.

#### Frieze group

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frieze_group)

A [discrete subgroup](topological-group.md#discrete-subgroup) of [Euclidean isometries](#euclidean-isometry) is a frieze group when its [translation subgroup](#translation-subgroup) is infinite cyclic and has finite index. Translations along a line alone give $\mathbb Z$; adding perpendicular mirrors gives the [infinite dihedral group](representation-theory.md#infinite-dihedral-group), while adding a mirror along the translation direction gives $\mathbb Z\times C_2$. These groups describe patterns periodic in one planar direction.

#### Glide reflection

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)

A glide reflection of the plane composes reflection in a line with a nonzero translation parallel to that line. It reverses orientation and has no fixed point. It cannot be one reflection, because a reflection fixes a line, or a product of two reflections, because such a product preserves orientation. The [finite reflection decomposition of a Euclidean isometry](#finite-reflection-decomposition-of-a-euclidean-isometry) therefore shows that it requires exactly three reflections.

#### Finite reflection decomposition of a Euclidean isometry

↑ **Parent:** [Euclidean isometry](#euclidean-isometry)

Every [Euclidean isometry](#euclidean-isometry) of $\mathbb R^n$ is a product of at most $n+1$ operations of [reflection in a hyperplane](linear-algebra.md#reflection-in-a-hyperplane). An isometry fixing zero is orthogonal: the [polarization identity](linear-algebra.md#polarization-identity) preserves inner products, and its values on an orthonormal basis determine its linear action. An [orthogonal transformation](linear-algebra.md#orthogonal-transformation) is a product of at most $n$ linear reflections, by reflecting the image of the first basis vector back to that vector and inducting on its orthogonal complement. For an arbitrary isometry, first reflect its image of zero back to zero, if necessary, and apply the orthogonal result. Affine reflection hyperplanes, rather than only hyperplanes through zero, are essential here.

##### Reflection length of a Euclidean orthogonal map

↑ **Parent:** [Finite reflection decomposition of a Euclidean isometry](#finite-reflection-decomposition-of-a-euclidean-isometry)

A product of $m$ [reflections](linear-algebra.md#reflection-mathematics) has $\operatorname{rank}(I-Q)\le m$, by the rank inequality applied successively to $I-AB=(I-A)+A(I-B)$. Conversely an [orthogonal transformation](linear-algebra.md#orthogonal-transformation) fixes the orthogonal complement of its moved space; successive Householder reflections fix one new basis direction at each step in that moved space. At most its dimension $\operatorname{rank}(I-Q)$ are required. Thus central inversion in three dimensions needs exactly three reflections.

### Isometric embedding

↑ **Parent:** [Isometry](#isometry)

An isometric embedding $f:X\to Y$ between [metric spaces](topological-analysis.md#metric-space) is an [injective function](algebra.md#injective-function) satisfying $d_Y(f(x),f(x'))=d_X(x,x')$ for all $x,x'\in X$.

#### Isometric extension

↑ **Parent:** [Isometric embedding](#isometric-embedding)

An [isometric extension](#isometric-extension) of a connected metric manifold is a proper embedding onto an open subset of a larger connected manifold of the same dimension, preserving the [metric tensor](general-relativity.md#metric-tensor). Smooth complete connected [Riemannian manifolds](#riemannian-manifold) admit no such proper extension; Lorentzian geodesic completeness has different subtleties.

## Geodesic

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic)

A geodesic is a curve whose tangent vector is parallel along the curve. Equivalently, it has zero covariant acceleration; on an embedded surface, a unit-speed geodesic has acceleration normal to the surface.

### Conjugate points

↑ **Parent:** [Geodesic](#geodesic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_points)

Two points along a [geodesic](#geodesic) are conjugate when a nonzero [Jacobi field](general-relativity.md#jacobi-field) along it vanishes at both points. This detects singularity of the geodesic exponential map and governs loss of local length minimization.

### Local extension of geodesic velocity

↑ **Parent:** [Geodesic](#geodesic)

The velocity of a [geodesic](#geodesic) can be extended to one smooth ambient [vector field](calculus.md#vector-field) on a sufficiently short neighbourhood of any parameter value. If its initial velocity is zero, uniqueness of the [geodesic equation](#geodesic-equation) makes it locally constant, and the zero field works. Otherwise one coordinate has nonzero velocity; the [inverse function theorem](calculus.md#inverse-function-theorem) supplies coordinates straightening the small embedded arc to $(t,0,\ldots,0)$. The coordinate field $\partial/\partial t$ is the required extension. Shrinking the interval is essential: arbitrary fields along self-intersecting curves need not have one ambient extension.

### Liouville metric geodesic integral

↑ **Parent:** [Geodesic](#geodesic)

For a surface metric $(U(u)+V(v))(du^2+dv^2)$ with $U+V>0$, an affinely parametrized [geodesic](#geodesic) has constant energy $E=(U+V)(\dot u^2+\dot v^2)/2$. Put $p=(U+V)\dot u$. The [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) give $\dot p=EU'/(U+V)$. Thus $K=p^2-2EU$ has derivative zero, proving the displayed additional quadratic integral. This separation structure is a geometric example of [Liouville integrability](classical-mechanics.md#integrable-hamiltonian-system).

### Spacelike geodesic

↑ **Parent:** [Geodesic](#geodesic)

A spacelike geodesic has positive tangent norm in signature $(-+++)$ and satisfies the [geodesic equation](#geodesic-equation) with an [affine parameter](#affine-parameter). [Metric compatibility](fiber-bundle.md#metric-compatibility) preserves that norm along the curve. In [Minkowski spacetime](special-relativity.md#minkowski-spacetime) these are straight lines whose spatial tangent is larger in magnitude than the time component; their two ends approach [spacelike infinity](general-relativity.md#spacelike-infinity) in a [conformal completion](general-relativity.md#conformal-completion).

### Closed geodesic

↑ **Parent:** [Geodesic](#geodesic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_geodesic)

A nonconstant [geodesic](#geodesic) whose position and tangent velocity repeat after a positive time. On a [flat torus](second-fundamental-form.md#flat-torus) it is a straight line modulo the lattice, closing when its displacement is a [Euclidean lattice](fourier-analysis.md#euclidean-lattice) vector. A primitive closed geodesic traverses its image without being an iterate of a shorter periodic geodesic.

#### Primitive closed geodesic

↑ **Parent:** [Closed geodesic](#closed-geodesic)

A [primitive closed geodesic](#primitive-closed-geodesic) is a closed [geodesic](#geodesic) with its smallest positive period, rather than a repeated traversal of a shorter periodic geodesic. A degree-$m$ lift of a primitive base geodesic is still primitive upstairs when its [monodromy permutation](algebraic-topology.md#monodromy-permutation) has a cycle of exact length $m$: no smaller number of traversals returns to the starting sheet.

### Uniqueness of a closed geodesic on a negatively curved cylinder

↑ **Parent:** [Geodesic](#geodesic)

A surface homeomorphic to a cylinder with strictly negative Gaussian curvature has at most one closed geodesic image. Geodesic disks, monogons and bigons are excluded by [Gauss-Bonnet theorem](differential-geometry.md#gauss-bonnet-theorem); distinct essential simple geodesics would bound an annulus whose curvature integral must vanish. Repeated traversals count as the same image.

### Pregeodesic

↑ **Parent:** [Geodesic](#geodesic)

A [pregeodesic](#pregeodesic) is a curve whose tangent obeys $\nabla_UU=\kappa U$ for some scalar $\kappa$. A change of parameter makes it a [geodesic](#geodesic) with an [affine parameter](#affine-parameter). A varying speed along a geodesic changes its parameter, not its image.

#### Null pregeodesic

↑ **Parent:** [Pregeodesic](#pregeodesic)

A [null pregeodesic](#null-pregeodesic) has a [null tangent](special-relativity.md#null-vector) and can be parametrized as a [null geodesic](special-relativity.md#null-geodesic). In a two-dimensional [Lorentzian metric](general-relativity.md#lorentzian-metric), the acceleration of a regular [null curve](special-relativity.md#null-curve) is orthogonal to its tangent and therefore proportional to it.

### Geodesic convexity

↑ **Parent:** [Geodesic](#geodesic)

A subset of a [Riemannian manifold](#riemannian-manifold) is geodesically convex when any two of its points can be joined by a minimizing [geodesic segment](#geodesic-segment) lying in the subset. In the [hyperbolic plane](geometry-and-topology.md#hyperbolic-plane) the joining [geodesic segment](#geodesic-segment) is unique. Thus in the [Beltrami-Klein model](geometry-and-topology.md#beltrami-klein-model), geodesically convex subsets correspond to Euclidean [convex sets](mathematical-optimization.md#convex-set).

### Geodesic segment

↑ **Parent:** [Geodesic](#geodesic)

A geodesic segment is the restriction of a [geodesic](#geodesic) to a compact parameter interval. In the [hyperbolic plane](geometry-and-topology.md#hyperbolic-plane), two points determine a unique geodesic segment, which minimizes the [hyperbolic distance](geometry-and-topology.md#hyperbolic-distance) between them.

### Distance minimizers on a punctured sphere

↑ **Parent:** [Geodesic](#geodesic)

On the unit [sphere](geometry-and-topology.md#sphere) with one point deleted, a distinct nonantipodal pair has a length minimizer exactly when its shorter [great circle](geometry-and-topology.md#great-circle) arc avoids the deleted point. Antipodal pairs admit an avoiding semicircle. If the unique shorter arc crosses the puncture, smooth detours approach its length without attaining it.

### Geodesic variation

↑ **Parent:** [Geodesic](#geodesic)

A geodesic variation of a given [geodesic](#geodesic) is a smooth family $F(s,t)$ with $F(0,t)=\gamma(t)$, whose curves at fixed $s$ are affinely parametrized geodesics. Differentiating its geodesic equation and using the torsion-free [Levi-Civita connection](general-relativity.md#levi-civita-connection) gives the [Jacobi field](general-relativity.md#jacobi-field) equation $D_t^2J+R(J,\dot\gamma)\dot\gamma=0$ for $J=\partial_sF|_{s=0}$.

#### Deviation vector

↑ **Parent:** [Geodesic variation](#geodesic-variation)

For a [geodesic variation](#geodesic-variation) $F(s,\tau)$, the [deviation vector](#deviation-vector) $S=F_*\partial_s$ describes infinitesimal separation at equal parameter values. With $T=F_*\partial_\tau$, commuting parameter derivatives give $[S,T]=0$. A [torsion-free connection](fiber-bundle.md#torsion-free-connection) then gives $\nabla_TS=\nabla_ST$. For an affinely parametrized variation, [geodesic deviation](general-relativity.md#geodesic-deviation) states $\nabla_T^2S=R(T,S)T$ with the convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$.

#### Realization of Jacobi fields by geodesic variations

↑ **Parent:** [Geodesic variation](#geodesic-variation)

Given a [Jacobi field](general-relativity.md#jacobi-field) with initial values $J(0)=a$ and $D_tJ(0)=b$, vary the initial point along a curve with tangent $a$ and the initial velocity with covariant derivative $b$. The resulting [geodesic variation](#geodesic-variation) has the same Jacobi initial values and therefore the same field by uniqueness of the linear equation. Smooth dependence on initial conditions gives a common parameter interval around any fixed compact geodesic segment, even on an incomplete manifold.

### Geodesic triangle

↑ **Parent:** [Geodesic](#geodesic)

A geodesic triangle is bounded by three geodesic segments. On a surface its angle excess is the integral of the [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) over the triangle.

It is the three-sided instance of a [geodesic polygon](#geodesic-polygon).

### Surface covariant derivative

↑ **Parent:** [Geodesic](#geodesic)

For a tangent vector field $V$ along a curve on an embedded surface, the surface covariant derivative is the tangential projection of its ordinary derivative:

$$
D_sV=\left(\frac{dV}{ds}\right)^\top.
$$

It is the covariant derivative induced by the surface metric.

#### Surface tangent projector

↑ **Parent:** [Surface covariant derivative](#surface-covariant-derivative)

The orthogonal projector onto the tangent plane of a surface with unit [normal vector](differential-geometry.md#normal-vector) $\mathbf n$. It removes the normal component of a vector and defines the [surface gradient](#surface-gradient) $\nabla_s=P\nabla$.

##### Sphere surface derivative identities

↑ **Parent:** [Surface tangent projector](#surface-tangent-projector)

On a sphere of radius $a$, $\nabla_s\mathbf n=P/a$, $\nabla_s\cdot\mathbf n=2/a$, and $\Delta_s\mathbf n=-2\mathbf n/a^2$. For a constant vector $\mathbf U$, $\nabla_s\cdot(P\mathbf U)=-2\mathbf U\cdot\mathbf n/a$. These identities simplify dipolar [surface diffusion](fluid-mechanics.md#surface-diffusion) and interfacial transport.

#### Surface gradient

↑ **Parent:** [Surface covariant derivative](#surface-covariant-derivative)

For an embedded surface with unit [normal vector](differential-geometry.md#normal-vector) $\mathbf n$, the surface gradient is $\nabla_sf=(\mathbf I-\mathbf n\mathbf n^T)\nabla f$. It projects the ambient [gradient](calculus.md#gradient) onto the [tangent space](differential-geometry.md#tangent-space) and is independent of how $f$ is extended normally off the surface.

#### Surface divergence

↑ **Parent:** [Surface covariant derivative](#surface-covariant-derivative)

The surface divergence of an ambient [vector field](calculus.md#vector-field) is the tangential [trace](linear-algebra.md#matrix-trace) $\nabla_s\cdot\mathbf v=(\delta_{ij}-n_in_j)\partial_jv_i$. For a tangent [vector field](calculus.md#vector-field) it is the intrinsic [divergence](calculus.md#divergence). For $\mathbf v=\mathbf n$ it gives the sum of the two principal [curvatures](differential-geometry.md#curvature); a sphere with outward normal has $\nabla_s\cdot\mathbf n=2/a$.

##### Surface divergence theorem for a tangent field

↑ **Parent:** [Surface divergence](#surface-divergence)

For a smooth tangent [vector field](calculus.md#vector-field) $v$ on a compact [orientable surface](differential-geometry.md#orientable-surface) with smooth boundary and [outward conormal of a surface boundary](differential-geometry.md#outward-conormal-of-a-surface-boundary), the integral of its [surface divergence](#surface-divergence) is its boundary [flux](physics.md#flux). Extend the unit [normal vector](differential-geometry.md#normal-vector) to a unit field $m$. The [curl of a cross product](calculus.md#curl-of-a-cross-product) gives $m\cdot\nabla\times(m\times v)=\nabla\cdot v-m_im_j\partial_jv_i$ on the surface: $m\cdot v=0$ there and $m\cdot\partial_jm=0$ by unit length. Apply [Stokes theorem](calculus.md#stokes-theorem) and use $(m\times v)\cdot d\mathbf r=v\cdot(d\mathbf r\times m)$ to obtain the formula.

### Exponential map (Riemannian geometry)

↑ **Parent:** [Geodesic](#geodesic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_map_(Riemannian_geometry))

For $p$ in a Riemannian manifold and $v$ sufficiently close to zero in $T_pM$, let $\gamma_v$ be the geodesic with $\gamma_v(0)=p$ and $\dot\gamma_v(0)=v$. The exponential map is

$$
\exp_p(v)=\gamma_v(1).
$$

Equivalently, $\exp_p(tv)=\gamma_v(t)$ wherever both sides are defined.

#### Differential of the exponential map at zero

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)

For the [Riemannian exponential map](#exponential-map-riemannian-geometry) $\exp_p(v)=\gamma_v(1)$, uniqueness of the [geodesic equation](#geodesic-equation) gives $\exp_p(tv)=\gamma_v(t)$. Differentiation at $t=0$ yields $(d\exp_p)_0v=v$. Smooth ODE dependence and the [inverse function theorem](calculus.md#inverse-function-theorem) therefore make $\exp_p$ a [diffeomorphism](geometry-and-topology.md#diffeomorphism) on a neighborhood of zero, producing [geodesic normal coordinates](#geodesic-normal-coordinates). This is a local assertion and requires no geodesic completeness.

#### Convex normal neighbourhood

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)

A convex normal neighbourhood is an open set whose points have unique smoothly varying joining [geodesics](#geodesic), with the joining geodesic contained in the set. The corresponding star-shaped restriction of each [exponential map](#exponential-map-riemannian-geometry) is a [diffeomorphism](geometry-and-topology.md#diffeomorphism) onto the neighbourhood. Hence its differential is invertible and no such joining geodesic admits a nonzero [Jacobi field](general-relativity.md#jacobi-field) vanishing at both endpoints. Every point of a [Riemannian manifold](#riemannian-manifold) has arbitrarily small such neighbourhoods. This is stronger than merely requiring the existence of a minimizing geodesic in the set.

#### Geodesic flow

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_flow)

The geodesic flow sends a tangent vector $v$ to the velocity at time $t$ of the unique geodesic with initial velocity $v$. Smooth dependence of solutions of the [geodesic equation](#geodesic-equation) makes it a smooth flow on the tangent bundle wherever defined.

##### Geodesic hyperbolicity from negative Gaussian curvature

↑ **Parent:** [Geodesic flow](#geodesic-flow)

A perpendicular [Jacobi field](general-relativity.md#jacobi-field) on a [Riemannian surface](#riemannian-surface) has scalar equation $\ddot y+Ky=0$. For strictly negative curvature on a [closed manifold](differential-geometry.md#closed-manifold), the displayed derivative is uniformly positive definite, so the [quadratic-form criterion for an Anosov flow](dynamical-systems.md#quadratic-form-criterion-for-an-anosov-flow) makes the [geodesic flow](#geodesic-flow) Anosov. When $K=-1$, the stable and unstable lines in the canonical frame are respectively $\mathbb R(H-V)$ and $\mathbb R(H+V)$, with factors $e^{-t}$ and $e^t$.

##### Generalized thermostat on a Riemannian surface

↑ **Parent:** [Geodesic flow](#geodesic-flow)

A smooth real function $\lambda$ on the [unit tangent bundle](fiber-bundle.md#unit-tangent-bundle) determines this unit-speed [smooth flow](dynamical-systems.md#smooth-flow). Its base velocity is $v$, so its generator never vanishes. In the canonical frame its divergence in [Liouville volume of a surface geodesic flow](fiber-bundle.md#liouville-volume-of-a-surface-geodesic-flow) is $V\lambda$. The special case where $\lambda$ depends only on the base is a [magnetic flow](#magnetic-flow-on-a-riemannian-surface); when $\lambda(x,v)=\langle E(x),iv\rangle$ it is a [Gaussian thermostat](#gaussian-thermostat).

###### Linearized transverse equation for a surface thermostat

↑ **Parent:** [Generalized thermostat on a Riemannian surface](#generalized-thermostat-on-a-riemannian-surface)

Write a tangent variation of a [surface thermostat](#generalized-thermostat-on-a-riemannian-surface) as $aF+yH+zV$ in the canonical frame. The commutators $[F,H]=-\lambda F+(K-H\lambda+\lambda^2)V$ and $[F,V]=-H-(V\lambda)V$ give $\dot a=\lambda y$ and the stated transverse equation. Near the vertical projective direction, $r=y/z$ obeys $\dot r=1-(V\lambda)r+(K-H\lambda+\lambda^2)r^2$.

###### Gaussian thermostat

↑ **Parent:** [Generalized thermostat on a Riemannian surface](#generalized-thermostat-on-a-riemannian-surface)

At unit speed on a [Riemannian surface](#riemannian-surface), the right-hand side is $\langle E,iv\rangle iv$. This removes the velocity-parallel component of the forcing, so differentiating $|\dot\gamma|^2$ gives zero. The dynamics need not preserve the ordinary [Liouville volume of a surface geodesic flow](fiber-bundle.md#liouville-volume-of-a-surface-geodesic-flow).

###### Divergence of a Gaussian thermostat

↑ **Parent:** [Gaussian thermostat](#gaussian-thermostat)

For $F=X+\lambda V$, the canonical fields $X,V$ preserve [Liouville volume of a surface geodesic flow](fiber-bundle.md#liouville-volume-of-a-surface-geodesic-flow), so the divergence is $V\lambda$. For a [Gaussian thermostat](#gaussian-thermostat), $\lambda=\langle E,iv\rangle$ and $V(iv)=-v$, giving the stated sign. If $E=\nabla f$, then the density $e^{f\circ\pi}$ makes this divergence zero.

##### Magnetic flow on a Riemannian surface

↑ **Parent:** [Geodesic flow](#geodesic-flow)

A unit-speed curve with $D_t\dot\gamma=f(\gamma)i\dot\gamma$ defines the magnetic flow. The vertical term rotates the velocity while the horizontal part transports it along the base. Since $V(f\circ\pi)=0$, the divergence of $X+fV$ in Liouville volume vanishes. The associated two-form on the unit tangent bundle is $d\alpha-f\pi^*\Omega_a=-\iota_F\mu$, whose kernel is the magnetic flow direction.

###### Contact rigidity of a zero-flux Anosov magnetic flow

↑ **Parent:** [Magnetic flow on a Riemannian surface](#magnetic-flow-on-a-riemannian-surface)

On a connected closed oriented surface, a magnetic Anosov flow with $\int f\Omega_a=0$ preserves a smooth contact form only when $f=0$. To see the obstruction, take $d\eta=f\Omega_a$ and $\sigma=\alpha-\pi^*\eta$. An invariant contact form can be normalized to evaluate to one on $F$; its differential is a constant multiple of $\iota_F\mu$, since smooth invariant functions are constant. Averaging closed one-forms forces that multiple to be $-1$, so the contact form differs from $\sigma$ by a closed form. Its fibre-average decomposition gives $Fh=(\eta-\xi)(v)-af$. The degree-zero/one kernel theorem gives $af=0$ and $d\eta=d\xi=aK\Omega_a$, forcing $f=0$ whether $a$ vanishes or not. For $f=0$, the canonical form $\alpha$ is invariant and contact.

##### Geodesic Hamiltonian

↑ **Parent:** [Geodesic flow](#geodesic-flow)

The metric defines this globally smooth [Hamiltonian](classical-mechanics.md#hamiltonian) on the [cotangent bundle](symplectic-geometry.md#cotangent-bundle). With $\omega=dx^i\wedge dp_i$ and $\iota_{X_H}\omega=dH$, its [Hamiltonian vector field](symplectic-geometry.md#hamiltonian-vector-field) projects to affinely parametrized [geodesics](#geodesic). The momentum is $p_i=g_{ij}\dot x^j$, and its conserved value is half the squared speed.

#### Domain of the exponential map

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)

The domain of $\exp_p$ is the star-shaped open set

$$
\mathcal D_p=\{v\in T_pM:\gamma_v\text{ exists on }[0,1]\}.
$$

Smooth dependence for ordinary differential equations makes $(p,v)\mapsto\exp_p(v)$ smooth on its open domain in $TM$.

##### Exponential map of the punctured plane

↑ **Parent:** [Domain of the exponential map](#domain-of-the-exponential-map)

For $S=(\mathbb R^2\setminus\{0\})\times\{0\}\subset\mathbb R^3$ and $p=(1,0,0)$, geodesics are straight lines until they hit the missing origin. Thus $(-2,0,0)\notin\mathcal D_p$, and $(-1,0,0)$ is not in the image of $\exp_p$ because its unique straight segment from $p$ passes through the origin.

#### Normal neighbourhood

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)

A normal neighbourhood of $p$ is the diffeomorphic image under $\exp_p$ of a star-shaped neighbourhood of $0$ in $T_pM$. In a sufficiently small normal ball, radial geodesics from $p$ uniquely minimize length.

##### Radial distance in a normal neighbourhood

↑ **Parent:** [Normal neighbourhood](#normal-neighbourhood)

In a [normal neighbourhood](#normal-neighbourhood) $U=\exp_p(V)$ with $V$ star-shaped, define $r(q)=|\exp_p^{-1}(q)|$. Away from $p$, the [Gauss lemma](#gauss-s-lemma-riemannian-geometry) gives $\nabla r=(d\exp_p)_v(v/|v|)$ for $v=\exp_p^{-1}(q)$. Thus $|\nabla r|=1$ and this unit [vector field](calculus.md#vector-field) is tangent to unit-speed radial [geodesics](#geodesic). The function $r$ is not smooth at $p$, but $r^2/2$ is smooth and $\nabla(r^2/2)=(d\exp_p)_v v$ extends by zero. On a sufficiently small normal ball, $r$ equals the [Riemannian distance](#riemannian-distance) from $p$.

// Target: riemannian-geometry.bigb

###### Radial vector field in a normal neighbourhood

↑ **Parent:** [Radial distance in a normal neighbourhood](#radial-distance-in-a-normal-neighbourhood)

The unit radial [vector field](calculus.md#vector-field) is $E=\nabla r$ on the punctured [normal neighbourhood](#normal-neighbourhood), where $r$ is the [radial distance in a normal neighbourhood](#radial-distance-in-a-normal-neighbourhood). Along $\gamma_u(t)=\exp_p(tu)$ with $|u|=1$, it satisfies $E(\gamma_u(t))=\dot\gamma_u(t)$. The scaled radial field $W=rE=\nabla(r^2/2)$ is smooth at the centre and vanishes there. These conventions have different associated radial functions.

// Target: riemannian-geometry.bigb

##### Injectivity radius

↑ **Parent:** [Normal neighbourhood](#normal-neighbourhood)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Injectivity_radius)

The injectivity radius at $p$ is the largest radius on which $\exp_p$ is a diffeomorphism from the tangent-space ball onto its image. The injectivity radius of a compact Riemannian manifold is the positive infimum of these pointwise radii.

##### Geodesic normal coordinates

↑ **Parent:** [Normal neighbourhood](#normal-neighbourhood)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_normal_coordinates)

Choose an orthonormal basis of $T_pM$ and use its linear coordinates on a neighborhood of zero on which $\exp_p$ is a diffeomorphism. Transporting these coordinates through $\exp_p$ gives geodesic normal coordinates centered at $p$.

###### Christoffel symbols vanish at the center of normal coordinates

↑ **Parent:** [Geodesic normal coordinates](#geodesic-normal-coordinates)

In [geodesic normal coordinates](#geodesic-normal-coordinates) at $p$, radial [geodesics](#geodesic) have coordinates $x(t)=tv$. The [geodesic equation](#geodesic-equation) at $t=0$ gives $\Gamma^i_{jk}(p)v^jv^k=0$ for every $v$. The [Levi-Civita connection](general-relativity.md#levi-civita-connection) is torsion free, making these coefficients symmetric in $j,k$; the [polarization identity](linear-algebra.md#polarization-identity) then gives $\Gamma^i_{jk}(p)=0$. This does not imply vanishing curvature, which depends on derivatives of the coefficients.

###### Geodesic sphere

↑ **Parent:** [Geodesic normal coordinates](#geodesic-normal-coordinates)

A geodesic sphere is a level set of [Riemannian distance](#riemannian-distance) from a point. For sufficiently small positive $r$, it is the [exponential map](#exponential-map-riemannian-geometry) image of the radius-$r$ tangent sphere, a smooth compact hypersurface. The [Gauss lemma](#gauss-s-lemma-riemannian-geometry) makes its tangent space orthogonal to the radial direction. Larger distance spheres need not be smooth at the [cut locus](#cut-locus).

###### Radial Christoffel-symbol criterion for geodesic coordinates

↑ **Parent:** [Geodesic normal coordinates](#geodesic-normal-coordinates)

A chart $x$ centered at $p$ on a star-shaped coordinate domain is a geodesic normal chart exactly when $g_{ij}(0)=\delta_{ij}$ and

$$
x^ix^j\Gamma^k_{ij}(x)=0
$$

for every $x$ and $k$. This is the geodesic equation for every radial curve $t\mapsto tx$.

#### Geodesic polar coordinates

↑ **Parent:** [Exponential map (Riemannian geometry)](#exponential-map-riemannian-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_polar_coordinates)

Choose an orthonormal basis of $T_pM$ and put $e(\theta)=(\cos\theta,\sin\theta)$. Away from the centre and cut locus,

$$
\phi(r,\theta)=\exp_p\bigl(r e(\theta)\bigr)
$$

defines geodesic polar coordinates centred at $p$.

##### Radial Riccati equation for distance spheres

↑ **Parent:** [Geodesic polar coordinates](#geodesic-polar-coordinates)

Before the [cut locus](#cut-locus), define $A(X)=\nabla_X\partial_r$ on the tangent space of a distance sphere. This is the negative of the [shape operator](second-fundamental-form.md#shape-operator) with outward normal under the convention $S=-\nabla\nu$. A nonsingular matrix $Y$ of radial [Jacobi fields](general-relativity.md#jacobi-field) satisfies $Y''+\mathcal R_{\partial_r}Y=0$ and $A=Y'Y^{-1}$, yielding the displayed matrix [Riccati equation](analysis.md#riccati-equation). Taking its trace gives $h'+\operatorname{tr}(A^2)+\operatorname{Ric}(\partial_r,\partial_r)=0$, where $h=\operatorname{tr}A=\partial_r\log\det Y$. This is the local differential identity behind the [Bishop-Gromov inequality](second-fundamental-form.md#bishop-gromov-inequality).

##### Geodesic circle

↑ **Parent:** [Geodesic polar coordinates](#geodesic-polar-coordinates)

For $r$ smaller than the normal-coordinate radius, the [geodesic circle](#geodesic-circle) on a [Riemannian surface](#riemannian-surface) consists of points at distance $r$ from $p$. The [exponential map](#exponential-map-riemannian-geometry) restricted to the radius-$r$ circle in $T_pS$ gives its smooth embedded parameterization. Outside the injectivity range a distance sphere need not be smooth.

###### Close geodesic circles intersect twice

↑ **Parent:** [Geodesic circle](#geodesic-circle)

Fix $p$ on a [Riemannian surface](#riemannian-surface). For sufficiently small $r>0$, the [geodesic circles](#geodesic-circle) of radius $r$ centered at $p$ and at every sufficiently nearby distinct $q$ meet transversally at exactly two points. In a strongly convex normal neighbourhood, write $q=\exp_p(\varepsilon v)$ and $x(\theta)=\exp_p(re(\theta))$. First variation gives

$$
\left.\partial_\varepsilon[d(q,x(\theta))^2-r^2]\right|_{\varepsilon=0}
=-2r\langle v,e(\theta)\rangle.
$$

The quotient of the bracketed function by $\varepsilon$ extends smoothly and has two simple zeros at zero. The [implicit function theorem](calculus.md#implicit-function-theorem), uniformly over unit $v$, preserves these two zeros and excludes others. The nonzero angular derivatives prove transversality. The distinct-centre hypothesis is essential: coincident circles are not transverse.

<h5 id="gauss-s-lemma-riemannian-geometry">Gauss's lemma (Riemannian geometry)</h5>

↑ **Parent:** [Geodesic polar coordinates](#geodesic-polar-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss's_lemma_(Riemannian_geometry))

The radial direction is orthogonal to the angular directions under the exponential map. On a surface this makes the first fundamental form in geodesic polar coordinates

$$
I=dr^2+G(r,\theta)\,d\theta^2,
\qquad
G=|\phi_\theta|^2,
$$

with $\sqrt{G(r,\theta)}/r\to1$ as $r\to0$.

###### Jacobi equation in geodesic polar coordinates

↑ **Parent:** [Gauss's lemma (Riemannian geometry)](#gauss-s-lemma-riemannian-geometry)

For $h(r,\theta)=\sqrt{G(r,\theta)}$, the angular [Jacobi field](general-relativity.md#jacobi-field) equation on a surface becomes

$$
h_{rr}+K(r,\theta)h=0,
\qquad h(0,\theta)=0,
\qquad h_r(0,\theta)=1.
$$

The [Riemannian area element](differential-geometry.md#area-element-of-a-surface) is $h(r,\theta)\,dr\,d\theta$.

###### One-dimensional Rauch comparison inequality

↑ **Parent:** [Jacobi equation in geodesic polar coordinates](#jacobi-equation-in-geodesic-polar-coordinates)

If $h''+Kh=0$, $h(0)=0$, $h'(0)=1$, $h>0$, and $K\leq C$ for $C>0$, then

$$
h(r)\geq\frac{\sin(\sqrt C r)}{\sqrt C}
\qquad(0\leq r<\pi/\sqrt C).
$$

Subtract a smaller multiple of the sine solution and use the monotonicity of its Wronskian with $h$.

###### Area of a geodesic polar ball with nonpositive curvature

↑ **Parent:** [Jacobi equation in geodesic polar coordinates](#jacobi-equation-in-geodesic-polar-coordinates)

If $K\leq0$, then $h_{rr}=-Kh\geq0$, so $h\geq r$. Every geodesic polar ball of radius $\varepsilon$ therefore satisfies

$$
\operatorname{Area}B(p,\varepsilon)\geq\pi\varepsilon^2.
$$

###### Area of a small geodesic polar ball under an upper curvature bound

↑ **Parent:** [Jacobi equation in geodesic polar coordinates](#jacobi-equation-in-geodesic-polar-coordinates)

If $K\leq C$ with $C>0$, scalar comparison gives

$$
h(r,\theta)\geq\frac{\sin(\sqrt C r)}{\sqrt C}
$$

before $\pi/\sqrt C$. Consequently

$$
\operatorname{Area}B(p,\varepsilon)
\geq\frac{2\pi}{C}\bigl(1-\cos(\sqrt C\varepsilon)\bigr)
=\pi\varepsilon^2(1+O(\varepsilon^2)).
$$

### Complete geodesic

↑ **Parent:** [Geodesic](#geodesic)

A geodesic is complete when its maximal affine parameter interval is all of $\mathbb R$.

#### Maximal geodesic

↑ **Parent:** [Complete geodesic](#complete-geodesic)

A geodesic $\gamma:I\to M$ is maximal when it has no geodesic extension to a strictly larger interval. Every initial position and velocity determine a unique maximal geodesic through the [geodesic equation](#geodesic-equation).

##### Extendible geodesic

↑ **Parent:** [Maximal geodesic](#maximal-geodesic)

An [extendible geodesic](#extendible-geodesic) is a [geodesic](#geodesic) segment that can be continued beyond at least one endpoint within the same manifold after retaining an [affine parameter](#affine-parameter). An artificial truncation at a regular event is extendible even when its continuation eventually reaches a singularity.

#### Geodesic completeness

↑ **Parent:** [Complete geodesic](#complete-geodesic)

A Riemannian manifold is geodesically complete when every maximal geodesic is defined for every real affine parameter, equivalently when every exponential map is defined on its entire tangent space.

##### Upward stability of Riemannian completeness

↑ **Parent:** [Geodesic completeness](#geodesic-completeness)

Pointwise domination of [Riemannian metrics](differential-geometry.md#riemannian-metric) gives domination of their distances. A Cauchy sequence for the larger distance is Cauchy for the complete smaller one. Smooth positive metrics induce the same manifold topology, so its limit is also a limit in the larger distance. The [Hopf-Rinow theorem](#hopf-rinow-theorem) turns metric completeness into [geodesic completeness](#geodesic-completeness). Mere positivity of the second metric, without domination, is insufficient.

##### Compact-core completeness for a Euclidean end

↑ **Parent:** [Geodesic completeness](#geodesic-completeness)

Suppose these sets exhaust a manifold, and its [Riemannian metric](differential-geometry.md#riemannian-metric) is Euclidean beyond some radius in the end coordinates. A finite-time [geodesic](#geodesic) has fixed speed and cannot increase its exterior radius faster than that speed. It remains in one [compact](topology.md#compact-space) core enlargement, with velocity in a [compact](topology.md#compact-space) disk bundle. The [geodesic](#geodesic) equation therefore continues beyond every finite parameter endpoint. The [compactness](topology.md#compact-space) hypothesis is substantive: the open exterior of a closed Euclidean ball, with empty core, is incomplete at its inner boundary despite having a [Euclidean metric](differential-geometry.md#euclidean-metric) at infinity.

##### Geodesic incompleteness

↑ **Parent:** [Geodesic completeness](#geodesic-completeness)

A Riemannian manifold is geodesically incomplete when some [maximal geodesic](#maximal-geodesic) has a finite endpoint in its affine-parameter interval.

###### Curvature-blowup criterion for inextendibility of a surface

↑ **Parent:** [Geodesic incompleteness](#geodesic-incompleteness)

Let $S\subset\mathbb R^3$ be a smooth surface. Suppose its [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) tends to infinity in absolute value along every [maximal geodesic](#maximal-geodesic) with a finite affine-parameter endpoint. Then $S$ is an [inextendible embedded surface](differential-geometry.md#inextendible-embedded-surface): a smooth extension would let some geodesic reach the extension boundary in finite time while its curvature remained locally bounded.

###### Incomplete surface z equals r to three halves

↑ **Parent:** [Curvature-blowup criterion for inextendibility of a surface](#curvature-blowup-criterion-for-inextendibility-of-a-surface)

The [surface of revolution](differential-geometry.md#surface-of-revolution)

$$
S=\{(r\cos\theta,r\sin\theta,r^{3/2}):r>0\}
$$

is [geodesically incomplete](#geodesic-incompleteness): a meridian reaches the missing origin in finite length. Its Gaussian curvature, computed using the [curvatures of a parametrized surface of revolution](differential-geometry.md#curvatures-of-a-parametrized-surface-of-revolution), is

$$
K(r)=\frac{9}{8r(1+9r/4)^2},
$$

which tends to infinity as $r\downarrow0$. Every finite-time endpoint of a constant-speed geodesic must approach the origin, the only finite point in the ambient closure missing from $S$, so this surface satisfies the curvature-blowup criterion.

##### Hopf-Rinow theorem

↑ **Parent:** [Geodesic completeness](#geodesic-completeness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf–Rinow_theorem)

For a connected finite-dimensional [Riemannian manifold](#riemannian-manifold), completeness of the [Riemannian distance](#riemannian-distance), [geodesic completeness](#geodesic-completeness), and [compactness](topology.md#compact-space) of every closed bounded subset are equivalent. These conditions imply that any two points are joined by a [minimizing geodesic](#minimizing-geodesic). Pairwise existence of [minimizing geodesics](#minimizing-geodesic) alone does not imply completeness: an open [Euclidean ball](functional-analysis.md#euclidean-ball) is incomplete, yet the [line segment](mathematical-optimization.md#line-segment) between any two of its points stays in the ball and minimizes length.

###### Hopf-Rinow lemma

↑ **Parent:** [Hopf-Rinow theorem](#hopf-rinow-theorem)

If the [Riemannian exponential map](#exponential-map-riemannian-geometry) at one point $p$ of a connected finite-dimensional [Riemannian manifold](#riemannian-manifold) is defined on all of $T_pM$, every point can be joined to $p$ by a [minimizing geodesic](#minimizing-geodesic). The [distance splitting through a small geodesic sphere](#distance-splitting-through-a-small-geodesic-sphere) selects a radial direction attaining $d(p,q)=r+d(\gamma(r),q)$. If this equality stopped before the target, repeat the splitting at its last point. A broken minimizing path cannot have a corner, so the new segment continues the same [geodesic](#geodesic), contradicting maximality. This is the minimizing-geodesic lemma used in the [radial continuation proof of Hopf-Rinow](#radial-continuation-proof-of-hopf-rinow).

// Target: riemannian-geometry.bigb

###### Radial continuation proof of Hopf-Rinow

↑ **Parent:** [Hopf-Rinow theorem](#hopf-rinow-theorem)

Assume [geodesic completeness](#geodesic-completeness). Minimize the distance to a target over a small [compact](topology.md#compact-space) [geodesic sphere](#geodesic-sphere) about the initial point. The [distance splitting through a small geodesic sphere](#distance-splitting-through-a-small-geodesic-sphere) gives an initial direction satisfying $d(p,\gamma(t))+d(\gamma(t),q)=d(p,q)$. If this equality stops before the target, repeat the splitting at the last equality point. The resulting broken path minimizes, so its corner must smooth into the same continuing [geodesic](#geodesic), a contradiction. This supplies a [minimizing geodesic](#minimizing-geodesic) to every target. Every closed metric ball is then the image under the [Riemannian exponential map](#exponential-map-riemannian-geometry) of a closed tangent ball, hence [compact](topology.md#compact-space). A [Cauchy sequence](real-analysis.md#cauchy-sequence) has a convergent subsequence in such a ball and therefore converges, proving metric completeness without presupposing a global minimizing [curve](topology.md#curve).

### Line in a Riemannian manifold

↑ **Parent:** [Geodesic](#geodesic)

A line is a unit-speed geodesic $\gamma:\mathbb R\to M$ that minimizes between every two of its points: $d_g(\gamma(s),\gamma(t))=|s-t|$.

This is a globally [minimizing geodesic](#minimizing-geodesic), a Riemannian specialization of the general geometric line notion.

#### Disconnected at infinity

↑ **Parent:** [Line in a Riemannian manifold](#line-in-a-riemannian-manifold)

A connected noncompact manifold is disconnected at infinity when the complement of some compact subset has at least two unbounded connected components. Equivalently, it has at least two ends.

The relevant general concept is an [End](topology.md#end-topology); having several ends is a property of the space, not a synonym for one end.

##### A line from disconnection at infinity

↑ **Parent:** [Disconnected at infinity](#disconnected-at-infinity)

A connected complete [Riemannian manifold](#riemannian-manifold) that is [disconnected at infinity](#disconnected-at-infinity) contains a [line in a Riemannian manifold](#line-in-a-riemannian-manifold). Choose points escaping in two components outside a fixed compact set and join them by [minimizing geodesics](#minimizing-geodesic). Each segment crosses the compact set. Parametrize from a crossing point; both parameter endpoints tend to infinity in opposite directions. Compactness of the unit tangent vectors over the crossing set gives a subsequence converging to an entire [geodesic](#geodesic). Every finite subsegment is minimizing by continuity of distance, so the limit is a line.

### Tangency invariance of an ambient-surface geodesic

↑ **Parent:** [Geodesic](#geodesic)

If two embedded surfaces are tangent along a curve, their tangent planes agree there. The curve's ambient acceleration is normal to one surface exactly when it is normal to the other, so it is a geodesic of one exactly when it is a geodesic of the other.

#### Cylindrical-helix tangency construction

↑ **Parent:** [Tangency invariance of an ambient-surface geodesic](#tangency-invariance-of-an-ambient-surface-geodesic)

A circular helix on a circular cylinder has radial ambient acceleration and is therefore a geodesic. Any surface tangent to the cylinder along that helix has the same curve as a geodesic.

## Energy of a curve

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)

The energy of a curve is one half the integral of its squared speed.

### Fixed-endpoint variation of a curve

↑ **Parent:** [Energy of a curve](#energy-of-a-curve)

A fixed-endpoint variation of a [curve](topology.md#curve) $\gamma:[a,b]\to S$ is a smooth family $\Gamma(s,t)$ with $\Gamma(0,t)=\gamma(t)$, $\Gamma(s,a)=\gamma(a)$ and $\Gamma(s,b)=\gamma(b)$. Its [variation vector field](#variation-vector-field) $V(t)=\partial_s\Gamma(0,t)$ vanishes at the endpoints. Consequently integration by parts in the first variation of [energy of a curve](#energy-of-a-curve) has no boundary contribution, and stationarity is characterized by the [geodesic equation](#geodesic-equation).

### First variation of geodesic energy

↑ **Parent:** [Energy of a curve](#energy-of-a-curve)

For $E(\gamma)=\tfrac12\int_0^1|\dot\gamma|^2dt$ and [variation vector field](#variation-vector-field) $V$, the first variation is $[\langle V,\dot\gamma\rangle]_0^1-\int_0^1\langle V,D_t\dot\gamma\rangle dt$. For fixed endpoints the boundary term vanishes, so the [critical points](analysis.md#critical-point) of the energy are exactly affinely parametrized [geodesics](#geodesic).

### Variation vector field

↑ **Parent:** [Energy of a curve](#energy-of-a-curve)

For a variation $F(s,t)$ of a curve $\gamma(t)=F(0,t)$, the variation vector field is $V(t)=\partial_sF(0,t)$. A fixed-endpoint variation has $V=0$ at both endpoints.

#### Riemannian index form

↑ **Parent:** [Variation vector field](#variation-vector-field)

Along a geodesic $\gamma$ with tangent $T$, the index form on endpoint-vanishing vector fields is

$$
I(V,W)=\int\bigl(\langle D_tV,D_tW\rangle-\langle R(V,T)T,W\rangle\bigr)dt.
$$

##### Riccati factorization of the Riemannian index form

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

In a parallel orthonormal frame along a [geodesic](#geodesic), write the [Jacobi equation](calculus-of-variations.md#jacobi-equation) as $A''+KA=0$, with $A(0)=0$, $A'(0)=I$ and symmetric $K$. In the absence of [conjugate points](#conjugate-points) on $(0,b]$, $A$ is invertible there. The conserved quantity $A^TA'-A'^TA=0$ makes $S=A'A^{-1}$ symmetric, and $S'+S^2+K=0$. For a field $u$ vanishing at both endpoints,

$$
I(u,u)=\int_0^b|u'-Su|^2\,dt.
$$

Indeed the difference of the integrands is $(u^TSu)'$; its boundary value at zero vanishes because $S=t^{-1}I+O(t)$ and $u=O(t)$. Equality forces $u=Ac$ and then $A(b)c=0$, so $u=0$. This proves strict positivity and the minimizing property of the [Jacobi field](general-relativity.md#jacobi-field) with prescribed endpoint values.

// Target: riemannian-geometry.bigb

##### Jacobi fields form the radical of the fixed-endpoint index form

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

On continuous piecewise smooth [vector field along a curve](fiber-bundle.md#vector-field-along-a-curve) with zero endpoints, the [radical of a bilinear form](linear-algebra.md#radical-of-a-bilinear-form) of the [Riemannian index form](#riemannian-index-form) is exactly the space of endpoint-vanishing [Jacobi fields](general-relativity.md#jacobi-field). Integration by parts against tests supported inside each smooth piece gives the [Jacobi equation](calculus-of-variations.md#jacobi-equation); tests with arbitrary values at breakpoints force continuity of the covariant derivative, hence a global smooth [Jacobi field](general-relativity.md#jacobi-field). This characterization uses $I(V,W)=0$ for every test field $W$, not merely $I(V,V)=0$, which is insufficient for an indefinite form.

// Target: riemannian-geometry.bigb

##### Conjugate-point criterion for the Riemannian index form

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

On continuous piecewise smooth perpendicular fields with zero endpoints, the [Riemannian index form](#riemannian-index-form) is nonnegative exactly when no point strictly inside the [geodesic](#geodesic) segment is conjugate to its initial point. It is positive on every nonzero field exactly when no [conjugate point](calculus-of-variations.md#conjugate-point) occurs up to and including the final endpoint. At a first conjugate endpoint its nullspace consists of the endpoint-vanishing [Jacobi fields](general-relativity.md#jacobi-field). These statements distinguish nonnegative quadratic forms from strictly positive ones and do not assume global minimization.

###### Loss of geodesic minimality beyond a conjugate point

↑ **Parent:** [Conjugate-point criterion for the Riemannian index form](#conjugate-point-criterion-for-the-riemannian-index-form)

Let a nonzero [Jacobi field](general-relativity.md#jacobi-field) $J$ vanish at times zero and $a$. On a longer [geodesic](#geodesic) segment ending at $b>a$, extend it by zero to a continuous piecewise smooth field $Z$. Then $I(Z,Z)=0$. Choose an endpoint-vanishing field $P$ with $P(a)=-D_tJ(a)$; [integration by parts](calculus.md#integration-by-parts) gives $I(Z,P)=-|D_tJ(a)|^2<0$. Thus $I(Z+\varepsilon P,Z+\varepsilon P)<0$ for small positive $\varepsilon$. Smooth approximation preserves negativity. The [second variation of geodesic energy](#second-variation-of-geodesic-energy) supplies a shorter path, so a [minimizing geodesic](#minimizing-geodesic) cannot extend beyond its first [conjugate point](calculus-of-variations.md#conjugate-point).

// Target: differential-geometry.bigb

##### Sine index-form bound for positive Ricci curvature

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

Along a unit-speed [minimizing geodesic](#minimizing-geodesic) of positive length $L$, take perpendicular parallel orthonormal fields $E_i$ and set $V_i=\sin(\pi t/L)E_i$. The [second variation of geodesic energy](#second-variation-of-geodesic-energy) makes each index form nonnegative, while $\operatorname{Ric}\geq(n-1)\kappa g$ bounds their sum as displayed. For $n\geq2$ and $\kappa>0$, lengths greater than $\pi/\sqrt\kappa$ are impossible. Completeness is what supplies a [minimizing geodesic](#minimizing-geodesic) between arbitrary points in the [Bonnet-Myers theorem](second-fundamental-form.md#myers-s-theorem).

##### Second variation of geodesic energy

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

For $E=\tfrac12\int|\dot\gamma|^2$ and a geodesic base curve, a variation field $V$ satisfies

$$
E''(0)=[\langle\nabla_sV,\dot\gamma\rangle]_a^b+
\int_a^b\left(|\nabla_tV|^2-\langle R(V,\dot\gamma)\dot\gamma,V\rangle\right)dt.
$$

The endpoint term vanishes for fixed endpoints and for periodic variations of closed geodesics. The integral is the [Riemannian index form](#riemannian-index-form). This uses the [Levi-Civita connection](general-relativity.md#levi-civita-connection) and the convention $R(X,Y)=\nabla_X\nabla_Y-\nabla_Y\nabla_X-\nabla_{[X,Y]}$.

###### Instability of a closed geodesic in positive even-dimensional curvature

↑ **Parent:** [Second variation of geodesic energy](#second-variation-of-geodesic-energy)

On an oriented even-dimensional [Riemannian manifold](#riemannian-manifold) of strictly positive [sectional curvature](second-fundamental-form.md#sectional-curvature), a nonconstant closed geodesic has a length-decreasing smooth variation. Its [parallel transport](fiber-bundle.md#parallel-transport) fixes the tangent and acts on the odd-dimensional normal space by a [special orthogonal group](linear-algebra.md#special-orthogonal-group) element. An [odd-dimensional special orthogonal transformation has a fixed vector](linear-algebra.md#odd-dimensional-special-orthogonal-transformation-has-a-fixed-vector), so there is a nonzero periodic parallel normal field $V$. The [second variation of geodesic energy](#second-variation-of-geodesic-energy) is then strictly negative. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) converts lower energy into strictly lower length because the original geodesic has constant speed. For an embedded geodesic the small variation is a [smooth isotopy](differential-geometry.md#smooth-isotopy); otherwise it is a deformation through immersed loops.

##### Second variation of Riemannian arc length

↑ **Parent:** [Riemannian index form](#riemannian-index-form)

For a unit-speed geodesic and a fixed-endpoint variation, the second variation of length is the index form of the normal component of its variation vector field.

###### Moving-endpoint second variation of Riemannian arc length

↑ **Parent:** [Second variation of Riemannian arc length](#second-variation-of-riemannian-arc-length)

For a variation of a unit-speed [geodesic](#geodesic), let $T$ be its tangent, $J$ its [variation vector field](#variation-vector-field) and $A=\nabla_sJ$ its variation acceleration. The [second variation of Riemannian arc length](#second-variation-of-riemannian-arc-length) has the displayed endpoint term in addition to the [Riemannian index form](#riemannian-index-form) of $J^\perp=J-\langle J,T\rangle T$. Differentiating the speed twice gives $|D_tJ|^2-\langle D_tJ,T\rangle^2+\langle D_sD_tJ,T\rangle$. Commuting derivatives and integrating $D_tA$ by parts gives the formula. The term cannot be discarded unless the endpoints are fixed or an appropriate endpoint condition makes it zero.

## Christoffel symbol

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Christoffel_symbol)

In a coordinate frame, the Levi-Civita connection is determined by

$$
\nabla_{\partial_i}\partial_j=\Gamma^k_{ij}\partial_k.
$$

The coefficients $\Gamma^k_{ij}$ are the Christoffel symbols. They are not the components of a tensor because a coordinate change contributes second derivatives.

### Christoffel trace identity

↑ **Parent:** [Christoffel symbol](#christoffel-symbol)

For a nondegenerate [metric tensor](general-relativity.md#metric-tensor) and its [Levi-Civita connection](general-relativity.md#levi-civita-connection), contracting the [Christoffel symbol](#christoffel-symbol) formula gives $\Gamma^\rho{}_{\rho\mu}=\tfrac12g^{ab}\partial_\mu g_{ab}$. The [Jacobi determinant derivative formula](linear-algebra.md#jacobi-determinant-derivative-formula) identifies this with $\partial_\mu\log\sqrt{|\det g|}$. The volume density, rather than the determinant without an absolute value, works in every fixed metric signature.

### Christoffel symbols of a diagonal spherical spacetime metric

↑ **Parent:** [Christoffel symbol](#christoffel-symbol)

For

$$
ds^2=-\lambda(t,r)^2dt^2+\mu(t,r)^2dr^2
+r^2d\theta^2+r^2\sin^2\theta\,d\phi^2,
$$

write dots and primes for $t$- and $r$-derivatives. Up to symmetry in the lower indices, the nonzero connection coefficients are

$$
\begin{gathered}
\Gamma^t_{tt}=\dot\lambda/\lambda,
\quad \Gamma^t_{tr}=\lambda'/\lambda,
\quad \Gamma^t_{rr}=\mu\dot\mu/\lambda^2,\\
\Gamma^r_{tt}=\lambda\lambda'/\mu^2,
\quad \Gamma^r_{tr}=\dot\mu/\mu,
\quad \Gamma^r_{rr}=\mu'/\mu,\\
\Gamma^r_{\theta\theta}=-r/\mu^2,
\quad \Gamma^r_{\phi\phi}=-r\sin^2\theta/\mu^2,\\
\Gamma^\theta_{r\theta}=1/r,
\quad \Gamma^\theta_{\phi\phi}=-\sin\theta\cos\theta,
\quad \Gamma^\phi_{r\phi}=1/r,
\quad \Gamma^\phi_{\theta\phi}=\cot\theta.
\end{gathered}
$$

## Geodesic equation

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geodesic_equation)

A geodesic has zero covariant acceleration and in coordinates satisfies $\ddot u^k+\Gamma^k_{ij}\dot u^i\dot u^j=0$.

### Geodesic coordinate grid

↑ **Parent:** [Geodesic equation](#geodesic-equation)

For a surface metric $E\,du^2+2F\,du\,dv+G\,dv^2$, all coordinate curves are unparametrized [geodesics](#geodesic) precisely when the displayed identities hold. Parametrize $u=c$ by [arc length](#arc-length), so $\dot v=G^{-1/2}$, and substitute into the transverse [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) for [energy of a curve](#energy-of-a-curve). This gives the first identity; $v=d$ gives the second. These identities concern geodesic images and do not assert that the coordinate variable itself is an affine parameter.

#### Constant-angle geodesic coordinate grids are locally flat

↑ **Parent:** [Geodesic coordinate grid](#geodesic-coordinate-grid)

If the oriented coordinate tangent vectors meet at a constant [angle](geometry-and-topology.md#angle) with cosine $k$, the [first fundamental form](differential-geometry.md#first-fundamental-form) has $F=k\sqrt{EG}$. The [geodesic coordinate grid](#geodesic-coordinate-grid) identities reduce to $k(\sqrt E)_v=(\sqrt G)_u$ and $k(\sqrt G)_u=(\sqrt E)_v$. Since positive definiteness gives $|k|<1$, both derivatives vanish. Thus $E=E(u)$ and $G=G(v)$ locally. Changing coordinates to $U=\int\sqrt E\,du$ and $V=\int\sqrt G\,dv$ gives the constant metric $dU^2+2k\,dU\,dV+dV^2$. It is locally Euclidean after a linear change of coordinates, hence has zero [Gaussian curvature](second-fundamental-form.md#gaussian-curvature).

// Target: geometry-and-topology.bigb

### Unparametrized geodesic equation

↑ **Parent:** [Geodesic equation](#geodesic-equation)

A regular curve with tangent $v=dx/du$ is an unparametrized [geodesic](#geodesic) of an [affine connection](fiber-bundle.md#affine-connection) if $\nabla_vv=f(u)v$. Choose a new parameter $s$ with $ds/du=r(u)>0$ and $r'/r=f$. Then $w=dx/ds=v/r$ obeys $\nabla_ww=r^{-2}(\nabla_vv-(r'/r)v)=0$. Conversely a reparametrized affine geodesic has acceleration proportional to its tangent. This criterion concerns the geometric curve, not a fixed parametrization.

#### Timelike length and energy have the same geodesic images

↑ **Parent:** [Unparametrized geodesic equation](#unparametrized-geodesic-equation)

For a [Lorentzian metric](general-relativity.md#lorentzian-metric) and timelike $v=dx/du$, put $L=\sqrt{-g(v,v)}>0$ and $\mathscr L=L^2/2$. The [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) of $\mathscr L$ give $\nabla_vv=0$, while those of $L$ give $\nabla_vv=(\dot L/L)v$. Taking $ds/du=L$ removes the latter tangential acceleration and gives a unit timelike tangent. Thus the two actions have the same geodesic images; the quadratic action singles out an [affine parameter](#affine-parameter). They do not have the same solutions for an arbitrary fixed parameter: $t=u^2$, $\mathbf x=0$, $u>0$, in [Minkowski spacetime](special-relativity.md#minkowski-spacetime) solves the length equation but not the energy equation. Null curves are excluded since $L=0$.

### Geodesic Lagrangian

↑ **Parent:** [Geodesic equation](#geodesic-equation)

For a metric $g_{ij}$, the Lagrangian $L=g_{ij}\dot x^i\dot x^j/2$ has the affinely parametrized geodesic equations as its Euler-Lagrange equations. Its value is half the constant squared norm of the tangent.

### Ambient acceleration criterion for a surface geodesic

↑ **Parent:** [Geodesic equation](#geodesic-equation)

For a smoothly parametrized curve on an embedded surface in Euclidean space, the geodesic equations hold exactly when the ambient acceleration is normal to the surface.

#### Constant speed of an affinely parametrized geodesic

↑ **Parent:** [Ambient acceleration criterion for a surface geodesic](#ambient-acceleration-criterion-for-a-surface-geodesic)

The velocity of a surface curve is tangent. If its acceleration is normal, then

$$
\frac d{dt}|\dot\gamma|^2=2\dot\gamma\mathbin{\cdot}\ddot\gamma=0,
$$

so every affinely parametrized geodesic has constant speed.

### Normal section of a surface

↑ **Parent:** [Geodesic equation](#geodesic-equation)

A constant-speed intersection with a plane containing every surface normal along the curve is a geodesic.

### Affine parameter

↑ **Parent:** [Geodesic equation](#geodesic-equation)

An affine parameter on a geodesic is one for which the coordinate equation has the form $\ddot x^k+\Gamma^k_{ij}\dot x^i\dot x^j=0$. Its affine changes $\lambda\mapsto A\lambda+B$, with $A\ne0$, preserve this form.

## Geodesic polygon

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)

A geodesic polygon is a closed polygonal curve whose sides are [geodesic segments](#geodesic-segment). A [geodesic triangle](#geodesic-triangle) has three sides. Surface angle excess is governed by the [Gauss-Bonnet theorem](differential-geometry.md#gauss-bonnet-theorem).

<h2 id="schur-s-lemma-riemannian-geometry">Schur's lemma (Riemannian geometry)</h2>

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur's_lemma_(Riemannian_geometry))

On a connected [Riemannian manifold](#riemannian-manifold) of dimension at least three, pointwise independence of [sectional curvature](second-fundamental-form.md#sectional-curvature) from the tangent two-plane forces the curvature to be constant. The contracted [Bianchi identity](fiber-bundle.md#bianchi-identity) differentiates the relation $\operatorname{Ric}=(n-1)Kg$ and gives $(n-2)dK=0$.

## Complete manifold

↑ **Parent:** [Riemannian geometry](riemannian-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_manifold)

A (pseudo-)[Riemannian manifold](#riemannian-manifold) is geodesically complete when every inextendible affinely parametrized [geodesic](#geodesic) is defined for all real parameter values. In the positive-definite case, the [Hopf-Rinow theorem](#hopf-rinow-theorem) identifies this with metric completeness. Null-only completeness in spacetime is a separate weaker condition.

## ↑ Ancestors (5)

1. [Differential geometry](differential-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Harmonic coordinate](numerical-relativity.md#harmonic-coordinate)
