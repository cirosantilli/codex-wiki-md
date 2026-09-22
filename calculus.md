# Calculus

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Calculus)

Calculus studies local change through derivatives and accumulated change through integrals.

**Table of contents**

- [Floor and ceiling functions](#floor-and-ceiling-functions)
  - [Floor function](#floor-function)
    - [Fractional part](#fractional-part)
  - [Ceiling function](#ceiling-function)
- [Integral](#integral)
  - [Wallis integrals](#wallis-integrals)
  - [Dipole line-integral identity](#dipole-line-integral-identity)
  - [Integrand](#integrand)
  - [Multiple integral](#multiple-integral)
    - [Odd-integrand cancellation by reflection](#odd-integrand-cancellation-by-reflection)
  - [Integral representation](#integral-representation)
    - [Trigonometric integral](#trigonometric-integral)
      - [Cosine integral](#cosine-integral)
      - [Sine integral](#sine-integral)
  - [Lebesgue integration](#lebesgue-integration)
    - [Prékopa–Leindler inequality](#prekopa-leindler-inequality)
    - [Absolute continuity of the Lebesgue integral](#absolute-continuity-of-the-lebesgue-integral)
  - [Time integral](#time-integral)
  - [Double integral](#double-integral)
  - [Monotonicity of the Lebesgue integral](#monotonicity-of-the-lebesgue-integral)
  - [Antiderivative](#antiderivative)
    - [Constant of integration](#constant-of-integration)
    - [Additive constant](#additive-constant)
  - [Gaussian integral](#gaussian-integral)
    - [Linear-source multivariate Gaussian integral](#linear-source-multivariate-gaussian-integral)
    - [Dawson function](#dawson-function)
      - [Gaussian drift primitives](#gaussian-drift-primitives)
    - [Error function](#error-function)
      - [Quadrant asymptotics of the error function](#quadrant-asymptotics-of-the-error-function)
      - [Complementary error function](#complementary-error-function)
        - [Faddeeva function](#faddeeva-function)
          - [Gaussian pole integral](#gaussian-pole-integral)
- [Taylor polynomial](#taylor-polynomial)
  - [Multivariate Taylor polynomial](#multivariate-taylor-polynomial)
- [Exponential function](#exponential-function)
  - [e (mathematical constant)](#e-mathematical-constant)
    - [Irrationality of e](#irrationality-of-e)
  - [Exponential series](#exponential-series)
  - [Complex exponential function](#complex-exponential-function)
    - [Modulus of the complex exponential](#modulus-of-the-complex-exponential)
    - [Complex sine function](#complex-sine-function)
      - [Periodicity of the complex sine](#periodicity-of-the-complex-sine)
  - [Logarithm](#logarithm)
    - [Geometric-series bound for the logarithmic remainder](#geometric-series-bound-for-the-logarithmic-remainder)
    - [Irrational logarithm criterion](#irrational-logarithm-criterion)
    - [Concavity of the logarithm](#concavity-of-the-logarithm)
    - [Logarithmic integral function](#logarithmic-integral-function)
    - [Natural logarithm](#natural-logarithm)
    - [Logarithm inequality](#logarithm-inequality)
    - [Operator monotonicity of logarithm](#operator-monotonicity-of-logarithm)
  - [Gaussian function](#gaussian-function)
    - [Gaussian decay dominates every power](#gaussian-decay-dominates-every-power)
    - [Gaussian dyadic summation bound](#gaussian-dyadic-summation-bound)
  - [Hyperbolic function](#hyperbolic-function)
    - [Inverse hyperbolic functions](#inverse-hyperbolic-functions)
    - [Hyperbolic cosine](#hyperbolic-cosine)
      - [Factorial-tail irrationality proof for a hyperbolic cosine](#factorial-tail-irrationality-proof-for-a-hyperbolic-cosine)
      - [Inverse hyperbolic cosine](#inverse-hyperbolic-cosine)
    - [Hyperbolic sine](#hyperbolic-sine)
    - [Hyperbolic cotangent](#hyperbolic-cotangent)
      - [Partial-fraction expansion of the hyperbolic cotangent](#partial-fraction-expansion-of-the-hyperbolic-cotangent)
    - [Hyperbolic secant](#hyperbolic-secant)
- [Fundamental theorem of calculus](#fundamental-theorem-of-calculus)
  - [Fundamental theorem of calculus for Lebesgue integration](#fundamental-theorem-of-calculus-for-lebesgue-integration)
- [Mean value theorem](#mean-value-theorem)
  - [Cauchy mean value theorem](#cauchy-mean-value-theorem)
  - [Endpoint secant-tangent approximation](#endpoint-secant-tangent-approximation)
- [Rolle theorem](#rolle-theorem)
  - [Rolle root count with multiplicities](#rolle-root-count-with-multiplicities)
- [Taylor theorem](#taylor-theorem)
  - [Taylor expansion from a periodic derivative equation](#taylor-expansion-from-a-periodic-derivative-equation)
  - [Integral first-order Taylor formula for a vector map](#integral-first-order-taylor-formula-for-a-vector-map)
  - [Integral remainder in Taylor theorem](#integral-remainder-in-taylor-theorem)
    - [Logarithmic series from an integral Taylor remainder](#logarithmic-series-from-an-integral-taylor-remainder)
  - [Taylor expansion](#taylor-expansion)
    - [Peano zero](#peano-zero)
    - [Parabolic approximation](#parabolic-approximation)
  - [Taylor formula for a polynomial](#taylor-formula-for-a-polynomial)
  - [Taylor theorem with Lagrange remainder](#taylor-theorem-with-lagrange-remainder)
  - [Taylor remainder](#taylor-remainder)
  - [Taylor formula with integral remainder](#taylor-formula-with-integral-remainder)
  - [Taylor series](#taylor-series)
- [Limit of a function](#limit-of-a-function)
  - [One-sided limit](#one-sided-limit)
  - [Continuous function](#continuous-function)
    - [Blancmange curve](#blancmange-curve)
    - [Bounded continuous functions](#bounded-continuous-functions)
    - [Upper semicontinuity](#upper-semicontinuity)
    - [Oscillation multiplied by a vanishing amplitude](#oscillation-multiplied-by-a-vanishing-amplitude)
    - [Lower semicontinuity](#lower-semicontinuity)
    - [Discontinuity of a function](#discontinuity-of-a-function)
      - [Removable discontinuity](#removable-discontinuity)
      - [Jump discontinuity](#jump-discontinuity)
    - [Sequential lower semicontinuity](#sequential-lower-semicontinuity)
      - [Sublevel set](#sublevel-set)
        - [Compact sublevel set](#compact-sublevel-set)
      - [Closed-sublevel-set characterization of lower semicontinuity](#closed-sublevel-set-characterization-of-lower-semicontinuity)
    - [Locally constant function](#locally-constant-function)
      - [Compactly supported locally constant function](#compactly-supported-locally-constant-function)
    - [Intermediate value theorem](#intermediate-value-theorem)
      - [Continuous image of a real interval](#continuous-image-of-a-real-interval)
      - [Interval order theorem for continuous injections](#interval-order-theorem-for-continuous-injections)
      - [Horizontal chord of reciprocal-integer length](#horizontal-chord-of-reciprocal-integer-length)
      - [Zero on a line segment](#zero-on-a-line-segment)
      - [Telescoping increment lemma](#telescoping-increment-lemma)
      - [Continuous bijection of the real line is monotone](#continuous-bijection-of-the-real-line-is-monotone)
    - [Composition of continuous functions](#composition-of-continuous-functions)
    - [Continuity set of a function](#continuity-set-of-a-function)
    - [Right-continuous function](#right-continuous-function)
      - [Càdlàg](#cadlag)
    - [Uniformly continuous function](#uniformly-continuous-function)
      - [Decay of a nonnegative uniformly continuous integrable function](#decay-of-a-nonnegative-uniformly-continuous-integrable-function)
  - [Squeeze theorem](#squeeze-theorem)
- [Derivative](#derivative)
  - [Symmetric second derivative](#symmetric-second-derivative)
  - [Symmetric second differences detect an affine corner](#symmetric-second-differences-detect-an-affine-corner)
  - [Symmetric first-order differences remove an affine corner](#symmetric-first-order-differences-remove-an-affine-corner)
  - [Vanishing symmetric second derivative forces an affine function](#vanishing-symmetric-second-derivative-forces-an-affine-function)
  - [One-sided derivative](#one-sided-derivative)
  - [Tangent line](#tangent-line)
  - [Automatic differentiation](#automatic-differentiation)
  - [Differentiation](#differentiation)
  - [Second derivative](#second-derivative)
  - [Difference quotient](#difference-quotient)
    - [Discrete integration by parts](#discrete-integration-by-parts)
  - [Total derivative](#total-derivative)
  - [L'Hôpital's rule](#l-hopital-s-rule)
    - [Derivative quotient limits on partial domains](#derivative-quotient-limits-on-partial-domains)
  - [Darboux's theorem (analysis)](#darboux-s-theorem-analysis)
    - [Intermediate secant slope from endpoint derivatives](#intermediate-secant-slope-from-endpoint-derivatives)
  - [Product rule](#product-rule)
    - [Differentiability restored by a quadratic zero](#differentiability-restored-by-a-quadratic-zero)
    - [Leibniz rule](#leibniz-rule)
    - [Nondifferentiable factor with a differentiable nondegenerate product](#nondifferentiable-factor-with-a-differentiable-nondegenerate-product)
  - [Quotient rule](#quotient-rule)
  - [Chain rule](#chain-rule)
    - [Nondifferentiable inner function with a differentiable nondegenerate composite](#nondifferentiable-inner-function-with-a-differentiable-nondegenerate-composite)
    - [Second derivative chain rule](#second-derivative-chain-rule)
- [Monotonic function](#monotonic-function)
  - [Monotone mean-value point of an integral average](#monotone-mean-value-point-of-an-integral-average)
  - [Nonincreasing function](#nonincreasing-function)
  - [Non-strict inverse of a continuous nondecreasing function](#non-strict-inverse-of-a-continuous-nondecreasing-function)
  - [Left-continuous cumulative function of an atomic measure](#left-continuous-cumulative-function-of-an-atomic-measure)
  - [Nondecreasing function](#nondecreasing-function)
  - [Strict generalized inverse of a nondecreasing function](#strict-generalized-inverse-of-a-nondecreasing-function)
  - [Strictly increasing function](#strictly-increasing-function)
    - [Continuity of an increasing interval surjection](#continuity-of-an-increasing-interval-surjection)
  - [Lebesgue theorem on differentiability of monotone functions](#lebesgue-theorem-on-differentiability-of-monotone-functions)
- [Multivariable calculus](#multivariable-calculus)
  - [Volume integral](#volume-integral)
  - [Fundamental theorem of calculus along a line segment](#fundamental-theorem-of-calculus-along-a-line-segment)
  - [Partial derivative](#partial-derivative)
    - [Partial derivatives do not imply continuity](#partial-derivatives-do-not-imply-continuity)
    - [Mixed partial derivative](#mixed-partial-derivative)
      - [Unequal mixed partial derivatives](#unequal-mixed-partial-derivatives)
      - [Symmetry of second derivatives](#symmetry-of-second-derivatives)
    - [Time derivative](#time-derivative)
    - [Spatial derivative](#spatial-derivative)
    - [Directional derivative](#directional-derivative)
      - [Directional derivatives do not imply differentiability](#directional-derivatives-do-not-imply-differentiability)
      - [Directional derivative of a convex function is sublinear](#directional-derivative-of-a-convex-function-is-sublinear)
    - [Gradient](#gradient)
      - [Gradient of a dot product](#gradient-of-a-dot-product)
      - [Gradient field](#gradient-field)
    - [Total differential](#total-differential)
  - [Hessian matrix](#hessian-matrix)
    - [Quadratic growth from a bounded Hessian](#quadratic-growth-from-a-bounded-hessian)
    - [Higher-order test for separated extrema](#higher-order-test-for-separated-extrema)
    - [Negative semidefinite matrix](#negative-semidefinite-matrix)
    - [Second-derivative test](#second-derivative-test)
      - [Critical points escaping to infinity in a Gaussian-weighted bilinear function](#critical-points-escaping-to-infinity-in-a-gaussian-weighted-bilinear-function)
    - [Nondegenerate critical point](#nondegenerate-critical-point)
  - [Vector calculus](#vector-calculus)
    - [Dot-product gradient identity](#dot-product-gradient-identity)
    - [Helmholtz decomposition](#helmholtz-decomposition)
    - [Divergence of a cross product](#divergence-of-a-cross-product)
    - [Vector field](#vector-field)
      - [Flow of a vector field](#flow-of-a-vector-field)
      - [Time-dependent vector field](#time-dependent-vector-field)
        - [Finite-time flow completeness on a compact manifold](#finite-time-flow-completeness-on-a-compact-manifold)
      - [Radial dilation tangency to homogeneous zero sets](#radial-dilation-tangency-to-homogeneous-zero-sets)
      - [Divergence and curl of a radial vector field](#divergence-and-curl-of-a-radial-vector-field)
      - [Azimuthal inverse-radius vector field](#azimuthal-inverse-radius-vector-field)
      - [Integral curve of a vector field](#integral-curve-of-a-vector-field)
        - [Curvature of an integral curve of a vector field](#curvature-of-an-integral-curve-of-a-vector-field)
      - [Axisymmetric vector field](#axisymmetric-vector-field)
      - [Solenoidal vector field](#solenoidal-vector-field)
        - [Poloidal-toroidal decomposition](#poloidal-toroidal-decomposition)
          - [Poloidal magnetic energy bound by the radial scalar gradient](#poloidal-magnetic-energy-bound-by-the-radial-scalar-gradient)
    - [Spherically symmetric function](#spherically-symmetric-function)
    - [Helicity conservation by tangent boundary conditions](#helicity-conservation-by-tangent-boundary-conditions)
    - [Divergence](#divergence)
      - [Divergence of a Riemannian vector field](#divergence-of-a-riemannian-vector-field)
      - [Cylindrically radial divergence](#cylindrically-radial-divergence)
      - [Distributional divergence](#distributional-divergence)
      - [Divergence in polar coordinates](#divergence-in-polar-coordinates)
      - [Product rule for divergence](#product-rule-for-divergence)
      - [Total divergence](#total-divergence)
      - [Divergence of a curl is zero](#divergence-of-a-curl-is-zero)
    - [Curl](#curl)
      - [Curl of a gradient](#curl-of-a-gradient)
      - [Irrotational vector field](#irrotational-vector-field)
      - [Vector potential](#vector-potential)
        - [Radial vector potential of a solenoidal vector field](#radial-vector-potential-of-a-solenoidal-vector-field)
      - [Curl of the curl identity](#curl-of-the-curl-identity)
    - [Laplacian](#laplacian)
      - [Laplacian in polar coordinates](#laplacian-in-polar-coordinates)
      - [Product rule for the Laplacian](#product-rule-for-the-laplacian)
      - [Biharmonic operator](#biharmonic-operator)
        - [Clamped biharmonic problem](#clamped-biharmonic-problem)
        - [Biharmonic equation](#biharmonic-equation)
          - [Spherical mean of a biharmonic function](#spherical-mean-of-a-biharmonic-function)
    - [Divergence and curl of a cross product](#divergence-and-curl-of-a-cross-product)
      - [Curl of a cross product](#curl-of-a-cross-product)
    - [Levi-Civita symbol](#levi-civita-symbol)
      - [Rotation invariance of the Levi-Civita symbol](#rotation-invariance-of-the-levi-civita-symbol)
      - [Contraction of two Levi-Civita symbols](#contraction-of-two-levi-civita-symbols)
      - [Lagrange identity for the cross product](#lagrange-identity-for-the-cross-product)
      - [Triple product](#triple-product)
        - [Vector triple product](#vector-triple-product)
    - [Feasible inner products with two unit vectors](#feasible-inner-products-with-two-unit-vectors)
    - [Conservative vector field](#conservative-vector-field)
      - [Integrating-factor equation for a planar vector field](#integrating-factor-equation-for-a-planar-vector-field)
      - [Periods obstruct a periodic potential](#periods-obstruct-a-periodic-potential)
      - [Potential of a conservative vector field](#potential-of-a-conservative-vector-field)
        - [Radial integral potential for a curl-free field](#radial-integral-potential-for-a-curl-free-field)
    - [Divergence theorem](#divergence-theorem)
      - [Gradient volume-to-boundary identity](#gradient-volume-to-boundary-identity)
      - [Vector gradient form of the divergence theorem](#vector-gradient-form-of-the-divergence-theorem)
      - [Boundary integral of position and normal components](#boundary-integral-of-position-and-normal-components)
      - [An entire bounded vector field cannot have nonzero constant divergence](#an-entire-bounded-vector-field-cannot-have-nonzero-constant-divergence)
      - [Riemannian divergence theorem](#riemannian-divergence-theorem)
    - [Fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals)
      - [Path independence](#path-independence)
    - [Stokes theorem](#stokes-theorem)
      - [Vector-valued Stokes identity](#vector-valued-stokes-identity)
      - [Stokes flux through an annular paraboloid](#stokes-flux-through-an-annular-paraboloid)
    - [Surface integral](#surface-integral)
      - [Vector surface element of a graph](#vector-surface-element-of-a-graph)
      - [Oriented surface element](#oriented-surface-element)
      - [Parametrized surface](#parametrized-surface)
      - [Surface area of a graph](#surface-area-of-a-graph)
      - [Flux integral](#flux-integral)
    - [Green theorem](#green-theorem)
      - [Boundary formula for planar area](#boundary-formula-for-planar-area)
    - [Line integral](#line-integral)
    - [Tensor divergence theorem](#tensor-divergence-theorem)
      - [Integration by parts for tensor fields](#integration-by-parts-for-tensor-fields)
  - [Jacobian matrix and determinant](#jacobian-matrix-and-determinant)
    - [Jacobian matrix](#jacobian-matrix)
      - [Spatial derivative control in perturbations of the identity map](#spatial-derivative-control-in-perturbations-of-the-identity-map)
      - [Jacobian determinant](#jacobian-determinant)
        - [Jacobian determinant as a divergence](#jacobian-determinant-as-a-divergence)
  - [Change of variables formula](#change-of-variables-formula)
    - [Ordered-cone substitution by products and ratios](#ordered-cone-substitution-by-products-and-ratios)
    - [Ratio-product coordinates](#ratio-product-coordinates)
    - [Squared-radius difference substitution](#squared-radius-difference-substitution)
    - [Weighted inverse multiplicity](#weighted-inverse-multiplicity)
    - [Rational square diffeomorphism](#rational-square-diffeomorphism)
    - [Hyperbolic substitution](#hyperbolic-substitution)
    - [Monotone substitution inequality](#monotone-substitution-inequality)
    - [Area formula (geometric measure theory)](#area-formula-geometric-measure-theory)
    - [Polar coordinates](#polar-coordinates)
      - [Cylindrical coordinate system](#cylindrical-coordinate-system)
        - [Azimuthal derivative of a cylindrical vector Fourier mode](#azimuthal-derivative-of-a-cylindrical-vector-fourier-mode)
        - [Cylindrical radius](#cylindrical-radius)
      - [Cardioid](#cardioid)
    - [Orthogonal coordinates](#orthogonal-coordinates)
      - [Del in cylindrical and spherical coordinates](#del-in-cylindrical-and-spherical-coordinates)
      - [Hyperspherical coordinates](#hyperspherical-coordinates)
        - [Spherical coordinate system](#spherical-coordinate-system)
          - [Radial unit vector in spherical coordinates](#radial-unit-vector-in-spherical-coordinates)
          - [Scale factors of orthogonal coordinates](#scale-factors-of-orthogonal-coordinates)
          - [Curl in spherical coordinates](#curl-in-spherical-coordinates)
        - [Volume of an n-ball](#volume-of-an-n-ball)
        - [Surface area of an n-sphere](#surface-area-of-an-n-sphere)
  - [Differentiable map](#differentiable-map)
    - [Functionally independent functions](#functionally-independent-functions)
    - [Derivative of a map into a level set](#derivative-of-a-map-into-a-level-set)
    - [Fréchet derivative](#frechet-derivative)
      - [Differentiability under equivalent norms](#differentiability-under-equivalent-norms)
      - [Hadamard differentiability](#hadamard-differentiability)
        - [Hadamard remainder near a compact set](#hadamard-remainder-near-a-compact-set)
        - [Stieltjes bilinear functional under a variation constraint](#stieltjes-bilinear-functional-under-a-variation-constraint)
      - [Fréchet differentiability](#frechet-differentiability)
      - [Derivative of matrix inversion](#derivative-of-matrix-inversion)
    - [Continuously differentiable function](#continuously-differentiable-function)
    - [Invertible linear map](#invertible-linear-map)
    - [Mean value inequality](#mean-value-inequality)
      - [Zero derivative on a connected open set](#zero-derivative-on-a-connected-open-set)
    - [Inverse function theorem](#inverse-function-theorem)
      - [Constant rank theorem](#constant-rank-theorem)
        - [Rank-one level curves from a characteristic differential equation](#rank-one-level-curves-from-a-characteristic-differential-equation)
      - [Local diffeomorphism](#local-diffeomorphism)
        - [Noninjective map with constant Jacobian determinant](#noninjective-map-with-constant-jacobian-determinant)
        - [Open map](#open-map)
      - [Implicit function theorem](#implicit-function-theorem)
        - [Holomorphic implicit function theorem](#holomorphic-implicit-function-theorem)
        - [Implicit differentiation](#implicit-differentiation)
          - [Cyclic partial derivative identity](#cyclic-partial-derivative-identity)
- [Symmetry in integration](#symmetry-in-integration)
- [Integration by parts](#integration-by-parts)
  - [Boundary term](#boundary-term)
- [Hyperbolic tangent](#hyperbolic-tangent)
  - [Inverse hyperbolic tangent](#inverse-hyperbolic-tangent)
  - [Small-argument expansion of the hyperbolic tangent](#small-argument-expansion-of-the-hyperbolic-tangent)
  - [Hyperbolic-function identity](#hyperbolic-function-identity)
  - [Hyperbolic Pythagorean identity](#hyperbolic-pythagorean-identity)
- [Even function](#even-function)
- [Odd function](#odd-function)
  - [Odd extension](#odd-extension)

## Floor and ceiling functions

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Floor_and_ceiling_functions)

The floor and ceiling functions round a [real number](arithmetic.md#real-number) $x$ to the nearest enclosing [integers](number-theory.md#integer): $\lfloor x\rfloor$ is the greatest integer at most $x$, and $\lceil x\rceil$ is the least integer at least $x$. They satisfy $\lceil x\rceil=-\lfloor-x\rfloor$.

### Floor function

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

The floor $\lfloor x\rfloor$ is the greatest [integer](number-theory.md#integer) not exceeding the real number $x$.

#### Fractional part

↑ **Parent:** [Floor function](#floor-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fractional_part)

The fractional part of a [real number](arithmetic.md#real-number) is $\{x\}=x-\lfloor x\rfloor\in[0,1)$.

### Ceiling function

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

The [ceiling function](#ceiling-function) gives the least [integer](number-theory.md#integer) greater than or equal to its input [real number](arithmetic.md#real-number).

## Integral

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral)

An integral accumulates a function over a domain and may be defined as a limit of finite sums.

### Wallis integrals

↑ **Parent:** [Integral](#integral)

The [Wallis integrals](#wallis-integrals) are $I_n=\int_0^{\pi/2}\sin^n x\,dx$ for integers $n\geq0$. [Integration by parts](#integration-by-parts) gives $nI_n=(n-1)I_{n-2}$ for $n\geq2$, with $I_0=\pi/2$, $I_1=1$. Hence

$$
I_{2n}=\frac{(2n)!}{2^{2n}(n!)^2}\frac\pi2,\qquad
I_{2n+1}=\frac{2^{2n}(n!)^2}{(2n+1)!}.
$$

Because $0<\sin x<1$ in the integration interval, $0<I_n<I_{n-1}$ for $n\geq1$. Combining this with the recurrence gives $2n/(2n+1)<I_{2n+1}/I_{2n}<1$, proving that the ratio tends to one and yielding the [Wallis product](topology.md#wallis-product).

### Dipole line-integral identity

↑ **Parent:** [Integral](#integral)

Here $r=|\mathbf r|$, $\mathbf P_c=\mathbf r-c\mathbf r_0$ and $P_c=|\mathbf P_c|$. The identity holds where the segment of source points $t\mathbf r_0$, $0\leq t\leq c$, avoids the observation point and the denominator is nonzero. Differentiating the right side with respect to $c$ gives the integrand and its value at $c=0$ is zero. Dotting with a [current dipole](electromagnetism.md#current-dipole) moment evaluates a continuous line of dipole [electric potentials](electromagnetism.md#electric-potential).

### Integrand

↑ **Parent:** [Integral](#integral)

In $\int_a^b f(x)\,dx$, the [function](function.md) $f$ is the [integrand](#integrand). It is distinct from the integration variable, the bounds and the resulting [integral](#integral). In [contour integration](complex-analysis.md#contour-integration), the transformed [integrand](#integrand) includes the parametrization derivative.

### Multiple integral

↑ **Parent:** [Integral](#integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiple_integral)

A multiple integral accumulates a [function](function.md) over a region with several coordinates. The [Fubini theorem](measure-theory.md#fubini-s-theorem) and [Tonelli theorem](measure-theory.md#tonelli-theorem) give conditions under which it equals successive one-dimensional [integrals](#integral). A [change of variables formula](#change-of-variables-formula) expresses it in new coordinates using the absolute [Jacobian determinant](#jacobian-determinant).

#### Odd-integrand cancellation by reflection

↑ **Parent:** [Multiple integral](#multiple-integral)

If a region is invariant under one coordinate reflection and an integrable function changes sign under that reflection, its [multiple integral](#multiple-integral) is zero. Apply the [change of variables formula](#change-of-variables-formula) to the reflection, whose absolute [Jacobian determinant](#jacobian-determinant) is one: the integral equals its negative. This applies to odd coordinate powers in symmetric volumes and to the off-diagonal entries of an [inertia tensor](classical-mechanics.md#inertia-tensor) when the [mass density](fluid-mechanics.md#density) shares the coordinate-reflection symmetries.

### Integral representation

↑ **Parent:** [Integral](#integral)

An integral representation expresses a [function](function.md) through an [integral](#integral) of specified data and an [integral kernel](functional-analysis.md#integral-kernel). [Green-function representations](analysis.md#green-function-representation) solve [differential equations](differential-equation.md) this way, while the [Bromwich inversion formula](analysis.md#bromwich-inversion-formula) reconstructs a function from its [Laplace transform](analysis.md#laplace-transform).

#### Trigonometric integral

↑ **Parent:** [Integral representation](#integral-representation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trigonometric_integral)

The sine and cosine integrals accumulate $\sin t/t$ and $\cos t/t$, with different normalizations at zero and infinity. They arise in [oscillatory integrals](distribution-theory.md#oscillatory-integral), [Fourier transforms](analysis.md#fourier-transform) of singular kernels and [Fourier series](fourier-series.md) of logarithmic profiles.

##### Cosine integral

↑ **Parent:** [Trigonometric integral](#trigonometric-integral)

For real $x>0$, its small-argument expansion is $\operatorname{Ci}(x)=\gamma_E+\log x+O(x^2)$. Integrating $\operatorname{Ci}'(x)=\cos x/x$ separates the logarithm from the regular correction. Its conventional constant is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant); the primary series normalization is [https://dlmf.nist.gov/6.6.E6](https://dlmf.nist.gov/6.6.E6) .

##### Sine integral

↑ **Parent:** [Trigonometric integral](#trigonometric-integral)

For real $x>0$, the sine integral approaches $\pi/2$. Exponential damping gives $\int_0^\infty e^{-at}\sin t/t\,dt=\arctan(1/a)$, so the limiting constant follows by letting $a\downarrow0$. [Integration by parts](#integration-by-parts) of the tail gives $\operatorname{Si}(x)=\pi/2-\cos x/x-\sin x/x^2+O(x^{-3})$.

### Lebesgue integration

↑ **Parent:** [Integral](#integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_integration)

Lebesgue integration constructs an integral from the measure of level sets or from approximation by simple functions. It is linear on integrable functions and is stable under the principal convergence theorems of [measure theory](measure-theory.md).

<h4 id="prekopa-leindler-inequality">Prékopa–Leindler inequality</h4>

↑ **Parent:** [Lebesgue integration](#lebesgue-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prékopa–Leindler_inequality)

If $0<\theta<1$ and nonnegative [measurable functions](measure-theory.md#measurable-function) satisfy $h((1-\theta)x+\theta y)\geq f(x)^{1-\theta}g(y)^\theta$ for all $x,y\in\mathbb R^n$, then their [Lebesgue integrals](measure-theory.md#lebesgue-integral) obey

$$
\int h\geq\left(\int f\right)^{1-\theta}\left(\int g\right)^\theta.
$$

The [quantile derivative identity](probability-theory.md#quantile-derivative-identity) and [monotone substitution inequality](#monotone-substitution-inequality) prove the one-dimensional case; [Tonelli theorem](measure-theory.md#tonelli-theorem) extends it by induction. It implies the [Brunn–Minkowski inequality](geometry-and-topology.md#brunn-minkowski-theorem).

#### Absolute continuity of the Lebesgue integral

↑ **Parent:** [Lebesgue integration](#lebesgue-integration)

If $f\in L^1$, then for every $\varepsilon>0$ there is $\delta>0$ such that $\int_E|f|<\varepsilon$ whenever the measure of $E$ is below $\delta$. In particular, integrals over a sequence of shrinking measurable sets tend to zero.

### Time integral

↑ **Parent:** [Integral](#integral)

A time integral accumulates an integrand over a time coordinate. In perturbation theory it commonly sums the effect of an interaction over all possible vertex times.

### Double integral

↑ **Parent:** [Integral](#integral)

A double integral integrates a function over a two-dimensional region. A [change of variables formula](#change-of-variables-formula) can replace the region and area element using a [Jacobian determinant](#jacobian-determinant).

It is a [multiple integral](#multiple-integral) with two integration variables.

### Monotonicity of the Lebesgue integral

↑ **Parent:** [Integral](#integral)

If measurable functions satisfy $f\leq g$ almost everywhere, then

$$
\int f\,d\mu\leq\int g\,d\mu
$$

whenever the two sides are defined.

### Antiderivative

↑ **Parent:** [Integral](#integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiderivative)

An antiderivative of $g$ is a [differentiable function](analysis.md#differentiable-function) $p$ satisfying $p'=g$.

#### Constant of integration

↑ **Parent:** [Antiderivative](#antiderivative)

If $F'=f$ on a connected interval, every other antiderivative is $F+C$ for a constant $C$. Indeed $(G-F)'=0$, so the [mean value theorem](#mean-value-theorem) makes $G-F$ constant. A boundary condition fixes $C$. For example $T'=-B/r^2$ integrates to $T=B/r+C$, and $T(R_s)=T_s$ gives $C=T_s-B/R_s$. Discarding an integration constant therefore needs an actual boundary condition or an approximation showing that its effect is small.

#### Additive constant

↑ **Parent:** [Antiderivative](#antiderivative)

Any two antiderivatives of the same function on a connected interval differ by an additive constant.

When parameterizing all antiderivatives, the arbitrary additive constant is the [constant of integration](#constant-of-integration).

### Gaussian integral

↑ **Parent:** [Integral](#integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_integral)

The Gaussian integral is

$$
\int_{-\infty}^{\infty}e^{-ax^2}\,dx=\sqrt{\frac\pi a},
\qquad a>0.
$$

Squaring the integral and changing to polar coordinates proves the formula.

#### Linear-source multivariate Gaussian integral

↑ **Parent:** [Gaussian integral](#gaussian-integral)

For real symmetric positive-definite $A$, complete the square with $v=u-A^{-1}b$. Orthogonal diagonalization reduces the remaining integral to the product of one-dimensional [Gaussian integrals](#gaussian-integral), proving the displayed expression. Positivity ensures convergence and the positive determinant square root. Replacing matrices by regulated field kernels gives the [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral); an oscillatory Minkowski integral instead requires a causal convergence prescription.

#### Dawson function

↑ **Parent:** [Gaussian integral](#gaussian-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dawson_function)

The Dawson function obeys $F_D'+2zF_D=1$ by [differentiation](#differentiation). Its large-real-argument [asymptotic expansion](analysis.md#asymptotic-expansion) begins $F_D(z)=1/(2z)+1/(4z^3)+O(z^{-5})$. This inverse-power behavior contrasts with the separate exponentially growing factors in its definition.

##### Gaussian drift primitives

↑ **Parent:** [Dawson function](#dawson-function)

Define $E_0(z)=\int_0^z e^{-t^2}\int_0^t e^{u^2}\,du\,dt$ and $E_1(z)=\int_0^z e^{-t^2}\int_0^t e^{u^2}\operatorname{erf}u\,du\,dt$. They satisfy $(D^2+2zD)E_0=1$ and $(D^2+2zD)E_1=\operatorname{erf}z$. The first is an [even function](#even-function), the second an [odd function](#odd-function), and their real tails are respectively $\frac12\log|z|+C_1+o(1)$ and $\operatorname{sgn}z[\frac12\log|z|+C_2+o(1)]$. Their derivatives have inverse-linear tails, explaining the logarithmic matching constants in a [singular perturbation](differential-equation.md#singular-perturbation).

#### Error function

↑ **Parent:** [Gaussian integral](#gaussian-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error_function)

The error function is

$$
\operatorname{erf}(x)=\frac2{\sqrt\pi}\int_0^xe^{-u^2}\,du.
$$

It is odd and tends to $\pm1$ as $x\to\pm\infty$.

##### Quadrant asymptotics of the error function

↑ **Parent:** [Error function](#error-function)

For $z=re^{i\theta}$ with fixed $0\le\theta\le\pi/2$, a horizontal tail gives $f(z)=\sqrt\pi/2-e^{-z^2}(2z)^{-1}[1+O(z^{-2})]$. The constant dominates through $\theta=\pi/4$; above that angle the exponential endpoint dominates. At the boundary angle its modulus is only $O(r^{-1})$, so the constant remains leading. On the imaginary axis the integral is purely imaginary and grows as $ie^{r^2}/(2r)$. The approximation is not a determination of exponentially subdominant constants in that growing sector.

##### Complementary error function

↑ **Parent:** [Error function](#error-function)

The complementary [error function](#error-function) avoids subtracting a quantity close to one when describing a small [Gaussian integral](#gaussian-integral) tail. For real $x>0$, $\operatorname{erfc}x=(2/\sqrt\pi)\int_x^\infty e^{-t^2}\,dt$; [analytic continuation](complex-analysis.md#analytic-continuation) defines it for complex arguments.

###### Faddeeva function

↑ **Parent:** [Complementary error function](#complementary-error-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faddeeva_function)

The Faddeeva function is an [entire function](complex-analysis.md#entire-function) built from the [complementary error function](#complementary-error-function). Its integral representation for $\operatorname{Im}z>0$ is $w(z)=(i\pi)^{-1}\int_{-\infty}^{\infty}e^{-t^2}/(t-z)\,dt$, as normalized in [NIST's integral representation](https://dlmf.nist.gov/7.7#E2). Its reflection identity is $w(-z)=2e^{-z^2}-w(z)$, directly from the [odd function](#odd-function) property of the [error function](#error-function).

###### Gaussian pole integral

↑ **Parent:** [Faddeeva function](#faddeeva-function)

For a pole off the real axis, substitution $s=2t$ into the [Faddeeva function](#faddeeva-function) integral gives $G(a)=i\pi w(a/2)$ when $\operatorname{Im}a>0$, and $G(a)=-i\pi w(-a/2)$ when $\operatorname{Im}a<0$. The difference of boundary values is the [residue theorem](analysis.md#residue-theorem) jump $2\pi i e^{-a^2/4}$. In particular, for a lower-half-plane pole, $G(a)+2\pi i e^{-a^2/4}=i\pi w(a/2)$, which packages a crossed residue and a nearby saddle into one smooth expression.

## Taylor polynomial

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_polynomial)

### Multivariate Taylor polynomial

↑ **Parent:** [Taylor polynomial](#taylor-polynomial)

The multivariate Taylor polynomial of total degree $p$ at $x_0$ is

$$
T_{x_0,p}(x)=\sum_{|\alpha|\leq p}
\frac{D^\alpha f(x_0)}{\alpha!}(x-x_0)^\alpha.
$$

## Exponential function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_function)

### e (mathematical constant)

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/e_(mathematical_constant))

Euler's number is the value $\exp(1)=\sum_{n=0}^{\infty}1/n!$ of the [exponential function](#exponential-function), approximately $2.71828$. It is the base of the natural [logarithm](#logarithm). Its factorial-series tail gives an elementary proof of the [irrationality of e](#irrationality-of-e).

#### Irrationality of e

↑ **Parent:** [e (mathematical constant)](#e-mathematical-constant)

If [Euler's number](#e-mathematical-constant) were $a/b$, choose $n\geq\max(b,2)$ and multiply its factorial-series tail by $n!$. This produces an [integer](number-theory.md#integer), but the tail is positive and smaller than $\sum_{j\geq1}(n+1)^{-j}=1/n<1$. The contradiction proves that the number is an [irrational number](algebra.md#irrational-number). The argument illustrates how a rapidly convergent rational series can [force](classical-mechanics.md#force) a hypothetical rational remainder into an impossible [integer](number-theory.md#integer) interval.

### Exponential series

↑ **Parent:** [Exponential function](#exponential-function)

The exponential function has the everywhere-convergent [power series](real-analysis.md#power-series)

$$
e^x=\sum_{n=0}^{\infty}\frac{x^n}{n!}.
$$

### Complex exponential function

↑ **Parent:** [Exponential function](#exponential-function)

The complex exponential is the entire function

$$
e^z=\sum_{n=0}^{\infty}\frac{z^n}{n!}.
$$

It maps $\mathbb C$ onto $\mathbb C^*$ and has kernel $2\pi i\mathbb Z$.

#### Modulus of the complex exponential

↑ **Parent:** [Complex exponential function](#complex-exponential-function)

For real $x,y$, the [complex exponential function](#complex-exponential-function) has $e^{x+iy}=e^x(\cos y+i\sin y)$. Since the trigonometric factor lies on the [unit circle](complex-analysis.md#complex-unit-circle),

$$
|e^z|=e^{\operatorname{Re}z}.
$$

Thus the [real part](complex-analysis.md#real-part) of the exponent controls its [modulus](complex-analysis.md#modulus), while the [imaginary part](complex-analysis.md#imaginary-part) controls its direction on the complex plane.

#### Complex sine function

↑ **Parent:** [Complex exponential function](#complex-exponential-function)

The complex sine is the entire function

$$
\sin z=\frac{e^{iz}-e^{-iz}}{2i}.
$$

For real $x,y$, $\sin(x+iy)=\sin x\cosh y+i\cos x\sinh y$.

##### Periodicity of the complex sine

↑ **Parent:** [Complex sine function](#complex-sine-function)

The kernel $2\pi i\mathbb Z$ of the [complex exponential function](#complex-exponential-function) gives

$$
\sin(z+2\pi)
=\frac{e^{iz}e^{2\pi i}-e^{-iz}e^{-2\pi i}}{2i}
=\sin z.
$$

The same period appears as the translation generated by the [monodromy of the complex inverse sine](complex-analysis.md#monodromy-of-the-complex-inverse-sine).

### Logarithm

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithm)

The logarithm to base $b>0$, $b\ne1$, is the inverse of the [exponential function](#exponential-function) $x\mapsto b^x$.

#### Geometric-series bound for the logarithmic remainder

↑ **Parent:** [Logarithm](#logarithm)

For $0<u<1$, the [power series](real-analysis.md#power-series) for the [logarithm](#logarithm) gives $-\log(1-u)-u=\sum_{n=2}^\infty u^n/n<\frac12\sum_{n=2}^\infty u^n=u^2/[2(1-u)]$. The inequality is strict because $1/n<1/2$ for every $n\geq3$.

#### Irrational logarithm criterion

↑ **Parent:** [Logarithm](#logarithm)

For [integers](number-theory.md#integer) $a,b>1$, rationality of $\log_a b$ is equivalent to equality of some positive [integer](number-theory.md#integer) powers $a^p=b^q$. Exponentiation proves one direction and taking [logarithms](#logarithm) proves the other. Thus multiplicatively independent [integers](number-theory.md#integer) give an [irrational number](algebra.md#irrational-number) as their logarithm ratio. For distinct prime bases and arguments, [unique factorization](algebra.md#unique-factorization-in-an-integral-domain) supplies that independence.

#### Concavity of the logarithm

↑ **Parent:** [Logarithm](#logarithm)

The [logarithm](#logarithm) is [strictly concave](real-analysis.md#strictly-concave-function) on positive real numbers, as its second [derivative](#derivative) is negative. Thus the [Jensen inequality](real-analysis.md#jensen-s-inequality) gives $\int\log f\,d\mu\le\log\int f\,d\mu$ for a [probability measure](probability-theory.md#probability-measure) and an integrable positive $f$, whenever the left side is defined. It also controls the negative logarithmic part of [convex](real-analysis.md#convex-function) combinations of strictly positive functions.

#### Logarithmic integral function

↑ **Parent:** [Logarithm](#logarithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_integral_function)

The [Cauchy principal value](complex-analysis.md#cauchy-principal-value) integral $\operatorname{li}(x)=\operatorname{PV}\int_0^xdt/\log t$ is the logarithmic integral. The offset version $\operatorname{Li}(x)=\int_2^xdt/\log t$ differs by a constant and is often used with the [prime-counting function](number-theory.md#prime-counting-function). It has $\operatorname{Li}(x)\sim x/\log x$.

#### Natural logarithm

↑ **Parent:** [Logarithm](#logarithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_logarithm)

The natural logarithm is the inverse of the real [exponential function](#exponential-function) on the positive real numbers.

#### Logarithm inequality

↑ **Parent:** [Logarithm](#logarithm)

For $x>0$, [concavity](real-analysis.md#concave-function) of the [natural logarithm](#natural-logarithm) gives

$$
\ln x\leq x-1.
$$

Equivalently, $\log_bx\leq(\log_be)(x-1)$ for $b>1$.

#### Operator monotonicity of logarithm

↑ **Parent:** [Logarithm](#logarithm)

For positive-definite [Hermitian operators](hilbert-space.md#hermitian-operator),

$$
0<A\leq B\quad\Longrightarrow\quad\log A\leq\log B.
$$

The same statement on supports follows by regularizing with a positive multiple of the identity and taking a [limit](#limit-of-a-function).

### Gaussian function

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_function)

A Gaussian function has the form $A\exp[-a(x-b)^2]$ with $a>0$. Its integral and moments reduce by translation and scaling to the [Gaussian integral](#gaussian-integral).

#### Gaussian decay dominates every power

↑ **Parent:** [Gaussian function](#gaussian-function)

For every fixed $m\ge0$, choose an integer $N>m/2$. The positive [exponential series](#exponential-series) gives $e^{t^2}\ge t^{2N}/N!$, so $|t|^m e^{-t^2}\le N!|t|^{m-2N}\to0$. Equivalently, $|x|^{-m}e^{-1/x^2}\to0$ as $x\to0$.

#### Gaussian dyadic summation bound

↑ **Parent:** [Gaussian function](#gaussian-function)

For fixed $c,h>0$, $L\ge1$ and $\varepsilon\ge0$, complete the square in the exponent. A translated [Gaussian function](#gaussian-function) summed on a fixed-spaced lattice has mass $O(\sqrt L)$ uniformly in the translate, by comparison with its integral and its maximum. This keeps a square-root logarithm, rather than the full number of dyadic intervals, when summing exponentially damped [exponential sum](analytic-number-theory.md#exponential-sum) bounds.

### Hyperbolic function

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_function)

Hyperbolic functions are combinations of the [exponential function](#exponential-function) analogous to [trigonometric functions](geometry-and-topology.md#trigonometric-function). The [hyperbolic cosine](#hyperbolic-cosine) and [hyperbolic sine](#hyperbolic-sine) satisfy $\cosh^2x-\sinh^2x=1$ and parametrize a unit [hyperbola](geometry-and-topology.md#hyperbola).

#### Inverse hyperbolic functions

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_hyperbolic_functions)

The inverse hyperbolic functions invert the [hyperbolic functions](#hyperbolic-function), with real branches on their standard ranges and complex branches obtained through [analytic continuation](complex-analysis.md#analytic-continuation). For example, $\operatorname{arsinh}z=\log(z+\sqrt{z^2+1})$ on a chosen branch; the [multivalued inverse hyperbolic sine](complex-analysis.md#multivalued-inverse-hyperbolic-sine) records all inverse values.

#### Hyperbolic cosine

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The hyperbolic cosine is $\cosh x=(e^x+e^{-x})/2$.

##### Factorial-tail irrationality proof for a hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](#hyperbolic-cosine)

For a fixed positive integer $q$, $\cosh(1/q)=\sum_{k\ge0}q^{-2k}/(2k)!$ is irrational. If it were rational with denominator $b$, choose $N$ large enough that $b\mid(2N)!$. After multiplication by $q^{2N}(2N)!$, the finite partial sum is an integer and the remaining positive tail is bounded by a geometric series whose ratio is at most $1/[q^2(2N+1)(2N+2)]$. For sufficiently large $N$, this tail is strictly between zero and one, contradicting its integer value. Only a finite integer partial sum is used; convergence of an infinite series of rationals does not itself prove irrationality.

##### Inverse hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](#hyperbolic-cosine)

For $x\geq1$, the inverse [hyperbolic cosine](#hyperbolic-cosine) on its nonnegative real branch is $\operatorname{arcosh}x=\log(x+\sqrt{x^2-1})$. It is the real cosine member of the [inverse hyperbolic functions](#inverse-hyperbolic-functions).

#### Hyperbolic sine

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The hyperbolic sine is $\sinh x=(e^x-e^{-x})/2$.

#### Hyperbolic cotangent

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The hyperbolic cotangent is $\coth x=\cosh x/\sinh x$ where $\sinh x\ne0$.

##### Partial-fraction expansion of the hyperbolic cotangent

↑ **Parent:** [Hyperbolic cotangent](#hyperbolic-cotangent)

The [hyperbolic-sine infinite product](real-analysis.md#hyperbolic-sine-infinite-product) gives, by taking its logarithmic derivative,

$$
\coth z=\frac1z+2z\sum_{n=1}^{\infty}\frac1{z^2+\pi^2n^2}.
$$

The identity holds away from the poles, with locally convergent sums. For real $z>0$, it makes $(z\coth z-1)/z^2$ positive and strictly decreasing. It is useful for [Hartmann flow](astrophysical-fluid-dynamics.md#hartmann-flow) flux monotonicity and small-argument expansions of [hyperbolic functions](#hyperbolic-function).

#### Hyperbolic secant

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The hyperbolic secant is

$$
\operatorname{sech}x=\frac1{\cosh x}.
$$

## Fundamental theorem of calculus

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_calculus)

### Fundamental theorem of calculus for Lebesgue integration

↑ **Parent:** [Fundamental theorem of calculus](#fundamental-theorem-of-calculus)

If $g\in L^1(a,b)$, then $F(x)=F(a)+\int_a^xg(s)\,ds$ is [absolutely continuous](sobolev-space.md#absolutely-continuous-function) and satisfies $F'=g$ [almost everywhere](measure-theory.md#almost-everywhere). Conversely, every absolutely continuous function has this form.

## Mean value theorem

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_value_theorem)

### Cauchy mean value theorem

↑ **Parent:** [Mean value theorem](#mean-value-theorem)

For real functions continuous on $[a,b]$ and differentiable on $(a,b)$, there exists $\xi\in(a,b)$ with

$$
[f(b)-f(a)]g'(\xi)=[g(b)-g(a)]f'(\xi).
$$

Apply [Rolle's theorem](#rolle-theorem) to a linear combination of the functions with equal endpoint values. If $g'$ never vanishes, $g(b)\ne g(a)$ and the equality can be divided into a ratio. This form directly proves the zero-over-zero endpoint case of [L'Hôpital's rule](#l-hopital-s-rule), without continuity of the derivatives.

### Endpoint secant-tangent approximation

↑ **Parent:** [Mean value theorem](#mean-value-theorem)

If $f$ is continuous at an interval endpoint, differentiable in its interior, and has a finite one-sided derivative there, then its secant slope and tangent slope are arbitrarily close at some interior point. Apply the [mean value theorem](#mean-value-theorem) on a short endpoint interval; both the secant at its far endpoint and the secant at the resulting intermediate point approach the same one-sided derivative. No continuity of the derivative is required.

## Rolle theorem

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rolle_theorem)

If a continuous real function is differentiable between two distinct points at which it has the same value, its derivative vanishes at some point between them.

### Rolle root count with multiplicities

↑ **Parent:** [Rolle theorem](#rolle-theorem)

If a nonzero real [polynomial](polynomial.md) has $N$ roots in an open real interval, counted with [multiplicity of a root](polynomial.md#multiplicity-of-a-root), its derivative has at least $N-1$ roots in that interval, also counted with multiplicity, provided $N\ge1$. Each root of multiplicity $m$ becomes a root of the derivative of multiplicity $m-1$. The [Rolle theorem](#rolle-theorem) supplies one further root between each pair of distinct consecutive roots. Thus $k$ distinct roots of multiplicities $m_j$ give at least $\sum_j(m_j-1)+(k-1)=N-1$ derivative roots.

## Taylor theorem

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_theorem)

The Taylor theorem expresses a sufficiently differentiable function as a finite [Taylor polynomial](#taylor-polynomial) plus a remainder.

### Taylor expansion from a periodic derivative equation

↑ **Parent:** [Taylor theorem](#taylor-theorem)

For a smooth real [function](function.md) satisfying the displayed equation with positive [integer](number-theory.md#integer) $r$, differentiating makes $f^{(j+r)}=f^{(j)}$. On any [compact](topology.md#compact-space) interval, all [derivatives](#derivative) are therefore bounded by the maximum of the bounds of $f,f',\ldots,f^{(r-1)}$. The [Taylor formula with integral remainder](#taylor-formula-with-integral-remainder) consequently has error at most $M R^{n+1}/(n+1)!$, which tends to zero uniformly for $|x|\le R$. Hence the [function](function.md) equals its globally convergent [Taylor series](#taylor-series). For $r=3$ and initial [derivatives](#derivative) $(1,0,0)$, it is $\sum_{k\ge0}x^{3k}/(3k)!$.

### Integral first-order Taylor formula for a vector map

↑ **Parent:** [Taylor theorem](#taylor-theorem)

For a continuously differentiable [vector-valued function](function.md#vector-valued-function) whose domain contains the segment from $x$ to $x+h$, apply the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) componentwise to $t\mapsto F(x+th)$. The resulting integral matrix is valid even when there is no common intermediate point giving a vector mean-value formula. For a [score function](statistical-modelling.md#informant-function), it integrates the [Hessian matrix](#hessian-matrix) along the segment to a candidate estimate.

### Integral remainder in Taylor theorem

↑ **Parent:** [Taylor theorem](#taylor-theorem)

If $f$ has $k+1$ continuous derivatives, its Taylor remainder about $a$ is

$$
R_k(x)=\frac1{k!}\int_a^x(x-t)^kf^{(k+1)}(t)\,dt.
$$

#### Logarithmic series from an integral Taylor remainder

↑ **Parent:** [Integral remainder in Taylor theorem](#integral-remainder-in-taylor-theorem)

The [integral remainder in Taylor theorem](#integral-remainder-in-taylor-theorem) for $\log(1-t)$ gives the exact finite identity

$$
-\log(1-t)=\sum_{k=1}^N\frac{t^k}{k}+\int_0^t\frac{(t-x)^N}{(1-x)^{N+1}}\,dx.
$$

For $0\leq x\leq t<1$, $(t-x)/(1-x)\leq t$, so the nonnegative remainder is at most $t^{N+1}/(1-t)$ and tends to zero. At $t=1/2$ it is at most $2^{-N}$, proving both convergence to $\log2$ and an explicit error bound without assuming the logarithmic [power series](real-analysis.md#power-series) beforehand.

### Taylor expansion

↑ **Parent:** [Taylor theorem](#taylor-theorem)

A Taylor expansion about a point consists of successive derivative terms there, together with either a finite remainder or an infinite [Taylor series](#taylor-series) when that series represents the function.

#### Peano zero

↑ **Parent:** [Taylor expansion](#taylor-expansion)

A Peano zero through order $r$ means that the [function](function.md) admits the zero [Taylor polynomial](#taylor-polynomial) with remainder $o(|t|^r)$ at $x_0$. This does not assert the existence of ordinary iterated [derivatives](#derivative) on a neighborhood. For example, multiplying $t^{r+1}$ by a bounded [continuous function](#continuous-function) with [dense](topology.md#dense-set) points of nondifferentiability preserves this estimate while destroying neighborhood [differentiability](analysis.md#differentiability).

#### Parabolic approximation

↑ **Parent:** [Taylor expansion](#taylor-expansion)

A parabolic approximation retains terms through second order in a local [Taylor expansion](#taylor-expansion). Near the closest point of a circle of radius $a$ and its tangent line, the separation is $x^2/(2a)+O(x^4/a^3)$.

### Taylor formula for a polynomial

↑ **Parent:** [Taylor theorem](#taylor-theorem)

For a polynomial $p$ of degree at most $m$, the Taylor formula is exact:

$$
p(t)=\sum_{j=0}^m\frac{p^{(j)}(x)}{j!}(t-x)^j.
$$

### Taylor theorem with Lagrange remainder

↑ **Parent:** [Taylor theorem](#taylor-theorem)

If $f$ is $n$ times differentiable between $a$ and $x$, then for some $\xi$ strictly between them,

$$
f(x)=\sum_{j=0}^{n-1}\frac{f^{(j)}(a)}{j!}(x-a)^j
+\frac{f^{(n)}(\xi)}{n!}(x-a)^n.
$$

### Taylor remainder

↑ **Parent:** [Taylor theorem](#taylor-theorem)

The Taylor remainder is the difference between a function and a finite [Taylor polynomial](#taylor-polynomial). Bounds on higher derivatives or their [Hölder continuity](sobolev-space.md#holder-condition) control this error.

### Taylor formula with integral remainder

↑ **Parent:** [Taylor theorem](#taylor-theorem)

If $f^{(m-1)}$ is locally absolutely continuous, then its Taylor remainder can be written as an integral involving the weak derivative $f^{(m)}$. This form permits norm bounds when the highest derivative is only integrable.

### Taylor series

↑ **Parent:** [Taylor theorem](#taylor-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_series)

The Taylor series of a sufficiently regular [function](function.md) about $a$ is

$$
\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n.
$$

## Limit of a function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_of_a_function)

The limit records the value approached by a function as its argument approaches a point.

### One-sided limit

↑ **Parent:** [Limit of a function](#limit-of-a-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-sided_limit)

A one-sided limit restricts the argument to values above or below the limiting point. It is denoted $\lim_{x\downarrow a}f(x)$ from above and $\lim_{x\uparrow a}f(x)$ from below.

### Continuous function

↑ **Parent:** [Limit of a function](#limit-of-a-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_function)

A function is continuous at a point when its limit there equals its value.

#### Blancmange curve

↑ **Parent:** [Continuous function](#continuous-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Blancmange_curve)

The Takagi function is a continuous nowhere [differentiable function](analysis.md#differentiable-function). The triangular summands are continuous and the geometric tail is bounded uniformly. On dyadic intervals of length $2^{-N}$, all terms of index at least $N$ vanish at both endpoints, while every lower summand has slope $+1$ or $-1$. Each refinement therefore changes the secant slope by exactly one in absolute value. The [secants straddling a differentiability point](analysis.md#secants-straddling-a-differentiability-point) lemma rules out a derivative at every real point.

#### Bounded continuous functions

↑ **Parent:** [Continuous function](#continuous-function)

[Bounded continuous functions](#bounded-continuous-functions) on a topological space form a [Banach space](banach-space.md) with the [supremum norm](functional-analysis.md#supremum-norm). A uniform limit is continuous and bounded, proving completeness. This space differs from the bounded uniformly [continuous functions](#continuous-function): free-transport composition is jointly continuous in time and position, but need not be continuous in the global sup [norm](functional-analysis.md#norm) as time varies.

#### Upper semicontinuity

↑ **Parent:** [Continuous function](#continuous-function)

A real or extended-real [function](function.md) is [upper semicontinuous](#upper-semicontinuity) when every strict sublevel set is open. Equivalently its negative is [lower semicontinuous](#lower-semicontinuity). An arbitrary infimum of continuous [functions](function.md) is [upper semicontinuous](#upper-semicontinuity), even when the infimum is over an uncountable family; its strict sublevel sets are unions of the corresponding open sublevel sets.

#### Oscillation multiplied by a vanishing amplitude

↑ **Parent:** [Continuous function](#continuous-function)

If $|h(x)|\leq C$ near $c$ and $a(x)\to0$ as $x\to c$, then $a(x)h(x)\to0$ by the [squeeze theorem](#squeeze-theorem), even if $h$ has no limit. Defining the product to be zero at $c$ gives continuity there. For example, $\sqrt{|x|}\sin(1/\sin x)$ extends continuously at zero; the same oscillation near a nonzero multiple of $\pi$ has nonvanishing amplitude and does not have a continuous zero extension.

#### Lower semicontinuity

↑ **Parent:** [Continuous function](#continuous-function)

A function is lower semicontinuous when its strict superlevel sets are open, equivalently when its sublevel sets are closed. In Euclidean spaces this is the [sequential lower semicontinuity](#sequential-lower-semicontinuity) condition $f(x)\leq\liminf_k f(x_k)$ whenever $x_k\to x$. This closedness property is essential to existence of proximal minimizers.

#### Discontinuity of a function

↑ **Parent:** [Continuous function](#continuous-function)

##### Removable discontinuity

↑ **Parent:** [Discontinuity of a function](#discontinuity-of-a-function)

A removable discontinuity has an existing finite limit that differs from the assigned point value, or a missing point value. Changing the point value removes it. Integrals and [Fourier coefficients](fourier-series.md#fourier-coefficient) do not detect changes on a set of measure zero, so purely integral hypotheses cannot prohibit this kind of discontinuity for an arbitrary representative.

##### Jump discontinuity

↑ **Parent:** [Discontinuity of a function](#discontinuity-of-a-function)

A jump occurs when both finite one-sided limits of a function exist but differ. Unlike an isolated change in value, a jump changes limiting values on whole one-sided neighbourhoods. [One-sided Fourier spectrum excludes jumps](partial-differential-equation.md#one-sided-fourier-spectrum-excludes-jumps) explains an obstruction to jumps for functions with only nonnegative [Fourier coefficients](fourier-series.md#fourier-coefficient).

#### Sequential lower semicontinuity

↑ **Parent:** [Continuous function](#continuous-function)

An extended-real functional $f$ is sequentially lower semicontinuous when $x_n\to x$ implies $f(x)\leq\liminf_nf(x_n)$.

##### Sublevel set

↑ **Parent:** [Sequential lower semicontinuity](#sequential-lower-semicontinuity)

A [sublevel set](#sublevel-set) consists of points whose objective value is at most a chosen threshold. [Coercivity](real-analysis.md#coercive-function) makes finite [sublevel sets](#sublevel-set) bounded, while [sequential lower semicontinuity](#sequential-lower-semicontinuity) makes them [sequentially closed sets](topology.md#sequentially-closed-set) in the selected [topology](topology.md).

###### Compact sublevel set

↑ **Parent:** [Sublevel set](#sublevel-set)

A [sublevel set](#sublevel-set) which is [compact](topology.md#compact-space). A [good rate function](convergence-of-random-variables.md#good-rate-function) has this property for every finite level.

##### Closed-sublevel-set characterization of lower semicontinuity

↑ **Parent:** [Sequential lower semicontinuity](#sequential-lower-semicontinuity)

On a metric space, a functional is [sequentially lower semicontinuous](#sequential-lower-semicontinuity) exactly when every sublevel set $\{x:f(x)\leq\eta\}$ is closed.

#### Locally constant function

↑ **Parent:** [Continuous function](#continuous-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_constant_function)

A function is locally constant when every point has a neighbourhood on which the function is constant.

##### Compactly supported locally constant function

↑ **Parent:** [Locally constant function](#locally-constant-function)

The space $C_c^\infty(X)$ consists of locally constant complex functions with compact support. On a [locally profinite group](topological-group.md#locally-profinite-group), finite compact-open coset covers of the support show that every such function is fixed by one common [compact-open subgroup](topological-group.md#compact-open-subgroup) under right translation. The symbol infinity describes local constancy in this context, not real differentiability.

#### Intermediate value theorem

↑ **Parent:** [Continuous function](#continuous-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intermediate_value_theorem)

If $f:[a,b]\to\mathbb R$ is continuous and $y$ lies between $f(a)$ and $f(b)$, then some $c\in[a,b]$ satisfies $f(c)=y$.

##### Continuous image of a real interval

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

A [continuous function](#continuous-function) on any [real interval](real-analysis.md#interval-mathematics) has image a [real interval](real-analysis.md#interval-mathematics). Given two image values and an intermediate value, choose preimages and apply the [intermediate value theorem](#intermediate-value-theorem) on the closed segment joining them, which stays inside the domain. Neither compactness nor boundedness of the original interval is needed. In particular $f(x)=\sin(1/x)/x$ on $(0,1]$ is a continuous surjection onto $\mathbb R$: its values are unbounded above and below, so its interval image contains every real number.

##### Interval order theorem for continuous injections

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

A continuous injective real-valued function on a real interval is strictly monotone. A value outside the interval between two endpoint values would, by the [intermediate value theorem](#intermediate-value-theorem), create a repeated value. Applying this observation to subintervals gives consistent strict ordering. If the left endpoint value is smaller than the right endpoint value, the function is strictly increasing; otherwise it is strictly decreasing.

##### Horizontal chord of reciprocal-integer length

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

If $f:[0,1]\to\mathbb R$ is continuous and $f(0)=f(1)$, then for every positive integer $n$ there is $\alpha\in[0,1-1/n]$ with $f(\alpha+1/n)=f(\alpha)$. For $n>1$, the continuous difference $h_n(x)=f(x+1/n)-f(x)$ satisfies $\sum_{j=0}^{n-1}h_n(j/n)=0$. Either one sampled difference is zero or two have opposite signs; the [intermediate value theorem](#intermediate-value-theorem) then supplies a zero between them. For $n=1$, the endpoint chord suffices.

##### Zero on a line segment

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

If a continuous real-valued function on a real or complex vector space has opposite signs at two points, restricting it to the line segment between them and applying the intermediate value theorem gives a zero.

##### Telescoping increment lemma

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

If a continuous $g:[0,na]\to\mathbb R$ satisfies $g(na)-g(0)=na$, then the increments

$$
h(x)=g(x+a)-g(x)-a
$$

satisfy $\sum_{k=0}^{n-1}h(ka)=0$. Continuity forces $h$ to vanish somewhere on $[0,(n-1)a]$.

##### Continuous bijection of the real line is monotone

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

Every continuous injective function from a real interval to the real line is strictly monotone. A continuous bijection $\mathbb R\to\mathbb R$ therefore has a continuous inverse.

#### Composition of continuous functions

↑ **Parent:** [Continuous function](#continuous-function)

If $f$ is continuous at $x$ and $g$ is continuous at $f(x)$, then $g\circ f$ is continuous at $x$.

#### Continuity set of a function

↑ **Parent:** [Continuous function](#continuous-function)

The continuity set of a function is the set of points where it is continuous. For a real function $f$, define its oscillation at $x$ by

$$
\omega_f(x)=\inf_{r>0}\sup\{|f(y)-f(z)|:y,z\in(x-r,x+r)\}.
$$

The sets $\{x:\omega_f(x)<\varepsilon\}$ are open, and $f$ is continuous at $x$ exactly when $\omega_f(x)=0$. Hence its continuity set is the $G_\delta$ [Borel set](measure-theory.md#borel-set)

$$
\bigcap_{n=1}^{\infty}\{x:\omega_f(x)<1/n\}.
$$

#### Right-continuous function

↑ **Parent:** [Continuous function](#continuous-function)

A function $f$ on the real line is right-continuous at $t$ when $f(s)\to f(t)$ as $s\downarrow t$.

Two-sided [continuity](#continuous-function) requires both the right and left limits to equal the function value.

<h5 id="cadlag">Càdlàg</h5>

↑ **Parent:** [Right-continuous function](#right-continuous-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Càdlàg)

A càdlàg function is right-continuous and has a finite left limit at every positive time. The name abbreviates the French phrase /continue à droite, limites à gauche/.

#### Uniformly continuous function

↑ **Parent:** [Continuous function](#continuous-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniformly_continuous_function)

A function is uniformly continuous when one input tolerance works at every point of its domain.

##### Decay of a nonnegative uniformly continuous integrable function

↑ **Parent:** [Uniformly continuous function](#uniformly-continuous-function)

A nonnegative uniformly continuous function on $[0,\infty)$ with finite integral tends to zero. Otherwise uniform continuity gives disjoint intervals of a fixed width on which the function exceeds a fixed positive value, contradicting integrability. This supplies a useful dissipation argument for [Lyapunov functions](dynamical-systems.md#lyapunov-function) with merely continuous vector fields.

### Squeeze theorem

↑ **Parent:** [Limit of a function](#limit-of-a-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squeeze_theorem)

If two functions with the same limit bound a third nearby, the bounded function has that limit too.

## Derivative

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Derivative)

The derivative is the limit of the difference quotient and gives the best linear approximation to local change.

### Symmetric second derivative

↑ **Parent:** [Derivative](#derivative)

The symmetric second derivative is the displayed limit when it exists. For a twice continuously differentiable function it equals the ordinary second derivative by Taylor expansion; the definition itself does not require ordinary differentiability. A [continuous function](#continuous-function) with vanishing symmetric second derivative throughout an interval must be affine, by [vanishing symmetric second derivative forces an affine function](#vanishing-symmetric-second-derivative-forces-an-affine-function). For a twice-integrated Fourier series, sinc-squared weights express this quotient, connecting the operation to [Riemann summation of a convergent trigonometric series](fourier-series.md#riemann-summation-of-a-convergent-trigonometric-series).

### Symmetric second differences detect an affine corner

↑ **Parent:** [Derivative](#derivative)

For a continuous function with affine formulas $At+B$ to the left of $c$ and $A't+B'$ to its right, the quotient $[F(c+h)-2F(c)+F(c-h)]/h$ equals $A'-A$ for positive $h$. If it tends to zero, the slopes agree, and continuity at $c$ makes the intercepts agree as well. This detects slope jumps that ordinary pointwise derivatives away from the corner cannot detect.

### Symmetric first-order differences remove an affine corner

↑ **Parent:** [Derivative](#derivative)

For a continuous function with affine formulas $At+B$ to the left of $c$ and $A't+B'$ to its right, the quotient $[F(c+h)-2F(c)+F(c-h)]/h$ equals $A'-A$ for positive $h$. If it tends to zero, the slopes agree, and continuity at $c$ makes the intercepts agree as well. This detects slope jumps that ordinary pointwise derivatives away from the corner cannot detect.

### Vanishing symmetric second derivative forces an affine function

↑ **Parent:** [Derivative](#derivative)

If a continuous real function on an interval has the displayed limit zero at every interior point, it is affine. On any compact subinterval subtract its endpoint chord. If the difference were positive somewhere, adding $\varepsilon(t-a)(t-b)$ for sufficiently small positive $\varepsilon$ would retain a positive interior maximum. At a maximum every symmetric second difference is nonpositive, but its normalized limit would be $2\varepsilon>0$. Thus the function lies below its chord; applying the same argument to its negative gives equality. Real and imaginary parts give the complex-valued version. Existence of ordinary second derivatives is unnecessary.

### One-sided derivative

↑ **Parent:** [Derivative](#derivative)

The right and left [one-sided derivatives](#one-sided-derivative) are the limits of the [difference quotient](#difference-quotient) restricted respectively to positive and negative increments:

$$
f'_+(a)=\lim_{h\downarrow0}\frac{f(a+h)-f(a)}h,
\qquad
f'_-(a)=\lim_{h\uparrow0}\frac{f(a+h)-f(a)}h.
$$

At an interior point, [differentiability](analysis.md#differentiability) is equivalent to existence and equality of these two finite limits. For the [absolute value function](real-analysis.md#absolute-value), $f'_+(0)=1$ and $f'_-(0)=-1$, so it is continuous at zero but not differentiable there.

### Tangent line

↑ **Parent:** [Derivative](#derivative)

The [tangent line](#tangent-line) to a differentiable [function](function.md) at $a$ is its affine first-order approximation $f(a)+f'(a)(x-a)$. For a differentiable [concave function](real-analysis.md#concave-function), it is an upper bound throughout a convex interval: the secant-slope inequality and passage to the [derivative](#derivative) give $f(x)\leq f(a)+f'(a)(x-a)$. This upper bound constructs valid envelopes in [adaptive rejection sampling](probability-and-statistics.md#adaptive-rejection-sampling).

### Automatic differentiation

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Automatic_differentiation)

[Automatic differentiation](#automatic-differentiation) evaluates derivatives of a computational graph using the [chain rule](#chain-rule). Reverse mode is [backpropagation](statistical-learning.md#backpropagation) and is useful for [reparameterization gradients](statistical-inference.md#reparameterization-gradient) through simulated trajectories.

### Differentiation

↑ **Parent:** [Derivative](#derivative)

Differentiation computes the [derivative](#derivative) of a [function](function.md). A [difference quotient](#difference-quotient) approximates a [derivative](#derivative) using finite increments; its [limit](#limit-of-a-function) is the [derivative](#derivative) when the [function](function.md) is [differentiable](analysis.md#differentiable-function).

### Second derivative

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_derivative)

The [derivative](#derivative) of the first [derivative](#derivative). For a twice [differentiable function](analysis.md#differentiable-function), its sign governs local [convexity](real-analysis.md#convex-function) and its magnitude controls the second-order [Taylor remainder](#taylor-remainder).

### Difference quotient

↑ **Parent:** [Derivative](#derivative)

A difference quotient divides a finite change in a function by the corresponding change in its argument. Its limit, when it exists, is the [derivative](#derivative).

#### Discrete integration by parts

↑ **Parent:** [Difference quotient](#difference-quotient)

With $\delta_h f(x)=[f(x+he_\ell)-f(x)]/h$, a change of variables gives

$$
\int g\,\delta_h f=-\int(\delta_{-h}g)f.
$$

The [compact support](function.md#compact-support) of $f$ and its translates must remain inside the integration domain, or one must integrate over the whole space with convergent integrals. In particular $\delta_{-h}g(x)=[g(x)-g(x-he_\ell)]/h$: the denominator's sign matters. This is the [difference quotient](#difference-quotient) analogue of [integration by parts](#integration-by-parts).

### Total derivative

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_derivative)

A total derivative accounts for every dependence of a quantity on the variable of differentiation. Its integral contributes only boundary terms.

<h3 id="l-hopital-s-rule">L'Hôpital's rule</h3>

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/L'Hôpital's_rule)

For an indeterminate quotient whose numerator and denominator both tend to zero or both diverge, suitable differentiability and denominator conditions allow its limit to be computed from the limit of the quotient of their derivatives.

#### Derivative quotient limits on partial domains

↑ **Parent:** [L'Hôpital's rule](#l-hopital-s-rule)

The usual zero-over-zero [L'Hopital rule](#l-hopital-s-rule) requires the denominator's [derivative](#derivative) to be nonzero throughout a sufficiently small deleted neighborhood. A limit taken only where that [derivative](#derivative) is nonzero is insufficient. An explicit counterexample uses $x_n=2^{-n}$, $h_n=4^{-n}$, $S(u)=3u^2-2u^3$ and $q(u)=16u^2(1-u)^2$. On $[3x_n/4,x_n]$ put $g=h_n$ and $f=h_nq((x-3x_n/4)/(x_n/4))$. On $[x_n/2,3x_n/4]$ put $g=h_{n+1}+(h_n-h_{n+1})S((x-x_n/2)/(x_n/4))$ and $f=0$. Extend $g=1,f=0$ beyond one. Values and first [derivatives](#derivative) agree at the joins, both functions tend to zero, and $g$ is positive. Where $g'\ne0$, it lies inside a transition interval and $f'=0$. Thus $f'/g'$ has natural-domain limit zero, but $f/g$ equals zero at $x_n$ and one at $7x_n/8$, so has no limit.

<h3 id="darboux-s-theorem-analysis">Darboux's theorem (analysis)</h3>

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Darboux's_theorem_(analysis))

Every derivative has the intermediate-value property, even when the derivative is discontinuous.

#### Intermediate secant slope from endpoint derivatives

↑ **Parent:** [Darboux's theorem (analysis)](#darboux-s-theorem-analysis)

Let $m=(f(b)-f(a))/(b-a)$ for a function differentiable on a neighborhood of $[a,b]$. If $m=k$, use the whole interval. If $m>k$, the continuous extension of $(f(x)-f(a))/(x-a)$ takes values $f'(a)$ and $m$ at the endpoints, so the [intermediate value theorem](#intermediate-value-theorem) supplies a secant of slope $k$ starting at $a$. If $m<k$, use the continuous extension of $(f(b)-f(x))/(b-x)$ and obtain a secant ending at $b$. The [mean value theorem](#mean-value-theorem) then produces an interior [derivative](#derivative) equal to $k$, without requiring a continuous derivative.

### Product rule

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_rule)

If $f$ and $g$ are differentiable at $a$, then

$$
(fg)'(a)=f'(a)g(a)+f(a)g'(a).
$$

#### Differentiability restored by a quadratic zero

↑ **Parent:** [Product rule](#product-rule)

For a [continuous function](#continuous-function) $f:\mathbb R\to\mathbb R$, $g(t)=t^2f(t)$ is [differentiable](analysis.md#differentiable-function) at zero with $g'(0)=0$, because $[g(h)-g(0)]/h=hf(h)\to0$. At any nonzero point $x$, $g$ is [differentiable](analysis.md#differentiable-function) exactly when $f$ is: one direction uses the [product rule](#product-rule), and the converse applies it to $f(t)=t^{-2}g(t)$ near $x$.

#### Leibniz rule

↑ **Parent:** [Product rule](#product-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leibniz_rule)

The higher-order product rule is

$$
(fg)^{(n)}=\sum_{k=0}^n\binom nk f^{(k)}g^{(n-k)}.
$$

#### Nondifferentiable factor with a differentiable nondegenerate product

↑ **Parent:** [Product rule](#product-rule)

At zero, $f(x)=x$ and $g(x)=1+|x|$ give a differentiable product

$$
f(x)g(x)=x+x|x|
$$

with derivative one, although $g$ is not differentiable.

### Quotient rule

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_rule)

If $f$ and $g$ are [differentiable](analysis.md#differentiable-function) and $g\ne0$, then

$$
\left(\frac fg\right)'
=\frac{f'g-fg'}{g^2}.
$$

### Chain rule

↑ **Parent:** [Derivative](#derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chain_rule)

If $f$ is differentiable at $a$ and $g$ is differentiable at $f(a)$, then

$$
(g\circ f)'(a)=g'(f(a))f'(a).
$$

#### Nondifferentiable inner function with a differentiable nondegenerate composite

↑ **Parent:** [Chain rule](#chain-rule)

At zero, $f(x)=\sqrt[3]x$ is not differentiable and $g(y)=y^3$ is differentiable, while $g\circ f(x)=x$ has derivative one.

#### Second derivative chain rule

↑ **Parent:** [Chain rule](#chain-rule)

For twice differentiable functions,

$$
(g\circ f)''(a)
=g''(f(a))[f'(a)]^2+g'(f(a))f''(a).
$$

## Monotonic function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monotonic_function)

A function is increasing when $x\le y$ implies $f(x)\le f(y)$.

### Monotone mean-value point of an integral average

↑ **Parent:** [Monotonic function](#monotonic-function)

For a continuous strictly decreasing real function, its average $h(x)=x^{-1}\int_0^xf(t)dt$ lies strictly between $f(x)$ and $f(0)$ for $x>0$. There is a unique $g(x)\in(0,x)$ with $f(g(x))=h(x)$. If $f$ is [differentiable](analysis.md#differentiable-function) and $f'<0$ throughout the positive half-line, the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) and the derivative formula for the monotone inverse give

$$
g'(x)=\frac{f(x)-f(g(x))}{xf'(g(x))}>0.
$$

Continuity of $f'$ is unnecessary: differentiability of a strictly monotone function with nonzero derivative at a point suffices for differentiability of its inverse there.

### Nonincreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A nonincreasing [function](function.md) may be constant on intervals. A nonincreasing sequence of natural numbers has finitely many strict drops, so it is eventually constant. This differs from a strictly decreasing sequence, which cannot continue indefinitely within the natural numbers.

// Target: foundations-of-mathematics.bigb

### Non-strict inverse of a continuous nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

For a continuous unbounded [nondecreasing function](#nondecreasing-function) $f$ on the nonnegative half-line and $a>f(0)$, the non-strict inverse $h$ is left-continuous in its level argument. It equals the left limit of the [strict generalized inverse of a nondecreasing function](#strict-generalized-inverse-of-a-nondecreasing-function) $G(a)=\inf\{t:f(t)>a\}$. Indeed $G(b)\leq h(a)$ for $b<a$, while for every $t<h(a)$, $f(t)<a$ and choosing $b\in(f(t),a)$ gives $G(b)\geq t$. Similarly $h(a+)=G(a)$. A flat part of $f$ at level $a$ gives a discrepancy between the two inverses: $h(a)$ selects the beginning of the flat part and $G(a)$ its end. For a [Brownian running maximum](brownian-motion.md#brownian-running-maximum), these are the non-strict and strict passage times.

### Left-continuous cumulative function of an atomic measure

↑ **Parent:** [Monotonic function](#monotonic-function)

For positive summable weights $w_j$ at points $q_j$, the strict cumulative function $F(x)=\sum_{q_j<x}w_j$ is nondecreasing and left-continuous. A finite-head/tail argument proves left-continuity, and its right jump at an atom is the mass there. This strict convention differs at atoms from the usual right-continuous [cumulative distribution function](probability-theory.md#cumulative-distribution-function).

### Nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A nondecreasing [function](function.md) never decreases when its argument increases. Flat intervals are allowed, unlike for a [strictly increasing function](#strictly-increasing-function). Nondecreasing allocation functions permit [critical-value payments](game-theory.md#critical-value-payment) in [single-parameter mechanisms](game-theory.md#single-parameter-mechanism).

### Strict generalized inverse of a nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

For an unbounded nondecreasing function $f:[0,\infty)\to\mathbb R$, its strict generalized inverse is $G(a)=\inf\{t\geq0:f(t)>a\}$. It is nondecreasing and right-continuous in $a$. If $a_n\downarrow a$, then for any $t>G(a)$ monotonicity gives $f(t)>a$, so eventually $f(t)>a_n$ and $G(a_n)\leq t$; also $G(a_n)\geq G(a)$. Local finiteness gives finite left limits. Flat parts of $f$ create jumps of $G$. For the continuous running maximum of [Brownian motion](brownian-motion.md), this gives the [càdlàg](#cadlag) [Brownian first-passage subordinator](stochastic-process.md#brownian-first-passage-subordinator).

### Strictly increasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A function is strictly increasing when $x<y$ implies $f(x)<f(y)$. It is therefore [injective](algebra.md#injective-function) and each value has at most one preimage.

#### Continuity of an increasing interval surjection

↑ **Parent:** [Strictly increasing function](#strictly-increasing-function)

A strictly increasing function from a closed real interval onto the interval between its endpoint values is continuous. Given a desired output tolerance, choose nearby output values on either side and use their preimages to trap nearby inputs. At the endpoints only one side is needed. Equivalently, a discontinuity of a monotone function creates a gap in its range, which is incompatible with surjectivity onto an interval.

### Lebesgue theorem on differentiability of monotone functions

↑ **Parent:** [Monotonic function](#monotonic-function)

Every real-valued [monotone function](#monotonic-function) on a [real interval](real-analysis.md#interval-mathematics) is [differentiable](analysis.md#differentiable-function) with a finite [derivative](#derivative) at [almost every](measure-theory.md#almost-everywhere) point.

This strengthens the regularity known for a [monotonic function](#monotonic-function) beyond the restriction on its jump discontinuities.

## Multivariable calculus

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multivariable_calculus)

Multivariable calculus extends differentiation and integration to functions of several variables.

### Volume integral

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_integral)

A [volume integral](#volume-integral) integrates a scalar or componentwise [vector field](#vector-field) over a three-dimensional region with its [volume form](differential-form.md#volume-form). In [spherical polar coordinates](#spherical-coordinate-system) the Euclidean volume form is $r^2\sin\theta\,dr\,d\theta\,d\phi$. The [divergence theorem](#divergence-theorem) relates a volume integral of a [divergence](#divergence) to a boundary [flux integral](#flux-integral).

### Fundamental theorem of calculus along a line segment

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)

If $f:U\to\mathbb R^m$ is continuously differentiable and the segment from $x$ to $y$ lies in $U$, then

$$
f(y)-f(x)=\int_0^1Df(x+t(y-x))(y-x)\,dt.
$$

### Partial derivative

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_derivative)

A partial derivative differentiates a multivariable [function](function.md) with respect to one variable while holding the others fixed.

#### Partial derivatives do not imply continuity

↑ **Parent:** [Partial derivative](#partial-derivative)

Define $f(x,y)=xy/(x^2+y^2)$ away from the origin and zero at the origin. Both [partial derivatives](#partial-derivative) exist everywhere and are zero at the origin, yet along $x=y$ the function is $1/2$, so it is not [continuous](#continuous-function) there. Coordinate-axis derivative tests do not control all neighboring directions.

#### Mixed partial derivative

↑ **Parent:** [Partial derivative](#partial-derivative)

A mixed partial derivative takes [partial derivatives](#partial-derivative) in different variables, for example $f_{xy}=\partial_y(\partial_x f)$. If both second [partial derivatives](#partial-derivative) are continuous in a neighbourhood, their order can be interchanged: $f_{xy}=f_{yx}$. The [chain rule](#chain-rule) transforms mixed partial derivatives under a linear [change of variables](#change-of-variables-formula) by composing the corresponding first-order differential operators.

##### Unequal mixed partial derivatives

↑ **Parent:** [Mixed partial derivative](#mixed-partial-derivative)

For $f(x,y)=xy(x^2-y^2)/(x^2+y^2)$ away from the origin and zero at the origin, $|f|\leq(x^2+y^2)/2$ proves [Fréchet differentiability](#frechet-differentiability) with zero derivative. Yet $f_x(0,y)=-y$ and $f_y(x,0)=x$, giving the displayed unequal [mixed partial derivatives](#mixed-partial-derivative). They exist but are not continuous at the origin, so [Clairaut's theorem](#symmetry-of-second-derivatives) does not apply.

##### Symmetry of second derivatives

↑ **Parent:** [Mixed partial derivative](#mixed-partial-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetry_of_second_derivatives)

When the second [partial derivatives](#partial-derivative) are continuous in a neighborhood, the order of the [mixed partial derivatives](#mixed-partial-derivative) can be interchanged. Expressing a rectangular finite difference as either iterated integral by the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) and shrinking the rectangle proves the equality. Mere existence of both derivatives does not imply this symmetry.

#### Time derivative

↑ **Parent:** [Partial derivative](#partial-derivative)

A time derivative is the [partial derivative](#partial-derivative) of an evolving field with respect to time while holding its spatial coordinates fixed. For a quantity depending only on time, it is an ordinary [derivative](#derivative).

#### Spatial derivative

↑ **Parent:** [Partial derivative](#partial-derivative)

A spatial derivative is a [partial derivative](#partial-derivative) with respect to a spatial coordinate.

#### Directional derivative

↑ **Parent:** [Partial derivative](#partial-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Directional_derivative)

The directional derivative of $f$ at $x$ in the direction $v$ is

$$
D_vf(x)=\left.\frac d{dt}f(x+tv)\right|_{t=0}.
$$

For a differentiable scalar function on Euclidean space, it equals $v\mathbin\cdot\nabla f(x)$.

##### Directional derivatives do not imply differentiability

↑ **Parent:** [Directional derivative](#directional-derivative)

Define $f(x,y)=x^3/(x^2+y^2)$ away from the origin and zero at the origin. Every [directional derivative](#directional-derivative) exists. Along a unit vector $n$, the derivative at the origin is $n_1^3$, which is not linear in $n$. Thus these directional derivatives cannot be the restrictions of one [Fréchet derivative](#frechet-derivative), and the function is not [Fréchet differentiable](#frechet-differentiability) at that point.

##### Directional derivative of a convex function is sublinear

↑ **Parent:** [Directional derivative](#directional-derivative)

For a [locally Lipschitz function](real-analysis.md#locally-lipschitz-function) that is [convex](real-analysis.md#convex-function) near $x$, increasing secant slopes have a finite right limit. Positive rescaling of $t$ gives positive homogeneity in $y$. The [convexity](real-analysis.md#convex-function) bound $f(x+t(y+z))\leq[f(x+2ty)+f(x+2tz)]/2$ gives subadditivity after subtracting $f(x)$, dividing by $t$ and taking the limit. Thus $p_x$ is a finite [sublinear functional](functional-analysis.md#sublinear-function), although it need not be a [linear functional](linear-algebra.md#linear-functional).

#### Gradient

↑ **Parent:** [Partial derivative](#partial-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gradient)

The gradient of a scalar-valued [differentiable function](analysis.md#differentiable-function) is the [vector](vector-space.md#vector) of its first partial derivatives.

##### Gradient of a dot product

↑ **Parent:** [Gradient](#gradient)

For differentiable [vector fields](#vector-field), expand the [cross products](vector-space.md#cross-product) using the [contraction of two Levi-Civita symbols](#contraction-of-two-levi-civita-symbols). The directional-derivative terms cancel the corresponding terms in the two cross products, leaving $\partial_i(F_jG_j)$. This proves the displayed [gradient](#gradient) identity by the [product rule](#product-rule).

##### Gradient field

↑ **Parent:** [Gradient](#gradient)

A gradient field is a vector field of the form $\nabla f$ for a scalar potential $f$. Its curl vanishes wherever the required second derivatives commute.

#### Total differential

↑ **Parent:** [Partial derivative](#partial-derivative)

For a differentiable scalar function of several variables, the total differential is

$$
df=\sum_i\frac{\partial f}{\partial x_i}\,dx_i.
$$

### Hessian matrix

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hessian_matrix)

The Hessian is the symmetric matrix of second partial derivatives; definiteness classifies [nondegenerate critical points](#nondegenerate-critical-point).

#### Quadratic growth from a bounded Hessian

↑ **Parent:** [Hessian matrix](#hessian-matrix)

For $F\in C^2(\mathbb R^n)$ with bounded [Hessian matrix](#hessian-matrix), Taylor's formula along the line from zero to $p$ gives $|F(p)|\leq|F(0)|+|DF(0)||p|+\frac12\|D^2F\|_\infty|p|^2$. Its gradient obeys $|DF(p)|\leq|DF(0)|+\|D^2F\|_\infty|p|$. Consequently $\int_\Omega F(Du)$ is finite for $u\in H^1(\Omega)$ when $\Omega$ has finite measure, and $DF(Du)\in L^2$.

#### Higher-order test for separated extrema

↑ **Parent:** [Hessian matrix](#hessian-matrix)

For $f(x,y)=g(x)+h(y)$, a degenerate [Hessian matrix](#hessian-matrix) can be supplemented by the first nonzero term of each one-variable displacement. Two negative leading even powers give a strict [local maximum](analysis.md#local-maximum), two positive ones a strict [local minimum](analysis.md#local-minimum), and opposite signs give a saddle. Looking along the coordinate directions and bounding the separated terms avoids an inconclusive quadratic test.

#### Negative semidefinite matrix

↑ **Parent:** [Hessian matrix](#hessian-matrix)

A symmetric matrix $A$ is negative semidefinite when $v^TAv\leq0$ for every vector $v$. Equivalently, all its [eigenvalues](linear-operator-theory.md#eigenvalue) are nonpositive.

#### Second-derivative test

↑ **Parent:** [Hessian matrix](#hessian-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second-derivative_test)

At an interior local maximum of a twice differentiable function, its [Hessian matrix](#hessian-matrix) is negative semidefinite; at a local minimum it is positive semidefinite. For a scalar function on Euclidean space, the Laplacian is therefore nonpositive at a local maximum and nonnegative at a local minimum.

##### Critical points escaping to infinity in a Gaussian-weighted bilinear function

↑ **Parent:** [Second-derivative test](#second-derivative-test)

The origin is a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function) for every real parameter. For $\alpha>0$ four further [critical points](analysis.md#critical-point) have $x^2=y^2=1/(2\alpha)$. Equal-sign coordinates give global maxima and opposite-sign coordinates give [global minima](analysis.md#global-minimum), with values $\pm1/(2e\alpha)$. The [Hessian matrix](#hessian-matrix) there is $-4\alpha xy e^{-1}I$. Their distance from the origin is $\alpha^{-1/2}$, so as $\alpha\downarrow0$ they escape every compact region. At nonpositive $\alpha$ the origin is the only [critical point](analysis.md#critical-point). This illustrates why the number of [critical points](analysis.md#critical-point) on an unbounded domain can change without a finite degenerate [critical point](analysis.md#critical-point) appearing.

#### Nondegenerate critical point

↑ **Parent:** [Hessian matrix](#hessian-matrix)

A critical point of a twice differentiable function is nondegenerate when its [Hessian matrix](#hessian-matrix) is invertible there. A positive-definite Hessian gives a strict local minimum, a negative-definite Hessian gives a strict local maximum, and an indefinite Hessian gives a saddle point.

Such critical points are the local building blocks of [Morse theory](differential-geometry.md#morse-theory).

### Vector calculus

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_calculus)

Vector calculus studies differentiation and integration of scalar and vector fields.

#### Dot-product gradient identity

↑ **Parent:** [Vector calculus](#vector-calculus)

For continuously differentiable [vector fields](#vector-field), the [gradient](#gradient) of their [dot product](linear-algebra.md#dot-product) expands as displayed. The [contraction of two Levi-Civita symbols](#contraction-of-two-levi-civita-symbols) gives $[F\times(\nabla\times G)]_i=F_j\partial_iG_j-F_j\partial_jG_i$; adding the directional derivative cancels the second term. Interchanging the fields and using the [product rule](#product-rule) proves the identity. It does not require either field to be irrotational.

#### Helmholtz decomposition

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helmholtz_decomposition)

The [Helmholtz decomposition](#helmholtz-decomposition) separates a [vector field](#vector-field) into a [gradient](#gradient) field and a field with zero [divergence](#divergence). The precise function spaces, [boundary conditions](differential-equation.md#boundary-condition) and decay hypotheses determine existence and uniqueness. In the square-integrable bounded-domain formulation, the solenoidal component is selected by the [Leray-Helmholtz projection](viscous-fluid-flow.md#leray-helmholtz-projection).

#### Divergence of a cross product

↑ **Parent:** [Vector calculus](#vector-calculus)

For differentiable vector fields $A$ and $B$,

$$
\nabla\cdot(A\times B)=B\cdot(\nabla\times A)-A\cdot(\nabla\times B).
$$

#### Vector field

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_field)

A vector field assigns a vector to every point of its domain.

##### Flow of a vector field

↑ **Parent:** [Vector field](#vector-field)

The local flow of a smooth [vector field](#vector-field) is the family of solutions of its [ordinary differential equation](differential-equation.md#ordinary-differential-equation), with $\Phi_0(p)=p$. Uniqueness gives $\Phi_{s+t}=\Phi_s\circ\Phi_t$ wherever defined. A compactly supported smooth [vector field](#vector-field) on a manifold without boundary is complete, so its flow exists for all real times.

##### Time-dependent vector field

↑ **Parent:** [Vector field](#vector-field)

A smooth family $Y_t$ assigns a tangent vector at each space-time point. Its [flow maps](dynamical-systems.md#flow-map) solve $\partial_t\rho_t=Y_t\circ\rho_t$, with $\rho_0$ the identity. For a varying [differential form](differential-form.md), differentiation gives $\partial_t(\rho_t^*\alpha_t)=\rho_t^*(\dot\alpha_t+\mathcal L_{Y_t}\alpha_t)$.

###### Finite-time flow completeness on a compact manifold

↑ **Parent:** [Time-dependent vector field](#time-dependent-vector-field)

A smooth [time-dependent vector field](#time-dependent-vector-field) on a compact manifold without boundary has [flow maps](dynamical-systems.md#flow-map) throughout each compact time interval on which the field is defined. Finite-time escape is impossible on the compact state space. Uniqueness and the backward-time equation supply smooth inverses, so the flow is a [smooth isotopy](differential-geometry.md#smooth-isotopy).

##### Radial dilation tangency to homogeneous zero sets

↑ **Parent:** [Vector field](#vector-field)

Differentiate the displayed homogeneity relation in $\lambda$ at $1$. On every regular point of $H=0$, the radial [vector field](#vector-field) $x$ is therefore perpendicular to the normal [gradient](#gradient) and tangent to the level surface. Its flow $x(t)=e^t x(0)$ preserves that zero set. At a singular vertex this flow formulation remains meaningful even if there is no tangent plane.

##### Divergence and curl of a radial vector field

↑ **Parent:** [Vector field](#vector-field)

For $r=|x|>0$, the [gradient](#gradient) satisfies $\partial_i r=x_i/r$. The [product rule](#product-rule) and [Einstein notation](linear-algebra.md#einstein-notation) then give the displayed [divergence](#divergence) formula in dimension $n$. In dimension three, its derivative [matrix](vector-space.md#matrix) is symmetric, so the [curl](#curl) vanishes. Zero [divergence](#divergence) forces $f(r)=Cr^{-n}$ on each positive radial interval. This formula does not assert regularity at the origin.

##### Azimuthal inverse-radius vector field

↑ **Parent:** [Vector field](#vector-field)

The [vector field](#vector-field) $\mathbf G=(-y,x,0)/(x^2+y^2)$ has zero [curl](#curl) away from its excluded axis, but has circulation $2\pi$ around a positively oriented circle enclosing that axis. [Stokes theorem](#stokes-theorem) gives zero total circulation for a smooth annular surface avoiding the axis, whose inner and outer boundary circles have opposite orientations. It cannot be applied directly to a disk meeting the axis, because the field is undefined there.

##### Integral curve of a vector field

↑ **Parent:** [Vector field](#vector-field)

An integral curve follows a [vector field](#vector-field) by solving the displayed [ordinary differential equation](differential-equation.md#ordinary-differential-equation). For a smooth [vector field](#vector-field), integral curves through initial points assemble into its [local flow](differential-geometry.md#local-flow).

###### Curvature of an integral curve of a vector field

↑ **Parent:** [Integral curve of a vector field](#integral-curve-of-a-vector-field)

For a [continuously differentiable](#continuously-differentiable-function) nonzero [vector field](#vector-field) $F$, the [curvature of a space curve](differential-geometry.md#curvature-of-a-space-curve) following its direction is

$$
\kappa=\frac{|F\times(F\cdot\nabla)F|}{|F|^3}.
$$

Take the [unit tangent vector](differential-geometry.md#unit-tangent-vector) $t=\pm F/|F|$ and differentiate with respect to [arc length](riemannian-geometry.md#arc-length). The derivative of $|F|^{-1}$ is parallel to $F$ and disappears from $t\times t'$. Since $t\cdot t'=0$, we have $|t\times t'|=|t'|=\kappa$, proving the formula. It remains valid with zero curvature, even where the usual [Frenet frame](differential-geometry.md#frenet-frame) is undefined.

##### Axisymmetric vector field

↑ **Parent:** [Vector field](#vector-field)

An axisymmetric vector field is invariant under rotations about a chosen axis. In cylindrical coordinates, its components are independent of the azimuthal angle.

##### Solenoidal vector field

↑ **Parent:** [Vector field](#vector-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solenoidal_vector_field)

A solenoidal vector field has zero [divergence](#divergence). Magnetic fields are solenoidal because $\nabla\mathbin\cdot\mathbf B=0$.

###### Poloidal-toroidal decomposition

↑ **Parent:** [Solenoidal vector field](#solenoidal-vector-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poloidal–toroidal_decomposition)

A spherical [poloidal-toroidal decomposition](#poloidal-toroidal-decomposition) represents a [solenoidal vector field](#solenoidal-vector-field) with zero flux through each sphere by scalar potentials $S,T$. The second term is tangent to concentric spheres; the first carries the radial component. Requiring zero angular means for the potentials fixes their otherwise irrelevant radial additions. In a plane layer, the analogous fluctuating components are $\nabla\times\nabla\times(\phi\hat{\mathbf z})$ and $\nabla\times(\psi\hat{\mathbf z})$, with any horizontally uniform components handled separately. These constructions enforce the [divergence-free](#solenoidal-vector-field) condition because the [divergence](#divergence) of a [curl](#curl) vanishes.

// Target: fluid-mechanics.bigb

###### Poloidal magnetic energy bound by the radial scalar gradient

↑ **Parent:** [Poloidal-toroidal decomposition](#poloidal-toroidal-decomposition)

For an isolated [solenoidal](#solenoidal-vector-field) [magnetic field](electromagnetism.md#magnetic-field), zero flux through every sphere removes the degree-zero [spherical harmonic](analysis.md#spherical-harmonic) of $P=\mathbf B\cdot\mathbf x$. In a [poloidal-toroidal decomposition](#poloidal-toroidal-decomposition), let $\mathcal L^2=-\Delta_{S^2}$. The spherical poloidal component obeys

$$
\int_{\mathbb R^3}|\mathbf B_P|^2=\int_{\mathbb R^3}\nabla(\mathcal L^{-2}P)\cdot\nabla P.
$$

If $P=\sum_{l\geq1,m}p_{lm}(r)Y_{lm}$, put $D_{lm}=\int_0^\infty[r^2|p'_{lm}|^2+l(l+1)|p_{lm}|^2]\,dr$. The two sides of the bound are respectively $\sum D_{lm}/[l(l+1)]$ and $\tfrac12\sum D_{lm}$. Since $l(l+1)\geq2$, the bound follows, with equality for degree-one radial scalars. Together with the [radial-flow dynamo energy bound](astrophysical-fluid-dynamics.md#radial-flow-dynamo-energy-bound) it gives $(q/\eta)^2\geq2E_P/E_{\mathrm{total}}$ for a marginal or growing dynamo field.

// Target: fluid-mechanics.bigb

#### Spherically symmetric function

↑ **Parent:** [Vector calculus](#vector-calculus)

A scalar function on Euclidean space is spherically symmetric when it depends only on the distance $r=|x|$ from a fixed center.

#### Helicity conservation by tangent boundary conditions

↑ **Parent:** [Vector calculus](#vector-calculus)

If a helicity density evolves as a sum of directional derivatives along divergence-free fields tangent to the boundary, its volume integral is conserved because both terms become vanishing boundary fluxes.

#### Divergence

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divergence)

For $F=(F_1,F_2,F_3)$ in Cartesian coordinates,

$$
\nabla\cdot F=\partial_iF_i
=\frac{\partial F_1}{\partial x}
+\frac{\partial F_2}{\partial y}
+\frac{\partial F_3}{\partial z}.
$$

##### Divergence of a Riemannian vector field

↑ **Parent:** [Divergence](#divergence)

For the [Levi-Civita connection](general-relativity.md#levi-civita-connection) of a [Riemannian metric](differential-geometry.md#riemannian-metric), the divergence of $X$ is $\operatorname{div}_gX=\operatorname{tr}(Y\mapsto\nabla_YX)$. In coordinates it equals $(\det g)^{-1/2}\partial_i((\det g)^{1/2}X^i)$. On an oriented manifold it satisfies $\mathcal L_X\omega_g=(\operatorname{div}_gX)\omega_g$. The [codifferential](differential-form.md#codifferential) on a [one-form](differential-form.md#one-form) satisfies $\delta\theta=-\operatorname{div}_g(\theta^\sharp)$, where $\sharp$ is the [musical isomorphism](differential-geometry.md#musical-isomorphism); this follows by [integration by parts](#integration-by-parts) or the [Hodge star](differential-form.md#hodge-star-operator) formula.

##### Cylindrically radial divergence

↑ **Parent:** [Divergence](#divergence)

For a [vector field](#vector-field) directed radially from a fixed axis and depending only on distance $\rho$ from that axis, [cylindrical coordinates](#cylindrical-coordinate-system) give $\nabla\cdot[f(\rho)\mathbf e_\rho]=f\prime+f/\rho$. Zero [divergence](#divergence) gives $f=A/\rho$ on any positive radial interval. Unless $A=0$, this field is singular on the axis, so applications of the [divergence theorem](#divergence-theorem) must use a domain avoiding it or account separately for that singularity.

##### Distributional divergence

↑ **Parent:** [Divergence](#divergence)

For a locally integrable [vector field](#vector-field), this formula defines its divergence as a [distribution](distribution-theory.md#distribution-mathematical-analysis). For a piecewise [smooth](analysis.md#smooth-function) field, a jump of its normal component across an interface adds a surface measure to the [smooth](analysis.md#smooth-function) divergences. A [continuous](#continuous-function) normal component eliminates that measure, as follows by [integration by parts](#integration-by-parts) on the two sides.

##### Divergence in polar coordinates

↑ **Parent:** [Divergence](#divergence)

For $\mathbf u=u_r\mathbf e_r+u_\theta\mathbf e_\theta$,

$$
\nabla\cdot\mathbf u
=\frac1r\frac{\partial(ru_r)}{\partial r}
+\frac1r\frac{\partial u_\theta}{\partial\theta}.
$$

##### Product rule for divergence

↑ **Parent:** [Divergence](#divergence)

For a scalar field $\phi$ and vector field $F$,

$$
\nabla\mathbin\cdot(\phi F)=\nabla\phi\mathbin\cdot F+\phi\nabla\mathbin\cdot F.
$$

##### Total divergence

↑ **Parent:** [Divergence](#divergence)

A total divergence has the form $\nabla\mathbin\cdot\mathbf F$. The [divergence theorem](#divergence-theorem) converts its volume integral into a boundary flux, which vanishes when the field has suitable decay or boundary conditions.

##### Divergence of a curl is zero

↑ **Parent:** [Divergence](#divergence)

For a twice continuously differentiable [vector field](#vector-field), commuting partial derivatives and antisymmetry of the Levi-Civita symbol give

$$
\nabla\mathbin\cdot(\nabla\times\mathbf F)=0.
$$

#### Curl

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Curl)

The curl of $F$ has components

$$
(\nabla\times F)_i=\epsilon_{ijk}\partial_jF_k.
$$

##### Curl of a gradient

↑ **Parent:** [Curl](#curl)

For a twice continuously differentiable [function](function.md), the [curl](#curl) of its [gradient](#gradient) vanishes. In components, $\epsilon_{ijk}\partial_j\partial_kf=0$ because the second derivatives are symmetric in $j,k$ while the [Levi-Civita symbol](#levi-civita-symbol) is antisymmetric. Thus adding a gradient to a [vector potential](#vector-potential) preserves the represented curl. No topological assumption is needed for this identity, unlike the converse assertion that every [curl-free vector field](#irrotational-vector-field) has a global potential.

##### Irrotational vector field

↑ **Parent:** [Curl](#curl)

A continuously differentiable [vector field](#vector-field) on an open subset of three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm) is irrotational when its [curl](#curl) is zero. Under the Euclidean identification $\alpha=X_i\,dx^i$, this says that the [differential one-form](differential-form.md#one-form) $\alpha$ is a [closed differential form](differential-form.md#closed-differential-form). The [Poincaré lemma](differential-form.md#poincare-lemma) gives a [potential of a conservative vector field](#potential-of-a-conservative-vector-field) locally. A global potential additionally requires zero [line integrals](#line-integral) around every closed curve; [simply connected](algebraic-topology.md#simply-connected-space) domains ensures this. On the punctured plane extended in the third direction, $X=(-y,x,0)/(x^2+y^2)$ has zero curl but integral $2\pi$ around a circle, so it is locally conservative and has no single-valued global potential.

##### Vector potential

↑ **Parent:** [Curl](#curl)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_potential)

A vector potential for a divergence-free vector field $F$ is a vector field $A$ satisfying $F=\nabla\times A$. It is not unique because adding a [gradient](#gradient) leaves its curl unchanged.

###### Radial vector potential of a solenoidal vector field

↑ **Parent:** [Vector potential](#vector-potential)

Let $B$ be a [continuously differentiable](#continuously-differentiable-function) [solenoidal vector field](#solenoidal-vector-field) on an open [star-shaped set](algebra.md#star-shaped-set) containing the origin. Then

$$
A(x)=\left(\int_0^1tB(tx)\,dt\right)\times x
$$

is a [vector potential](#vector-potential) for $B$. For $D=\int_0^1tB(tx)\,dt$, differentiation gives $\nabla\cdot D=0$ and $\nabla\times(D\times x)=2D+(x\cdot\nabla)D=\int_0^1\partial_t(t^2B(tx))\,dt=B(x)$. Boundedness near the origin removes the lower endpoint. A field defined only on a punctured domain need not satisfy these hypotheses.

##### Curl of the curl identity

↑ **Parent:** [Curl](#curl)

For a twice differentiable vector field $A$,

$$
\nabla\times(\nabla\times A)
=\nabla(\nabla\cdot A)-\nabla^2A.
$$

#### Laplacian

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplacian)

The Laplacian of a twice differentiable scalar field is the divergence of its gradient, $\nabla^2f=\nabla\cdot\nabla f$; it acts componentwise on vector fields.

##### Laplacian in polar coordinates

↑ **Parent:** [Laplacian](#laplacian)

For a twice differentiable scalar field on the plane,

$$
\nabla^2f=\frac1r\frac{\partial}{\partial r}\left(r\frac{\partial f}{\partial r}\right)
+\frac1{r^2}\frac{\partial^2f}{\partial\theta^2}.
$$

##### Product rule for the Laplacian

↑ **Parent:** [Laplacian](#laplacian)

For twice differentiable scalar fields,

$$
\nabla^2(fg)
=f\nabla^2g+2\nabla f\mathbin\cdot\nabla g
+g\nabla^2f.
$$

##### Biharmonic operator

↑ **Parent:** [Laplacian](#laplacian)

The biharmonic operator applies the [Laplacian](#laplacian) twice. Under clamped boundary conditions, two integrations by parts give the positive quadratic form

$$
\langle\Delta^2u,u\rangle=\int_\Omega|\Delta u|^2.
$$

###### Clamped biharmonic problem

↑ **Parent:** [Biharmonic operator](#biharmonic-operator)

The clamped problem uses the [weak solution](partial-differential-equation.md#weak-solution) identity $\int\Delta u\Delta v=\int fv$ for every $v$ in the [clamped second-order Sobolev space](sobolev-space.md#clamped-second-order-sobolev-space). For $f\in L^2(U)$, the [clamped Hessian identity](sobolev-space.md#clamped-hessian-identity) and the [Poincaré inequality](sobolev-space.md#poincare-inequality) make this a bounded [coercive bilinear form](linear-algebra.md#coercive-bilinear-form). The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique [weak solution](partial-differential-equation.md#weak-solution) without a mean-zero condition on $f$.

###### Biharmonic equation

↑ **Parent:** [Biharmonic operator](#biharmonic-operator)

The [biharmonic equation](#biharmonic-equation) is $\nabla^4f=0$, where the [biharmonic operator](#biharmonic-operator) is the square of the [Laplacian](#laplacian). In planar [Stokes flow](stokes-flow.md), taking the curl of the momentum equation and using a [Cartesian streamfunction](fluid-mechanics.md#cartesian-streamfunction) produces this equation. Its decaying spatial [Fourier series](fourier-series.md) modes have form $(A+By)e^{-|k|y}e^{ikx}$.

###### Spherical mean of a biharmonic function

↑ **Parent:** [Biharmonic equation](#biharmonic-equation)

For a smooth three-dimensional biharmonic function regular throughout a ball, its surface average has exactly this form. Taylor expansion and rotationally invariant spherical moments turn each even term into a multiple of an iterated [Laplacian](#laplacian); terms from the fourth derivative onward vanish when $\Delta^2f=0$. This is the mean-value identity that converts the reciprocal surface average into [Faxén's first law](stokes-flow.md#faxen-s-first-law).

#### Divergence and curl of a cross product

↑ **Parent:** [Vector calculus](#vector-calculus)

For smooth vector fields $F,G$,

$$
\nabla\cdot(F\times G)
=G\cdot(\nabla\times F)-F\cdot(\nabla\times G)
$$

and

$$
\nabla\times(F\times G)
=F(\nabla\cdot G)-G(\nabla\cdot F)
+(G\cdot\nabla)F-(F\cdot\nabla)G.
$$

Both follow by contracting two Levi-Civita symbols and applying the product rule.

##### Curl of a cross product

↑ **Parent:** [Divergence and curl of a cross product](#divergence-and-curl-of-a-cross-product)

The displayed [vector calculus](#vector-calculus) identity follows by contracting the two alternating tensors in the component formula for [curl](#curl). If both fields have zero [divergence](#divergence), only the two directional derivatives remain. It rewrites the transport terms in the [adjoint linearized Navier-Stokes evolution](hydrodynamic-stability.md#adjoint-linearized-navier-stokes-evolution).

#### Levi-Civita symbol

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Levi-Civita_symbol)

In three dimensions, $\epsilon_{ijk}$ is zero when indices repeat and is the sign of the permutation $(i,j,k)$ otherwise.

##### Rotation invariance of the Levi-Civita symbol

↑ **Parent:** [Levi-Civita symbol](#levi-civita-symbol)

The [determinant](linear-algebra.md#determinant) transformation formula for the [Levi-Civita symbol](#levi-civita-symbol) shows that it is invariant under every proper [rotation matrix](linear-algebra.md#rotation-matrix), for which $\det R=1$. Under an orthogonal reflection its sign reverses. This distinguishes proper-rotation isotropy from the [pseudotensor](linear-algebra.md#pseudotensor) transformation convention when both orientations are included.

##### Contraction of two Levi-Civita symbols

↑ **Parent:** [Levi-Civita symbol](#levi-civita-symbol)

Contracting one index gives

$$
\epsilon_{ijk}\epsilon_{ipq}
=\delta_{jp}\delta_{kq}-\delta_{jq}\delta_{kp}.
$$

##### Lagrange identity for the cross product

↑ **Parent:** [Levi-Civita symbol](#levi-civita-symbol)

For three-dimensional vectors,

$$
|x\times y|^2=|x|^2|y|^2-(x\cdot y)^2.
$$

The corresponding identity in $\mathbb R^n$ is

$$
|x|^2|y|^2-(x\cdot y)^2
=\frac12\sum_{i,j}(x_iy_j-x_jy_i)^2.
$$

##### Triple product

↑ **Parent:** [Levi-Civita symbol](#levi-civita-symbol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triple_product)

For three vectors in oriented Euclidean three-space, the scalar [triple product](#triple-product) is $a\cdot(b\times c)$ and the vector triple product is $a\times(b\times c)$. The former is their signed volume; the latter is the vector operation appearing in the [vector triple product identity](#vector-triple-product).

###### Vector triple product

↑ **Parent:** [Triple product](#triple-product)

Contracting two Levi-Civita symbols gives

$$
a\times(b\times c)=b(a\cdot c)-c(a\cdot b).
$$

#### Feasible inner products with two unit vectors

↑ **Parent:** [Vector calculus](#vector-calculus)

For linearly independent unit vectors $y,z$ with $c=y\cdot z$, a pair

$$
p=x\cdot y,\qquad q=x\cdot z
$$

is attained by some unit vector $x$ exactly when

$$
\frac{p^2-2cpq+q^2}{1-c^2}\leq1.
$$

The left-hand side is the squared norm of the least-norm vector having those two inner products.

#### Conservative vector field

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conservative_vector_field)

A [vector field](#vector-field) $X$ is conservative when $X=\nabla\Phi$ for a [potential of a conservative vector field](#potential-of-a-conservative-vector-field) $\Phi$. On a [simply connected](algebraic-topology.md#simply-connected-space) open subset of $\mathbb R^3$, every continuously differentiable [curl-free vector field](#irrotational-vector-field) is conservative. Locally this follows from the [Poincaré lemma](differential-form.md#poincare-lemma) applied to the [differential one-form](differential-form.md#one-form) $X_i\,dx^i$; globally, simple connectivity makes its [line integral](#line-integral) independent of the path. The [fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals) expresses that path independence as the difference of the potential at the endpoints.

##### Integrating-factor equation for a planar vector field

↑ **Parent:** [Conservative vector field](#conservative-vector-field)

If $\psi(A_1,A_2)$ is a [conservative vector field](#conservative-vector-field), equality of the mixed derivatives of its potential gives $\partial_y(\psi A_1)=\partial_x(\psi A_2)$. Expanding proves the displayed necessary equation. For continuously differentiable data on the whole plane, the vanishing planar curl is also sufficient for a potential. A useful [integrating factor](differential-equation.md#integrating-factor) is nonzero on the region under consideration.

##### Periods obstruct a periodic potential

↑ **Parent:** [Conservative vector field](#conservative-vector-field)

If a periodic [vector field](#vector-field) has a periodic [potential of a conservative vector field](#potential-of-a-conservative-vector-field), the [line integral](#line-integral) between points separated by a period vector must vanish, since it is the potential difference. A periodic gradient field need not satisfy this: the constant field $(1,2)$ on the plane has potential $x+2y$, but its integrals over the two unit translations are $1$ and $2$. On the periodic quotient these translation integrals are nonzero periods, obstructing a single-valued potential there.

##### Potential of a conservative vector field

↑ **Parent:** [Conservative vector field](#conservative-vector-field)

A potential for a [conservative vector field](#conservative-vector-field) $X$ is a [function](function.md) with [scalar](vector-space.md#scalar) values $\Phi$ whose [gradient](#gradient) is $X$. Potentials differ by a constant on each connected component. The [fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals) gives $\int_\gamma X\cdot d\mathbf x=\Phi(\gamma(1))-\Phi(\gamma(0))$. In mechanics a conservative force is conventionally written $-\nabla V$, so its potential energy is $V=-\Phi$. This spatial potential differs from the [scalar potential](quantum-field-theory.md#scalar-potential) $V(\phi)$ that denotes the derivative-free energy density of a [scalar field](quantum-field-theory.md#scalar-field).

###### Radial integral potential for a curl-free field

↑ **Parent:** [Potential of a conservative vector field](#potential-of-a-conservative-vector-field)

For a continuously differentiable [curl-free vector field](#irrotational-vector-field) $F$ on a domain star-shaped about the origin, define $\Phi$ by the displayed integral. Differentiation and $\partial_iF_j=\partial_jF_i$ give $\partial_i\Phi=\int_0^1[F_i(tx)+t x_j\partial_jF_i(tx)]\,dt=\int_0^1\partial_t[tF_i(tx)]\,dt=F_i(x)$. Thus $F=\nabla\Phi$. To adopt the sign convention $F=-\nabla\phi$, take $\phi=-\Phi$. The star-shaped-domain hypothesis ensures every segment used in the construction lies in the domain; curl-free fields need not have global potentials on arbitrary domains.

#### Divergence theorem

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divergence_theorem)

##### Gradient volume-to-boundary identity

↑ **Parent:** [Divergence theorem](#divergence-theorem)

For a continuously differentiable scalar $\Omega$ on a bounded region $V$ with outward boundary normal, $\int_V\nabla\Omega\,dV=\int_{\partial V}\Omega\mathbf n\,dS$. Apply the [divergence theorem](#divergence-theorem) to $\mathbf c\Omega$ for every constant vector $\mathbf c$; equality of all scalar projections gives the vector identity. The theorem applies to piecewise smooth boundaries, with singular points removed by a limiting argument when necessary.

##### Vector gradient form of the divergence theorem

↑ **Parent:** [Divergence theorem](#divergence-theorem)

For a continuously differentiable scalar-valued function $f$ on a bounded sufficiently regular region, apply the [divergence theorem](#divergence-theorem) to $fk$, where $k$ is any constant vector. Since $\nabla\cdot(fk)=k\cdot\nabla f$, the dot products of the two displayed vector integrals with every $k$ agree. The vector integrals are therefore equal. This is the scalar-gradient analogue of the usual flux identity.

##### Boundary integral of position and normal components

↑ **Parent:** [Divergence theorem](#divergence-theorem)

For a bounded sufficiently regular region, the [divergence theorem](#divergence-theorem) applied to the vector field $x_i e_j$ gives the displayed identity. Contracting with constant vectors gives $\int_{\partial\Omega}(b\cdot x)(c\cdot n)\,dS=|\Omega|b\cdot c$. Contracting with the [Kronecker delta](linear-algebra.md#kronecker-delta) or the [Levi-Civita symbol](#levi-civita-symbol) respectively gives $\int x\cdot n\,dS=3|\Omega|$ and $\int x\times n\,dS=0$ in three dimensions.

##### An entire bounded vector field cannot have nonzero constant divergence

↑ **Parent:** [Divergence theorem](#divergence-theorem)

For $X\in C^1(\mathbb R^n;\mathbb R^n)$, integration over $B_R$ gives $|\kappa||B_R|\leq\|X\|_\infty|\partial B_R|$, so $|\kappa|\leq n\|X\|_\infty/R$. Let $R\to\infty$. In particular, the bounded flux $Du/\sqrt{1+|Du|^2}$ of an entire constant-mean-curvature graph forces its divergence constant to be zero, independently of any bound on $Du$.

##### Riemannian divergence theorem

↑ **Parent:** [Divergence theorem](#divergence-theorem)

On an oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with boundary, the [divergence of a Riemannian vector field](#divergence-of-a-riemannian-vector-field) obeys the displayed integral identity for smooth [compactly supported](function.md#compact-support) [vector fields](#vector-field) $X$, or for arbitrary smooth $X$ if the manifold is compact. Here $N$ is the outward unit [normal vector](differential-geometry.md#normal-vector) and the boundary has the [outward-normal-first boundary orientation](differential-geometry.md#outward-normal-first-boundary-orientation). Its induced [Riemannian volume form](differential-geometry.md#riemannian-volume-form) is $j^*\iota_N\omega_g$. Splitting $X$ into its normal and tangential components gives $j^*\iota_X\omega_g=g(X,N)\omega_{\widetilde g}$, since a top form vanishes on $n$ boundary-tangent arguments. Apply the [Stokes theorem](#stokes-theorem) to $d\iota_X\omega_g=(\operatorname{div}X)\omega_g$.

Without a support or decay condition, flux at infinity can invalidate the result even if the integrals converge. On $[0,\infty)$ with [Riemannian metric](differential-geometry.md#riemannian-metric) $dx^2$, $X=(\arctan x)\partial_x$ has boundary flux zero but integral of divergence $\pi/2$.

#### Fundamental theorem for line integrals

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_for_line_integrals)

##### Path independence

↑ **Parent:** [Fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals)

A line integral is path independent when its value depends only on the two endpoints. On a connected domain, this holds for the line integral of every [exact differential](differential-form.md#exact-differential).

For a vector-field [line integral](#line-integral), this condition is equivalent to the field being a [conservative vector field](#conservative-vector-field).

#### Stokes theorem

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stokes_theorem)

##### Vector-valued Stokes identity

↑ **Parent:** [Stokes theorem](#stokes-theorem)

For an oriented smooth surface and compatible boundary orientation, apply [Stokes theorem](#stokes-theorem) to $\phi\mathbf k$ for an arbitrary constant vector $\mathbf k$. Since $\nabla\times(\phi\mathbf k)=\nabla\phi\times\mathbf k$, its surface integral is $\mathbf k\cdot\int_S d\mathbf S\times\nabla\phi$. The boundary integral is $\mathbf k\cdot\oint\phi\,d\mathbf x$. Equality for every $\mathbf k$ proves the displayed vector identity. Reversing both orientations preserves the identity.

##### Stokes flux through an annular paraboloid

↑ **Parent:** [Stokes theorem](#stokes-theorem)

For an upward-oriented band of the circular [elliptic paraboloid](geometry-and-topology.md#elliptic-paraboloid) between radii $r_0$ and $R$, the [vector field](#vector-field) $B=(-y^3,x^3,z^3)$ has vertical [curl](#curl) $3(x^2+y^2)$. Its [surface integral](#surface-integral) is $3\pi(R^4-r_0^4)/2$. [Stokes theorem](#stokes-theorem) gives the same value from the counterclockwise outer circle minus the counterclockwise inner circle. Equivalently the induced inner boundary direction is clockwise. Forgetting the inner boundary or its reversed orientation changes the answer.

#### Surface integral

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_integral)

A surface integral uses the area element induced by a parametrisation to integrate over a surface.

##### Vector surface element of a graph

↑ **Parent:** [Surface integral](#surface-integral)

The graph $z=g(x,y)$ has upward-oriented vector area element $d\mathbf S=(-g_x,-g_y,1)\,dx\,dy$ and scalar area element $dS=\sqrt{1+g_x^2+g_y^2}\,dx\,dy$. These follow from the [cross product](vector-space.md#cross-product) of the parametrization derivatives $(1,0,g_x)$ and $(0,1,g_y)$. The vector element is used in flux [surface integrals](#surface-integral) and [Stokes theorem](#stokes-theorem); reversing orientation changes its sign.

##### Oriented surface element

↑ **Parent:** [Surface integral](#surface-integral)

For an oriented parametrized surface $r(u,v)$, the vector surface element is $d\mathbf S=(r_u\times r_v)\,du\,dv$, with the sign chosen to match the orientation.

##### Parametrized surface

↑ **Parent:** [Surface integral](#surface-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parametrized_surface)

A parametrised surface $r(u,v)$ has area element $|r_u\times r_v|\,du\,dv$.

##### Surface area of a graph

↑ **Parent:** [Surface integral](#surface-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_area_of_a_graph)

The graph $z=f(x,y)$ has area element $\sqrt{1+f_x^2+f_y^2}\,dx\,dy$.

##### Flux integral

↑ **Parent:** [Surface integral](#surface-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flux_integral)

A flux integral $\int_SF\cdot n\,dS$ measures flow through an oriented surface.

#### Green theorem

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Green_theorem)

Green’s theorem converts circulation around a positively oriented planar boundary into the area integral of scalar curl.

##### Boundary formula for planar area

↑ **Parent:** [Green theorem](#green-theorem)

Apply [Green theorem](#green-theorem) with $P=-y/2$ and $Q=x/2$ to a positively oriented regular planar region. Since $Q_x-P_y=1$, its area is the displayed [line integral](#line-integral). Clockwise orientation changes the sign; holes have the opposite boundary orientation to the outer curve.

#### Line integral

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_integral)

A line integral integrates a scalar or tangential vector-field component along a curve.

#### Tensor divergence theorem

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_divergence_theorem)

Applying the divergence theorem componentwise to $T_{ij}v_i$ yields a boundary traction term and a volume contraction.

##### Integration by parts for tensor fields

↑ **Parent:** [Tensor divergence theorem](#tensor-divergence-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integration_by_parts_for_tensor_fields)

Tensor integration by parts transfers a derivative between tensor factors and introduces the boundary contraction with the outward normal.

### Jacobian matrix and determinant

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)

The [Jacobian matrix](#jacobian-matrix) collects all first [partial derivatives](#partial-derivative) of a [differentiable map](#differentiable-map). When it is square, its [Jacobian determinant](#jacobian-determinant) gives the signed local volume factor.

#### Jacobian matrix

↑ **Parent:** [Jacobian matrix and determinant](#jacobian-matrix-and-determinant)

The Jacobian matrix contains all first partial derivatives of a coordinate transformation.

##### Spatial derivative control in perturbations of the identity map

↑ **Parent:** [Jacobian matrix](#jacobian-matrix)

To deduce $Du_t=I+tDF+o(t)$ from $u_t(x)=x+tF(x)+o(t)$, the remainder must be small in a topology controlling its spatial derivatives, such as $C^1$ locally. Small displacement alone is insufficient: $u_t(x,y,z)=(x+t^2\sin(x/t^2),y,z)$ differs uniformly from the identity by $o(t)$, but has [Jacobian determinant](#jacobian-determinant) $2$ at $x=0$ for nonzero $t$. A smooth [flow map](dynamical-systems.md#flow-map) generated by a smooth [vector field](#vector-field) has the required derivative control.

##### Jacobian determinant

↑ **Parent:** [Jacobian matrix](#jacobian-matrix)

The Jacobian determinant is the [determinant](linear-algebra.md#determinant) of the square [Jacobian matrix](#jacobian-matrix). Its absolute value is the local volume-scaling factor in the [change of variables formula](#change-of-variables-formula).

The [Jacobian matrix and determinant](#jacobian-matrix-and-determinant) describe respectively the linear derivative and its signed volume factor.

###### Jacobian determinant as a divergence

↑ **Parent:** [Jacobian determinant](#jacobian-determinant)

For a smooth map $u:\mathbb R^3\to\mathbb R^3$, set $V_i=\epsilon_{ijk}\epsilon_{abc}(\partial_j u_a)(\partial_k u_b)u_c/6$. In [Einstein summation convention](linear-algebra.md#einstein-notation), applying the [product rule](#product-rule) leaves only the term differentiating $u_c$: the terms with second derivatives cancel against antisymmetry. The remaining [Levi-Civita symbol](#levi-civita-symbol) contraction is $\det Du$, so $\nabla\cdot V=J[u]$. Equivalently this vector field is one third of the cofactor matrix transposed, applied to $u$.

### Change of variables formula

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_variables_formula)

The change-of-variables formula multiplies an integral by the absolute determinant of the Jacobian.

#### Ordered-cone substitution by products and ratios

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

On $x>0$, $0<y<1$, $0<z<x$, this [change of variables](#change-of-variables-formula) is a [bijection](function.md#bijection) onto $0<\gamma<\beta<\alpha$. Its inverse is $x=\sqrt{\alpha\beta}$, $y=\sqrt{\beta/\alpha}$, $z=\gamma\sqrt{\alpha/\beta}$, and its forward [Jacobian determinant](#jacobian-determinant) is $2x$. Thus $x\,dx\,dy\,dz=\tfrac12\,d\alpha\,d\beta\,d\gamma$. Passing to increments $(\alpha-\beta,\beta-\gamma,\gamma)$ then maps the ordered cone to the positive octant, turning an exponential with linear exponent into a product of three one-dimensional [integrals](#integral).

#### Ratio-product coordinates

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

On the positive quadrant, the inverse coordinate change is $x=\sqrt{uv}$, $y=\sqrt{v/u}$. Its [Jacobian determinant](#jacobian-determinant) is $1/(2u)>0$. Regions bounded by positive constant-ratio lines and constant-product hyperbolas become rectangles in these coordinates. An integrand $x/y=u$ then cancels the Jacobian factor, making weighted area integrals particularly simple. The positivity restriction selects a unique square-root branch and fixes orientation.

#### Squared-radius difference substitution

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

In the open first quadrant this is one-to-one, with $x=\sqrt{(u+v)/2}$, $y=\sqrt{(u-v)/2}$ and [Jacobian determinant](#jacobian-determinant) $-8xy$. Its image satisfies $u>v$ and $u+v>0$. In particular $1\leq v\leq u\leq U$ is a triangular image for a circular-hyperbolic region. A factor $xy$ in the original integrand cancels the inverse-Jacobian factor $1/(8xy)$; moreover $x^4-y^4=uv$ and $4x^2y^2=u^2-v^2$. Boundary degeneracy on $y=0$ is confined to a measure-zero set and must not be confused with an interior failure of invertibility.

#### Weighted inverse multiplicity

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

For a smooth [local diffeomorphism](#local-diffeomorphism) $a:\mathbb R^d\to\mathbb R^d$, each inverse branch contributes an inverse [Jacobian determinant](#jacobian-determinant) in the [area formula](#area-formula-geometric-measure-theory). Their sum is the weighted inverse multiplicity. A lower determinant bound controls each branch separately, not the number of branches. Bounded weighted inverse multiplicity is sufficient for [dispersion with a nonlinear velocity map](partial-differential-equation.md#dispersion-with-a-nonlinear-velocity-map).

#### Rational square diffeomorphism

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

The displayed map is a [diffeomorphism](geometry-and-topology.md#diffeomorphism) of the open unit square onto itself. For fixed $u$, the second coordinate decreases strictly from one to zero as $v$ increases from zero to one. Its inverse is $u=1-x$, $v=(1-y)/[1-(1-x)y]$, and its positive [Jacobian determinant](#jacobian-determinant) is $[1-(1-x)y]^2/x$. Composing it with $(t,w)\mapsto((1-t)/(1-wt),1-w)$ gives determinant $[1-(1-x)y][1-(1-x^2)y]^2/[x(1-y)]$. The reciprocal determinant therefore integrates to one over the target square by the [change of variables formula](#change-of-variables-formula), despite boundary singularities.

#### Hyperbolic substitution

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

A hyperbolic change of integration variable uses identities such as $1+\sinh^2u=\cosh^2u$ to simplify square roots. For an [open matter-dominated Friedmann solution](cosmology.md#open-matter-dominated-friedmann-solution), $a=b\sinh^2(\eta/2)$ makes the cosmic-time integral elementary.

#### Monotone substitution inequality

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)

For a nondecreasing real function $z$ on an interval $I$ and nonnegative [measurable function](measure-theory.md#measurable-function) $h$,

$$
\int_I h(z(u))z^{\prime}(u)\,du\leq\int_{\mathbb R}h(s)\,ds.
$$

The pushforward of $z^{\prime}(u)\,du$ is dominated by [Lebesgue measure](measure-theory.md#lebesgue-measure): on each interval, the integral of the derivative is at most the increase of $z$. This handles jumps and singular parts without a smoothness assumption.

#### Area formula (geometric measure theory)

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Area_formula_(geometric_measure_theory))

For a [locally Lipschitz function](real-analysis.md#locally-lipschitz-function) $T$ between Euclidean spaces of the same dimension, the area formula integrates its absolute [Jacobian determinant](#jacobian-determinant) against the multiplicity of its fibers. In particular, for an injective $C^1$ map $T:X\to\mathbb R^d$ and nonnegative measurable $a$,

$$
\int_X a(T(x))|\det DT(x)|\,dx=\int_{T(X)}a(y)\,dy.
$$

This injective version extends the [change of variables formula](#change-of-variables-formula) to maps with a possibly singular derivative.

#### Polar coordinates

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polar_coordinates)

Polar coordinates use $x=r\cos\theta$, $y=r\sin\theta$ and area element $r\,dr\,d\theta$.

##### Cylindrical coordinate system

↑ **Parent:** [Polar coordinates](#polar-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cylindrical_coordinate_system)

The cylindrical coordinate system extends planar polar coordinates by an axial coordinate: $(x,y,z)=(R\cos\phi,R\sin\phi,z)$.

###### Azimuthal derivative of a cylindrical vector Fourier mode

↑ **Parent:** [Cylindrical coordinate system](#cylindrical-coordinate-system)

If the cylindrical components of a [vector field](#vector-field) have dependence $e^{im\phi}$, differentiation of the rotating basis adds the displayed [cross product](vector-space.md#cross-product) term. Scalar-component differentiation alone misses this contribution. For $\mathbf B=(J/2)s\widehat{\boldsymbol\phi}$, one also has $(\mathbf v\cdot\nabla)\mathbf B=(J/2)\widehat{\mathbf z}\times\mathbf v$. These identities are useful in cylindrical [magnetohydrodynamic waves](astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave).

###### Cylindrical radius

↑ **Parent:** [Cylindrical coordinate system](#cylindrical-coordinate-system)

The cylindrical radius $R=\sqrt{x^2+y^2}$ is the perpendicular distance from the symmetry axis.

##### Cardioid

↑ **Parent:** [Polar coordinates](#polar-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardioid)

A cardioid is an epicycloid with one cusp; a standard polar equation is $r=a(1+\cos\theta)$.

#### Orthogonal coordinates

↑ **Parent:** [Change of variables formula](#change-of-variables-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthogonal_coordinates)

[Orthogonal coordinates](#orthogonal-coordinates) have pairwise [orthogonal](linear-algebra.md#orthogonal-vectors) coordinate tangent directions. Their metric is diagonal, with [scale factors of orthogonal coordinates](#scale-factors-of-orthogonal-coordinates) $h_i=|\partial\mathbf x/\partial q_i|$. [Spherical coordinates](#spherical-coordinate-system) and cylindrical coordinates are examples.

##### Del in cylindrical and spherical coordinates

↑ **Parent:** [Orthogonal coordinates](#orthogonal-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Del_in_cylindrical_and_spherical_coordinates)

This collects the [gradient](#gradient), [divergence](#divergence), [curl](#curl) and [Laplacian](#laplacian) formulas in cylindrical and [spherical coordinates](#spherical-coordinate-system). Coordinate [unit vectors](vector-space.md#unit-vector) vary with position, so taking their derivatives is essential when translating [vector calculus](#vector-calculus) operators from Cartesian coordinates. [Curl in spherical coordinates](#curl-in-spherical-coordinates) is one of these formulas.

##### Hyperspherical coordinates

↑ **Parent:** [Orthogonal coordinates](#orthogonal-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperspherical_coordinates)

Hyperspherical coordinates extend polar coordinates to $n$ dimensions with one radius and $n-1$ angles.

###### Spherical coordinate system

↑ **Parent:** [Hyperspherical coordinates](#hyperspherical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spherical_coordinate_system)

Spherical coordinates $(r,\theta,\phi)$ in $\mathbb R^3$ use

$$
(x,y,z)=(r\sin\theta\cos\phi,r\sin\theta\sin\phi,r\cos\theta).
$$

###### Radial unit vector in spherical coordinates

↑ **Parent:** [Spherical coordinate system](#spherical-coordinate-system)

At fixed angular coordinates, differentiating the [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) with respect to radial distance gives this [unit vector](vector-space.md#unit-vector). It is the local direction of increasing radius in the [spherical coordinate system](#spherical-coordinate-system).

###### Scale factors of orthogonal coordinates

↑ **Parent:** [Spherical coordinate system](#spherical-coordinate-system)

If orthogonal coordinates $q_i$ satisfy

$$
d\mathbf x=\sum_i h_i\mathbf e_i\,dq_i,
$$

then $h_i=|\partial\mathbf x/\partial q_i|$ are their scale factors.

These factors determine the diagonal metric and volume element of [orthogonal coordinates](#orthogonal-coordinates).

###### Curl in spherical coordinates

↑ **Parent:** [Spherical coordinate system](#spherical-coordinate-system)

For $\mathbf A=A_r\mathbf e_r+A_\theta\mathbf e_\theta+A_\phi\mathbf e_\phi$, the spherical-coordinate curl follows from the orthogonal-coordinate scale factors $1,r,r\sin\theta$.

Its coordinate expression is part of [del in cylindrical and spherical coordinates](#del-in-cylindrical-and-spherical-coordinates).

###### Volume of an n-ball

↑ **Parent:** [Hyperspherical coordinates](#hyperspherical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_of_an_n-ball)

The radius-$R$ ball in $\mathbb R^n$ has volume $\pi^{n/2}R^n/\Gamma(n/2+1)$.

###### Surface area of an n-sphere

↑ **Parent:** [Hyperspherical coordinates](#hyperspherical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_area_of_an_n-sphere)

The boundary of the radius-$R$ ball has area $2\pi^{n/2}R^{n-1}/\Gamma(n/2)$.

### Differentiable map

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)

A map is differentiable at $x$ when it differs from an affine map with linear part $Df_x$ by $o(\lVert h\rVert)$ at $x+h$.

#### Functionally independent functions

↑ **Parent:** [Differentiable map](#differentiable-map)

Functions whose [differentials](differential-geometry.md#differential-of-a-smooth-map) are [linearly independent](vector-space.md#linear-independence) at the point in question. For $F=(F_1,\ldots,F_r)$ this means the derivative has rank $r$, so $F$ is a [submersion](differential-geometry.md#submersion) there. The condition is open. It is distinct from global [algebraic independence](algebra.md#algebraic-independence) of functions.

#### Derivative of a map into a level set

↑ **Parent:** [Differentiable map](#differentiable-map)

If a [differentiable map](#differentiable-map) $F$ takes values in a level set of a differentiable scalar function $H$, the [chain rule](#chain-rule) gives $DH_{F(x)}DF_x=0$. At a regular point, the image of the [derivative](#derivative) lies in the kernel of the nonzero covector $DH$: the tangent space of the level set. For a map into the unit circle this forces rank at most one.

<h4 id="frechet-derivative">Fréchet derivative</h4>

↑ **Parent:** [Differentiable map](#differentiable-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fréchet_derivative)

The Frechet derivative of $f$ at $a$ is the unique [linear map](vector-space.md#linear-map) $Df_a$ such that

$$
\frac{\lVert f(a+h)-f(a)-Df_a(h)\rVert}{\lVert h\rVert}\to0.
$$

##### Differentiability under equivalent norms

↑ **Parent:** [Fréchet derivative](#frechet-derivative)

Suppose $f(a+h)=f(a)+Lh+r(h)$ and $|r(h)|/\|h\|_1\to0$. If $c\|h\|_1\le\|h\|_2\le C\|h\|_1$, then $|r(h)|/\|h\|_2\le c^{-1}|r(h)|/\|h\|_1\to0$. The boundedness of $L$ is also preserved, and the same argument in reverse proves equivalence of differentiability. The [derivative](#derivative) is the same [linear map](vector-space.md#linear-map), not a [norm](functional-analysis.md#norm)-dependent replacement.

##### Hadamard differentiability

↑ **Parent:** [Fréchet derivative](#frechet-derivative)

A map on a subset of a [normed vector space](functional-analysis.md#normed-vector-space) is [Hadamard differentiable](#hadamard-differentiability) at $s$ if its directional difference quotients converge to a [continuous linear map](topological-vector-space.md#continuous-linear-operator) uniformly along all convergent sequences of directions: $t_j\to0$, $a_j\to a$, and $s+t_ja_j$ in the domain imply $(\Phi(s+t_ja_j)-\Phi(s))/t_j\to\dot\Phi_s(a)$. Tangential differentiability restricts the limit directions to a specified subspace. This is the regularity used by the [functional delta method](statistical-inference.md#functional-delta-method).

###### Hadamard remainder near a compact set

↑ **Parent:** [Hadamard differentiability](#hadamard-differentiability)

For a [Hadamard differentiable](#hadamard-differentiability) functional with continuous linear derivative $L$, define $R_t(h)=(\Phi(s+th)-\Phi(s))/t-L(h)$. For every compact $K$ and positive $\epsilon$, some positive $\delta,a$ make $|R_t(h)|<\epsilon$ whenever $\operatorname{dist}(h,K)<\delta$ and $0<|t|<a$. If this failed, choose $t_j\to0$, directions within $1/j$ of $K$ and remainders at least $\epsilon$. Compactness gives a convergent subsequence of nearby points of $K$, hence convergent directions. The derivative definition and continuity of $L$ give remainder tending to zero, a contradiction. With a tight weak limit, the [Portmanteau theorem](convergence-of-random-variables.md#portmanteau-theorem) makes random directions lie near a suitable compact set with arbitrarily large probability. Thus this lemma proves the [functional delta method](statistical-inference.md#functional-delta-method) without assuming separability of the entire normed space or uniform differentiability on its whole unit ball.

###### Stieltjes bilinear functional under a variation constraint

↑ **Parent:** [Hadamard differentiability](#hadamard-differentiability)

On bounded continuously differentiable functions with uniformly bounded [total variation of a function](real-analysis.md#total-variation-of-a-function), the map $T$ is [Hadamard differentiable](#hadamard-differentiability) in the [supremum norm](functional-analysis.md#supremum-norm) with [derivative](#derivative) $\dot T_{F,G}(a,b)=\int_0^ubF^{\prime}+G(u)a(u)-G(0)a(0)-\int_0^uG^{\prime}a$. Use [weak convergence of bounded-variation integrators](real-analysis.md#weak-convergence-of-bounded-variation-integrators) for the first term and [integration by parts](#integration-by-parts) for the remaining terms. No [derivatives](#derivative) of the limiting continuous directions are required.

<h5 id="frechet-differentiability">Fréchet differentiability</h5>

↑ **Parent:** [Fréchet derivative](#frechet-derivative)

A map is [Fréchet differentiable](#frechet-differentiability) at $x$ if it admits a bounded linear first-order approximation: $f(x+h)=f(x)+Ah+o(\|h\|)$ for a [continuous linear map](topological-vector-space.md#continuous-linear-operator) $A$.

##### Derivative of matrix inversion

↑ **Parent:** [Fréchet derivative](#frechet-derivative)

On the open set of invertible square matrices, the inversion map is [differentiable](#differentiable-map) and

$$
D(A\mapsto A^{-1})_A[H]=-A^{-1}HA^{-1}.
$$

#### Continuously differentiable function

↑ **Parent:** [Differentiable map](#differentiable-map)

A function is continuously differentiable when its derivative exists and varies continuously.

#### Invertible linear map

↑ **Parent:** [Differentiable map](#differentiable-map)

An invertible linear map is a linear bijection; its inverse is also linear.

Invertibility adds a [bijection](function.md#bijection) requirement to the definition of a [linear map](vector-space.md#linear-map).

#### Mean value inequality

↑ **Parent:** [Differentiable map](#differentiable-map)

If the line segment from $x$ to $y$ lies in the domain of a differentiable map and $\lVert Df_z\rVert\leq M$ along it, then

$$
\lVert f(y)-f(x)\rVert\leq M\lVert y-x\rVert.
$$

##### Zero derivative on a connected open set

↑ **Parent:** [Mean value inequality](#mean-value-inequality)

A differentiable map on a connected open subset of Euclidean space whose derivative vanishes everywhere is constant. The [mean value inequality](#mean-value-inequality) makes it constant on every ball in the domain, hence locally constant; connectedness then makes the value global.

#### Inverse function theorem

↑ **Parent:** [Differentiable map](#differentiable-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_function_theorem)

If a continuously differentiable map has invertible derivative at a point, it is a local continuously differentiable diffeomorphism there.

##### Constant rank theorem

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constant_rank_theorem)

If a smooth map has constant rank $r$ near a point, there are local coordinates in which it is

$$
(x^1,\ldots,x^m)\longmapsto(x^1,\ldots,x^r,0,\ldots,0).
$$

###### Rank-one level curves from a characteristic differential equation

↑ **Parent:** [Constant rank theorem](#constant-rank-theorem)

For a smooth map $F=(f,g)$ on the plane with zero Jacobian determinant and $f_y\ne0$, set $e=g_y/f_y$. The determinant identity gives $\nabla g=e\nabla f$. Along a curve solving $y'=-f_x/f_y$, both $f$ and $g$ have zero derivative. Local existence and uniqueness for this smooth differential equation through every nearby point produce a local foliation by curves of constant $F$.

##### Local diffeomorphism

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_diffeomorphism)

A local diffeomorphism restricts near every point to a diffeomorphism onto an open subset. In particular, every local diffeomorphism is an open map.

###### Noninjective map with constant Jacobian determinant

↑ **Parent:** [Local diffeomorphism](#local-diffeomorphism)

The displayed [smooth map](differential-geometry.md#smooth-map-between-manifolds) from $\mathbb R^2$ to the punctured plane has [Jacobian determinant](#jacobian-determinant) one: in [polar coordinates](#polar-coordinates) its radius is $e^s$ and its angle is $re^{-2s}$, so the determinant is $e^{2s}e^{-2s}=1$. Nevertheless $a(0,2\pi k)=(1,0)$ for every integer $k$. Thus a local volume-preserving map need not be injective or have bounded [weighted inverse multiplicity](#weighted-inverse-multiplicity). Compactly supported data distributed over many inverse branches disprove a determinant-only [dispersion with a nonlinear velocity map](partial-differential-equation.md#dispersion-with-a-nonlinear-velocity-map) estimate.

###### Open map

↑ **Parent:** [Local diffeomorphism](#local-diffeomorphism)

An open map sends every open set to an open set.

Together, [open and closed maps](topology.md#open-and-closed-maps) describe the two image-set preservation properties.

##### Implicit function theorem

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_function_theorem)

If $F(x_0,y_0)=0$ and the partial derivative with respect to $y$ is invertible at $(x_0,y_0)$, then the nearby zero set is the graph $y=g(x)$ of a continuously differentiable function.

###### Holomorphic implicit function theorem

↑ **Parent:** [Implicit function theorem](#implicit-function-theorem)

If a holomorphic function $F(z,w)$ satisfies $F(z_0,w_0)=0$ and $F_w(z_0,w_0)\ne0$, then near $(z_0,w_0)$ its zero set is the graph $w=g(z)$ of a unique holomorphic function. The analogous statement with $F_z\ne0$ uses $w$ as the local coordinate.

###### Implicit differentiation

↑ **Parent:** [Implicit function theorem](#implicit-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_differentiation)

Implicit differentiation differentiates an identity $F(x,y(x))=0$ and uses the [chain rule](#chain-rule) to solve for derivatives of the implicitly defined function. In one dimension, $y'=-F_x/F_y$ when $F_y\ne0$.

###### Cyclic partial derivative identity

↑ **Parent:** [Implicit differentiation](#implicit-differentiation)

On a [level set](topology.md#level-set) $f(x,y,z)=c$, [implicit differentiation](#implicit-differentiation) gives the three ratios $-f_y/f_x$, $-f_z/f_y$ and $-f_x/f_z$. Their product is $-1$ wherever all the required coordinate representations are differentiable with nonzero denominators. At coordinate singularities the quotient product need not be defined.

## Symmetry in integration

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetry_in_integration)

If an integrand is odd under a measure-preserving symmetry of the domain, its integral is zero.

## Integration by parts

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integration_by_parts)

Integration by parts is the integrated product rule: $\int u\,dv=uv-\int v\,du$.

### Boundary term

↑ **Parent:** [Integration by parts](#integration-by-parts)

A boundary term is an endpoint or boundary integral left when derivatives are transferred by [integration by parts](#integration-by-parts). It vanishes under some boundary conditions and otherwise supplies natural boundary conditions, conserved charges, or physical surface forces.

## Hyperbolic tangent

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_tangent)

The hyperbolic tangent is sinh divided by cosh and approaches plus or minus one at the two infinities.

### Inverse hyperbolic tangent

↑ **Parent:** [Hyperbolic tangent](#hyperbolic-tangent)

For $|x|<1$, the inverse hyperbolic tangent is

$$
\operatorname{artanh}x=\frac12\log\frac{1+x}{1-x}.
$$

### Small-argument expansion of the hyperbolic tangent

↑ **Parent:** [Hyperbolic tangent](#hyperbolic-tangent)

The [taylor series](#taylor-series) at zero begins

$$
\tanh x=x-\frac{x^3}{3}+O(x^5),
$$

so $\tanh x\sim x$ as $x\to0$.

### Hyperbolic-function identity

↑ **Parent:** [Hyperbolic tangent](#hyperbolic-tangent)

The exponential definitions of the hyperbolic functions imply identities such as

$$
\frac{\sinh x}{1+\cosh x}=\tanh\!\left(\frac x2\right).
$$

### Hyperbolic Pythagorean identity

↑ **Parent:** [Hyperbolic tangent](#hyperbolic-tangent)

The identity $\cosh^2x-\sinh^2x=1$ implies

$$
1-\tanh^2x=\operatorname{sech}^2x,
\qquad
\coth^2x-\operatorname{csch}^2x=1.
$$

The identity follows directly from the exponential definitions of the [hyperbolic functions](#hyperbolic-function).

## Even function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Even_function)

An even function satisfies $f(-x)=f(x)$; its [Laurent series](analysis.md#laurent-series) or [taylor series](#taylor-series) contains only even powers.

## Odd function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Odd_function)

An odd function satisfies $f(-x)=-f(x)$; its [Laurent series](analysis.md#laurent-series) or [taylor series](#taylor-series) contains only odd powers.

### Odd extension

↑ **Parent:** [Odd function](#odd-function)

An odd extension of a function $f$ on the positive half-line is $\widetilde f(r)=f(r)$ for $r>0$ and $\widetilde f(r)=-f(-r)$ for $r<0$. At zero it is set to zero when the boundary value is zero. Smoothness requires compatible even derivatives at zero. In the [radial reduction of the three-dimensional wave equation](wave-equation.md#radial-reduction-of-the-three-dimensional-wave-equation), $r\phi(t,r)$ has a smooth [odd extension](#odd-extension) whenever $\phi$ is smooth and radial.

## ↑ Ancestors (5)

1. [Real analysis](real-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
