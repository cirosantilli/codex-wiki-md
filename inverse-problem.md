# Inverse problem

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_problem)

An inverse problem seeks an unknown $u$ from data $f$ related by a forward map $A(u)=f$. Small singular values of the forward map can amplify measurement noise and make direct inversion unstable.

**Table of contents**

- [Tomography](#tomography)
  - [Computed tomography](#computed-tomography)
  - [Single-photon emission computed tomography](#single-photon-emission-computed-tomography)
- [Ill-posed inverse problem](#ill-posed-inverse-problem)
- [X-ray transform](#x-ray-transform)
  - [Thermostat X-ray transform](#thermostat-x-ray-transform)
    - [Kernel of the thermostat X-ray transform in degrees zero and one](#kernel-of-the-thermostat-x-ray-transform-in-degrees-zero-and-one)
  - [Magnetic X-ray transform](#magnetic-x-ray-transform)
    - [Kernel of the magnetic X-ray transform in degrees zero and one](#kernel-of-the-magnetic-x-ray-transform-in-degrees-zero-and-one)
  - [Geodesic X-ray transform](#geodesic-x-ray-transform)
    - [Counterexample to geodesic one-form injectivity on the round sphere](#counterexample-to-geodesic-one-form-injectivity-on-the-round-sphere)
    - [Pestov identity for a geodesic flow](#pestov-identity-for-a-geodesic-flow)
    - [Potential symmetric 2-tensor](#potential-symmetric-2-tensor)
- [Forward problem](#forward-problem)
- [Residual of an inverse problem](#residual-of-an-inverse-problem)
- [Inverse scattering problem](#inverse-scattering-problem)
  - [Spherical far-field range condition](#spherical-far-field-range-condition)
    - [Unbounded spherical far-to-near-field continuation](#unbounded-spherical-far-to-near-field-continuation)
  - [Fourier diffraction theorem](#fourier-diffraction-theorem)
    - [Ewald sphere](#ewald-sphere)
  - [Kirchhoff–Helmholtz representation](#kirchhoff-helmholtz-representation)
    - [Surface representation of an obstacle far-field pattern](#surface-representation-of-an-obstacle-far-field-pattern)
  - [Herglotz wave function](#herglotz-wave-function)
    - [Herglotz pairing with an obstacle far field](#herglotz-pairing-with-an-obstacle-far-field)
      - [Shape recovery from a Herglotz boundary identity](#shape-recovery-from-a-herglotz-boundary-identity)
  - [Scattering potential](#scattering-potential)
    - [Born approximation for scalar wave scattering](#born-approximation-for-scalar-wave-scattering)
      - [Born non-scattering contrasts at one incident direction](#born-non-scattering-contrasts-at-one-incident-direction)
      - [Born series](#born-series)
  - [Rytov approximation](#rytov-approximation)
    - [First-Rytov coherent mean](#first-rytov-coherent-mean)
    - [Phase covariance in the first Rytov approximation](#phase-covariance-in-the-first-rytov-approximation)
    - [Validity of the first Rytov approximation](#validity-of-the-first-rytov-approximation)
    - [Logarithmic wave perturbation](#logarithmic-wave-perturbation)
    - [Gaussian intensity in the first Rytov approximation](#gaussian-intensity-in-the-first-rytov-approximation)
      - [Mean-potential correction to weak Rytov intensity](#mean-potential-correction-to-weak-rytov-intensity)
  - [Far-field pattern](#far-field-pattern)
    - [Far-field approximation for an outgoing source](#far-field-approximation-for-an-outgoing-source)
    - [Sommerfeld radiation condition](#sommerfeld-radiation-condition)
- [Well-posed problem](#well-posed-problem)
- [Regularization of an inverse problem](#regularization-of-an-inverse-problem)
  - [Lavrentiev regularization](#lavrentiev-regularization)
  - [Linear regularization](#linear-regularization)
    - [Central-difference noise-bias bound](#central-difference-noise-bias-bound)
    - [Overlap multiplicity bound for piecewise difference operators](#overlap-multiplicity-bound-for-piecewise-difference-operators)
  - [Regularization parameter](#regularization-parameter)
  - [Convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem)
    - [Noise-bias decomposition for linear regularization](#noise-bias-decomposition-for-linear-regularization)
  - [Spectral regularization method](#spectral-regularization-method)
    - [Asymptotic regularization](#asymptotic-regularization)
    - [Truncated singular value decomposition](#truncated-singular-value-decomposition)
  - [Tikhonov regularization](#tikhonov-regularization)
    - [Tikhonov regularization of spherical far-field continuation](#tikhonov-regularization-of-spherical-far-field-continuation)
    - [Tikhonov reconstruction from two-plane scattering data](#tikhonov-reconstruction-from-two-plane-scattering-data)
    - [Truncated Tikhonov resolvent](#truncated-tikhonov-resolvent)
    - [Quadratic norm penalty](#quadratic-norm-penalty)
    - [Singular-system Tikhonov filter](#singular-system-tikhonov-filter)
    - [Tikhonov stability bound](#tikhonov-stability-bound)
    - [Tikhonov filter norm bound](#tikhonov-filter-norm-bound)
    - [Tikhonov regularization with a coercive penalty operator](#tikhonov-regularization-with-a-coercive-penalty-operator)
      - [Approximate source bound for coercive Tikhonov regularization](#approximate-source-bound-for-coercive-tikhonov-regularization)
      - [Normal equation for coercive Tikhonov regularization](#normal-equation-for-coercive-tikhonov-regularization)
    - [Source condition for quadratic regularization](#source-condition-for-quadratic-regularization)
    - [Tikhonov normal equation](#tikhonov-normal-equation)
    - [Spectral filter](#spectral-filter)
      - [Evenization of a nonnegative bandlimited filter](#evenization-of-a-nonnegative-bandlimited-filter)
    - [Regularization parameter choice](#regularization-parameter-choice)
      - [Balancing noise and approximation bias](#balancing-noise-and-approximation-bias)
      - [A priori regularization parameter choice](#a-priori-regularization-parameter-choice)
    - [Iterated Tikhonov regularization](#iterated-tikhonov-regularization)
      - [Iterated Tikhonov spectral filter](#iterated-tikhonov-spectral-filter)
  - [Variational regularization](#variational-regularization)
    - [Discrete Hessian-norm denoising](#discrete-hessian-norm-denoising)
    - [Global discrete gradient-norm denoising](#global-discrete-gradient-norm-denoising)
      - [Global gradient-norm projection residual](#global-gradient-norm-projection-residual)
    - [Poisson data fidelity](#poisson-data-fidelity)
      - [Shifted Poisson data fidelity](#shifted-poisson-data-fidelity)
        - [Existence for nonnegative shifted Poisson regularization](#existence-for-nonnegative-shifted-poisson-regularization)
        - [Nonattainment under strict positivity for shifted Poisson fidelity](#nonattainment-under-strict-positivity-for-shifted-poisson-fidelity)
      - [Proximal operator of Poisson data fidelity](#proximal-operator-of-poisson-data-fidelity)
    - [Maximum-entropy regularization functional](#maximum-entropy-regularization-functional)
    - [Data compatibility with the regularizer domain](#data-compatibility-with-the-regularizer-domain)
    - [Value function of variational regularization](#value-function-of-variational-regularization)
      - [Monotonicity of data fidelity and regularization penalty](#monotonicity-of-data-fidelity-and-regularization-penalty)
    - [Parameter continuity of variational regularization](#parameter-continuity-of-variational-regularization)
    - [Quartic-norm variational regularization](#quartic-norm-variational-regularization)
    - [J-minimizing solution](#j-minimizing-solution)
    - [Residual method for variational regularization](#residual-method-for-variational-regularization)
      - [Compact-sublevel convergence of the residual method](#compact-sublevel-convergence-of-the-residual-method)
    - [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)
      - [Total variation under opposite smooth flows](#total-variation-under-opposite-smooth-flows)
      - [Total variation calibration](#total-variation-calibration)
      - [Total variation flow](#total-variation-flow)
      - [Total variation denoising](#total-variation-denoising)
        - [Box-constrained TV-L1 denoising](#box-constrained-tv-l1-denoising)
        - [Jump-amplitude inequality for total variation denoising](#jump-amplitude-inequality-for-total-variation-denoising)
          - [No-new-jumps property of total variation denoising](#no-new-jumps-property-of-total-variation-denoising)
          - [Jump-amplitude inequality for a bounded ROF minimizer](#jump-amplitude-inequality-for-a-bounded-rof-minimizer)
        - [Residual-preserving clipping of an ROF minimizer](#residual-preserving-clipping-of-an-rof-minimizer)
        - [Quadratic fidelity](#quadratic-fidelity)
          - [Opposite-flow fidelity identity for quadratic data](#opposite-flow-fidelity-identity-for-quadratic-data)
        - [ROF level-set formulation](#rof-level-set-formulation)
          - [Noncontact of ROF level boundaries](#noncontact-of-rof-level-boundaries)
        - [Signed layer-cake identity for quadratic fidelity](#signed-layer-cake-identity-for-quadratic-fidelity)
        - [Constrained-penalized equivalence for total variation denoising](#constrained-penalized-equivalence-for-total-variation-denoising)
        - [Graph total variation](#graph-total-variation)
          - [Graph total variation denoising](#graph-total-variation-denoising)
        - [Total variation denoising of a disk](#total-variation-denoising-of-a-disk)
        - [Staircasing in total variation denoising](#staircasing-in-total-variation-denoising)
        - [Discrete isotropic total variation](#discrete-isotropic-total-variation)
          - [Projection residual for discrete total variation](#projection-residual-for-discrete-total-variation)
            - [Projected-gradient dual total variation algorithm](#projected-gradient-dual-total-variation-algorithm)
      - [Total variation of an interval indicator](#total-variation-of-an-interval-indicator)
      - [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)
        - [Completeness of the bounded-variation space](#completeness-of-the-bounded-variation-space)
        - [BV slicing theorem](#bv-slicing-theorem)
          - [BV jump-product limit with one bounded factor](#bv-jump-product-limit-with-one-bounded-factor)
        - [BV trace on a hypersurface](#bv-trace-on-a-hypersurface)
        - [Approximate gradient](#approximate-gradient)
        - [Approximate discontinuity set](#approximate-discontinuity-set)
        - [One-sided representatives of a one-dimensional BV function](#one-sided-representatives-of-a-one-dimensional-bv-function)
        - [Approximate mean limit of a function](#approximate-mean-limit-of-a-function)
          - [Approximate jump point](#approximate-jump-point)
        - [Coarea formula for BV functions](#coarea-formula-for-bv-functions)
        - [Structure theorem for functions of bounded variation](#structure-theorem-for-functions-of-bounded-variation)
          - [Decomposition of a BV derivative](#decomposition-of-a-bv-derivative)
            - [Jump part of a BV derivative](#jump-part-of-a-bv-derivative)
        - [BV translation estimate](#bv-translation-estimate)
          - [BV mollification error estimate](#bv-mollification-error-estimate)
        - [Bounded BV extension operator](#bounded-bv-extension-operator)
        - [Weak-star convergence in BV](#weak-star-convergence-in-bv)
          - [Strict convergence in BV](#strict-convergence-in-bv)
        - [Set of finite perimeter](#set-of-finite-perimeter)
          - [Perimeter](#perimeter)
          - [Perimeter quasiminimizer](#perimeter-quasiminimizer)
          - [Relative perimeter](#relative-perimeter)
          - [Submodularity of relative perimeter](#submodularity-of-relative-perimeter)
            - [Comparison of perimeter minimizers with ordered forcing](#comparison-of-perimeter-minimizers-with-ordered-forcing)
          - [Caccioppoli partition](#caccioppoli-partition)
        - [Cantor part of a bounded-variation derivative](#cantor-part-of-a-bounded-variation-derivative)
        - [Jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function)
        - [Special bounded-variation space](#special-bounded-variation-space)
          - [SBV compactness theorem](#sbv-compactness-theorem)
        - [Relaxed graph-area functional](#relaxed-graph-area-functional)
          - [Graph-area Euler-Lagrange equation](#graph-area-euler-lagrange-equation)
          - [Independent box constraints in a graph-area supremum](#independent-box-constraints-in-a-graph-area-supremum)
        - [Bounded-variation compactness](#bounded-variation-compactness)
        - [Homogeneous bounded-variation space](#homogeneous-bounded-variation-space)
          - [Failure of L2 closure of the global BV domain](#failure-of-l2-closure-of-the-global-bv-domain)
        - [Bounded-variation step outside W11](#bounded-variation-step-outside-w11)
        - [Bounded-variation contraction under clipping](#bounded-variation-contraction-under-clipping)
          - [Scalar total variation splitting under clipping](#scalar-total-variation-splitting-under-clipping)
        - [Noncoercivity of total variation on constants](#noncoercivity-of-total-variation-on-constants)
        - [Zero-mean bounded-variation space](#zero-mean-bounded-variation-space)
          - [Poincaré inequality for total variation](#poincare-inequality-for-total-variation)
    - [Indicator functional of a constraint set](#indicator-functional-of-a-constraint-set)
    - [Source condition in variational regularization](#source-condition-in-variational-regularization)
      - [Normal-operator source condition](#normal-operator-source-condition)
        - [Shifted-comparator Bregman bound](#shifted-comparator-bregman-bound)
      - [Source-condition certification of a penalty-minimizing solution](#source-condition-certification-of-a-penalty-minimizing-solution)
      - [Range condition in variational regularization](#range-condition-in-variational-regularization)
    - [Bregman divergence](#bregman-divergence)
      - [Bregman iteration](#bregman-iteration)
        - [Finite termination of Bregman iteration on a singular vector](#finite-termination-of-bregman-iteration-on-a-singular-vector)
      - [Symmetric Bregman distance](#symmetric-bregman-distance)
        - [Source-condition estimate for symmetric Bregman distance](#source-condition-estimate-for-symmetric-bregman-distance)
      - [Zero Bregman distance and supporting faces](#zero-bregman-distance-and-supporting-faces)
    - [Exact penalty method](#exact-penalty-method)
      - [Exact-penalty threshold from a source condition](#exact-penalty-threshold-from-a-source-condition)
- [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)
  - [Least-squares solution of a linear inverse problem](#least-squares-solution-of-a-linear-inverse-problem)
    - [Least-squares existence criterion](#least-squares-existence-criterion)
    - [Nearest least-squares solution](#nearest-least-squares-solution)
  - [Singular system of a compact operator](#singular-system-of-a-compact-operator)
    - [Singular system of a periodic convolution operator](#singular-system-of-a-periodic-convolution-operator)
  - [Picard criterion](#picard-criterion)
  - [Landweber iteration](#landweber-iteration)
    - [Strong convergence of relaxed Landweber iteration](#strong-convergence-of-relaxed-landweber-iteration)
    - [Landweber iteration with a Tikhonov initial value](#landweber-iteration-with-a-tikhonov-initial-value)
      - [Closed form of a Tikhonov-initialized Landweber iterate](#closed-form-of-a-tikhonov-initialized-landweber-iterate)
    - [Landweber relaxation parameter](#landweber-relaxation-parameter)
    - [Landweber spectral filter](#landweber-spectral-filter)
      - [Landweber full inverse filter](#landweber-full-inverse-filter)
      - [Landweber noise amplification bound](#landweber-noise-amplification-bound)
        - [Uniform noise bound for relaxed Landweber iteration](#uniform-noise-bound-for-relaxed-landweber-iteration)
    - [Early stopping of Landweber iteration](#early-stopping-of-landweber-iteration)
  - [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator)
    - [Minimum-norm least-squares solution](#minimum-norm-least-squares-solution)

## Tomography

↑ **Parent:** [Inverse problem](inverse-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tomography)

Tomography reconstructs an interior distribution from measurements along multiple lines or paths through it. A linear unattenuated model is the [Radon transform](analysis.md#radon-transform); absorption changes it to an [attenuated Radon transform](analysis.md#attenuated-radon-transform).

### Computed tomography

↑ **Parent:** [Tomography](#tomography)

Transmission measurements determine line integrals of an absorption coefficient after taking the logarithm of incident intensity divided by transmitted intensity. Under the ideal straight-ray model, these measurements are a [Radon transform](analysis.md#radon-transform); [filtered backprojection](analysis.md#filtered-backprojection) reconstructs a planar slice. Angular coverage, calibration and noise control matter because differentiating measured projections amplifies high frequencies. In contrast, [single-photon emission computed tomography](#single-photon-emission-computed-tomography) reconstructs an emitting source through a possibly attenuating medium.

### Single-photon emission computed tomography

↑ **Parent:** [Tomography](#tomography)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Single-photon_emission_computed_tomography)

A form of [tomography](#tomography) that reconstructs an internal radioactive source from directional counts of individually emitted [photons](quantum-mechanics.md#photon). Known spatial [photon absorption](quantum-mechanics.md#photon-absorption) gives the exponential path weight in an [attenuated Radon transform](analysis.md#attenuated-radon-transform). Full directed data and a suitable reconstruction formula recover the source intensity rather than a transmitted exterior-beam attenuation map.

## Ill-posed inverse problem

↑ **Parent:** [Inverse problem](inverse-problem.md)

An [inverse problem](inverse-problem.md) is an [ill-posed problem](partial-differential-equation.md#ill-posed-problem) when its specified data do not give existence, uniqueness and continuous dependence of the recovered object in the chosen spaces. Missing Fourier modes can cause nonuniqueness, while small singular values can cause instability even when a unique solution exists. [Regularization of an inverse problem](#regularization-of-an-inverse-problem) adds information or a stability preference to the reconstruction.

## X-ray transform

↑ **Parent:** [Inverse problem](inverse-problem.md)

The X-ray transform records integrals of a function or tensor evaluation over a specified family of curves. The curve family, parametrization and any weights are part of the definition. Straight lines, [geodesics](riemannian-geometry.md#geodesic) and [magnetic flows](riemannian-geometry.md#magnetic-flow-on-a-riemannian-surface) give different versions; their injectivity and unavoidable potential kernels depend on that geometry.

### Thermostat X-ray transform

↑ **Parent:** [X-ray transform](#x-ray-transform)

The transform integrates a base function and a velocity-evaluated one-form along the closed trajectories of a [surface thermostat](riemannian-geometry.md#generalized-thermostat-on-a-riemannian-surface). Every [exact differential form](differential-form.md#exact-differential-form) of degree one integrates to zero, because $F(f\circ\pi)=df(v)$. The relevant kernel theorem concerns these functions of velocity degree zero and one, rather than arbitrary functions on the [unit tangent bundle](fiber-bundle.md#unit-tangent-bundle).

#### Kernel of the thermostat X-ray transform in degrees zero and one

↑ **Parent:** [Thermostat X-ray transform](#thermostat-x-ray-transform)

For a smooth [Anosov flow](dynamical-systems.md#anosov-flow) generated by a [surface thermostat](riemannian-geometry.md#generalized-thermostat-on-a-riemannian-surface) on a closed oriented [Riemannian surface](riemannian-geometry.md#riemannian-surface), a smooth base function plus a smooth one-form is a smooth [flow coboundary](dynamical-systems.md#flow-coboundary) precisely when the base function is zero and the one-form is an [exact differential form](differential-form.md#exact-differential-form). This is the nontrivial degree-zero/one kernel theorem. It does not require negative curvature or preservation of Liouville volume. The converse follows directly from $F(f\circ\pi)=df(v)$. A primary proof of the kernel theorem is [https://arxiv.org/abs/math/0601039.](https://arxiv.org/abs/math/0601039.)

### Magnetic X-ray transform

↑ **Parent:** [X-ray transform](#x-ray-transform)

The magnetic transform integrates functions or velocity-evaluated one-forms along magnetic trajectories, rather than ordinary geodesics. For closed trajectories, every exact one-form integrates to zero. Hyperbolic dynamics can make these the entire degree-one kernel.

#### Kernel of the magnetic X-ray transform in degrees zero and one

↑ **Parent:** [Magnetic X-ray transform](#magnetic-x-ray-transform)

For a smooth Anosov magnetic flow on a closed oriented surface, a smooth function plus a smooth one-form can be a smooth flow coboundary only when the function is zero and the one-form is exact. Equivalently their sum has zero integral along every closed orbit precisely in that case, using the smooth [Livsic theorem](dynamical-systems.md#livsic-theorem). This is the nontrivial magnetic transform kernel theorem. Exact one-forms give the converse directly, since $F(w\circ\pi)=dw(v)$. The theorem does not require pointwise negative Gaussian curvature.

### Geodesic X-ray transform

↑ **Parent:** [X-ray transform](#x-ray-transform)

For a symmetric covariant two-tensor, the geodesic transform integrates its evaluation on the unit velocity along boundary-to-boundary or closed [geodesics](riemannian-geometry.md#geodesic), as appropriate to the manifold. A [potential symmetric 2-tensor](#potential-symmetric-2-tensor) gives a total derivative along each geodesic and therefore integrates to zero on closed geodesics; boundary data require the corresponding boundary potential to vanish.

#### Counterexample to geodesic one-form injectivity on the round sphere

↑ **Parent:** [Geodesic X-ray transform](#geodesic-x-ray-transform)

The displayed one-form on the unit round sphere has zero integral on every closed [geodesic](riemannian-geometry.md#geodesic). Indeed, the [antipodal map](homology.md#antipodal-map) pulls it back to its negative, and the second half of an oriented great circle is the antipodal image of the first. Nevertheless $d\theta=2x_3\,dx_3\wedge dx_1$ is nonzero on an open set, so the one-form is not a [closed differential form](differential-form.md#closed-differential-form) and cannot be an [exact differential form](differential-form.md#exact-differential-form). Thus a curvature-free extension of one-form injectivity fails.

#### Pestov identity for a geodesic flow

↑ **Parent:** [Geodesic X-ray transform](#geodesic-x-ray-transform)

On a closed oriented Riemannian surface this integral identity follows from the canonical commutators and integration by parts against [Liouville volume of a surface geodesic flow](fiber-bundle.md#liouville-volume-of-a-surface-geodesic-flow). If $VX\varphi=-2H\varphi$ and $K<0$, substitution gives $\|X\varphi\|^2+5\|H\varphi\|^2+\int(-K)(V\varphi)^2=0$. Each term is nonnegative, forcing all three derivatives to vanish. For $\varphi=V^2u+u$, the fibre equation then makes $u$ a constant plus a fibrewise linear function, supplying the [potential symmetric 2-tensor](#potential-symmetric-2-tensor) kernel.

#### Potential symmetric 2-tensor

↑ **Parent:** [Geodesic X-ray transform](#geodesic-x-ray-transform)

For a vector field $Z$, define $\beta(v,w)=\langle\nabla_vZ,w\rangle+\langle\nabla_wZ,v\rangle$. Its diagonal evaluation is $2\langle\nabla_vZ,v\rangle$. Along a geodesic this equals $2\,d\langle Z,\dot\gamma\rangle/dt$, so it is invisible to closed-geodesic integrals. If a fibrewise linear function $u(x,v)=\eta_x(v)$ solves $Xu=\beta(v,v)$, then $Z=\eta^\sharp/2$ gives this convention.

## Forward problem

↑ **Parent:** [Inverse problem](inverse-problem.md)

A forward problem computes observable data $f=Ku$ from a known state or parameter $u$ and a specified model $K$. Its associated [inverse problem](inverse-problem.md) reconstructs $u$ from $f$ and the model. Inverse problems can fail existence, uniqueness or continuous dependence on the data.

## Residual of an inverse problem

↑ **Parent:** [Inverse problem](inverse-problem.md)

The residual is the difference between predicted and observed data. Its [norm](functional-analysis.md#norm) measures data misfit and can determine an iteration stopping rule for [regularization of an inverse problem](#regularization-of-an-inverse-problem).

## Inverse scattering problem

↑ **Parent:** [Inverse problem](inverse-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_scattering_problem)

An inverse scattering problem reconstructs a medium or obstacle from measured scattered waves. Under the [Born approximation](quantum-theory.md#born-approximation), fixed-frequency far-field data sample the [Fourier transform](analysis.md#fourier-transform) of the scattering potential on a restricted frequency surface.

### Spherical far-field range condition

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)

For an outgoing field outside a sphere of radius $R$, write $u_s=k\sum_{n,m}i^{n+1}a_n^m h_n^{(1)}(kr)Y_n^m$. Its [far-field pattern](#far-field-pattern) is $\sum a_n^mY_n^m$. If its trace on that sphere lies in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), Parseval's identity gives $k^2\sum|h_n^{(1)}(kR)|^2|a_n^m|^2<\infty$. The [fixed-argument growth of spherical Hankel functions](analysis.md#fixed-argument-growth-of-spherical-hankel-functions) yields the displayed equivalent range condition, with the low-order weights defined finitely. Square summability of the far-field coefficients alone does not ensure continuation to the chosen sphere.

#### Unbounded spherical far-to-near-field continuation

↑ **Parent:** [Spherical far-field range condition](#spherical-far-field-range-condition)

Continuation of a [far-field pattern](#far-field-pattern) to a spherical trace multiplies harmonic coefficients by the displayed factor, whose magnitude grows faster than exponentially with order. A data error of size $\delta$ in one normalized high-order harmonic therefore produces near-field error $\delta k|h_n^{(1)}(kR)|$, unbounded as its order increases. Some noisy square-summable far fields fail the range condition entirely. This proves unstable field continuation; bounds on actual obstacle geometry additionally require an admissible shape class and a stable boundary-extraction procedure.

### Fourier diffraction theorem

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)

The [Born approximation for scalar wave scattering](#born-approximation-for-scalar-wave-scattering) relates an incident [plane wave](quantum-mechanics.md#plane-wave) and the transverse [Fourier transform](analysis.md#fourier-transform) of its scattered field to samples of the three-dimensional Fourier transform of a [scattering potential](#scattering-potential) on a shifted [Ewald sphere](#ewald-sphere). One incident direction at one frequency samples a surface, rather than an entire three-dimensional frequency region. Additional illuminations, frequencies or structural constraints are needed for a full reconstruction.

#### Ewald sphere

↑ **Parent:** [Fourier diffraction theorem](#fourier-diffraction-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ewald_sphere)

With $|\mathbf k_i|=k$, elastic scattering into a propagating wavevector $\mathbf k_s$ samples Fourier transfer $\boldsymbol\kappa=\mathbf k_s-\mathbf k_i$. These transfers satisfy the displayed shifted sphere relation. This reciprocal-space construction appears in crystallographic diffraction and the [Fourier diffraction theorem](#fourier-diffraction-theorem).

<h3 id="kirchhoff-helmholtz-representation">Kirchhoff–Helmholtz representation</h3>

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)

With the normal directed out of an obstacle $D$ into the fluid, a field solving $(\Delta+k^2)\psi=-Q$ outside $D$ has the representation

$$
\psi(\mathbf r)=\int Q(\mathbf r')G_k(\mathbf r,\mathbf r')\,d\mathbf r'+\int_{\partial D}[\psi\partial_{n'}G_k-G_k\partial_{n'}\psi]\,dS'.
$$

Here $G_k$ is the [outgoing Green function for the three-dimensional Helmholtz equation](partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation) and the observation point lies outside the obstacle. The formula follows from [Green second identity](partial-differential-equation.md#green-second-identity); the normal to the exterior fluid on its inner boundary is the negative of the stated obstacle normal. The surface term represents the scattered field.

#### Surface representation of an obstacle far-field pattern

↑ **Parent:** [Kirchhoff–Helmholtz representation](#kirchhoff-helmholtz-representation)

For a scattered field satisfying $\psi_s=e^{ikr}f_\infty(\widehat{\mathbf r})/r+O(r^{-2})$, the [Kirchhoff–Helmholtz representation](#kirchhoff-helmholtz-representation) gives

$$
f_\infty(\widehat{\mathbf r})=-\frac1{4\pi}\int_{\partial D}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}[\partial_{n'}\psi_s+ik(\widehat{\mathbf r}\cdot\mathbf n')\psi_s]\,dS'.
$$

The sign assumes the normal points out of the obstacle.

### Herglotz wave function

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)

A Herglotz wave function is a superposition of incident [plane waves](quantum-mechanics.md#plane-wave),

$$
v_g(\mathbf r)=\int_{S^2}e^{ik\widehat{\mathbf d}\cdot\mathbf r}g(\widehat{\mathbf d})\,dS(\widehat{\mathbf d}),\qquad g\in L^2(S^2).
$$

It solves the [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) everywhere and is [real analytic](analysis.md#real-analytic-function). The finite sphere area makes the density integrable, so each spatial [derivative](calculus.md#derivative) can be taken under the integral.

#### Herglotz pairing with an obstacle far field

↑ **Parent:** [Herglotz wave function](#herglotz-wave-function)

Pairing a [far-field pattern](#far-field-pattern) with the conjugate density of a [Herglotz wave function](#herglotz-wave-function) converts the angular integral into boundary data:

$$
\int_{S^2}f_\infty(\widehat{\mathbf r})\overline{g(\widehat{\mathbf r})}\,dS=\frac1{4\pi}\int_{\partial D}[\psi_s\partial_n\overline{v_g}-\overline{v_g}\partial_n\psi_s]\,dS.
$$

This follows by substituting the [surface representation of an obstacle far-field pattern](#surface-representation-of-an-obstacle-far-field-pattern) and interchanging the integrals.

##### Shape recovery from a Herglotz boundary identity

↑ **Parent:** [Herglotz pairing with an obstacle far field](#herglotz-pairing-with-an-obstacle-far-field)

If measured [far-field patterns](#far-field-pattern) determine a density $g$ and its [Herglotz wave function](#herglotz-wave-function) equals a prescribed spherical wave on the obstacle boundary, that trace identity can locate the boundary. A star-shaped axisymmetric obstacle can be represented by one radial function $h(\theta)$. Numerically, expand $g$ and $h$ in suitable bases, match the far-field constraints, and minimize the complex boundary residual at angular collocation points, using [regularization of an inverse problem](#regularization-of-an-inverse-problem) for noise and small singular values. A single scalar pairing constraint alone does not determine an arbitrary density.

### Scattering potential

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)

For a refractive index $n(\mathbf r)$ and background wavenumber $k_0$, one sign convention defines the scattering potential by $V=k_0^2(1-n^2)$. The total field then satisfies $(\Delta+k_0^2)\psi=V\psi$.

The opposite convention $V=k_0^2(n^2-1)$ gives $(\Delta+k_0^2)\psi=-V\psi$ and reverses the sign attached to the corresponding Green-function integral. Either convention is valid when used consistently.

#### Born approximation for scalar wave scattering

↑ **Parent:** [Scattering potential](#scattering-potential)

Using $V=k_0^2(n^2-1)$, the scalar [Lippmann-Schwinger equation](quantum-mechanics.md#lippmann-schwinger-equation) is $\psi=\psi_i+\int_DG_{k_0}V\psi$. The [Born approximation](quantum-theory.md#born-approximation) replaces the total field inside the integral by the known incident field:

$$
\psi_B=\psi_i+\int_DG_{k_0}(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r'.
$$

For a unit [plane wave](quantum-mechanics.md#plane-wave), its [far-field pattern](#far-field-pattern) is $(4\pi)^{-1}\int_D V(\mathbf r')e^{ik_0(\widehat{\mathbf r}_0-\widehat{\mathbf r})\cdot\mathbf r'}\,d\mathbf r'$. Thus each incident direction samples a shifted sphere in the [Fourier transform](analysis.md#fourier-transform) of the potential.

##### Born non-scattering contrasts at one incident direction

↑ **Parent:** [Born approximation for scalar wave scattering](#born-approximation-for-scalar-wave-scattering)

For real $h\in C_c^\infty(D)$, the displayed real compactly supported contrast has [Fourier transform](analysis.md#fourier-transform) $\widehat V(\boldsymbol\kappa)=[|\boldsymbol\kappa|^4-4(\mathbf k_i\cdot\boldsymbol\kappa)^2]\widehat h(\boldsymbol\kappa)$. This vanishes on the shifted [Ewald sphere](#ewald-sphere) because $|\boldsymbol\kappa|^2+2\mathbf k_i\cdot\boldsymbol\kappa=0$ there. Thus nonzero contrasts can have zero fixed-frequency, fixed-incidence [Born approximation](quantum-theory.md#born-approximation) data. A small amplitude preserves weak contrast and a positive [refractive index](electromagnetism.md#refractive-index).

##### Born series

↑ **Parent:** [Born approximation for scalar wave scattering](#born-approximation-for-scalar-wave-scattering)

The Born series is the [Neumann series](banach-algebra.md#neumann-series) expansion of the [Lippmann-Schwinger equation](quantum-mechanics.md#lippmann-schwinger-equation). Its terms describe successive orders of [wave scattering](physics.md#wave-scattering); convergence is ensured, for example, by a scattering [operator norm](continuous-dual-space.md#operator-norm) smaller than one.

### Rytov approximation

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rytov_approximation)

The Rytov approximation writes a total wave field as $\psi=\psi_i e^\phi$ and linearizes the equation for the complex logarithmic perturbation $\phi$. At first order, $\psi_i\phi$ equals the first [Born approximation](quantum-theory.md#born-approximation) scattered field, so

$$
\psi_R=\psi_i\exp(\psi_{s,B}/\psi_i).
$$

It can remain useful when phase accumulation is appreciable but local scattering is weak.

#### First-Rytov coherent mean

↑ **Parent:** [Rytov approximation](#rytov-approximation)

If the first logarithmic perturbation $\chi_1$ is a centered linear functional of a [Gaussian random field](stochastic-process.md#gaussian-random-field), the [complex Gaussian exponential moment](probability-theory.md#complex-gaussian-exponential-moment) gives the displayed mean of the first [Rytov approximation](#rytov-approximation) $\psi_R=\psi_i e^{\mu\chi_1}$. This is the mean of the truncated logarithmic model. A nonzero mean of the omitted second logarithmic perturbation can change the true field mean at order $\mu^2$.

#### Phase covariance in the first Rytov approximation

↑ **Parent:** [Rytov approximation](#rytov-approximation)

For a centered real [scattering potential](#scattering-potential) fluctuation $W$ and the imaginary part $b$ of the incident-field-weighted [Green function](analysis.md#green-s-function), $\varphi(\mathbf r)=-\int b(\mathbf r,\mathbf r')W(\mathbf r')d\mathbf r'$. Its mean vanishes, and its [covariance function](stochastic-process.md#covariance-function) is the double integral of the two deterministic kernels against the [covariance function](stochastic-process.md#covariance-function) of $W$. The correlation of the [refractive index](electromagnetism.md#refractive-index) itself is insufficient when the [scattering potential](#scattering-potential) depends quadratically on that index.

#### Validity of the first Rytov approximation

↑ **Parent:** [Rytov approximation](#rytov-approximation)

The [Rytov approximation](#rytov-approximation) omits the quadratic gradient source in the [logarithmic wave perturbation](#logarithmic-wave-perturbation) equation. Its next correction solves $\mathcal L_i\chi_2=-\nabla\chi_1\cdot\nabla\chi_1$. Control of the propagated correction, weak [amplitude](physics.md#wave-amplitude) fluctuations and avoidance of field zeros are needed. An appreciable smooth accumulated phase can be retained by exponentiation; small total phase is not the same condition as small local phase gradients.

#### Logarithmic wave perturbation

↑ **Parent:** [Rytov approximation](#rytov-approximation)

The [logarithmic wave perturbation](#logarithmic-wave-perturbation) measures relative [complex amplitude](physics.md#complex-amplitude) and phase through $\psi=\psi_i e^\chi$. A continuous branch requires nonzero incident and total fields in the region considered. For the [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) with [scattering potential](#scattering-potential) convention $L_0\psi=-V\psi$, its equation is $(\Delta+2\nabla\log\psi_i\cdot\nabla)\chi+\nabla\chi\cdot\nabla\chi=-V$. The dot product is bilinear, not a squared modulus.

#### Gaussian intensity in the first Rytov approximation

↑ **Parent:** [Rytov approximation](#rytov-approximation)

Let $\psi_R=\psi_i e^{\phi_1}$ with unit-modulus incidence and $\phi_1=\int_DK(\mathbf r,\mathbf r')V(\mathbf r')\,d\mathbf r'$. For a centered real [Gaussian random field](stochastic-process.md#gaussian-random-field) $V$, the [exponential moment of a Gaussian linear functional](stochastic-process.md#exponential-moment-of-a-gaussian-linear-functional) gives

$$
\mathbb E|\psi_R|^2=\exp\left[\frac12\int_D\int_D a(\mathbf r')a(\mathbf r'')C_V(\mathbf r'-\mathbf r'')\,d\mathbf r'\,d\mathbf r''\right],\qquad a=2\operatorname{Re}K.
$$

Here $C_V$ is the [autocorrelation function of a random field](stochastic-process.md#autocorrelation-function-of-a-random-field). Both the covariance $\mathbb E|\phi_1|^2$ and the generally nonzero term $\operatorname{Re}\mathbb E\phi_1^2$ enter the exponent; dropping the latter is not justified for an arbitrary finite real random medium.

##### Mean-potential correction to weak Rytov intensity

↑ **Parent:** [Gaussian intensity in the first Rytov approximation](#gaussian-intensity-in-the-first-rytov-approximation)

For $n=1+\mu W$ with jointly centered unit-variance [Gaussian random field](stochastic-process.md#gaussian-random-field) $W$, the [scattering potential](#scattering-potential) $V=k_0^2(n^2-1)$ has mean $\mu^2k_0^2$ and covariance $4\mu^2k_0^4C_W+2\mu^4k_0^4C_W^2$. It is not Gaussian. In the far-field [Rytov approximation](#rytov-approximation) let $h(y)=2\operatorname{Re}[B e^{-iq\cdot y}]$, so intensity is $\mathbb E\exp(\int hV)$. Expansion through order $\mu^2$ includes both the mean term and the covariance term shown. The remainder starts at order $\mu^4$ under suitable exponential integrability. Keeping a covariance correction while omitting the same-order mean term is inconsistent. The exact quadratic model uses the [Gaussian quadratic exponential moment](stochastic-process.md#gaussian-quadratic-exponential-moment).

### Far-field pattern

↑ **Parent:** [Inverse scattering problem](#inverse-scattering-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Far-field_pattern)

The far-field pattern is the directional coefficient $f_\infty(\widehat{\mathbf r})$ in an outgoing asymptotic field $u_s(\mathbf r)=e^{ikr}f_\infty(\widehat{\mathbf r})/r+O(r^{-2})$.

#### Far-field approximation for an outgoing source

↑ **Parent:** [Far-field pattern](#far-field-pattern)

For a bounded source region and fixed positive [wavenumber](wave-equation.md#wavenumber), expand $|R\boldsymbol\theta-\mathbf r'|=R-\boldsymbol\theta\cdot\mathbf r'+O(R^{-1})$. In the [outgoing Green function for the three-dimensional Helmholtz equation](partial-differential-equation.md#outgoing-green-function-for-the-three-dimensional-helmholtz-equation), this gives $G=e^{ikR}e^{-ik\boldsymbol\theta\cdot\mathbf r'}/(4\pi R)+O(R^{-2})$. Volume integration gives the outgoing field's [far-field pattern](#far-field-pattern) with an $O(R^{-2})$ remainder. The estimate is an asymptotic statement for fixed source size and frequency.

#### Sommerfeld radiation condition

↑ **Parent:** [Far-field pattern](#far-field-pattern)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sommerfeld_radiation_condition)

The Sommerfeld radiation condition selects outgoing solutions of the exterior [Helmholtz equation](partial-differential-equation.md#helmholtz-equation). In three dimensions it requires $r(\partial_r u-iku)\to0$ as $r\to\infty$ uniformly in direction.

## Well-posed problem

↑ **Parent:** [Inverse problem](inverse-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Well-posed_problem)

A problem is well posed in the sense of Hadamard when a solution exists for every admissible datum, is unique, and depends continuously on the data. Failure of any condition makes it ill posed.

## Regularization of an inverse problem

↑ **Parent:** [Inverse problem](inverse-problem.md)

A regularization is a family of continuous maps $R_\alpha$ such that $R_\alpha f\to A^\dagger f$ as $\alpha\downarrow0$ for every datum in the domain of the [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator). A linear regularization uses bounded [linear operators](vector-space.md#linear-operator); nonlinear [variational regularization](#variational-regularization) can use nonquadratic penalties. A parameter rule that also ensures stability as the data noise tends to zero makes it a [convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem).

### Lavrentiev regularization

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)

For a positive self-adjoint [linear operator](vector-space.md#linear-operator) $A$, Lavrentiev regularization shifts $A$ itself rather than $A^*A$. In a finite-dimensional positive-definite problem, writing $y^\delta=Ax+e$ gives error coefficients $(e_i-\alpha x_i)/(\lambda_i+\alpha)$ in its [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis). Consequently $\|x_\alpha^\delta-x\|\leq\delta/(\lambda_1+\alpha)+\alpha\|x\|/(\lambda_1+\alpha)\leq\delta/\alpha+\alpha\|x\|/\lambda_1$. A known bound $X\geq\|x\|$ permits $\alpha=\sqrt{\delta\lambda_1/X}$, giving a robust bound $2\sqrt{\delta X/\lambda_1}$. For fixed positive $\lambda_1$, the sharper finite-dimensional estimate can give a linear noise rate with a smaller parameter; regularization is then a conditioning choice, not a cure for nonexistence of the inverse.

### Linear regularization

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)

A linear regularization uses a family of [bounded linear operators](topological-vector-space.md#continuous-linear-operator) $R_\alpha$ such that $R_\alpha f\to K^\dagger f$ for each $f\in\mathcal D(K^\dagger)$. A [regularization parameter choice](#regularization-parameter-choice) must balance approximation error with noise amplification to obtain a [convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem).

#### Central-difference noise-bias bound

↑ **Parent:** [Linear regularization](#linear-regularization)

For the mixed forward, [central finite difference](finite-difference.md#central-finite-difference), and backward derivative regularizer on $[0,1]$, with dividing points $(1-\alpha)/2$ and $(1+\alpha)/2$, the [overlap multiplicity bound for piecewise difference operators](#overlap-multiplicity-bound-for-piecewise-difference-operators) has $m=3$. On the middle interval, the error kernel is $\operatorname{sgn}(s)(\alpha/2-|s|)/\alpha$ for $|s|\leq\alpha/2$, with [L1 norm](functional-analysis.md#l1-norm) $\alpha/4$. [Young's convolution inequality](fourier-analysis.md#young-s-convolution-inequality) bounds that part of the bias by $\alpha\|f''\|_2/4$. If the two outer intervals together have squared error at most $\alpha^2\|f''\|_2^2$, combining the three pieces gives the displayed estimate for $\|f''\|_2\leq c$ and $\|f^\delta-f\|_2\leq\delta$. Interpreting $f'$ as the inverse of the [Volterra integration operator](functional-analysis.md#volterra-operator) requires the [range of the Volterra integration operator](functional-analysis.md#range-of-the-volterra-integration-operator) boundary condition $f(0)=0$.

#### Overlap multiplicity bound for piecewise difference operators

↑ **Parent:** [Linear regularization](#linear-regularization)

Suppose a piecewise [finite difference](finite-difference.md) uses two translated evaluations divided by $\alpha$. If the pulled-back evaluation intervals cover almost every input point at most $m$ times, then $|a-b|^2\leq2(|a|^2+|b|^2)$ gives $\|R_\alpha f\|_2^2\leq2m\|f\|_2^2/\alpha^2$. This converts an interval-overlap count into an [operator norm](continuous-dual-space.md#operator-norm) estimate without requiring pointwise values of an [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) equivalence class outside the almost-everywhere evaluation rule.

### Regularization parameter

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)

A regularization parameter controls the tradeoff between approximation bias and data-noise amplification in an [inverse problem](inverse-problem.md). For [early stopping of Landweber iteration](#early-stopping-of-landweber-iteration) with fixed step $\tau$, the convention $\alpha=1/(\tau n)$ associates a smaller parameter with more iterations.

### Convergent regularization of an inverse problem

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)

A regularization $R_\alpha$ is convergent when its parameter can be chosen from the noise level and data so that the regularized reconstruction converges to the exact [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator) solution as the noise level tends to zero.

#### Noise-bias decomposition for linear regularization

↑ **Parent:** [Convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem)

For a bounded linear regularization operator $R_\alpha$ and noisy data with $\|f_\delta-f\|\leq\delta$, the [triangle inequality](topological-analysis.md#triangle-inequality) gives

$$
\|R_\alpha f_\delta-A^\dagger f\|
\leq\delta\|R_\alpha\|+\|R_\alpha f-A^\dagger f\|.
$$

The first term is noise amplification; the second is the approximation bias on exact data. Thus $\alpha(\delta)\to0$ and $\delta\|R_{\alpha(\delta)}\|\to0$ suffice for a [convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem), provided $R_\alpha$ is consistent on exact data.

### Spectral regularization method

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)

A spectral regularization method applies a bounded scalar filter to the spectrum of $A^*A$. In a [singular system of a compact operator](#singular-system-of-a-compact-operator), it has the form

$$
R_\alpha f=\sum_jg_\alpha(\sigma_j^2)\sigma_j\langle f,u_j\rangle v_j,
$$

where the filters approximate $1/\lambda$ while controlling amplification near $\lambda=0$.

#### Asymptotic regularization

↑ **Parent:** [Spectral regularization method](#spectral-regularization-method)

Asymptotic regularization stops the [gradient flow](analysis.md#gradient-flow) $x'=-A^*(Ax-f)$ at $t=1/\alpha$, starting from zero. With the [singular system of a compact operator](#singular-system-of-a-compact-operator) convention $Av_j=\sigma_j u_j$, its spectral filter gives

$$
R_\alpha f=\sum_j\frac{1-e^{-\sigma_j^2/\alpha}}{\sigma_j}\langle f,u_j\rangle v_j.
$$

The scalar coefficient solves $c_j'=-\sigma_j^2c_j+\sigma_j\langle f,u_j\rangle$ with zero initial value. Since $1-e^{-s}\leq\min(s,1)$ for $s\geq0$, the [operator norm](continuous-dual-space.md#operator-norm) is at most $\alpha^{-1/2}$. On the domain of the [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator), [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) of the squared spectral coefficients proves $R_\alpha f\to A^\dagger f$. The [noise-bias decomposition for linear regularization](#noise-bias-decomposition-for-linear-regularization) then gives noisy-data convergence when $\delta/\sqrt\alpha\to0$.

#### Truncated singular value decomposition

↑ **Parent:** [Spectral regularization method](#spectral-regularization-method)

For a [singular value decomposition](linear-algebra.md#singular-value-decomposition) $A v_j=\sigma_j u_j$, truncated SVD with cutoff $\tau>0$ estimates the inverse action by $x_\tau=\sum_{\sigma_j\geq\tau}\sigma_j^{-1}\langle b,u_j\rangle v_j$. Discarding small singular values limits amplification of data errors; this is a [spectral regularization method](#spectral-regularization-method).

Truncated singular value decomposition retains only singular components above a threshold, or equivalently only a finite leading set of singular vectors.

### Tikhonov regularization

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tikhonov_regularization)

Tikhonov regularization minimizes

$$
\lVert Ax-y^\delta\rVert^2+\alpha\lVert x\rVert^2,
$$

giving $x_\alpha^\delta=(A^*A+\alpha I)^{-1}A^*y^\delta$. The spectral filter $\sigma/(\sigma^2+\alpha)$ suppresses unstable division by small singular values.

#### Tikhonov regularization of spherical far-field continuation

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

Let $d_n=ki^{n+1}h_n^{(1)}(kR)$ and map the near-field trace to the far field by $A g=(g_n^m/d_n)_{n,m}$. Quadratic [Tikhonov regularization](#tikhonov-regularization) minimizes $\|Ag-y^\delta\|^2+\alpha\|g\|^2$ and yields the displayed filtered coefficients. Its data-error gain is at most $1/(2\sqrt\alpha)$. Total error also contains bias: $\|g_\alpha^\delta-g^\dagger\|\le\delta/(2\sqrt\alpha)+\|\alpha(A^*A+\alpha I)^{-1}g^\dagger\|$. A convergent parameter rule has $\alpha\to0$ and $\delta/\sqrt\alpha\to0$. Under $g^\dagger=A^*Aw$, $\|w\|\le C$, the bias is at most $C\alpha$; choosing $\alpha=(\delta/(4C))^{2/3}$ minimizes that error bound. Making $\alpha$ indefinitely large removes noise by shrinking the reconstruction to zero, not by recovering the true field.

#### Tikhonov reconstruction from two-plane scattering data

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

The two [Born approximation](quantum-theory.md#born-approximation) measurement operators $A_\pm$ map a supported [scattering potential](#scattering-potential) to fields on planes above and below it. The displayed [Tikhonov regularization](#tikhonov-regularization) functional balances their residuals against a positive quadratic penalty. With an $L^2$ penalty, the unconstrained minimizer is $(A^*A+\alpha I)^{-1}A^*d$, where $A=(A_+,A_-)$. Regularization stabilizes estimation but cannot remove the nonuniqueness of [Born non-scattering contrasts at one incident direction](#born-non-scattering-contrasts-at-one-incident-direction) without extra information.

#### Truncated Tikhonov resolvent

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

For $B=AA^*\ge0$, the polynomial displayed here truncates the [Neumann series](banach-algebra.md#neumann-series) for $(\alpha I+B)^{-1}$. It obeys $(\alpha I+B)R_{\alpha,2}=I+\alpha^{-3}B^3$, and is not an exact inverse. If $\|B\|/\alpha<1$, it is a controlled large-parameter expansion; its error is $\alpha^{-3}B^3(\alpha I+B)^{-1}$. At each fixed positive parameter the reconstruction $A^*R_{\alpha,2}$ is bounded. However this polynomial diverges on nonzero singular modes as $\alpha\to0$ and is not a substitute for the exact convergent Tikhonov filter in that limit.

#### Quadratic norm penalty

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

A squared [Hilbert space](hilbert-space.md) norm penalizes reconstruction size in [Tikhonov regularization](#tikhonov-regularization). For $\alpha>0$, adding $\alpha\|x\|^2$ to $\|Ax-y\|^2$ produces a [strictly convex](real-analysis.md#strictly-convex-function) [coercive function](real-analysis.md#coercive-function) with unique minimizer. Its first variation contributes $\alpha x$ to the [normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem), shifting $A^*A$ to $A^*A+\alpha I$. It selects a minimum-norm representative and controls amplification of noisy small-singular-value components.

#### Singular-system Tikhonov filter

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

For a [singular system of a compact operator](#singular-system-of-a-compact-operator) with $Av_i=\sigma_i u_i$, [Tikhonov regularization](#tikhonov-regularization) gives $x_\alpha=\sum_i g_\alpha(\sigma_i)(y,u_i)v_i$, where $g_\alpha(\sigma)=\sigma/(\sigma^2+\alpha)$ and the [inner product](linear-algebra.md#inner-product) is linear in the first argument. The bounded gain yields a norm-convergent reconstruction; components in $\ker A^*$ are discarded and no component in $\ker A$ is introduced.

#### Tikhonov stability bound

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

The reconstruction operator in [Tikhonov regularization](#tikhonov-regularization) has scalar gain $\sigma/(\sigma^2+\alpha)$. Its maximum over $\sigma\geq0$ is $1/(2\sqrt\alpha)$, so a data perturbation of norm at most $\delta$ changes the solution by at most $\delta/(2\sqrt\alpha)$. A convergent noisy-data parameter choice satisfies $\alpha\to0$ and $\delta/\sqrt\alpha\to0$. Fixed-parameter stability is distinct from stability of the unregularized inverse.

#### Tikhonov filter norm bound

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) between [Hilbert spaces](hilbert-space.md), the [spectral regularization method](#spectral-regularization-method) for quadratic [Tikhonov regularization](#tikhonov-regularization) has scalar coefficient $s/(s^2+\alpha)$. Since $(s-\sqrt\alpha)^2\geq0$, this coefficient is at most $1/(2\sqrt\alpha)$. The [spectral theorem for normal operators](hilbert-space.md#spectral-theorem-for-normal-operators) transfers this scalar bound to the [operator norm](continuous-dual-space.md#operator-norm), providing the noise term in the [noise-bias decomposition for linear regularization](#noise-bias-decomposition-for-linear-regularization).

#### Tikhonov regularization with a coercive penalty operator

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

For [bounded linear operators](topological-vector-space.md#continuous-linear-operator) between [Hilbert spaces](hilbert-space.md) with $\|Bu\|\geq\beta\|u\|$ and $\beta>0$, the operator $K^*K+\alpha B^*B$ is coercive and invertible for $\alpha>0$. The reconstruction uniquely minimizes $\|Ku-f\|^2/2+\alpha\|Bu\|^2/2$. Testing its [normal equation for coercive Tikhonov regularization](#normal-equation-for-coercive-tikhonov-regularization) by $u$ gives $\|R_\alpha\|\leq1/(2\beta\sqrt\alpha)$. If $K$ is injective, exact-data consistency and $\alpha\to0$, $\delta/\sqrt\alpha\to0$ give [norm convergence](functional-analysis.md#norm-convergence) to $K^\dagger f$.

##### Approximate source bound for coercive Tikhonov regularization

↑ **Parent:** [Tikhonov regularization with a coercive penalty operator](#tikhonov-regularization-with-a-coercive-penalty-operator)

Let $K$ be injective, $u^\dagger=K^\dagger f$, $z=\beta^{-2}B^*Bu^\dagger$, and $\eta_r=\inf_{\|w\|\leq r}\|z-K^*w\|$. Since $\overline{\mathcal R(K^*)}=\mathcal N(K)^\perp=U$, $\eta_r\to0$. For $e=R_\alpha f-u^\dagger$ the [normal equation for coercive Tikhonov regularization](#normal-equation-for-coercive-tikhonov-regularization) gives $\|Ke\|^2+\alpha\|Be\|^2=-\alpha\beta^2\langle z,e\rangle$. Insert an approximate $K^*w$ and complete the square in $\|Ke\|$ to obtain $\|e\|^2\leq\|z-K^*w\|\|e\|+\alpha\beta^2r^2/4$. This implies the displayed bound, even with coefficient $1/2$ on its last term, and proves consistency without a fixed exact [source condition for quadratic regularization](#source-condition-for-quadratic-regularization).

##### Normal equation for coercive Tikhonov regularization

↑ **Parent:** [Tikhonov regularization with a coercive penalty operator](#tikhonov-regularization-with-a-coercive-penalty-operator)

For [bounded linear operators](topological-vector-space.md#continuous-linear-operator) $K:U\to V$ and $B:U\to W$ between real [Hilbert spaces](hilbert-space.md), $\alpha>0$ and $\|Bu\|\geq\beta\|u\|$ with $\beta>0$, the unique minimizer of $\|Ku-f\|^2/2+\alpha\|Bu\|^2/2$ satisfies $(K^*K+\alpha B^*B)u_\alpha=K^*f$. Differentiate the objective in every direction and use the [adjoint operator](hilbert-space.md#adjoint-operator) to obtain this equation. The coercive quadratic penalty makes its left-hand operator boundedly invertible. Setting $B=I$ gives the [Tikhonov normal equation](#tikhonov-normal-equation); omitting the penalty instead gives the [normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem).

#### Source condition for quadratic regularization

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

This range condition puts the exact solution in the [operator range](topological-vector-space.md#range-of-a-bounded-linear-operator) of the [adjoint operator](hilbert-space.md#adjoint-operator). It controls the small-[singular value](linear-algebra.md#singular-value) components of the solution and supplies convergence rates for [spectral regularization methods](#spectral-regularization-method). It is the quadratic-penalty case of a [source condition in variational regularization](#source-condition-in-variational-regularization).

#### Tikhonov normal equation

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

The unique minimizer of $\|Au-f\|^2+\alpha\|u\|^2$ satisfies

$$
(A^*A+\alpha I)u=A^*f.
$$

#### Spectral filter

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

A spectral filter replaces unstable inversion of a singular value $\sigma$ by a bounded scalar factor $g_\alpha(\sigma)$. For Tikhonov regularization, $g_\alpha(\sigma)=\sigma/(\sigma^2+\alpha)$.

##### Evenization of a nonnegative bandlimited filter

↑ **Parent:** [Spectral filter](#spectral-filter)

For a nonzero nonnegative integrable [bandlimited function](analysis.md#bandlimited-function) $f$ with frequency support in $[-\Delta,\Delta]$, the displayed construction is even, nonnegative and normalizable. Each factor has half-width frequency support, so their product retains width $\Delta$. Boundedness gives $\int_T^\infty w(t)dt\leq2C\|f\|_\infty\int_{T/2}^\infty f(u)du$. Thus a positive-time tail estimate becomes a two-sided estimate after evenization, with a rescaled decay constant. A simple average with $f(-t)$ would not establish this from an uncontrolled negative tail.

#### Regularization parameter choice

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

A regularization parameter choice selects the amount of stabilization from the noise level, the measured data, or both. For Tikhonov regularization with deterministic error at most $\delta$, a sufficient a priori condition for convergence is $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$.

##### Balancing noise and approximation bias

↑ **Parent:** [Regularization parameter choice](#regularization-parameter-choice)

An error bound $A\delta/\alpha+Bc\alpha$, with positive $A,B,c$, is minimized at $\alpha_* =\sqrt{A\delta/(Bc)}$, with value $2\sqrt{ABc\delta}$. Differentiate the scalar bound, or apply the arithmetic-geometric mean inequality. This is an [a priori regularization parameter choice](#a-priori-regularization-parameter-choice) for a [linear regularization](#linear-regularization) with inverse-parameter noise amplification and first-order approximation bias; the parameter must also lie in the method's allowed interval.

##### A priori regularization parameter choice

↑ **Parent:** [Regularization parameter choice](#regularization-parameter-choice)

An a priori regularization parameter choice depends on a known noise bound and fixed problem information, but not on the observed values of the noisy data.

#### Iterated Tikhonov regularization

↑ **Parent:** [Tikhonov regularization](#tikhonov-regularization)

Iterated Tikhonov regularization repeatedly applies a filtered correction based on $A^*(y-Ax_n)$. Its singular-system representation exposes the iteration as a family of scalar spectral filters.

##### Iterated Tikhonov spectral filter

↑ **Parent:** [Iterated Tikhonov regularization](#iterated-tikhonov-regularization)

The implicit iteration $(I+\tau K^*K)u_{k+1}=u_k+\tau K^*f$, starting from zero, multiplies each data [singular vector](semisimple-lie-algebra.md#singular-vector) by $[1-(1+\tau\sigma^2)^{-k}]/\sigma$. Its [operator norm](continuous-dual-space.md#operator-norm) is at most $\sqrt{k\tau}$.

### Variational regularization

↑ **Parent:** [Regularization of an inverse problem](#regularization-of-an-inverse-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variational_regularization)

Variational regularization balances data fidelity against a lower-semicontinuous penalty, for example by minimizing $\frac12\lVert Au-f\rVert^2+\alpha J(u)$.

#### Discrete Hessian-norm denoising

↑ **Parent:** [Variational regularization](#variational-regularization)

Replacing a discrete [gradient](calculus.md#gradient) by a second-difference operator $H:X\to X^4$ gives the global-norm penalty $\alpha\|Hu\|_2$. Its reconstruction is $g-P_Cg$ for $C=H^*B_\alpha$. Components in $\ker H$ are preserved; affine-image membership of this kernel depends on the boundary stencil. Pixelwise Hessian penalties instead use a product of four-component balls.

#### Global discrete gradient-norm denoising

↑ **Parent:** [Variational regularization](#variational-regularization)

For a discrete [image signal](computer-science.md#image-signal) operator $A$, minimize $\alpha\|Au\|_2+\tfrac12\|u-g\|_2^2$ with one [Euclidean norm](functional-analysis.md#euclidean-norm) on the full [gradient](calculus.md#gradient) array. This differs from [discrete isotropic total variation](#discrete-isotropic-total-variation), which sums pixelwise Euclidean lengths. The global [norm](functional-analysis.md#norm)'s dual ball is a single ball; its [convex projection](mathematical-optimization.md#euclidean-projection-onto-a-convex-set) normalizes the whole vector array.

##### Global gradient-norm projection residual

↑ **Parent:** [Global discrete gradient-norm denoising](#global-discrete-gradient-norm-denoising)

Let $C=A^*B_\alpha$ with one global dual ball. Its [support function](mathematical-optimization.md#support-function) is $\alpha\|Au\|_2$, and the [proximal operator of a support function](convex-optimization.md#proximal-operator-of-a-support-function) gives $u=g-P_Cg$. The removed component is the [convex projection](mathematical-optimization.md#euclidean-projection-onto-a-convex-set), while the reconstructed [image signal](computer-science.md#image-signal) is its residual. [Projected gradient descent](convex-optimization.md#projected-gradient-descent) on $\tfrac12\|g-A^*p\|_2^2$, $p\in B_\alpha$, converges for $0<\tau<2/\|A\|^2$.

#### Poisson data fidelity

↑ **Parent:** [Variational regularization](#variational-regularization)

For positive observations $y$ and positive predicted intensities $s$, this is the [generalized Kullback–Leibler divergence](probability-and-statistics.md#generalized-kullback-leibler-divergence) with observation in the first argument. Its scalar derivative in $s$ is $1-y/s$ and its second derivative is $y/s^2>0$. It differs from the divergence of a reconstructed density from a reference density by which argument is varied. A linear prediction $s=Kx$ gives derivative $K^*(1-y/(Kx))$ through the [adjoint operator](hilbert-space.md#adjoint-operator), on suitable admissible function spaces. This fidelity arises from the negative log likelihood of a [Poisson observation model](discrete-probability-distribution.md#poisson-observation-model), after removal of terms depending only on observations.

##### Shifted Poisson data fidelity

↑ **Parent:** [Poisson data fidelity](#poisson-data-fidelity)

For $u\ge0$ and a [positivity-preserving operator](topological-vector-space.md#positivity-preserving-linear-operator-on-l1), this is the negative [log-likelihood](statistical-modelling.md#log-likelihood) for independent [Poisson observations](discrete-probability-distribution.md#poisson-observation) with intensity $1+Tu$, up to constants depending only on the data and the unit background. For bounded $g\ge0$, its scalar [derivatives](calculus.md#derivative) are $1-g/(1+s)$ and $g/(1+s)^2$ on $s=Tu\ge0$. It is [convex](real-analysis.md#convex-function), and [strictly convex](real-analysis.md#strictly-convex-function) in the predicted intensity when $g>0$ almost everywhere. On a unit-area domain, the [Jensen inequality](real-analysis.md#jensen-s-inequality) gives $D_g(u)\ge\|Tu\|_1-\|g\|_\infty\log(1+\|Tu\|_1)$. The shift makes $\log(1+Tu)$ integrable whenever $Tu\in L^1$; no integrability of $\log u$ is needed.

###### Existence for nonnegative shifted Poisson regularization

↑ **Parent:** [Shifted Poisson data fidelity](#shifted-poisson-data-fidelity)

Let $\Omega$ be a bounded connected [Lipschitz domain](real-analysis.md#lipschitz-domain), $\alpha>0$, $g\ge0$ bounded, and $T:L^1\to L^1$ bounded and positivity preserving with $T1\ne0$. Minimize $\alpha\operatorname{TV}(u)+D_g(u)$ over nonnegative [BV space](#function-of-bounded-variation-on-a-domain) functions. The logarithmic [Jensen inequality](real-analysis.md#jensen-s-inequality) bounds $\|Tu\|_1$ and variation on sublevels; [mean control for positive imaging operators](topological-vector-space.md#mean-control-for-positive-imaging-operators) then bounds the full $BV$ [norm](functional-analysis.md#norm). [Bounded-variation compactness](#bounded-variation-compactness) gives strong $L^1$ convergence, including nonnegativity. The scalar fidelity has bounded [derivative](calculus.md#derivative) on $s\ge0$, so [continuity](calculus.md#continuous-function) of $T$ makes its integral [continuous](calculus.md#continuous-function) in that [limit](calculus.md#limit-of-a-function). [Lower semicontinuity](calculus.md#lower-semicontinuity) of variation proves existence by the [direct method in the calculus of variations](calculus-of-variations.md#direct-method-in-the-calculus-of-variations). If $g>0$ almost everywhere and $T$ is [injective](algebra.md#injective-function), strict [convexity](real-analysis.md#convex-function) of the fidelity gives uniqueness. For $0<g<1$, zero is the unique [minimizer](analysis.md#global-minimizer) even without injectivity, since zero energy forces both $Tu=0$ and a constant nonnegative $u$.

###### Nonattainment under strict positivity for shifted Poisson fidelity

↑ **Parent:** [Shifted Poisson data fidelity](#shifted-poisson-data-fidelity)

On a bounded domain, suppose $0<g<1$, $\alpha>0$, and a bounded [positivity-preserving operator](topological-vector-space.md#positivity-preserving-linear-operator-on-l1) satisfies $T1\ne0$. Every strictly positive $u$ has $Tu\ne0$: otherwise $T\chi_{\{u\ge1/n\}}=0$ for all $n$, and [continuity](calculus.md#continuous-function) gives $T1=0$. Since $s-g\log(1+s)>0$ whenever $s>0$, every such $u$ has positive energy. The constants $u=\varepsilon$ have zero variation and energy at most $\varepsilon\|T1\|_1\to0$. Their excluded zero [limit](calculus.md#limit-of-a-function) proves nonattainment. [Coercivity](real-analysis.md#coercive-function) and [bounded-variation compactness](#bounded-variation-compactness) cannot by themselves preserve a nonclosed strict-positivity constraint.

##### Proximal operator of Poisson data fidelity

↑ **Parent:** [Poisson data fidelity](#poisson-data-fidelity)

For $y>0$ and $\gamma>0$, minimizing $|x-z|^2/2+\gamma[y\log(y/x)+x-y]$ on $x>0$ gives $x^2+(\gamma-z)x-\gamma y=0$. The roots have opposite signs, so only the displayed positive root belongs to the effective domain. Strict positivity of the second derivative proves uniqueness. For an integral [Poisson data fidelity](#poisson-data-fidelity), the [proximal operator](convex-optimization.md#proximal-operator) separates pointwise under the appropriate integrability assumptions.

#### Maximum-entropy regularization functional

↑ **Parent:** [Variational regularization](#variational-regularization)

This [convex function](real-analysis.md#convex-function) penalizes positive densities using negative entropy, with $0\log0=0$ and infinite value for negative inputs. Its scalar derivative is $\log x$ on $x>0$. On a bounded domain, restricting to uniformly positive bounded functions gives a simple setting for a [Fréchet derivative](calculus.md#frechet-derivative). Its [Bregman distance](#bregman-divergence) is the [generalized Kullback–Leibler divergence](probability-and-statistics.md#generalized-kullback-leibler-divergence). With fixed total mass, minimizing this negative-entropy expression maximizes the corresponding entropy.

#### Data compatibility with the regularizer domain

↑ **Parent:** [Variational regularization](#variational-regularization)

Exact fitting in the small-parameter limit requires data that can be approximated by forward images of elements in the regulariser's [effective domain](real-analysis.md#effective-domain). Membership merely in the [operator range](topological-vector-space.md#range-of-a-bounded-linear-operator) is insufficient when an extended-real regulariser imposes a hard constraint.

#### Value function of variational regularization

↑ **Parent:** [Variational regularization](#variational-regularization)

For a nonnegative regulariser $J$, the optimal objective value is non-decreasing and [concave](real-analysis.md#concave-function) in the positive regularization parameter. If $J(0)=0$ and $D(0)<\infty$, comparison with zero makes it finite and a [locally Lipschitz function](real-analysis.md#locally-lipschitz-function) away from parameter zero.

##### Monotonicity of data fidelity and regularization penalty

↑ **Parent:** [Value function of variational regularization](#value-function-of-variational-regularization)

For $0<\alpha<\beta$, choosing [global minimizers](analysis.md#global-minimizer) of $D+\alpha J$ and $D+\beta J$ gives $J(u_\beta)\leq J(u_\alpha)$ and $D(u_\beta)\geq D(u_\alpha)$. The decrease in penalty and increase in data misfit satisfy $\alpha\Delta J\leq\Delta D\leq\beta\Delta J$.

#### Parameter continuity of variational regularization

↑ **Parent:** [Variational regularization](#variational-regularization)

For objectives $D+\alpha J$ with $J\ge0$ and positive parameter, suppose nearby-parameter [global minimizers](analysis.md#global-minimizer) have uniformly bounded penalty, stay in a bounded set with [convergent subsequences](real-analysis.md#convergent-subsequence), and $D$ and $J$ are [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity) in the chosen [topology](topology.md). Their optimality inequalities and lower semicontinuity show that every subsequential limit minimizes the limiting objective. Uniqueness makes the regularized solution [continuous](calculus.md#continuous-function) in the parameter. Existence alone does not make an arbitrary selection among multiple [global minimizers](analysis.md#global-minimizer) [continuous](calculus.md#continuous-function).

#### Quartic-norm variational regularization

↑ **Parent:** [Variational regularization](#variational-regularization)

For a bounded [linear operator](vector-space.md#linear-operator) $A$ between [Hilbert spaces](hilbert-space.md), minimize $\|Au-f\|^2+\alpha\|u\|^4$, with $\alpha>0$. The objective is coercive and weakly lower semicontinuous, and its [strictly convex](real-analysis.md#strictly-convex-function) norm penalty gives a unique minimizer. Its stationarity equation is

$$
A^*(Au-f)+2\alpha\|u\|^2u=0,
$$

so the map from data to solution is generally nonlinear. For admissible fixed $f$, comparison with $u^\dagger=A^\dagger f$ bounds the minimizer's norm by $\|u^\dagger\|$ and makes its squared residual converge to the minimum least-squares residual. Every weak cluster point is therefore a least-squares solution of norm at most $\|u^\dagger\|$, hence equals the [minimum-norm least-squares solution](#minimum-norm-least-squares-solution). Weak lower semicontinuity then forces convergence of norms, and the [Radon-Riesz theorem](hilbert-space.md#radon-riesz-theorem) gives strong convergence. This supplies a nonlinear [regularization of an inverse problem](#regularization-of-an-inverse-problem).

For completeness, the fixed-$\alpha$ data-to-solution map is continuous. For $g(u)=\|u\|^2u$, setting $m=(u+v)/2$ and $d=(u-v)/2$ gives

$$
\operatorname{Re}\langle g(u)-g(v),u-v\rangle
=4(\|m\|^2+\|d\|^2)\|d\|^2+8(\operatorname{Re}\langle m,d\rangle)^2
\geq\tfrac14\|u-v\|^4.
$$

Subtracting the stationarity equations for data $f,h$ and pairing with $u-v$ therefore gives $\frac\alpha2\|u-v\|^4\leq\|A\|\|f-h\|\|u-v\|$. Thus

$$
\|R_\alpha f-R_\alpha h\|\leq\left(\frac{2\|A\|}{\alpha}\|f-h\|\right)^{1/3},
$$

which proves continuity directly.

#### J-minimizing solution

↑ **Parent:** [Variational regularization](#variational-regularization)

For an exact equation $Au=f$ and a penalty $J$, a $J$-minimizing solution is a feasible point $u_J^\dagger$ such that

$$
J(u_J^\dagger)=\inf\{J(u):Au=f\}.
$$

#### Residual method for variational regularization

↑ **Parent:** [Variational regularization](#variational-regularization)

Given $\|f_\delta-f\|\leq\delta$, the residual method minimizes a penalty $J(u)$ subject to $\|Au-f_\delta\|\leq\delta$. Every exact solution is feasible, so a reconstruction $u_\delta$ has penalty no larger than that of any [J-minimizing solution](#j-minimizing-solution).

##### Compact-sublevel convergence of the residual method

↑ **Parent:** [Residual method for variational regularization](#residual-method-for-variational-regularization)

Suppose $J$ is nonnegative and [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity), and its sublevel sets are strongly sequentially compact. For a solvable exact equation $Au=f$, every sequence of residual-method minimizers with $\delta\to0$ has a strongly convergent subsequence, and every limit is a [J-minimizing solution](#j-minimizing-solution). Indeed, comparison with an exact penalty minimizer bounds all reconstructions in one compact sublevel set; the residual bound gives $\|Au_\delta-f\|\leq2\delta$. Continuity of $A$ and lower semicontinuity of $J$ identify each subsequential limit as an exact minimizer. Thus the [distance to a set](topological-analysis.md#distance-to-a-set) of exact penalty minimizers tends to zero. Uniqueness of the exact minimizer upgrades this to full [strong convergence](functional-analysis.md#norm-convergence).

Uniqueness cannot be omitted: for $A=0$, $f_\delta=f=0$, and $J(u)=\max\{|u|-1,0\}$ on $\mathbb R$, the sublevel sets are compact intervals but the minimizers $u_{1/k}=(-1)^k$ do not converge.

#### Total variation seminorm on a domain

↑ **Parent:** [Variational regularization](#variational-regularization)

For $u\in L^1(\Omega)$, the total variation seminorm is

$$
\operatorname{TV}(u)=\sup_{\substack{\varphi\in C_c^1(\Omega;\mathbb R^n)\\\|\varphi\|_\infty\leq1}}
\int_\Omega u\,\operatorname{div}\varphi\,dx.
$$

It extends the integral of the magnitude of the [gradient](calculus.md#gradient) to nonsmooth functions.

##### Total variation under opposite smooth flows

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

For the [local flow](differential-geometry.md#local-flow) of a smooth compactly supported [vector field](calculus.md#vector-field) and any scalar [BV space](#function-of-bounded-variation-on-a-domain) function $w$, the [change of variables formula](calculus.md#change-of-variables-formula) and [polar decomposition of a vector measure](measure-theory.md#polar-decomposition-of-a-vector-measure) give

$$
\operatorname{TV}(w\circ\Phi_t)=\int|\operatorname{cof}(D\Phi_{-t})\sigma_w|\,d|Dw|.
$$

The two [cofactor matrices](linear-algebra.md#cofactor-matrix) are $I\pm tB+O(t^2)$ uniformly. On $|\sigma_w|=1$, the linear terms in their Euclidean [norm](functional-analysis.md#norm) expansions cancel. Integration bounds the remainder by $Ct^2|Dw|(\Omega)$. The identity includes all components of the [decomposition of a BV derivative](#decomposition-of-a-bv-derivative); it does not require smoothness of $w$ or its jump interfaces.

##### Total variation calibration

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

For an [absolutely one-homogeneous functional](convex-optimization.md#absolutely-one-homogeneous-functional) $J=\operatorname{TV}$ on a real [Hilbert space](hilbert-space.md), a [subgradient](real-analysis.md#subgradient) $q$ at $u$ is characterized by $\langle q,v\rangle\le J(v)$ for every $v$ and $\langle q,u\rangle=J(u)$. A bounded [vector](vector-space.md#vector) field with $|z|\le1$ and $q=\operatorname{div}z$ proves the inequality through the dual definition, provided cutoff approximation is valid in the ambient space. Equality is called a calibration. It certifies a global minimizer of [total variation denoising](#total-variation-denoising), rather than only a minimizer within a chosen ansatz.

##### Total variation flow

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

Total variation flow is the $L^2$ [gradient flow](analysis.md#gradient-flow) of the [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain). Formally it is $u_t=\operatorname{div}(\nabla u/|\nabla u|)$, but the [subgradient](real-analysis.md#subgradient) formulation handles zero gradients and jumps. Adding quadratic fidelity gives a [strictly convex](real-analysis.md#strictly-convex-function) stationary [total variation denoising](#total-variation-denoising) problem.

##### Total variation denoising

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

For $g\in L^2$ on a bounded domain, total variation denoising has a unique minimizer. A bounded minimizing sequence has a weakly convergent $L^2$ subsequence; variation is a supremum of weakly continuous test-function pairings and the fidelity has [weak lower semicontinuity](functional-analysis.md#weak-lower-semicontinuity). The [strictly convex](real-analysis.md#strictly-convex-function) fidelity proves uniqueness. [Bounded-variation contraction under clipping](#bounded-variation-contraction-under-clipping) proves that data range bounds pass to the minimizer.

###### Box-constrained TV-L1 denoising

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

This finite-image [convex optimization](convex-optimization.md) model combines robust [L1 norm](functional-analysis.md#l1-norm) fidelity with [discrete isotropic total variation](#discrete-isotropic-total-variation) and pixel-range constraints. An exact [second-order cone program](mathematical-optimization.md#second-order-cone-programming) uses two orthant fidelity slacks per pixel, two box slacks per pixel and a three-dimensional [Lorentz cone](mathematical-optimization.md#second-order-cone) for each gradient magnitude. The product canonical barrier has parameter $6n$ for $n$ pixels.

###### Jump-amplitude inequality for total variation denoising

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

For scalar [total variation denoising](#total-variation-denoising) with $f\in BV(\Omega)\cap L^2(\Omega)$ on a bounded [Lipschitz domain](real-analysis.md#lipschitz-domain) in arbitrary dimension, the inequality holds with common oriented [BV traces on a hypersurface](#bv-trace-on-a-hypersurface). It says that every surviving jump has the same direction as its data jump and no larger amplitude. Reversing the normal changes both differences and preserves the inequality.

Use [residual-preserving clipping of an ROF minimizer](#residual-preserving-clipping-of-an-rof-minimizer) and the [jump-amplitude inequality for a bounded ROF minimizer](#jump-amplitude-inequality-for-a-bounded-rof-minimizer). At each finite jump, choose an integer clipping level above both output traces. The clipped function has those same traces, and its residual-adjusted data have the same traces as $f$. Taking a countable union over the integer clipping levels proves the result. This gives the [no-new-jumps property of total variation denoising](#no-new-jumps-property-of-total-variation-denoising) under the full $L^2\cap BV$ assumptions, without asserting regularity of unbounded-forcing perimeter [minimizers](analysis.md#global-minimizer).

###### No-new-jumps property of total variation denoising

↑ **Parent:** [Jump-amplitude inequality for total variation denoising](#jump-amplitude-inequality-for-total-variation-denoising)

For scalar [total variation denoising](#total-variation-denoising) with $f\in BV(\Omega)\cap L^2(\Omega)$ on a bounded [Lipschitz domain](real-analysis.md#lipschitz-domain) in arbitrary dimension, the reconstructed [jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function) lies in the data [jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function) up to a surface-null set. The [jump-amplitude inequality for total variation denoising](#jump-amplitude-inequality-for-total-variation-denoising) proves this: outside $J_f$, the two [BV traces on a hypersurface](#bv-trace-on-a-hypersurface) of $f$ agree, so $[u]([f]-[u])\ge0$ forces $[u]=0$. Surviving jumps cannot be stronger than the corresponding data jumps and must have the same orientation. Existing jumps may disappear.

The proof uses [scalar total variation splitting under clipping](#scalar-total-variation-splitting-under-clipping), [residual-preserving clipping of an ROF minimizer](#residual-preserving-clipping-of-an-rof-minimizer), [total variation under opposite smooth flows](#total-variation-under-opposite-smooth-flows) and the [BV jump-product limit with one bounded factor](#bv-jump-product-limit-with-one-bounded-factor). It requires neither bounded data nor bounded output. The bounded-forcing geometric proof through [noncontact of ROF level boundaries](#noncontact-of-rof-level-boundaries) remains an alternative for bounded images; it is not used to infer regularity under unbounded forcing.

###### Jump-amplitude inequality for a bounded ROF minimizer

↑ **Parent:** [Jump-amplitude inequality for total variation denoising](#jump-amplitude-inequality-for-total-variation-denoising)

Assume $w\in BV\cap L^\infty$ minimizes scalar [total variation denoising](#total-variation-denoising) for $g\in BV\cap L^2$. The data $g$ may be unbounded. For the [local flow](differential-geometry.md#local-flow) of $\varphi e_j$, use $(1-\theta)w+\theta w\circ\Phi_{\pm t}$ as two competitors. The [total variation under opposite smooth flows](#total-variation-under-opposite-smooth-flows) and convexity of the [total variation seminorm](#total-variation-seminorm-on-a-domain) bound the sum of regularizer changes by $O(t^2)$. Minimality and the [opposite-flow fidelity identity for quadratic data](#opposite-flow-fidelity-identity-for-quadratic-data), evaluated using the [BV jump-product limit with one bounded factor](#bv-jump-product-limit-with-one-bounded-factor), imply

$$
\int_{J_w}([g][w]-(1-\theta)[w]^2)\varphi|\nu_w\cdot e_j|\,d\mathcal H^{n-1}\ge0.
$$

Let $\theta\downarrow0$. The integrands define finite signed [Radon measures](measure-theory.md#radon-measure), since $w$ is bounded and the jump variation of $g$ is finite. Arbitrary nonnegative smooth $\varphi$ make their densities nonnegative. Testing every coordinate direction removes the factor $|\nu_w\cdot e_j|$ and proves the stated inequality.

###### Residual-preserving clipping of an ROF minimizer

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

If $u$ minimizes scalar [total variation denoising](#total-variation-denoising) with $f\in BV\cap L^2$, set $w=T_Mu$, $r=u-w$ and $g=f-r$. The [scalar total variation splitting under clipping](#scalar-total-variation-splitting-under-clipping) gives $\operatorname{TV}(u)=\operatorname{TV}(w)+\operatorname{TV}(r)$. Compare $u$ with $v+r$ and use $\operatorname{TV}(v+r)\le\operatorname{TV}(v)+\operatorname{TV}(r)$; cancelling the tail shows that $w$ minimizes the same model for $g$. It is bounded while $g$ may be unbounded, and $w-g=u-f$ exactly. This reduction concerns the actual [minimizer](analysis.md#global-minimizer), rather than convergence of [minimizers](analysis.md#global-minimizer) for truncated data.

###### Quadratic fidelity

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

The squared-error term $\frac12\|u-f\|_2^2$ is a [strictly convex](real-analysis.md#strictly-convex-function) cost measuring agreement with data.

###### Opposite-flow fidelity identity for quadratic data

↑ **Parent:** [Quadratic fidelity](#quadratic-fidelity)

Let $w\in BV\cap L^\infty$ and $g\in BV\cap L^2$ on a bounded domain, $F_g(v)=\tfrac12\|v-g\|_2^2$, and $w_{\pm t}=(1-\theta)w+\theta w\circ\Phi_{\pm t}$ for a smooth compactly supported [local flow](differential-geometry.md#local-flow). The displayed formula is exact to an $o(t)$ remainder, and $g$ need not be bounded. Writing $J_t=\det D\Phi_t$, its cross-term identity is

$$
\int g(\delta_tw+\delta_{-t}w)=-\int\delta_tg\,\delta_tw+\int g(1-J_{-t})\delta_{-t}w.
$$

The remainder is $o(t)$ because $1-J_{-t}=O(t)$ and weighted $L^1$ convergence follows from

$$
\int|g||\delta_{-t}w|\le K\|\delta_{-t}w\|_1+2\|w\|_\infty\int_{|g|>K}|g|.
$$

First let $t\to0$, then $K\to\infty$. The mass change of $w^2$ under opposite flows is $O(t^2)\|w\|_2^2$. Combined with the [BV jump-product limit with one bounded factor](#bv-jump-product-limit-with-one-bounded-factor), this evaluates the jump contribution without a bounded fidelity derivative.

###### ROF level-set formulation

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

The scalar [ROF denoising](#total-variation-denoising) [minimizer](analysis.md#global-minimizer) has perimeter-plus-forcing minimizing [superlevel sets](topology.md#superlevel-set) at almost every height. Conversely any finite-energy function with that property minimizes the full energy. The [signed layer-cake identity for quadratic fidelity](#signed-layer-cake-identity-for-quadratic-fidelity) and [coarea formula for BV functions](#coarea-formula-for-bv-functions) prove sufficiency. To prove necessity, construct nested minimizing sets using [comparison of perimeter minimizers with ordered forcing](#comparison-of-perimeter-minimizers-with-ordered-forcing), reconstruct a function from rational levels, clip to establish energy bounds, and use uniqueness from [strict convexity](real-analysis.md#strictly-convex-function) of the squared fidelity.

###### Noncontact of ROF level boundaries

↑ **Parent:** [ROF level-set formulation](#rof-level-set-formulation)

For bounded [BV space](#function-of-bounded-variation-on-a-domain) data and $s<t$, nested [ROF level-set formulation](#rof-level-set-formulation) minimizing sets cannot share an interface of positive surface [measure](measure-theory.md#measure) away from data jumps. On regular graph patches, upward and downward [first variations](calculus-of-variations.md#first-variation) use the [BV traces on a hypersurface](#bv-trace-on-a-hypersurface). At contacts outside $J_f$ the forcing [BV trace on a hypersurface](#bv-trace-on-a-hypersurface) agrees, whereas the two levels differ by $t-s$. Graph regularity and contact differentiation give the contradiction. Bounded forcing is a hypothesis of this argument; arbitrary unbounded $L^2\cap BV$ data are not covered by this statement.

###### Signed layer-cake identity for quadratic fidelity

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

For positive $u$, integrate $t-f$ from zero to $u$; for negative $u$, reverse the integral from $u$ to zero. This proves the identity without a positivity restriction on the data. For $u,f\in L^2$, the absolute integral is bounded by $u^2/2+|fu|$, so [Fubini's theorem](measure-theory.md#fubini-s-theorem) applies. The zero-function baseline removes the divergence from the negative-height tail.

###### Constrained-penalized equivalence for total variation denoising

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

For finite convex [total variation](real-analysis.md#total-variation) and a positive squared-error budget, the [Slater condition](mathematical-optimization.md#slater-s-condition) supplies a multiplier $\lambda\geq0$ such that every constrained minimizer also minimizes $\operatorname{TV}(u)+\lambda\|u-g\|^2$. Conversely, a minimizer of that penalized objective with $\lambda>0$ minimizes total variation under the budget equal to its own squared error. [Complementary slackness](mathematical-optimization.md#complementary-slackness) proves the first implication; a comparison of objective values proves the second. This does not assert uniqueness of the multiplier or equality of all minimizer sets when $\lambda=0$.

###### Graph total variation

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

The graph total variation measures absolute variation of a vertex signal across [edges](graph-theory.md#edge-of-a-graph). It is independent of the orientation used for the [oriented incidence matrix](graph.md#oriented-incidence-matrix). It vanishes exactly on signals constant on each [connected component of a graph](graph.md#component-graph-theory). A [graph total variation denoising](#graph-total-variation-denoising) estimator combines this penalty with squared error, favouring signals that are piecewise constant on connected regions.

###### Graph total variation denoising

↑ **Parent:** [Graph total variation](#graph-total-variation)

Graph total variation denoising is a [penalized least-squares estimator](statistical-learning.md#penalized-least-squares-estimator) for noisy vertex signals on a [graph](graph.md). The squared loss is strictly [convex](real-analysis.md#convex-function), so the fitted signal is unique. Its [basic inequality for a penalized least-squares estimator](statistical-learning.md#basic-inequality-for-a-penalized-least-squares-estimator) separates a noise inner product from the change in penalty. The [incidence pseudoinverse decomposition](graph.md#incidence-pseudoinverse-decomposition) controls the nonconstant noise through the geometry of the [graph](graph.md).

###### Total variation denoising of a disk

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

For data $g=\chi_{B(0,R)}$ on $\mathbb R^2$, the minimizer of $\alpha\operatorname{TV}(u)+\tfrac12\|u-g\|_2^2$ is the displayed amplitude shrinkage, including extinction at $\alpha=R/2$. The [total variation calibration](#total-variation-calibration) uses $z(x)=x/R$ inside the disk and $z(x)=Rx/|x|^2$ outside. Its [continuous](calculus.md#continuous-function) normal component creates no boundary measure, and $\operatorname{div}z=(2/R)\chi_{B(0,R)}$. This [subgradient](real-analysis.md#subgradient) certifies the positive branch; scaling it down certifies the zero branch. The quadratic fidelity is [strictly convex](real-analysis.md#strictly-convex-function), ensuring uniqueness.

###### Staircasing in total variation denoising

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

Staircasing is the formation of approximately constant plateaux in reconstructed data, even when the original data vary smoothly. The linear growth of the [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain) favors sparse spatial gradients, so preserving jumps can come at the cost of flattening gradual transitions.

###### Discrete isotropic total variation

↑ **Parent:** [Total variation denoising](#total-variation-denoising)

With zero forward differences at the grid boundary, discrete isotropic total variation is the sum of the Euclidean lengths of the two-component forward gradients. Its dual constraint is the product of unit Euclidean balls, and minimizing $\tfrac12\|g-D^*p\|_2^2$ over that product yields $u_*=g-D^*p_*$. The exact difference [adjoint operator](hilbert-space.md#adjoint-operator) is essential. A dual [proximal gradient method](convex-optimization.md#proximal-gradient-method) projects $p+\tau D(g-D^*p)$ pointwise onto unit balls; $0<\tau\le1/8$ is safe on an unscaled square grid.

###### Projection residual for discrete total variation

↑ **Parent:** [Discrete isotropic total variation](#discrete-isotropic-total-variation)

For $C=D^*\{p:|p_i|_2\le\lambda\}$, discrete [total variation denoising](#total-variation-denoising) is the [proximal operator](convex-optimization.md#proximal-operator) of the [support function](mathematical-optimization.md#support-function) of $C$. The [Moreau decomposition](convex-optimization.md#moreau-decomposition) gives the displayed projection residual. It is generally not itself a [metric projection onto a closed convex set](mathematical-optimization.md#euclidean-projection-onto-a-convex-set): such a projection is idempotent, but TV denoising shrinks a sufficiently large two-level jump again when reapplied.

###### Projected-gradient dual total variation algorithm

↑ **Parent:** [Projection residual for discrete total variation](#projection-residual-for-discrete-total-variation)

Minimize $F(p)=\tfrac12\|g-D^*p\|_2^2$ over $P=\{p:|p_i|_2\le\lambda\}$ using

$$
p^{k+1}=\Pi_P\bigl(p^k+\tau D(g-D^*p^k)\bigr).
$$

The pointwise [Euclidean projection onto a convex set](mathematical-optimization.md#euclidean-projection-onto-a-convex-set) sends a block $r$ to $r/\max(1,|r|_2/\lambda)$. The [gradient](calculus.md#gradient) of $F$ has [Lipschitz constant](real-analysis.md#lipschitz-constant) $\|D\|^2$, so finite-dimensional [projected gradient descent](convex-optimization.md#projected-gradient-descent) converges for $0<\tau<2/\|D\|^2$. On an unscaled square grid with $N>1$, $0<\tau<1/4$ is safe. Reconstruct $u^k=g-D^*p^k$; unused dual directions may make the minimizing $p$ nonunique while the primal minimizer is unique.

##### Total variation of an interval indicator

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

For $a<b$ strictly inside a one-dimensional domain, the indicator $u=1_{[a,b]}$ has [distributional derivative](distribution-theory.md#distributional-derivative) $Du=\delta_a-\delta_b$, hence $\operatorname{TV}(u)=2$. Directly from the test-function definition, $\int u\varphi'=\varphi(b)-\varphi(a)\leq2$, and two disjoint normalized [smooth bump functions](partial-differential-equation.md#smooth-bump-function) attain the bound. Values at the endpoints themselves do not change the $L^1$ function.

##### Function of bounded variation on a domain

↑ **Parent:** [Total variation seminorm on a domain](#total-variation-seminorm-on-a-domain)

A function $u\in L^1(\Omega)$ has bounded variation when $\operatorname{TV}(u)<\infty$. The space $BV(\Omega)$ is a [Banach space](banach-space.md) with norm $\|u\|_{L^1}+\operatorname{TV}(u)$.

###### Completeness of the bounded-variation space

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

A [Cauchy sequence](real-analysis.md#cauchy-sequence) $(u_n)$ in the [BV space](#function-of-bounded-variation-on-a-domain) converges in $L^1$ to $u$. For fixed sufficiently large $n$, [lower semicontinuity](calculus.md#lower-semicontinuity) gives $|D(u_n-u)|(\Omega)\le\liminf_m|D(u_n-u_m)|(\Omega)$. The $L^1$ [norm](functional-analysis.md#norm) of the same difference converges, so the small full-norm Cauchy bound passes to $u_n-u$. The [triangle inequality](topological-analysis.md#triangle-inequality) then puts $u$ in the [BV space](#function-of-bounded-variation-on-a-domain) and proves convergence in its full [norm](functional-analysis.md#norm). This argument turns completeness of $L^1$ and [lower semicontinuity](calculus.md#lower-semicontinuity) of variation into completeness of the combined [norm](functional-analysis.md#norm).

###### BV slicing theorem

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a [BV space](#function-of-bounded-variation-on-a-domain) function $a$, almost every restriction $a_y$ to a line parallel to $e_j$ has bounded variation on the corresponding domain slice. Directional derivative variation disintegrates as $|D_ja|=\mathcal L^{n-1}\otimes|Da_y|$. Slice jump values agree with the appropriate oriented [BV traces on a hypersurface](#bv-trace-on-a-hypersurface) for almost every crossing of a rectifiable jump surface. Integrating slice jump sums produces a surface integral with projection factor $|\nu\cdot e_j|$. Uniform essential bounds on the slices are not asserted for an unbounded function.

###### BV jump-product limit with one bounded factor

↑ **Parent:** [BV slicing theorem](#bv-slicing-theorem)

Let $a\in BV(\Omega)$, $b\in BV(\Omega)\cap L^\infty(\Omega)$ and $\delta_tc=c\circ\Phi_t-c$, where $\Phi_t$ is the [local flow](differential-geometry.md#local-flow) of $\varphi e_j$ with nonnegative $\varphi\in C_c^\infty(\Omega)$. The formula uses common oriented [BV traces on a hypersurface](#bv-trace-on-a-hypersurface); the trace difference of $a$ is zero almost everywhere on $J_b\setminus J_a$. It also holds for both negative-time increments with denominator positive $t$.

The [BV slicing theorem](#bv-slicing-theorem) reduces the calculation to one dimension. With a right-continuous representative of $a$ and $\mu=Da$, [Fubini's theorem](measure-theory.md#fubini-s-theorem) yields

$$
\frac1t\int\delta_ta\,\delta_tb=\int\left(\frac1t\int_{\Phi_{-t}(s)}^s\delta_tb(x)\,dx\right)d\mu(s).
$$

The inner factor tends to $\varphi(s)[b](s)$ and is bounded in absolute value by $2\|b\|_\infty\|\varphi\|_\infty$. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) against $|\mu|$ leaves only its [measure atoms](measure-theory.md#atom-measure-theory) at the countable slice jumps of $b$. That same bound times $|Da_y|$ permits integration over the transverse coordinates. No essential bound on $a$ is used, even if its slice values grow without bound. The formula is useful for [opposite-flow fidelity identity for quadratic data](#opposite-flow-fidelity-identity-for-quadratic-data) with unbounded data and a bounded comparison function.

###### BV trace on a hypersurface

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

A [BV space](#function-of-bounded-variation-on-a-domain) function has two one-sided approximate mean [BV traces on a hypersurface](#bv-trace-on-a-hypersurface) at almost every point of an oriented countably rectifiable hypersurface, with respect to [Hausdorff measure](measure-theory.md#hausdorff-measure). They agree outside its [approximate discontinuity set](#approximate-discontinuity-set). At an [approximate jump point](#approximate-jump-point), they are the jump values, up to the choice of orientation.

###### Approximate gradient

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

A [BV space](#function-of-bounded-variation-on-a-domain) function is approximately differentiable at almost every point with respect to [Lebesgue measure](measure-theory.md#lebesgue-measure). Its [approximate gradient](#approximate-gradient) is the density of the absolutely continuous part of its [distributional derivative](distribution-theory.md#distributional-derivative). This does not imply membership in a [Sobolev space](sobolev-space.md).

###### Approximate discontinuity set

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a [BV space](#function-of-bounded-variation-on-a-domain) function, this is the set where no finite [approximate mean limit of a function](#approximate-mean-limit-of-a-function) exists. Its difference from the [jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function) has zero $(n-1)$-dimensional [Hausdorff measure](measure-theory.md#hausdorff-measure).

###### One-sided representatives of a one-dimensional BV function

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

Both functions represent the same $L^1$ [equivalence class](set-theory.md#equivalence-class). [Fubini's theorem](measure-theory.md#fubini-s-theorem) shows that the interval-mass function has [derivative](calculus.md#derivative) $Du$, so its difference from $u$ is constant. Continuity of a [finite measure](measure-theory.md#finite-measure) gives left continuity for $u_l$ and right continuity for $u_r$. Their opposite one-sided limits differ by the [measure atom](measure-theory.md#atom-measure-theory) $Du(\{t\})$. There are only countably many nonzero [measure atoms](measure-theory.md#atom-measure-theory), since every set of [measure atoms](measure-theory.md#atom-measure-theory) above a fixed magnitude threshold is finite.

###### Approximate mean limit of a function

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

An [approximate mean limit of a function](#approximate-mean-limit-of-a-function) is a value satisfying the displayed condition. Functions in the [BV space](#function-of-bounded-variation-on-a-domain) have such finite limits outside an [approximate discontinuity set](#approximate-discontinuity-set) up to negligible sets in the appropriate [measure](measure-theory.md#measure). Their [approximate jump points](#approximate-jump-point) instead have two distinct half-ball limits.

###### Approximate jump point

↑ **Parent:** [Approximate mean limit of a function](#approximate-mean-limit-of-a-function)

A scalar function in the [BV space](#function-of-bounded-variation-on-a-domain) has an approximate jump at a point when its mean on each of two half-balls approaches a different finite value. The half-balls are determined by a unit normal $\nu_u$. Reversing the normal exchanges the two [BV traces on a hypersurface](#bv-trace-on-a-hypersurface). Their collection is the [jump set of a BV function](#jump-set-of-a-bounded-variation-function).

###### Coarea formula for BV functions

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a scalar function in the [BV space](#function-of-bounded-variation-on-a-domain), [derivative](calculus.md#derivative) variation is the integral of the relative perimeter [measures](measure-theory.md#measure) of its [superlevel sets](topology.md#superlevel-set). The formula holds on every Borel subset $A$ of the domain, not just for total mass. It converts the continuous [ROF denoising](#total-variation-denoising) problem into linked minimization problems for [finite-perimeter sets](#set-of-finite-perimeter).

###### Structure theorem for functions of bounded variation

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

The functional $\varphi\mapsto-\int u\operatorname{div}\varphi$ is bounded in the uniform [norm](functional-analysis.md#norm) exactly when $u$ belongs to the [BV space](#function-of-bounded-variation-on-a-domain). Extend it from compactly supported smooth tests to $C_0$, then apply the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) to obtain the unique finite [vector Radon measure](measure-theory.md#vector-radon-measure) $Du$. Its dual [norm](functional-analysis.md#norm) is the defining variation supremum. This representation should be distinguished from the deeper rectifiability results used in the [decomposition of a BV derivative](#decomposition-of-a-bv-derivative).

###### Decomposition of a BV derivative

↑ **Parent:** [Structure theorem for functions of bounded variation](#structure-theorem-for-functions-of-bounded-variation)

The [Lebesgue decomposition theorem](measure-theory.md#lebesgue-decomposition-theorem) separates the absolutely continuous part from the singular part. BV fine structure then splits the latter into the [jump part of a BV derivative](#jump-part-of-a-bv-derivative) and the [Cantor part of a BV derivative](#cantor-part-of-a-bounded-variation-derivative). The density of the absolutely continuous part is the almost-everywhere [approximate gradient](#approximate-gradient). These three mutually singular components distinguish smooth variation, surface discontinuities and diffuse singular variation.

###### Jump part of a BV derivative

↑ **Parent:** [Decomposition of a BV derivative](#decomposition-of-a-bv-derivative)

This [derivative](calculus.md#derivative) component is carried by the [jump set of a BV function](#jump-set-of-a-bounded-variation-function). Swapping the two [BV traces on a hypersurface](#bv-trace-on-a-hypersurface) and reversing the normal leaves it unchanged. In one dimension it consists of the point [measure atoms](measure-theory.md#atom-measure-theory), each weighted by the difference between the right and left limits.

###### BV translation estimate

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a smooth function, integrate its directional [derivative](calculus.md#derivative) along each segment of length $|h|$ and then integrate in space. This gives the displayed bound with $\int|\nabla w|$. Smooth BV approximation and [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity) give the same inequality for general functions in the [BV space](#function-of-bounded-variation-on-a-domain). Averaging it over a [mollifier](distribution-theory.md#mollifier) proves the [BV mollification error estimate](#bv-mollification-error-estimate).

###### BV mollification error estimate

↑ **Parent:** [BV translation estimate](#bv-translation-estimate)

For a nonnegative normalized [mollifier](distribution-theory.md#mollifier) supported in the radius-$\epsilon$ ball, integrate the [BV translation estimate](#bv-translation-estimate) with weight $\rho_\epsilon(h)$. The full-space [derivative](calculus.md#derivative) variation controls the full-space error. Replacing it by variation on a smaller domain is invalid without a support condition: a nonconstant bump outside that domain has zero [derivative](calculus.md#derivative) [measure](measure-theory.md#measure) inside but a nonzero mollification error.

###### Bounded BV extension operator

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a bounded [Lipschitz domain](real-analysis.md#lipschitz-domain), functions can be extended with the displayed bound and common [compact support](function.md#compact-support). Reflect across local Lipschitz boundary graphs, combine the reflected functions with a [partition of unity](differential-geometry.md#partition-of-unity), and multiply by a fixed [cutoff function](distribution-theory.md#cutoff-function). Lipschitz coordinate changes control [derivative](calculus.md#derivative) [measures](measure-theory.md#measure); the product rule bounds [cutoff function](distribution-theory.md#cutoff-function) terms by the $L^1$ [norm](functional-analysis.md#norm). Zero extension is also possible with an estimate for [BV traces on a hypersurface](#bv-trace-on-a-hypersurface), but its boundary jump must be included in the variation.

###### Weak-star convergence in BV

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

Convergence in the displayed sense combines strong function convergence with weak-star convergence of [derivative](calculus.md#derivative) [vector measures](measure-theory.md#vector-measure) against $C_0$ tests. Strong $L^1$ convergence and a uniform variation bound imply the [derivative](calculus.md#derivative) convergence by [integration by parts](calculus.md#integration-by-parts) and uniform test-function approximation. Conversely the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) bounds the [derivative](calculus.md#derivative) [measures](measure-theory.md#measure) of a convergent sequence.

###### Strict convergence in BV

↑ **Parent:** [Weak-star convergence in BV](#weak-star-convergence-in-bv)

Strict convergence combines [strong convergence](functional-analysis.md#norm-convergence) in $L^1$ with convergence of the [total variation seminorm](#total-variation-seminorm-on-a-domain). It implies [weak-star convergence in BV](#weak-star-convergence-in-bv) but does not make jump sets stable: [mollifications](distribution-theory.md#mollification) of an interior step can converge strictly to the step while every approximant has an empty [jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function).

###### Set of finite perimeter

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

A measurable set $E$ has finite perimeter in $\Omega$ when $\chi_E$ belongs to the [BV space](#function-of-bounded-variation-on-a-domain). Its relative perimeter is $\operatorname{Per}(E;\Omega)=|D\chi_E|(\Omega)$. Relative perimeter excludes the exterior [image signal](computer-science.md#image-signal) boundary and [measures](measure-theory.md#measure) the interior interface in [Caccioppoli partitions](#caccioppoli-partition).

###### Perimeter

↑ **Parent:** [Set of finite perimeter](#set-of-finite-perimeter)

The [perimeter](#perimeter) of a measurable set relative to an open domain is the [total variation seminorm](#total-variation-seminorm-on-a-domain) of its [indicator function](measure-theory.md#indicator-function) there. For a smooth region it equals the [Hausdorff measure](measure-theory.md#hausdorff-measure) of the boundary lying inside the domain. Global [perimeter](#perimeter) uses the entire space as the domain; an internal interface shared by two regions appears in both relative perimeters and must be counted only once in a segmentation energy.

###### Perimeter quasiminimizer

↑ **Parent:** [Set of finite perimeter](#set-of-finite-perimeter)

Here the [sets of finite perimeter](#set-of-finite-perimeter) $E,F$ differ only compactly inside $U$. A minimizing set with bounded volume forcing satisfies this inequality. Interior regularity theorems give graph patches outside a singular set negligible for surface [Hausdorff measure](measure-theory.md#hausdorff-measure); bounded forcing allows the graph estimates used in the [noncontact of ROF level boundaries](#noncontact-of-rof-level-boundaries).

###### Relative perimeter

↑ **Parent:** [Set of finite perimeter](#set-of-finite-perimeter)

The [total variation seminorm](#total-variation-seminorm-on-a-domain) of the [indicator function](measure-theory.md#indicator-function) within an open set counts only its interior interface. The perimeter of a zero extension may add a boundary contribution.

###### Submodularity of relative perimeter

↑ **Parent:** [Set of finite perimeter](#set-of-finite-perimeter)

The BV lattice inequality $|D\min(v,w)|+|D\max(v,w)|\le|Dv|+|Dw|$ applied to two [indicator functions](measure-theory.md#indicator-function) gives the perimeter inequality. For smooth approximations, minima and maxima partition the two [gradients](calculus.md#gradient); [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity) passes the estimate to BV. It prevents a crossing of [minimizers](analysis.md#global-minimizer) with strictly ordered set forcing.

###### Comparison of perimeter minimizers with ordered forcing

↑ **Parent:** [Submodularity of relative perimeter](#submodularity-of-relative-perimeter)

Suppose $E_g$ minimizes $\operatorname{Per}(E)-\int_Eg$ and $E_h$ minimizes $\operatorname{Per}(E)-\int_Eh$. Compare them with their intersection and union. Adding their optimality inequalities and using [submodularity of relative perimeter](#submodularity-of-relative-perimeter) gives $\int_{E_g\setminus E_h}(h-g)\le0$. Strict ordering forces that set to be null. Applied to $g=(f-t)/\alpha$, this yields nested [ROF denoising](#total-variation-denoising) [superlevel sets](topology.md#superlevel-set).

###### Caccioppoli partition

↑ **Parent:** [Set of finite perimeter](#set-of-finite-perimeter)

A [Caccioppoli partition](#caccioppoli-partition) is a countable measurable partition, up to null sets, into [sets of finite perimeter](#set-of-finite-perimeter) with finite sum of relative perimeters. Its interior interfaces are counted twice by that sum. It represents regions of a piecewise constant [image signal](computer-science.md#image-signal) in the [piecewise-constant Mumford–Shah problem](computer-science.md#piecewise-constant-mumford-shah-problem).

###### Cantor part of a bounded-variation derivative

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

The [derivative](calculus.md#derivative) [measure](measure-theory.md#measure) of a [BV space](#function-of-bounded-variation-on-a-domain) function decomposes into its absolutely continuous, jump and Cantor parts. The [Cantor part of a bounded-variation derivative](#cantor-part-of-a-bounded-variation-derivative) is singular but not a jump [measure](measure-theory.md#measure) on a rectifiable hypersurface. The [special bounded-variation space](#special-bounded-variation-space) excludes it; finite-length [image signal](computer-science.md#image-signal) interfaces alone cannot describe it.

###### Jump set of a bounded-variation function

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

The jump set consists of points where a [BV space](#function-of-bounded-variation-on-a-domain) function has distinct one-sided approximate values across an approximate normal. In the plane its [derivative](calculus.md#derivative) contribution is $[u]\nu_u\mathcal H^1\!\lfloor J_u$. The [Mumford–Shah functional](computer-science.md#mumford-shah-functional) penalizes its length rather than the jump amplitude.

###### Special bounded-variation space

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

A [BV space](#function-of-bounded-variation-on-a-domain) function is special when its [derivative](calculus.md#derivative) has no [Cantor part of a bounded-variation derivative](#cantor-part-of-a-bounded-variation-derivative): $Du=\nabla u\,dx+[u]\nu_u\mathcal H^{n-1}\!\lfloor J_u$. The remaining singular part is supported on the [jump set of a bounded-variation function](#jump-set-of-a-bounded-variation-function). This space accommodates sharp interfaces and is the natural setting for the [Mumford–Shah functional](computer-science.md#mumford-shah-functional).

###### SBV compactness theorem

↑ **Parent:** [Special bounded-variation space](#special-bounded-variation-space)

For uniformly bounded values, an $L^p$ [gradient](calculus.md#gradient) bound with $p>1$, and bounded $(n-1)$-dimensional jump [measure](measure-theory.md#measure), a sequence in the [SBV space](#special-bounded-variation-space) admits an $L^1$-convergent subsequence whose limit remains special. [Gradients](calculus.md#gradient) converge weakly in $L^p$, and jump [measure](measure-theory.md#measure) is [lower semicontinuous](calculus.md#lower-semicontinuity). These hypotheses prevent diffuse singular [derivatives](calculus.md#derivative) from replacing the controlled interfaces in a minimizing limit.

###### Relaxed graph-area functional

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For a [BV space](#function-of-bounded-variation-on-a-domain) function with $Du=\nabla u\,dx+D^su$, relaxed graph area is $A(u)=\int\sqrt{1+|\nabla u|^2}\,dx+|D^su|(\Omega)$. Its dual [supremum](real-analysis.md#supremum) uses the coupled constraint $\varphi_0^2+|\varphi|^2\leq1$ in the pairing $\int(\varphi_0+u\operatorname{div}\varphi)$. It is convex and [lower semicontinuous](calculus.md#lower-semicontinuity) in $L^1$. Independent bounds on the two test fields define a different [functional](calculus-of-variations.md#functional).

###### Graph-area Euler-Lagrange equation

↑ **Parent:** [Relaxed graph-area functional](#relaxed-graph-area-functional)

For an assumed $W^{1,1}$ [minimizer](analysis.md#global-minimizer) of $\alpha A(u)+\tfrac12\|u-g\|_2^2$, compactly supported variations give $u-g-\alpha\operatorname{div}(\nabla u/\sqrt{1+|\nabla u|^2})=0$ in distributions. If the regularizer is instead the [total variation seminorm](#total-variation-seminorm-on-a-domain), a bounded calibration field replaces the quotient and handles zero [gradients](calculus.md#gradient).

###### Independent box constraints in a graph-area supremum

↑ **Parent:** [Relaxed graph-area functional](#relaxed-graph-area-functional)

The independent constraints $|\varphi_0|\leq1$ and $|\varphi|\leq1$ separate the dual [supremum](real-analysis.md#supremum) into $|\Omega|+|Du|(\Omega)$. They do not define square-root graph area. For $|\nabla u|=1$ the box-constrained value is $2|\Omega|$, while the [relaxed graph-area functional](#relaxed-graph-area-functional) is $\sqrt2|\Omega|$.

###### Bounded-variation compactness

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

On a bounded [Lipschitz domain](real-analysis.md#lipschitz-domain), a sequence with bounded $L^1$ [norms](functional-analysis.md#norm) and bounded [total variation seminorm](#total-variation-seminorm-on-a-domain) has a subsequence converging strongly in $L^1$. The limit is in the [BV space](#function-of-bounded-variation-on-a-domain), and its variation does not exceed the limit inferior. This supplies the [compactness](topology.md#compact-space) step of the [direct method in the calculus of variations](calculus-of-variations.md#direct-method-in-the-calculus-of-variations) for linearly growing [gradient](calculus.md#gradient) energies.

###### Homogeneous bounded-variation space

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

In the $L^2$ formulation of [total variation denoising](#total-variation-denoising) on the entire plane, one may allow finite distributional [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain) without requiring global $L^1$ membership. Its extended penalty is a supremum of [continuous](calculus.md#continuous-function) test-function pairings and hence is [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity). This domain can be larger than $BV(\mathbb R^2)\cap L^2$, since the usual [bounded-variation space](#function-of-bounded-variation-on-a-domain) includes an $L^1$ condition.

###### Failure of L2 closure of the global BV domain

↑ **Parent:** [Homogeneous bounded-variation space](#homogeneous-bounded-variation-space)

For $1<a\le2$, the radial [function](function.md) $f(x)=(1+|x|)^{-a}$ belongs to $L^2(\mathbb R^2)$ and has finite distributional [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain), but is not in $L^1(\mathbb R^2)$. Cutting it off outside radius $T$ gives [bounded-variation space](#function-of-bounded-variation-on-a-domain) [functions](function.md) tending to $f$ in $L^2$, with variation tending to that of $f$: the added jump costs $2\pi T(1+T)^{-a}\to0$. Thus the penalty equal to TV on $BV\cap L^2$ and infinity elsewhere is not [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity) in $L^2$. The closed [homogeneous bounded-variation space](#homogeneous-bounded-variation-space) extension avoids this domain issue.

###### Bounded-variation step outside W11

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

The [distributional derivative](distribution-theory.md#distributional-derivative) of this [indicator function](measure-theory.md#indicator-function) is $e_1\mathcal H^1$ on the vertical segment $x_1=1/2$, so its [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain) is one. This is singular with respect to planar [Lebesgue measure](measure-theory.md#lebesgue-measure), whereas [Sobolev space](sobolev-space.md) weak [derivatives](calculus.md#derivative) in $W^{1,1}$ have integrable densities. Its [bounded-variation space](#function-of-bounded-variation-on-a-domain) [norm](functional-analysis.md#norm) is $1/2+1=3/2$.

###### Bounded-variation contraction under clipping

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

For $T(t)=\min(b,\max(a,t))$ and $u\in BV(\Omega)$, $T\circ u\in BV(\Omega)$ and $|D(T\circ u)|(\Omega)\le|Du|(\Omega)$. This is the contraction property of a one-Lipschitz scalar composition, obtainable by smooth approximation and [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity). It proves range preservation for [total variation denoising](#total-variation-denoising) when the data lie in $[a,b]$.

###### Scalar total variation splitting under clipping

↑ **Parent:** [Bounded-variation contraction under clipping](#bounded-variation-contraction-under-clipping)

For a scalar [BV space](#function-of-bounded-variation-on-a-domain) function, clipping to $[-M,M]$ partitions its [coarea formula for BV functions](#coarea-formula-for-bv-functions) into middle and tail levels. The clipped function has the original [superlevel sets](topology.md#superlevel-set) at heights in $(-M,M)$. The positive tail levels of $u-T_Mu$ correspond to original heights above $M$, and its negative tail levels to heights below $-M$. Thus their [total variation seminorms](#total-variation-seminorm-on-a-domain) add exactly. This is stronger than the [triangle inequality](topological-analysis.md#triangle-inequality) and is specific to scalar monotone clipping. It supports [residual-preserving clipping of an ROF minimizer](#residual-preserving-clipping-of-an-rof-minimizer).

###### Noncoercivity of total variation on constants

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

On a bounded domain of positive measure, the constant functions $u_k\equiv k$ satisfy $\operatorname{TV}(u_k)=0$ while $\|u_k\|_{BV}=k|\Omega|\to\infty$. Thus the [total variation seminorm on a domain](#total-variation-seminorm-on-a-domain) is neither coercive in the $BV$ norm nor strictly convex. Additional control of the mean can remove this obstruction; the [Poincaré inequality for total variation](#poincare-inequality-for-total-variation) supplies the needed bound on suitable connected domains.

###### Zero-mean bounded-variation space

↑ **Parent:** [Function of bounded variation on a domain](#function-of-bounded-variation-on-a-domain)

The zero-mean bounded-variation space is

$$
BV_0(\Omega)=\left\{u\in BV(\Omega):\int_\Omega u\,dx=0\right\}.
$$

On a bounded connected [Lipschitz domain](real-analysis.md#lipschitz-domain), removing the constant nullspace makes total variation coercive on this subspace by the [Poincaré inequality for total variation](#poincare-inequality-for-total-variation).

<h6 id="poincare-inequality-for-total-variation">Poincaré inequality for total variation</h6>

↑ **Parent:** [Zero-mean bounded-variation space](#zero-mean-bounded-variation-space)

On a bounded connected Lipschitz domain,

$$
\|u-u_\Omega\|_{L^1(\Omega)}\leq C_\Omega\operatorname{TV}(u),
\qquad
u_\Omega=|\Omega|^{-1}\int_\Omega u.
$$

It reduces to $\|u\|_{L^1}\leq C_\Omega\operatorname{TV}(u)$ on $BV_0(\Omega)$.

#### Indicator functional of a constraint set

↑ **Parent:** [Variational regularization](#variational-regularization)

For a set $C$, its extended-real indicator functional is zero on $C$ and $+\infty$ outside $C$. It converts minimization subject to $x\in C$ into unconstrained minimization after adding the indicator to the objective.

#### Source condition in variational regularization

↑ **Parent:** [Variational regularization](#variational-regularization)

A $J$-minimizing exact solution $u^\dagger$ satisfies the source condition when some $w^\dagger\in Y^*$ obeys

$$
p^\dagger=A^*w^\dagger\in\partial J(u^\dagger).
$$

It connects a penalty subgradient to the range of the adjoint forward operator.

##### Normal-operator source condition

↑ **Parent:** [Source condition in variational regularization](#source-condition-in-variational-regularization)

This stronger [source condition in variational regularization](#source-condition-in-variational-regularization) requires a [subgradient](real-analysis.md#subgradient) $w=K^*Kv$ at $u^\dagger$. For each $\alpha>0$ it is equivalent to making $u^\dagger$ minimize $\|Ku-K\bar u\|^2/2+\alpha J(u)$ for artificial input $\bar u=u^\dagger+\alpha v$. The [subgradient optimality condition](real-analysis.md#subgradient-optimality-condition) proves both implications. The source vector may be zero: $K=I$ and $J\equiv0$ satisfy the condition but admit no nonzero source vector.

###### Shifted-comparator Bregman bound

↑ **Parent:** [Normal-operator source condition](#normal-operator-source-condition)

Let $u^\dagger$ be a [least-squares solution](#least-squares-solution-of-a-linear-inverse-problem) and $w=K^*Kv\in\partial J(u^\dagger)$. For a minimizer $u_\alpha$ of $\|Ku-f\|^2/2+\alpha J(u)$, expand the objective about $u^\dagger$. The [normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem) removes the data-residual cross term, while the [Bregman distance](#bregman-divergence) definition gives

$$
\mathcal F_\alpha(u)-\mathcal F_\alpha(u^\dagger)=\frac12\|K(u-u^\dagger+\alpha v)\|^2+\alpha D_J^w(u,u^\dagger)-\frac{\alpha^2}2\|Kv\|^2.
$$

Compare the minimizer with $u^\dagger-\alpha v$, where the square vanishes, and divide by $\alpha$. The bound is informative when that comparator has finite penalty.

##### Source-condition certification of a penalty-minimizing solution

↑ **Parent:** [Source condition in variational regularization](#source-condition-in-variational-regularization)

If $Au=f$ and $A^*\mu\in\partial J(u)$, then $u$ is a [J-minimizing solution](#j-minimizing-solution). For every other exact solution $v$, the [subgradient inequality](real-analysis.md#subgradient-inequality) gives $J(v)\geq J(u)+\langle\mu,Av-Au\rangle=J(u)$. This is a certificate of global optimality supplied by the range of the [adjoint operator](hilbert-space.md#adjoint-operator).

##### Range condition in variational regularization

↑ **Parent:** [Source condition in variational regularization](#source-condition-in-variational-regularization)

The range condition asks whether a prescribed exact solution is also a minimizer of a penalized problem with suitably chosen artificial data. The [subgradient optimality condition](real-analysis.md#subgradient-optimality-condition) makes it equivalent to a source subgradient lying in the range of the adjoint forward operator.

#### Bregman divergence

↑ **Parent:** [Variational regularization](#variational-regularization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bregman_divergence)

For a [convex functional](real-analysis.md#convex-function) $J$ and $p\in\partial J(v)$, the Bregman divergence is

$$
D_J^p(u,v)=J(u)-J(v)-\langle p,u-v\rangle.
$$

It is nonnegative but need not be symmetric or satisfy the triangle inequality.

##### Bregman iteration

↑ **Parent:** [Bregman divergence](#bregman-divergence)

Starting with $u^0=0$ and $p^0=0\in\partial J(0)$, update $p^{k+1}=p^k+K^*(f-Ku^{k+1})/\alpha$. The optimality condition makes $p^{k+1}\in\partial J(u^{k+1})$. The iteration replaces a fixed penalty by its [Bregman distance](#bregman-divergence) from the preceding iterate and accumulates residual information in the dual variable. The first update uses $k=0$.

###### Finite termination of Bregman iteration on a singular vector

↑ **Parent:** [Bregman iteration](#bregman-iteration)

For a [generalized singular vector](convex-optimization.md#generalized-singular-vector), exact data $f=\gamma Ku_\lambda$, and fixed $\alpha>0$, a compatible branch of [Bregman iteration](#bregman-iteration) has $p^k=\min\{k\gamma/\alpha,\lambda\}K^*Ku_\lambda$ and the displayed $u^k$. Verify these formulas with the [subgradient](real-analysis.md#subgradient) characterization of an [absolutely one-homogeneous functional](convex-optimization.md#absolutely-one-homogeneous-functional); before activation the dual coefficient remains at most $\lambda$, and after activation it is $\lambda$. The branch reaches $\gamma u_\lambda$ at $k_*=\lceil\alpha\lambda/\gamma\rceil+1$. Every minimizer branch has the same predicted data, since the quadratic data fidelity is [strictly convex](real-analysis.md#strictly-convex-function) in $Ku$. Exact recovery of this particular vector for arbitrary branch choices needs uniqueness, for example injectivity of $K$. For $K(x,y)=x$ and $J(x,y)=|x|$, the second coordinate of every minimizer is arbitrary.

##### Symmetric Bregman distance

↑ **Parent:** [Bregman divergence](#bregman-divergence)

For $p_u\in\partial J(u)$ and $p_v\in\partial J(v)$, add the two [Bregman distances](#bregman-divergence) to get $D_J^{p_v}(u,v)+D_J^{p_u}(v,u)=\langle p_u-p_v,u-v\rangle\geq0$. The choice of [subgradients](real-analysis.md#subgradient) matters. This is generally not a metric: it need not separate points or satisfy a [triangle inequality](topological-analysis.md#triangle-inequality).

###### Source-condition estimate for symmetric Bregman distance

↑ **Parent:** [Symmetric Bregman distance](#symmetric-bregman-distance)

Let $K:U\to V$ be a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) from a real [Banach space](banach-space.md) to a real [Hilbert space](hilbert-space.md), let $J$ be a proper lower-semicontinuous [convex function](real-analysis.md#convex-function), and let $\alpha>0$ and $\|f^\delta-Ku^\dagger\|\leq\delta$. For an existing minimizer of $\|Ku-f^\delta\|^2/2+\alpha J(u)$ and a [source condition in variational regularization](#source-condition-in-variational-regularization) $p^\dagger=K^*w\in\partial J(u^\dagger)$, let $e=f^\delta-Ku^\dagger$ and $q=K(u_\alpha-u^\dagger)$. Its optimality [subgradient](real-analysis.md#subgradient) is $p_\alpha=K^*(f^\delta-Ku_\alpha)/\alpha$. Then $\alpha D_J^{\mathrm{sym}}=\langle e-\alpha w,q\rangle-\|q\|^2\leq\|e-\alpha w\|^2/4$. The displayed estimate follows from $\|e-\alpha w\|^2\leq2\delta^2+2\alpha^2\|w\|^2$.

##### Zero Bregman distance and supporting faces

↑ **Parent:** [Bregman divergence](#bregman-divergence)

For $p\in\partial J(v)$, zero [Bregman distance](#bregman-divergence) means that $J(u)$ equals the supporting affine function $J(v)+\langle p,u-v\rangle$. If $J$ is [strictly convex](real-analysis.md#strictly-convex-function), two distinct contact points are impossible: convexity along their segment would be strict, while the [subgradient inequality](real-analysis.md#subgradient-inequality) supplies the opposite bound. Thus zero distance then implies $u=v$. Without strict convexity, $J(s)=|s|$, $v=1$, $p=1$ gives zero distance for every $u\geq0$. These are all on the same supporting face.

#### Exact penalty method

↑ **Parent:** [Variational regularization](#variational-regularization)

An exact penalty method uses a nonsquared residual such as $\lVert Au-f\rVert+\alpha J(u)$. Under a source condition it can recover an exact constrained minimizer for every sufficiently small fixed positive $\alpha$.

##### Exact-penalty threshold from a source condition

↑ **Parent:** [Exact penalty method](#exact-penalty-method)

Suppose $Au^\dagger=f$ and $p^\dagger=A^*\mu^\dagger\in\partial J(u^\dagger)$. For $F_\alpha(u)=\|Au-f\|+\alpha J(u)$, the [subgradient inequality](real-analysis.md#subgradient-inequality) and [dual pairing](continuous-dual-space.md#dual-pairing) bound give

$$
F_\alpha(u)-F_\alpha(u^\dagger)
\geq(1-\alpha\|\mu^\dagger\|)\|Au-f\|.
$$

Thus $0<\alpha\|\mu^\dagger\|<1$ forces every minimizer to solve $Au=f$ exactly. Comparison of penalties then shows it is a [J-minimizing solution](#j-minimizing-solution), and $D_J^{p^\dagger}(u,u^\dagger)=0$. The conclusion also holds for all $\alpha>0$ when $\mu^\dagger=0$. One-homogeneity is not needed for this argument.

## Normal equation for a linear inverse problem

↑ **Parent:** [Inverse problem](inverse-problem.md)

The normal equation for $Au=f$ is $A^*Au=A^*f$. Its solutions minimize $\lVert Au-f\rVert$; when they exist, the unique solution orthogonal to $\ker A$ is the Moore--Penrose solution $A^\dagger f$.

### Least-squares solution of a linear inverse problem

↑ **Parent:** [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)

A [least-squares solution](#least-squares-solution-of-a-linear-inverse-problem) minimizes $\|Ku-f\|$ over the source [Hilbert space](hilbert-space.md). It exists exactly when $f\in\mathcal R(K)\oplus\mathcal R(K)^\perp$, and then the solutions form a closed [affine subspace](vector-space.md#affine-subspace) with direction $\mathcal N(K)$.

#### Least-squares existence criterion

↑ **Parent:** [Least-squares solution of a linear inverse problem](#least-squares-solution-of-a-linear-inverse-problem)

For a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $K:U\to V$ between [Hilbert spaces](hilbert-space.md), a [least-squares solution](#least-squares-solution-of-a-linear-inverse-problem) for $f$ exists exactly when $P_{\overline{\mathcal R(K)}}f\in\mathcal R(K)$, equivalently $f\in\mathcal R(K)\oplus\mathcal R(K)^\perp$. Indeed the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the closure uniquely minimizes distance to that closed space, and it can be realized by $Ku$ exactly under this condition. Thus all data admit [least-squares solutions](#least-squares-solution-of-a-linear-inverse-problem) exactly when the range is closed.

#### Nearest least-squares solution

↑ **Parent:** [Least-squares solution of a linear inverse problem](#least-squares-solution-of-a-linear-inverse-problem)

The [orthogonal projection](hilbert-space.md#orthogonal-projection) of a prescribed point $u_0$ onto the [affine subspace](vector-space.md#affine-subspace) of [least-squares solutions](#least-squares-solution-of-a-linear-inverse-problem) is unique. It retains $u_0$'s [null space](linear-algebra.md#kernel-of-a-linear-map) component and chooses the determined component from the [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator).

### Singular system of a compact operator

↑ **Parent:** [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)

A singular system $(\sigma_j,u_j,v_j)$ for a compact operator $A:X\to Y$ has positive singular values $\sigma_j\to0$ and orthonormal vectors satisfying $Av_j=\sigma_j u_j$ and $A^*u_j=\sigma_jv_j$. It diagonalizes spectral regularization methods.

#### Singular system of a periodic convolution operator

↑ **Parent:** [Singular system of a compact operator](#singular-system-of-a-compact-operator)

The displayed [singular value system](#singular-system-of-a-compact-operator) applies when the Fourier multipliers $c_n$ are nonzero. The phase in the left singular vector is necessary for complex kernels. If a multiplier vanishes, its mode instead belongs to the corresponding null spaces and is excluded from the positive singular system.

### Picard criterion

↑ **Parent:** [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)

For a compact operator with singular system $(\sigma_j,u_j,v_j)$, the datum $f$ lies in the domain of $A^\dagger$ exactly when its component in $\overline{\operatorname{ran}A}$ satisfies

$$
\sum_j\frac{|\langle f,u_j\rangle|^2}{\sigma_j^2}<\infty.
$$

### Landweber iteration

↑ **Parent:** [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Landweber_iteration)

Landweber iteration applies $u_{n+1}=u_n+\tau A^*(f-Au_n)$. Starting at zero,

$$
u_N=\tau\sum_{n=0}^{N-1}(I-\tau A^*A)^nA^*f,
$$

and early stopping regularizes the inverse problem.

#### Strong convergence of relaxed Landweber iteration

↑ **Parent:** [Landweber iteration](#landweber-iteration)

For nonzero [compact operator](compact-operator.md) $A$, step $0<\tau<2/\|A\|^2$, and data admitting a [minimum-norm least-squares solution](#minimum-norm-least-squares-solution) $x^\dagger$, zero-initialized [Landweber iteration](#landweber-iteration) satisfies

$$
 \|x_n-x^\dagger\|^2=\sum_i|1-\tau\sigma_i^2|^{2n}\frac{|\langle y,u_i\rangle|^2}{\sigma_i^2}\longrightarrow0.
$$

The [Picard criterion](#picard-criterion) makes the majorant summable, so the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) proves this limit. No mesh-independent or singular-value-independent strict contraction factor is required. At $\tau=2/\|A\|^2$, the top singular mode has multiplier $-1$ and may not converge. Without solvable projected data, the iterates need not have a limit in the solution [Hilbert space](hilbert-space.md), even when their residuals approach the least-squares infimum.

#### Landweber iteration with a Tikhonov initial value

↑ **Parent:** [Landweber iteration](#landweber-iteration)

Initialize [Landweber iteration](#landweber-iteration) by [Tikhonov regularization](#tikhonov-regularization), then use step $1/\alpha$. Writing $B=A^*A$ and $R=I-B/\alpha$, the iterate is $x_n=R^n(B+\alpha I)^{-1}A^*y+\alpha^{-1}\sum_{j=0}^{n-1}R^jA^*y$. For nonzero $A$, the sufficient convergence condition is $\alpha>\|A\|^2/2$. This explicit method differs from [Iterated Tikhonov regularization](#iterated-tikhonov-regularization), whose update is $(B+\alpha I)x_{n+1}=\alpha x_n+A^*y$.

##### Closed form of a Tikhonov-initialized Landweber iterate

↑ **Parent:** [Landweber iteration with a Tikhonov initial value](#landweber-iteration-with-a-tikhonov-initial-value)

In a [singular system of a compact operator](#singular-system-of-a-compact-operator), [Landweber iteration with a Tikhonov initial value](#landweber-iteration-with-a-tikhonov-initial-value) has coefficients $g_{\alpha,n}(\sigma_i)(y,u_i)$. Summing the finite geometric series gives the displayed filter. For fixed $n$, $g_{\alpha,n}(\sigma)=(n+1)\sigma/\alpha+O(\sigma^3)$ at zero, so each finite iterate is bounded. Under $\alpha>\|A\|^2/2$ the filter approaches $1/\sigma$ on every positive singular mode; noisy data require [early stopping of Landweber iteration](#early-stopping-of-landweber-iteration).

#### Landweber relaxation parameter

↑ **Parent:** [Landweber iteration](#landweber-iteration)

The relaxation parameter $\tau$ controls the step in [Landweber iteration](#landweber-iteration). Convergence from zero to the [minimum-norm least-squares solution](#minimum-norm-least-squares-solution) requires $0<\tau<2/\|A\|^2$. Thus $\|A\|<2$ allows $\tau=1/2$, while unit steps require $\|A\|<\sqrt2$.

#### Landweber spectral filter

↑ **Parent:** [Landweber iteration](#landweber-iteration)

Starting [Landweber iteration](#landweber-iteration) at zero gives

$$
x_n=\sum_j\frac{1-(1-\tau\sigma_j^2)^n}{\sigma_j}\langle y,u_j\rangle v_j
$$

in a [singular system of a compact operator](#singular-system-of-a-compact-operator). The dimensionless damping filter is $f_n(\sigma)=1-(1-\tau\sigma^2)^n$. If the full inverse coefficient is called the filter instead, it is $f_n(\sigma)/\sigma$; these conventions describe the same operator.

##### Landweber full inverse filter

↑ **Parent:** [Landweber spectral filter](#landweber-spectral-filter)

Starting [Landweber iteration](#landweber-iteration) at zero with fixed step $\tau$, the full data-to-solution coefficient on a [singular value](linear-algebra.md#singular-value) $\sigma>0$ is

$$
 g_n(\sigma)=\frac{1-(1-\tau\sigma^2)^n}{\sigma}.
$$

This follows by summing the scalar [geometric series](real-analysis.md#geometric-series) in a [singular system of a compact operator](#singular-system-of-a-compact-operator). For fixed $n$, $g_n(\sigma)=n\tau\sigma+O(\sigma^3)$ near zero and extends with $g_n(0)=0$. Its dimensionless damping factor is $\sigma g_n(\sigma)$, so the two common filter conventions must not be confused. Writing $\alpha=1/n$ uses a discrete parameter sequence; if negative multipliers occur, noninteger real powers are not a definition of the same iteration.

##### Landweber noise amplification bound

↑ **Parent:** [Landweber spectral filter](#landweber-spectral-filter)

For $\tau=1$ and $\|A\|\leq1$, $0\leq1-(1-\sigma^2)^n\leq\min(n\sigma^2,1)$ gives

$$
\|R_n\|\leq\sup_{0<\sigma\leq1}\min(n\sigma,\sigma^{-1})\leq\sqrt n.
$$

Thus a data error of norm at most $\delta$ produces an iterate error at most $\sqrt n\,\delta$.

###### Uniform noise bound for relaxed Landweber iteration

↑ **Parent:** [Landweber noise amplification bound](#landweber-noise-amplification-bound)

For $0<\tau<2/\|A\|^2$, the [Landweber full inverse filter](#landweber-full-inverse-filter) obeys

$$
 |g_n(\sigma)|\leq\min(n\tau\sigma,2/\sigma)\leq\sqrt{2n\tau}.
$$

Indeed, with $t=\tau\sigma^2\in[0,2]$, the telescoping [geometric series](real-analysis.md#geometric-series) and $|1-t|\leq1$ give $|1-(1-t)^n|\leq\min(nt,2)$. Thus noise of [norm](functional-analysis.md#norm) at most $\delta$ produces iterate error at most $\delta\sqrt{2n\tau}$. If $\tau\|A\|^2\leq1$, replace 2 by 1 to obtain $\delta\sqrt{n\tau}$. Together with exact-data strong convergence, a stopping choice $n\to\infty$ and $\delta\sqrt n\to0$ proves [convergent regularization of an inverse problem](#convergent-regularization-of-an-inverse-problem).

#### Early stopping of Landweber iteration

↑ **Parent:** [Landweber iteration](#landweber-iteration)

The [Landweber spectral filter](#landweber-spectral-filter) progressively admits smaller singular-value components. Its approximation bias tends to zero on exact admissible data, but its noise amplification grows. With $\|A\|\leq1$, a sufficient [a priori regularization parameter choice](#a-priori-regularization-parameter-choice) is $n(\delta)\to\infty$ and $\sqrt{n(\delta)}\,\delta\to0$. Taking regularization parameter $\alpha=1/n$ expresses this as $\alpha\to0$ and $\delta/\sqrt\alpha\to0$; the [noise-bias decomposition for linear regularization](#noise-bias-decomposition-for-linear-regularization) proves convergence.

<h3 id="moore-penrose-inverse-of-an-operator">Moore–Penrose inverse of an operator</h3>

↑ **Parent:** [Normal equation for a linear inverse problem](#normal-equation-for-a-linear-inverse-problem)

For a bounded operator $A:X\to Y$ between Hilbert spaces, the Moore–Penrose inverse maps admissible data to the unique minimum-norm least-squares solution. If $(\sigma_j,u_j,v_j)$ is a [singular system of a compact operator](#singular-system-of-a-compact-operator), then

$$
A^\dagger y
=\sum_j\frac{\langle y,u_j\rangle}{\sigma_j}v_j
$$

on the data for which this series converges.

More precisely, its domain is $\operatorname{ran}A\oplus(\operatorname{ran}A)^\perp$. It vanishes on $(\operatorname{ran}A)^\perp$ and takes values in $(\ker A)^\perp$. An infinite-rank [compact operator](compact-operator.md) on infinite-dimensional spaces has singular values approaching zero, so its inverse on its range is generally unbounded; [Picard criterion](#picard-criterion) specifies admissible data.

#### Minimum-norm least-squares solution

↑ **Parent:** [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator)

A minimum-norm least-squares solution minimizes $\lVert Ax-y\rVert$ and, among all such minimizers, minimizes $\lVert x\rVert$. It lies in $(\ker A)^\perp$ and equals $A^\dagger y$ when the [Moore–Penrose inverse of an operator](#moore-penrose-inverse-of-an-operator) is defined at $y$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Forward problem](#forward-problem)
- [Ill-posed inverse problem](#ill-posed-inverse-problem)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#1/1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326.md#1/1/solution)
- [Regularization parameter](#regularization-parameter)
