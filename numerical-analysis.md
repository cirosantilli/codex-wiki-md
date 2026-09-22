# Numerical analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_analysis)

Numerical analysis studies algorithms for approximating mathematical problems and controlling their errors.

**Table of contents**

- [Newton root-finding iteration](#newton-root-finding-iteration)
  - [Newton iteration in a Banach space](#newton-iteration-in-a-banach-space)
    - [Frozen Newton correction for a fixed-point equation](#frozen-newton-correction-for-a-fixed-point-equation)
    - [Quadratic Newton error bound in a Banach space](#quadratic-newton-error-bound-in-a-banach-space)
  - [Monotone Newton convergence for a strictly convex function](#monotone-newton-convergence-for-a-strictly-convex-function)
- [Bisection method](#bisection-method)
- [Chord error bound](#chord-error-bound)
- [Interval arithmetic](#interval-arithmetic)
- [Continuation method](#continuation-method)
  - [Transversal surface intersection tracing](#transversal-surface-intersection-tracing)
    - [Transversal intersection of two parametric surfaces](#transversal-intersection-of-two-parametric-surfaces)
- [Computer aided geometric design](#computer-aided-geometric-design)
  - [Affine equivariance of a geometric basis](#affine-equivariance-of-a-geometric-basis)
  - [Translational penetration depth](#translational-penetration-depth)
  - [Linear precision of a geometric basis](#linear-precision-of-a-geometric-basis)
  - [Control point](#control-point)
    - [Control net](#control-net)
    - [Control polygon](#control-polygon)
  - [Apparent-gravity camera frame](#apparent-gravity-camera-frame)
  - [Subdivision curve](#subdivision-curve)
    - [Binary linear interpolatory subdivision](#binary-linear-interpolatory-subdivision)
    - [Functional precision set of a subdivision scheme](#functional-precision-set-of-a-subdivision-scheme)
    - [Chaikin subdivision](#chaikin-subdivision)
      - [Chaikin basis function](#chaikin-basis-function)
      - [Polynomial degree preservation under Chaikin subdivision](#polynomial-degree-preservation-under-chaikin-subdivision)
    - [Support of a stationary subdivision scheme](#support-of-a-stationary-subdivision-scheme)
    - [Subdivision curve interrogation](#subdivision-curve-interrogation)
      - [Closest-point search on a subdivision curve](#closest-point-search-on-a-subdivision-curve)
      - [Shadow tracing for a subdivision curve](#shadow-tracing-for-a-subdivision-curve)
      - [Recursive half-space clipping of a subdivision curve](#recursive-half-space-clipping-of-a-subdivision-curve)
  - [Subdivision surface](#subdivision-surface)
    - [Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface)
      - [Extrusion invariance of a ternary triangular scheme](#extrusion-invariance-of-a-ternary-triangular-scheme)
    - [Mid-edge subdivision](#mid-edge-subdivision)
      - [Mid-edge facet centroid invariance](#mid-edge-facet-centroid-invariance)
    - [Subdivision surface interrogation](#subdivision-surface-interrogation)
      - [Intersection of subdivision limit surfaces](#intersection-of-subdivision-limit-surfaces)
      - [Plane section of a subdivision surface](#plane-section-of-a-subdivision-surface)
      - [Minimum distance between subdivision bodies](#minimum-distance-between-subdivision-bodies)
    - [Extraordinary subdivision vertex](#extraordinary-subdivision-vertex)
      - [Characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface)
    - [Quincunx subdivision](#quincunx-subdivision)
    - [Loop subdivision surface](#loop-subdivision-surface)
      - [Polynomial generation by regular Loop subdivision](#polynomial-generation-by-regular-loop-subdivision)
      - [Extrusion invariance of Loop subdivision](#extrusion-invariance-of-loop-subdivision)
    - [Subdivision mask](#subdivision-mask)
      - [Subdivision mask width](#subdivision-mask-width)
      - [Subdivision arity](#subdivision-arity)
      - [Subdivision difference scheme](#subdivision-difference-scheme)
        - [Norm and spectral bounds for subdivision regularity](#norm-and-spectral-bounds-for-subdivision-regularity)
      - [Subdivision matrix](#subdivision-matrix)
  - [Bézier curve](#bezier-curve)
    - [Bézier derivative control polygon](#bezier-derivative-control-polygon)
      - [Parametric first-derivative join of Bézier curves](#parametric-first-derivative-join-of-bezier-curves)
    - [De Casteljau's algorithm](#de-casteljau-s-algorithm)
  - [Bounding volume](#bounding-volume)
    - [Bounding volume hierarchy](#bounding-volume-hierarchy)
    - [Axis-aligned bounding box](#axis-aligned-bounding-box)
  - [Triangle-triangle intersection algorithm](#triangle-triangle-intersection-algorithm)
- [Round-off error](#round-off-error)
- [Richardson extrapolation](#richardson-extrapolation)
- [Error control for ODE solvers](#error-control-for-ode-solvers)
  - [Adaptive step-size controller](#adaptive-step-size-controller)
  - [Absolute and relative error tolerances](#absolute-and-relative-error-tolerances)
  - [Local error estimator](#local-error-estimator)
    - [Predictor-corrector error estimation](#predictor-corrector-error-estimation)
    - [Embedded Runge-Kutta pair](#embedded-runge-kutta-pair)
    - [Step-doubling error estimation](#step-doubling-error-estimation)
- [Finite volume method](#finite-volume-method)
  - [Monotone conservative scheme](#monotone-conservative-scheme)
    - [Total variation diminishing scheme](#total-variation-diminishing-scheme)
    - [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme)
    - [Engquist-Osher method](#engquist-osher-method)
      - [CFL necessity for explicit Engquist-Osher stability](#cfl-necessity-for-explicit-engquist-osher-stability)
      - [Engquist-Osher flux](#engquist-osher-flux)
        - [Sonic-point splitting of a convex Engquist-Osher flux](#sonic-point-splitting-of-a-convex-engquist-osher-flux)
  - [Numerical flux](#numerical-flux)
    - [Godunov numerical flux](#godunov-numerical-flux)
- [Interval bisection](#interval-bisection)
- [Implicit time-stepping method](#implicit-time-stepping-method)
- [Multigrid method](#multigrid-method)
  - [Full multigrid](#full-multigrid)
  - [Two-grid Poisson factor with weighted Jacobi](#two-grid-poisson-factor-with-weighted-jacobi)
  - [Geometric multigrid V-cycle](#geometric-multigrid-v-cycle)
  - [Full-weighting restriction](#full-weighting-restriction)
  - [Coarse-grid correction](#coarse-grid-correction)
    - [Galerkin coarse-grid operator](#galerkin-coarse-grid-operator)
- [Convergence of a numerical method](#convergence-of-a-numerical-method)
  - [Quadratic convergence](#quadratic-convergence)
- [Global discretization error](#global-discretization-error)
  - [Variable-step global ODE error bound](#variable-step-global-ode-error-bound)
  - [Residual bound for global ODE error](#residual-bound-for-global-ode-error)
- [Midpoint quadrature rule](#midpoint-quadrature-rule)
- [Truncation error](#truncation-error)
- [Spectral method](#spectral-method)
  - [Spectral accuracy](#spectral-accuracy)
  - [Fourier spectral method](#fourier-spectral-method)
    - [Spectral truncation](#spectral-truncation)
    - [Fourier spectral system for a cosine-modulated second derivative](#fourier-spectral-system-for-a-cosine-modulated-second-derivative)
    - [Fourier–Galerkin method](#fourier-galerkin-method)
- [Stability of a numerical method](#stability-of-a-numerical-method)
- [Consistency of a numerical method](#consistency-of-a-numerical-method)
  - [Order of a numerical method](#order-of-a-numerical-method)
    - [Local truncation error](#local-truncation-error)
      - [Normalized local truncation error](#normalized-local-truncation-error)
- [Energy method](#energy-method)
  - [Dirichlet convection-diffusion contraction](#dirichlet-convection-diffusion-contraction)
  - [Periodic centered advection-diffusion contractivity](#periodic-centered-advection-diffusion-contractivity)
  - [Centered Dirichlet drift-diffusion energy identity](#centered-dirichlet-drift-diffusion-energy-identity)
  - [Energy stability for variable-coefficient reaction diffusion](#energy-stability-for-variable-coefficient-reaction-diffusion)
  - [Uniqueness of Sobolev weak solutions of a wave equation](#uniqueness-of-sobolev-weak-solutions-of-a-wave-equation)
- [Finite element method](#finite-element-method)
  - [Semidiscrete finite element heat equation](#semidiscrete-finite-element-heat-equation)
    - [Forward Euler limit for a consistent hat mass matrix](#forward-euler-limit-for-a-consistent-hat-mass-matrix)
  - [Finite element](#finite-element)
  - [Conforming finite element space](#conforming-finite-element-space)
  - [Finite element mesh](#finite-element-mesh)
    - [Shape-regular mesh](#shape-regular-mesh)
  - [Finite element interpolation estimate](#finite-element-interpolation-estimate)
  - [Mass matrix](#mass-matrix)
    - [Mass eigenstate](#mass-eigenstate)
    - [Affine-weighted hat mass matrix](#affine-weighted-hat-mass-matrix)
  - [Stiffness matrix](#stiffness-matrix)
    - [Reaction-diffusion finite element matrix](#reaction-diffusion-finite-element-matrix)
  - [Energy conservation for semidiscrete Galerkin advection](#energy-conservation-for-semidiscrete-galerkin-advection)
  - [Cubic Hermite finite element](#cubic-hermite-finite-element)
  - [Rayleigh-Ritz method](#rayleigh-ritz-method)
    - [Ritz-Galerkin equivalence for a symmetric coercive form](#ritz-galerkin-equivalence-for-a-symmetric-coercive-form)
      - [Symmetry and coercivity in quadratic energy minimization](#symmetry-and-coercivity-in-quadratic-energy-minimization)
    - [Energy norm](#energy-norm)
  - [Galerkin orthogonality](#galerkin-orthogonality)
    - [Céa's lemma](#cea-s-lemma)
      - [Aubin–Nitsche duality argument](#aubin-nitsche-duality-argument)
  - [Piecewise-linear hat function](#piecewise-linear-hat-function)
- [Arithmetic operation](#arithmetic-operation)
- [Schur stability criterion](#schur-stability-criterion)
  - [Complex quadratic Schur criterion](#complex-quadratic-schur-criterion)
- [Lie product formula](#lie-product-formula)
  - [Exponential product defect identity](#exponential-product-defect-identity)
    - [Decaying bound for symmetric negative matrix splitting](#decaying-bound-for-symmetric-negative-matrix-splitting)
  - [Symmetrized exponential-splitting defect identity](#symmetrized-exponential-splitting-defect-identity)
  - [Lie-Trotter splitting commutator error](#lie-trotter-splitting-commutator-error)
  - [First-order unitary product-formula error bound](#first-order-unitary-product-formula-error-bound)
- [Strang splitting](#strang-splitting)
  - [Strang splitting contraction for symmetric diffusion and skew advection](#strang-splitting-contraction-for-symmetric-diffusion-and-skew-advection)
  - [Higher-order composition of a symmetric splitting](#higher-order-composition-of-a-symmetric-splitting)
- [Composite midpoint rule error](#composite-midpoint-rule-error)
  - [Quadratic substitution for a square-root endpoint singularity](#quadratic-substitution-for-a-square-root-endpoint-singularity)
- [Polynomial interpolation](#polynomial-interpolation)
  - [Interpolation polynomial](#interpolation-polynomial)
  - [Interpolation nodes from best uniform approximation](#interpolation-nodes-from-best-uniform-approximation)
  - [Interpolation node](#interpolation-node)
  - [Lagrange polynomial](#lagrange-polynomial)
    - [Differentiation weights from nodal evaluations](#differentiation-weights-from-nodal-evaluations)
    - [Discrete minimax interpolation on ordered nodes](#discrete-minimax-interpolation-on-ordered-nodes)
    - [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)
      - [Endpoint derivative signs of Lagrange cardinal polynomials](#endpoint-derivative-signs-of-lagrange-cardinal-polynomials)
      - [Nodal derivative norm from Lagrange cardinal polynomials](#nodal-derivative-norm-from-lagrange-cardinal-polynomials)
  - [Divided difference](#divided-difference)
    - [Omitted-node identities for divided differences](#omitted-node-identities-for-divided-differences)
    - [Exponential divided difference](#exponential-divided-difference)
    - [Leibniz rule for divided differences](#leibniz-rule-for-divided-differences)
    - [Newton polynomial](#newton-polynomial)
- [Discrete Fourier transform](#discrete-fourier-transform)
  - [Prime Fourier matrix minor theorem](#prime-fourier-matrix-minor-theorem)
  - [Finite-field discrete Fourier transform](#finite-field-discrete-fourier-transform)
  - [Discrete Parseval identity](#discrete-parseval-identity)
  - [Fourier representation of a Kronecker delta](#fourier-representation-of-a-kronecker-delta)
  - [Fourier frequency](#fourier-frequency)
  - [Inverse discrete Fourier transform](#inverse-discrete-fourier-transform)
  - [Discrete Fourier mode](#discrete-fourier-mode)
  - [Cooley-Tukey FFT algorithm](#cooley-tukey-fft-algorithm)
    - [FFT butterfly](#fft-butterfly)
    - [Even--odd fast Fourier transform recursion](#even-odd-fast-fourier-transform-recursion)
  - [Discrete cosine transform](#discrete-cosine-transform)
    - [Discrete cosine transform from an even-reflected discrete Fourier transform](#discrete-cosine-transform-from-an-even-reflected-discrete-fourier-transform)
  - [Discrete sine transform](#discrete-sine-transform)
    - [Discrete sine transform Poisson solver](#discrete-sine-transform-poisson-solver)
    - [Discrete sine transform from a sign-modulated discrete cosine transform](#discrete-sine-transform-from-a-sign-modulated-discrete-cosine-transform)
- [Gershgorin circle theorem](#gershgorin-circle-theorem)
  - [Gershgorin disc](#gershgorin-disc)
  - [Gershgorin stability bound for a variable-coefficient diffusion stencil](#gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil)
- [Finite difference](finite-difference.md)
  - [Three-point asymmetric second-derivative formula](finite-difference.md#three-point-asymmetric-second-derivative-formula)
  - [Randomized symmetric finite-difference derivative estimator](finite-difference.md#randomized-symmetric-finite-difference-derivative-estimator)
  - [Finite difference method](finite-difference.md#finite-difference-method)
    - [Midpoint flux stencil for one-dimensional diffusion](finite-difference.md#midpoint-flux-stencil-for-one-dimensional-diffusion)
    - [Finite difference coefficient](finite-difference.md#finite-difference-coefficient)
    - [Fourth-order two-step advection stencil](finite-difference.md#fourth-order-two-step-advection-stencil)
    - [Mehrstellen method](finite-difference.md#mehrstellen-method)
      - [Compact semidiscrete nine-point diffusion](finite-difference.md#compact-semidiscrete-nine-point-diffusion)
    - [Rational implicit advection stencil with exact shift exceptions](finite-difference.md#rational-implicit-advection-stencil-with-exact-shift-exceptions)
    - [Centered discrete advection is skew-adjoint](finite-difference.md#centered-discrete-advection-is-skew-adjoint)
    - [Positive definiteness of the grounded nine-point Poisson stencil](finite-difference.md#positive-definiteness-of-the-grounded-nine-point-poisson-stencil)
    - [Implicit advection scheme with exact integer shifts](finite-difference.md#implicit-advection-scheme-with-exact-integer-shifts)
    - [Lax-Friedrichs method](finite-difference.md#lax-friedrichs-method)
    - [L2-compatible initialization of grid data](finite-difference.md#l2-compatible-initialization-of-grid-data)
      - [Cell-average projection](finite-difference.md#cell-average-projection)
    - [Discrete summation by parts](finite-difference.md#discrete-summation-by-parts)
      - [Inflow advection energy estimate from summation by parts](finite-difference.md#inflow-advection-energy-estimate-from-summation-by-parts)
    - [Four-neighbour mean expansion](finite-difference.md#four-neighbour-mean-expansion)
    - [Parabolic mesh refinement](finite-difference.md#parabolic-mesh-refinement)
    - [Lax-Wendroff advection scheme](finite-difference.md#lax-wendroff-advection-scheme)
    - [Symmetric half-grid diffusion consistency](finite-difference.md#symmetric-half-grid-diffusion-consistency)
      - [Monotone half-grid diffusion update](finite-difference.md#monotone-half-grid-diffusion-update)
    - [Upwind finite difference scheme](finite-difference.md#upwind-finite-difference-scheme)
      - [Dissipative second-order forward advection stencil](finite-difference.md#dissipative-second-order-forward-advection-stencil)
    - [Five-point Laplacian](finite-difference.md#five-point-laplacian)
      - [Unweighted grid error for the five-point Poisson formula](finite-difference.md#unweighted-grid-error-for-the-five-point-poisson-formula)
      - [Five-point heat-reaction stability threshold](finite-difference.md#five-point-heat-reaction-stability-threshold)
    - [Nine-point finite-difference stencil](finite-difference.md#nine-point-finite-difference-stencil)
      - [Five-point versus nine-point Laplacian eigenvalue accuracy](finite-difference.md#five-point-versus-nine-point-laplacian-eigenvalue-accuracy)
      - [Harmonic superconvergence of the nine-point stencil](finite-difference.md#harmonic-superconvergence-of-the-nine-point-stencil)
      - [Compact fourth-order Helmholtz stencil](finite-difference.md#compact-fourth-order-helmholtz-stencil)
      - [Jacobi convergence for the nine-point Dirichlet stencil](finite-difference.md#jacobi-convergence-for-the-nine-point-dirichlet-stencil)
      - [Negative definiteness of a nine-point Dirichlet stencil](finite-difference.md#negative-definiteness-of-a-nine-point-dirichlet-stencil)
      - [Fourth-order correction of the nine-point Poisson stencil](finite-difference.md#fourth-order-correction-of-the-nine-point-poisson-stencil)
        - [Sixth-order source correction of the nine-point Poisson stencil](finite-difference.md#sixth-order-source-correction-of-the-nine-point-poisson-stencil)
        - [Maximum-norm convergence of the corrected nine-point Poisson scheme](finite-difference.md#maximum-norm-convergence-of-the-corrected-nine-point-poisson-scheme)
    - [Fourier stability analysis](finite-difference.md#fourier-stability-analysis)
      - [Fourier amplification symbol](finite-difference.md#fourier-amplification-symbol)
        - [Scalar Fourier power criterion](finite-difference.md#scalar-fourier-power-criterion)
        - [Uniform power bound for matrix Fourier symbols](finite-difference.md#uniform-power-bound-for-matrix-fourier-symbols)
    - [Central finite difference](finite-difference.md#central-finite-difference)
      - [Fourth-order centered second derivative](finite-difference.md#fourth-order-centered-second-derivative)
      - [Sharp central-secant derivative error](finite-difference.md#sharp-central-secant-derivative-error)
      - [Centered-advection refinement-dependent stability](finite-difference.md#centered-advection-refinement-dependent-stability)
      - [Second-order central difference](finite-difference.md#second-order-central-difference)
    - [Forward difference operator](finite-difference.md#forward-difference-operator)
      - [Adjoint of a discrete forward gradient](finite-difference.md#adjoint-of-a-discrete-forward-gradient)
      - [Discrete antiderivative](finite-difference.md#discrete-antiderivative)
      - [Newton series for an integer-valued polynomial sequence](finite-difference.md#newton-series-for-an-integer-valued-polynomial-sequence)
    - [von Neumann stability analysis](finite-difference.md#von-neumann-stability-analysis)
      - [Nonnormal Fourier amplification matrix](finite-difference.md#nonnormal-fourier-amplification-matrix)
      - [Uniform power bound from separated amplification roots](finite-difference.md#uniform-power-bound-from-separated-amplification-roots)
      - [Stability of a spatially shifted BDF2 stencil](finite-difference.md#stability-of-a-spatially-shifted-bdf2-stencil)
      - [Fourier symbol of a difference operator](finite-difference.md#fourier-symbol-of-a-difference-operator)
      - [Power boundedness of a two-level Fourier scheme](finite-difference.md#power-boundedness-of-a-two-level-fourier-scheme)
        - [Uniform stability of a shifted two-level advection scheme](finite-difference.md#uniform-stability-of-a-shifted-two-level-advection-scheme)
      - [Forward Euler stability for centered advection-diffusion](finite-difference.md#forward-euler-stability-for-centered-advection-diffusion)
      - [Laurent operator](finite-difference.md#laurent-operator)
        - [Toeplitz operator](finite-difference.md#toeplitz-operator)
          - [Toeplitz exponential determinant identity](finite-difference.md#toeplitz-exponential-determinant-identity)
          - [Toeplitz index theorem for continuous symbols](finite-difference.md#toeplitz-index-theorem-for-continuous-symbols)
      - [Boundary stability of a finite-difference method](finite-difference.md#boundary-stability-of-a-finite-difference-method)
        - [Boundary closure of a difference scheme](finite-difference.md#boundary-closure-of-a-difference-scheme)
        - [Uniform Kreiss--Lopatinskii condition](finite-difference.md#uniform-kreiss-lopatinskii-condition)
      - [Eigenvalue stability analysis of a finite difference method](finite-difference.md#eigenvalue-stability-analysis-of-a-finite-difference-method)
        - [Finite-time stability versus power boundedness](finite-difference.md#finite-time-stability-versus-power-boundedness)
        - [Negative spectra do not imply uniform semidiscrete stability](finite-difference.md#negative-spectra-do-not-imply-uniform-semidiscrete-stability)
        - [Nonnormal upwind amplification matrix](finite-difference.md#nonnormal-upwind-amplification-matrix)
      - [Backward Euler diffusion scheme](finite-difference.md#backward-euler-diffusion-scheme)
        - [No positive-Courant cancellation for backward Euler diffusion](finite-difference.md#no-positive-courant-cancellation-for-backward-euler-diffusion)
        - [Backward Euler diffusion stability on a finite Dirichlet interval](finite-difference.md#backward-euler-diffusion-stability-on-a-finite-dirichlet-interval)
      - [Forward Euler diffusion scheme](finite-difference.md#forward-euler-diffusion-scheme)
        - [Explicit time stepping for bounded reaction diffusion](finite-difference.md#explicit-time-stepping-for-bounded-reaction-diffusion)
      - [Stability of a two-parameter implicit-explicit diffusion scheme](finite-difference.md#stability-of-a-two-parameter-implicit-explicit-diffusion-scheme)
      - [Amplification factor](finite-difference.md#amplification-factor)
        - [Amplification factor of a two-sided one-step stencil](finite-difference.md#amplification-factor-of-a-two-sided-one-step-stencil)
      - [Amplification polynomial of a multilevel finite difference scheme](finite-difference.md#amplification-polynomial-of-a-multilevel-finite-difference-scheme)
        - [Leapfrog advection scheme](finite-difference.md#leapfrog-advection-scheme)
          - [Two-dimensional leapfrog stability threshold](finite-difference.md#two-dimensional-leapfrog-stability-threshold)
          - [Two-level stability at the leapfrog Courant boundary](finite-difference.md#two-level-stability-at-the-leapfrog-courant-boundary)
        - [Leapfrog finite-difference scheme for the diffusion equation](finite-difference.md#leapfrog-finite-difference-scheme-for-the-diffusion-equation)
      - [Crank-Nicolson diffusion scheme](finite-difference.md#crank-nicolson-diffusion-scheme)
      - [Crank-Nicolson centered-advection scheme on a finite interval](finite-difference.md#crank-nicolson-centered-advection-scheme-on-a-finite-interval)
      - [Centered three-level wave scheme](finite-difference.md#centered-three-level-wave-scheme)
    - [Courant number](finite-difference.md#courant-number)
      - [Diffusion Courant number](finite-difference.md#diffusion-courant-number)
      - [Courant–Friedrichs–Lewy condition](finite-difference.md#courant-friedrichs-lewy-condition)
    - [Dirichlet discrete Laplacian](finite-difference.md#dirichlet-discrete-laplacian)
      - [Crank-Nicolson stability on a finite Dirichlet interval](finite-difference.md#crank-nicolson-stability-on-a-finite-dirichlet-interval)
      - [Five-point Dirichlet Laplacian as a Kronecker sum](finite-difference.md#five-point-dirichlet-laplacian-as-a-kronecker-sum)
        - [One-implicit-direction diffusion splitting](finite-difference.md#one-implicit-direction-diffusion-splitting)
          - [Stability limit of one-implicit-direction diffusion splitting](finite-difference.md#stability-limit-of-one-implicit-direction-diffusion-splitting)
          - [Unconditionally stable corrected directional diffusion splitting](finite-difference.md#unconditionally-stable-corrected-directional-diffusion-splitting)
      - [Seven-point Dirichlet Laplacian](finite-difference.md#seven-point-dirichlet-laplacian)
    - [Centered convection-diffusion semidiscretization](finite-difference.md#centered-convection-diffusion-semidiscretization)
    - [Discrete maximum principle](finite-difference.md#discrete-maximum-principle)
    - [Method of lines](finite-difference.md#method-of-lines)
      - [Dissipative second-order forward advection semidiscretization](finite-difference.md#dissipative-second-order-forward-advection-semidiscretization)
      - [Energy contraction for centered drift-diffusion](finite-difference.md#energy-contraction-for-centered-drift-diffusion)
      - [Displacement stability of a symmetric semidiscrete wave equation](finite-difference.md#displacement-stability-of-a-symmetric-semidiscrete-wave-equation)
        - [All-time boundedness of a semidiscrete reaction wave equation](finite-difference.md#all-time-boundedness-of-a-semidiscrete-reaction-wave-equation)
      - [Norm conservation of a semidiscrete Schrödinger equation](finite-difference.md#norm-conservation-of-a-semidiscrete-schrodinger-equation)
    - [Lax equivalence theorem](finite-difference.md#lax-equivalence-theorem)
- [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)
- [Gaussian quadrature](#gaussian-quadrature)
  - [Orthogonal-node criterion for Gaussian quadrature](#orthogonal-node-criterion-for-gaussian-quadrature)
  - [Two-node Gaussian quadrature with quadratic weight](#two-node-gaussian-quadrature-with-quadratic-weight)
  - [Chebyshev–Gauss quadrature](#chebyshev-gauss-quadrature)
  - [Gauss-Laguerre quadrature](#gauss-laguerre-quadrature)
  - [Two-node Gaussian quadrature with linear weight](#two-node-gaussian-quadrature-with-linear-weight)
  - [Two-node Gaussian quadrature with sine weight](#two-node-gaussian-quadrature-with-sine-weight)
  - [Positive weights of Gaussian quadrature](#positive-weights-of-gaussian-quadrature)
  - [Gauss-Hermite quadrature](#gauss-hermite-quadrature)
- [Lobatto quadrature](#lobatto-quadrature)
- [Chebyshev polynomial](#chebyshev-polynomial)
  - [Chebyshev projection of a semicircle](#chebyshev-projection-of-a-semicircle)
  - [Chebyshev nodal derivative comparison](#chebyshev-nodal-derivative-comparison)
  - [Chebyshev polynomial of the second kind](#chebyshev-polynomial-of-the-second-kind)
  - [Rational cosine of an integral submultiple of pi](#rational-cosine-of-an-integral-submultiple-of-pi)
  - [Positivity of Chebyshev derivatives beyond the unit interval](#positivity-of-chebyshev-derivatives-beyond-the-unit-interval)
  - [Monic Chebyshev extremal polynomial](#monic-chebyshev-extremal-polynomial)
  - [Chebyshev polynomial domination lemma](#chebyshev-polynomial-domination-lemma)
    - [Chebyshev interpolation represents external evaluation](#chebyshev-interpolation-represents-external-evaluation)
  - [Chebyshev differential equation](#chebyshev-differential-equation)
    - [Chebyshev derivative Sturm-Liouville pair](#chebyshev-derivative-sturm-liouville-pair)
- [Backward differentiation formula](#backward-differentiation-formula)
  - [Second-order backward differentiation formula](#second-order-backward-differentiation-formula)
  - [BDF2 discrete energy identity](#bdf2-discrete-energy-identity)
- [Constrained optimization](#constrained-optimization)
  - [Optimization constraint](#optimization-constraint)
- [Equally spaced interpolation](#equally-spaced-interpolation)
- [Givens rotation](#givens-rotation)
  - [QR decomposition by Givens rotations](#qr-decomposition-by-givens-rotations)
- [Gradient descent](#gradient-descent)
  - [Gradient ascent](#gradient-ascent)
  - [Stochastic gradient descent](#stochastic-gradient-descent)
    - [Projected stochastic gradient descent](#projected-stochastic-gradient-descent)
    - [Unbiased stochastic gradient](#unbiased-stochastic-gradient)
  - [Lipschitz gradient](#lipschitz-gradient)
    - [Descent lemma](#descent-lemma)
  - [Exact line search for a positive-definite quadratic](#exact-line-search-for-a-positive-definite-quadratic)
  - [Conjugate gradient method](#conjugate-gradient-method)
    - [Linear-system residual](#linear-system-residual)
    - [Conjugate-gradient residual orthogonality](#conjugate-gradient-residual-orthogonality)
    - [Preconditioned conjugate gradient method](#preconditioned-conjugate-gradient-method)
      - [Exact inverse-square-root preconditioner](#exact-inverse-square-root-preconditioner)
    - [Krylov subspace](#krylov-subspace)
      - [Krylov dimension from spectral components](#krylov-dimension-from-spectral-components)
    - [Finite termination of the conjugate gradient method](#finite-termination-of-the-conjugate-gradient-method)
  - [Heavy-ball method](#heavy-ball-method)
    - [Heavy-ball residual recurrence](#heavy-ball-residual-recurrence)
    - [Heavy-ball error propagation matrix](#heavy-ball-error-propagation-matrix)
      - [Heavy-ball rate for a two-eigenvalue diagonal quadratic](#heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic)
- [Peano kernel theorem](#peano-kernel-theorem)
  - [Peano kernel](#peano-kernel)
    - [Centered second-derivative Peano kernel](#centered-second-derivative-peano-kernel)
    - [Sharp Peano bound for an interior three-point first derivative](#sharp-peano-bound-for-an-interior-three-point-first-derivative)
    - [Sharp error constants for a Peano kernel](#sharp-error-constants-for-a-peano-kernel)
      - [Sharp Peano-kernel constant for the three-point endpoint first derivative](#sharp-peano-kernel-constant-for-the-three-point-endpoint-first-derivative)
  - [Four-point one-sided second-derivative formula](#four-point-one-sided-second-derivative-formula)
    - [Sharp Peano-kernel constant for the four-point endpoint second derivative](#sharp-peano-kernel-constant-for-the-four-point-endpoint-second-derivative)
- [Periodic trapezoidal Fourier aliasing](#periodic-trapezoidal-fourier-aliasing)
  - [Periodic N-point rectangle-rule error](#periodic-n-point-rectangle-rule-error)
- [Fourier-Galerkin matrix for a drift-diffusion equation](#fourier-galerkin-matrix-for-a-drift-diffusion-equation)
- [Fourier spectral method for variable-coefficient advection](#fourier-spectral-method-for-variable-coefficient-advection)
  - [Positive Fourier-symbol Toeplitz matrix](#positive-fourier-symbol-toeplitz-matrix)
  - [Real spectrum of a positive-Hermitian times Hermitian product](#real-spectrum-of-a-positive-hermitian-times-hermitian-product)
  - [Explicit Euler instability on a nonzero imaginary eigenvalue](#explicit-euler-instability-on-a-nonzero-imaginary-eigenvalue)
- [Runge-Kutta method](#runge-kutta-method)
  - [Maximal-order Runge-Kutta methods are A-stable](#maximal-order-runge-kutta-methods-are-a-stable)
  - [Theta method](#theta-method)
    - [Theta diffusion stability criterion](#theta-diffusion-stability-criterion)
      - [Rough-data damping distinction for the theta method](#rough-data-damping-distinction-for-the-theta-method)
  - [Strong stability preserving Runge-Kutta method](#strong-stability-preserving-runge-kutta-method)
  - [Classical fourth-order Runge-Kutta method](#classical-fourth-order-runge-kutta-method)
  - [Butcher tableau](#butcher-tableau)
  - [Butcher order condition](#butcher-order-condition)
    - [Second-order conditions with independent Runge-Kutta abscissae](#second-order-conditions-with-independent-runge-kutta-abscissae)
    - [Fourth-order conditions for a Runge-Kutta method](#fourth-order-conditions-for-a-runge-kutta-method)
  - [Implicit Runge-Kutta method](#implicit-runge-kutta-method)
    - [Two-stage Runge-Kutta family with an implicit second stage](#two-stage-runge-kutta-family-with-an-implicit-second-stage)
    - [Stage solvability of an implicit Runge-Kutta method](#stage-solvability-of-an-implicit-runge-kutta-method)
    - [Implicit midpoint rule](#implicit-midpoint-rule)
    - [Crank-Nicolson method](#crank-nicolson-method)
      - [Contractivity of split Crank-Nicolson diffusion](#contractivity-of-split-crank-nicolson-diffusion)
    - [Collocation Runge-Kutta method](#collocation-runge-kutta-method)
      - [Two-node collocation A-stability criterion](#two-node-collocation-a-stability-criterion)
      - [Collocation order theorem](#collocation-order-theorem)
        - [Collocation endpoint superconvergence by quadrature orthogonality](#collocation-endpoint-superconvergence-by-quadrature-orthogonality)
      - [Collocation tableau row-sum identity](#collocation-tableau-row-sum-identity)
      - [Lobatto IIIA method](#lobatto-iiia-method)
      - [Gauss-Legendre method](#gauss-legendre-method)
        - [Gauss collocation coefficient construction](#gauss-collocation-coefficient-construction)
        - [Fourth-order two-stage Gauss collocation method](#fourth-order-two-stage-gauss-collocation-method)
      - [Radau IIA method](#radau-iia-method)
        - [Padé identification of a Radau stability function](#pade-identification-of-a-radau-stability-function)
      - [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)
        - [Runge-Kutta conservation of quadratic invariants](#runge-kutta-conservation-of-quadratic-invariants)
        - [Butcher contractivity theorem](#butcher-contractivity-theorem)
        - [Runge-Kutta contractivity identity](#runge-kutta-contractivity-identity)
    - [Trapezoidal rule](#trapezoidal-rule)
      - [Trapezoidal rule fails B-stability](#trapezoidal-rule-fails-b-stability)
  - [Time-symmetric numerical method](#time-symmetric-numerical-method)
  - [Order of a Runge-Kutta method](#order-of-a-runge-kutta-method)
    - [Third-order conditions for an explicit Runge-Kutta method](#third-order-conditions-for-an-explicit-runge-kutta-method)
- [Simplex algorithm](#simplex-algorithm)
  - [Dual simplex algorithm](#dual-simplex-algorithm)
  - [Simplex dictionary](#simplex-dictionary)
- [Sparse optimization](#sparse-optimization)
  - [Compressed sensing](#compressed-sensing)
    - [Coherence of a normalized matrix](#coherence-of-a-normalized-matrix)
      - [Cumulative coherence](#cumulative-coherence)
        - [Cumulative coherence bound for restricted isometry](#cumulative-coherence-bound-for-restricted-isometry)
    - [Sparse injectivity](#sparse-injectivity)
    - [Restricted isometry property](#restricted-isometry-property)
      - [Restricted isometry constant](#restricted-isometry-constant)
        - [Sharp order-s restricted-isometry recovery theorem](#sharp-order-s-restricted-isometry-recovery-theorem)
    - [Basis pursuit](#basis-pursuit)
      - [Strict dual certificate for basis pursuit](#strict-dual-certificate-for-basis-pursuit)
        - [Least-norm dual certificate](#least-norm-dual-certificate)
      - [Nullspace property](#nullspace-property)
        - [Lq null space property](#lq-null-space-property)
          - [Monotonicity of uniform sparse recovery in the exponent](#monotonicity-of-uniform-sparse-recovery-in-the-exponent)
        - [Robust null space property](#robust-null-space-property)
        - [Fixed-sign null space condition](#fixed-sign-null-space-condition)
    - [Sparse vector](#sparse-vector)
      - [L0 sparsity count](#l0-sparsity-count)
      - [Support of a vector](#support-of-a-vector)
        - [Maximum-support vector in a finite-dimensional subspace](#maximum-support-vector-in-a-finite-dimensional-subspace)
- [Stability function](#stability-function)
  - [Dahlquist test equation](#dahlquist-test-equation)
- [Linear multistep method](#linear-multistep-method)
  - [Reciprocal-root three-step multistep family](#reciprocal-root-three-step-multistep-family)
  - [Simpson multistep method](#simpson-multistep-method)
  - [First Dahlquist barrier](#first-dahlquist-barrier)
    - [Newton-Cotes multistep methods attaining the first Dahlquist barrier](#newton-cotes-multistep-methods-attaining-the-first-dahlquist-barrier)
    - [Cayley coefficient proof of the first Dahlquist barrier](#cayley-coefficient-proof-of-the-first-dahlquist-barrier)
      - [Coefficient sign lemma for the first Dahlquist barrier](#coefficient-sign-lemma-for-the-first-dahlquist-barrier)
  - [Two-step family with a third-order member](#two-step-family-with-a-third-order-member)
  - [Adams-Bashforth method](#adams-bashforth-method)
    - [Adams-Bashforth stability for centered diffusion](#adams-bashforth-stability-for-centered-diffusion)
  - [Common-factor cancellation defect in a multistep recurrence](#common-factor-cancellation-defect-in-a-multistep-recurrence)
  - [Trapezoidal-BDF two-step family](#trapezoidal-bdf-two-step-family)
  - [Multiderivative multistep method](#multiderivative-multistep-method)
    - [Symmetric sixth-order two-derivative method](#symmetric-sixth-order-two-derivative-method)
    - [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)
      - [Bounded-root stability set of the symmetric two-derivative formula](#bounded-root-stability-set-of-the-symmetric-two-derivative-formula)
      - [Empty strict decay domain of the symmetric two-derivative formula](#empty-strict-decay-domain-of-the-symmetric-two-derivative-formula)
      - [Negative-real instability of the symmetric two-derivative formula](#negative-real-instability-of-the-symmetric-two-derivative-formula)
    - [A-stable third-order two-step multiderivative method](#a-stable-third-order-two-step-multiderivative-method)
    - [Convergence of a zero-stable multiderivative method](#convergence-of-a-zero-stable-multiderivative-method)
  - [Zero-stability](#zero-stability)
    - [Root condition for a multistep method](#root-condition-for-a-multistep-method)
      - [Parasitic amplification root](#parasitic-amplification-root)
        - [Centered two-step discretization of exponential decay](#centered-two-step-discretization-of-exponential-decay)
      - [Root stability of a cubic multistep polynomial](#root-stability-of-a-cubic-multistep-polynomial)
  - [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem)
    - [Necessity of the root condition for multistep convergence](#necessity-of-the-root-condition-for-multistep-convergence)
  - [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)
    - [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)
      - [Amplification root](#amplification-root)
      - [Exterior roots of the derivative polynomial bound multistep stability](#exterior-roots-of-the-derivative-polynomial-bound-multistep-stability)
    - [Order conditions for a linear multistep method](#order-conditions-for-a-linear-multistep-method)
      - [Exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method)
  - [Adams–Moulton method](#adams-moulton-method)
  - [Second Dahlquist barrier](#second-dahlquist-barrier)
- [Numerical linear algebra](#numerical-linear-algebra)
  - [Matrix preconditioning](#matrix-preconditioning)
    - [Matrix preconditioner](#matrix-preconditioner)
  - [Power iteration](#power-iteration)
  - [Gaussian elimination](#gaussian-elimination)
    - [Sparse Gaussian elimination](#sparse-gaussian-elimination)
      - [Leaf elimination of a tree-pattern positive-definite matrix](#leaf-elimination-of-a-tree-pattern-positive-definite-matrix)
      - [Symbolic factorization](#symbolic-factorization)
      - [Elimination tree](#elimination-tree)
      - [Nested dissection](#nested-dissection)
      - [Minimum degree algorithm](#minimum-degree-algorithm)
      - [Fill-in](#fill-in)
      - [Matrix graph](#matrix-graph)
        - [Elimination graph](#elimination-graph)
          - [Fill-path criterion for symmetric elimination](#fill-path-criterion-for-symmetric-elimination)
    - [Columnwise partial pivoting](#columnwise-partial-pivoting)
    - [Row echelon form](#row-echelon-form)
    - [Elementary row operation](#elementary-row-operation)
      - [Elementary matrix](#elementary-matrix)
  - [LU decomposition](#lu-decomposition)
  - [LDL decomposition](#ldl-decomposition)
  - [Machine epsilon](#machine-epsilon)
  - [Eigenpair residual](#eigenpair-residual)
    - [Backward error of an approximate eigenpair](#backward-error-of-an-approximate-eigenpair)
  - [Householder QR decomposition](#householder-qr-decomposition)
    - [Householder reduction of an overdetermined consistent system](#householder-reduction-of-an-overdetermined-consistent-system)
  - [Householder tridiagonalization](#householder-tridiagonalization)
    - [Skew-symmetric Householder tridiagonalization](#skew-symmetric-householder-tridiagonalization)
  - [Unshifted QR algorithm](#unshifted-qr-algorithm)
    - [Accumulated QR factorization identity](#accumulated-qr-factorization-identity)
    - [Symmetric bandwidth preservation under QR iteration](#symmetric-bandwidth-preservation-under-qr-iteration)
    - [Simultaneous iteration interpretation of the QR algorithm](#simultaneous-iteration-interpretation-of-the-qr-algorithm)
      - [Two-column dominant-subspace condition](#two-column-dominant-subspace-condition)
    - [Block deflation in the QR algorithm](#block-deflation-in-the-qr-algorithm)
  - [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)
    - [Semiconvergence of cyclic Poisson iterations](#semiconvergence-of-cyclic-poisson-iterations)
    - [Richardson iteration](#richardson-iteration)
    - [Gauss-Seidel method](#gauss-seidel-method)
    - [Successive over-relaxation](#successive-over-relaxation)
    - [Iteration matrix](#iteration-matrix)
    - [Matrix splitting](#matrix-splitting)
      - [Householder-John theorem](#householder-john-theorem)
    - [Jacobi method](#jacobi-method)
      - [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](#skew-tridiagonal-jacobi-and-gauss-seidel-iterations)
      - [Weighted Jacobi method](#weighted-jacobi-method)
        - [Weighted Jacobi eigenvalues for a square Dirichlet grid](#weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid)
        - [Weighted Jacobi method for the one-dimensional Poisson equation](#weighted-jacobi-method-for-the-one-dimensional-poisson-equation)
          - [High-frequency smoothing factor of weighted Jacobi](#high-frequency-smoothing-factor-of-weighted-jacobi)
            - [Exact finite-grid high-frequency Jacobi smoothing optimum](#exact-finite-grid-high-frequency-jacobi-smoothing-optimum)
      - [Jacobi convergence for a three-by-three equicorrelation matrix](#jacobi-convergence-for-a-three-by-three-equicorrelation-matrix)
      - [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](#jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix)
- [Linear stability domain](#linear-stability-domain)
  - [Strict linear stability domain](#strict-linear-stability-domain)
  - [A-alpha stability](#a-alpha-stability)
  - [Euler method](#euler-method)
  - [A-stability](#a-stability)
    - [A-stability of near-diagonal exponential Padé approximants](#a-stability-of-near-diagonal-exponential-pade-approximants)
    - [Principal-root obstruction to A-stability](#principal-root-obstruction-to-a-stability)
    - [Explicit multistep methods cannot be A-stable](#explicit-multistep-methods-cannot-be-a-stable)
    - [Boundary-locus test for multistep A-stability](#boundary-locus-test-for-multistep-a-stability)
    - [L-stability](#l-stability)
    - [B-stability](#b-stability)
    - [Backward Euler method](#backward-euler-method)
    - [A-stability of a symmetric two-stage implicit Runge-Kutta family](#a-stability-of-a-symmetric-two-stage-implicit-runge-kutta-family)
  - [Stiff equation](#stiff-equation)
    - [Stiff two-mode linear system](#stiff-two-mode-linear-system)
  - [Milne device for forward and backward Euler](#milne-device-for-forward-and-backward-euler)
- [Orthogonal polynomial](#orthogonal-polynomial)
  - [Kravchuk polynomials](#kravchuk-polynomials)
  - [Orthogonality forces many interior zeros](#orthogonality-forces-many-interior-zeros)
  - [Zernike polynomials](#zernike-polynomials)
    - [Zernike spherical mode](#zernike-spherical-mode)
  - [Monic orthogonal polynomial](#monic-orthogonal-polynomial)
    - [Three-term recurrence for monic orthogonal polynomials](#three-term-recurrence-for-monic-orthogonal-polynomials)
  - [Hermite polynomial](#hermite-polynomial)
    - [Hermite function](#hermite-function)
      - [Hermite functions are Fourier eigenfunctions](#hermite-functions-are-fourier-eigenfunctions)
      - [Mehler formula for Hermite functions](#mehler-formula-for-hermite-functions)
    - [Probabilists' Hermite polynomial](#probabilists-hermite-polynomial)
      - [Space-time Hermite polynomial](#space-time-hermite-polynomial)
  - [Zeros of orthogonal polynomials](#zeros-of-orthogonal-polynomials)
  - [Jacobi matrix](#jacobi-matrix)
- [Numerical integration](#numerical-integration)
  - [Boole's rule](#boole-s-rule)
  - [Quadrature rule](#quadrature-rule)
    - [Newton-Cotes closed quadrature](#newton-cotes-closed-quadrature)
    - [Simpson's rule](#simpson-s-rule)
    - [Convergence of positive quadrature on continuous functions](#convergence-of-positive-quadrature-on-continuous-functions)
    - [Nodal-polynomial criterion for quadrature exactness](#nodal-polynomial-criterion-for-quadrature-exactness)
    - [Degree ceiling for quadrature exactness](#degree-ceiling-for-quadrature-exactness)
    - [Positivity of quadrature weights from degree 2n exactness](#positivity-of-quadrature-weights-from-degree-2n-exactness)
    - [Convergence of positive quadrature rules](#convergence-of-positive-quadrature-rules)
    - [Moment matching](#moment-matching)
- [Midpoint method](#midpoint-method)
- [Collocation method](#collocation-method)
- [QR algorithm](#qr-algorithm)
- [Iterative method](#iterative-method)

## Newton root-finding iteration

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The Newton root-finding iteration solves the local tangent-line approximation to a scalar equation $F(t)=0$. For a twice continuously differentiable function near a simple root, with [derivative](calculus.md#derivative) bounded away from zero, Taylor's theorem gives $|t_{r+1}-t_*|\leq C|t_r-t_*|^2$ once the iteration is sufficiently close. Global convergence is not automatic. A sign-changing bracket can safeguard the method by replacing unsuitable steps by the [bisection method](#bisection-method).

### Newton iteration in a Banach space

↑ **Parent:** [Newton root-finding iteration](#newton-root-finding-iteration)

For a $C^2$ map $\Phi$ on a [Banach space](banach-space.md), define $N(p)=p-[D\Phi(p)]^{-1}\Phi(p)$ wherever the bounded [derivative](calculus.md#derivative) is invertible. It solves the local affine approximation to $\Phi=0$. Every zero is a [fixed point](function.md#fixed-point) of $N$. Near a zero with invertible [derivative](calculus.md#derivative), bounded inverses and a locally Lipschitz [derivative](calculus.md#derivative) give the [quadratic Newton error bound in a Banach space](#quadratic-newton-error-bound-in-a-banach-space).

// Target: numerical-analysis.bigb

#### Frozen Newton correction for a fixed-point equation

↑ **Parent:** [Newton iteration in a Banach space](#newton-iteration-in-a-banach-space)

To solve $\Phi(p)=p$, let $J$ be a bounded approximation to $(D\Phi(p_0)-I)^{-1}$ and set $A(p)=p-J(\Phi(p)-p)$. Its [derivative](calculus.md#derivative) is $DA(p)=I-J(D\Phi(p)-I)$. Every [fixed point](function.md#fixed-point) of $\Phi$ is fixed by $A$; the converse holds when $J$ is injective. A good inverse approximation makes $A$ a [contraction mapping](analysis.md#contraction-mapping) even if $\Phi$ itself has an expanding direction.

// Target: analysis.bigb

#### Quadratic Newton error bound in a Banach space

↑ **Parent:** [Newton iteration in a Banach space](#newton-iteration-in-a-banach-space)

Let $\Phi(\bar p)=0$, $\|[D\Phi(p)]^{-1}\|\leq M$ and $\|D\Phi(p)-D\Phi(q)\|\leq L\|p-q\|$ near $\bar p$. The integral [Taylor remainder](calculus.md#taylor-remainder) gives

$$
\|N(p)-\bar p\|\leq\frac{ML}{2}\|p-\bar p\|^2.
$$

A small ball with $(ML/2)r<1$ is invariant under $N$. Iteration there converges at least quadratically, with $Ce_{n+k}\leq(Ce_n)^{2^k}$ for $C=ML/2$.

// Target: numerical-analysis.bigb

### Monotone Newton convergence for a strictly convex function

↑ **Parent:** [Newton root-finding iteration](#newton-root-finding-iteration)

Let $f\in C^2([a,b])$ have $f',f''>0$ and $f(a)<0<f(b)$. Its unique root $r$ lies in $(a,b)$. Starting [Newton root-finding iteration](#newton-root-finding-iteration) at $b$, strict convexity puts the tangent root strictly between $r$ and the current iterate, so the iterates decrease to $r$. Taylor expansion about the current iterate gives $e_{n+1}=f''(\xi_n)e_n^2/[2f'(x_n)]$, where $e_n=x_n-r$ and $\xi_n\in(r,x_n)$. Continuity proves the displayed positive asymptotic constant and [quadratic convergence](#quadratic-convergence).

## Bisection method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a continuous scalar function with opposite endpoint signs on $[a,b]$, evaluate its midpoint and retain the half interval with a sign change. The [intermediate value theorem](calculus.md#intermediate-value-theorem) preserves a root bracket. After $r$ halvings its midpoint is at most $(b-a)/2^{r+1}$ from a bracketed root. Endpoint and midpoint zeros are recorded directly; tangent roots with no sign change require a different isolation test.

## Chord error bound

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

If a twice differentiable [parametric curve](topology.md#parametric-curve) $R:[a,b]\to\mathbb R^m$ satisfies $\lVert R''\rVert\le M$, its deviation from the linearly parameterized chord is at most $M(b-a)^2/8$. This follows from the Green function for the second derivative with zero endpoint values. It bounds the [Hausdorff distance](topological-analysis.md#hausdorff-distance) between the arc and its chord.

// Target: analysis.bigb

## Interval arithmetic

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interval_arithmetic)

[Interval arithmetic](#interval-arithmetic) computes enclosing intervals rather than single floating-point values. Exclusion and validated root tests on recursively subdivided boxes can support exhaustive implicit-curve tracing and certified geometric error bounds.

// Target: analysis.bigb

## Continuation method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuation_method)

A [continuation method](#continuation-method) follows solutions of a parameter-dependent equation. Predictor-corrector tracing of a regular implicit curve uses a tangent predictor followed by a [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) correction on a transverse section.

// Target: analysis.bigb

### Transversal surface intersection tracing

↑ **Parent:** [Continuation method](#continuation-method)

For a [parametric surface](differential-geometry.md#parametric-surface) $F(u,v)$ and a scalar implicit equation $f(P)=0$, set $g=f\circ F$. At a regular transversal intersection, $\nabla g\ne0$, and $(-g_v,g_u)$ is a parameter [tangent vector](differential-geometry.md#tangent-vector). Normalize its image under $DF$ to choose physical [arc length](riemannian-geometry.md#arc-length) steps. A predictor followed by [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) correction of $g=0$ and a transverse plane equation gives a local [continuation method](#continuation-method). Certified patch bounds are useful for finding seeds; corner signs alone do not detect a closed intersection entirely inside a patch.

#### Transversal intersection of two parametric surfaces

↑ **Parent:** [Transversal surface intersection tracing](#transversal-surface-intersection-tracing)

At regular transverse intersections, the displayed map has a rank-three $3\times4$ [Jacobian matrix](calculus.md#jacobian-matrix). Its one-dimensional kernel is the parameter tangent, while the physical tangent is parallel to the [cross product](vector-space.md#cross-product) of the surface normals. A [continuation method](#continuation-method) predicts along that tangent and corrects $F=0$ together with a transverse section equation using [Newton method](mathematical-optimization.md#newton-s-method-in-optimization). Patch bounds and component isolation supply seeds; one seed alone cannot discover every disconnected curve or closed loop. Tangency or coincident surfaces violate the regular-curve assumptions and require separate analysis.

## Computer aided geometric design

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[Computer aided geometric design](#computer-aided-geometric-design) studies computational representations, evaluation and manipulation of [curves](topology.md#curve) and [regular surfaces](differential-geometry.md#smooth-surface), especially using [splines](uniform-approximation.md#spline-mathematics) and [subdivision surfaces](#subdivision-surface).

// Target: geometry-and-topology.bigb

### Affine equivariance of a geometric basis

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

A geometry representation with scalar [partition of unity](differential-geometry.md#partition-of-unity) basis functions commutes with every [affine map](geometry-and-topology.md#affine-map) of its [control points](#control-point). For $T(x)=Ax+b$, linearity moves $A$ through the sum and the sum-to-one identity supplies the translation $b$. Positivity is needed for a [convex hull](mathematical-optimization.md#convex-hull) property, but not for this equivariance. The same argument applies to linear [subdivision matrices](#subdivision-matrix) whose rows sum to one. General [projective transformations](projective-space.md#projective-linear-transformation) require homogeneous [control points](#control-point) and rational dehomogenization rather than transforming Euclidean controls with unchanged weights.

### Translational penetration depth

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

For overlapping solid bodies, the penetration depth is the smallest translation needed to remove interior overlap, with orientation fixed. It is distance from the origin to the complement of the translational collision region. Define signed separation as positive ordinary separation for disjoint bodies, zero for contact, and $-\delta$ for interior overlap. Translation-space [branch and bound](mathematical-optimization.md#branch-and-bound) can bracket it using certified intersection/containment queries. This convention handles crossing and complete containment; merely negating unsigned boundary distance does not.

### Linear precision of a geometric basis

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

A basis with the displayed identities reproduces [affine functions](vector-space.md#affine-function) from their values at the precision sites $\xi_j$. For two such bases, the tensor-product precision sites are $(\xi_j,\eta_k)$: summation independently recovers $u$ and $v$. Affine images of this site grid therefore produce exact planar parameterizations, independent of the chosen control-grid representation.

### Control point

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

A [control point](#control-point) is geometric data used to specify a curve or surface through a basis or refinement rule. In a linear representation $C(t)=\sum_i b_i(t)P_i$, moving $P_i$ by $h$ changes the curve by $b_i(t)h$. The support of $b_i$ is therefore precisely its influence region. A [control point](#control-point) need not lie on the curve: [Bézier curves](#bezier-curve) interpolate their endpoint controls, whereas generic interior [B-spline](uniform-approximation.md#b-spline) controls are approximated.

#### Control net

↑ **Parent:** [Control point](#control-point)

A mesh connecting a surface's [control points](#control-point) according to the representation's indexing topology. A [tensor-product surface basis](differential-geometry.md#tensor-product-surface-basis) gives a rectangular index grid and quadrilateral cells, even when its points in space are neither planar nor rectangular. The drawn mesh is a geometric skeleton, not generally the exact limit surface or an enclosing solid. Positive [partition of unity](differential-geometry.md#partition-of-unity) coefficients give a [convex hull](mathematical-optimization.md#convex-hull) bound on the relevant controls.

#### Control polygon

↑ **Parent:** [Control point](#control-point)

A [control polygon](#control-polygon) joins successive [control points](#control-point) by [line segments](mathematical-optimization.md#line-segment). It gives an editable geometric skeleton, not usually the exact curve. Positive partition-of-unity basis functions place the curve inside the [convex hull](mathematical-optimization.md#convex-hull) of its active [control points](#control-point); subdivision can refine this polygon to approximate the limit curve with a certified error.

### Apparent-gravity camera frame

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

If $g$ is gravitational [acceleration](classical-mechanics.md#acceleration) and $a$ is the camera's [acceleration](classical-mechanics.md#acceleration), the locally felt upward vector is $U=a-g$. Choose the travel [unit vector](vector-space.md#unit-vector) $X$, set $W=U-(U\cdot X)X$, and, when $W\ne0$, take $Z=W/\|W\|$ and $Y=Z\times X$. These form an [orthonormal basis](linear-algebra.md#orthonormal-basis) with $U$ in the $XZ$ plane. If $U$ is parallel to $X$, the condition leaves the roll angle free even when $U\ne0$; transport a previous transverse axis or choose a well-conditioned coordinate axis and project it into $X^\perp$.

### Subdivision curve

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

A [subdivision curve](#subdivision-curve) is the limit of a repeated control-polygon refinement rule. Linear stationary rules can be studied through their subdivision masks and often represent [splines](uniform-approximation.md#spline-mathematics).

// Target: analysis.bigb

#### Binary linear interpolatory subdivision

↑ **Parent:** [Subdivision curve](#subdivision-curve)

The centered [subdivision mask](#subdivision-mask) $[1,2,1]/2$ retains old [control points](#control-point) and inserts edge midpoints. Its [control polygon](#control-polygon) is unchanged as a geometric curve by refinement. Its basic limit is the hat $\phi(t)=\max(1-|t|,0)$, with support $[-1,1]$. This [linear spline](uniform-approximation.md#linear-spline) representation reproduces constants and linear functions, and is $C^0$ but generally not $C^1$ at its [spline knots](uniform-approximation.md#spline-knot).

#### Functional precision set of a subdivision scheme

↑ **Parent:** [Subdivision curve](#subdivision-curve)

The [functional precision set of a subdivision scheme](#functional-precision-set-of-a-subdivision-scheme) consists of functions exactly reproduced by refining their uniform samples with the scheme's consistent parameter placement. Polynomial precision usually specifies the reproduced polynomial space. If exactness is required for every grid spacing and shift, the binary midpoint-interpolation scheme has precision exactly the [affine functions](vector-space.md#affine-function). At one fixed grid, its entire reconstruction range is the space of continuous [piecewise linear functions](function.md#piecewise-linear-function) on that grid; this larger range should not be confused with polynomial precision or arbitrary-grid reproduction.

#### Chaikin subdivision

↑ **Parent:** [Subdivision curve](#subdivision-curve)

Iteratively replace every polygon edge by its quarter and three-quarter points, joining the resulting points in order. On an infinite or appropriately treated closed uniform control sequence, the limit is a quadratic [B-spline](uniform-approximation.md#b-spline) curve. For equally spaced abscissae, its centered [Chaikin basis function](#chaikin-basis-function) has support of width three original grid intervals and is $C^1$, generally not $C^2$. Finite open polygons need an endpoint convention.

##### Chaikin basis function

↑ **Parent:** [Chaikin subdivision](#chaikin-subdivision)

This centered [quadratic cardinal B-spline](uniform-approximation.md#quadratic-cardinal-b-spline) weights each original control ordinate at its uniformly spaced abscissa. Its translates sum to one. It and its first [derivative](calculus.md#derivative) match at half-integer knots, while the second [derivative](calculus.md#derivative) can jump. The limit graph is $\sum_i y_i\beta((x-x_i)/h)$; one ordinate influences exactly three original intervals. Refinement of a quadratic adds $ah^2/4$ in the limit, yielding this basis by extending each three-point neighborhood quadratically.

##### Polynomial degree preservation under Chaikin subdivision

↑ **Parent:** [Chaikin subdivision](#chaikin-subdivision)

For uniformly spaced abscissae, quarter and three-quarter averages applied to constant or affine samples leave the same polynomial. For $P(x)=ax^2+bx+c$ on spacing $h$, both new subgrids lie on $P(x)+3ah^2/16$. For degree $n\geq3$, their candidate polynomial formulas differ with leading term $(h^3/32)P'''$, which has a nonzero highest-degree coefficient. Thus preservation of polynomial degree for arbitrary sufficiently long data sequences holds exactly for degrees zero, one and two, despite quadratic values changing.

#### Support of a stationary subdivision scheme

↑ **Parent:** [Subdivision curve](#subdivision-curve)

Under $P_i^{\ell+1}=\sum_jM_{i-aj}P_j^\ell$, the descendants of control index zero lie at $a^{\ell-1}j_1+\cdots+j_\ell$, where each $j_k$ is in the mask support. Dividing by the refined parameter scale $a^\ell$ gives a limiting influence enclosure with the displayed endpoints. For a mask supported on $[-w,w]$ its width is $2w/(a-1)$ when the endpoints are active and a nonzero compactly supported basic limit exists. To prove exactness, the largest active mask term is the only surviving term near the right endpoint of the refinement equation, forcing $\beta=(\beta+j_{\max})/a$; the analogous left-end argument completes the result. Mask padding should be removed, and a nonconvergent rule has no limit support.

#### Subdivision curve interrogation

↑ **Parent:** [Subdivision curve](#subdivision-curve)

A useful [subdivision curve](#subdivision-curve) interface provides parameter ranges, endpoint and limit evaluation, derivatives, subdivision into equivalent restricted pieces, a certified [bounding volume](#bounding-volume), and a certified error relative to a chord. Positive [subdivision masks](#subdivision-mask) often give a [convex hull](mathematical-optimization.md#convex-hull) bound. Masks with negative coefficients need a separate enclosing bound; their control-point hull need not enclose the limit curve.

##### Closest-point search on a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

At a regular differentiable interior nearest point of a [parametric curve](topology.md#parametric-curve), the displacement from the query point is perpendicular to the [tangent vector](differential-geometry.md#tangent-vector). A [branch and bound](mathematical-optimization.md#branch-and-bound) search uses distances to certified enclosing [bounding volumes](#bounding-volume) as lower bounds, and evaluated limit points as upper bounds. Refine the most promising restricted pieces until the upper bound differs from the global lower bound by the chosen distance tolerance. Safeguarded [Newton root-finding iteration](#newton-root-finding-iteration) accelerates local candidates, but endpoints, nonregular points, ties and other stationary branches must not be omitted.

##### Shadow tracing for a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

For a point light at $L$, the shadow of a curve point is the first surface intersection on its ray beyond that point. Certified patch bounds and subdivision isolate intersections; regular hits are corrected with a three-variable [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) solve. Differentiating the displayed equation gives $[S_u,S_v,-(C-L)](u',v',\lambda')^T=\lambda C'$, a predictor for continuation along the shadow. Surface boundaries and grazing rays require clipping and reseeding; every visible component must be isolated, rather than assumed detectable from a fixed sample of the casting curve.

##### Recursive half-space clipping of a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](#subdivision-curve-interrogation)

For an oriented plane function $\ell$, certified extrema over a [bounding volume](#bounding-volume) allow a [subdivision curve](#subdivision-curve) piece to be rejected when $\max\ell<0$, or wholly retained when $\min\ell\geq0$. Otherwise subdivide. At an explicitly chosen rendering tolerance, a sufficiently flat, sufficiently short piece can be replaced by its clipped chord. This is an approximation, not a proof of exact crossing topology. Exact treatment of tangent contacts and small excursions requires root isolation of $\ell(C(t))$ and splitting into sign-constant intervals, when the curve representation supports such isolation.

### Subdivision surface

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subdivision_surface)

A [subdivision surface](#subdivision-surface) is the limit of repeated mesh refinement and vertex averaging. Exact interrogation evaluates this limit and, where defined, its [tangent vectors](differential-geometry.md#tangent-vector) and [normal vectors](differential-geometry.md#normal-vector); a finite refined control mesh is generally only an approximation to the limit.

// Target: analysis.bigb

#### Lateral artifacts of a subdivision surface

↑ **Parent:** [Subdivision surface](#subdivision-surface)

[Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface) are unwanted variations along an intended straight extrusion: input cross-sections identical along a lattice direction acquire ripples in that direction under refinement. For a stationary arity-$m$ lattice rule $a_{i,j}$, extrusion along the first lattice coordinate is preserved exactly when $\sum_{i\equiv r\ (\mathrm{mod}\ m)}a_{i,j}$ is independent of the residue $r$ for every transverse offset $j$. Then summing along each row gives a single associated univariate [subdivision mask](#subdivision-mask). This direction-specific criterion does not promise invariance under every possible oblique extrusion.

##### Extrusion invariance of a ternary triangular scheme

↑ **Parent:** [Lateral artifacts of a subdivision surface](#lateral-artifacts-of-a-subdivision-surface)

If a triangular-lattice [subdivision mask](#subdivision-mask) has the displayed residue-sum equality, refining data $p_{i,j}=q_j$ gives $p'_{I,J}=\sum_k b_{J-3k}q_k$, independent of $I$. If affine coordinates reproduce their parameter positions, a geometrically straight extrusion is preserved. Rotationally symmetric masks give the corresponding property in all three lattice-edge directions. A boundary curve compatible with this extrusion uses the collapsed mask $b$, not just the central row of the two-dimensional mask.

#### Mid-edge subdivision

↑ **Parent:** [Subdivision surface](#subdivision-surface)

Mid-edge subdivision replaces each mesh edge by its midpoint, joins successive midpoints around every old face, and joins successive midpoints around every old vertex. For an interior [manifold](topology.md#topological-manifold) mesh, each new vertex has valence four. Each geometric update is a [convex combination](mathematical-optimization.md#convex-combination), so every refined control point remains in the [convex hull](mathematical-optimization.md#convex-hull) of the original control mesh. The regular limit is associated with the [quadratic four-direction box spline](uniform-approximation.md#quadratic-four-direction-box-spline).

##### Mid-edge facet centroid invariance

↑ **Parent:** [Mid-edge subdivision](#mid-edge-subdivision)

The descendant of a face with cyclic vertices $p_0,\ldots,p_{n-1}$ has vertices $p_i'=(p_i+p_{i+1})/2$. Their arithmetic mean is unchanged. On the cyclic [Fourier basis](fourier-series.md#fourier-basis), a mode of frequency $j$ is multiplied by $(1+e^{2\pi ij/n})/2$. Every nonconstant mode has modulus less than one, so the descendant face shrinks to the original vertex [centroid](geometry-and-topology.md#centroid). This puts that [centroid](geometry-and-topology.md#centroid) on the subdivision limit, without requiring the original face to be planar.

#### Subdivision surface interrogation

↑ **Parent:** [Subdivision surface](#subdivision-surface)

Interrogation of a subdivision limit needs patch/topology navigation, refinement, limit evaluation and [derivatives](calculus.md#derivative) where they exist, with certified bounds and geometric error estimates. On regular patches one may use the corresponding spline representation. At [extraordinary subdivision vertices](#extraordinary-subdivision-vertex), local [subdivision matrices](#subdivision-matrix) determine limit positions and tangents under the scheme's smoothness conditions. A [normal vector](differential-geometry.md#normal-vector) may exist even when [second derivatives](calculus.md#second-derivative) and [Gaussian curvature](second-fundamental-form.md#gaussian-curvature) do not; finite refined polygons are approximations rather than exact limit queries.

##### Intersection of subdivision limit surfaces

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

A robust intersection search applies [branch and bound](mathematical-optimization.md#branch-and-bound) to pairs of [subdivision surface](#subdivision-surface) patches. Certified [bounding volumes](#bounding-volume) reject disjoint pairs, and refinement reduces unresolved pairs. Limit evaluation, tangent data and controlled approximation bounds produce and correct local intersection arcs, then patch adjacency joins them. Bounds must enclose the limit, not merely the current mesh. Flat polygon intersections are approximations and can miss tiny components or tangencies unless the associated geometric and transversality conditions are verified.

##### Plane section of a subdivision surface

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

A [plane section of a subdivision surface](#plane-section-of-a-subdivision-surface) is a zero set of the plane functional evaluated on the limit [parametric surface](differential-geometry.md#parametric-surface). Certified patch [bounding volumes](#bounding-volume) reject sign-definite patches. On a regular transverse section, $\nabla g\ne0$ and the parameter tangent is $(-g_v,g_u)$; predictor-corrector [continuation method](#continuation-method) traces a branch after every component has been isolated. Closed loops, tangencies, coplanar patches and extraordinary-vertex neighborhoods require more than corner-sign tests. Degenerate sections can contain isolated points or two-dimensional portions rather than only regular curves.

##### Minimum distance between subdivision bodies

↑ **Parent:** [Subdivision surface interrogation](#subdivision-surface-interrogation)

For disjoint compact bodies, the minimum occurs on their boundaries. Patch [bounding volumes](#bounding-volume) give certified lower bounds and evaluated limit-point pairs give upper bounds. A [branch and bound](mathematical-optimization.md#branch-and-bound) search refines promising patch pairs until the global bounds differ by the tolerance. Boundary distance alone cannot detect containment; touching, crossing or nested solid bodies have ordinary set distance zero. Negative overlap values require an additional convention such as [translational penetration depth](#translational-penetration-depth).

#### Extraordinary subdivision vertex

↑ **Parent:** [Subdivision surface](#subdivision-surface)

An [extraordinary subdivision vertex](#extraordinary-subdivision-vertex) has a valence different from that of the regular refinement lattice. Regular [box spline](uniform-approximation.md#box-spline) calculations do not alone establish smoothness at this vertex. The finite local [subdivision matrix](#subdivision-matrix), its [eigenvalues](linear-operator-theory.md#eigenvalue), and the associated [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) determine convergence and tangent behavior.

##### Characteristic map of a subdivision surface

↑ **Parent:** [Extraordinary subdivision vertex](#extraordinary-subdivision-vertex)

The [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) is the planar limit map obtained from the two independent tangent [eigenvectors](linear-operator-theory.md#eigenvector) of its local [subdivision matrix](#subdivision-matrix). In the usual stationary setting, a simple constant eigenvalue one, a semisimple double subdominant eigenvalue $0<\lambda<1$, strictly smaller other eigenvalues, and a regular injective characteristic map establish the standard $C^1$ tangent-plane behavior for nondegenerate data. The eigenvalue inequalities alone do not exclude a folded or singular characteristic map. For an alternating scheme these tests must use a full period of refinement.

#### Quincunx subdivision

↑ **Parent:** [Subdivision surface](#subdivision-surface)

A regular [quincunx subdivision](#quincunx-subdivision) step replaces a square lattice by the union of its old vertices and face centres. In lattice indices one may use

$$
D=\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad D^2=2I.
$$

Thus two steps give ordinary binary refinement. If $A(z,w)$ is the one-step [subdivision mask](#subdivision-mask) symbol, the two-step symbol is $A(z,w)A(zw,z/w)$. The two lattice parity classes separately determine the old-vertex and face-vertex stencils; their coefficient sums must each be one to reproduce constants.

#### Loop subdivision surface

↑ **Parent:** [Subdivision surface](#subdivision-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_subdivision_surface)

On a regular triangular grid, [Loop subdivision](#loop-subdivision-surface) retains an old vertex with weight $10/16$ and adds its six neighbors with weight $1/16$ each. A new edge vertex has weights $3/8$ on the endpoints and $1/8$ on the two opposite vertices. Extraordinary vertices require valence-dependent rules.

// Target: analysis.bigb

##### Polynomial generation by regular Loop subdivision

↑ **Parent:** [Loop subdivision surface](#loop-subdivision-surface)

For the three unit-grid edge vectors $v_1,v_2,v_3$ and a [multivariate polynomial](polynomial.md#multivariate-polynomial) $f$ of total degree at most three, sampled regular-grid [Loop subdivision](#loop-subdivision-surface) generates the graph of $f+\frac1{12}\sum_{r=1}^3(v_r\cdot\nabla)^2f$. Thus affine polynomials are reproduced exactly and all polynomials through degree three retain their degree. Fourth-degree data constant along one edge direction reduce to a [Cardinal cubic B-spline](uniform-approximation.md#cardinal-cubic-b-spline), whose limit need not be a polynomial.

##### Extrusion invariance of Loop subdivision

↑ **Parent:** [Loop subdivision surface](#loop-subdivision-surface)

On an infinite regular triangular grid, height data constant along one edge direction remain constant along that direction under [Loop subdivision](#loop-subdivision-surface). Across rows the induced rule is $g'_{2j}=(g_{j-1}+6g_j+g_{j+1})/8$, $g'_{2j+1}=(g_j+g_{j+1})/2$, the centered [Cardinal cubic B-spline](uniform-approximation.md#cardinal-cubic-b-spline) rule.

// Target: analysis.bigb

#### Subdivision mask

↑ **Parent:** [Subdivision surface](#subdivision-surface)

A stationary binary [subdivision mask](#subdivision-mask) $a$ specifies a refinement operator $q_j=\sum_i a_{j-2i}p_i$. Indices may be vectors for a surface. Coefficients restricted to a parity class give the stencil for one type of refined vertex.

// Target: analysis.bigb

##### Subdivision mask width

↑ **Parent:** [Subdivision mask](#subdivision-mask)

For a stationary univariate refinement $S_{ij}=a_{i-mj}$, the [subdivision mask width](#subdivision-mask-width) counts fine-grid positions from the first to the last active entry in a column, including any internal zeros. Consecutive columns are translates by $m$ rows, the [subdivision arity](#subdivision-arity). The number of old [control points](#control-point) used by a particular new point is instead the size of its row stencil; it need not equal the mask width. A span convention counts $w-1$ fine intervals, so numerical width claims should specify the convention.

##### Subdivision arity

↑ **Parent:** [Subdivision mask](#subdivision-mask)

The subdivision arity is the integer factor $a>1$ by which a stationary refinement shrinks parameter-grid intervals: control index $i$ has coordinate $i/a^\ell$ after $\ell$ levels. It is distinct from the mask width and from the number of neighbors in a stencil.

##### Subdivision difference scheme

↑ **Parent:** [Subdivision mask](#subdivision-mask)

For backward differences $\Delta P_i=P_i-P_{i-1}$, a [scalar](vector-space.md#scalar) stationary arity-$a$ [subdivision mask](#subdivision-mask) has symbol $M(z)=\sum_iM_i z^i$. The identity $(1-z)M(z)=B(z)(1-z^a)$ gives the displayed intertwining whenever the quotient is a finite [Laurent polynomial](polynomial.md#laurent-polynomial). Iterating supplies higher-difference masks. The coefficients $a^{r\ell}\Delta^rP_i^\ell$ are candidate $r$th-derivative controls. A convergent [derivative](calculus.md#derivative) scheme, proved by contraction of its first differences, establishes corresponding smoothness of the original limit under the standard consistent parameterization.

###### Norm and spectral bounds for subdivision regularity

↑ **Parent:** [Subdivision difference scheme](#subdivision-difference-scheme)

Finite local [subdivision matrices](#subdivision-matrix) for the scaled difference scheme track [derivative](calculus.md#derivative) variations in nested parameter intervals. A product-norm bound below one proves uniform contraction for every interval and therefore gives a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) on [derivative](calculus.md#derivative) [continuity](calculus.md#continuous-function). A product [eigenvalue](linear-operator-theory.md#eigenvalue) of modulus at least one is an obstruction when its mode is reachable from the data and visible in the limit: generic data excite it, so the corresponding [derivative](calculus.md#derivative) differences fail to vanish. Harmless [polynomial](polynomial.md) or unobservable modes must be removed before applying such an [upper bound](set.md#upper-bound-in-a-partially-ordered-set). Borderline smoothness needs direct analysis, not rounding a numerical exponent. Stability and convergence of the underlying scheme must be checked rather than inferred from mask width.

##### Subdivision matrix

↑ **Parent:** [Subdivision mask](#subdivision-mask)

A local [subdivision matrix](#subdivision-matrix) maps the [control points](#control-point) in a refinement-invariant neighborhood to the refined neighborhood. Row sums one express constant reproduction. Its constant [eigenvector](linear-operator-theory.md#eigenvector) has [eigenvalue](linear-operator-theory.md#eigenvalue) one; remaining [eigenvalues](linear-operator-theory.md#eigenvalue) govern decay of shape modes. Near an [extraordinary subdivision vertex](#extraordinary-subdivision-vertex), tangent modes and a [characteristic map of a subdivision surface](#characteristic-map-of-a-subdivision-surface) are needed to test geometric smoothness, beyond simple convergence.

<h3 id="bezier-curve">Bézier curve</h3>

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bézier_curve)

A degree-$p$ [Bézier curve](#bezier-curve) with control points $B_j$ is $\sum_{j=0}^p\binom pj(1-t)^{p-j}t^jB_j$. Its [Bernstein polynomial](functional-analysis.md#bernstein-polynomial) basis gives affine invariance and the [convex hull](mathematical-optimization.md#convex-hull) property.

// Target: analysis.bigb

<h4 id="bezier-derivative-control-polygon">Bézier derivative control polygon</h4>

↑ **Parent:** [Bézier curve](#bezier-curve)

For a degree-$n$ [Bézier curve](#bezier-curve), the $r$th [derivative](calculus.md#derivative) has degree at most $n-r$ and [control points](#control-point) $n!\Delta^rP_j/(n-r)!$. The first [derivative](calculus.md#derivative) follows by differentiating the [Bernstein basis](functional-analysis.md#bernstein-basis) and shifting one summation index; iteration proves the general formula. A parameter interval of length $h$ multiplies these [derivative](calculus.md#derivative) controls by $h^{-r}$.

<h5 id="parametric-first-derivative-join-of-bezier-curves">Parametric first-derivative join of Bézier curves</h5>

↑ **Parent:** [Bézier derivative control polygon](#bezier-derivative-control-polygon)

Two adjacent [Bézier curves](#bezier-curve) of degrees $n,m$ and interval lengths $h,k$ have a $C^1$ join precisely when their endpoint positions and their [derivatives](calculus.md#derivative) in the common parameter agree. Parallel endpoint polygon edges alone give tangent-direction agreement; their scaled vectors must be equal for parametric first-derivative [continuity](calculus.md#continuous-function).

<h4 id="de-casteljau-s-algorithm">De Casteljau's algorithm</h4>

↑ **Parent:** [Bézier curve](#bezier-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Casteljau's_algorithm)

[De Casteljau's algorithm](#de-casteljau-s-algorithm) repeatedly replaces neighboring control points by $(1-t)B_j+tB_{j+1}$ until a single point remains. The same triangular construction gives both subcurves split at $t$.

// Target: analysis.bigb

### Bounding volume

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounding_volume)

A [bounding volume](#bounding-volume) encloses an object. Disjoint [bounding volumes](#bounding-volume) certify that their enclosed objects do not meet.

// Target: analysis.bigb

#### Bounding volume hierarchy

↑ **Parent:** [Bounding volume](#bounding-volume)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounding_volume_hierarchy)

A [bounding volume hierarchy](#bounding-volume-hierarchy) stores enclosing volumes in a tree, with each internal volume enclosing all descendants. Collision detection descends only through pairs of overlapping volumes.

// Target: optics.bigb

#### Axis-aligned bounding box

↑ **Parent:** [Bounding volume](#bounding-volume)

An [axis-aligned bounding box](#axis-aligned-bounding-box) is the product of coordinate intervals containing an object. Overlap requires overlap in every coordinate interval.

// Target: analysis.bigb

### Triangle-triangle intersection algorithm

↑ **Parent:** [Computer aided geometric design](#computer-aided-geometric-design)

For two noncoplanar [triangles](geometry-and-topology.md#triangle), first reject vertices strictly on one side of the other triangle's plane. Otherwise intersect each triangle with the other plane and compare the resulting intervals along the common line. Coplanar triangles require a planar overlap test; zero-area triangles require separate [line segment](mathematical-optimization.md#line-segment) or point tests.

// Target: analysis.bigb

## Round-off error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

Round-off error arises from representing numbers and performing arithmetic at finite precision. It is distinct from discretization error. Cancellation, ill-conditioning and accumulation can amplify it, so decreasing a mesh size or time step indefinitely need not improve the final accuracy.

## Richardson extrapolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Richardson_extrapolation)

If $Y_h=Y+Ch^p+o(h^p)$, combine two resolutions with the displayed formula to cancel the leading error. A further term in the asymptotic expansion determines the new order; cancellation alone does not guarantee any particular next power. In [step-doubling error estimation](#step-doubling-error-estimation), the accumulated fine local error has ratio $2^{-p}$ because two half steps each contribute order $h^{p+1}$.

## Error control for ODE solvers

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

Error control selects discretization parameters and checks approximations against requested accuracy. [Local error estimators](#local-error-estimator), [absolute and relative error tolerances](#absolute-and-relative-error-tolerances) and an [adaptive step-size controller](#adaptive-step-size-controller) provide practical local control. Propagation of defects determines the [global error](#global-discretization-error), while stiffness, [roundoff error](#round-off-error) and algebraic-solve accuracy impose additional limits.

### Adaptive step-size controller

↑ **Parent:** [Error control for ODE solvers](#error-control-for-ode-solvers)

If a scaled [local error estimator](#local-error-estimator) behaves as $E\propto h^r$, the displayed update targets a fixed local level. A safety factor $\eta<1$, minimum/maximum change factors and rejected-step rollback improve robustness. A zero estimate needs finite capped growth. For an embedded $p/(p-1)$ pair, usually $r=p$; for a true order-$p$ exact-start defect, $r=p+1$. Controllers using previous estimates can smooth step sequences. The [GSL ODE documentation](https://www.gnu.org/software/gsl/doc/html/ode-initval.html) illustrates component error scaling, safety factors and growth limits in an actual solver; controller-specific exponents depend on how the solver defines its error estimate.

### Absolute and relative error tolerances

↑ **Parent:** [Error control for ODE solvers](#error-control-for-ode-solvers)

Absolute tolerances provide a nonzero error scale near zero, while relative tolerances follow component magnitude. A max-norm test $\max_i|\widehat e_i|/s_i\leq1$ controls every scaled estimated component locally. A root-mean-square test has a different componentwise implication. Neither test automatically certifies the complete trajectory's [global error](#global-discretization-error).

### Local error estimator

↑ **Parent:** [Error control for ODE solvers](#error-control-for-ode-solvers)

A local error estimator approximates a numerical step's defect from the exact solution starting at the same input. Differences between formulas estimate error only after their asymptotic orders and constants are accounted for. [Step-doubling error estimation](#step-doubling-error-estimation), an [embedded Runge-Kutta pair](#embedded-runge-kutta-pair) and [predictor-corrector error estimation](#predictor-corrector-error-estimation) are common constructions. They do not by themselves bound accumulated [global error](#global-discretization-error).

#### Predictor-corrector error estimation

↑ **Parent:** [Local error estimator](#local-error-estimator)

A predictor and corrector give distinct approximations from the same local history. Their difference, scaled by their leading error constants and orders, can estimate a local defect. Raw differences without that calibration need not estimate the corrected solution's error. Variable-step [multistep methods](#linear-multistep-method) also require updated coefficients and controlled history handling.

#### Embedded Runge-Kutta pair

↑ **Parent:** [Local error estimator](#local-error-estimator)

Two [Runge-Kutta methods](#runge-kutta-method) share a stage matrix and nodes but use different output weights. An order-$p$ and order-$q$ pair with $q<p$ gives an output difference generally of order $h^{q+1}$, estimating the lower-order defect. Shared stage evaluations reduce the cost. The [adaptive step-size controller](#adaptive-step-size-controller) exponent must reflect this estimator order, rather than blindly the higher reported solution order.

#### Step-doubling error estimation

↑ **Parent:** [Local error estimator](#local-error-estimator)

For an order-$p$ one-step method with leading numerical error $Ch^{p+1}$, two half steps have leading error $Ch^{p+1}/2^p$. The displayed difference estimates exact minus the finer approximation. Adding it implements [Richardson extrapolation](#richardson-extrapolation). It requires a common starting value, the smooth local expansion, and accuracy of all algebraic solves; it can fail across a nonsmooth event.

## Finite volume method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_volume_method)

A finite volume method evolves cell integrals or cell averages by differences of shared interface [numerical fluxes](#numerical-flux). For a [scalar conservation law](partial-differential-equation.md#scalar-conservation-law), $U_j^{n+1}=U_j^n-(k/d)(F_{j+1/2}-F_{j-1/2})$. Sharing the same flux between neighboring cells makes conservation follow by telescoping.

### Monotone conservative scheme

↑ **Parent:** [Finite volume method](#finite-volume-method)

A scalar finite-volume update is monotone if increasing any input state cannot decrease any output state. A consistent conservative update preserves constants and has an invariant interval by comparison. On a periodic grid, or an infinite grid with summable perturbations, conservation and monotonicity imply [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme). Translation invariance then implies the [total variation diminishing scheme](#total-variation-diminishing-scheme) property.

#### Total variation diminishing scheme

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

A translation-invariant conservative monotone update decreases discrete [total variation](real-analysis.md#total-variation). If $S$ is the one-cell shift, $TS=ST$, and [L1 contraction of a monotone conservative scheme](#l1-contraction-of-a-monotone-conservative-scheme) applied to $U,SU$ gives $\sum_j|(TU)_{j+1}-(TU)_j|\leq\sum_j|U_{j+1}-U_j|$. This prevents creation of new total variation, though it does not make every discontinuity sharply resolved.

#### L1 contraction of a monotone conservative scheme

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

Let $T$ be a monotone conservative scalar update on a periodic grid. Since $T(U\vee V)\geq TU,TV$, one has $(TU-TV)_+\leq T(U\vee V)-TV$. Conservation makes the sum of the right side equal to $\sum(U-V)_+$. Reverse $U,V$ and add to obtain $\|TU-TV\|_1\leq\|U-V\|_1$. On an infinite grid the same proof holds for summable differences with a Lipschitz flux on the state range.

#### Engquist-Osher method

↑ **Parent:** [Monotone conservative scheme](#monotone-conservative-scheme)

The Engquist-Osher method is the [finite volume method](#finite-volume-method) using the [Engquist-Osher flux](#engquist-osher-flux). Under $(k/d)\sup|f\prime|\leq1$ on the invariant state interval, its update is monotone. It preserves the state range, is contractive for summable perturbations in $L^1$, and decreases discrete [total variation](real-analysis.md#total-variation).

##### CFL necessity for explicit Engquist-Osher stability

↑ **Parent:** [Engquist-Osher method](#engquist-osher-method)

[Monotonicity](calculus.md#monotonic-function) of the explicit update requires $(k/h)\sup_{[m,M]}|f'|\le1$ on its invariant state interval. [Convexity](real-analysis.md#convex-function) and a unique [sonic point of a scalar flux](partial-differential-equation.md#sonic-point-of-a-scalar-flux) do not remove this time-step restriction. For $f(u)=u^2/2$, linearization about a positive constant $U$ gives an [upwind finite difference scheme](finite-difference.md#upwind-finite-difference-scheme) for [advection equation](partial-differential-equation.md#transport-equation): $v_j^{n+1}=(1-rU)v_j^n+rUv_{j-1}^n$, where $r=k/h$. At [Fourier frequency](#fourier-frequency) $\pi$ the multiplier is $1-2rU$, whose modulus exceeds one when $rU>1$. Thus a [CFL condition](finite-difference.md#courant-friedrichs-lewy-condition) is essential to the claimed nonlinear [stability](#stability-of-a-numerical-method).

##### Engquist-Osher flux

↑ **Parent:** [Engquist-Osher method](#engquist-osher-method)

The Engquist-Osher [numerical flux](#numerical-flux) is $F(a,b)=f(0)+\int_0^a\max(f\prime(s),0)ds+\int_0^b\min(f\prime(s),0)ds$. It sends positive-speed contributions from the left state and negative-speed contributions from the right state. Its consistency $F(u,u)=f(u)$ and opposite monotonicities in the two arguments yield a [monotone conservative scheme](#monotone-conservative-scheme) under the appropriate [Courant–Friedrichs–Lewy condition](finite-difference.md#courant-friedrichs-lewy-condition). For the [Inviscid Burgers equation](partial-differential-equation.md#inviscid-burgers-equation), it is $\tfrac12\max(a,0)^2+\tfrac12\min(b,0)^2$.

###### Sonic-point splitting of a convex Engquist-Osher flux

↑ **Parent:** [Engquist-Osher flux](#engquist-osher-flux)

For a flux that is a differentiable [convex function](real-analysis.md#convex-function) with unique minimum at $s_*$, define $f^+(u)=f(u)-f(s_*)$ for $u>s_*$ and zero otherwise, and $f^-(u)=f(u)-f(s_*)$ for $u<s_*$ and zero otherwise. The [Engquist-Osher flux](#engquist-osher-flux) is $F(a,b)=f(s_*)+f^+(a)+f^-(b)$. Thus transsonic [rarefaction wave](partial-differential-equation.md#rarefaction-wave) states $a\le s_*\le b$ give $F=f(s_*)$, while reversed transsonic states give $F=f(a)+f(b)-f(s_*)$. This follows by integrating the positive and negative parts of $f'$.

### Numerical flux

↑ **Parent:** [Finite volume method](#finite-volume-method)

A numerical flux approximates the transported quantity through a cell interface using nearby states. For a two-state flux $F(a,b)$ approximating a [scalar conservation law](partial-differential-equation.md#scalar-conservation-law) with flux $f$, consistency requires $F(u,u)=f(u)$. A [monotone conservative scheme](#monotone-conservative-scheme) uses a flux nondecreasing in its left state and nonincreasing in its right state, with a time step making the complete update monotone.

#### Godunov numerical flux

↑ **Parent:** [Numerical flux](#numerical-flux)

For a [scalar conservation law](partial-differential-equation.md#scalar-conservation-law) whose flux is a [convex function](real-analysis.md#convex-function), the [Godunov numerical flux](#godunov-numerical-flux) is the physical flux at the origin of the [entropy solution](partial-differential-equation.md#entropy-solution) of the [Riemann problem](partial-differential-equation.md#riemann-problem) between states $a,b$. It is $\min_{u\in[a,b]}f(u)$ for $a\le b$ and $\max_{u\in[b,a]}f(u)$ for $a>b$. For a [rarefaction wave](partial-differential-equation.md#rarefaction-wave), the [characteristic speed](partial-differential-equation.md#characteristic-speed) is monotone across its states, so the origin sees either an endpoint or a zero-speed minimizing state. For a [shock wave](partial-differential-equation.md#shock-wave), its speed is $(f(a)-f(b))/(a-b)$; the origin sees the left state if this speed is positive and the right state if negative, selecting the larger endpoint flux. Unlike the [Godunov flux](#godunov-numerical-flux), the [Engquist-Osher flux](#engquist-osher-flux) at reversed transsonic states may equal $f(a)+f(b)-f(s_*)$.

## Interval bisection

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a continuous increasing scalar function, retain an interval whose endpoints bracket a target value, evaluate its midpoint, and keep the half that still brackets the target. Each step halves the interval length. Applied to a strictly increasing water-level equation, this finds its unique solution to any specified error tolerance.

## Implicit time-stepping method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An implicit time-stepping method determines a new solution value through an equation involving that same value. A small-step [contraction mapping](analysis.md#contraction-mapping) argument often establishes local solvability when the vector field is [Lipschitz continuous](real-analysis.md#lipschitz-continuity). Examples include the [Backward Euler method](#backward-euler-method), [implicit Runge-Kutta methods](#implicit-runge-kutta-method) and implicit [linear multistep methods](#linear-multistep-method). Solvability of the update is a separate issue from [stability of a numerical method](#stability-of-a-numerical-method).

## Multigrid method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multigrid_method)

A [multigrid method](#multigrid-method) combines relaxation of high-frequency fine-grid errors with [coarse-grid correction](#coarse-grid-correction) of smooth errors. Residual restriction, an approximate coarse error solve, error prolongation and post-smoothing form a two-grid cycle; recursive coarse solves give multilevel cycles.

### Full multigrid

↑ **Parent:** [Multigrid method](#multigrid-method)

Full multigrid solves first on a coarse mesh, interpolates that approximation to the next finer mesh, and applies a fixed number of [geometric multigrid V-cycles](#geometric-multigrid-v-cycle) before proceeding to the next level. If interpolation introduces only the expected discretization-scale error and the cycle count reduces the inherited error sufficiently at every level, the final algebraic error matches the fine-grid discretization error. The geometric sum of level costs is then $O(N)$, unlike reducing an arbitrary fine-grid initial error by an arbitrarily small tolerance.

### Two-grid Poisson factor with weighted Jacobi

↑ **Parent:** [Multigrid method](#multigrid-method)

For the one-dimensional [Poisson equation](partial-differential-equation.md#poisson-equation), use linear interpolation, [full-weighting restriction](#full-weighting-restriction), an exact coarse solve, and one pre- and one post-sweep of [weighted Jacobi](#weighted-jacobi-method) with weight $2/3$. On a pair of harmonics $\theta,\theta+\pi$, put $s=\sin^2(\theta/2)$ and $c=1-s$. The coarse correction is $C=\left(\begin{smallmatrix}s&-c\\-s&c\end{smallmatrix}\right)$, and the smoother is $S=\operatorname{diag}(1-4s/3,1-4c/3)$. The rank-one error operator $SCS$ has nonzero eigenvalue $s(1-4s/3)^2+c(1-4c/3)^2=1/9$. This exact harmonic calculation illustrates mesh-independent two-grid contraction for the constant-coefficient model; it is not an unconditional result for arbitrary operators or transfer choices.

### Geometric multigrid V-cycle

↑ **Parent:** [Multigrid method](#multigrid-method)

A geometric multigrid V-cycle pre-smooths an approximate solution, restricts its residual, recursively solves the coarse error equation once from zero, prolongs and adds that error correction, and post-smooths. The recursion ends in a direct solve on a small coarsest grid. With fixed sweep counts and bounded stencil work, coarsening in $d$ dimensions gives total work $O(N)\sum_{j\geq0}2^{-dj}=O(N)$ per cycle. A mesh-independent convergence factor also requires compatible coarse approximation and effective smoothing; linear work alone does not prove convergence.

### Full-weighting restriction

↑ **Parent:** [Multigrid method](#multigrid-method)

Full-weighting restriction transfers a fine-grid residual to a coarser grid by local averaging. In one dimension its weights are $(1,2,1)/4$; in two dimensions they are the tensor-product stencil $\left(\begin{smallmatrix}1&2&1\\2&4&2\\1&2&1\end{smallmatrix}\right)/16$. For linear or bilinear interpolation $P$ and coarsening by two in every direction, it equals $2^{-d}P^T$ in unweighted coordinates. This scaling makes restriction the adjoint of interpolation for mesh-weighted inner products.

### Coarse-grid correction

↑ **Parent:** [Multigrid method](#multigrid-method)

For residual $r_h=b_h-A_hu_h$, restrict to a coarse grid, solve $A_He_H=Rr_h$ approximately, and update $u_h$ by $Pe_H$. This corrects error that is smooth on the fine grid but representable on the coarse grid.

#### Galerkin coarse-grid operator

↑ **Parent:** [Coarse-grid correction](#coarse-grid-correction)

A Galerkin coarse-grid operator is obtained by composing interpolation, the fine operator and residual restriction. With $R=cP^T$, $c>0$, and positive-definite $A_h$, the exact [coarse-grid correction](#coarse-grid-correction) $I-P(RA_hP)^{-1}RA_h$ is the energy-orthogonal projection onto the complement of the coarse space. Indeed it annihilates every vector $Pz$, and its corrected error $e'$ satisfies $P^TA_he'=0$. These identities explain why compatible transfers remove representable smooth error rather than merely averaging an approximate solution.

## Convergence of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For an [initial value problem](differential-equation.md#initial-value-problem), convergence means that the largest [global error](#global-discretization-error) on each fixed finite time interval tends to zero as the step size tends to zero and the starting errors vanish. For [linear multistep methods](#linear-multistep-method), the [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem) separates this requirement into [consistency of a numerical method](#consistency-of-a-numerical-method) and [zero-stability](#zero-stability).

### Quadratic convergence

↑ **Parent:** [Convergence of a numerical method](#convergence-of-a-numerical-method)

An iteration converges at least quadratically to a limit if its errors eventually satisfy the displayed bound with a fixed finite $C>0$. If $Ce_N<1$, induction gives $|e_{N+k}|\le C^{-1}(C|e_N|)^{2^k}$. Exact asymptotic quadratic convergence has $|e_{n+1}|/|e_n|^2\to c\in(0,\infty)$. [Newton root-finding iteration](#newton-root-finding-iteration) at a simple scalar root has this order when the second derivative at the root is nonzero; if that derivative vanishes, convergence can be faster.

## Global discretization error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The [global error](#global-discretization-error) is the difference between the computed and exact solutions after accumulated numerical steps, rather than the [local truncation error](#local-truncation-error) of a single step started from exact data. An estimate for the [stability of a numerical method](#stability-of-a-numerical-method) controls how initial errors and local defects accumulate. For a stable order-$p$ time integrator with starting errors $O(h^p)$, local defects $O(h^{p+1})$ accumulated over $O(1/h)$ steps give [global error](#global-discretization-error) $O(h^p)$ on a fixed time interval.

### Variable-step global ODE error bound

↑ **Parent:** [Global discretization error](#global-discretization-error)

If a one-step map is Lipschitz with factor at most $1+Lh_n$ and its exact-start defect is at most $Ch_n^{p+1}$, iteration of the error recurrence gives the displayed global bound on a time interval of length $T$. Since $\sum h_n\leq T$, the defect sum is at most $T(\max h_n)^p$. Local tolerance control alone is not a global accuracy certificate: propagation, the number of steps, stiffness, roundoff and nonlinear-solve errors also enter. The [discrete Gronwall inequality](probability-and-statistics.md#discrete-gronwall-inequality) organizes this distinction.

### Residual bound for global ODE error

↑ **Parent:** [Global discretization error](#global-discretization-error)

For a differentiable approximation $\eta$, put $d=\eta'-f(t,\eta)$. If $f$ is [Lipschitz continuous](real-analysis.md#lipschitz-continuity) with constant $L$ on the relevant region, the exact solution's error satisfies the displayed bound by [Gronwall's inequality](probability-and-statistics.md#gronwall-inequality). Thus a bound on the residual over the whole interval supplies an a posteriori [global error](#global-discretization-error) estimate. A small estimated defect at a single step does not furnish this bound by itself.

## Midpoint quadrature rule

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The midpoint quadrature rule approximates an integral on $[a,b]$ by

$$
\int_a^bf(x)\,dx\approx(b-a)f\left(\frac{a+b}{2}\right).
$$

It is exact for linear polynomials.

## Truncation error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Truncation_error)

A truncation error is the error introduced by replacing an exact mathematical operation with a finite approximation, such as replacing a [derivative](calculus.md#derivative) by a [finite difference](finite-difference.md).

## Spectral method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_method)

A spectral method approximates a differential equation in a global basis and enforces the equation after projection or collocation. Smooth and analytic solutions often give rapidly convergent coefficients.

### Spectral accuracy

↑ **Parent:** [Spectral method](#spectral-method)

A [spectral method](#spectral-method) has [spectral accuracy](#spectral-accuracy) for a class of smooth data when its error decreases faster than any fixed inverse power of the truncation size. For periodic [Fourier series](fourier-series.md), this follows from arbitrarily many integrations by parts when every derivative matches across the periodic boundary. An analytic periodic extension to a complex strip gives exponential coefficient decay. Analyticity inside one period and matching only endpoint values do not suffice: a jump in a derivative of the periodic extension yields algebraic decay instead.

### Fourier spectral method

↑ **Parent:** [Spectral method](#spectral-method)

A Fourier spectral method represents a periodic unknown by finitely many [Fourier modes](fourier-analysis.md#fourier-mode) and converts differentiation into multiplication by wavenumber.

#### Spectral truncation

↑ **Parent:** [Fourier spectral method](#fourier-spectral-method)

A spectral truncation retains a finite set of basis modes and sets all omitted coefficients to zero.

#### Fourier spectral system for a cosine-modulated second derivative

↑ **Parent:** [Fourier spectral method](#fourier-spectral-method)

For the two-periodic problem

$$
-\frac{1+2\cos\pi x}{\pi^2}u''+u=f,
$$

the Fourier coefficients satisfy the tridiagonal system

$$
(m-1)^2\widehat u_{m-1}
+(m^2+1)\widehat u_m
+(m+1)^2\widehat u_{m+1}
=\widehat f_m,
\qquad m\in\mathbb Z.
$$

<h4 id="fourier-galerkin-method">Fourier–Galerkin method</h4>

↑ **Parent:** [Fourier spectral method](#fourier-spectral-method)

The Fourier–Galerkin method seeks a finite [Fourier series](fourier-series.md) whose residual is orthogonal to every retained [Fourier mode](fourier-analysis.md#fourier-mode).

## Stability of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a numerical evolution, stability means that perturbations of the initial data and forcing remain bounded over a fixed time interval, with a bound independent of the discretization parameters. For a linear homogeneous recurrence, a mesh-uniform bound on powers of its update [matrix](vector-space.md#matrix) provides this estimate. [von Neumann stability analysis](finite-difference.md#von-neumann-stability-analysis) and the [energy method](#energy-method) are two complementary ways to establish it.

## Consistency of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

A numerical method is consistent when its local defect tends to zero at the rate required to approximate the differential equation. Stability then determines whether these local defects accumulate into a convergent global approximation.

### Order of a numerical method

↑ **Parent:** [Consistency of a numerical method](#consistency-of-a-numerical-method)

For a time-stepping formula written with an unscaled step residual $R_h$, order at least $p$ means that substituting a smooth exact solution gives $R_h=O(h^{p+1})$. Under the relevant [stability of a numerical method](#stability-of-a-numerical-method) assumptions and starting errors $O(h^p)$, this produces [global error](#global-discretization-error) $O(h^p)$. Residuals divided by the step size instead use the equivalent convention $O(h^p)$.

#### Local truncation error

↑ **Parent:** [Order of a numerical method](#order-of-a-numerical-method)

The local truncation error is the defect left when exact solution values are inserted into a numerical update. For a one-step method started from the exact solution,

$$
\tau_{n+1}
=y(t_{n+1})-y(t_n)-h\phi(t_n,y(t_n),h).
$$

A local error $O(h^{p+1})$ generally leads to global error $O(h^p)$ under a uniform stability bound.

##### Normalized local truncation error

↑ **Parent:** [Local truncation error](#local-truncation-error)

For a time update with one-step defect $\delta_{h,k}$ after exact solution values are inserted, the normalized defect divides by the time step $k$. If $\delta_{h,k}=O(k^{p+1})$, the normalized [local truncation error](#local-truncation-error) is $O(k^p)$. A spatial mesh contributes its own powers: for a diffusion update, $\mathcal T_{h,k}=O(k+h^2)$ means $\delta_{h,k}=O(k^2+kh^2)$. Under $k=O(h^2)$ these are respectively second and fourth powers of $h$. Neither normalization changes the actual [order of a numerical method](#order-of-a-numerical-method); it changes the power used to express its residual.

## Energy method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The energy method differentiates a norm or quadratic energy along a differential equation or numerical evolution and estimates the resulting terms. Dissipative, skew-adjoint, and boundary contributions can yield stability or conservation without diagonalizing the operator.

### Dirichlet convection-diffusion contraction

↑ **Parent:** [Energy method](#energy-method)

For zero endpoint values and real constant drift, integration by parts gives $\tfrac12 d\|u\|_{L^2}^2/dt=-\|u_x\|_{L^2}^2$. The drift contributes only a zero boundary term in the real part. Thus the solution is contractive, uniformly in the drift. Multiplication by $e^{\kappa x}$ converts the equation to a [heat equation](diffusion-equation.md#heat-equation) with constant killing rate $\kappa^2$, providing existence and uniqueness as well as the direct [energy estimate](partial-differential-equation.md#energy-estimate).

### Periodic centered advection-diffusion contractivity

↑ **Parent:** [Energy method](#energy-method)

The semidiscrete system $U'=D_{xx}U+\alpha D_0U$, for real fixed $\alpha$, is contractive in the periodic discrete [L2 norm](real-analysis.md#l2-norm). [Discrete summation by parts](finite-difference.md#discrete-summation-by-parts) makes the drift term's real energy contribution zero and the diffusion term nonpositive. Equivalently its [Fourier amplification symbol](finite-difference.md#fourier-amplification-symbol) generator has real part $-4h^{-2}\sin^2(\theta/2)$. This continuous-time estimate does not prove stability of an arbitrarily chosen time integrator.

### Centered Dirichlet drift-diffusion energy identity

↑ **Parent:** [Energy method](#energy-method)

For the centered second difference and centered first difference on a finite interval with zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the diffusion [matrix](vector-space.md#matrix) is symmetric negative definite and the drift [matrix](vector-space.md#matrix) is [skew-symmetric](linear-algebra.md#skew-symmetric-matrix). Discrete [summation by parts](analytic-number-theory.md#abel-s-summation-formula) gives the displayed mesh-weighted identity. It proves contraction in the discrete [L2 norm](real-analysis.md#l2-norm) without needing periodic modes, positive stencil coefficients or simultaneous diagonalization.

### Energy stability for variable-coefficient reaction diffusion

↑ **Parent:** [Energy method](#energy-method)

For a zero-boundary centered semidiscretization $U'=D_hU+V_hU$, where $D_h$ is the scaled [Dirichlet discrete Laplacian](finite-difference.md#dirichlet-discrete-laplacian) and $V_h=\operatorname{diag}(a_j)$ with $a_j\leq a_+$, [summation by parts](analytic-number-theory.md#abel-s-summation-formula) gives $(U,D_hU)_h\leq0$. Hence $\tfrac12(d/dt)\|U\|_h^2\leq a_+\|U\|_h^2$. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) yields $\|U(t)\|_h\leq e^{a_+t}\|U(0)\|_h$, a mesh-independent [stability](#stability-of-a-numerical-method) bound on every fixed finite interval. Positive reaction coefficients can permit physical growth without violating this form of [stability](#stability-of-a-numerical-method).

### Uniqueness of Sobolev weak solutions of a wave equation

↑ **Parent:** [Energy method](#energy-method)

For the [weak energy solution of a variable-coefficient wave equation](partial-differential-equation.md#weak-energy-solution-of-a-variable-coefficient-wave-equation), uniqueness can be proved without using $u_t$ as a spatial $H_0^1$ test function. For a difference with zero data, fix $s$ and test by $v(t)=\int_t^su(r)dr$ for $t<s$, extended by zero afterwards. Put $z(t)=\int_0^tu(r)dr$, so $v(t)=z(s)-z(t)$. [Integration by parts](calculus.md#integration-by-parts) in time for the symmetric principal form, and in space for the first-order terms, give

$$
\|u(s)\|_2^2+\theta\|Dz(s)\|_2^2
\leq C\int_0^s\bigl(\|u(t)\|_2^2+\|Dz(t)\|_2^2\bigr)dt+Cs\|Dz(s)\|_2^2.
$$

For short enough intervals the last term is absorbed. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) forces $u=0$, and repetition proves uniqueness on the full interval. This antiderivative test is valid at the stated space-time $H^1$ regularity, unlike an unqualified direct energy test by $u_t$.

## Finite element method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_element_method)

The finite element method approximates a variational problem in a finite-dimensional space of piecewise polynomial functions and determines the coefficients by testing against the same trial space.

### Semidiscrete finite element heat equation

↑ **Parent:** [Finite element method](#finite-element-method)

The spatial [Galerkin method](partial-differential-equation.md#galerkin-method) for the [heat equation](diffusion-equation.md#heat-equation) gives a [mass matrix](#mass-matrix) $M$ and a diffusion [stiffness matrix](#stiffness-matrix) $S$. With zero forcing, $\frac{d}{dt}(c^TMc)=-2c^TSc\leq0$. The [quadratic form](linear-algebra.md#quadratic-form) $c^TMc$ is the squared [L2 norm](real-analysis.md#l2-norm) of the represented finite-element function, proving an energy contraction. For nonzero forcing, the corresponding identity has the additional term $2c^TF$, which can be estimated using the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

#### Forward Euler limit for a consistent hat mass matrix

↑ **Parent:** [Semidiscrete finite element heat equation](#semidiscrete-finite-element-heat-equation)

For a uniform piecewise-linear Galerkin heat discretization, the consistent [mass matrix](#mass-matrix) is $M=(h/6)\operatorname{tridiag}(1,4,1)$ and the [stiffness matrix](#stiffness-matrix) is $K=h^{-1}\operatorname{tridiag}(-1,2,-1)$. The generalized [eigenvalues](linear-operator-theory.md#eigenvalue) are $6(1-\cos\theta)/[h^2(2+\cos\theta)]$. Applying [Forward Euler method](#euler-method) requires $k\lambda\leq2$, giving the displayed uniform bound for $\mu=k/h^2$. For $J$ intervals with Dirichlet endpoints the exact finite-grid upper bound is $(2-\cos(\pi/J))/[3(1+\cos(\pi/J))]$, which approaches $1/6$. Replacing the consistent [mass matrix](#mass-matrix) by a lumped one changes the [stability](#stability-of-a-numerical-method) restriction.

### Finite element

↑ **Parent:** [Finite element method](#finite-element-method)

A finite element specifies a reference region, a finite-dimensional space of local trial functions, and degrees of freedom that uniquely determine each such function. Assembling compatible copies over a [finite element mesh](#finite-element-mesh) gives a global trial space. For a one-dimensional linear element, the region is an interval, the functions are [affine functions](vector-space.md#affine-function), and the degrees of freedom are the endpoint values.

### Conforming finite element space

↑ **Parent:** [Finite element method](#finite-element-method)

A conforming finite element space is a finite-dimensional [vector subspace](vector-space.md#vector-subspace) of the solution's variational space $V$. For a second-order problem with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), continuous piecewise-polynomial functions vanishing on the boundary form such a subspace of the [zero-boundary Sobolev space](sobolev-space.md#zero-boundary-sobolev-space) $H_0^1(\Omega)$. Conformity allows exact [Galerkin orthogonality](#galerkin-orthogonality) and the [Céa lemma](#cea-s-lemma).

### Finite element mesh

↑ **Parent:** [Finite element method](#finite-element-method)

A finite element mesh partitions the domain into simple elements, such as intervals, triangles or tetrahedra. Piecewise-polynomial trial functions and local integration assemble the [stiffness matrix](#stiffness-matrix) and [mass matrix](#mass-matrix).

#### Shape-regular mesh

↑ **Parent:** [Finite element mesh](#finite-element-mesh)

A family of simplicial meshes is shape-regular when the ratio of each element's diameter to its inscribed-ball radius stays uniformly bounded. This excludes degenerating shapes and makes [finite element interpolation estimates](#finite-element-interpolation-estimate) uniform in the mesh size. The element sizes may still vary substantially across the domain.

### Finite element interpolation estimate

↑ **Parent:** [Finite element method](#finite-element-method)

On a [shape-regular mesh](#shape-regular-mesh) in dimensions at most three, nodal piecewise-linear interpolation of $u\in H^2(\Omega)$ satisfies

$$
\|u-I_hu\|_{L^2(\Omega)}+h\|u-I_hu\|_{H^1(\Omega)}
\leq Ch^2\|u\|_{H^2(\Omega)},
$$

where $h$ is the largest element diameter and $C$ is independent of $h$. For homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), $I_hu$ belongs to the [conforming finite element space](#conforming-finite-element-space). Scaling each element to a reference element gives the estimate; [shape regularity](#shape-regular-mesh) bounds the scaling constants, while subtraction of an [affine function](vector-space.md#affine-function) leaves an error controlled by the second derivatives.

### Mass matrix

↑ **Parent:** [Finite element method](#finite-element-method)

The mass matrix is the [Gram matrix](linear-algebra.md#gram-matrix) of a [finite element](#finite-element) basis in the [L2 inner product](measure-theory.md#l2-inner-product). Its coefficient [quadratic form](linear-algebra.md#quadratic-form) is the squared [L2 norm](real-analysis.md#l2-norm) of the represented trial function, so it is a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) for a linearly independent basis.

#### Mass eigenstate

↑ **Parent:** [Mass matrix](#mass-matrix)

A [mass eigenstate](#mass-eigenstate) diagonalizes the Hermitian [mass](classical-mechanics.md#mass) operator or [mass matrix](#mass-matrix) and has a definite [mass](classical-mechanics.md#mass). In a flavor basis with off-diagonal [mass](classical-mechanics.md#mass) terms, it is a linear combination of flavor states. For unstable particles, decay propagation instead involves an effective complex matrix; its [eigenvectors](linear-operator-theory.md#eigenvector) need not inherit the orthogonality of a Hermitian [mass](classical-mechanics.md#mass) problem.

#### Affine-weighted hat mass matrix

↑ **Parent:** [Mass matrix](#mass-matrix)

On a one-dimensional uniform [finite element mesh](#finite-element-mesh) of spacing $h$, let $w$ be an [affine function](vector-space.md#affine-function) and $\phi_i$ the interior [piecewise-linear hat functions](#piecewise-linear-hat-function). The weighted [mass matrix](#mass-matrix) has entries

$$
W_{ii}=\frac{2h}{3}w(x_i),\qquad
W_{i,i+1}=W_{i+1,i}=\frac h{12}\bigl(w(x_i)+w(x_{i+1})\bigr),
$$

and zero entries for nonadjacent indices. The diagonal product $\phi_i^2$ is symmetric about $x_i$ and integrates to $2h/3$; the neighbouring product is symmetric about $(x_i+x_{i+1})/2$ and integrates to $h/6$. The odd part of an [affine function](vector-space.md#affine-function) integrates to zero around each centre, giving the formulas. This evaluates a variable reaction term exactly without substituting a constant coefficient or a quadrature approximation.

### Stiffness matrix

↑ **Parent:** [Finite element method](#finite-element-method)

The stiffness matrix represents a variational [bilinear form](linear-algebra.md#bilinear-form) $a$ in a [finite element](#finite-element) basis. A symmetric [coercive bilinear form](linear-algebra.md#coercive-bilinear-form) gives a [positive-definite matrix](linear-algebra.md#positive-definite-matrix). Local support of the [piecewise-linear hat functions](#piecewise-linear-hat-function) produces a sparse [matrix](vector-space.md#matrix), allowing efficient numerical solution.

#### Reaction-diffusion finite element matrix

↑ **Parent:** [Stiffness matrix](#stiffness-matrix)

For $-u''+u=f$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the conforming [piecewise-linear hat functions](#piecewise-linear-hat-function) on a uniform grid give a diffusion [stiffness matrix](#stiffness-matrix) $S$ and a [mass matrix](#mass-matrix) $M$. Their nonzero entries are $S_{ii}=2/h$, $S_{i,i+1}=-1/h$, $M_{ii}=2h/3$, and $M_{i,i+1}=h/6$, with symmetric counterparts. The sum is a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) because its coefficient [quadratic form](linear-algebra.md#quadratic-form) is $\int((u_h')^2+u_h^2)$. For forcing $f(x)=x$, the load at $x_i$ is $hx_i$.

### Energy conservation for semidiscrete Galerkin advection

↑ **Parent:** [Finite element method](#finite-element-method)

For periodic $u_t=u_x$, the conforming [Galerkin method](partial-differential-equation.md#galerkin-method) has $M\dot U=CU$, with [mass matrix](#mass-matrix) $M_{ij}=\int\phi_i\phi_j$ and $C_{ij}=\int\phi_i\phi_j'$. [Integration by parts](calculus.md#integration-by-parts) and periodicity give $C^T=-C$. Therefore

$$
\frac{d}{dt}(U^TMU)=2U^TCU=0.
$$

The conserved quantity is the squared [L2 norm](real-analysis.md#l2-norm) of the [finite element](#finite-element) function. On a uniform one-dimensional mesh of spacing $h$, the [piecewise-linear hat functions](#piecewise-linear-hat-function) give $M_{ii}=2h/3$, $M_{i,i\pm1}=h/6$, $C_{i,i+1}=1/2$ and $C_{i,i-1}=-1/2$.

### Cubic Hermite finite element

↑ **Parent:** [Finite element method](#finite-element-method)

A cubic Hermite finite element is piecewise cubic and joins with continuous first derivative. It is therefore conforming for fourth-order variational problems whose energy space lies in $H^2$.

### Rayleigh-Ritz method

↑ **Parent:** [Finite element method](#finite-element-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh–Ritz_method)

The Ritz method minimizes a quadratic energy over a finite-dimensional trial space. For basis functions $\phi_j$ and bilinear form $a$, its linear system is $Ka=F$ with $K_{jk}=a(\phi_k,\phi_j)$ and $F_j=\langle f,\phi_j\rangle$.

#### Ritz-Galerkin equivalence for a symmetric coercive form

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

For a bounded symmetric [coercive bilinear form](linear-algebra.md#coercive-bilinear-form) on a Hilbert space, a solution of $a(u,w)=\ell(w)$ minimizes $J(v)=a(v,v)/2-\ell(v)$. The displayed identity proves strict minimality and uniqueness. Restricting to a [conforming finite element space](#conforming-finite-element-space) makes the discrete [Ritz method](#rayleigh-ritz-method) equivalent to the [Galerkin method](partial-differential-equation.md#galerkin-method). [Galerkin orthogonality](#galerkin-orthogonality) gives exact best approximation in the [energy norm](#energy-norm); the [Céa lemma](#cea-s-lemma) translates it into a reference-norm estimate.

##### Symmetry and coercivity in quadratic energy minimization

↑ **Parent:** [Ritz-Galerkin equivalence for a symmetric coercive form](#ritz-galerkin-equivalence-for-a-symmetric-coercive-form)

A continuous symmetric [coercive bilinear form](linear-algebra.md#coercive-bilinear-form) $a$ on a real [Hilbert space](hilbert-space.md) and a continuous [linear functional](linear-algebra.md#linear-functional) $\ell$ give a unique minimum of $I$. The parallelogram identity makes any minimizing sequence Cauchy in the energy norm; coercivity and completeness give its limit. Differentiation gives $a(u,w)=\ell(w)$, and $I(v)-I(u)=a(v-u,v-u)$ proves uniqueness. A nonsymmetric operator instead differentiates to its symmetric part. Mere pointwise positivity without a lower bound in the chosen norm need not yield a minimizing vector.

#### Energy norm

↑ **Parent:** [Rayleigh-Ritz method](#rayleigh-ritz-method)

A symmetric coercive bilinear form $a$ defines the energy norm $\|v\|_a=\sqrt{a(v,v)}$. In this norm the [Ritz method](#rayleigh-ritz-method) is an orthogonal projection onto its finite-dimensional trial space.

### Galerkin orthogonality

↑ **Parent:** [Finite element method](#finite-element-method)

If $u$ solves a variational problem and $u_h$ is its conforming [Galerkin method](partial-differential-equation.md#galerkin-method) approximation in $V_h$, then

$$
a(u-u_h,v_h)=0
$$

for every $v_h\in V_h$.

<h4 id="cea-s-lemma">Céa's lemma</h4>

↑ **Parent:** [Galerkin orthogonality](#galerkin-orthogonality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Céa's_lemma)

For a continuous coercive bilinear form with continuity constant $M$ and coercivity constant $\alpha$, a conforming finite-element solution satisfies

$$
\|u-u_h\|_V\leq\frac M\alpha
\inf_{v_h\in V_h}\|u-v_h\|_V.
$$

For a symmetric problem measured in its [energy norm](#energy-norm), the constant is one.

For any $v_h\in V_h$, [Galerkin orthogonality](#galerkin-orthogonality) gives $a(e,e)=a(e,u-v_h)$, where $e=u-u_h$. Coercivity and continuity yield $\alpha\|e\|_V^2\leq M\|e\|_V\|u-v_h\|_V$. Divide by $\|e\|_V$ when it is nonzero and take the infimum. In the symmetric case, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in the [energy norm](#energy-norm) gives the constant one.

<h5 id="aubin-nitsche-duality-argument">Aubin–Nitsche duality argument</h5>

↑ **Parent:** [Céa's lemma](#cea-s-lemma)

For a symmetric elliptic variational problem with [Galerkin orthogonality](#galerkin-orthogonality), let $e=u-u_h$ and solve the dual problem $a(v,z)=(e,v)_{L^2}$ for every $v\in H_0^1(\Omega)$. If [elliptic regularity](distribution-theory.md#elliptic-regularity) gives $\|z\|_{H^2}\leq C\|e\|_{L^2}$, then a [finite element interpolation estimate](#finite-element-interpolation-estimate) gives

$$
\|e\|_{L^2}^2=a(e,z-I_hz)
\leq Ch\|e\|_{H^1}\|z\|_{H^2}
\leq Ch\|e\|_{H^1}\|e\|_{L^2}.
$$

Thus $\|e\|_{L^2}\leq Ch\|e\|_{H^1}$. Combining this with the [Céa lemma](#cea-s-lemma) and an $O(h)$ [energy norm](#energy-norm) error gives an $O(h^2)$ [L2 norm](real-analysis.md#l2-norm) error. The additional order depends on the dual regularity assumption, which can fail on unsuitable domains.

### Piecewise-linear hat function

↑ **Parent:** [Finite element method](#finite-element-method)

A piecewise-linear hat function is one at one mesh node, zero at all other nodes, and affine on each adjacent mesh interval. Interior hat functions form the standard nodal basis for continuous piecewise-linear finite elements with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition).

## Arithmetic operation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An arithmetic operation is one scalar addition, subtraction, multiplication, or division. Counting such operations gives a basic model of an algorithm's computational cost.

## Schur stability criterion

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a real monic quadratic $z^2+a_1z+a_2$, both roots lie in the closed unit disk when

$$
|a_2|\leq1,
\qquad
1+a_1+a_2\geq0,
\qquad
1-a_1+a_2\geq0,
$$

with the usual simplicity requirement for roots on the unit circle.

### Complex quadratic Schur criterion

↑ **Parent:** [Schur stability criterion](#schur-stability-criterion)

For a complex [polynomial](polynomial.md) $p(z)=az^2+bz+c$, assume $|a|>|c|$ and put $D=|a|^2-|c|^2$ and $E=\overline a b-c\overline b$. Both [roots of a polynomial](polynomial.md#root-of-a-polynomial) lie in the closed unit disk if and only if $|E|\leq D$. Strict inequality puts both roots in the open disk. Under the strict product assumption $|c/a|<1$, any unit-modulus root is automatically simple.

To prove the strict version, define $p^\#(z)=z^2\overline{p(1/\overline z)}$ and $q=\overline a p-cp^\#=z(Dz+E)$. On the unit circle $|p^\#|=|p|$, so the [Rouche theorem](complex-analysis.md#rouche-s-theorem) shows that a stable $p$ and $q$ have the same two interior zeros. Conversely $Dp=aq+cq^\#$, and the same [Rouche theorem](complex-analysis.md#rouche-s-theorem) implies that two interior zeros of $q$ give two interior zeros of $p$. The nonzero root of $q$ is $-E/D$, proving the criterion. The closed version follows by continuity, replacing $b$ by $(1-\varepsilon)b$ in the sufficiency direction. In the necessity direction with a boundary root, replace $p(z)$ by $p(z/r)$ for $r<1$ close to one and let $r\to1$. The product of the two [roots of a polynomial](polynomial.md#root-of-a-polynomial) excludes two unit-modulus roots and excludes a repeated unit-modulus root.

## Lie product formula

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_product_formula)

For bounded [matrices](vector-space.md#matrix) $A_j$, the Lie product formula gives [operator norm](continuous-dual-space.md#operator-norm) convergence

$$
e^{t\sum_jA_j}=\lim_{k\to\infty}\left(\prod_je^{tA_j/k}\right)^k.
$$

For two summands, expanding their [matrix exponentials](linear-operator-theory.md#matrix-exponential) gives the one-step difference below. For [Hermitian matrices](hilbert-space.md#hermitian-operator) multiplied by $-i$, the factors are [unitary operators](vector-space.md#unitary-operator) and the [first-order unitary product-formula error bound](#first-order-unitary-product-formula-error-bound) gives an explicit error estimate.

### Exponential product defect identity

↑ **Parent:** [Lie product formula](#lie-product-formula)

For finite [matrices](vector-space.md#matrix), differentiate the ordered product to obtain $\Phi'-(A+B)\Phi=[e^{tA},B]e^{tB}$. Multiplying the error by $e^{-t(A+B)}$ and integrating gives $\Phi(t)-e^{t(A+B)}=\int_0^t e^{(t-s)(A+B)}[e^{sA},B]e^{sB}\,ds$. This exact [variation-of-constants formula](functional-analysis.md#variation-of-constants-formula) identifies noncommutativity as the source of [Lie-Trotter splitting](#lie-product-formula) error.

#### Decaying bound for symmetric negative matrix splitting

↑ **Parent:** [Exponential product defect identity](#exponential-product-defect-identity)

For symmetric negative-definite [matrices](vector-space.md#matrix), put $a=\lambda_{\max}(A)$, $b=\lambda_{\max}(B)$ and $c=\lambda_{\max}(A+B)\leq a+b$. The [spectral theorem](hilbert-space.md#spectral-theorem) gives exact exponential norm bounds, and $\|[e^{sA},B]\|_2\leq2\|B\|_2e^{sa}$. Integration in the [exponential product defect identity](#exponential-product-defect-identity) proves the displayed estimate if $c<a+b$. At equality its continuous limit is $2t\|B\|_2e^{tc}$; the quotient must not be interpreted as division by zero.

### Symmetrized exponential-splitting defect identity

↑ **Parent:** [Lie product formula](#lie-product-formula)

For bounded [matrices](vector-space.md#matrix), differentiating the symmetrized product gives $F'-(A+B)F=\tfrac12([e^{tB},A]e^{tA}+[e^{tA},B]e^{tB})$. The [variation-of-constants formula](functional-analysis.md#variation-of-constants-formula) turns this into an integral expression for $F-e^{t(A+B)}$. This retains the noncommutativity of the factors explicitly; cancellation of their leading opposite [commutators](lie-algebra.md#commutator) explains why the averaged product is more accurate than either ordering alone.

### Lie-Trotter splitting commutator error

↑ **Parent:** [Lie product formula](#lie-product-formula)

For bounded [matrices](vector-space.md#matrix),

$$
e^{hB}e^{hC}=e^{h(B+C)}+\frac{h^2}{2}(BC-CB)+O(h^3).
$$

Commutativity removes this splitting error, though first-order substeps such as [Backward Euler method](#backward-euler-method) retain their own quadratic local errors.

### First-order unitary product-formula error bound

↑ **Parent:** [Lie product formula](#lie-product-formula)

For [Hermitian matrices](hilbert-space.md#hermitian-operator) $H_1,\ldots,H_m$ and $t\geq0$, let $S(t)=\prod_{j=1}^m e^{-itH_j}$. Then

$$
\boxed{\left\|S(t)-e^{-it\sum_jH_j}\right\|
\leq\frac{t^2}{2}\sum_{j<l}\|[H_j,H_l]\|.}
$$

Here every norm is the [spectral norm](continuous-dual-space.md#matrix-2-norm). A short proof starts with two summands. Differentiate $F(s)=e^{-i(t-s)(A+B)}e^{-isA}e^{-isB}$; its derivative has norm at most $\|[e^{-isA},B]\|$. Differentiating $e^{-iuA}Be^{iuA}$ and integrating yields $\|[e^{-isA},B]\|\leq s\|[A,B]\|$, because [unitary operators](vector-space.md#unitary-operator) preserve the norm. Integrating $s$ from zero to $t$ gives $t^2\|[A,B]\|/2$. Inductively separate $H_1$ from the remaining sum, use the [triangle inequality](topological-analysis.md#triangle-inequality) on their [commutator](lie-algebra.md#commutator), and apply the [telescoping bound for products of operators](continuous-dual-space.md#telescoping-bound-for-products-of-operators) to obtain the displayed many-term bound.

Repeating steps of size $t/k$ and telescoping across $k$ steps gives

$$
\left\|S(t/k)^k-e^{-it\sum_jH_j}\right\|
\leq\frac{t^2}{2k}\sum_{j<l}\|[H_j,H_l]\|.
$$

For a chain of $O(n)$ bounded nearest-neighbor terms, only $O(n)$ pairs fail to commute. Consequently first-order [product-formula Hamiltonian simulation](quantum-theory.md#product-formula-hamiltonian-simulation) has error $O(nt^2/k)$ and uses $O(nk)$ constant-size gates. The general bound is also given in Proposition 9 of [Childs and collaborators' analysis of Trotter error](https://journals.aps.org/prx/pdf/10.1103/PhysRevX.11.011020).

## Strang splitting

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strang_splitting)

Strang splitting approximates $e^{h(A+B)}$ by $e^{hA/2}e^{hB}e^{hA/2}$. Its time symmetry cancels the quadratic local commutator defect, giving local error $O(h^3)$ and global order two.

### Strang splitting contraction for symmetric diffusion and skew advection

↑ **Parent:** [Strang splitting](#strang-splitting)

If real matrices satisfy $A^T=A\leq0$ and $B^T=-B$, then $e^{tA}$ is a contraction and $e^{tB}$ is an [orthogonal matrix](linear-algebra.md#orthogonal-matrix) for $t\geq0$. Hence $\|e^{kA/2}e^{kB}e^{kA/2}\|_2\leq1$ for every $k\geq0$. The bound is independent of commutativity and gives unconditional stability for a [centered convection-diffusion semidiscretization](finite-difference.md#centered-convection-diffusion-semidiscretization) with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). It does not itself bound the mesh-dependent commutators that enter a time-error estimate.

### Higher-order composition of a symmetric splitting

↑ **Parent:** [Strang splitting](#strang-splitting)

If $S_h$ is a symmetric second-order splitting, then $S_{\gamma h}S_{\delta h}S_{\gamma h}$ is fourth order for $\gamma=(2-2^{1/3})^{-1}$ and $\delta=-2^{1/3}(2-2^{1/3})^{-1}$. The identities $2\gamma+\delta=1$ and $2\gamma^3+\delta^3=0$ preserve the total step and cancel the leading odd defect.

## Composite midpoint rule error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For $f\in C^2[a,b]$, the composite midpoint rule with mesh width $h$ has local error $O(h^3)$ and global error $O(h^2)$.

### Quadratic substitution for a square-root endpoint singularity

↑ **Parent:** [Composite midpoint rule error](#composite-midpoint-rule-error)

If $f(x)=x^{-1/2}g(x)$ with $g$ smooth near zero, the substitution $x=s^2$ gives

$$
\int_0^1f(x)\,dx=\int_0^12g(s^2)\,ds.
$$

The transformed integrand is smooth, so an ordinary second-order midpoint rule recovers its usual convergence rate.

## Polynomial interpolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_interpolation)

Given distinct nodes $x_0,\ldots,x_n$ and values $f(x_i)$, there is a unique polynomial of degree at most $n$ taking those values.

### Interpolation polynomial

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

An interpolation polynomial for distinct nodes $x_0,\ldots,x_n$ and prescribed values $y_0,\ldots,y_n$ is a [polynomial](polynomial.md) $p$ satisfying $p(x_i)=y_i$. There is a unique such [polynomial](polynomial.md) of degree at most $n$: the [Lagrange interpolation polynomial](#lagrange-polynomial) constructs it explicitly, and uniqueness follows because a nonzero degree-at-most-$n$ difference cannot have $n+1$ distinct roots. [Newton interpolation polynomials](#newton-polynomial) express the same object using [divided differences](#divided-difference).

### Interpolation nodes from best uniform approximation

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

For a real [continuous function](calculus.md#continuous-function) on a compact interval, choose its [best uniform approximation](uniform-approximation.md#best-uniform-approximation) $p_n^*$ of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n$. If its error is nonzero, the [Chebyshev alternation theorem](uniform-approximation.md#equioscillation-theorem) supplies $n+2$ ordered alternating extrema. The [intermediate value theorem](calculus.md#intermediate-value-theorem) gives a zero of $f-p_n^*$ in each intervening interval. At these $n+1$ distinct points, the [polynomial interpolant](#lagrange-polynomial) is exactly $p_n^*$. If the best error is zero, arbitrary distinct nodes suffice. The [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) shows that these function-dependent interpolants converge uniformly. The nodes depend on the target function; the conclusion does not provide one universal node sequence for every continuous target.

### Interpolation node

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)

An interpolation node is one of the distinct argument values at which an interpolating function is required to match prescribed data.

### Lagrange polynomial

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange_polynomial)

The interpolating polynomial is

$$
p_n(x)=\sum_{j=0}^nf(x_j)
\prod_{\substack{0\leq i\leq n\\i\ne j}}
\frac{x-x_i}{x_j-x_i}.
$$

#### Differentiation weights from nodal evaluations

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

At distinct nodes $a_0,\ldots,a_n$, the [Lagrange interpolation polynomial](#lagrange-polynomial) has basis $\ell_j(x)=\prod_{i\ne j}(x-a_i)/(a_j-a_i)$. Differentiating its exact expression for a polynomial of degree at most $n$ gives the displayed weights. Their uniqueness follows because the nodal evaluations form a basis of the [dual space](linear-algebra.md#dual-space) of that polynomial space.

#### Discrete minimax interpolation on ordered nodes

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

For $n+2$ increasingly ordered nodes $y_j$, let $r_j$ be their [Lagrange cardinal polynomials](#lagrange-cardinal-polynomial), $t=\sum f(y_j)r_j$, and $r=\sum(-1)^jr_j$. The leading coefficient of $r_j$ has sign $(-1)^{n+2-j}$, so all summands in the leading coefficient of $r$ have the same nonzero sign. There is a unique $\lambda$ canceling degree $n+1$ in $t-\lambda r$. Its errors at the nodes are $\lambda(-1)^j$, and a better degree-at-most-$n$ approximation would have a difference polynomial with at least $n+1$ roots. Thus it minimizes the maximum node error. Increasing order matters: for the permutation $(0,1/3,1,2/3)$ the alternating interpolant is already the quadratic $-1+9x(1-x)$, so the leading-coefficient assertion for $n=2$ fails.

#### Lagrange cardinal polynomial

↑ **Parent:** [Lagrange polynomial](#lagrange-polynomial)

For distinct [interpolation nodes](#interpolation-node) $x_0,\ldots,x_n$, the polynomial $\ell_i(x)=\prod_{j\ne i}(x-x_j)/(x_i-x_j)$ has $\ell_i(x_j)=\delta_{ij}$. These cardinal polynomials form a [basis](vector-space.md#basis) of the [polynomials](polynomial.md) of degree at most $n$, and give $p(x)=\sum_i p(x_i)\ell_i(x)$.

##### Endpoint derivative signs of Lagrange cardinal polynomials

↑ **Parent:** [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)

At decreasing distinct [interpolation nodes](#interpolation-node) $1\ge t_0>\cdots>t_n\ge-1$, the [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial) $L_i(x)=\prod_{j\ne i}(x-t_j)/\prod_{j\ne i}(t_i-t_j)$ has denominator sign $(-1)^i$. For $1\le k\le n$, its numerator's $k$th [derivative](calculus.md#derivative) at one is $k!$ times a sum of products of $n-k$ nonnegative factors $1-t_j$. At most one factor vanishes, and at least one product avoids it, so that sum is strictly positive. The same alternating nodal signs therefore maximize every endpoint derivative simultaneously.

##### Nodal derivative norm from Lagrange cardinal polynomials

↑ **Parent:** [Lagrange cardinal polynomial](#lagrange-cardinal-polynomial)

At distinct [interpolation nodes](#interpolation-node), differentiating [Lagrange interpolation](#lagrange-polynomial) gives $p^{(k)}(x)=\sum_i p(t_i)\ell_i^{(k)}(x)$. The [triangle inequality](topological-analysis.md#triangle-inequality) gives the displayed upper bound, attained by prescribing each nodal value to be the sign of the corresponding [derivative](calculus.md#derivative) weight. For increasingly ordered real nodes, the [Markov interlacing lemma](polynomial.md#markov-interlacing-lemma) and [monotonicity of polynomial critical points in their roots](polynomial.md#monotonicity-of-polynomial-critical-points-in-their-roots) imply that $(-1)^i\ell_i^{(k)}(x)$ has at most one sign change, ignoring zero weights. Thus an extremizer has alternating nodal signs with at most one reversal of that alternating pattern. This reduces a choice among $2^{n+1}$ sign patterns to $n+1$ candidate [polynomials](polynomial.md).

### Divided difference

↑ **Parent:** [Polynomial interpolation](#polynomial-interpolation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divided_difference)

For distinct nodes,

$$
f[x_0,\ldots,x_k]
=\sum_{j=0}^k\frac{f(x_j)}
{\prod_{i\ne j}(x_j-x_i)}.
$$

It is the leading coefficient of the interpolating polynomial through those nodes and obeys

$$
f[x_0,\ldots,x_k]
=\frac{f[x_1,\ldots,x_k]-f[x_0,\ldots,x_{k-1}]}
{x_k-x_0}.
$$

#### Omitted-node identities for divided differences

↑ **Parent:** [Divided difference](#divided-difference)

For distinct [interpolation nodes](#interpolation-node), write $D_i$ for the [divided difference](#divided-difference) with $x_i$ omitted. Symmetry and the divided-difference recurrence give the displayed identity. Consequently, for $0<i<n$,

$$
D_i=\frac{x_i-x_0}{x_n-x_0}D_n+\frac{x_n-x_i}{x_n-x_0}D_0.
$$

The identity is algebraic and does not require the nodes to be ordered; the coefficients need not be nonnegative.

#### Exponential divided difference

↑ **Parent:** [Divided difference](#divided-difference)

The displayed integral is $(e^{t\beta}-e^{t\gamma})/(\beta-\gamma)$ for distinct exponents and $te^{t\gamma}$ when they coincide. The latter is the continuous limit, so a zero denominator is a removable singularity. This quantity appears in [variation-of-constants formula](functional-analysis.md#variation-of-constants-formula) estimates of [matrix](vector-space.md#matrix) evolution and avoids omitting an equal-exponent case.

#### Leibniz rule for divided differences

↑ **Parent:** [Divided difference](#divided-difference)

For $h=fg$,

$$
h[t_0,\ldots,t_k]=\sum_{m=0}^kf[t_0,\ldots,t_m]g[t_m,\ldots,t_k].
$$

#### Newton polynomial

↑ **Parent:** [Divided difference](#divided-difference)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton_polynomial)

Newton's nested interpolation form is

$$
p_n(x)=f(x_0)+\sum_{k=1}^nf[x_0,\ldots,x_k]
\prod_{i=0}^{k-1}(x-x_i).
$$

A triangular divided-difference table computes all its coefficients using exactly $n(n+1)/2$ divisions.

## Discrete Fourier transform

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_Fourier_transform)

For samples $y_0,\ldots,y_{m-1}$, their discrete Fourier transform is

$$
Y_k=\sum_{n=0}^{m-1}y_ne^{-2\pi ink/m}.
$$

### Prime Fourier matrix minor theorem

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

For a prime $p$, distinct row and column residues and $\zeta=e^{2\pi i/p}$, every square [discrete Fourier transform](#discrete-fourier-transform) submatrix is nonsingular. Sort the selected column exponents decreasingly as $b_i$ and write $b_i=\lambda_i+N-i$. Its [determinant](linear-algebra.md#determinant) factors by the [bialternant formula](combinatorics.md#bialternant-formula) into a nonzero [Vandermonde determinant](galois-theory.md#vandermonde-determinant) and $s_\lambda(\zeta^{r_1},\ldots,\zeta^{r_N})$. Modulo $1-\zeta$, this Schur factor is $s_\lambda(1^N)$ in $\mathbb F_p$. The [Schur evaluation at all ones](combinatorics.md#schur-evaluation-at-all-ones) product has numerator and denominator differences strictly between zero and $p$, so its residue is nonzero. The Schur factor, and hence the minor, cannot vanish.

### Finite-field discrete Fourier transform

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

If $\omega$ is a primitive $n$th root in a [finite field](algebra.md#finite-field) and the field [characteristic](algebra.md#characteristic-of-a-field) does not divide $n$, the inverse transform is $c_j=n^{-1}\sum_{\ell=0}^{n-1}\widehat c_\ell\omega^{-j\ell}$. The identity $\sum_{j=0}^{n-1}\omega^{jm}=0$ unless $n\mid m$, when the sum is $n$, proves inversion. For a [primitive cyclic Reed-Solomon code](coding-theory.md#primitive-cyclic-reed-solomon-code), encoding assigns the $k$ unconstrained transform values and makes the remaining values zero; received transform values at those zeros are [syndromes](coding-theory.md#syndrome).

### Discrete Parseval identity

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

With normalization $\widehat U_k=N^{-1/2}\sum_mU_me^{-2\pi imk/N}$, the [discrete Fourier transform](#discrete-fourier-transform) is a [unitary matrix](linear-operator-theory.md#unitary-matrix). Orthogonality of the roots-of-unity vectors gives the displayed identity. Multiplying both sides by the grid spacing gives the corresponding discrete [L2 norm](real-analysis.md#l2-norm). Modal contraction therefore proves grid-norm contraction without a mesh-dependent change-of-basis constant.

### Fourier representation of a Kronecker delta

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

Orthogonality of integer-frequency [Fourier modes](fourier-analysis.md#fourier-mode) gives this identity: the integral is one for $n=m$ and zero otherwise. It converts integer step-count constraints into products of generating functions, as in the [dilute-hopping lattice propagator](quantum-theory.md#dilute-hopping-lattice-propagator).

### Fourier frequency

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

$\lambda_j=2\pi j/T$ is a frequency of the length-$T$ [discrete Fourier transform](#discrete-fourier-transform). Distinct interior frequencies give orthogonal sine and cosine vectors; for a Gaussian [white noise](time-series.md#white-noise) record this makes the corresponding Fourier components independent.

### Inverse discrete Fourier transform

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_discrete_Fourier_transform)

The inverse discrete Fourier transform reconstructs samples from their [discrete Fourier transform](#discrete-fourier-transform). Under one common normalization,

$$
x_\ell=\frac1n\sum_{j=0}^{n-1}Y_je^{2\pi i j\ell/n};
$$

moving the factor $1/n$ between the forward and inverse transforms gives other standard conventions.

### Discrete Fourier mode

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)

On a cyclic index set of length $n$, the $k$th discrete Fourier mode is the vector with $j$th coordinate $e^{2\pi ikj/n}$. Its real and imaginary parts are the corresponding cosine and sine modes.

### Cooley-Tukey FFT algorithm

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cooley–Tukey_FFT_algorithm)

The radix-two Cooley--Tukey algorithm recursively splits a discrete Fourier transform into transforms of the even-indexed and odd-indexed samples. For a power-of-two length this evaluates the transform in $O(m\log m)$ arithmetic operations.

#### FFT butterfly

↑ **Parent:** [Cooley-Tukey FFT algorithm](#cooley-tukey-fft-algorithm)

An [FFT butterfly](#fft-butterfly) combines corresponding outputs of two half-sized transforms using a twiddle factor $w$. Sharing the product $wb$ costs one complex multiplication and two additions. For the unnormalized positive-exponent inverse [discrete Fourier transform](#discrete-fourier-transform) of length $2m$, use $w=e^{2\pi i\ell/(2m)}$ at index $\ell$.

<h4 id="even-odd-fast-fourier-transform-recursion">Even--odd fast Fourier transform recursion</h4>

↑ **Parent:** [Cooley-Tukey FFT algorithm](#cooley-tukey-fft-algorithm)

For $\omega_m=e^{-2\pi i/m}$ and length-$m/2$ transforms $E_k,O_k$ of the even and odd samples,

$$
Y_k=E_k+\omega_m^kO_k,
\qquad Y_{k+m/2}=E_k-\omega_m^kO_k.
$$

### Discrete cosine transform

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_cosine_transform)

The type-II discrete cosine transform of $x_0,\ldots,x_{N-1}$ is

$$
Z_k=\sum_{n=0}^{N-1}x_n\cos\left(\frac{\pi}{N}\left(n+\frac12\right)k\right).
$$

#### Discrete cosine transform from an even-reflected discrete Fourier transform

↑ **Parent:** [Discrete cosine transform](#discrete-cosine-transform)

Reflect $x$ evenly to length $2N$ by $y_n=x_n$ and $y_{2N-1-n}=x_n$. If $Y$ is the discrete Fourier transform of $y$, then

$$
Z_k=\frac12e^{-\pi ik/(2N)}Y_k.
$$

This reduction computes the cosine transform with one fast Fourier transform and $O(N)$ additional work.

### Discrete sine transform

↑ **Parent:** [Discrete Fourier transform](#discrete-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_sine_transform)

One half-grid sine-transform convention is

$$
\widetilde Z_k=\sum_{n=0}^{N-1}x_n
\sin\left(\frac{\pi}{N}\left(n+\frac12\right)(k+1)\right).
$$

#### Discrete sine transform Poisson solver

↑ **Parent:** [Discrete sine transform](#discrete-sine-transform)

For $-\Delta u=f$ on a square with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), the five-point [finite difference](finite-difference.md) operator on a mesh $h=1/N$ is diagonalized by $\sin(\pi ki/N)\sin(\pi\ell j/N)$. Its eigenvalues are $\lambda_{k\ell}=4h^{-2}[\sin^2(\pi k/(2N))+\sin^2(\pi\ell/(2N))]$. A two-dimensional [discrete sine transform](#discrete-sine-transform), division by these nonzero eigenvalues and the inverse transform give the solution. Odd extension realizes each one-dimensional transform by a [Fast Fourier transform](#cooley-tukey-fft-algorithm) of length $2N$, making the total cost $O(N^2\log N)$ and storage $O(N^2)$. These finite-difference eigenvalues should not be confused with the continuous spectral eigenvalues $\pi^2(k^2+\ell^2)$.

#### Discrete sine transform from a sign-modulated discrete cosine transform

↑ **Parent:** [Discrete sine transform](#discrete-sine-transform)

If $\xi_n=(-1)^nx_n$ and $C_j(\xi)$ is its type-II cosine transform, then

$$
\widetilde Z_k=C_{N-1-k}(\xi).
$$

Thus a sign modulation, one fast cosine transform, and output reversal give an $O(N\log N)$ sine-transform algorithm.

## Gershgorin circle theorem

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gershgorin_circle_theorem)

Every eigenvalue of a complex matrix $A=(a_{ij})$ lies in at least one disk

$$
\left\{z:|z-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\right\}.
$$

### Gershgorin disc

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

For row $i$ of a matrix, the [Gershgorin disc](#gershgorin-disc) has centre $M_{ii}$ and radius $\sum_{j\ne i}|M_{ij}|$. The [Gershgorin disc theorem](#gershgorin-circle-theorem) places every [eigenvalue](linear-operator-theory.md#eigenvalue) in the union of these discs. For a Hermitian matrix the real intervals cut out by the discs bound energies; an isolated disc contains exactly one [eigenvalue](linear-operator-theory.md#eigenvalue).

### Gershgorin stability bound for a variable-coefficient diffusion stencil

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

A symmetric conservative five-point diffusion matrix has row center $-s/h^2$ and radius at most $s/h^2$, where $s$ is the sum of its four nonnegative edge coefficients. If every coefficient is at most $a_{\max}$, its eigenvalues lie in $[-8a_{\max}/h^2,0]$. Forward Euler is therefore stable when $\Delta t/h^2\leq1/(4a_{\max})$.

## Finite difference

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](finite-difference.md)

## Tridiagonal matrix algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tridiagonal_matrix_algorithm)

The Thomas algorithm is specialized Gaussian elimination for a tridiagonal linear system and uses linear time and storage in the system dimension.

## Gaussian quadrature

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_quadrature)

An $n$-node Gaussian quadrature rule uses orthogonal-polynomial roots and integrates every polynomial of degree at most $2n-1$ exactly.

### Orthogonal-node criterion for Gaussian quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

An $(n+1)$-node quadrature exact on degree $n$ is exact through degree $2n+1$ precisely when its node polynomial $p=\prod_i(x-x_i)$ is [orthogonal](linear-algebra.md#orthogonal-vectors) to every degree-$n$ [polynomial](polynomial.md) for the integration weight. Necessity applies the rule to $pr$. Sufficiency divides an arbitrary degree-$2n+1$ polynomial as $pq+r$, with both $q,r$ of degree at most $n$; the integral and quadrature of $pq$ vanish while both agree on $r$.

### Two-node Gaussian quadrature with quadratic weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

The even weight $1-x^2$ has moments $m_0=4/3$ and $m_2=4/15$. Its monic quadratic orthogonal polynomial is $x^2-1/5$, so the two [Gaussian quadrature](#gaussian-quadrature) nodes are $\pm1/\sqrt5$. Symmetry and constant exactness give weights $2/3$ each. These nodes and weights integrate every polynomial of degree at most three exactly. Degree four fails: the true integral is $4/35$, whereas the rule gives $4/75$.

<h3 id="chebyshev-gauss-quadrature">Chebyshev–Gauss quadrature</h3>

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev–Gauss_quadrature)

The first-kind rule approximates $\int_{-1}^1 f(x)(1-x^2)^{-1/2}\,dx$ at the zeros of the [Chebyshev polynomial](#chebyshev-polynomial) $T_n$. It integrates all [polynomials](polynomial.md) of degree at most $2n-1$ exactly. The weights follow by integrating the [Lagrange interpolation polynomial](#lagrange-polynomial) at those nodes. Orthogonality kills the quotient when a degree-$2n-1$ polynomial is divided by $T_n$; its remainder is recovered by interpolation. No $n$-node rule can integrate every degree-$2n$ polynomial, since the squared nodal polynomial has zero quadrature sum and strictly positive weighted integral.

// Target: probability-and-statistics.bigb

### Gauss-Laguerre quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Laguerre_quadrature)

For the weight $e^{-x}$ on $[0,\infty)$, use the zeros of a degree-$n$ [Laguerre polynomial](linear-operator-theory.md#laguerre-polynomial) as quadrature nodes. Divide a polynomial of degree at most $2n-1$ by that polynomial. The quotient term integrates to zero by orthogonality and vanishes at every node; interpolation of the remainder proves exactness. The two-node rule has nodes $2\pm\sqrt2$ and corresponding weights $(2\pm\sqrt2)/4$, with the larger weight at the smaller node.

### Two-node Gaussian quadrature with linear weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For weight $w(x)=x$ on $[0,1]$, the two-node [Gaussian quadrature](#gaussian-quadrature) nodes are roots of $x^2-6x/5+3/10$, the monic quadratic orthogonal to all linear [polynomials](polynomial.md). Its weights come from integrating the [Lagrange interpolation](#lagrange-polynomial) cardinal functions. Orthogonality gives exactness on cubic [polynomials](polynomial.md) and positive weights.

### Two-node Gaussian quadrature with sine weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For integration against $\sin x$ on $[0,\pi]$, the monic quadratic [orthogonal polynomial](#orthogonal-polynomial) is $x^2-\pi x+2$. Its two roots are the [Gaussian quadrature](#gaussian-quadrature) nodes $c_{1,2}=\pi/2\mp\sqrt{\pi^2/4-2}$, with weights one. The rule integrates every cubic exactly: divide it by the orthogonal quadratic and integrate the degree-one remainder.

### Positive weights of Gaussian quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For an $n$-node [Gaussian quadrature](#gaussian-quadrature) rule exact through degree $2n-1$, the cardinal [Lagrange interpolation polynomial](#lagrange-polynomial) $\ell_j$ has square of degree $2n-2$. Exactness gives $A_j=\int\ell_j^2>0$ for a positive integration weight. This proof turns [polynomial](polynomial.md) exactness directly into positivity.

### Gauss-Hermite quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss-Hermite_quadrature)

Gauss-Hermite quadrature uses the roots of a degree-$N$ [Hermite polynomial](#hermite-polynomial) as nodes for an integral with Gaussian weight. Its positive interpolation weights make it exact for every polynomial of degree at most $2N-1$.

## Lobatto quadrature

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An $s$-node Lobatto quadrature rule includes both endpoints and is exact for [polynomials](polynomial.md) of degree at most $2s-3$. On $[-1,1]$, its interior nodes are the zeros of the derivative of the degree-$(s-1)$ [Legendre polynomial](differential-equation.md#legendre-polynomial). The three-node rule on $[0,1]$ has nodes $0,1/2,1$ and weights $1/6,2/3,1/6$. Integrating the interpolation basis from zero to each node gives the three-stage [Lobatto IIIA method](#lobatto-iiia-method).

## Chebyshev polynomial

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_polynomial)

$T_n(\cos\theta)=\cos(n\theta)$. These polynomials are orthogonal for weight $(1-x^2)^{-1/2}$ and support spectrally accurate approximation.

### Chebyshev projection of a semicircle

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

For weighted [least-squares polynomial in an orthogonal-polynomial basis](linear-algebra.md#least-squares-polynomial-in-an-orthogonal-polynomial-basis) with weight $(1-x^2)^{-1/2}$ on $[-1,1]$, the projection of $\sqrt{1-x^2}$ onto [polynomials](polynomial.md) of degree at most $n$ is the displayed sum. Put $x=\cos\theta$ to obtain $T_j(x)=\cos j\theta$ and $f(x)=\sin\theta$ on $[0,\pi]$. The constant coefficient is $2/\pi$, odd coefficients vanish, and the coefficient of $T_{2m}$ is $4/[\pi(1-4m^2)]$. For odd $n$ the optimal [polynomial](polynomial.md) can have degree $n-1$.

### Chebyshev nodal derivative comparison

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

Let $x_j=\cos((2j-1)\pi/(2n))$ be the roots of the [Chebyshev polynomial](#chebyshev-polynomial), and let $q$ have degree at most $n-1$ with $|q(x_j)|\le |T_n'(x_j)|$. Its [Lagrange interpolation polynomial](#lagrange-polynomial) uses basis $\ell_j(x)=T_n(x)/[(x-x_j)T_n'(x_j)]$. For $x>x_1$, $T_n(x)>0$ and $x-x_j>0$, so $\ell_j(x)T_n'(x_j)>0$. Therefore $|q(x)|\le\sum_j|\ell_j(x)T_n'(x_j)|=T_n'(x)$, the last equality being interpolation of the derivative. Continuity includes $x=x_1$ and reflection proves the left-hand region.

### Chebyshev polynomial of the second kind

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_polynomial_of_the_second_kind)

The Chebyshev polynomial of the second kind is defined by

$$
U_n(\cos\theta)=\frac{\sin((n+1)\theta)}{\sin\theta}.
$$

It is orthogonal on $[-1,1]$ with weight $\sqrt{1-x^2}$ and has roots $\cos(j\pi/(n+1))$ for $1\leq j\leq n$.

### Rational cosine of an integral submultiple of pi

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

The number $2\cos(\pi/n)$ is an algebraic integer. If it is rational it must be an integer, which shows that $\cos(\pi/n)$ is rational only for $n=1,2,3$.

### Positivity of Chebyshev derivatives beyond the unit interval

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

Every root of $T_n^{(k)}$ lies in $(-1,1)$ and its leading coefficient is positive. Hence

$$
T_n^{(k)}(x)>0
$$

for $x\geq1$ and $0\leq k\leq n$.

### Monic Chebyshev extremal polynomial

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

Among monic real polynomials of degree $n$, $2^{1-n}T_n$ uniquely minimizes the supremum norm on $[-1,1]$, attaining the value $2^{1-n}$.

### Chebyshev polynomial domination lemma

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

If $f$ has degree at most $n$ and $|f|<1$ on $[-1,1]$, alternation at the extrema of $T_n$ implies $|f(t)|<|T_n(t)|$ outside that interval.

#### Chebyshev interpolation represents external evaluation

↑ **Parent:** [Chebyshev polynomial domination lemma](#chebyshev-polynomial-domination-lemma)

On real polynomials of degree at most $n\geq1$ with the [uniform norm](functional-analysis.md#supremum-norm) on $[-1,1]$, set $x_j=\cos(j\pi/n)$ and let $\ell_j$ be the [Lagrange interpolation](#lagrange-polynomial) basis. If $u>1$, the denominator of $\ell_j(u)$ has exactly $j$ negative factors while its numerator is positive. Therefore $|\ell_j(u)|=(-1)^j\ell_j(u)$. Since $T_n(x_j)=(-1)^j$, interpolation gives $\sum_j|\ell_j(u)|=T_n(u)$. Hence $|P(u)|\leq\|P\|_\infty T_n(u)$, and $P=T_n$ attains equality. Reflection and Chebyshev parity give the case $u<-1$. Dividing the interpolation weights by $T_n(u)$ yields an exact signed evaluation representation of norm one on $n+1$ nodes. Constants give the immediate degree-zero case.

### Chebyshev differential equation

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_differential_equation)

The equation $(1-z^2)w''-zw'+n^2w=0$ is obtained from the harmonic equation $w_{xx}+n^2w=0$ by $z=\cos x$.

#### Chebyshev derivative Sturm-Liouville pair

↑ **Parent:** [Chebyshev differential equation](#chebyshev-differential-equation)

The Chebyshev equation has self-adjoint form

$$
\left(\sqrt{1-x^2}\,T_n'\right)'
+\frac{n^2}{\sqrt{1-x^2}}T_n=0.
$$

For $U_n=T_n'$, differentiation gives

$$
\left((1-x^2)^{3/2}U_n'\right)'
+(n^2-1)\sqrt{1-x^2}\,U_n=0.
$$

The respective orthogonality weights are $(1-x^2)^{-1/2}$ and $(1-x^2)^{1/2}$.

## Backward differentiation formula

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backward_differentiation_formula)

### Second-order backward differentiation formula

↑ **Parent:** [Backward differentiation formula](#backward-differentiation-formula)

The displayed implicit [linear multistep method](#linear-multistep-method) is second order and [A-stable](#a-stability). It is the $\alpha=4/3$ member of the [trapezoidal-BDF two-step family](#trapezoidal-bdf-two-step-family), whose order and boundary-locus proof establish both properties. Its derivative formula uses three equally spaced values; changing the steps requires different coefficients.

### BDF2 discrete energy identity

↑ **Parent:** [Backward differentiation formula](#backward-differentiation-formula)

For three [vectors](vector-space.md#vector) $a,b,c$ in an [inner product space](linear-algebra.md#inner-product-space), expansion of each squared [norm](functional-analysis.md#norm) proves

$$
2\operatorname{Re}\langle3a-4b+c,a\rangle
=\|a\|^2+\|2a-b\|^2-\|b\|^2-\|2b-c\|^2+\|a-2b+c\|^2.
$$

Therefore the second-order [backward differentiation formula](#backward-differentiation-formula) $3U^{n+2}-4U^{n+1}+U^n=2kLU^{n+2}$ with a [dissipative operator](functional-analysis.md#dissipative-operator) $L$ decreases the discrete [energy](classical-mechanics.md#energy) $\mathcal E_n=\|U^{n+1}\|^2+\|2U^{n+1}-U^n\|^2$. This [quadratic form](linear-algebra.md#quadratic-form) is equivalent to the product [norm](functional-analysis.md#norm) of the two time levels with constants independent of $k$ and $L$. It proves uniform [stability](#stability-of-a-numerical-method) even when amplification [roots of a polynomial](polynomial.md#root-of-a-polynomial) coalesce inside the unit disk, where an eigenvector-separation proof may lose its bound.

## Constrained optimization

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constrained_optimization)

### Optimization constraint

↑ **Parent:** [Constrained optimization](#constrained-optimization)

An optimization constraint restricts the feasible points in [constrained optimization](#constrained-optimization), for example by an equality $g(x)=0$ or an inequality $h(x)\leq0$. Extrema are considered on the resulting feasible set rather than on the whole domain of the objective.

## Equally spaced interpolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equally_spaced_interpolation)

## Givens rotation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Givens_rotation)

A Givens rotation is the identity except for a coordinate-plane block

$$
\begin{pmatrix}c&s\\-s&c\end{pmatrix},
\qquad c^2+s^2=1.
$$

Choosing $(c,s)=(a,b)/\sqrt{a^2+b^2}$ maps the vector $(a,b)^T$ to $(\sqrt{a^2+b^2},0)^T$.

### QR decomposition by Givens rotations

↑ **Parent:** [Givens rotation](#givens-rotation)

Successive Givens rotations eliminate entries below a matrix diagonal. If their product is $\Omega$ and $R=\Omega A$ is upper triangular, then

$$
A=QR,
\qquad Q=\Omega^T,
$$

is a QR decomposition.

## Gradient descent

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gradient_descent)

Gradient descent updates $x$ in the negative-gradient direction. For $F(x)=x^TAx/2-b^Tx$, this direction is the residual $r=b-Ax$.

### Gradient ascent

↑ **Parent:** [Gradient descent](#gradient-descent)

[Gradient ascent](#gradient-ascent) seeks a maximum by stepping along the [gradient](calculus.md#gradient) of a differentiable objective. It is [gradient descent](#gradient-descent) applied to $-J$. Taylor expansion gives $J(x+\eta\nabla J)=J(x)+\eta\|\nabla J\|^2+O(\eta^2)$, so sufficiently small positive steps improve the objective when the [gradient](calculus.md#gradient) is nonzero. Line search, projection onto admissible controls, and noise-aware [gradient](calculus.md#gradient) estimates are common practical modifications; a local stationary result need not be globally optimal.

### Stochastic gradient descent

↑ **Parent:** [Gradient descent](#gradient-descent)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)

Stochastic gradient descent updates parameters using an unbiased or approximate gradient computed from one observation or a mini-batch rather than the complete data set.

#### Projected stochastic gradient descent

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

Projected stochastic gradient descent takes a stochastic-gradient step and then projects the result onto a closed feasible set. For a convex set $C$ it has the form $x_{s+1}=\Pi_C(x_s-\eta_sG_s)$.

#### Unbiased stochastic gradient

↑ **Parent:** [Stochastic gradient descent](#stochastic-gradient-descent)

A random vector $G_s$ is an unbiased stochastic gradient at $x_s$ when $\mathbb E[G_s\mid x_s]=\nabla f(x_s)$.

### Lipschitz gradient

↑ **Parent:** [Gradient descent](#gradient-descent)

A differentiable function has a $\beta$-Lipschitz gradient when

$$
\|\nabla f(x)-\nabla f(y)\|\leq\beta\|x-y\|.
$$

#### Descent lemma

↑ **Parent:** [Lipschitz gradient](#lipschitz-gradient)

A differentiable function with an $L$-[Lipschitz gradient](#lipschitz-gradient) obeys $f(v)\leq f(u)+\langle\nabla f(u),v-u\rangle+(L/2)\|v-u\|^2$. Integrate the gradient along the line segment and bound the deviation from its initial value. The lemma does not require convexity.

### Exact line search for a positive-definite quadratic

↑ **Parent:** [Gradient descent](#gradient-descent)

For $f(x)=x^TAx/2-b^Tx$ with $A$ positive definite and residual $r=b-Ax$, exact line search along $r$ uses

$$
t=\frac{r^Tr}{r^TAr}.
$$

The objective error contracts by

$$
1-\frac{(r^Tr)^2}{(r^TA^{-1}r)(r^TAr)}
\leq 1-\frac{\lambda_{\min}(A)}{\lambda_{\max}(A)}.
$$

### Conjugate gradient method

↑ **Parent:** [Gradient descent](#gradient-descent)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_gradient_method)

For a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) $A$, the conjugate gradient method chooses mutually $A$-conjugate search directions. Starting with $r_0=b-Ax_0$ and $p_0=r_0$, it uses

$$
\alpha_k=\frac{r_k^Tr_k}{p_k^TAp_k},\quad
x_{k+1}=x_k+\alpha_kp_k,\quad
r_{k+1}=r_k-\alpha_kAp_k,
$$

and $p_{k+1}=r_{k+1}+\beta_kp_k$ with  
$\beta_k=r_{k+1}^Tr_{k+1}/(r_k^Tr_k)$.

#### Linear-system residual

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

The residual of an approximate solution $x$ of $Ax=b$ is $r=b-Ax$. It is the unbalanced right-hand side, while the solution error is $x_*-x=A^{-1}r$. The [Conjugate gradient method](#conjugate-gradient-method) makes residuals orthogonal to successive [Krylov subspaces](#krylov-subspace).

#### Conjugate-gradient residual orthogonality

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

At iteration $m$ of the conjugate gradient method,

$$
x_m-x_0\in\mathcal K_m(A,r_0),
\qquad
r_m\perp\mathcal K_m(A,r_0),
$$

and $r_m$ itself lies in $\mathcal K_{m+1}(A,r_0)$. These Galerkin conditions imply finite termination once the Krylov subspace becomes invariant under $A$.

#### Preconditioned conjugate gradient method

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

A symmetric preconditioner transforms $Ax=b$ into

$$
PAP^T\widehat x=Pb,\qquad x=P^T\widehat x.
$$

The aim is to make the transformed positive-definite matrix have clustered eigenvalues while keeping application of $P$ inexpensive.

##### Exact inverse-square-root preconditioner

↑ **Parent:** [Preconditioned conjugate gradient method](#preconditioned-conjugate-gradient-method)

For a positive-definite matrix $A$, choosing $P=A^{-1/2}$ gives $PAP^T=I$, so conjugate gradients terminates in one step. Constructing or applying the exact inverse square root is generally as expensive as solving the original system.

#### Krylov subspace

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krylov_subspace)

The order-$k$ Krylov subspace generated by $A$ and $b$ is

$$
\mathcal K_k(A,b)=\operatorname{span}\{b,Ab,\ldots,A^{k-1}b\}.
$$

##### Krylov dimension from spectral components

↑ **Parent:** [Krylov subspace](#krylov-subspace)

For a [diagonalizable](linear-operator-theory.md#diagonalizable-matrix) finite-dimensional operator, write $v=\sum_j u_j$ with nonzero $u_j$ in distinct [eigenspaces](linear-operator-theory.md#eigenspace) of eigenvalues $\lambda_j$. Then $A^rv=\sum_j\lambda_j^ru_j$. The [Vandermonde matrix](galois-theory.md#vandermonde-matrix) of the first $k$ powers is invertible for $k$ distinct eigenvalues, so these powers span exactly the $k$ independent components $u_j$. Thus the stabilized [Krylov subspace](#krylov-subspace) dimension is $k$. It counts distinct spectral components, not the number of nonzero coefficients in an arbitrary eigenbasis: $A=I$, $v=e_1+e_2$ has Krylov dimension one. Equivalently it is the minimum number of eigenvectors needed when those vectors may be chosen freely.

#### Finite termination of the conjugate gradient method

↑ **Parent:** [Conjugate gradient method](#conjugate-gradient-method)

In exact arithmetic, conjugate gradients reaches the exact solution in at most the number of distinct eigenvalues of $A$, and therefore in at most $n$ steps for an $n$-dimensional system.

### Heavy-ball method

↑ **Parent:** [Gradient descent](#gradient-descent)

The heavy-ball iteration adds momentum to gradient descent:

$$
x_{k+1}=x_k-\alpha\nabla F(x_k)+\beta(x_k-x_{k-1}).
$$

#### Heavy-ball residual recurrence

↑ **Parent:** [Heavy-ball method](#heavy-ball-method)

For $F(x)=x^TAx/2-b^Tx$ and $r_k=b-Ax_k$,

$$
r_{k+1}=((1+\beta)I-\alpha A)r_k-\beta r_{k-1}.
$$

Thus $r_k$ is a polynomial in $A$ applied to the initial residual and lies in the corresponding [Krylov subspace](#krylov-subspace).

#### Heavy-ball error propagation matrix

↑ **Parent:** [Heavy-ball method](#heavy-ball-method)

For $e_k=x^*-x_k$,

$$
\binom{e_{k+1}}{e_k}
=
\begin{pmatrix}
(1+\beta)I-\alpha A&-\beta I\\
I&0
\end{pmatrix}
\binom{e_k}{e_{k-1}}.
$$

If $A$ is diagonal with entries $\lambda_i$, a coordinate permutation turns this matrix into blocks

$$
\begin{pmatrix}1+\beta-\alpha\lambda_i&-\beta\\1&0\end{pmatrix}.
$$

##### Heavy-ball rate for a two-eigenvalue diagonal quadratic

↑ **Parent:** [Heavy-ball error propagation matrix](#heavy-ball-error-propagation-matrix)

For $A=\operatorname{diag}(1,\gamma)$, $\alpha=1/\gamma$, and $\beta=(1-\gamma^{-1/2})^2$, every error-propagation block has spectral radius at most $1-\gamma^{-1/2}$, and equality occurs.

## Peano kernel theorem

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Peano_kernel_theorem)

The Peano kernel theorem represents a linear approximation error $L$ that annihilates polynomials below degree $r$ as

$$
L(f)=\int_a^bK(t)f^{(r)}(t)\,dt,
\qquad
K(t)=L\left(\frac{(x-t)_+^{r-1}}{(r-1)!}\right).
$$

### Peano kernel

↑ **Parent:** [Peano kernel theorem](#peano-kernel-theorem)

The Peano kernel of a linear error functional $L$ that annihilates all polynomials of degree at most $k$ is

$$
K(\theta)=L[(x-\theta)^k_+/k!].
$$

It represents the error by integrating $K$ against the $(k+1)$st derivative.

#### Centered second-derivative Peano kernel

↑ **Parent:** [Peano kernel](#peano-kernel)

For $L(f)=f''(0)-f(-1)+2f(0)-f(1)$ on $C^3[-1,1]$, quadratic polynomials are annihilated. The [Peano kernel theorem](#peano-kernel-theorem) gives $L(f)=\int_{-1}^1K(t)f'''(t)\,dt$, with the displayed kernel; its value at zero does not affect the integral. Its absolute integral is $1/3$, proving $|L(f)|\le\|f'''\|_\infty/3$. The kernel changes sign, consistent with exactness also on cubic polynomials despite the estimate using only three derivatives.

#### Sharp Peano bound for an interior three-point first derivative

↑ **Parent:** [Peano kernel](#peano-kernel)

For $L(f)=-5f(0)/3+4f(1/2)/3+f(1)/3-f'(1/3)$ on $C^3[0,1]$, quadratic polynomials are annihilated. Taylor's formula with integral remainder gives $L(f)=\int_0^1K(t)f'''(t)dt$ with $K(t)=2(1/2-t)_+^2/3+(1-t)^2/6-(1/3-t)_+$. This [Peano kernel](#peano-kernel) is nonnegative throughout the interval and integrates to $1/36$, giving the sharp bound; $f(x)=x^3/6$ attains equality. The derivative is at an interior point, so this is distinct from an endpoint differentiation formula.

#### Sharp error constants for a Peano kernel

↑ **Parent:** [Peano kernel](#peano-kernel)

If $\lambda(f)=k!^{-1}\int K f^{(k+1)}$, the best unrestricted derivative-norm bounds are $|\lambda(f)|\le \|K\|_\infty\|f^{(k+1)}\|_1/k!$ and $|\lambda(f)|\le\|K\|_1\|f^{(k+1)}\|_\infty/k!$. Continuous concentrated bumps approach the first constant, and continuous approximations to $\operatorname{sgn}K$ approach the second. For the [three-point asymmetric second-derivative formula](finite-difference.md#three-point-asymmetric-second-derivative-formula), these constants are $5/6$ and $7/9$.

##### Sharp Peano-kernel constant for the three-point endpoint first derivative

↑ **Parent:** [Sharp error constants for a Peano kernel](#sharp-error-constants-for-a-peano-kernel)

For $L(f)=f'(0)+\frac32f(0)-2f(1)+\frac12f(2)$ on $C^3[0,2]$, the [Peano kernel](#peano-kernel) is

$$
K(t)=\begin{cases}t-\frac34t^2,&0\le t\le1,\\\frac14(2-t)^2,&1\le t\le2.\end{cases}
$$

The [Taylor expansion](calculus.md#taylor-expansion) with [integral](calculus.md#integral) remainder gives $L(f)=\int_0^2K(t)f^{(3)}(t)\,dt$, because $L$ annihilates [polynomials](polynomial.md) of degree at most two. Since $K\ge0$ and $\int_0^2K=1/3$, the sharp bound is $|L(f)|\le\frac13\|f^{(3)}\|_\infty$. Equality holds for $f(x)=x^3/6$.

### Four-point one-sided second-derivative formula

↑ **Parent:** [Peano kernel theorem](#peano-kernel-theorem)

At unit spacing, exactness through cubic polynomials gives

$$
f''(-1)\approx2f(-1)-5f(0)+4f(1)-f(2).
$$

#### Sharp Peano-kernel constant for the four-point endpoint second derivative

↑ **Parent:** [Four-point one-sided second-derivative formula](#four-point-one-sided-second-derivative-formula)

If the fourth-order Peano kernel of the four-point endpoint formula is nonnegative, its sharp sup-norm error constant is its integral. Evaluating the error on $(x+1)^4/24$ gives

$$
c=\int_{-1}^2K(t)\,dt=\frac{11}{12}.
$$

## Periodic trapezoidal Fourier aliasing

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a two-periodic Fourier series sampled at $2N$ equally spaced points, discrete averaging retains exactly the modes divisible by $2N$:

$$
I_N(h)-I(h)=\sum_{j\ne0}\widehat h_{2Nj}.
$$

If $|\widehat h_n|\leq Mc^{|n|}$ with $0<c<1$, then

$$
|I_N-I|\leq\frac{2Mc^{2N}}{1-c^{2N}},
$$

which is exponentially small.

### Periodic N-point rectangle-rule error

↑ **Parent:** [Periodic trapezoidal Fourier aliasing](#periodic-trapezoidal-fourier-aliasing)

For a two-periodic function and $N$ equally spaced samples,

$$
\frac2N\sum_{k=-N/2+1}^{N/2}h(2k/N)
=2\sum_{j\in\mathbb Z}\widehat h_{jN}.
$$

Consequently

$$
e_N(h)=-2\sum_{j\ne0}\widehat h_{jN}.
$$

Exponential [Fourier coefficient](fourier-series.md#fourier-coefficient) decay therefore gives exponential convergence in $N$.

## Fourier-Galerkin matrix for a drift-diffusion equation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For $u_t=u_{xx}-w'u_x$ and Fourier truncation $|n|\leq D$,

$$
\dot{\widehat u}_n=\sum_{|m|\leq D}B_{nm}\widehat u_m,
$$

where

$$
B_{nm}=-\pi^2n^2\delta_{nm}
+\pi^2(n-m)m\,\widehat w_{n-m}.
$$

For $w(x)=\cos\pi x$, the nonconstant block has Gershgorin discs in the closed left half-plane, while the constant mode lies in the kernel. Hence every eigenvalue has nonpositive real part and the matrix is singular.

## Fourier spectral method for variable-coefficient advection

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For $u_t+c(x)u_x=0$ with two-periodic Fourier truncations $|n|\leq d$, let $C_{nm}=\widehat c_{n-m}$ and $D_{mm}=m$. Fourier projection gives

$$
\dot{\widehat{\mathbf u}}=-i\pi CD\widehat{\mathbf u}.
$$

### Positive Fourier-symbol Toeplitz matrix

↑ **Parent:** [Fourier spectral method for variable-coefficient advection](#fourier-spectral-method-for-variable-coefficient-advection)

If a real Fourier polynomial $c(x)$ is strictly positive, then $C_{nm}=\widehat c_{n-m}$ is Hermitian positive definite because

$$
z^*Cz=\frac12\int_{-1}^1c(x)
\left|\sum_{m=-d}^dz_me^{i\pi mx}\right|^2dx>0
$$

for every nonzero $z$.

### Real spectrum of a positive-Hermitian times Hermitian product

↑ **Parent:** [Fourier spectral method for variable-coefficient advection](#fourier-spectral-method-for-variable-coefficient-advection)

If $C$ is Hermitian positive definite and $D$ is Hermitian, every eigenvalue of $CD$ is real. Equivalently, $CD$ is similar to the Hermitian matrix $C^{1/2}DC^{1/2}$.

### Explicit Euler instability on a nonzero imaginary eigenvalue

↑ **Parent:** [Fourier spectral method for variable-coefficient advection](#fourier-spectral-method-for-variable-coefficient-advection)

For $y'=i\omega y$ with real nonzero $\omega$, explicit Euler has amplification factor $1+i\omega h$, whose modulus $\sqrt{1+\omega^2h^2}$ exceeds one for every $h>0$.

## Runge-Kutta method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Runge-Kutta_method)

### Maximal-order Runge-Kutta methods are A-stable

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

An $s$-stage [Runge-Kutta method](#runge-kutta-method) has [stability function](#stability-function) $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$, a [rational function](isolated-singularity.md#rational-function) with numerator and denominator degrees at most $s$. Order $2s$ forces $R(z)-e^z=O(z^{2s+1})$, so uniqueness of the diagonal [Padé approximant](isolated-singularity.md#pade-approximant) identifies $R$ with $[s/s]_{e^z}$. That approximant has no poles in the closed left half-plane and modulus at most one there. Hence every such maximal-order method is [A-stable](#a-stability). Since the [Padé approximant](isolated-singularity.md#pade-approximant) numerator and denominator are coprime and both have degree $s$, the original stage [determinant](linear-algebra.md#determinant) cannot have hidden canceled poles in that half-plane.

### Theta method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

This one-step family interpolates between the [Forward Euler method](#euler-method) at $a=0$, the [trapezoidal rule](#trapezoidal-rule) at $a=1/2$, and the [Backward Euler method](#backward-euler-method) at $a=1$. Its [stability function](#stability-function) is $R(z)=[1+(1-a)z]/[1-az]$. It is first order except at one half, where it is second order. Applying it to spatial diffusion gives the [theta diffusion stability criterion](#theta-diffusion-stability-criterion).

#### Theta diffusion stability criterion

↑ **Parent:** [Theta method](#theta-method)

On an orthogonal diffusion eigenmode, the [theta method](#theta-method) has the displayed amplification with $s=-\Delta t\lambda$. The identity $(1+as)^2-[1-(1-a)s]^2=2s+(2a-1)s^2$ proves contraction at all nonnegative $s$ exactly when $a\geq1/2$. For $a<1/2$, contraction holds up to $s\leq2/(1-2a)$, with a positive denominator in that range. Orthogonality is what transfers these modal bounds to a full [L2 norm](real-analysis.md#l2-norm) estimate.

##### Rough-data damping distinction for the theta method

↑ **Parent:** [Theta diffusion stability criterion](#theta-diffusion-stability-criterion)

At $a=1/2$, arbitrarily stiff heat modes approach amplification $-1$: the [Crank-Nicolson method](#crank-nicolson-method) is contractive but does not rapidly damp unresolved rough components. The [Backward Euler method](#backward-euler-method) instead has limit zero. Thus unconditional linear stability and strong stiff decay are different requirements. High smooth-data consistency order alone does not imply a uniform high-order estimate down to the initial instant for arbitrary [L2 initial conditions](differential-equation.md#l2-initial-condition).

### Strong stability preserving Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

A strong stability preserving Runge-Kutta method writes its stages as convex combinations of previously computed states and suitable [Forward Euler method](#euler-method) steps. It transfers any convex-functional nonincrease property of the forward step, such as a [norm](functional-analysis.md#norm) bound, under a proportionally scaled time-step restriction.

For example, if $E_k(U)=U+kF(U)$ is nonexpansive in a [norm](functional-analysis.md#norm), then $Y=E_k(U)$ and $U_{\mathrm{new}}=(U+E_k(Y))/2$ is also nonexpansive: the [triangle inequality](topological-analysis.md#triangle-inequality) bounds the new difference by one half of the initial difference plus one half of the twice-advanced difference. Both are at most the initial difference. A [Taylor expansion](calculus.md#taylor-expansion) yields $U_{\mathrm{new}}=U+kF(U)+k^2F'(U)F(U)/2+O(k^3)$, so this is a second-order [Runge-Kutta method](#runge-kutta-method). The forward-step hypothesis must hold on the stage states; preservation of one chosen convex bound is not the same as unconditional [B-stability](#b-stability).

### Classical fourth-order Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

The classical four-stage explicit [Runge-Kutta method](#runge-kutta-method) uses

$$
A=\begin{pmatrix}0&0&0&0\\1/2&0&0&0\\0&1/2&0&0\\0&0&1&0\end{pmatrix},\qquad
b=(1/6,1/3,1/3,1/6)^T,\qquad c=(0,1/2,1/2,1)^T.
$$

It satisfies the [fourth-order conditions for a Runge-Kutta method](#fourth-order-conditions-for-a-runge-kutta-method). Its polynomial [stability function](#stability-function) excludes [A-stability](#a-stability), while $|R(iq)|^2=1-q^6/72+q^8/576$ gives the imaginary-axis stability interval $|q|\leq2\sqrt2$.

### Butcher tableau

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

A Butcher tableau records a Runge-Kutta method's stage matrix $A$, nodes $c$, and output weights $b$ in the block array

$$
\begin{array}{c|c}c&A\\\hline&b^T\end{array}.
$$

### Butcher order condition

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

A Butcher order condition equates the coefficient assigned by a [Runge-Kutta method](#runge-kutta-method) to a rooted tree with the corresponding exact Taylor coefficient. Satisfying every condition through tree order $p$ is equivalent to Runge–Kutta order at least $p$.

#### Second-order conditions with independent Runge-Kutta abscissae

↑ **Parent:** [Butcher order condition](#butcher-order-condition)

For a general nonautonomous [Runge-Kutta method](#runge-kutta-method), [Taylor expansion](calculus.md#taylor-expansion) of stage $i$ gives $k_i=f+h[c_if_t+(Ae)_if_yf]+O(h^2)$. Matching the exact increment $hf+h^2(f_t+f_yf)/2$ gives the three displayed conditions. When internal consistency $c=Ae$ is imposed, the last two coincide. Internal consistency is a usual tableau convention, but is not logically necessary for order two of a generalized tableau.

#### Fourth-order conditions for a Runge-Kutta method

↑ **Parent:** [Butcher order condition](#butcher-order-condition)

With $c=Ae$ and $C=\operatorname{diag}(c)$, a [Runge-Kutta method](#runge-kutta-method) has order at least four exactly when the eight [Butcher order conditions](#butcher-order-condition)

$$
b^Te=1,\quad b^Tc=\frac12,\quad b^Tc^2=\frac13,\quad b^TAc=\frac16,\quad b^Tc^3=\frac14,\quad b^TCAc=\frac18,\quad b^TAc^2=\frac1{12},\quad b^TA^2c=\frac1{24}
$$

hold; powers of $c$ are componentwise. These conditions match the numerical and exact coefficients indexed by [rooted trees](combinatorics.md#rooted-tree) through order four. Matching the scalar [Dahlquist test equation](#dahlquist-test-equation) alone is insufficient to check the nonlinear [Butcher order conditions](#butcher-order-condition).

### Implicit Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_Runge-Kutta_method)

An implicit Runge-Kutta method defines one or more stages through equations involving those same stages.

#### Two-stage Runge-Kutta family with an implicit second stage

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

For stages $k_1=f(y)$ and $k_2=f(y+(1-a)hk_1+ahk_2)$ with update $y+h(k_1+k_2)/2$, the method has order two for every fixed real $a$. The third-order coefficient of $f''f^2$ is always $1/4$, not $1/6$, so no parameter gives third order on general nonlinear equations. The displayed [stability function](#stability-function) is bounded throughout the left half-plane only when $a=1/2$, when it is the A-stable trapezoidal function $(1+z/2)/(1-z/2)$. It is not L-stable.

#### Stage solvability of an implicit Runge-Kutta method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

For a vector field uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity) in the state with constant $L$, the stage fixed-point map of an [implicit Runge-Kutta method](#implicit-runge-kutta-method) is a contraction in the maximum stage norm if $hL\max_i\sum_j|a_{ij}|<1$. The [contraction mapping theorem](analysis.md#contraction-mapping-theorem) then gives unique stages. This is a sufficient small-step condition; a [dissipative vector field](differential-equation.md#dissipative-vector-field) may permit solvability for larger steps. An [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) or [B-stability](#b-stability) estimate compares existing stage solutions and should not be mistaken for an unqualified stage-existence theorem.

#### Implicit midpoint rule

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

The implicit midpoint rule advances an autonomous ordinary differential equation by

$$
y_{n+1}=y_n+h f\left(\frac{y_n+y_{n+1}}2\right).
$$

It is a second-order, [A-stable](#a-stability), [time-symmetric numerical method](#time-symmetric-numerical-method).

The [implicit midpoint rule](#implicit-midpoint-rule) is the [midpoint method](#midpoint-method) with $y_{n+1}=y_n+h f(t_n+h/2,(y_n+y_{n+1})/2)$. It is a one-stage [implicit Runge-Kutta method](#implicit-runge-kutta-method).

#### Crank-Nicolson method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crank–Nicolson_method)

The Crank--Nicolson method applies the [trapezoidal rule](#trapezoidal-rule) to a semidiscrete evolution equation. For a linear system $u'=Lu$ its update is

$$
\left(I-\frac h2L\right)u^{n+1}=\left(I+\frac h2L\right)u^n.
$$

##### Contractivity of split Crank-Nicolson diffusion

↑ **Parent:** [Crank-Nicolson method](#crank-nicolson-method)

For symmetric negative semidefinite matrices $A,B$, each factor $C_A(h)=(I-hA/2)^{-1}(I+hA/2)$ has norm at most one, since its eigenvalues are $(1+h\lambda/2)/(1-h\lambda/2)$ with $\lambda\le0$. The same holds for $B$, so their ordered product is a contraction for every $h\ge0$, whether or not $A,B$ commute. This proves unconditional discrete [L2 norm](real-analysis.md#l2-norm) stability of the split [Crank-Nicolson method](#crank-nicolson-method) for directional diffusion. Its splitting error remains first order in general, because the product's quadratic defect is $h^2[A,B]/2$.

#### Collocation Runge-Kutta method

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)

Given distinct nodes $c_i$, a collocation Runge-Kutta method uses the Lagrange basis $\ell_j$ with $a_{ij}=\int_0^{c_i}\ell_j(\tau)d\tau$ and $b_j=\int_0^1\ell_j(\tau)d\tau$. Its stages enforce the differential equation at the collocation nodes.

This applies the [collocation method](#collocation-method) to the time-step polynomial of an [ordinary differential equation](differential-equation.md#ordinary-differential-equation).

##### Two-node collocation A-stability criterion

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For distinct nodes $c_1,c_2\in[0,1]$, the two-stage [collocation Runge-Kutta method](#collocation-runge-kutta-method) has [stability function](#stability-function)

$$
R(z)=\frac{1+(1-a)z+rz^2}{1-az+dz^2},\qquad a=(c_1+c_2)/2,\quad d=c_1c_2/2,\quad r=(1-c_1)(1-c_2)/2.
$$

The denominator has no zeros in the closed left half-plane. On the imaginary axis the denominator's squared modulus minus the numerator's is $(d^2-r^2)y^4$. Thus $d\geq r$, equivalently $c_1+c_2\geq1$, is necessary and sufficient for [A-stability](#a-stability), using the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) and the bound at infinity.

##### Collocation order theorem

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For $s$ distinct collocation nodes, let $\pi_s(t)=\prod_{i=1}^s(t-c_i)$. If $\int_0^1t^j\pi_s(t)dt=0$ for $0\le j<k$, and the next moment is nonzero, the associated interpolatory quadrature has order $s+k$, and the [collocation Runge-Kutta method](#collocation-runge-kutta-method) has the same classical order for sufficiently smooth differential equations. Here $0\le k\le s$. Equivalently, if the quadrature is exact through degree $p-1$ but not degree $p$, the method has order $p$. The generic order is at least $s$, [Gauss collocation methods](#gauss-legendre-method) reach $2s$, and [Radau IIA methods](#radau-iia-method) reach $2s-1$.

###### Collocation endpoint superconvergence by quadrature orthogonality

↑ **Parent:** [Collocation order theorem](#collocation-order-theorem)

For $s$ collocation nodes, the residual of the collocation polynomial vanishes at each node and contains the factor $\omega(\tau)=\prod_i(\tau-c_i)$. Quadrature exactness through degree $q-1$ implies $\int_0^1\omega(\tau)p(\tau)d\tau=0$ for every polynomial of degree at most $q-s-1$. Expand the smooth vector-field interpolation error and the derivative of the exact flow in powers of the step. Every endpoint-error term of degree below $q$ has this vanishing weighted moment, so the endpoint local error is $O(h^{q+1})$, although the interior stage accuracy is generally only $s$. A step Lipschitz estimate and [discrete Gronwall inequality](probability-and-statistics.md#discrete-gronwall-inequality) then give global order $q$. Gaussian nodes attain $q=2s$, while the first nonexact quadrature moment bounds the order from above.

##### Collocation tableau row-sum identity

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

For a [collocation Runge-Kutta method](#collocation-runge-kutta-method), $a_{ij}=\int_0^{c_i}\ell_j(t)dt$, where the [Lagrange interpolation](#lagrange-polynomial) basis obeys $\sum_j\ell_j=1$. Hence each row sum is its collocation node. Failure of this identity disproves a claimed collocation tableau with those nodes. The identity alone is necessary rather than sufficient: the individual integrated basis coefficients must also agree.

##### Lobatto IIIA method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

A Lobatto IIIA method collocates at the [Lobatto quadrature](#lobatto-quadrature) nodes, including both endpoints of the time interval. Its three-stage version has

$$
A=\begin{pmatrix}0&0&0\\5/24&1/3&-1/24\\1/6&2/3&1/6\end{pmatrix},
\qquad b=(1/6,2/3,1/6)^T,
\qquad c=(0,1/2,1)^T.
$$

The [Butcher order conditions](#butcher-order-condition) give order four. Its [stability function](#stability-function) is

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},
$$

which is [A-stable](#a-stability) but not [L-stable](#l-stability). It is not [algebraically stable](#algebraic-stability-of-a-runge-kutta-method): the first diagonal entry of the defining [matrix](vector-space.md#matrix) is $2b_1a_{11}-b_1^2=-1/36$. This distinguishes linear [A-stability](#a-stability) from nonlinear [algebraic stability](#algebraic-stability-of-a-runge-kutta-method).

##### Gauss-Legendre method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Legendre_method)

The $s$-stage Gauss--Legendre Runge--Kutta method collocates at the Gauss--Legendre quadrature nodes on $[0,1]$. It is symmetric, A-stable, and has order $2s$.

###### Gauss collocation coefficient construction

↑ **Parent:** [Gauss-Legendre method](#gauss-legendre-method)

Choose $c_1,\ldots,c_s$ as the [polynomial roots](polynomial.md#root-of-a-polynomial) of $P_s(2c-1)$ in $(0,1)$, and form the [Lagrange interpolation polynomials](#lagrange-polynomial) $\ell_j(t)=\prod_{m\ne j}(t-c_m)/(c_j-c_m)$. The [Gauss collocation method](#gauss-legendre-method) has $a_{ij}=\int_0^{c_i}\ell_j(t)dt$ and $b_j=\int_0^1\ell_j(t)dt$. This gives explicit coefficient formulas after finding [polynomial roots](polynomial.md#root-of-a-polynomial): if $\ell_j(t)=\sum_rd_{jr}t^r$, these [integrals](calculus.md#integral) are $\sum_rd_{jr}c_i^{r+1}/(r+1)$ and $\sum_rd_{jr}/(r+1)$. [Gaussian quadrature](#gaussian-quadrature) gives order $2s$.

###### Fourth-order two-stage Gauss collocation method

↑ **Parent:** [Gauss-Legendre method](#gauss-legendre-method)

The two-stage [Gauss--Legendre Runge-Kutta method](#gauss-legendre-method) uses nodes $c_{1,2}=1/2\mp\sqrt3/6$, weights $b_1=b_2=1/2$ and coefficients $a_{11}=a_{22}=1/4$, $a_{12}=1/4-\sqrt3/6$, $a_{21}=1/4+\sqrt3/6$. The [Butcher order conditions](#butcher-order-condition) give order four. Its [stability function](#stability-function) is the displayed rational function, which is [A-stable](#a-stability). The [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) matrix is zero, so positive weights also give nonlinear contractivity for dissipative vector fields.

##### Radau IIA method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

An $s$-stage Radau IIA method collocates at the right-endpoint Radau nodes. It has order $2s-1$ and is both [algebraically stable](#algebraic-stability-of-a-runge-kutta-method) and [L-stable](#l-stability).

<h6 id="pade-identification-of-a-radau-stability-function">Padé identification of a Radau stability function</h6>

↑ **Parent:** [Radau IIA method](#radau-iia-method)

Suppose an $s$-stage [Runge-Kutta method](#runge-kutta-method) has order $2s-1$, an [invertible matrix](linear-algebra.md#invertible-matrix) $A$, and $b^TA^{-1}\mathbf1=1$. Its [stability function](#stability-function) is $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. The [adjugate matrix](linear-algebra.md#adjugate-matrix) formula gives a [rational function](isolated-singularity.md#rational-function) with denominator degree $s$ and numerator degree at most $s$; its zero [limit](calculus.md#limit-of-a-function) at infinity lowers the latter degree to at most $s-1$. The [order of a numerical method](#order-of-a-numerical-method) gives $R(z)-e^z=O(z^{2s})$, identifying the $[s-1/s]$ [Padé approximant](isolated-singularity.md#pade-approximant). Uniqueness follows because the cross-multiplied difference of two candidates has degree at most $2s-1$ but a zero of order at least $2s$, so is identically zero. The [A-stability of near-diagonal exponential Padé approximants](#a-stability-of-near-diagonal-exponential-pade-approximants) then proves [A-stability](#a-stability), and the zero limit proves [L-stability](#l-stability). These conditions identify the stability function; they do not alone claim uniqueness of all entries of the [Runge-Kutta method](#runge-kutta-method) tableau.

##### Algebraic stability of a Runge-Kutta method

↑ **Parent:** [Collocation Runge-Kutta method](#collocation-runge-kutta-method)

A Runge-Kutta method is algebraically stable when $b_i\geq0$ and the matrix $M$ with $M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j$ is positive semidefinite. Algebraic stability implies contractivity for dissipative differential equations.

###### Runge-Kutta conservation of quadratic invariants

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

For stage states $Y_i=y_n+h\sum_ja_{ij}k_j$ and a vector field with $Y_i^Tk_i=0$, expansion of the new squared norm gives $\|y_{n+1}\|^2-\|y_n\|^2=-h^2\sum_{i,j}M_{ij}k_i^Tk_j$, where $M_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j$. Hence $M=0$ preserves the [quadratic form](linear-algebra.md#quadratic-form) exactly for every well-defined step. The same argument with a fixed symmetric matrix in the inner product preserves any quadratic invariant of the vector field. In particular it preserves the Euclidean norm for a [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) differential equation.

###### Butcher contractivity theorem

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

An [algebraically stable](#algebraic-stability-of-a-runge-kutta-method) [Runge-Kutta method](#runge-kutta-method) is [B-stable](#b-stability): for a [dissipative vector field](differential-equation.md#dissipative-vector-field), a well-defined step cannot increase the distance between two starting values. This assumes that the compared stage equations have solutions, as required by [stage solvability of an implicit Runge-Kutta method](#stage-solvability-of-an-implicit-runge-kutta-method). The [Runge-Kutta contractivity identity](#runge-kutta-contractivity-identity) expresses the distance change as a nonpositive weighted term coming from the [dissipative vector field](differential-equation.md#dissipative-vector-field) minus a nonnegative [quadratic form](linear-algebra.md#quadratic-form) involving the matrix defining [algebraic stability](#algebraic-stability-of-a-runge-kutta-method). Positive weights also rule out stage poles in the open left half-plane on the scalar test equation, giving [A-stability](#a-stability) there; zero-weight redundant stages need separate solvability attention.

###### Runge-Kutta contractivity identity

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method)

For differences $D_i$ between corresponding stages and differences $F_i$ between their vector fields, a Runge--Kutta step satisfies

$$
\|d_{n+1}\|^2=\|d_n\|^2+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

To derive the identity, expand the squared [norm](functional-analysis.md#norm) of $d_{n+1}=d_n+h\sum_i b_iF_i$ and substitute $d_n=D_i-h\sum_j a_{ij}F_j$ in the linear term. Symmetrizing the double sum gives the displayed coefficients $m_{ij}$. For a [dissipative vector field](differential-equation.md#dissipative-vector-field), the first sum is nonpositive when $b_i\geq0$, and the second sum is nonnegative when the [matrix](vector-space.md#matrix) $(m_{ij})$ is a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix). Thus [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) implies [B-stability](#b-stability).

#### Trapezoidal rule

↑ **Parent:** [Implicit Runge-Kutta method](#implicit-runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trapezoidal_rule)

The trapezoidal ODE rule averages vector fields at the old and new states and is A-stable.

##### Trapezoidal rule fails B-stability

↑ **Parent:** [Trapezoidal rule](#trapezoidal-rule)

The [trapezoidal rule](#trapezoidal-rule) is [A-stable](#a-stability) but is not [B-stable](#b-stability). For the [dissipative vector field](differential-equation.md#dissipative-vector-field) $f(y)=-y^3$ at step size one, its uniquely defined step map $T$ obeys $T+T^3/2=y-y^3/2$. At $y=\sqrt2$, $T=0$ and implicit differentiation gives $T'=-2$, so nearby states expand rather than contract. This is a concrete nonlinear obstruction, rather than merely failure of the sufficient [algebraic stability](#algebraic-stability-of-a-runge-kutta-method) criterion.

### Time-symmetric numerical method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)

A one-step numerical method with step map $\Phi_h$ is time symmetric when $\Phi_{-h}=\Phi_h^{-1}$. Its leading local-error power is odd, so every nontrivial consistent time-symmetric method has even order.

### Order of a Runge-Kutta method

↑ **Parent:** [Runge-Kutta method](#runge-kutta-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_of_a_Runge-Kutta_method)

The order is the highest power through which the one-step expansion matches the exact Taylor expansion.

#### Third-order conditions for an explicit Runge-Kutta method

↑ **Parent:** [Order of a Runge-Kutta method](#order-of-a-runge-kutta-method)

For an explicit [Runge-Kutta method](#runge-kutta-method) with coefficients $A,b$, put $c=A\mathbf1$ and let $c^2$ mean componentwise squaring. The conditions $b^T\mathbf1=1$, $b^Tc=1/2$, $b^Tc^2=1/3$ and $b^TAc=1/6$ match the exact flow expansion through degree three: the two cubic differentials are $f^{\prime\prime}[f,f]$ and $(f^\prime)^2f$. For sufficiently smooth vector fields these give local error $O(h^4)$ and, under the usual finite-interval [Lipschitz continuity](real-analysis.md#lipschitz-continuity) assumptions, global error $O(h^3)$.

## Simplex algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex_algorithm)

### Dual simplex algorithm

↑ **Parent:** [Simplex algorithm](#simplex-algorithm)

The dual simplex algorithm keeps the objective row dual feasible while repairing negative basic values. In a maximization dictionary $x_B=b+\sum_j a_jx_j$ with $b<0$ and nonbasic objective coefficients $d_j\leq0$, eligible entering columns have $a_j>0$; choose one minimizing $(-d_j)/a_j$. The pivot restores progress toward primal feasibility without losing the objective bound.

### Simplex dictionary

↑ **Parent:** [Simplex algorithm](#simplex-algorithm)

A simplex dictionary expresses the basic variables and the objective as affine functions of the nonbasic variables in a [linear program](mathematical-optimization.md#linear-programming). Setting the nonbasic variables to zero gives a [basic feasible solution](mathematical-optimization.md#basic-feasible-solution) when all basic values are nonnegative. A [simplex algorithm](#simplex-algorithm) pivot exchanges one basic and one nonbasic variable. For maximization, a feasible dictionary with all nonbasic objective coefficients nonpositive certifies optimality.

## Sparse optimization

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sparse_optimization)

### Compressed sensing

↑ **Parent:** [Sparse optimization](#sparse-optimization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressed_sensing)

Compressed sensing reconstructs a [sparse vector](#sparse-vector), or an approximately sparse one, from fewer linear measurements than its ambient dimension. [Basis pursuit](#basis-pursuit) replaces counting nonzero coordinates by [convex](real-analysis.md#convex-function) $\ell^1$ minimization. A [null space property](#nullspace-property) characterizes exact uniform recovery, while a [robust null space property](#robust-null-space-property) controls errors from noise and nonsparse tails.

#### Coherence of a normalized matrix

↑ **Parent:** [Compressed sensing](#compressed-sensing)

For a [matrix](vector-space.md#matrix) with at least two columns of unit [Euclidean norm](functional-analysis.md#euclidean-norm), its mutual coherence is the largest magnitude of an [inner product](linear-algebra.md#inner-product) between distinct columns. It measures the strongest pairwise ambiguity of linear measurements. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $0\le\mu\le1$. The order-two [restricted isometry constant](#restricted-isometry-constant) equals the [mutual coherence](#coherence-of-a-normalized-matrix), because every two-column [Gram matrix](linear-algebra.md#gram-matrix) has eigenvalues $1\pm|\langle a_i,a_j\rangle|$.

##### Cumulative coherence

↑ **Parent:** [Coherence of a normalized matrix](#coherence-of-a-normalized-matrix)

For unit [Euclidean norm](functional-analysis.md#euclidean-norm) columns, cumulative coherence measures the largest sum of $k$ correlations with one other column. Its domain is $0\le k\le N-1$, with $\mu_1(0)=0$ by the empty-sum convention. It is nondecreasing, $\mu_1(1)=\mu$ for $N\ge2$, and $\mu_1(k)\le k\mu$, where $\mu$ is the [mutual coherence](#coherence-of-a-normalized-matrix). Keeping a sum of actual correlations can be substantially sharper than replacing each summand by the largest one.

###### Cumulative coherence bound for restricted isometry

↑ **Parent:** [Cumulative coherence](#cumulative-coherence)

For normalized columns and $1\le s\le N$, the [restricted isometry constant](#restricted-isometry-constant) is bounded by the [cumulative coherence](#cumulative-coherence) at $s-1$. A restricted [Gram matrix](linear-algebra.md#gram-matrix) has diagonal one and every off-diagonal row sum at most $\mu_1(s-1)$. The [Gershgorin circle theorem](#gershgorin-circle-theorem) and the [finite-dimensional spectral theorem](linear-operator-theory.md#finite-dimensional-spectral-theorem) bound its [eigenvalues](linear-operator-theory.md#eigenvalue) between $1-\mu_1(s-1)$ and $1+\mu_1(s-1)$. At $s=1$ the distortion is zero, and at $s=2$ it is exactly the [mutual coherence](#coherence-of-a-normalized-matrix).

#### Sparse injectivity

↑ **Parent:** [Compressed sensing](#compressed-sensing)

A [linear map](vector-space.md#linear-map) is injective on the class of [sparse vectors](#sparse-vector) of order $s$ exactly when its [null space](linear-algebra.md#kernel-of-a-linear-map) contains no nonzero [vector](vector-space.md#vector) with at most $2s$ nonzero entries. Differences of two sparse [vectors](vector-space.md#vector) have at most $2s$ active coordinates. Conversely, splitting the [support of a vector](#support-of-a-vector) of a $2s$-sparse null [vector](vector-space.md#vector) into two parts constructs two distinct $s$-sparse [vectors](vector-space.md#vector) with the same image. The strict [null space property](#nullspace-property) implies sparse injectivity by applying it to both parts of such a split.

#### Restricted isometry property

↑ **Parent:** [Compressed sensing](#compressed-sensing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Restricted_isometry_property)

The restricted isometry property controls $\|Ax\|_2^2/\|x\|_2^2$ uniformly over [sparse vectors](#sparse-vector). It supplies quantitative near-orthogonality of disjoint sparse coordinate combinations, not merely normalization of individual columns.

##### Restricted isometry constant

↑ **Parent:** [Restricted isometry property](#restricted-isometry-property)

The order-s restricted isometry constant is the smallest nonnegative $\delta$ satisfying $(1-\delta)\|x\|_2^2\le\|Ax\|_2^2\le(1+\delta)\|x\|_2^2$ for every vector with at most $s$ nonzero coordinates. Equivalently it is $\max_{|S|\le s}\|A_S^*A_S-I\|_{2\to2}$. The sparse-vector quantifier is essential, and the constant can equal zero.

###### Sharp order-s restricted-isometry recovery theorem

↑ **Parent:** [Restricted isometry constant](#restricted-isometry-constant)

For $s\ge2$ and $\delta=\delta_s(A)<1/3$, noisy [basis pursuit](#basis-pursuit) has error $\|\hat x-x_0\|_2\le C_1\eta+C_2\sigma_s(x_0)/\sqrt s$, with constants depending only on $\delta$. One admissible pair is

$$
C_1=\frac{2\sqrt{2(1+\delta)}}{1-3\delta},\qquad
C_2=\frac{2\sqrt2(2\delta+\sqrt{(1-3\delta)\delta})+2(1-3\delta)}{1-3\delta}.
$$

These constants follow from Theorem 3.3 of [the sharp restricted-isometry recovery analysis](https://arxiv.org/pdf/1302.1236), with the actual noise bounded by the tolerance $\eta$. The restriction $s\ge2$ is necessary: equal unit columns give $\delta_1=0$ without unique recovery. The coefficient of the approximation term cannot universally be one.

#### Basis pursuit

↑ **Parent:** [Compressed sensing](#compressed-sensing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basis_pursuit)

Basis pursuit minimizes an $\ell^1$ [norm](functional-analysis.md#norm) subject to exact linear measurements. Basis pursuit with a noise tolerance replaces the equality by $\|Ax-y\|_2\le\eta$. A unique minimizer has linearly independent active columns, and hence at most $\operatorname{rank}A$ nonzero coordinates: a null direction on its support would make the objective locally affine on a feasible line, contradicting minimality or uniqueness.

##### Strict dual certificate for basis pursuit

↑ **Parent:** [Basis pursuit](#basis-pursuit)

For a real [vector](vector-space.md#vector) $x$ with [support of a vector](#support-of-a-vector) $S$, this certificate is a [vector](vector-space.md#vector) $h$ whose measurements under the [adjoint operator](hilbert-space.md#adjoint-operator) match the active [sign function](foundations-of-mathematics.md#sign-function) values and lie strictly between minus one and one on the inactive coordinates. If $A_S$ is [injective](algebra.md#injective-function), such a certificate proves that $x$ is the unique [basis pursuit](#basis-pursuit) [minimizer](analysis.md#global-minimizer). For a nonzero $v\in\ker A$, [injectivity](algebra.md#injective-function) ensures $v_{S^c}\ne0$, and $0=\langle A^*h,v\rangle$ implies the [fixed-sign null space condition](#fixed-sign-null-space-condition). The strict inequality is interpreted coordinatewise if $S^c$ is empty. The condition with the [sign function](foundations-of-mathematics.md#sign-function) written here is for real variables; complex [basis pursuit](#basis-pursuit) uses the unit phases of active coordinates instead.

###### Least-norm dual certificate

↑ **Parent:** [Strict dual certificate for basis pursuit](#strict-dual-certificate-for-basis-pursuit)

When $A_S$ is [injective](algebra.md#injective-function), this [vector](vector-space.md#vector) solves $A_S^*h_0=\operatorname{sgn}(x_S)$. Any other solution differs by a [vector](vector-space.md#vector) in $\ker A_S^*$, orthogonal to the range of $A_S$ containing $h_0$. The [Pythagorean identity](linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) therefore proves that $h_0$ has the smallest [Euclidean norm](functional-analysis.md#euclidean-norm). It is a [strict dual certificate for basis pursuit](#strict-dual-certificate-for-basis-pursuit) exactly when each inactive coordinate of $A^*h_0$ has magnitude less than one. Failure of that test does not rule out another certificate: a [null space](linear-algebra.md#kernel-of-a-linear-map) component of $A_S^*$ can alter those inactive coordinates.

##### Nullspace property

↑ **Parent:** [Basis pursuit](#basis-pursuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nullspace_property)

The null space property relative to $S$ is $\|h_S\|_1<\|h_{S^c}\|_1$ for every nonzero $h\in\ker A$. It is equivalent to exact [basis pursuit](#basis-pursuit) recovery of every vector supported in $S$. Sufficiency follows from the [triangle inequality](topological-analysis.md#triangle-inequality); for necessity, compare $-h_S$ and $h_{S^c}$, which have the same image under $A$. Recovery of a single fixed signed vector can hold without this uniform property.

###### Lq null space property

↑ **Parent:** [Nullspace property](#nullspace-property)

For $0<q\le1$, this strict inequality for every nonzero $v\in\ker A$ and every $|S|\le s$ is equivalent to unique constrained $\ell^q$ recovery of every [sparse vector](#sparse-vector) of order $s$. For sufficiency, use $|x_i+v_i|^q\ge|x_i|^q-|v_i|^q$ on the [support of a vector](#support-of-a-vector). For necessity compare $x=-v_S$ with $v_{S^c}$, which have the same measurements. The statement concerns uniform recovery over the whole sparse class, rather than a single signed [vector](vector-space.md#vector).

###### Monotonicity of uniform sparse recovery in the exponent

↑ **Parent:** [Lq null space property](#lq-null-space-property)

If the [Lq null space property](#lq-null-space-property) holds at $q\le1$, it holds at every $0<p<q$. Order a nonzero null [vector](vector-space.md#vector)'s magnitudes $a_1\ge\cdots\ge a_N$ and put $t=a_s>0$. Since $p-q<0$, the top-$s$ $p$-power sum is at most $t^{p-q}$ times its $q$-power sum, while the tail $p$-power sum is at least that multiple of the tail $q$-power sum. The strict $q$ inequality therefore gives the strict $p$ inequality. The largest $s$ magnitudes are the worst [support of a vector](#support-of-a-vector), so all other supports satisfy it too.

###### Robust null space property

↑ **Parent:** [Nullspace property](#nullspace-property)

The displayed property holds for every $h$ and every $|S|\le s$, with $0\le\rho<1$ and $\tau>0$. It converts the cone inequality from [basis pursuit](#basis-pursuit) minimality and the tube inequality from noisy feasibility into a two-constant bound $\|\hat x-x_0\|_2\le C_1\eta+C_2\sigma_s(x_0)/\sqrt s$. Both constants are needed in general; a fixed coefficient one on the approximation term does not follow.

###### Fixed-sign null space condition

↑ **Parent:** [Nullspace property](#nullspace-property)

For a real vector $x_0$ with support $S$, uniqueness in [basis pursuit](#basis-pursuit) is equivalent to $|\langle\operatorname{sgn}(x_{0,S}),h_S\rangle|<\|h_{S^c}\|_1$ for every nonzero $h\in\ker A$. The supporting-line inequality for the [absolute value](real-analysis.md#absolute-value) proves sufficiency. Taking small positive and negative multiples of $h$ before any active sign changes proves necessity.

#### Sparse vector

↑ **Parent:** [Compressed sensing](#compressed-sensing)

A vector is s-sparse if it has at most $s$ nonzero coordinates. For $x\in\mathbb R^N$, its best s-term $\ell^1$ approximation error is $\sigma_s(x)=\min_{z\text{ s-sparse}}\|x-z\|_1$, equal to the sum of the absolute values of the coordinates outside the largest $s$.

##### L0 sparsity count

↑ **Parent:** [Sparse vector](#sparse-vector)

The number of nonzero coordinates of a finite [vector](vector-space.md#vector) is its L0 sparsity count. It vanishes only at zero, but is unchanged under multiplication by a nonzero scalar, so it is not a [norm](functional-analysis.md#norm). Minimizing it under linear measurement constraints finds a [sparse vector](#sparse-vector) with the smallest possible [support of a vector](#support-of-a-vector). [Sparse injectivity](#sparse-injectivity) of order $s$ guarantees unique recovery of every [sparse vector](#sparse-vector) with at most $s$ nonzero coordinates by this objective.

##### Support of a vector

↑ **Parent:** [Sparse vector](#sparse-vector)

The support of a finite vector is the set of indices of its nonzero coordinates. It is the [support of a function](function.md#support) on a finite discrete index set, and its cardinality defines sparsity.

###### Maximum-support vector in a finite-dimensional subspace

↑ **Parent:** [Support of a vector](#support-of-a-vector)

For any [field](algebra.md#field) $F$ and [vector subspace](vector-space.md#vector-subspace) $W\subseteq F^m$, some $u\in W$ has at least $\dim W$ nonzero coordinates. Choose $u$ with largest [support of a vector](#support-of-a-vector) $S$. Restriction from $W$ to $F^S$ is injective: a nonzero vector in its [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) vanishes on $S$, so adding it to $u$ would enlarge $S$. Thus $\dim W\leq|S|$. The argument works over [finite fields](algebra.md#finite-field), where assuming a generic vector avoids finitely many hyperplanes would be invalid.

## Stability function

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stability_function)

### Dahlquist test equation

↑ **Parent:** [Stability function](#stability-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dahlquist_test_equation)

The Dahlquist test equation is the scalar linear initial-value problem $y'=\lambda y$. A one-step method reduces it to $y_{n+1}=R(h\lambda)y_n$, thereby defining its [stability function](#stability-function) $R$.

## Linear multistep method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_multistep_method)

A linear multistep method approximates an ODE using several previous solution and derivative values.

### Reciprocal-root three-step multistep family

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

Take $\sigma(\zeta)=\zeta[(5+\alpha)\zeta^2-(4+8\alpha)\zeta+11-5\alpha]/6$. The [root condition for a multistep method](#root-condition-for-a-multistep-method) holds exactly for $-1<\alpha<1$. Since $\rho'(1)=\sigma(1)=2(1-\alpha)$, these and only these parameters give a convergent method. Its [exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method) has defect $-(\alpha+5)z^4/12+O(z^5)$, giving formal order three except at $\alpha=-5$, where the first defect is $z^5/10$. None of the convergent family is [A-stable](#a-stability): for a parasitic root $r=\alpha+i\sqrt{1-\alpha^2}$, perturbation of $\rho(r(z))-z\sigma(r(z))=0$ gives $\operatorname{Re}[r'(0)/r]=(\alpha-1)/12<0$. A small negative real $z$ therefore moves it outside the unit disk. At $\alpha=1$, cancellation would remove a double unit root, but the original recurrence retains that unstable parasitic behavior; it is not legitimately replaced by the reduced Backward Euler recurrence for arbitrary starting values.

### Simpson multistep method

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

Integrating a quadratic interpolant of the derivative over two steps gives this [linear multistep method](#linear-multistep-method), which has order four. Its [local truncation error](#local-truncation-error) is $-h^5y^{(5)}(t_{n+1})/90+O(h^7)$ and its [zero-stability](#zero-stability) polynomial is $\rho(\zeta)=\zeta^2-1$, with simple roots $1,-1$. The [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem) therefore gives fourth-order convergence with sufficiently accurate starts. This attains the even two-step [first Dahlquist barrier](#first-dahlquist-barrier). Its undamped parasitic zero-step mode need not have favorable long-time [absolute stability](#linear-stability-domain); finite-time convergence and stiff damping are separate requirements.

### First Dahlquist barrier

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

For a consistent [zero-stable](#zero-stability) real linear $k$-step method with constant coefficients and only first-derivative evaluations, the attainable order is at most $k+1$ for odd $k$ and $k+2$ for even $k$. For an explicit method the bound is $k$. These are order barriers under the [root condition for a multistep method](#root-condition-for-a-multistep-method), not bounds on multiderivative methods or on arbitrary variable-step formulations. The [Second Dahlquist barrier](#second-dahlquist-barrier) adds the stronger bound of order two for irreducible [A-stable](#a-stability) methods.

#### Newton-Cotes multistep methods attaining the first Dahlquist barrier

↑ **Parent:** [First Dahlquist barrier](#first-dahlquist-barrier)

Using [Newton-Cotes closed quadrature](#newton-cotes-closed-quadrature) for the integrated derivative yields the displayed [linear multistep method](#linear-multistep-method). Its first [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is $\rho(z)=z^s-1$, whose unit-circle roots are all simple, proving [zero-stability](#zero-stability). Quadrature exactness gives order $s+1$ for odd $s$ and at least $s+2$ for even $s$. The [first Dahlquist barrier](#first-dahlquist-barrier) gives equality, while the [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem) gives convergence with consistent starts. These are finite-time convergence statements, not claims of [A-stability](#a-stability).

#### Cayley coefficient proof of the first Dahlquist barrier

↑ **Parent:** [First Dahlquist barrier](#first-dahlquist-barrier)

For a real consistent [zero-stable](#zero-stability) [linear multistep method](#linear-multistep-method), transform its first [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) by $z=(1+x)/(1-x)$ to $(1-x)^s\rho(z)=xP(x)$. The [root condition for a multistep method](#root-condition-for-a-multistep-method) puts all finite roots of $P$ in the closed left half-plane; real linear factors and conjugate quadratic factors consequently give nonnegative coefficients, after choosing $P(0)>0$. The order criterion requires a [polynomial](polynomial.md) of degree at most $s$ to agree through degree $p-1$ with $P(x)x/(2\operatorname{arctanh}x)$. The latter quotient has strictly negative nonconstant even coefficients. Its first even coefficient beyond degree $s$ includes a strictly negative multiple of $P(0)$ and cannot vanish. This gives the stated bound.

##### Coefficient sign lemma for the first Dahlquist barrier

↑ **Parent:** [Cayley coefficient proof of the first Dahlquist barrier](#cayley-coefficient-proof-of-the-first-dahlquist-barrier)

Write $F(x)=\int_0^1(1+x)^t(1-x)^{1-t}\,dt=x/\operatorname{arctanh}x$. Pairing $t$ and $1-t$ after differentiating twice gives

$$
F''(x)=-4\int_0^1t(1-t)(1-x^2)^{-3/2}\cosh[(2t-1)\operatorname{arctanh}x]\,dt.
$$

The [power series](real-analysis.md#power-series) of $(1-x^2)^{-3/2}$ has strictly positive even coefficients, and the other factor has nonnegative even coefficients. Thus every even coefficient of $F''$ is negative. Since $F$ is even with $F(0)=1$, the displayed sign pattern follows. This supplies a short positivity argument for the [first Dahlquist barrier](#first-dahlquist-barrier).

### Two-step family with a third-order member

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

The [exponential-symbol order criterion for a multistep method](#exponential-symbol-order-criterion-for-a-multistep-method) gives leading defect $-(1+5a)z^3/12$, so the family has order two except at $a=-1/5$, where it has order three. The [root condition for a multistep method](#root-condition-for-a-multistep-method) holds exactly for $-1\leq a<1$, and the convergent [A-stable](#a-stability) members are exactly $0\leq a<1$. At $a=0$ it reduces to the [trapezoidal rule](#trapezoidal-rule) after removal of a zero root. At $a=1$ a repeated root one destroys [convergence of a numerical method](#convergence-of-a-numerical-method) of the original recurrence despite a common [polynomial](polynomial.md) factor and a formally vanishing second-order residual.

### Adams-Bashforth method

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

An explicit [linear multistep method](#linear-multistep-method) that integrates a polynomial extrapolation of the past derivative values. The displayed two-step member is second order in time: the linear interpolant through $f_{n-1},f_n$, integrated over the next step, gives coefficients $3/2,-1/2$. For a spatially discretized partial differential equation, the spatial error must also be included in the total local defect.

#### Adams-Bashforth stability for centered diffusion

↑ **Parent:** [Adams-Bashforth method](#adams-bashforth-method)

For centered-space diffusion, a [Fourier mode](fourier-analysis.md#fourier-mode) gives $z^2-(1-3a/2)z-a/2=0$, with $a=4\mu\sin^2(\theta/2)$. For $a>0$ the roots have opposite signs, the positive root lies in $(0,1)$, and the negative root lies in $[-1,0)$ exactly when $P(-1)=2-2a\geq0$. At $a=0,1$ the unit-modulus roots are simple. Hence the [root condition for a multistep method](#root-condition-for-a-multistep-method) holds for every Fourier frequency exactly when $\mu\leq1/4$. Under fixed $\mu$, the unscaled one-step defect is $-\Delta t^2u_{xxxx}/(12\mu)+O(\Delta t^3)$; dividing by the step changes its order to $O(\Delta t)$.

### Common-factor cancellation defect in a multistep recurrence

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

Canceling a common factor of the characteristic polynomials changes the allowed starting relations and can remove a parasitic mode rather than prove stability of the original recurrence. For example $\rho=(\zeta-1)^2$ and $\sigma=(\zeta^2-1)/2$ fail [zero-stability](#zero-stability). On $y'=0$, the original recurrence admits $y_n=y_0+n(y_1-y_0)$; starting perturbations $y_1-y_0=\sqrt h$ vanish but give divergent error at fixed positive time. The canceled one-step recurrence excludes these data, so its stability cannot be assigned to the original scheme.

### Trapezoidal-BDF two-step family

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

This real-parameter [linear multistep method](#linear-multistep-method) has formal order two except at the degenerate value $\alpha=2$, where its local symbol vanishes to fourth degree. The zero-stability roots are $1$ and $\alpha-1$, so it is convergent exactly for $0\leq\alpha<2$. Every convergent member is [A-stable](#a-stability): the [boundary-locus test for multistep A-stability](#boundary-locus-test-for-multistep-a-stability) gives nonnegative real part $\alpha(2-\alpha)(1-\cos\theta)^2/(2|\sigma(e^{i\theta})|^2)$, with no unit-circle denominator zero for $0<\alpha<2$. At $\alpha=0$ the two interlaced sequences obey a trapezoidal step of length $2h$. At $\alpha=4/3$ it is the [BDF2 method](#second-order-backward-differentiation-formula). The endpoint two fails the [root condition for a multistep method](#root-condition-for-a-multistep-method) even though canceling a common polynomial factor resembles the [trapezoidal rule](#trapezoidal-rule).

### Multiderivative multistep method

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

A multiderivative multistep method uses higher time derivatives as well as values and first derivatives from several time levels. For an autonomous [ordinary differential equation](differential-equation.md#ordinary-differential-equation) $y'=f(y)$, the second time derivative is $y''=f'(y)f(y)$ by the [chain rule](calculus.md#chain-rule). Its [local truncation error](#local-truncation-error) must include the higher-derivative terms. Consequently the usual second-order barrier for [A-stable](#a-stability) [linear multistep methods](#linear-multistep-method), which only use first derivatives, does not apply.

#### Symmetric sixth-order two-derivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For $y'=f(y)$ and $g=f'f$, inserting a smooth exact solution into the displayed recurrence gives defect $h^7y^{(7)}(t_n)/4725+O(h^9)$. This follows by expanding $2\sinh z-(14/15)z\cosh z-(16/15)z+(2/15)z^2\sinh z$. The terms through $z^6$ vanish and the $z^7$ coefficient is nonzero. Its zero-step polynomial is $\zeta^2-1$, whose roots are simple and of unit modulus. Thus it is [zero-stable](#zero-stability) and has order six, provided starting values and derivative evaluations have corresponding accuracy.

#### Symmetric two-step two-derivative formula

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For the [multiderivative multistep method](#multiderivative-multistep-method) $y_{n+1}-\alpha h f_{n+1}+\beta h^2g_{n+1}=\gamma h f_n+y_{n-1}+\alpha h f_{n-1}+\beta h^2g_{n-1}$, with $g=f'f$, centered expansion gives defect coefficients $2-2\alpha-\gamma$, $1/3-\alpha+2\beta$, and $1/60-\alpha/12+\beta/3$ at powers $h,h^3,h^5$. Their simultaneous vanishing gives the displayed parameters. The next coefficient is $1/4725$ at $h^7$, so the formal order is six. Reflection symmetry removes every even defect power. The method satisfies fifth-order conditions but cannot have exact order five.

##### Bounded-root stability set of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

For the [symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula), the closed-disk [root condition for a multistep method](#root-condition-for-a-multistep-method) fails off the imaginary axis. Positive real part makes the product of root moduli exceed one; negative real part fails the [complex quadratic Schur criterion](#complex-quadratic-schur-criterion), as in the [empty strict decay domain of the symmetric two-derivative formula](#empty-strict-decay-domain-of-the-symmetric-two-derivative-formula) proof. On $z=iy$, write $D=15-y^2-7iy=|D|e^{i\delta}$ and set $\xi=i e^{-i\delta}\eta$. The [amplification polynomial](#amplification-polynomial-of-a-multistep-method) becomes $\eta^2-16y\eta/|D|+1=0$. Its two roots are distinct and on the [unit circle](complex-analysis.md#complex-unit-circle) exactly when $|16y/|D||<2$, or $y^4-45y^2+225>0$. Thus the bounded-root set consists of the imaginary intervals $|y|<\sqrt{(45-15\sqrt5)/2}$ and $|y|>\sqrt{(45+15\sqrt5)/2}$, including $y=0$ and excluding the double-root endpoints. In particular, the set is unbounded. Unit-modulus oscillations are bounded but do not tend to zero.

##### Empty strict decay domain of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

On the [Dahlquist test equation](#dahlquist-test-equation), write the [amplification polynomial](#amplification-polynomial-of-a-multistep-method) as $D\xi^2-16z\xi-A$, where $D=z^2-7z+15$ and $A=z^2+7z+15$. The identity $|A|^2-|D|^2=28\operatorname{Re}z(|z|^2+15)$ shows that both [roots of a polynomial](polynomial.md#root-of-a-polynomial) can lie inside the open [unit disk](geometry-and-topology.md#unit-disk) only if $\operatorname{Re}z<0$. But the [complex quadratic Schur criterion](#complex-quadratic-schur-criterion) would then require $32|\operatorname{Re}z|(|z|^2+15)<28|\operatorname{Re}z|(|z|^2+15)$, which is impossible. Thus the [strict linear stability domain](#strict-linear-stability-domain) is empty. This concerns robust damping of all modes, rather than convergence on fixed time intervals or the [bounded-root stability set of the symmetric two-derivative formula](#bounded-root-stability-set-of-the-symmetric-two-derivative-formula).

##### Negative-real instability of the symmetric two-derivative formula

↑ **Parent:** [Symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula)

On the [Dahlquist test equation](#dahlquist-test-equation), the [symmetric two-step two-derivative formula](#symmetric-two-step-two-derivative-formula) has amplification polynomial $F_z(w)=(z^2-7z+15)w^2-16zw-(z^2+7z+15)$. For every real $z<0$, its leading coefficient is positive and $F_z(-1)=2z<0$, whereas $F_z(w)\to+\infty$ as $w\to-\infty$. The [intermediate value theorem](calculus.md#intermediate-value-theorem) therefore gives a real root below minus one. Thus the method is not [A-stable](#a-stability), without any appeal to a multistep order barrier.

#### A-stable third-order two-step multiderivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

The endpoint expansion of this [multiderivative multistep method](#multiderivative-multistep-method) has unscaled defect $h^4y^{(4)}/3+O(h^5)$ and [zero-stability](#zero-stability) roots $1,1/7$, giving third-order convergence with suitably accurate starting values. On the [Dahlquist test equation](#dahlquist-test-equation) its amplification roots obey $(7-6z+2z^2)\zeta^2-8\zeta+1=0$. The [complex quadratic Schur criterion](#complex-quadratic-schur-criterion) puts both roots in the open unit disk for $\operatorname{Re}z<0$, and only the simple root one reaches the boundary at $z=0$. Thus it is [A-stable](#a-stability); its higher derivative places it outside the hypotheses of the [Second Dahlquist barrier](#second-dahlquist-barrier).

#### Convergence of a zero-stable multiderivative method

↑ **Parent:** [Multiderivative multistep method](#multiderivative-multistep-method)

For a fixed-step [multiderivative multistep method](#multiderivative-multistep-method), the ordinary [zero-stability](#zero-stability) root condition still controls propagation of the starting errors when all derivative evaluation maps are uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity) on the relevant bounded region. A local defect $O(h^{p+1})$ then yields global error $O(h^p)$ over a fixed time interval, provided the starting errors are $O(h^p)$ and the implicit updates use the nearby solution branch.

For example, writing the numerical error equation as $\rho(E)e_n=hF_h(e_{n+s})+d_n$, with $F_h$ uniformly [Lipschitz continuous](real-analysis.md#lipschitz-continuity), a bounded impulse response for the [root condition for a multistep method](#root-condition-for-a-multistep-method) gives

$$
\max_{j\leq n}\|e_j\|
\leq C\left(\max_{j<s}\|e_j\|+\sum_{j<n}\|d_j\|\right)
+Ch\sum_{j\leq n}\max_{i\leq j}\|e_i\|.
$$

Absorbing the last current-step term for small $h$ and applying the [discrete Gronwall inequality](probability-and-statistics.md#discrete-gronwall-inequality) gives the stated order. The higher derivatives enter through $F_h$, whose bound stays uniform as $h\to0$.

### Zero-stability

↑ **Parent:** [Linear multistep method](#linear-multistep-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero-stability)

Zero-stability requires the roots of the first characteristic polynomial to lie in the closed unit disc, with unit-modulus roots simple.

#### Root condition for a multistep method

↑ **Parent:** [Zero-stability](#zero-stability)

The root condition is the polynomial criterion equivalent to zero-stability for a linear multistep method.

##### Parasitic amplification root

↑ **Parent:** [Root condition for a multistep method](#root-condition-for-a-multistep-method)

An amplification root of a [multistep method](#linear-multistep-method) is parasitic when it represents an additional numerical mode rather than the principal mode approximating the exact differential-equation flow. For a consistent method the principal root starts at one as the step tends to zero, while other roots can start elsewhere. A simple parasitic root on the unit circle is compatible with [zero-stability](#zero-stability), but its motion outside the circle for a negative test parameter can destroy [absolute stability](#linear-stability-domain). Fixed-time convergence and all-time damping must be distinguished.

###### Centered two-step discretization of exponential decay

↑ **Parent:** [Parasitic amplification root](#parasitic-amplification-root)

Replacing the derivative in $x'=-Kx$ by a [central finite difference](finite-difference.md#central-finite-difference) gives $x_{n+1}+2Khx_n-x_{n-1}=0$. Its principal root is $\rho_+=e^{-\operatorname{arsinh}(Kh)}$, while the [parasitic amplification root](#parasitic-amplification-root) is $\rho_-=-e^{\operatorname{arsinh}(Kh)}$. On a fixed time interval, $A_h\rho_+^n+B_h\rho_-^n$ converges uniformly to $Ce^{-Kt}$ exactly when $A_h\to C$ and $B_h\to0$. A fixed nonzero parasitic amplitude alternates between two incompatible limits, but a vanishing starting error can converge despite the root's modulus exceeding one. This distinguishes fixed-time [numerical convergence](#convergence-of-a-numerical-method) from long-time [absolute stability](#linear-stability-domain).

##### Root stability of a cubic multistep polynomial

↑ **Parent:** [Root condition for a multistep method](#root-condition-for-a-multistep-method)

The polynomial $\rho(w)=(w-1)(w^2+w+a)$ satisfies the [root condition for a multistep method](#root-condition-for-a-multistep-method) exactly for $0\leq a\leq1$. For $a<0$ a root is below $-1$; for $a>1$ the quadratic root product forces a root outside the unit disc. The endpoints have simple unit-modulus roots, and the repeated root at $a=1/4$ is strictly inside. A consistent method with this polynomial is convergent throughout the closed interval.

### Dahlquist equivalence theorem

↑ **Parent:** [Linear multistep method](#linear-multistep-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dahlquist_equivalence_theorem)

A consistent linear multistep method is convergent exactly when it is zero-stable.

#### Necessity of the root condition for multistep convergence

↑ **Parent:** [Dahlquist equivalence theorem](#dahlquist-equivalence-theorem)

For a [linear multistep method](#linear-multistep-method), convergence for every set of consistent starting values requires the [root condition for a multistep method](#root-condition-for-a-multistep-method). Apply the recurrence to $y'=0$ over $N$ steps. A root $\xi$ with $|\xi|>1$ gives the error mode $e_n=|\xi|^{-N}\xi^n$: its fixed-index starting errors vanish as $N\to\infty$, but $|e_N|=1$. A unit-modulus root of multiplicity $m\geq2$ instead gives $e_n=N^{-(m-1)}n^{m-1}\xi^n$, with the same failure. Repeated roots inside the unit disk are harmless because their polynomial growth is dominated by exponential decay.

### Characteristic polynomials of a linear multistep method

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

For $\sum_{j=0}^s\alpha_jy_{n+j}=h\sum_{j=0}^s\beta_jf_{n+j}$, the characteristic polynomials are $\rho(\zeta)=\sum_j\alpha_j\zeta^j$ and $\sigma(\zeta)=\sum_j\beta_j\zeta^j$. Applied to $y'=\lambda y$, the amplification roots solve $\rho(\zeta)-h\lambda\sigma(\zeta)=0$.

#### Amplification polynomial of a multistep method

↑ **Parent:** [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)

Applying a [linear multistep method](#linear-multistep-method) to the [Dahlquist test equation](#dahlquist-test-equation) with $z=h\lambda$ produces a constant-coefficient recurrence whose modes satisfy $P_z(w)=0$. [Absolute stability](#linear-stability-domain) requires the resulting [roots of a polynomial](polynomial.md#root-of-a-polynomial) to lie in the unit disk, with unit-modulus roots simple. Thus multistep stability depends on every recurrence mode, rather than a single one-step [stability function](#stability-function).

##### Amplification root

↑ **Parent:** [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)

An amplification root is a [root of a polynomial](polynomial.md#root-of-a-polynomial) governing a geometric mode $y_n=\xi^n$ of a numerical recurrence on the [Dahlquist test equation](#dahlquist-test-equation). Its [modulus](complex-analysis.md#modulus) measures damping or growth per step. A repeated root produces additional modes such as $n\xi^n$; therefore a [unit-circle root](polynomial.md#unit-circle-root) can be permitted by a bounded-root condition only when it is simple. The principal root approximates $e^z$ near zero, while additional roots can describe [parasitic amplification roots](#parasitic-amplification-root).

##### Exterior roots of the derivative polynomial bound multistep stability

↑ **Parent:** [Amplification polynomial of a multistep method](#amplification-polynomial-of-a-multistep-method)

If the derivative [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) $\sigma$ of a [linear multistep method](#linear-multistep-method) has a simple root outside the [unit disk](geometry-and-topology.md#unit-disk) and keeps its degree in the limit, then its [absolute stability](#linear-stability-domain) region is bounded. Otherwise a stable sequence with $|z|\to\infty$ would give amplification polynomials $\sigma-\rho/z$ tending coefficientwise to $\sigma$. A root near the exterior root would persist by continuity, contradicting the [root condition for a multistep method](#root-condition-for-a-multistep-method). This argument excludes stability at every sufficiently large complex $z$, not only along the negative real axis.

#### Order conditions for a linear multistep method

↑ **Parent:** [Characteristic polynomials of a linear multistep method](#characteristic-polynomials-of-a-linear-multistep-method)

A linear multistep method has order $p$ exactly when

$$
\sum_j\alpha_jj^q=q\sum_j\beta_jj^{q-1}
$$

for $0\leq q\leq p$, with the right side interpreted as zero for $q=0$, and the identity first fails at $q=p+1$.

##### Exponential-symbol order criterion for a multistep method

↑ **Parent:** [Order conditions for a linear multistep method](#order-conditions-for-a-linear-multistep-method)

The [Taylor expansion](calculus.md#taylor-expansion) of the exact-solution residual for a [linear multistep method](#linear-multistep-method) has the same coefficient sequence as

$$
\rho(e^z)-z\sigma(e^z).
$$

Vanishing through degree $p$ is therefore equivalent to order at least $p$. Exact order $p$ additionally requires a nonzero coefficient at degree $p+1$. This symbol conveniently collects all polynomial consistency and order conditions.

<h3 id="adams-moulton-method">Adams–Moulton method</h3>

↑ **Parent:** [Linear multistep method](#linear-multistep-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adams–Moulton_method)

An Adams–Moulton method is an implicit [linear multistep method](#linear-multistep-method) obtained by integrating an interpolation polynomial for the vector field that includes the new time level.

### Second Dahlquist barrier

↑ **Parent:** [Linear multistep method](#linear-multistep-method)

An irreducible A-stable linear multistep method has order at most two.

This is an order restriction for an [A-stable](#a-stability) [linear multistep method](#linear-multistep-method).

## Numerical linear algebra

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_linear_algebra)

Numerical linear algebra develops stable finite algorithms for matrix computations.

### Matrix preconditioning

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)

Matrix preconditioning transforms a system using an inexpensive auxiliary solve to improve its spectrum. For symmetric positive definite matrices, a positive definite $M$ produces $M^{-1/2}AM^{-1/2}$, preserving the symmetric structure needed by [Conjugate gradient method](#conjugate-gradient-method).

#### Matrix preconditioner

↑ **Parent:** [Matrix preconditioning](#matrix-preconditioning)

A matrix preconditioner is an auxiliary invertible matrix whose inverse is cheap to apply and whose use improves the spectrum of a linear system. In symmetric positive definite problems, a positive definite $M$ preserves that structure under the symmetric transformation $M^{-1/2}AM^{-1/2}$.

### Power iteration

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_iteration)

### Gaussian elimination

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_elimination)

Gaussian elimination applies elementary row operations to reduce a linear system to triangular form. Dense elimination uses $O(n^3)$ arithmetic operations.

#### Sparse Gaussian elimination

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

A sparse direct solver performs [Gaussian elimination](#gaussian-elimination) while storing and updating only the predicted nonzero entries. A symbolic phase predicts the factor pattern from an elimination ordering, and a numerical phase evaluates the factors. The ordering can greatly alter [fill-in](#fill-in) and arithmetic work. For symmetric positive-definite systems, [Cholesky decomposition](linear-algebra.md#cholesky-decomposition) avoids numerical pivoting; general systems require a balance between sparsity and stable pivot selection.

##### Leaf elimination of a tree-pattern positive-definite matrix

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

Associate an undirected graph with a symmetric matrix's off-diagonal nonzero pattern. Eliminating vertex $i$ updates the remaining matrix by $a_{jk}\mapsto a_{jk}-a_{ji}a_{ik}/a_{ii}$. Only pairs of neighbors of $i$ can acquire [fill-in](#fill-in). If the graph is a tree, remove leaves successively: each eliminated vertex has at most one remaining neighbor, so only a diagonal entry can change. Every [Schur complement](linear-algebra.md#schur-complement) of a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) is positive definite, so no zero pivot forces a different ordering. Leaf removal therefore constructs a [perfect elimination ordering](graph-theory.md#perfect-elimination-ordering) and a fill-free factorization.

##### Symbolic factorization

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

[Symbolic factorization](#symbolic-factorization) computes possible nonzero positions and update dependencies from a [sparse matrix](vector-space.md#sparse-matrix) pattern and ordering before calculating numerical factor values. The [elimination graph](#elimination-graph) predicts fill and the [elimination tree](#elimination-tree) organizes dependencies. Numerical pivoting or exceptional cancellation can make the computed factor pattern differ from this structural prediction.

##### Elimination tree

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

For a symmetric factorization in a fixed ordering, the [elimination tree](#elimination-tree) assigns the displayed parent to a column of the lower-triangular factor when that set is nonempty. A column with no later entry is a root. The tree records dependencies of descendant updates on later pivots, supports symbolic factor allocation, and exposes parallel subtrees. It describes the factorization ordering, not merely a spanning tree of the original [matrix graph](#matrix-graph).

##### Nested dissection

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

A [vertex separator](graph-theory.md#vertex-separator) divides the remaining unknowns into disconnected subdomains. Nested dissection recursively eliminates each subdomain before its separator, keeping interaction localized until late in the factorization. For a regular two-dimensional mesh with $N$ unknowns, separators have size $O(\sqrt N)$; the resulting direct factorization uses $O(N^{3/2})$ work and $O(N\log N)$ storage under the usual geometric separator assumptions.

##### Minimum degree algorithm

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

At each step choose a remaining vertex of minimum degree in the current [elimination graph](#elimination-graph). This heuristic reduces the size of the immediate [Schur complement](linear-algebra.md#schur-complement) update and often reduces [fill-in](#fill-in), but does not guarantee a globally optimal ordering. Its degrees must reflect earlier fill, rather than just the original [graph](graph.md).

##### Fill-in

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

[Fill-in](#fill-in) consists of factor entries that become nonzero despite being zero in the original [sparse matrix](vector-space.md#sparse-matrix). In symmetric elimination these are the added edges of the [elimination graph](#elimination-graph). Removing a high-degree vertex can create many fill entries, whereas a [perfect elimination ordering](graph-theory.md#perfect-elimination-ordering) creates none. Symbolic fill predicts possible nonzeros before floating-point arithmetic; special cancellation can reduce the numerical pattern.

##### Matrix graph

↑ **Parent:** [Sparse Gaussian elimination](#sparse-gaussian-elimination)

For a symmetric [sparse matrix](vector-space.md#sparse-matrix), its [matrix graph](#matrix-graph) has one vertex per unknown and an edge $i-j$ whenever the off-diagonal entry $a_{ij}$ is structurally nonzero. Simultaneous row and column permutation relabels this [graph](graph.md). Nonsymmetric patterns are instead represented by directed or bipartite [graphs](graph.md) when row and column roles must be distinguished.

###### Elimination graph

↑ **Parent:** [Matrix graph](#matrix-graph)

One step of symmetric [Gaussian elimination](#gaussian-elimination) removes the pivot vertex and connects its remaining neighbors into a [clique](graph-theory.md#clique-graph-theory). The rule follows from the [Schur complement](linear-algebra.md#schur-complement) update $a_{ij}\leftarrow a_{ij}-a_{ik}a_{kj}/a_{kk}$. Repeating it predicts the generic factor sparsity; exceptional numerical cancellations can remove structurally predicted entries.

###### Fill-path criterion for symmetric elimination

↑ **Parent:** [Elimination graph](#elimination-graph)

After eliminating a vertex set $E$, a generic edge between remaining vertices $i,j$ exists exactly when the original [matrix graph](#matrix-graph) contains a path from $i$ to $j$ whose internal vertices all belong to $E$. Inductively, the new edges at pivot $k$ concatenate two such paths through $k$; conversely split any allowed path at $k$, or retain it when it avoids $k$. This characterizes fill by [graph](graph.md) reachability.

#### Columnwise partial pivoting

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

At each step of [Gaussian elimination](#gaussian-elimination), select the largest absolute entry in the uneliminated part of the current column and interchange rows to put it on the diagonal. A nonsingular trailing [Schur complement](linear-algebra.md#schur-complement) has a nonzero entry in its first column, so this procedure always finds a nonzero pivot in exact arithmetic. The [permutation matrix](vector-space.md#permutation-matrix) $P$ records row interchanges; earlier multipliers must be interchanged too when assembling the lower-triangular factor. This yields the [LU decomposition](#lu-decomposition) $PA=LU$ with unit diagonal in $L$. Searching within columns and interchanging rows is distinct from interchanging columns.

#### Row echelon form

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

A [matrix](vector-space.md#matrix) is in row echelon form if zero rows follow all nonzero rows, each nonzero row has a first nonzero entry (pivot) to the right of the pivot in the preceding row, and entries below each pivot vanish. [Elementary row operations](#elementary-row-operation) bring every [matrix](vector-space.md#matrix) to this form: choose a nonzero entry in the earliest nonzero column, swap its row to the top, eliminate entries below it, and continue on the remaining submatrix. The nonzero rows are independent by their successively positioned pivots; the pivot columns are independent and span the [column space](vector-space.md#column-space). Thus the number of pivots equals both [row rank](vector-space.md#row-rank) and [column rank](vector-space.md#column-rank).

#### Elementary row operation

↑ **Parent:** [Gaussian elimination](#gaussian-elimination)

An [elementary row operation](#elementary-row-operation) interchanges two rows of a [matrix](vector-space.md#matrix), multiplies one row by a nonzero scalar, or adds a scalar multiple of another row to it. These invertible operations are used in [Gaussian elimination](#gaussian-elimination). For a square [matrix](vector-space.md#matrix), interchange changes the sign of its [determinant](linear-algebra.md#determinant), multiplication scales its [determinant](linear-algebra.md#determinant) by the same scalar, and adding another row leaves its [determinant](linear-algebra.md#determinant) unchanged, by multilinearity and alternation.

##### Elementary matrix

↑ **Parent:** [Elementary row operation](#elementary-row-operation)

An elementary matrix is obtained by applying one [elementary row operation](#elementary-row-operation) to the [identity matrix](vector-space.md#identity-matrix). Multiplying $A$ by it on the left performs the same row operation on $A$. Such a [matrix](vector-space.md#matrix) is invertible: reverse a row swap, reverse a nonzero row scaling by its reciprocal, or reverse adding a multiple of another row by adding its negative. Right multiplication gives an [elementary column operation](vector-space.md#elementary-column-operation). In particular these operations preserve [matrix rank](vector-space.md#matrix-rank).

### LU decomposition

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/LU_decomposition)

An LU decomposition factors a matrix as a lower-triangular matrix times an upper-triangular matrix. It records Gaussian elimination so that multiple right-hand sides can be solved by forward and backward substitution.

### LDL decomposition

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)

An LDL decomposition of a real symmetric matrix is

$$
A=LDL^T,
$$

where $L$ is unit lower triangular and $D$ is diagonal. Symmetric elimination computes it one [Schur complement](linear-algebra.md#schur-complement) at a time. The matrix is positive definite exactly when every diagonal pivot in $D$ is positive.

### Machine epsilon

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Machine_epsilon)

Machine precision is the characteristic relative rounding scale of a floating-point system.

### Eigenpair residual

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)

For an approximate eigenpair $(\widetilde\lambda,\widetilde v)$, the residual is

$$
r=A\widetilde v-\widetilde\lambda\widetilde v.
$$

#### Backward error of an approximate eigenpair

↑ **Parent:** [Eigenpair residual](#eigenpair-residual)

If $\|\widetilde v\|_2=1$, the smallest operator-norm perturbation that makes $(\widetilde\lambda,\widetilde v)$ an exact eigenpair has norm $\|r\|_2$. One such rank-one perturbation is

$$
E=-r\widetilde v^T.
$$

### Householder QR decomposition

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_QR_decomposition)

Successive Householder reflections zero subdiagonal column entries and factor a matrix into an orthogonal factor and an upper-triangular factor.

#### Householder reduction of an overdetermined consistent system

↑ **Parent:** [Householder QR decomposition](#householder-qr-decomposition)

For full column rank $A\in\mathbb R^{m\times n}$, a full [QR factorization](linear-algebra.md#qr-decomposition) gives $Q^TA=(R_1,0)^T$ with invertible upper triangular $R_1$. The equation $Ax=b$ is consistent exactly when the final $m-n$ entries of $Q^Tb$ vanish. If consistent, [back substitution](linear-algebra.md#back-substitution) gives its unique solution. This separates consistency from uniqueness in overdetermined systems.

### Householder tridiagonalization

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_tridiagonalization)

Orthogonal Householder similarities reduce a real symmetric matrix to symmetric tridiagonal form.

#### Skew-symmetric Householder tridiagonalization

↑ **Parent:** [Householder tridiagonalization](#householder-tridiagonalization)

An [orthogonal](linear-algebra.md#orthogonal-vectors) similarity preserves skew symmetry, so upper-Hessenberg reduction of a real [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix) is automatically tridiagonal with zero diagonal. For a [Householder reflection](linear-algebra.md#householder-transformation), the scalar $v^TAv$ vanishes, eliminating the fourth term of the general similarity update. Storing only one triangle and using the displayed skew rank-two update costs $2n^3/3+O(n^2)$ scalar products, the same leading product count as optimized symmetric tridiagonalization; the simplification saves lower-order work.

### Unshifted QR algorithm

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)

The unshifted QR algorithm factors $A_k=Q_kR_k$ and forms $A_{k+1}=R_kQ_k=Q_k^TA_kQ_k$, preserving eigenvalues while driving the matrix toward block diagonal form.

This is the zero-shift case of the [QR algorithm](#qr-algorithm).

#### Accumulated QR factorization identity

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

Let

$$
\overline Q_k=Q_0Q_1\cdots Q_k,
\qquad
\overline R_k=R_kR_{k-1}\cdots R_0.
$$

Then

$$
A_{k+1}=\overline Q_k^TA\overline Q_k,
\qquad
A^{k+1}=\overline Q_k\overline R_k.
$$

Thus $\overline Q_k\overline R_k$ is a [QR decomposition](linear-algebra.md#qr-decomposition) of the matrix power $A^{k+1}$. In particular, the first $r$ columns of $\overline Q_k$ span the same subspace as the first $r$ columns of $A^{k+1}$ whenever those columns are independent.

#### Symmetric bandwidth preservation under QR iteration

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

An unshifted QR step preserves the bandwidth of a real symmetric banded matrix. A Givens-rotation implementation exposes this as bulges created during triangularization and removed when the factors are multiplied in reverse order.

#### Simultaneous iteration interpretation of the QR algorithm

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

The accumulated orthogonal factor in QR iteration is the $Q$ factor of a matrix power, so its leading columns span the same spaces as simultaneous power iteration.

##### Two-column dominant-subspace condition

↑ **Parent:** [Simultaneous iteration interpretation of the QR algorithm](#simultaneous-iteration-interpretation-of-the-qr-algorithm)

Let a real [symmetric matrix](linear-algebra.md#symmetric-matrix) have an [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis) $w_1,\ldots,w_n$, with

$$
|\lambda_1|\leq\cdots\leq|\lambda_{n-2}|<
|\lambda_{n-1}|=|\lambda_n|.
$$

Write two starting vectors as

$$
u=\sum_i b_iw_i,
\qquad
v=\sum_i c_iw_i.
$$

For two-column [subspace iteration](linear-operator-theory.md#subspace-iteration) to recover  
$\operatorname{span}(w_{n-1},w_n)$, the two projections onto that dominant subspace must be independent. The exact condition is

$$
\det\begin{pmatrix}
b_{n-1}&c_{n-1}\\
b_n&c_n
\end{pmatrix}
=b_{n-1}c_n-b_nc_{n-1}\ne0.
$$

Requiring each of the four coefficients to be nonzero does not imply this determinant condition.

#### Block deflation in the QR algorithm

↑ **Parent:** [Unshifted QR algorithm](#unshifted-qr-algorithm)

When an off-block subdiagonal entry tends to zero, QR iteration asymptotically separates the corresponding invariant spectral blocks even if eigenvalues within one block have equal modulus.

### Stationary iterative method for a linear system

↑ **Parent:** [Numerical linear algebra](#numerical-linear-algebra)

A stationary iteration has the form

$$
x^{(k+1)}=Hx^{(k)}+v,
$$

with a fixed iteration matrix $H$. It converges for every initial vector exactly when the [spectral radius](analysis.md#spectral-radius) satisfies $\rho(H)<1$.

This is an [iterative method](#iterative-method) whose update matrix remains fixed.

#### Semiconvergence of cyclic Poisson iterations

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

The periodic second-difference [circulant matrix](linear-algebra.md#circulant-matrix) has constant [null space](linear-algebra.md#kernel-of-a-linear-map), so solvability requires $\sum b_j=0$. Its [Jacobi method](#jacobi-method) has eigenvalues $\cos(2\pi j/n)$: for odd $n$ it converges to some solution, while for even $n$ an alternating mode oscillates unless absent from the error. Lexicographic [Gauss-Seidel iteration](#gauss-seidel-method) converges to some solution for every compatible right-hand side and every initial vector. For $K=-A=D+L+U$, a coordinate sweep decreases the energy $e^TKe/2$ by the sum of squared coordinate changes. This excludes all nonconstant unit-modulus eigenmodes. The constant unit eigenvalue is simple, since the invariant left vector $w=(0,1,\ldots,1,2)^T$ has $w^T\mathbf1=n\ne0$. Neither method is a strict contraction to a unique solution without fixing the constant nullspace.

#### Richardson iteration

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

For a real symmetric positive definite [matrix](vector-space.md#matrix) $A$, the error in each [eigenvector](linear-operator-theory.md#eigenvector) direction is multiplied by $1-\tau\lambda$. Convergence from every initial vector is therefore equivalent to $0<\tau<2/\lambda_{\max}$. At either endpoint there is a nondecaying error direction. The optimal constant parameter is $2/(\lambda_{\min}+\lambda_{\max})$, giving contraction factor $(\lambda_{\max}-\lambda_{\min})/(\lambda_{\max}+\lambda_{\min})$.

#### Gauss-Seidel method

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Seidel_method)

With $A=D+L+U$, the [Gauss-Seidel method](#gauss-seidel-method) solves $(D+L)x^{(k+1)}=b-Ux^{(k)}$. It uses each newly computed coordinate immediately in the remaining triangular solve. It is [successive over-relaxation](#successive-over-relaxation) with parameter one, and converges from every start when $A$ is symmetric positive definite.

#### Successive over-relaxation

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successive_over-relaxation)

For a splitting $A=D+L+U$, [successive over-relaxation](#successive-over-relaxation) updates

$$
(D+\omega L)x^{(k+1)}=[(1-\omega)D-\omega U]x^{(k)}+\omega b.
$$

It reduces to the [Gauss-Seidel method](#gauss-seidel-method) at $\omega=1$. If $A$ is symmetric positive definite, the [Householder-John theorem](#householder-john-theorem) applies to $M=D/\omega+L$, $N=(1/\omega-1)D-U$, since $M^T+N=(2/\omega-1)D$ is positive definite for $0<\omega<2$.

#### Iteration matrix

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)

For a stationary iteration $x^{(k+1)}=Hx^{(k)}+v$, the matrix $H$ propagates the error by $e^{(k+1)}=He^{(k)}$. Convergence from every initial error is equivalent to $\rho(H)<1$.

#### Matrix splitting

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_splitting)

A splitting $A=M-N$ with invertible $M$ produces

$$
x^{(k+1)}=M^{-1}Nx^{(k)}+M^{-1}b.
$$

##### Householder-John theorem

↑ **Parent:** [Matrix splitting](#matrix-splitting)

Let $A=M-N$ be Hermitian positive definite. If $M^*+N$ is also Hermitian positive definite, then $M$ is invertible and

$$
\rho(M^{-1}N)<1.
$$

Thus the stationary iteration associated with the splitting converges from every initial vector.

#### Jacobi method

↑ **Parent:** [Stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_method)

Writing $A=D+L+U$, where $D$ is diagonal and $L,U$ are strictly triangular, the Jacobi iteration is

$$
x^{(k+1)}=D^{-1}\left(b-(L+U)x^{(k)}\right).
$$

##### Skew-tridiagonal Jacobi and Gauss-Seidel iterations

↑ **Parent:** [Jacobi method](#jacobi-method)

For $A=\mu^{-1}I+U-U^T$, with $U$ the four-dimensional unit superdiagonal, the [Jacobi method](#jacobi-method) has eigenvalues $2i\mu\cos(j\pi/5)$, $j=1,\ldots,4$. The [Gauss-Seidel method](#gauss-seidel-method) has two zero eigenvalues and $-\mu^2(3\pm\sqrt5)/2$. Therefore both methods converge for every starting vector exactly when $0<|\mu|<(\sqrt5-1)/2$. This equality of convergence ranges follows from their spectra, not from positive-definiteness of the nonsymmetric coefficient matrix.

##### Weighted Jacobi method

↑ **Parent:** [Jacobi method](#jacobi-method)

With relaxation parameter $\omega$, weighted Jacobi updates by

$$
x^{(\nu+1)}
=x^{(\nu)}+\omega D^{-1}(b-Ax^{(\nu)}).
$$

Its [iteration matrix](#iteration-matrix) is $H_\omega=I-\omega D^{-1}A$.

###### Weighted Jacobi eigenvalues for a square Dirichlet grid

↑ **Parent:** [Weighted Jacobi method](#weighted-jacobi-method)

For the five-point discretization of $-\Delta+c$ on the unit square, the weighted iteration [eigenvalues](linear-operator-theory.md#eigenvalue) are $1-\omega[4\sin^2(\pi kh/2)+4\sin^2(\pi lh/2)+ch^2]/(4+ch^2)$. A fixed parameter converges for every mesh when $0<\omega\leq1$, but $\omega=1$ poorly damps the highest frequencies.

###### Weighted Jacobi method for the one-dimensional Poisson equation

↑ **Parent:** [Weighted Jacobi method](#weighted-jacobi-method)

For the centered second-difference matrix with diagonal $-2$ and off-diagonals $1$, the weighted-Jacobi eigenvalues are

$$
\lambda_k(\omega)
=1-\omega+\omega\cos\frac{k\pi}{n+1},
\qquad 1\leq k\leq n.
$$

The method converges for every grid size exactly when $0<\omega\leq1$.

###### High-frequency smoothing factor of weighted Jacobi

↑ **Parent:** [Weighted Jacobi method for the one-dimensional Poisson equation](#weighted-jacobi-method-for-the-one-dimensional-poisson-equation)

For modes with $k/(n+1)\in[1/2,1]$ and large $n$, the worst attenuation factor is

$$
\mu_\omega=\max\{|1-\omega|,|1-2\omega|\}.
$$

It is minimized by $\omega=2/3$, for which $\mu_\omega=1/3$.

###### Exact finite-grid high-frequency Jacobi smoothing optimum

↑ **Parent:** [High-frequency smoothing factor of weighted Jacobi](#high-frequency-smoothing-factor-of-weighted-jacobi)

For the one-dimensional Dirichlet second-difference grid, high sine modes have eigenvalues $1-\omega t_k$, with $t_k=1-\cos(k\pi/(n+1))$ and $k\geq\lceil(n+1)/2\rceil$. Let $a$ and $b$ be the smallest and largest of these $t_k$. Convexity gives attenuation $\max(|1-\omega a|,|1-\omega b|)$. Balancing its endpoint values with opposite signs gives the displayed exact minimax choice. For odd $n$, $a=1$; for even $n$, $a=1+\sin(\pi/[2(n+1)])$, and always $b=1+\cos(\pi/(n+1))$. Only in the large-grid or uniform-in-grid limit do these become $\omega_*=2/3$, $\mu_*=1/3$.

##### Jacobi convergence for a three-by-three equicorrelation matrix

↑ **Parent:** [Jacobi method](#jacobi-method)

For a three-by-three matrix with diagonal entries one and every off-diagonal entry $\alpha$, the [Jacobi method](#jacobi-method) iteration matrix has eigenvalue $-2\alpha$ on the all-ones vector and eigenvalue $\alpha$ with multiplicity two on its orthogonal complement. Its [spectral radius](analysis.md#spectral-radius) is $2|\alpha|$, so Jacobi iteration converges exactly when $|\alpha|<1/2$.

##### Jacobi convergence for a symmetric positive-definite tridiagonal matrix

↑ **Parent:** [Jacobi method](#jacobi-method)

If $A=D+L+L^T$ is symmetric positive definite and tridiagonal, set $S=\operatorname{diag}(1,-1,1,-1,\ldots)$. Then

$$
SAS=D-L-L^T
$$

is positive definite. Applying the [Householder-John theorem](#householder-john-theorem) to $M=D$ and $N=-(L+L^T)$ proves that the Jacobi iteration converges.

## Linear stability domain

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_stability_domain)

For a one-step method applied to $y'=\lambda y$, write $y_{n+1}=R(h\lambda)y_n$. Its linear stability domain is

$$
\mathcal S=\{z\in\mathbb C:|R(z)|\leq1\}.
$$

Forward Euler has $R(z)=1+z$, while backward Euler has $R(z)=(1-z)^{-1}$ and is A-stable.

### Strict linear stability domain

↑ **Parent:** [Linear stability domain](#linear-stability-domain)

The strict decay convention for a [linear stability domain](#linear-stability-domain) demands that every numerical mode tends to zero on the [Dahlquist test equation](#dahlquist-test-equation). For a one-step [stability function](#stability-function) it requires $|R(z)|<1$; for a [multistep method](#linear-multistep-method) it requires every [amplification root](#amplification-root) to have [modulus](complex-analysis.md#modulus) below one. This differs from a boundedness convention that allows simple [unit-circle roots](polynomial.md#unit-circle-root), and from mesh-uniform finite-time [numerical stability](#stability-of-a-numerical-method). [Cambridge numerical analysis notes](https://www.damtp.cam.ac.uk/user/na/PartIB/Lect10.pdf) use the decay convention. Explicitly specifying the convention is essential for methods with undamped modes.

### A-alpha stability

↑ **Parent:** [Linear stability domain](#linear-stability-domain)

A numerical time-stepping method is $A(\alpha)$-stable if its [absolute stability](#linear-stability-domain) region contains the negative-axis sector $\{z:|\arg(-z)|\leq\alpha\}$, for $0<\alpha\leq\pi/2$. With a [stability function](#stability-function) $R$, this requires $|R(z)|\leq1$ throughout that sector. At $\alpha=\pi/2$, this is [A-stability](#a-stability).

### Euler method

↑ **Parent:** [Linear stability domain](#linear-stability-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_method)

Explicit Euler advances $y'=f(t,y)$ by $y_{n+1}=y_n+h f(t_n,y_n)$. Its [stability function](#stability-function) is $R(z)=1+z$.

### A-stability

↑ **Parent:** [Linear stability domain](#linear-stability-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/A-stability)

A method is A-stable when its stability domain contains the closed left half-plane.

<h4 id="a-stability-of-near-diagonal-exponential-pade-approximants">A-stability of near-diagonal exponential Padé approximants</h4>

↑ **Parent:** [A-stability](#a-stability)

For nonnegative degrees $m,n$ with $n-2\le m\le n$, the $[m/n]$ [Padé approximant](isolated-singularity.md#pade-approximant) $R$ to the [exponential function](calculus.md#exponential-function) has no poles in the left half-plane and satisfies $|R(z)|\le1$ for $\operatorname{Re}z\le0$. Consequently a numerical method having that [stability function](#stability-function) is [A-stable](#a-stability). In particular, the near-diagonal choice $[s-1/s]$ gives the [Radau IIA method](#radau-iia-method) stability function, while $[s/s]$ corresponds to the [Gauss collocation method](#gauss-legendre-method). The theorem concerns these exponential approximants, not arbitrary rational approximations with the same degrees.

#### Principal-root obstruction to A-stability

↑ **Parent:** [A-stability](#a-stability)

Suppose a consistent [linear multistep method](#linear-multistep-method) has a simple principal [polynomial root](polynomial.md#root-of-a-polynomial) and its analytic [logarithm](calculus.md#logarithm) satisfies $\log w(z)=z+Cz^{2r}+O(z^{2r+1})$ near zero, with real coefficients. If $C(-1)^r>0$, then at $z=i\varepsilon$ the real part of $\log w$ is positive to leading order. The same remains true after giving $z$ a small negative real part of smaller magnitude than that leading term. Thus a growing [amplification factor](finite-difference.md#amplification-factor) occurs inside the left half-plane, ruling out [A-stability](#a-stability). For an order-three method with $C>0$, choose $z=-C\varepsilon^4/2+i\varepsilon$.

#### Explicit multistep methods cannot be A-stable

↑ **Parent:** [A-stability](#a-stability)

For an explicit [linear multistep method](#linear-multistep-method), the highest-degree coefficient of $\rho(w)-z\sigma(w)$ is fixed while at least one lower coefficient grows unboundedly with negative real $z$. If all roots stayed in the [unit disk](geometry-and-topology.md#unit-disk), the [elementary symmetric polynomials](polynomial.md#elementary-symmetric-polynomial) of those roots would keep every monic coefficient bounded. This contradiction proves that no nontrivial consistent explicit method is [A-stable](#a-stability).

#### Boundary-locus test for multistep A-stability

↑ **Parent:** [A-stability](#a-stability)

A unit-modulus amplification root of a [linear multistep method](#linear-multistep-method) puts its test-equation parameter on this boundary locus, except when numerator and denominator both vanish. If the locus avoids the open left half-plane, the leading coefficient never vanishes there and the roots are initially inside the disk at one point there, continuity keeps them inside throughout that connected region. Checking [zero-stability](#zero-stability), imaginary-axis roots and common polynomial factors is still necessary. A boundary plot alone is not a proof of [A-stability](#a-stability).

#### L-stability

↑ **Parent:** [A-stability](#a-stability)

An A-stable one-step method is L-stable when its [stability function](#stability-function) also satisfies $R(z)\to0$ as $|z|\to\infty$ within the left half-plane. It damps modes whose decay time is far shorter than the numerical step.

#### B-stability

↑ **Parent:** [A-stability](#a-stability)

A Runge--Kutta method is B-stable when it does not increase distances between numerical solutions of a dissipative differential equation. [Algebraic stability of a Runge-Kutta method](#algebraic-stability-of-a-runge-kutta-method) is a standard sufficient condition.

#### Backward Euler method

↑ **Parent:** [A-stability](#a-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backward_Euler_method)

Backward Euler advances $y'=f(t,y)$ by $y_{n+1}=y_n+h f(t_{n+1},y_{n+1})$. Its stability function $R(z)=(1-z)^{-1}$ makes it [L-stable](#l-stability).

#### A-stability of a symmetric two-stage implicit Runge-Kutta family

↑ **Parent:** [A-stability](#a-stability)

For the two-stage [implicit Runge-Kutta method](#implicit-runge-kutta-method) with

$$
A=
\begin{pmatrix}
\frac14&\frac14-a\\
\frac14+a&\frac14
\end{pmatrix},
\qquad
b=\begin{pmatrix}\frac12\\\frac12\end{pmatrix},
$$

the [stability function](#stability-function) is

$$
R(z)=\frac{2+z+2a^2z^2}{2-z+2a^2z^2}.
$$

For $z=x+iy$,

$$
|2-z+2a^2z^2|^2-|2+z+2a^2z^2|^2
=-8x(1+a^2|z|^2).
$$

The denominator has no zero in the closed left half-plane, so the method is [A-stable](#a-stability) for every real $a$.

### Stiff equation

↑ **Parent:** [Linear stability domain](#linear-stability-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stiff_equation)

A stiff differential equation contains rapidly decaying modes alongside much slower dynamics. An explicit method may then require a small step for stability even when accuracy only requires resolving the slow modes.

#### Stiff two-mode linear system

↑ **Parent:** [Stiff equation](#stiff-equation)

If a linear system has negative eigenvalues with widely separated magnitudes, an explicit method can be forced to resolve the fastest decaying mode solely for stability. For eigenvalues $-1$ and $-100$, forward Euler requires $h\leq0.02$, whereas backward Euler is stable for every positive step size.

### Milne device for forward and backward Euler

↑ **Parent:** [Linear stability domain](#linear-stability-domain)

Starting at the same value, forward and backward Euler have opposite leading local errors. Their half-difference therefore estimates either local error:

$$
E_n=\frac12\lVert y_B-y_F\rVert.
$$

For a first-order method, a local-tolerance controller consequently scales the next step by $(\mathrm{tol}/E_n)^{1/2}$, usually with a safety factor.

## Orthogonal polynomial

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_polynomial)

Orthogonal polynomials of distinct degrees are orthogonal under a positive weighted inner product.

### Kravchuk polynomials

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kravchuk_polynomials)

These [polynomials](polynomial.md) are orthogonal for a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) weight and encode the coefficient transformation in the [MacWilliams identity](coding-theory.md#macwilliams-identity). Their [generating function](real-analysis.md#generating-function) follows by expanding the two factors:

$$
\sum_{s=0}^nK_s(t;n,q)z^s=(1-z)^t(1+(q-1)z)^{n-t}.
$$

For binary [linear codes](coding-theory.md#linear-code), $q=2$. Expanding the factors gives $K_s(t;n,2)=\sum_j(-1)^j\binom tj\binom{n-t}{s-j}$, where [binomial coefficients](combinatorics.md#binomial-coefficient) outside their usual integer range are zero. Orthogonality follows by multiplying [generating functions](real-analysis.md#generating-function) and summing over $t$ with weight $\binom nt(q-1)^t$: the result is $q^n(1+(q-1)zw)^n$, whose coefficient of $z^rw^s$ is zero for $r\ne s$ and $q^n(q-1)^r\binom nr$ for $r=s$.

### Orthogonality forces many interior zeros

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)

If a nonzero continuous real function on an interval is orthogonal to every [polynomial](polynomial.md) of degree below $n$, it has at least $n$ distinct interior zeros. If it had only finitely many zeros and fewer than $n$ sign changes, multiply it by the product of linear factors at its sign-changing zeros. The product has constant sign and is nonzero on an [open interval](topology.md#open-interval), so its integral cannot vanish. Orthogonality to this degree-below-$n$ [polynomial](polynomial.md) contradicts that conclusion. Infinitely many interior zeros already satisfy the assertion. Orthogonal [polynomials](polynomial.md) of respective degrees $0,\ldots,n-1$ form a [basis](vector-space.md#basis) of the needed [polynomial](polynomial.md) space.

### Zernike polynomials

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zernike_polynomials)

The real Zernike polynomials form an [orthogonal polynomial](#orthogonal-polynomial) basis on the unit [Euclidean disk](topology.md#disk-mathematics), with radial factor $R_n^m(\rho)$ and angular factor $\cos m\phi$ or $\sin m\phi$. Here $0\leq m\leq n$ and $n-m$ is [even](calculus.md#even-function). They decompose [wavefront errors](optics.md#wavefront-error) into modes useful for optical correction. Normalizations differ, so coefficients should specify the chosen convention.

#### Zernike spherical mode

↑ **Parent:** [Zernike polynomials](#zernike-polynomials)

The unnormalized rotationally symmetric mode is $Z_4^0(\rho)=6\rho^4-6\rho^2+1$. It describes balanced primary [spherical aberration](optics.md#spherical-aberration). The lower-degree terms make it orthogonal to constant piston and quadratic defocus under the disk area measure: direct integration gives $\int_0^1 Z_4^0\rho\,d\rho=0$ and $\int_0^1 Z_4^0(2\rho^2-1)\rho\,d\rho=0$.

### Monic orthogonal polynomial

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)

A monic orthogonal polynomial has leading coefficient one. For a fixed positive weight, there is a unique monic orthogonal polynomial of each degree.

#### Three-term recurrence for monic orthogonal polynomials

↑ **Parent:** [Monic orthogonal polynomial](#monic-orthogonal-polynomial)

For monic orthogonal polynomials,

$$
p_{n+1}(x)=(x-\alpha_n)p_n(x)-\beta_np_{n-1}(x),
$$

where

$$
\alpha_n=\frac{\langle xp_n,p_n\rangle}{\langle p_n,p_n\rangle},
\qquad
\beta_n=\frac{\langle p_n,p_n\rangle}{\langle p_{n-1},p_{n-1}\rangle}.
$$

### Hermite polynomial

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hermite_polynomial)

#### Hermite function

↑ **Parent:** [Hermite polynomial](#hermite-polynomial)

The normalized Hermite functions multiply the physicists' [Hermite polynomials](#hermite-polynomial) by a Gaussian. They form an [orthonormal basis](linear-algebra.md#orthonormal-basis) of $L^2(\mathbb R)$ and satisfy $(-d^2/dx^2+x^2)H_n=(2n+1)H_n$. With $a=(x+d/dx)/\sqrt2$ and $a^*=(x-d/dx)/\sqrt2$, they are $(a^*)^nH_0/\sqrt{n!}$ and the [quantum harmonic oscillator](quantum-mechanics.md#quantum-harmonic-oscillator) is $2a^*a+1$. For completeness, if $u$ is orthogonal to all of them, all moments of $u(x)e^{-x^2/2}$ vanish. Its transform $\int u(x)e^{-x^2/2}e^{zx}\,dx$ is entire by [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), has every derivative zero at zero, and hence vanishes identically. Uniqueness of the [Fourier transform](analysis.md#fourier-transform) gives $u=0$.

##### Hermite functions are Fourier eigenfunctions

↑ **Parent:** [Hermite function](#hermite-function)

Use the unitary [Fourier transform](analysis.md#fourier-transform) with phase $e^{-i\lambda x}$. It commutes with $-d^2/dx^2+x^2$, because differentiation transforms to multiplication by $i\lambda$ and multiplication by $x$ transforms to $i\,d/d\lambda$. The [Hermite differential equation](analysis.md#hermite-differential-equation) has a unique polynomial solution of each degree up to scale, and multiplying by the Gaussian gives a [Hermite function](#hermite-function). Transforming a polynomial times this Gaussian again gives a polynomial times the Gaussian of the same degree; comparison of leading coefficients gives the eigenvalue $(-i)^n$.

##### Mehler formula for Hermite functions

↑ **Parent:** [Hermite function](#hermite-function)

For $|t|<1$, this identity sums the [Hermite function](#hermite-function) expansion into a Gaussian. One proof takes the [Bargmann-Fock space](hilbert-space.md#bargmann-fock-space) inner product of the generating functions $\pi^{-1/4}\exp(-x^2/2+\sqrt2 xz-z^2/2)$ at $\sqrt t\,z$. Writing $z=u+iv$, the two resulting real [Gaussian integrals](calculus.md#gaussian-integral) have quadratic coefficients $1+t$ and $1-t$ and linear coefficients $\sqrt{2t}(x+y)$ and $i\sqrt{2t}(x-y)$. Evaluation gives the formula. Setting $t=e^{-2s}$ and multiplying by $e^{-s}$ gives the [harmonic oscillator transition kernel](quantum-mechanics.md#harmonic-oscillator-transition-kernel) of $e^{-s(-d^2/dx^2+x^2)}$.

#### Probabilists' Hermite polynomial

↑ **Parent:** [Hermite polynomial](#hermite-polynomial)

The probabilists' Hermite polynomials are

$$
\mathrm{He}_n(x)=(-1)^ne^{x^2/2}\frac{d^n}{dx^n}e^{-x^2/2}.
$$

They are orthogonal for the standard Gaussian weight and satisfy $\mathrm{He}_{n+1}=x\mathrm{He}_n-n\mathrm{He}_{n-1}$.

This is the Gaussian-probability normalization of the [Hermite polynomial](#hermite-polynomial) family.

##### Space-time Hermite polynomial

↑ **Parent:** [Probabilists' Hermite polynomial](#probabilists-hermite-polynomial)

The space-time [Probabilists' Hermite polynomial](#probabilists-hermite-polynomial) $H_n(x,t)=t^{n/2}\mathrm{He}_n(x/\sqrt t)$ extends polynomially to $t=0$ and solves $\partial_tH_n+\frac12\partial_x^2H_n=0$. Therefore $H_n(B_t,t)$ is a [martingale](martingale.md) for a standard [Brownian motion](brownian-motion.md), by the [Itô formula](stochastic-calculus.md#ito-s-lemma) and Gaussian [moments](probability-theory.md#moment).

### Zeros of orthogonal polynomials

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zeros_of_orthogonal_polynomials)

A degree-n orthogonal polynomial for a positive interval weight has n simple zeros in the interval interior.

### Jacobi matrix

↑ **Parent:** [Orthogonal polynomial](#orthogonal-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_matrix)

A Jacobi matrix is a symmetric tridiagonal matrix whose characteristic polynomials obey the orthogonal-polynomial three-term recurrence.

## Numerical integration

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_integration)

Numerical integration approximates definite integrals using finitely many arithmetic operations and function evaluations.

<h3 id="boole-s-rule">Boole's rule</h3>

↑ **Parent:** [Numerical integration](#numerical-integration)

Integrate the five [Lagrange interpolation polynomials](#lagrange-polynomial) at the equally spaced nodes to obtain the displayed rule. It is exact for [polynomials](polynomial.md) through degree four, and symmetry also makes it exact in degree five. Symmetric endpoint, inner-node and midpoint weights $a,b,c$ satisfy $2a+2b+c=2$, $2a+b/2=2/3$, $2a+b/8=2/5$, giving $a=7/45$, $b=32/45$, $c=12/45$.

### Quadrature rule

↑ **Parent:** [Numerical integration](#numerical-integration)

A quadrature rule approximates a weighted integral by a finite weighted sum of function values.

#### Newton-Cotes closed quadrature

↑ **Parent:** [Quadrature rule](#quadrature-rule)

Integrate the [Lagrange polynomial](#lagrange-polynomial) through values at all equally spaced nodes $0,\ldots,s$, including both endpoints. The resulting [quadrature rule](#quadrature-rule) is exact through degree $s$. For even $s$, the node [polynomial](polynomial.md) $\prod_{j=0}^s(t-j)$ is odd about $s/2$, so its integral vanishes and exactness extends through degree $s+1$. The weights need not remain positive as the number of nodes increases.

<h4 id="simpson-s-rule">Simpson's rule</h4>

↑ **Parent:** [Quadrature rule](#quadrature-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simpson's_rule)

[Simpson's rule](#simpson-s-rule) integrates the quadratic interpolant through two endpoints and their midpoint. It is exact also on cubic [polynomials](polynomial.md). On $[0,2]$, define the raw kernel $K(t)=L[(x-t)_+^3]$, where $L$ is integral minus the rule. Then $K(t)=-t^3(4-3t)/12$ for $0\leq t\leq1$ and $K(t)=-(2-t)^3(3t-2)/12$ for $1\leq t\leq2$. It is strictly negative inside the interval and integrates to $-1/15$. The [Peano kernel theorem](#peano-kernel-theorem) therefore gives the sharp bound $|L(f)|\leq\|f^{(4)}\|_\infty/90$; $f(x)=x^4/24$ attains equality. Scaling to endpoint spacing $h$ gives $h^5/90$. The normalized [Peano kernel](#peano-kernel) is $K/3!$, so the external factorial must be omitted when using that normalization.

#### Convergence of positive quadrature on continuous functions

↑ **Parent:** [Quadrature rule](#quadrature-rule)

On a compact interval, positive [quadrature rule](#quadrature-rule) weights whose sum is the interval length define uniformly bounded functionals on [continuous functions](calculus.md#continuous-function). If the rules eventually integrate every fixed [polynomial](polynomial.md) exactly, the [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) proves convergence for every [continuous function](calculus.md#continuous-function).

#### Nodal-polynomial criterion for quadrature exactness

↑ **Parent:** [Quadrature rule](#quadrature-rule)

An $(n+1)$-node [quadrature rule](#quadrature-rule) already exact through degree $n$ is exact through degree $n+1+k$ exactly when its nodal polynomial

$$
Q_{n+1}(x)=\prod_{i=0}^n(x-x_i)
$$

is orthogonal to every polynomial of degree at most $k$.

#### Degree ceiling for quadrature exactness

↑ **Parent:** [Quadrature rule](#quadrature-rule)

No $(n+1)$-node quadrature rule for a positive interval weight can be exact through degree $2n+2$, because it evaluates the nonnegative nodal square $Q_{n+1}^2$ as zero although its integral is positive.

#### Positivity of quadrature weights from degree 2n exactness

↑ **Parent:** [Quadrature rule](#quadrature-rule)

If an $(n+1)$-node quadrature rule for a positive interval weight is exact through degree $2n$, every weight is positive. Indeed, applying the rule to the square of the corresponding degree-$n$ Lagrange cardinal polynomial isolates that weight.

#### Convergence of positive quadrature rules

↑ **Parent:** [Quadrature rule](#quadrature-rule)

If each $(n+1)$-node quadrature rule is exact through degree $n$ and has positive weights, then it converges on every continuous function. The [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) reduces the error to the uniform polynomial-approximation error, while exactness on constants controls the sum of the weights.

#### Moment matching

↑ **Parent:** [Quadrature rule](#quadrature-rule)

A quadrature rule is exact through degree $d$ precisely when its node weights reproduce the first $d+1$ moments of the integration measure.

## Midpoint method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Midpoint_method)

The [midpoint method](#midpoint-method) advances an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) using a derivative evaluated at a temporal midpoint. Its explicit form predicts that midpoint from the initial derivative, while the [implicit midpoint rule](#implicit-midpoint-rule) solves for the derivative at the mean of the endpoint states.

## Collocation method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Collocation_method)

A [collocation method](#collocation-method) chooses an approximate solution from a finite-dimensional trial space and forces the residual of a [differential equation](differential-equation.md) to vanish at selected nodes. [Collocation Runge-Kutta methods](#collocation-runge-kutta-method) apply this principle to polynomial approximations on each time step.

## QR algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/QR_algorithm)

The [QR algorithm](#qr-algorithm) computes [eigenvalues](linear-operator-theory.md#eigenvalue) through repeated [QR decompositions](linear-algebra.md#qr-decomposition) and similarity updates. Shifted and unshifted forms have different convergence rates; the [unshifted QR algorithm](#unshifted-qr-algorithm) uses a zero shift at every step.

## Iterative method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iterative_method)

An [iterative method](#iterative-method) approximates a solution by repeatedly updating an initial guess. In [numerical linear algebra](#numerical-linear-algebra), a [stationary iterative method for a linear system](#stationary-iterative-method-for-a-linear-system) uses a fixed iteration map; other iterations can change their update rule or search space at each step.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
