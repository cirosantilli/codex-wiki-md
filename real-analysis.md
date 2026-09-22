# Real analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real_analysis)

Real analysis studies limits, continuity, differentiation, integration, and convergence for real-valued functions.

**Table of contents**

- [Hardy's inequality](#hardy-s-inequality)
- [Infimum and supremum](#infimum-and-supremum)
  - [Essential infimum and essential supremum](#essential-infimum-and-essential-supremum)
    - [Essential infimum](#essential-infimum)
  - [Supremum](#supremum)
    - [Accumulation below an unattained supremum](#accumulation-below-an-unattained-supremum)
  - [Infimum](#infimum)
- [Asymptotic analysis](#asymptotic-analysis)
  - [Asymptotic equivalence](#asymptotic-equivalence)
    - [Asymptotic comparison of exponential functions](#asymptotic-comparison-of-exponential-functions)
    - [Stirling formula](#stirling-formula)
      - [Stirling correction by Gaussian moments](#stirling-correction-by-gaussian-moments)
- [Monotone integral Tauberian lemma](#monotone-integral-tauberian-lemma)
- [Homogeneous function](#homogeneous-function)
  - [Homogeneity](#homogeneity)
  - [Positively homogeneous function (degree one)](#positively-homogeneous-function-degree-one)
  - [Euler theorem for homogeneous functions](#euler-theorem-for-homogeneous-functions)
    - [Euler differential identity characterizes homogeneity](#euler-differential-identity-characterizes-homogeneity)
    - [Volume integral of a homogeneous function](#volume-integral-of-a-homogeneous-function)
- [Regular variation](#regular-variation)
  - [Slowly varying function](#slowly-varying-function)
- [Lipschitz continuity](#lipschitz-continuity)
  - [Bounded Lipschitz norm](#bounded-lipschitz-norm)
    - [Diagonal compactness for bounded Lipschitz functions](#diagonal-compactness-for-bounded-lipschitz-functions)
    - [Pointwise closure of the bounded Lipschitz unit ball](#pointwise-closure-of-the-bounded-lipschitz-unit-ball)
  - [One-sided Lipschitz condition](#one-sided-lipschitz-condition)
  - [Lipschitz domain](#lipschitz-domain)
  - [McShane extension theorem](#mcshane-extension-theorem)
  - [Lipschitz constant](#lipschitz-constant)
  - [Globally Lipschitz function](#globally-lipschitz-function)
  - [Lipschitz bound](#lipschitz-bound)
  - [Locally Lipschitz function](#locally-lipschitz-function)
- [Big O notation](#big-o-notation)
- [Real line](#real-line)
  - [Interval (mathematics)](#interval-mathematics)
    - [Nested intervals](#nested-intervals)
      - [Nested interval theorem](#nested-interval-theorem)
    - [Closed real interval](#closed-real-interval)
- [Extreme value theorem](#extreme-value-theorem)
  - [Interior-value criterion for an attained maximum](#interior-value-criterion-for-an-attained-maximum)
  - [Supremum can fail to be attained at an oscillatory endpoint](#supremum-can-fail-to-be-attained-at-an-oscillatory-endpoint)
- [Coercive function](#coercive-function)
  - [Range of a continuous coercive real function](#range-of-a-continuous-coercive-real-function)
- [Lp norm](#lp-norm)
  - [Lq quasi-norm](#lq-quasi-norm)
  - [Minkowski inequality](#minkowski-inequality)
  - [L2 norm](#l2-norm)
  - [Marcinkiewicz–Zygmund inequality](#marcinkiewicz-zygmund-inequality)
  - [Hölder's inequality](#holder-s-inequality)
- [Sequence and series](#sequence-and-series)
  - [Dyadic-block alternation of reciprocal terms](#dyadic-block-alternation-of-reciprocal-terms)
  - [Lucas number](#lucas-number)
  - [Sequence](#sequence)
    - [Limit inferior and limit superior](#limit-inferior-and-limit-superior)
      - [Limit inferior](#limit-inferior)
    - [Recurrence relation](#recurrence-relation)
      - [Difference equation](#difference-equation)
    - [Thue–Morse sequence](#thue-morse-sequence)
      - [Thue–Morse Fourier product](#thue-morse-fourier-product)
        - [Uniform interval cancellation for binary digit parity](#uniform-interval-cancellation-for-binary-digit-parity)
          - [Small Type I sums for binary digit parity](#small-type-i-sums-for-binary-digit-parity)
    - [Cluster-set matching of bounded sequences](#cluster-set-matching-of-bounded-sequences)
    - [Fejér monotonicity](#fejer-monotonicity)
    - [Finite repetition-free sequence](#finite-repetition-free-sequence)
    - [Subadditive sequence](#subadditive-sequence)
      - [Asymmetrically almost-subadditive sequence](#asymmetrically-almost-subadditive-sequence)
    - [Geometric progression](#geometric-progression)
    - [Subsequence](#subsequence)
      - [Monotone subsequence theorem](#monotone-subsequence-theorem)
    - [Null sequence](#null-sequence)
    - [Bounded sequence](#bounded-sequence)
      - [Bounded subsequence](#bounded-subsequence)
    - [Bitstream](#bitstream)
      - [Uncountability by interleaving prescribed binary coordinates](#uncountability-by-interleaving-prescribed-binary-coordinates)
    - [Monotone sequence](#monotone-sequence)
      - [Minimum-decrement convergence criterion](#minimum-decrement-convergence-criterion)
      - [Bounded nondecreasing rational sequences are uncountable](#bounded-nondecreasing-rational-sequences-are-uncountable)
      - [Bounded nondecreasing integer sequences are eventually constant](#bounded-nondecreasing-integer-sequences-are-eventually-constant)
      - [Bounded monotone sequence theorem](#bounded-monotone-sequence-theorem)
    - [Limit superior](#limit-superior)
  - [Series (mathematics)](#series-mathematics)
    - [Cesàro summation](#cesaro-summation)
    - [Factorial series](#factorial-series)
      - [Irrationality criterion for factorial series](#irrationality-criterion-for-factorial-series)
    - [Polynomial-logarithmic series convergence](#polynomial-logarithmic-series-convergence)
    - [Root test](#root-test)
    - [Telescoping series](#telescoping-series)
    - [Term test for divergence](#term-test-for-divergence)
    - [Infinite product](#infinite-product)
      - [Reciprocal geometric infinite product](#reciprocal-geometric-infinite-product)
      - [Weierstrass elementary factor](#weierstrass-elementary-factor)
      - [Infinite product convergence from logarithmic tails](#infinite-product-convergence-from-logarithmic-tails)
      - [Positive sum-product convergence criterion](#positive-sum-product-convergence-criterion)
      - [Hyperbolic-sine infinite product](#hyperbolic-sine-infinite-product)
    - [Lattice sum](#lattice-sum)
    - [Partial sum](#partial-sum)
    - [Kronecker lemma](#kronecker-lemma)
    - [Harmonic series](#harmonic-series)
      - [Alternating harmonic series](#alternating-harmonic-series)
    - [Cauchy condensation test](#cauchy-condensation-test)
  - [Fekete's lemma](#fekete-s-lemma)
  - [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem)
    - [Extended real subsequence theorem](#extended-real-subsequence-theorem)
    - [Diagonal subsequence argument](#diagonal-subsequence-argument)
    - [Unique subsequential limit of a bounded sequence](#unique-subsequential-limit-of-a-bounded-sequence)
  - [Convergent sequence](#convergent-sequence)
    - [Bounded sequence with vanishing increments need not converge](#bounded-sequence-with-vanishing-increments-need-not-converge)
    - [Limit of a sequence](#limit-of-a-sequence)
      - [Reciprocal limits and escape in absolute value](#reciprocal-limits-and-escape-in-absolute-value)
    - [Cesaro mean](#cesaro-mean)
      - [Cesaro theorem for convergent sequences](#cesaro-theorem-for-convergent-sequences)
    - [Geometric mean of a sequence](#geometric-mean-of-a-sequence)
    - [Monotone bounded sequence](#monotone-bounded-sequence)
  - [Fibonacci number](#fibonacci-number)
    - [Fibonacci recurrence matrix modulo an integer](#fibonacci-recurrence-matrix-modulo-an-integer)
    - [Fibonacci addition formula](#fibonacci-addition-formula)
      - [Fibonacci gcd reduction](#fibonacci-gcd-reduction)
    - [Binet formula](#binet-formula)
    - [Fibonacci determinant identity](#fibonacci-determinant-identity)
  - [Pointwise convergence](#pointwise-convergence)
    - [Factorial cosine iterated limit detects rationality](#factorial-cosine-iterated-limit-detects-rationality)
    - [Shrinking continuous spikes with vanishing integral](#shrinking-continuous-spikes-with-vanishing-integral)
    - [Pointwise limit](#pointwise-limit)
  - [Power series](#power-series)
    - [Generating function](#generating-function)
      - [Exponential generating function](#exponential-generating-function)
    - [Lacunary power series](#lacunary-power-series)
      - [Factorial-gap power series](#factorial-gap-power-series)
    - [Binomial series](#binomial-series)
      - [Negative binomial series](#negative-binomial-series)
    - [Majorant series](#majorant-series)
    - [Radius of convergence](#radius-of-convergence)
      - [Bounded power-series terms force interior absolute convergence](#bounded-power-series-terms-force-interior-absolute-convergence)
      - [Sum of power series with unequal radii of convergence](#sum-of-power-series-with-unequal-radii-of-convergence)
      - [Terms of a power series are unbounded outside its convergence disc](#terms-of-a-power-series-are-unbounded-outside-its-convergence-disc)
      - [Radius of convergence of a sparse power series](#radius-of-convergence-of-a-sparse-power-series)
      - [Polynomial-coefficient power series](#polynomial-coefficient-power-series)
      - [Polynomial coefficient growth with unit power-series radius](#polynomial-coefficient-growth-with-unit-power-series-radius)
      - [Cauchy-Hadamard theorem](#cauchy-hadamard-theorem)
      - [Radius of convergence after powering coefficients](#radius-of-convergence-after-powering-coefficients)
      - [Half-plane of convergence of an exponential power series](#half-plane-of-convergence-of-an-exponential-power-series)
    - [Cauchy product](#cauchy-product)
    - [Termwise differentiation of a power series](#termwise-differentiation-of-a-power-series)
    - [Leading Taylor term](#leading-taylor-term)
  - [Uniform convergence](#uniform-convergence)
    - [Uniformly vanishing functions can retain a nonzero integral](#uniformly-vanishing-functions-can-retain-a-nonzero-integral)
    - [Uniform convergence preserves integrals on a compact interval](#uniform-convergence-preserves-integrals-on-a-compact-interval)
    - [Uniform convergence at moving evaluation points](#uniform-convergence-at-moving-evaluation-points)
    - [Uniform derivative convergence with an anchored value](#uniform-derivative-convergence-with-an-anchored-value)
    - [Egorov's theorem](#egorov-s-theorem)
    - [Uniform limit theorem](#uniform-limit-theorem)
    - [Dini's theorem](#dini-s-theorem)
    - [Uniformly Cauchy sequence](#uniformly-cauchy-sequence)
    - [Locally uniform convergence](#locally-uniform-convergence)
      - [Compact-open topology](#compact-open-topology)
        - [Weighted metric for local uniform convergence](#weighted-metric-for-local-uniform-convergence)
      - [Local uniform convergence on compact subsets](#local-uniform-convergence-on-compact-subsets)
  - [Geometric series](#geometric-series)
    - [Iterated contraction gives a summable orbit](#iterated-contraction-gives-a-summable-orbit)
    - [Finite geometric series](#finite-geometric-series)
      - [Finite trigonometric sum](#finite-trigonometric-sum)
      - [Exponential geometric sum bound](#exponential-geometric-sum-bound)
  - [Cauchy sequence](#cauchy-sequence)
    - [Convergence from arbitrary variable-lag increments](#convergence-from-arbitrary-variable-lag-increments)
    - [Cauchy subsequence](#cauchy-subsequence)
    - [Completeness of the real numbers](#completeness-of-the-real-numbers)
      - [Least-upper-bound property](#least-upper-bound-property)
  - [Conditional convergence](#conditional-convergence)
    - [Riemann series theorem](#riemann-series-theorem)
      - [Rearrangement of a series](#rearrangement-of-a-series)
    - [Alternating series test](#alternating-series-test)
  - [P-series](#p-series)
  - [Absolute convergence](#absolute-convergence)
    - [Squares of a summable positive sequence](#squares-of-a-summable-positive-sequence)
    - [Geometric means of two summable positive sequences](#geometric-means-of-two-summable-positive-sequences)
    - [Weighted square roots of a summable sequence](#weighted-square-roots-of-a-summable-sequence)
  - [Total variation](#total-variation)
    - [Total generalized variation](#total-generalized-variation)
      - [TGV divergence splitting](#tgv-divergence-splitting)
  - [Harmonic sum](#harmonic-sum)
  - [Convergent series](#convergent-series)
    - [Convergence from fixed-length series blocks](#convergence-from-fixed-length-series-blocks)
    - [Dirichlet test](#dirichlet-test)
    - [Comparison test for series](#comparison-test-for-series)
      - [Ratio comparison test](#ratio-comparison-test)
      - [Clipping preserves divergence of a positive series](#clipping-preserves-divergence-of-a-positive-series)
      - [Integral test for convergence](#integral-test-for-convergence)
    - [Summable sequence](#summable-sequence)
    - [Limit comparison test](#limit-comparison-test)
    - [Ratio test](#ratio-test)
      - [Power-law comparison from a refined ratio bound](#power-law-comparison-from-a-refined-ratio-bound)
      - [Ratio limit implies root limit](#ratio-limit-implies-root-limit)
      - [Factorial-over-power series](#factorial-over-power-series)
  - [Uniform limit](#uniform-limit)
- [Calculus](calculus.md)
  - [Floor and ceiling functions](calculus.md#floor-and-ceiling-functions)
    - [Floor function](calculus.md#floor-function)
      - [Fractional part](calculus.md#fractional-part)
    - [Ceiling function](calculus.md#ceiling-function)
  - [Integral](calculus.md#integral)
    - [Wallis integrals](calculus.md#wallis-integrals)
    - [Dipole line-integral identity](calculus.md#dipole-line-integral-identity)
    - [Integrand](calculus.md#integrand)
    - [Multiple integral](calculus.md#multiple-integral)
      - [Odd-integrand cancellation by reflection](calculus.md#odd-integrand-cancellation-by-reflection)
    - [Integral representation](calculus.md#integral-representation)
      - [Trigonometric integral](calculus.md#trigonometric-integral)
        - [Cosine integral](calculus.md#cosine-integral)
        - [Sine integral](calculus.md#sine-integral)
    - [Lebesgue integration](calculus.md#lebesgue-integration)
      - [Prékopa–Leindler inequality](calculus.md#prekopa-leindler-inequality)
      - [Absolute continuity of the Lebesgue integral](calculus.md#absolute-continuity-of-the-lebesgue-integral)
    - [Time integral](calculus.md#time-integral)
    - [Double integral](calculus.md#double-integral)
    - [Monotonicity of the Lebesgue integral](calculus.md#monotonicity-of-the-lebesgue-integral)
    - [Antiderivative](calculus.md#antiderivative)
      - [Constant of integration](calculus.md#constant-of-integration)
      - [Additive constant](calculus.md#additive-constant)
    - [Gaussian integral](calculus.md#gaussian-integral)
      - [Linear-source multivariate Gaussian integral](calculus.md#linear-source-multivariate-gaussian-integral)
      - [Dawson function](calculus.md#dawson-function)
        - [Gaussian drift primitives](calculus.md#gaussian-drift-primitives)
      - [Error function](calculus.md#error-function)
        - [Quadrant asymptotics of the error function](calculus.md#quadrant-asymptotics-of-the-error-function)
        - [Complementary error function](calculus.md#complementary-error-function)
          - [Faddeeva function](calculus.md#faddeeva-function)
            - [Gaussian pole integral](calculus.md#gaussian-pole-integral)
  - [Taylor polynomial](calculus.md#taylor-polynomial)
    - [Multivariate Taylor polynomial](calculus.md#multivariate-taylor-polynomial)
  - [Exponential function](calculus.md#exponential-function)
    - [e (mathematical constant)](calculus.md#e-mathematical-constant)
      - [Irrationality of e](calculus.md#irrationality-of-e)
    - [Exponential series](calculus.md#exponential-series)
    - [Complex exponential function](calculus.md#complex-exponential-function)
      - [Modulus of the complex exponential](calculus.md#modulus-of-the-complex-exponential)
      - [Complex sine function](calculus.md#complex-sine-function)
        - [Periodicity of the complex sine](calculus.md#periodicity-of-the-complex-sine)
    - [Logarithm](calculus.md#logarithm)
      - [Geometric-series bound for the logarithmic remainder](calculus.md#geometric-series-bound-for-the-logarithmic-remainder)
      - [Irrational logarithm criterion](calculus.md#irrational-logarithm-criterion)
      - [Concavity of the logarithm](calculus.md#concavity-of-the-logarithm)
      - [Logarithmic integral function](calculus.md#logarithmic-integral-function)
      - [Natural logarithm](calculus.md#natural-logarithm)
      - [Logarithm inequality](calculus.md#logarithm-inequality)
      - [Operator monotonicity of logarithm](calculus.md#operator-monotonicity-of-logarithm)
    - [Gaussian function](calculus.md#gaussian-function)
      - [Gaussian decay dominates every power](calculus.md#gaussian-decay-dominates-every-power)
      - [Gaussian dyadic summation bound](calculus.md#gaussian-dyadic-summation-bound)
    - [Hyperbolic function](calculus.md#hyperbolic-function)
      - [Inverse hyperbolic functions](calculus.md#inverse-hyperbolic-functions)
      - [Hyperbolic cosine](calculus.md#hyperbolic-cosine)
        - [Factorial-tail irrationality proof for a hyperbolic cosine](calculus.md#factorial-tail-irrationality-proof-for-a-hyperbolic-cosine)
        - [Inverse hyperbolic cosine](calculus.md#inverse-hyperbolic-cosine)
      - [Hyperbolic sine](calculus.md#hyperbolic-sine)
      - [Hyperbolic cotangent](calculus.md#hyperbolic-cotangent)
        - [Partial-fraction expansion of the hyperbolic cotangent](calculus.md#partial-fraction-expansion-of-the-hyperbolic-cotangent)
      - [Hyperbolic secant](calculus.md#hyperbolic-secant)
  - [Fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus)
    - [Fundamental theorem of calculus for Lebesgue integration](calculus.md#fundamental-theorem-of-calculus-for-lebesgue-integration)
  - [Mean value theorem](calculus.md#mean-value-theorem)
    - [Cauchy mean value theorem](calculus.md#cauchy-mean-value-theorem)
    - [Endpoint secant-tangent approximation](calculus.md#endpoint-secant-tangent-approximation)
  - [Rolle theorem](calculus.md#rolle-theorem)
    - [Rolle root count with multiplicities](calculus.md#rolle-root-count-with-multiplicities)
  - [Taylor theorem](calculus.md#taylor-theorem)
    - [Taylor expansion from a periodic derivative equation](calculus.md#taylor-expansion-from-a-periodic-derivative-equation)
    - [Integral first-order Taylor formula for a vector map](calculus.md#integral-first-order-taylor-formula-for-a-vector-map)
    - [Integral remainder in Taylor theorem](calculus.md#integral-remainder-in-taylor-theorem)
      - [Logarithmic series from an integral Taylor remainder](calculus.md#logarithmic-series-from-an-integral-taylor-remainder)
    - [Taylor expansion](calculus.md#taylor-expansion)
      - [Peano zero](calculus.md#peano-zero)
      - [Parabolic approximation](calculus.md#parabolic-approximation)
    - [Taylor formula for a polynomial](calculus.md#taylor-formula-for-a-polynomial)
    - [Taylor theorem with Lagrange remainder](calculus.md#taylor-theorem-with-lagrange-remainder)
    - [Taylor remainder](calculus.md#taylor-remainder)
    - [Taylor formula with integral remainder](calculus.md#taylor-formula-with-integral-remainder)
    - [Taylor series](calculus.md#taylor-series)
  - [Limit of a function](calculus.md#limit-of-a-function)
    - [One-sided limit](calculus.md#one-sided-limit)
    - [Continuous function](calculus.md#continuous-function)
      - [Blancmange curve](calculus.md#blancmange-curve)
      - [Bounded continuous functions](calculus.md#bounded-continuous-functions)
      - [Upper semicontinuity](calculus.md#upper-semicontinuity)
      - [Oscillation multiplied by a vanishing amplitude](calculus.md#oscillation-multiplied-by-a-vanishing-amplitude)
      - [Lower semicontinuity](calculus.md#lower-semicontinuity)
      - [Discontinuity of a function](calculus.md#discontinuity-of-a-function)
        - [Removable discontinuity](calculus.md#removable-discontinuity)
        - [Jump discontinuity](calculus.md#jump-discontinuity)
      - [Sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity)
        - [Sublevel set](calculus.md#sublevel-set)
          - [Compact sublevel set](calculus.md#compact-sublevel-set)
        - [Closed-sublevel-set characterization of lower semicontinuity](calculus.md#closed-sublevel-set-characterization-of-lower-semicontinuity)
      - [Locally constant function](calculus.md#locally-constant-function)
        - [Compactly supported locally constant function](calculus.md#compactly-supported-locally-constant-function)
      - [Intermediate value theorem](calculus.md#intermediate-value-theorem)
        - [Continuous image of a real interval](calculus.md#continuous-image-of-a-real-interval)
        - [Interval order theorem for continuous injections](calculus.md#interval-order-theorem-for-continuous-injections)
        - [Horizontal chord of reciprocal-integer length](calculus.md#horizontal-chord-of-reciprocal-integer-length)
        - [Zero on a line segment](calculus.md#zero-on-a-line-segment)
        - [Telescoping increment lemma](calculus.md#telescoping-increment-lemma)
        - [Continuous bijection of the real line is monotone](calculus.md#continuous-bijection-of-the-real-line-is-monotone)
      - [Composition of continuous functions](calculus.md#composition-of-continuous-functions)
      - [Continuity set of a function](calculus.md#continuity-set-of-a-function)
      - [Right-continuous function](calculus.md#right-continuous-function)
        - [Càdlàg](calculus.md#cadlag)
      - [Uniformly continuous function](calculus.md#uniformly-continuous-function)
        - [Decay of a nonnegative uniformly continuous integrable function](calculus.md#decay-of-a-nonnegative-uniformly-continuous-integrable-function)
    - [Squeeze theorem](calculus.md#squeeze-theorem)
  - [Derivative](calculus.md#derivative)
    - [Symmetric second derivative](calculus.md#symmetric-second-derivative)
    - [Symmetric second differences detect an affine corner](calculus.md#symmetric-second-differences-detect-an-affine-corner)
    - [Symmetric first-order differences remove an affine corner](calculus.md#symmetric-first-order-differences-remove-an-affine-corner)
    - [Vanishing symmetric second derivative forces an affine function](calculus.md#vanishing-symmetric-second-derivative-forces-an-affine-function)
    - [One-sided derivative](calculus.md#one-sided-derivative)
    - [Tangent line](calculus.md#tangent-line)
    - [Automatic differentiation](calculus.md#automatic-differentiation)
    - [Differentiation](calculus.md#differentiation)
    - [Second derivative](calculus.md#second-derivative)
    - [Difference quotient](calculus.md#difference-quotient)
      - [Discrete integration by parts](calculus.md#discrete-integration-by-parts)
    - [Total derivative](calculus.md#total-derivative)
    - [L'Hôpital's rule](calculus.md#l-hopital-s-rule)
      - [Derivative quotient limits on partial domains](calculus.md#derivative-quotient-limits-on-partial-domains)
    - [Darboux's theorem (analysis)](calculus.md#darboux-s-theorem-analysis)
      - [Intermediate secant slope from endpoint derivatives](calculus.md#intermediate-secant-slope-from-endpoint-derivatives)
    - [Product rule](calculus.md#product-rule)
      - [Differentiability restored by a quadratic zero](calculus.md#differentiability-restored-by-a-quadratic-zero)
      - [Leibniz rule](calculus.md#leibniz-rule)
      - [Nondifferentiable factor with a differentiable nondegenerate product](calculus.md#nondifferentiable-factor-with-a-differentiable-nondegenerate-product)
    - [Quotient rule](calculus.md#quotient-rule)
    - [Chain rule](calculus.md#chain-rule)
      - [Nondifferentiable inner function with a differentiable nondegenerate composite](calculus.md#nondifferentiable-inner-function-with-a-differentiable-nondegenerate-composite)
      - [Second derivative chain rule](calculus.md#second-derivative-chain-rule)
  - [Monotonic function](calculus.md#monotonic-function)
    - [Monotone mean-value point of an integral average](calculus.md#monotone-mean-value-point-of-an-integral-average)
    - [Nonincreasing function](calculus.md#nonincreasing-function)
    - [Non-strict inverse of a continuous nondecreasing function](calculus.md#non-strict-inverse-of-a-continuous-nondecreasing-function)
    - [Left-continuous cumulative function of an atomic measure](calculus.md#left-continuous-cumulative-function-of-an-atomic-measure)
    - [Nondecreasing function](calculus.md#nondecreasing-function)
    - [Strict generalized inverse of a nondecreasing function](calculus.md#strict-generalized-inverse-of-a-nondecreasing-function)
    - [Strictly increasing function](calculus.md#strictly-increasing-function)
      - [Continuity of an increasing interval surjection](calculus.md#continuity-of-an-increasing-interval-surjection)
    - [Lebesgue theorem on differentiability of monotone functions](calculus.md#lebesgue-theorem-on-differentiability-of-monotone-functions)
  - [Multivariable calculus](calculus.md#multivariable-calculus)
    - [Volume integral](calculus.md#volume-integral)
    - [Fundamental theorem of calculus along a line segment](calculus.md#fundamental-theorem-of-calculus-along-a-line-segment)
    - [Partial derivative](calculus.md#partial-derivative)
      - [Partial derivatives do not imply continuity](calculus.md#partial-derivatives-do-not-imply-continuity)
      - [Mixed partial derivative](calculus.md#mixed-partial-derivative)
        - [Unequal mixed partial derivatives](calculus.md#unequal-mixed-partial-derivatives)
        - [Symmetry of second derivatives](calculus.md#symmetry-of-second-derivatives)
      - [Time derivative](calculus.md#time-derivative)
      - [Spatial derivative](calculus.md#spatial-derivative)
      - [Directional derivative](calculus.md#directional-derivative)
        - [Directional derivatives do not imply differentiability](calculus.md#directional-derivatives-do-not-imply-differentiability)
        - [Directional derivative of a convex function is sublinear](calculus.md#directional-derivative-of-a-convex-function-is-sublinear)
      - [Gradient](calculus.md#gradient)
        - [Gradient of a dot product](calculus.md#gradient-of-a-dot-product)
        - [Gradient field](calculus.md#gradient-field)
      - [Total differential](calculus.md#total-differential)
    - [Hessian matrix](calculus.md#hessian-matrix)
      - [Quadratic growth from a bounded Hessian](calculus.md#quadratic-growth-from-a-bounded-hessian)
      - [Higher-order test for separated extrema](calculus.md#higher-order-test-for-separated-extrema)
      - [Negative semidefinite matrix](calculus.md#negative-semidefinite-matrix)
      - [Second-derivative test](calculus.md#second-derivative-test)
        - [Critical points escaping to infinity in a Gaussian-weighted bilinear function](calculus.md#critical-points-escaping-to-infinity-in-a-gaussian-weighted-bilinear-function)
      - [Nondegenerate critical point](calculus.md#nondegenerate-critical-point)
    - [Vector calculus](calculus.md#vector-calculus)
      - [Dot-product gradient identity](calculus.md#dot-product-gradient-identity)
      - [Helmholtz decomposition](calculus.md#helmholtz-decomposition)
      - [Divergence of a cross product](calculus.md#divergence-of-a-cross-product)
      - [Vector field](calculus.md#vector-field)
        - [Flow of a vector field](calculus.md#flow-of-a-vector-field)
        - [Time-dependent vector field](calculus.md#time-dependent-vector-field)
          - [Finite-time flow completeness on a compact manifold](calculus.md#finite-time-flow-completeness-on-a-compact-manifold)
        - [Radial dilation tangency to homogeneous zero sets](calculus.md#radial-dilation-tangency-to-homogeneous-zero-sets)
        - [Divergence and curl of a radial vector field](calculus.md#divergence-and-curl-of-a-radial-vector-field)
        - [Azimuthal inverse-radius vector field](calculus.md#azimuthal-inverse-radius-vector-field)
        - [Integral curve of a vector field](calculus.md#integral-curve-of-a-vector-field)
          - [Curvature of an integral curve of a vector field](calculus.md#curvature-of-an-integral-curve-of-a-vector-field)
        - [Axisymmetric vector field](calculus.md#axisymmetric-vector-field)
        - [Solenoidal vector field](calculus.md#solenoidal-vector-field)
          - [Poloidal-toroidal decomposition](calculus.md#poloidal-toroidal-decomposition)
            - [Poloidal magnetic energy bound by the radial scalar gradient](calculus.md#poloidal-magnetic-energy-bound-by-the-radial-scalar-gradient)
      - [Spherically symmetric function](calculus.md#spherically-symmetric-function)
      - [Helicity conservation by tangent boundary conditions](calculus.md#helicity-conservation-by-tangent-boundary-conditions)
      - [Divergence](calculus.md#divergence)
        - [Divergence of a Riemannian vector field](calculus.md#divergence-of-a-riemannian-vector-field)
        - [Cylindrically radial divergence](calculus.md#cylindrically-radial-divergence)
        - [Distributional divergence](calculus.md#distributional-divergence)
        - [Divergence in polar coordinates](calculus.md#divergence-in-polar-coordinates)
        - [Product rule for divergence](calculus.md#product-rule-for-divergence)
        - [Total divergence](calculus.md#total-divergence)
        - [Divergence of a curl is zero](calculus.md#divergence-of-a-curl-is-zero)
      - [Curl](calculus.md#curl)
        - [Curl of a gradient](calculus.md#curl-of-a-gradient)
        - [Irrotational vector field](calculus.md#irrotational-vector-field)
        - [Vector potential](calculus.md#vector-potential)
          - [Radial vector potential of a solenoidal vector field](calculus.md#radial-vector-potential-of-a-solenoidal-vector-field)
        - [Curl of the curl identity](calculus.md#curl-of-the-curl-identity)
      - [Laplacian](calculus.md#laplacian)
        - [Laplacian in polar coordinates](calculus.md#laplacian-in-polar-coordinates)
        - [Product rule for the Laplacian](calculus.md#product-rule-for-the-laplacian)
        - [Biharmonic operator](calculus.md#biharmonic-operator)
          - [Clamped biharmonic problem](calculus.md#clamped-biharmonic-problem)
          - [Biharmonic equation](calculus.md#biharmonic-equation)
            - [Spherical mean of a biharmonic function](calculus.md#spherical-mean-of-a-biharmonic-function)
      - [Divergence and curl of a cross product](calculus.md#divergence-and-curl-of-a-cross-product)
        - [Curl of a cross product](calculus.md#curl-of-a-cross-product)
      - [Levi-Civita symbol](calculus.md#levi-civita-symbol)
        - [Rotation invariance of the Levi-Civita symbol](calculus.md#rotation-invariance-of-the-levi-civita-symbol)
        - [Contraction of two Levi-Civita symbols](calculus.md#contraction-of-two-levi-civita-symbols)
        - [Lagrange identity for the cross product](calculus.md#lagrange-identity-for-the-cross-product)
        - [Triple product](calculus.md#triple-product)
          - [Vector triple product](calculus.md#vector-triple-product)
      - [Feasible inner products with two unit vectors](calculus.md#feasible-inner-products-with-two-unit-vectors)
      - [Conservative vector field](calculus.md#conservative-vector-field)
        - [Integrating-factor equation for a planar vector field](calculus.md#integrating-factor-equation-for-a-planar-vector-field)
        - [Periods obstruct a periodic potential](calculus.md#periods-obstruct-a-periodic-potential)
        - [Potential of a conservative vector field](calculus.md#potential-of-a-conservative-vector-field)
          - [Radial integral potential for a curl-free field](calculus.md#radial-integral-potential-for-a-curl-free-field)
      - [Divergence theorem](calculus.md#divergence-theorem)
        - [Gradient volume-to-boundary identity](calculus.md#gradient-volume-to-boundary-identity)
        - [Vector gradient form of the divergence theorem](calculus.md#vector-gradient-form-of-the-divergence-theorem)
        - [Boundary integral of position and normal components](calculus.md#boundary-integral-of-position-and-normal-components)
        - [An entire bounded vector field cannot have nonzero constant divergence](calculus.md#an-entire-bounded-vector-field-cannot-have-nonzero-constant-divergence)
        - [Riemannian divergence theorem](calculus.md#riemannian-divergence-theorem)
      - [Fundamental theorem for line integrals](calculus.md#fundamental-theorem-for-line-integrals)
        - [Path independence](calculus.md#path-independence)
      - [Stokes theorem](calculus.md#stokes-theorem)
        - [Vector-valued Stokes identity](calculus.md#vector-valued-stokes-identity)
        - [Stokes flux through an annular paraboloid](calculus.md#stokes-flux-through-an-annular-paraboloid)
      - [Surface integral](calculus.md#surface-integral)
        - [Vector surface element of a graph](calculus.md#vector-surface-element-of-a-graph)
        - [Oriented surface element](calculus.md#oriented-surface-element)
        - [Parametrized surface](calculus.md#parametrized-surface)
        - [Surface area of a graph](calculus.md#surface-area-of-a-graph)
        - [Flux integral](calculus.md#flux-integral)
      - [Green theorem](calculus.md#green-theorem)
        - [Boundary formula for planar area](calculus.md#boundary-formula-for-planar-area)
      - [Line integral](calculus.md#line-integral)
      - [Tensor divergence theorem](calculus.md#tensor-divergence-theorem)
        - [Integration by parts for tensor fields](calculus.md#integration-by-parts-for-tensor-fields)
    - [Jacobian matrix and determinant](calculus.md#jacobian-matrix-and-determinant)
      - [Jacobian matrix](calculus.md#jacobian-matrix)
        - [Spatial derivative control in perturbations of the identity map](calculus.md#spatial-derivative-control-in-perturbations-of-the-identity-map)
        - [Jacobian determinant](calculus.md#jacobian-determinant)
          - [Jacobian determinant as a divergence](calculus.md#jacobian-determinant-as-a-divergence)
    - [Change of variables formula](calculus.md#change-of-variables-formula)
      - [Ordered-cone substitution by products and ratios](calculus.md#ordered-cone-substitution-by-products-and-ratios)
      - [Ratio-product coordinates](calculus.md#ratio-product-coordinates)
      - [Squared-radius difference substitution](calculus.md#squared-radius-difference-substitution)
      - [Weighted inverse multiplicity](calculus.md#weighted-inverse-multiplicity)
      - [Rational square diffeomorphism](calculus.md#rational-square-diffeomorphism)
      - [Hyperbolic substitution](calculus.md#hyperbolic-substitution)
      - [Monotone substitution inequality](calculus.md#monotone-substitution-inequality)
      - [Area formula (geometric measure theory)](calculus.md#area-formula-geometric-measure-theory)
      - [Polar coordinates](calculus.md#polar-coordinates)
        - [Cylindrical coordinate system](calculus.md#cylindrical-coordinate-system)
          - [Azimuthal derivative of a cylindrical vector Fourier mode](calculus.md#azimuthal-derivative-of-a-cylindrical-vector-fourier-mode)
          - [Cylindrical radius](calculus.md#cylindrical-radius)
        - [Cardioid](calculus.md#cardioid)
      - [Orthogonal coordinates](calculus.md#orthogonal-coordinates)
        - [Del in cylindrical and spherical coordinates](calculus.md#del-in-cylindrical-and-spherical-coordinates)
        - [Hyperspherical coordinates](calculus.md#hyperspherical-coordinates)
          - [Spherical coordinate system](calculus.md#spherical-coordinate-system)
            - [Radial unit vector in spherical coordinates](calculus.md#radial-unit-vector-in-spherical-coordinates)
            - [Scale factors of orthogonal coordinates](calculus.md#scale-factors-of-orthogonal-coordinates)
            - [Curl in spherical coordinates](calculus.md#curl-in-spherical-coordinates)
          - [Volume of an n-ball](calculus.md#volume-of-an-n-ball)
          - [Surface area of an n-sphere](calculus.md#surface-area-of-an-n-sphere)
    - [Differentiable map](calculus.md#differentiable-map)
      - [Functionally independent functions](calculus.md#functionally-independent-functions)
      - [Derivative of a map into a level set](calculus.md#derivative-of-a-map-into-a-level-set)
      - [Fréchet derivative](calculus.md#frechet-derivative)
        - [Differentiability under equivalent norms](calculus.md#differentiability-under-equivalent-norms)
        - [Hadamard differentiability](calculus.md#hadamard-differentiability)
          - [Hadamard remainder near a compact set](calculus.md#hadamard-remainder-near-a-compact-set)
          - [Stieltjes bilinear functional under a variation constraint](calculus.md#stieltjes-bilinear-functional-under-a-variation-constraint)
        - [Fréchet differentiability](calculus.md#frechet-differentiability)
        - [Derivative of matrix inversion](calculus.md#derivative-of-matrix-inversion)
      - [Continuously differentiable function](calculus.md#continuously-differentiable-function)
      - [Invertible linear map](calculus.md#invertible-linear-map)
      - [Mean value inequality](calculus.md#mean-value-inequality)
        - [Zero derivative on a connected open set](calculus.md#zero-derivative-on-a-connected-open-set)
      - [Inverse function theorem](calculus.md#inverse-function-theorem)
        - [Constant rank theorem](calculus.md#constant-rank-theorem)
          - [Rank-one level curves from a characteristic differential equation](calculus.md#rank-one-level-curves-from-a-characteristic-differential-equation)
        - [Local diffeomorphism](calculus.md#local-diffeomorphism)
          - [Noninjective map with constant Jacobian determinant](calculus.md#noninjective-map-with-constant-jacobian-determinant)
          - [Open map](calculus.md#open-map)
        - [Implicit function theorem](calculus.md#implicit-function-theorem)
          - [Holomorphic implicit function theorem](calculus.md#holomorphic-implicit-function-theorem)
          - [Implicit differentiation](calculus.md#implicit-differentiation)
            - [Cyclic partial derivative identity](calculus.md#cyclic-partial-derivative-identity)
  - [Symmetry in integration](calculus.md#symmetry-in-integration)
  - [Integration by parts](calculus.md#integration-by-parts)
    - [Boundary term](calculus.md#boundary-term)
  - [Hyperbolic tangent](calculus.md#hyperbolic-tangent)
    - [Inverse hyperbolic tangent](calculus.md#inverse-hyperbolic-tangent)
    - [Small-argument expansion of the hyperbolic tangent](calculus.md#small-argument-expansion-of-the-hyperbolic-tangent)
    - [Hyperbolic-function identity](calculus.md#hyperbolic-function-identity)
    - [Hyperbolic Pythagorean identity](calculus.md#hyperbolic-pythagorean-identity)
  - [Even function](calculus.md#even-function)
  - [Odd function](calculus.md#odd-function)
    - [Odd extension](calculus.md#odd-extension)
- [Riemann integration](#riemann-integration)
  - [Single-point changes preserve Riemann integrals](#single-point-changes-preserve-riemann-integrals)
  - [Riemann-Stieltjes integral](#riemann-stieltjes-integral)
  - [Quadrature error](#quadrature-error)
  - [Partition of an interval](#partition-of-an-interval)
    - [Partition refinement](#partition-refinement)
    - [Dyadic partition](#dyadic-partition)
      - [Dyadic interval](#dyadic-interval)
        - [Alternating dyadic colouring excludes symmetric weighted pair sums](#alternating-dyadic-colouring-excludes-symmetric-weighted-pair-sums)
  - [Riemann sum](#riemann-sum)
  - [Continuous approximation of a Riemann-integrable function](#continuous-approximation-of-a-riemann-integrable-function)
  - [Total variation of a function](#total-variation-of-a-function)
    - [p-variation of a path](#p-variation-of-a-path)
    - [Dyadic approximation of total variation](#dyadic-approximation-of-total-variation)
    - [Weak convergence of bounded-variation integrators](#weak-convergence-of-bounded-variation-integrators)
    - [Jordan decomposition of a function of bounded variation](#jordan-decomposition-of-a-function-of-bounded-variation)
  - [Riemann integral](#riemann-integral)
    - [Unbounded derivative obstruction to Riemann integrability](#unbounded-derivative-obstruction-to-riemann-integrability)
    - [Weighted mean value theorem for integrals](#weighted-mean-value-theorem-for-integrals)
    - [Direct Riemann integrability](#direct-riemann-integrability)
    - [Improper integral](#improper-integral)
      - [Logarithmic divergence](#logarithmic-divergence)
      - [Improper power integral](#improper-power-integral)
    - [Monotonicity of the Riemann integral](#monotonicity-of-the-riemann-integral)
  - [Riemann integrability criterion](#riemann-integrability-criterion)
    - [Pointwise supremum need not preserve Riemann integrability](#pointwise-supremum-need-not-preserve-riemann-integrability)
    - [Dirichlet function](#dirichlet-function)
    - [Riemann integrability is closed under addition and maximum](#riemann-integrability-is-closed-under-addition-and-maximum)
    - [Bounded functions continuous away from one endpoint are Riemann integrable](#bounded-functions-continuous-away-from-one-endpoint-are-riemann-integrable)
    - [Indicator of a restricted-digit decimal set](#indicator-of-a-restricted-digit-decimal-set)
    - [Riemann integrability from almost full interval coverage](#riemann-integrability-from-almost-full-interval-coverage)
    - [Lipschitz composition preserves Riemann integrability](#lipschitz-composition-preserves-riemann-integrability)
    - [Uniform-mesh Darboux criterion](#uniform-mesh-darboux-criterion)
      - [Finite bad-cell estimate for Darboux sums](#finite-bad-cell-estimate-for-darboux-sums)
    - [Riemann-integrable function](#riemann-integrable-function)
      - [Dense jumps do not prevent Riemann integrability](#dense-jumps-do-not-prevent-riemann-integrability)
    - [Continuous functions are Riemann integrable](#continuous-functions-are-riemann-integrable)
  - [Darboux sum](#darboux-sum)
    - [Oscillation of a function on an interval](#oscillation-of-a-function-on-an-interval)
    - [Darboux sum refinement monotonicity](#darboux-sum-refinement-monotonicity)
    - [Upper Darboux sum](#upper-darboux-sum)
    - [Lower Darboux sum](#lower-darboux-sum)
      - [Exponential bound for a lower-sum product](#exponential-bound-for-a-lower-sum-product)
    - [Upper and lower Darboux integrals](#upper-and-lower-darboux-integrals)
      - [Lower Darboux integral](#lower-darboux-integral)
      - [Upper Darboux integral](#upper-darboux-integral)
  - [Improper integration by truncation](#improper-integration-by-truncation)
    - [First occurrence of a decimal digit](#first-occurrence-of-a-decimal-digit)
- [Convergent subsequence](#convergent-subsequence)
- [Proper extended-real function](#proper-extended-real-function)
  - [Effective domain](#effective-domain)
- [Convex function](#convex-function)
  - [Finite convex function as supremum of affine minorants](#finite-convex-function-as-supremum-of-affine-minorants)
  - [Essential smoothness of a convex function](#essential-smoothness-of-a-convex-function)
  - [Convex quadratic function](#convex-quadratic-function)
  - [Bounded convex functions are locally Lipschitz on an open ball](#bounded-convex-functions-are-locally-lipschitz-on-an-open-ball)
  - [Negative part of a finite convex function is Lipschitz](#negative-part-of-a-finite-convex-function-is-lipschitz)
  - [Affine minorant](#affine-minorant)
  - [Proper convex function](#proper-convex-function)
  - [Operator convex function](#operator-convex-function)
    - [Operator concave function](#operator-concave-function)
  - [Continuity of a convex function](#continuity-of-a-convex-function)
  - [Pointwise maximum of convex functions](#pointwise-maximum-of-convex-functions)
  - [Softplus](#softplus)
  - [Absolute value](#absolute-value)
    - [Absolute value at a simple zero](#absolute-value-at-a-simple-zero)
    - [Summable absolute-value cusp series](#summable-absolute-value-cusp-series)
  - [Strongly convex function](#strongly-convex-function)
    - [Uniformly convex variational integrand](#uniformly-convex-variational-integrand)
      - [Interior gradient regularity for uniformly convex autonomous energies](#interior-gradient-regularity-for-uniformly-convex-autonomous-energies)
      - [Uniqueness for uniformly convex gradient Dirichlet problems](#uniqueness-for-uniformly-convex-gradient-dirichlet-problems)
  - [Strictly convex function](#strictly-convex-function)
    - [Uniqueness of a minimizer of a strictly convex function](#uniqueness-of-a-minimizer-of-a-strictly-convex-function)
  - [Convexity domain of x cubed plus y cubed plus Axy](#convexity-domain-of-x-cubed-plus-y-cubed-plus-axy)
  - [Perspective function](#perspective-function)
  - [Subgradient](#subgradient)
    - [Continuous supporting functional for a locally bounded convex function](#continuous-supporting-functional-for-a-locally-bounded-convex-function)
    - [Subgradient optimality condition](#subgradient-optimality-condition)
    - [Subgradient of the absolute value](#subgradient-of-the-absolute-value)
    - [Subgradient inequality](#subgradient-inequality)
  - [Jensen's inequality](#jensen-s-inequality)
    - [Sharp two-term convex power bound](#sharp-two-term-convex-power-bound)
- [Concave function](#concave-function)
  - [Extrema of a concave power sum on a simplex](#extrema-of-a-concave-power-sum-on-a-simplex)
  - [Strictly increasing concave function](#strictly-increasing-concave-function)
  - [Concave supporting-tangent inequality](#concave-supporting-tangent-inequality)
  - [Concave majorant](#concave-majorant)
  - [Strictly concave function](#strictly-concave-function)
    - [Strict concavity](#strict-concavity)
      - [Positive-product maximization on a convex set](#positive-product-maximization-on-a-convex-set)
    - [Uniform negative curvature and global maximization](#uniform-negative-curvature-and-global-maximization)
    - [Product maximizer on a compact convex subset of the positive orthant](#product-maximizer-on-a-compact-convex-subset-of-the-positive-orthant)
- [Measure theory](measure-theory.md)
  - [Wiener covering lemma](measure-theory.md#wiener-covering-lemma)
    - [Disjoint ball decomposition modulo null sets](measure-theory.md#disjoint-ball-decomposition-modulo-null-sets)
  - [Geometric measure theory](measure-theory.md#geometric-measure-theory)
  - [Vector measure](measure-theory.md#vector-measure)
    - [Vector Radon measure](measure-theory.md#vector-radon-measure)
      - [Polar decomposition of a vector measure](measure-theory.md#polar-decomposition-of-a-vector-measure)
  - [Standard Borel probability space](measure-theory.md#standard-borel-probability-space)
  - [Measurable space](measure-theory.md#measurable-space)
    - [Standard Borel space](measure-theory.md#standard-borel-space)
  - [Hausdorff measure](measure-theory.md#hausdorff-measure)
    - [Scale-restricted Hausdorff content](measure-theory.md#scale-restricted-hausdorff-content)
    - [Hausdorff dimension](measure-theory.md#hausdorff-dimension)
      - [Pressure upper bound for Hausdorff dimension](measure-theory.md#pressure-upper-bound-for-hausdorff-dimension)
      - [Hausdorff dimension of a connected set](measure-theory.md#hausdorff-dimension-of-a-connected-set)
  - [Null set](measure-theory.md#null-set)
    - [Borel null set](measure-theory.md#borel-null-set)
  - [Random measure](measure-theory.md#random-measure)
  - [Measurable partition](measure-theory.md#measurable-partition)
    - [Partition atom](measure-theory.md#partition-atom)
    - [Entropy of a countable measurable partition](measure-theory.md#entropy-of-a-countable-measurable-partition)
      - [Conditional information function](measure-theory.md#conditional-information-function)
        - [Maximal inequality for conditional information functions](measure-theory.md#maximal-inequality-for-conditional-information-functions)
        - [Conditional entropy of a countable measurable partition](measure-theory.md#conditional-entropy-of-a-countable-measurable-partition)
    - [Join of measurable partitions](measure-theory.md#join-of-measurable-partitions)
  - [Field of sets](measure-theory.md#field-of-sets)
  - [Semiring of sets](measure-theory.md#semiring-of-sets)
  - [Monotone class](measure-theory.md#monotone-class)
    - [Monotone class theorem](measure-theory.md#monotone-class-theorem)
      - [Functional monotone-class theorem](measure-theory.md#functional-monotone-class-theorem)
  - [Measurable function](measure-theory.md#measurable-function)
    - [Essential range](measure-theory.md#essential-range)
    - [Measurability](measure-theory.md#measurability)
    - [Borel measurable function](measure-theory.md#borel-measurable-function)
    - [Composition of measurable functions](measure-theory.md#composition-of-measurable-functions)
  - [Measure density](measure-theory.md#measure-density)
    - [Spherical derivative of a measure](measure-theory.md#spherical-derivative-of-a-measure)
      - [Spherical derivative of a singular measure vanishes](measure-theory.md#spherical-derivative-of-a-singular-measure-vanishes)
    - [Lebesgue differentiation theorem](measure-theory.md#lebesgue-differentiation-theorem)
      - [Oscillating annuli obstruct differentiation at a point](measure-theory.md#oscillating-annuli-obstruct-differentiation-at-a-point)
      - [Lebesgue point](measure-theory.md#lebesgue-point)
      - [Differentiation of an indefinite Lebesgue integral](measure-theory.md#differentiation-of-an-indefinite-lebesgue-integral)
    - [Lebesgue's density theorem](measure-theory.md#lebesgue-s-density-theorem)
      - [Density point](measure-theory.md#density-point)
      - [High-density interval in a positive-measure subset of the real line](measure-theory.md#high-density-interval-in-a-positive-measure-subset-of-the-real-line)
  - [Lebesgue measurable set](measure-theory.md#lebesgue-measurable-set)
    - [Regularity of Lebesgue measure](measure-theory.md#regularity-of-lebesgue-measure)
  - [Almost everywhere](measure-theory.md#almost-everywhere)
  - [Lebesgue integrable function](measure-theory.md#lebesgue-integrable-function)
    - [Integrability](measure-theory.md#integrability)
  - [Conditional expectation](measure-theory.md#conditional-expectation)
    - [Conditional expectation preserving a distribution](measure-theory.md#conditional-expectation-preserving-a-distribution)
    - [Dyadic conditional averages recover integrable functions](measure-theory.md#dyadic-conditional-averages-recover-integrable-functions)
    - [Symmetrization as conditional expectation](measure-theory.md#symmetrization-as-conditional-expectation)
      - [Sampling with and without replacement comparison for bounded products](measure-theory.md#sampling-with-and-without-replacement-comparison-for-bounded-products)
    - [Conditional expectation from finite-measure densities](measure-theory.md#conditional-expectation-from-finite-measure-densities)
    - [Equality case for conditional second moments](measure-theory.md#equality-case-for-conditional-second-moments)
    - [Conditional L2 norm](measure-theory.md#conditional-l2-norm)
      - [Conditional norm covariance under a factor map](measure-theory.md#conditional-norm-covariance-under-a-factor-map)
      - [Uniform conditional L2 norm](measure-theory.md#uniform-conditional-l2-norm)
    - [Conditional Jensen inequality](measure-theory.md#conditional-jensen-inequality)
    - [L1 contraction of conditional expectation](measure-theory.md#l1-contraction-of-conditional-expectation)
    - [Conditional expectation of a summand given future partial sums](measure-theory.md#conditional-expectation-of-a-summand-given-future-partial-sums)
    - [Law of total expectation](measure-theory.md#law-of-total-expectation)
    - [Independent sigma-algebras have trivial intersection](measure-theory.md#independent-sigma-algebras-have-trivial-intersection)
    - [Iterated conditional expectation over nonnested sigma-algebras](measure-theory.md#iterated-conditional-expectation-over-nonnested-sigma-algebras)
    - [Conditional Fatou lemma](measure-theory.md#conditional-fatou-lemma)
  - [Fatou's lemma](measure-theory.md#fatou-s-lemma)
    - [Fatou lemma for series](measure-theory.md#fatou-lemma-for-series)
    - [Proof of Fatou lemma](measure-theory.md#proof-of-fatou-lemma)
    - [Strict inequality in Fatou lemma](measure-theory.md#strict-inequality-in-fatou-lemma)
  - [Ergodic theory](measure-theory.md#ergodic-theory)
    - [Generic point for an invariant measure](measure-theory.md#generic-point-for-an-invariant-measure)
    - [Invariant measure](measure-theory.md#invariant-measure)
      - [Invariant probability measure for a semigroup](measure-theory.md#invariant-probability-measure-for-a-semigroup)
        - [Krylov–Bogolyubov theorem](measure-theory.md#krylov-bogolyubov-theorem)
    - [Cutting and stacking](measure-theory.md#cutting-and-stacking)
      - [Chacon transformation](measure-theory.md#chacon-transformation)
    - [Unique ergodicity](measure-theory.md#unique-ergodicity)
      - [Uniform ergodic convergence for uniquely ergodic systems](measure-theory.md#uniform-ergodic-convergence-for-uniquely-ergodic-systems)
    - [Van der Corput lemma (Hilbert space sequences)](measure-theory.md#van-der-corput-lemma-hilbert-space-sequences)
      - [Van der Corput inequality for finite scalar sequences](measure-theory.md#van-der-corput-inequality-for-finite-scalar-sequences)
    - [Equidistributed sequence](measure-theory.md#equidistributed-sequence)
      - [Equidistribution criterion for a torus translation](measure-theory.md#equidistribution-criterion-for-a-torus-translation)
      - [Interval discrepancy](measure-theory.md#interval-discrepancy)
      - [Weyl criterion](measure-theory.md#weyl-criterion)
        - [Differencing obstruction to equidistribution](measure-theory.md#differencing-obstruction-to-equidistribution)
        - [Equidistribution of a quadratic polynomial with irrational leading coefficient](measure-theory.md#equidistribution-of-a-quadratic-polynomial-with-irrational-leading-coefficient)
          - [Uniform square recurrence on the circle](measure-theory.md#uniform-square-recurrence-on-the-circle)
    - [Nonsingular transformation](measure-theory.md#nonsingular-transformation)
    - [Koopman operator](measure-theory.md#koopman-operator)
      - [Spectral measure of a Koopman observable](measure-theory.md#spectral-measure-of-a-koopman-observable)
      - [Almost periodic observable](measure-theory.md#almost-periodic-observable)
        - [Syndetic near returns of an almost periodic observable](measure-theory.md#syndetic-near-returns-of-an-almost-periodic-observable)
        - [Compact measure-preserving system](measure-theory.md#compact-measure-preserving-system)
      - [Decay of autocorrelation implies weak convergence of an observable](measure-theory.md#decay-of-autocorrelation-implies-weak-convergence-of-an-observable)
      - [Bounded Koopman operator criterion](measure-theory.md#bounded-koopman-operator-criterion)
    - [Measure-preserving transformation](measure-theory.md#measure-preserving-transformation)
      - [Lebesgue-measure-preserving map](measure-theory.md#lebesgue-measure-preserving-map)
      - [Integer multiplication map on the circle](measure-theory.md#integer-multiplication-map-on-the-circle)
        - [Ergodicity of integer multiplication on the circle](measure-theory.md#ergodicity-of-integer-multiplication-on-the-circle)
      - [Measure-preserving system](measure-theory.md#measure-preserving-system)
        - [Factor of a measure-preserving system](measure-theory.md#factor-of-a-measure-preserving-system)
          - [Factor map between measure-preserving systems](measure-theory.md#factor-map-between-measure-preserving-systems)
            - [Compact extension of a measure-preserving system](measure-theory.md#compact-extension-of-a-measure-preserving-system)
              - [Finite-fiber compact extension](measure-theory.md#finite-fiber-compact-extension)
              - [Positive-measure almost periodic indicator in a compact extension](measure-theory.md#positive-measure-almost-periodic-indicator-in-a-compact-extension)
            - [Relatively almost periodic observable](measure-theory.md#relatively-almost-periodic-observable)
              - [Localization of relative almost periodicity to base sets](measure-theory.md#localization-of-relative-almost-periodicity-to-base-sets)
      - [Finite full-support measure-preserving map is bijective](measure-theory.md#finite-full-support-measure-preserving-map-is-bijective)
      - [Invertible measure-preserving system](measure-theory.md#invertible-measure-preserving-system)
      - [Invariant sigma-algebra](measure-theory.md#invariant-sigma-algebra)
        - [Invariant set of a measure-preserving transformation](measure-theory.md#invariant-set-of-a-measure-preserving-transformation)
      - [Ergodicity](measure-theory.md#ergodicity)
        - [Strong mixing](measure-theory.md#strong-mixing)
          - [Diagonal set-correlation criterion for mixing](measure-theory.md#diagonal-set-correlation-criterion-for-mixing)
        - [Ergodic decomposition](measure-theory.md#ergodic-decomposition)
          - [Ergodic components of a rational circle rotation](measure-theory.md#ergodic-components-of-a-rational-circle-rotation)
          - [Ergodic component](measure-theory.md#ergodic-component)
            - [Countable-test proof of ergodicity of conditional components](measure-theory.md#countable-test-proof-of-ergodicity-of-conditional-components)
          - [Affinity of entropy under ergodic decomposition](measure-theory.md#affinity-of-entropy-under-ergodic-decomposition)
        - [Ergodic invariant probability on a countable state space has finite cyclic support](measure-theory.md#ergodic-invariant-probability-on-a-countable-state-space-has-finite-cyclic-support)
        - [Invariant-function characterization of ergodicity](measure-theory.md#invariant-function-characterization-of-ergodicity)
        - [Bernoulli shift](measure-theory.md#bernoulli-shift)
          - [Bernoulli coordinate observable is not almost periodic](measure-theory.md#bernoulli-coordinate-observable-is-not-almost-periodic)
          - [Cantor Bernoulli measure](measure-theory.md#cantor-bernoulli-measure)
        - [Irrational rotation](measure-theory.md#irrational-rotation)
          - [Ergodicity criterion for a circle rotation](measure-theory.md#ergodicity-criterion-for-a-circle-rotation)
          - [Everywhere interval frequency under an irrational rotation](measure-theory.md#everywhere-interval-frequency-under-an-irrational-rotation)
        - [Weakly mixing measure-preserving transformation](measure-theory.md#weakly-mixing-measure-preserving-transformation)
          - [Arithmetic-progression multiple averages under weak mixing](measure-theory.md#arithmetic-progression-multiple-averages-under-weak-mixing)
            - [Density convergence of multiple weak-mixing correlations](measure-theory.md#density-convergence-of-multiple-weak-mixing-correlations)
          - [Stability of weak mixing under powers and products](measure-theory.md#stability-of-weak-mixing-under-powers-and-products)
          - [Product characterization of weak mixing](measure-theory.md#product-characterization-of-weak-mixing)
            - [Square-correlation proof of weak mixing from product ergodicity](measure-theory.md#square-correlation-proof-of-weak-mixing-from-product-ergodicity)
          - [Koopman eigenfunction obstruction to weak mixing](measure-theory.md#koopman-eigenfunction-obstruction-to-weak-mixing)
          - [Simultaneous hitting characterization of weak mixing](measure-theory.md#simultaneous-hitting-characterization-of-weak-mixing)
      - [Poincaré recurrence theorem](measure-theory.md#poincare-recurrence-theorem)
        - [Furstenberg multiple recurrence theorem](measure-theory.md#furstenberg-multiple-recurrence-theorem)
          - [SZ property](measure-theory.md#sz-property)
          - [Multiple recurrence for circle rotations](measure-theory.md#multiple-recurrence-for-circle-rotations)
    - [Birkhoff ergodic theorem](measure-theory.md#birkhoff-ergodic-theorem)
      - [Nonnegative ergodic averages with infinite integral](measure-theory.md#nonnegative-ergodic-averages-with-infinite-integral)
      - [Maximal ergodic lemma](measure-theory.md#maximal-ergodic-lemma)
      - [Triangular ergodic averaging lemma](measure-theory.md#triangular-ergodic-averaging-lemma)
      - [Linear growth bound for integrable observables](measure-theory.md#linear-growth-bound-for-integrable-observables)
        - [Sharpness of the linear growth bound for integrable observables](measure-theory.md#sharpness-of-the-linear-growth-bound-for-integrable-observables)
      - [L1 convergence in the Birkhoff ergodic theorem on a finite measure space](measure-theory.md#l1-convergence-in-the-birkhoff-ergodic-theorem-on-a-finite-measure-space)
    - [Upper Banach density](measure-theory.md#upper-banach-density)
      - [Furstenberg correspondence principle](measure-theory.md#furstenberg-correspondence-principle)
    - [Convergence in density of a sequence](measure-theory.md#convergence-in-density-of-a-sequence)
      - [Mean-square criterion for convergence in density](measure-theory.md#mean-square-criterion-for-convergence-in-density)
      - [Cesaro convergence of a sequence](measure-theory.md#cesaro-convergence-of-a-sequence)
    - [Entropy of a finite measurable partition](measure-theory.md#entropy-of-a-finite-measurable-partition)
      - [Conditional entropy of finite measurable partitions](measure-theory.md#conditional-entropy-of-finite-measurable-partitions)
      - [Entropy rate of a measurable partition](measure-theory.md#entropy-rate-of-a-measurable-partition)
        - [Infinite-future formula for partition entropy rate](measure-theory.md#infinite-future-formula-for-partition-entropy-rate)
          - [Block conditional entropy given the infinite future](measure-theory.md#block-conditional-entropy-given-the-infinite-future)
        - [Shannon-McMillan-Breiman theorem](measure-theory.md#shannon-mcmillan-breiman-theorem)
        - [Monotonicity of normalized block entropy](measure-theory.md#monotonicity-of-normalized-block-entropy)
        - [Kolmogorov-Sinai entropy](measure-theory.md#kolmogorov-sinai-entropy)
          - [Completely positive entropy](measure-theory.md#completely-positive-entropy)
          - [Generating measurable partition](measure-theory.md#generating-measurable-partition)
            - [One-sided generator](measure-theory.md#one-sided-generator)
              - [Finite one-sided generator of an invertible system forces zero entropy](measure-theory.md#finite-one-sided-generator-of-an-invertible-system-forces-zero-entropy)
            - [Kolmogorov-Sinai generator theorem](measure-theory.md#kolmogorov-sinai-generator-theorem)
          - [Host equidistribution theorem](measure-theory.md#host-equidistribution-theorem)
            - [Rudolph measure rigidity theorem](measure-theory.md#rudolph-measure-rigidity-theorem)
          - [Entropy preservation under a finite-to-one factor](measure-theory.md#entropy-preservation-under-a-finite-to-one-factor)
          - [Pinsker sigma-algebra](measure-theory.md#pinsker-sigma-algebra)
            - [Tail characterization of the Pinsker sigma-algebra](measure-theory.md#tail-characterization-of-the-pinsker-sigma-algebra)
        - [Infimum rule for partition entropy rate](measure-theory.md#infimum-rule-for-partition-entropy-rate)
    - [K-mixing](measure-theory.md#k-mixing)
      - [Tail sigma-algebra of a measurable partition](measure-theory.md#tail-sigma-algebra-of-a-measurable-partition)
        - [Finite partitions measurable in a partition tail have zero entropy rate](measure-theory.md#finite-partitions-measurable-in-a-partition-tail-have-zero-entropy-rate)
  - [Outer measure](measure-theory.md#outer-measure)
    - [Carathéodory's criterion](measure-theory.md#caratheodory-s-criterion)
    - [Lebesgue outer measure](measure-theory.md#lebesgue-outer-measure)
  - [Measure](measure-theory.md#measure)
    - [Inner regular measure](measure-theory.md#inner-regular-measure)
    - [p-adic measure](measure-theory.md#p-adic-measure)
      - [Mahler expansion of continuous p-adic functions](measure-theory.md#mahler-expansion-of-continuous-p-adic-functions)
      - [Amice transform](measure-theory.md#amice-transform)
      - [Convolution of p-adic measures](measure-theory.md#convolution-of-p-adic-measures)
    - [Stieltjes transform of a measure](measure-theory.md#stieltjes-transform-of-a-measure)
    - [Outer regular measure](measure-theory.md#outer-regular-measure)
    - [Complex measure](measure-theory.md#complex-measure)
    - [Countable subadditivity of a measure](measure-theory.md#countable-subadditivity-of-a-measure)
    - [Complete measure](measure-theory.md#complete-measure)
      - [Completion of a measure](measure-theory.md#completion-of-a-measure)
    - [Variation measure](measure-theory.md#variation-measure)
      - [Total variation norm of a measure](measure-theory.md#total-variation-norm-of-a-measure)
    - [Signed measure](measure-theory.md#signed-measure)
    - [Dirac measure](measure-theory.md#dirac-measure)
    - [Atom (measure theory)](measure-theory.md#atom-measure-theory)
      - [Non-atomic measure](measure-theory.md#non-atomic-measure)
        - [Lyapunov convexity theorem](measure-theory.md#lyapunov-convexity-theorem)
    - [Counting measure](measure-theory.md#counting-measure)
      - [Series as a Lebesgue integral against counting measure](measure-theory.md#series-as-a-lebesgue-integral-against-counting-measure)
    - [Premeasure](measure-theory.md#premeasure)
      - [Cylinder premeasure from a positive functional](measure-theory.md#cylinder-premeasure-from-a-positive-functional)
      - [Carathéodory's extension theorem](measure-theory.md#caratheodory-s-extension-theorem)
    - [Positive measure](measure-theory.md#positive-measure)
    - [Borel measure](measure-theory.md#borel-measure)
      - [Support of a measure](measure-theory.md#support-of-a-measure)
        - [Support under a continuous map](measure-theory.md#support-under-a-continuous-map)
      - [Borel probability measure](measure-theory.md#borel-probability-measure)
        - [Continuous approximation of Borel indicators on a compact metric space](measure-theory.md#continuous-approximation-of-borel-indicators-on-a-compact-metric-space)
      - [Regular Borel measure](measure-theory.md#regular-borel-measure)
      - [Radon measure](measure-theory.md#radon-measure)
        - [Regularity of finite Borel measures on Euclidean space](measure-theory.md#regularity-of-finite-borel-measures-on-euclidean-space)
    - [Measure space](measure-theory.md#measure-space)
    - [Pushforward measure](measure-theory.md#pushforward-measure)
      - [Probability pushforward embedding theorem](measure-theory.md#probability-pushforward-embedding-theorem)
    - [Change of measure](measure-theory.md#change-of-measure)
      - [Density process](measure-theory.md#density-process)
    - [Haar measure](measure-theory.md#haar-measure)
      - [Haar measure from a left-invariant coframe](measure-theory.md#haar-measure-from-a-left-invariant-coframe)
      - [Haar measure from normalized covering functionals](measure-theory.md#haar-measure-from-normalized-covering-functionals)
      - [Compact-group invariant probability by finite averaging](measure-theory.md#compact-group-invariant-probability-by-finite-averaging)
      - [Haar integral](measure-theory.md#haar-integral)
      - [Weyl integration formula for SU(2)](measure-theory.md#weyl-integration-formula-for-su-2)
      - [Pauli-coordinate Haar measure on SU(2)](measure-theory.md#pauli-coordinate-haar-measure-on-su-2)
      - [Minimal left covering net of a compact group](measure-theory.md#minimal-left-covering-net-of-a-compact-group)
        - [Matching minimal covering nets of a compact group](measure-theory.md#matching-minimal-covering-nets-of-a-compact-group)
    - [Countable additivity](measure-theory.md#countable-additivity)
      - [Continuity from below of a measure](measure-theory.md#continuity-from-below-of-a-measure)
      - [Continuity from above of a measure](measure-theory.md#continuity-from-above-of-a-measure)
    - [Finite measure](measure-theory.md#finite-measure)
      - [Finite-measure set](measure-theory.md#finite-measure-set)
    - [Sigma-finite measure](measure-theory.md#sigma-finite-measure)
  - [Step function](measure-theory.md#step-function)
  - [Lebesgue integral](measure-theory.md#lebesgue-integral)
    - [Integral average](measure-theory.md#integral-average)
      - [Volume average](measure-theory.md#volume-average)
    - [Simple function](measure-theory.md#simple-function)
  - [Indicator function](measure-theory.md#indicator-function)
    - [Indicator vector](measure-theory.md#indicator-vector)
  - [Sigma-algebra](measure-theory.md#sigma-algebra)
    - [Algebra of sets](measure-theory.md#algebra-of-sets)
      - [Countable generating algebra](measure-theory.md#countable-generating-algebra)
    - [Measurable set](measure-theory.md#measurable-set)
    - [Atom of a sigma-algebra](measure-theory.md#atom-of-a-sigma-algebra)
    - [Borel set](measure-theory.md#borel-set)
      - [Borel hierarchy](measure-theory.md#borel-hierarchy)
      - [Borel sigma-algebra](measure-theory.md#borel-sigma-algebra)
        - [Borel sigma-algebra of a discrete space](measure-theory.md#borel-sigma-algebra-of-a-discrete-space)
    - [Pi-system](measure-theory.md#pi-system)
    - [Dynkin system](measure-theory.md#dynkin-system)
      - [Dynkin lemma](measure-theory.md#dynkin-lemma)
  - [Fubini's theorem](measure-theory.md#fubini-s-theorem)
    - [Frullani integral](measure-theory.md#frullani-integral)
  - [Sigma-finite uniqueness theorem for measures](measure-theory.md#sigma-finite-uniqueness-theorem-for-measures)
    - [Lebesgue measure](measure-theory.md#lebesgue-measure)
      - [Null-set limsup cover by finite arc families](measure-theory.md#null-set-limsup-cover-by-finite-arc-families)
      - [Compact batching of a small open set](measure-theory.md#compact-batching-of-a-small-open-set)
      - [Inner regularity of Lebesgue measure](measure-theory.md#inner-regularity-of-lebesgue-measure)
      - [Sierpiński set](measure-theory.md#sierpinski-set)
      - [Divisibility of Lebesgue measure](measure-theory.md#divisibility-of-lebesgue-measure)
      - [Completeness of Lebesgue measure](measure-theory.md#completeness-of-lebesgue-measure)
  - [Bochner integral](measure-theory.md#bochner-integral)
    - [Mean-square integral](measure-theory.md#mean-square-integral)
    - [Barycenter of a measure on a Banach space](measure-theory.md#barycenter-of-a-measure-on-a-banach-space)
    - [Strongly measurable function](measure-theory.md#strongly-measurable-function)
  - [Lp space](measure-theory.md#lp-space)
    - [L1 space](measure-theory.md#l1-space)
    - [Sum of Lp spaces](measure-theory.md#sum-of-lp-spaces)
      - [Threshold decomposition between Lp spaces](measure-theory.md#threshold-decomposition-between-lp-spaces)
    - [Sine sequence is not Cauchy in the integral norm](measure-theory.md#sine-sequence-is-not-cauchy-in-the-integral-norm)
    - [Translation continuity in Lp on a locally compact group](measure-theory.md#translation-continuity-in-lp-on-a-locally-compact-group)
    - [Derivative of a power of the Lp norm](measure-theory.md#derivative-of-a-power-of-the-lp-norm)
    - [Closest point theorem for a closed convex subset of Lp](measure-theory.md#closest-point-theorem-for-a-closed-convex-subset-of-lp)
    - [Completeness of Lp spaces](measure-theory.md#completeness-of-lp-spaces)
    - [Weak Lq space](measure-theory.md#weak-lq-space)
      - [Integral norm for weak Lq](measure-theory.md#integral-norm-for-weak-lq)
    - [Mixed Lebesgue norm](measure-theory.md#mixed-lebesgue-norm)
    - [Locally square-integrable function](measure-theory.md#locally-square-integrable-function)
    - [Translation continuity in Lp](measure-theory.md#translation-continuity-in-lp)
    - [Translation continuity in L1 on the circle](measure-theory.md#translation-continuity-in-l1-on-the-circle)
    - [Lp norms converge to the supremum norm](measure-theory.md#lp-norms-converge-to-the-supremum-norm)
      - [Moment ratios converge to the essential supremum](measure-theory.md#moment-ratios-converge-to-the-essential-supremum)
    - [Lp interpolation inequality](measure-theory.md#lp-interpolation-inequality)
      - [Nonvanishing level-set bound between three Lp norms](measure-theory.md#nonvanishing-level-set-bound-between-three-lp-norms)
    - [Square-integrable function](measure-theory.md#square-integrable-function)
    - [L2 space is a Hilbert space](measure-theory.md#l2-space-is-a-hilbert-space)
      - [Exponentially weighted L2 space](measure-theory.md#exponentially-weighted-l2-space)
        - [Weighted essential spectrum of a Fisher travelling front](measure-theory.md#weighted-essential-spectrum-of-a-fisher-travelling-front)
      - [Mean-zero L2 space](measure-theory.md#mean-zero-l2-space)
      - [L2 inner product](measure-theory.md#l2-inner-product)
    - [Riesz-Fischer theorem](measure-theory.md#riesz-fischer-theorem)
    - [Banach intersection of L1 and L2](measure-theory.md#banach-intersection-of-l1-and-l2)
  - [Approximation by nonnegative simple functions](measure-theory.md#approximation-by-nonnegative-simple-functions)
  - [Monotone convergence theorem](measure-theory.md#monotone-convergence-theorem)
    - [Moving-spike obstruction to interchanging a limit and an infinite sum](measure-theory.md#moving-spike-obstruction-to-interchanging-a-limit-and-an-infinite-sum)
  - [Dominated convergence theorem](measure-theory.md#dominated-convergence-theorem)
  - [Bounded convergence theorem](measure-theory.md#bounded-convergence-theorem)
  - [Tonelli theorem](measure-theory.md#tonelli-theorem)
  - [Mutually singular measures](measure-theory.md#mutually-singular-measures)
    - [Density level sets separate a singular measure](measure-theory.md#density-level-sets-separate-a-singular-measure)
  - [Absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures)
    - [Dominating measure](measure-theory.md#dominating-measure)
    - [Lusin condition N](measure-theory.md#lusin-condition-n)
    - [Image-length measure of a strictly increasing continuous function](measure-theory.md#image-length-measure-of-a-strictly-increasing-continuous-function)
    - [Uniform absolute continuity for a finite measure](measure-theory.md#uniform-absolute-continuity-for-a-finite-measure)
    - [Mutually absolutely continuous measures](measure-theory.md#mutually-absolutely-continuous-measures)
      - [Equivalent probability measure](measure-theory.md#equivalent-probability-measure)
    - [Radon-Nikodym theorem](measure-theory.md#radon-nikodym-theorem)
      - [Hilbert-space construction of dominated measure densities](measure-theory.md#hilbert-space-construction-of-dominated-measure-densities)
      - [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative)
        - [Radon-Nikodym density martingale](measure-theory.md#radon-nikodym-density-martingale)
      - [Positive Radon-Nikodym derivative](measure-theory.md#positive-radon-nikodym-derivative)
    - [Lebesgue decomposition theorem](measure-theory.md#lebesgue-decomposition-theorem)
      - [Dyadic density martingale](measure-theory.md#dyadic-density-martingale)
        - [Martingale construction of Lebesgue decomposition](measure-theory.md#martingale-construction-of-lebesgue-decomposition)
      - [Lebesgue decomposition from a sum-measure density](measure-theory.md#lebesgue-decomposition-from-a-sum-measure-density)
    - [Dominating mixture measure](measure-theory.md#dominating-mixture-measure)
  - [Lebesgue-Stieltjes measure](measure-theory.md#lebesgue-stieltjes-measure)
    - [Lebesgue–Stieltjes integration](measure-theory.md#lebesgue-stieltjes-integration)
  - [Lp inclusion on a finite measure space](measure-theory.md#lp-inclusion-on-a-finite-measure-space)
    - [Almost-everywhere convergent subsequence from Lp convergence](measure-theory.md#almost-everywhere-convergent-subsequence-from-lp-convergence)
    - [Lq inclusion implies finite measure on a Euclidean Borel subset](measure-theory.md#lq-inclusion-implies-finite-measure-on-a-euclidean-borel-subset)
    - [Essential supremum](measure-theory.md#essential-supremum)
    - [Power singularity integrability](measure-theory.md#power-singularity-integrability)

<h2 id="hardy-s-inequality">Hardy's inequality</h2>

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hardy's_inequality)

[Hardy's inequality](#hardy-s-inequality) bounds averages or weighted functions by their original size or [derivatives](calculus.md#derivative). For $p>1$ and $f\geq0$, its integral form is $\int_0^\infty(x^{-1}\int_0^xf(t)\,dt)^p\,dx\leq(p/(p-1))^p\int_0^\infty f(x)^p\,dx$. Spatial weighted forms include the [Hardy inequality in Euclidean space](sobolev-space.md#hardy-inequality-in-euclidean-space).

## Infimum and supremum

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infimum_and_supremum)

The [infimum](#infimum) of a subset of an ordered set is its greatest lower bound; its [supremum](#supremum) is its least upper bound. Neither bound must belong to the subset. For bounded nonempty subsets of the real numbers both bounds exist by [completeness of the real numbers](#completeness-of-the-real-numbers).

### Essential infimum and essential supremum

↑ **Parent:** [Infimum and supremum](#infimum-and-supremum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Essential_infimum_and_essential_supremum)

The essential bounds disregard [null sets](measure-theory.md#null-set). For a real [measurable function](measure-theory.md#measurable-function) $f$, its [essential supremum](measure-theory.md#essential-supremum) is $\inf\{a:f\leq a\text{ almost everywhere}\}$ and its [essential infimum](#essential-infimum) is $\sup\{a:f\geq a\text{ almost everywhere}\}$. Unlike pointwise [infimum](#infimum) and [supremum](#supremum), these values are unchanged by changing $f$ on a [null set](measure-theory.md#null-set).

#### Essential infimum

↑ **Parent:** [Essential infimum and essential supremum](#essential-infimum-and-essential-supremum)

The [essential infimum](#essential-infimum) of a [measurable function](measure-theory.md#measurable-function) is $\operatorname{ess\,inf}u=-\operatorname{ess\,sup}(-u)$. It is the largest lower bound that holds [almost everywhere](measure-theory.md#almost-everywhere). Unlike a pointwise [infimum](#infimum), it is unchanged by altering a representative on a [null set](measure-theory.md#null-set).

### Supremum

↑ **Parent:** [Infimum and supremum](#infimum-and-supremum)

The supremum of a set of real numbers is its least upper bound.

#### Accumulation below an unattained supremum

↑ **Parent:** [Supremum](#supremum)

If a nonempty real set $A$ has finite [supremum](#supremum) $s$ and $s\notin A$, then every interval $(s-\varepsilon,s)$ contains infinitely many elements of $A$. Otherwise its finitely many elements have a largest value $m<s$; all remaining elements are at most $s-\varepsilon$, making $\max(m,s-\varepsilon)<s$ an [upper bound](set.md#upper-bound-in-a-partially-ordered-set). The interval cannot be empty either, by the defining approximation property of a [supremum](#supremum). Thus failure to attain a finite [supremum](#supremum) forces accumulation from below.

### Infimum

↑ **Parent:** [Infimum and supremum](#infimum-and-supremum)

The infimum of a set of real numbers is its greatest lower bound.

## Asymptotic analysis

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_analysis)

Asymptotic analysis compares functions or [sequences](#sequence) as their argument approaches a limit, using bounds such as [Big O notation](#big-o-notation) and relations such as [asymptotic equivalence](#asymptotic-equivalence). It records the leading behavior and the size of errors.

### Asymptotic equivalence

↑ **Parent:** [Asymptotic analysis](#asymptotic-analysis)

The notation $a_n\sim b_n$ means $a_n/b_n\to1$.

#### Asymptotic comparison of exponential functions

↑ **Parent:** [Asymptotic equivalence](#asymptotic-equivalence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_comparison_of_exponential_functions)

Ratios of exponential functions are controlled by comparing their linear growth exponents.

#### Stirling formula

↑ **Parent:** [Asymptotic equivalence](#asymptotic-equivalence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stirling_formula)

Stirling’s formula gives n factorial asymptotic to square root of 2 pi n times (n/e)^n.

##### Stirling correction by Gaussian moments

↑ **Parent:** [Stirling formula](#stirling-formula)

In [Laplace method](analysis.md#laplace-s-method) for the [Gamma function](complex-analysis.md#gamma-function), scaling $t=x(1+s/\sqrt x)$ gives a standard [Gaussian integral](calculus.md#gaussian-integral). The first even correction polynomial is $s^2-7s^4/12+s^6/18$. Its expectation under a unit-variance centered Gaussian is $1-7\cdot3/12+15/18=1/12$. The amplitude expansion contributes to this coefficient as well as the phase expansion; expanding only the latter gives the wrong [Stirling formula](#stirling-formula) correction.

## Monotone integral Tauberian lemma

↑ **Parent:** [Real analysis](real-analysis.md)

For nondecreasing real $\beta$, convergence of the displayed improper integral forces $\beta(x)/x\to1$. For $\lambda>1$, the integral over $[X,\lambda X]$ tends to zero and is at least $(1-\lambda^{-1})\beta(X)/X-\log\lambda$. The integral over $[X/\lambda,X]$ tends to zero and is at most $(\lambda-1)\beta(X)/X-\log\lambda$. These bound the upper and lower limits by $\log\lambda/(1-\lambda^{-1})$ and $\log\lambda/(\lambda-1)$. Letting $\lambda\downarrow1$ squeezes both to one. The limit of the improper integral must be finite.

## Homogeneous function

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homogeneous_function)

A [function](function.md) is homogeneous of degree $k$ when rescaling its arguments by a common [scalar](vector-space.md#scalar) $\lambda$ rescales its value by $\lambda^k$, whenever the arguments and that power are defined. For integer $k$ over a [vector space](vector-space.md), one can require every nonzero scalar; a [homogeneous polynomial](algebra.md#homogeneous-polynomial) gives an example. On a domain stable under positive real rescaling, the positive-scaling version allows real $k$. Degree-one [positive homogeneity](#positively-homogeneous-function-degree-one) is the convention used for [norms](functional-analysis.md#norm) and many [convex functions](#convex-function). The [Euler theorem for homogeneous functions](#euler-theorem-for-homogeneous-functions) turns this scaling law into a differential identity for a [differentiable function](analysis.md#differentiable-function).

### Homogeneity

↑ **Parent:** [Homogeneous function](#homogeneous-function)

Homogeneity of degree $k$ means that multiplying all arguments by a common positive factor $a$ multiplies the output by $a^k$. A [homogeneous function](#homogeneous-function) is the function possessing this property. This is different from degree-one [positive homogeneity](#positively-homogeneous-function-degree-one); investment values with [constant relative risk aversion utility](utility-function.md#constant-relative-risk-aversion-utility) usually have degree $1-R$.

### Positively homogeneous function (degree one)

↑ **Parent:** [Homogeneous function](#homogeneous-function)

A [function](function.md) on a cone is positively homogeneous of degree one when $f(tX)=t f(X)$ for every $t>0$. If such a function is [concave](#concave-function), then

$$
f(X+tY)\geq f(X)+t f(Y),
$$

because homogeneity rewrites the left-hand side as $(1+t)f((X+tY)/(1+t))$ before [concavity](#concave-function) is applied.

### Euler theorem for homogeneous functions

↑ **Parent:** [Homogeneous function](#homogeneous-function)

Let $f$ be a [differentiable function](analysis.md#differentiable-function) on an open domain stable under positive rescaling, with $f(\lambda x)=\lambda^kf(x)$ for $\lambda>0$. The [chain rule](calculus.md#chain-rule) differentiates this [homogeneous function](#homogeneous-function) identity at $\lambda=1$ to give

$$
\sum_ix_i\partial_i f(x)=k f(x).
$$

If $f$ is twice differentiable, differentiating once more gives $\sum_i x_i\partial_i\partial_jf=(k-1)\partial_j f$. In degree one its [Hessian matrix](calculus.md#hessian-matrix) therefore annihilates the radial vector $x$. This is the identity used in the [no-scale identity from degree-one homogeneity](supersymmetry.md#no-scale-identity-from-degree-one-homogeneity). For an [extensive quantity](thermodynamics.md#extensive-quantity), the degree-one formula also supplies the thermodynamic identity behind the [Gibbs-Duhem equation](thermodynamics.md#gibbs-duhem-equation).

#### Euler differential identity characterizes homogeneity

↑ **Parent:** [Euler theorem for homogeneous functions](#euler-theorem-for-homogeneous-functions)

On an open domain invariant under positive scaling, $Df_x(x)=cf(x)$ implies $f(\lambda x)=\lambda^cf(x)$. Indeed, $\frac d{d\lambda}[\lambda^{-c}f(\lambda x)]=\lambda^{-c-1}[Df_{\lambda x}(\lambda x)-cf(\lambda x)]=0$. The converse follows by differentiating the scaling identity at $\lambda=1$. Connectedness of the whole domain is unnecessary: the argument works along each positive ray.

#### Volume integral of a homogeneous function

↑ **Parent:** [Euler theorem for homogeneous functions](#euler-theorem-for-homogeneous-functions)

For a sufficiently regular [homogeneous function](#homogeneous-function) $f$ of degree $n$ on a three-dimensional region, [Euler theorem for homogeneous functions](#euler-theorem-for-homogeneous-functions) gives $x\cdot\nabla f=nf$. Hence $\nabla\cdot(fx)=(n+3)f$, and the [divergence theorem](calculus.md#divergence-theorem) gives the displayed reduction when $n\ne-3$. At degree $-3$ only the zero-flux identity follows, so division by $n+3$ is unavailable. Singular functions additionally require an excision or limiting argument; the surface contribution at a removed singularity must not be silently dropped. On the sloping side of a cone with its apex at zero, $x$ is tangent to the side and $x\cdot n=0$, so only the cap contributes to this formula.

## Regular variation

↑ **Parent:** [Real analysis](real-analysis.md)

A positive measurable function $q$ has [regular variation](#regular-variation) at infinity with index $\rho$ if $q(tu)/q(t)\to u^\rho$ for every $u>0$. Equivalently, $q(t)=t^\rho\ell(t)$ with $\ell$ a [slowly varying function](#slowly-varying-function).

### Slowly varying function

↑ **Parent:** [Regular variation](#regular-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slowly_varying_function)

A [slowly varying function](#slowly-varying-function) has [regular variation](#regular-variation) with index zero: $\ell(tu)/\ell(t)\to1$ for every $u>0$. A power of $\log t$ is an example.

## Lipschitz continuity

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lipschitz_continuity)

A function $f$ is Lipschitz continuous when there is a constant $L\geq0$ such that

$$
|f(x)-f(y)|\leq L|x-y|
$$

for all points in its domain.

### Bounded Lipschitz norm

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

The bounded Lipschitz norm combines the [Lipschitz constant](#lipschitz-constant) and [supremum norm](functional-analysis.md#supremum-norm) of a bounded real-valued [Lipschitz function](#lipschitz-continuity) on a [metric space](topological-analysis.md#metric-space). Both summands satisfy the [triangle inequality](topological-analysis.md#triangle-inequality); the supremum term makes the sum definite even on constant functions. Its unit ball requires the sum of the two bounds to be at most one, a stronger requirement than bounding each separately by one.

#### Diagonal compactness for bounded Lipschitz functions

↑ **Parent:** [Bounded Lipschitz norm](#bounded-lipschitz-norm)

On a separable [metric space](topological-analysis.md#metric-space), a sequence uniformly bounded in [bounded Lipschitz norm](#bounded-lipschitz-norm) has a pointwise convergent subsequence. Enumerate a countable dense subset and use the [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem) and [diagonal subsequence argument](#diagonal-subsequence-argument) to obtain convergence there. Uniform control of the [Lipschitz constant](#lipschitz-constant) then makes the subsequence Cauchy at every point. The [pointwise closure of the bounded Lipschitz unit ball](#pointwise-closure-of-the-bounded-lipschitz-unit-ball) preserves the original norm bound after rescaling.

#### Pointwise closure of the bounded Lipschitz unit ball

↑ **Parent:** [Bounded Lipschitz norm](#bounded-lipschitz-norm)

For every fixed $x\ne y$ and $z$, the sum $|f_i(x)-f_i(y)|/d(x,y)+|f_i(z)|$ is at most one. [Pointwise convergence](#pointwise-convergence) preserves this inequality. Taking the independent suprema over the pair $(x,y)$ and the point $z$ proves the assertion. Taking each bound separately would only give the weaker estimate two.

### One-sided Lipschitz condition

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

A one-sided Lipschitz condition controls the growth of distances between solutions of an [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Differentiating the squared difference and applying the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) gives $\|y(t)-z(t)\|\leq e^{\nu t}\|y(0)-z(0)\|$. The case $\nu\leq0$ is a [dissipative vector field](differential-equation.md#dissipative-vector-field). Ordinary [Lipschitz continuity](#lipschitz-continuity) implies such a bound, but the converse fails: $f(y)=-y^3$ has one-sided constant zero on the real line without being globally [Lipschitz continuous](#lipschitz-continuity).

### Lipschitz domain

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lipschitz_domain)

A Lipschitz domain is an open connected subset of [Euclidean space](functional-analysis.md#euclidean-norm) whose boundary is locally the graph of a [Lipschitz continuous](#lipschitz-continuity) function after rotating and translating coordinates. Locally the domain lies on one side of that graph. This permits corners but excludes boundary cusps that cannot be represented with a finite Lipschitz constant. Bounded Lipschitz domains are a standard setting for [Sobolev spaces](sobolev-space.md) and the [Poincaré inequality for total variation](inverse-problem.md#poincare-inequality-for-total-variation).

### McShane extension theorem

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/McShane_extension_theorem)

If $f:A\to\mathbb R$ is $L$-Lipschitz on a subset of a metric space, then

$$
F(x)=\inf_{y\in A}\{f(y)+Ld(x,y)\}
$$

extends $f$ to the whole space and remains $L$-Lipschitz.

### Lipschitz constant

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

The least $L\geq0$ for which $d(f(x),f(y))\leq Ld(x,y)$ for every $x,y$ is the [Lipschitz constant](#lipschitz-constant) of $f$. Any admissible $L$ is a [Lipschitz bound](#lipschitz-bound).

### Globally Lipschitz function

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

A function is globally Lipschitz when one [Lipschitz bound](#lipschitz-bound) holds for every pair of points in its domain. Unlike local Lipschitz continuity, this condition gives a uniform growth control over the whole domain.

### Lipschitz bound

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

A Lipschitz bound has the form $|f(x)-f(y)|\leq L|x-y|$. It controls the change of a function by the change of its argument.

### Locally Lipschitz function

↑ **Parent:** [Lipschitz continuity](#lipschitz-continuity)

A function is locally Lipschitz when every point has a neighborhood on which the function satisfies a [Lipschitz bound](#lipschitz-bound). Continuously differentiable functions are locally Lipschitz.

## Big O notation

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Big_O_notation)

The relation $f(x)=O(g(x))$ near a limit point means that $|f(x)|\leq C|g(x)|$ there for some constant $C$.

## Real line

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real_line)

The real line is the set $\mathbb R$ of real numbers equipped with its usual order, metric, and topology.

### Interval (mathematics)

↑ **Parent:** [Real line](#real-line)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interval_(mathematics))

A real interval contains every real number lying between any two of its elements.

#### Nested intervals

↑ **Parent:** [Interval (mathematics)](#interval-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nested_intervals)

A nested family of [real intervals](#interval-mathematics) satisfies $I_{n+1}\subseteq I_n$. The [nested interval theorem](#nested-interval-theorem) ensures a common point for nonempty closed bounded members; open intervals can instead have empty intersection.

##### Nested interval theorem

↑ **Parent:** [Nested intervals](#nested-intervals)

If $I_1\supseteq I_2\supseteq\cdots$ are nonempty closed bounded intervals, then their intersection is nonempty. If their lengths tend to zero, the intersection consists of exactly one point.

#### Closed real interval

↑ **Parent:** [Interval (mathematics)](#interval-mathematics)

A bounded closed real interval has the form $[a,b]=\{x\in\mathbb R:a\leq x\leq b\}$.

This is a closed instance of a [real interval](#interval-mathematics); the general interval concept also includes open and half-open intervals.

## Extreme value theorem

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extreme_value_theorem)

A real-valued [continuous function](calculus.md#continuous-function) on a nonempty [compact space](topology.md#compact-space) attains both its minimum and its maximum.

### Interior-value criterion for an attained maximum

↑ **Parent:** [Extreme value theorem](#extreme-value-theorem)

Let $f$ be continuous on $(a,b]$, bounded above, and suppose its [limit superior](#limit-superior) at $a$ from the right is at most $L$. If some $c\in(a,b]$ has $f(c)>\max\{L,f(a)\}$, then $f$ attains its maximum on $[a,b]$. A sufficiently short initial interval has all values below $f(c)$. On the remaining closed interval, the [extreme value theorem](#extreme-value-theorem) supplies a maximum, which is consequently global. This can prove attainment despite an oscillatory discontinuity at one endpoint.

### Supremum can fail to be attained at an oscillatory endpoint

↑ **Parent:** [Extreme value theorem](#extreme-value-theorem)

The [extreme value theorem](#extreme-value-theorem) requires continuity on the entire closed interval. A bounded function can have values tending to an endpoint envelope without ever reaching that envelope, while its defined endpoint value is smaller. To prove nonattainment, establish a strict pointwise upper bound and construct a sequence approaching that bound. An oscillatory factor can supply the approaching sequence by selecting phases where it equals $1$.

## Coercive function

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coercive_function)

A real-valued function on a normed vector space is coercive when its value tends to positive infinity as the norm of its argument tends to infinity. A continuous coercive function on a finite-dimensional real vector space attains a global minimum.

### Range of a continuous coercive real function

↑ **Parent:** [Coercive function](#coercive-function)

A real [continuous function](calculus.md#continuous-function) on $\mathbb R$ that tends to $+\infty$ as $|x|\to\infty$ has range $[m,\infty)$ for an attained minimum $m$. Choose a compact interval outside which its values exceed $f(0)$, and minimize there by the [extreme value theorem](#extreme-value-theorem). For any $y>m$, choose a far point with value larger than $y$ and apply the [intermediate value theorem](calculus.md#intermediate-value-theorem) between it and a minimizer. Distance from a fixed point to a continuous graph is an example because it is at least the horizontal distance.

## Lp norm

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lp_norm)

For a measurable function $f$, its $L^p$ norm is

$$
\lVert f\rVert_p=\left(\int |f|^p\right)^{1/p}
$$

when $1\leq p<\infty$, while $\lVert f\rVert_\infty$ is its essential supremum.

### Lq quasi-norm

↑ **Parent:** [Lp norm](#lp-norm)

The displayed quantity is homogeneous and separates zero, but generally violates the [triangle inequality](topological-analysis.md#triangle-inequality). Its $q$th power is subadditive because $(a+b)^q\le a^q+b^q$ for nonnegative $a,b$. Minimizing it is equivalent to minimizing its $q$th power. On finite [vectors](vector-space.md#vector) it is a standard nonconvex sparsity penalty.

### Minkowski inequality

↑ **Parent:** [Lp norm](#lp-norm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minkowski_inequality)

For $1\leq p\leq\infty$, the [Lp norm](#lp-norm) satisfies the [triangle inequality](topological-analysis.md#triangle-inequality). For $1<p<\infty$, apply the [Holder inequality](functional-analysis.md#holder-inequality) to $\int(|f|+|g|)|f+g|^{p-1}$, then divide by $\|f+g\|_p^{p-1}$ when it is nonzero. The cases $p=1$ and $p=\infty$ follow directly from the pointwise triangle inequality. In particular, a series whose term norms have a finite sum converges in the complete $L^p$ space.

### L2 norm

↑ **Parent:** [Lp norm](#lp-norm)

The $L^2$ norm is

$$
\lVert f\rVert_2=\left(\int|f|^2\right)^{1/2}.
$$

It is induced by the $L^2$ inner product and is the continuous analogue of the [Euclidean norm](functional-analysis.md#euclidean-norm).

<h3 id="marcinkiewicz-zygmund-inequality">Marcinkiewicz–Zygmund inequality</h3>

↑ **Parent:** [Lp norm](#lp-norm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Marcinkiewicz–Zygmund_inequality)

For independent mean-zero random variables $X_1,\ldots,X_n$ and $p\geq1$, the Marcinkiewicz–Zygmund inequality compares the $L^p$ norm of their sum with the square function:

$$
\mathbb E\left|\sum_iX_i\right|^p
\leq C_p\,\mathbb E\left(\sum_i|X_i|^2\right)^{p/2}.
$$

For $p=2m$, one may take $C_p^{1/p}=O(\sqrt m)$.

<h3 id="holder-s-inequality">Hölder's inequality</h3>

↑ **Parent:** [Lp norm](#lp-norm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hölder's_inequality)

For conjugate exponents $p,q\in[1,\infty]$, [Hölder's inequality](#holder-s-inequality) states $\lVert fg\rVert_1\leq\lVert f\rVert_p\lVert g\rVert_q$. For finite vectors, the case $p=1$, $q=\infty$ is $|x^Ty|\leq\lVert x\rVert_1\lVert y\rVert_\infty$.

## Sequence and series

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sequence_and_series)

A sequence is an ordered family indexed by the natural numbers; a series studies the partial sums of a sequence of terms.

### Dyadic-block alternation of reciprocal terms

↑ **Parent:** [Sequence and series](#sequence-and-series)

For $0\le r<2^n$ and $n\ge0$, the displayed [sequence](#sequence) tends to zero, but its [series](#series-mathematics) diverges. The signed sum across the $n$th dyadic block has magnitude $\sum_{r=0}^{2^n-1}(2^n+r)^{-1}\ge1/2$. Differences of arbitrarily late [partial sums](#partial-sum) therefore fail the [Cauchy sequence](#cauchy-sequence) condition on [partial sums](#partial-sum). Alternating signs between blocks do not rescue convergence when the total contribution of an entire block stays away from zero.

### Lucas number

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lucas_number)

The [Lucas numbers](#lucas-number) obey the same second-order recurrence as the [Fibonacci numbers](#fibonacci-number) but start with $2,1$, so their sequence is $2,1,3,4,7,11,\ldots$. For $n\ge1$, $L_n=F_{n-1}+F_{n+1}$. Substitution in the [Fibonacci addition formula](#fibonacci-addition-formula) gives $F_{2n}=F_nL_n$. Consecutive [Fibonacci numbers](#fibonacci-number) are coprime by the [Euclidean algorithm](number-theory.md#euclidean-algorithm); since $L_n=F_n+2F_{n-1}$, [Bézout's identity](algebra.md#bezout-identity) gives $\gcd(F_n,L_n)=\gcd(F_n,2)\le2$.

### Sequence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sequence)

A sequence is a function whose domain is usually the natural numbers.

#### Limit inferior and limit superior

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_inferior_and_limit_superior)

For a real [sequence](#sequence) $(a_n)$, the [limit inferior](#limit-inferior) is the limit of the infima of its tails and the [limit superior](#limit-superior) is the limit of the suprema of its tails. These extended-real bounds describe its lowest and highest limiting behavior.

##### Limit inferior

↑ **Parent:** [Limit inferior and limit superior](#limit-inferior-and-limit-superior)

The limit inferior of a real sequence $(a_n)$ is

$$
\liminf_{n\to\infty}a_n=\lim_{n\to\infty}\inf_{k\geq n}a_k.
$$

It is the smallest subsequential limit when the sequence is bounded.

#### Recurrence relation

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Recurrence_relation)

A recurrence relation specifies members of a [sequence](#sequence) in terms of previous members, together with enough initial values to determine the sequence. A three-term recurrence for [orthogonal polynomials](numerical-analysis.md#orthogonal-polynomial) relates consecutive orders. For example, the physicists' [Hermite polynomials](numerical-analysis.md#hermite-polynomial) satisfy $H_{n+1}(x)=2xH_n(x)-2nH_{n-1}(x)$, starting from $H_0=1$ and $H_1=2x$.

##### Difference equation

↑ **Parent:** [Recurrence relation](#recurrence-relation)

A [difference equation](#difference-equation) relates values of a [sequence](#sequence) at different indices, or its finite differences. A first-order autonomous system has the displayed form, with a scalar or vector state. Writing $z_{n+1}-z_n=F(z_n)-z_n$ gives its equivalent finite-difference form. Its [fixed point](function.md#fixed-point) stability is determined by the [Jacobian matrix](calculus.md#jacobian-matrix) of the update and the [unit circle](complex-analysis.md#complex-unit-circle), whereas a continuous-time [differential equation](differential-equation.md) uses the real parts of its linearized [eigenvalues](linear-operator-theory.md#eigenvalue).

<h4 id="thue-morse-sequence">Thue–Morse sequence</h4>

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thue–Morse_sequence)

Here $s_2(n)$ is the sum of the [binary digits](number-theory.md#binary-digit) of the nonnegative [integer](number-theory.md#integer) $n$. The sign version is $f(n)=(-1)^{s_2(n)}$. Concatenating binary digits gives $f(a2^j+r)=f(a)f(r)$ for $0\le r<2^j$. It supplies cancellation controlled by binary blocks rather than multiplicative factorization.

<h5 id="thue-morse-fourier-product">Thue–Morse Fourier product</h5>

↑ **Parent:** [Thue–Morse sequence](#thue-morse-sequence)

Each [binary digit](number-theory.md#binary-digit) independently contributes either $1$ or $-e(2^l\theta)$, proving the product. Two adjacent factors have modulus $8|\cos(\pi t)|(1-\cos^2(\pi t))\le16/(3\sqrt3)<4$. Consequently the product is $O(2^{\sigma j})$, with $\sigma=2-\frac34\log_2 3<1$. This two-factor estimate suffices for a power saving, though its exponent is not optimal.

###### Uniform interval cancellation for binary digit parity

↑ **Parent:** [Thue–Morse Fourier product](#thue-morse-fourier-product)

An integer interval is a disjoint union of aligned binary blocks with at most two of each length. On $[a2^j,(a+1)2^j)$ the [Thue–Morse sequence](#thue-morse-sequence) sign factors as $f(a)f(r)$, so the [Thue–Morse Fourier product](#thue-morse-fourier-product) bounds its [exponential sum](analytic-number-theory.md#exponential-sum) by $O(2^{\sigma j})$. Sum the geometric series over block lengths to obtain the uniform bound, for $\sigma=2-\frac34\log_2 3$.

###### Small Type I sums for binary digit parity

↑ **Parent:** [Uniform interval cancellation for binary digit parity](#uniform-interval-cancellation-for-binary-digit-parity)

The additive [character orthogonality](representation-theory.md#character-orthogonality) filter $1_{m\mid r}=m^{-1}\sum_{a=0}^{m-1}e(ar/m)$ restricts the [uniform interval cancellation for binary digit parity](#uniform-interval-cancellation-for-binary-digit-parity) to multiples of $m$, without increasing its bound. Each inner [Type I sum](analytic-number-theory.md#type-i-sum) is therefore $O(N^\sigma)$. Summing the at most $N^{1/100}$ outer terms proves the displayed estimate, which is smaller than every fixed negative power of $\log N$ for large $N$.

#### Cluster-set matching of bounded sequences

↑ **Parent:** [Sequence](#sequence)

Two bounded real sequences with the same set of subsequential limits admit permutations that match their terms with differences tending to zero. Alternate between taking the least unused index of the first sequence and of the second. Match its value to an unused term of the other sequence near a nearest common cluster point, with additional error at most $1/j$ at stage $j$. Every cluster-point neighbourhood contains infinitely many available terms. The actively chosen indices tend to infinity, whose distance to the common cluster set tends to zero by boundedness. By step $2j$, both lists have included every index up to $j$.

<h4 id="fejer-monotonicity">Fejér monotonicity</h4>

↑ **Parent:** [Sequence](#sequence)

A sequence is Fejér monotone with respect to a nonempty set $C$ if $\|z^{k+1}-p\|\leq\|z^k-p\|$ for every $p\in C$. It is bounded. If it has a cluster point $\bar z\in C$, its nonincreasing distance to $\bar z$ and that convergent subsequence force the entire sequence to converge to $\bar z$.

#### Finite repetition-free sequence

↑ **Parent:** [Sequence](#sequence)

A [finite repetition-free sequence](#finite-repetition-free-sequence) in a [set](set.md) $X$ is an [injective function](algebra.md#injective-function) from an initial segment $\{0,\ldots,k-1\}$ of the [natural numbers](arithmetic.md#natural-number) into $X$, including the empty [sequence](#sequence) for $k=0$. For a [finite set](set.md#finite-set) of size $m$, the number of these [sequences](#sequence) is

$$
\sum_{k=0}^m\frac{m!}{(m-k)!}.
$$

The order of each list is part of the data, so it can be enumerated without choosing an order on its underlying support.

#### Subadditive sequence

↑ **Parent:** [Sequence](#sequence)

A real sequence $(a_n)$ is subadditive when $a_{m+n}\leq a_m+a_n$ for all positive $m,n$. [Fekete lemma](#fekete-s-lemma) gives

$$
\lim_{n\to\infty}\frac{a_n}{n}=\inf_{n\geq1}\frac{a_n}{n},
$$

allowing the value negative infinity.

##### Asymmetrically almost-subadditive sequence

↑ **Parent:** [Subadditive sequence](#subadditive-sequence)

If the real error depends only on the second index and $\alpha_n/n\to0$, the normalized sequence has a limit in $[-\infty,\infty)$. For fixed $k$, write $n=qk+r$ with $1\leq r\leq k$ and iterate to obtain $x_n\leq x_r+q(x_k+\alpha_k)$. It follows that $\limsup x_n/n\leq(x_k+\alpha_k)/k$ for every $k$; a subsequence attaining the lower limit proves convergence. The limit is $\inf_k(x_k+\alpha_k)/k$, even when the errors can be negative.

#### Geometric progression

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_progression)

A geometric progression is a [sequence](#sequence) whose successive terms have a constant ratio: $a_n=ar^n$ for constants $a$ and $r$.

#### Subsequence

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subsequence)

A subsequence of $(a_n)$ has the form $(a_{n_k})$, where $n_1<n_2<\cdots$ is a strictly increasing sequence of indices.

##### Monotone subsequence theorem

↑ **Parent:** [Subsequence](#subsequence)

Every real sequence has a monotone [subsequence](#subsequence), without a boundedness assumption. Call an index a peak when its term is at least every later term. Infinitely many peaks give a nonincreasing subsequence; beyond finitely many peaks each term has a larger later term, which recursively gives an increasing subsequence.

#### Null sequence

↑ **Parent:** [Sequence](#sequence)

A null sequence is a sequence that converges to the additive identity zero in its ambient topological vector space.

#### Bounded sequence

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounded_sequence)

A sequence $(x_n)$ in a metric space is bounded when all its terms lie in some ball of finite radius.

##### Bounded subsequence

↑ **Parent:** [Bounded sequence](#bounded-sequence)

A bounded subsequence is a [subsequence](#subsequence) whose terms all lie in one fixed bounded set.

#### Bitstream

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bitstream)

A binary sequence is a finite or infinite sequence whose terms belong to $\{0,1\}$.

##### Uncountability by interleaving prescribed binary coordinates

↑ **Parent:** [Bitstream](#bitstream)

Partition the positive [natural numbers](arithmetic.md#natural-number) into three infinite coordinate [sets](set.md). Fix the coordinates on the first two [sets](set.md) to any prescribed binary values, and leave those on the third [set](set.md) free. Reading the third coordinate [set](set.md) embeds all infinite [binary sequences](#bitstream) in the resulting family, so the family is an [uncountable set](set-theory.md#uncountable-set) by [Cantor's diagonal argument](set-theory.md#cantor-s-diagonal-argument). For example, fixing $x_{3k-2}=0$ and $x_{3k-1}=a_{3k-1}$ while leaving $x_{3k}$ free guarantees infinitely many zeros and infinitely many agreements with any prescribed [binary sequence](#bitstream) $(a_n)$. Infinite free coordinates remain even after both requirements are enforced.

#### Monotone sequence

↑ **Parent:** [Sequence](#sequence)

A real sequence is increasing when $a_{n+1}\geq a_n$ and decreasing when $a_{n+1}\leq a_n$.

##### Minimum-decrement convergence criterion

↑ **Parent:** [Monotone sequence](#monotone-sequence)

Suppose $x_n,y_n>0$ and the displayed inequality holds with fixed $\lambda>0$. Then $y_n$ decreases to some $l\ge0$. Telescoping shows $\sum_n\min(x_n,y_n)\le y_1/\lambda$. If $l>0$, this bounds $\sum_n\min(x_n,l)$, contradicting [clipping preserves divergence of a positive series](#clipping-preserves-divergence-of-a-positive-series) when $\sum_nx_n$ diverges. Thus divergence of the positive input series forces $y_n\to0$.

##### Bounded nondecreasing rational sequences are uncountable

↑ **Parent:** [Monotone sequence](#monotone-sequence)

Map a [binary sequence](#bitstream) $(\epsilon_j)$ to the rational partial sums $s_n=\sum_{j=1}^n\epsilon_j3^{-j}$. They are nondecreasing and bounded above by $1/2$. A first different digit makes the corresponding partial sums different at that index, so the map is injective. [Cantor's diagonal argument](set-theory.md#cantor-s-diagonal-argument) then makes this family uncountable despite every individual term being rational.

// Target: special-relativity.bigb

##### Bounded nondecreasing integer sequences are eventually constant

↑ **Parent:** [Monotone sequence](#monotone-sequence)

If an integer-valued [monotone sequence](#monotone-sequence) $(a_n)$ is nondecreasing and bounded above by $M$, it can increase strictly at most $\lfloor M\rfloor-a_1$ times. Thus its values eventually remain constant. Such sequences are determined by a finite initial list followed by a constant tail, so their collection is a [countable set](set-theory.md#countable-set).

##### Bounded monotone sequence theorem

↑ **Parent:** [Monotone sequence](#monotone-sequence)

A real increasing [sequence](#sequence) bounded above converges to its [supremum](#supremum); a decreasing [sequence](#sequence) bounded below converges to its [infimum](#infimum). For the increasing case, the definition of [supremum](#supremum) provides a term above $L-\varepsilon$, and every later term remains between that term and $L$. Negation reduces the decreasing case to the increasing case. This elementary result is distinct from the measure-theoretic [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) for integrals.

#### Limit superior

↑ **Parent:** [Sequence](#sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_superior)

The limit superior of a real sequence $(a_n)$ is

$$
\limsup_{n\to\infty}a_n=\lim_{n\to\infty}\sup_{k\geq n}a_k.
$$

It is the largest subsequential limit when the sequence is bounded.

### Series (mathematics)

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Series_(mathematics))

A series is the formal or limiting sum of the terms of a [sequence](#sequence).

<h4 id="cesaro-summation">Cesàro summation</h4>

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cesàro_summation)

A [series](#series-mathematics) is Cesàro summable to $L$ when the [Cesaro means](#cesaro-mean) of its [partial sums](#partial-sum) converge to $L$. This is a summation method for series, distinct from a mean of the original terms. The [Cesaro theorem for convergent sequences](#cesaro-theorem-for-convergent-sequences) ensures that every ordinarily convergent [series](#series-mathematics) has the same Cesàro sum. The alternating series $1-1+1-\cdots$ has Cesàro sum $1/2$ without an ordinary sum.

#### Factorial series

↑ **Parent:** [Series (mathematics)](#series-mathematics)

A factorial series with digits $0\leq a_n<n$ is an absolutely convergent [series](#series-mathematics) of [real numbers](arithmetic.md#real-number) between zero and one. The [telescoping series](#telescoping-series) identity

$$
\frac{n-1}{n!}=\frac1{(n-1)!}-\frac1{n!}
$$

shows that its largest possible tail after place $N$ is $1/N!$. Multiplying this tail by $N!$ gives a number between zero and one, a useful arithmetic constraint on [rational numbers](number-theory.md#rational-number).

##### Irrationality criterion for factorial series

↑ **Parent:** [Factorial series](#factorial-series)

A [factorial series](#factorial-series) with integral digits $0\leq a_n<n$ is an [irrational number](algebra.md#irrational-number) exactly when positive digits occur infinitely often and digits below their maximum occur infinitely often. Under these two conditions every scaled tail $N!\sum_{n>N}a_n/n!$ lies strictly between zero and one. If the sum were a [rational number](number-theory.md#rational-number) $A/B$, choose $N\geq B$; then $N!A/B$ and the scaled finite head are [integers](number-theory.md#integer), contradicting the strict tail bound. Conversely, an eventually zero digit sequence gives a finite [rational number](number-theory.md#rational-number) sum, and an eventually maximal sequence gives a finite head plus $1/N!$, again a [rational number](number-theory.md#rational-number).

#### Polynomial-logarithmic series convergence

↑ **Parent:** [Series (mathematics)](#series-mathematics)

For $p,q>0$, the positive [series](#series-mathematics) converges precisely when $p>1$, or $p=1$ and $q>1$. For $p>1$ use comparison with a convergent [p-series](#p-series); for $0<p<1$, the bound $(\log n)^q<n^{(1-p)/2}$ gives a lower comparison with a divergent [p-series](#p-series). At $p=1$, the [integral test for convergence](#integral-test-for-convergence) and $u=\log x$ reduce the question to $\int u^{-q}\,du$. In contrast, $\sum_{n\geq3}[n(\log\log n)^r]^{-1}$ diverges for every finite $r>0$, since $(\log\log n)^r<\log n$ eventually and $\sum[n\log n]^{-1}$ diverges.

#### Root test

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Root_test)

For a series $\sum_n a_n$, let $r=\limsup_{n\to\infty}|a_n|^{1/n}$. If $r<1$, choose $r<\rho<1$; eventually $|a_n|\leq\rho^n$, so geometric comparison gives absolute convergence. If $r>1$, the terms fail to tend to zero along a subsequence and the series diverges. At $r=1$, the test is inconclusive.

#### Telescoping series

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Telescoping_series)

A telescoping series has partial sums in which consecutive terms cancel, commonly because its summand has the form $b_n-b_{n+1}$.

#### Term test for divergence

↑ **Parent:** [Series (mathematics)](#series-mathematics)

If the terms $a_n$ of a series do not converge to zero, then $\sum_na_n$ diverges. This is the contrapositive of $a_n=S_n-S_{n-1}\to0$ for convergent partial sums.

#### Infinite product

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite_product)

An infinite product is the [limit](calculus.md#limit-of-a-function) of the finite partial products $\prod_{n=1}^N a_n$. If $a_n=1+u_n$, every factor is nonzero, and $\sum_n|u_n|<\infty$, then the product converges to a nonzero value.

##### Reciprocal geometric infinite product

↑ **Parent:** [Infinite product](#infinite-product)

For $|q|>1$, define $S_q(z)=\prod_{k\geq0}(1-q^{-2k-1}z)(1-q^{-2k-1}z^{-1})$ on $\mathbb C^*$. The geometric decay gives locally uniform absolute tail convergence there. Its [simple zeros](complex-analysis.md#simple-zero) are $q^{2k+1}$ and $q^{-2k-1}$ for $k\geq0$, and reindexing gives $S_q(qz)=-zS_q(q^{-1}z)$. The variable zero is outside its domain, and the poles introduced by each reciprocal factor cannot be interpreted as a value of the product at zero.

// Destination: analysis.bigb

##### Weierstrass elementary factor

↑ **Parent:** [Infinite product](#infinite-product)

The Weierstrass elementary factor has a simple zero at $w=1$ and no other zeros. Its logarithmic series begins at degree $p+1$: $\log E_p(w)=-\sum_{\nu\geq p+1}w^\nu/\nu$ for $|w|<1$. Raising the factor order $p$ makes the tail arbitrarily small on a fixed compact set and enables [infinite product convergence from logarithmic tails](#infinite-product-convergence-from-logarithmic-tails) for unrestricted discrete zero data.

##### Infinite product convergence from logarithmic tails

↑ **Parent:** [Infinite product](#infinite-product)

If a tail of holomorphic factors admits logarithms whose absolute values have a summable bound uniformly on every compact set, their product converges locally uniformly to the exponential of the logarithmic sum. The tail is holomorphic and nowhere zero. Finite initial factors may have zeros; those finite factors determine the locations and orders of all zeros near any given compact set. The scalar sufficient condition $\sum_j|u_j|<\infty$ for factors $1+u_j$ follows from $|\log(1+u_j)|\leq2|u_j|$ for $|u_j|\leq1/2$.

##### Positive sum-product convergence criterion

↑ **Parent:** [Infinite product](#infinite-product)

For $a_j\geq0$, the finite product satisfies

$$
1+\sum_{j=1}^na_j\leq\prod_{j=1}^n(1+a_j)\leq\exp\left(\sum_{j=1}^na_j\right).
$$

The lower inequality follows by product expansion; the upper one uses $1+t\leq e^t$. Since both the partial sums and partial products are increasing, one converges to a finite limit exactly when the other does. The [monotone bounded sequence](#monotone-bounded-sequence) theorem proves both implications. The product cannot tend to zero in this nonnegative setting.

##### Hyperbolic-sine infinite product

↑ **Parent:** [Infinite product](#infinite-product)

This [infinite product](#infinite-product) converges uniformly on compact subsets of the complex plane. Pair the factors at $iz$ and $-iz$ in the [Weierstrass product for the reciprocal gamma function](complex-analysis.md#weierstrass-product-for-the-reciprocal-gamma-function), and use the [Gamma reflection formula](complex-analysis.md#gamma-reflection-formula) together with $\Gamma(1+w)=w\Gamma(w)$. This gives $[\Gamma(1+iz)\Gamma(1-iz)]^{-1}=\sinh(\pi z)/(\pi z)$ and the displayed product. The removable value at $z=0$ is one. Matching zeros alone would not exclude multiplication by a nonvanishing [entire function](complex-analysis.md#entire-function); the normalized product fixes that ambiguity.

#### Lattice sum

↑ **Parent:** [Series (mathematics)](#series-mathematics)

A lattice sum is a [series](#series-mathematics) indexed by the points of a [lattice](mathematical-logic.md#lattice). For example, comparison with annular lattice-point counts shows that $\sum_{(m,n)\ne(0,0)}(m^2+n^2)^{-s}$ converges when $s>1$.

#### Partial sum

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_sum)

For terms $(a_n)$, the $n$th partial sum is $S_n=\sum_{j=1}^n a_j$. A [series](#series-mathematics) converges when its sequence of partial sums converges.

#### Kronecker lemma

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kronecker_lemma)

Let $(b_n)$ be positive and increase to infinity. If the [series](#series-mathematics) $\sum_{n\geq1}x_n/b_n$ converges, then

$$
\frac1{b_n}\sum_{k=1}^nx_k\longrightarrow0.
$$

This follows from [summation by parts](analytic-number-theory.md#abel-s-summation-formula): write $x_k/b_k$ as a convergent series and average its tails with the increasing weights $b_k$.

#### Harmonic series

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_series)

The harmonic series diverges. Grouping terms from $2^k+1$ through $2^{k+1}$ gives at least $2^k/2^{k+1}=1/2$ from every block.

##### Alternating harmonic series

↑ **Parent:** [Harmonic series](#harmonic-series)

The alternating harmonic series $\sum_{n\geq1}(-1)^{n+1}/n$ converges. Its even partial sums increase, its odd partial sums decrease, and the two limits agree because their difference is the next term. In particular, every even partial sum is a lower bound and every odd partial sum is an upper bound for the limit.

This alternates the signs of the terms of the [harmonic series](#harmonic-series), which itself diverges.

#### Cauchy condensation test

↑ **Parent:** [Series (mathematics)](#series-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_condensation_test)

If $(a_n)$ is a nonnegative decreasing [sequence](#sequence), then $\sum_{n\geq1}a_n$ converges if and only if the condensed series $\sum_{k\geq0}2^ka_{2^k}$ converges. Comparing each dyadic block with its first and last terms proves both directions.

<h3 id="fekete-s-lemma">Fekete's lemma</h3>

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fekete's_lemma)

For a real [subadditive sequence](#subadditive-sequence) $(x_n)_{n\geq1}$, the normalized [sequence](#sequence) has the extended-real [limit of a sequence](#limit-of-a-sequence)

$$
\lim_{n\to\infty}\frac{x_n}{n}=\inf_{k\geq1}\frac{x_k}{k}\in[-\infty,\infty).
$$

No lower-bound hypothesis is needed for this conclusion. The [limit of a sequence](#limit-of-a-sequence) is finite precisely when the ratios are bounded below. The example $x_n=-n^2$ is a [subadditive sequence](#subadditive-sequence) with normalized [limit of a sequence](#limit-of-a-sequence) $-\infty$.

To prove the result, fix $k\geq1$ and, for $n\geq k$, write $n=qk+r$ with $q\geq1$ and $0\leq r<k$. Iterating [subadditivity](#subadditive-sequence) gives $x_n\leq qx_k+C_k$, where $C_k=\max(0,x_1,\ldots,x_{k-1})$ and $C_1=0$. Hence $\limsup_n x_n/n\leq x_k/k$ for every $k$. Every ratio is at least their [infimum](#infimum). If that [infimum](#infimum) is finite these bounds identify the [limit of a sequence](#limit-of-a-sequence); if it is $-\infty$, choosing $k$ with an arbitrarily negative ratio gives convergence to $-\infty$.

### Bolzano-Weierstrass theorem

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bolzano-Weierstrass_theorem)

Every bounded real sequence has a convergent subsequence. One proof repeatedly bisects a closed interval containing infinitely many terms, chooses a nested half containing infinitely many terms, and then chooses indices increasingly from those halves. Their interval diameters tend to zero, so completeness gives convergence.

#### Extended real subsequence theorem

↑ **Parent:** [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem)

Every real [sequence](#sequence) has a [subsequence](#subsequence) converging to an [extended real number](arithmetic.md#extended-real-number-line). A bounded sequence has a real convergent subsequence by the [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem). If it is unbounded above, every tail is unbounded above, so choose increasing indices $n_j$ with $a_{n_j}>j$. These terms tend to positive infinity. If it is unbounded below, use $a_{n_j}<-j$.

#### Diagonal subsequence argument

↑ **Parent:** [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem)

A diagonal subsequence argument successively extracts nested subsequences that converge in the first, first two, and then first $k$ coordinates. Taking the $j$th term from the $j$th nested subsequence produces one subsequence that converges in every fixed coordinate.

#### Unique subsequential limit of a bounded sequence

↑ **Parent:** [Bolzano-Weierstrass theorem](#bolzano-weierstrass-theorem)

If a bounded real sequence has the property that every convergent subsequence converges to the same number $L$, then the full sequence converges to $L$. Otherwise, a subsequence stays at least some fixed distance from $L$; Bolzano--Weierstrass gives it a convergent subsubsequence, contradicting the assumed uniqueness.

### Convergent sequence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convergent_sequence)

#### Bounded sequence with vanishing increments need not converge

↑ **Parent:** [Convergent sequence](#convergent-sequence)

The [sequence](#sequence) is bounded and $|a_{n+1}-a_n|\le\sqrt{n+1}-\sqrt n\to0$ by the [mean value theorem](calculus.md#mean-value-theorem). Nevertheless, along the integer parts of $(\pi/2+2\pi j)^2$ its terms tend to one, and along the integer parts of $(3\pi/2+2\pi j)^2$ they tend to minus one. The [square root](algebra.md#square-root) rounding error is $O(1/j)$. Thus a [bounded sequence](#bounded-sequence) with vanishing successive increments need not be a [convergent sequence](#convergent-sequence).

#### Limit of a sequence

↑ **Parent:** [Convergent sequence](#convergent-sequence)

A real [sequence](#sequence) $(x_n)$ has [limit of a sequence](#limit-of-a-sequence) $L\in\mathbb R$ when for every $\varepsilon>0$ there is $N$ such that $|x_n-L|<\varepsilon$ for all $n\geq N$. Its [limit of a sequence](#limit-of-a-sequence) is unique. Extended-real convergence to $-\infty$ means that every real upper bound eventually exceeds all the terms; convergence to $+\infty$ is the corresponding lower-bound condition. The [extended-real Fekete lemma](#fekete-s-lemma) is an example where the [limit of a sequence](#limit-of-a-sequence) need not be finite.

##### Reciprocal limits and escape in absolute value

↑ **Parent:** [Limit of a sequence](#limit-of-a-sequence)

For a real [sequence](#sequence) with no zero terms, the displayed equivalence follows directly by comparing $|1/a_n|$ with $1/M$. Escape to positive infinity implies reciprocal convergence to zero, but the converse does not retain the sign: $a_n=-n$ is a counterexample. If $a_n\to a\ne0$, eventually $|a_n|>|a|/2$, and $|1/a_n-1/a|\le2|a_n-a|/|a|^2$. This proves reciprocal convergence at a nonzero finite [limit of a sequence](#limit-of-a-sequence).

#### Cesaro mean

↑ **Parent:** [Convergent sequence](#convergent-sequence)

The Cesaro mean of the first $n$ terms of a sequence is their arithmetic average. If $a_n\to L$, then its Cesaro means also tend to $L$.

##### Cesaro theorem for convergent sequences

↑ **Parent:** [Cesaro mean](#cesaro-mean)

If a [sequence](#sequence) converges, its [Cesaro means](#cesaro-mean) have the same limit. Given a small tolerance, split the average error into a fixed finite initial segment and a tail whose individual errors are below that tolerance. The first contribution is a fixed constant divided by $n$, while the second is bounded by the tolerance. The converse fails: the alternating [sequence](#sequence) $(-1)^n$ has means tending to zero while its terms do not converge.

#### Geometric mean of a sequence

↑ **Parent:** [Convergent sequence](#convergent-sequence)

For a positive sequence converging to $L\geq0$, its cumulative geometric means converge to the same limit.

#### Monotone bounded sequence

↑ **Parent:** [Convergent sequence](#convergent-sequence)

An increasing real sequence converges exactly when it is bounded above. For a bounded sequence, its limit is the supremum of its set of terms.

### Fibonacci number

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fibonacci_number)

The Fibonacci numbers satisfy $F_0=0$, $F_1=1$, and $F_{n+1}=F_n+F_{n-1}$.

#### Fibonacci recurrence matrix modulo an integer

↑ **Parent:** [Fibonacci number](#fibonacci-number)

The vector $(F_{n+1},F_n)^T$ advances by multiplication by $A$. Matrix powers therefore prove modular recurrence identities uniformly in $n$. Explicitly, $A^3\equiv I\pmod2$, $A^8\equiv I\pmod3$, and $A^5\equiv3I\pmod5$. The last congruence gives $F_{n+5}\equiv3F_n\pmod5$, hence $5\mid F_{5j}$ for every nonnegative $j$.

#### Fibonacci addition formula

↑ **Parent:** [Fibonacci number](#fibonacci-number)

With the standard [Fibonacci numbers](#fibonacci-number) $F_0=0$, $F_1=1$, this identity holds for $n\ge0$, $k\ge1$. At $k=1$ it is immediate. If it holds for $k$ at every $n$, apply it at $n+1$ and use $F_{n+2}=F_{n+1}+F_n$ to obtain $F_{n+k+1}=F_{k+1}F_{n+1}+F_kF_n$, proving the assertion by [mathematical induction](foundations-of-mathematics.md#mathematical-induction). Taking $k=n$ gives $F_{2n}=F_n(F_{n+1}+F_{n-1})$ for $n\ge1$, linking the doubling formula to the [Lucas numbers](#lucas-number).

##### Fibonacci gcd reduction

↑ **Parent:** [Fibonacci addition formula](#fibonacci-addition-formula)

Consecutive [Fibonacci numbers](#fibonacci-number) are [coprime](number-theory.md#coprime-integers) by the [Euclidean algorithm](number-theory.md#euclidean-algorithm). The [Fibonacci addition formula](#fibonacci-addition-formula) writes $F_m=F_{m-n}F_{n+1}+F_{m-n-1}F_n$ for $m>n$. Taking the [greatest common divisor](number-theory.md#greatest-common-divisor) with $F_n$ removes the last summand, and multiplication by the [coprime](number-theory.md#coprime-integers) factor $F_{n+1}$ leaves that gcd unchanged. The case $m=n$ uses $F_0=0$. Applying the [Euclidean algorithm](number-theory.md#euclidean-algorithm) to the indices yields the strong-divisibility identity $\gcd(F_m,F_n)=F_{\gcd(m,n)}$ for nonnegative indices, with the usual zero conventions.

#### Binet formula

↑ **Parent:** [Fibonacci number](#fibonacci-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binet_formula)

For $\phi=(1+\sqrt5)/2$ and $\psi=(1-\sqrt5)/2$, the Fibonacci numbers satisfy

$$
F_n=\frac{\phi^n-\psi^n}{\sqrt5}.
$$

#### Fibonacci determinant identity

↑ **Parent:** [Fibonacci number](#fibonacci-number)

For nonnegative $n,m,l$,

$$
F_{n+l}F_{n+m}-F_nF_{n+m+l}
=(-1)^nF_mF_l.
$$

Cassini's identity is the adjacent-index special case.

### Pointwise convergence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pointwise_convergence)

#### Factorial cosine iterated limit detects rationality

↑ **Parent:** [Pointwise convergence](#pointwise-convergence)

For fixed $m$, the inner [limit](calculus.md#limit-of-a-function) is one precisely when $m!x$ is an [integer](number-theory.md#integer), and zero otherwise, because $|\cos(\pi y)|=1$ exactly at integers and powers of a number with modulus below one tend to zero. If $x=p/q$ is a [rational number](number-theory.md#rational-number), $q$ divides $m!$ for every $m\geq q$, making the inner limit eventually one. If $x$ is an [irrational number](algebra.md#irrational-number), multiplication by a nonzero integer cannot make it integral, making every inner limit zero. The order of the two limits is essential to this argument.

#### Shrinking continuous spikes with vanishing integral

↑ **Parent:** [Pointwise convergence](#pointwise-convergence)

For $n\ge2$, these [continuous functions](calculus.md#continuous-function) on $[0,1]$ have maximum one and integral $1/n^2$. Their supports shrink towards zero while their value at zero remains zero. They converge pointwise to zero and their integrals converge to zero, but their convergence is not [uniform convergence](#uniform-convergence). Thus convergence of integrals and continuity of the pointwise limit do not imply [uniform convergence](#uniform-convergence).

#### Pointwise limit

↑ **Parent:** [Pointwise convergence](#pointwise-convergence)

A pointwise limit assigns to each point the limit of the sequence of function values there. The convergence rate may depend on that point. [Uniform convergence](#uniform-convergence) additionally bounds the error simultaneously over the whole domain.

### Power series

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power_series)

#### Generating function

↑ **Parent:** [Power series](#power-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generating_function)

A [generating function](#generating-function) encodes a [sequence](#sequence) as a [series](#series-mathematics), whose coefficients or prescribed weighted coefficients recover the [sequence](#sequence). An [ordinary generating function](commutative-algebra.md#ordinary-generating-function) uses the [power series](#power-series) $A(x)=\sum_{n\geq0}a_nx^n$; an [exponential generating function](#exponential-generating-function) uses $\sum_{n\geq0}a_nx^n/n!$. A [Dirichlet series](analytic-number-theory.md#dirichlet-series) $\sum_{n\geq1}a_nn^{-s}$ gives another generating-function encoding. The displayed [power series](#power-series) is the ordinary specialization, rather than a restriction on all [generating functions](#generating-function). These encodings turn combinatorial splitting and concatenation rules into algebraic identities. A counting [generating function](#generating-function) is not necessarily a [probability generating function](probability-theory.md#probability-generating-function): its coefficients need not sum to one.

##### Exponential generating function

↑ **Parent:** [Generating function](#generating-function)

An exponential [generating function](#generating-function) encodes a [sequence](#sequence) using the displayed [factorial](combinatorics.md#factorial) denominators. It is especially useful for counting labelled combinatorial structures: taking an unordered set of structures with positive size corresponds to exponentiating their exponential generating function. The [rooted-tree generating function](combinatorics.md#rooted-tree-generating-function) illustrates this through $T=z e^T$.

#### Lacunary power series

↑ **Parent:** [Power series](#power-series)

A power series is lacunary when only a sparse sequence of powers has nonzero coefficients. For $\sum_jc_jz^{m_j}$ with strictly increasing integer exponents, the [radius of convergence](#radius-of-convergence) satisfies $R^{-1}=\limsup_j|c_j|^{1/m_j}$ by the [Cauchy-Hadamard theorem](#cauchy-hadamard-theorem). The exponent $m_j$, rather than the term index $j$, controls the coefficient root.

##### Factorial-gap power series

↑ **Parent:** [Lacunary power series](#lacunary-power-series)

This [lacunary power series](#lacunary-power-series) has [radius of convergence](#radius-of-convergence) one. For $|z|<1$, the inequality $n!\geq n$ for $n\geq1$ gives absolute convergence by a [geometric series](#geometric-series) comparison. For $|z|>1$ its terms do not tend to zero. At every point of the unit circle the terms have modulus one, so the [term test for divergence](#term-test-for-divergence) proves divergence there too. The two initial terms both equal $z$, since $0!=1!=1$; this finite repetition does not affect any convergence conclusion.

#### Binomial series

↑ **Parent:** [Power series](#power-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binomial_series)

For $|x|<1$, the binomial series is

$$
(1+x)^\alpha=\sum_{n=0}^{\infty}\binom{\alpha}{n}x^n,
\qquad
\binom{\alpha}{n}=\frac{\alpha(\alpha-1)\cdots(\alpha-n+1)}{n!}.
$$

##### Negative binomial series

↑ **Parent:** [Binomial series](#binomial-series)

For a nonnegative integer $L$ and $|z|<1$, this specialization of the [binomial series](#binomial-series) sums the normalizing coefficients of a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution).

#### Majorant series

↑ **Parent:** [Power series](#power-series)

A power series $g(x)=\sum_\alpha b_\alpha x^\alpha$ with nonnegative coefficients majorizes $f(x)=\sum_\alpha a_\alpha x^\alpha$ when $|a_\alpha|\leq b_\alpha$ for every [multi-index](distribution-theory.md#multi-index-notation) $\alpha$. Coefficientwise majorization turns estimates for an analytic equation into estimates for a simpler positive-coefficient equation.

#### Radius of convergence

↑ **Parent:** [Power series](#power-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radius_of_convergence)

##### Bounded power-series terms force interior absolute convergence

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

If the terms of a [power series](#power-series) at a nonzero point $z$ are bounded by $M$, then $|a_nw^n|\le M(|w|/|z|)^n$. A convergent [geometric series](#geometric-series) and the [comparison test for series](#comparison-test-for-series) give [absolute convergence](#absolute-convergence) at every point strictly inside that circle. Consequently terms at every point outside the [radius of convergence](#radius-of-convergence) must be unbounded. This conclusion is stronger than merely saying that those terms fail to tend to zero.

##### Sum of power series with unequal radii of convergence

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

Inside both convergence discs, the [triangle inequality](topological-analysis.md#triangle-inequality) gives [absolute convergence](#absolute-convergence) of the sum. Suppose $R<S$ and the sum had radius $T>R$. At any modulus between $R$ and $\min(T,S)$, subtracting the absolutely convergent second series from the absolutely convergent sum would give [absolute convergence](#absolute-convergence) of the first series outside its [radius of convergence](#radius-of-convergence), a contradiction. Interchanging the two series covers $S<R$.

##### Terms of a power series are unbounded outside its convergence disc

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

Let a [power series](#power-series) $\sum_{n\geq0}a_nz^n$ have finite [radius of convergence](#radius-of-convergence) $R$. If its terms were bounded in [complex modulus](complex-analysis.md#complex-modulus) at a point $z$ with $|z|>R$, say $|a_nz^n|\leq M$, choose $w$ with $R<|w|<|z|$. Then

$$
|a_nw^n|\leq M\left(\frac{|w|}{|z|}\right)^n.
$$

The [comparison test for series](#comparison-test-for-series) with a convergent [geometric series](#geometric-series) would give [absolute convergence](#absolute-convergence) at $w$, contradicting its position outside the convergence disc. Hence the terms are unbounded at every such $z$. The argument also works when $R=0$ and gives a stronger obstruction than the usual [term test for divergence](#term-test-for-divergence).

##### Radius of convergence of a sparse power series

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

For a series $\sum_n a_n x^{m_n}$ with distinct increasing integer exponents, define the ordinary coefficients to be $a_n$ at $m_n$ and zero elsewhere. The [Cauchy-Hadamard theorem](#cauchy-hadamard-theorem) then gives

$$
R^{-1}=\limsup_n|a_n|^{1/m_n}.
$$

The exponent in the root is the actual degree $m_n$, not the index $n$. For $a_n=(n!)^2$ and $m_n=n^2$, $0\leq2\log(n!)/n^2\leq2\log n/n\to0$, so $R=1$. Boundary behavior is a separate question.

##### Polynomial-coefficient power series

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

For a nonzero polynomial $p$, the [power series](#power-series) $\sum_{n\geq0}p(n)z^n$ has [radius of convergence](#radius-of-convergence) $1$. If $p$ has degree $d$ and leading coefficient $c\ne0$, then $p(n)\sim cn^d$ and $|p(n+1)/p(n)|\to1$, so the [ratio test](#ratio-test) applies inside the unit disk. At every point of its boundary, the terms fail to tend to zero. The zero polynomial is the exceptional case with [radius of convergence](#radius-of-convergence) $\infty$.

##### Polynomial coefficient growth with unit power-series radius

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

Suppose real coefficients satisfy $c\le a_n\le C(1+n)^m$ for all sufficiently large $n$, where $c,C>0$ and $m\ge0$. Then the [power series](#power-series) $\sum a_nz^n$ has [radius of convergence](#radius-of-convergence) one. For $|z|<1$, the [comparison test for series](#comparison-test-for-series) and the [ratio test](#ratio-test) dominate it by a polynomial times a geometric sequence. For $|z|\ge1$, the terms have [modulus](complex-analysis.md#modulus) at least $c$ eventually and violate the [term test for divergence](#term-test-for-divergence). Finite changes to the coefficients do not affect the conclusion.

##### Cauchy-Hadamard theorem

↑ **Parent:** [Radius of convergence](#radius-of-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy–Hadamard_theorem)

For $\sum a_nz^n$,

$$
\frac1R=\limsup_{n\to\infty}|a_n|^{1/n},
$$

with the usual conventions for zero and infinity.

##### Radius of convergence after powering coefficients

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

If $L=\limsup a_n^{1/n}$ for positive coefficients, then the coefficients $a_n^2$ have root limsup $L^2$. Coefficients $a_n^{a_n}$ instead have root terms

$$
a_n^{a_n/n}=\exp\left(\frac{a_n\log a_n}{n}\right),
$$

so their radius depends on the growth of $a_n\log a_n$ relative to $n$.

##### Half-plane of convergence of an exponential power series

↑ **Parent:** [Radius of convergence](#radius-of-convergence)

If the ordinary power series $\sum_{n\geq0}b_nw^n$ has radius $R\in(0,\infty)$, then

$$
\sum_{n\geq0}b_ne^{nz}
$$

converges for $\operatorname{Re}z<\log R$ and diverges for $\operatorname{Re}z>\log R$. Behavior on the boundary depends on the coefficients.

#### Cauchy product

↑ **Parent:** [Power series](#power-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_product)

The Cauchy product has coefficients $c_n=\sum_{k=0}^na_kb_{n-k}$. Absolute convergence permits regrouping and makes its sum the product of the two sums.

#### Termwise differentiation of a power series

↑ **Parent:** [Power series](#power-series)

Inside its radius of convergence, a power series may be differentiated term by term, and the differentiated series has the same radius.

#### Leading Taylor term

↑ **Parent:** [Power series](#power-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leading_Taylor_term)

The first nonzero Taylor term controls a holomorphic function’s local magnitude and angular sign pattern.

### Uniform convergence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_convergence)

A sequence of functions $f_n:X\to Y$ converges uniformly when one index $N$ makes $f_n(x)$ close to the limit simultaneously for every $x\in X$.

#### Uniformly vanishing functions can retain a nonzero integral

↑ **Parent:** [Uniform convergence](#uniform-convergence)

On the half-line, $\sup f_n=1/(en)\to0$, but $\int_0^\infty f_n=1$. The change of variable $x=ny$ shows why: the decreasing amplitude is spread over an increasing interval. [Uniform convergence](#uniform-convergence) controls integrals on finite-measure domains; it does not alone control total mass on an infinite-measure domain.

#### Uniform convergence preserves integrals on a compact interval

↑ **Parent:** [Uniform convergence](#uniform-convergence)

For [Riemann integrable](#riemann-integrable-function) functions on a fixed compact interval, [uniform convergence](#uniform-convergence) implies convergence of their [integrals](calculus.md#integral) by the displayed estimate. It need not imply convergence of [derivatives](calculus.md#derivative): $f_n(x)=\sin(n^2x)/n$ converges uniformly to zero on $[-1,1]$, while $f_n'(0)=n$.

#### Uniform convergence at moving evaluation points

↑ **Parent:** [Uniform convergence](#uniform-convergence)

If continuous $f_n$ converge uniformly to $f$ on a domain and $x_n\to x$ within it, the uniform limit is continuous and $|f_n(x_n)-f(x)|\le\|f_n-f\|_\infty+|f(x_n)-f(x)|\to0$. Uniform convergence supplies control at changing points that pointwise convergence does not.

#### Uniform derivative convergence with an anchored value

↑ **Parent:** [Uniform convergence](#uniform-convergence)

If continuously differentiable functions have uniformly convergent [derivatives](calculus.md#derivative) on an interval and their values converge at one point, the functions converge locally uniformly to a continuously differentiable limit whose [derivative](calculus.md#derivative) is the [derivative](calculus.md#derivative) limit. The proof integrates from the anchored point using the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus). [Uniform convergence](#uniform-convergence) of the functions on the entire interval follows when the interval is bounded; it need not follow on an unbounded interval.

<h4 id="egorov-s-theorem">Egorov's theorem</h4>

↑ **Parent:** [Uniform convergence](#uniform-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Egorov's_theorem)

On a finite-measure measurable [set](set.md), a [sequence](#sequence) of [measurable functions](measure-theory.md#measurable-function) converging pointwise almost everywhere converges uniformly outside a [set](set.md) of arbitrarily small measure. For tolerance $1/k$, the [sets](set.md) on which every index after $N$ has error at most $1/k$ increase to full measure as $N\to\infty$. Choose $N_k$ with exceptional measure at most $\varepsilon2^{-k-1}$ and intersect the good [sets](set.md). [Countable subadditivity](measure-theory.md#countable-subadditivity-of-a-measure) bounds the discarded measure, and the resulting tail estimates prove [uniform convergence](#uniform-convergence). Finite measure is essential: $\mathbf1_{[n,\infty)}$ on $[0,\infty)$ is a counterexample.

#### Uniform limit theorem

↑ **Parent:** [Uniform convergence](#uniform-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_limit_theorem)

A [uniform limit](#uniform-limit) of [continuous functions](calculus.md#continuous-function) is continuous.

<h4 id="dini-s-theorem">Dini's theorem</h4>

↑ **Parent:** [Uniform convergence](#uniform-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dini's_theorem)

Dini's theorem says that a monotone sequence of continuous real-valued functions on a compact space that converges pointwise to a continuous function converges uniformly.

#### Uniformly Cauchy sequence

↑ **Parent:** [Uniform convergence](#uniform-convergence)

A sequence of functions is uniformly Cauchy when, for every $\varepsilon>0$, all sufficiently late pairs satisfy

$$
\sup_x d(f_n(x),f_m(x))<\varepsilon.
$$

#### Locally uniform convergence

↑ **Parent:** [Uniform convergence](#uniform-convergence)

A sequence $f_n:X\to Y$ converges locally uniformly to $f$ when every point has a neighbourhood on which the convergence is uniform.

##### Compact-open topology

↑ **Parent:** [Locally uniform convergence](#locally-uniform-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact-open_topology)

The compact-open topology on a space of functions is generated by uniform control on compact subsets. For scalar-valued functions, its basic seminorms are $f\mapsto\sup_{x\in K}|f(x)|$ as $K$ ranges over compact subsets of the domain.

###### Weighted metric for local uniform convergence

↑ **Parent:** [Compact-open topology](#compact-open-topology)

For a compact exhaustion $K_n$ and positive summable weights $w_n$, use the [bounded metric transform](topological-analysis.md#bounded-metric-transform) $\phi(s)=s/(1+s)$ on each compact [supremum norm](functional-analysis.md#supremum-norm). The resulting series defines a [metric](topological-analysis.md#metric) on continuous functions and realizes [local uniform convergence on compact subsets](#local-uniform-convergence-on-compact-subsets). The triangle inequality is termwise. For convergence, control finitely many compact seminorms and then the uniformly bounded weight tail; conversely a vanishing metric controls each fixed seminorm.

##### Local uniform convergence on compact subsets

↑ **Parent:** [Locally uniform convergence](#locally-uniform-convergence)

A locally uniform limit of continuous real-valued functions is continuous. Moreover, local uniform convergence is uniform on every compact subset: choose finitely many neighbourhoods from the local uniformity cover and take the largest of their convergence indices.

### Geometric series

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_series)

#### Iterated contraction gives a summable orbit

↑ **Parent:** [Geometric series](#geometric-series)

If a map on a [normed vector space](functional-analysis.md#normed-vector-space) satisfies $\|T(x)\|\le q\|x\|$ for every $x$, with $0\le q<1$, induction gives $\|T^n(x)\|\le q^n\|x\|$. The [geometric series](#geometric-series) then proves [absolute convergence](#absolute-convergence) of its orbit series whenever the ambient [normed vector space](functional-analysis.md#normed-vector-space) is complete. The scalar map $T(x)=\sin(qx)$ satisfies the bound because $|\sin u|\le|u|$.

#### Finite geometric series

↑ **Parent:** [Geometric series](#geometric-series)

For $r\ne1$, a finite geometric series satisfies

$$
\sum_{j=m}^n r^j=r^m\frac{1-r^{n-m+1}}{1-r}.
$$

##### Finite trigonometric sum

↑ **Parent:** [Finite geometric series](#finite-geometric-series)

Taking the real and imaginary parts of the [finite geometric series](#finite-geometric-series) $\sum_{m=1}^N e^{im\theta}$ yields

$$
\sum_{m=1}^N\cos(m\theta)=\frac{\sin(N\theta/2)\cos((N+1)\theta/2)}{\sin(\theta/2)},\qquad\sum_{m=1}^N\sin(m\theta)=\frac{\sin(N\theta/2)\sin((N+1)\theta/2)}{\sin(\theta/2)}.
$$

These formulas apply when $\theta\notin2\pi\mathbb Z$. At multiples of $2\pi$, the sums are directly $N$ and $0$. Complex exponentials turn two real trigonometric summations into one [finite geometric series](#finite-geometric-series).

##### Exponential geometric sum bound

↑ **Parent:** [Finite geometric series](#finite-geometric-series)

For an interval $I$ of $L$ consecutive integers and $e(x)=e^{2\pi ix}$,

$$
\left|\sum_{n\in I}e(\beta n)\right|
\ll\min(L,\|\beta\|^{-1}),
$$

where $\|\beta\|$ is the distance to the nearest integer. This follows from the finite geometric-series formula and $|1-e(\beta)|\asymp\|\beta\|$.

### Cauchy sequence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_sequence)

A sequence is Cauchy when its terms become arbitrarily close to one another beyond some index.

#### Convergence from arbitrary variable-lag increments

↑ **Parent:** [Cauchy sequence](#cauchy-sequence)

A real [sequence](#sequence) converges if and only if the displayed condition holds. A [Cauchy sequence](#cauchy-sequence) makes all future differences uniformly small, so the forward implication is immediate. Conversely, failure of the [Cauchy sequence](#cauchy-sequence) criterion produces a fixed tolerance and, for each $n$, a future term differing from $a_n$ by at least half that tolerance. Choosing the least such positive lag defines one function that contradicts the displayed condition. The [completeness of the real numbers](#completeness-of-the-real-numbers) then gives convergence. Testing only every fixed integer lag is weaker: $a_n=\log n$ passes those tests but diverges.

#### Cauchy subsequence

↑ **Parent:** [Cauchy sequence](#cauchy-sequence)

A Cauchy subsequence is a subsequence that is a [Cauchy sequence](#cauchy-sequence). Every convergent subsequence is Cauchy.

#### Completeness of the real numbers

↑ **Parent:** [Cauchy sequence](#cauchy-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Completeness_of_the_real_numbers)

Every Cauchy sequence of real numbers converges to a real number.

##### Least-upper-bound property

↑ **Parent:** [Completeness of the real numbers](#completeness-of-the-real-numbers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Least-upper-bound_property)

The least-upper-bound property states that every nonempty set of [real numbers](arithmetic.md#real-number) that has an [upper bound](set.md#upper-bound-in-a-partially-ordered-set) has a [supremum](#supremum) in the real numbers. It is an order-theoretic formulation of the [completeness of the real numbers](#completeness-of-the-real-numbers).

### Conditional convergence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_convergence)

A series is conditionally convergent when it converges but does not converge absolutely.

#### Riemann series theorem

↑ **Parent:** [Conditional convergence](#conditional-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_series_theorem)

A conditionally convergent real [series](#series-mathematics) can be rearranged to converge to any prescribed real value or to diverge. Its positive and negative subseries have infinite total magnitudes: successively add positive terms to cross a desired value and negative terms to cross back. Since the terms tend to zero, the overshoots shrink to zero.

##### Rearrangement of a series

↑ **Parent:** [Riemann series theorem](#riemann-series-theorem)

A rearrangement changes the order of a series without changing its multiset of terms. A conditionally convergent real series can be rearranged to approach any prescribed real limit or to diverge.

The [Riemann series theorem](#riemann-series-theorem) specifies the possible sums of rearrangements of a conditionally convergent real series.

#### Alternating series test

↑ **Parent:** [Conditional convergence](#conditional-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alternating_series_test)

If $a_n\geq0$ decreases to zero, then $\sum_{n=1}^{\infty}(-1)^na_n$ converges.

### P-series

↑ **Parent:** [Sequence and series](#sequence-and-series)

The series $\sum_{n=1}^{\infty}n^{-p}$ converges exactly when $p>1$.

### Absolute convergence

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolute_convergence)

A series converges absolutely when the series of absolute values converges; absolute convergence implies convergence.

#### Squares of a summable positive sequence

↑ **Parent:** [Absolute convergence](#absolute-convergence)

If $a_n\geq0$ and $\sum a_n<\infty$, then $a_n\to0$, so eventually $a_n^2\leq a_n$ and $\sum a_n^2$ converges.

#### Geometric means of two summable positive sequences

↑ **Parent:** [Absolute convergence](#absolute-convergence)

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\sum_n\sqrt{a_nb_n}
\leq\left(\sum_na_n\right)^{1/2}
\left(\sum_nb_n\right)^{1/2}.
$$

#### Weighted square roots of a summable sequence

↑ **Parent:** [Absolute convergence](#absolute-convergence)

If $a_n\geq0$, $\sum a_n<\infty$, and $p>1/2$, then

$$
\sum_n\sqrt{a_n}\,n^{-p}
\leq\left(\sum_na_n\right)^{1/2}
\left(\sum_nn^{-2p}\right)^{1/2}<\infty.
$$

The endpoint can fail: $a_n=1/(n(\log n)^2)$ gives the divergent series $\sum1/(n\log n)$.

### Total variation

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_variation)

The total variation of a sequence is $\sum_n|a_{n+1}-a_n|$; convergence alone does not make it finite.

#### Total generalized variation

↑ **Parent:** [Total variation](#total-variation)

Second-order total generalized variation combines a first derivative with an auxiliary vector field and its symmetric derivative. A standard continuous form is

$$
\operatorname{TGV}_{\alpha}^{2}(u)=\inf_w\{\alpha_1\|Du-w\|_{\mathcal M}+\alpha_0\|Ew\|_{\mathcal M}\},\qquad\alpha_0,\alpha_1>0.
$$

Here $Ew$ denotes the symmetric distributional derivative and the norms are total variations of the corresponding measures. Discrete variants replace these operators by linear maps and use sums of row norms. Unlike first-order [total variation](#total-variation), this regularizer accommodates piecewise-affine behavior. A [TGV divergence splitting](#tgv-divergence-splitting) makes its constrained divergence dual amenable to explicit [proximal operators](convex-optimization.md#proximal-operator).

##### TGV divergence splitting

↑ **Parent:** [Total generalized variation](#total-generalized-variation)

For a quadratic data term and divergence maps $A_1,A_2$, the dual constraint $A_1v\in D$ can be split through $\delta_D(A_1v)=\sup_w[\langle w,A_1v\rangle-\delta_D^*(w)]$. For a product of Euclidean row balls of radius $\beta$, its [support function](mathematical-optimization.md#support-function) is $\delta_D^*(w)=\beta\sum_i\|w_i\|_2$. The resulting saddle coupling is $K(u,w)=A_2^*u-A_1^*w$. The [Chambolle–Pock algorithm](convex-optimization.md#chambolle-pock-algorithm) then uses a row-ball projection, a quadratic [proximal operator](convex-optimization.md#proximal-operator) and [radial soft thresholding](convex-optimization.md#radial-soft-thresholding), with no projection onto an intersection involving a divergence operator.

### Harmonic sum

↑ **Parent:** [Sequence and series](#sequence-and-series)

Harmonic sums satisfy $\sum_{j=n+1}^{2n}1/j\to\log2$ by integral comparison.

### Convergent series

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convergent_series)

A series converges when its sequence of partial sums converges to a finite limit.

#### Convergence from fixed-length series blocks

↑ **Parent:** [Convergent series](#convergent-series)

For a fixed positive [integer](number-theory.md#integer) $m$, if $a_n\to0$ and the [series](#series-mathematics) of the displayed block sums converges, then the original [series](#series-mathematics) converges to the same [limit of a sequence](#limit-of-a-sequence). Its [partial sum](#partial-sum) at a block endpoint is exactly a [partial sum](#partial-sum) of $\sum b_n$; the difference at an intermediate endpoint has at most $m-1$ terms, all tending to zero. This justification is essential when block cancellation proves convergence without [absolute convergence](#absolute-convergence). It does not apply without further control to blocks whose lengths grow.

#### Dirichlet test

↑ **Parent:** [Convergent series](#convergent-series)

If the partial sums of $\sum b_n$ are bounded and $a_n$ decreases to zero, then $\sum a_nb_n$ converges. The uniform version holds for functions $b_n(x)$ when their partial sums have one bound $M$ independent of $x$. Indeed partial sums starting at index $N$ have absolute value at most $2M$, and summation by parts bounds every weighted tail from $N$ to $K$ by $2Ma_N$. The [uniformly Cauchy sequence](#uniformly-cauchy-sequence) criterion proves [uniform convergence](#uniform-convergence). This justifies integrating a conditionally convergent [Fourier series](fourier-series.md) on intervals staying away from its endpoint jump.

#### Comparison test for series

↑ **Parent:** [Convergent series](#convergent-series)

For nonnegative sequences with $0\leq a_n\leq b_n$, convergence of $\sum_nb_n$ implies convergence of $\sum_na_n$, while divergence of $\sum_na_n$ implies divergence of $\sum_nb_n$.

##### Ratio comparison test

↑ **Parent:** [Comparison test for series](#comparison-test-for-series)

For positive [sequences](#sequence) $(a_n),(b_n)$, suppose $a_{n+1}/a_n\leq b_{n+1}/b_n$ eventually. Then $a_n/b_n$ is eventually nonincreasing, so $a_n\leq Cb_n$ beyond a fixed index. The [comparison test for series](#comparison-test-for-series) proves convergence of $\sum a_n$ whenever $\sum b_n$ converges. Reversing the ratio inequality gives an eventual lower bound $a_n\geq cb_n$ and hence divergence when the positive comparison [series](#series-mathematics) diverges. The initial finite set of terms does not affect either conclusion.

##### Clipping preserves divergence of a positive series

↑ **Parent:** [Comparison test for series](#comparison-test-for-series)

If $x_n>0$ and $c>0$, clipping every term at $c$ preserves divergence. If infinitely many terms are at least $c$, the clipped series has infinitely many terms equal to $c$ and diverges. Otherwise its tail agrees with the original series. This lemma is useful in proving convergence from minimum-decrement inequalities.

##### Integral test for convergence

↑ **Parent:** [Comparison test for series](#comparison-test-for-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_test_for_convergence)

If $f:[1,\infty)\to[0,\infty)$ is decreasing, then $\sum_{n\geq1}f(n)$ and $\int_1^\infty f(x)\,dx$ either both converge or both diverge. This follows by bounding the area under the graph between adjacent upper and lower rectangle sums.

#### Summable sequence

↑ **Parent:** [Convergent series](#convergent-series)

A sequence $(a_n)$ is summable when the [series](#series-mathematics) $\sum_na_n$ is [convergent](#convergent-series).

#### Limit comparison test

↑ **Parent:** [Convergent series](#convergent-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_comparison_test)

For positive terms, if the ratio of two sequences tends to a finite positive number, their series either both converge or both diverge.

#### Ratio test

↑ **Parent:** [Convergent series](#convergent-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ratio_test)

For nonzero terms, if

$$
\limsup_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|<1,
$$

then $\sum a_n$ converges absolutely. If the ratio has a limit greater than one, the terms do not tend to zero and the series diverges.

##### Power-law comparison from a refined ratio bound

↑ **Parent:** [Ratio test](#ratio-test)

Suppose $a_n>0$ and, for all sufficiently large $n$, $a_{n+1}/a_n\le1-c/n$ with fixed $c>0$. Choose an initial index $N>c$. Since $\log(1-x)\le-x$ for $0<x<1$, summing logarithmic ratios gives $\log(a_n/a_N)\le-c\sum_{k=N}^{n-1}1/k\le-c\log(n/N)$. Thus $a_n\le a_NN^c n^{-c}$. For $c>1$, the [comparison test for series](#comparison-test-for-series) with a [P-series](#p-series) proves convergence. This supplies a useful refinement when a limiting ratio of one makes the ordinary [ratio test](#ratio-test) inconclusive.

##### Ratio limit implies root limit

↑ **Parent:** [Ratio test](#ratio-test)

For a positive sequence, if $a_{n+1}/a_n\to L\geq0$, then

$$
a_n^{1/n}\to L.
$$

For $L>0$ this follows by taking logarithms and applying Cesàro averaging; the case $L=0$ follows from an eventual geometric upper bound.

##### Factorial-over-power series

↑ **Parent:** [Ratio test](#ratio-test)

For $a_n=n!/n^n$,

$$
\frac{a_{n+1}}{a_n}=\left(\frac n{n+1}\right)^n\to e^{-1}.
$$

Thus $\sum n!/n^n$ converges and $n/(n!)^{1/n}\to e$.

### Uniform limit

↑ **Parent:** [Sequence and series](#sequence-and-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_limit)

A sequence converges uniformly when one index makes the approximation accurate at every point of the domain.

## Calculus

↑ **Parent:** [Real analysis](real-analysis.md)

[This section is present in another page, follow this link to view it.](calculus.md)

## Riemann integration

↑ **Parent:** [Real analysis](real-analysis.md)

Riemann integration approximates area by upper and lower sums over finite partitions.

### Single-point changes preserve Riemann integrals

↑ **Parent:** [Riemann integration](#riemann-integration)

Changing the value of a bounded [Riemann-integrable function](#riemann-integrable-function) at one point preserves its [Riemann integral](#riemann-integral). The difference is supported at that point: partitions isolating it in intervals of arbitrarily small total length make both [Darboux sums](#darboux-sum) tend to zero. Thus a nonnegative single-point spike can have zero integral without vanishing everywhere. Its indefinite integral is identically zero, so the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) derivative identity can fail at the changed point despite differentiability of the primitive.

### Riemann-Stieltjes integral

↑ **Parent:** [Riemann integration](#riemann-integration)

For continuous $f$ and an integrator $g$ of [bounded variation](#total-variation-of-a-function), the Riemann-Stieltjes integral is the limit of tagged sums $\sum f(\xi_j)(g(t_{j+1})-g(t_j))$ as the mesh tends to zero. It exists and equals integration against the signed measure induced by $g$. Continuous vector-valued integrators are handled componentwise, which defines [path signatures](analysis.md#signature-of-a-bounded-variation-path) of continuous [bounded variation](#total-variation-of-a-function) paths.

### Quadrature error

↑ **Parent:** [Riemann integration](#riemann-integration)

The difference between a weighted integral and a discrete approximation is a quadrature error. For a [Hölder continuous function](sobolev-space.md#holder-condition) on a [partition of an interval](#partition-of-an-interval) with mesh $\Delta$, a left endpoint approximation has error of order $\Delta^\alpha$. For a normalized window [indicator function](measure-theory.md#indicator-function), only the two endpoint cells contribute and the error is bounded by a constant times $\Delta/h$.

### Partition of an interval

↑ **Parent:** [Riemann integration](#riemann-integration)

A partition of $[a,b]$ is a finite increasing sequence $a=t_0<t_1<\cdots<t_n=b$. Its mesh is $\max_i(t_i-t_{i-1})$, and a sequence of partitions is refining when each partition contains the preceding one.

#### Partition refinement

↑ **Parent:** [Partition of an interval](#partition-of-an-interval)

A refinement of a finite interval partition inserts additional points without removing original points. The union of two partitions is a common refinement. Refinement makes each subinterval smaller, increasing its infimum and decreasing its supremum; this proves [Darboux sum refinement monotonicity](#darboux-sum-refinement-monotonicity).

#### Dyadic partition

↑ **Parent:** [Partition of an interval](#partition-of-an-interval)

A [dyadic partition](#dyadic-partition) of $[0,1]$ at level $J$ consists of $2^J$ equal cells of length $2^{-J}$. Each cell splits into two cells at the next level. Use left-closed, right-open cells, adding the endpoint $1$ to the final cell when a pointwise representative is needed. These nested partitions underlie the [Haar scaling functions](fourier-analysis.md#haar-scaling-function) and [Haar wavelets](fourier-analysis.md#haar-wavelet).

##### Dyadic interval

↑ **Parent:** [Dyadic partition](#dyadic-partition)

A [dyadic interval](#dyadic-interval) is one cell in a [dyadic partition](#dyadic-partition). Its children are the left and right half intervals. Disjoint [dyadic intervals](#dyadic-interval) at a fixed level produce orthogonal [indicator functions](measure-theory.md#indicator-function) and [independent](random-variable.md#independent-random-variables) [Brownian motion](brownian-motion.md) increments.

###### Alternating dyadic colouring excludes symmetric weighted pair sums

↑ **Parent:** [Dyadic interval](#dyadic-interval)

Define a [finite colouring](ramsey-theory.md#finite-coloring) of the positive [integers](number-theory.md#integer) by $c(n)=\lfloor\log_2 n\rfloor\pmod 2$. No increasing infinite [sequence](#sequence) has all the numbers $x_i+2x_j$, $i\ne j$, in one [colour class](ramsey-theory.md#colour-class).

Write $\delta(y)=2^{\lfloor\log_2 y\rfloor+1}-y$. If $\delta$ is unbounded on the [sequence](#sequence), fix a term $x$ and choose a later term $y>2x$ with $\delta(y)>2x$. With $L=2^{\lfloor\log_2 y\rfloor}$, the numbers $y+2x$ and $2y+x$ lie respectively in the adjacent [dyadic intervals](#dyadic-interval) $[L,2L)$ and $[2L,4L)$, so their colours differ. If $\delta$ is bounded by $D$ on the [sequence](#sequence), choose $x>2D$ and then $y>2x$. Now $y+2x=2L-\delta(y)+2x$ lies in $[2L,4L)$, whereas $2y+x=4L-2\delta(y)+x$ lies in $[4L,8L)$. Their colours again differ. The [finite colouring](ramsey-theory.md#finite-coloring) therefore excludes the symmetric weighted-pair configuration.

### Riemann sum

↑ **Parent:** [Riemann integration](#riemann-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_sum)

For a tagged partition $a=x_0<\cdots<x_n=b$ with $t_i\in[x_{i-1},x_i]$, the corresponding Riemann sum is

$$
\sum_{i=1}^n f(t_i)(x_i-x_{i-1}).
$$

Its limits over increasingly fine partitions define the [Riemann integral](#riemann-integral).

### Continuous approximation of a Riemann-integrable function

↑ **Parent:** [Riemann integration](#riemann-integration)

Every Riemann-integrable function on a compact interval can be approximated in $L^1$ by continuous functions. Consequently their integrals converge uniformly over all subintervals.

### Total variation of a function

↑ **Parent:** [Riemann integration](#riemann-integration)

The total variation of $f:[a,b]\to\mathbb R$ is

$$
V_a^b(f)=\sup_{a=t_0<\cdots<t_n=b}
\sum_{k=1}^n|f(t_k)-f(t_{k-1})|.
$$

The function has bounded variation when this quantity is finite.

#### p-variation of a path

↑ **Parent:** [Total variation of a function](#total-variation-of-a-function)

For $p\ge1$, the displayed quantity measures the accumulated oscillation of a path in a [metric space](topological-analysis.md#metric-space). For $p=1$ it is total variation. A [Hölder continuous](sobolev-space.md#holder-condition) path of exponent $\alpha$ has finite $p$-variation on a compact interval if $p\alpha\ge1$. Applying this construction to the [Carnot-Carathéodory distance](differential-geometry.md#carnot-caratheodory-distance) gives the defining regularity of a [weak geometric p-rough path](analysis.md#weak-geometric-p-rough-path).

#### Dyadic approximation of total variation

↑ **Parent:** [Total variation of a function](#total-variation-of-a-function)

For a [càdlàg function](calculus.md#cadlag), replace the last sampled value at $2^{-n}\lceil2^nt\rceil$ by $X_t$. Right continuity makes this change tend to zero. The corrected sum is bounded by the [total variation of a function](#total-variation-of-a-function). Conversely every finite [partition of an interval](#partition-of-an-interval) can be approximated by dyadic points from the right, retaining the endpoint $t$. The [triangle inequality](topological-analysis.md#triangle-inequality) bounds that partition's limiting sum by the dyadic sums. Taking the [supremum](#supremum) proves convergence, including the value $+\infty$.

#### Weak convergence of bounded-variation integrators

↑ **Parent:** [Total variation of a function](#total-variation-of-a-function)

If continuously differentiable $F_j,F$ converge uniformly on a [compact](topology.md#compact-space) interval and have uniformly bounded [total variation of a function](#total-variation-of-a-function), then $\int bF_j^{\prime}\to\int bF^{\prime}$ for every continuous $b$. For continuously differentiable test functions this is [integration by parts](calculus.md#integration-by-parts). Uniform approximation by [polynomials](polynomial.md) extends the conclusion to continuous tests using the variation bound.

#### Jordan decomposition of a function of bounded variation

↑ **Parent:** [Total variation of a function](#total-variation-of-a-function)

Every real function $f$ of [bounded variation](#total-variation-of-a-function) is the difference of two nondecreasing functions. Writing $V_f$ for its cumulative total variation, one may take

$$
f_+=\frac{V_f+f}{2},\qquad f_-=\frac{V_f-f}{2},
$$

up to constants chosen for the desired normalization.

### Riemann integral

↑ **Parent:** [Riemann integration](#riemann-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_integral)

#### Unbounded derivative obstruction to Riemann integrability

↑ **Parent:** [Riemann integral](#riemann-integral)

A proper [Riemann integral](#riemann-integral) on a compact interval requires a bounded integrand, but a [derivative](calculus.md#derivative) can be unbounded. For $f(x)=x^2\sin(1/x^2)$ away from zero and $f(0)=0$, the [difference quotient](calculus.md#difference-quotient) gives $f'(0)=0$, whereas $f'(x)=2x\sin(1/x^2)-2\cos(1/x^2)/x$ for $x\ne0$. At $x_n=(2\pi n)^{-1/2}$, this derivative is $-2/x_n$ and is unbounded. The [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) version that integrates a derivative therefore needs an explicit integrability hypothesis.

#### Weighted mean value theorem for integrals

↑ **Parent:** [Riemann integral](#riemann-integral)

For real [continuous functions](calculus.md#continuous-function) $f,g$ on a compact interval with $g\geq0$, some $\alpha$ in the interval satisfies $\int fg=f(\alpha)\int g$. If $\int g>0$, the weighted average lies between the minimum and maximum of $f$, and the [intermediate value theorem](calculus.md#intermediate-value-theorem) supplies $\alpha$. If $\int g=0$, the bound $|\int fg|\leq\sup|f|\int g$ makes both sides zero. Nonnegativity of the weight is essential to this argument.

#### Direct Riemann integrability

↑ **Parent:** [Riemann integral](#riemann-integral)

A function $g$ on $[0,\infty)$ is directly Riemann integrable when its upper and lower sums on an equal-width mesh are absolutely finite and converge to the same finite integral as the mesh width tends to zero. A locally absolutely continuous integrable function with integrable derivative has this property: the upper-minus-lower sum is bounded by mesh width times its total variation. The derivative bound therefore gives [bounded variation](#total-variation-of-a-function) as well as tail control. This stronger form of integrability is a hypothesis of the [key renewal theorem](probability-theory.md#key-renewal-theorem).

#### Improper integral

↑ **Parent:** [Riemann integral](#riemann-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Improper_integral)

An improper integral is defined by taking a [limit](calculus.md#limit-of-a-function) when an integration endpoint is infinite or the integrand is unbounded. Its convergence must be established before ordinary integral manipulations are applied.

##### Logarithmic divergence

↑ **Parent:** [Improper integral](#improper-integral)

A [logarithmic divergence](#logarithmic-divergence) grows like a [logarithm](calculus.md#logarithm) as a cutoff is removed. For example $\int_\epsilon^1dx/x=\log(1/\epsilon)\to\infty$ as $\epsilon\to0^+$. An integrand $f(x)=C/x+O(1)$ near zero gives $C\log(1/\epsilon)+O(1)$. This behavior distinguishes logarithmic sensitivity to an infrared or ultraviolet cutoff from power-law divergence.

##### Improper power integral

↑ **Parent:** [Improper integral](#improper-integral)

The [improper integral](#improper-integral) $\int_1^\infty u^{-p}\,du$ converges exactly when $p>1$, in which case its value is $1/(p-1)$.

#### Monotonicity of the Riemann integral

↑ **Parent:** [Riemann integral](#riemann-integral)

If Riemann-integrable functions satisfy $f(x)\leq g(x)$ throughout $[a,b]$, then

$$
\int_a^bf(x)\,dx\leq\int_a^bg(x)\,dx.
$$

This follows directly by comparing their lower and upper Darboux sums, or their Riemann sums on a common sequence of refining partitions.

### Riemann integrability criterion

↑ **Parent:** [Riemann integration](#riemann-integration)

A bounded function is Riemann integrable exactly when for every $\varepsilon>0$ some partition $P$ satisfies $U(f,P)-L(f,P)<\varepsilon$.

#### Pointwise supremum need not preserve Riemann integrability

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

Enumerate the rational points of a compact nondegenerate interval as $q_1,q_2,\ldots$. Each singleton [indicator function](measure-theory.md#indicator-function) $f_n=1_{\{q_n\}}$ is [Riemann integrable](#riemann-integrable-function) with integral zero. Their pointwise supremum is the [Dirichlet function](#dirichlet-function), which is not [Riemann integrable](#riemann-integrable-function). Thus even a uniformly bounded countable supremum need not preserve integrability.

#### Dirichlet function

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_function)

The indicator of the [rational numbers](number-theory.md#rational-number) is not [Riemann integrable](#riemann-integrable-function) on a nondegenerate interval: every subinterval contains both rational and irrational points, so its lower sum is zero and its upper sum is the interval length.

#### Riemann integrability is closed under addition and maximum

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

For a common interval partition, the [oscillation of a function on an interval](#oscillation-of-a-function-on-an-interval) satisfies $\operatorname{osc}_I(f+g)\le\operatorname{osc}_I f+\operatorname{osc}_I g$. Refining two good [Darboux sums](#darboux-sum) therefore proves integrability of the sum. [Lipschitz composition preserves Riemann integrability](#lipschitz-composition-preserves-riemann-integrability), so absolute values preserve it too. The identity $\max(f,g)=(f+g+|f-g|)/2$ then proves the assertion for the maximum.

#### Bounded functions continuous away from one endpoint are Riemann integrable

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

Let $f$ be bounded on $[a,b]$ and continuous on $(a,b]$. For any positive error tolerance, isolate $[a,a+\delta]$. Its contribution to the difference of [upper Darboux sums](#upper-darboux-sum) and [lower Darboux sums](#lower-darboux-sum) is at most $2\|f\|_\infty\delta$. On $[a+\delta,b]$, [uniform continuity](topological-analysis.md#uniform-continuity) supplies a [partition of an interval](#partition-of-an-interval) with arbitrarily small remaining oscillation sum. The [Riemann integrability criterion](#riemann-integrability-criterion) then proves integrability, even when the values oscillate without a limit at the endpoint.

#### Indicator of a restricted-digit decimal set

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

Let $K$ consist of numbers whose decimal digits all lie in a fixed set $D\subseteq\{1,\ldots,8\}$ with $m<10$ digits. The $m^N$ allowed prefixes give closed decimal intervals of length $10^{-N}$ covering $K$, with no endpoints in $K$. A [partition of an interval](#partition-of-an-interval) at those endpoints gives an [upper Darboux sum](#upper-darboux-sum) at most $(m/10)^N$. Every cell contains a terminating decimal outside $K$, so the [lower Darboux sum](#lower-darboux-sum) is zero. Thus the [indicator function](measure-theory.md#indicator-function) is [Riemann integrable](#riemann-integrable-function) with [Riemann integral](#riemann-integral) zero. Such sets illustrate how an uncountable set may have an integrable [indicator function](measure-theory.md#indicator-function) of zero integral.

#### Riemann integrability from almost full interval coverage

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

Let $|f|\le M$ on $[0,1]$. Suppose finitely many nonoverlapping closed intervals, of total length at least $1-\delta$, can be chosen for each $\delta>0$, with $f$ [Riemann integrable](#riemann-integrable-function) on each. Refine the intervals to make their total [Darboux sum](#darboux-sum) gap less than $\varepsilon/2$. The remaining length contributes at most $2M\delta$. Taking $\delta<\varepsilon/(4M)$ proves global [Riemann integrability](#riemann-integrable-function) by the [Riemann integrability criterion](#riemann-integrability-criterion).

#### Lipschitz composition preserves Riemann integrability

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

If $f$ is [Riemann integrable](#riemann-integrable-function) and $g$ is Lipschitz on an interval containing the range of $f$, then $g\circ f$ is [Riemann integrable](#riemann-integrable-function). With Lipschitz constant $K$, the oscillation on each partition cell satisfies $\operatorname{osc}(g\circ f)\leq K\operatorname{osc}(f)$, and hence the gap between [Darboux sums](#darboux-sum) is multiplied by at most $K$. A continuously differentiable $g$ is Lipschitz on each closed bounded interval by the [mean value theorem](calculus.md#mean-value-theorem) and the [extreme value theorem](#extreme-value-theorem) applied to $g'$.

#### Uniform-mesh Darboux criterion

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

A bounded function on $[0,1]$ is [Riemann integrable](#riemann-integrable-function) if and only if its [upper Darboux sum](#upper-darboux-sum) minus its [lower Darboux sum](#lower-darboux-sum) on the equal-length partition $D_n$ tends to zero. Sufficiency follows directly from the [Riemann integrability criterion](#riemann-integrability-criterion). Necessity follows by comparing with a fixed partition whose gap is small and using the [finite bad-cell estimate for Darboux sums](#finite-bad-cell-estimate-for-darboux-sums). The equal-length partitions need not be nested.

##### Finite bad-cell estimate for Darboux sums

↑ **Parent:** [Uniform-mesh Darboux criterion](#uniform-mesh-darboux-criterion)

Let $|f|\leq M$ on $[0,1]$ and let $P$ have $r$ interior division points. At most $r$ cells of the equal-length partition $D_n$ have one of those points in their interior. Their total length is at most $r/n$, and their oscillation is at most $2M$. Every other cell lies in a single cell of $P$. Therefore

$$
U(f,D_n)-L(f,D_n)\leq U(f,P)-L(f,P)+\frac{2Mr}{n}.
$$

This comparison of [Darboux sums](#darboux-sum) avoids the incorrect assumption that $D_n$ refines $P$ for all large $n$.

#### Riemann-integrable function

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

A bounded function on a closed interval is Riemann-integrable when its [upper and lower Darboux integrals](#upper-and-lower-darboux-integrals) agree.

##### Dense jumps do not prevent Riemann integrability

↑ **Parent:** [Riemann-integrable function](#riemann-integrable-function)

A [left-continuous cumulative function of an atomic measure](calculus.md#left-continuous-cumulative-function-of-an-atomic-measure) with positive masses at a dense countable set has dense discontinuities. Nevertheless it is bounded and monotone on a compact interval, hence a [Riemann-integrable function](#riemann-integrable-function). Finite step-function sums approximate it uniformly because the positive masses are summable. Thus dense discontinuities do not imply failure of the [Riemann integral](#riemann-integral).

#### Continuous functions are Riemann integrable

↑ **Parent:** [Riemann integrability criterion](#riemann-integrability-criterion)

A continuous function on a compact interval is uniformly continuous. A partition with sufficiently small mesh then makes the oscillation on every subinterval small, so its upper and lower Darboux sums can be made arbitrarily close.

### Darboux sum

↑ **Parent:** [Riemann integration](#riemann-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Darboux_sum)

A lower Darboux sum uses the infimum of a function on each partition interval, while an upper sum uses the supremum.

#### Oscillation of a function on an interval

↑ **Parent:** [Darboux sum](#darboux-sum)

For a bounded real function, its oscillation on an interval is its full range width there. An [upper Darboux sum](#upper-darboux-sum) minus a [lower Darboux sum](#lower-darboux-sum) is the sum of these widths multiplied by their interval lengths. This gives the [Riemann integrability criterion](#riemann-integrability-criterion) in terms of oscillation.

#### Darboux sum refinement monotonicity

↑ **Parent:** [Darboux sum](#darboux-sum)

For a bounded real function, inserting partition points increases its [lower Darboux sum](#lower-darboux-sum) and decreases its [upper Darboux sum](#upper-darboux-sum). This follows interval by interval because infima increase on smaller sets while suprema decrease, and the new widths sum to the original width. A common [partition refinement](#partition-refinement) consequently proves $s(f,D_1)\leq S(f,D_2)$ for arbitrary two partitions.

#### Upper Darboux sum

↑ **Parent:** [Darboux sum](#darboux-sum)

For a bounded function $f$ and a [partition of an interval](#partition-of-an-interval) $P$, the upper Darboux sum multiplies the [supremum](#supremum) of $f$ on each subinterval by its length and adds the results.

#### Lower Darboux sum

↑ **Parent:** [Darboux sum](#darboux-sum)

For a bounded function $f$ and a [partition of an interval](#partition-of-an-interval) $P$, the lower Darboux sum multiplies the [infimum](#infimum) of $f$ on each subinterval by its length and adds the results.

##### Exponential bound for a lower-sum product

↑ **Parent:** [Lower Darboux sum](#lower-darboux-sum)

For a nonnegative [Riemann-integrable function](#riemann-integrable-function) and an interval partition,

$$
\prod_k(1+m_k\Delta x_k)\leq e^{\sum_km_k\Delta x_k}\leq e^{\int_a^bf(x)\,dx},\qquad m_k=\inf_{[x_{k-1},x_k]}f.
$$

Every factor is nonnegative, so multiplication of $1+t\leq e^t$ is legitimate. The final step uses the lower-sum bound on the [Riemann integral](#riemann-integral).

#### Upper and lower Darboux integrals

↑ **Parent:** [Darboux sum](#darboux-sum)

For a bounded function,

$$
\overline{\int_a^b}f=\inf_PU(f,P),
\qquad
\underline{\int_a^b}f=\sup_PL(f,P).
$$

The function is Riemann integrable exactly when these values agree.

##### Lower Darboux integral

↑ **Parent:** [Upper and lower Darboux integrals](#upper-and-lower-darboux-integrals)

The lower Darboux integral of a bounded real function on a closed interval is the [supremum](#supremum) of its [lower Darboux sums](#lower-darboux-sum) over all [partitions of an interval](#partition-of-an-interval). Refinement increases a [lower Darboux sum](#lower-darboux-sum). A common refinement of two arbitrary [partitions of an interval](#partition-of-an-interval) proves that every [lower Darboux sum](#lower-darboux-sum) is at most every [upper Darboux sum](#upper-darboux-sum), hence the lower Darboux integral never exceeds the [upper Darboux integral](#upper-darboux-integral).

##### Upper Darboux integral

↑ **Parent:** [Upper and lower Darboux integrals](#upper-and-lower-darboux-integrals)

The upper Darboux integral of a bounded real function on a closed interval is the [infimum](#infimum) of its [upper Darboux sums](#upper-darboux-sum) over all [partitions of an interval](#partition-of-an-interval). Refinement decreases an [upper Darboux sum](#upper-darboux-sum), and the function is [Riemann integrable](#riemann-integrable-function) precisely when this infimum agrees with its [lower Darboux integral](#lower-darboux-integral).

### Improper integration by truncation

↑ **Parent:** [Riemann integration](#riemann-integration)

For a nonnegative unbounded function, one truncation convention sets $f_r=\min(f,r)$ and asks that every $f_r$ be Riemann integrable and that $\int f_r$ have a finite limit as $r\to\infty$.

#### First occurrence of a decimal digit

↑ **Parent:** [Improper integration by truncation](#improper-integration-by-truncation)

Under uniform length on $[0,1]$, the position $K$ of the first occurrence of a fixed decimal digit has

$$
\Pr(K=k)=\frac1{10}\left(\frac9{10}\right)^{k-1}.
$$

The set of expansions in which the digit never occurs has length zero, and

$$
\mathbb E K=\sum_{k\geq1}\frac{k}{10}\left(\frac9{10}\right)^{k-1}=10.
$$

## Convergent subsequence

↑ **Parent:** [Real analysis](real-analysis.md)

A convergent subsequence of $(x_n)$ is a sequence $(x_{n_k})$ with strictly increasing indices $n_k$ that converges to a limit.

## Proper extended-real function

↑ **Parent:** [Real analysis](real-analysis.md)

An extended-real function is proper if it never takes $-\infty$ and is finite at at least one point. It can take $+\infty$ to impose a constraint. A [convex function](#convex-function) with this property is a [proper convex function](#proper-convex-function).

### Effective domain

↑ **Parent:** [Proper extended-real function](#proper-extended-real-function)

The [effective domain](#effective-domain) of an extended-real [function](function.md) is $\operatorname{dom}E=\{u:E(u)<+\infty\}$. An infinite value can impose a hard constraint through an [indicator functional of a constraint set](inverse-problem.md#indicator-functional-of-a-constraint-set).

## Convex function

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convex_function)

A function is convex when its value on a line segment is at most the corresponding affine interpolation of endpoint values.

### Finite convex function as supremum of affine minorants

↑ **Parent:** [Convex function](#convex-function)

For a finite real [convex function](#convex-function) on an entire real [vector space](vector-space.md), apply the [convex domination form of the Hahn-Banach theorem](functional-analysis.md#convex-domination-form-of-the-hahn-banach-theorem) to $\phi(y+z)-\phi(y)$ and the zero functional on $\{0\}$. It supplies a [linear functional](linear-algebra.md#linear-functional) $\ell_y$ dominated by this translated function. The [affine function](vector-space.md#affine-function) $a_y(x)=\phi(y)+\ell_y(x-y)$ lies below $\phi$ everywhere and equals it at $y$. Taking the supremum proves the formula. These are algebraic affine minorants; continuity requires additional topological hypotheses.

### Essential smoothness of a convex function

↑ **Parent:** [Convex function](#convex-function)

An extended-real [convex function](#convex-function) $\Lambda:\mathbb R^d\to\mathbb R\cup\{+\infty\}$ is [essentially smooth](#essential-smoothness-of-a-convex-function) if its effective domain has nonempty interior, it is differentiable throughout that interior, and $\|\nabla\Lambda(\theta_n)\|\to\infty$ whenever interior points converge to a finite boundary point of the domain. A differentiable [convex function](#convex-function) finite on all of $\mathbb R^d$ satisfies the boundary condition vacuously. The [cumulant-generating function](probability-theory.md#cumulant-generating-function) $\log(r/(r-\theta))$ on $\theta<r$ has derivative $(r-\theta)^{-1}$ and is [essentially smooth](#essential-smoothness-of-a-convex-function). Restricting its domain to $\theta<\lambda<r$ destroys this property. This distinction matters in the lower bounds of the [Gärtner–Ellis theorem](convergence-of-random-variables.md#gartner-ellis-theorem).

### Convex quadratic function

↑ **Parent:** [Convex function](#convex-function)

A [convex quadratic function](#convex-quadratic-function) on $\mathbb R^n$ has the form $q(x)=\tfrac12x^THx+b^Tx+c$ with a symmetric [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) $H$. Its Hessian is $H$, and $q(y)-q(x)-\nabla q(x)\cdot(y-x)=\tfrac12(y-x)^TH(y-x)\geq0$, proving convexity directly. A stationary point is a global minimum. On a compact polytope, a minimum either is stationary in the interior or minimizes a restriction to a boundary face.

### Bounded convex functions are locally Lipschitz on an open ball

↑ **Parent:** [Convex function](#convex-function)

Let a real [convex function](#convex-function) satisfy $|f|\leq M$ on the open unit ball of a [normed space](functional-analysis.md#normed-vector-space). For $4r=1-\|x\|$, points $u,v\in B(x,r)$ satisfy $|f(u)-f(v)|\leq(M/r)\|u-v\|$. Extend the segment from $u$ through $v$ to length $2r$; its endpoint still lies in the domain, and [convexity](#convex-function) bounds the difference by $2M\|u-v\|/(2r)$. Reverse $u,v$ for the opposite inequality. Unlike finite-dimensional local continuity theorems, this argument applies in arbitrary dimension because boundedness on a full neighborhood is assumed.

### Negative part of a finite convex function is Lipschitz

↑ **Parent:** [Convex function](#convex-function)

For a finite [convex function](#convex-function) $f:\mathbb R\to\mathbb R$, its negative part $f^-=\max(-f,0)$ is globally [Lipschitz continuous](#lipschitz-continuity). The negative sublevel set is an interval. If bounded, local Lipschitz continuity of finite convex functions bounds the slopes on its closure. If it is a left ray, any negative slope there would force $f$ positive far to the left by the supporting-line inequality; all slopes on that ray are therefore nonnegative and bounded above near its finite endpoint. For a right ray the analogous slopes are nonpositive and bounded below. If $f$ is negative everywhere, convexity and boundedness above force it to be constant. These cases bound the slopes of $f^-$ globally, including its zero extension outside the interval. In particular, integrability of $f(Z)$ implies integrability of the negative part of every fixed translate $f(Z+x)$.

### Affine minorant

↑ **Parent:** [Convex function](#convex-function)

An affine minorant of $f$ is a function $x\mapsto\langle a,x\rangle+b$ that is everywhere at most $f(x)$. Every proper lower-semicontinuous [convex function](#convex-function) has such a minorant, by separating a point below its closed [epigraph](calculus-of-variations.md#epigraph). Adding a positive quadratic then yields a [coercive function](#coercive-function), which establishes existence in proximal minimization.

### Proper convex function

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_convex_function)

A proper convex function is both a [convex function](#convex-function) and a [proper extended-real function](#proper-extended-real-function). For example, the [total variation seminorm on a domain](inverse-problem.md#total-variation-seminorm-on-a-domain) is nonnegative, finite at zero, and a supremum of linear functionals, making it proper and convex.

### Operator convex function

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operator_convex_function)

A real function $f$ on an interval $I$ is operator convex when

$$
f(\lambda A+(1-\lambda)B)
\leq\lambda f(A)+(1-\lambda)f(B)
$$

in the [Loewner order](linear-algebra.md#loewner-order) for all [Hermitian operators](hilbert-space.md#hermitian-operator) $A,B$ with spectra in $I$ and every $0\leq\lambda\leq1$.

#### Operator concave function

↑ **Parent:** [Operator convex function](#operator-convex-function)

A function is operator concave when its negative is [operator convex](#operator-convex-function). Equivalently, the defining operator-convexity inequality is reversed.

### Continuity of a convex function

↑ **Parent:** [Convex function](#convex-function)

A finite convex function on an open convex subset of a finite-dimensional real vector space is locally Lipschitz, and therefore [continuous](calculus.md#continuous-function). In one dimension this follows by bounding its secant slopes between two slightly wider endpoints.

### Pointwise maximum of convex functions

↑ **Parent:** [Convex function](#convex-function)

The pointwise maximum of finitely many convex functions is convex because

$$
\max_i f_i(tx+(1-t)y)
\leq t\max_i f_i(x)+(1-t)\max_i f_i(y).
$$

### Softplus

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Softplus)

The softplus function $s(x)=\log(1+e^x)$ is convex because

$$
s''(x)=\frac{e^x}{(1+e^x)^2}>0.
$$

### Absolute value

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolute_value)

The absolute value function is convex by the triangle inequality:

$$
|tx+(1-t)y|\leq t|x|+(1-t)|y|.
$$

For a real number $x$, its [absolute value](#absolute-value) is $x$ when $x\geq0$ and $-x$ otherwise; for a complex number $z$, it is the nonnegative magnitude $\sqrt{z\overline z}$.

#### Absolute value at a simple zero

↑ **Parent:** [Absolute value](#absolute-value)

Suppose a real function $g$ is differentiable at $a$, with $g(a)=0$ and $g'(a)\ne0$. The [derivative](calculus.md#derivative) definition gives $g(a+h)=g'(a)h+o(|h|)$. The [reverse triangle inequality](topological-analysis.md#reverse-triangle-inequality) then implies

$$
|g(a+h)|=|g'(a)|\,|h|+o(|h|).
$$

Thus $|g|$ has unequal [one-sided derivatives](calculus.md#one-sided-derivative), $|g'(a)|$ on the right and $-|g'(a)|$ on the left. More generally, multiplication by a function $w$ continuous at $a$ with $w(a)\ne0$ gives right and left slopes $w(a)|g'(a)|$ and $-w(a)|g'(a)|$. This elementary expansion explains how a smooth oscillation can acquire infinitely many corners under the [absolute value function](#absolute-value), even after multiplication by a factor that makes it differentiable at an accumulation point.

#### Summable absolute-value cusp series

↑ **Parent:** [Absolute value](#absolute-value)

Let the locations $a_n$ be distinct and bounded, and let $c_n>0$ with $\sum_nc_n<\infty$. The [Weierstrass M-test](probability-and-statistics.md#weierstrass-m-test) gives locally [uniform convergence](#uniform-convergence) of $G$, so the [uniform limit theorem](#uniform-limit-theorem) makes it [continuous](calculus.md#continuous-function). The [reverse triangle inequality](topological-analysis.md#reverse-triangle-inequality) bounds each term's [difference quotient](calculus.md#difference-quotient) by $c_n$. Consequently a uniformly small tail permits passing each one-sided difference-quotient limit through the series. At every point outside the locations, $G'(x)=\sum_nc_n\operatorname{sgn}(x-a_n)$; at $a_m$, the right derivative minus the left derivative is $2c_m>0$. Thus the function has precisely the prescribed cusp locations, even when they accumulate at another point where the function remains [differentiable](analysis.md#differentiable-function).

### Strongly convex function

↑ **Parent:** [Convex function](#convex-function)

A differentiable function is $\alpha$-strongly convex when

$$
f(y)\geq f(x)+\nabla f(x)\cdot(y-x)
+\frac\alpha2\|y-x\|^2.
$$

#### Uniformly convex variational integrand

↑ **Parent:** [Strongly convex function](#strongly-convex-function)

A gradient integrand is uniformly convex in this elliptic variational sense when its [Hessian matrix](calculus.md#hessian-matrix) in the gradient variables has a common positive lower bound. Then $(F_p(x,p)-F_p(x,q))\cdot(p-q)\geq\lambda|p-q|^2$. Averaging $F_{pp}$ along a line segment in gradient space preserves the same lower bound.

##### Interior gradient regularity for uniformly convex autonomous energies

↑ **Parent:** [Uniformly convex variational integrand](#uniformly-convex-variational-integrand)

For scalar minimizers of $\int F(Du)$ with $F\in C^2(\mathbb R^n)$ and globally bounded uniformly positive [Hessian matrix](calculus.md#hessian-matrix), no higher differentiability of $F$ is needed for interior gradient Hölder continuity. The weak Euler-Lagrange equation is $\operatorname{div}DF(Du)=0$. Difference quotients solve uniformly elliptic equations with coefficient matrices obtained by averaging $D^2F$ along gradient segments. The [Caccioppoli inequality](partial-differential-equation.md#caccioppoli-inequality) and difference quotient characterization give $u\in H^2_{\mathrm{loc}}$. The [Sobolev chain rule](distribution-theory.md#sobolev-chain-rule) then gives $\operatorname{div}(D^2F(Du)D(D_ku))=0$. The [De Giorgi-Nash-Moser theorem](elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem) makes each derivative Hölder continuous, with exponent depending only on dimension and the ellipticity ratio. This scalar conclusion should not be assumed for vector-valued elliptic systems.

##### Uniqueness for uniformly convex gradient Dirichlet problems

↑ **Parent:** [Uniformly convex variational integrand](#uniformly-convex-variational-integrand)

On a bounded domain, classical solutions continuous on the closure have difference $w=u-v$ satisfying $D_i(A_{ij}D_jw)=0$, where $A=\int_0^1F_{pp}(x,Dv+tDw)\,dt$. The coefficients are uniformly elliptic and locally smooth. Apply the [weak maximum principle](elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) on inner domains whose closures lie in the original domain, then let their boundary distances tend to zero. The common continuous boundary values make their boundary differences tend uniformly to zero, proving uniqueness without assuming global bounds on derivatives of the linearized coefficients.

### Strictly convex function

↑ **Parent:** [Convex function](#convex-function)

A function $f$ on a [convex set](mathematical-optimization.md#convex-set) is strictly convex when

$$
f(tx+(1-t)y)<tf(x)+(1-t)f(y)
$$

whenever $x\ne y$ and $0<t<1$.

#### Uniqueness of a minimizer of a strictly convex function

↑ **Parent:** [Strictly convex function](#strictly-convex-function)

A strictly convex function has at most one minimizer: if distinct points attained the same minimum, every strict convex combination of them would have a smaller value.

### Convexity domain of x cubed plus y cubed plus Axy

↑ **Parent:** [Convex function](#convex-function)

The [Hessian matrix](calculus.md#hessian-matrix) of

$$
f(x,y)=x^3+y^3+Axy
$$

is positive semidefinite exactly when

$$
x\geq0,\qquad y\geq0,\qquad 36xy\geq A^2.
$$

This region is convex: for $A\ne0$ it is the epigraph of $A^2/(36x)$ in the positive quadrant, and for $A=0$ it is the closed first quadrant.

### Perspective function

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perspective_function)

The perspective of f is g(t,x)=t f(x/t) for positive t and preserves convexity.

### Subgradient

↑ **Parent:** [Convex function](#convex-function)

A subgradient of a [convex function](#convex-function) $f$ at $x$ is a vector $g$ such that $f(y)\geq f(x)+g^T(y-x)$ for every $y$ in the domain.

#### Continuous supporting functional for a locally bounded convex function

↑ **Parent:** [Subgradient](#subgradient)

A real [convex function](#convex-function) locally bounded on an open [convex set](mathematical-optimization.md#convex-set) has a continuous supporting [linear functional](linear-algebra.md#linear-functional) at every interior point. Apply the dominated [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) to its sublinear [directional derivative](calculus.md#directional-derivative) $p_x$ to obtain $l\leq p_x$. Increasing secant slopes imply $p_x(z)\leq f(x+z)-f(x)$ whenever the endpoint is in the domain. A local [Lipschitz continuity](#lipschitz-continuity) bound gives both $l(y)\leq L\|y\|$ and $-l(y)=l(-y)\leq L\|y\|$, proving continuity.

#### Subgradient optimality condition

↑ **Parent:** [Subgradient](#subgradient)

A proper convex function $f$ is minimized at $x$ exactly when $0\in\partial f(x)$. For a differentiable convex term $g$ and another convex term $h$, the [subdifferential sum rule](convex-optimization.md#subdifferential-sum-rule) gives the condition $0\in\nabla g(x)+\partial h(x)$.

#### Subgradient of the absolute value

↑ **Parent:** [Subgradient](#subgradient)

The [absolute value function](#absolute-value) has

$$
\partial|x|=
\begin{cases}
\{\operatorname{sgn}x\},&x\ne0,\\
[-1,1],&x=0.
\end{cases}
$$

#### Subgradient inequality

↑ **Parent:** [Subgradient](#subgradient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subgradient_inequality)

A vector is a subgradient when its supporting affine function lies below the convex function.

<h3 id="jensen-s-inequality">Jensen's inequality</h3>

↑ **Parent:** [Convex function](#convex-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jensen's_inequality)

For a [convex function](#convex-function) $f$ and an integrable [random variable](random-variable.md) $X$,

$$
f(\mathbb E X)\leq\mathbb E[f(X)].
$$

The inequality is reversed when $f$ is [concave](#concave-function).

#### Sharp two-term convex power bound

↑ **Parent:** [Jensen's inequality](#jensen-s-inequality)

Apply [Jensen's inequality](#jensen-s-inequality) to the two equally weighted values $a,b$ and the [convex function](#convex-function) $t\mapsto t^p$. Equality for $a=b>0$ proves that $2^{p-1}$ is the smallest possible constant. For $p>1$, strict convexity makes equality equivalent to $a=b$; for $p=1$, equality holds for every pair.

## Concave function

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Concave_function)

A function $f$ is concave exactly when $-f$ is [convex](#convex-function). Equivalently,

$$
f(tx+(1-t)y)\geq tf(x)+(1-t)f(y)
$$

for $0\leq t\leq1$.

### Extrema of a concave power sum on a simplex

↑ **Parent:** [Concave function](#concave-function)

For $0<c<1$ on the [probability simplex](algebraic-topology.md#probability-simplex), $x_i^c\geq x_i$ gives the lower bound, with equality exactly at its vertices. Strict concavity and the [Jensen inequality](#jensen-s-inequality) give the upper bound, with equality exactly at the uniform point $x_i=1/n$. Thus the boundary can minimize a strictly concave objective, while its unique maximum lies at the symmetric interior point; a Lagrange-multiplier calculation alone would miss the boundary minimum.

### Strictly increasing concave function

↑ **Parent:** [Concave function](#concave-function)

Let a differentiable [concave function](#concave-function) on all of $\mathbb R^d$ be strictly increasing in each coordinate separately. Every coordinate derivative is strictly positive. Indeed it is nonnegative by monotonicity and nonincreasing along its coordinate by [concavity](#concave-function); a zero value would force zero derivative on the remaining positive ray and hence a constant segment. The global-domain assumption matters at endpoints of restricted domains.

### Concave supporting-tangent inequality

↑ **Parent:** [Concave function](#concave-function)

For a differentiable [concave](#concave-function) function, secant slopes lie below the tangent slope at their left endpoint and above the tangent slope at their right endpoint. This gives the displayed inequality for either order of $x,y$. It converts a first-order optimality relation into a global utility bound. Strict [concavity](#concave-function) makes equality possible only at $x=y$, on the differentiability domain.

### Concave majorant

↑ **Parent:** [Concave function](#concave-function)

A concave majorant of $F$ is a [concave function](#concave-function) lying everywhere above $F$ on the specified domain. The least concave majorant, when it exists, is the pointwise smallest such function. A common tangent can replace an upward derivative kink by a linear segment joining two contact points.

### Strictly concave function

↑ **Parent:** [Concave function](#concave-function)

A function is strictly concave when its concavity inequality is strict for distinct points and coefficients strictly between zero and one. A strictly concave function has at most one maximizer on a convex set.

#### Strict concavity

↑ **Parent:** [Strictly concave function](#strictly-concave-function)

Strict concavity is the displayed property for distinct $x,y$ in a [convex set](mathematical-optimization.md#convex-set) and $0<t<1$. It makes a stationary point of a [differentiable function](analysis.md#differentiable-function) its unique global maximum, whenever such a stationary point exists.

##### Positive-product maximization on a convex set

↑ **Parent:** [Strict concavity](#strict-concavity)

A compact convex subset of $\mathbb R^2$ meeting the positive quadrant has a unique positive point maximizing $xy$. Existence follows by maximizing the continuous product on the intersection with the closed nonnegative quadrant; a positive attainable value excludes its axes. Uniqueness follows from strict concavity of $\log x+\log y$ on the positive quadrant. This is a useful way to optimize a product even though the product itself is not concave.

#### Uniform negative curvature and global maximization

↑ **Parent:** [Strictly concave function](#strictly-concave-function)

If a twice differentiable real [function](function.md) on $\mathbb R$ satisfies $f''(x)\le-c$ for some fixed $c>0$, then it has a unique [global maximum](function.md#global-maximum). The [mean value theorem](calculus.md#mean-value-theorem) shows that $f'$ is strictly decreasing, and that $f'(x)+cx$ is nonincreasing. Hence $f'(x)\le f'(0)-cx$ for $x>0$ and $f'(x)\ge f'(0)-cx$ for $x<0$. These inequalities force opposite derivative signs at the two ends. The [intermediate value theorem](calculus.md#intermediate-value-theorem) supplies a unique zero of $f'$, at which $f$ changes from increasing to decreasing. Merely having $f''<0$ does not guarantee existence: $f(x)=-e^{-x}$ is increasing and approaches its unattained supremum zero.

#### Product maximizer on a compact convex subset of the positive orthant

↑ **Parent:** [Strictly concave function](#strictly-concave-function)

On the positive orthant,

$$
F(x)=\sum_{j=1}^n\log x_j
$$

is strictly concave. Its unique maximizer $x^*$ on a compact convex feasible set satisfies the first-order inequality

$$
\nabla F(x^*)\cdot(x-x^*)\leq0,
$$

equivalently

$$
\sum_{j=1}^n\frac{x_j}{x_j^*}\leq n.
$$

## Measure theory

↑ **Parent:** [Real analysis](real-analysis.md)

[This section is present in another page, follow this link to view it.](measure-theory.md)

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Analytic number theory](analytic-number-theory.md)
