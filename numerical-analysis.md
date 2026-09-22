# Numerical analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_analysis)

Numerical analysis designs [algorithms](algorithm.md) that approximate mathematical answers while controlling cost and error. Its central question is how much of a computed answer can be trusted. Finding a [zero of a function](polynomial.md#zero-of-a-function), evaluating an [integral](integral.md), solving a [linear system](linear-algebra.md#system-of-linear-equations), and evolving an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) all demand choices about accuracy, work, and the information available. MIT's numerical-methods course explicitly treats performance and accuracy as joint concerns.[Steven G. Johnson, MIT 18.335J, Week 1, 2019](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/pages/week-1/)

Three questions organize error analysis. [Truncation error](#truncation-error) measures the approximation introduced by an [algorithm](algorithm.md) even in exact arithmetic; [roundoff error](#round-off-error) comes from finite precision; the [condition number](quadratic-form.md#condition-number) measures sensitivity inherent in the problem. [Numerical stability](#stability-of-a-numerical-method) asks how the chosen [algorithm](algorithm.md) propagates perturbations. These distinctions suggest different remedies: refine an approximation, change precision or arithmetic, or improve the accuracy of the input.

For example, the [square root](algebra.md#square-root) $s(a)=\sqrt a$ has relative [condition number](quadratic-form.md#condition-number) $|as'(a)/s(a)|=1/2$ for $a>0$: a small relative change in $a$ produces about half that relative change in $s(a)$. In contrast, $g(a)=1/(1-a)$ has relative [condition number](quadratic-form.md#condition-number) $|a/(1-a)|$. Changing $a=0.99$ to $0.9901$ changes $g(a)=100$ to about $101.010101$: an input change of about $0.0101\%$ produces an output change of about $1.0101\%$. This sensitivity exists even with exact arithmetic. MIT's conditioning lecture separates the [condition number](quadratic-form.md#condition-number) from [roundoff error](#round-off-error) in precisely this way.[Steven G. Johnson, MIT 18.335J, Lecture 5: Condition Numbers, 2019](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/pages/week-2/)

**Table of contents**

- [Root finding](#root-finding)
- [Fixed-point iteration](#fixed-point-iteration)
- [Fixed-point arithmetic](#fixed-point-arithmetic)
- [Rounding](#rounding)
- [Shooting method](#shooting-method)
- [Golden-section search](#golden-section-search)
- [Significant figures](#significant-figures)
- [Numerical method](#numerical-method)
  - [Velocity Verlet method](#velocity-verlet-method)
  - [Numerical algorithm](#numerical-algorithm)
- [Floating-point arithmetic](floating-point-arithmetic.md)
  - [Floating-point underflow](floating-point-arithmetic.md#floating-point-underflow)
  - [Floating-point representation](floating-point-arithmetic.md#floating-point-representation)
  - [Floating-point number](floating-point-arithmetic.md#floating-point-number)
  - [Compensated summation](floating-point-arithmetic.md#compensated-summation)
    - [Kahan summation algorithm](floating-point-arithmetic.md#kahan-summation-algorithm)
  - [Machine epsilon](floating-point-arithmetic.md#machine-epsilon)
  - [Unit roundoff](floating-point-arithmetic.md#unit-roundoff)
  - [Subnormal number](floating-point-arithmetic.md#subnormal-number)
  - [Catastrophic cancellation](floating-point-arithmetic.md#catastrophic-cancellation)
- [Newton root-finding iteration](#newton-root-finding-iteration)
  - [Exact Newton error identity for a quadratic](#exact-newton-error-identity-for-a-quadratic)
  - [Local quadratic convergence of Newton iteration](#local-quadratic-convergence-of-newton-iteration)
  - [Newton iteration in a Banach space](#newton-iteration-in-a-banach-space)
    - [Frozen Newton correction for a fixed-point equation](#frozen-newton-correction-for-a-fixed-point-equation)
    - [Quadratic Newton error bound in a Banach space](#quadratic-newton-error-bound-in-a-banach-space)
  - [Monotone Newton convergence for a strictly convex function](#monotone-newton-convergence-for-a-strictly-convex-function)
- [Bracketing method](#bracketing-method)
  - [Root bracket](#root-bracket)
  - [Bisection method](#bisection-method)
    - [Bisection error bound](#bisection-error-bound)
    - [Bisection stopping criterion](#bisection-stopping-criterion)
    - [Limitations of bisection](#limitations-of-bisection)
- [Chord error bound](#chord-error-bound)
- [Interval arithmetic](#interval-arithmetic)
  - [Interval enclosure](#interval-enclosure)
  - [Interval arithmetic operations](#interval-arithmetic-operations)
    - [Natural interval extension](#natural-interval-extension)
      - [Interval dependency problem](#interval-dependency-problem)
        - [Interval subdivision](#interval-subdivision)
    - [Interval square range](#interval-square-range)
  - [Outward rounding](#outward-rounding)
  - [Interval root exclusion](#interval-root-exclusion)
- [Continuation method](#continuation-method)
  - [Solution branch](#solution-branch)
  - [Parameter continuation](#parameter-continuation)
  - [Fold of a solution branch](#fold-of-a-solution-branch)
  - [Pseudo-arclength continuation](#pseudo-arclength-continuation)
    - [Continuation predictor-corrector step](#continuation-predictor-corrector-step)
  - [Transversal surface intersection tracing](#transversal-surface-intersection-tracing)
    - [Transversal intersection of two parametric surfaces](#transversal-intersection-of-two-parametric-surfaces)
- [Computer aided geometric design](computer-aided-geometric-design.md)
  - [Affine equivariance of a geometric basis](computer-aided-geometric-design.md#affine-equivariance-of-a-geometric-basis)
  - [Translational penetration depth](computer-aided-geometric-design.md#translational-penetration-depth)
  - [Linear precision of a geometric basis](computer-aided-geometric-design.md#linear-precision-of-a-geometric-basis)
  - [Control point](computer-aided-geometric-design.md#control-point)
    - [Control-point influence on a curve](computer-aided-geometric-design.md#control-point-influence-on-a-curve)
    - [Control net](computer-aided-geometric-design.md#control-net)
    - [Control polygon](computer-aided-geometric-design.md#control-polygon)
  - [Apparent-gravity camera frame](computer-aided-geometric-design.md#apparent-gravity-camera-frame)
  - [Subdivision curve](computer-aided-geometric-design.md#subdivision-curve)
    - [Binary linear interpolatory subdivision](computer-aided-geometric-design.md#binary-linear-interpolatory-subdivision)
    - [Functional precision set of a subdivision scheme](computer-aided-geometric-design.md#functional-precision-set-of-a-subdivision-scheme)
    - [Chaikin subdivision](computer-aided-geometric-design.md#chaikin-subdivision)
      - [Chaikin basis function](computer-aided-geometric-design.md#chaikin-basis-function)
      - [Polynomial degree preservation under Chaikin subdivision](computer-aided-geometric-design.md#polynomial-degree-preservation-under-chaikin-subdivision)
    - [Support of a stationary subdivision scheme](computer-aided-geometric-design.md#support-of-a-stationary-subdivision-scheme)
    - [Subdivision curve interrogation](computer-aided-geometric-design.md#subdivision-curve-interrogation)
      - [Closest-point search on a subdivision curve](computer-aided-geometric-design.md#closest-point-search-on-a-subdivision-curve)
      - [Shadow tracing for a subdivision curve](computer-aided-geometric-design.md#shadow-tracing-for-a-subdivision-curve)
      - [Recursive half-space clipping of a subdivision curve](computer-aided-geometric-design.md#recursive-half-space-clipping-of-a-subdivision-curve)
  - [Subdivision surface](computer-aided-geometric-design.md#subdivision-surface)
    - [Lateral artifacts of a subdivision surface](computer-aided-geometric-design.md#lateral-artifacts-of-a-subdivision-surface)
      - [Extrusion invariance of a ternary triangular scheme](computer-aided-geometric-design.md#extrusion-invariance-of-a-ternary-triangular-scheme)
    - [Mid-edge subdivision](computer-aided-geometric-design.md#mid-edge-subdivision)
      - [Mid-edge facet centroid invariance](computer-aided-geometric-design.md#mid-edge-facet-centroid-invariance)
    - [Subdivision surface interrogation](computer-aided-geometric-design.md#subdivision-surface-interrogation)
      - [Intersection of subdivision limit surfaces](computer-aided-geometric-design.md#intersection-of-subdivision-limit-surfaces)
      - [Plane section of a subdivision surface](computer-aided-geometric-design.md#plane-section-of-a-subdivision-surface)
      - [Minimum distance between subdivision bodies](computer-aided-geometric-design.md#minimum-distance-between-subdivision-bodies)
    - [Extraordinary subdivision vertex](computer-aided-geometric-design.md#extraordinary-subdivision-vertex)
      - [Characteristic map of a subdivision surface](computer-aided-geometric-design.md#characteristic-map-of-a-subdivision-surface)
    - [Quincunx subdivision](computer-aided-geometric-design.md#quincunx-subdivision)
    - [Loop subdivision surface](computer-aided-geometric-design.md#loop-subdivision-surface)
      - [Polynomial generation by regular Loop subdivision](computer-aided-geometric-design.md#polynomial-generation-by-regular-loop-subdivision)
      - [Extrusion invariance of Loop subdivision](computer-aided-geometric-design.md#extrusion-invariance-of-loop-subdivision)
    - [Subdivision mask](computer-aided-geometric-design.md#subdivision-mask)
      - [Subdivision mask width](computer-aided-geometric-design.md#subdivision-mask-width)
      - [Subdivision arity](computer-aided-geometric-design.md#subdivision-arity)
      - [Subdivision difference scheme](computer-aided-geometric-design.md#subdivision-difference-scheme)
        - [Norm and spectral bounds for subdivision regularity](computer-aided-geometric-design.md#norm-and-spectral-bounds-for-subdivision-regularity)
      - [Subdivision matrix](computer-aided-geometric-design.md#subdivision-matrix)
  - [Bézier curve](computer-aided-geometric-design.md#bezier-curve)
    - [Bézier derivative control polygon](computer-aided-geometric-design.md#bezier-derivative-control-polygon)
      - [Parametric first-derivative join of Bézier curves](computer-aided-geometric-design.md#parametric-first-derivative-join-of-bezier-curves)
    - [De Casteljau's algorithm](computer-aided-geometric-design.md#de-casteljau-s-algorithm)
  - [Bounding volume](computer-aided-geometric-design.md#bounding-volume)
    - [Conservative enclosure test](computer-aided-geometric-design.md#conservative-enclosure-test)
    - [Collision detection](computer-aided-geometric-design.md#collision-detection)
      - [Broad phase](computer-aided-geometric-design.md#broad-phase)
      - [Narrow phase](computer-aided-geometric-design.md#narrow-phase)
    - [Bounding volume hierarchy](computer-aided-geometric-design.md#bounding-volume-hierarchy)
      - [Bounding volume hierarchy traversal](computer-aided-geometric-design.md#bounding-volume-hierarchy-traversal)
    - [Axis-aligned bounding box](computer-aided-geometric-design.md#axis-aligned-bounding-box)
  - [Triangle-triangle intersection algorithm](computer-aided-geometric-design.md#triangle-triangle-intersection-algorithm)
- [Round-off error](#round-off-error)
- [Richardson extrapolation](#richardson-extrapolation)
- [Error control for ODE solvers](error-control-for-ode-solvers.md)
  - [Adaptive step-size controller](error-control-for-ode-solvers.md#adaptive-step-size-controller)
  - [Absolute and relative error tolerances](error-control-for-ode-solvers.md#absolute-and-relative-error-tolerances)
  - [Local error estimator](error-control-for-ode-solvers.md#local-error-estimator)
    - [Predictor-corrector error estimation](error-control-for-ode-solvers.md#predictor-corrector-error-estimation)
    - [Embedded Runge-Kutta pair](error-control-for-ode-solvers.md#embedded-runge-kutta-pair)
      - [Euler-Heun embedded pair](error-control-for-ode-solvers.md#euler-heun-embedded-pair)
        - [Adaptive Euler-Heun integration of exponential growth](error-control-for-ode-solvers.md#adaptive-euler-heun-integration-of-exponential-growth)
    - [Step-doubling error estimation](error-control-for-ode-solvers.md#step-doubling-error-estimation)
  - [Adaptive Euler step doubling for exponential decay](error-control-for-ode-solvers.md#adaptive-euler-step-doubling-for-exponential-decay)
- [Finite volume method](finite-volume-method.md)
  - [Shared face flux cancellation](finite-volume-method.md#shared-face-flux-cancellation)
  - [Periodic upwind finite volume advection](finite-volume-method.md#periodic-upwind-finite-volume-advection)
  - [Monotone conservative scheme](finite-volume-method.md#monotone-conservative-scheme)
    - [Total variation diminishing scheme](finite-volume-method.md#total-variation-diminishing-scheme)
    - [L1 contraction of a monotone conservative scheme](finite-volume-method.md#l1-contraction-of-a-monotone-conservative-scheme)
    - [Engquist-Osher method](finite-volume-method.md#engquist-osher-method)
      - [CFL necessity for explicit Engquist-Osher stability](finite-volume-method.md#cfl-necessity-for-explicit-engquist-osher-stability)
      - [Engquist-Osher flux](finite-volume-method.md#engquist-osher-flux)
        - [Sonic-point splitting of a convex Engquist-Osher flux](finite-volume-method.md#sonic-point-splitting-of-a-convex-engquist-osher-flux)
  - [Numerical flux](finite-volume-method.md#numerical-flux)
    - [Godunov numerical flux](finite-volume-method.md#godunov-numerical-flux)
- [Interval bisection](#interval-bisection)
- [Implicit time-stepping method](#implicit-time-stepping-method)
- [Multigrid method](multigrid-method.md)
  - [Full multigrid](multigrid-method.md#full-multigrid)
  - [Two-grid Poisson factor with weighted Jacobi](multigrid-method.md#two-grid-poisson-factor-with-weighted-jacobi)
  - [Geometric multigrid V-cycle](multigrid-method.md#geometric-multigrid-v-cycle)
  - [Full-weighting restriction](multigrid-method.md#full-weighting-restriction)
  - [Coarse-grid correction](multigrid-method.md#coarse-grid-correction)
    - [Galerkin coarse-grid operator](multigrid-method.md#galerkin-coarse-grid-operator)
- [Convergence of a numerical method](#convergence-of-a-numerical-method)
  - [Quadratic convergence](#quadratic-convergence)
- [Global discretization error](#global-discretization-error)
  - [Variable-step global ODE error bound](#variable-step-global-ode-error-bound)
  - [Residual bound for global ODE error](#residual-bound-for-global-ode-error)
- [Midpoint quadrature rule](#midpoint-quadrature-rule)
  - [Composite midpoint quadrature rule](#composite-midpoint-quadrature-rule)
- [Approximation error](#approximation-error)
  - [Error bound](#error-bound)
  - [Absolute error](#absolute-error)
  - [Relative error](#relative-error)
    - [Signed relative error](#signed-relative-error)
- [Truncation error](#truncation-error)
  - [Series truncation error](#series-truncation-error)
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
- [Finite element method](finite-element-method.md)
  - [Finite element solution of the one-dimensional Poisson equation](finite-element-method.md#finite-element-solution-of-the-one-dimensional-poisson-equation)
  - [Semidiscrete finite element heat equation](finite-element-method.md#semidiscrete-finite-element-heat-equation)
    - [Forward Euler limit for a consistent hat mass matrix](finite-element-method.md#forward-euler-limit-for-a-consistent-hat-mass-matrix)
  - [Finite element](finite-element-method.md#finite-element)
  - [Conforming finite element space](finite-element-method.md#conforming-finite-element-space)
  - [Finite element mesh](finite-element-method.md#finite-element-mesh)
    - [Shape-regular mesh](finite-element-method.md#shape-regular-mesh)
  - [Finite element interpolation estimate](finite-element-method.md#finite-element-interpolation-estimate)
  - [Mass matrix](finite-element-method.md#mass-matrix)
    - [Mass eigenstate](finite-element-method.md#mass-eigenstate)
    - [Affine-weighted hat mass matrix](finite-element-method.md#affine-weighted-hat-mass-matrix)
  - [Stiffness matrix](finite-element-method.md#stiffness-matrix)
    - [Reaction-diffusion finite element matrix](finite-element-method.md#reaction-diffusion-finite-element-matrix)
  - [Energy conservation for semidiscrete Galerkin advection](finite-element-method.md#energy-conservation-for-semidiscrete-galerkin-advection)
  - [Cubic Hermite finite element](finite-element-method.md#cubic-hermite-finite-element)
  - [Rayleigh-Ritz method](finite-element-method.md#rayleigh-ritz-method)
    - [Trial function](finite-element-method.md#trial-function)
    - [Affine-parameter Sturm-Liouville eigenvalue bound](finite-element-method.md#affine-parameter-sturm-liouville-eigenvalue-bound)
    - [Exponential-polynomial trial space for a mixed Sturm-Liouville problem](finite-element-method.md#exponential-polynomial-trial-space-for-a-mixed-sturm-liouville-problem)
    - [Ritz-Galerkin equivalence for a symmetric coercive form](finite-element-method.md#ritz-galerkin-equivalence-for-a-symmetric-coercive-form)
      - [Symmetry and coercivity in quadratic energy minimization](finite-element-method.md#symmetry-and-coercivity-in-quadratic-energy-minimization)
    - [Energy norm](finite-element-method.md#energy-norm)
  - [Galerkin orthogonality](finite-element-method.md#galerkin-orthogonality)
    - [Céa's lemma](finite-element-method.md#cea-s-lemma)
      - [Aubin–Nitsche duality argument](finite-element-method.md#aubin-nitsche-duality-argument)
  - [Piecewise-linear hat function](finite-element-method.md#piecewise-linear-hat-function)
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
- [Discrete Fourier transform](discrete-fourier-transform.md)
  - [Number-theoretic transform](discrete-fourier-transform.md#number-theoretic-transform)
  - [Fourier frequency resolution](discrete-fourier-transform.md#fourier-frequency-resolution)
  - [Discrete Fourier conjugate symmetry](discrete-fourier-transform.md#discrete-fourier-conjugate-symmetry)
  - [Periodic extension of a finite sequence](discrete-fourier-transform.md#periodic-extension-of-a-finite-sequence)
  - [Aliasing of discrete Fourier modes](discrete-fourier-transform.md#aliasing-of-discrete-fourier-modes)
  - [Prime Fourier matrix minor theorem](discrete-fourier-transform.md#prime-fourier-matrix-minor-theorem)
  - [Finite-field discrete Fourier transform](discrete-fourier-transform.md#finite-field-discrete-fourier-transform)
  - [Discrete Parseval identity](discrete-fourier-transform.md#discrete-parseval-identity)
  - [Fourier representation of a Kronecker delta](discrete-fourier-transform.md#fourier-representation-of-a-kronecker-delta)
  - [Fourier frequency](discrete-fourier-transform.md#fourier-frequency)
  - [Inverse discrete Fourier transform](discrete-fourier-transform.md#inverse-discrete-fourier-transform)
  - [Discrete Fourier mode](discrete-fourier-transform.md#discrete-fourier-mode)
  - [Fast Fourier transform](discrete-fourier-transform.md#fast-fourier-transform)
    - [Good-Thomas algorithm](discrete-fourier-transform.md#good-thomas-algorithm)
    - [Cooley-Tukey FFT algorithm](discrete-fourier-transform.md#cooley-tukey-fft-algorithm)
      - [FFT butterfly](discrete-fourier-transform.md#fft-butterfly)
      - [Even--odd fast Fourier transform recursion](discrete-fourier-transform.md#even-odd-fast-fourier-transform-recursion)
  - [Discrete cosine transform](discrete-fourier-transform.md#discrete-cosine-transform)
    - [Discrete cosine transform from an even-reflected discrete Fourier transform](discrete-fourier-transform.md#discrete-cosine-transform-from-an-even-reflected-discrete-fourier-transform)
  - [Discrete sine transform](discrete-fourier-transform.md#discrete-sine-transform)
    - [Discrete sine transform Poisson solver](discrete-fourier-transform.md#discrete-sine-transform-poisson-solver)
    - [Discrete sine transform from a sign-modulated discrete cosine transform](discrete-fourier-transform.md#discrete-sine-transform-from-a-sign-modulated-discrete-cosine-transform)
- [Interpolation](interpolation.md)
  - [Extrapolation](interpolation.md#extrapolation)
  - [Interpolant](interpolation.md#interpolant)
  - [Polynomial interpolation](interpolation.md#polynomial-interpolation)
    - [Newton forward interpolation](interpolation.md#newton-forward-interpolation)
    - [Interpolation polynomial](interpolation.md#interpolation-polynomial)
    - [Interpolation nodes from best uniform approximation](interpolation.md#interpolation-nodes-from-best-uniform-approximation)
    - [Interpolation node](interpolation.md#interpolation-node)
      - [Chebyshev-Lobatto node](interpolation.md#chebyshev-lobatto-node)
    - [Runge's phenomenon](interpolation.md#runge-s-phenomenon)
    - [Lagrange polynomial](interpolation.md#lagrange-polynomial)
      - [Differentiation weights from nodal evaluations](interpolation.md#differentiation-weights-from-nodal-evaluations)
      - [Discrete minimax interpolation on ordered nodes](interpolation.md#discrete-minimax-interpolation-on-ordered-nodes)
      - [Lagrange cardinal polynomial](interpolation.md#lagrange-cardinal-polynomial)
        - [Endpoint derivative signs of Lagrange cardinal polynomials](interpolation.md#endpoint-derivative-signs-of-lagrange-cardinal-polynomials)
        - [Nodal derivative norm from Lagrange cardinal polynomials](interpolation.md#nodal-derivative-norm-from-lagrange-cardinal-polynomials)
      - [Barycentric interpolation formula](interpolation.md#barycentric-interpolation-formula)
    - [Divided difference](interpolation.md#divided-difference)
      - [Divided difference table](interpolation.md#divided-difference-table)
      - [Symmetry of divided differences](interpolation.md#symmetry-of-divided-differences)
      - [Omitted-node identities for divided differences](interpolation.md#omitted-node-identities-for-divided-differences)
      - [Exponential divided difference](interpolation.md#exponential-divided-difference)
      - [Leibniz rule for divided differences](interpolation.md#leibniz-rule-for-divided-differences)
      - [Newton polynomial](interpolation.md#newton-polynomial)
        - [Node order in Newton interpolation](interpolation.md#node-order-in-newton-interpolation)
- [Gershgorin circle theorem](#gershgorin-circle-theorem)
  - [Gershgorin disc](#gershgorin-disc)
  - [Gershgorin eigenvalue counting](#gershgorin-eigenvalue-counting)
  - [Gershgorin bounds for symmetric matrices](#gershgorin-bounds-for-symmetric-matrices)
  - [Diagonal scaling of Gershgorin discs](#diagonal-scaling-of-gershgorin-discs)
  - [Gershgorin stability bound for a variable-coefficient diffusion stencil](#gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil)
- [Finite difference](finite-difference.md)
  - [Newton series](finite-difference.md#newton-series)
  - [Forward difference](finite-difference.md#forward-difference)
  - [First difference](finite-difference.md#first-difference)
  - [Three-point asymmetric second-derivative formula](finite-difference.md#three-point-asymmetric-second-derivative-formula)
  - [Randomized symmetric finite-difference derivative estimator](finite-difference.md#randomized-symmetric-finite-difference-derivative-estimator)
  - [Finite difference method](finite-difference.md#finite-difference-method)
    - [Even-reflection closure for Neumann diffusion](finite-difference.md#even-reflection-closure-for-neumann-diffusion)
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
  - [Tridiagonal elimination recurrences](#tridiagonal-elimination-recurrences)
  - [Dirichlet Poisson solution by tridiagonal elimination](#dirichlet-poisson-solution-by-tridiagonal-elimination)
  - [Safe pivots for tridiagonal elimination](#safe-pivots-for-tridiagonal-elimination)
  - [Zero-pivot failure of tridiagonal elimination](#zero-pivot-failure-of-tridiagonal-elimination)
  - [Tridiagonal solve costs](#tridiagonal-solve-costs)
- [Gaussian quadrature](#gaussian-quadrature)
  - [Gauss-Legendre quadrature](#gauss-legendre-quadrature)
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
    - [Neumann eigenfunctions of the Chebyshev differential operator](#neumann-eigenfunctions-of-the-chebyshev-differential-operator)
    - [Dirichlet eigenfunctions of the Chebyshev differential operator](#dirichlet-eigenfunctions-of-the-chebyshev-differential-operator)
    - [Power series of the Chebyshev differential equation](#power-series-of-the-chebyshev-differential-equation)
    - [Regular solution of a forced Chebyshev equation](#regular-solution-of-a-forced-chebyshev-equation)
    - [Chebyshev derivative Sturm-Liouville pair](#chebyshev-derivative-sturm-liouville-pair)
- [Backward differentiation formula](#backward-differentiation-formula)
  - [Second-order backward differentiation formula](#second-order-backward-differentiation-formula)
  - [BDF2 discrete energy identity](#bdf2-discrete-energy-identity)
- [Constrained optimization](#constrained-optimization)
  - [Constraint reparameterization](#constraint-reparameterization)
  - [Optimization constraint](#optimization-constraint)
- [Equally spaced interpolation](#equally-spaced-interpolation)
- [Givens rotation](#givens-rotation)
  - [Stable construction of a Givens rotation](#stable-construction-of-a-givens-rotation)
  - [Givens row-pair update](#givens-row-pair-update)
  - [QR decomposition by Givens rotations](#qr-decomposition-by-givens-rotations)
- [Gradient descent](gradient-descent.md)
  - [Fixed-step gradient descent on a positive-definite quadratic](gradient-descent.md#fixed-step-gradient-descent-on-a-positive-definite-quadratic)
    - [Optimal fixed step for quadratic gradient descent](gradient-descent.md#optimal-fixed-step-for-quadratic-gradient-descent)
  - [Gradient ascent](gradient-descent.md#gradient-ascent)
  - [Stochastic gradient descent](gradient-descent.md#stochastic-gradient-descent)
    - [Projected stochastic gradient descent](gradient-descent.md#projected-stochastic-gradient-descent)
    - [Unbiased stochastic gradient](gradient-descent.md#unbiased-stochastic-gradient)
  - [Lipschitz gradient](gradient-descent.md#lipschitz-gradient)
    - [Descent lemma](gradient-descent.md#descent-lemma)
  - [Exact line search for a positive-definite quadratic](gradient-descent.md#exact-line-search-for-a-positive-definite-quadratic)
  - [Conjugate gradient method](gradient-descent.md#conjugate-gradient-method)
    - [Linear-system residual](gradient-descent.md#linear-system-residual)
    - [Conjugate-gradient residual orthogonality](gradient-descent.md#conjugate-gradient-residual-orthogonality)
    - [Preconditioned conjugate gradient method](gradient-descent.md#preconditioned-conjugate-gradient-method)
      - [Exact inverse-square-root preconditioner](gradient-descent.md#exact-inverse-square-root-preconditioner)
    - [Krylov subspace](gradient-descent.md#krylov-subspace)
      - [Krylov dimension from spectral components](gradient-descent.md#krylov-dimension-from-spectral-components)
    - [Finite termination of the conjugate gradient method](gradient-descent.md#finite-termination-of-the-conjugate-gradient-method)
  - [Heavy-ball method](gradient-descent.md#heavy-ball-method)
    - [Heavy-ball residual recurrence](gradient-descent.md#heavy-ball-residual-recurrence)
    - [Heavy-ball error propagation matrix](gradient-descent.md#heavy-ball-error-propagation-matrix)
      - [Heavy-ball rate for a two-eigenvalue diagonal quadratic](gradient-descent.md#heavy-ball-rate-for-a-two-eigenvalue-diagonal-quadratic)
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
- [Runge-Kutta method](runge-kutta-method.md)
  - [Runge-Kutta stage](runge-kutta-method.md#runge-kutta-stage)
  - [Explicit Runge-Kutta method](runge-kutta-method.md#explicit-runge-kutta-method)
    - [Heun's method](runge-kutta-method.md#heun-s-method)
  - [Maximal-order Runge-Kutta methods are A-stable](runge-kutta-method.md#maximal-order-runge-kutta-methods-are-a-stable)
  - [Theta method](runge-kutta-method.md#theta-method)
    - [Theta diffusion stability criterion](runge-kutta-method.md#theta-diffusion-stability-criterion)
      - [Rough-data damping distinction for the theta method](runge-kutta-method.md#rough-data-damping-distinction-for-the-theta-method)
  - [Strong stability preserving Runge-Kutta method](runge-kutta-method.md#strong-stability-preserving-runge-kutta-method)
  - [Classical fourth-order Runge-Kutta method](runge-kutta-method.md#classical-fourth-order-runge-kutta-method)
  - [Butcher tableau](runge-kutta-method.md#butcher-tableau)
  - [Butcher order condition](runge-kutta-method.md#butcher-order-condition)
    - [Second-order conditions with independent Runge-Kutta abscissae](runge-kutta-method.md#second-order-conditions-with-independent-runge-kutta-abscissae)
    - [Fourth-order conditions for a Runge-Kutta method](runge-kutta-method.md#fourth-order-conditions-for-a-runge-kutta-method)
  - [Implicit Runge-Kutta method](runge-kutta-method.md#implicit-runge-kutta-method)
    - [Two-stage Runge-Kutta family with an implicit second stage](runge-kutta-method.md#two-stage-runge-kutta-family-with-an-implicit-second-stage)
    - [Stage solvability of an implicit Runge-Kutta method](runge-kutta-method.md#stage-solvability-of-an-implicit-runge-kutta-method)
    - [Implicit midpoint rule](runge-kutta-method.md#implicit-midpoint-rule)
    - [Crank-Nicolson method](runge-kutta-method.md#crank-nicolson-method)
      - [Contractivity of split Crank-Nicolson diffusion](runge-kutta-method.md#contractivity-of-split-crank-nicolson-diffusion)
    - [Collocation Runge-Kutta method](runge-kutta-method.md#collocation-runge-kutta-method)
      - [Two-node collocation A-stability criterion](runge-kutta-method.md#two-node-collocation-a-stability-criterion)
      - [Collocation order theorem](runge-kutta-method.md#collocation-order-theorem)
        - [Collocation endpoint superconvergence by quadrature orthogonality](runge-kutta-method.md#collocation-endpoint-superconvergence-by-quadrature-orthogonality)
      - [Collocation tableau row-sum identity](runge-kutta-method.md#collocation-tableau-row-sum-identity)
      - [Lobatto IIIA method](runge-kutta-method.md#lobatto-iiia-method)
      - [Gauss-Legendre method](runge-kutta-method.md#gauss-legendre-method)
        - [Gauss collocation coefficient construction](runge-kutta-method.md#gauss-collocation-coefficient-construction)
        - [Fourth-order two-stage Gauss collocation method](runge-kutta-method.md#fourth-order-two-stage-gauss-collocation-method)
      - [Radau IIA method](runge-kutta-method.md#radau-iia-method)
        - [Padé identification of a Radau stability function](runge-kutta-method.md#pade-identification-of-a-radau-stability-function)
      - [Algebraic stability of a Runge-Kutta method](runge-kutta-method.md#algebraic-stability-of-a-runge-kutta-method)
        - [Runge-Kutta conservation of quadratic invariants](runge-kutta-method.md#runge-kutta-conservation-of-quadratic-invariants)
        - [Butcher contractivity theorem](runge-kutta-method.md#butcher-contractivity-theorem)
        - [Runge-Kutta contractivity identity](runge-kutta-method.md#runge-kutta-contractivity-identity)
    - [Trapezoidal rule](runge-kutta-method.md#trapezoidal-rule)
      - [Composite trapezoidal rule](runge-kutta-method.md#composite-trapezoidal-rule)
      - [Trapezoidal rule fails B-stability](runge-kutta-method.md#trapezoidal-rule-fails-b-stability)
  - [Time-symmetric numerical method](runge-kutta-method.md#time-symmetric-numerical-method)
  - [Order of a Runge-Kutta method](runge-kutta-method.md#order-of-a-runge-kutta-method)
    - [Third-order conditions for an explicit Runge-Kutta method](runge-kutta-method.md#third-order-conditions-for-an-explicit-runge-kutta-method)
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
- [Linear multistep method](linear-multistep-method.md)
  - [Reciprocal-root three-step multistep family](linear-multistep-method.md#reciprocal-root-three-step-multistep-family)
  - [Simpson multistep method](linear-multistep-method.md#simpson-multistep-method)
  - [First Dahlquist barrier](linear-multistep-method.md#first-dahlquist-barrier)
    - [Newton-Cotes multistep methods attaining the first Dahlquist barrier](linear-multistep-method.md#newton-cotes-multistep-methods-attaining-the-first-dahlquist-barrier)
    - [Cayley coefficient proof of the first Dahlquist barrier](linear-multistep-method.md#cayley-coefficient-proof-of-the-first-dahlquist-barrier)
      - [Coefficient sign lemma for the first Dahlquist barrier](linear-multistep-method.md#coefficient-sign-lemma-for-the-first-dahlquist-barrier)
  - [Two-step family with a third-order member](linear-multistep-method.md#two-step-family-with-a-third-order-member)
  - [Adams-Bashforth method](linear-multistep-method.md#adams-bashforth-method)
    - [Adams-Bashforth stability for centered diffusion](linear-multistep-method.md#adams-bashforth-stability-for-centered-diffusion)
  - [Common-factor cancellation defect in a multistep recurrence](linear-multistep-method.md#common-factor-cancellation-defect-in-a-multistep-recurrence)
  - [Trapezoidal-BDF two-step family](linear-multistep-method.md#trapezoidal-bdf-two-step-family)
  - [Multiderivative multistep method](linear-multistep-method.md#multiderivative-multistep-method)
    - [Symmetric sixth-order two-derivative method](linear-multistep-method.md#symmetric-sixth-order-two-derivative-method)
    - [Symmetric two-step two-derivative formula](linear-multistep-method.md#symmetric-two-step-two-derivative-formula)
      - [Bounded-root stability set of the symmetric two-derivative formula](linear-multistep-method.md#bounded-root-stability-set-of-the-symmetric-two-derivative-formula)
      - [Empty strict decay domain of the symmetric two-derivative formula](linear-multistep-method.md#empty-strict-decay-domain-of-the-symmetric-two-derivative-formula)
      - [Negative-real instability of the symmetric two-derivative formula](linear-multistep-method.md#negative-real-instability-of-the-symmetric-two-derivative-formula)
    - [A-stable third-order two-step multiderivative method](linear-multistep-method.md#a-stable-third-order-two-step-multiderivative-method)
    - [Convergence of a zero-stable multiderivative method](linear-multistep-method.md#convergence-of-a-zero-stable-multiderivative-method)
  - [Zero-stability](linear-multistep-method.md#zero-stability)
    - [Root condition for a multistep method](linear-multistep-method.md#root-condition-for-a-multistep-method)
      - [Parasitic amplification root](linear-multistep-method.md#parasitic-amplification-root)
        - [Centered two-step discretization of exponential decay](linear-multistep-method.md#centered-two-step-discretization-of-exponential-decay)
      - [Root stability of a cubic multistep polynomial](linear-multistep-method.md#root-stability-of-a-cubic-multistep-polynomial)
  - [Dahlquist equivalence theorem](linear-multistep-method.md#dahlquist-equivalence-theorem)
    - [Necessity of the root condition for multistep convergence](linear-multistep-method.md#necessity-of-the-root-condition-for-multistep-convergence)
  - [Characteristic polynomials of a linear multistep method](linear-multistep-method.md#characteristic-polynomials-of-a-linear-multistep-method)
    - [Amplification polynomial of a multistep method](linear-multistep-method.md#amplification-polynomial-of-a-multistep-method)
      - [Amplification root](linear-multistep-method.md#amplification-root)
      - [Exterior roots of the derivative polynomial bound multistep stability](linear-multistep-method.md#exterior-roots-of-the-derivative-polynomial-bound-multistep-stability)
    - [Order conditions for a linear multistep method](linear-multistep-method.md#order-conditions-for-a-linear-multistep-method)
      - [Exponential-symbol order criterion for a multistep method](linear-multistep-method.md#exponential-symbol-order-criterion-for-a-multistep-method)
  - [Adams–Moulton method](linear-multistep-method.md#adams-moulton-method)
  - [Second Dahlquist barrier](linear-multistep-method.md#second-dahlquist-barrier)
- [Numerical linear algebra](numerical-linear-algebra.md)
  - [Matrix preconditioning](numerical-linear-algebra.md#matrix-preconditioning)
    - [Matrix preconditioner](numerical-linear-algebra.md#matrix-preconditioner)
      - [Jacobi preconditioner](numerical-linear-algebra.md#jacobi-preconditioner)
    - [Left preconditioning](numerical-linear-algebra.md#left-preconditioning)
    - [Right preconditioning](numerical-linear-algebra.md#right-preconditioning)
    - [Symmetric positive-definite preconditioning](numerical-linear-algebra.md#symmetric-positive-definite-preconditioning)
      - [Symmetric preconditioning as energy geometry](numerical-linear-algebra.md#symmetric-preconditioning-as-energy-geometry)
    - [Diagonal scaling for a two-dimensional linear system](numerical-linear-algebra.md#diagonal-scaling-for-a-two-dimensional-linear-system)
    - [Preconditioned steepest descent](numerical-linear-algebra.md#preconditioned-steepest-descent)
      - [Condition-number bound for preconditioned steepest descent](numerical-linear-algebra.md#condition-number-bound-for-preconditioned-steepest-descent)
  - [Power iteration](numerical-linear-algebra.md#power-iteration)
    - [Exact two-dimensional power iteration](numerical-linear-algebra.md#exact-two-dimensional-power-iteration)
    - [Power iteration convergence for a diagonalizable matrix](numerical-linear-algebra.md#power-iteration-convergence-for-a-diagonalizable-matrix)
      - [Power iteration direction error](numerical-linear-algebra.md#power-iteration-direction-error)
    - [Sign and phase in power iteration](numerical-linear-algebra.md#sign-and-phase-in-power-iteration)
    - [Power iteration eigenpair diagnostics](numerical-linear-algebra.md#power-iteration-eigenpair-diagnostics)
    - [Power iteration failure cases](numerical-linear-algebra.md#power-iteration-failure-cases)
  - [Gaussian elimination](numerical-linear-algebra.md#gaussian-elimination)
    - [Bareiss algorithm](numerical-linear-algebra.md#bareiss-algorithm)
    - [Gaussian elimination with a row swap](numerical-linear-algebra.md#gaussian-elimination-with-a-row-swap)
    - [Pivot element](numerical-linear-algebra.md#pivot-element)
    - [Elimination multiplier](numerical-linear-algebra.md#elimination-multiplier)
    - [Sparse Gaussian elimination](numerical-linear-algebra.md#sparse-gaussian-elimination)
      - [Sparse elimination of a four-leaf star](numerical-linear-algebra.md#sparse-elimination-of-a-four-leaf-star)
      - [Leaf elimination of a tree-pattern positive-definite matrix](numerical-linear-algebra.md#leaf-elimination-of-a-tree-pattern-positive-definite-matrix)
      - [Symbolic factorization](numerical-linear-algebra.md#symbolic-factorization)
      - [Elimination tree](numerical-linear-algebra.md#elimination-tree)
      - [Nested dissection](numerical-linear-algebra.md#nested-dissection)
      - [Minimum degree algorithm](numerical-linear-algebra.md#minimum-degree-algorithm)
      - [Fill-in](numerical-linear-algebra.md#fill-in)
      - [Matrix graph](numerical-linear-algebra.md#matrix-graph)
        - [Elimination graph](numerical-linear-algebra.md#elimination-graph)
          - [Fill-path criterion for symmetric elimination](numerical-linear-algebra.md#fill-path-criterion-for-symmetric-elimination)
    - [Columnwise partial pivoting](numerical-linear-algebra.md#columnwise-partial-pivoting)
      - [Tiny-pivot roundoff in Gaussian elimination](numerical-linear-algebra.md#tiny-pivot-roundoff-in-gaussian-elimination)
    - [Row echelon form](numerical-linear-algebra.md#row-echelon-form)
      - [Row-equivalent matrices](numerical-linear-algebra.md#row-equivalent-matrices)
      - [Row reduction with a parameterized right-hand side](numerical-linear-algebra.md#row-reduction-with-a-parameterized-right-hand-side)
      - [Reduced row echelon form](numerical-linear-algebra.md#reduced-row-echelon-form)
        - [Reading solutions from reduced row echelon form](numerical-linear-algebra.md#reading-solutions-from-reduced-row-echelon-form)
        - [Uniqueness of reduced row echelon form](numerical-linear-algebra.md#uniqueness-of-reduced-row-echelon-form)
    - [Elementary row operation](numerical-linear-algebra.md#elementary-row-operation)
      - [Elementary matrix](numerical-linear-algebra.md#elementary-matrix)
  - [LU decomposition](numerical-linear-algebra.md#lu-decomposition)
    - [Computed three-by-three LU decomposition](numerical-linear-algebra.md#computed-three-by-three-lu-decomposition)
    - [Unit triangular matrix](numerical-linear-algebra.md#unit-triangular-matrix)
    - [Triangular solves for LU decomposition](numerical-linear-algebra.md#triangular-solves-for-lu-decomposition)
      - [Forward substitution](numerical-linear-algebra.md#forward-substitution)
    - [Pivoted LU decomposition](numerical-linear-algebra.md#pivoted-lu-decomposition)
    - [Reusing LU factors for multiple right-hand sides](numerical-linear-algebra.md#reusing-lu-factors-for-multiple-right-hand-sides)
    - [LU factorization and solve costs](numerical-linear-algebra.md#lu-factorization-and-solve-costs)
  - [LDL decomposition](numerical-linear-algebra.md#ldl-decomposition)
  - [Eigenpair residual](numerical-linear-algebra.md#eigenpair-residual)
    - [Backward error of an approximate eigenpair](numerical-linear-algebra.md#backward-error-of-an-approximate-eigenpair)
  - [Householder QR decomposition](numerical-linear-algebra.md#householder-qr-decomposition)
    - [Householder reduction of an overdetermined consistent system](numerical-linear-algebra.md#householder-reduction-of-an-overdetermined-consistent-system)
  - [Householder tridiagonalization](numerical-linear-algebra.md#householder-tridiagonalization)
    - [Skew-symmetric Householder tridiagonalization](numerical-linear-algebra.md#skew-symmetric-householder-tridiagonalization)
  - [Unshifted QR algorithm](numerical-linear-algebra.md#unshifted-qr-algorithm)
    - [Accumulated QR factorization identity](numerical-linear-algebra.md#accumulated-qr-factorization-identity)
    - [Symmetric bandwidth preservation under QR iteration](numerical-linear-algebra.md#symmetric-bandwidth-preservation-under-qr-iteration)
    - [Simultaneous iteration interpretation of the QR algorithm](numerical-linear-algebra.md#simultaneous-iteration-interpretation-of-the-qr-algorithm)
      - [Two-column dominant-subspace condition](numerical-linear-algebra.md#two-column-dominant-subspace-condition)
    - [Block deflation in the QR algorithm](numerical-linear-algebra.md#block-deflation-in-the-qr-algorithm)
  - [Stationary iterative method for a linear system](numerical-linear-algebra.md#stationary-iterative-method-for-a-linear-system)
    - [Semiconvergence of cyclic Poisson iterations](numerical-linear-algebra.md#semiconvergence-of-cyclic-poisson-iterations)
    - [Richardson iteration](numerical-linear-algebra.md#richardson-iteration)
    - [Gauss-Seidel method](numerical-linear-algebra.md#gauss-seidel-method)
      - [Gauss-Seidel iteration for a two-variable positive-definite system](numerical-linear-algebra.md#gauss-seidel-iteration-for-a-two-variable-positive-definite-system)
        - [Exact error contraction of a two-variable Gauss-Seidel iteration](numerical-linear-algebra.md#exact-error-contraction-of-a-two-variable-gauss-seidel-iteration)
      - [Gauss-Seidel convergence from diagonal dominance and positive definiteness](numerical-linear-algebra.md#gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness)
        - [Gauss-Seidel iteration can diverge for an invertible matrix](numerical-linear-algebra.md#gauss-seidel-iteration-can-diverge-for-an-invertible-matrix)
    - [Successive over-relaxation](numerical-linear-algebra.md#successive-over-relaxation)
    - [Iteration matrix](numerical-linear-algebra.md#iteration-matrix)
      - [Convergence criterion for a stationary iteration](numerical-linear-algebra.md#convergence-criterion-for-a-stationary-iteration)
      - [Residual and forward error in a stationary iteration](numerical-linear-algebra.md#residual-and-forward-error-in-a-stationary-iteration)
    - [Matrix splitting](numerical-linear-algebra.md#matrix-splitting)
      - [Householder-John theorem](numerical-linear-algebra.md#householder-john-theorem)
    - [Jacobi method](numerical-linear-algebra.md#jacobi-method)
      - [Jacobi iteration for a three-variable tridiagonal system](numerical-linear-algebra.md#jacobi-iteration-for-a-three-variable-tridiagonal-system)
        - [Error modes of a three-variable Jacobi iteration](numerical-linear-algebra.md#error-modes-of-a-three-variable-jacobi-iteration)
      - [Jacobi convergence from strict diagonal dominance](numerical-linear-algebra.md#jacobi-convergence-from-strict-diagonal-dominance)
      - [Skew-tridiagonal Jacobi and Gauss-Seidel iterations](numerical-linear-algebra.md#skew-tridiagonal-jacobi-and-gauss-seidel-iterations)
      - [Weighted Jacobi method](numerical-linear-algebra.md#weighted-jacobi-method)
        - [Weighted Jacobi eigenvalues for a square Dirichlet grid](numerical-linear-algebra.md#weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid)
        - [Weighted Jacobi method for the one-dimensional Poisson equation](numerical-linear-algebra.md#weighted-jacobi-method-for-the-one-dimensional-poisson-equation)
          - [High-frequency smoothing factor of weighted Jacobi](numerical-linear-algebra.md#high-frequency-smoothing-factor-of-weighted-jacobi)
            - [Exact finite-grid high-frequency Jacobi smoothing optimum](numerical-linear-algebra.md#exact-finite-grid-high-frequency-jacobi-smoothing-optimum)
      - [Jacobi convergence for a three-by-three equicorrelation matrix](numerical-linear-algebra.md#jacobi-convergence-for-a-three-by-three-equicorrelation-matrix)
      - [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](numerical-linear-algebra.md#jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix)
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
- [Numerical integration](numerical-integration.md)
  - [Finite samples do not certify quadrature accuracy](numerical-integration.md#finite-samples-do-not-certify-quadrature-accuracy)
  - [Boole's rule](numerical-integration.md#boole-s-rule)
  - [Quadrature rule](numerical-integration.md#quadrature-rule)
    - [Quadrature node](numerical-integration.md#quadrature-node)
    - [Quadrature weight](numerical-integration.md#quadrature-weight)
    - [Degree of precision of a quadrature rule](numerical-integration.md#degree-of-precision-of-a-quadrature-rule)
    - [Noise sensitivity of a quadrature rule](numerical-integration.md#noise-sensitivity-of-a-quadrature-rule)
    - [Newton-Cotes closed quadrature](numerical-integration.md#newton-cotes-closed-quadrature)
    - [Simpson's rule](numerical-integration.md#simpson-s-rule)
      - [Adaptive Simpson's method](numerical-integration.md#adaptive-simpson-s-method)
      - [Cubic exactness of Simpson's rule](numerical-integration.md#cubic-exactness-of-simpson-s-rule)
      - [Composite Simpson's rule](numerical-integration.md#composite-simpson-s-rule)
        - [Error bound for composite Simpson's rule](numerical-integration.md#error-bound-for-composite-simpson-s-rule)
    - [Convergence of positive quadrature on continuous functions](numerical-integration.md#convergence-of-positive-quadrature-on-continuous-functions)
    - [Nodal-polynomial criterion for quadrature exactness](numerical-integration.md#nodal-polynomial-criterion-for-quadrature-exactness)
    - [Degree ceiling for quadrature exactness](numerical-integration.md#degree-ceiling-for-quadrature-exactness)
    - [Positivity of quadrature weights from degree 2n exactness](numerical-integration.md#positivity-of-quadrature-weights-from-degree-2n-exactness)
    - [Convergence of positive quadrature rules](numerical-integration.md#convergence-of-positive-quadrature-rules)
    - [Moment matching](numerical-integration.md#moment-matching)
- [Orthogonal polynomial](orthogonal-polynomial.md)
  - [Rodrigues' formula](orthogonal-polynomial.md#rodrigues-formula)
  - [Decoupled coefficients of orthogonal polynomial projections](orthogonal-polynomial.md#decoupled-coefficients-of-orthogonal-polynomial-projections)
    - [Legendre least-squares projections of a cubic](orthogonal-polynomial.md#legendre-least-squares-projections-of-a-cubic)
  - [Kravchuk polynomials](orthogonal-polynomial.md#kravchuk-polynomials)
  - [Orthogonality forces many interior zeros](orthogonal-polynomial.md#orthogonality-forces-many-interior-zeros)
  - [Zernike polynomials](orthogonal-polynomial.md#zernike-polynomials)
    - [Zernike spherical mode](orthogonal-polynomial.md#zernike-spherical-mode)
  - [Monic orthogonal polynomial](orthogonal-polynomial.md#monic-orthogonal-polynomial)
    - [Three-term recurrence for monic orthogonal polynomials](orthogonal-polynomial.md#three-term-recurrence-for-monic-orthogonal-polynomials)
  - [Hermite polynomial](orthogonal-polynomial.md#hermite-polynomial)
    - [Hermite polynomial derivative recurrence](orthogonal-polynomial.md#hermite-polynomial-derivative-recurrence)
    - [Hermite function](orthogonal-polynomial.md#hermite-function)
      - [Hermite functions are Fourier eigenfunctions](orthogonal-polynomial.md#hermite-functions-are-fourier-eigenfunctions)
      - [Mehler formula for Hermite functions](orthogonal-polynomial.md#mehler-formula-for-hermite-functions)
    - [Probabilists' Hermite polynomial](orthogonal-polynomial.md#probabilists-hermite-polynomial)
      - [Space-time Hermite polynomial](orthogonal-polynomial.md#space-time-hermite-polynomial)
  - [Zeros of orthogonal polynomials](orthogonal-polynomial.md#zeros-of-orthogonal-polynomials)
  - [Jacobi matrix](orthogonal-polynomial.md#jacobi-matrix)
- [Midpoint method](#midpoint-method)
- [Collocation method](#collocation-method)
- [QR algorithm](#qr-algorithm)
- [Iterative method](#iterative-method)
- [Forward error](#forward-error)
- [Backward error](#backward-error)

## Root finding

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

Find a value $x$ satisfying $f(x)=0$ for a given function. Methods include the [bisection method](#bisection-method), which retains a bracket around a root, and derivative-based iteration. Finding a root numerically is distinct from the root as a mathematical object.

## Fixed-point iteration

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

Fixed-point iteration seeks a [fixed point](function.md#fixed-point) of a map $F$ by repeatedly setting $x_{k+1}=F(x_k)$. Convergence requires additional hypotheses; for example, a [contraction mapping](analysis.md#contraction-mapping) on a complete metric space has a unique fixed point reached by this iteration.

## Fixed-point arithmetic

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

## Rounding

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

## Shooting method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

## Golden-section search

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An [optimization](mathematical-optimization.md) [algorithm](algorithm.md) that brackets an extremum of a unimodal [function](function.md) on an [interval](real-analysis.md#interval-mathematics). Two interior probes divide the bracket in the golden ratio; after discarding one side, one probe can be reused, so each subsequent contraction needs only one new [function](function.md) evaluation.

## Significant figures

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Significant_figures)

In [numerical analysis](numerical-analysis.md), [significant figures](#significant-figures) record how many meaningful digits are retained in a written numerical value. Leading zeros locate the decimal point rather than adding precision: $0.0079$ and $79$ each have two [significant figures](#significant-figures). Trailing zeros may require an explicit convention to distinguish measured precision from positional notation.

## Numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

A [numerical method](#numerical-method) is an [algorithm](algorithm.md) for computing an exact or approximate solution to a mathematical problem through finitely many [arithmetic operations](#arithmetic-operation) and other prescribed steps. For example, [Gaussian elimination](numerical-linear-algebra.md#gaussian-elimination) solves a [linear system](linear-algebra.md#system-of-linear-equations) exactly in exact arithmetic, whereas finite precision can introduce [roundoff error](#round-off-error).

### Velocity Verlet method

↑ **Parent:** [Numerical method](#numerical-method)

For an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) $\ddot x=f(x,t)$ with [acceleration](classical-mechanics.md#acceleration) independent of [velocity](classical-mechanics.md#velocity), the [velocity Verlet method](#velocity-verlet-method) advances [position](classical-mechanics.md#position) and [velocity](classical-mechanics.md#velocity) by

$$
a_n=f(x_n,t_n),\qquad x_{n+1}=x_n+h v_n+\frac{h^2}{2}a_n,\qquad
v_{n+1}=v_n+\frac h2\bigl(a_n+f(x_{n+1},t_n+h)\bigr).
$$

Here $h$ is the time step and $t_{n+1}=t_n+h$. For sufficiently smooth $f$, the [global error](#global-discretization-error) on a fixed time interval is $O(h^2)$, so halving $h$ reduces the leading [global error](#global-discretization-error) by a factor of four once the asymptotic regime is reached.

### Numerical algorithm

↑ **Parent:** [Numerical method](#numerical-method)

A [numerical algorithm](#numerical-algorithm) implements a [numerical method](#numerical-method) through specified finite computation steps, including [arithmetic operations](#arithmetic-operation) and any required [function evaluations](function.md#function-evaluation).

## Floating-point arithmetic

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](floating-point-arithmetic.md)

## Newton root-finding iteration

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The Newton root-finding iteration seeks a [zero of a function](polynomial.md#zero-of-a-function) $F$ by repeatedly solving its [tangent line](calculus.md#tangent-line) approximation. At a current guess $t_r$ with [derivative](calculus.md#derivative) $F'(t_r)\ne0$, set

$$
0=F(t_r)+F'(t_r)(t_{r+1}-t_r),\qquad t_{r+1}=t_r-\frac{F(t_r)}{F'(t_r)}.
$$

Geometrically, follow the [tangent line](calculus.md#tangent-line) to the horizontal axis, then return to the [function graph](function.md#graph-of-a-function) for the next [tangent line](calculus.md#tangent-line). Close to a suitable [zero of a function](polynomial.md#zero-of-a-function), the error becomes dramatically smaller.[Laurent Demanet, MIT 18.330, Chapter 4, §4.1, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/5b325bfa56a599794c7196de926844b0_MIT18_330S12_Chapter4.pdf)

For a concrete [square root](algebra.md#square-root) calculation, take the [polynomial](polynomial.md) $F(t)=t^2-2$ and start at $t_0=1$. The [Newton root-finding iteration](#newton-root-finding-iteration) becomes $t_{r+1}=(t_r+2/t_r)/2$, giving

$$
\begin{array}{c|c|c}
r&t_r&|t_r-\sqrt2|\\\hline
0&1&4.14214\times10^{-1}\\
1&1.5&8.57864\times10^{-2}\\
2&1.416666666667&2.45310\times10^{-3}\\
3&1.414215686275&2.12390\times10^{-6}\\
4&1.414213562375&1.59486\times10^{-12}
\end{array}
$$

The errors use the unrounded iterates. After the first step, each iterate overestimates $\sqrt2$, and the exact identity

$$
t_{r+1}-\sqrt2=\frac{(t_r-\sqrt2)^2}{2t_r}
$$

exhibits [quadratic convergence](#quadratic-convergence): once close, the number of correct decimal digits roughly doubles per step. This speed makes the [Newton root-finding iteration](#newton-root-finding-iteration) useful when accurate [derivatives](calculus.md#derivative) are available.

<a id="image-newton-tangent-steps-toward-a-square-root-and-a-nonconvergent-two-cycle"></a>
![](newton-root-iteration.png)

**[Figure 1](#image-newton-tangent-steps-toward-a-square-root-and-a-nonconvergent-two-cycle). Newton tangent steps toward a square root and a nonconvergent two-cycle**.

Global convergence requires additional care. For the [polynomial](polynomial.md) $F(x)=x^3-2x+2$, starting at $x_0=0$ gives $F(0)=2$, $F'(0)=-2$, hence $x_1=1$. Then $F(1)=1$, $F'(1)=1$ gives $x_2=0$. The sequence repeats $0,1,0,1,\ldots$ forever, although a real [polynomial root](polynomial.md#root-of-a-polynomial) lies in $(-2,-1)$ by the [intermediate value theorem](calculus.md#intermediate-value-theorem). Neither point in the cycle is a [zero of a function](polynomial.md#zero-of-a-function), and neither has zero [derivative](calculus.md#derivative). A maintained sign-changing interval and fallback [bisection method](#bisection-method) can protect a root solver from unsuitable Newton steps.

### Exact Newton error identity for a quadratic

↑ **Parent:** [Newton root-finding iteration](#newton-root-finding-iteration)

For the [quadratic polynomial](polynomial.md#quadratic-polynomial) $f(x)=(x-a)^2-b^2$ with $b>0$, consider the [Newton root-finding iteration](#newton-root-finding-iteration) towards the [polynomial root](polynomial.md#root-of-a-polynomial) $x_*=a+b$. If $x_k\ne a$, its signed error $e_k=x_k-x_*$ satisfies

$$
e_{k+1}=\frac{e_k^2}{2(x_k-a)}.
$$

Indeed the iteration for $u_k=x_k-a$ is $u_{k+1}=(u_k+b^2/u_k)/2$, and subtracting $b$ yields $(u_k-b)^2/(2u_k)$. This exact identity explains [quadratic convergence](#quadratic-convergence) near the simple [polynomial root](polynomial.md#root-of-a-polynomial). If an initial error is asymptotic to $C\varepsilon^m$ and $x_k-a\to b\ne0$ as $\varepsilon\to0$, one step changes its leading power to $2m$ and its coefficient to $C^2/(2b)$.

### Local quadratic convergence of Newton iteration

↑ **Parent:** [Newton root-finding iteration](#newton-root-finding-iteration)

Let $F$ be twice [continuously differentiable](multivariable-calculus.md#continuously-differentiable-function) on an interval around a [zero of a function](polynomial.md#zero-of-a-function) $t_*$, with $|F'(t)|\geq m>0$ and $|F''(t)|\leq M$ there. Choose a closed interval $[t_*-\rho,t_*+\rho]$ inside that interval with $M\rho/(2m)<1$. Starting inside it makes the [Newton root-finding iteration](#newton-root-finding-iteration) well defined, keeps it inside, and gives the displayed [quadratic convergence](#quadratic-convergence) bound for $e_r=t_r-t_*$. The nonzero [derivative](calculus.md#derivative) and sufficiently close start are essential hypotheses. The scalar estimate follows from the [Taylor remainder](calculus.md#taylor-remainder) argument in MIT's root-finding notes.[Laurent Demanet, MIT 18.330, Chapter 4, pp. 2–3, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/5b325bfa56a599794c7196de926844b0_MIT18_330S12_Chapter4.pdf)

For a short proof outline, apply [Taylor's theorem](calculus.md#taylor-s-theorem) between $t_r$ and $t_*$; subtract the defining [tangent line](calculus.md#tangent-line) equation. The linear error cancels, leaving $e_{r+1}=F''(\xi_r)e_r^2/(2F'(t_r))$. The displayed bound shrinks the error and preserves the chosen interval. If $F''(t_*)\ne0$, the error ratio tends to $|F''(t_*)/(2F'(t_*))|$; if it vanishes, convergence can be faster.

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

## Bracketing method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

A [bracketing method](#bracketing-method) finds a [zero of a function](polynomial.md#zero-of-a-function) by maintaining a [root bracket](#root-bracket) and shrinking it as new values of the [function](function.md) become available. The [bisection method](#bisection-method) always tries the [midpoint](convex-set.md#midpoint); its special attraction is a predictable [bisection error bound](#bisection-error-bound) without any [derivative](calculus.md#derivative) evaluations.

### Root bracket

↑ **Parent:** [Bracketing method](#bracketing-method)

A [root bracket](#root-bracket) is a [closed interval](real-analysis.md#closed-real-interval) known to contain at least one [zero of a function](polynomial.md#zero-of-a-function). For a real-valued [continuous function](calculus.md#continuous-function) on $[a,b]$, a strict change of sign between $f(a)$ and $f(b)$ certifies such an enclosure by the [intermediate value theorem](calculus.md#intermediate-value-theorem). An endpoint with value zero already supplies a [zero of a function](polynomial.md#zero-of-a-function). For example, $[1,2]$ is a [root bracket](#root-bracket) for the [polynomial](polynomial.md) $f(x)=x^2-2$, since $f(1)=-1$ and $f(2)=2$. A [root bracket](#root-bracket) need not contain a unique [zero of a function](polynomial.md#zero-of-a-function).

### Bisection method

↑ **Parent:** [Bracketing method](#bracketing-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bisection_method)

The [bisection method](#bisection-method) finds a [zero of a function](polynomial.md#zero-of-a-function) by repeatedly halving a [root bracket](#root-bracket). Let $f$ be a real-valued [continuous function](calculus.md#continuous-function) on the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$, with $a<b$. First check for endpoint [zeros of a function](polynomial.md#zero-of-a-function); otherwise require strictly opposite signs at the endpoints. Evaluate the [midpoint](convex-set.md#midpoint) and retain the half with strictly opposite endpoint signs, stopping immediately if the [midpoint](convex-set.md#midpoint) is a [zero of a function](polynomial.md#zero-of-a-function). The [intermediate value theorem](calculus.md#intermediate-value-theorem) ensures that every retained [root bracket](#root-bracket) still contains a [zero of a function](polynomial.md#zero-of-a-function). This is the construction in MIT's root-finding notes.[Laurent Demanet, MIT 18.330, Chapter 4, §4.1, pp. 1–2, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/5b325bfa56a599794c7196de926844b0_MIT18_330S12_Chapter4.pdf)

For a worked [square root](algebra.md#square-root) calculation, use the [polynomial](polynomial.md) $f(x)=x^2-2$ on $[1,2]$. Write $[a_k,b_k]$ for the [root bracket](#root-bracket) after $k$ halvings, with $[a_0,b_0]=[1,2]$. The candidate evaluated during update $k$ is the old [midpoint](convex-set.md#midpoint) $m_{k-1}$:

$$
\begin{array}{c|c|r|c}
\text{update }k&\text{candidate }m_{k-1}&f(m_{k-1})&\text{retained }[a_k,b_k]\\\hline
1&1.5&0.25&[1,1.5]\\
2&1.25&-0.4375&[1.25,1.5]\\
3&1.375&-0.109375&[1.375,1.5]\\
4&1.4375&0.06640625&[1.375,1.4375]
\end{array}
$$

The initial [midpoint](convex-set.md#midpoint) is $m_0=1.5$. After four halvings the new [midpoint](convex-set.md#midpoint) is $m_4=1.40625$, and the [bisection error bound](#bisection-error-bound) is $|m_4-\sqrt2|\leq0.03125$. Its actual error is approximately $0.00796356237310$. The last tested candidate $m_3=1.4375$ and the reported [midpoint](convex-set.md#midpoint) $m_4$ are different points.

<a id="image-bisection-of-a-square-root-bracket-the-graph-and-first-four-retained-intervals"></a>
![](bisection-root-brackets.png)

**[Figure 2](#image-bisection-of-a-square-root-bracket-the-graph-and-first-four-retained-intervals). Bisection of a square-root bracket: the graph and first four retained intervals**.

The useful feature of the [bisection method](#bisection-method) is that the retained width halves on every update, independently of the shape of the [function graph](function.md#graph-of-a-function). The [bisection error bound](#bisection-error-bound) therefore supplies an accuracy guarantee before the [zero of a function](polynomial.md#zero-of-a-function) is known. No [derivative](calculus.md#derivative) is needed, and a valid initial [root bracket](#root-bracket) gives convergence without a close initial guess. This makes the [bisection method](#bisection-method) a dependable fallback for the faster [Newton root-finding iteration](#newton-root-finding-iteration).

#### Bisection error bound

↑ **Parent:** [Bisection method](#bisection-method)

In exact arithmetic, after $k$ completed halvings the retained [root bracket](#root-bracket) has width $W_k=b_k-a_k$ and [midpoint](convex-set.md#midpoint) $m_k$, where

$$
W_k=\frac{b-a}{2^k},\qquad m_k=\frac{a_k+b_k}{2},\qquad |m_k-x_*|\leq\frac{W_k}{2}=\frac{b-a}{2^{k+1}}.
$$

The [absolute value](real-analysis.md#absolute-value) bound holds for every [zero of a function](polynomial.md#zero-of-a-function) $x_*$ in the current [root bracket](#root-bracket), including the one approached by continued [bisection method](#bisection-method) updates. A [zero of a function](polynomial.md#zero-of-a-function) discarded with an earlier half need not satisfy later bounds. Before update $k\geq1$, the evaluated candidate is $m_{k-1}$, whose corresponding guarantee is $(b-a)/2^k$. After update $k$, the new [midpoint](convex-set.md#midpoint) $m_k$ has the smaller guarantee $(b-a)/2^{k+1}$, even without evaluating $f(m_k)$.

<a id="image-bisection-widths-midpoint-error-bounds-and-actual-square-root-errors-after-zero-to-fifteen-halvings"></a>
![](bisection-error-halving.png)

**[Figure 3](#image-bisection-widths-midpoint-error-bounds-and-actual-square-root-errors-after-zero-to-fifteen-halvings). Bisection widths, midpoint error bounds, and actual square-root errors after zero to fifteen halvings**.

The guaranteed error halves at every step; the actual [absolute value](real-analysis.md#absolute-value) error need not decrease at every step or have successive ratio $1/2$. In the [square root](algebra.md#square-root) example it increases from $|m_6-\sqrt2|\approx0.000151062$ to $|m_7-\sqrt2|\approx0.003755188$, while both errors remain below their guarantees. An exact [midpoint](convex-set.md#midpoint) [zero of a function](polynomial.md#zero-of-a-function) instead gives zero error and immediate termination. For this example $\sqrt2$ is an [irrational number](algebra.md#irrational-number), so no finite exact halving can produce it as a [midpoint](convex-set.md#midpoint).

For a brief proof outline, each retained half has half the previous width and contains a [zero of a function](polynomial.md#zero-of-a-function) by the [intermediate value theorem](calculus.md#intermediate-value-theorem). Every point in the retained [root bracket](#root-bracket) is at most half its width from its [midpoint](convex-set.md#midpoint). If the process does not stop at a [zero of a function](polynomial.md#zero-of-a-function), the [nested interval theorem](real-analysis.md#nested-interval-theorem) gives one common point as the widths tend to zero; [continuity](calculus.md#continuous-function) and the opposite endpoint signs force its [function](function.md) value to be zero. Uniqueness in the initial [root bracket](#root-bracket) is unnecessary.

#### Bisection stopping criterion

↑ **Parent:** [Bisection method](#bisection-method)

For a requested absolute tolerance $\varepsilon>0$, stop when the retained [root bracket](#root-bracket) has width at most $2\varepsilon$, and report its [midpoint](convex-set.md#midpoint). The [bisection error bound](#bisection-error-bound) then guarantees $|m_k-x_*|\leq\varepsilon$ in exact arithmetic. Using the [ceiling function](calculus.md#ceiling-function) and the base-two [logarithm](calculus.md#logarithm), the required number of halvings is

$$
k_{\min}=\max\left\{0,\left\lceil\log_2\frac{b-a}{2\varepsilon}\right\rceil\right\}.
$$

The zero allows stopping before any update when the initial [root bracket](#root-bracket) is already sufficiently narrow. For the [polynomial](polynomial.md) $f(x)=x^2-2$ on $[1,2]$ with $\varepsilon=10^{-3}$, $k_{\min}=\lceil\log_2 500\rceil=9$. After nine halvings,

$$
[a_9,b_9]=[1.4140625,1.416015625],\qquad m_9=1.4150390625,\qquad \frac{W_9}{2}=\frac{1}{1024}=0.0009765625.
$$

Thus the reported [midpoint](convex-set.md#midpoint) meets the tolerance; its actual error from the [square root](algebra.md#square-root) $\sqrt2$ is approximately $0.000825500126905$. After eight halvings the bound is $1/512>10^{-3}$, so eight do not give this worst-case guarantee.

Cache the endpoint values. Each update of the [bisection method](#bisection-method) needs just one new [function](function.md) evaluation, at the old [midpoint](convex-set.md#midpoint). With no early [zero of a function](polynomial.md#zero-of-a-function), $k$ updates therefore cost $k+2$ [function](function.md) evaluations, including the two initial endpoints. Returning the new [midpoint](convex-set.md#midpoint) requires no additional [function](function.md) evaluation; requesting its value would add one. The nine-update example needs eleven evaluations for the guarantee.

A small [function](function.md) value $|f(m_k)|$ alone does not guarantee a small position error: rescaling $f$ changes those values without changing its [zeros of a function](polynomial.md#zero-of-a-function). In a practical implementation, use an explicit width test and an iteration limit. With [floating-point arithmetic](floating-point-arithmetic.md), also stop if the computed [midpoint](convex-set.md#midpoint) equals either endpoint: the [root bracket](#root-bracket) can no longer shrink, so repeating the update would loop forever. Report this precision limit separately if the requested tolerance remains unmet. Reliable sign evaluations are needed to preserve the [root bracket](#root-bracket); compare signs directly rather than multiplying endpoint values, which can suffer overflow or underflow in [floating-point arithmetic](floating-point-arithmetic.md).

For a rounded [midpoint](convex-set.md#midpoint) $m$ still inside a valid [root bracket](#root-bracket), the geometric error bound is $\max\{m-a_k,b_k-m\}$; it need not equal $W_k/2$ because of [roundoff error](#round-off-error). A rigorous computed enclosure also needs conservative arithmetic for that bound and reliable endpoint signs. The exact-arithmetic [bisection error bound](#bisection-error-bound) should not be claimed unchanged after precision prevents further halving.

For practical tolerance conventions, SciPy's `bisect` combines absolute and relative tolerances through $|x-x_0|\leq\mathrm{xtol}+\mathrm{rtol}|x_0|$, and provides a maximum iteration count and convergence status. These differ from the purely absolute width test above.[SciPy, scipy.optimize.bisect documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.bisect.html)

#### Limitations of bisection

↑ **Parent:** [Bisection method](#bisection-method)

Several [zeros of a function](polynomial.md#zero-of-a-function) can lie in one initial [root bracket](#root-bracket): the [bisection method](#bisection-method) seeks one, rather than enumerating them. For instance, the [polynomial](polynomial.md) $(x-1)(x-2)(x-3)$ has opposite endpoint signs on $[0,4]$, but its first [midpoint](convex-set.md#midpoint) evaluation returns only the [polynomial root](polynomial.md#root-of-a-polynomial) $2$. The initial [zero of a function](polynomial.md#zero-of-a-function) need not be unique for the [bisection error bound](#bisection-error-bound) to apply to a retained [zero of a function](polynomial.md#zero-of-a-function).

A [zero of a function](polynomial.md#zero-of-a-function) without a sign change cannot be located by the strict sign-change test alone. The [polynomial](polynomial.md) $(x-1)^2$ touches zero at $1$ but is positive on either side. On $[0,3]$ both endpoint values are positive: although the [closed interval](real-analysis.md#closed-real-interval) contains a [polynomial root](polynomial.md#root-of-a-polynomial), it fails the usual starting test for the [bisection method](#bisection-method). An endpoint or evaluated [midpoint](convex-set.md#midpoint) [zero of a function](polynomial.md#zero-of-a-function) can still be recognized directly.

Opposite signs certify a [root bracket](#root-bracket) only with the required [continuity](calculus.md#continuous-function). For $f(x)=1/x$, the values at $-1$ and $1$ have opposite signs, but $f$ is undefined at the [midpoint](convex-set.md#midpoint) $0$ and has no [zero of a function](polynomial.md#zero-of-a-function). Hence $[-1,1]$ is invalid input for the [bisection method](#bisection-method); the [intermediate value theorem](calculus.md#intermediate-value-theorem) does not apply across the gap.

## Chord error bound

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

If a twice differentiable [parametric curve](topology.md#parametric-curve) $R:[a,b]\to\mathbb R^m$ satisfies $\lVert R''\rVert\le M$, its deviation from the linearly parameterized chord is at most $M(b-a)^2/8$. This follows from the Green function for the second derivative with zero endpoint values. It bounds the [Hausdorff distance](topological-analysis.md#hausdorff-distance) between the arc and its chord.

// Target: analysis.bigb

## Interval arithmetic

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interval_arithmetic)

[Interval arithmetic](#interval-arithmetic) calculates with [closed intervals](real-analysis.md#closed-real-interval) that contain the possible values of a quantity. If all we know is $x\in X=[a,b]$, an [interval enclosure](#interval-enclosure) for a [function](function.md) $f$ must contain $f(x)$ for every allowed $x$. The result says what is guaranteed, including uncertainty in the input and, with [outward rounding](#outward-rounding), [roundoff error](#round-off-error) in the calculation. A wide answer can still be correct; a narrow answer is useful only if it contains every possible value.

The attraction is that a finite calculation can make a statement about infinitely many [real numbers](arithmetic.md#real-number) at once. An [interval enclosure](#interval-enclosure) can certify that a [function](function.md) stays positive throughout a whole [closed interval](real-analysis.md#closed-real-interval), or bound its [maximum](set.md#maximum-of-a-subset-of-a-total-order) for [mathematical optimization](mathematical-optimization.md). For example, on $X=[0,1]$, the actual [image of a function](set-theory.md#image-of-a-function) for $f(x)=x(1-x)$ is $[0,1/4]$, but direct [interval arithmetic](#interval-arithmetic) gives the wider $[0,1]$. [Interval subdivision](#interval-subdivision) and the [interval square range](#interval-square-range) improve this answer in different ways.

Historically, Ramon E. Moore's 1962 Stanford dissertation studied [interval arithmetic](#interval-arithmetic) and automatic error analysis in digital computing; his book _Interval Analysis_ followed in 1966. Eldon Hansen's account documents earlier reports as well: these dates describe important steps in developing and disseminating the subject, rather than a claim of sole invention in a particular year.[Eldon R. Hansen, Publications Related to Early Interval Work of R. E. Moore, 2001, references 5 and 8](https://interval.louisiana.edu/Moores_early_papers/bibliography.html) Moore, R. Baker Kearfott and Michael J. Cloud later wrote _Introduction to Interval Analysis_ (2009).[R. Baker Kearfott, Books written or edited, entry for Introduction to Interval Analysis](https://interval.louisiana.edu/books.html)

### Interval enclosure

↑ **Parent:** [Interval arithmetic](#interval-arithmetic)

An [interval enclosure](#interval-enclosure) $F(X)=[L,U]$ for a real-valued [function](function.md) $f$ on a [closed interval](real-analysis.md#closed-real-interval) $X$ satisfies

$$
L\leq f(x)\leq U\quad\text{for every }x\in X,\qquad f(X):=\{f(x):x\in X\}\subseteq F(X).
$$

Here $f(X)$ means the actual [image of a function](set-theory.md#image-of-a-function), also called its pointwise range on $X$; $F(X)$ denotes a calculated [interval enclosure](#interval-enclosure). They need not agree. Sampling a few inputs can suggest a bound, but does not establish an [interval enclosure](#interval-enclosure) between those inputs. Kearfott and coauthors explicitly distinguish the [image of a function](set-theory.md#image-of-a-function) from evaluating an expression with [interval arithmetic](#interval-arithmetic), because different expressions for the same [function](function.md) can give different bounds.[Kearfott, Nakao, Neumaier, Rump, Shary and Van Hentenryck, Standardized notation in interval analysis, 2010, Arithmetic expressions and Intervals and boxes](https://www.tuhh.de/ti3/paper/rump/KeNaNeRuShHe10.pdf)

### Interval arithmetic operations

↑ **Parent:** [Interval arithmetic](#interval-arithmetic)

For [closed intervals](real-analysis.md#closed-real-interval) $X=[a,b]$ and $Y=[c,d]$, exact [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction) and [multiplication](arithmetic.md#multiplication) give

$$
\begin{aligned}
X+Y&=[a+c,b+d],\\
X-Y&=[a-d,b-c],\\
XY&=[\min\{ac,ad,bc,bd\},\max\{ac,ad,bc,bd\}].
\end{aligned}
$$

These [interval arithmetic operations](#interval-arithmetic-operations) describe all results $u\mathbin{\circ}v$ for $(u,v)$ in the [Cartesian product](set-theory.md#cartesian-product) $X\times Y$: the two inputs are allowed to vary independently. Independence here means freedom to choose either input anywhere in its [closed interval](real-analysis.md#closed-real-interval); it does not assert anything about [probability](probability-theory.md#probability). For example, $[1,2]+[3,5]=[4,7]$ and $[1,2]-[3,5]=[-4,-1]$.

All four endpoint [products](arithmetic.md#product-of-numbers) matter when signs change. For $X=[-2,3]$ and $Y=[-4,1]$, the endpoint [products](arithmetic.md#product-of-numbers) are $8,-2,-12,3$, so $XY=[-12,8]$. Taking just $ac$ and $bd$, even after sorting them, would give $[3,8]$ and lose valid negative [products](arithmetic.md#product-of-numbers).

For [division](arithmetic.md#division-mathematics), if $0\notin Y$, the [multiplicative inverse](arithmetic.md#multiplicative-inverse) gives $1/Y=[1/d,1/c]$ and $X/Y=X(1/Y)$. Thus $[1,2]/[3,4]=[1/4,2/3]$. This ordinary finite-[closed interval](real-analysis.md#closed-real-interval) rule requires a [denominator](number-theory.md#denominator) that excludes zero. When the [denominator](number-theory.md#denominator) contains zero, [division](arithmetic.md#division-mathematics) is undefined for some pairs and can become unbounded near zero; these formulas cannot supply a finite [interval enclosure](#interval-enclosure) of all quotients. The operations above use exact endpoints; a computer implementation must also apply [outward rounding](#outward-rounding).

#### Natural interval extension

↑ **Parent:** [Interval arithmetic operations](#interval-arithmetic-operations)

A [natural interval extension](#natural-interval-extension) evaluates a chosen expression by replacing its [arithmetic operations](#arithmetic-operation) with [interval arithmetic operations](#interval-arithmetic-operations), its [constants](mathematics.md#constant-mathematics) with enclosing [closed intervals](real-analysis.md#closed-real-interval), and any additional [functions](function.md) with valid [interval enclosures](#interval-enclosure). Each intermediate result must remain defined on its inputs. The resulting $F(X)$ encloses the actual [image of a function](set-theory.md#image-of-a-function) $f(X)$, but its width depends on the expression used. Rump's INTLAB tutorial describes this inclusion principle and warns that repeated inputs can produce severe overestimation.[Siegfried M. Rump, Interval computations in INTLAB, Overestimation of interval operations and A common misuse of interval arithmetic](https://www.tuhh.de/ti3/rump/intlab/demos/html/dintval.html)

##### Interval dependency problem

↑ **Parent:** [Natural interval extension](#natural-interval-extension)

The [interval dependency problem](#interval-dependency-problem) is the loss of relationships between repeated occurrences of the same input. For $X=[0,1]$, interval [subtraction](arithmetic.md#subtraction) gives $X-X=[-1,1]$: it permits $u-v$ with independent choices $u,v\in X$. But the [function](function.md) $x\mapsto x-x$ has actual [image of a function](set-theory.md#image-of-a-function) $\{0\}=[0,0]$. Giving both operands the name $X$ does not tell an [interval arithmetic](#interval-arithmetic) calculation to enforce $u=v$.

For the [polynomial](polynomial.md) $f(x)=x(1-x)$ on $X=[0,1]$, the [natural interval extension](#natural-interval-extension) is

$$
F(X)=X([1,1]-X)=[0,1][0,1]=[0,1].
$$

This allows the impossible combination $x=1$ in the first factor and $x=0$ in the second, producing the spurious upper bound $1$. In the actual [function](function.md), both occurrences use the same $x$. [Completing the square](polynomial.md#completing-the-square) gives $x(1-x)=1/4-(x-1/2)^2$, which lies between $0$ and $1/4$ on $[0,1]$; every value between these bounds occurs, by [continuity](calculus.md#continuous-function) and the [intermediate value theorem](calculus.md#intermediate-value-theorem). The [maximum](set.md#maximum-of-a-subset-of-a-total-order) $1/4$ occurs at $x=1/2$, while either endpoint gives the [minimum](set.md#minimum-of-a-subset-of-a-total-order) $0$.

<a id="image-independent-interval-inputs-lose-the-diagonal-constraint-subdivision-tightens-the-enclosure-of-x-times-one-minus-x"></a>
![](interval-dependency-and-subdivision.png)

**[Figure 4](#image-independent-interval-inputs-lose-the-diagonal-constraint-subdivision-tightens-the-enclosure-of-x-times-one-minus-x). Independent interval inputs lose the diagonal constraint; subdivision tightens the enclosure of x times one minus x**. Left: the [Cartesian product](set-theory.md#cartesian-product) permits separate choices $u,v\in[0,1]$, while the actual [function](function.md) uses only $u=v$. Right: rectangles from four pieces contain the [polynomial](polynomial.md) curve. Below: one, two and four pieces give [interval enclosures](#interval-enclosure) with upper bounds $1$, $1/2$ and $3/8$; the [interval square range](#interval-square-range) gives the exact $1/4$.

###### Interval subdivision

↑ **Parent:** [Interval dependency problem](#interval-dependency-problem)

[Interval subdivision](#interval-subdivision) covers $X$ by smaller [closed intervals](real-analysis.md#closed-real-interval) $X_j$, computes a valid [interval enclosure](#interval-enclosure) $F(X_j)$ on each, and takes their [union](set.md#set-union). Every allowed input belongs to a piece, so its output belongs to that [union](set.md#set-union). If one [closed interval](real-analysis.md#closed-real-interval) is wanted, take the smallest one containing the [union](set.md#set-union); gaps between separate output pieces can then be lost. Splitting narrows the freedom given to repeated inputs, while increasing the number of evaluations.

For $f(x)=x(1-x)$, split $[0,1]$ at $1/2$. The [natural interval extensions](#natural-interval-extension) are

$$
\begin{aligned}
F([0,1/2])&=[0,1/2][1/2,1]=[0,1/2],\\
F([1/2,1])&=[1/2,1][0,1/2]=[0,1/2].
\end{aligned}
$$

Their [union](set.md#set-union) is $[0,1/2]$. Four equal pieces sharpen the upper bound again:

$$
\begin{array}{c|c|c}
X_j&[1,1]-X_j&F(X_j)\\\hline
[0,1/4]&[3/4,1]&[0,1/4]\\
[1/4,1/2]&[1/2,3/4]&[1/8,3/8]\\
[1/2,3/4]&[1/4,1/2]&[1/8,3/8]\\
[3/4,1]&[0,1/4]&[0,1/4]
\end{array}
$$

The [union](set.md#set-union) is now $[0,3/8]=[0,0.375]$, still wider than the actual [image of a function](set-theory.md#image-of-a-function) $[0,1/4]$. These are exact [rational number](number-theory.md#rational-number) bounds: the excess width comes from the [interval dependency problem](#interval-dependency-problem), rather than [roundoff error](#round-off-error).

#### Interval square range

↑ **Parent:** [Interval arithmetic operations](#interval-arithmetic-operations)

The [interval square range](#interval-square-range) treats squaring as one [function](function.md) of one input. For $X=[a,b]$ it is exactly

$$
\operatorname{sqr}([a,b])=
\begin{cases}
[0,\max\{a^2,b^2\}],&a\leq0\leq b,\\
[\min\{a^2,b^2\},\max\{a^2,b^2\}],&\text{otherwise}.
\end{cases}
$$

It retains the relationship that ordinary interval [multiplication](arithmetic.md#multiplication) loses: for $Z=[-1/2,1/2]$, the [interval square range](#interval-square-range) is $[0,1/4]$, whereas the independent-input [product](arithmetic.md#product-of-numbers) $ZZ$ is $[-1/4,1/4]$.

Consequently, [completing the square](polynomial.md#completing-the-square) for $x(1-x)$ and using the [interval square range](#interval-square-range) gives

$$
Z=X-[1/2,1/2]=[-1/2,1/2],\qquad [1/4,1/4]-\operatorname{sqr}(Z)=[0,1/4].
$$

This is the exact [image of a function](set-theory.md#image-of-a-function) on $X=[0,1]$. Merely rewriting the expression and evaluating $[1/4,1/4]-ZZ$ gives $[0,1/2]$, so it does not achieve the same sharpening. A mathematical $Z^2$ must be interpreted explicitly here: a [square range operation](#interval-square-range) and an independent-input interval [product](arithmetic.md#product-of-numbers) have different meanings. Choosing an operation that preserves known structure can save many steps of [interval subdivision](#interval-subdivision).

### Outward rounding

↑ **Parent:** [Interval arithmetic](#interval-arithmetic)

[Outward rounding](#outward-rounding) replaces an exact lower endpoint by a representable value no larger than it, and an exact upper endpoint by a representable value no smaller than it. This preserves an [interval enclosure](#interval-enclosure) under [floating-point arithmetic](floating-point-arithmetic.md). In the [binary numeral system](integer.md#binary-numeral-system), most [rational numbers](number-theory.md#rational-number) cannot be represented exactly with finitely many digits, so the rounding direction is essential even for elementary calculations. Rump explains directed rounding and its use in interval bounds in §§4 and 5.3 of his survey.[Siegfried M. Rump, Verification methods: rigorous results using floating-point arithmetic, Acta Numerica 19, 287–449, 2010, §§4 and 5.3](https://www.tuhh.de/ti3/paper/rump/Ru10.pdf)

To see the issue without long binary digit strings, use an illustrative decimal grid with step $0.001$. Exact interval [division](arithmetic.md#division-mathematics) gives $[1,1]/[3,3]=[1/3,1/3]$. Rounding both endpoints to the nearest grid value gives $[0.333,0.333]$, which excludes the true answer because $0.333<1/3$. [Outward rounding](#outward-rounding) instead gives

$$
\left[\frac{333}{1000},\frac{334}{1000}\right]=[0.333,0.334],\qquad \frac{333}{1000}<\frac13<\frac{334}{1000}.
$$

This decimal toy illustrates the rule; its displayed endpoints are not the results of binary directed rounding. Real implementations need valid [outward rounding](#outward-rounding) throughout the calculation, including input conversion and intermediate [interval arithmetic operations](#interval-arithmetic-operations); rounding only the final output cannot repair an earlier lost bound. INTLAB's tutorial demonstrates why decimal input strings and previously rounded intermediate values need care.[Rump, Interval computations in INTLAB, How to define an interval II and Invoking interval operations](https://www.tuhh.de/ti3/rump/intlab/demos/html/dintval.html)

<a id="image-outward-rounding-encloses-one-third-on-a-decimal-toy-grid-sign-changing-interval-products-require-all-four-endpoint-combinations"></a>
![](interval-rounding-enclosures.png)

**[Figure 5](#image-outward-rounding-encloses-one-third-on-a-decimal-toy-grid-sign-changing-interval-products-require-all-four-endpoint-combinations). Outward rounding encloses one third on a decimal toy grid; sign-changing interval products require all four endpoint combinations**. Above: rounding to the nearest decimal grid point misses $1/3$, while down to $0.333$ and up to $0.334$ enclose it. Below: the [Cartesian product](set-theory.md#cartesian-product) of $[-2,3]$ and $[-4,1]$ has endpoint [products](arithmetic.md#product-of-numbers) $8,-2,-12,3$, giving $[-12,8]$. The two same-side endpoint [products](arithmetic.md#product-of-numbers) alone give the invalid enclosure $[3,8]$.

### Interval root exclusion

↑ **Parent:** [Interval arithmetic](#interval-arithmetic)

[Interval root exclusion](#interval-root-exclusion) certifies that a [function](function.md) has no [zero of a function](polynomial.md#zero-of-a-function) on $X$ when a valid [interval enclosure](#interval-enclosure) $F(X)$ excludes zero. For $g(x)=x(1-x)-1/3$ on $[0,1]$, the [interval square range](#interval-square-range) yields $G(X)=[-1/3,-1/12]$, which excludes zero. Direct [interval arithmetic](#interval-arithmetic) yields $[-1/3,2/3]$ and is inconclusive, even though the [function](function.md) has no [zero of a function](polynomial.md#zero-of-a-function) there.

Knowing only that a calculated [interval enclosure](#interval-enclosure) contains zero does not certify a [zero of a function](polynomial.md#zero-of-a-function): it may contain unattainable values. Even the positive [constant function](function.md#constant-function) $f(x)=1$ has a valid, loose [interval enclosure](#interval-enclosure) $[-1,2]$. A separate existence argument, such as reliable opposite endpoint signs together with [continuity](calculus.md#continuous-function) in the [intermediate value theorem](calculus.md#intermediate-value-theorem), is required; see [root bracket](#root-bracket) and [bisection method](#bisection-method). [Interval subdivision](#interval-subdivision) can resolve some inconclusive pieces, but remaining pieces must be reported as unresolved unless an existence argument succeeds. This makes [interval root exclusion](#interval-root-exclusion) useful for systematically discarding regions in a search.

// Target: analysis.bigb

## Continuation method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuation_method)

A [continuation method](#continuation-method) follows a [solution branch](#solution-branch) of a parameter-dependent equation from a known solution, using nearby solutions to guide the next solve. This is useful when one wants to understand how solutions change, rather than obtain just one isolated answer. A [continuation predictor-corrector step](#continuation-predictor-corrector-step) follows a [tangent vector](tangent-vector.md) and then uses a [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) correction on a transverse section. The same geometry supports both [pseudo-arclength continuation](#pseudo-arclength-continuation) through a [continuation fold](#fold-of-a-solution-branch) and [transversal surface intersection tracing](#transversal-surface-intersection-tracing).

Consider the original scalar [polynomial](polynomial.md) example

$$
F(x,\lambda)=x^3-x+\lambda=0,\qquad \lambda=x-x^3.
$$

Its [solution branch](#solution-branch) bends back twice in $\lambda$. Increasing $\lambda$ alone eventually stops following the same nearby solutions; following the [curve](topology.md#curve) in the $(x,\lambda)$ plane can continue around both bends. The [continuation folds](#fold-of-a-solution-branch) are

$$
(x_-,\lambda_-)=\left(-\frac1{\sqrt3},-\frac2{3\sqrt3}\right),\qquad
(x_+,\lambda_+)=\left(\frac1{\sqrt3},\frac2{3\sqrt3}\right).
$$

For $|\lambda|<2/(3\sqrt3)$ there are three distinct real [zeros of a function](polynomial.md#zero-of-a-function) at that fixed $\lambda$, all lying on this one connected [curve](topology.md#curve). A [continuation method](#continuation-method) keeps their geometric relationship visible.

<a id="image-a-connected-cubic-solution-curve-with-two-folds-and-three-solutions-at-the-same-parameter-value"></a>
![](continuation-cubic-solution-curve-folds.png)

**[Figure 6](#image-a-connected-cubic-solution-curve-with-two-folds-and-three-solutions-at-the-same-parameter-value). A connected cubic solution curve with two folds and three solutions at the same parameter value**. The arrows follow increasing $x$ along $\lambda=x-x^3$, even where $\lambda$ changes direction. The dashed horizontal line $\lambda=0.2$ meets the [solution branch](#solution-branch) three times. The marked [continuation folds](#fold-of-a-solution-branch) are extrema of $\lambda$, not singularities of the full [curve](topology.md#curve).

Every [continuation method](#continuation-method) needs a seed, supplied by an independent solve, an explicitly known solution, or another search. Following one [solution branch](#solution-branch) does not guarantee finding every [connected component](geometry-and-topology.md#connected-component) of the solution set. A large step can miss detail or make the correction converge to a distant solution. At branch intersections or a loss of [rank](quadratic-form.md#rank-one-quadratic-form) of the full [Jacobian matrix](multivariable-calculus.md#jacobian-matrix), the regular-[curve](topology.md#curve) argument needs separate analysis. The seed and component limitations also matter in [transversal surface intersection tracing](#transversal-surface-intersection-tracing).

### Solution branch

↑ **Parent:** [Continuation method](#continuation-method)

A [solution branch](#solution-branch) is a portion of a solution set followed continuously as a [curve](topology.md#curve). For $F(u,\lambda)=0$ with $u\in\mathbb R^n$, a full [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) $[F_u\ F_\lambda]$ of [rank](quadratic-form.md#rank-one-quadratic-form) $n$ makes the nearby solution set a one-dimensional [regular level set](topology.md#regular-level-set). It need not be a [graph of a function](function.md#graph-of-a-function) $u(\lambda)$: a [continuation fold](#fold-of-a-solution-branch) can obstruct that particular choice of parameter while leaving the [solution branch](#solution-branch) regular.

### Parameter continuation

↑ **Parent:** [Continuation method](#continuation-method)

[Parameter continuation](#parameter-continuation) changes $\lambda$ by a small amount and solves again for $u$, using the previous solution as the initial guess for [Newton method](mathematical-optimization.md#newton-s-method-in-optimization). If $F_u$ is an [invertible matrix](linear-algebra.md#invertible-matrix), the [implicit function theorem](multivariable-calculus.md#implicit-function-theorem) gives a local [solution branch](#solution-branch) $u(\lambda)$, with

$$
\frac{du}{d\lambda}=-F_u^{-1}F_\lambda.
$$

Local convergence of [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) also needs regularity and a sufficiently small step: the cited result assumes a [Lipschitz continuous](real-analysis.md#lipschitz-continuity) [derivative](calculus.md#derivative) and an invertible $F_u$ at the seed.[§2.1, Corollary 2.1, printed pp. 264–265: Lipschitz continuously differentiable map, nonsingular state Jacobian, and a sufficiently small parameter increment](mathematics-bibliography.md#condition-estimates-for-pseudo-arclength-continuation-by-k-i-dickson-and-others)

For the cubic [polynomial](polynomial.md),

$$
F_x=3x^2-1,\qquad F_\lambda=1,\qquad \frac{dx}{d\lambda}=\frac1{1-3x^2}.
$$

The [derivative](calculus.md#derivative) becomes unbounded at either [continuation fold](#fold-of-a-solution-branch), and the scalar [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) divides by $F_x=0$ there. Just beyond the upper [continuation fold](#fold-of-a-solution-branch), no nearby real solution exists at the increased $\lambda$, although a distant negative-$x$ solution still exists. Converging to that solution would jump away from the local [solution branch](#solution-branch). Decreasing the parameter step cannot make $x(\lambda)$ a valid smooth local description at the bend.

### Fold of a solution branch

↑ **Parent:** [Continuation method](#continuation-method)

A nondegenerate [fold of a solution branch](#fold-of-a-solution-branch) in a smooth scalar equation satisfies the displayed conditions. The [implicit function theorem](multivariable-calculus.md#implicit-function-theorem) still gives $\lambda=\lambda(x)$ because $F_\lambda\ne0$. [Implicit differentiation](multivariable-calculus.md#implicit-differentiation) gives $\lambda'(x_*)=0$ and $\lambda''(x_*)=-F_{xx}/F_\lambda\ne0$: the parameter has a genuine local extremum on the [curve](topology.md#curve).

In the cubic [polynomial](polynomial.md), $F_x=0$ gives $x_*=\pm1/\sqrt3$, and substituting into $F=0$ gives $\lambda_*=2x_*/3$. Furthermore, $F_{xx}=6x_*\ne0$. Yet $\nabla F=(3x^2-1,1)$ never vanishes, so the full [solution branch](#solution-branch) remains a [regular level set](topology.md#regular-level-set) everywhere. The obstruction belongs to the projection onto $\lambda$, not to the [curve](topology.md#curve) itself.

For systems, the cited continuation account uses a one-dimensional [kernel](kernel-of-a-linear-map.md) of $F_u$ and $F_\lambda$ outside its [image of a linear map](vector-space.md#image-of-a-linear-map) to define a simple fold (its Definition 2.2). These conditions make $[F_u\ F_\lambda]$ have full [rank](quadratic-form.md#rank-one-quadratic-form) and support a transverse correction. A nonzero second-order term along the [kernel](kernel-of-a-linear-map.md) is additionally needed to describe a nondegenerate quadratic turning point; in the scalar example this is $F_{xx}\ne0$.[§2.2, Definition 2.2, printed p. 265: one-dimensional kernel of the state Jacobian and parameter derivative outside its range](mathematics-bibliography.md#condition-estimates-for-pseudo-arclength-continuation-by-k-i-dickson-and-others)

### Pseudo-arclength continuation

↑ **Parent:** [Continuation method](#continuation-method)

[Pseudo-arclength continuation](#pseudo-arclength-continuation) allows both the state and the parameter to change. Write $z=(u,\lambda)$ and choose a [unit vector](vector-space.md#unit-vector) $t_k$ in the [kernel](kernel-of-a-linear-map.md) of the full [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) $DF(z_k)$. A [continuation predictor-corrector step](#continuation-predictor-corrector-step) seeks the next solution on a [hyperplane](vector-space.md#hyperplane) perpendicular to $t_k$, a distance $h>0$ along the old [tangent vector](tangent-vector.md). This adds one equation to $F(z)=0$ and makes the correction a square system. The constraint approximates [arc length](riemannian-geometry.md#arc-length); $h$ is the displacement projected onto the old [tangent vector](tangent-vector.md), rather than the exact curved distance.[§2.2, equations (2.2)–(2.5), printed pp. 265–266: unit tangent and hyperplane normalization; Corollary 2.3 gives local Newton convergence for sufficiently small steps](mathematics-bibliography.md#condition-estimates-for-pseudo-arclength-continuation-by-k-i-dickson-and-others)

#### Continuation predictor-corrector step

↑ **Parent:** [Pseudo-arclength continuation](#pseudo-arclength-continuation)

For the cubic [polynomial](polynomial.md), an oriented, normalized [tangent vector](tangent-vector.md) is

$$
t_k=\frac{(1,\ 1-3x_k^2)}{\sqrt{1+(1-3x_k^2)^2}}.
$$

Its [Euclidean norm](normed-vector-space.md#euclidean-norm) is one and $DF(z_k)t_k=0$. The sign here follows increasing $x$; for a general [solution branch](#solution-branch), choose the sign of each new [tangent vector](tangent-vector.md) so its [dot product](inner-product.md#dot-product) with the previous one is positive. First predict $z_{\mathrm p}=z_k+h t_k$, then apply [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) starting at $z_{\mathrm p}$ to

$$
H(z)=\begin{pmatrix}F(z)\\t_k^{\mathsf T}(z-z_{\mathrm p})\end{pmatrix}=0,\qquad
DH(z)=\begin{pmatrix}3x^2-1&1\\t_{k,x}&t_{k,\lambda}\end{pmatrix}.
$$

The second equation keeps the correction on the transverse line in this two-dimensional example; in higher dimensions it is a [hyperplane](vector-space.md#hyperplane). Solving the [linear system](linear-algebra.md#system-of-linear-equations) $DH(z^{(j)})\delta z=-H(z^{(j)})$ and updating $z^{(j+1)}=z^{(j)}+\delta z$ corrects both coordinates together.

<a id="image-a-tangent-predictor-and-transverse-correction-step-across-the-upper-fold"></a>
![](continuation-pseudo-arclength-predictor-corrector.png)

**[Figure 7](#image-a-tangent-predictor-and-transverse-correction-step-across-the-upper-fold). A tangent predictor and transverse correction step across the upper fold**. From $z_k=(0.45,0.358875)$ with $h=0.18$, the predictor lies above the largest attainable nearby $\lambda$. Correction along the transverse line returns to the [solution branch](#solution-branch) on the far side of the [continuation fold](#fold-of-a-solution-branch). Both axes use the same scale, so perpendicularity is visible.

This step gives $z_{\mathrm p}\approx(0.617556,0.424641)$ and $z_{k+1}\approx(0.635532,0.378840)$. Check both equations: the solution must satisfy $x^3-x+\lambda=0$ and $t_k^{\mathsf T}(z-z_{\mathrm p})=0$. Checking only the first could accept any point on the [solution branch](#solution-branch). The new $x$ exceeds $1/\sqrt3$, so the step crosses the [continuation fold](#fold-of-a-solution-branch), even though the predictor's $\lambda$ exceeds $2/(3\sqrt3)$.

At the seed, set $a=3x_k^2-1$. The [determinant](multilinear-algebra.md#determinant) of the correction [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) with the exact [unit vector](vector-space.md#unit-vector) above is

$$
\det DH(z_k)=-\sqrt{1+a^2}\ne0.
$$

At either [continuation fold](#fold-of-a-solution-branch), $a=0$, $t_k=(1,0)$ and $DH(z_k)=\begin{pmatrix}0&1\\1&0\end{pmatrix}$: the correction remains invertible. More generally, if $DF$ has full [rank](quadratic-form.md#rank-one-quadratic-form) and a one-dimensional [kernel](kernel-of-a-linear-map.md) spanned by $t_k$, adding $t_k^{\mathsf T}$ gives an [invertible matrix](linear-algebra.md#invertible-matrix), since a [vector](vector-space.md#vector) annihilated by both rows must be zero. This is a local argument; the old transverse [hyperplane](vector-space.md#hyperplane) need not work arbitrarily far along the [curve](topology.md#curve). Reduce $h$ and retry when correction fails, and check the equations and orientation after successful steps. Scaling state and parameter coordinates also matters, because it changes the [Euclidean norm](normed-vector-space.md#euclidean-norm) used to normalize the [tangent vector](tangent-vector.md).

// Target: analysis.bigb

### Transversal surface intersection tracing

↑ **Parent:** [Continuation method](#continuation-method)

For a [parametric surface](differential-geometry.md#parametric-surface) $F(u,v)$ and a scalar implicit equation $f(P)=0$, set $g=f\circ F$. At a regular transversal intersection, $\nabla g\ne0$, and $(-g_v,g_u)$ is a parameter [tangent vector](tangent-vector.md). Normalize its image under $DF$ to choose physical [arc length](riemannian-geometry.md#arc-length) steps. A predictor followed by [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) correction of $g=0$ and a transverse plane equation gives a local [continuation method](#continuation-method). Certified patch bounds are useful for finding seeds; corner signs alone do not detect a closed intersection entirely inside a patch.

#### Transversal intersection of two parametric surfaces

↑ **Parent:** [Transversal surface intersection tracing](#transversal-surface-intersection-tracing)

At regular transverse intersections, the displayed map has a rank-three $3\times4$ [Jacobian matrix](multivariable-calculus.md#jacobian-matrix). Its one-dimensional kernel is the parameter tangent, while the physical tangent is parallel to the [cross product](vector-space.md#cross-product) of the surface normals. A [continuation method](#continuation-method) predicts along that tangent and corrects $F=0$ together with a transverse section equation using [Newton method](mathematical-optimization.md#newton-s-method-in-optimization). Patch bounds and component isolation supply seeds; one seed alone cannot discover every disconnected curve or closed loop. Tangency or coincident surfaces violate the regular-curve assumptions and require separate analysis.

## Computer aided geometric design

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](computer-aided-geometric-design.md)

## Round-off error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[Round-off error](#round-off-error) arises when numbers or arithmetic results are rounded to a finite set of representable values. Its scale is associated with [machine epsilon](floating-point-arithmetic.md#machine-epsilon), and its effects depend on subsequent operations. Even a formula with zero [truncation error](#truncation-error) can lose information. In decimal arithmetic rounded to three significant digits, $1.234$ becomes $1.23$ and $1.233$ becomes $1.23$: subtracting the stored numbers gives zero although the exact difference is $0.001$. The subtraction exposes errors already present in its nearly equal operands.

This example also has a large [condition number](quadratic-form.md#condition-number): independently perturbing the two inputs of $a-b$ can produce a relative amplification $(|a|+|b|)/|a-b|=2467$. High sensitivity belongs to the input-output problem; [numerical stability](#stability-of-a-numerical-method) concerns the arithmetic used to solve it. Conversely, on a common binary system with 53 significant bits and rounding to nearest, $(10^{16}+1)-10^{16}$ evaluates to zero while $(10^{16}-10^{16})+1$ evaluates to one. Exact arithmetic makes both one: changing summation order changes the accumulated [roundoff error](#round-off-error). MIT's summation lecture explains why [numerical stability](#stability-of-a-numerical-method) and the [condition number](quadratic-form.md#condition-number) must be assessed separately.[Steven G. Johnson, MIT 18.335J, Lecture 3: Floating-Point Summation and Backwards Stability, 2019](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/pages/week-2/)

## Richardson extrapolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Richardson_extrapolation)

[Richardson extrapolation](#richardson-extrapolation) improves an approximation by combining two resolutions so that their leading [truncation errors](#truncation-error) cancel. The useful surprise is that the size of that leading error need not be known: its scaling under refinement is enough. This lets an existing [finite difference method](finite-difference.md#finite-difference-method) or [quadrature rule](numerical-integration.md#quadrature-rule) produce a more accurate answer from two runs, without first deriving a new method from scratch.

Suppose $A(h)$ approximates a fixed [limit](calculus.md#limit-of-a-function) $L$ as the positive resolution parameter $h$ tends to zero, with an [asymptotic expansion](asymptotic-expansion.md)

$$
A(h)=L+c h^p+O(h^{p+q}),\qquad p>0,\quad q>0.
$$

Here $p$ is known, $c$ is independent of $h$, and $O$ denotes [Big O notation](real-analysis.md#big-o-notation). The same [asymptotic expansion](asymptotic-expansion.md), with the same $c$, must describe both $h$ and $h/2$. Nested grids make it natural to reuse samples, although nesting itself does not establish this error model. Define the [linear combination](vector-space.md#linear-combination)

$$
R(h)=\frac{2^p A(h/2)-A(h)}{2^p-1}
=A(h/2)+\frac{A(h/2)-A(h)}{2^p-1}.
$$

The weights sum to one, preserving $L$, while $2^p c(h/2)^p-c h^p=0$. Thus [Richardson extrapolation](#richardson-extrapolation) gives $R(h)=L+O(h^{p+q})$: the next available term in the [asymptotic expansion](asymptotic-expansion.md) determines the improved order. Justin Solomon's numerical analysis text develops this cancellation for [finite differences](finite-difference.md) and applies it to [numerical integration](numerical-integration.md).[Justin Solomon, Numerical Algorithms, §14.3.3 and Exercise 14.9](https://people.csail.mit.edu/jsolomon/share/book/numerical_book.pdf)

Geometrically, regard the approximation as a [function](function.md) of $t=h^p$. Its first two terms are a straight line $L+ct$. The two computed points lie at positive $t$; extending the line through them to $t=0$ gives $R(h)$. This is why the operation is extrapolation: it estimates a value outside the sampled parameter interval. The remaining curvature corresponds to the uncancelled terms of the [asymptotic expansion](asymptotic-expansion.md).

**Worked example: a centered derivative of sine**. For the [smooth function](analysis.md#smooth-function) $f(x)=\sin x$, the exact [derivative](calculus.md#derivative) at $x=0$ is $L=\cos0=1$. The centered [difference quotient](calculus.md#difference-quotient), a [central finite difference](finite-difference.md#central-finite-difference), is

$$
A(h)=\frac{f(h)-f(-h)}{2h}=\frac{\sin h}{h}.
$$

The [Taylor series](calculus.md#taylor-series) of [sine](geometry-and-topology.md#sine) gives the signed [truncation error](#truncation-error)

$$
A(h)-1=-\frac{h^2}{6}+\frac{h^4}{120}+O(h^6).
$$

Thus $p=2$, $q=2$ and $c=-1/6$. Halving $h$ divides the leading [truncation error](#truncation-error) by four. Combining the two centered [difference quotients](calculus.md#difference-quotient) with [Richardson extrapolation](#richardson-extrapolation) gives

$$
R(h)=\frac{4A(h/2)-A(h)}{3},\qquad
R(h)-1=-\frac{h^4}{480}+O(h^6).
$$

Indeed, the $h^4$ coefficient becomes $(4/16-1)/(3\cdot120)=-1/480$; the $h^2$ coefficient vanishes. This is the even-power case of [Richardson extrapolation](#richardson-extrapolation) discussed in Persson's authored lecture notes.[Per-Olof Persson, Math 128A, Chapter 4, §§4.1–4.2](https://persson.berkeley.edu/math128a/lecture_notes/math128a_lecture_notes_chapter_4.html)

For $h=0.4$ and $h/2=0.2$, the actual computations are

$$
\begin{aligned}
A(0.4)&\approx0.973545855771626,\\
A(0.2)&\approx0.993346653975306,\\
R(0.4)&\approx0.999946920043199.
\end{aligned}
$$

The absolute error drops from about $2.6454\times10^{-2}$ for $A(0.4)$ to $5.3080\times10^{-5}$ for $R(0.4)$, an improvement by roughly a factor of 498. Refining again gives $R(0.2)\approx0.999996670632607$, whose absolute error is about $3.3294\times10^{-6}$. The refined [truncation errors](#truncation-error) decrease by nearly four for $A$ and nearly sixteen for $R$, reflecting their second and fourth orders.

<a id="image-centered-sine-derivative-errors-second-order-before-richardson-extrapolation-and-fourth-order-after-cancellation"></a>
![](richardson-derivative-error-orders.png)

**[Figure 8](#image-centered-sine-derivative-errors-second-order-before-richardson-extrapolation-and-fourth-order-after-cancellation). Centered sine derivative errors: second order before Richardson extrapolation and fourth order after cancellation**. [Source](richardson-derivative-error-orders.py).

The [logarithmic scale](calculus.md#logarithmic-scale) on each axis turns power laws into straight lines. The dashed reference curves are $h^2/6$ and $h^4/480$, the magnitudes of the leading [truncation errors](#truncation-error). The plotted errors are computed with 70-digit decimal arithmetic, rather than clipped to a display floor; this isolates the [asymptotic expansion](asymptotic-expansion.md) from [roundoff error](#round-off-error).

**Worked example: integrating an exponential**. Approximate the [definite integral](integral.md#definite-integral) of the [exponential function](calculus.md#exponential-function) on $[0,1]$:

$$
L=\int_0^1 e^x\,dx=e-1\approx1.718281828459045.
$$

For [numerical integration](numerical-integration.md), the composite [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule) adds the areas of trapezoids between successive samples; this is the quadrature use of the endpoint average that also occurs in the ODE [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule). On $n$ equal intervals, with $h=1/n$, define

$$
T_n=h\left[\frac{1+e}{2}+\sum_{j=1}^{n-1}e^{jh}\right].
$$

Summing the [geometric series](sequence-and-series.md#geometric-series) gives $T_n=(e-1)\frac h2\frac{e^h+1}{e^h-1}$. Expanding the [exponential function](calculus.md#exponential-function) near zero yields

$$
T_n-L=L\left(\frac{h^2}{12}-\frac{h^4}{720}+O(h^6)\right).
$$

The leading [truncation error](#truncation-error) again has $p=2$, $q=2$. On the uniform nested grids with $n$ and $2n$ intervals, [Richardson extrapolation](#richardson-extrapolation) therefore gives

$$
S_{2n}=\frac{4T_{2n}-T_n}{3},\qquad
S_{2n}-L=\frac{Lh^4}{2880}+O(h^6).
$$

This [linear combination](vector-space.md#linear-combination) is exactly composite [Simpson's rule](numerical-integration.md#simpson-s-rule) on the finer grid, whose spacing is $h/2$. On each coarse panel, an old endpoint receives weight $h/6$ and the new [midpoint](convex-set.md#midpoint) weight $2h/3$; shared old endpoints receive weight $h/3$. These are the usual [Simpson's rule](numerical-integration.md#simpson-s-rule) weights $1,4,2,\ldots,4,1$ multiplied by $h/6$. The equivalence is explained directly in LeMesurier's university notes.[Brenton LeMesurier, MATH 375, §19.1: The Basic Simpson's Rule by Richardson Extrapolation](https://lemesurierb.people.charleston.edu/elementary-numerical-analysis-python/notebooks/definite-integrals-3-simpson-richardson.html)

For two coarse panels and four fine panels,

$$
\begin{aligned}
T_2&\approx1.753931092464825,\\
T_4&\approx1.727221904557517,\\
S_4&\approx1.718318841921747.
\end{aligned}
$$

The absolute errors are about $0.0356493$, $0.00894008$ and $0.0000370135$, respectively. Reusing the fine-grid samples makes [Richardson extrapolation](#richardson-extrapolation) especially attractive here: the resulting [Simpson's rule](numerical-integration.md#simpson-s-rule) needs no samples beyond those already used by $T_{2n}$.

<a id="image-exponential-quadrature-on-nested-grids-trapezoidal-areas-reused-sample-nodes-and-the-fourth-order-simpson-combination"></a>
![](richardson-trapezoid-extrapolation.png)

**[Figure 9](#image-exponential-quadrature-on-nested-grids-trapezoidal-areas-reused-sample-nodes-and-the-fourth-order-simpson-combination). Exponential quadrature on nested grids: trapezoidal areas, reused sample nodes, and the fourth-order Simpson combination**. [Source](richardson-trapezoid-extrapolation.py).

**When the improvement is justified**. [Richardson extrapolation](#richardson-extrapolation) requires the stated [asymptotic expansion](asymptotic-expansion.md) and the correct positive $p$. If the actual leading exponent is $r\ne p$, its coefficient after combination is $c(2^{p-r}-1)/(2^p-1)$, so the leading [truncation error](#truncation-error) generally remains. Merely knowing $A(h)-L=O(h^p)$ does not supply a common coefficient $c$ or a higher-order remainder. A [discontinuity of a function](calculus.md#discontinuity-of-a-function), a singular endpoint, or unrelated changes between grids can invalidate the assumed [asymptotic expansion](asymptotic-expansion.md); refinement alone does not guarantee improvement for every numerical problem.

[Roundoff error](#round-off-error) and errors in the sampled values survive the cancellation of [truncation error](#truncation-error). If the coarse and fine values have absolute perturbations bounded by $\varepsilon$, the perturbation in $R(h)$ is bounded by $(2^p+1)\varepsilon/(2^p-1)$; for $p=2$ this is $5\varepsilon/3$. In [floating-point arithmetic](floating-point-arithmetic.md), a centered [difference quotient](calculus.md#difference-quotient) can also amplify sample errors through division by $h$, so an indefinitely smaller $h$ need not be more accurate. Persson's notes describe this balance between [truncation error](#truncation-error) and [roundoff error](#round-off-error).[Per-Olof Persson, Math 128A, Chapter 4, §4.1: Roundoff Error Instability](https://persson.berkeley.edu/math128a/lecture_notes/math128a_lecture_notes_chapter_4.html)

The same cancellation idea appears in [step-doubling error estimation](error-control-for-ode-solvers.md#step-doubling-error-estimation). For an order-$p$ one-step method for an [ordinary differential equation](differential-equation.md#ordinary-differential-equation), two half steps each contribute [local truncation error](#local-truncation-error) of order $h^{p+1}$, so their accumulated leading local error has ratio $2^{-p}$ to one full step. This explains the denominator $2^p-1$ there; the appropriate exponent follows from that local error model, rather than automatically from a generic use of [Richardson extrapolation](#richardson-extrapolation).

## Error control for ODE solvers

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](error-control-for-ode-solvers.md)

## Finite volume method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](finite-volume-method.md)

## Interval bisection

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[Interval bisection](#interval-bisection) solves a target equation $f(x)=t$ by repeatedly halving a [closed interval](real-analysis.md#closed-real-interval) known to contain a solution. It is the [bisection method](#bisection-method) applied to $g(x)=f(x)-t$, so the target becomes a [zero of a function](polynomial.md#zero-of-a-function). This reduction from an equation to root finding is described in Demanet's notes.[Laurent Demanet, MIT 18.330, Chapter 4, §4.1, pp. 1–2, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/5b325bfa56a599794c7196de926844b0_MIT18_330S12_Chapter4.pdf) Here the emphasis is on a [continuous](calculus.md#continuous-function) [strictly increasing function](calculus.md#strictly-increasing-function): the target identifies one input, making [interval bisection](#interval-bisection) a way to evaluate its [inverse function](function.md#inverse-function) without an explicit inverse formula.

Let $f:[a_0,b_0]\to\mathbb R$ be a [continuous function](calculus.md#continuous-function), with $a_0<b_0$ and $f(a_0)\leq t\leq f(b_0)$. The [intermediate value theorem](calculus.md#intermediate-value-theorem) guarantees existence; a [strictly increasing function](calculus.md#strictly-increasing-function) also guarantees uniqueness. Check endpoint equality first. Otherwise, for the current [root bracket](#root-bracket) $[a_k,b_k]$, evaluate its [midpoint](convex-set.md#midpoint) $m_k=(a_k+b_k)/2$. If $f(m_k)<t$, retain $[m_k,b_k]$; if $f(m_k)>t$, retain $[a_k,m_k]$; if $f(m_k)=t$, return that exact solution. These comparisons preserve the target bracket. General [bisection method](#bisection-method) needs [continuity](calculus.md#continuous-function) and opposite signs of $g$ at the endpoints, without requiring [monotonicity](calculus.md#monotonic-function) or a unique [zero of a function](polynomial.md#zero-of-a-function); see [limitations of bisection](#limitations-of-bisection).

An original dimensionless [polynomial](polynomial.md) example is

$$
f(x)=x^3+x,\qquad t=10,\qquad [a_0,b_0]=[0,3].
$$

Here $f(0)=0<10<30=f(3)$ and the [derivative](calculus.md#derivative) $f'(x)=3x^2+1>0$, so there is exactly one solution. In fact $x_*=2$; knowing this lets us check the computed [absolute error](#absolute-error) independently of the guarantee. The first four halvings give the following exact [rational numbers](number-theory.md#rational-number):

$$
\begin{array}{c|c|r|c}
\text{update }k&\text{tested }m_{k-1}&f(m_{k-1})-10&\text{retained }[a_k,b_k]\\\hline
1&3/2&-41/8&[3/2,3]\\
2&9/4&233/64&[3/2,9/4]\\
3&15/8&-785/512&[15/8,9/4]\\
4&33/16&3425/4096&[15/8,33/16]
\end{array}
$$

<a id="image-finding-the-input-for-a-target-output-cubic-graph-and-four-retained-brackets"></a>
![](interval-bisection-cubic-target-brackets.png)

**[Figure 10](#image-finding-the-input-for-a-target-output-cubic-graph-and-four-retained-brackets). Finding the input for a target output: cubic graph and four retained brackets**.

The beauty of [interval bisection](#interval-bisection) is that the enclosure itself supplies the certificate: one comparison removes half the possible inputs, regardless of the steepness of the [function graph](function.md#graph-of-a-function). In exact arithmetic, after $k$ completed halvings without exact termination, the width and the [bisection error bound](#bisection-error-bound) for the new [midpoint](convex-set.md#midpoint) are

$$
W_k=b_k-a_k=\frac{3}{2^k},\qquad |m_k-x_*|\leq\frac{W_k}{2}=\frac{3}{2^{k+1}}.
$$

The reported [midpoint](convex-set.md#midpoint) after update four is $m_4=63/32$, rather than the last tested point $m_3=33/16$. Its certified [absolute error](#absolute-error) is at most $3/32$, and its actual [absolute error](#absolute-error) is $1/32$. For a requested position tolerance $10^{-3}$, the [bisection stopping criterion](#bisection-stopping-criterion) requires eleven halvings: ten give $3/2048>10^{-3}$, while eleven give

$$
[a_{11},b_{11}]=[4095/2048,2049/1024],\qquad m_{11}=8193/4096,\qquad |m_{11}-2|\leq3/4096<10^{-3}.
$$

The actual [absolute error](#absolute-error) is $1/4096$. The new [midpoint](convex-set.md#midpoint) need not be evaluated to obtain this certificate.

The signed **output residual** is $r=f(m)-t$; the position [approximation error](#approximation-error) is $m-x_*$. They answer different questions: how close is the output to the target, and how close is the input to the solution? Driscoll and Braun explain why a small residual needs information about the [derivative](calculus.md#derivative) to imply small position error.[Toby A. Driscoll and Richard J. Braun, Fundamentals of Numerical Computation, §4.1.1, Conditioning, error, and residual](https://fncbook.com/rootproblem/) For this particular [polynomial](polynomial.md), direct factorization gives

$$
f(m)-10=(m-2)(m^2+2m+5).
$$

Thus at $m_4=63/32$ the residual is $-13121/32768\approx-0.400421$, despite position [absolute error](#absolute-error) $1/32=0.03125$. If a differentiable [function](function.md) satisfies $0<\ell\leq f'(x)\leq L$ throughout the bracket, the [mean value theorem](calculus.md#mean-value-theorem) gives the rigorous conversion

$$
\ell|m-x_*|\leq|f(m)-t|\leq L|m-x_*|.
$$

Our example permits $\ell=1$ and $L=28$ on $[0,3]$. Strict increase alone supplies no positive lower [derivative](calculus.md#derivative) bound: $f(x)=x^3$ is [strictly increasing](calculus.md#strictly-increasing-function) but $f'(0)=0$. A small residual alone is therefore not a universal position certificate; even the target equation $10^{-6}(x-2)=0$ has residual $10^{-6}$ at $x=3$, a full unit from its solution.

<a id="image-certified-position-error-and-output-residual-measure-different-distances"></a>
![](interval-bisection-position-output-errors.png)

**[Figure 11](#image-certified-position-error-and-output-residual-measure-different-distances). Certified position error and output residual measure different distances**.

The guarantees require [continuity](calculus.md#continuous-function) and correct evaluations, not just narrowing endpoints. For the [strictly increasing function](calculus.md#strictly-increasing-function) $h(x)=x$ when $x<0$ and $h(x)=x+1$ when $x\geq0$, the target $1/2$ lies between $h(-1)$ and $h(1)$ but is never attained: a [jump discontinuity](calculus.md#jump-discontinuity) defeats the existence argument. With [floating-point arithmetic](floating-point-arithmetic.md) or an approximate evaluation, an incorrect comparison can discard the true solution. A certified [interval enclosure](#interval-enclosure) of $f(m)$ wholly below or above $t$ certifies the corresponding decision; an enclosure containing $t$ is inconclusive, rather than proof of equality. If rounding makes the [midpoint](convex-set.md#midpoint) equal an endpoint, report the precision limit; see [bisection stopping criterion](#bisection-stopping-criterion) for the rounded position bound. Both figures are exact mathematical examples, not measured data.

## Implicit time-stepping method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An implicit time-stepping method determines a new solution value through an equation involving that same value. A small-step [contraction mapping](analysis.md#contraction-mapping) argument often establishes local solvability when the vector field is [Lipschitz continuous](real-analysis.md#lipschitz-continuity). Examples include the [Backward Euler method](#backward-euler-method), [implicit Runge-Kutta methods](runge-kutta-method.md#implicit-runge-kutta-method) and implicit [linear multistep methods](linear-multistep-method.md). Solvability of the update is a separate issue from [stability of a numerical method](#stability-of-a-numerical-method).

## Multigrid method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](multigrid-method.md)

## Convergence of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For an [initial value problem](differential-equation.md#initial-value-problem), convergence means that the largest [global error](#global-discretization-error) on each fixed finite time interval tends to zero as the step size tends to zero and the starting errors vanish. For [linear multistep methods](linear-multistep-method.md), the [Dahlquist equivalence theorem](linear-multistep-method.md#dahlquist-equivalence-theorem) separates this requirement into [consistency of a numerical method](#consistency-of-a-numerical-method) and [zero-stability](linear-multistep-method.md#zero-stability).

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

The [midpoint quadrature rule](#midpoint-quadrature-rule) replaces the [integrand](integral.md#integrand) on $[a,b]$, $a<b$, by its value halfway across the interval:

$$
I(f)=\int_a^bf(x)\,dx\approx M(f)=(b-a)f\left(\frac{a+b}{2}\right).
$$

Geometrically, $M(f)$ is the signed area of a [rectangle](euclidean-geometry.md#rectangle) with width $b-a$ and height $f((a+b)/2)$. Its single [quadrature node](numerical-integration.md#quadrature-node) is $(a+b)/2$ and its [quadrature weight](numerical-integration.md#quadrature-weight) is $b-a$. Sampling in the interior is useful when endpoint evaluation is inconvenient, although an endpoint singularity can invalidate the [quadrature error](real-analysis.md#quadrature-error) estimates below.

The [midpoint quadrature rule](#midpoint-quadrature-rule) is exact for every [affine function](vector-space.md#affine-function) $f(x)=\alpha x+\beta$: the average height over an interval equals its midpoint height. For example, on $[0,2]$, $f(x)=2x+1$ gives $I(f)=6$ and $M(f)=2f(1)=6$. Positive and negative area discrepancies cancel for a sloping straight line. For the [polynomial](polynomial.md) $f(x)=x^2$ on $[0,1]$, however, $I(f)=1/3$ and $M(f)=1/4$, giving [approximation error](#approximation-error) $M(f)-I(f)=-1/12$. Thus its [degree of precision of a quadrature rule](numerical-integration.md#degree-of-precision-of-a-quadrature-rule) is exactly one.[§5.8, printed p. 223: midpoint rectangles, linear exactness and signed quadratic errors](mathematics-bibliography.md#calculus-by-gilbert-strang/5-8-numerical-integration)

<a id="image-midpoint-rectangles-and-trapezoids-approximate-the-area-under-a-quadratic"></a>
![](midpoint-trapezoidal-quadratic-areas.png)

**[Figure 12](#image-midpoint-rectangles-and-trapezoids-approximate-the-area-under-a-quadratic). Midpoint rectangles and trapezoids approximate the area under a quadratic**.

For the [polynomial](polynomial.md) $f(x)=x^2$ on $[0,1]$, four panels give [composite midpoint quadrature rule](#composite-midpoint-quadrature-rule) value $21/64$ and [composite trapezoidal rule](runge-kutta-method.md#composite-trapezoidal-rule) value $11/32$, bracketing the exact [integral](integral.md) $1/3$. Individual midpoint rectangles can cross the curve; it is their total signed area that underestimates the [integral](integral.md).

For $f\in C^2[a,b]$, meaning that its first two [derivatives](calculus.md#derivative) exist and are [continuous functions](calculus.md#continuous-function) on the closed interval, the signed [approximation error](#approximation-error) has the form

$$
M(f)-I(f)=-\frac{(b-a)^3}{24}f''(\xi_M),\qquad a<\xi_M<b.
$$

Hence a [convex function](real-analysis.md#convex-function) with $f''\geq0$ is underestimated, and a [concave function](real-analysis.md#concave-function) with $f''\leq0$ is overestimated. A short justification uses the [Taylor formula with integral remainder](calculus.md#taylor-formula-with-integral-remainder): writing $m=(a+b)/2$, it gives $I(f)-M(f)=\int_a^b k(t)f''(t)\,dt$, where $k(t)=(t-a)^2/2$ for $a\leq t\leq m$ and $k(t)=(b-t)^2/2$ for $m\leq t\leq b$. This nonnegative [Peano kernel](#peano-kernel) has [integral](integral.md) $(b-a)^3/24$, so the [weighted mean value theorem for integrals](real-analysis.md#weighted-mean-value-theorem-for-integrals) gives the stated sign and coefficient.

### Composite midpoint quadrature rule

↑ **Parent:** [Midpoint quadrature rule](#midpoint-quadrature-rule)

Apply the [midpoint quadrature rule](#midpoint-quadrature-rule) on each of $n$ equal panels of a [partition of an interval](real-analysis.md#partition-of-an-interval), with $h=(b-a)/n$:

$$
M_n(f)=h\sum_{j=0}^{n-1}f\left(a+(j+\tfrac12)h\right).
$$

Each [quadrature node](numerical-integration.md#quadrature-node) is a panel midpoint and each [quadrature weight](numerical-integration.md#quadrature-weight) is $h$. For $f\in C^2[a,b]$, put $K=\max_{x\in[a,b]}|f''(x)|$. Summing the panel [quadrature errors](real-analysis.md#quadrature-error) gives

$$
M_n(f)-I(f)=-\frac{b-a}{24}h^2f''(\xi),\qquad |M_n(f)-I(f)|\leq\frac{b-a}{24}h^2K
$$

for some $\xi\in(a,b)$. Each panel contributes at most $Kh^3/24$; there are $n=(b-a)/h$ panels, explaining the [composite midpoint rule error](#composite-midpoint-rule-error) of order $O(h^2)$ in [big O notation](real-analysis.md#big-o-notation). On a nonuniform [partition of an interval](real-analysis.md#partition-of-an-interval) with panel widths $h_j$ and largest width $H$, the corresponding bound is $K\sum_jh_j^3/24\leq K(b-a)H^2/24$.

For $f(x)=x^2$ on $[0,1]$, summing the sampled [polynomial](polynomial.md) exactly yields

$$
M_n(f)=\frac13-\frac{1}{12n^2}.
$$

Doubling $n$ divides the [absolute error](#absolute-error) by exactly four. For a general $C^2$ [function](function.md), halving $h$ divides the displayed error bound by four, but the actual [absolute error](#absolute-error) need not follow that ratio: cancellation can make it smaller or zero. [Continuous functions](calculus.md#continuous-function) still give convergence as the largest panel width tends to zero, by [uniform continuity](topological-analysis.md#uniform-continuity); without the bounded second [derivative](calculus.md#derivative), the second-order rate is not guaranteed. [Noise sensitivity of a quadrature rule](numerical-integration.md#noise-sensitivity-of-a-quadrature-rule) explains a separate limitation when samples are inexact.

## Approximation error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a numerical reference value $x$ and a computed value $x_{\mathrm{approx}}$, the signed [approximation error](#approximation-error) is $x_{\mathrm{approx}}-x$. Stating the reference matters: comparison with a measured value assesses agreement with that value, rather than with an unknown exact value.

### Error bound

↑ **Parent:** [Approximation error](#approximation-error)

An [error bound](#error-bound) is an established [upper bound](set.md#upper-bound-in-a-partially-ordered-set) on a specified [approximation error](#approximation-error), on a stated domain and under stated assumptions. A numerical comparison at selected points can test an approximation but does not by itself establish a bound throughout that domain. An [absolute error](#absolute-error) bound controls $|\widetilde f-f|$; a [relative error](#relative-error) bound additionally specifies the reference scale.

### Absolute error

↑ **Parent:** [Approximation error](#approximation-error)

The [absolute error](#absolute-error) is the [absolute value](real-analysis.md#absolute-value) of the [approximation error](#approximation-error), $|x_{\mathrm{approx}}-x|$, measured in the same units as the numerical reference $x$. For example, approximating $1/3$ by $0.33$ gives [absolute error](#absolute-error) $|0.33-1/3|=1/300$.

### Relative error

↑ **Parent:** [Approximation error](#approximation-error)

For a nonzero reference value $x$, the relative error is the [absolute error](#absolute-error) divided by the reference's [absolute value](real-analysis.md#absolute-value):

$$
\frac{|x_{\mathrm{approx}}-x|}{|x|}.
$$

It is [dimensionless](physics.md#dimensionless-quantity) and expresses the size of the error compared with the quantity being approximated. Approximating $1/3$ by $0.33$ has [absolute error](#absolute-error) $1/300$ and [relative error](#relative-error) $1/100=1\%$. The definition is unavailable when the reference is zero; use an [absolute error](#absolute-error) or a separately stated scale in that case.

#### Signed relative error

↑ **Parent:** [Relative error](#relative-error)

The signed relative error is $\varepsilon=(x_{\mathrm{approx}}-x)/x$ for a nonzero reference $x$. Its [absolute value](real-analysis.md#absolute-value) is the [relative error](#relative-error). For a positive reference, a negative [signed relative error](#signed-relative-error) means underestimation, and a positive one means overestimation. For a negative reference that interpretation reverses, so retain the displayed definition when interpreting its sign.

## Truncation error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Truncation_error)

[Truncation error](#truncation-error) is introduced by replacing an exact operation with a finite approximation. It remains even when all arithmetic is exact. For $f(x)=x^2$, the forward [finite difference](finite-difference.md) for its [derivative](calculus.md#derivative) at $x=1$ gives

$$
\frac{f(1+h)-f(1)}h=2+h,\qquad f'(1)=2.
$$

Thus the [truncation error](#truncation-error) is exactly $h$: $h=0.1$ gives $2.1$ and $h=0.01$ gives $2.01$. In finite precision, however, the numerator subtracts nearly equal values, and their [roundoff error](#round-off-error) can be amplified by division by $h$. For smooth data with bounded evaluation errors of scale $u$, a typical bound has competing terms $C_1h+C_2u/h$. Smaller $h$ reduces the first term and increases the second; with fixed positive constants the balancing scale is $h\sim\sqrt u$. This is why blindly refining a [finite difference](finite-difference.md) eventually stops improving it.

### Series truncation error

↑ **Parent:** [Truncation error](#truncation-error)

For a [convergent series](sequence-and-series.md#convergent-series) with [sum](arithmetic.md#sum) $S$, the error from keeping only the first $N$ terms is the remaining [sum](arithmetic.md#sum) $R_N=\sum_{n>N}a_n$. This [truncation error](#truncation-error) exists even with exact arithmetic. The [zeta series truncation error](bernoulli-number.md#zeta-series-truncation-error) gives explicit bounds for positive reciprocal-power terms.

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

For a numerical evolution, [numerical stability](#stability-of-a-numerical-method) means that perturbations remain controlled over a fixed finite interval by a bound independent of sufficiently small discretization parameters. With perturbations $\delta_n$ to starting data and added step defects $d_n$, a typical estimate is

$$
\max_{nh\leq T}\|\delta_n\|\leq C_T\left(\|\delta_0\|+\sum_{nh<T}\|d_n\|\right),
$$

where $C_T$ is independent of $h$. For a linear homogeneous recurrence, a uniform bound on powers of its update [matrix](vector-space.md#matrix) supplies this control. [von Neumann stability analysis](finite-difference.md#von-neumann-stability-analysis) and the [energy method](#energy-method) provide complementary tools.

Finite-interval [numerical stability](#stability-of-a-numerical-method) differs from [absolute stability](#linear-stability-domain) at a fixed step size. Applying the [Euler method](#euler-method) to $y'=-2y$ multiplies a perturbation by $1-2h$ each step. At $h=0.2$ this is $0.6$, so perturbations shrink; at $h=1.2$ it is $-1.4$, so they alternate and grow. Nevertheless the [Euler method](#euler-method) converges as $h\to0$ for this problem: failure at a coarse step does not contradict the convergence theorem. [Absolute stability](#linear-stability-domain) asks whether a selected step preserves boundedness of the [Dahlquist test equation](#dahlquist-test-equation) over arbitrarily many steps. MIT's analysis uses strict decay, $|1+h\lambda|<1$, rather than the boundary-inclusive boundedness convention.[Laurent Demanet, MIT 18.330, Chapter 5, Example 14, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/a9d2bd9be098f0ada172af40379a17cc_MIT18_330S12_Chapter5.pdf)

## Consistency of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

For a one-step approximation $y_{n+1}=y_n+h\phi(t_n,y_n,h)$ to an [ordinary differential equation](differential-equation.md#ordinary-differential-equation), insert the exact solution and define the unscaled [local truncation error](#local-truncation-error)

$$
\tau_{n+1}=y(t_n+h)-y(t_n)-h\phi(t_n,y(t_n),h).
$$

[Consistency of a numerical method](#consistency-of-a-numerical-method) requires $\tau_{n+1}/h\to0$ uniformly on the finite interval being approximated, under the stated smoothness assumptions. Merely asking $\tau_{n+1}\to0$ is too weak: the useless update $y_{n+1}=y_n$ has defect $h y'(t_n)+O(h^2)$, which tends to zero but generally fails the scaled test. Here $O$ denotes [Big O notation](real-analysis.md#big-o-notation). MIT uses this division-by-step convention.[Laurent Demanet, MIT 18.330, Chapter 5, Definition 6, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/a9d2bd9be098f0ada172af40379a17cc_MIT18_330S12_Chapter5.pdf)

For the [Euler method](#euler-method), [Taylor's theorem](calculus.md#taylor-s-theorem) gives $\tau_{n+1}=h^2y''(\xi_n)/2$. A bounded second [derivative](calculus.md#derivative) therefore gives [local truncation error](#local-truncation-error) $O(h^2)$ and a scaled defect $O(h)$. Under a uniform [Lipschitz continuity](real-analysis.md#lipschitz-continuity) assumption on $f$ in $y$, within a region containing the exact and numerical solutions, [numerical stability](#stability-of-a-numerical-method) controls accumulation over about $T/h$ steps. This yields [global error](#global-discretization-error) $O(h)$ with exact starting data. [Consistency of a numerical method](#consistency-of-a-numerical-method) checks each step; [numerical stability](#stability-of-a-numerical-method) controls their combination.

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

[This section is present in another page, follow this link to view it.](finite-element-method.md)

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

## Discrete Fourier transform

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](discrete-fourier-transform.md)

## Interpolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](interpolation.md)

## Gershgorin circle theorem

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gershgorin_circle_theorem)

The [Gershgorin circle theorem](#gershgorin-circle-theorem) locates every [eigenvalue](linear-operator-theory.md#eigenvalue) of a [square matrix](vector-space.md#square-matrix) using only its entries. A diagonal entry supplies a centre in the [complex plane](complex-analysis.md#complex-plane), and the sum of the off-diagonal [absolute values](real-analysis.md#absolute-value) in its row supplies a radius. Small off-diagonal couplings therefore confine the [eigenvalues](linear-operator-theory.md#eigenvalue) near the diagonal entries. This turns a global [eigenvalue](linear-operator-theory.md#eigenvalue) problem into a picture built one row at a time.

Precisely, let $A=(a_{ij})\in\mathbb C^{n\times n}$, with $n\geq1$, and define the closed [Gershgorin discs](#gershgorin-disc)

$$
r_i=\sum_{\substack{j=1\\j\ne i}}^n|a_{ij}|,\qquad D_i(A)=\{z\in\mathbb C:|z-a_{ii}|\leq r_i\},\qquad i=1,\ldots,n.
$$

Every [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ of $A$ satisfies $\lambda\in\bigcup_iD_i(A)$, including [eigenvalues](linear-operator-theory.md#eigenvalue) on the boundaries. No symmetry or [diagonalizability](linear-operator-theory.md#diagonalizable-matrix) is required. Despite the name, the theorem uses filled [disks](topology.md#disk-mathematics), not just their circular boundaries.[Gene H. Golub, CME 302: Numerical Linear Algebra, Lecture 2, §6, 2005; notes by James Lambers, edited by Lek-Heng Lim](https://www.stat.uchicago.edu/~lekheng/courses/302/notes2.pdf)

The short reason is the [triangle inequality](topological-analysis.md#triangle-inequality). For a nonzero [eigenvector](linear-operator-theory.md#eigenvector) $x$ with $Ax=\lambda x$, choose $i$ with $|x_i|=\max_j|x_j|>0$. The $i$th row gives

$$
(\lambda-a_{ii})x_i=\sum_{j\ne i}a_{ij}x_j,\qquad |\lambda-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\frac{|x_j|}{|x_i|}\leq r_i.
$$

Thus the largest [eigenvector](linear-operator-theory.md#eigenvector) coordinate identifies a [Gershgorin disc](#gershgorin-disc) containing $\lambda$, even though that [eigenvector](linear-operator-theory.md#eigenvector) need never be computed to use the bound.

This is useful when a full [eigenvalue](linear-operator-theory.md#eigenvalue) computation would be expensive: forming the [Gershgorin discs](#gershgorin-disc) needs one pass over the nonzero entries of a [sparse matrix](vector-space.md#sparse-matrix). If $0$ lies outside every [Gershgorin disc](#gershgorin-disc), then $A$ is an [invertible matrix](linear-algebra.md#invertible-matrix), since zero is not an [eigenvalue](linear-operator-theory.md#eigenvalue). The condition is exactly $|a_{ii}|>r_i$ in every row, namely [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix). This connects [diagonal dominance](algebra.md#diagonal-dominance) to solvability of a [linear system](linear-algebra.md#system-of-linear-equations); the [inverse infinity-norm bound from diagonal dominance](vector-space.md#inverse-infinity-norm-bound-from-diagonal-dominance) adds a quantitative bound. It is a sufficient test: failure to exclude zero does not prove singularity.

For a concrete [symmetric matrix](linear-algebra.md#symmetric-matrix), take

$$
A=\begin{pmatrix}2&0.2&0.1\\0.2&5&0.3\\0.1&0.3&9\end{pmatrix},\qquad (r_1,r_2,r_3)=(0.3,0.5,0.4).
$$

The three [Gershgorin discs](#gershgorin-disc) have centres $2,5,9$ and are pairwise disjoint. The [finite-dimensional spectral theorem](linear-operator-theory.md#finite-dimensional-spectral-theorem) makes the [eigenvalues](linear-operator-theory.md#eigenvalue) real, so their possible locations reduce to the [intervals](real-analysis.md#interval-mathematics) $[1.7,2.3]$, $[4.5,5.5]$, and $[8.6,9.4]$. [Gershgorin eigenvalue counting](#gershgorin-eigenvalue-counting) gives exactly one [eigenvalue](linear-operator-theory.md#eigenvalue) in each. Independently, the [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) is

$$
\det(\lambda I-A)=\lambda^3-16\lambda^2+72.86\lambda-89.422,
$$

whose numerical [polynomial roots](polynomial.md#root-of-a-polynomial) are $1.985811$, $4.989942$, and $9.024247$, rounded to six decimal places. All are positive, as [Gershgorin bounds for symmetric matrices](#gershgorin-bounds-for-symmetric-matrices) already guarantee without finding those [polynomial roots](polynomial.md#root-of-a-polynomial).

<a id="image-three-separated-gershgorin-discs-each-containing-one-real-eigenvalue-of-the-symmetric-example"></a>
![](gershgorin-eigenvalue-disks.png)

**[Figure 13](#image-three-separated-gershgorin-discs-each-containing-one-real-eigenvalue-of-the-symmetric-example). Three separated Gershgorin discs, each containing one real eigenvalue of the symmetric example**.

S. Gerschgorin published the result in 1931 in _Über die Abgrenzung der Eigenwerte einer Matrix_, in the _Bulletin de l'Académie des Sciences de l'URSS_, issue 6, pages 749–754. The original paper's §2 states both [eigenvalue](linear-operator-theory.md#eigenvalue) inclusion and counting in separated groups of [Gershgorin discs](#gershgorin-disc); §3 already discusses column bounds and transformations preserving the [eigenvalues](linear-operator-theory.md#eigenvalue). Thus both the localization picture and ways to sharpen it were part of the original development.[S. Gerschgorin, Über die Abgrenzung der Eigenwerte einer Matrix, 1931, pp. 749–754; original German paper in the journal archive](https://www.mathnet.ru/php/getFT.phtml?jrnid=im&paperid=5235&what=fullt&option_lang=eng)

### Gershgorin disc

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

A row [Gershgorin disc](#gershgorin-disc) of a [square matrix](vector-space.md#square-matrix) $A=(a_{ij})$ is the closed [disk](topology.md#disk-mathematics) in the [complex plane](complex-analysis.md#complex-plane) with centre $a_{ii}$ and radius $r_i=\sum_{j\ne i}|a_{ij}|$. A zero radius gives a single point. The [Gershgorin disc theorem](#gershgorin-circle-theorem) places every [eigenvalue](linear-operator-theory.md#eigenvalue) in the union of these [disks](topology.md#disk-mathematics). For a [Hermitian matrix](hilbert-space.md#hermitian-operator), the real [intervals](real-analysis.md#interval-mathematics) cut out by the [Gershgorin discs](#gershgorin-disc) bound the [eigenvalues](linear-operator-theory.md#eigenvalue), including [energy](energy.md) levels when the [matrix](vector-space.md#matrix) represents a [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics).

Applying the [Gershgorin circle theorem](#gershgorin-circle-theorem) to the [transpose](vector-space.md#transpose) $A^T$ gives column [Gershgorin discs](#gershgorin-disc) with the same centres and radii $c_i=\sum_{j\ne i}|a_{ji}|$. Since $A$ and $A^T$ have the same [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial), every [eigenvalue](linear-operator-theory.md#eigenvalue) lies in the intersection of the row-disc union and the column-disc union. This is an intersection of two unions; one cannot generally replace each row radius by $\min(r_i,c_i)$. An isolated row [Gershgorin disc](#gershgorin-disc) contains exactly one [eigenvalue](linear-operator-theory.md#eigenvalue) by [Gershgorin eigenvalue counting](#gershgorin-eigenvalue-counting).[Marshall Hampton, Introduction to Numerical Methods, Eigenstuff: Gershgorin circle theorem](https://www.d.umn.edu/~mhampton/NA/Eigenstuff/)

### Gershgorin eigenvalue counting

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

Let $C$ be a [connected component](geometry-and-topology.md#connected-component) of the union of the row [Gershgorin discs](#gershgorin-disc) of an $n\times n$ [matrix](vector-space.md#matrix). If $C$ comprises $k$ of the indexed [Gershgorin discs](#gershgorin-disc), then it contains exactly $k$ [eigenvalues](linear-operator-theory.md#eigenvalue), counted with [algebraic multiplicity](linear-operator-theory.md#algebraic-multiplicity). Coincident [disks](topology.md#disk-mathematics) still count separately, once for each row. In particular, a [Gershgorin disc](#gershgorin-disc) disjoint from all the others contains one simple [eigenvalue](linear-operator-theory.md#eigenvalue). More generally, any union of $k$ indexed [Gershgorin discs](#gershgorin-disc) disjoint from the remaining $n-k$ contains exactly $k$ [eigenvalues](linear-operator-theory.md#eigenvalue), whether or not that union is connected.[Chi-Kwong Li, Math 408 lecture notes, §6.1, Theorem 6.1.1, p. 48](https://cklixx.people.wm.edu/teaching/math408/408-note.pdf)

The separation is essential: overlapping [Gershgorin discs](#gershgorin-disc) do not individually promise one [eigenvalue](linear-operator-theory.md#eigenvalue) each. Discs that touch at a boundary point belong to the same [connected component](geometry-and-topology.md#connected-component). For example, the [matrix](vector-space.md#matrix) $\left(\begin{smallmatrix}2&1&0\\0&2&0\\0&0&8\end{smallmatrix}\right)$ has [Gershgorin discs](#gershgorin-disc) of radii $1,0,0$ with centres $2,2,8$. The component around $2$ comprises two indexed [disks](topology.md#disk-mathematics) and contains the [eigenvalue](linear-operator-theory.md#eigenvalue) $2$ with [algebraic multiplicity](linear-operator-theory.md#algebraic-multiplicity) two; the isolated point at $8$ contains the remaining [eigenvalue](linear-operator-theory.md#eigenvalue).

For intuition, continuously turn on the off-diagonal entries using the [diagonal matrix](linear-algebra.md#diagonal-matrix) $E=\operatorname{diag}(a_{11},\ldots,a_{nn})$ and $A(t)=E+t(A-E)$, $0\leq t\leq1$. At $t=0$ the [eigenvalues](linear-operator-theory.md#eigenvalue) are the disk centres; at every later time the [Gershgorin discs](#gershgorin-disc) stay inside their final union. The [continuity](calculus.md#continuous-function) of the [eigenvalues](linear-operator-theory.md#eigenvalue) as a collection means that no [eigenvalue](linear-operator-theory.md#eigenvalue) can cross a gap between final components. The count gives a useful certificate that an [eigenvalue](linear-operator-theory.md#eigenvalue) cluster is complete.[Gene H. Golub, CME 302, Lecture 2, §6: turning on the off-diagonal entries continuously](https://www.stat.uchicago.edu/~lekheng/courses/302/notes2.pdf)

### Gershgorin bounds for symmetric matrices

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

For a real [symmetric matrix](linear-algebra.md#symmetric-matrix), or more generally a [Hermitian matrix](hilbert-space.md#hermitian-operator), the [finite-dimensional spectral theorem](linear-operator-theory.md#finite-dimensional-spectral-theorem) makes all [eigenvalues](linear-operator-theory.md#eigenvalue) real. Intersecting its [Gershgorin discs](#gershgorin-disc) with the real axis gives

$$
\lambda\in\bigcup_{i=1}^n[a_{ii}-r_i,a_{ii}+r_i],\qquad \min_i(a_{ii}-r_i)\leq\lambda\leq\max_i(a_{ii}+r_i).
$$

The union preserves gaps that the single outer [interval](real-analysis.md#interval-mathematics) loses. If every $a_{ii}-r_i>0$, all [eigenvalues](linear-operator-theory.md#eigenvalue) are positive, so the [matrix](vector-space.md#matrix) is a [positive-definite matrix](quadratic-form.md#positive-definite-matrix). This is the positive-diagonal [strictly diagonally dominant matrix](vector-space.md#strictly-diagonally-dominant-matrix) criterion. For the three-by-three example, $1.7\leq\lambda\leq9.4$ gives a [positive-definite matrix](quadratic-form.md#positive-definite-matrix) certificate and bounds its [spectral condition number of a positive-definite matrix](quadratic-form.md#spectral-condition-number-of-a-positive-definite-matrix) by $9.4/1.7\approx5.529412$; the computed value is about $4.544364$.

Strictness matters. The [symmetric matrix](linear-algebra.md#symmetric-matrix) $\left(\begin{smallmatrix}1&-1\\-1&1\end{smallmatrix}\right)$ has positive diagonal and is a [diagonally dominant matrix](vector-space.md#diagonally-dominant-matrix), but its [eigenvalues](linear-operator-theory.md#eigenvalue) are $0$ and $2$: it is singular. For a general complex [matrix](vector-space.md#matrix), the condition $\operatorname{Re}a_{ii}>r_i$ only puts the [eigenvalues](linear-operator-theory.md#eigenvalue) in the open [right half-plane](complex-analysis.md#right-half-plane). The [Hermitian matrix](hilbert-space.md#hermitian-operator) assumption is what converts that statement into positive definiteness.

### Diagonal scaling of Gershgorin discs

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

A positive [diagonal matrix](linear-algebra.md#diagonal-matrix) $D=\operatorname{diag}(d_1,\ldots,d_n)$, with $d_i>0$, is an [invertible matrix](linear-algebra.md#invertible-matrix) and changes the coordinate scales through the [similarity transformation](linear-algebra.md#similarity-transformation) $B=D^{-1}AD$. Its diagonal entries are still $a_{ii}$, while $b_{ij}=a_{ij}d_j/d_i$. Thus the [Gershgorin discs](#gershgorin-disc) have the same centres but different radii. [Matrix similarity](linear-algebra.md#matrix-similarity) preserves the [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) and [eigenvalues](linear-operator-theory.md#eigenvalue), so the original and scaled disk unions are both valid bounds and may be intersected. Suitable scaling can compensate for badly unbalanced off-diagonal entries; it need not shrink every radius.[Chi-Kwong Li, Math 408 lecture notes, §6.1: similarity transformations for eigenvalue localization](https://cklixx.people.wm.edu/teaching/math408/408-note.pdf)

For example,

$$
A=\begin{pmatrix}2&100\\0.01&3\end{pmatrix},\qquad D=\begin{pmatrix}100&0\\0&1\end{pmatrix},\qquad D^{-1}AD=\begin{pmatrix}2&1\\1&3\end{pmatrix}.
$$

The original [Gershgorin discs](#gershgorin-disc) are $|z-2|\leq100$ and $|z-3|\leq0.01$. Their union is simply the huge first [disk](topology.md#disk-mathematics); the small second [disk](topology.md#disk-mathematics) contains no [eigenvalue](linear-operator-theory.md#eigenvalue). After scaling, both radii are $1$, giving $|z-2|\leq1$ or $|z-3|\leq1$. The two [Gershgorin discs](#gershgorin-disc) overlap, so their individual [eigenvalue](linear-operator-theory.md#eigenvalue) counts are not certified. The scaled [matrix](vector-space.md#matrix) is a real [symmetric matrix](linear-algebra.md#symmetric-matrix), however, so [matrix similarity](linear-algebra.md#matrix-similarity) now proves that the original [matrix](vector-space.md#matrix) has real [eigenvalues](linear-operator-theory.md#eigenvalue) in $[1,4]$ and is an [invertible matrix](linear-algebra.md#invertible-matrix). Directly, both [matrices](vector-space.md#matrix) have [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) $\lambda^2-5\lambda+5$, hence

$$
\lambda_\pm=\frac{5\pm\sqrt5}{2}\approx1.381966,\ 3.618034.
$$

The scaling changes the available bounds, while these [eigenvalues](linear-operator-theory.md#eigenvalue) stay fixed.

<a id="image-diagonal-similarity-scaling-replaces-a-radius-100-gershgorin-disc-by-two-radius-1-discs-while-preserving-both-eigenvalues"></a>
![](gershgorin-diagonal-scaling.png)

**[Figure 14](#image-diagonal-similarity-scaling-replaces-a-radius-100-gershgorin-disc-by-two-radius-1-discs-while-preserving-both-eigenvalues). Diagonal similarity scaling replaces a radius-100 Gershgorin disc by two radius-1 discs while preserving both eigenvalues**.

### Gershgorin stability bound for a variable-coefficient diffusion stencil

↑ **Parent:** [Gershgorin circle theorem](#gershgorin-circle-theorem)

A [symmetric matrix](linear-algebra.md#symmetric-matrix) obtained from a conservative five-point discretization of a [diffusion equation](diffusion-equation.md) has row centre $-s_i/h^2$ and radius at most $s_i/h^2$, where $h>0$ is the grid spacing and $s_i$ is the sum of its four nonnegative edge coefficients. Here the [matrix](vector-space.md#matrix) represents the diffusion generator, with nonnegative off-diagonal entries; boundary elimination may reduce the row radius. If every coefficient is at most $a_{\max}>0$, then $s_i\leq4a_{\max}$, and the [Gershgorin bounds for symmetric matrices](#gershgorin-bounds-for-symmetric-matrices) place every [eigenvalue](linear-operator-theory.md#eigenvalue) in $[-8a_{\max}/h^2,0]$.

For the [forward Euler method](#euler-method), an [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda\leq0$ has amplification factor $1+\Delta t\lambda$. Requiring $|1+\Delta t\lambda|\leq1$ for every such [eigenvalue](linear-operator-theory.md#eigenvalue) gives the sufficient [absolute stability](#linear-stability-domain) condition $\Delta t/h^2\leq1/(4a_{\max})$. Symmetry makes this also prevent growth of the [Euclidean norm](normed-vector-space.md#euclidean-norm). For $a_{\max}=2$ and $h=0.1$, the bound is $\lambda\in[-1600,0]$ and $\Delta t\leq0.00125$. At that step size the [interval](real-analysis.md#interval-mathematics) maps to amplification factors in $[-1,1]$. This illustrates why cheap [Gershgorin disc](#gershgorin-disc) bounds can select a stable time step before any [eigenvalues](linear-operator-theory.md#eigenvalue) are computed.

## Finite difference

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](finite-difference.md)

## Tridiagonal matrix algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tridiagonal_matrix_algorithm)

The [Thomas algorithm](#tridiagonal-matrix-algorithm) is [Gaussian elimination](numerical-linear-algebra.md#gaussian-elimination) specialized to a [tridiagonal matrix](vector-space.md#tridiagonal-matrix): each row couples an unknown only to its immediate neighbours. Eliminating one unknown changes just the next diagonal entry and right-hand side. Provided all [pivot elements](numerical-linear-algebra.md#pivot-element) are nonzero, a forward sweep followed by [back substitution](linear-algebra.md#back-substitution) solves an $n$-unknown [linear system](linear-algebra.md#system-of-linear-equations) in $O(n)$ time and storage, using [Big O notation](real-analysis.md#big-o-notation). Treating the same entries as a full [matrix](vector-space.md#matrix) wastes the zeros: classical dense [LU factorization and solve costs](numerical-linear-algebra.md#lu-factorization-and-solve-costs) grow cubically for factorization and quadratically for storage.

A concrete reason to care is the [Dirichlet Poisson solution by tridiagonal elimination](#dirichlet-poisson-solution-by-tridiagonal-elimination): a three-point [finite difference](finite-difference.md) for the [second derivative](calculus.md#second-derivative) couples adjacent points on a [mesh](finite-element-method.md#finite-element-mesh), producing precisely this [tridiagonal matrix](vector-space.md#tridiagonal-matrix). The same structure occurs in one-dimensional [Crank-Nicolson method](runge-kutta-method.md#crank-nicolson-method) calculations. NPTEL's archived Lecture 13 introduces the [Thomas algorithm](#tridiagonal-matrix-algorithm) from that time-stepping problem and labels the procedure “Thomas algorithm (1949)”.[Lecture 13, Thomas algorithm: opening historical attribution and Crank Nicolson motivation](mathematics-bibliography.md#thomas-algorithm-nptel-lecture-13)

### Tridiagonal elimination recurrences

↑ **Parent:** [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)

Let $n\geq1$. Store the [tridiagonal matrix](vector-space.md#tridiagonal-matrix) $A$ by its diagonal $b_1,\ldots,b_n$, lower diagonal $a_2,\ldots,a_n$, and upper diagonal $c_1,\ldots,c_{n-1}$. The [linear system](linear-algebra.md#system-of-linear-equations) $Ax=d$ is

$$
a_ix_{i-1}+b_ix_i+c_ix_{i+1}=d_i,\qquad 1\leq i\leq n,
$$

with the nonexistent endpoint terms omitted. Initialize $p_1=b_1$ and $g_1=d_1$. For $i=2,\ldots,n$, compute the [elimination multiplier](numerical-linear-algebra.md#elimination-multiplier), modified [pivot element](numerical-linear-algebra.md#pivot-element), and modified right-hand side:

$$
m_i=\frac{a_i}{p_{i-1}},\qquad p_i=b_i-m_ic_{i-1},\qquad g_i=d_i-m_ig_{i-1}.
$$

These [recurrence relations](sequence-and-series.md#recurrence-relation) apply the [elementary row operation](numerical-linear-algebra.md#elementary-row-operation) $R_i\leftarrow R_i-m_iR_{i-1}$ after the preceding row has already been reduced. The transformed [linear system](linear-algebra.md#system-of-linear-equations) is an upper [bidiagonal matrix](vector-space.md#bidiagonal-matrix):

$$
p_ix_i+c_ix_{i+1}=g_i\quad(1\leq i<n),\qquad p_nx_n=g_n.
$$

Thus [back substitution](linear-algebra.md#back-substitution) is especially short:

$$
x_n=\frac{g_n}{p_n},\qquad x_i=\frac{g_i-c_ix_{i+1}}{p_i}\quad(i=n-1,n-2,\ldots,1).
$$

For $n=1$, only $x_1=d_1/b_1$ remains. Check each [pivot element](numerical-linear-algebra.md#pivot-element) before its first [division](arithmetic.md#division-mathematics), including $p_n$ before [back substitution](linear-algebra.md#back-substitution).

<a id="image-tridiagonal-elimination-preserves-the-narrow-band-only-one-row-and-one-diagonal-coefficient-change-per-step"></a>
![](tridiagonal-elimination-band-structure.png)

**[Figure 15](#image-tridiagonal-elimination-preserves-the-narrow-band-only-one-row-and-one-diagonal-coefficient-change-per-step). Tridiagonal elimination preserves the narrow band: only one row and one diagonal coefficient change per step**.

Equivalently, this constructs an [LU decomposition](numerical-linear-algebra.md#lu-decomposition) with unit lower [bidiagonal matrix](vector-space.md#bidiagonal-matrix) $L$, whose lower diagonal is $m_2,\ldots,m_n$, and upper [bidiagonal matrix](vector-space.md#bidiagonal-matrix) $U$, whose diagonal is $p_1,\ldots,p_n$ and upper diagonal is $c_1,\ldots,c_{n-1}$. The $g$ sweep is [forward substitution](numerical-linear-algebra.md#forward-substitution) in $Lg=d$. There is no [fill-in](numerical-linear-algebra.md#fill-in) outside these bands when no rows are interchanged. LAPACK's `DGTSV` source uses these same coefficient and right-hand-side updates in its branch without row interchange.[DGTSV, LAPACK 3.12.1, Fortran lines 175–180: multiplier and two updates without row interchange](mathematics-bibliography.md#dgtsv-lapack-3-12-1-by-lapack-project)

### Dirichlet Poisson solution by tridiagonal elimination

↑ **Parent:** [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)

Consider the original small [Poisson equation](partial-differential-equation.md#poisson-s-equation) example

$$
-u''(x)=2\quad(0<x<1),\qquad u(0)=1,\qquad u(1)=2.
$$

Its exact solution is the [quadratic polynomial](polynomial.md#quadratic-polynomial) $u(x)=1+2x-x^2$. Use a uniform [mesh](finite-element-method.md#finite-element-mesh) $x_i=ih$ with $h=1/4$ and three interior unknowns $U_1,U_2,U_3$. The [finite difference method](finite-difference.md#finite-difference-method) replaces the negative [second derivative](calculus.md#second-derivative) by

$$
\frac{-U_{i-1}+2U_i-U_{i+1}}{h^2}=2.
$$

Multiplying by $h^2$ and moving the prescribed [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) to the right gives

$$
\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix}
\begin{pmatrix}U_1\\U_2\\U_3\end{pmatrix}
=\begin{pmatrix}1+2h^2\\2h^2\\2+2h^2\end{pmatrix}
=\begin{pmatrix}9/8\\1/8\\17/8\end{pmatrix}.
$$

The endpoint values contribute $1$ and $2$ to the first and last equations; they are not additional unknowns. The [Thomas algorithm](#tridiagonal-matrix-algorithm) gives

$$
\begin{array}{c|c|c|c}
i&m_i&p_i&g_i\\\hline
1&\text{unused}&2&9/8\\
2&-1/2&3/2&11/16\\
3&-2/3&4/3&31/12
\end{array}
$$

and [back substitution](linear-algebra.md#back-substitution) yields

$$
U_3=\frac{31}{16},\qquad U_2=\frac74,\qquad U_1=\frac{23}{16}.
$$

All three values equal $u(x_i)$ exactly: the centered [finite difference](finite-difference.md) for the [second derivative](calculus.md#second-derivative) is exact on a [quadratic polynomial](polynomial.md#quadratic-polynomial). This special nodal exactness does not assert exactness for arbitrary forcing or for the piecewise-linear curve joining the nodes.

<a id="image-exact-quadratic-dirichlet-poisson-solution-and-the-three-interior-values-recovered-by-tridiagonal-elimination"></a>
![](dirichlet-poisson-tridiagonal-solution.png)

**[Figure 16](#image-exact-quadratic-dirichlet-poisson-solution-and-the-three-interior-values-recovered-by-tridiagonal-elimination). Exact quadratic Dirichlet Poisson solution and the three interior values recovered by tridiagonal elimination**.

For any $n$ interior points with $h=1/(n+1)$, the scaled [tridiagonal matrix](vector-space.md#tridiagonal-matrix) has $b_i=2$ and $a_i=c_i=-1$. Its [pivot elements](numerical-linear-algebra.md#pivot-element) are $p_i=(i+1)/i$: start at $p_1=2$ and use $p_i=2-1/p_{i-1}$. All are positive. Interior rows have equality in [diagonal dominance](algebra.md#diagonal-dominance), so [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix) is not the reason this example works. Instead it is a [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), since for a real [vector](vector-space.md#vector) $v\ne0$ with $v_0=v_{n+1}=0$,

$$
v^TAv=\sum_{i=0}^{n}(v_{i+1}-v_i)^2>0.
$$

Zero would force every neighbouring value equal and hence all values zero. This connects the boundary constraints directly to the [safe pivots for tridiagonal elimination](#safe-pivots-for-tridiagonal-elimination).

### Safe pivots for tridiagonal elimination

↑ **Parent:** [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)

The displayed [Thomas algorithm](#tridiagonal-matrix-algorithm) requires every modified [pivot element](numerical-linear-algebra.md#pivot-element) to be nonzero in exact [arithmetic](arithmetic.md). Nonzero original diagonal entries alone are insufficient: later [pivot elements](numerical-linear-algebra.md#pivot-element) can vanish after elimination. Two useful sufficient contexts are a real [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix), and [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix) by rows:

$$
|b_i|>|a_i|+|c_i|\quad(1\leq i\leq n),\qquad a_1=c_n=0.
$$

For the [symmetric positive-definite matrix](linear-algebra.md#symmetric-positive-definite-matrix) case, elimination leaves positive-definite remaining blocks by the [Schur complement](linear-algebra.md#schur-complement), so each $p_i>0$. Equivalently, the initial [principal minors](vector-space.md#principal-minor) $\Delta_i=\det A_{1:i,1:i}$ are positive, and $p_i=\Delta_i/\Delta_{i-1}$ with $\Delta_0=1$.

For [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix), a short induction shows $|p_i|>|c_i|$. The first row gives $|p_1|=|b_1|>|c_1|$. Assuming the preceding bound, the [triangle inequality](topological-analysis.md#triangle-inequality) gives

$$
|p_i|\geq|b_i|-\frac{|a_i|\,|c_{i-1}|}{|p_{i-1}|}\geq|b_i|-|a_i|>|c_i|.
$$

In particular $p_n\ne0$. These are structural guarantees against a zero [pivot element](numerical-linear-algebra.md#pivot-element), not universal bounds on forward error in [floating-point arithmetic](floating-point-arithmetic.md). A poorly conditioned [linear system](linear-algebra.md#system-of-linear-equations) can still amplify [roundoff error](#round-off-error); [numerical stability](#stability-of-a-numerical-method) and the [condition number](quadratic-form.md#condition-number) must be distinguished.

### Zero-pivot failure of tridiagonal elimination

↑ **Parent:** [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)

An [invertible matrix](linear-algebra.md#invertible-matrix) need not admit the unpivoted [Thomas algorithm](#tridiagonal-matrix-algorithm). For example,

$$
A=\begin{pmatrix}0&1\\1&1\end{pmatrix},\qquad d=\begin{pmatrix}2\\3\end{pmatrix},\qquad x=\begin{pmatrix}1\\2\end{pmatrix}.
$$

Here $\det A=-1$ and $Ax=d$, but $p_1=0$ makes $m_2=1/0$ undefined. Interchanging the two equations instead gives the upper [triangular matrix](linear-algebra.md#triangular-matrix) system $x_1+x_2=3$, $x_2=2$, solved immediately by [back substitution](linear-algebra.md#back-substitution). Even a nonzero first diagonal does not guarantee all later [pivot elements](numerical-linear-algebra.md#pivot-element): $\begin{pmatrix}1&1&0\\1&1&1\\0&1&1\end{pmatrix}$ has [determinant](multilinear-algebra.md#determinant) $-1$, yet $p_2=1-1=0$.

For a general [tridiagonal matrix](vector-space.md#tridiagonal-matrix), use a solver with [partial pivoting](numerical-linear-algebra.md#columnwise-partial-pivoting) when these structural guarantees are unavailable or a dangerously small [pivot element](numerical-linear-algebra.md#pivot-element) occurs. Adjacent row interchanges can introduce a second upper diagonal, so a pivoted solver must track that additional [fill-in](numerical-linear-algebra.md#fill-in); it cannot blindly continue the unpivoted [recurrence relations](sequence-and-series.md#recurrence-relation). LAPACK's `DGTSV` explicitly performs [partial pivoting](numerical-linear-algebra.md#columnwise-partial-pivoting), stores this extra upper diagonal, and includes it in [back substitution](linear-algebra.md#back-substitution). Its fixed-width storage and bounded work per row retain $O(n)$ time for one right-hand side and $O(n)$ storage.[DGTSV, Purpose lines 34–39; DL argument lines 63–69; adjacent interchange lines 188–199; back solve lines 295–305](mathematics-bibliography.md#dgtsv-lapack-3-12-1-by-lapack-project)

### Tridiagonal solve costs

↑ **Parent:** [Tridiagonal matrix algorithm](#tridiagonal-matrix-algorithm)

For the displayed unpivoted [Thomas algorithm](#tridiagonal-matrix-algorithm) with one right-hand side, count each scalar [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), [multiplication](arithmetic.md#multiplication) or [division](arithmetic.md#division-mathematics) as one [arithmetic operation](#arithmetic-operation). Forming $m_i,p_i,g_i$ takes five [arithmetic operations](#arithmetic-operation) per forward step. The last unknown takes one [division](arithmetic.md#division-mathematics); each remaining [back substitution](linear-algebra.md#back-substitution) step takes three [arithmetic operations](#arithmetic-operation). Thus

$$
5(n-1)+1+3(n-1)=8n-7.
$$

This is an operation-count model, excluding assignments, indexing, pivot checks and any special simplifications of the coefficients. It is not a timing benchmark. The original [tridiagonal matrix](vector-space.md#tridiagonal-matrix) needs $3n-2$ scalar entries, and its right-hand side another $n$. Overwriting $b_i$ with $p_i$ and $d_i$ with $g_i$, then with $x_i$, keeps storage $O(n)$; the arrays, rather than the few loop temporaries, determine the total [space complexity](theoretical-computer-science.md#space-complexity).

For repeated right-hand sides, retain the [LU decomposition](numerical-linear-algebra.md#lu-decomposition): computing $m_i,p_i$ once costs $3(n-1)$ [arithmetic operations](#arithmetic-operation), and each subsequent pair of [forward substitution](numerical-linear-algebra.md#forward-substitution) and [back substitution](linear-algebra.md#back-substitution) sweeps costs $5n-4$. Hence $r$ right-hand sides cost $3(n-1)+r(5n-4)$ [arithmetic operations](#arithmetic-operation). This is the banded counterpart of [Reusing LU factors for multiple right-hand sides](numerical-linear-algebra.md#reusing-lu-factors-for-multiple-right-hand-sides).

## Gaussian quadrature

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_quadrature)

[Gaussian quadrature](#gaussian-quadrature) is a [quadrature rule](numerical-integration.md#quadrature-rule) that chooses both sample locations and coefficients to achieve unusually high [polynomial](polynomial.md) exactness. For a finite [interval](real-analysis.md#interval-mathematics) $[a,b]$ with $a<b$, assume the integration weight $w$ is integrable and positive almost everywhere. Define

$$
I_w(f)=\int_a^b f(x)w(x)\,dx,\qquad Q_n(f)=\sum_{i=1}^n A_i f(x_i),\qquad n\geq1.
$$

Let $p_n$ be the [monic orthogonal polynomial](orthogonal-polynomial.md#monic-orthogonal-polynomial) of [polynomial degree](polynomial.md#degree-of-a-polynomial) $n$ for the [inner product](inner-product.md) $\langle u,v\rangle_w=\int_a^b u(x)v(x)w(x)\,dx$: it satisfies $\langle p_n,q\rangle_w=0$ for every [polynomial](polynomial.md) $q$ of [polynomial degree](polynomial.md#degree-of-a-polynomial) below $n$. The [polynomial roots](polynomial.md#root-of-a-polynomial) of $p_n$ are distinct and inside $(a,b)$; take them as the nodes $x_i$. Integrate the [Lagrange cardinal polynomials](interpolation.md#lagrange-cardinal-polynomial) $\ell_i$ to obtain $A_i=I_w(\ell_i)$. These coefficients are positive, and

$$
Q_n(f)=I_w(f)\qquad\text{for every polynomial }f\text{ with }\deg f\leq2n-1.
$$

The integration weight $w(x)$ and the discrete coefficients $A_i$ play different roles: $w$ specifies the [integral](integral.md) being approximated, while $A_i$ tell us how much each sample contributes.[Nico M. Temme, NIST Digital Library of Mathematical Functions, §3.5(v), Gauss quadrature: nodes, coefficients and exactness](https://dlmf.nist.gov/3.5#v)

A proof outline explains the gain over simply integrating an arbitrary [polynomial interpolation](interpolation.md#polynomial-interpolation). Use [polynomial division](polynomial.md#polynomial-division) to write $f=p_nq+r$, with $\deg q\leq n-1$ and $\deg r\leq n-1$. [Orthogonality](inner-product.md#orthogonal-vectors) makes $I_w(p_nq)=0$, and sampling at the [polynomial roots](polynomial.md#root-of-a-polynomial) of $p_n$ makes $Q_n(p_nq)=0$. The [Lagrange cardinal polynomials](interpolation.md#lagrange-cardinal-polynomial) recover $r$ exactly, so both expressions agree. Also $A_i=Q_n(\ell_i^2)=I_w(\ell_i^2)>0$, since $\ell_i^2$ has [polynomial degree](polynomial.md#degree-of-a-polynomial) $2n-2$. This is the mechanism behind [positive weights of Gaussian quadrature](#positive-weights-of-gaussian-quadrature).

For a concrete two-node example, set $w=1$ on $[-1,1]$. The [Legendre polynomial](linear-ordinary-differential-equation.md#legendre-polynomial) $P_2(x)=(3x^2-1)/2$ has [polynomial roots](polynomial.md#root-of-a-polynomial) $x=\pm1/\sqrt3$. Its [monic polynomial](polynomial.md#monic-polynomial) version $p_2=x^2-1/3$ has zero [integral](integral.md) against both $1$ and $x$, as required. Symmetry and exactness for the constant [polynomial](polynomial.md) give $A_1=A_2=1$. Thus the Gauss–Legendre instance of [Gaussian quadrature](#gaussian-quadrature) is

$$
\int_{-1}^1 f(x)\,dx\ \approx\ f(-1/\sqrt3)+f(1/\sqrt3).
$$

Direct evaluation on $1,x,x^2,x^3$ gives $2,0,2/3,0$, exactly their [integrals](integral.md). For the [polynomial](polynomial.md) $f(x)=1+x+x^2+x^3$, two samples therefore give $8/3$ exactly. But for $x^4$ the rule gives $2/9$, whereas the [integral](integral.md) is $2/5$: the error $I_1-Q_2$ is $8/45$.

<a id="image-analytical-illustration-of-two-node-gauss-legendre-sampling-exact-monomial-integrals-through-degree-three-and-failure-at-degree-four"></a>
![](gaussian-quadrature-chebyshev-legendre-exactness.png)

**[Figure 17](#image-analytical-illustration-of-two-node-gauss-legendre-sampling-exact-monomial-integrals-through-degree-three-and-failure-at-degree-four). Analytical illustration of two-node Gauss–Legendre sampling: exact monomial integrals through degree three and failure at degree four**.

The ceiling $2n-1$ is sharp for $n$ distinct real nodes under the positive-weight assumptions. Their squared nodal [polynomial](polynomial.md) $\prod_i(x-x_i)^2$ has [polynomial degree](polynomial.md#degree-of-a-polynomial) $2n$, is zero at every sample, and has a strictly positive weighted [integral](integral.md). Thus no such [quadrature rule](numerical-integration.md#quadrature-rule) integrates every [polynomial](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) $2n$ exactly. Nor does [Gaussian quadrature](#gaussian-quadrature) integrate every nonpolynomial [function](function.md) exactly: the same two-node example gives $Q_2(|x|)=2/\sqrt3$, while $I_1(|x|)=1$.

[Gaussian quadrature](#gaussian-quadrature) is useful when evaluations are costly and a modest [polynomial](polynomial.md) captures the integrand well. More precisely, for a [continuous function](calculus.md#continuous-function) $f$ and any [polynomial](polynomial.md) $r$ of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $2n-1$, positivity and constant exactness give

$$
|I_w(f)-Q_n(f)|\leq2I_w(1)\,\|f-r\|_\infty.
$$

The [uniform norm](normed-vector-space.md#supremum-norm) on $[a,b]$ measures the approximation between samples. This bound connects [quadrature rule](numerical-integration.md#quadrature-rule) accuracy to [uniform approximation](uniform-approximation.md), rather than promising an error from sample count alone. Corners, sharp unresolved features and [roundoff error](#round-off-error) require their own assessment; the [absolute value function](real-analysis.md#absolute-value) example already shows why [polynomial](polynomial.md) exactness is a qualified guarantee.

### Gauss-Legendre quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

Gauss-Legendre quadrature approximates an [integral](integral.md) on a finite interval using nodes obtained from roots of a [Legendre polynomial](linear-ordinary-differential-equation.md#legendre-polynomial). With $n$ nodes it integrates every [polynomial](polynomial.md) of degree at most $2n-1$ exactly.

### Orthogonal-node criterion for Gaussian quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

An $(n+1)$-node quadrature exact on degree $n$ is exact through degree $2n+1$ precisely when its node polynomial $p=\prod_i(x-x_i)$ is [orthogonal](inner-product.md#orthogonal-vectors) to every degree-$n$ [polynomial](polynomial.md) for the integration weight. Necessity applies the rule to $pr$. Sufficiency divides an arbitrary degree-$2n+1$ polynomial as $pq+r$, with both $q,r$ of degree at most $n$; the integral and quadrature of $pq$ vanish while both agree on $r$.

### Two-node Gaussian quadrature with quadratic weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

The even weight $1-x^2$ has moments $m_0=4/3$ and $m_2=4/15$. Its monic quadratic orthogonal polynomial is $x^2-1/5$, so the two [Gaussian quadrature](#gaussian-quadrature) nodes are $\pm1/\sqrt5$. Symmetry and constant exactness give weights $2/3$ each. These nodes and weights integrate every polynomial of degree at most three exactly. Degree four fails: the true integral is $4/35$, whereas the rule gives $4/75$.

<h3 id="chebyshev-gauss-quadrature">Chebyshev–Gauss quadrature</h3>

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev–Gauss_quadrature)

The first-kind rule approximates $\int_{-1}^1 f(x)(1-x^2)^{-1/2}\,dx$ at the zeros of the [Chebyshev polynomial](#chebyshev-polynomial) $T_n$. It integrates all [polynomials](polynomial.md) of degree at most $2n-1$ exactly. The weights follow by integrating the [Lagrange interpolation polynomial](interpolation.md#lagrange-polynomial) at those nodes. Orthogonality kills the quotient when a degree-$2n-1$ polynomial is divided by $T_n$; its remainder is recovered by interpolation. No $n$-node rule can integrate every degree-$2n$ polynomial, since the squared nodal polynomial has zero quadrature sum and strictly positive weighted integral.

// Target: probability-and-statistics.bigb

### Gauss-Laguerre quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Laguerre_quadrature)

For the weight $e^{-x}$ on $[0,\infty)$, use the zeros of a degree-$n$ [Laguerre polynomial](linear-operator-theory.md#laguerre-polynomial) as quadrature nodes. Divide a polynomial of degree at most $2n-1$ by that polynomial. The quotient term integrates to zero by orthogonality and vanishes at every node; interpolation of the remainder proves exactness. The two-node rule has nodes $2\pm\sqrt2$ and corresponding weights $(2\pm\sqrt2)/4$, with the larger weight at the smaller node.

### Two-node Gaussian quadrature with linear weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For weight $w(x)=x$ on $[0,1]$, the two-node [Gaussian quadrature](#gaussian-quadrature) nodes are roots of $x^2-6x/5+3/10$, the monic quadratic orthogonal to all linear [polynomials](polynomial.md). Its weights come from integrating the [Lagrange interpolation](interpolation.md#lagrange-polynomial) cardinal functions. Orthogonality gives exactness on cubic [polynomials](polynomial.md) and positive weights.

### Two-node Gaussian quadrature with sine weight

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For integration against $\sin x$ on $[0,\pi]$, the monic quadratic [orthogonal polynomial](orthogonal-polynomial.md) is $x^2-\pi x+2$. Its two roots are the [Gaussian quadrature](#gaussian-quadrature) nodes $c_{1,2}=\pi/2\mp\sqrt{\pi^2/4-2}$, with weights one. The rule integrates every cubic exactly: divide it by the orthogonal quadratic and integrate the degree-one remainder.

### Positive weights of Gaussian quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)

For an $n$-node [Gaussian quadrature](#gaussian-quadrature) rule exact through degree $2n-1$, the cardinal [Lagrange interpolation polynomial](interpolation.md#lagrange-polynomial) $\ell_j$ has square of degree $2n-2$. Exactness gives $A_j=\int\ell_j^2>0$ for a positive integration weight. This proof turns [polynomial](polynomial.md) exactness directly into positivity.

### Gauss-Hermite quadrature

↑ **Parent:** [Gaussian quadrature](#gaussian-quadrature)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss-Hermite_quadrature)

Gauss-Hermite quadrature uses the roots of a degree-$N$ [Hermite polynomial](orthogonal-polynomial.md#hermite-polynomial) as nodes for an integral with Gaussian weight. Its positive interpolation weights make it exact for every polynomial of degree at most $2N-1$.

## Lobatto quadrature

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

An $s$-node Lobatto quadrature rule includes both endpoints and is exact for [polynomials](polynomial.md) of degree at most $2s-3$. On $[-1,1]$, its interior nodes are the zeros of the derivative of the degree-$(s-1)$ [Legendre polynomial](linear-ordinary-differential-equation.md#legendre-polynomial). The three-node rule on $[0,1]$ has nodes $0,1/2,1$ and weights $1/6,2/3,1/6$. Integrating the interpolation basis from zero to each node gives the three-stage [Lobatto IIIA method](runge-kutta-method.md#lobatto-iiia-method).

## Chebyshev polynomial

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_polynomial)

The first-kind [Chebyshev polynomial](#chebyshev-polynomial) $T_n$ converts a multiple-angle [cosine](geometry-and-topology.md#cosine) into a [polynomial](polynomial.md):

$$
T_n(\cos\theta)=\cos(n\theta),\qquad 0\leq\theta\leq\pi,\quad n\geq0.
$$

The [cosine addition formula](geometry-and-topology.md#cosine-addition-formula) gives the [recurrence relation](sequence-and-series.md#recurrence-relation)

$$
T_0(x)=1,\qquad T_1(x)=x,\qquad T_{n+1}(x)=2xT_n(x)-T_{n-1}(x)\quad(n\geq1).
$$

This constructs [polynomials](polynomial.md) valid for every real $x$, including outside $[-1,1]$, where the real-angle description is unavailable. For example,

$$
T_2(x)=2x^2-1,\qquad T_3(x)=4x^3-3x,\qquad T_4(x)=8x^4-8x^2+1.
$$

For $n\geq1$, $T_n$ has [polynomial degree](polynomial.md#degree-of-a-polynomial) $n$ and leading coefficient $2^{n-1}$. On $[-1,1]$ its [uniform norm](normed-vector-space.md#supremum-norm) is one, even as its oscillations become more numerous.[T. H. Koornwinder and collaborators, NIST Digital Library of Mathematical Functions, §18.5(i), equation 18.5.1: trigonometric representation](https://dlmf.nist.gov/18.5#i)[Koornwinder and collaborators, NIST DLMF, §18.9(i), Table 18.9.1: recurrence coefficients](https://dlmf.nist.gov/18.9#i)

The [polynomial roots](polynomial.md#root-of-a-polynomial) of $T_n$ are especially simple:

$$
x_k=\cos\!\left(\frac{(2k-1)\pi}{2n}\right),\qquad k=1,\ldots,n.
$$

They correspond to equally spaced angles, but their locations in $x$ cluster near $-1$ and $1$. For $T_3$, the [polynomial roots](polynomial.md#root-of-a-polynomial) are $\sqrt3/2,0,-\sqrt3/2$. For $T_8$, the positive [polynomial roots](polynomial.md#root-of-a-polynomial) are approximately $0.980785,0.831470,0.555570,0.195090$, with their negatives completing the set. The distance from the right endpoint to the nearest [polynomial root](polynomial.md#root-of-a-polynomial) is $1-\cos(\pi/(2n))\sim\pi^2/(8n^2)$; central neighboring [polynomial roots](polynomial.md#root-of-a-polynomial) are separated on the larger scale $1/n$. The small change of [cosine](geometry-and-topology.md#cosine) near angles zero and $\pi$ explains the clustering.

<a id="image-analytical-illustration-of-the-eight-roots-of-t8-equally-spaced-angles-on-a-semicircle-project-to-endpoint-clustered-interpolation-nodes"></a>
![](gaussian-quadrature-chebyshev-root-projection.png)

**[Figure 18](#image-analytical-illustration-of-the-eight-roots-of-t8-equally-spaced-angles-on-a-semicircle-project-to-endpoint-clustered-interpolation-nodes). Analytical illustration of the eight roots of T8: equally spaced angles on a semicircle project to endpoint-clustered interpolation nodes**.

These [polynomial roots](polynomial.md#root-of-a-polynomial) supply $n$ [interpolation nodes](interpolation.md#interpolation-node) for a [polynomial interpolation](interpolation.md#polynomial-interpolation) of [polynomial degree](polynomial.md#degree-of-a-polynomial) at most $n-1$. They differ from the $n+1$ [Chebyshev-Lobatto nodes](interpolation.md#chebyshev-lobatto-node) $\cos(j\pi/n)$, which include both endpoints. This choice of [polynomial roots](polynomial.md#root-of-a-polynomial) has nodal [polynomial](polynomial.md)

$$
\prod_{k=1}^n(x-x_k)=2^{1-n}T_n(x).
$$

The [monic Chebyshev extremal polynomial](#monic-chebyshev-extremal-polynomial) minimizes the [uniform norm](normed-vector-space.md#supremum-norm) of this product among [monic polynomials](polynomial.md#monic-polynomial) of [polynomial degree](polynomial.md#degree-of-a-polynomial) $n$ on $[-1,1]$. Consequently, if $f$ has $n$ continuous [derivatives](calculus.md#derivative), the usual [polynomial interpolation error](algebra.md#polynomial-interpolation-error) gives the useful bound

$$
\|f-p\|_\infty\leq\frac{2^{1-n}}{n!}\max_{-1\leq x\leq1}|f^{(n)}(x)|,\qquad\deg p\leq n-1.
$$

This optimizes the nodal factor in that bound, not the actual error for every [function](function.md). Endpoint clustering helps control the large endpoint oscillations of [equally spaced interpolation](#equally-spaced-interpolation) associated with [Runge's phenomenon](interpolation.md#runge-s-phenomenon). The two node conventions and their geometric construction are discussed in Trefethen's authored text.[Lloyd N. Trefethen, Approximation Theory and Approximation Practice, Chapters 2–3 and Exercise 2.4: endpoint clustering, first-kind roots and polynomials](https://people.maths.ox.ac.uk/trefethen/ATAP/ATAPfirst6chapters.pdf)

The same [cosine substitution for polynomial approximation](uniform-approximation.md#cosine-substitution-for-polynomial-approximation) explains the weighted [orthogonality](inner-product.md#orthogonal-vectors):

$$
\int_{-1}^1\frac{T_m(x)T_n(x)}{\sqrt{1-x^2}}\,dx=\int_0^\pi\cos(m\theta)\cos(n\theta)\,d\theta=\begin{cases}0,&m\ne n,\\\pi,&m=n=0,\\\pi/2,&m=n\geq1.\end{cases}
$$

The endpoint singularities of the weight are integrable. Thus the [Chebyshev polynomials](#chebyshev-polynomial) are [orthogonal polynomials](orthogonal-polynomial.md) for this weight, making coefficients in a [least-squares polynomial in an orthogonal-polynomial basis](inner-product.md#least-squares-polynomial-in-an-orthogonal-polynomial-basis) separate cleanly. Their [polynomial roots](polynomial.md#root-of-a-polynomial) also give [Chebyshev–Gauss quadrature](#chebyshev-gauss-quadrature), connecting [polynomial interpolation](interpolation.md#polynomial-interpolation) to [Gaussian quadrature](#gaussian-quadrature).[NIST Digital Library of Mathematical Functions; Koornwinder and collaborators, NIST DLMF, §18.3, Table 18.3.1: first-kind Chebyshev weight and normalization](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/18-orthogonal-polynomials)

Accuracy still depends on the target [function](function.md). The [absolute value function](real-analysis.md#absolute-value) $|x|$ has a corner at zero, so the hypothesis requiring continuous [derivatives](calculus.md#derivative) in the displayed [polynomial interpolation error](algebra.md#polynomial-interpolation-error) bound fails. Endpoint clustering cannot remove that corner. A jump poses a stronger obstruction: [polynomials](polynomial.md) are [continuous functions](calculus.md#continuous-function), so they cannot converge in the [uniform norm](normed-vector-space.md#supremum-norm) to a discontinuous [function](function.md) on the whole [interval](real-analysis.md#interval-mathematics). Chebfun's documented examples show persistent overshoot for such jumps; these are a limitation of global [polynomial interpolation](interpolation.md#polynomial-interpolation), not a universal promise of rapid accuracy from [Chebyshev polynomials](#chebyshev-polynomial).[Chebfun development team, Chebfun Guide, §4.3: polynomial interpolation of discontinuous functions](https://www.chebfun.org/docs/guide/guide04.html#4.3)

### Chebyshev projection of a semicircle

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

For weighted [least-squares polynomial in an orthogonal-polynomial basis](inner-product.md#least-squares-polynomial-in-an-orthogonal-polynomial-basis) with weight $(1-x^2)^{-1/2}$ on $[-1,1]$, the projection of $\sqrt{1-x^2}$ onto [polynomials](polynomial.md) of degree at most $n$ is the displayed sum. Put $x=\cos\theta$ to obtain $T_j(x)=\cos j\theta$ and $f(x)=\sin\theta$ on $[0,\pi]$. The constant coefficient is $2/\pi$, odd coefficients vanish, and the coefficient of $T_{2m}$ is $4/[\pi(1-4m^2)]$. For odd $n$ the optimal [polynomial](polynomial.md) can have degree $n-1$.

### Chebyshev nodal derivative comparison

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)

Let $x_j=\cos((2j-1)\pi/(2n))$ be the roots of the [Chebyshev polynomial](#chebyshev-polynomial), and let $q$ have degree at most $n-1$ with $|q(x_j)|\le |T_n'(x_j)|$. Its [Lagrange interpolation polynomial](interpolation.md#lagrange-polynomial) uses basis $\ell_j(x)=T_n(x)/[(x-x_j)T_n'(x_j)]$. For $x>x_1$, $T_n(x)>0$ and $x-x_j>0$, so $\ell_j(x)T_n'(x_j)>0$. Therefore $|q(x)|\le\sum_j|\ell_j(x)T_n'(x_j)|=T_n'(x)$, the last equality being interpolation of the derivative. Continuity includes $x=x_1$ and reflection proves the left-hand region.

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

On real polynomials of degree at most $n\geq1$ with the [uniform norm](normed-vector-space.md#supremum-norm) on $[-1,1]$, set $x_j=\cos(j\pi/n)$ and let $\ell_j$ be the [Lagrange interpolation](interpolation.md#lagrange-polynomial) basis. If $u>1$, the denominator of $\ell_j(u)$ has exactly $j$ negative factors while its numerator is positive. Therefore $|\ell_j(u)|=(-1)^j\ell_j(u)$. Since $T_n(x_j)=(-1)^j$, interpolation gives $\sum_j|\ell_j(u)|=T_n(u)$. Hence $|P(u)|\leq\|P\|_\infty T_n(u)$, and $P=T_n$ attains equality. Reflection and Chebyshev parity give the case $u<-1$. Dividing the interpolation weights by $T_n(u)$ yields an exact signed evaluation representation of norm one on $n+1$ nodes. Constants give the immediate degree-zero case.

### Chebyshev differential equation

↑ **Parent:** [Chebyshev polynomial](#chebyshev-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_differential_equation)

The equation $(1-z^2)w''-zw'+n^2w=0$ is obtained from the harmonic equation $w_{xx}+n^2w=0$ by $z=\cos x$.

#### Neumann eigenfunctions of the Chebyshev differential operator

↑ **Parent:** [Chebyshev differential equation](#chebyshev-differential-equation)

With the [weighted inner product](inner-product.md#weighted-inner-product) $\int_{-1}^1\overline f g\,dx/\sqrt{1-x^2}$, the [Chebyshev differential equation](#chebyshev-differential-equation) has the [Sturm-Liouville form](sturm-liouville-theory.md#sturm-liouville-form) with coefficients $p=\sqrt{1-x^2}$, $w=(1-x^2)^{-1/2}$ and $q=0$. The substitution $x=\cos\theta$ converts its operator to $-d^2/d\theta^2$ on $(0,\pi)$ and its inner product to the ordinary one in $d\theta$. The natural endpoint conditions $py'\to0$ become zero derivative conditions at $\theta=0,\pi$.

Consequently the [eigenfunctions](linear-operator-theory.md#eigenfunction) are the [Chebyshev polynomials](#chebyshev-polynomial) $T_n(x)=\cos(n\arccos x)$ with [eigenvalues](linear-operator-theory.md#eigenvalue) $n^2$, $n=0,1,2,\ldots$. Their squared norms are $\pi$ for $n=0$ and $\pi/2$ otherwise. In particular $T_1=x$ and $T_3=4x^3-3x$ are orthogonal. The endpoints of the original differential expression are singular; specifying these transformed [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) defines its self-adjoint realization. The [Dirichlet eigenfunctions of the Chebyshev differential operator](#dirichlet-eigenfunctions-of-the-chebyshev-differential-operator) use a different endpoint condition and have sine rather than cosine profiles.

#### Dirichlet eigenfunctions of the Chebyshev differential operator

↑ **Parent:** [Chebyshev differential equation](#chebyshev-differential-equation)

The [Chebyshev differential equation](#chebyshev-differential-equation) $-(1-x^2)y''+xy'=\lambda y$ on $-1<x<1$, with zero endpoint values, has the [Sturm-Liouville form](sturm-liouville-theory.md#sturm-liouville-form)

$$
-\frac d{dx}\left[\sqrt{1-x^2}\,y'\right]=\lambda\frac{y}{\sqrt{1-x^2}}.
$$

Thus $p=\sqrt{1-x^2}$ and the weight defining the [weighted inner product](inner-product.md#weighted-inner-product) is $w=(1-x^2)^{-1/2}$. The substitution $x=\cos\theta$ maps the problem to $-Y''=\lambda Y$ on $0<\theta<\pi$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). It also transforms $w(x)\,dx$ into $-d\theta$. Consequently the normalized [eigenfunctions](linear-operator-theory.md#eigenfunction) are

$$
\boxed{y_n(x)=\sqrt{\frac2\pi}\sin(n\arccos x),\qquad\lambda_n=n^2,\quad n=1,2,\ldots.}
$$

Their [weighted inner product](inner-product.md#weighted-inner-product) is the ordinary sine [inner product](inner-product.md) on $[0,\pi]$. Equivalently, $y_n=\sqrt{2/\pi}\sqrt{1-x^2}\,U_{n-1}(x)$, where $U_{n-1}$ is a [Chebyshev polynomial of the second kind](#chebyshev-polynomial-of-the-second-kind). These are not the cosine solutions $T_n$, which have different endpoint values. The original endpoints are singular because $p$ vanishes and $w$ diverges there, but the transformed Dirichlet problem specifies the self-adjoint realization. The eigenfunctions vanish at both endpoints and their quasi-derivatives $py_n'$ have finite limits, so the boundary form vanishes.

#### Power series of the Chebyshev differential equation

↑ **Parent:** [Chebyshev differential equation](#chebyshev-differential-equation)

For the [Chebyshev differential equation](#chebyshev-differential-equation) $(1-x^2)y''-xy'+k^2y=0$, a [power series](sequence-and-series.md#power-series) about the [ordinary point](complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation) zero splits into even and odd solutions with the displayed [recurrence relation](sequence-and-series.md#recurrence-relation). Every nonterminating parity series has [radius of convergence](sequence-and-series.md#radius-of-convergence) one. If $k^2=m^2$ for a nonnegative integer $m$, the parity series containing $x^m$ terminates, giving a [polynomial](polynomial.md) with infinite [radius of convergence](sequence-and-series.md#radius-of-convergence); the other independent series still has radius one. Normalized solutions are $\cos(k\arcsin x)$ and $\sin(k\arcsin x)/k$, with the latter replaced by $\arcsin x$ when $k=0$.

#### Regular solution of a forced Chebyshev equation

↑ **Parent:** [Chebyshev differential equation](#chebyshev-differential-equation)

For noninteger real $\gamma$, expand a smooth forcing as $F=\sum_{n\geq0}F_nT_n$ in [Chebyshev polynomials](#chebyshev-polynomial). Because $(1-x^2)T_n''-xT_n'=-n^2T_n$, division of each coefficient by $\gamma^2-n^2$ gives the regular solution. The coefficients use the [weighted inner product](inner-product.md#weighted-inner-product) with weight $(1-x^2)^{-1/2}$. Choosing the same endpoint domain as the regular [eigenfunctions](linear-operator-theory.md#eigenfunction) of the [Sturm-Liouville problem](sturm-liouville-theory.md#sturm-liouville-problem) is essential: finite values alone also allow homogeneous solutions $\cos(\gamma\arccos x)$ and $\sin(\gamma\arccos x)$, which generally have divergent endpoint derivatives. Setting $x=\cos\theta$ converts the regular endpoint condition into the [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) $Z_\theta(0)=Z_\theta(\pi)=0$. The homogeneous equation then has no nonzero solution when $\gamma$ is noninteger, proving uniqueness in this domain.

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

The displayed implicit [linear multistep method](linear-multistep-method.md) is second order and [A-stable](#a-stability). It is the $\alpha=4/3$ member of the [trapezoidal-BDF two-step family](linear-multistep-method.md#trapezoidal-bdf-two-step-family), whose order and boundary-locus proof establish both properties. Its derivative formula uses three equally spaced values; changing the steps requires different coefficients.

### BDF2 discrete energy identity

↑ **Parent:** [Backward differentiation formula](#backward-differentiation-formula)

For three [vectors](vector-space.md#vector) $a,b,c$ in an [inner product space](inner-product.md#inner-product-space), expansion of each squared [norm](normed-vector-space.md#norm) proves

$$
2\operatorname{Re}\langle3a-4b+c,a\rangle
=\|a\|^2+\|2a-b\|^2-\|b\|^2-\|2b-c\|^2+\|a-2b+c\|^2.
$$

Therefore the second-order [backward differentiation formula](#backward-differentiation-formula) $3U^{n+2}-4U^{n+1}+U^n=2kLU^{n+2}$ with a [dissipative operator](functional-analysis.md#dissipative-operator) $L$ decreases the discrete [energy](energy.md) $\mathcal E_n=\|U^{n+1}\|^2+\|2U^{n+1}-U^n\|^2$. This [quadratic form](quadratic-form.md) is equivalent to the product [norm](normed-vector-space.md#norm) of the two time levels with constants independent of $k$ and $L$. It proves uniform [stability](#stability-of-a-numerical-method) even when amplification [roots of a polynomial](polynomial.md#root-of-a-polynomial) coalesce inside the unit disk, where an eigenvector-separation proof may lose its bound.

## Constrained optimization

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constrained_optimization)

### Constraint reparameterization

↑ **Parent:** [Constrained optimization](#constrained-optimization)

Represent feasible variables using unconstrained coordinates. For example, $x=a+e^y$ enforces $x>a$, while $x=a+y^2$ includes $x=a$ but introduces a stationary point at $y=0$. A transformation can change conditioning and does not remove a nonconvex objective's multiple extrema.

### Optimization constraint

↑ **Parent:** [Constrained optimization](#constrained-optimization)

An optimization constraint restricts the feasible points in [constrained optimization](#constrained-optimization), for example by an equality $g(x)=0$ or an inequality $h(x)\leq0$. Extrema are considered on the resulting feasible set rather than on the whole domain of the objective.

## Equally spaced interpolation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equally_spaced_interpolation)

## Givens rotation

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Givens_rotation)

A [Givens rotation](#givens-rotation) eliminates one component of a [vector](vector-space.md#vector) by rotating just two coordinates, preserving its [Euclidean norm](normed-vector-space.md#euclidean-norm). For example,

$$
\begin{pmatrix}3/5&4/5\\-4/5&3/5\end{pmatrix}
\begin{pmatrix}3\\4\end{pmatrix}
=\begin{pmatrix}5\\0\end{pmatrix}.
$$

The length remains five: elimination moves the component into the retained coordinate rather than discarding it. Applied to a [matrix](vector-space.md#matrix), the same operation mixes two rows; [QR decomposition by Givens rotations](#qr-decomposition-by-givens-rotations) uses these local operations to build an [upper triangular matrix](linear-algebra.md#upper-triangular-matrix).

<a id="image-a-givens-rotation-takes-3-4-t-clockwise-to-5-0-t-while-preserving-the-euclidean-norm"></a>
![](givens-rotation-geometry.png)

**[Figure 19](#image-a-givens-rotation-takes-3-4-t-clockwise-to-5-0-t-while-preserving-the-euclidean-norm). A Givens rotation takes $(3,4)^T$ clockwise to $(5,0)^T$ while preserving the Euclidean norm**.

For indices $i<j$, the [matrix](vector-space.md#matrix) $G_{ij}(c,s)$ is the [identity matrix](vector-space.md#identity-matrix) except for its block on coordinates $i,j$:

$$
G\big|_{i,j}=\begin{pmatrix}c&s\\-s&c\end{pmatrix},\qquad c^2+s^2=1.
$$

This article uses left [matrix multiplication](vector-space.md#matrix-multiplication) on column [vectors](vector-space.md#vector). If $c=\cos\theta$ and $s=\sin\theta$, the block is a [rotation matrix](linear-algebra.md#rotation-matrix) through angle $-\theta$: the minus sign belongs in the lower left. Its [transpose](vector-space.md#transpose) reverses the [rotation](riemannian-geometry.md#rotation-mathematics). Direct multiplication gives $G^TG=I$ and [determinant](multilinear-algebra.md#determinant) one, so it is an [orthogonal matrix](linear-algebra.md#orthogonal-matrix); consequently $\|Gx\|_2^2=x^TG^TGx=\|x\|_2^2$. Only two coordinates change, but this [Euclidean norm](normed-vector-space.md#euclidean-norm) identity holds for the entire [vector](vector-space.md#vector).

### Stable construction of a Givens rotation

↑ **Parent:** [Givens rotation](#givens-rotation)

For finite [real numbers](arithmetic.md#real-number) $a,b$, a [Givens rotation](#givens-rotation) that annihilates $b$ is defined mathematically by

$$
r=\operatorname{hypot}(a,b)=\sqrt{a^2+b^2},\qquad
(c,s)=\begin{cases}(a/r,b/r),&r>0,\\(1,0),&a=b=0.\end{cases}
$$

Here `hypot` means an evaluation of the [Euclidean norm](normed-vector-space.md#euclidean-norm) of $(a,b)^T$ designed to avoid unnecessary range failures in [floating-point arithmetic](floating-point-arithmetic.md). The zero case selects the [identity matrix](vector-space.md#identity-matrix), avoiding division by zero. If $a=0,b\ne0$, then $c=0,s=\operatorname{sign}(b)$; if $b=0,a\ne0$, then $c=\operatorname{sign}(a),s=0$. Thus the retained component is nonnegative, including when $a<0$. In exact arithmetic, $ca+sb=r$ and $-sa+cb=0$.

Computing the [square root](algebra.md#square-root) of `a*a + b*b` directly can fail even when the final [norm](normed-vector-space.md#norm) is representable. In binary64 [floating-point arithmetic](floating-point-arithmetic.md), $a=b=10^{308}$ makes the squares overflow, whereas $r\approx1.4142\times10^{308}$ is finite. With $a=b=10^{-300}$ the squares round to zero, although $r\approx1.4142\times10^{-300}$ is representable. A range-safe `hypot` avoids these intermediate failures.

The simple divisions $a/r,b/r$ still need care when $r$ is a [subnormal number](floating-point-arithmetic.md#subnormal-number): rounding $r$ can cause large relative errors. For the smallest positive binary64 [subnormal number](floating-point-arithmetic.md#subnormal-number) $\eta=2^{-1074}$, taking $a=b=\eta$ rounds $\sqrt2\eta$ to $\eta$; dividing by that rounded value gives $c=s=1$, which is not an [orthogonal matrix](linear-algebra.md#orthogonal-matrix). For nonzero finite inputs, compute the [coefficients](vector-space.md#coefficient) before rescaling the [norm](normed-vector-space.md#norm):

$$
t=\max(|a|,|b|),\qquad \alpha=a/t,\quad\beta=b/t,\quad
h=\operatorname{hypot}(\alpha,\beta),\qquad
c=\alpha/h,\quad s=\beta/h,\quad r=th.
$$

At least one scaled component has [absolute value](real-analysis.md#absolute-value) one, and $1\leq h\leq\sqrt2$. This construction keeps the [coefficients](vector-space.md#coefficient) meaningful even when rounding $r$ is severe. It cannot make an unrepresentably large $r$ finite, preserve an arbitrarily tiny $s$ against underflow, or repair inputs already rounded to zero. The row updates themselves can also overflow if their exact results exceed the available range.

LAPACK's `DLARTG` uses scaling for [numerical stability](#stability-of-a-numerical-method) but a different sign convention: for $a\ne0$ it chooses $r=\operatorname{sign}(a)\sqrt{a^2+b^2}$ and $c\geq0$; for $b=0$ it returns $c=1,s=0,r=a$. Its block still has the lower-left minus sign. Do not combine its returned [coefficients](vector-space.md#coefficient) with an assumed nonnegative $r$.[DLARTG, LAPACK 3.12.1, Purpose: block, signed R, scaling and zero-input cases; implementation lines 137–159](mathematics-bibliography.md#dlartg-lapack-3-12-1-by-edward-anderson)

### Givens row-pair update

↑ **Parent:** [Givens rotation](#givens-rotation)

Left [matrix multiplication](vector-space.md#matrix-multiplication) by a [Givens rotation](#givens-rotation) replaces rows $i,j$ of a [matrix](vector-space.md#matrix) by

$$
A'_{ik}=cA_{ik}+sA_{jk},\qquad
A'_{jk}=-sA_{ik}+cA_{jk}.
$$

Both right-hand sides use the old entries. An in-place [algorithm](algorithm.md) must save the first result temporarily, update the second entry, and only then overwrite the first. The reference BLAS `DROT` implementation follows this order with its temporary `DTEMP`.[DROT source, lines 116–120 and 130–134: temporary first-row value and second-row update](mathematics-bibliography.md#drot-reference-blas-lapack-3-12-1-by-lapack-project)

For elimination in column $k$, construct $(c,s)$ from $(A_{ik},A_{jk})$. This sets the lower component to zero in exact arithmetic. In [floating-point arithmetic](floating-point-arithmetic.md) the computed expression can leave a small remainder; after computing the other updated entries, explicitly store $A'_{jk}=0$ and $A'_{ik}=r$. Previously eliminated columns stay zero if both participating rows are already zero there. This is why the ordering in [QR decomposition by Givens rotations](#qr-decomposition-by-givens-rotations) matters.

### QR decomposition by Givens rotations

↑ **Parent:** [Givens rotation](#givens-rotation)

Successive [Givens rotations](#givens-rotation) eliminate entries below the diagonal of a [matrix](vector-space.md#matrix). For an $m\times n$ [matrix](vector-space.md#matrix) with $m\geq n$, process columns $k=1,\ldots,n$; within column $k$, rotate rows $k,j$ for each $j>k$ whose entry needs elimination. Apply each [Givens row-pair update](#givens-row-pair-update) to columns $k,\ldots,n$. Both rows are zero in earlier columns, so these operations preserve earlier eliminations. No assumption of [full column rank](vector-space.md#full-column-rank) is needed to perform the eliminations.

For a concrete example, take

$$
A=\begin{pmatrix}3&0\\4&5\\0&2\end{pmatrix}.
$$

First use $G_1=G_{12}(3/5,4/5)$, then $G_2=G_{23}(3/\sqrt{13},2/\sqrt{13})$:

$$
G_1A=\begin{pmatrix}5&4\\0&3\\0&2\end{pmatrix},\qquad
R=G_2G_1A=\begin{pmatrix}5&4\\0&\sqrt{13}\\0&0\end{pmatrix}.
$$

The entry in position $(3,1)$ was already zero, so its elimination was skipped. The second [Givens rotation](#givens-rotation) combines the remaining pair $(3,2)^T$ in column two. This yields the full [QR decomposition](inner-product.md#qr-decomposition)

$$
Q=G_1^TG_2^T=
\begin{pmatrix}
3/5&-12/(5\sqrt{13})&8/(5\sqrt{13})\\
4/5&9/(5\sqrt{13})&-6/(5\sqrt{13})\\
0&2/\sqrt{13}&3/\sqrt{13}
\end{pmatrix},\qquad A=QR.
$$

The first two columns of $Q$ and first two rows of $R$ give the reduced [QR decomposition](inner-product.md#qr-decomposition). Direct multiplication verifies both $QR=A$ and $Q^TQ=I$. For these displayed factors evaluated in binary64 [floating-point arithmetic](floating-point-arithmetic.md), the [Frobenius norms](compact-operator.md#frobenius-norm) $\|A-QR\|_F$ and $\|Q^TQ-I\|_F$ are both below $10^{-14}$; these measure reconstruction and loss of [orthogonality](inner-product.md#orthogonal-vectors) separately.

<a id="image-two-local-givens-row-pair-updates-turn-a-3-times2-matrix-into-the-rectangular-r-of-a-qr-decomposition"></a>
![](givens-qr-row-elimination.png)

**[Figure 20](#image-two-local-givens-row-pair-updates-turn-a-3-times2-matrix-into-the-rectangular-r-of-a-qr-decomposition). Two local Givens row-pair updates turn a $3\times2$ matrix into the rectangular $R$ of a QR decomposition**.

More generally, if the chronological rotations are $G_1,\ldots,G_p$, then

$$
\Omega=G_p\cdots G_1,\qquad R=\Omega A,\qquad
Q=\Omega^T=G_1^T\cdots G_p^T.
$$

Each factor is an [orthogonal matrix](linear-algebra.md#orthogonal-matrix), so $Q$ is too. For a rectangular [matrix](vector-space.md#matrix), $R$ has zeros below its diagonal; its leading $n\times n$ block is an [upper triangular matrix](linear-algebra.md#upper-triangular-matrix). With [full column rank](vector-space.md#full-column-rank), retaining the first $n$ columns of $Q$ gives [orthonormal](inner-product.md#orthonormal-set) columns. To impose a positive diagonal when necessary, flip matching columns of $Q$ and rows of $R$, preserving their product.

For a [linear least-squares problem](inner-product.md#linear-least-squares-problem), apply the same chronological [Givens rotations](#givens-rotation) to the right-hand side $b$, obtaining $z=\Omega b$, without explicitly constructing $Q$. Since the [Euclidean norm](normed-vector-space.md#euclidean-norm) is preserved, solve the leading [upper triangular matrix](linear-algebra.md#upper-triangular-matrix) system $R_1x=z_{1:n}$ by [back substitution](linear-algebra.md#back-substitution) when $A$ has [full column rank](vector-space.md#full-column-rank); the remaining entries of $z$ give the minimum residual [norm](normed-vector-space.md#norm). In the example, $b=(0,0,1)^T$ gives $z=(0,2/\sqrt{13},3/\sqrt{13})^T$, $x=(-8/65,2/13)^T$, and minimum residual [Euclidean norm](normed-vector-space.md#euclidean-norm) $3/\sqrt{13}$.

The locality is useful for a [sparse matrix](vector-space.md#sparse-matrix) or an existing [QR decomposition](inner-product.md#qr-decomposition) needing an extra row: only two rows change at each step, and the new row can be eliminated against the stored [upper triangular matrix](linear-algebra.md#upper-triangular-matrix). For an $n\times n$ factor, this extra-row procedure takes $n$ rotations and $O(n^2)$ arithmetic operations. Locality does not guarantee preservation of sparsity: mixing rows can create nonzeros wherever either row had one. For a fully populated $m\times n$ input, the straightforward elimination uses $\sum_{k=1}^n(m-k)$ rotations, each touching $n-k+1$ columns, giving $O(mn^2)$ work. Storage layout, zero patterns and implementation affect speed; this count alone establishes no universal advantage over other [QR decomposition](inner-product.md#qr-decomposition) [algorithms](algorithm.md).

The [Euclidean norm](normed-vector-space.md#euclidean-norm) preservation explains the appeal for [numerical stability](#stability-of-a-numerical-method): exact rotations do not amplify a perturbation's length. Rounded [coefficients](vector-space.md#coefficient) and [Givens row-pair updates](#givens-row-pair-update) still introduce [roundoff error](#round-off-error). Small reconstruction and [orthogonality](inner-product.md#orthogonal-vectors) residuals check the computed factors, while the [condition number](quadratic-form.md#condition-number) of the original problem still controls how accurately a [linear least-squares problem](inner-product.md#linear-least-squares-problem) determines its solution.

## Gradient descent

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](gradient-descent.md)

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

The [Taylor expansion](calculus.md#taylor-expansion) with [integral](integral.md) remainder gives $L(f)=\int_0^2K(t)f^{(3)}(t)\,dt$, because $L$ annihilates [polynomials](polynomial.md) of degree at most two. Since $K\ge0$ and $\int_0^2K=1/3$, the sharp bound is $|L(f)|\le\frac13\|f^{(3)}\|_\infty$. Equality holds for $f(x)=x^3/6$.

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

[This section is present in another page, follow this link to view it.](runge-kutta-method.md)

## Simplex algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simplex_algorithm)

### Dual simplex algorithm

↑ **Parent:** [Simplex algorithm](#simplex-algorithm)

The dual simplex algorithm keeps the objective row dual feasible while repairing negative basic values. In a maximization dictionary $x_B=b+\sum_j a_jx_j$ with $b<0$ and nonbasic objective coefficients $d_j\leq0$, eligible entering columns have $a_j>0$; choose one minimizing $(-d_j)/a_j$. The pivot restores progress toward primal feasibility without losing the objective bound.

### Simplex dictionary

↑ **Parent:** [Simplex algorithm](#simplex-algorithm)

A simplex dictionary expresses the basic variables and the objective as affine functions of the nonbasic variables in a [linear program](linear-programming.md). Setting the nonbasic variables to zero gives a [basic feasible solution](linear-programming.md#basic-feasible-solution) when all basic values are nonnegative. A [simplex algorithm](#simplex-algorithm) pivot exchanges one basic and one nonbasic variable. For maximization, a feasible dictionary with all nonbasic objective coefficients nonpositive certifies optimality.

## Sparse optimization

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sparse_optimization)

### Compressed sensing

↑ **Parent:** [Sparse optimization](#sparse-optimization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressed_sensing)

Compressed sensing reconstructs a [sparse vector](#sparse-vector), or an approximately sparse one, from fewer linear measurements than its ambient dimension. [Basis pursuit](#basis-pursuit) replaces counting nonzero coordinates by [convex](real-analysis.md#convex-function) $\ell^1$ minimization. A [null space property](#nullspace-property) characterizes exact uniform recovery, while a [robust null space property](#robust-null-space-property) controls errors from noise and nonsparse tails.

#### Coherence of a normalized matrix

↑ **Parent:** [Compressed sensing](#compressed-sensing)

For a [matrix](vector-space.md#matrix) with at least two columns of unit [Euclidean norm](normed-vector-space.md#euclidean-norm), its mutual coherence is the largest magnitude of an [inner product](inner-product.md) between distinct columns. It measures the strongest pairwise ambiguity of linear measurements. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $0\le\mu\le1$. The order-two [restricted isometry constant](#restricted-isometry-constant) equals the [mutual coherence](#coherence-of-a-normalized-matrix), because every two-column [Gram matrix](inner-product.md#gram-matrix) has eigenvalues $1\pm|\langle a_i,a_j\rangle|$.

##### Cumulative coherence

↑ **Parent:** [Coherence of a normalized matrix](#coherence-of-a-normalized-matrix)

For unit [Euclidean norm](normed-vector-space.md#euclidean-norm) columns, cumulative coherence measures the largest sum of $k$ correlations with one other column. Its domain is $0\le k\le N-1$, with $\mu_1(0)=0$ by the empty-sum convention. It is nondecreasing, $\mu_1(1)=\mu$ for $N\ge2$, and $\mu_1(k)\le k\mu$, where $\mu$ is the [mutual coherence](#coherence-of-a-normalized-matrix). Keeping a sum of actual correlations can be substantially sharper than replacing each summand by the largest one.

###### Cumulative coherence bound for restricted isometry

↑ **Parent:** [Cumulative coherence](#cumulative-coherence)

For normalized columns and $1\le s\le N$, the [restricted isometry constant](#restricted-isometry-constant) is bounded by the [cumulative coherence](#cumulative-coherence) at $s-1$. A restricted [Gram matrix](inner-product.md#gram-matrix) has diagonal one and every off-diagonal row sum at most $\mu_1(s-1)$. The [Gershgorin circle theorem](#gershgorin-circle-theorem) and the [finite-dimensional spectral theorem](linear-operator-theory.md#finite-dimensional-spectral-theorem) bound its [eigenvalues](linear-operator-theory.md#eigenvalue) between $1-\mu_1(s-1)$ and $1+\mu_1(s-1)$. At $s=1$ the distortion is zero, and at $s=2$ it is exactly the [mutual coherence](#coherence-of-a-normalized-matrix).

#### Sparse injectivity

↑ **Parent:** [Compressed sensing](#compressed-sensing)

A [linear map](vector-space.md#linear-map) is injective on the class of [sparse vectors](#sparse-vector) of order $s$ exactly when its [null space](kernel-of-a-linear-map.md) contains no nonzero [vector](vector-space.md#vector) with at most $2s$ nonzero entries. Differences of two sparse [vectors](vector-space.md#vector) have at most $2s$ active coordinates. Conversely, splitting the [support of a vector](#support-of-a-vector) of a $2s$-sparse null [vector](vector-space.md#vector) into two parts constructs two distinct $s$-sparse [vectors](vector-space.md#vector) with the same image. The strict [null space property](#nullspace-property) implies sparse injectivity by applying it to both parts of such a split.

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

Basis pursuit minimizes an $\ell^1$ [norm](normed-vector-space.md#norm) subject to exact linear measurements. Basis pursuit with a noise tolerance replaces the equality by $\|Ax-y\|_2\le\eta$. A unique minimizer has linearly independent active columns, and hence at most $\operatorname{rank}A$ nonzero coordinates: a null direction on its support would make the objective locally affine on a feasible line, contradicting minimality or uniqueness.

##### Strict dual certificate for basis pursuit

↑ **Parent:** [Basis pursuit](#basis-pursuit)

For a real [vector](vector-space.md#vector) $x$ with [support of a vector](#support-of-a-vector) $S$, this certificate is a [vector](vector-space.md#vector) $h$ whose measurements under the [adjoint operator](hilbert-space.md#adjoint-operator) match the active [sign function](foundations-of-mathematics.md#sign-function) values and lie strictly between minus one and one on the inactive coordinates. If $A_S$ is [injective](algebra.md#injective-function), such a certificate proves that $x$ is the unique [basis pursuit](#basis-pursuit) [minimizer](analysis.md#global-minimizer). For a nonzero $v\in\ker A$, [injectivity](algebra.md#injective-function) ensures $v_{S^c}\ne0$, and $0=\langle A^*h,v\rangle$ implies the [fixed-sign null space condition](#fixed-sign-null-space-condition). The strict inequality is interpreted coordinatewise if $S^c$ is empty. The condition with the [sign function](foundations-of-mathematics.md#sign-function) written here is for real variables; complex [basis pursuit](#basis-pursuit) uses the unit phases of active coordinates instead.

###### Least-norm dual certificate

↑ **Parent:** [Strict dual certificate for basis pursuit](#strict-dual-certificate-for-basis-pursuit)

When $A_S$ is [injective](algebra.md#injective-function), this [vector](vector-space.md#vector) solves $A_S^*h_0=\operatorname{sgn}(x_S)$. Any other solution differs by a [vector](vector-space.md#vector) in $\ker A_S^*$, orthogonal to the range of $A_S$ containing $h_0$. The [Pythagorean identity](inner-product.md#pythagorean-theorem-in-an-inner-product-space) therefore proves that $h_0$ has the smallest [Euclidean norm](normed-vector-space.md#euclidean-norm). It is a [strict dual certificate for basis pursuit](#strict-dual-certificate-for-basis-pursuit) exactly when each inactive coordinate of $A^*h_0$ has magnitude less than one. Failure of that test does not rule out another certificate: a [null space](kernel-of-a-linear-map.md) component of $A_S^*$ can alter those inactive coordinates.

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

The number of nonzero coordinates of a finite [vector](vector-space.md#vector) is its L0 sparsity count. It vanishes only at zero, but is unchanged under multiplication by a nonzero scalar, so it is not a [norm](normed-vector-space.md#norm). Minimizing it under linear measurement constraints finds a [sparse vector](#sparse-vector) with the smallest possible [support of a vector](#support-of-a-vector). [Sparse injectivity](#sparse-injectivity) of order $s$ guarantees unique recovery of every [sparse vector](#sparse-vector) with at most $s$ nonzero coordinates by this objective.

##### Support of a vector

↑ **Parent:** [Sparse vector](#sparse-vector)

The support of a finite vector is the set of indices of its nonzero coordinates. It is the [support of a function](function.md#support) on a finite discrete index set, and its cardinality defines sparsity.

###### Maximum-support vector in a finite-dimensional subspace

↑ **Parent:** [Support of a vector](#support-of-a-vector)

For any [field](algebra.md#field) $F$ and [vector subspace](vector-space.md#vector-subspace) $W\subseteq F^m$, some $u\in W$ has at least $\dim W$ nonzero coordinates. Choose $u$ with largest [support of a vector](#support-of-a-vector) $S$. Restriction from $W$ to $F^S$ is injective: a nonzero vector in its [kernel of a linear map](kernel-of-a-linear-map.md) vanishes on $S$, so adding it to $u$ would enlarge $S$. Thus $\dim W\leq|S|$. The argument works over [finite fields](algebra.md#finite-field), where assuming a generic vector avoids finitely many hyperplanes would be invalid.

## Stability function

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stability_function)

### Dahlquist test equation

↑ **Parent:** [Stability function](#stability-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dahlquist_test_equation)

The Dahlquist test equation is the scalar linear initial-value problem $y'=\lambda y$. A one-step method reduces it to $y_{n+1}=R(h\lambda)y_n$, thereby defining its [stability function](#stability-function) $R$.

## Linear multistep method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](linear-multistep-method.md)

## Numerical linear algebra

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](numerical-linear-algebra.md)

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

The strict decay convention for a [linear stability domain](#linear-stability-domain) demands that every numerical mode tends to zero on the [Dahlquist test equation](#dahlquist-test-equation). For a one-step [stability function](#stability-function) it requires $|R(z)|<1$; for a [multistep method](linear-multistep-method.md) it requires every [amplification root](linear-multistep-method.md#amplification-root) to have [modulus](complex-analysis.md#modulus) below one. This differs from a boundedness convention that allows simple [unit-circle roots](polynomial.md#unit-circle-root), and from mesh-uniform finite-time [numerical stability](#stability-of-a-numerical-method). [Cambridge numerical analysis notes](https://www.damtp.cam.ac.uk/user/na/PartIB/Lect10.pdf) use the decay convention. Explicitly specifying the convention is essential for methods with undamped modes.

### A-alpha stability

↑ **Parent:** [Linear stability domain](#linear-stability-domain)

A numerical time-stepping method is $A(\alpha)$-stable if its [absolute stability](#linear-stability-domain) region contains the negative-axis sector $\{z:|\arg(-z)|\leq\alpha\}$, for $0<\alpha\leq\pi/2$. With a [stability function](#stability-function) $R$, this requires $|R(z)|\leq1$ throughout that sector. At $\alpha=\pi/2$, this is [A-stability](#a-stability).

### Euler method

↑ **Parent:** [Linear stability domain](#linear-stability-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_method)

The [Euler method](#euler-method) approximates an [initial value problem](differential-equation.md#initial-value-problem) $y'=f(t,y)$, $y(t_0)=y_0$, by evaluating the [derivative](calculus.md#derivative) at the current point and moving along that [tangent line](calculus.md#tangent-line) for a time $h$. With $t_n=t_0+nh$, its displayed update needs one evaluation of $f$ per step. This simple rule turns local slope information into a whole approximate trajectory. MIT's course notes derive it by dropping the second-order [Taylor remainder](calculus.md#taylor-remainder).[MIT 10.001, Forward and Backward Euler Methods, equations 6–7](https://web.mit.edu/10.001/Web/Course_Notes/Differential_Equations_Notes/node3.html)

Take $y'=-2y$, $y(0)=1$, whose exact solution is the [exponential function](calculus.md#exponential-function) $y(t)=e^{-2t}$. The [Euler method](#euler-method) gives

$$
y_{n+1}=(1-2h)y_n,\qquad y_n=(1-2h)^n.
$$

At $h=0.2$, the first values are $1,0.6,0.36,0.216$. At $t=1$, five steps give $0.6^5=0.07776$, compared with $e^{-2}\approx0.135335$. The result decays but is too small: [absolute stability](#linear-stability-domain) alone does not ensure accuracy. At $h=1.2$, the first values are $1,-1.4,1.96,-2.744$, and at $t=6$ five steps give $-5.37824$, while the exact solution is about $0.00000614421$.

<a id="image-euler-approximations-to-exponential-decay-on-the-same-finite-time-interval"></a>
![](euler-stability-example.png)

**[Figure 21](#image-euler-approximations-to-exponential-decay-on-the-same-finite-time-interval). Euler approximations to exponential decay on the same finite time interval**.

For the [Dahlquist test equation](#dahlquist-test-equation) $y'=\lambda y$, the [Euler method](#euler-method) has [stability function](#stability-function) $R(z)=1+z$ with $z=h\lambda$. Its [absolute stability](#linear-stability-domain) region is $|1+z|\leq1$, the closed disk centred at $-1$ with radius one. For the present real decay problem and $h>0$, bounded numerical values require $0<h\leq1$; strict decay requires $0<h<1$. At $h=1$ the values alternate $1,-1,1,\ldots$ without decay. These conditions follow directly from the [amplification factor](finite-difference.md#amplification-factor) $1-2h$, matching MIT's criterion for $y'=-ay$.[MIT 10.001, Forward and Backward Euler Methods, linear decay example](https://web.mit.edu/10.001/Web/Course_Notes/Differential_Equations_Notes/node3.html)

The [Euler method](#euler-method) is first order: with bounded second [derivative](calculus.md#derivative) and suitable [Lipschitz continuity](real-analysis.md#lipschitz-continuity), its [global error](#global-discretization-error) is $O(h)$ on a fixed interval. In this example the [logarithm](calculus.md#logarithm) gives $\log(1-2h)=-2h-2h^2+O(h^3)$ for small positive $h$. At $t=nh$, this means $y_n=e^{-2t}(1-2th+O(h^2))$. It explains both the downward bias and why halving the step roughly halves the error once $h$ is sufficiently small.

### A-stability

↑ **Parent:** [Linear stability domain](#linear-stability-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/A-stability)

A method is A-stable when its stability domain contains the closed left half-plane.

<h4 id="a-stability-of-near-diagonal-exponential-pade-approximants">A-stability of near-diagonal exponential Padé approximants</h4>

↑ **Parent:** [A-stability](#a-stability)

For nonnegative degrees $m,n$ with $n-2\le m\le n$, the $[m/n]$ [Padé approximant](isolated-singularity.md#pade-approximant) $R$ to the [exponential function](calculus.md#exponential-function) has no poles in the left half-plane and satisfies $|R(z)|\le1$ for $\operatorname{Re}z\le0$. Consequently a numerical method having that [stability function](#stability-function) is [A-stable](#a-stability). In particular, the near-diagonal choice $[s-1/s]$ gives the [Radau IIA method](runge-kutta-method.md#radau-iia-method) stability function, while $[s/s]$ corresponds to the [Gauss collocation method](runge-kutta-method.md#gauss-legendre-method). The theorem concerns these exponential approximants, not arbitrary rational approximations with the same degrees.

#### Principal-root obstruction to A-stability

↑ **Parent:** [A-stability](#a-stability)

Suppose a consistent [linear multistep method](linear-multistep-method.md) has a simple principal [polynomial root](polynomial.md#root-of-a-polynomial) and its analytic [logarithm](calculus.md#logarithm) satisfies $\log w(z)=z+Cz^{2r}+O(z^{2r+1})$ near zero, with real coefficients. If $C(-1)^r>0$, then at $z=i\varepsilon$ the real part of $\log w$ is positive to leading order. The same remains true after giving $z$ a small negative real part of smaller magnitude than that leading term. Thus a growing [amplification factor](finite-difference.md#amplification-factor) occurs inside the left half-plane, ruling out [A-stability](#a-stability). For an order-three method with $C>0$, choose $z=-C\varepsilon^4/2+i\varepsilon$.

#### Explicit multistep methods cannot be A-stable

↑ **Parent:** [A-stability](#a-stability)

For an explicit [linear multistep method](linear-multistep-method.md), the highest-degree coefficient of $\rho(w)-z\sigma(w)$ is fixed while at least one lower coefficient grows unboundedly with negative real $z$. If all roots stayed in the [unit disk](euclidean-geometry.md#unit-disk), the [elementary symmetric polynomials](polynomial.md#elementary-symmetric-polynomial) of those roots would keep every monic coefficient bounded. This contradiction proves that no nontrivial consistent explicit method is [A-stable](#a-stability).

#### Boundary-locus test for multistep A-stability

↑ **Parent:** [A-stability](#a-stability)

A unit-modulus amplification root of a [linear multistep method](linear-multistep-method.md) puts its test-equation parameter on this boundary locus, except when numerator and denominator both vanish. If the locus avoids the open left half-plane, the leading coefficient never vanishes there and the roots are initially inside the disk at one point there, continuity keeps them inside throughout that connected region. Checking [zero-stability](linear-multistep-method.md#zero-stability), imaginary-axis roots and common polynomial factors is still necessary. A boundary plot alone is not a proof of [A-stability](#a-stability).

#### L-stability

↑ **Parent:** [A-stability](#a-stability)

An A-stable one-step method is L-stable when its [stability function](#stability-function) also satisfies $R(z)\to0$ as $|z|\to\infty$ within the left half-plane. It damps modes whose decay time is far shorter than the numerical step.

#### B-stability

↑ **Parent:** [A-stability](#a-stability)

A Runge--Kutta method is B-stable when it does not increase distances between numerical solutions of a dissipative differential equation. [Algebraic stability of a Runge-Kutta method](runge-kutta-method.md#algebraic-stability-of-a-runge-kutta-method) is a standard sufficient condition.

#### Backward Euler method

↑ **Parent:** [A-stability](#a-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backward_Euler_method)

Backward Euler advances $y'=f(t,y)$ by $y_{n+1}=y_n+h f(t_{n+1},y_{n+1})$. Its stability function $R(z)=(1-z)^{-1}$ makes it [L-stable](#l-stability).

#### A-stability of a symmetric two-stage implicit Runge-Kutta family

↑ **Parent:** [A-stability](#a-stability)

For the two-stage [implicit Runge-Kutta method](runge-kutta-method.md#implicit-runge-kutta-method) with

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

## Numerical integration

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](numerical-integration.md)

## Orthogonal polynomial

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

[This section is present in another page, follow this link to view it.](orthogonal-polynomial.md)

## Midpoint method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Midpoint_method)

The [midpoint method](#midpoint-method) advances an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) using a derivative evaluated at a temporal midpoint. Its explicit form predicts that midpoint from the initial derivative, while the [implicit midpoint rule](runge-kutta-method.md#implicit-midpoint-rule) solves for the derivative at the mean of the endpoint states.

## Collocation method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Collocation_method)

A [collocation method](#collocation-method) chooses an approximate solution from a finite-dimensional trial space and forces the residual of a [differential equation](differential-equation.md) to vanish at selected nodes. [Collocation Runge-Kutta methods](runge-kutta-method.md#collocation-runge-kutta-method) apply this principle to polynomial approximations on each time step.

## QR algorithm

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/QR_algorithm)

The [QR algorithm](#qr-algorithm) computes [eigenvalues](linear-operator-theory.md#eigenvalue) through repeated [QR decompositions](inner-product.md#qr-decomposition) and similarity updates. Shifted and unshifted forms have different convergence rates; the [unshifted QR algorithm](numerical-linear-algebra.md#unshifted-qr-algorithm) uses a zero shift at every step.

## Iterative method

↑ **Parent:** [Numerical analysis](numerical-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iterative_method)

An [iterative method](#iterative-method) approximates a solution by repeatedly updating an initial guess. In [numerical linear algebra](numerical-linear-algebra.md), a [stationary iterative method for a linear system](numerical-linear-algebra.md#stationary-iterative-method-for-a-linear-system) uses a fixed iteration map; other iterations can change their update rule or search space at each step.

## Forward error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

The [forward error](#forward-error) is the difference between a computed result $\widehat{x}$ and the exact result $x_*$ for the original data. Its size can be measured by a [norm](normed-vector-space.md#norm), or relative to $\|x_*\|$ when $x_*\ne0$. A [linear-system residual](gradient-descent.md#linear-system-residual) measures the equation imbalance instead; the [condition number](quadratic-form.md#condition-number) relates that imbalance to the [forward error](#forward-error).

## Backward error

↑ **Parent:** [Numerical analysis](numerical-analysis.md)

A [backward error](#backward-error) measures a perturbation $\delta d$ of the input data for which the computed result is an exact solution of the perturbed problem. Specify which data may change and which [norm](normed-vector-space.md#norm) measures the perturbation. For a [linear system](linear-algebra.md#system-of-linear-equations) $A\widehat{x}=b$, holding $A$ fixed gives $\delta b=A\widehat{x}-b$, the negative [linear-system residual](gradient-descent.md#linear-system-residual). The corresponding [forward error](#forward-error) also depends on the [condition number](quadratic-form.md#condition-number).

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Discrete Fourier transform](discrete-fourier-transform.md)
- [Polynomial](polynomial.md)
- [Significant figures](#significant-figures)
