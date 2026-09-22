# Calculus

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Calculus)

Calculus connects **local change** with **accumulated change**. A [derivative](#derivative) asks how fast a [function](function.md) changes near one input; an [integral](#integral) adds its contributions across an [interval](real-analysis.md#interval-mathematics). The [fundamental theorem of calculus](#fundamental-theorem-of-calculus) explains why these operations fit together: accumulating a continuous rate produces a quantity whose [derivative](#derivative) is that rate.

For example, suppose a particle moves along a [straight line](geometry-and-topology.md#straight-line) with [position](classical-mechanics.md#position) $s(t)=t^2+t$ metres at time $t$ seconds. Its [velocity](classical-mechanics.md#velocity) is $s'(t)=2t+1$ metres per second. Between $t=0$ and $t=3$, adding the [velocity](classical-mechanics.md#velocity) over time gives

$$
\int_0^3(2t+1)\,dt=s(3)-s(0)=12\text{ metres}.
$$

Here the [velocity](classical-mechanics.md#velocity) stays positive, so the [displacement](classical-mechanics.md#displacement) also equals the distance travelled. If the particle reverses direction, the [integral](#integral) of its signed [velocity](classical-mechanics.md#velocity) still gives [displacement](classical-mechanics.md#displacement), while the [integral](#integral) of its [speed](classical-mechanics.md#speed) gives total distance.

This is useful because local rules are often easier to specify than whole trajectories. A [differential equation](differential-equation.md) can prescribe a particle's [velocity](classical-mechanics.md#velocity) or a population's growth rate; [integration](#integral) then reconstructs its evolution, subject to an [initial condition](differential-equation.md#initial-condition). In the other direction, a [derivative](#derivative) extracts local information from a known [function](function.md), and [optimization](mathematical-optimization.md) uses that information to locate or approach promising inputs. The same two operations therefore connect measurement, prediction and design.

The visual connection is developed in [derivative](#derivative), [integral](#integral) and [fundamental theorem of calculus](#fundamental-theorem-of-calculus). The definitions depend on [limits](#limit-of-a-function), which turn progressively finer finite measurements into exact mathematical statements. A graph with a corner need not have a [derivative](#derivative) there, and the conditions permitting [integration](#integral) or interchange of [limits](#limit-of-a-function) matter; calculus is more than a collection of symbolic rules.

Historically, Isaac Newton described changing quantities and their rates in the language of fluents and fluxions; his manuscript _History of the Method of Fluxions_ records that approach.[Isaac Newton, History of the Method of Fluxions, Cambridge University Library MS Add. 3968](https://www.newtonproject.ox.ac.uk/view/texts/normalized/NATP00356) Gottfried Wilhelm Leibniz's _Nova methodus pro maximis et minimis_ appeared in _Acta Eruditorum_ in October 1684, pp. 467–473; the original article is preserved in the HKUST Library collection.[Gottfried Wilhelm Leibniz, Nova methodus pro maximis et minimis, 1684](https://digitalcollections.hkust.edu.hk/Detail/objects/b540295) The modern [limit](#limit-of-a-function) definitions used here should not be read back into those seventeenth-century formulations.

**Table of contents**

- [Differential calculus](#differential-calculus)
- [Floor and ceiling functions](#floor-and-ceiling-functions)
  - [Integer count in a closed interval](#integer-count-in-a-closed-interval)
  - [Floor function](#floor-function)
    - [Fractional part](#fractional-part)
  - [Ceiling function](#ceiling-function)
    - [Ceiling count for fixed-size batches](#ceiling-count-for-fixed-size-batches)
  - [Truncation toward zero](#truncation-toward-zero)
- [Integral](#integral)
  - [Average value of a function](#average-value-of-a-function)
  - [Linearity of integration](#linearity-of-integration)
  - [Signed area under a graph](#signed-area-under-a-graph)
    - [Total geometric area under a graph](#total-geometric-area-under-a-graph)
  - [Definite integral](#definite-integral)
    - [Distance traveled from velocity](#distance-traveled-from-velocity)
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
      - [Antiderivatives on disconnected domains](#antiderivatives-on-disconnected-domains)
    - [Additive constant](#additive-constant)
  - [Gaussian integral](#gaussian-integral)
    - [Polar-coordinate proof of the Gaussian integral](#polar-coordinate-proof-of-the-gaussian-integral)
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
  - [Exponential growth](#exponential-growth)
    - [Doubling time](#doubling-time)
  - [e (mathematical constant)](#e-mathematical-constant)
    - [Compounding limit for e](#compounding-limit-for-e)
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
    - [Logarithmic scale](#logarithmic-scale)
    - [Logarithm inequality](#logarithm-inequality)
    - [Operator monotonicity of logarithm](#operator-monotonicity-of-logarithm)
  - [Gaussian function](#gaussian-function)
    - [Gaussian decay dominates every power](#gaussian-decay-dominates-every-power)
    - [Gaussian dyadic summation bound](#gaussian-dyadic-summation-bound)
  - [Hyperbolic function](#hyperbolic-function)
    - [Hyperbolic angle](#hyperbolic-angle)
    - [Inverse hyperbolic functions](#inverse-hyperbolic-functions)
    - [Hyperbolic cosine](#hyperbolic-cosine)
      - [Catenary from hyperbolic cosine](#catenary-from-hyperbolic-cosine)
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
- [Taylor's theorem](#taylor-s-theorem)
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
    - [Maclaurin series](#maclaurin-series)
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
      - [Intermediate value theorem hypotheses and counterexamples](#intermediate-value-theorem-hypotheses-and-counterexamples)
      - [A cubic root from existence to a quantitative bracket](#a-cubic-root-from-existence-to-a-quantitative-bracket)
      - [Nested-bracket proof of the intermediate value theorem](#nested-bracket-proof-of-the-intermediate-value-theorem)
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
  - [Local linear approximation](#local-linear-approximation)
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
    - [Linear approximation](#linear-approximation)
    - [Multivariable chain rule](#multivariable-chain-rule)
      - [Derivative along a curve](#derivative-along-a-curve)
    - [Nondifferentiable inner function with a differentiable nondegenerate composite](#nondifferentiable-inner-function-with-a-differentiable-nondegenerate-composite)
    - [Second derivative chain rule](#second-derivative-chain-rule)
- [Monotonic function](#monotonic-function)
  - [Derivative criterion for monotonicity](#derivative-criterion-for-monotonicity)
  - [Monotone mean-value point of an integral average](#monotone-mean-value-point-of-an-integral-average)
  - [Nonincreasing function](#nonincreasing-function)
  - [Non-strict inverse of a continuous nondecreasing function](#non-strict-inverse-of-a-continuous-nondecreasing-function)
  - [Left-continuous cumulative function of an atomic measure](#left-continuous-cumulative-function-of-an-atomic-measure)
  - [Nondecreasing function](#nondecreasing-function)
  - [Strict generalized inverse of a nondecreasing function](#strict-generalized-inverse-of-a-nondecreasing-function)
  - [Strictly increasing function](#strictly-increasing-function)
    - [Continuity of an increasing interval surjection](#continuity-of-an-increasing-interval-surjection)
  - [Strictly decreasing function](#strictly-decreasing-function)
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
    - [Vector Analysis (book)](#vector-analysis-book)
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
      - [Derivative of a local inverse map](#derivative-of-a-local-inverse-map)
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

## Differential calculus

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_calculus)

[Differential calculus](#differential-calculus) studies [derivatives](#derivative): how a [function](function.md) changes near an input and how that local information describes its graph or evolution. Its tools include [linear approximation](#linear-approximation), higher [derivatives](#derivative), and [Taylor series](#taylor-series); applications include finding [velocity](classical-mechanics.md#velocity) from [position](classical-mechanics.md#position) and studying [optimization](mathematical-optimization.md) through [critical points](analysis.md#critical-point).

## Floor and ceiling functions

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Floor_and_ceiling_functions)

The [floor function](#floor-function) and [ceiling function](#ceiling-function) turn a [real number](arithmetic.md#real-number) into directed [integer](number-theory.md#integer) bounds. They answer two different questions: which [integer](number-theory.md#integer) is the largest one that does not exceed $x$, and which is the smallest one that is not less than $x$?

$$
\lfloor x\rfloor\leq x<\lfloor x\rfloor+1,\qquad
\lceil x\rceil-1<x\leq\lceil x\rceil.
$$

Both outputs are [integers](number-theory.md#integer). These are exact mathematical operations; they need not choose the closest [integer](number-theory.md#integer), and they do not refer to [roundoff error](numerical-analysis.md#round-off-error) in [floating-point arithmetic](numerical-analysis.md#floating-point-arithmetic).

For example,

$$
\begin{array}{c|r|r|r}
x&\lfloor x\rfloor&\lceil x\rceil&\{x\}\\\hline
2.7&2&3&0.7\\
2&2&2&0\\
-2.7&-3&-2&0.3\\
-2&-2&-2&0
\end{array}
$$

The [fractional part](#fractional-part) is $\{x\}=x-\lfloor x\rfloor$. The negative example matters: discarding the digits after the decimal point would give $-2$, which is [truncation toward zero](#truncation-toward-zero), rather than the [floor function](#floor-function)'s value $-3$. At an [integer](number-theory.md#integer), the [floor function](#floor-function) and [ceiling function](#ceiling-function) agree and the [fractional part](#fractional-part) vanishes.

<a id="image-floor-and-ceiling-give-enclosing-integers-fractional-part-repeats-on-each-unit-interval"></a>
![](floor-ceiling-and-fractional-part.png)

**[Figure 1](#image-floor-and-ceiling-give-enclosing-integers-fractional-part-repeats-on-each-unit-interval). Floor and ceiling give enclosing integers; fractional part repeats on each unit interval**.

The usefulness is a bridge from continuous quantities to discrete decisions. An [integer count in a closed interval](#integer-count-in-a-closed-interval) uses both bounds. A [ceiling count for fixed-size batches](#ceiling-count-for-fixed-size-batches) counts how many containers or pages are needed; a [floor function](#floor-function) counts how many complete groups fit. In [Euclidean division](number-theory.md#euclidean-division), the same bounds specify the quotient, while the [fractional part](#fractional-part) records the scaled [remainder](number-theory.md#remainder). A small amount of notation removes many cases that would otherwise have to be stated separately.

The reflection identity

$$
\lceil x\rceil=-\lfloor-x\rfloor
$$

follows by reflecting the ordered [integers](number-theory.md#integer) across zero: the largest one below $-x$ becomes the smallest one above $x$. For every [integer](number-theory.md#integer) $m$, translation gives $\lfloor x+m\rfloor=\lfloor x\rfloor+m$ and $\lceil x+m\rceil=\lceil x\rceil+m$. These formulas turn upper bounds into lower bounds and move examples between neighboring [intervals](real-analysis.md#interval-mathematics).

For a historical example of the notation in use, Kenneth E. Iverson's 1962 conference paper _A Programming Language_ lists the [floor function](#floor-function), [ceiling function](#ceiling-function) and residue operation alongside the ordinary [arithmetic operations](numerical-analysis.md#arithmetic-operation). It states the two defining inequalities above, then extends operations component by component to [vectors](vector-space.md#vector) and [matrices](vector-space.md#matrix). This shows their role as tools for describing [algorithms](computer-science.md#algorithm), rather than merely conventions for writing decimal numbers. [Iverson, A Programming Language, AFIPS Spring Joint Computer Conference, May 1962, Basic Operations; transcription with typography changes documented at the end](https://www.jsoftware.com/papers/AFIPS196205a.htm)

### Integer count in a closed interval

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

For [real numbers](arithmetic.md#real-number) $a\leq b$, the [integers](number-theory.md#integer) in the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$ begin at $\lceil a\rceil$ and end at $\lfloor b\rfloor$, if there are any. Their number is therefore

$$
|[a,b]\cap\mathbb Z|=\max\!\left(0,\lfloor b\rfloor-\lceil a\rceil+1\right).
$$

The extra one includes both ends of the resulting [integer interval](number-theory.md#integer-interval). The [maximum](set.md#maximum-of-a-subset-of-a-total-order) with zero handles an empty [intersection](set.md#set-intersection): $[0.2,0.8]$ contains no [integer](number-theory.md#integer), even though it has positive length.

For $[-2.7,1.1]$, the [ceiling function](#ceiling-function) selects $-2$ and the [floor function](#floor-function) selects $1$, giving $1-(-2)+1=4$. The four points are $-2,-1,0,1$. For $[-2,2]$, the count is five, not four: the real length $2-(-2)$ and the number of [integer](number-theory.md#integer) points are different quantities.

The endpoint convention matters. For the half-open [interval](real-analysis.md#interval-mathematics) $[a,b)$ with $a\leq b$, the last allowed [integer](number-theory.md#integer) is $\lceil b\rceil-1$, so the count becomes $\max(0,\lceil b\rceil-\lceil a\rceil)$. This handles an [integer](number-theory.md#integer) endpoint $b$ without including it accidentally. For example, $[-2,2)$ has four [integer](number-theory.md#integer) points.

### Floor function

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

The floor $\lfloor x\rfloor$ is the greatest [integer](number-theory.md#integer) not exceeding the [real number](arithmetic.md#real-number) $x$. Equivalently, $\lfloor x\rfloor=m$ exactly when $m\leq x<m+1$, for an [integer](number-theory.md#integer) $m$. The [floor function](#floor-function) is constant on each such half-open [interval](real-analysis.md#interval-mathematics) and has a [discontinuity of a function](#discontinuity-of-a-function) at each [integer](number-theory.md#integer).

For nonnegative [integers](number-theory.md#integer) $N$ and positive [integers](number-theory.md#integer) $k$, $\lfloor N/k\rfloor$ is the number of complete groups of size $k$ that fit into $N$ items. With $N=102$ and $k=20$, five complete groups use 100 items. [Euclidean division](number-theory.md#euclidean-division) writes $102=20\cdot5+2$, retaining the two-item [remainder](number-theory.md#remainder) rather than treating the [quotient](arithmetic.md#quotient) $102/20=5.1$ as a number of complete groups.

#### Fractional part

↑ **Parent:** [Floor function](#floor-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fractional_part)

The fractional part of a [real number](arithmetic.md#real-number) is

$$
\{x\}=x-\lfloor x\rfloor\in[0,1).
$$

It is the amount left after removing the lower enclosing [integer](number-theory.md#integer), even for negative inputs. Thus $\{-2.7\}=-2.7-(-3)=0.3$. It is not the signed string of digits obtained by [truncation toward zero](#truncation-toward-zero).

Translation by an [integer](number-theory.md#integer) leaves the [fractional part](#fractional-part) unchanged: $\{x+m\}=\{x\}$. It is therefore a [periodic function](function.md#periodic-function) with period one, increasing from zero toward one on each unit [interval](real-analysis.md#interval-mathematics), then returning to zero at the next [integer](number-theory.md#integer). In [Euclidean division](number-theory.md#euclidean-division) $N=kq+r$ with $0\leq r<k$, $\{N/k\}=r/k$; for $102/20$, this is $2/20=0.1$.

The notation is useful for following repeated motion modulo an [integer](number-theory.md#integer). In [normality and equidistribution under integer multiplication](number-theory.md#normality-and-equidistribution-under-integer-multiplication), the values $\{K^n x\}$ shift the digits of a [positional notation](number-theory.md#positional-notation); the [fractional part](#fractional-part) discards the leading [integer](number-theory.md#integer) portion without losing the remaining digits. Its braces must be distinguished by context from the braces denoting a [set](set.md).

### Ceiling function

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

The ceiling function gives the least [integer](number-theory.md#integer) large enough to meet a real lower bound. For a [real number](arithmetic.md#real-number) $x$,

$$
\lceil x\rceil=m\quad\Longleftrightarrow\quad m-1<x\leq m,\qquad m\in\mathbb Z.
$$

Thus $\lceil2.7\rceil=3$, $\lceil-2.7\rceil=-2$, and $\lceil2\rceil=2$. The operation rounds upward in the [total order](set.md#total-order) on the [real numbers](arithmetic.md#real-number), which can move a negative input towards zero. Its difference from the input obeys $0\leq\lceil x\rceil-x<1$. Python's `math.ceil` implements this least-integer definition. [Python 3.14 math.ceil documentation: the least integer at least x](https://docs.python.org/3.14/library/math.html#math.ceil).

The [ceiling count for fixed-size batches](#ceiling-count-for-fixed-size-batches) is a direct application. Suppose each box holds at most $k$ items, with positive [integer](number-theory.md#integer) $k$, and there are $N\geq0$ items. The smallest number of boxes with enough capacity is $\lceil N/k\rceil$: a candidate count $b$ must satisfy $bk\geq N$. For $N=101$, $k=20$, **six boxes are needed**, leaving $120-101=19$ unused places. Exactly 100 items need only five boxes, and zero items need zero boxes. Adding one to the [floor function](#floor-function) result unconditionally would therefore overcount at exact multiples of $k$.

<a id="image-the-ceiling-function-retains-the-endpoint-on-the-left-and-counts-enough-whole-containers"></a>
![](ceiling-function-thresholds-and-capacity.png)

**[Figure 2](#image-the-ceiling-function-retains-the-endpoint-on-the-left-and-counts-enough-whole-containers). The ceiling function retains the endpoint on the left and counts enough whole containers**. Left: open and filled endpoints distinguish the half-open [intervals](real-analysis.md#interval-mathematics) $(m-1,m]$ where $\lceil x\rceil=m$, including negative inputs. Right: the original capacity example uses 20 items per box; 101 items need six boxes, while an exact multiple of 20 needs no extra box. The right-hand inputs are integer item counts.

For nonnegative [integer](number-theory.md#integer) $N$ and positive [integer](number-theory.md#integer) $k$, [Euclidean division](number-theory.md#euclidean-division) gives the exact identity

$$
\boxed{\left\lceil\frac Nk\right\rceil=\left\lfloor\frac{N+k-1}{k}\right\rfloor.}
$$

Write $N=qk+r$, $0\leq r<k$. The count is $q$ when the [remainder](number-theory.md#remainder) is zero and $q+1$ otherwise, and the right-hand side encodes these two cases. This argument specifies the domain of the identity; arbitrary negative denominators require their own sign conventions.

The [ceiling function](#ceiling-function) is a [nondecreasing function](#nondecreasing-function), constant on each of the half-open [intervals](real-analysis.md#interval-mathematics) $(m-1,m]$, and has a [discontinuity of a function](#discontinuity-of-a-function) at every [integer](number-theory.md#integer). It is tied to the [floor function](#floor-function) by $\lceil x\rceil=-\lfloor-x\rfloor$. Adding an [integer](number-theory.md#integer) $j$ shifts its output by the same amount: $\lceil x+j\rceil=\lceil x\rceil+j$. At an [integer](number-theory.md#integer) the floor and ceiling agree; at every other input they differ by one. These statements refer to exact [real numbers](arithmetic.md#real-number); an input already perturbed by [floating-point arithmetic](numerical-analysis.md#floating-point-arithmetic) can land on the other side of a threshold.

#### Ceiling count for fixed-size batches

↑ **Parent:** [Ceiling function](#ceiling-function)

Suppose $N$ is a nonnegative [integer](number-theory.md#integer) count of items and each batch holds at most $k$ items, where $k$ is a positive [integer](number-theory.md#integer). The smallest sufficient number of batches is

$$
b=\left\lceil\frac Nk\right\rceil.
$$

Indeed, $bk\geq N$ exactly when the [integer](number-theory.md#integer) $b$ is at least $N/k$. If $N=0$, no batches are needed. If $N$ is a multiple of $k$, no partly filled batch is needed.

For $102$ items with capacity $20$ per batch, $b=\lceil5.1\rceil=6$. Five batches can be full and the sixth holds two items, leaving $6\cdot20-102=18$ unused places. This is a different question from the five complete groups counted by $\lfloor102/20\rfloor$.

<a id="image-endpoint-aware-integer-counts-and-six-twenty-place-batches-needed-for-102-items"></a>
![](integer-interval-and-batch-counts.png)

**[Figure 3](#image-endpoint-aware-integer-counts-and-six-twenty-place-batches-needed-for-102-items). Endpoint-aware integer counts and six twenty-place batches needed for 102 items**.

Writing the [Euclidean division](number-theory.md#euclidean-division) $N=kq+r$, $0\leq r<k$, gives the equivalent rule $b=q$ when $r=0$, and $b=q+1$ when $r>0$. This explains the [ceiling function](#ceiling-function)'s jump: one extra item beyond a complete multiple demands a whole additional batch. For exact [integer arithmetic](arithmetic.md#integer-arithmetic), the identity $b=\lfloor(N+k-1)/k\rfloor$ avoids a fractional intermediate value; an implementation still needs an [integer](number-theory.md#integer) representation large enough to hold $N+k-1$.

### Truncation toward zero

↑ **Parent:** [Floor and ceiling functions](#floor-and-ceiling-functions)

Truncation toward zero removes the fractional magnitude of a [real number](arithmetic.md#real-number), giving the [integer](number-theory.md#integer) obtained by applying the [floor function](#floor-function) to its [absolute value](real-analysis.md#absolute-value) and restoring the original sign; a magnitude below one gives zero. More precisely,

$$
\operatorname{trunc}(x)=\begin{cases}\lfloor x\rfloor&x\geq0,\\\lceil x\rceil&x<0.\end{cases}
$$

The result is zero for $-1<x<1$. For example, $\operatorname{trunc}(2.7)=2$ and $\operatorname{trunc}(-2.7)=-2$, whereas $\lfloor-2.7\rfloor=-3$. Python's `math.trunc` uses this towards-zero convention, so replacing it by `math.floor` changes calculations with negative noninteger inputs. [Python 3.14 math.trunc documentation: floor on positive inputs, ceiling on negative inputs](https://docs.python.org/3.14/library/math.html#math.trunc).

<a id="image-truncation-toward-zero-is-symmetric-in-sign-while-the-fractional-part-defined-by-the-floor-function-is-always-nonnegative"></a>
![](truncation-toward-zero-and-signed-errors.png)

**[Figure 4](#image-truncation-toward-zero-is-symmetric-in-sign-while-the-fractional-part-defined-by-the-floor-function-is-always-nonnegative). Truncation toward zero is symmetric in sign, while the fractional part defined by the floor function is always nonnegative**. Left: exact integer endpoint values distinguish the two sign-dependent truncation rules; a whole neighborhood of zero maps to zero. Right: $x-\operatorname{trunc}(x)$ takes the sign of a noninteger input, while $x-\lfloor x\rfloor$ lies in $[0,1)$ on both sides of zero. Open endpoints show excluded limiting values.

For every [real number](arithmetic.md#real-number) $x$,

$$
|x-\operatorname{trunc}(x)|<1,\qquad \operatorname{trunc}(-x)=-\operatorname{trunc}(x).
$$

The discarded difference $x-\operatorname{trunc}(x)$ has the sign of $x$ when $x$ is noninteger. In contrast, the [fractional part](#fractional-part) $x-\lfloor x\rfloor$ is always in $[0,1)$. At $x=-2.7$, these two differences are $-0.7$ and $0.3$. Thus specifying a signed fractional remainder requires specifying which integer-valued operation is used.

Unlike the [floor function](#floor-function) and [ceiling function](#ceiling-function), [truncation toward zero](#truncation-toward-zero) need not commute with adding an [integer](number-theory.md#integer). At $x=-0.7$ and $j=1$, $\operatorname{trunc}(x+j)=\operatorname{trunc}(0.3)=0$, whereas $\operatorname{trunc}(x)+j=1$. This matters if negative coordinates are assigned to equal-width bins by converting a quotient to an [integer](number-theory.md#integer): $x=-0.7$ belongs to the bin $[-1,0)$ under the [floor function](#floor-function), but truncation gives zero. The appropriate operation follows from the declared bin [intervals](real-analysis.md#interval-mathematics).

[Truncation toward zero](#truncation-toward-zero) is a [nondecreasing function](#nondecreasing-function) with a [discontinuity of a function](#discontinuity-of-a-function) at each nonzero [integer](number-theory.md#integer). It has no [discontinuity of a function](#discontinuity-of-a-function) at zero, because it is identically zero on $(-1,1)$. Its agreement with the [floor function](#floor-function) on the positive side and the [ceiling function](#ceiling-function) on the negative side explains the different closed endpoints in the diagram.

## Integral

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral)

An integral adds up contributions of a [function](function.md) across a [domain](topology.md#domain-mathematical-analysis). For a [continuous function](#continuous-function) $f$ on $[a,b]$, the [Riemann integral](real-analysis.md#riemann-integral) is the common [limit](#limit-of-a-function) of its [Riemann sums](real-analysis.md#riemann-sum) as the largest subinterval width tends to zero:

$$
\int_a^b f(x)\,dx
=\lim_{\max_i\Delta x_i\to0}\sum_i f(\xi_i)\Delta x_i,
\qquad \xi_i\in[x_{i-1},x_i],\quad \Delta x_i=x_i-x_{i-1}.
$$

Each product combines a value with the width over which it acts. When $f$ is nonnegative, the result is the [area](differential-geometry.md#surface-area) beneath its graph; values below the horizontal axis contribute with the opposite sign. The [signed area under a graph](#signed-area-under-a-graph) can therefore vanish even when the graph encloses nonzero geometric [area](differential-geometry.md#surface-area).

For a [velocity](classical-mechanics.md#velocity) $v(t)=1+2t$ on $0\le t\le3$, use $n$ equal time steps. The left and right [Riemann sums](real-analysis.md#riemann-sum) are

$$
L_n=12-\frac9n,\qquad R_n=12+\frac9n.
$$

Because the [function](function.md) is increasing, they bound the [integral](#integral). With six steps they give $10.5$ and $13.5$; with sixty steps they give $11.85$ and $12.15$. Both approach the same total, $12$. This is accumulation made exact by refining finite measurements.

<a id="image-left-and-right-riemann-sums-bracket-the-accumulated-displacement-of-a-particle-with-velocity-1-plus-2t"></a>
![](integral-riemann-sums.png)

**[Figure 5](#image-left-and-right-riemann-sums-bracket-the-accumulated-displacement-of-a-particle-with-velocity-1-plus-2t). Left and right Riemann sums bracket the accumulated displacement of a particle with velocity 1 + 2t**.

An [integral](#integral) retains units: [velocity](classical-mechanics.md#velocity) times time gives [displacement](classical-mechanics.md#displacement), and a [probability density function](continuous-probability-distribution.md#probability-density-function) integrated over an [interval](real-analysis.md#interval-mathematics) gives a [probability](probability-theory.md#probability). Weighting a [density](fluid-mechanics.md#density) by a [function](function.md) gives its [expectation](probability-theory.md#expected-value). The same operation serves different subjects because it expresses a common pattern, **value multiplied by extent, then accumulated**.

The [fundamental theorem of calculus](#fundamental-theorem-of-calculus) often evaluates a [definite integral](#definite-integral) by finding an [antiderivative](#antiderivative), but a finite sum or a numerical approximation is still useful when no convenient [antiderivative](#antiderivative) is available. An [indefinite integral](#antiderivative) denotes a family of [antiderivatives](#antiderivative); a [definite integral](#definite-integral) denotes an accumulated value between specified endpoints. More general constructions, including [Lebesgue integration](#lebesgue-integration), extend the class of [functions](function.md) and [domains](topology.md#domain-mathematical-analysis) that can be handled.

### Average value of a function

↑ **Parent:** [Integral](#integral)

For an [integrable function](measure-theory.md#lebesgue-integrable-function) on an [interval](real-analysis.md#interval-mathematics) $I$ of positive finite length, its average value is the [integral](#integral) divided by that length:

$$
\overline f_I=\frac1{|I|}\int_I f(x)\,dx.
$$

If $f$ is constant on equal-length subintervals, this is their values' [arithmetic mean](arithmetic.md#arithmetic-mean); unequal lengths require a [weighted mean](arithmetic.md#weighted-arithmetic-mean). For example, values $2$ and $6$ on two equal halves give average value $4$, whereas value $2$ on the first quarter and $6$ on the remaining three quarters give $5$. The [integral](#integral) measures total contribution; the [average value of a function](#average-value-of-a-function) divides out the interval length.

For the [function](function.md) $f(x)=2x$ on $[0,1]$, the [average value of a function](#average-value-of-a-function) is $\int_0^1 2x\,dx=1$. Replacing it by the constant $1$ preserves its [integral](#integral) on this interval. This is why the [Haar projection](fourier-analysis.md#haar-projection) uses [cell averages](#average-value-of-a-function) to obtain a coarser description while retaining each cell's total contribution.

### Linearity of integration

↑ **Parent:** [Integral](#integral)

For [integrable](measure-theory.md#integrability) [real-valued functions](function.md#real-valued-function) $f,g$ on a [measure space](measure-theory.md#measure-space) $(X,\mu)$ and fixed [real numbers](arithmetic.md#real-number) $a,b$, their [linear combination](vector-space.md#linear-combination) $af+bg$ is [integrable](measure-theory.md#integrability), and the [Lebesgue integral](measure-theory.md#lebesgue-integral) satisfies

$$
\int_X(af+bg)\,d\mu=a\int_X f\,d\mu+b\int_X g\,d\mu.
$$

The same rule applies to any finite [summation](arithmetic.md#summation): $\int_X\sum_{j=1}^n a_jf_j\,d\mu=\sum_{j=1}^n a_j\int_X f_j\,d\mu$ for [integrable](measure-theory.md#integrability) [functions](function.md) $f_j$ and fixed [scalars](vector-space.md#scalar) $a_j$. Finite signed values matter: [integrability](measure-theory.md#integrability) ensures all these [integrals](#integral) are finite, so no undefined $\infty-\infty$ occurs.

This is the [distributive property](algebra.md#distributive-property) of finite [summation](arithmetic.md#summation) carried into [integration](#integral): a fixed factor can be pulled out, and a finite sum can be integrated term by term. For [simple functions](measure-theory.md#simple-function), distribute the finite sums of value times [measure](measure-theory.md#measure); approximation extends additivity to nonnegative [measurable functions](measure-theory.md#measurable-function), and splitting into a [positive part](function.md#positive-part-of-a-real-valued-function) and [negative part](function.md#negative-part-of-a-real-valued-function) gives the [integrable](measure-theory.md#integrability) signed case. See [Lecture 12: Lebesgue Integrable Functions, the Lebesgue Integral and the Dominated Convergence Theorem](mathematics-bibliography.md#18-102-introduction-to-functional-analysis-spring-2021-lecture-notes-by-andrew-lin/lecture-12-lebesgue-integrable-functions-the-lebesgue-integral-and-the-dominated-convergence-theorem) (Proposition 122: linearity for integrable functions). For example, $\int_0^1(2x-3)\,dx=2\int_0^1x\,dx-3\int_0^1 1\,dx=-2$. With a [probability measure](probability-theory.md#probability-measure), [linearity of integration](#linearity-of-integration) gives [linearity of expectation](probability-theory.md#linearity-of-expectation).

### Signed area under a graph

↑ **Parent:** [Integral](#integral)

For $a<b$ and a [real-valued function](function.md#real-valued-function) $f$ with a finite [Riemann integral](real-analysis.md#riemann-integral) or [Lebesgue integral](measure-theory.md#lebesgue-integral) on $[a,b]$, the [signed area under a graph](#signed-area-under-a-graph) is its [definite integral](#definite-integral): geometric [area](differential-geometry.md#surface-area) above the horizontal axis contributes positively, and geometric [area](differential-geometry.md#surface-area) below it contributes negatively. If these two nonnegative [areas](differential-geometry.md#surface-area) are $A_+$ and $A_-$, then

$$
\int_a^b f(x)\,dx=A_+-A_-,\qquad
\int_a^b |f(x)|\,dx=A_++A_-.
$$

The second expression is the [total geometric area under a graph](#total-geometric-area-under-a-graph). Taking the [absolute value](real-analysis.md#absolute-value) of the first expression does not usually give the second: cancellation has already removed information about how much [area](differential-geometry.md#surface-area) lies on each side.[5.2 The Definite Integral](mathematics-bibliography.md#calculus-volume-1-by-gilbert-strang-and-others/5-2-the-definite-integral)

For an exact example, take the [polynomial function](polynomial.md#polynomial-function) $f(x)=x^2-1$ on $[-2,2]$. Its [polynomial roots](polynomial.md#root-of-a-polynomial) are $-1$ and $1$: it is negative between them and positive on the two outer [intervals](real-analysis.md#interval-mathematics). An [antiderivative](#antiderivative) is $F(x)=x^3/3-x$, so the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) gives

$$
\int_{-2}^{-1}(x^2-1)\,dx=\frac43,\qquad
\int_{-1}^{1}(x^2-1)\,dx=-\frac43,\qquad
\int_{1}^{2}(x^2-1)\,dx=\frac43.
$$

Thus $A_+=8/3$ and $A_-=4/3$. The [signed area under a graph](#signed-area-under-a-graph) is $4/3$, whereas the [total geometric area under a graph](#total-geometric-area-under-a-graph) is $4$. To compute the latter with [antiderivatives](#antiderivative), split at each sign-changing [polynomial root](polynomial.md#root-of-a-polynomial) and reverse the sign of the negative contribution.

<a id="signed-polynomial-area-and-absolute-area"></a>
![](signed-polynomial-area-and-absolute-area.png)

**[Figure 6](#signed-polynomial-area-and-absolute-area). The polynomial x squared minus one has signed integral 4/3 and total geometric area 4 on the interval from minus two to two**.

Cancellation is useful information when the [integrand](#integrand) represents a signed contribution. For the [polynomial function](polynomial.md#polynomial-function) $f(x)=x$ on $[-1,1]$, the two triangular [areas](differential-geometry.md#surface-area) give $\int_{-1}^1x\,dx=0$, although $\int_{-1}^1|x|\,dx=1$. Zero [net signed area](#signed-area-under-a-graph) therefore means balanced positive and negative contributions, rather than an empty region.

The short algebraic justification uses the [positive part](function.md#positive-part-of-a-real-valued-function) $f_+=\max(f,0)$ and [negative part](function.md#negative-part-of-a-real-valued-function) $f_-=\max(-f,0)$: $f=f_+-f_-$ and $|f|=f_++f_-$. Their [integrals](#integral) give $A_+$ and $A_-$, and [linearity of integration](#linearity-of-integration) gives the difference and sum formulas. For [Lebesgue integration](#lebesgue-integration), require both contributions to be finite to avoid the undefined subtraction $\infty-\infty$.[Definitions 120–121 and Proposition 122](mathematics-bibliography.md#18-102-introduction-to-functional-analysis-spring-2021-lecture-notes-by-andrew-lin/lecture-12-lebesgue-integrable-functions-the-lebesgue-integral-and-the-dominated-convergence-theorem)

#### Total geometric area under a graph

↑ **Parent:** [Signed area under a graph](#signed-area-under-a-graph)

### Definite integral

↑ **Parent:** [Integral](#integral)

A [definite integral](#definite-integral) accumulates an [integrand](#integrand) between specified endpoints, retaining the sign of each contribution. For a [real-valued function](function.md#real-valued-function) on a finite [real interval](real-analysis.md#interval-mathematics), a finite [definite integral](#definite-integral) is a [scalar](vector-space.md#scalar); an [indefinite integral](#antiderivative) describes a family of [antiderivatives](#antiderivative). The lower and upper limits of integration $a,b$ specify where accumulation starts and ends. The integration variable is a placeholder: $\int_a^b f(x)\,dx=\int_a^b f(u)\,du$.

This is useful whenever a varying rate must be converted into a total change. For motion along a [straight line](geometry-and-topology.md#straight-line) with [continuous](#continuous-function) [velocity](classical-mechanics.md#velocity) $v(t)$ and [position](classical-mechanics.md#position) $s(t)$ satisfying $s'(t)=v(t)$, the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) gives [displacement](classical-mechanics.md#displacement), while accumulating [speed](classical-mechanics.md#speed) gives the [distance traveled from velocity](#distance-traveled-from-velocity):

$$
s(b)-s(a)=\int_a^b v(t)\,dt,\qquad
D=\int_a^b |v(t)|\,dt,\qquad a<b.
$$

Negative [velocity](classical-mechanics.md#velocity) reduces [displacement](classical-mechanics.md#displacement) while adding to the [distance traveled from velocity](#distance-traveled-from-velocity). The [physical dimension](physics.md#physical-dimension) of a [definite integral](#definite-integral) is the product of the [integrand](#integrand)'s [physical dimension](physics.md#physical-dimension) and the integration variable's [physical dimension](physics.md#physical-dimension): here $(\mathrm{m}/\mathrm{s})\mathrm{s}=\mathrm{m}$. An [area](differential-geometry.md#surface-area) on a rate graph need not be a spatial [area](differential-geometry.md#surface-area).[Theorem 5.6 and the displacement and total-distance discussion](mathematics-bibliography.md#calculus-volume-1-by-gilbert-strang-and-others/5-4-integration-formulas-and-the-net-change-theorem)

As an explicitly synthetic motion model, let $v(t)=(2\,\mathrm{m}\,\mathrm{s}^{-2})t-2\,\mathrm{m}\,\mathrm{s}^{-1}$ for $0\le t\le3\,\mathrm{s}$, with $s(0)=0$. Using numerical values in seconds and metres, an [antiderivative](#antiderivative) gives $s(t)=t^2-2t$. The [velocity](classical-mechanics.md#velocity) changes sign at $t=1$: the model first moves $1$ m in the negative direction, then $4$ m in the positive direction. Its [displacement](classical-mechanics.md#displacement) is $-1+4=3$ m, and its [distance traveled from velocity](#distance-traveled-from-velocity) is $1+4=5$ m. The initial [position](classical-mechanics.md#position) fixes the [constant of integration](#constant-of-integration), but does not change either accumulated quantity.

<a id="variable-velocity-displacement-and-distance"></a>
![](variable-velocity-displacement-and-distance.png)

**[Figure 7](#variable-velocity-displacement-and-distance). Synthetic variable velocity model with displacement 3 metres and distance traveled 5 metres over three seconds**.

Orientation matters independently of whether the [integrand](#integrand) is positive or negative. For a [function](function.md) [integrable](measure-theory.md#integrability) on the [interval](real-analysis.md#interval-mathematics) containing the endpoints, use the conventions

$$
\int_a^a f(x)\,dx=0,\qquad
\int_b^a f(x)\,dx=-\int_a^b f(x)\,dx,\qquad
\int_a^c f(x)\,dx=\int_a^b f(x)\,dx+\int_b^c f(x)\,dx.
$$

For the preceding [velocity](classical-mechanics.md#velocity) model, accumulation from $3$ seconds back to $0$ seconds gives $-3$ m. Reversing the bounds of the [speed](classical-mechanics.md#speed) [integral](#integral) gives $-5$ m, which is an oriented [integral](#integral), not a negative [distance traveled from velocity](#distance-traveled-from-velocity); physical elapsed-time totals use the earlier endpoint first. The splitting rule holds even when $b$ is outside the [interval](real-analysis.md#interval-mathematics) between $a$ and $c$, provided [integrability](measure-theory.md#integrability) holds on the [interval](real-analysis.md#interval-mathematics) containing all three endpoints.[5.2 The Definite Integral](mathematics-bibliography.md#calculus-volume-1-by-gilbert-strang-and-others/5-2-the-definite-integral)

Existence needs hypotheses. For a [bounded function](function.md#bounded-function) $f$ on $[a,b]$ with $a<b$, a finite [Riemann integral](real-analysis.md#riemann-integral) exists when every tagged [Riemann sum](real-analysis.md#riemann-sum) approaches the same value as the largest cell width tends to zero:

$$
\int_a^b f(x)\,dx=\lim_{\max_i(x_i-x_{i-1})\to0}
\sum_{i=1}^n f(\xi_i)(x_i-x_{i-1}),\qquad
a=x_0<\cdots<x_n=b,\quad \xi_i\in[x_{i-1},x_i].
$$

The [limit](#limit-of-a-function) must be independent of both the [partition of an interval](real-analysis.md#partition-of-an-interval) and the tags. Merely making the number of cells large can leave a wide cell unresolved. On a finite [closed interval](real-analysis.md#closed-real-interval), every [continuous function](#continuous-function), and every [bounded function](function.md#bounded-function) that is [continuous](#continuous-function) except at finitely many points, is [Riemann integrable](real-analysis.md#riemann-integrable-function).[Lemma 5.2.7 and Theorem 5.2.9](mathematics-bibliography.md#basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/5-2-properties-of-the-integral) Boundedness alone is insufficient: the [Dirichlet function](real-analysis.md#dirichlet-function) on $[0,1]$ is $1$ on the [rational numbers](number-theory.md#rational-number) and $0$ on the [irrational numbers](algebra.md#irrational-number). Tags can all be chosen rational or all irrational, giving [Riemann sums](real-analysis.md#riemann-sum) of $1$ or $0$ at arbitrarily small cell widths.[Example 5.1.4](mathematics-bibliography.md#basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/5-1-the-riemann-integral)

For a finite signed [Lebesgue integral](measure-theory.md#lebesgue-integral), the condition is instead that $f$ be a [measurable function](measure-theory.md#measurable-function) for [Lebesgue measure](measure-theory.md#lebesgue-measure) and $\int_{[a,b]}|f|\,dx<\infty$. A [measurable function](measure-theory.md#measurable-function) for [Lebesgue measure](measure-theory.md#lebesgue-measure) that is also a [bounded function](function.md#bounded-function) on a finite [interval](real-analysis.md#interval-mathematics) satisfies this condition since $|f|\le M$ gives $\int|f|\le M(b-a)$. The [Dirichlet function](real-analysis.md#dirichlet-function) therefore has [Lebesgue integral](measure-theory.md#lebesgue-integral) zero: the [rational numbers](number-theory.md#rational-number) form a [null set](measure-theory.md#null-set), so it equals zero [Lebesgue almost everywhere](measure-theory.md#almost-everywhere). The [Riemann integral](real-analysis.md#riemann-integral) and [Lebesgue integral](measure-theory.md#lebesgue-integral) agree for the [continuous functions](#continuous-function) used in the diagrams.[Definition 120, Proposition 123(2), Remark 124 and Theorem 126](mathematics-bibliography.md#18-102-introduction-to-functional-analysis-spring-2021-lecture-notes-by-andrew-lin/lecture-12-lebesgue-integrable-functions-the-lebesgue-integral-and-the-dominated-convergence-theorem) An unbounded [integrand](#integrand) or infinite endpoint requires further analysis, for example the [limits](#limit-of-a-function) defining an [improper integral](real-analysis.md#improper-integral); the notation alone does not establish convergence.

#### Distance traveled from velocity

↑ **Parent:** [Definite integral](#definite-integral)

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

An antiderivative recovers a [function](function.md) from its local rate of change. For a [real-valued function](function.md#real-valued-function) $g$ on an [open subset](topology.md#open-set) $U$ of the [real line](real-analysis.md#real-line), a [differentiable function](analysis.md#differentiable-function) $F$ is an antiderivative when

$$
\boxed{F'(x)=g(x)\qquad(x\in U).}
$$

For example, $g(x)=x^2$ has the antiderivatives $F_C(x)=x^3/3+C$ for every real [additive constant](#additive-constant) $C$. Their [derivatives](#derivative) agree, while their values can differ. On an [interval](real-analysis.md#interval-mathematics), the [constant of integration](#constant-of-integration) describes the entire freedom in the answer. [OpenStax Calculus 1, §4.10: antiderivatives and their families](https://openstax.org/books/calculus-volume-1/pages/4-10-antiderivatives)

<a id="image-a-family-of-antiderivatives-has-one-common-derivative-and-an-initial-value-selects-one-member"></a>
![](antiderivative-family-and-initial-value.png)

**[Figure 8](#image-a-family-of-antiderivatives-has-one-common-derivative-and-an-initial-value-selects-one-member). A family of antiderivatives has one common derivative, and an initial value selects one member**.

The indefinite-integral notation $\int g(x)\,dx=F(x)+C$ records this family on an [interval](real-analysis.md#interval-mathematics). For the illustrated family, the extra condition $F(1)=2$ selects $C=5/3$. Thus reversing [differentiation](#differentiation) requires both a rate and a reference value if a unique [function](function.md) is wanted.

The [fundamental theorem of calculus](#fundamental-theorem-of-calculus) supplies a construction when $g$ is [continuous](#continuous-function) on an [interval](real-analysis.md#interval-mathematics) $I$. Choose $x_0\in I$ and set $F(x)=\int_{x_0}^x g(t)\,dt$; then $F'=g$. [Integrability](measure-theory.md#integrability) alone does not guarantee a classical antiderivative. The [Heaviside step function](analysis.md#heaviside-step-function) is [Riemann integrable](real-analysis.md#riemann-integrable-function) on bounded [intervals](real-analysis.md#interval-mathematics), but cannot be a [derivative](#derivative) throughout an [interval](real-analysis.md#interval-mathematics) containing its jump: [Darboux theorem for derivatives](#darboux-s-theorem-analysis) requires every intermediate value. [Lebl, Basic Analysis I, §4.2.5: the intermediate-value property of derivatives](https://www.jirka.org/ra/html/sec_mvt.html)

#### Constant of integration

↑ **Parent:** [Antiderivative](#antiderivative)

On a connected open [interval](real-analysis.md#interval-mathematics), if $F'=g$, every [antiderivative](#antiderivative) of $g$ has the form $F+C$, where $C$ is a [constant function](function.md#constant-function). Indeed, two solutions satisfy $(G-F)'=0$: the [zero derivative on a connected open set](#zero-derivative-on-a-connected-open-set) principle makes their difference constant. In one dimension, the [mean value theorem](#mean-value-theorem) proves this on any closed subinterval. [Lebl, Basic Analysis I, Proposition 4.2.6: zero derivative on an interval](https://www.jirka.org/ra/html/sec_mvt.html)

An [initial condition](differential-equation.md#initial-condition) or [boundary condition](differential-equation.md#boundary-condition) can determine $C$. If a particular [antiderivative](#antiderivative) is $F_0$ and $F(x_0)=y_0$, then

$$
\boxed{C=y_0-F_0(x_0).}
$$

For $g(x)=x^2$, $F_0(x)=x^3/3$ and $F(1)=2$, this gives $C=5/3$. Without that reference value, choosing $C=0$ simply selects one member of the family.

The freedom has a physical meaning in a simple kinematic model. A [velocity](classical-mechanics.md#velocity) $v(t)=at$, with constant [acceleration](classical-mechanics.md#acceleration) $a$, determines [position](classical-mechanics.md#position) only as $x(t)=at^2/2+C$. The [initial condition](differential-equation.md#initial-condition) $x(0)=x_0$ selects $C=x_0$; changing the starting [position](classical-mechanics.md#position) does not change the prescribed [velocity](classical-mechanics.md#velocity).

For the [differential equation](differential-equation.md) $T'=-B/r^2$ on $r>0$, the [antiderivative](#antiderivative) is $T=B/r+C$. The [boundary condition](differential-equation.md#boundary-condition) $T(R_s)=T_s$ gives $C=T_s-B/R_s$. Discarding the [constant of integration](#constant-of-integration) therefore needs a specified condition or an approximation that quantifies its effect. On a domain with several [connected components](geometry-and-topology.md#connected-component), the freedom is larger: [antiderivatives on disconnected domains](#antiderivatives-on-disconnected-domains) require a separate constant on each component.

##### Antiderivatives on disconnected domains

↑ **Parent:** [Constant of integration](#constant-of-integration)

Let $U$ be an [open subset](topology.md#open-set) of the [real line](real-analysis.md#real-line), and let $F,G$ be [antiderivatives](#antiderivative) of the same [function](function.md) on $U$. Each [connected component](geometry-and-topology.md#connected-component) $I_j$ is an open [interval](real-analysis.md#interval-mathematics). On that component, $(G-F)'=0$, so the [mean value theorem](#mean-value-theorem) gives $G-F=C_j$. The constants on different components are independent: there is no subinterval inside $U$ joining them. Conversely, adding any chosen constant on each component preserves the [derivative](#derivative) everywhere on $U$.

For example, the domain of $g(x)=1/x$ is $U=\mathbb R\setminus\{0\}$. Every [antiderivative](#antiderivative) on this domain has the form

$$
F(x)=
\begin{cases}
\log|x|+C_-,&x<0,\\
\log|x|+C_+,&x>0,
\end{cases}
$$

with arbitrary real $C_-,C_+$. The [logarithm](#logarithm) of the [absolute value](real-analysis.md#absolute-value) differentiates to $1/x$ on each side. The function with $C_-=2$ and $C_+=-1$ is therefore a valid [antiderivative](#antiderivative), although it cannot be written as $\log|x|+C$ with one global constant.

<a id="image-two-disconnected-intervals-allow-independent-constants-while-the-derivative-stays-the-same"></a>
![](antiderivative-disconnected-domain-constants.png)

**[Figure 9](#image-two-disconnected-intervals-allow-independent-constants-while-the-derivative-stays-the-same). Two disconnected intervals allow independent constants while the derivative stays the same**.

An [initial condition](differential-equation.md#initial-condition) at $x=1$ fixes $C_+$ and leaves $C_-$ free. Fixing both constants requires one reference value in each [connected component](geometry-and-topology.md#connected-component), or additional conditions that couple the components. The [locally constant function](#locally-constant-function) $F(x)-\log|x|$ captures this remaining freedom.

#### Additive constant

↑ **Parent:** [Antiderivative](#antiderivative)

A constant added to a [function](function.md) changes its reference level without changing its [derivative](#derivative):

$$
\frac{d}{dx}\bigl(F(x)+C\bigr)=F'(x).
$$

Geometrically, it is a vertical [translation](geometry-and-topology.md#translation-geometry) of the graph. For $F(x)=x^3/3$, changing $C$ moves every plotted value by the same amount while preserving every tangent slope. This is the geometric reason that [antiderivatives](#antiderivative) form a family.

When $F$ represents a [physical quantity](physics.md#physical-quantity), the [physical dimension](physics.md#physical-dimension) of $C$ must match that of $F$. When [position](classical-mechanics.md#position) is obtained from [velocity](classical-mechanics.md#velocity), $C$ is a position offset. An unknown starting position remains unknown even when the rate of change is known exactly.

When describing the family of [antiderivatives](#antiderivative) on an [interval](real-analysis.md#interval-mathematics), the arbitrary additive constant is the [constant of integration](#constant-of-integration). On a disconnected open domain, the corresponding freedom is a [locally constant function](#locally-constant-function), as in [antiderivatives on disconnected domains](#antiderivatives-on-disconnected-domains), rather than necessarily one constant on the whole domain.

### Gaussian integral

↑ **Parent:** [Integral](#integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_integral)

The [Gaussian integral](#gaussian-integral) gives the exact area under a [Gaussian function](#gaussian-function). For a positive [real number](arithmetic.md#real-number) $a$,

$$
\boxed{I(a)=\int_{-\infty}^{\infty}e^{-ax^2}\,dx=\sqrt{\frac\pi a}.}
$$

This is a finite [improper integral](real-analysis.md#improper-integral) over the whole [real line](real-analysis.md#real-line). For example, $I(1)=\sqrt\pi\approx1.772454$ and $I(4)=\sqrt\pi/2\approx0.886227$. Increasing $a$ from one to four narrows the curve and halves its area, while its height at zero stays one. The [change of variables](#change-of-variables-formula) $u=\sqrt a\,x$ explains the factor $a^{-1/2}$.

<a id="image-narrower-gaussian-curves-have-less-area-unless-their-height-is-adjusted"></a>
![](gaussian-integral-width-and-area.png)

**[Figure 10](#image-narrower-gaussian-curves-have-less-area-unless-their-height-is-adjusted). Narrower Gaussian curves have less area unless their height is adjusted**. Left: the full-line areas of $e^{-x^2}$ and $e^{-4x^2}$ are $\sqrt\pi$ and $\sqrt\pi/2$. Right: multiplication by $\sqrt{a/\pi}$ makes both areas one. Shading shows the plotted finite interval; the stated areas refer to the whole [real line](real-analysis.md#real-line).

The useful consequence is an exact normalization. For $a>0$ and any real center $\mu$,

$$
p_a(x)=\sqrt{\frac a\pi}\,e^{-a(x-\mu)^2},\qquad
\int_{\mathbb R}p_a(x)\,dx=1.
$$

This is a [probability density function](continuous-probability-distribution.md#probability-density-function) for a [normal distribution](probability-theory.md#normal-distribution) with [expected value](probability-theory.md#expected-value) $\mu$ and [variance](variance.md) $1/(2a)$. A narrower [probability density function](continuous-probability-distribution.md#probability-density-function) must be taller to keep total [probability](probability-theory.md#probability) one. In the usual notation $a=1/(2\sigma^2)$, the prefactor is $1/(\sigma\sqrt{2\pi})$, where $\sigma$ is the [standard deviation](variance.md#standard-deviation).

The same area calculation makes the one-dimensional [heat kernel](diffusion-equation.md#heat-kernel)

$$
K(x,t)=\frac1{\sqrt{4\pi Dt}}e^{-x^2/(4Dt)},\qquad D>0,\quad t>0,
$$

integrate to one in $x$, with $D$ the [diffusion coefficient](brownian-motion.md#diffusion-coefficient). A spreading [Gaussian function](#gaussian-function) can therefore preserve total mass while its height falls. This links the [Gaussian integral](#gaussian-integral) with both the [normal distribution](probability-theory.md#normal-distribution) and the [diffusion equation](diffusion-equation.md).

Finite intervals lead to the [error function](#error-function), rather than this single constant:

$$
\operatorname{erf}(z)=\frac2{\sqrt\pi}\int_0^z e^{-u^2}\,du,\qquad
\int_{-R}^{R}e^{-ax^2}\,dx
=\sqrt{\frac\pi a}\operatorname{erf}(\sqrt a\,R),\quad R\ge0.
$$

The complementary tail is described by the [complementary error function](#complementary-error-function). These definitions and their real-axis limits are given in the NIST reference. [NIST Digital Library of Mathematical Functions, §7.2, equations 7.2.1–7.2.4](https://dlmf.nist.gov/7.2)

The [polar-coordinate proof of the Gaussian integral](#polar-coordinate-proof-of-the-gaussian-integral) explains why $\pi$ appears in an integral of a function defined on a line: squaring its area creates a rotationally symmetric integral on a plane. Substitution $t=x^2$ also gives $\Gamma(1/2)=2\int_0^\infty e^{-x^2}\,dx=\sqrt\pi$, connecting the result with the [Gamma function](complex-analysis.md#gamma-function).

#### Polar-coordinate proof of the Gaussian integral

↑ **Parent:** [Gaussian integral](#gaussian-integral)

Put $I=I(1)$. The nonnegative [integrand](#integrand) allows [Tonelli's theorem](measure-theory.md#tonelli-theorem) to write the square as a [double integral](#double-integral):

$$
I^2=\int_{\mathbb R^2}e^{-(x^2+y^2)}\,dx\,dy.
$$

In [polar coordinates](#polar-coordinates), $x=r\cos\theta$, $y=r\sin\theta$, and the [Jacobian determinant](#jacobian-determinant) supplies the area factor $r$:

$$
I^2=\int_0^{2\pi}\int_0^\infty e^{-r^2}r\,dr\,d\theta
=2\pi\left[-\frac12e^{-r^2}\right]_0^\infty
=\pi.
$$

Since $I>0$, take the positive [square root](algebra.md#square-root) to get $I=\sqrt\pi$. The computation proves finiteness as well as the value. For an explicit limiting argument, first integrate over disks of radius $R$; their integrals are $\pi(1-e^{-R^2})$, which increase to $\pi$ as $R\to\infty$. [Strang and Herman, Calculus Volume 3, §5.3: the polar area element](https://openstax.org/books/calculus-volume-3/pages/5-3-double-integrals-in-polar-coordinates)

<a id="image-gaussian-height-times-the-circumference-of-a-ring-gives-its-radial-contribution"></a>
![](gaussian-integral-polar-annulus.png)

**[Figure 11](#image-gaussian-height-times-the-circumference-of-a-ring-gives-its-radial-contribution). Gaussian height times the circumference of a ring gives its radial contribution**. Left: $e^{-(x^2+y^2)}$ is constant around each circle; the marked annulus illustrates a finite-width shell. Right: the radial contribution $2\pi r e^{-r^2}$ includes the circumference factor and integrates to $\pi$. The shell in the picture has finite width; $2\pi r\,dr$ is the infinitesimal area element.

The geometric surprise is that radial shells get longer as $r$ increases, even while the [Gaussian function](#gaussian-function) gets smaller. Its central height is largest at zero, but the radial contribution $2\pi r e^{-r^2}$ vanishes there and peaks at $r=1/\sqrt2$. Differentiating gives $2\pi e^{-r^2}(1-2r^2)$, which changes sign at that radius. Keeping the [Jacobian determinant](#jacobian-determinant) is what makes the one-dimensional [integral](#integral) and the plane geometry agree.

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

A [Taylor polynomial](#taylor-polynomial) replaces a [function](function.md) near a chosen point by a [polynomial](polynomial.md) with matching [derivatives](#derivative). If $f$ has [derivatives](#derivative) through order $n$ at $a$, define

$$
T_{n,a}(x)=\sum_{k=0}^n\frac{f^{(k)}(a)}{k!}(x-a)^k.
$$

The [factorial](combinatorics.md#factorial) denominator makes $T_{n,a}^{(j)}(a)=f^{(j)}(a)$ for $0\leq j\leq n$. This determines a unique [polynomial](polynomial.md) of [degree of a polynomial](polynomial.md#degree-of-a-polynomial) at most $n$. Order zero matches the value, order one also matches the [tangent line](#tangent-line), and order two also incorporates the second [derivative](#derivative). Matching more local information is useful because [polynomials](polynomial.md) are easy to evaluate, differentiate, and integrate. The distinction between the finite [Taylor polynomial](#taylor-polynomial) and the infinite [Taylor series](#taylor-series) is developed in [OpenStax, Taylor and Maclaurin series](https://openstax.org/books/calculus-volume-2/pages/6-3-taylor-and-maclaurin-series).

For a computed example, let $f(x)=\sqrt{1+x}$ and expand at zero. Its first three [derivatives](#derivative) give

$$
f(0)=1,\qquad f'(0)=\frac12,\qquad f''(0)=-\frac14,\qquad T_{2,0}(x)=1+\frac x2-\frac{x^2}8.
$$

At $x=0.1$, the linear approximation is $1.05$ and the quadratic approximation is $1.04875$, compared with $\sqrt{1.1}\approx1.048808848$. The quadratic correction captures the downward bending of the [square root](algebra.md#square-root) and reduces the absolute difference from about $0.00119115$ to $0.0000588482$.

<a id="image-matching-more-derivatives-improves-a-local-square-root-approximation-and-the-third-derivative-supplies-an-error-bound"></a>
![](taylor-square-root-approximation.png)

**[Figure 12](#image-matching-more-derivatives-improves-a-local-square-root-approximation-and-the-third-derivative-supplies-an-error-bound). Matching more derivatives improves a local square-root approximation, and the third derivative supplies an error bound**.

The [Taylor remainder](#taylor-remainder) turns this convenient approximation into a controlled calculation. On $[0,0.1]$, $f'''(x)=3/[8(1+x)^{5/2}]$ is positive and at most $3/8$. The [Taylor theorem with Lagrange remainder](#taylor-theorem-with-lagrange-remainder) therefore gives

$$
0<\sqrt{1.1}-1.04875\leq\frac{(3/8)(0.1)^3}{3!}=\frac1{16000}.
$$

Consequently **$1.04875<\sqrt{1.1}\leq1.0488125$** follows without using the displayed decimal evaluation as evidence. The [Taylor polynomial](#taylor-polynomial) and the [Taylor remainder](#taylor-remainder) play different roles: the former supplies an answer that is easy to compute, while the latter specifies what accuracy is justified. Farther from the expansion point, the same low-degree [polynomial](polynomial.md) need not remain accurate.

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

The real [exponential function](#exponential-function) $\exp(x)=e^x$ converts addition into multiplication:

$$
\exp(x+y)=\exp(x)\exp(y),\qquad \exp(0)=1,\qquad \frac{d}{dx}\exp(x)=\exp(x).
$$

Its values are positive, and it defines a [bijection](function.md#bijection) from the [real numbers](arithmetic.md#real-number) to the positive [real numbers](arithmetic.md#real-number). The [natural logarithm](#natural-logarithm) is its [inverse function](function.md#inverse-function). These properties connect arithmetic with [calculus](calculus.md): adding an amount to the input multiplies the output by a fixed factor, and the local rate of change equals the current value. The [exponential series](#exponential-series) gives one construction; an equivalent characterization is the unique [solution of a differential equation](differential-equation.md#solution-of-a-differential-equation) $y'=y$, $y(0)=1$.

For a concrete example, $y(t)=10e^{0.2t}$ starts at $10$ and satisfies $y'=0.2y$. The absolute [derivative](#derivative) increases with $y$, while the relative rate $y'/y$ stays $0.2$. At $t=5$, $y=10e\approx27.1828$ and $y'\approx5.43656$. The [exponential function](#exponential-function) therefore models accumulation proportional to what is already present, rather than addition of a fixed amount at every step. A positive constant rate gives [exponential growth](#exponential-growth); a negative one gives [exponential decay](analysis.md#exponential-decay).

Every positive real base $b\ne1$ fits the same construction through $b^x=e^{x\ln b}$. Thus its [derivative](#derivative) is $(\ln b)b^x$: base $e$ is special because $\ln e=1$. The [exponential function](#exponential-function) is also unchanged in form by [differentiation](#differentiation) and [integration](#integral), helping explain its repeated appearance in [linear ordinary differential equations](differential-equation.md#linear-ordinary-differential-equation). Its real definition, inverse relationship, and derivative rules are developed in [OpenStax, integrals, exponential functions, and logarithms](https://openstax.org/books/calculus-volume-1/pages/6-7-integrals-exponential-functions-and-logarithms).

### Exponential growth

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_growth)

A positive quantity undergoes [exponential growth](#exponential-growth) at constant rate $r>0$ when $y'=ry$. For $y_0>0$, the [solution of a differential equation](differential-equation.md#solution-of-a-differential-equation) is $y(t)=y_0e^{rt}$. Every interval of duration $\Delta t$ multiplies the value by the same factor $e^{r\Delta t}$, independently of its starting value.

#### Doubling time

↑ **Parent:** [Exponential growth](#exponential-growth)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doubling_time)

The interval required to double a quantity under constant-rate [exponential growth](#exponential-growth). Solving $e^{rt_2}=2$ with the [natural logarithm](#natural-logarithm) gives $t_2=\ln2/r$. At $r=0.2$ per time unit, it is approximately $3.46574$ time units; every subsequent doubling takes the same interval.

### e (mathematical constant)

↑ **Parent:** [Exponential function](#exponential-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/e_(mathematical_constant))

[Euler's number](#e-mathematical-constant) is the value $\exp(1)=\sum_{n=0}^{\infty}1/n!$ of the [exponential function](#exponential-function), approximately $2.71828$. It is the base of the [natural logarithm](#natural-logarithm). Its factorial-series tail gives an elementary proof of the [irrationality of e](#irrationality-of-e). The [compounding limit for e](#compounding-limit-for-e) shows how the same constant arises from repeated small multiplications.

#### Compounding limit for e

↑ **Parent:** [e (mathematical constant)](#e-mathematical-constant)

Start at one and apply $n$ updates, each multiplying the current value by $1+1/n$. The final value is $(1+1/n)^n$: one update gives $2$, two give $2.25$, ten give approximately $2.59374$, and one hundred give approximately $2.70481$. Increasing the number of steps, while reducing each increment proportionally, approaches [Euler's number](#e-mathematical-constant) rather than producing unbounded accumulation.

<a id="image-repeated-smaller-proportional-updates-approach-euler-s-number-over-one-fixed-interval"></a>
![](compound-growth-limit.png)

**[Figure 13](#image-repeated-smaller-proportional-updates-approach-euler-s-number-over-one-fixed-interval). Repeated smaller proportional updates approach Euler's number over one fixed interval**.

The [natural logarithm](#natural-logarithm) makes the [limit](#limit-of-a-function) transparent. For $u>0$, its [integral](#integral) definition gives $u/(1+u)\leq\ln(1+u)\leq u$, by bounding $1/t$ on $[1,1+u]$. With $u=1/n$,

$$
\frac1{1+1/n}\leq n\ln(1+1/n)\leq1.
$$

The [squeeze theorem](#squeeze-theorem) gives a logarithmic [limit](#limit-of-a-function) of one; continuity of the [exponential function](#exponential-function) gives $(1+1/n)^n\to e$. This links a discrete multiplicative rule with continuous [exponential growth](#exponential-growth), without assuming that a finite number of steps equals the limiting value.

#### Irrationality of e

↑ **Parent:** [e (mathematical constant)](#e-mathematical-constant)

If [Euler's number](#e-mathematical-constant) were $a/b$, choose $n\geq\max(b,2)$ and multiply its factorial-series tail by $n!$. This produces an [integer](number-theory.md#integer), but the tail is positive and smaller than $\sum_{j\geq1}(n+1)^{-j}=1/n<1$. The contradiction proves that the number is an [irrational number](algebra.md#irrational-number). The argument rules out a hypothetical rational remainder by placing it in an impossible [integer](number-theory.md#integer) interval.

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

For a positive real base $b\ne1$, the [logarithm](#logarithm) is the [inverse function](function.md#inverse-function) of the [exponential function](#exponential-function) $t\mapsto b^t$:

$$
\log_b x=t\quad\Longleftrightarrow\quad b^t=x,\qquad x>0.
$$

It asks which exponent produces a given positive number. Thus $\log_2 8=3$ and $\log_2(1/8)=-3$. The base restrictions matter: $b=1$ would produce only one value, while a negative base does not define $b^t$ as a real-valued [function](function.md) for every real exponent.

The useful transformation is

$$
\log_b(xy)=\log_bx+\log_by,\qquad \log_b(x/y)=\log_bx-\log_by.
$$

For example, $8\cdot16=128$ corresponds to $3+4=7$ in base two. Products become sums and ratios become differences. The [logarithm](#logarithm) does not generally convert a sum into a sum of logarithms. Base conversion uses the [natural logarithm](#natural-logarithm): $\log_bx=\ln x/\ln b$. It also gives $d(\log_bx)/dx=1/(x\ln b)$, positive when $b>1$ and negative when $0<b<1$.

Historically, [John Napier](mathematics.md#john-napier)'s 1614 Mirifici logarithmorum canonis descriptio presented logarithmic tables and their use, documented in [the Smithsonian Libraries' digitized original](https://library.si.edu/digital-library/book/mirificilogarit00napi). Tables made multiplication-heavy calculations more manageable by replacing products with addition and a lookup. The 1619 Constructio title page below belongs to a later publication from the same work on [logarithms](#logarithm). These historical publications preceded the modern [inverse function](function.md#inverse-function) and [integral](#integral) presentation used here.

<a id="image-title-page-of-napier-s-1619-mirifici-logarithmorum-canonis-constructio"></a>
<img src="https://upload.wikimedia.org/wikipedia/commons/3/3b/Napier&#039;s_Constructio_Latin_title_page.jpg" alt="" height="650">

**[Figure 14](#image-title-page-of-napier-s-1619-mirifici-logarithmorum-canonis-constructio). Title page of Napier's 1619 Mirifici logarithmorum canonis constructio**. [Source](https://commons.wikimedia.org/wiki/File:Napier's\_Constructio\_Latin\_title\_page.jpg).

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

The [natural logarithm](#natural-logarithm) $\ln x$ is the [logarithm](#logarithm) with base [Euler's number](#e-mathematical-constant), and the [inverse function](function.md#inverse-function) of the real [exponential function](#exponential-function). A particularly geometric definition is

$$
\ln x=\int_1^x\frac{dt}{t},\qquad x>0.
$$

For $x>1$, it is the [area](differential-geometry.md#surface-area) under the [hyperbola](geometry-and-topology.md#hyperbola) $y=1/t$ from $1$ to $x$. For $0<x<1$, the reversed [integration](#integral) limits give a negative value. The [fundamental theorem of calculus](#fundamental-theorem-of-calculus) gives $(\ln x)'=1/x$, so the [natural logarithm](#natural-logarithm) is increasing, while $(\ln x)''=-1/x^2$ gives [concavity](real-analysis.md#concave-function).

<a id="image-exponential-function-and-natural-logarithm-graphs-reflect-across-y-x-equal-multiplicative-intervals-have-equal-logarithmic-areas"></a>
![](exponential-logarithm-geometry.png)

**[Figure 15](#image-exponential-function-and-natural-logarithm-graphs-reflect-across-y-x-equal-multiplicative-intervals-have-equal-logarithmic-areas). Exponential function and natural logarithm graphs reflect across $y=x$; equal multiplicative intervals have equal logarithmic areas**.

The [change of variables](#change-of-variables-formula) $t=au$ shows $\int_a^{ab}dt/t=\int_1^bdu/u=\ln b$ for $a,b>0$. Thus the intervals from $1$ to $2$ and from $2$ to $4$ each contribute [area](differential-geometry.md#surface-area) $\ln2$, explaining $\ln4=2\ln2$. Equal ratios give equal increments on a [logarithmic scale](#logarithmic-scale), even though the ordinary differences grow. This makes the [natural logarithm](#natural-logarithm) useful for comparing multiplicative changes and solving for time in [exponential growth](#exponential-growth) or [exponential decay](analysis.md#exponential-decay). The [integral](#integral) construction and [inverse function](function.md#inverse-function) properties are discussed in [OpenStax, the natural logarithm as an integral](https://openstax.org/books/calculus-volume-1/pages/6-7-integrals-exponential-functions-and-logarithms).

#### Logarithmic scale

↑ **Parent:** [Logarithm](#logarithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_scale)

A scale whose coordinate is a [logarithm](#logarithm) of a positive quantity. Equal ratios occupy equal coordinate intervals; for example, $1,2,4,8$ are equally spaced under the [natural logarithm](#natural-logarithm) because every successive difference is $\ln2$.

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

[Hyperbolic functions](#hyperbolic-function) combine the [exponential function](#exponential-function) to describe a [hyperbola](geometry-and-topology.md#hyperbola) much as [trigonometric functions](geometry-and-topology.md#trigonometric-function) describe a [circle](topology.md#circle). Their two basic members are the [hyperbolic cosine](#hyperbolic-cosine) and [hyperbolic sine](#hyperbolic-sine), defined for every [real number](arithmetic.md#real-number) $t$ by

$$
\cosh t=\frac{e^t+e^{-t}}2,\qquad \sinh t=\frac{e^t-e^{-t}}2.
$$

Their [derivatives](#derivative) exchange the two [functions](function.md):

$$
\frac{d}{dt}\cosh t=\sinh t,\qquad \frac{d}{dt}\sinh t=\cosh t.
$$

These formulas follow by applying [differentiation](#differentiation) to the [exponential function](#exponential-function) definitions. [Gilbert Strang and Edwin Herman, OpenStax Calculus Volume 2, §2.9: hyperbolic definitions and derivatives](https://openstax.org/books/calculus-volume-2/pages/2-9-calculus-of-the-hyperbolic-functions)

Adding and subtracting gives $\cosh t+\sinh t=e^t$ and $\cosh t-\sinh t=e^{-t}$. Multiplying these equalities proves the [hyperbolic Pythagorean identity](#hyperbolic-pythagorean-identity):

$$
\boxed{\cosh^2t-\sinh^2t=1.}
$$

Consequently the [parametric equation](geometry-and-topology.md#parametric-equation) $(x,y)=(\cosh t,\sinh t)$ traverses the entire right branch of the unit [hyperbola](geometry-and-topology.md#hyperbola) $x^2-y^2=1$, where $x\geq1$. For example, $t=0$ gives $(1,0)$, while $t=\pm1$ gives approximately $(1.543,\pm1.175)$. Compare $(\cos\theta,\sin\theta)$ on the [unit circle](complex-analysis.md#complex-unit-circle), where the squared coordinates add to one. The minus sign changes the geometry from a closed [circle](topology.md#circle) to an unbounded [hyperbola](geometry-and-topology.md#hyperbola).

<a id="image-hyperbolic-cosine-and-sine-become-the-coordinates-of-the-right-branch-of-a-unit-hyperbola"></a>
![](hyperbolic-functions-and-unit-hyperbola.png)

**[Figure 16](#image-hyperbolic-cosine-and-sine-become-the-coordinates-of-the-right-branch-of-a-unit-hyperbola). Hyperbolic cosine and sine become the coordinates of the right branch of a unit hyperbola**. The same inputs $t=-1,0,1$ are marked on both [function](function.md) graphs and the unit [hyperbola](geometry-and-topology.md#hyperbola). The shaded region has [area](differential-geometry.md#surface-area) $1/2$ and corresponds to [hyperbolic angle](#hyperbolic-angle) $t=1$.

The other members are ratios and reciprocals: [hyperbolic tangent](#hyperbolic-tangent) is $\tanh t=\sinh t/\cosh t$, [hyperbolic cotangent](#hyperbolic-cotangent) is $\coth t=\cosh t/\sinh t$, and [hyperbolic secant](#hyperbolic-secant) is $\operatorname{sech}t=1/\cosh t$; denominators must be nonzero. The [hyperbolic sine](#hyperbolic-sine) and [hyperbolic cosine](#hyperbolic-cosine) both solve the [second-order linear differential equation](differential-equation.md#second-order-linear-differential-equation) $f''=f$. In fact $f(t)=A\cosh t+B\sinh t$ has $f(0)=A$ and $f'(0)=B$, making this [basis](vector-space.md#basis) convenient for an [initial value problem](differential-equation.md#initial-value-problem). Their geometry also makes [hyperbolic substitution](#hyperbolic-substitution) useful for [integrals](#integral) containing $\sqrt{1+u^2}$, and the [hyperbolic cosine](#hyperbolic-cosine) gives the physical [catenary](analysis.md#catenary) of a hanging chain.

#### Hyperbolic angle

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

A [hyperbolic angle](#hyperbolic-angle) $t$ is twice the signed [area](differential-geometry.md#surface-area) $A$ enclosed by the two rays from the origin to $(1,0)$ and $(\cosh t,\sinh t)$ and the intervening arc of the unit [hyperbola](geometry-and-topology.md#hyperbola). Counterclockwise traversal is positive: $t>0$ gives an ordinary [area](differential-geometry.md#surface-area) $t/2$ above the horizontal axis, and $t<0$ gives signed [area](differential-geometry.md#surface-area) $t/2$ below it. This parallels the [unit circle](complex-analysis.md#complex-unit-circle), whose sector has [area](differential-geometry.md#surface-area) $\theta/2$ for an [angle](geometry-and-topology.md#angle) $\theta$ measured in [radians](geometry-and-topology.md#radian).

To check the [area](differential-geometry.md#surface-area) interpretation, write $x(u)=\cosh u$ and $y(u)=\sinh u$. [Green's theorem](#green-theorem) expresses the signed [area](differential-geometry.md#surface-area) as a [line integral](#line-integral); the straight radial edges contribute zero, leaving

$$
A(t)=\frac12\int_0^t\bigl(x(u)y'(u)-y(u)x'(u)\bigr)\,du=\frac12\int_0^t\bigl(\cosh^2u-\sinh^2u\bigr)\,du=\frac t2.
$$

Thus $t$ is an [area](differential-geometry.md#surface-area) parameter, rather than the ordinary [angle](geometry-and-topology.md#angle) of the ray. For $t>0$, that ordinary [angle](geometry-and-topology.md#angle) is $\arctan(\tanh t)$; it stays below $\pi/4$ even as the [hyperbolic angle](#hyperbolic-angle) grows without bound.

#### Inverse hyperbolic functions

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_hyperbolic_functions)

The inverse hyperbolic functions invert the [hyperbolic functions](#hyperbolic-function), with real branches on their standard ranges and complex branches obtained through [analytic continuation](complex-analysis.md#analytic-continuation). For example, $\operatorname{arsinh}z=\log(z+\sqrt{z^2+1})$ on a chosen branch; the [multivalued inverse hyperbolic sine](complex-analysis.md#multivalued-inverse-hyperbolic-sine) records all inverse values.

#### Hyperbolic cosine

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The [hyperbolic cosine](#hyperbolic-cosine) is the [even function](#even-function)

$$
\cosh x=\frac{e^x+e^{-x}}2.
$$

It has [derivative](#derivative) $\sinh x$ and second [derivative](#derivative) $\cosh x>0$, so it is a strictly [convex function](real-analysis.md#convex-function). Its unique [global minimum](analysis.md#global-minimum) is $\cosh0=1$, and its [image](set-theory.md#image-of-a-function) is $[1,\infty)$. For example, $\cosh(-1)=\cosh1\approx1.543081$. On the unit [hyperbola](geometry-and-topology.md#hyperbola), the [hyperbolic cosine](#hyperbolic-cosine) is the horizontal coordinate; as a graph against $x$, it is a symmetric bowl.

Its [Taylor series](#taylor-series) begins

$$
\cosh x=1+\frac{x^2}{2!}+\frac{x^4}{4!}+\cdots.
$$

The positive fourth-order term explains why the bowl resembles a [parabola](geometry-and-topology.md#parabola) near its minimum yet differs from one away from it. Restricting to $x\geq0$ gives the [inverse hyperbolic cosine](#inverse-hyperbolic-cosine).

##### Catenary from hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](#hyperbolic-cosine)

A [catenary](analysis.md#catenary) is the static shape of an ideal flexible, inextensible chain hanging under its own [gravitational weight](classical-mechanics.md#weight-physics) in a [uniform gravitational field](classical-mechanics.md#uniform-gravitational-field), with uniform [linear mass density](fluid-mechanics.md#linear-mass-density) along its [arc length](riemannian-geometry.md#arc-length). With the lowest point above $x=0$, one convenient vertical origin gives

$$
y(x)=a\cosh(x/a),\qquad a>0.
$$

Here $a$ has units of [length](physics.md#length). The supports and the chain's [arc length](riemannian-geometry.md#arc-length) determine the scale and position; horizontal and vertical shifts give the general [catenary](analysis.md#catenary). [Robert Hunt, Cambridge Mathematical Methods II: worked example, The Catenary](https://www.damtp.cam.ac.uk/user/reh10/lectures/nst-mmii-handout3.pdf)

For $a=1$, the three points at $x=-1,0,1$ have heights $\cosh1\approx1.543081$, $1$, and $\cosh1\approx1.543081$. If heights should instead be measured from the lowest point, subtract $a$:

$$
y_{\mathrm{shifted}}(x)=a\bigl(\cosh(x/a)-1\bigr).
$$

The same three heights are then approximately $0.543081$, $0$, and $0.543081$. The shift changes the vertical origin and preserves the [catenary](analysis.md#catenary) shape.

<a id="image-a-hanging-chain-follows-a-scaled-hyperbolic-cosine-with-an-optional-shift-of-its-lowest-point-to-zero"></a>
![](hyperbolic-cosine-catenary.png)

**[Figure 17](#image-a-hanging-chain-follows-a-scaled-hyperbolic-cosine-with-an-optional-shift-of-its-lowest-point-to-zero). A hanging chain follows a scaled hyperbolic cosine, with an optional shift of its lowest point to zero**. The left panel marks $x=-1,0,1$ on $y=\cosh x$. The right panel puts the lowest point at zero, compares three positive scales $a$, and shows the local [parabola](geometry-and-topology.md#parabola) $y=x^2/2$ for $a=1$.

The scale also measures [tension](classical-mechanics.md#tension): if $H>0$ is its constant horizontal component, $\mu$ is the [linear mass density](fluid-mechanics.md#linear-mass-density), and $g$ is the magnitude of [gravitational acceleration](classical-mechanics.md#gravitational-acceleration), then $a=H/(\mu g)$. A short [force](classical-mechanics.md#force) balance explains this. For the portion from the lowest point to $x\geq0$, with [arc length](riemannian-geometry.md#arc-length) $s(x)$, vertical [tension](classical-mechanics.md#tension) balances its [gravitational weight](classical-mechanics.md#weight-physics) and horizontal [tension](classical-mechanics.md#tension) gives

$$
Hy'(x)=\mu g\,s(x),\qquad s'(x)=\sqrt{1+y'(x)^2}.
$$

Applying [differentiation](#differentiation) yields $ay''=\sqrt{1+y'^2}$. The proposed [hyperbolic cosine](#hyperbolic-cosine) solves this [differential equation](differential-equation.md), because $y'=\sinh(x/a)$ and $ay''=\cosh(x/a)=\sqrt{1+\sinh^2(x/a)}$. This is the mechanism behind the shape, under the stated ideal chain assumptions.

The same identity simplifies the [arc length](riemannian-geometry.md#arc-length) between symmetric supports at $x=\pm b$:

$$
L=\int_{-b}^b\sqrt{1+y'(x)^2}\,dx=\int_{-b}^b\cosh(x/a)\,dx=2a\sinh(b/a).
$$

For $a=b=1$, $L\approx2.350402$, exceeding the horizontal span of two. A larger $a$ at fixed $b$ gives a shallower sag: the [Taylor series](#taylor-series) gives $a(\cosh(x/a)-1)=x^2/(2a)+x^4/(24a^3)+\cdots$. Thus a [parabola](geometry-and-topology.md#parabola) is a local approximation, while the exact ideal chain shape is a [catenary](analysis.md#catenary). The useful connection is that the same [hyperbolic Pythagorean identity](#hyperbolic-pythagorean-identity) controls its coordinates, [force](classical-mechanics.md#force) balance, and [arc length](riemannian-geometry.md#arc-length).

##### Factorial-tail irrationality proof for a hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](#hyperbolic-cosine)

For a fixed positive integer $q$, $\cosh(1/q)=\sum_{k\ge0}q^{-2k}/(2k)!$ is irrational. If it were rational with denominator $b$, choose $N$ large enough that $b\mid(2N)!$. After multiplication by $q^{2N}(2N)!$, the finite partial sum is an integer and the remaining positive tail is bounded by a geometric series whose ratio is at most $1/[q^2(2N+1)(2N+2)]$. For sufficiently large $N$, this tail is strictly between zero and one, contradicting its integer value. Only a finite integer partial sum is used; convergence of an infinite series of rationals does not itself prove irrationality.

##### Inverse hyperbolic cosine

↑ **Parent:** [Hyperbolic cosine](#hyperbolic-cosine)

For $x\geq1$, the inverse [hyperbolic cosine](#hyperbolic-cosine) on its nonnegative real branch is $\operatorname{arcosh}x=\log(x+\sqrt{x^2-1})$. It is the real cosine member of the [inverse hyperbolic functions](#inverse-hyperbolic-functions).

#### Hyperbolic sine

↑ **Parent:** [Hyperbolic function](#hyperbolic-function)

The [hyperbolic sine](#hyperbolic-sine) is the [odd function](#odd-function)

$$
\sinh x=\frac{e^x-e^{-x}}2.
$$

Its [derivative](#derivative) is $\cosh x\geq1$, so it increases strictly from $-\infty$ to $\infty$ and is a [bijection](function.md#bijection) of $\mathbb R$ onto itself. For example, $\sinh0=0$, $\sinh1\approx1.175201$, and $\sinh(-1)\approx-1.175201$. It is the vertical coordinate on the unit [hyperbola](geometry-and-topology.md#hyperbola) parametrized by $(\cosh x,\sinh x)$.

The [Taylor series](#taylor-series)

$$
\sinh x=x+\frac{x^3}{3!}+\frac{x^5}{5!}+\cdots
$$

shows that $\sinh x\approx x$ near zero. Its [tangent line](#tangent-line) there is $y=x$; unlike the ordinary [sine](geometry-and-topology.md#sine), the [hyperbolic sine](#hyperbolic-sine) grows without bound. Its [antiderivative](#antiderivative) is $\cosh x+C$. In the [catenary](analysis.md#catenary) $y=a\cosh(x/a)$, the [hyperbolic sine](#hyperbolic-sine) gives both the slope, through the [derivative](#derivative) $y'=\sinh(x/a)$, and the [arc length](riemannian-geometry.md#arc-length) $s(x)=a\sinh(x/a)$ from the lowest point for $x\geq0$.

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

The fundamental theorem of calculus says that **accumulation and local change undo one another**, under appropriate regularity conditions. If $f$ is a [continuous function](#continuous-function) on $[a,b]$ and

$$
A(x)=\int_a^x f(t)\,dt,
$$

then $A$ is [differentiable](analysis.md#differentiable-function) for $a<x<b$ and $A'(x)=f(x)$. Conversely, if $G$ is an [antiderivative](#antiderivative) of $f$ on this [interval](real-analysis.md#interval-mathematics), continuous at its endpoints, then

$$
\boxed{\int_a^b f(x)\,dx=G(b)-G(a).}
$$

The first statement turns an [integral](#integral) into a [function](function.md) with a known [derivative](#derivative); the second turns an entire accumulation into two endpoint values.

For $f(t)=1+2t$, accumulation from zero gives $A(x)=x+x^2$. At $x=2$, its [derivative](#derivative) is $A'(2)=5$, exactly the current value $f(2)$. The accumulated value there is $A(2)=6$, and by $x=3$ it has reached $A(3)=12$. The accumulated quantity and its rate are different [functions](function.md), linked by [differentiation](#differentiation).

<a id="image-the-instantaneous-rate-determines-the-tangent-to-the-accumulation-curve"></a>
![](fundamental-theorem-calculus.png)

**[Figure 18](#image-the-instantaneous-rate-determines-the-tangent-to-the-accumulation-curve). The instantaneous rate determines the tangent to the accumulation curve**.

This connection makes the theorem useful far beyond geometric [area](differential-geometry.md#surface-area). It recovers [displacement](classical-mechanics.md#displacement) from [velocity](classical-mechanics.md#velocity), gives a [probability](probability-theory.md#probability) from a [probability density function](continuous-probability-distribution.md#probability-density-function), and converts many [differential equations](differential-equation.md) into [integral equations](analysis.md#integral-equation). The striking economy is that information spread across a whole [interval](real-analysis.md#interval-mathematics) can sometimes be recovered from an [antiderivative](#antiderivative) at its two boundaries.

A short explanation of the first part is that

$$
\frac{A(x+h)-A(x)}h=\frac1h\int_x^{x+h}f(t)\,dt
$$

is the local average of $f$. [Continuity](#continuous-function) makes this average approach $f(x)$. For the second part, $G-A$ has zero [derivative](#derivative) and is constant by the [mean value theorem](#mean-value-theorem). These are the ideas behind the proof; the endpoint and regularity conditions make them valid.

An early geometric form of this connection appears in Isaac Barrow's _Lectiones geometricae_ (1670), Lecture X, Proposition 11. The original volume is catalogued by CESIMA, and Michael Nauenberg's historical research reproduces and examines the geometric argument.[Isaac Barrow, Lectiones geometricae, 1670](https://cesimadigital.pucsp.br/handle/bcd/3675)[Michael Nauenberg, Barrow and Leibniz on the fundamental theorem of the calculus, 2011](https://arxiv.org/abs/1111.6145)

### Fundamental theorem of calculus for Lebesgue integration

↑ **Parent:** [Fundamental theorem of calculus](#fundamental-theorem-of-calculus)

If $g\in L^1(a,b)$, then $F(x)=F(a)+\int_a^xg(s)\,ds$ is [absolutely continuous](sobolev-space.md#absolutely-continuous-function) and satisfies $F'=g$ [almost everywhere](measure-theory.md#almost-everywhere). Conversely, every absolutely continuous function has this form.

## Mean value theorem

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_value_theorem)

The [mean value theorem](#mean-value-theorem) says that an average rate of change is attained as an instantaneous rate somewhere between the endpoints. Let $a<b$ and let the [real-valued function](function.md#real-valued-function) $f:[a,b]\to\mathbb R$ be [continuous](#continuous-function) on the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$ and [differentiable](analysis.md#differentiable-function) on the [open interval](topology.md#open-interval) $(a,b)$. Then there exists $c\in(a,b)$ such that

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

The right-hand side is the [slope](geometry-and-topology.md#slope) of the [secant line](geometry-and-topology.md#secant-line) joining $(a,f(a))$ to $(b,f(b))$; the left-hand side is the [slope](geometry-and-topology.md#slope) of the [tangent line](#tangent-line) at $(c,f(c))$. The [derivative](#derivative) need not be [continuous](#continuous-function), and the [function](function.md) need not be [differentiable](analysis.md#differentiable-function) at the endpoints. [OpenStax, Calculus Volume 1, Section 4.4: mean value theorem](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem)

For the [polynomial](polynomial.md) $f(x)=x^2$ on $[1,3]$, the [secant line](geometry-and-topology.md#secant-line) has [slope](geometry-and-topology.md#slope) $(9-1)/(3-1)=4$. Since the [derivative](#derivative) is $f'(x)=2x$, the required interior point is $c=2$. The [tangent line](#tangent-line) there is $y=4+4(x-2)=4x-4$, whereas the [secant line](geometry-and-topology.md#secant-line) is $y=1+4(x-1)=4x-3$. Their equal [slopes](geometry-and-topology.md#slope) make them parallel, but they are distinct [straight lines](geometry-and-topology.md#straight-line): the theorem equates rates, not heights.

<a id="image-the-secant-line-and-interior-tangent-line-to-x-2-have-equal-slopes-but-different-heights"></a>
![](mean-value-theorem-secant-and-tangent.png)

**[Figure 19](#image-the-secant-line-and-interior-tangent-line-to-x-2-have-equal-slopes-but-different-heights). The secant line and interior tangent line to $x^2$ have equal slopes but different heights**.

The practical strength is that the unknown point $c$ can disappear from an estimate. Under the same hypotheses, if the [derivative](#derivative) satisfies $|f'(x)|\leq M$ throughout $(a,b)$, where $M\geq0$, then

$$
|f(b)-f(a)|=|f'(c)|\,|b-a|\leq M|b-a|.
$$

Applying this to every subinterval proves [Lipschitz continuity](real-analysis.md#lipschitz-continuity) with [Lipschitz bound](real-analysis.md#lipschitz-bound) $M$. For example, $f(x)=x^2$ on $[1,3]$ has $|f'(x)|\leq6$, so an input change of size at most $\delta$ changes its output by at most $6\delta$, as long as both inputs lie in that [interval](real-analysis.md#interval-mathematics). A local [derivative](#derivative) bound therefore controls finite changes without computing an [integral](#integral). The sign of the [derivative](#derivative) similarly gives the [derivative criterion for monotonicity](#derivative-criterion-for-monotonicity).

Taking $M=0$ shows that a [function](function.md) with zero [derivative](#derivative) throughout a [real interval](real-analysis.md#interval-mathematics) is a [constant function](function.md#constant-function), provided it is [continuous](#continuous-function) at any included endpoints. The [interval](real-analysis.md#interval-mathematics) condition is essential: on the [domain of a function](function.md#domain-of-a-function) $(-2,-1)\cup(1,2)$, the [function](function.md) equal to zero on the left [interval](real-analysis.md#interval-mathematics) and one on the right [interval](real-analysis.md#interval-mathematics) has zero [derivative](#derivative) everywhere. It is a [locally constant function](#locally-constant-function), yet not a [constant function](function.md#constant-function) on the whole [domain of a function](function.md#domain-of-a-function). The [mean value theorem](#mean-value-theorem) cannot cross the gap.

A concise proof subtracts the [secant line](geometry-and-topology.md#secant-line): set $m=(f(b)-f(a))/(b-a)$ and $h(x)=f(x)-f(a)-m(x-a)$. Then $h(a)=h(b)=0$, and [Rolle's theorem](#rolle-theorem) gives an interior point with $h'(c)=f'(c)-m=0$. The geometric idea is to remove the average trend and find a horizontal [tangent line](#tangent-line) in what remains.

### Cauchy mean value theorem

↑ **Parent:** [Mean value theorem](#mean-value-theorem)

For $a<b$ and [real-valued functions](function.md#real-valued-function) $f,g$ that are [continuous](#continuous-function) on the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$ and [differentiable](analysis.md#differentiable-function) on the [open interval](topology.md#open-interval) $(a,b)$, there exists $\xi\in(a,b)$ with

$$
[f(b)-f(a)]g'(\xi)=[g(b)-g(a)]f'(\xi).
$$

Apply [Rolle's theorem](#rolle-theorem) to the [linear combination](vector-space.md#linear-combination) $h(x)=[f(b)-f(a)]g(x)-[g(b)-g(a)]f(x)$, which has equal endpoint values. The displayed product identity permits zero [derivatives](#derivative). For the ratio form, additionally assume $g'(x)\ne0$ for every $x\in(a,b)$. Then [Rolle's theorem](#rolle-theorem) ensures $g(b)\ne g(a)$, so both denominators below are nonzero:

$$
\frac{f(b)-f(a)}{g(b)-g(a)}=\frac{f'(\xi)}{g'(\xi)}.
$$

Neither [derivative](#derivative) needs to be [continuous](#continuous-function), and $f'$ may vanish. Choosing $g(x)=x$ recovers the [mean value theorem](#mean-value-theorem); the ratio form also gives the zero-over-zero endpoint case of [L'Hôpital's rule](#l-hopital-s-rule). [Jiří Lebl, Basic Analysis I, Section 4.2, Theorem 4.2.5](https://www.jirka.org/ra/html/sec_mvt.html)

### Endpoint secant-tangent approximation

↑ **Parent:** [Mean value theorem](#mean-value-theorem)

If $f$ is continuous at an interval endpoint, differentiable in its interior, and has a finite one-sided derivative there, then its secant slope and tangent slope are arbitrarily close at some interior point. Apply the [mean value theorem](#mean-value-theorem) on a short endpoint interval; both the secant at its far endpoint and the secant at the resulting intermediate point approach the same one-sided derivative. No continuity of the derivative is required.

## Rolle theorem

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rolle_theorem)

[Rolle's theorem](#rolle-theorem) is the equal-endpoint case of the [mean value theorem](#mean-value-theorem). Let $a<b$ and let the [real-valued function](function.md#real-valued-function) $f:[a,b]\to\mathbb R$ be [continuous](#continuous-function) on the [closed interval](real-analysis.md#closed-real-interval) $[a,b]$ and [differentiable](analysis.md#differentiable-function) on the [open interval](topology.md#open-interval) $(a,b)$. If $f(a)=f(b)$, there exists $c\in(a,b)$ with $f'(c)=0$. Geometrically, a [tangent line](#tangent-line) somewhere in the [interior](topology.md#interior-topology) is horizontal, like the [secant line](geometry-and-topology.md#secant-line) joining the endpoints. [OpenStax, Calculus Volume 1, Section 4.4: Rolle's theorem](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem)

For the [polynomial](polynomial.md) $f(x)=x(x-2)$ on $[0,2]$, both endpoint values are zero and the [derivative](#derivative) is $f'(x)=2x-2$. Thus $c=1$, where $f(1)=-1$, and the horizontal [tangent line](#tangent-line) is $y=-1$. The horizontal [secant line](geometry-and-topology.md#secant-line) is $y=0$: equal endpoint values do not force the interior [tangent line](#tangent-line) to pass through those endpoints.

The [absolute value function](real-analysis.md#absolute-value) $f(x)=|x|$ on $[-1,1]$ exposes the importance of [differentiability](analysis.md#differentiability). It is [continuous](#continuous-function) and $f(-1)=f(1)=1$, so the [secant line](geometry-and-topology.md#secant-line) has [slope](geometry-and-topology.md#slope) zero. However,

$$
f'(x)=\begin{cases}-1,&-1<x<0,\\1,&0<x<1,\end{cases}
$$

and the [derivative](#derivative) does not exist at zero because the [one-sided derivatives](#one-sided-derivative) disagree. Every existing [derivative](#derivative) in the [interior](topology.md#interior-topology) is nonzero. The corner fails a hypothesis of both [Rolle's theorem](#rolle-theorem) and the [mean value theorem](#mean-value-theorem), so neither conclusion is guaranteed.

<a id="image-rolle-s-theorem-gives-a-horizontal-tangent-line-for-a-polynomial-while-a-corner-defeats-differentiability"></a>
![](rolle-theorem-and-corner-counterexample.png)

**[Figure 20](#image-rolle-s-theorem-gives-a-horizontal-tangent-line-for-a-polynomial-while-a-corner-defeats-differentiability). Rolle's theorem gives a horizontal tangent line for a polynomial, while a corner defeats differentiability**.

For a short proof, the [extreme value theorem](real-analysis.md#extreme-value-theorem) supplies a greatest and a least value on $[a,b]$. If $f$ is a [constant function](function.md#constant-function), every interior point works. Otherwise at least one of these values differs from the common endpoint value, so it is attained at an interior [extremum](mathematical-optimization.md#maximum-and-minimum). At an interior [local maximum](analysis.md#local-maximum) or [local minimum](analysis.md#local-minimum), [differentiability](analysis.md#differentiability) forces the [derivative](#derivative) to be zero: the [difference quotients](#difference-quotient) from the two sides have opposite weak signs and the same [limit](#limit-of-a-function).

This turns repeated values into information about [derivatives](#derivative). Two distinct [roots of a polynomial](polynomial.md#root-of-a-polynomial) force a root of its [derivative](#derivative) between them; iterating this idea gives the [Rolle root count with multiplicities](#rolle-root-count-with-multiplicities). More generally, a [differentiable function](analysis.md#differentiable-function) with nonzero [derivative](#derivative) throughout a [real interval](real-analysis.md#interval-mathematics) cannot repeat a value there, hence is [injective](algebra.md#injective-function). The beauty is that knowing only two equal values guarantees an exact local feature somewhere between them.

### Rolle root count with multiplicities

↑ **Parent:** [Rolle theorem](#rolle-theorem)

If a nonzero real [polynomial](polynomial.md) has $N$ roots in an open real interval, counted with [multiplicity of a root](polynomial.md#multiplicity-of-a-root), its derivative has at least $N-1$ roots in that interval, also counted with multiplicity, provided $N\ge1$. Each root of multiplicity $m$ becomes a root of the derivative of multiplicity $m-1$. The [Rolle theorem](#rolle-theorem) supplies one further root between each pair of distinct consecutive roots. Thus $k$ distinct roots of multiplicities $m_j$ give at least $\sum_j(m_j-1)+(k-1)=N-1$ derivative roots.

<h2 id="taylor-s-theorem">Taylor's theorem</h2>

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor's_theorem)

[Taylor's theorem](#taylor-s-theorem) expresses a sufficiently [differentiable function](analysis.md#differentiable-function) as a finite [Taylor polynomial](#taylor-polynomial) plus a [Taylor remainder](#taylor-remainder). One convenient version assumes $f$ is $n+1$ times continuously [differentiable](analysis.md#differentiable-function) on the segment between $a$ and $x$. Then

$$
f(x)=T_{n,a}(x)+R_{n,a}(x),\qquad R_{n,a}(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-a)^{n+1}
$$

for some intermediate point $\xi$, when $x\ne a$. Thus a bound $|f^{(n+1)}|\leq M$ on that segment gives $|R_{n,a}(x)|\leq M|x-a|^{n+1}/(n+1)!$. The intermediate point usually need not be computed: bounding the [derivative](#derivative) throughout the segment is enough. This is why local approximation can yield reliable numerical bounds. A finite [Taylor polynomial](#taylor-polynomial) does not require an infinite [Taylor series](#taylor-series) to represent the [function](function.md).

Historically, the Royal Society holds [Brook Taylor](mathematics.md#brook-taylor)'s letter of 26 July 1712 to John Machin. Its catalogue connects his work on [Kepler's second law](physics.md#kepler-s-second-law) with the expansion later published in the 1715 Methodus incrementorum directa et inversa. This is a documented route from an orbital calculation to a general approximation method, rather than a claim that every earlier use of such expansions began with Taylor. See [Royal Society archive, letter MS/82/2](https://catalogues.royalsociety.org/calmview/Record.aspx?id=MS%2F82%2F2&src=CalmView.Catalog).

### Taylor expansion from a periodic derivative equation

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

For a smooth real [function](function.md) satisfying the displayed equation with positive [integer](number-theory.md#integer) $r$, differentiating makes $f^{(j+r)}=f^{(j)}$. On any [compact](topology.md#compact-space) interval, all [derivatives](#derivative) are therefore bounded by the maximum of the bounds of $f,f',\ldots,f^{(r-1)}$. The [Taylor formula with integral remainder](#taylor-formula-with-integral-remainder) consequently has error at most $M R^{n+1}/(n+1)!$, which tends to zero uniformly for $|x|\le R$. Hence the [function](function.md) equals its globally convergent [Taylor series](#taylor-series). For $r=3$ and initial [derivatives](#derivative) $(1,0,0)$, it is $\sum_{k\ge0}x^{3k}/(3k)!$.

### Integral first-order Taylor formula for a vector map

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

For a continuously differentiable [vector-valued function](function.md#vector-valued-function) whose domain contains the segment from $x$ to $x+h$, apply the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) componentwise to $t\mapsto F(x+th)$. The resulting integral matrix is valid even when there is no common intermediate point giving a vector mean-value formula. For a [score function](statistical-modelling.md#informant-function), it integrates the [Hessian matrix](#hessian-matrix) along the segment to a candidate estimate.

### Integral remainder in Taylor theorem

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

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

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

A Taylor expansion about a point consists of successive derivative terms there, together with either a finite remainder or an infinite [Taylor series](#taylor-series) when that series represents the function.

#### Peano zero

↑ **Parent:** [Taylor expansion](#taylor-expansion)

A Peano zero through order $r$ means that the [function](function.md) admits the zero [Taylor polynomial](#taylor-polynomial) with remainder $o(|t|^r)$ at $x_0$. This does not assert the existence of ordinary iterated [derivatives](#derivative) on a neighborhood. For example, multiplying $t^{r+1}$ by a bounded [continuous function](#continuous-function) with [dense](topology.md#dense-set) points of nondifferentiability preserves this estimate while destroying neighborhood [differentiability](analysis.md#differentiability).

#### Parabolic approximation

↑ **Parent:** [Taylor expansion](#taylor-expansion)

A parabolic approximation retains terms through second order in a local [Taylor expansion](#taylor-expansion). Near the closest point of a circle of radius $a$ and its tangent line, the separation is $x^2/(2a)+O(x^4/a^3)$.

### Taylor formula for a polynomial

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

For a polynomial $p$ of degree at most $m$, the Taylor formula is exact:

$$
p(t)=\sum_{j=0}^m\frac{p^{(j)}(x)}{j!}(t-x)^j.
$$

### Taylor theorem with Lagrange remainder

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

If $f$ is $n$ times differentiable between $a$ and $x$, then for some $\xi$ strictly between them,

$$
f(x)=\sum_{j=0}^{n-1}\frac{f^{(j)}(a)}{j!}(x-a)^j
+\frac{f^{(n)}(\xi)}{n!}(x-a)^n.
$$

### Taylor remainder

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

The Taylor remainder is the difference between a function and a finite [Taylor polynomial](#taylor-polynomial). Bounds on higher derivatives or their [Hölder continuity](sobolev-space.md#holder-condition) control this error.

### Taylor formula with integral remainder

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)

If $f^{(m-1)}$ is locally absolutely continuous, then its Taylor remainder can be written as an integral involving the weak derivative $f^{(m)}$. This form permits norm bounds when the highest derivative is only integrable.

### Taylor series

↑ **Parent:** [Taylor's theorem](#taylor-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_series)

For a [function](function.md) with [derivatives](#derivative) of every order at $a$, its [Taylor series](#taylor-series) is the [power series](real-analysis.md#power-series)

$$
\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n.
$$

Its [partial sums](real-analysis.md#partial-sum) are [Taylor polynomials](#taylor-polynomial). At $a=0$ it is called a [Maclaurin series](#maclaurin-series). Forming the coefficients, proving that its [partial sums](real-analysis.md#partial-sum) form a [convergent sequence](real-analysis.md#convergent-sequence), and proving that their [limit](#limit-of-a-function) equals $f(x)$ are separate tasks. A [smooth function](analysis.md#smooth-function) provides all the coefficients, but a [real analytic function](analysis.md#real-analytic-function) is additionally represented locally by the resulting [power series](real-analysis.md#power-series).

For the [exponential function](#exponential-function), every [derivative](#derivative) of $e^x$ at zero equals one, giving

$$
e^x=\sum_{n=0}^{\infty}\frac{x^n}{n!}.
$$

Here equality holds for every real $x$: the [Taylor remainder](#taylor-remainder) is bounded by $e^{|x|}|x|^{N+1}/(N+1)!$, which tends to zero for each fixed $x$. At $x=1$, the degree-five [Taylor polynomial](#taylor-polynomial) is $163/60\approx2.71666667$, and the absolute difference from $e$ is less than $e/720$. The [factorial](combinatorics.md#factorial) denominator eventually overwhelms every fixed power, allowing local [derivative](#derivative) information to reconstruct this [function](function.md) throughout the real line.

The [geometric series](real-analysis.md#geometric-series) shows why the region of validity matters. For $f(x)=1/(1-x)$, the [Taylor series](#taylor-series) at zero is $\sum_{k\geq0}x^k$, with [radius of convergence](real-analysis.md#radius-of-convergence) one. For $x\ne1$, its finite [Taylor polynomial](#taylor-polynomial) satisfies the exact identity

$$
\frac1{1-x}-\sum_{k=0}^N x^k=\frac{x^{N+1}}{1-x}.
$$

At $x=1/2$ and $N=5$, the remainder is $1/32$. At $x=0.9$, the same degree-five [polynomial](polynomial.md) has value $4.68559$ and remainder $5.31441$, although the [Taylor series](#taylor-series) still converges to $10$ there. Convergence of the infinite expression does not guarantee accuracy from a particular small number of terms. For $|x|>1$, even the terms fail to tend to zero, so this [power series](real-analysis.md#power-series) cannot represent the [function](function.md). The standard expansions and the conditions for [convergent series](real-analysis.md#convergent-series) are discussed in [OpenStax, working with Taylor series](https://openstax.org/books/calculus-volume-2/pages/6-4-working-with-taylor-series).

<a id="image-geometric-partial-sums-converge-slowly-near-their-convergence-boundary-while-a-smooth-flat-function-has-an-identically-zero-taylor-series"></a>
![](taylor-series-convergence-and-flatness.png)

**[Figure 21](#image-geometric-partial-sums-converge-slowly-near-their-convergence-boundary-while-a-smooth-flat-function-has-an-identically-zero-taylor-series). Geometric partial sums converge slowly near their convergence boundary, while a smooth flat function has an identically zero Taylor series**.

A stronger caution comes from the [flat function](analysis.md#flat-function)

$$
h(x)=\begin{cases}e^{-1/x^2},&x\ne0,\\0,&x=0.\end{cases}
$$

It is a [smooth function](analysis.md#smooth-function) with $h^{(n)}(0)=0$ for every $n$, so every [Taylor polynomial](#taylor-polynomial) at zero is zero and its [Taylor series](#taylor-series) converges everywhere to zero. Nevertheless $h(1/2)=e^{-4}>0$. Off zero, repeated [differentiation](#differentiation) produces a [polynomial](polynomial.md) in $1/x$ times $e^{-1/x^2}$; the exponential decay makes each required [limit](#limit-of-a-function) at zero vanish. This explains how all the local coefficients can miss a positive [function](function.md) arbitrarily close to the centre. [Real analyticity](analysis.md#real-analytic-function) supplies the additional condition that rules out this behavior.

#### Maclaurin series

↑ **Parent:** [Taylor series](#taylor-series)

A [Taylor series](#taylor-series) centred at zero. Its coefficients are the [derivatives](#derivative) there divided by the corresponding [factorials](combinatorics.md#factorial).

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

The [intermediate value theorem](#intermediate-value-theorem) says that a real-valued [continuous function](#continuous-function) cannot skip a value between two of its outputs. Let $a<b$ and let $f:[a,b]\to\mathbb R$ be a [continuous function](#continuous-function) on the entire [closed interval](real-analysis.md#closed-real-interval) $[a,b]$. Then

$$
\min\{f(a),f(b)\}\leq y\leq\max\{f(a),f(b)\}
\quad\Longrightarrow\quad
\text{there exists }c\in[a,b]\text{ with }f(c)=y.
$$

The word "between" includes both endpoint values: choose $c=a$ when $y=f(a)$, or $c=b$ when $y=f(b)$. If $y$ is strictly between them, every such $c$ lies in the [open interval](topology.md#open-interval) $(a,b)$. [Continuity](#continuous-function) on $[a,b]$ means [continuity](#continuous-function) at every interior point, together with the endpoint [one-sided limits](#one-sided-limit) $\lim_{x\to a^+}f(x)=f(a)$ and $\lim_{x\to b^-}f(x)=f(b)$. No [derivative](#derivative) is required.[§2.4, Continuity over an Interval and Theorem 2.11, The Intermediate Value Theorem](mathematics-bibliography.md#calculus-volume-1-by-gilbert-strang-and-others)

For finding a [zero of a function](polynomial.md#zero-of-a-function), the useful special case is

$$
f(a)f(b)<0\quad\Longrightarrow\quad
\text{there exists }c\in(a,b)\text{ with }f(c)=0.
$$

Strictly opposite endpoint signs certify a [root bracket](numerical-analysis.md#root-bracket), because zero is strictly between $f(a)$ and $f(b)$. If an endpoint value is already zero, that endpoint supplies a [zero of a function](polynomial.md#zero-of-a-function) directly; an interior [zero of a function](polynomial.md#zero-of-a-function) need not exist. For example, $f(x)=x$ on $[0,1]$ has its only [zero of a function](polynomial.md#zero-of-a-function) at the left endpoint. The [intermediate value theorem](#intermediate-value-theorem) guarantees existence, but neither uniqueness nor a necessary sign-change test. Its numerical usefulness is that the [bisection method](numerical-analysis.md#bisection-method) can turn existence into successively tighter [root brackets](numerical-analysis.md#root-bracket).

##### Intermediate value theorem hypotheses and counterexamples

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

Three explicit [functions](function.md) separate the hypotheses from the conclusion. These are original mathematical illustrations, not measured data.

The [polynomial function](polynomial.md#polynomial-function) $h(x)=x^3-x=x(x-1)(x+1)$ is a [continuous function](#continuous-function) on $[-3/2,3/2]$, with $h(-3/2)=-15/8$ and $h(3/2)=15/8$. The [intermediate value theorem](#intermediate-value-theorem) guarantees at least one [zero of a function](polynomial.md#zero-of-a-function) in the interior, while the [polynomial factorization](polynomial.md#factorization-of-polynomials) displays three: $-1,0,1$. Thus strict opposite signs do not establish uniqueness.

The everywhere-defined [function](function.md)

$$
j(x)=\begin{cases}-1,&-1\leq x<0,\\1,&0\leq x\leq1\end{cases}
$$

has $j(-1)=-1$ and $j(1)=1$, yet no [zero of a function](polynomial.md#zero-of-a-function). Its [jump discontinuity](#jump-discontinuity) at zero is exactly where the [continuity](#continuous-function) hypothesis fails. A drawn vertical connector would be misleading: the [function graph](function.md#graph-of-a-function) contains neither the intermediate heights nor a [zero of a function](polynomial.md#zero-of-a-function) at that jump. Even [continuity](#continuous-function) only on the interior is insufficient: setting $q(x)=-1$ for $0\leq x<1$ and $q(1)=1$ gives opposite endpoint signs on $[0,1]$ with no [zero of a function](polynomial.md#zero-of-a-function), because the left [one-sided limit](#one-sided-limit) at $1$ is not $q(1)$.

The [polynomial function](polynomial.md#polynomial-function) $t(x)=x^2$ on $[-1,1]$ is a [continuous function](#continuous-function), and $t(-1)=t(1)=1$, yet $t(0)=0$. Its [root of a polynomial](polynomial.md#root-of-a-polynomial) at zero has [multiplicity of a root](polynomial.md#multiplicity-of-a-root) two. The [function graph](function.md#graph-of-a-function) touches its horizontal [tangent line](#tangent-line) there and stays positive on both sides: existence of a [zero of a function](polynomial.md#zero-of-a-function) does not require a sign change. More generally, near a real [root of a polynomial](polynomial.md#root-of-a-polynomial) $r$, a [polynomial factorization](polynomial.md#factorization-of-polynomials) $p(x)=(x-r)^{2m}u(x)$ with $m\geq1$ and $u(r)\neq0$ has the same sign on both sides sufficiently close to $r$, since the [continuous function](#continuous-function) $u$ retains its sign. The [intermediate value theorem](#intermediate-value-theorem) does not rule out values outside the range between endpoint outputs.[§2.4, Example 2.37: positive endpoint values do not exclude an interior zero; Theorem 2.11 requires continuity on the whole interval](mathematics-bibliography.md#calculus-volume-1-by-gilbert-strang-and-others)

<a id="image-intermediate-value-hypotheses-three-continuous-roots-a-jump-with-no-root-and-a-double-root-without-a-sign-change"></a>
![](intermediate-value-continuous-jump-tangent.png)

**[Figure 22](#image-intermediate-value-hypotheses-three-continuous-roots-a-jump-with-no-root-and-a-double-root-without-a-sign-change). Intermediate value hypotheses: three continuous roots, a jump with no root, and a double root without a sign change**.

##### A cubic root from existence to a quantitative bracket

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

Consider the original worked example $f(x)=x^3+x-1$ on $[0,1]$. First, existence: a [polynomial function](polynomial.md#polynomial-function) is a [continuous function](#continuous-function), and $f(0)=-1<0<1=f(1)$. The [intermediate value theorem](#intermediate-value-theorem) therefore supplies a [zero of a function](polynomial.md#zero-of-a-function) $r\in(0,1)$, even before its value has been calculated.

Second, uniqueness is a separate argument. The [derivative](#derivative) is $f'(x)=3x^2+1>0$. The [derivative criterion for monotonicity](#derivative-criterion-for-monotonicity), obtained from the [mean value theorem](#mean-value-theorem), makes $f$ a [strictly increasing function](#strictly-increasing-function). Two distinct [zeros of a function](polynomial.md#zero-of-a-function) would contradict that strict increase. Thus this [root bracket](numerical-analysis.md#root-bracket) contains exactly one [zero of a function](polynomial.md#zero-of-a-function); indeed the same [derivative](#derivative) argument proves uniqueness on the entire [real line](real-analysis.md#real-line).

Third, localization uses the existing [bisection method](numerical-analysis.md#bisection-method). Set $[a_0,b_0]=[0,1]$; after $k$ completed halvings, retain $[a_k,b_k]$ with opposite endpoint signs. Each update tests the old [midpoint](mathematical-optimization.md#midpoint) $m_{k-1}=(a_{k-1}+b_{k-1})/2$. The first five exact updates are

$$
\begin{array}{c|c|r|c}
k&\text{tested }m_{k-1}&f(m_{k-1})&\text{retained }[a_k,b_k]\\\hline
1&1/2&-3/8&[1/2,1]\\
2&3/4&11/64&[1/2,3/4]\\
3&5/8&-67/512&[5/8,3/4]\\
4&11/16&51/4096&[5/8,11/16]\\
5&21/32&-2003/32768&[21/32,11/16]
\end{array}
$$

Every retained [root bracket](numerical-analysis.md#root-bracket) contains $r$ by the [intermediate value theorem](#intermediate-value-theorem). After ten halvings, exact arithmetic gives

$$
a_{10}=\frac{349}{512},\qquad b_{10}=\frac{699}{1024},\qquad
f(a_{10})=-\frac{220923}{134217728}<0,
\qquad f(b_{10})=\frac{744899}{1073741824}>0.
$$

Hence $0.681640625<r<0.6826171875$. The new [midpoint](mathematical-optimization.md#midpoint) and its [bisection error bound](numerical-analysis.md#bisection-error-bound) are

$$
m_{10}=\frac{1397}{2048}=0.68212890625,\qquad
|m_{10}-r|\leq\frac{1}{2048}=0.00048828125.
$$

This [midpoint](mathematical-optimization.md#midpoint) is the estimate after the tenth update; the last tested point was $m_9=699/1024$. In general the retained width is $2^{-k}$, so the [bisection error bound](numerical-analysis.md#bisection-error-bound) is $2^{-(k+1)}$. Nine halvings already suffice for an error at most $10^{-3}$, since $2^{-10}=0.0009765625<10^{-3}$. This guarantee comes from the width of the [root bracket](numerical-analysis.md#root-bracket), independently of any displayed decimal approximation to the unknown [zero of a function](polynomial.md#zero-of-a-function). Endpoint signs must be established reliably if evaluations use [floating-point arithmetic](numerical-analysis.md#floating-point-arithmetic).

<a id="image-the-cubic-x-cubed-plus-x-minus-one-its-unique-root-and-the-first-five-nested-bisection-brackets"></a>
![](intermediate-value-cubic-nested-root-brackets.png)

**[Figure 23](#image-the-cubic-x-cubed-plus-x-minus-one-its-unique-root-and-the-first-five-nested-bisection-brackets). The cubic x cubed plus x minus one: its unique root and the first five nested bisection brackets**.

##### Nested-bracket proof of the intermediate value theorem

↑ **Parent:** [Intermediate value theorem](#intermediate-value-theorem)

For a short proof outline, endpoint values give the non-strict cases immediately. If $y$ is strictly between $f(a)$ and $f(b)$, apply the [bisection method](numerical-analysis.md#bisection-method) to the [continuous function](#continuous-function) $g(x)=f(x)-y$. A [midpoint](mathematical-optimization.md#midpoint) with $g=0$ finishes the proof. Otherwise retain [nested intervals](real-analysis.md#nested-intervals) $[a_k,b_k]$ with strictly opposite signs and widths $(b-a)2^{-k}$. The [nested interval theorem](real-analysis.md#nested-interval-theorem), using [completeness of the real numbers](real-analysis.md#completeness-of-the-real-numbers), gives a common point $c$ to which both endpoint [sequences](real-analysis.md#sequence) converge. After reversing the sign of $g$ if necessary, $g(a_k)<0<g(b_k)$. [Continuity](#continuous-function) makes both endpoint value [sequences](real-analysis.md#sequence) converge to $g(c)$, forcing $g(c)\leq0$ and $g(c)\geq0$, hence $f(c)=y$. The original endpoint values differ from $y$, so $c\in(a,b)$. This proof explains why a jump can defeat the construction: shrinking a candidate [closed interval](real-analysis.md#closed-real-interval) cannot supply the missing [continuity](#continuous-function).

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

The derivative measures the instantaneous rate at which a [function](function.md) changes. For a real [function](function.md) $f$ defined near $a$, it exists when the [difference quotient](#difference-quotient) has a finite two-sided [limit](#limit-of-a-function):

$$
f'(a)=\lim_{h\to0}\frac{f(a+h)-f(a)}h.
$$

The quotient is the [slope](geometry-and-topology.md#slope) of the [straight line](geometry-and-topology.md#straight-line) joining two nearby points of the graph. Its [limit](#limit-of-a-function) is the [slope](geometry-and-topology.md#slope) of the [tangent line](#tangent-line). Thus a [derivative](#derivative) describes a local rate without choosing a particular finite measurement interval.

For $f(x)=x^2$, expanding the numerator gives

$$
\frac{(a+h)^2-a^2}h=2a+h,\qquad f'(a)=2a.
$$

At $a=1$, the increments $h=1$, $1/2$ and $1/10$ give [secant line](geometry-and-topology.md#secant-line) [slopes](geometry-and-topology.md#slope) $3$, $2.5$ and $2.1$. The [limit](#limit-of-a-function) is $2$, and the [tangent line](#tangent-line) is $y=1+2(x-1)$. The picture makes the limiting process visible.

<a id="image-secant-lines-to-x-squared-approach-its-tangent-line-at-x-1"></a>
![](derivative-secant-tangent.png)

**[Figure 24](#image-secant-lines-to-x-squared-approach-its-tangent-line-at-x-1). Secant lines to x squared approach its tangent line at x = 1**.

The same calculation shows why the [derivative](#derivative) is useful for approximation:

$$
f(a+h)=f(a)+f'(a)h+r(h),\qquad \frac{r(h)}h\longrightarrow0.
$$

This is a [local linear approximation](#local-linear-approximation). Near $a=1$, replacing $(1+h)^2$ by $1+2h$ makes the exact error $h^2$, smaller than the leading change when $h$ is small. A curved graph can therefore be studied locally using a [straight line](geometry-and-topology.md#straight-line).

If the [function](function.md) records [position](classical-mechanics.md#position) against time, its [derivative](#derivative) is [velocity](classical-mechanics.md#velocity). If it records an [objective function](mathematical-optimization.md#objective-function), its [derivative](#derivative) tests local changes that matter in [optimization](mathematical-optimization.md); in several variables, the [gradient](#gradient) collects these directional rates and guides [gradient descent](numerical-analysis.md#gradient-descent). The interpretation comes from the [function](function.md) and its units, rather than from a new rule for each application.

Existence matters. For the [absolute value function](real-analysis.md#absolute-value) $f(x)=|x|$, the [one-sided derivatives](#one-sided-derivative) at zero are $-1$ and $1$, so there is no single [tangent line](#tangent-line) described by a finite [derivative](#derivative) there. Nor does a zero [derivative](#derivative) alone identify a maximum or minimum: $f(x)=x^3$ has $f'(0)=0$ but keeps increasing through zero.

### Local linear approximation

↑ **Parent:** [Derivative](#derivative)

For a [differentiable function](analysis.md#differentiable-function), a [local linear approximation](#local-linear-approximation) replaces nearby values by its value plus its [derivative](#derivative) times the input change. The error divided by that change tends to zero. It uses the first-order [Taylor polynomial](#taylor-polynomial); the statement concerns a [limit](#limit-of-a-function) near the specified point, not a guaranteed approximation far from it.

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

A [total derivative](#total-derivative) accounts for every dependence of a quantity on the variable of [differentiation](#differentiation). For a [differentiable function](analysis.md#differentiable-function) $F(t,x_1,\ldots,x_n)$ evaluated along [differentiable](analysis.md#differentiable-function) coordinate [functions](function.md) $x_i(t)$, the [multivariable chain rule](#multivariable-chain-rule) gives

$$
\frac{d}{dt}F(t,x_1(t),\ldots,x_n(t))
=\frac{\partial F}{\partial t}+\sum_{i=1}^n\frac{\partial F}{\partial x_i}\frac{dx_i}{dt}.
$$

All the [partial derivatives](#partial-derivative) on the right are evaluated at $(t,x_1(t),\ldots,x_n(t))$. The first term captures explicit dependence on $t$; the remaining terms capture changes transmitted through the coordinates.

For example, take $F(t,x)=tx^2$ and $x(t)=t$. The [partial derivative](#partial-derivative) with respect to $t$, holding $x$ fixed, is $x^2$, whose value on the path is $t^2$. The [total derivative](#total-derivative) is instead

$$
\frac d{dt}F(t,t)=\frac d{dt}t^3=3t^2
=\underbrace{t^2}_{\partial_t F}+\underbrace{2t^2}_{\partial_x F\,x'}.
$$

At $t=2$, the [partial derivative](#partial-derivative) is $4$ and the [total derivative](#total-derivative) is $12$. The difference is the contribution from changing $x$.

If the composite [function](function.md) is [continuously differentiable](#continuously-differentiable-function) on $[a,b]$, the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) gives

$$
\int_a^b\frac{d}{dt}F(t,x(t))\,dt=F(b,x(b))-F(a,x(a)).
$$

This is the sense in which an integrated [total derivative](#total-derivative) contributes endpoint terms. The endpoint statement concerns the whole composite [function](function.md) along the path. [OpenStax, Calculus Volume 3: the chain rule with dependent variables](https://openstax.org/books/calculus-volume-3/pages/4-5-the-chain-rule).

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

The [chain rule](#chain-rule) calculates the [derivative](#derivative) of a [function composition](function.md#function-composition) by combining local rates. If the inner [function](function.md) $f$ is [differentiable](analysis.md#differentiable-function) at $a$ and the outer [function](function.md) $g$ is [differentiable](analysis.md#differentiable-function) at $f(a)$, then

$$
(g\circ f)'(a)=g'(f(a))f'(a).
$$

The evaluation point matters: the outer [derivative](#derivative) is evaluated at the inner output $f(a)$, not at $a$. A small input change first scales by $f'(a)$; the resulting intermediate change then scales by $g'(f(a))$. In terms of [linear approximations](#linear-approximation), composing those two local descriptions multiplies their scale factors. [OpenStax, Calculus Volume 1: statement and proof of the chain rule](https://openstax.org/books/calculus-volume-1/pages/3-6-the-chain-rule).

For example, $h(x)=\sin(x^2)$ applies a [quadratic function](polynomial.md#quadratic-function) and then the [sine](geometry-and-topology.md#sine). With $f(x)=x^2$ and $g(u)=\sin u$, the [chain rule](#chain-rule) gives

$$
h'(x)=\cos(x^2)\,2x,\qquad h'(1)=2\cos1\approx1.08060461.
$$

Here all [angles](geometry-and-topology.md#angle) are in [radians](geometry-and-topology.md#radian). Near $x=1$, increasing the input by $\Delta x$ changes $x^2$ by about $2\Delta x$, and the [sine](geometry-and-topology.md#sine) changes by about $\cos1$ times that intermediate change. For $\Delta x=0.01$, the [linear approximation](#linear-approximation) predicts an output increase of $0.0108060$; the exact increase is $\sin(1.0201)-\sin1\approx0.0106894$.

<a id="image-the-chain-rule-multiplies-the-local-rates-through-two-successive-functions"></a>
![](chain-rule-local-rates.png)

**[Figure 25](#image-the-chain-rule-multiplies-the-local-rates-through-two-successive-functions). The chain rule multiplies the local rates through two successive functions**. The inner [quadratic function](polynomial.md#quadratic-function) has [derivative](#derivative) $2$ at $x=1$, and the outer [sine](geometry-and-topology.md#sine) has [derivative](#derivative) $\cos1$ at its input $u=1$. Their composite has [derivative](#derivative) $2\cos1$. Each panel shows the corresponding [tangent line](#tangent-line) and the exact output of the input change from $1$ to $1.01$. Tangents describe [linear approximations](#linear-approximation), not exact finite changes.

The same rule handles several nested stages. For $h=g\circ f\circ k$, the [derivative](#derivative) is $h'(x)=g'(f(k(x)))f'(k(x))k'(x)$ under the corresponding [differentiability](analysis.md#differentiability) assumptions. Writing each intermediate output prevents evaluating a [derivative](#derivative) at the wrong stage. It also makes the [chain rule](#chain-rule) useful for propagating sensitivities through a mathematical model, where one measured quantity influences another through several transformations.

For a quick proof idea, replace $f$ near $a$ by its [linear approximation](#linear-approximation), then replace $g$ near $f(a)$ by its [linear approximation](#linear-approximation). The composite leading term is their product; [differentiability](analysis.md#differentiability) ensures the remaining error is smaller than the original input change. This argument still applies when $f'(a)=0$, so the informal cancellation $dh/dx=(dh/du)(du/dx)$ should not be interpreted as division by a possibly zero finite change. The hypotheses are sufficient, but are not necessary for every composite to be [differentiable](analysis.md#differentiable-function), as the [nondifferentiable inner function with a differentiable nondegenerate composite](#nondifferentiable-inner-function-with-a-differentiable-nondegenerate-composite) example shows.

#### Linear approximation

↑ **Parent:** [Chain rule](#chain-rule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_approximation)

A [linear approximation](#linear-approximation) replaces a [differentiable function](analysis.md#differentiable-function) near a reference input by its value plus the first-order change supplied by its [derivative](#derivative). In one dimension, this is the [tangent line](#tangent-line) $f(a)+f'(a)(x-a)$. The [chain rule](#chain-rule) combines such local approximations through [function composition](function.md#function-composition); it does not assert their equality to the original [functions](function.md) over a finite [interval](real-analysis.md#interval-mathematics).

#### Multivariable chain rule

↑ **Parent:** [Chain rule](#chain-rule)

For [differentiable maps](#differentiable-map) $f:\mathbb R^n\to\mathbb R^m$ and $g:\mathbb R^m\to\mathbb R^r$, the [multivariable chain rule](#multivariable-chain-rule) multiplies their [Jacobian matrices](#jacobian-matrix):

$$
J_{g\circ f}(x)=J_g(f(x))J_f(x).
$$

The outer $r\times m$ [matrix](vector-space.md#matrix) multiplies the inner $m\times n$ [matrix](vector-space.md#matrix), producing an $r\times n$ [matrix](vector-space.md#matrix). This order records that the inner [linear map](vector-space.md#linear-map) acts first. Componentwise, the [matrix multiplication](vector-space.md#matrix-multiplication) sums the contributions of all intermediate coordinates. Existence of separate [partial derivatives](#partial-derivative) alone is not the required [differentiability](analysis.md#differentiability) hypothesis.

##### Derivative along a curve

↑ **Parent:** [Multivariable chain rule](#multivariable-chain-rule)

If $F:\mathbb R^n\to\mathbb R$ is [differentiable](analysis.md#differentiable-function) at the point $\gamma(t)$ of a [differentiable](analysis.md#differentiable-function) [parametric curve](topology.md#parametric-curve), the [multivariable chain rule](#multivariable-chain-rule) gives

$$
\frac d{dt}F(\gamma(t))=\nabla F(\gamma(t))\cdot\gamma'(t).
$$

The [gradient](#gradient) supplies the local spatial rates; the [velocity vector](differential-geometry.md#velocity-vector) $\gamma'(t)$ supplies the direction and rate of movement. Their [dot product](linear-algebra.md#dot-product) is the change in the sampled [scalar field](quantum-field-theory.md#scalar-field) per unit parameter. If the parameter is time, this is a rate per unit time; a [directional derivative](#directional-derivative) per unit distance instead uses a [unit vector](vector-space.md#unit-vector).

Take $F(x,y)=x^2+2y^2$ and the [unit circle](complex-analysis.md#complex-unit-circle) path $\gamma(t)=(\cos t,\sin t)$. Along the path,

$$
F(\gamma(t))=1+\sin^2t,\qquad
\frac d{dt}F(\gamma(t))=2\sin t\cos t=\sin2t.
$$

At $t=\pi/4$, the [gradient](#gradient) is $(\sqrt2,2\sqrt2)$, the [velocity vector](differential-geometry.md#velocity-vector) is $(-1/\sqrt2,1/\sqrt2)$, and their [dot product](linear-algebra.md#dot-product) is $-1+2=1$. The sampled value is $3/2$ and increases at rate one, even though one coordinate is decreasing. This is why a moving observation must combine every coordinate's contribution.

<a id="image-the-gradient-and-path-velocity-combine-to-give-the-rate-of-change-along-a-curve"></a>
![](chain-rule-along-a-path.png)

**[Figure 26](#image-the-gradient-and-path-velocity-combine-to-give-the-rate-of-change-along-a-curve). The gradient and path velocity combine to give the rate of change along a curve**. Left: [level curves](topology.md#level-curve) of $F(x,y)=x^2+2y^2$, the [unit circle](complex-analysis.md#complex-unit-circle) path, and arrows at $t=\pi/4$ for its [velocity vector](differential-geometry.md#velocity-vector) and a scaled [gradient](#gradient). Right: the sampled [function](function.md) $F(\gamma(t))=1+\sin^2t$ and its [tangent line](#tangent-line), of [slope](geometry-and-topology.md#slope) one at that parameter. The displayed gradient arrow is scaled for readability, without changing its direction.

For a [level curve](topology.md#level-curve), $F(\gamma(t))$ is constant, so the [derivative along a curve](#derivative-along-a-curve) is zero and its [velocity vector](differential-geometry.md#velocity-vector) is [orthogonal](linear-algebra.md#orthogonal-vectors) to the [gradient](#gradient). Along other paths, the same formula combines a field's geometry with the observer's motion. [OpenStax, multivariable chain rule and parameter-dependent inputs](https://openstax.org/books/calculus-volume-3/pages/4-5-the-chain-rule).

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

A [real-valued function](function.md#real-valued-function) $f:D\to\mathbb R$, with [domain of a function](function.md#domain-of-a-function) $D\subseteq\mathbb R$ in the usual order of the [real numbers](arithmetic.md#real-number), is a [monotonic function](#monotonic-function) if it is either a [nondecreasing function](#nondecreasing-function) throughout $D$ or a [nonincreasing function](#nonincreasing-function) throughout $D$. The same direction must work for every pair $x<y$ in $D$. Being a [strictly increasing function](#strictly-increasing-function) on one part and a [strictly decreasing function](#strictly-decreasing-function) on another does not make the whole [function](function.md) [monotone](#monotonic-function): for example, $x^2$ on the [real line](real-analysis.md#real-line) changes direction at zero. A [constant function](function.md#constant-function) is both a [nondecreasing function](#nondecreasing-function) and a [nonincreasing function](#nonincreasing-function).

The word "increasing" is ambiguous across textbooks: some allow equal outputs and some require unequal outputs. Use [nondecreasing function](#nondecreasing-function) for the weak inequality and [strictly increasing function](#strictly-increasing-function) for the strict inequality; use [nonincreasing function](#nonincreasing-function) and [strictly decreasing function](#strictly-decreasing-function) in the other direction. Neither [continuity](#continuous-function) nor [differentiability](analysis.md#differentiability) is part of the definition of a [monotonic function](#monotonic-function).

Strict [monotonicity](#monotonic-function) gives [injectivity](algebra.md#injective-function), so an equation $f(x)=b$ has at most one solution and an [inverse function](function.md#inverse-function) exists on the [image of a function](set-theory.md#image-of-a-function). Weak [monotonicity](#monotonic-function) permits repeated outputs and jumps. In [probability theory](probability-theory.md), a [cumulative distribution function](probability-theory.md#cumulative-distribution-function) is a [nondecreasing function](#nondecreasing-function); its [quantile function](probability-theory.md#quantile-function) uses a generalized inverse to handle those flat parts and jumps. [Monotonicity](#monotonic-function) alone does not guarantee [continuity](#continuous-function), even for a [strictly increasing function](#strictly-increasing-function).

<a id="image-strict-and-weak-monotonicity-cubic-functions-flat-portions-and-a-step"></a>
![](monotonicity-strict-and-weak.png)

**[Figure 27](#image-strict-and-weak-monotonicity-cubic-functions-flat-portions-and-a-step). Strict and weak monotonicity: cubic functions, flat portions, and a step**. The [strictly increasing function](#strictly-increasing-function) $x^3$ and [strictly decreasing function](#strictly-decreasing-function) $-x^3$ never repeat an output. The [nondecreasing function](#nondecreasing-function) $\min(1,\max(0,x))$ has flat [intervals](real-analysis.md#interval-mathematics), and the [step function](measure-theory.md#step-function) $F(x)=0$ for $x<0$, $F(x)=1$ for $x\geq0$ is a [discontinuous](#discontinuity-of-a-function) [cumulative distribution function](probability-theory.md#cumulative-distribution-function). The open and closed circles specify its value at the jump; no vertical segment belongs to its graph.

### Derivative criterion for monotonicity

↑ **Parent:** [Monotonic function](#monotonic-function)

Let $I$ be a [real interval](real-analysis.md#interval-mathematics), and let $f:I\to\mathbb R$ be [differentiable](analysis.md#differentiable-function) in its [interior](topology.md#interior-topology) and [continuous](#continuous-function) at any endpoints belonging to $I$. If the [derivative](#derivative) satisfies $f'(x)\geq0$ throughout the [interior](topology.md#interior-topology), then $f$ is a [nondecreasing function](#nondecreasing-function) on $I$. For $x<y$ in $I$, the [mean value theorem](#mean-value-theorem) supplies $c\in(x,y)$ with

$$
f(y)-f(x)=f'(c)(y-x)\geq0.
$$

Changing $\geq0$ to $\leq0$, $>0$, or $<0$ gives a [nonincreasing function](#nonincreasing-function), [strictly increasing function](#strictly-increasing-function), or [strictly decreasing function](#strictly-decreasing-function), respectively. The endpoint [continuity](#continuous-function) assumption lets the [mean value theorem](#mean-value-theorem) apply even when $x$ or $y$ is an endpoint. [OpenStax Calculus Volume 1, mean value theorem and its monotonicity corollary](https://openstax.org/books/calculus-volume-1/pages/4-4-the-mean-value-theorem).

Conversely, if a [nondecreasing function](#nondecreasing-function) on a [real interval](real-analysis.md#interval-mathematics) is [differentiable](analysis.md#differentiable-function) at an interior point $x$, then $f'(x)\geq0$: the [difference quotient](#difference-quotient) $(f(x+h)-f(x))/h$ is nonnegative for either sign of $h$. A [differentiable](analysis.md#differentiable-function) [nonincreasing function](#nonincreasing-function) has [derivative](#derivative) $f'(x)\leq0$. Strict [monotonicity](#monotonic-function) still only forces these weak signs: the [strictly increasing function](#strictly-increasing-function) $x^3$ has [derivative](#derivative) zero at zero. The sign of the [derivative](#derivative) helps locate [intervals](real-analysis.md#interval-mathematics) of [monotonicity](#monotonic-function) when sketching a graph. [OpenStax Calculus Volume 1, derivatives and the shape of a graph](https://openstax.org/books/calculus-volume-1/pages/4-5-derivatives-and-the-shape-of-a-graph).

The [real interval](real-analysis.md#interval-mathematics) hypothesis matters because a [connected subset of the real line](geometry-and-topology.md#connected-subset-of-the-real-line) contains every point between its inputs. On a disconnected [domain of a function](function.md#domain-of-a-function), positive [derivatives](#derivative) need not give a [nondecreasing function](#nondecreasing-function). For example, take

$$
D=(-2,-1)\cup(1,2),\qquad
f(x)=\begin{cases}x,&-2<x<-1,\\x-10,&1<x<2.\end{cases}
$$

Here $f'(x)=1$ everywhere in $D$, but $-3/2<3/2$ while $f(-3/2)=-3/2>-17/2=f(3/2)$. Each component has a [strictly increasing function](#strictly-increasing-function), yet their outputs are ordered the wrong way across the gap. This [function](function.md) is neither a [nondecreasing function](#nondecreasing-function) nor a [nonincreasing function](#nonincreasing-function) on all of $D$; the [mean value theorem](#mean-value-theorem) cannot cross the missing [interval](real-analysis.md#interval-mathematics).

<a id="image-a-zero-derivative-can-coexist-with-strict-increase-while-a-domain-gap-defeats-the-derivative-test"></a>
![](monotonicity-derivative-and-domain.png)

**[Figure 28](#image-a-zero-derivative-can-coexist-with-strict-increase-while-a-domain-gap-defeats-the-derivative-test). A zero derivative can coexist with strict increase, while a domain gap defeats the derivative test**. Left: the [strictly increasing function](#strictly-increasing-function) $f(x)=x^3$ and its [derivative](#derivative) $f'(x)=3x^2$, both zero at the origin. Right: two separate graph segments with [derivative](#derivative) one on $(-2,-1)\cup(1,2)$, but a lower output on the right component. Open circles exclude the four component endpoints.

### Monotone mean-value point of an integral average

↑ **Parent:** [Monotonic function](#monotonic-function)

For a continuous strictly decreasing real function, its average $h(x)=x^{-1}\int_0^xf(t)dt$ lies strictly between $f(x)$ and $f(0)$ for $x>0$. There is a unique $g(x)\in(0,x)$ with $f(g(x))=h(x)$. If $f$ is [differentiable](analysis.md#differentiable-function) and $f'<0$ throughout the positive half-line, the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) and the derivative formula for the monotone inverse give

$$
g'(x)=\frac{f(x)-f(g(x))}{xf'(g(x))}>0.
$$

Continuity of $f'$ is unnecessary: differentiability of a strictly monotone function with nonzero derivative at a point suffices for differentiability of its inverse there.

### Nonincreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A [real-valued function](function.md#real-valued-function) $f:D\to\mathbb R$ is a [nonincreasing function](#nonincreasing-function) if every pair $x<y$ in its [domain of a function](function.md#domain-of-a-function) satisfies $f(x)\geq f(y)$. Equal outputs and flat [intervals](real-analysis.md#interval-mathematics) are allowed. For example, $f(x)=-\min(1,\max(0,x))$ is a [nonincreasing function](#nonincreasing-function), with a falling segment between two flat portions. Requiring $f(x)>f(y)$ instead gives a [strictly decreasing function](#strictly-decreasing-function). Negating a [nondecreasing function](#nondecreasing-function) gives a [nonincreasing function](#nonincreasing-function).

A [nonincreasing](#nonincreasing-function) [sequence](real-analysis.md#sequence) of [natural numbers](arithmetic.md#natural-number) has finitely many strict drops, so it is eventually constant. This differs from a [strictly decreasing](#strictly-decreasing-function) [sequence](real-analysis.md#sequence), which cannot continue indefinitely within the [natural numbers](arithmetic.md#natural-number).

// Target: foundations-of-mathematics.bigb

### Non-strict inverse of a continuous nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

For a continuous unbounded [nondecreasing function](#nondecreasing-function) $f$ on the nonnegative half-line and $a>f(0)$, the non-strict inverse $h$ is left-continuous in its level argument. It equals the left limit of the [strict generalized inverse of a nondecreasing function](#strict-generalized-inverse-of-a-nondecreasing-function) $G(a)=\inf\{t:f(t)>a\}$. Indeed $G(b)\leq h(a)$ for $b<a$, while for every $t<h(a)$, $f(t)<a$ and choosing $b\in(f(t),a)$ gives $G(b)\geq t$. Similarly $h(a+)=G(a)$. A flat part of $f$ at level $a$ gives a discrepancy between the two inverses: $h(a)$ selects the beginning of the flat part and $G(a)$ its end. For a [Brownian running maximum](brownian-motion.md#brownian-running-maximum), these are the non-strict and strict passage times.

### Left-continuous cumulative function of an atomic measure

↑ **Parent:** [Monotonic function](#monotonic-function)

For positive summable weights $w_j$ at points $q_j$, the strict cumulative function $F(x)=\sum_{q_j<x}w_j$ is nondecreasing and left-continuous. A finite-head/tail argument proves left-continuity, and its right jump at an atom is the mass there. This strict convention differs at atoms from the usual right-continuous [cumulative distribution function](probability-theory.md#cumulative-distribution-function).

### Nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A [real-valued function](function.md#real-valued-function) $f:D\to\mathbb R$ is a [nondecreasing function](#nondecreasing-function) if every pair $x<y$ in its [domain of a function](function.md#domain-of-a-function) satisfies $f(x)\leq f(y)$. Flat [intervals](real-analysis.md#interval-mathematics) are allowed, unlike for a [strictly increasing function](#strictly-increasing-function). For example,

$$
p(x)=\min(1,\max(0,x))=\begin{cases}0,&x\leq0,\\x,&0<x<1,\\1,&x\geq1\end{cases}
$$

is a [continuous](#continuous-function) [nondecreasing function](#nondecreasing-function), but it repeats its output on each flat [interval](real-analysis.md#interval-mathematics).

A [nondecreasing function](#nondecreasing-function) can also be [discontinuous](#discontinuity-of-a-function). The [step function](measure-theory.md#step-function) $F(x)=0$ for $x<0$ and $F(x)=1$ for $x\geq0$ has a [jump discontinuity](#jump-discontinuity) at zero without ever decreasing. It is the [cumulative distribution function](probability-theory.md#cumulative-distribution-function) of a [random variable](random-variable.md) that equals zero with [probability](probability-theory.md#probability) one; [quantile functions](probability-theory.md#quantile-function) handle such jumps through a generalized inverse. [Nondecreasing](#nondecreasing-function) allocation [functions](function.md) permit [critical-value payments](game-theory.md#critical-value-payment) in [single-parameter mechanisms](game-theory.md#single-parameter-mechanism).

### Strict generalized inverse of a nondecreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

For an unbounded nondecreasing function $f:[0,\infty)\to\mathbb R$, its strict generalized inverse is $G(a)=\inf\{t\geq0:f(t)>a\}$. It is nondecreasing and right-continuous in $a$. If $a_n\downarrow a$, then for any $t>G(a)$ monotonicity gives $f(t)>a$, so eventually $f(t)>a_n$ and $G(a_n)\leq t$; also $G(a_n)\geq G(a)$. Local finiteness gives finite left limits. Flat parts of $f$ create jumps of $G$. For the continuous running maximum of [Brownian motion](brownian-motion.md), this gives the [càdlàg](#cadlag) [Brownian first-passage subordinator](stochastic-process.md#brownian-first-passage-subordinator).

### Strictly increasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A [real-valued function](function.md#real-valued-function) $f:D\to\mathbb R$ is a [strictly increasing function](#strictly-increasing-function) if every pair $x<y$ in its [domain of a function](function.md#domain-of-a-function) satisfies $f(x)<f(y)$. It is therefore [injective](algebra.md#injective-function), and each output has at most one [preimage](set-theory.md#preimage). Its [inverse function](function.md#inverse-function) on its [image of a function](set-theory.md#image-of-a-function) is also [strictly increasing](#strictly-increasing-function). Every [strictly increasing function](#strictly-increasing-function) is a [nondecreasing function](#nondecreasing-function); the converse fails when outputs repeat.

The [polynomial](polynomial.md) $f(x)=x^3$ is a [strictly increasing function](#strictly-increasing-function) on the [real line](real-analysis.md#real-line), although its [derivative](#derivative) $f'(x)=3x^2$ is zero at zero. Indeed, for $x<y$,

$$
y^3-x^3=(y-x)(x^2+xy+y^2)>0,
$$

because $x^2+xy+y^2=(x+y/2)^2+3y^2/4$ can vanish only when $x=y=0$. Thus a positive [derivative](#derivative) everywhere is sufficient on a [real interval](real-analysis.md#interval-mathematics), but is not necessary for a [strictly increasing function](#strictly-increasing-function).

Strict [monotonicity](#monotonic-function) does not ensure [continuity](#continuous-function): $g(x)=x$ for $x<0$ and $g(x)=x+1$ for $x\geq0$ is a [strictly increasing function](#strictly-increasing-function) with a [jump discontinuity](#jump-discontinuity). Its [image of a function](set-theory.md#image-of-a-function) omits $[0,1)$, so the [inverse function](function.md#inverse-function) exists only on the actual [image of a function](set-theory.md#image-of-a-function), rather than on all the [real numbers](arithmetic.md#real-number).

#### Continuity of an increasing interval surjection

↑ **Parent:** [Strictly increasing function](#strictly-increasing-function)

A strictly increasing function from a closed real interval onto the interval between its endpoint values is continuous. Given a desired output tolerance, choose nearby output values on either side and use their preimages to trap nearby inputs. At the endpoints only one side is needed. Equivalently, a discontinuity of a monotone function creates a gap in its range, which is incompatible with surjectivity onto an interval.

### Strictly decreasing function

↑ **Parent:** [Monotonic function](#monotonic-function)

A [real-valued function](function.md#real-valued-function) $f:D\to\mathbb R$ is a [strictly decreasing function](#strictly-decreasing-function) if every pair $x<y$ in its [domain of a function](function.md#domain-of-a-function) satisfies $f(x)>f(y)$. It is a [nonincreasing function](#nonincreasing-function) and is [injective](algebra.md#injective-function), with a [strictly decreasing](#strictly-decreasing-function) [inverse function](function.md#inverse-function) on its [image of a function](set-theory.md#image-of-a-function). Negating a [strictly increasing function](#strictly-increasing-function) gives a [strictly decreasing function](#strictly-decreasing-function): $f(x)=-x^3$ is an example on the [real line](real-analysis.md#real-line), even though its [derivative](#derivative) vanishes at zero. Equal outputs are forbidden, unlike for a general [nonincreasing function](#nonincreasing-function).

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

In [Cartesian coordinates](linear-algebra.md#cartesian-coordinate-system) on [Euclidean space](functional-analysis.md#euclidean-norm), the gradient of a scalar-valued [differentiable function](analysis.md#differentiable-function) is the [vector](vector-space.md#vector) of its first [partial derivatives](#partial-derivative). It converts a [scalar field](quantum-field-theory.md#scalar-field), such as [temperature](thermodynamics.md#temperature) or a height, into a [vector field](#vector-field) describing its local change.

For a [unit vector](vector-space.md#unit-vector) $u$, the [directional derivative](#directional-derivative) is $D_uf=u\cdot\nabla f$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $|D_uf|\leq|\nabla f|$. At a point where $\nabla f\ne0$, the greatest increase per unit distance occurs along $u=\nabla f/|\nabla f|$, while the opposite direction gives the greatest decrease. These are first-order statements at the current point; they do not predict how the [function](function.md) behaves far along a straight path.

For $f(x,y)=x^2+2y^2$ at $(1,1)$, $\nabla f=(2,4)$. Moving in the $x$ direction gives rate $2$ and moving in the $y$ direction gives rate $4$, but the steepest direction is $(1,2)/\sqrt5$, with

$$
D_uf=\boxed{2\sqrt5}.
$$

The direction $(-2,1)/\sqrt5$ has rate zero and is tangent to the [level curve](topology.md#level-curve) through that point. More generally, differentiating $f(\gamma(t))=\text{constant}$ along a regular [level curve](topology.md#level-curve) gives $\nabla f\cdot\gamma'=0$, so the [gradient](#gradient) is its [normal vector](differential-geometry.md#normal-vector).

<a id="image-a-gradient-is-normal-to-level-curves-and-determines-the-directional-derivative-for-every-unit-direction"></a>
![](gradient-directional-derivative.png)

**[Figure 29](#image-a-gradient-is-normal-to-level-curves-and-determines-the-directional-derivative-for-every-unit-direction). A gradient is normal to level curves and determines the directional derivative for every unit direction**.

This is useful when navigating a measured [scalar field](quantum-field-theory.md#scalar-field) or applying [gradient descent](numerical-analysis.md#gradient-descent): one collection of [partial derivatives](#partial-derivative) predicts every infinitesimal directional change. The derivative assumes a [differentiable function](analysis.md#differentiable-function), not merely the existence of all directional derivatives. [OpenStax: Directional derivatives and the gradient](https://openstax.org/books/calculus-volume-3/pages/4-6-directional-derivatives-and-the-gradient).

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

The [Hessian matrix](#hessian-matrix) describes how the slope of a [function](function.md) changes in different directions. For a real-valued [function](function.md) $f$ with continuous second [partial derivatives](#partial-derivative) on an [open subset](topology.md#open-set) of $\mathbb R^n$, it is

$$
H_f(x)=\left(\frac{\partial^2 f}{\partial x_i\partial x_j}(x)\right)_{i,j=1}^n.
$$

The [symmetry of second derivatives](#symmetry-of-second-derivatives) makes $H_f$ a [symmetric matrix](linear-algebra.md#symmetric-matrix) under these hypotheses. It is also the [Jacobian matrix](#jacobian-matrix) of the [gradient](#gradient): near $x$, a small displacement $h$ changes $\nabla f$ by $H_f(x)h+o(\|h\|)$. Thus the [gradient](#gradient) measures the current slope, while the [Hessian](#hessian-matrix) measures its local variation. [MIT 18.S096 matrix calculus notes, §12.1: Hessian matrices of scalar-valued functions](https://ocw.mit.edu/courses/18-s096-matrix-calculus-for-machine-learning-and-beyond-january-iap-2023/mit18_s096iap23_lec12.pdf)

For example, take the [quadratic form](linear-algebra.md#quadratic-form)

$$
q(x,y)=x^2+2xy+3y^2.
$$

Its [gradient](#gradient) and [Hessian matrix](#hessian-matrix) are

$$
\nabla q=(2x+2y,2x+6y)^T,
\qquad
H_q=\begin{pmatrix}2&2\\2&6\end{pmatrix}.
$$

The only [critical point](analysis.md#critical-point) is the origin. Completing the square gives $q=(x+y)^2+2y^2$, so the origin is a strict [global minimum](analysis.md#global-minimum). The [eigenvalues](linear-operator-theory.md#eigenvalue) $4-2\sqrt2$ and $4+2\sqrt2$ are both positive, recovering the same conclusion from the [positive definiteness](linear-algebra.md#positive-definiteness) of the [Hessian](#hessian-matrix). Its [eigenvectors](linear-operator-theory.md#eigenvector) identify the rotated directions in which the [quadratic form](linear-algebra.md#quadratic-form) has its smallest and largest bending.

<a id="image-positive-negative-and-mixed-hessian-eigenvalues-produce-different-critical-point-geometry"></a>
![](hessian-quadratic-critical-points.png)

**[Figure 30](#image-positive-negative-and-mixed-hessian-eigenvalues-produce-different-critical-point-geometry). Positive, negative and mixed Hessian eigenvalues produce different critical-point geometry**. Contour plots of $q=x^2+2xy+3y^2$, $-q$, and $s=x^2-y^2$. All three have a [critical point](analysis.md#critical-point) at the origin; the first two have elliptical contours, while the last has positive and negative sectors meeting along its zero contours.

For a fixed [vector](vector-space.md#vector) $v$, restriction to a [straight line](geometry-and-topology.md#straight-line) gives the directional interpretation

$$
\left.\frac{d^2}{dt^2}f(x+tv)\right|_{t=0}=v^TH_f(x)v.
$$

This is the [quadratic form](linear-algebra.md#quadratic-form) associated with the [Hessian matrix](#hessian-matrix). For a unit [eigenvector](linear-operator-theory.md#eigenvector) $v$, it equals the corresponding [eigenvalue](linear-operator-theory.md#eigenvalue). Opposite signs therefore mean that some directions bend upwards and others downwards. The [second-derivative test](#second-derivative-test) turns this information into a classification when the [gradient](#gradient) vanishes.

The same object is useful for computation. [Newton's method in optimization](mathematical-optimization.md#newton-s-method-in-optimization) chooses a displacement $h$ by solving $H_f(x)h=-\nabla f(x)$ when the [Hessian matrix](#hessian-matrix) is an [invertible matrix](linear-algebra.md#invertible-matrix); this makes the [gradient](#gradient) of the local quadratic model vanish. For the displayed $q$, the equation gives $h=-(x,y)^T$, so one exact step reaches the minimum from any starting point. For a general [function](function.md), a [Hessian](#hessian-matrix) with opposite-sign [eigenvalues](linear-operator-theory.md#eigenvalue) or a large [condition number](linear-algebra.md#condition-number) need not give a useful minimizing step, and the [local minimum](analysis.md#local-minimum) need not be a [global minimum](analysis.md#global-minimum).

The name honors Otto Hesse. [MIT World Web Math: the Hessian and its namesake](https://web.mit.edu/course/other/wwmath/vectorc/minmax/hessian.html) An older geometric use is the [Hessian criterion for flexes of a plane cubic](normalization-of-an-algebraic-curve.md#hessian-criterion-for-flexes-of-a-plane-cubic), connecting a [determinant](linear-algebra.md#determinant) of second [partial derivatives](#partial-derivative) with inflection points of an algebraic [curve](topology.md#curve). Hesse's 1844 paper _Über die Wendepuncte der Curven dritter Ordnung_ is an early source on that geometric problem. [Hesse (1844), Journal für die reine und angewandte Mathematik 28, pp. 97–107: publisher's bibliographic record](https://www.degruyterbrill.com/document/doi/10.1515/crll.1844.28.97/html)

#### Quadratic growth from a bounded Hessian

↑ **Parent:** [Hessian matrix](#hessian-matrix)

For $F\in C^2(\mathbb R^n)$ with bounded [Hessian matrix](#hessian-matrix), Taylor's formula along the line from zero to $p$ gives $|F(p)|\leq|F(0)|+|DF(0)||p|+\frac12\|D^2F\|_\infty|p|^2$. Its gradient obeys $|DF(p)|\leq|DF(0)|+\|D^2F\|_\infty|p|$. Consequently $\int_\Omega F(Du)$ is finite for $u\in H^1(\Omega)$ when $\Omega$ has finite measure, and $DF(Du)\in L^2$.

#### Higher-order test for separated extrema

↑ **Parent:** [Hessian matrix](#hessian-matrix)

For $f(x,y)=g(x)+h(y)$, a degenerate [Hessian matrix](#hessian-matrix) can be supplemented by the first nonzero term of each one-variable displacement. Two negative leading even powers give a strict [local maximum](analysis.md#local-maximum), two positive ones a strict [local minimum](analysis.md#local-minimum), and opposite signs give a saddle. Looking along the coordinate directions and bounding the separated terms avoids an inconclusive quadratic test.

For an explicit contrast, consider

$$
f_+(x,y)=x^4+y^4,
\qquad
f_-(x,y)=x^4-y^4.
$$

Both have zero [gradient](#gradient) and the same zero [Hessian matrix](#hessian-matrix) at the origin:

$$
H_{f_+}(0,0)=H_{f_-}(0,0)=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
$$

Nevertheless, $f_+$ is positive at every nonzero point, so the origin is a strict [global minimum](analysis.md#global-minimum). For $f_-$, the restrictions $f_-(t,0)=t^4>0$ and $f_-(0,t)=-t^4<0$ for $t\ne0$ show that the origin is a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function). Identical quadratic information can conceal different geometry when higher-order terms are decisive.

<a id="image-the-same-zero-hessian-can-occur-at-a-strict-minimum-or-a-saddle"></a>
![](hessian-degenerate-critical-points.png)

**[Figure 31](#image-the-same-zero-hessian-can-occur-at-a-strict-minimum-or-a-saddle). The same zero Hessian can occur at a strict minimum or a saddle**. The quartic functions $x^4+y^4$ and $x^4-y^4$ both have zero second [partial derivatives](#partial-derivative) at the origin. Their contour geometry and signs differ, so a singular [Hessian matrix](#hessian-matrix) alone cannot classify the [critical point](analysis.md#critical-point).

#### Negative semidefinite matrix

↑ **Parent:** [Hessian matrix](#hessian-matrix)

A symmetric matrix $A$ is negative semidefinite when $v^TAv\leq0$ for every vector $v$. Equivalently, all its [eigenvalues](linear-operator-theory.md#eigenvalue) are nonpositive.

#### Second-derivative test

↑ **Parent:** [Hessian matrix](#hessian-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second-derivative_test)

Let $f$ have continuous second [partial derivatives](#partial-derivative) near an interior [critical point](analysis.md#critical-point) $x_*$ of an [open subset](topology.md#open-set) of $\mathbb R^n$, with $\nabla f(x_*)=0$. The [Hessian matrix](#hessian-matrix) gives the following sufficient conditions:
- All [eigenvalues](linear-operator-theory.md#eigenvalue) positive: a strict [local minimum](analysis.md#local-minimum).
- All [eigenvalues](linear-operator-theory.md#eigenvalue) negative: a strict [local maximum](analysis.md#local-maximum).
- Both positive and negative [eigenvalues](linear-operator-theory.md#eigenvalue): a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function).

A [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix) or [negative semidefinite](#negative-semidefinite-matrix) [Hessian matrix](#hessian-matrix) with a zero [eigenvalue](linear-operator-theory.md#eigenvalue) does not settle the classification. The [higher-order test for separated extrema](#higher-order-test-for-separated-extrema) gives two quartic examples with exactly the same zero [Hessian](#hessian-matrix). These conditions apply to an interior [critical point](analysis.md#critical-point); a boundary optimum or a [constrained optimization](numerical-analysis.md#constrained-optimization) problem requires attention to the allowed directions. [MIT 18.013A Calculus with Applications, §11.3: Hessian eigenvalues and the critical-point criterion](https://ocw.mit.edu/ans7870/18/18.013a/textbook/chapter11/section03.html)

The proof outline is the [Taylor expansion](#taylor-expansion)

$$
f(x_*+h)-f(x_*)=\frac12h^TH_f(x_*)h+o(\|h\|^2).
$$

For a [positive-definite matrix](linear-algebra.md#positive-definite-matrix), the smallest [eigenvalue](linear-operator-theory.md#eigenvalue) supplies a positive bound proportional to $\|h\|^2$, which dominates the remainder for small enough $h$. Negate the [function](function.md) for the [local maximum](analysis.md#local-maximum) case. For opposite-sign [eigenvalues](linear-operator-theory.md#eigenvalue), choose the two corresponding [eigenvectors](linear-operator-theory.md#eigenvector): the leading terms have opposite signs along their lines.

There are also necessary conditions. At an interior [local minimum](analysis.md#local-minimum), the [Hessian matrix](#hessian-matrix) is [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix); at an interior [local maximum](analysis.md#local-maximum), it is [negative semidefinite](#negative-semidefinite-matrix). Restriction to each [straight line](geometry-and-topology.md#straight-line) reduces this to the one-variable [second derivative](#second-derivative) condition. Since the [Laplacian](#laplacian) is the [trace](linear-algebra.md#matrix-trace) of the [Hessian](#hessian-matrix), it is nonnegative at such a [local minimum](analysis.md#local-minimum) and nonpositive at such a [local maximum](analysis.md#local-maximum). The sign of the [Laplacian](#laplacian) alone is insufficient: $x^2-2y^2$ has negative [Laplacian](#laplacian) but a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function) at the origin.

##### Critical points escaping to infinity in a Gaussian-weighted bilinear function

↑ **Parent:** [Second-derivative test](#second-derivative-test)

The origin is a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function) for every real parameter. For $\alpha>0$ four further [critical points](analysis.md#critical-point) have $x^2=y^2=1/(2\alpha)$. Equal-sign coordinates give global maxima and opposite-sign coordinates give [global minima](analysis.md#global-minimum), with values $\pm1/(2e\alpha)$. The [Hessian matrix](#hessian-matrix) there is $-4\alpha xy e^{-1}I$. Their distance from the origin is $\alpha^{-1/2}$, so as $\alpha\downarrow0$ they escape every compact region. At nonpositive $\alpha$ the origin is the only [critical point](analysis.md#critical-point). This illustrates why the number of [critical points](analysis.md#critical-point) on an unbounded domain can change without a finite degenerate [critical point](analysis.md#critical-point) appearing.

#### Nondegenerate critical point

↑ **Parent:** [Hessian matrix](#hessian-matrix)

A [critical point](analysis.md#critical-point) of a real [function](function.md) with continuous second [partial derivatives](#partial-derivative) is nondegenerate when its [Hessian matrix](#hessian-matrix) is an [invertible matrix](linear-algebra.md#invertible-matrix) there, equivalently when none of its [eigenvalues](linear-operator-theory.md#eigenvalue) is zero. A [positive-definite matrix](linear-algebra.md#positive-definite-matrix) gives a strict [local minimum](analysis.md#local-minimum), a [negative definite](linear-algebra.md#negative-definite-matrix) [Hessian](#hessian-matrix) gives a strict [local maximum](analysis.md#local-maximum), and opposite-sign [eigenvalues](linear-operator-theory.md#eigenvalue) give a [saddle point of a scalar function](analysis.md#saddle-point-of-a-scalar-function). A nondegenerate [critical point](analysis.md#critical-point) need not be an extremum: $x^2-y^2$ has [Hessian matrix](#hessian-matrix) $\operatorname{diag}(2,-2)$, which is an [invertible matrix](linear-algebra.md#invertible-matrix).

Such critical points are the local building blocks of [Morse theory](differential-geometry.md#morse-theory).

### Vector calculus

↑ **Parent:** [Multivariable calculus](#multivariable-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_calculus)

Vector calculus studies differentiation and integration of [scalar fields](quantum-field-theory.md#scalar-field) and [vector fields](#vector-field). Three operators answer different local questions: the [gradient](#gradient) describes change of a scalar value, the [divergence](#divergence) describes net outward flow, and the [curl](#curl) describes local circulation. Their associated integral theorems turn local derivatives into measurements along paths and across boundaries.

The difference between [divergence](#divergence) and [curl](#curl) is especially visible in two smooth [vector fields](#vector-field) on three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm):

$$
F(x,y,z)=(x,y,0),\qquad G(x,y,z)=(-y,x,0).
$$

At each point they have the same [Euclidean norm](functional-analysis.md#euclidean-norm) $\sqrt{x^2+y^2}$, but their directions differ. For $F$, $\nabla\cdot F=2$ and $\nabla\times F=0$. For $G$, $\nabla\cdot G=0$ and $\nabla\times G=(0,0,2)$. One expands radially in each horizontal plane; the other describes rigid rotation.

<a id="image-equal-magnitude-fields-can-have-different-divergence-and-curl-radial-expansion-gives-outward-flux-while-rotation-gives-circulation"></a>
![](divergence-curl-flux.png)

**[Figure 32](#image-equal-magnitude-fields-can-have-different-divergence-and-curl-radial-expansion-gives-outward-flux-while-rotation-gives-circulation). Equal-magnitude fields can have different divergence and curl: radial expansion gives outward flux, while rotation gives circulation**.

Around the counterclockwise unit [circle](topology.md#circle) in the plane $z=0$, $F$ is normal to the boundary and has zero tangential component. Its outward planar [flux integral](#flux-integral) is $2\pi$, while its [line integral](#line-integral) around the circle is zero. For $G$ the values are reversed: outward planar [flux](physics.md#flux) is zero, and circulation is $2\pi$. The [divergence](#divergence) and [curl](#curl) predict exactly which boundary measurement survives.

Why is this useful? A [velocity field](fluid-mechanics.md#velocity-field) can move material through a boundary or circulate it within a region. [Conservation of mass](continuum-mechanics.md#mass-conservation) connects its [divergence](#divergence) with density changes through the [continuity equation](physics.md#continuity-equation); its [curl](#curl) is [vorticity](fluid-mechanics.md#vorticity). In [electromagnetism](electromagnetism.md), the [Maxwell equations](electromagnetism.md#maxwell-equations) use the same operators to connect [electric fields](electromagnetism.md#electric-field), [magnetic fields](electromagnetism.md#magnetic-field), and their sources. The common mathematical language lets the same integral calculations work across different physical models. [OpenStax: Divergence, curl, and their interpretations](https://openstax.org/books/calculus-volume-3/pages/6-5-divergence-and-curl).

The geometric framework behind these operators is developed in [differential forms](differential-form.md). The [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) unifies the [fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals), [Green theorem](#green-theorem), [Stokes theorem](#stokes-theorem), and [divergence theorem](#divergence-theorem). In coordinates their formulas look different, but each relates accumulation over a region to a measurement on its boundary.

[Wilson's Vector Analysis](#vector-analysis-book), published in 1901, was based on J. Willard Gibbs's lectures at Yale. Wilson's preface explains that examples from geometry, mechanics, and physics are interspersed with the mathematical development, so readers encounter applications as soon as they have the tools to understand them. That is a useful way to approach [vector calculus](#vector-calculus): learn each operation through a measurement it makes possible. [Wilson: Vector Analysis, 1901, title page and general preface](https://archive.org/details/vectoranalysiste00gibbiala).

#### Vector Analysis (book)

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_Analysis)

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

For a continuously differentiable [vector field](#vector-field), the divergence is the limiting outward [flux](physics.md#flux) per unit volume through a small closed surface. Opposite faces of a small rectangular box almost cancel; the remaining differences in the three components give the sum of [partial derivatives](#partial-derivative) above. The [divergence theorem](#divergence-theorem) extends this local balance to a whole region.

For $F=(x,y,0)$, the divergence is $1+1+0=2$. In a planar unit square, the right edge contributes outward [flux](physics.md#flux) $1$ and the top contributes $1$, while the left and bottom contribute zero. The total $2$ equals the integral of the planar divergence over area $1$.

If $F$ is a [velocity field](fluid-mechanics.md#velocity-field), positive divergence means local volume expansion, not automatically creation of mass. The [continuity equation](physics.md#continuity-equation) gives $D\rho/Dt=-\rho\,\nabla\cdot F$, where $D/Dt$ is the [material derivative](continuum-mechanics.md#material-derivative). For this field, a uniform initial [density](fluid-mechanics.md#density) evolves as $\rho(t)=\rho(0)e^{-2t}$ while material volumes grow as $e^{2t}$. Their product stays constant.

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

For a continuously differentiable [vector field](#vector-field) in three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm), the component of its curl along a [unit normal vector](differential-geometry.md#unit-normal) is the limiting circulation per unit area around a small loop in the perpendicular plane. The loop direction and the normal obey the [right-hand rule](electromagnetism.md#right-hand-rule). [Stokes theorem](#stokes-theorem) gives the corresponding relation for a finite surface.

For the rigidly rotating [velocity field](fluid-mechanics.md#velocity-field) $G=(-\Omega y,\Omega x,0)$, direct differentiation gives $\nabla\times G=(0,0,2\Omega)$. A circle of radius $R$ has tangential speed $\Omega R$ and circumference $2\pi R$, so its circulation is $2\pi\Omega R^2$, twice the [angular velocity](classical-mechanics.md#angular-velocity) times the enclosed area. The factor of two distinguishes [vorticity](fluid-mechanics.md#vorticity) from rigid-body angular velocity.

Curved [integral curves](#integral-curve-of-a-vector-field) alone do not demonstrate nonzero curl. The field $H=(x,-y,0)$ has zero curl, yet its trajectories satisfy $x=x_0e^t$, $y=y_0e^{-t}$ and hence $xy=x_0y_0$: away from the axes they are [hyperbolas](geometry-and-topology.md#hyperbola). The curl measures local circulation of the field, not the curvature of an individual trajectory.

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

Let $V$ be a bounded region in [Euclidean space](functional-analysis.md#euclidean-norm) with piecewise smooth boundary and outward [unit normal vector](differential-geometry.md#unit-normal) $n$. For a continuously differentiable [vector field](#vector-field) $F$ on a neighborhood of its closure,

$$
\int_V\nabla\cdot F\,dV=\int_{\partial V}F\cdot n\,dS.
$$

The total outward [flux](physics.md#flux) equals the accumulated [divergence](#divergence) inside. Contributions across shared internal faces cancel when a region is divided into small pieces.

For $F=(x,y,z)$ on a ball of radius $R$, the divergence is $3$, giving $3(4\pi R^3/3)=4\pi R^3$. On the boundary, $F\cdot n=R$, so the [surface integral](#surface-integral) is also $R(4\pi R^2)=\boxed{4\pi R^3}$. This agreement turns the derivative into a geometric flux measurement. The required regularity matters: a singular field at the center cannot be included without checking its contribution separately.

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

For a continuously differentiable [function](function.md) $\Phi$ and a piecewise smooth [parametric curve](topology.md#parametric-curve) $\gamma$ from $a$ to $b$,

$$
\int_\gamma\nabla\Phi\cdot d\mathbf x=\Phi(b)-\Phi(a).
$$

The [chain rule](#chain-rule) converts the integrand into $d(\Phi(\gamma(t)))/dt$, then the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) supplies the endpoint difference. This is why a [conservative vector field](#conservative-vector-field) has a [path independent](#path-independence) [line integral](#line-integral). For $\Phi(x,y)=x^2+y^2$, every path from $(0,0)$ to $(1,2)$ gives $5$, provided it lies in the domain where the potential is defined.

##### Path independence

↑ **Parent:** [Fundamental theorem for line integrals](#fundamental-theorem-for-line-integrals)

A line integral is path independent when its value depends only on the two endpoints. On a connected domain, this holds for the line integral of every [exact differential](differential-form.md#exact-differential).

For a vector-field [line integral](#line-integral), this condition is equivalent to the field being a [conservative vector field](#conservative-vector-field).

#### Stokes theorem

↑ **Parent:** [Vector calculus](#vector-calculus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stokes_theorem)

Let $S$ be an oriented smooth surface with piecewise smooth boundary, and let $F$ be a continuously differentiable [vector field](#vector-field) on a neighborhood of $S$. With the compatible boundary direction determined by the [right-hand rule](electromagnetism.md#right-hand-rule),

$$
\int_S(\nabla\times F)\cdot n\,dS=\oint_{\partial S}F\cdot d\mathbf x.
$$

For $G=(-y,x,0)$ on the horizontal unit disc with upward normal, the left side is $2$ times its area, giving $2\pi$. The counterclockwise boundary has tangential field of magnitude one and circumference $2\pi$, giving the same [line integral](#line-integral). Reversing the surface normal reverses the boundary direction and both signs. The theorem replaces a circulation calculation with a [surface integral](#surface-integral) of the [curl](#curl), whichever is easier.

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

The [change of variables formula](#change-of-variables-formula) expresses an [integral](#integral) in coordinates that make its [integrand](#integrand) or its region simpler. Three ingredients change together: the region, the [function](function.md) being integrated, and the element of [area](differential-geometry.md#surface-area) or volume. The last change is measured by the absolute [Jacobian determinant](#jacobian-determinant); forgetting it amounts to counting transformed cells as though their sizes had stayed the same.

In one dimension, substitution is the integrated [chain rule](#chain-rule). If $g$ is [continuously differentiable](#continuously-differentiable-function) on $[a,b]$ and $f$ is [continuous](#continuous-function) on its image, then

$$
\int_a^b f(g(x))g'(x)\,dx=\int_{g(a)}^{g(b)}f(u)\,du.
$$

These are directed [definite integrals](#definite-integral): if $g$ decreases, the transformed endpoints reverse. This identity does not require $g$ to be [injective](algebra.md#injective-function), because an [antiderivative](#antiderivative) composed with $g$ already accounts for any backtracking.[OpenStax, Calculus Volume 1, Section 5.5: Substitution](https://openstax.org/books/calculus-volume-1/pages/5-5-substitution)

For a concrete computation, set $u=1+x^2$, so $du=2x\,dx$. The endpoints $x=0,1$ become $u=1,2$:

$$
\int_0^1\frac{2x}{1+x^2}\,dx=\int_1^2\frac{du}{u}=[\ln u]_1^2=\ln 2\approx0.693147.
$$

The numerator is precisely the [derivative](#derivative) of the expression in the denominator. Substitution reveals the familiar [natural logarithm](#natural-logarithm) hidden inside this [rational function](isolated-singularity.md#rational-function). Keeping the original endpoints after changing the [integrand](#integrand) would describe a different [integral](#integral).

For the elementary two-dimensional theorem, let $T:U\to V$ be a $C^1$ [diffeomorphism](geometry-and-topology.md#diffeomorphism) between [open sets](topology.md#open-set) in the plane, let $S\subset U$ be a bounded region with piecewise smooth boundary, and let $f$ be [continuous](#continuous-function) on $T(S)$, with the displayed [integrals](#integral) finite. Then

$$
\iint_{T(S)}f(x,y)\,dx\,dy=\iint_S f(T(u,v))|\det DT(u,v)|\,du\,dv.
$$

Here $DT$ is the [Jacobian matrix](#jacobian-matrix). The [diffeomorphism](geometry-and-topology.md#diffeomorphism) assumption means a [bijection](function.md#bijection) with a [continuously differentiable](#continuously-differentiable-function) inverse, and ensures a nonzero [Jacobian determinant](#jacobian-determinant). This excludes overlapping sheets; the more general [area formula](#area-formula-geometric-measure-theory) handles multiplicity.[MIT 18.022: The change of variables theorem](https://math.mit.edu/~larsh/teaching/F2007/handouts/changeofvariables.pdf)

Take $S=[0,1]^2$ and the [linear map](vector-space.md#linear-map)

$$
T(u,v)=(2u+v,v),\qquad DT=\begin{pmatrix}2&1\\0&1\end{pmatrix},\qquad \det DT=2.
$$

Its inverse is $(u,v)=((x-y)/2,y)$. The square becomes a [parallelogram](geometry-and-topology.md#parallelogram) with vertices $(0,0),(2,0),(3,1),(1,1)$: base two, height one, [area](differential-geometry.md#surface-area) two. Consequently $\iint_{T(S)}1\,dx\,dy=\iint_S2\,du\,dv=2$. A nonconstant [integrand](#integrand) changes too: $\iint_{T(S)}x\,dx\,dy=\int_0^1\int_0^1(2u+v)2\,du\,dv=3$.

The direction of the map matters when selecting the factor. Here $T$ goes from the new coordinates to the original coordinates, so the factor is two. Its inverse has [Jacobian determinant](#jacobian-determinant) $1/2$, appropriate for converting [area](differential-geometry.md#surface-area) in the opposite direction. Writing down the map before computing its [Jacobian matrix](#jacobian-matrix) prevents a reciprocal-factor error.

<a id="image-a-unit-square-becomes-a-parallelogram-of-area-two-reflection-changes-the-determinant-sign-but-preserves-area"></a>
![](change-of-variables-area.png)

**[Figure 33](#image-a-unit-square-becomes-a-parallelogram-of-area-two-reflection-changes-the-determinant-sign-but-preserves-area). A unit square becomes a parallelogram of area two; reflection changes the determinant sign but preserves area**.

Now reflect the image vertically: $\widetilde T(u,v)=(2u+v,-v)$ has [Jacobian determinant](#jacobian-determinant) $-2$, but still produces [area](differential-geometry.md#surface-area) two. The sign records reversal of the [orientation of a vector space](linear-algebra.md#orientation-of-a-vector-space); ordinary [area](differential-geometry.md#surface-area) uses its absolute value. For oriented [differential forms](differential-form.md), the [pullback of a differential form](differential-form.md#pullback-of-a-differential-form) instead retains the signed [determinant](linear-algebra.md#determinant).[MIT 18.952 notes: Integration of forms, Chapter 3](https://math.mit.edu/classes/18.952/spring2013/docs/book.pdf)

The geometric beauty is that a nonlinear [differentiable map](#differentiable-map) has a [local linear approximation](#local-linear-approximation): tiny [rectangles](geometry-and-topology.md#rectangle) behave approximately like these [parallelograms](geometry-and-topology.md#parallelogram). Summing their scaled contributions gives the [change of variables formula](#change-of-variables-formula). In [polar coordinates](#polar-coordinates) this factor is $r$, explaining $dx\,dy=r\,dr\,d\theta$; equal angular steps cover more [area](differential-geometry.md#surface-area) farther from the origin. Choosing suitable coordinates can simplify both the boundary and the [integrand](#integrand).[OpenStax, Calculus Volume 3, Section 5.7: Change of variables in multiple integrals](https://openstax.org/books/calculus-volume-3/pages/5-7-change-of-variables-in-multiple-integrals)

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

The inverse function theorem answers a practical question: **can nearby outputs be used to recover nearby inputs uniquely and smoothly?** Its useful surprise is that a nonlinear [function](function.md) can be tested using its linear [derivative](#derivative). If the first-order changes preserve all input directions, then, on a sufficiently small region, the nonlinear map can also be reversed. This is the basis for treating a nonlinear map as a [coordinate transformation](differential-geometry.md#smooth-transition-map).

Precisely, let $f:U\to\mathbb R^n$ be [continuously differentiable](#continuously-differentiable-function) on an [open subset](topology.md#open-set) $U$ of [Euclidean space](functional-analysis.md#euclidean-norm), let $a\in U$, and put $b=f(a)$. If $Df(a)$ is an [invertible linear map](#invertible-linear-map), there are [open](topology.md#open-set) [neighbourhoods](topology.md#neighbourhood-mathematics) $U_0$ of $a$ and $V_0$ of $b$ such that $f:U_0\to V_0$ is a [bijection](function.md#bijection) with a [continuously differentiable](#continuously-differentiable-function) [inverse function](function.md#inverse-function) $g$. Thus this [restriction](function.md#restriction-mathematics) is a [diffeomorphism](geometry-and-topology.md#diffeomorphism). In coordinates the test is $\det Df(a)\ne0$, using the [Jacobian determinant](#jacobian-determinant). The [derivative of a local inverse map](#derivative-of-a-local-inverse-map) is obtained by inverting the [Jacobian matrix](#jacobian-matrix), at the corresponding input. [University of Toronto MAT237: the inverse function theorem](https://www.math.utoronto.ca/courses/mat237y1/20199/notes/Chapter3/S3.3.html)

For a one-dimensional example, $f(x)=x^2$ has $f'(1)=2$. Near $x=1$, the [inverse function](function.md#inverse-function) is $g(y)=\sqrt y$, and the [inverse function rule](function.md#inverse-function-rule) gives $g'(1)=1/2$. But $x^2$ has no [inverse function](function.md#inverse-function) on the whole [real line](real-analysis.md#real-line), since $x$ and $-x$ give the same output. The theorem supplies a local [restriction](function.md#restriction-mathematics), not global [injectivity](algebra.md#injective-function). At zero, the derivative test fails; the nonnegative branch still has a [square root](algebra.md#square-root) inverse, but that inverse has no finite [derivative](#derivative) at zero. [Jiří Lebl, Basic Analysis: the one-dimensional theorem and the square-root example](https://www.jirka.org/ra/html/sec_ift.html)

Here is a two-dimensional example with an invertible [derivative](#derivative) everywhere and infinitely repeated outputs:

$$
f(s,\theta)=(e^s\cos\theta,e^s\sin\theta),\qquad
Df(s,\theta)=e^s
\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix},\qquad
\det Df=e^{2s}>0.
$$

The [exponential function](#exponential-function) turns $s$ into a positive radius, while $\theta$ is the [angle](geometry-and-topology.md#angle) in [polar coordinates](#polar-coordinates). Restricting, for example, to $|s|<0.35$ and $|\theta|<0.6$ produces the reversible patch pictured below. On its image, with Cartesian coordinates $(u,v)$ and $u>0$, the [inverse function](function.md#inverse-function) is

$$
s=\frac12\log(u^2+v^2),\qquad \theta=\arctan(v/u).
$$

The [arctangent](geometry-and-topology.md#inverse-tangent) selects the angle near zero. Without an angle [restriction](function.md#restriction-mathematics), $f(s,\theta+2\pi k)=f(s,\theta)$ for every [integer](number-theory.md#integer) $k$, so there is no single global [inverse function](function.md#inverse-function). This map is a [local diffeomorphism](#local-diffeomorphism) but is not [injective](algebra.md#injective-function).

<a id="image-a-small-rectangular-coordinate-patch-maps-reversibly-to-a-curved-sector-despite-global-angle-repetition"></a>
![](inverse-function-theorem-local-grid.png)

**[Figure 34](#image-a-small-rectangular-coordinate-patch-maps-reversibly-to-a-curved-sector-despite-global-angle-repetition). A small rectangular coordinate patch maps reversibly to a curved sector, despite global angle repetition**.

The short proof idea is to correct a guessed input using the inverse linear response. With $A=Df(a)$, solving $f(x)=y$ is equivalent to finding a [fixed point](function.md#fixed-point) of

$$
T_y(x)=x+A^{-1}(y-f(x)).
$$

At $a$, the [derivative](#derivative) $DT_y(a)=I-A^{-1}Df(a)$ vanishes. Continuity makes $T_y$ a [contraction mapping](analysis.md#contraction-mapping) on a sufficiently small [closed ball](topological-analysis.md#closed-ball), which it maps into itself when $y$ is sufficiently close to $b$. The [contraction mapping theorem](analysis.md#contraction-mapping-theorem) then gives existence and uniqueness there. Establishing the smooth dependence on $y$ completes the inverse theorem. This explains why the nonlinearity can be tolerated: its correction has a small local slope.[§8.5: the contraction argument](mathematics-bibliography.md#basic-analysis-introduction-to-real-analysis-volume-ii-by-jiri-lebl/8-5-inverse-and-implicit-function-theorems)

##### Derivative of a local inverse map

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)

For the [continuously differentiable](#continuously-differentiable-function) [inverse function](function.md#inverse-function) $g$ supplied by the [inverse function theorem](#inverse-function-theorem), the [chain rule](#chain-rule) applied to $f(g(y))=y$ gives

$$
Df(g(y))Dg(y)=I,\qquad
Dg(y)=[Df(g(y))]^{-1}.
$$

Here $I$ is the [identity matrix](vector-space.md#identity-matrix). The [matrix inverse](linear-algebra.md#matrix-inverse) is taken at the recovered input $g(y)$, not at the output $y$. In one dimension this is the [inverse function rule](function.md#inverse-function-rule) $g'(y)=1/f'(g(y))$.

The formula also describes sensitivity. For a small output perturbation $h$, [differentiability](analysis.md#differentiability) gives $g(y+h)-g(y)=Dg(y)h+o(\|h\|)$. A large [operator norm](continuous-dual-space.md#operator-norm) of $Dg(y)$ permits large amplification in some directions. In the [square root](algebra.md#square-root) example, $g'(y)=1/(2\sqrt y)$ grows without bound as positive $y$ approaches zero. Existence of a local [inverse function](function.md#inverse-function) therefore does not imply that recovery is insensitive to measurement error.

##### Constant rank theorem

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constant_rank_theorem)

The constant rank theorem separates the directions a [smooth map](differential-geometry.md#smooth-map-between-manifolds) preserves from the directions it forgets. If a [smooth map](differential-geometry.md#smooth-map-between-manifolds) from an [open subset](topology.md#open-set) of $\mathbb R^m$ to $\mathbb R^n$ has [derivative](#derivative) of constant [rank](linear-algebra.md#rank-one-quadratic-form) $r$ on a neighbourhood of a point, there are local [coordinate transformations](differential-geometry.md#smooth-transition-map) in source and target in which it becomes

$$
(x^1,\ldots,x^m)\longmapsto(x^1,\ldots,x^r,0,\ldots,0).
$$

It keeps $r$ coordinates, discards the other $m-r$, and inserts $n-r$ zeros. This is stronger than simplifying the [Jacobian matrix](#jacobian-matrix) at one point: it straightens the actual nonlinear map on a neighbourhood. [Eleny Ionel, Differential Topology, notes by Andrew Lin (2023), Theorem 44](https://web.stanford.edu/~lindrew/math215B.pdf)

For a worked example, take

$$
f(x,y)=(x+y,(x+y)^2),\qquad
Df(x,y)=
\begin{pmatrix}1&1\\2(x+y)&2(x+y)\end{pmatrix}.
$$

The two columns agree, and the first row is nonzero, so the [rank](linear-algebra.md#rank-one-quadratic-form) is exactly one everywhere. The [image of a function](set-theory.md#image-of-a-function) is the [parabola](geometry-and-topology.md#parabola) $b=a^2$. Every [line](geometry-and-topology.md#straight-line) $x+y=a$ is a [fiber](function.md#fiber-of-a-function) mapping to the same point $(a,a^2)$.

Choose input coordinates $u=x+y$, $v=x-y$, and output coordinates $\alpha=a$, $\beta=b-a^2$. Both [coordinate transformations](differential-geometry.md#smooth-transition-map) are [diffeomorphisms](geometry-and-topology.md#diffeomorphism): their inverses are $x=(u+v)/2$, $y=(u-v)/2$ and $a=\alpha$, $b=\beta+\alpha^2$. In these coordinates,

$$
(u,v)\longmapsto(u,u^2)\longmapsto(u,0).
$$

The curved image has become a straight [line](geometry-and-topology.md#straight-line), and the unused coordinate $v$ is explicit.

<a id="image-a-rank-one-map-collapses-input-fibres-to-a-parabola-which-a-change-of-output-coordinates-straightens"></a>
![](constant-rank-straightening.png)

**[Figure 35](#image-a-rank-one-map-collapses-input-fibres-to-a-parabola-which-a-change-of-output-coordinates-straightens). A rank-one map collapses input fibres to a parabola, which a change of output coordinates straightens**.

Constant [rank](linear-algebra.md#rank-one-quadratic-form) on a neighbourhood is essential. The map $(x,y)\mapsto(x,y^2)$ has [rank](linear-algebra.md#rank-one-quadratic-form) one when $y=0$ and two when $y\ne0$, so the constant rank theorem does not supply one rank-one form across that line. By contrast, the full-rank square case of the theorem forgets no coordinates and recovers the [inverse function theorem](#inverse-function-theorem). The usefulness is that curved [fibers](function.md#fiber-of-a-function) and images can often be studied through this simpler local form.

###### Rank-one level curves from a characteristic differential equation

↑ **Parent:** [Constant rank theorem](#constant-rank-theorem)

For a smooth map $F=(f,g)$ on the plane with zero Jacobian determinant and $f_y\ne0$, set $e=g_y/f_y$. The determinant identity gives $\nabla g=e\nabla f$. Along a curve solving $y'=-f_x/f_y$, both $f$ and $g$ have zero derivative. Local existence and uniqueness for this smooth differential equation through every nearby point produce a local foliation by curves of constant $F$.

##### Local diffeomorphism

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_diffeomorphism)

A local diffeomorphism is a [differentiable map](#differentiable-map) that restricts near every point to a [diffeomorphism](geometry-and-topology.md#diffeomorphism) onto an [open subset](topology.md#open-set) of its target. The local [inverse functions](function.md#inverse-function) need not combine into a single global [inverse function](function.md#inverse-function): different parts of the [domain of a function](function.md#domain-of-a-function) can map onto the same output region.

For [continuously differentiable](#continuously-differentiable-function) maps between [open subsets](topology.md#open-set) of $\mathbb R^n$, being a [local diffeomorphism](#local-diffeomorphism) is equivalent to having an invertible [derivative](#derivative) at every point. The [inverse function theorem](#inverse-function-theorem) proves one direction. For the other, the [chain rule](#chain-rule) for each local [inverse function](function.md#inverse-function) gives two inverse [linear maps](vector-space.md#linear-map). The periodic angle example under the [inverse function theorem](#inverse-function-theorem) has this property everywhere, even though it has infinitely many inputs for every point of the punctured plane. The [noninjective map with constant Jacobian determinant](#noninjective-map-with-constant-jacobian-determinant) gives another useful distinction: even a constant nonzero [Jacobian determinant](#jacobian-determinant) need not give global [injectivity](algebra.md#injective-function).

Every [local diffeomorphism](#local-diffeomorphism) is an [open map](#open-map). To see this, take an [open subset](topology.md#open-set) of the source and intersect it with the neighbourhoods where the map is a [diffeomorphism](geometry-and-topology.md#diffeomorphism). Each local image is [open](topology.md#open-set), and their [union](set.md#set-union) is the full image. Thus nearby outputs remain available locally, despite the possible global ambiguity.

###### Noninjective map with constant Jacobian determinant

↑ **Parent:** [Local diffeomorphism](#local-diffeomorphism)

The displayed [smooth map](differential-geometry.md#smooth-map-between-manifolds) from $\mathbb R^2$ to the punctured plane has [Jacobian determinant](#jacobian-determinant) one: in [polar coordinates](#polar-coordinates) its radius is $e^s$ and its angle is $re^{-2s}$, so the determinant is $e^{2s}e^{-2s}=1$. Nevertheless $a(0,2\pi k)=(1,0)$ for every integer $k$. Thus a local volume-preserving map need not be injective or have bounded [weighted inverse multiplicity](#weighted-inverse-multiplicity). Compactly supported data distributed over many inverse branches disprove a determinant-only [dispersion with a nonlinear velocity map](partial-differential-equation.md#dispersion-with-a-nonlinear-velocity-map) estimate.

###### Open map

↑ **Parent:** [Local diffeomorphism](#local-diffeomorphism)

An open map sends every [open subset](topology.md#open-set) of its source to an [open subset](topology.md#open-set) of its target. This is an image property; [continuity](#continuous-function) instead concerns [preimages](set-theory.md#preimage) of [open sets](topology.md#open-set). A [local diffeomorphism](#local-diffeomorphism) has both properties, but openness alone does not promise unique recovery of an input. In the periodic coordinate map under the [inverse function theorem](#inverse-function-theorem), open patches give open output regions while multiple angle values still give the same output.

Together, [open and closed maps](topology.md#open-and-closed-maps) describe the two image-set preservation properties.

##### Implicit function theorem

↑ **Parent:** [Inverse function theorem](#inverse-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_function_theorem)

An equation can define a [function](function.md) without giving an explicit formula for it. The implicit function theorem tells us when the constraint $F(x,y)=0$ determines $y$ uniquely from nearby $x$, and makes the resulting [function](function.md) [continuously differentiable](#continuously-differentiable-function). It is useful when solving an equation explicitly is cumbersome or impossible: the [partial derivatives](#partial-derivative) already reveal whether local recovery is possible.

Let $F$ be a [continuously differentiable](#continuously-differentiable-function) map from an [open subset](topology.md#open-set) of $\mathbb R^m\times\mathbb R^n$ to $\mathbb R^n$. Suppose $F(x_0,y_0)=0$ and the [partial derivative](#partial-derivative) $D_yF(x_0,y_0)$ is an [invertible linear map](#invertible-linear-map). There are [open](topology.md#open-set) [neighbourhoods](topology.md#neighbourhood-mathematics) $U$ of $x_0$ and $V$ of $y_0$ and a unique [continuously differentiable](#continuously-differentiable-function) [function](function.md) $g:U\to V$ such that, for $(x,y)\in U\times V$,

$$
F(x,y)=0\quad\Longleftrightarrow\quad y=g(x),\qquad g(x_0)=y_0.
$$

Thus the nearby [level set](topology.md#level-set) is a [graph of a function](function.md#graph-of-a-function). The [derivative](#derivative) of this graph is

$$
Dg(x)=-[D_yF(x,g(x))]^{-1}D_xF(x,g(x)).
$$

The [matrix inverse](linear-algebra.md#matrix-inverse) acts on the left; the order matters in several dimensions.

For example, take the [unit circle](complex-analysis.md#complex-unit-circle), written as the [level set](topology.md#level-set) $F(x,y)=x^2+y^2-1=0$. At $(x_0,y_0)=(3/5,4/5)$, $F_y=2y_0=8/5\ne0$, so the local upper branch is $y=g(x)=\sqrt{1-x^2}$. [Implicit differentiation](#implicit-differentiation) gives

$$
g'(x)=-\frac{F_x}{F_y}=-\frac{x}{y},\qquad
\boxed{g'(3/5)=-3/4.}
$$

This [tangent line](#tangent-line) slope is available directly from the constraint. The negative [square root](algebra.md#square-root) branch is elsewhere on the same [circle](topology.md#circle); it does not destroy uniqueness near the selected upper point.

<a id="image-the-same-circle-uses-y-as-a-function-of-x-near-its-upper-arc-and-x-as-a-function-of-y-near-its-rightmost-point"></a>
![](implicit-function-theorem-circle-charts.png)

**[Figure 36](#image-the-same-circle-uses-y-as-a-function-of-x-near-its-upper-arc-and-x-as-a-function-of-y-near-its-rightmost-point). The same circle uses y as a function of x near its upper arc and x as a function of y near its rightmost point**.

At $(1,0)$, however, $F_y=0$ and the [circle](topology.md#circle) cannot be represented locally as one [function](function.md) $y=g(x)$: just to the left of $x=1$ there are two nearby values of $y$. The [circle](topology.md#circle) is still smooth there. Since $F_x=2\ne0$, use the other coordinate instead: $x=h(y)=\sqrt{1-y^2}$, with $h'(0)=0$. A failed coordinate choice is different from a geometric singularity.

The derivative condition is sufficient, not necessary for every possible implicit graph. For $F(x,y)=y^3$, the entire zero set is the smooth graph $y=0$, even though $F_y$ vanishes there. In this case the defining equation itself has a degenerate [derivative](#derivative); the theorem's test gives no conclusion.

The connection to the [inverse function theorem](#inverse-function-theorem) is particularly elegant. Augment the constraint to the map $H(x,y)=(x,F(x,y))$, whose [Jacobian matrix](#jacobian-matrix) is

$$
DH=
\begin{pmatrix}I&0\\D_xF&D_yF\end{pmatrix}.
$$

Its [determinant](linear-algebra.md#determinant) is $\det D_yF$. When this is nonzero, locally invert $H$ and set its second output to zero. The recovered second input is $g(x)$. In this way an implicit constraint becomes an ordinary [inverse function](function.md#inverse-function) problem. [University of Toronto MAT237: the implicit theorem as a corollary of the inverse theorem](https://www.math.utoronto.ca/courses/mat237y1/20199/notes/Chapter3/S3.3.html)

###### Holomorphic implicit function theorem

↑ **Parent:** [Implicit function theorem](#implicit-function-theorem)

If a holomorphic function $F(z,w)$ satisfies $F(z_0,w_0)=0$ and $F_w(z_0,w_0)\ne0$, then near $(z_0,w_0)$ its zero set is the graph $w=g(z)$ of a unique holomorphic function. The analogous statement with $F_z\ne0$ uses $w$ as the local coordinate.

###### Implicit differentiation

↑ **Parent:** [Implicit function theorem](#implicit-function-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Implicit_differentiation)

Implicit differentiation differentiates an identity $F(x,y(x))=0$ along a [differentiable](analysis.md#differentiable-function) branch and uses the [chain rule](#chain-rule) to solve for its [derivative](#derivative):

$$
F_x+F_y\,y'=0,\qquad y'=-\frac{F_x}{F_y}\quad(F_y\ne0).
$$

The [partial derivatives](#partial-derivative) $F_x,F_y$ treat $x,y$ as independent coordinates before evaluating on the branch. The [implicit function theorem](#implicit-function-theorem) justifies the branch's local existence and regularity under its hypotheses; differentiating alone does not establish either. For the [unit circle](complex-analysis.md#complex-unit-circle) at $(3/5,4/5)$, this calculation yields the [tangent line](#tangent-line) $y-4/5=-(3/4)(x-3/5)$.

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

[Integration by parts](#integration-by-parts) transfers a [derivative](#derivative) from one factor of a product to the other, while keeping an endpoint contribution. Its usefulness comes from choosing which factor becomes simpler when differentiated, and which has an accessible [antiderivative](#antiderivative). The [integral](#integral) is then replaced by a [boundary term](#boundary-term) minus another [integral](#integral).

For real [continuously differentiable functions](#continuously-differentiable-function) $u,v$ on $[a,b]$, the precise [definite integral](#definite-integral) formula is

$$
\int_a^b u(x)v'(x)\,dx=[u(x)v(x)]_a^b-\int_a^b u'(x)v(x)\,dx,
\qquad [uv]_a^b=u(b)v(b)-u(a)v(a).
$$

In the shorter notation, $du=u'(x)\,dx$ and $dv=v'(x)\,dx$, giving $\int u\,dv=uv-\int v\,du$ for [indefinite integrals](#antiderivative), with a [constant of integration](#constant-of-integration) understood. The [product rule](#product-rule) says $(uv)'=u'v+uv'$; the [fundamental theorem of calculus](#fundamental-theorem-of-calculus) turns its [integral](#integral) into the endpoint difference. Thus the formula packages a differentiation rule into a tool for [integration](#integral).[OpenStax, Calculus Volume 2, Section 3.1: Integration by parts](https://openstax.org/books/calculus-volume-2/pages/3-1-integration-by-parts)

For example, choose $u=x$ and $dv=e^x\,dx$. Then $du=dx$ and $v=e^x$, since the [exponential function](#exponential-function) is its own [derivative](#derivative):

$$
\int_0^1 xe^x\,dx=[xe^x]_0^1-\int_0^1e^x\,dx=e-(e-1)=1.
$$

The [boundary term](#boundary-term) is $e\approx2.718282$; the remaining [integral](#integral) is $e-1\approx1.718282$. Their difference is exactly one. The endpoint product alone would overcount, because its [derivative](#derivative) includes $u'v=e^x$ as well as the desired $uv'=xe^x$.

<a id="image-integration-by-parts-splits-the-accumulated-product-derivative-into-the-desired-integral-and-the-remaining-integral"></a>
![](integration-by-parts-example.png)

**[Figure 37](#image-integration-by-parts-splits-the-accumulated-product-derivative-into-the-desired-integral-and-the-remaining-integral). Integration by parts splits the accumulated product derivative into the desired integral and the remaining integral**.

In the figure, the [area](differential-geometry.md#surface-area) under $(xe^x)'=(1+x)e^x$ is the endpoint contribution $e$. Its lower band has [area](differential-geometry.md#surface-area) $e-1$, and its upper band has thickness $xe^x$ and [area](differential-geometry.md#surface-area) one. This decomposition makes the subtraction visible. The endpoint contribution is a difference of product values; it need not equal the [area](differential-geometry.md#surface-area) under either factor separately.

The same choice repeatedly lowers the [degree of a polynomial](polynomial.md#degree-of-a-polynomial) when integrating a [polynomial](polynomial.md) times an [exponential function](#exponential-function), while choosing $u=\ln x$ gives $\int\ln x\,dx=x\ln x-x+C$ for $x>0$. More broadly, moving a [derivative](#derivative) onto a convenient test function is the mechanism behind a [weak derivative](distribution-theory.md#weak-derivative). Always evaluate the [boundary term](#boundary-term): it disappears only when the relevant endpoint values justify doing so, often through a [boundary condition](differential-equation.md#boundary-condition).

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

The [Taylor series](#taylor-series) at zero begins

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

An even function satisfies $f(-x)=f(x)$; its [Laurent series](analysis.md#laurent-series) or [Taylor series](#taylor-series) contains only even powers.

## Odd function

↑ **Parent:** [Calculus](calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Odd_function)

An odd function satisfies $f(-x)=-f(x)$; its [Laurent series](analysis.md#laurent-series) or [Taylor series](#taylor-series) contains only odd powers.

### Odd extension

↑ **Parent:** [Odd function](#odd-function)

An odd extension of a function $f$ on the positive half-line is $\widetilde f(r)=f(r)$ for $r>0$ and $\widetilde f(r)=-f(-r)$ for $r<0$. At zero it is set to zero when the boundary value is zero. Smoothness requires compatible even derivatives at zero. In the [radial reduction of the three-dimensional wave equation](wave-equation.md#radial-reduction-of-the-three-dimensional-wave-equation), $r\phi(t,r)$ has a smooth [odd extension](#odd-extension) whenever $\phi$ is smooth and radial.

## ↑ Ancestors (5)

1. [Real analysis](real-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Brownian motion](brownian-motion.md)
- [Critical point](analysis.md#critical-point)
- [Differential geometry](differential-geometry.md)
- [Exponential function](#exponential-function)
- [Fluid mechanics](fluid-mechanics.md)
- [Mathematical optimization](mathematical-optimization.md)
- [Mathematics](mathematics.md)
