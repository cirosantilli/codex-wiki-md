# Complex analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_analysis)

**Table of contents**

- [Nontangential limit](#nontangential-limit)
  - [Stolz region](#stolz-region)
- [Polynomial hull](#polynomial-hull)
  - [Polynomial hull in one complex variable](#polynomial-hull-in-one-complex-variable)
- [Lower half-plane](#lower-half-plane)
- [Holomorphic square root](#holomorphic-square-root)
  - [Holomorphic square root outside all polynomial roots](#holomorphic-square-root-outside-all-polynomial-roots)
- [Monodromy](#monodromy)
  - [Isomonodromic deformation](#isomonodromic-deformation)
  - [Formal monodromy](#formal-monodromy)
    - [Formal monodromy correction to an entire-system Stokes product](#formal-monodromy-correction-to-an-entire-system-stokes-product)
  - [Monodromy eigenfunction Laurent representation](#monodromy-eigenfunction-laurent-representation)
- [Cayley transform between the half-plane and disk](#cayley-transform-between-the-half-plane-and-disk)
- [Holomorphic logarithm](#holomorphic-logarithm)
- [Upper half-plane (complex analysis)](#upper-half-plane-complex-analysis)
  - [Conformal automorphism of the upper half-plane](#conformal-automorphism-of-the-upper-half-plane)
- [Polylogarithm](#polylogarithm)
  - [Dilogarithm](#dilogarithm)
- [Holomorphic function](#holomorphic-function)
  - [Complex differentiability](#complex-differentiability)
  - [Nevanlinna class](#nevanlinna-class)
    - [Bounded characteristic](#bounded-characteristic)
      - [Quotient characterization of bounded characteristic](#quotient-characterization-of-bounded-characteristic)
  - [Multiplicity of a zero](#multiplicity-of-a-zero)
  - [Periodic holomorphic descent through the exponential map](#periodic-holomorphic-descent-through-the-exponential-map)
  - [Constant-modulus holomorphic function](#constant-modulus-holomorphic-function)
  - [Banach-space-valued holomorphic function](#banach-space-valued-holomorphic-function)
    - [Spectral-radius maximum principle](#spectral-radius-maximum-principle)
    - [Norm maximum principle for a Banach-space-valued holomorphic function](#norm-maximum-principle-for-a-banach-space-valued-holomorphic-function)
  - [Prescribed zeros in a plane domain via Runge approximation](#prescribed-zeros-in-a-plane-domain-via-runge-approximation)
  - [Antiholomorphic function](#antiholomorphic-function)
  - [Holomorphic convex hull](#holomorphic-convex-hull)
  - [Blaschke product](#blaschke-product)
    - [Interior zero count for a finite Blaschke product minus a constant](#interior-zero-count-for-a-finite-blaschke-product-minus-a-constant)
    - [Hyperbolic zero estimate for a Blaschke product](#hyperbolic-zero-estimate-for-a-blaschke-product)
    - [Vanishing absolute logarithmic mean characterization of Blaschke products](#vanishing-absolute-logarithmic-mean-characterization-of-blaschke-products)
    - [Blaschke factorization of a bounded holomorphic function](#blaschke-factorization-of-a-bounded-holomorphic-function)
    - [Radial logarithmic mean of a Blaschke product](#radial-logarithmic-mean-of-a-blaschke-product)
    - [Automorphy character of an orbit Blaschke product](#automorphy-character-of-an-orbit-blaschke-product)
    - [Blaschke condition](#blaschke-condition)
      - [Blaschke sequence](#blaschke-sequence)
  - [Jensen's formula](#jensen-s-formula)
    - [Poisson-Jensen formula](#poisson-jensen-formula)
      - [Annular spherical Jensen formula](#annular-spherical-jensen-formula)
    - [Jensen zero-count bound](#jensen-zero-count-bound)
      - [Lattice zeros force quadratic exponential growth](#lattice-zeros-force-quadratic-exponential-growth)
  - [Holomorphic primitive](#holomorphic-primitive)
  - [Complex differentiability at a point](#complex-differentiability-at-a-point)
  - [Space of holomorphic functions](#space-of-holomorphic-functions)
    - [Weighted holomorphic norm on a shrinking time domain](#weighted-holomorphic-norm-on-a-shrinking-time-domain)
      - [Contraction estimate on a shrinking holomorphic domain](#contraction-estimate-on-a-shrinking-holomorphic-domain)
  - [Order of a zero of a holomorphic function](#order-of-a-zero-of-a-holomorphic-function)
    - [Zero sets in the unit disc](#zero-sets-in-the-unit-disc)
    - [Simple zero](#simple-zero)
  - [Analytic continuation](#analytic-continuation)
    - [Natural boundary of a holomorphic function](#natural-boundary-of-a-holomorphic-function)
    - [Zeta function regularization](#zeta-function-regularization)
      - [Half-integer zeta-regularized mode sum](#half-integer-zeta-regularized-mode-sum)
    - [Meromorphic continuation](#meromorphic-continuation)
    - [Sokhotski–Plemelj theorem](#sokhotski-plemelj-theorem)
      - [Signed Cauchy boundary operators](#signed-cauchy-boundary-operators)
    - [Monodromy theorem](#monodromy-theorem)
      - [Monodromy group of a covering](#monodromy-group-of-a-covering)
        - [Monodromy transposition in a three-sheeted cover](#monodromy-transposition-in-a-three-sheeted-cover)
        - [Monodromy group of z squared plus z to the minus two](#monodromy-group-of-z-squared-plus-z-to-the-minus-two)
    - [Analytic continuation by contour deformation](#analytic-continuation-by-contour-deformation)
      - [Branch phase in a figure-eight analytic continuation integral](#branch-phase-in-a-figure-eight-analytic-continuation-integral)
    - [Multivalued inverse hyperbolic sine](#multivalued-inverse-hyperbolic-sine)
  - [Entire function](#entire-function)
    - [Injective entire functions are affine](#injective-entire-functions-are-affine)
    - [Exponential polynomial](#exponential-polynomial)
    - [Order of an entire function](#order-of-an-entire-function)
    - [Entire function of exponential type](#entire-function-of-exponential-type)
    - [Weierstrass factorization theorem](#weierstrass-factorization-theorem)
      - [Canonical product](#canonical-product)
        - [Canonical product construction for zeros escaping to the disk boundary](#canonical-product-construction-for-zeros-escaping-to-the-disk-boundary)
        - [Boundary-adapted holomorphic zero factor](#boundary-adapted-holomorphic-zero-factor)
      - [Hadamard factorization theorem](#hadamard-factorization-theorem)
      - [Entire functions with the same zero divisor](#entire-functions-with-the-same-zero-divisor)
    - [Pointwise vanishing derivative criterion for a polynomial](#pointwise-vanishing-derivative-criterion-for-a-polynomial)
    - [Picard theorem](#picard-theorem)
      - [Little Picard theorem](#little-picard-theorem)
        - [Great Picard theorem](#great-picard-theorem)
  - [Analytic function with image in an affine real line](#analytic-function-with-image-in-an-affine-real-line)
- [Simply connected domain](#simply-connected-domain)
  - [Crosscut](#crosscut)
  - [Primitive of a holomorphic function on a simply connected domain](#primitive-of-a-holomorphic-function-on-a-simply-connected-domain)
- [Complex inverse sine](#complex-inverse-sine)
  - [Branches of the complex inverse sine](#branches-of-the-complex-inverse-sine)
    - [Monodromy of the complex inverse sine](#monodromy-of-the-complex-inverse-sine)
- [Morera's theorem](#morera-s-theorem)
- [Cauchy's integral theorem](#cauchy-s-integral-theorem)
  - [Cauchy theorem for a triangle](#cauchy-theorem-for-a-triangle)
  - [Contour deformation](#contour-deformation)
  - [Gaussian contour translation](#gaussian-contour-translation)
- [Cauchy principal value](#cauchy-principal-value)
  - [Principal-value beta integral](#principal-value-beta-integral)
- [Principal-value residue rule](#principal-value-residue-rule)
- [Exponential integral](#exponential-integral)
  - [Logarithmic expansion of a symmetric exponential integral](#logarithmic-expansion-of-a-symmetric-exponential-integral)
    - [Moving-cutoff correction to a symmetric exponential integral](#moving-cutoff-correction-to-a-symmetric-exponential-integral)
  - [Small-argument expansion of the exponential integral](#small-argument-expansion-of-the-exponential-integral)
- [Gamma function](#gamma-function)
  - [Derivative of the gamma function](#derivative-of-the-gamma-function)
  - [Gamma function has no zeros](#gamma-function-has-no-zeros)
  - [Imaginary-argument gamma asymptotic](#imaginary-argument-gamma-asymptotic)
  - [Gamma function residue at a nonpositive integer](#gamma-function-residue-at-a-nonpositive-integer)
  - [Euler product for the gamma function](#euler-product-for-the-gamma-function)
  - [Residues of the Gamma function](#residues-of-the-gamma-function)
  - [Gamma integral](#gamma-integral)
    - [Cubic oscillatory Gamma integral](#cubic-oscillatory-gamma-integral)
  - [Gamma function recurrence](#gamma-function-recurrence)
  - [Bose integral](#bose-integral)
  - [Euler's constant](#euler-s-constant)
  - [Weierstrass product for the reciprocal gamma function](#weierstrass-product-for-the-reciprocal-gamma-function)
  - [Digamma function](#digamma-function)
    - [Trigamma function](#trigamma-function)
    - [Positive zero of the digamma function](#positive-zero-of-the-digamma-function)
  - [Gamma reflection formula](#gamma-reflection-formula)
  - [Gamma duplication formula](#gamma-duplication-formula)
  - [Beta function](#beta-function)
    - [Incomplete beta function](#incomplete-beta-function)
    - [Complex beta integral](#complex-beta-integral)
    - [Beta--gamma identity](#beta-gamma-identity)
      - [Sum-and-ratio substitution for gamma integrals](#sum-and-ratio-substitution-for-gamma-integrals)
    - [Beta-function recurrence](#beta-function-recurrence)
    - [Logarithmic moments of the Cauchy kernel](#logarithmic-moments-of-the-cauchy-kernel)
  - [Gamma function asymptotic at zero](#gamma-function-asymptotic-at-zero)
    - [Diagonal beta-function asymptotic at zero](#diagonal-beta-function-asymptotic-at-zero)
- [Riemann surfaces](#riemann-surfaces)
  - [Meromorphic differential on a Riemann surface](#meromorphic-differential-on-a-riemann-surface)
  - [Hyperbolic Riemann surface in potential theory](#hyperbolic-riemann-surface-in-potential-theory)
  - [Compact Riemann surface](#compact-riemann-surface)
  - [Abel-Jacobi map of a compact Riemann surface](#abel-jacobi-map-of-a-compact-riemann-surface)
    - [Abel theorem for divisors](#abel-theorem-for-divisors)
  - [Differential of the third kind](#differential-of-the-third-kind)
  - [Riemann bilinear relations for a compact surface](#riemann-bilinear-relations-for-a-compact-surface)
  - [Three-branch-point regular surface cover](#three-branch-point-regular-surface-cover)
    - [Orientation-reversing equivalence of branched-cover monodromy](#orientation-reversing-equivalence-of-branched-cover-monodromy)
  - [Quasiconformal mapping](#quasiconformal-mapping)
    - [Maximal dilatation](#maximal-dilatation)
    - [Beltrami coefficient](#beltrami-coefficient)
      - [Beltrami equation](#beltrami-equation)
  - [Conformal metric](#conformal-metric)
  - [Translation surface](#translation-surface)
    - [Slit connected sum of translation tori](#slit-connected-sum-of-translation-tori)
  - [Teichmüller theory](#teichmuller-theory)
    - [Teichmüller map](#teichmuller-map)
      - [Teichmüller's uniqueness theorem](#teichmuller-s-uniqueness-theorem)
      - [Reich–Strebel inequality](#reich-strebel-inequality)
    - [Extremal length](#extremal-length)
      - [Extremal length lower bound from a closed one-form](#extremal-length-lower-bound-from-a-closed-one-form)
      - [Conformal modulus of an annulus](#conformal-modulus-of-an-annulus)
        - [Conformal cylinder](#conformal-cylinder)
    - [SL2R action on differentials](#sl2r-action-on-differentials)
    - [Teichmüller space](#teichmuller-space)
  - [Local coordinate](#local-coordinate)
  - [Holomorphic map](#holomorphic-map)
    - [Biholomorphism](#biholomorphism)
  - [Germ of a holomorphic function](#germ-of-a-holomorphic-function)
    - [Function element](#function-element)
    - [Space of germs of holomorphic functions](#space-of-germs-of-holomorphic-functions)
      - [Analytic germ projection](#analytic-germ-projection)
        - [Surjective inverse-polynomial germ projection without even covering](#surjective-inverse-polynomial-germ-projection-without-even-covering)
      - [Evaluation map on a space of germs](#evaluation-map-on-a-space-of-germs)
      - [Germ surface of the square root of z to the eighth minus one](#germ-surface-of-the-square-root-of-z-to-the-eighth-minus-one)
  - [Complex structure lifted through a covering map](#complex-structure-lifted-through-a-covering-map)
  - [Uniformization theorem](#uniformization-theorem)
    - [Thrice-punctured sphere as a modular quotient](#thrice-punctured-sphere-as-a-modular-quotient)
    - [Green-function exhaustion proof of disk uniformization](#green-function-exhaustion-proof-of-disk-uniformization)
    - [Riemann mapping theorem](#riemann-mapping-theorem)
      - [Square-root improvement of a normalized conformal map](#square-root-improvement-of-a-normalized-conformal-map)
      - [Caratheodory boundary extension theorem](#caratheodory-boundary-extension-theorem)
      - [Koebe distortion theorem](#koebe-distortion-theorem)
        - [Koebe quarter theorem](#koebe-quarter-theorem)
          - [Boundary-distance derivative bound for a conformal bijection](#boundary-distance-derivative-bound-for-a-conformal-bijection)
    - [Automorphisms of simply connected Riemann surfaces](#automorphisms-of-simply-connected-riemann-surfaces)
    - [Riemann surfaces uniformized by the complex plane](#riemann-surfaces-uniformized-by-the-complex-plane)
    - [Plane domain with two omitted points is hyperbolic](#plane-domain-with-two-omitted-points-is-hyperbolic)
    - [Uniformization of a punctured compact Riemann surface](#uniformization-of-a-punctured-compact-riemann-surface)
    - [Compact Riemann surface containing an embedded punctured plane](#compact-riemann-surface-containing-an-embedded-punctured-plane)
  - [Identity theorem on a Riemann surface](#identity-theorem-on-a-riemann-surface)
  - [Harmonic function on a Riemann surface](#harmonic-function-on-a-riemann-surface)
    - [Conformal invariance of harmonicity](#conformal-invariance-of-harmonicity)
  - [Regular covering map](#regular-covering-map)
  - [Complete analytic function](#complete-analytic-function)
  - [Valency theorem](#valency-theorem)
    - [Local degree of a holomorphic map](#local-degree-of-a-holomorphic-map)
    - [Degree of a holomorphic map](#degree-of-a-holomorphic-map)
      - [Degree of a power map of the Riemann sphere](#degree-of-a-power-map-of-the-riemann-sphere)
    - [Degree of a rational map of the Riemann sphere](#degree-of-a-rational-map-of-the-riemann-sphere)
      - [Degree bounds for the derivative of a rational function](#degree-bounds-for-the-derivative-of-a-rational-function)
      - [Degree of the derivative of a rational function](#degree-of-the-derivative-of-a-rational-function)
    - [Degree of an elliptic function](#degree-of-an-elliptic-function)
      - [Degree of the derivative of an elliptic function](#degree-of-the-derivative-of-an-elliptic-function)
    - [Octahedral rotation orbits on the Riemann sphere](#octahedral-rotation-orbits-on-the-riemann-sphere)
    - [Degree-sized invariant separates finite-group orbits](#degree-sized-invariant-separates-finite-group-orbits)
  - [Riemann-Hurwitz formula](#riemann-hurwitz-formula)
    - [Ramification index of a holomorphic map](#ramification-index-of-a-holomorphic-map)
      - [Ramification point of a holomorphic map](#ramification-point-of-a-holomorphic-map)
        - [Critical point of a rational map](#critical-point-of-a-rational-map)
          - [Critical orbit of a rational map](#critical-orbit-of-a-rational-map)
          - [Critical points of iterates of a rational map](#critical-points-of-iterates-of-a-rational-map)
          - [Critical multiplicity of a rational map](#critical-multiplicity-of-a-rational-map)
            - [Total critical multiplicity of a rational map](#total-critical-multiplicity-of-a-rational-map)
        - [Branch value of a holomorphic map](#branch-value-of-a-holomorphic-map)
          - [Ramification at infinity of a superelliptic covering](#ramification-at-infinity-of-a-superelliptic-covering)
    - [Triangulation proof of the Riemann-Hurwitz formula](#triangulation-proof-of-the-riemann-hurwitz-formula)
    - [Affine normal forms of a complex cubic polynomial](#affine-normal-forms-of-a-complex-cubic-polynomial)
  - [Riemann sphere](#riemann-sphere)
    - [Chordal metric](#chordal-metric)
      - [Rational map is Lipschitz in the chordal metric](#rational-map-is-lipschitz-in-the-chordal-metric)
    - [Stereographic projection](#stereographic-projection)
      - [Circle-plane relation under stereographic projection](#circle-plane-relation-under-stereographic-projection)
        - [Antipodal equatorial intersection criterion for a great circle](#antipodal-equatorial-intersection-criterion-for-a-great-circle)
      - [Antipodal stereographic coordinate relation](#antipodal-stereographic-coordinate-relation)
        - [Antipodal cross-ratio and spherical distance](#antipodal-cross-ratio-and-spherical-distance)
      - [Holomorphic stereographic atlas of the sphere](#holomorphic-stereographic-atlas-of-the-sphere)
      - [Sphere rotations as special-unitary Möbius transformations](#sphere-rotations-as-special-unitary-mobius-transformations)
    - [Local cyclic quotient of a Riemann surface](#local-cyclic-quotient-of-a-riemann-surface)
      - [Finite conformal quotient of a Riemann surface](#finite-conformal-quotient-of-a-riemann-surface)
    - [Orbit-separating invariant for the standard dihedral action on the Riemann sphere](#orbit-separating-invariant-for-the-standard-dihedral-action-on-the-riemann-sphere)
  - [Punctured Riemann surface](#punctured-riemann-surface)
    - [Path avoidance in a surface](#path-avoidance-in-a-surface)
    - [Punctured complex plane](#punctured-complex-plane)
      - [Cylinder as a punctured plane](#cylinder-as-a-punctured-plane)
  - [Transport of a complex structure](#transport-of-a-complex-structure)
  - [Nodal crossing](#nodal-crossing)
    - [Topological manifold local obstruction](#topological-manifold-local-obstruction)
    - [Reducible complex curve](#reducible-complex-curve)
- [Elliptic integral](#elliptic-integral)
  - [Elliptic integral of the first kind](#elliptic-integral-of-the-first-kind)
    - [Lemniscatic integral](#lemniscatic-integral)
    - [Complete elliptic integral of the first kind](#complete-elliptic-integral-of-the-first-kind)
      - [Logarithmic endpoint asymptotic of the complete elliptic integral](#logarithmic-endpoint-asymptotic-of-the-complete-elliptic-integral)
      - [Complementary complete elliptic integral of the first kind](#complementary-complete-elliptic-integral-of-the-first-kind)
- [Elliptic function](#elliptic-function)
  - [Zero-pole sum of an elliptic function](#zero-pole-sum-of-an-elliptic-function)
  - [Elliptic divisor-sum identity](#elliptic-divisor-sum-identity)
  - [Period lattice](#period-lattice)
    - [Fundamental parallelogram of a period lattice](#fundamental-parallelogram-of-a-period-lattice)
  - [Nonconstant elliptic function has a pole](#nonconstant-elliptic-function-has-a-pole)
  - [Jacobi elliptic functions](#jacobi-elliptic-functions)
    - [Jacobi elliptic sine](#jacobi-elliptic-sine)
      - [Period lattice of the Jacobi elliptic sine](#period-lattice-of-the-jacobi-elliptic-sine)
  - [Value multiplicity of an elliptic function](#value-multiplicity-of-an-elliptic-function)
  - [Weierstrass functions](#weierstrass-functions)
    - [Weierstrass elliptic function](#weierstrass-elliptic-function)
      - [Weierstrass addition formula](#weierstrass-addition-formula)
      - [Weierstrass sigma function](#weierstrass-sigma-function)
        - [Legendre relation for Weierstrass quasi-periods](#legendre-relation-for-weierstrass-quasi-periods)
      - [Four totally ramified Weierstrass values](#four-totally-ramified-weierstrass-values)
      - [Termwise derivative proof of Weierstrass periodicity](#termwise-derivative-proof-of-weierstrass-periodicity)
      - [Weierstrass shift-difference identity by pole cancellation](#weierstrass-shift-difference-identity-by-pole-cancellation)
      - [Elliptic collinearity determinant](#elliptic-collinearity-determinant)
        - [Confluent elliptic collinearity determinant](#confluent-elliptic-collinearity-determinant)
      - [Elliptic function-field decomposition](#elliptic-function-field-decomposition)
      - [Even elliptic functions are rational in the Weierstrass function](#even-elliptic-functions-are-rational-in-the-weierstrass-function)
        - [Degree-two even elliptic function](#degree-two-even-elliptic-function)
      - [Normal convergence of the Weierstrass elliptic-function series](#normal-convergence-of-the-weierstrass-elliptic-function-series)
      - [Half-period values of the Weierstrass elliptic function](#half-period-values-of-the-weierstrass-elliptic-function)
        - [Weierstrass half-period translation formula](#weierstrass-half-period-translation-formula)
          - [Weierstrass quarter-period derivative identity](#weierstrass-quarter-period-derivative-identity)
        - [Two-torsion point of a complex torus](#two-torsion-point-of-a-complex-torus)
      - [Equianharmonic lattice](#equianharmonic-lattice)
      - [Weierstrass zeta function](#weierstrass-zeta-function)
      - [Laurent coefficients of the Weierstrass elliptic function](#laurent-coefficients-of-the-weierstrass-elliptic-function)
        - [Positive polynomial recurrence for lattice Eisenstein sums](#positive-polynomial-recurrence-for-lattice-eisenstein-sums)
      - [Weierstrass elliptic differential equation](#weierstrass-elliptic-differential-equation)
        - [Nonvanishing discriminant of a complex lattice](#nonvanishing-discriminant-of-a-complex-lattice)
- [Runge's theorem](#runge-s-theorem)
  - [Uniform rational approximation algebra with prescribed poles](#uniform-rational-approximation-algebra-with-prescribed-poles)
  - [Polynomial Runge theorem](#polynomial-runge-theorem)
    - [Runge exhaustion of a slit disk](#runge-exhaustion-of-a-slit-disk)
    - [Pointwise polynomial approximation of a half-plane sign](#pointwise-polynomial-approximation-of-a-half-plane-sign)
    - [Pole-moving polynomial approximation](#pole-moving-polynomial-approximation)
    - [Polynomially approximable resolvent point](#polynomially-approximable-resolvent-point)
      - [Resolvent propagation across a complementary component](#resolvent-propagation-across-a-complementary-component)
    - [Elementary polynomial approximation on a square](#elementary-polynomial-approximation-on-a-square)
    - [Polynomial approximation of the reciprocal on a proper circular arc](#polynomial-approximation-of-the-reciprocal-on-a-proper-circular-arc)
      - [Explicit polynomial approximation of the reciprocal on the left semicircle](#explicit-polynomial-approximation-of-the-reciprocal-on-the-left-semicircle)
    - [Polynomial approximation obstruction on a punctured circle](#polynomial-approximation-obstruction-on-a-punctured-circle)
    - [Pointwise approximation by a Runge exhaustion](#pointwise-approximation-by-a-runge-exhaustion)
- [Winding number](#winding-number)
  - [Winding number of a continuous closed path](#winding-number-of-a-continuous-closed-path)
    - [Continuous logarithm lifting criterion](#continuous-logarithm-lifting-criterion)
- [Homotopy invariance of winding number](#homotopy-invariance-of-winding-number)
  - [Dominated perturbation preserves winding number](#dominated-perturbation-preserves-winding-number)
  - [Winding-number proof of the fundamental theorem of algebra](#winding-number-proof-of-the-fundamental-theorem-of-algebra)
  - [Winding-number proof of the no-retraction theorem](#winding-number-proof-of-the-no-retraction-theorem)
- [Bromwich contour](#bromwich-contour)
  - [Bromwich inversion with a square-root branch cut](#bromwich-inversion-with-a-square-root-branch-cut)
- [Branch point](#branch-point)
  - [Algebraic branch point](#algebraic-branch-point)
  - [Branch of a multivalued function](#branch-of-a-multivalued-function)
  - [Monodromy reflection at a square-root branch point](#monodromy-reflection-at-a-square-root-branch-point)
    - [Translation generated by two square-root monodromy reflections](#translation-generated-by-two-square-root-monodromy-reflections)
- [Complex number](#complex-number)
  - [Polar form of a complex number](#polar-form-of-a-complex-number)
    - [Root of a complex number](#root-of-a-complex-number)
  - [Complex modulus](#complex-modulus)
  - [Imaginary unit](#imaginary-unit)
  - [Real part](#real-part)
  - [Imaginary part](#imaginary-part)
  - [Euler's formula](#euler-s-formula)
  - [Modulus](#modulus)
  - [Complex conjugate](#complex-conjugate)
    - [Complex conjugation](#complex-conjugation)
      - [Schwarz conjugation of a spectral function](#schwarz-conjugation-of-a-spectral-function)
  - [Argument (complex analysis)](#argument-complex-analysis)
  - [Complex plane](#complex-plane)
    - [Finite-hole neighborhoods of a planar compact set](#finite-hole-neighborhoods-of-a-planar-compact-set)
    - [Complex coordinate](#complex-coordinate)
    - [Real linear equation of a line in the complex plane](#real-linear-equation-of-a-line-in-the-complex-plane)
    - [Imaginary axis](#imaginary-axis)
    - [Complex unit circle](#complex-unit-circle)
- [Isolated singularity](isolated-singularity.md)
  - [Classification of isolated singularities](isolated-singularity.md#classification-of-isolated-singularities)
    - [Removable singularity](isolated-singularity.md#removable-singularity)
      - [Riemann removable singularity theorem](isolated-singularity.md#riemann-removable-singularity-theorem)
      - [Removable singularity at infinity](isolated-singularity.md#removable-singularity-at-infinity)
      - [Uniform L2 circle bound for a removable singularity](isolated-singularity.md#uniform-l2-circle-bound-for-a-removable-singularity)
    - [Pole](isolated-singularity.md#pole)
      - [Simple pole](isolated-singularity.md#simple-pole)
      - [Double pole](isolated-singularity.md#double-pole)
      - [Meromorphic function](isolated-singularity.md#meromorphic-function)
        - [Spherical derivative of a meromorphic function](isolated-singularity.md#spherical-derivative-of-a-meromorphic-function)
          - [Finite spherical area criterion for an isolated singularity](isolated-singularity.md#finite-spherical-area-criterion-for-an-isolated-singularity)
        - [Algebraic addition theorem](isolated-singularity.md#algebraic-addition-theorem)
          - [Simply periodic entire function without an algebraic addition theorem](isolated-singularity.md#simply-periodic-entire-function-without-an-algebraic-addition-theorem)
        - [Meromorphic functions on the sphere are rational](isolated-singularity.md#meromorphic-functions-on-the-sphere-are-rational)
        - [Mittag-Leffler's theorem](isolated-singularity.md#mittag-leffler-s-theorem)
        - [Polynomial growth forces a meromorphic function to be rational](isolated-singularity.md#polynomial-growth-forces-a-meromorphic-function-to-be-rational)
        - [Nevanlinna theory](isolated-singularity.md#nevanlinna-theory)
          - [Ahlfors covering surface theory](isolated-singularity.md#ahlfors-covering-surface-theory)
            - [Length-area exhaustion of the complex plane](isolated-singularity.md#length-area-exhaustion-of-the-complex-plane)
            - [Ahlfors second fundamental theorem](isolated-singularity.md#ahlfors-second-fundamental-theorem)
              - [Ahlfors five islands theorem](isolated-singularity.md#ahlfors-five-islands-theorem)
            - [Island of a meromorphic function](isolated-singularity.md#island-of-a-meromorphic-function)
              - [Simple island](isolated-singularity.md#simple-island)
            - [Average sheet number](isolated-singularity.md#average-sheet-number)
          - [Nevanlinna second main theorem](isolated-singularity.md#nevanlinna-second-main-theorem)
            - [Nevanlinna second main theorem in the unit disc](isolated-singularity.md#nevanlinna-second-main-theorem-in-the-unit-disc)
            - [Five values force infinitely many simple preimages](isolated-singularity.md#five-values-force-infinitely-many-simple-preimages)
          - [Nevanlinna logarithmic derivative lemma](isolated-singularity.md#nevanlinna-logarithmic-derivative-lemma)
            - [Derivative growth outside a finite-measure set](isolated-singularity.md#derivative-growth-outside-a-finite-measure-set)
          - [Nevanlinna ramification index](isolated-singularity.md#nevanlinna-ramification-index)
          - [Nevanlinna deficiency](isolated-singularity.md#nevanlinna-deficiency)
            - [Simultaneous deficiency and ramification for an exponential polynomial](isolated-singularity.md#simultaneous-deficiency-and-ramification-for-an-exponential-polynomial)
          - [Nevanlinna first main theorem](isolated-singularity.md#nevanlinna-first-main-theorem)
          - [Nevanlinna characteristic](isolated-singularity.md#nevanlinna-characteristic)
            - [Growth order of a meromorphic function](isolated-singularity.md#growth-order-of-a-meromorphic-function)
              - [Counting-order exceptions for a finite-order meromorphic function](isolated-singularity.md#counting-order-exceptions-for-a-finite-order-meromorphic-function)
            - [Rational composition law for the Nevanlinna characteristic](isolated-singularity.md#rational-composition-law-for-the-nevanlinna-characteristic)
          - [Nevanlinna integrated counting function](isolated-singularity.md#nevanlinna-integrated-counting-function)
            - [Truncated Nevanlinna counting function](isolated-singularity.md#truncated-nevanlinna-counting-function)
          - [Nevanlinna proximity function](isolated-singularity.md#nevanlinna-proximity-function)
        - [Meromorphic function as a holomorphic map to the Riemann sphere](isolated-singularity.md#meromorphic-function-as-a-holomorphic-map-to-the-riemann-sphere)
          - [Single-pole criterion for a spherical coordinate](isolated-singularity.md#single-pole-criterion-for-a-spherical-coordinate)
        - [Rational map (complex analysis)](isolated-singularity.md#rational-map-complex-analysis)
          - [Rational covering maps of the projective line](isolated-singularity.md#rational-covering-maps-of-the-projective-line)
          - [Common-factor reduction of a rational map](isolated-singularity.md#common-factor-reduction-of-a-rational-map)
          - [Rotational symmetry of a rational map](isolated-singularity.md#rotational-symmetry-of-a-rational-map)
            - [Axially equivariant monomial rational map](isolated-singularity.md#axially-equivariant-monomial-rational-map)
          - [Wronskian of a rational map](isolated-singularity.md#wronskian-of-a-rational-map)
          - [Angular Jacobian of a rational map](isolated-singularity.md#angular-jacobian-of-a-rational-map)
        - [Rational function](isolated-singularity.md#rational-function)
          - [Padé approximant](isolated-singularity.md#pade-approximant)
          - [Partial fraction decomposition](isolated-singularity.md#partial-fraction-decomposition)
            - [Reciprocal-polynomial root identities](isolated-singularity.md#reciprocal-polynomial-root-identities)
          - [Order of vanishing](isolated-singularity.md#order-of-vanishing)
      - [Exponential of a pole is an essential singularity](isolated-singularity.md#exponential-of-a-pole-is-an-essential-singularity)
    - [Essential singularity](isolated-singularity.md#essential-singularity)
      - [Casorati-Weierstrass theorem](isolated-singularity.md#casorati-weierstrass-theorem)
  - [Non-isolated singularity](isolated-singularity.md#non-isolated-singularity)
    - [Reciprocal cosine with accumulating poles](isolated-singularity.md#reciprocal-cosine-with-accumulating-poles)
  - [Zeros and poles](isolated-singularity.md#zeros-and-poles)
- [Contour integration](#contour-integration)
  - [Cauchy transform](#cauchy-transform)
    - [Paired radial jump of a continuous Cauchy transform](#paired-radial-jump-of-a-continuous-cauchy-transform)
  - [Pochhammer contour](#pochhammer-contour)
  - [Complex integration contour](#complex-integration-contour)
  - [Complex contour](#complex-contour)
  - [Contour rotation](#contour-rotation)
  - [Keyhole contour](#keyhole-contour)
  - [Contour integral](#contour-integral)
  - [Estimation lemma](#estimation-lemma)
  - [Uniform convergence and contour integration](#uniform-convergence-and-contour-integration)
  - [Contour shifting](#contour-shifting)
  - [Period obstruction to a holomorphic antiderivative](#period-obstruction-to-a-holomorphic-antiderivative)
  - [Jordan's lemma](#jordan-s-lemma)
    - [Alternating sine series with a quadratic denominator](#alternating-sine-series-with-a-quadratic-denominator)
  - [Complex line integral estimate](#complex-line-integral-estimate)
  - [Hankel contour](#hankel-contour)
    - [Hankel analytic continuation](#hankel-analytic-continuation)
    - [Residue extraction by a Hankel contour](#residue-extraction-by-a-hankel-contour)
      - [Cancellation of positive-integer gamma singularities on a Hankel contour](#cancellation-of-positive-integer-gamma-singularities-on-a-hankel-contour)
- [Univalent function](#univalent-function)
  - [Area theorem (conformal mapping)](#area-theorem-conformal-mapping)
  - [Normalized univalent function](#normalized-univalent-function)
    - [Second coefficient bound for normalized univalent functions](#second-coefficient-bound-for-normalized-univalent-functions)
    - [Odd square-root transform of a normalized univalent function](#odd-square-root-transform-of-a-normalized-univalent-function)
  - [A univalent function has nonzero derivative](#a-univalent-function-has-nonzero-derivative)
  - [Locally uniform limit of univalent functions](#locally-uniform-limit-of-univalent-functions)
  - [Koebe function](#koebe-function)
  - [Boundary logarithmic mean of a univalent function](#boundary-logarithmic-mean-of-a-univalent-function)
- [Liouville theorem](#liouville-theorem)
  - [Entire function confined to a half-plane is constant](#entire-function-confined-to-a-half-plane-is-constant)
  - [One-sided product bound for an entire function](#one-sided-product-bound-for-an-entire-function)
  - [Dense image of a nonconstant entire function](#dense-image-of-a-nonconstant-entire-function)
  - [Entire function under a horizontal inverse-square-root bound](#entire-function-under-a-horizontal-inverse-square-root-bound)
  - [Polynomial growth theorem for entire functions](#polynomial-growth-theorem-for-entire-functions)
- [Cauchy derivative formula](#cauchy-derivative-formula)
  - [Recovering an analytic derivative from the boundary real part](#recovering-an-analytic-derivative-from-the-boundary-real-part)
  - [Lipschitz bound inside a bounded analytic half-plane](#lipschitz-bound-inside-a-bounded-analytic-half-plane)
- [Locally uniform convergence of holomorphic functions](#locally-uniform-convergence-of-holomorphic-functions)
- [Schwarz reflection principle](#schwarz-reflection-principle)
- [Upper half-plane self-map](#upper-half-plane-self-map)
- [Argument principle](#argument-principle)
  - [Radial crossing test for polynomial root counts](#radial-crossing-test-for-polynomial-root-counts)
  - [Quarter-sector winding test for a real quartic](#quarter-sector-winding-test-for-a-real-quartic)
  - [Rouché's theorem](#rouche-s-theorem)
    - [Rouché localization of polynomial roots](#rouche-localization-of-polynomial-roots)
    - [Hurwitz's theorem](#hurwitz-s-theorem)
    - [Open mapping theorem (complex analysis)](#open-mapping-theorem-complex-analysis)
      - [Maximum modulus principle from the complex open mapping theorem](#maximum-modulus-principle-from-the-complex-open-mapping-theorem)
    - [Unit-disc image from a boundary modulus lower bound](#unit-disc-image-from-a-boundary-modulus-lower-bound)
  - [Integer residue of a logarithmic derivative](#integer-residue-of-a-logarithmic-derivative)
- [Meromorphic function with prescribed zeros and poles](#meromorphic-function-with-prescribed-zeros-and-poles)
- [Maximum modulus principle](#maximum-modulus-principle)
  - [Hadamard three-circle theorem](#hadamard-three-circle-theorem)
  - [Phragmén–Lindelöf principle](#phragmen-lindelof-principle)
  - [Maximum modulus principle on a bounded domain](#maximum-modulus-principle-on-a-bounded-domain)
    - [Bounded half-plane maximum principle](#bounded-half-plane-maximum-principle)
- [Mean value property for holomorphic functions](#mean-value-property-for-holomorphic-functions)
- [Dirichlet beta function](#dirichlet-beta-function)
  - [Special values of the Dirichlet beta function](#special-values-of-the-dirichlet-beta-function)
  - [Dirichlet beta reflection formula](#dirichlet-beta-reflection-formula)
- [Identity theorem](#identity-theorem)
- [Residue at infinity from an asymptotic constant](#residue-at-infinity-from-an-asymptotic-constant)
- [Large-circle contour estimate](#large-circle-contour-estimate)
- [Fuchsian differential equation](#fuchsian-differential-equation)
  - [Accessory parameter](#accessory-parameter)
  - [Regular singular point](#regular-singular-point)
    - [Logarithmically divergent derivative at a regular singular endpoint](#logarithmically-divergent-derivative-at-a-regular-singular-endpoint)
    - [Frobenius method](#frobenius-method)
      - [Undetermined coefficient at Frobenius resonance](#undetermined-coefficient-at-frobenius-resonance)
      - [Square-root reduction of a regular-singular differential equation](#square-root-reduction-of-a-regular-singular-differential-equation)
      - [Frobenius solution](#frobenius-solution)
      - [Hyperbolic reduction of a regular-singular differential equation](#hyperbolic-reduction-of-a-regular-singular-differential-equation)
      - [Terminating Frobenius series](#terminating-frobenius-series)
  - [Ordinary point criterion for a second-order equation](#ordinary-point-criterion-for-a-second-order-equation)
  - [Characteristic exponent at a regular singular point](#characteristic-exponent-at-a-regular-singular-point)
  - [Regular singular point criterion for a second-order equation](#regular-singular-point-criterion-for-a-second-order-equation)
    - [Regular singular point at infinity](#regular-singular-point-at-infinity)
    - [Logarithmic solution from a repeated Frobenius exponent](#logarithmic-solution-from-a-repeated-frobenius-exponent)
  - [Irregular singular point](#irregular-singular-point)
    - [Poincaré rank](#poincare-rank)
  - [Riemann's differential equation](#riemann-s-differential-equation)
    - [Papperitz symbol](#papperitz-symbol)
      - [Fuchs relation](#fuchs-relation)
      - [Möbius transformation of a Papperitz symbol](#mobius-transformation-of-a-papperitz-symbol)
      - [Dependent-variable rescaling of a Papperitz symbol](#dependent-variable-rescaling-of-a-papperitz-symbol)
  - [Gauss hypergeometric equation](#gauss-hypergeometric-equation)
    - [Euler's hypergeometric transformation](#euler-s-hypergeometric-transformation)
    - [Hypergeometric connection formula at one](#hypergeometric-connection-formula-at-one)
    - [Hypergeometric function](#hypergeometric-function)
      - [Euler integral for the hypergeometric function](#euler-integral-for-the-hypergeometric-function)
    - [Pfaff transformation](#pfaff-transformation)
    - [Second local hypergeometric solution](#second-local-hypergeometric-solution)
    - [Hypergeometric connection formula at infinity](#hypergeometric-connection-formula-at-infinity)
    - [Hypergeometric cancellation identity](#hypergeometric-cancellation-identity)
      - [Elementary specialization of a hypergeometric solution](#elementary-specialization-of-a-hypergeometric-solution)
        - [Hypergeometric cosine identity](#hypergeometric-cosine-identity)
        - [Hypergeometric sine identity](#hypergeometric-sine-identity)

## Nontangential limit

↑ **Parent:** [Complex analysis](complex-analysis.md)

A boundary limit taken while approaching within a cone that stays away from tangency. At zero in the [complex upper half-plane](#upper-half-plane-complex-analysis), every fixed cone $|\operatorname{Re}z|\leq A\operatorname{Im}z$ is allowed. A [nontangential limit](#nontangential-limit) need not be a limit along all paths approaching the boundary.

// Destination: analysis.bigb

### Stolz region

↑ **Parent:** [Nontangential limit](#nontangential-limit)

A fixed-aperture approach region at a boundary point of the [unit disc](topology.md#unit-disc). Its points approach the boundary point without becoming tangent to the circle. Convergence inside every such fixed region is a [nontangential limit](#nontangential-limit); the corresponding supremum defines a [non-tangential maximal function](analysis.md#non-tangential-maximal-function).

## Polynomial hull

↑ **Parent:** [Complex analysis](complex-analysis.md)

For a compact set $K\subset\mathbb C^n$, its polynomial hull is the set displayed, where $p$ ranges over all complex [multivariate polynomials](polynomial.md#multivariate-polynomial). It contains $K$. In one complex dimension, bounded complementary components are filled in: the [maximum modulus principle](#maximum-modulus-principle) bounds every [polynomial](polynomial.md) inside those components by its boundary values. Polynomial approximation and separation distinguish points outside the hull.

### Polynomial hull in one complex variable

↑ **Parent:** [Polynomial hull](#polynomial-hull)

For a [compact set](topology.md#compact-space) $K\subset\mathbb C$, its polynomial hull is $\widehat K=\{z:|P(z)|\le\sup_K|P|\text{ for every polynomial }P\}$. In one complex variable this is $K$ together with all bounded components of its complement. The [maximum modulus principle](#maximum-modulus-principle) proves inclusion of each filled hole. Conversely, polynomial approximation of an exterior pole by the [Runge approximation theorem](#runge-s-theorem) separates an exterior point from the filled compact set. The filled set has connected complement, which makes it the natural set for polynomial approximation of functions whose poles lie in the unbounded complementary component.

## Lower half-plane

↑ **Parent:** [Complex analysis](complex-analysis.md)

The [lower half-plane](#lower-half-plane) is the set of complex numbers with negative imaginary part. It is the reflection of the [complex upper half-plane](#upper-half-plane-complex-analysis) across the real axis.

## Holomorphic square root

↑ **Parent:** [Complex analysis](complex-analysis.md)

A holomorphic square root of a nonvanishing holomorphic function $f$ is a holomorphic function $g$ satisfying $g^2=f$. It exists locally, and globally exactly when the winding obstruction around every closed path vanishes.

### Holomorphic square root outside all polynomial roots

↑ **Parent:** [Holomorphic square root](#holomorphic-square-root)

An even-degree [polynomial](polynomial.md) with all roots in $|z|<R$ admits a [holomorphic square root](#holomorphic-square-root) throughout $|z|>R$. Factor out its even power of $z$ and use the convergent logarithm of each $1-a_j/z$ to construct it. Even degree removes the annular winding obstruction. The two choices differ by a global sign.

## Monodromy

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monodromy)

Monodromy is the change in a locally defined analytic object after analytic continuation around a closed path.

### Isomonodromic deformation

↑ **Parent:** [Monodromy](#monodromy)

A parameter deformation preserves generalized [monodromy](#monodromy) data, including [Stokes matrices](analysis.md#stokes-matrix) and [formal monodromy](#formal-monodromy) at irregular points. If normalized sectorial [matrices](vector-space.md#matrix) have parameter-independent jumps, $B=Y_zY^{-1}$ agrees across overlaps. Its finite singularities and growth at infinity determine it by complex analytic arguments. Compatibility of $Y_\lambda=AY$ and $Y_z=BY$ is precisely the displayed zero-curvature identity, obtained by differentiating both equations and subtracting.

### Formal monodromy

↑ **Parent:** [Monodromy](#monodromy)

An unramified formal [fundamental matrix](differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) $\widehat Y=\widehat G(\lambda)\lambda^\Theta e^{Q(\lambda)}$ acquires the right factor $e^{2\pi i\Theta}$ on a positive turn of the [logarithm](calculus.md#logarithm) branch. This is [formal monodromy](#formal-monodromy). It can be nontrivial even when the true equation has an entire [fundamental matrix](differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) and trivial actual [monodromy](#monodromy), because [Stokes matrices](analysis.md#stokes-matrix) compensate for it.

#### Formal monodromy correction to an entire-system Stokes product

↑ **Parent:** [Formal monodromy](#formal-monodromy)

When Stokes factors act on solution coefficient vectors, a full positive turn gives their ordered product equal to the inverse of [formal monodromy](#formal-monodromy) for a [polynomial](polynomial.md) system with no finite singularities. The true [fundamental matrix](differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) is entire, so its actual [monodromy](#monodromy) is trivial, but its normalized formal branch changes by $M_f$. Indeed, write $Y_{j+1}=Y_jS_j^{-1}$; then $Y_{N+1}=Y_1(S_N\cdots S_1)^{-1}$, whereas normalized continuation after the positive turn gives $Y_{N+1}=Y_1M_f$. Cancelling the invertible [fundamental matrix](differential-equation.md#fundamental-matrix-of-a-linear-differential-equation) proves the identity. The uncorrected product is identity only when $M_f=I$. For a cubic-exponential two-by-two system with $U=1,V=-1,P=1,R=2,d=3/2$, the formal exponent is $\theta=1/2$, so $M_f=-I$ and the Stokes product is $-I$.

### Monodromy eigenfunction Laurent representation

↑ **Parent:** [Monodromy](#monodromy)

For a linear [ordinary differential equation](differential-equation.md#ordinary-differential-equation) with [holomorphic](#complex-differentiability-at-a-point) coefficients on a punctured disc, analytic continuation of a basis gives an invertible [monodromy](#monodromy) matrix. A nonzero [eigenvector](linear-operator-theory.md#eigenvector) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda=e^{2\pi i\sigma}$ selects a solution $w$ for which $z^{-\sigma}w$ is single-valued and [holomorphic](#complex-differentiability-at-a-point). Its [Laurent series](analysis.md#laurent-series) gives $w=z^\sigma\sum_{n\in\mathbb Z}c_nz^n$. No regular-singular hypothesis is needed; infinitely many negative powers may occur.

## Cayley transform between the half-plane and disk

↑ **Parent:** [Complex analysis](complex-analysis.md)

The fractional linear maps

$$
w=\frac{z-1}{z+1},
\qquad
z=\frac{1+w}{1-w}
$$

map the right half-plane and unit disk conformally onto one another.

## Holomorphic logarithm

↑ **Parent:** [Complex analysis](complex-analysis.md)

A holomorphic logarithm of a nonvanishing holomorphic function $f$ is a holomorphic function $g$ with $e^g=f$. On a simply connected domain, every nonvanishing holomorphic function has one.

## Upper half-plane (complex analysis)

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_half-plane)

The complex upper half-plane is $\mathbb H=\{z\in\mathbb C:\operatorname{Im}z>0\}$.

### Conformal automorphism of the upper half-plane

↑ **Parent:** [Upper half-plane (complex analysis)](#upper-half-plane-complex-analysis)

A [conformal bijection](#biholomorphism) of the [complex upper half-plane](#upper-half-plane-complex-analysis) to itself is a real [Möbius transformation](group-theory.md#mobius-transformation) with $ad-bc>0$. Three distinct boundary values determine it uniquely. Its real derivative is positive away from its pole, and $\operatorname{Im}\phi(z)=(ad-bc)\operatorname{Im}z/|cz+d|^2$.

## Polylogarithm

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polylogarithm)

For $|z|<1$, the polylogarithm is $\operatorname{Li}_s(z)=\sum_{n\geq1}z^n/n^s$; contour formulas analytically continue it to a slit plane.

### Dilogarithm

↑ **Parent:** [Polylogarithm](#polylogarithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dilogarithm)

The dilogarithm is the order-two [polylogarithm](#polylogarithm), defined for $|z|<1$ by $\operatorname{Li}_2(z)=\sum_{n\geq1}z^n/n^2$. Its derivative is $-\operatorname{Log}(1-z)/z$, with a removable value at zero; a chosen [complex logarithm](analysis.md#complex-logarithm) branch gives its [analytic continuation](#analytic-continuation).

## Holomorphic function

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holomorphic_function)

A complex-valued [function](function.md) is holomorphic on an [open set](topology.md#open-set) when it has a complex [derivative](calculus.md#derivative) at every point of that set.

### Complex differentiability

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A complex-valued function is complex differentiable at a point if the displayed limit exists for arbitrary nonzero complex increments approaching zero. It is stronger than having directional derivatives along the real and imaginary axes: all approaches must agree. The two axis limits imply the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations). A function complex differentiable at every point of an open set is a [holomorphic function](#holomorphic-function) there.

### Nevanlinna class

↑ **Parent:** [Holomorphic function](#holomorphic-function)

The analytic Nevanlinna class consists of [holomorphic functions](#holomorphic-function) on the [unit disc](topology.md#unit-disc) with uniformly bounded means of their positive logarithmic modulus. Here $m$ is normalized angular measure. A bounded [holomorphic function](#holomorphic-function) belongs to this class, but the class also permits unbounded functions. It is the analytic version of [bounded characteristic](#bounded-characteristic).

#### Bounded characteristic

↑ **Parent:** [Nevanlinna class](#nevanlinna-class)

A [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc) has bounded characteristic when $\sup_{r<1}\int\log^+|f(r\xi)|\,dm(\xi)<\infty$, where $\log^+t=\max(0,\log t)$. Thus it belongs to the [Nevanlinna class](#nevanlinna-class). A general [meromorphic function](isolated-singularity.md#meromorphic-function) requires the additional pole-counting term in its characteristic; the displayed analytic definition has no such term.

##### Quotient characterization of bounded characteristic

↑ **Parent:** [Bounded characteristic](#bounded-characteristic)

A [meromorphic function](isolated-singularity.md#meromorphic-function) on the [unit disc](topology.md#unit-disc) has [bounded characteristic](#bounded-characteristic) if and only if it has this representation. Its pole [Blaschke product](#blaschke-product) $B$ makes $g=Bf$ analytic with bounded positive logarithmic means. The [least harmonic majorant by expanding disk lifts](partial-differential-equation.md#least-harmonic-majorant-by-expanding-disk-lifts) gives $H\ge\log^+|g|$. A [harmonic conjugate](partial-differential-equation.md#harmonic-conjugate) gives an analytic $A$ with $\operatorname{Re}A=H$, so $u=ge^{-A}$ and $v=Be^{-A}$ are bounded. Conversely the [Nevanlinna first main theorem](isolated-singularity.md#nevanlinna-first-main-theorem) bounds the characteristic of $u/v$ by that of $u$ and $1/v$, hence by a constant.

### Multiplicity of a zero

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A [holomorphic function](#holomorphic-function) that is not identically zero has a zero of multiplicity $m$ at $z_0$ if $f(z)=(z-z_0)^m h(z)$ for a [holomorphic function](#holomorphic-function) $h$ with $h(z_0)\ne0$. Its [Taylor series](calculus.md#taylor-series) identifies $m$ as the first nonzero coefficient index. Logarithmic differentiation gives $f'/f=m/(z-z_0)+h'/h$, so the [residue](analysis.md#residue) of $f'/f$ is $m$. Counting zeros with [zero multiplicity](#multiplicity-of-a-zero) repeats that zero $m$ times.

### Periodic holomorphic descent through the exponential map

↑ **Parent:** [Holomorphic function](#holomorphic-function)

If a [holomorphic function](#holomorphic-function) of $w$ is periodic with period one, then $F((\log z)/(2\pi i))$ is independent of the choice of a local logarithm: two choices differ by $2\pi i k$, hence their arguments differ by an integer. Consequently it defines a holomorphic function on the image of the original domain under $w\mapsto e^{2\pi iw}$, provided that domain is invariant under integer shifts. Local logarithms prove holomorphy across an arbitrary global branch cut. Singularities on an integer lattice all map to $z=1$.

### Constant-modulus holomorphic function

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A [holomorphic function](#holomorphic-function) with constant modulus on a connected [domain](topology.md#domain-mathematical-analysis) is constant. If $h=u+iv$ and $u^2+v^2=c^2>0$, differentiation and the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) give $uu_x+vv_x=0$ and $-uv_x+vu_x=0$. Their coefficient [determinant](linear-algebra.md#determinant) is $-c^2$, so $u_x=v_x=0$, and all first [derivatives](calculus.md#derivative) vanish. When $c=0$, the conclusion is immediate. Consequently two nonvanishing [holomorphic functions](#holomorphic-function) with equal moduli differ by a single constant phase on a connected [domain](topology.md#domain-mathematical-analysis).

### Banach-space-valued holomorphic function

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A map from an open subset of $\mathbb C$ to a complex [Banach space](banach-space.md) is holomorphic when the displayed limit exists in the Banach-space norm at every point. A norm-convergent power series is holomorphic inside its radius of convergence: on every smaller disk the series of derivatives converges uniformly by the geometric coefficient bound, allowing differentiation term by term. Applying a [continuous linear functional](topological-vector-space.md#continuous-linear-functional) produces an ordinary scalar [holomorphic function](#holomorphic-function). Scalar Cauchy identities therefore imply the corresponding vector-integral identities when bounded linear functionals separate points, as they do by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem).

#### Spectral-radius maximum principle

↑ **Parent:** [Banach-space-valued holomorphic function](#banach-space-valued-holomorphic-function)

For a [Banach algebra](banach-algebra.md)-valued [holomorphic function](#holomorphic-function), set $p_n(w)=\|f(w)^{2^n}\|^{1/2^n}$. These [continuous](calculus.md#continuous-function) functions decrease to the [spectral radius](analysis.md#spectral-radius) by the [spectral radius formula](analysis.md#spectral-radius-formula). If $M=\sup_{\partial K}r(f(w))$, the [continuous](calculus.md#continuous-function) functions $\max\{p_n,M\}$ on $\partial K$ decrease to the [continuous](calculus.md#continuous-function) constant $M$. The [Dini theorem](real-analysis.md#dini-s-theorem) gives [uniform convergence](real-analysis.md#uniform-convergence). Apply the [norm maximum principle for a Banach-space-valued holomorphic function](#norm-maximum-principle-for-a-banach-space-valued-holomorphic-function) to each power, and then let $n\to\infty$. This proof does not assume [continuity](calculus.md#continuous-function) of [spectral radius](analysis.md#spectral-radius).

#### Norm maximum principle for a Banach-space-valued holomorphic function

↑ **Parent:** [Banach-space-valued holomorphic function](#banach-space-valued-holomorphic-function)

For a [compact](topology.md#compact-space) set $K$ in the domain, a norming [bounded linear functional](topological-vector-space.md#continuous-linear-functional) at $f(z)$ reduces the assertion to the scalar [maximum modulus principle](#maximum-modulus-principle). If $z$ lies inside $K$, use its [connected](geometry-and-topology.md#connected-space) component of the [interior](topology.md#interior-topology); that component's [boundary](topology.md#boundary-of-a-set) lies in $\partial K$. If $z\in\partial K$, the inequality is immediate. No smoothness or connectedness assumption on $K$ is required.

### Prescribed zeros in a plane domain via Runge approximation

↑ **Parent:** [Holomorphic function](#holomorphic-function)

Every [closed discrete subset](topology.md#closed-discrete-subset) of a plane [domain](topology.md#domain-mathematical-analysis) is the zero set of a [holomorphic function](#holomorphic-function), with assigned finite positive multiplicities if desired. Exhaust the domain by relatively filled compact sets. For a prescribed point outside an earlier compact, choose a rational factor with that zero and its possible pole outside the domain in the same complementary component. A slit joining zero and pole allows a [holomorphic logarithm](#holomorphic-logarithm) near the earlier compact. Approximate that logarithm by [Runge theorem](#runge-s-theorem) and multiply the rational factor by the negative exponential of the approximant. The resulting factors tend to one with summable errors on each compact. Their [infinite product](real-analysis.md#infinite-product) has the prescribed zeros and no additional zeros.

// Destination: analysis.bigb

### Antiholomorphic function

↑ **Parent:** [Holomorphic function](#holomorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiholomorphic_function)

A complex-valued function is antiholomorphic when its complex conjugate is a [holomorphic function](#holomorphic-function). In one complex dimension it locally depends on $\overline z$ and satisfies $\partial_zf=0$. A nonconstant antiholomorphic map reverses the orientation induced by the complex coordinates. Thus complex conjugating a holomorphic sphere map reverses its [topological degree](geometry-and-topology.md#topological-degree) while preserving its Dirichlet energy.

### Holomorphic convex hull

↑ **Parent:** [Holomorphic function](#holomorphic-function)

For [compact](topology.md#compact-space) $K$ in a plane domain $\Omega$, its [holomorphic convex hull](#holomorphic-convex-hull) is

$$
\widehat K_{\Omega}=\{w\in\Omega:|f(w)|\le\sup_K|f|\text{ for every }f\in\mathcal O(\Omega)\}.
$$

It is $K$ together with the components of $\widehat{\mathbb C}\setminus K$ lying entirely in $\Omega$. Inclusion of those components follows from the [maximum modulus principle](#maximum-modulus-principle). For exclusion, suppose $w$ lies in a complementary component meeting $\widehat{\mathbb C}\setminus\Omega$. Choose an allowed [pole](isolated-singularity.md#pole) there. The open-and-closed resolvent argument in the proof of [Runge theorem](#runge-s-theorem) approximates $(z-w)^{-1}$ uniformly on $K$ by functions $h$ [holomorphic](#complex-differentiability-at-a-point) on $\Omega$. Then $1-(z-w)h(z)$ has value one at $w$ and arbitrarily small modulus on $K$, separating $w$ from the hull. For $\Omega=\mathbb C$, this is the [polynomial hull in one complex variable](#polynomial-hull-in-one-complex-variable).

### Blaschke product

↑ **Parent:** [Holomorphic function](#holomorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Blaschke_product)

For zeros $a_n$ in the [unit disc](topology.md#unit-disc) satisfying $\sum_n(1-|a_n|)<\infty$, with $m$ occurrences at zero, a [Blaschke product](#blaschke-product) is

$$
B(z)=\lambda z^m\prod_{a_n\ne0}\frac{|a_n|}{a_n}\frac{a_n-z}{1-\overline{a_n}z},\qquad |\lambda|=1.
$$

For $|z|\le R<1$ and $a\ne0$, the normalized factor $b_a$ satisfies $|1-b_a(z)|\le(1-|a|)(1+R)/(1-R)$. The product therefore converges locally uniformly; outside its prescribed zeros the logarithms of its tail factors converge absolutely, so it has no additional zeros. Every finite product has modulus at most one in the disc, and the limit does too. Since $|b_a(w)|$ is [pseudohyperbolic distance](geometry-and-topology.md#pseudohyperbolic-distance) from $w$ to $a$, its modulus can be estimated geometrically.

#### Interior zero count for a finite Blaschke product minus a constant

↑ **Parent:** [Blaschke product](#blaschke-product)

A finite [Blaschke product](#blaschke-product) is holomorphic across the unit circle and has modulus one there. For a constant $a$ with $|a|<1$, [Rouché's theorem](#rouche-s-theorem) makes $B-a$ and $B$ have the same number of interior zeros, counting [multiplicity](polynomial.md#multiplicity-mathematics). Each factor contributes its prescribed zero; the poles are outside the closed disk.

#### Hyperbolic zero estimate for a Blaschke product

↑ **Parent:** [Blaschke product](#blaschke-product)

Use curvature-minus-one [Hyperbolic distance in the Poincare disc](geometry-and-topology.md#hyperbolic-distance-in-the-poincare-disc). Each [Blaschke factor](group-theory.md#blaschke-factor) has modulus $\tanh(\rho(w,a)/2)=(1-t)/(1+t)$, with $t=e^{-\rho(w,a)}$. For $0\le t<1$, differentiating shows $\log[(1+t)/(1-t)]\ge2t$. Sum this logarithmic inequality over the zero factors and pass to the [Blaschke product](#blaschke-product) by [locally uniform convergence](real-analysis.md#locally-uniform-convergence). At a prescribed zero, its modulus vanishes and the bound is immediate. All sums count [multiplicities](polynomial.md#multiplicity-mathematics).

#### Vanishing absolute logarithmic mean characterization of Blaschke products

↑ **Parent:** [Blaschke product](#blaschke-product)

For a [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc), this boundary condition characterizes [Blaschke products](#blaschke-product), including unimodular constants. The nondecreasing radial means of the nonnegative [subharmonic function](partial-differential-equation.md#subharmonic-function) $\log^+|f|$ must vanish, so $|f|\le1$. In the [Blaschke factorization of a bounded holomorphic function](#blaschke-factorization-of-a-bounded-holomorphic-function) $f=Bg$, both logarithmic means tend to zero. The [mean value property for harmonic functions](partial-differential-equation.md#mean-value-property-for-harmonic-functions) applied to $\log|g|$ gives $|g(0)|=1$, and the [maximum modulus principle](#maximum-modulus-principle) makes $g$ unimodular constant. The converse follows from the [radial logarithmic mean of a Blaschke product](#radial-logarithmic-mean-of-a-blaschke-product). Omitting the outer absolute value changes the condition: $e^z$ has zero mean logarithmic modulus, but is not a [Blaschke product](#blaschke-product).

#### Blaschke factorization of a bounded holomorphic function

↑ **Parent:** [Blaschke product](#blaschke-product)

Every nonzero bounded [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc) has this factorization, with $B$ the [Blaschke product](#blaschke-product) of its zeros and $g$ zero-free and [holomorphic](#complex-differentiability-at-a-point). The [Blaschke condition](#blaschke-condition) follows from [Jensen's formula](#jensen-s-formula). Dividing by any finite partial zero product gives a [holomorphic function](#holomorphic-function); the [maximum modulus principle](#maximum-modulus-principle) and the finite product's boundary modulus one bound that quotient by $\|f\|_\infty$. [Locally uniform convergence](real-analysis.md#locally-uniform-convergence) of the partial products gives the same bound for $g$, with removable extensions at their zeros. This factorization alone does not make $g$ constant or a full inner-outer factorization.

#### Radial logarithmic mean of a Blaschke product

↑ **Parent:** [Blaschke product](#blaschke-product)

For $B(z)=\lambda z^m\prod_n b_{a_n}(z)$ with nonzero zeros $a_n$ counted with [multiplicity](polynomial.md#multiplicity-mathematics), [Jensen's formula](#jensen-s-formula) gives the displayed identity. The negative logarithms of partial products increase, so the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) permits termwise integration. The [Blaschke condition](#blaschke-condition) implies $\sum_n-\log|a_n|<\infty$, which dominates the absolute summands. The [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) therefore gives a limit of zero as $r\uparrow1$. Since $|B|\le1$, the mean of $|\log|B||$ tends to zero as well.

#### Automorphy character of an orbit Blaschke product

↑ **Parent:** [Blaschke product](#blaschke-product)

Let a [group](group.md) $G$ of [Möbius transformations](group-theory.md#mobius-transformation) of the [unit disk](geometry-and-topology.md#unit-disk) have an orbit satisfying the [Blaschke condition](#blaschke-condition), counted once per distinct orbit point. For its [Blaschke product](#blaschke-product) $B$, invariance of the [pseudohyperbolic distance](geometry-and-topology.md#pseudohyperbolic-distance) and permutation of the orbit give $|B(Tz)|=|B(z)|$. The ratio $B(Tz)/B(z)$ extends across its zeros and has modulus one, so the [open mapping theorem](#open-mapping-theorem-complex-analysis) makes it a constant $\chi(T)$. Composition gives a [group homomorphism](group-theory.md#group-homomorphism) $\chi:G\to\{\lambda:|\lambda|=1\}$. It is essential to compare moduli of the products: two arbitrary bounded [holomorphic functions](#holomorphic-function) with identical zeros need not have constant quotient.

#### Blaschke condition

↑ **Parent:** [Blaschke product](#blaschke-product)

The [Blaschke condition](#blaschke-condition) for a sequence in the [unit disc](topology.md#unit-disc) is $\sum_n(1-|a_n|)<\infty$. It characterizes the zero sequences, counted with [multiplicity](polynomial.md#multiplicity-mathematics), of nonzero bounded [holomorphic functions](#holomorphic-function). Sufficiency follows by constructing the [Blaschke product](#blaschke-product). For necessity, [Jensen's formula](#jensen-s-formula) gives $\sum_{|a_n|<r}\log(r/|a_n|)\le\log\|f\|_\infty-\log|f(0)|$ when $f(0)\ne0$. Letting $r\uparrow1$ and using $-\log|a|\ge1-|a|$ proves the condition. A finite zero at zero is factored out first. Equivalently, for the curvature-minus-one [hyperbolic metric](geometry-and-topology.md#hyperbolic-metric), $\sum_ne^{-\rho(0,a_n)}<\infty$, since $e^{-\rho(0,a)}=(1-|a|)/(1+|a|)$.

##### Blaschke sequence

↑ **Parent:** [Blaschke condition](#blaschke-condition)

A sequence in the [unit disc](topology.md#unit-disc), counted with [multiplicity](polynomial.md#multiplicity-mathematics), is a Blaschke sequence when it satisfies the [Blaschke condition](#blaschke-condition). The zeros of every nonzero bounded [holomorphic function](#holomorphic-function) form such a sequence: [Jensen's formula](#jensen-s-formula) bounds $\sum_{|a_n|<r}\log(r/|a_n|)$ uniformly as $r\uparrow1$, and $1-|a|\le-\log|a|$ gives the assertion. There are only finitely many zeros at the origin, which can be factored out first.

<h3 id="jensen-s-formula">Jensen's formula</h3>

↑ **Parent:** [Holomorphic function](#holomorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jensen's_formula)

For a [holomorphic function](#holomorphic-function) nonzero at zero and without boundary zeros, the formula relates its interior zeros, counted by multiplicity, to the circle mean of its logarithmic modulus. Divide out the finite interior zero factors; the remaining logarithmic modulus is [harmonic](partial-differential-equation.md#harmonic-function), and each zero contributes $\log(R/|a_j|)$ by the [harmonic](partial-differential-equation.md#harmonic-function) mean-value formula. Boundary radii follow by limits where appropriate.

#### Poisson-Jensen formula

↑ **Parent:** [Jensen's formula](#jensen-s-formula)

For a [meromorphic function](isolated-singularity.md#meromorphic-function) with no zero or [pole](isolated-singularity.md#pole) on $|w|=R$, set $G_R(z,a)=\log|(R^2-\overline az)/(R(z-a))|$. At source points that are neither zeros nor [poles](isolated-singularity.md#pole), the displayed identity expresses its logarithmic modulus as the Poisson integral of its boundary values, minus its zero Green potentials plus its [pole](isolated-singularity.md#pole) Green potentials. The Poisson kernel is $(R^2-|z|^2)/|Re^{i\theta}-z|^2$ with normalized angular measure. Subtracting the corresponding logarithmic singularities leaves a harmonic function, so the harmonic Poisson formula proves the identity. At zero it reduces to [Jensen's formula](#jensen-s-formula).

##### Annular spherical Jensen formula

↑ **Parent:** [Poisson-Jensen formula](#poisson-jensen-formula)

For a [meromorphic function](isolated-singularity.md#meromorphic-function) near $0<|z|\le1$, and a target $a$ off its image of the unit circle, let $u_a=-\log k(f,a)$ for the [chordal metric](#chordal-metric), $M_a(s)$ its normalized angular mean, and $I(a)=M_a'(1)$. The weighted spherical area $T(r)=(4\pi)^{-1}\int_{r<|z|<1}\log(|z|/r)(f^{\#}_{\mathrm{round}})^2\,dA$ satisfies the displayed formula, where $N$ counts $a$-points with [multiplicity](polynomial.md#multiplicity-mathematics) and weight $\log(|z|/r)$ and $\overline m=M_a(r)-M_a(1)$. Indeed $\Delta u_a=(f^{\#}_{\mathrm{round}})^2/2-2\pi\sum\deg_z(f)\delta_z$, and [Green's second identity](partial-differential-equation.md#green-second-identity) with the radial logarithmic weight proves the formula. The angular mean must include $1/(2\pi)$.

#### Jensen zero-count bound

↑ **Parent:** [Jensen's formula](#jensen-s-formula)

Every zero in the smaller disk contributes at least $\log(R/r)$ in [Jensen's formula](#jensen-s-formula). Bounding the outer circle average by its maximum proves the estimate. With $R=2r$, an exponential $O(r\log r)$ maximum bound gives an $O(r\log r)$ zero count.

##### Lattice zeros force quadratic exponential growth

↑ **Parent:** [Jensen zero-count bound](#jensen-zero-count-bound)

A nonzero [entire function](#entire-function) vanishing at every nonzero point of the integer lattice has at least a constant times $R^2$ zeros in the disc of radius $R/2$. Each contributes at least $\log2$ to [Jensen's formula](#jensen-s-formula) at radius $R$. Therefore the circle mean of $\log|F|$, and hence the logarithm of its maximum modulus, is bounded below by $cR^2$ for all sufficiently large boundary-zero-free radii. Choosing maximizing points yields $|F(z_j)|>e^{c'|z_j|^2}$ for some $c'>0$ and $|z_j|\to\infty$. If zero is also a zero, first factor out its finite multiplicity; the additional $m\log R$ term does not weaken the quadratic lower bound.

### Holomorphic primitive

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A holomorphic primitive of $f$ is a [holomorphic function](#holomorphic-function) $F$ with $F'=f$. A holomorphic $f$ on a domain has such a primitive exactly when its integrals around all closed piecewise smooth curves vanish. Integrating from a fixed starting point then constructs a path-independent primitive.

### Complex differentiability at a point

↑ **Parent:** [Holomorphic function](#holomorphic-function)

A function is complex differentiable at $p$ when

$$
f(p+h)=f(p)+f'(p)h+o(|h|).
$$

If $f'(p)\ne0$, the real derivative is multiplication by a nonzero complex number, hence a rotation and scaling; this is the local source of angle preservation by holomorphic maps.

### Space of holomorphic functions

↑ **Parent:** [Holomorphic function](#holomorphic-function)

For an [open set](topology.md#open-set) $U\subseteq\mathbb C$, the space $\mathcal O(U)$ consists of all [holomorphic functions](#holomorphic-function) on $U$. Its standard topology is locally uniform convergence, equivalently the [compact-open topology](real-analysis.md#compact-open-topology) defined by the seminorms $f\mapsto\sup_{z\in K}|f(z)|$ for compact $K\subset U$.

#### Weighted holomorphic norm on a shrinking time domain

↑ **Parent:** [Space of holomorphic functions](#space-of-holomorphic-functions)

Let $R,\alpha>0$ and $\mathcal C_\alpha=\{(x,t)\in\mathbb C^2:|x|<R,\;|t|<\alpha(1-|x|/R)\}$. The displayed [norm](functional-analysis.md#norm) makes the [holomorphic functions](#holomorphic-function) with finite norm a [Banach space](banach-space.md). Finiteness forces $u(x,0)=0$: for fixed $x$, the weight grows like $1/|t|$ near zero. A Cauchy sequence in this norm converges uniformly on every compact subset of $\mathcal C_\alpha$, including at $t=0$. Its limit is holomorphic by [locally uniform convergence of holomorphic functions](#locally-uniform-convergence-of-holomorphic-functions), and the pointwise norm bounds show convergence in the original norm. The shrinking domain compensates for loss of an $x$-[derivative](calculus.md#derivative) in a [Cauchy-Kovalevskaya theorem](partial-differential-equation.md#cauchy-kovalevskaya-theorem) argument.

##### Contraction estimate on a shrinking holomorphic domain

↑ **Parent:** [Weighted holomorphic norm on a shrinking time domain](#weighted-holomorphic-norm-on-a-shrinking-time-domain)

Write $N=\|u\|_\alpha$, $r=|t|$ and $A=\alpha(1-s)>r$. Along the straight integration segment, choose $\sigma(\tau)=s+(A-\tau)/(2\alpha)$. A [Cauchy estimate](analysis.md#cauchy-estimate) on a disc of radius $R(\sigma-s)$ bounds the integrand by $4\alpha N\tau/[R(A-\tau)^2]$. Therefore

$$
\frac{A-r}{r}\left|\int_0^t\partial_xu(x,z)\,dz\right|
\leq\frac{4\alpha N}{R}\left[1+\frac{A-r}{r}\log(1-r/A)\right]
\leq\frac{4\alpha N}{R}.
$$

The integral is taken at fixed $x$, and the disc and segment lie inside the shrinking domain. Consequently $u\mapsto\int_0^t(iu_x+f)\,dz$ is a [contraction mapping](analysis.md#contraction-mapping) when $0<\alpha<R/4$ and the holomorphic source $f$ is bounded on the relevant closed polydisc. The source term has weighted norm at most $\alpha\sup|f|$, so the [Banach fixed-point theorem](analysis.md#contraction-mapping-theorem) gives a holomorphic solution with zero initial data.

### Order of a zero of a holomorphic function

↑ **Parent:** [Holomorphic function](#holomorphic-function)

If a nonzero holomorphic function has expansion

$$
f(z)=(z-z_0)^m g(z),
\qquad g(z_0)\ne0,
$$

then $m$ is the order or multiplicity of its zero at $z_0$.

#### Zero sets in the unit disc

↑ **Parent:** [Order of a zero of a holomorphic function](#order-of-a-zero-of-a-holomorphic-function)

A nonzero [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc) can have exactly a prescribed sequence of zeros, counted with [multiplicity](polynomial.md#multiplicity-mathematics), if and only if that sequence is locally finite in the disc. Necessity is the [identity theorem for holomorphic functions](#identity-theorem). For sufficiency, remove a finite number $m$ of zeros at zero and enumerate the others as $a_n$, so $|a_n|\to1$. Use the [Weierstrass elementary factors](real-analysis.md#weierstrass-elementary-factor) $E_n(t)=(1-t)\exp(\sum_{j=1}^nt^j/j)$. On every [compact](topology.md#compact-space) subdisc, eventually $|z/a_n|\le q<1$ and $|\log E_n(z/a_n)|\le q^{n+1}/((n+1)(1-q))$. Hence $z^m\prod_nE_n(z/a_n)$ converges locally uniformly and has exactly the prescribed zeros. Finite sequences simply give finite products.

#### Simple zero

↑ **Parent:** [Order of a zero of a holomorphic function](#order-of-a-zero-of-a-holomorphic-function)

A simple zero has order one, equivalently $f(z_0)=0$ and $f'(z_0)\ne0$.

### Analytic continuation

↑ **Parent:** [Holomorphic function](#holomorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analytic_continuation)

An analytic continuation extends a [holomorphic function](#holomorphic-function) through overlapping connected open sets while preserving its values on their overlap. Continuation along different paths can produce different germs when the domain contains [branch points](#branch-point).

#### Natural boundary of a holomorphic function

↑ **Parent:** [Analytic continuation](#analytic-continuation)

A boundary of a domain of a [holomorphic function](#holomorphic-function) is natural if the function has no analytic continuation through any of its points. For $f(z)=\sum_{n\ge1}z^{2^n}$, each root of unity of order a power of two is a singular boundary point: along $z=r\zeta$ all sufficiently late terms equal $r^{2^n}$ and their sum tends to infinity as $r\uparrow1$. These roots are dense on the unit circle, so no boundary arc admits analytic continuation.

#### Zeta function regularization

↑ **Parent:** [Analytic continuation](#analytic-continuation)

Zeta function regularization assigns a finite value to a divergent spectral sum by first forming a convergent complex-power series and then using its [analytic continuation](#analytic-continuation). For positive frequencies $\omega_n$, continue $\sum_n\omega_n^{-s}$ to $s=-1$ to define a regulated frequency sum, when that continuation is regular there. This does not turn the divergent positive-term sum into an ordinary convergent sum. It is a useful subtraction convention for the [normal-ordering constant of a string](string-theory.md#normal-ordering-constant-of-a-string) and for vacuum energies.

##### Half-integer zeta-regularized mode sum

↑ **Parent:** [Zeta function regularization](#zeta-function-regularization)

For $r=n+1/2$, $n\geq0$, the convergent frequency zeta function, expressed through the [Riemann zeta function](analytic-number-theory.md#riemann-zeta-function), is $\sum_r r^{-s}=(2^s-1)\zeta_R(s)$ when $\operatorname{Re}s>1$. Its [analytic continuation](#analytic-continuation) at $s=-1$ gives $(1/2-1)(-1/12)=1/24$. A common exponential frequency cutoff gives $\sum_r r e^{-\varepsilon r}=\varepsilon^{-2}+1/24+O(\varepsilon^2)$, so the same finite part follows by subtracting the leading divergence. In contrast, integer frequencies have regulated sum $-1/12$.

#### Meromorphic continuation

↑ **Parent:** [Analytic continuation](#analytic-continuation)

A [meromorphic continuation](#meromorphic-continuation) extends a [holomorphic function](#holomorphic-function) from a connected open [set](set.md) to a larger connected domain as a [meromorphic function](isolated-singularity.md#meromorphic-function), allowing isolated poles. Equality on the initial open [set](set.md) determines the extension uniquely by the [identity theorem](#identity-theorem). [Integral](calculus.md#integral) formulas whose integrands depend holomorphically on a parameter often supply such an extension after contour deformation or subtraction of singular terms.

<h4 id="sokhotski-plemelj-theorem">Sokhotski–Plemelj theorem</h4>

↑ **Parent:** [Analytic continuation](#analytic-continuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sokhotski–Plemelj_theorem)

As distributions on the real line,

$$
\frac1{x\pm i0}
=\operatorname{PV}\frac1x\mp i\pi\delta(x).
$$

The Sokhotski--Plemelj formula relates the two boundary values of a Cauchy transform across its contour and fixes the spectral delta functions generated by retarded and advanced prescriptions.

##### Signed Cauchy boundary operators

↑ **Parent:** [Sokhotski–Plemelj theorem](#sokhotski-plemelj-theorem)

With $Hv(\rho)=\pi^{-1}\operatorname{PV}\int v(s)/(\rho-s)ds$, the upper and lower limiting [Cauchy integrals](#cauchy-transform) are $P^\pm v=\pm v/2+iHv/2$. They obey $P^+-P^-=I$. The actual complementary idempotent [projections](vector-space.md#projection-linear-algebra) are $P^+$ and $-P^-$; confusing this signed convention with two positive projectors changes reconstruction signs. These boundary operators naturally enter the [spectral reconstruction of an attenuated Radon transform](analysis.md#spectral-reconstruction-of-an-attenuated-radon-transform).

#### Monodromy theorem

↑ **Parent:** [Analytic continuation](#analytic-continuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monodromy_theorem)

If a function element can be analytically continued along every path in a domain, continuation along two endpoint-fixed homotopic paths gives the same terminal germ.

##### Monodromy group of a covering

↑ **Parent:** [Monodromy theorem](#monodromy-theorem)

For a covering $p:X\to Y$ and base point $y$, lifting loops based at $y$ permutes the fibre $p^{-1}(y)$. The image of

$$
\pi_1(Y,y)\longrightarrow\operatorname{Sym}(p^{-1}(y))
$$

is the monodromy group.

###### Monodromy transposition in a three-sheeted cover

↑ **Parent:** [Monodromy group of a covering](#monodromy-group-of-a-covering)

A connected three-sheeted cover has transitive monodromy. If it also has a simple branch point, its monodromy contains a transposition and must be the full symmetric group on three letters. A local triple branch supplies a three-cycle explicitly.

###### Monodromy group of z squared plus z to the minus two

↑ **Parent:** [Monodromy group of a covering](#monodromy-group-of-a-covering)

The degree-four [rational map](isolated-singularity.md#rational-map-complex-analysis) $F(z)=z^2+z^{-2}$ has branch values $-2,2,\infty$. Away from their inverse images, the transformations

$$
z\mapsto-z,
\qquad z\mapsto z^{-1}
$$

are commuting deck involutions. They generate a [Klein four-group](finite-group-theory.md#klein-four-group) acting transitively on each fibre

$$
\{z,-z,z^{-1},-z^{-1}\}.
$$

Consequently the monodromy group is $V_4$, acting by the identity and the three double transpositions.

#### Analytic continuation by contour deformation

↑ **Parent:** [Analytic continuation](#analytic-continuation)

If a parameter-dependent contour integral has a moving pole, deforming the integration contour continuously so that the pole never crosses it preserves a holomorphic branch. Returning the contour to its original path after crossing a pole adds or subtracts the corresponding residue contribution.

##### Branch phase in a figure-eight analytic continuation integral

↑ **Parent:** [Analytic continuation by contour deformation](#analytic-continuation-by-contour-deformation)

For a figure-eight contour around $1$ anticlockwise and $-1$ clockwise, start $(t^2-1)^z$ at $t=0$ with argument $-\pi$. Shrinking the two loops gives the displayed identity. If the interval integral instead uses $(t^2-1)^z=e^{-i\pi z}(1-t^2)^z$, the corresponding identity includes the extra factor $e^{i\pi z}$. Omitting this phase changes the value, rather than merely the locations of the meromorphic continuation's poles.

#### Multivalued inverse hyperbolic sine

↑ **Parent:** [Analytic continuation](#analytic-continuation)

The solutions of $\sinh w=z$ are

$$
w=\operatorname{Arcsinh}z+2\pi ik
\quad\hbox{or}\quad
w=-\operatorname{Arcsinh}z+(2k+1)\pi i,
\qquad k\in\mathbb Z,
$$

for any chosen local branch $\operatorname{Arcsinh}$.

It is the complex multivalued sine member of the [inverse hyperbolic functions](calculus.md#inverse-hyperbolic-functions).

### Entire function

↑ **Parent:** [Holomorphic function](#holomorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entire_function)

An entire function is a [holomorphic function](#holomorphic-function) whose domain is the whole [complex plane](#complex-plane).

#### Injective entire functions are affine

↑ **Parent:** [Entire function](#entire-function)

An injective [holomorphic function](#holomorphic-function) cannot have an [essential singularity](isolated-singularity.md#essential-singularity): [Casorati-Weierstrass theorem](isolated-singularity.md#casorati-weierstrass-theorem) would give values from a small punctured neighbourhood inside the open image of a disjoint neighbourhood, contradicting injectivity. Apply this at infinity to an injective [entire function](#entire-function). A removable singularity there would make the function constant by [Liouville's theorem](#liouville-theorem). A pole makes it a polynomial by the [Cauchy coefficient formula](analysis.md#cauchy-coefficient-formula); its derivative has no zero, so the [fundamental theorem of algebra](algebra.md#fundamental-theorem-of-algebra) forces degree one.

#### Exponential polynomial

↑ **Parent:** [Entire function](#entire-function)

An [exponential polynomial](#exponential-polynomial) is a finite sum of [polynomial](polynomial.md) multiples of exponentials. For distinct exponents, its terms are linearly independent over the [polynomial](polynomial.md) ring: to isolate one term, apply the product of operators $(D-\lambda_j)^{\deg P_j+1}$ for all the other terms. On the remaining [polynomial](polynomial.md) each operator becomes $D+\lambda_0-\lambda_j$, which is injective because its nonzero constant preserves the leading coefficient. A nonzero [exponential polynomial](#exponential-polynomial) is an [entire function](#entire-function) of exponential type. Its maximum-modulus [logarithm](calculus.md#logarithm) is $O(R+\log R)$, and [Jensen's formula](#jensen-s-formula) gives at most $O(R)$ zeros, counted with multiplicity, in a disk of radius $R$.

#### Order of an entire function

↑ **Parent:** [Entire function](#entire-function)

For a nonconstant [entire function](#entire-function), put $M_f(R)=\max_{|s|\leq R}|f(s)|$. Its order measures the exponent in its exponential growth. Bounds $\log M_f(R)=O(R\log R)$ imply order at most one; a matching lower bound along the positive real axis proves order exactly one. This distinction is stronger than mere entire analyticity and controls the genus in [Hadamard factorization](#hadamard-factorization-theorem).

// Target: analytic-number-theory.bigb

#### Entire function of exponential type

↑ **Parent:** [Entire function](#entire-function)

An [entire function](#entire-function) is of exponential type if constants $A,B>0$ give the displayed bound everywhere. A genus-zero [canonical product](#canonical-product) with $\sum_n|a_n|^{-1}<\infty$ obeys $|\prod_n(1-z/a_n)|\le\exp(|z|\sum_n|a_n|^{-1})$, since $1+u\le e^u$ for $u\ge0$.

#### Weierstrass factorization theorem

↑ **Parent:** [Entire function](#entire-function)

A nonzero [entire function](#entire-function) can be described by its discrete zero locations and multiplicities, a product of [Weierstrass elementary factors](real-analysis.md#weierstrass-elementary-factor) and a zero-free exponential factor. Conversely, consistent prescribed multiplicities at distinct points escaping every compact subset can be realized by choosing factor orders large enough for [infinite product convergence from logarithmic tails](real-analysis.md#infinite-product-convergence-from-logarithmic-tails). Repeated locations with incompatible exact multiplicities are not admissible data, and a finite accumulation of distinct zeros is excluded by the [identity theorem](#identity-theorem).

##### Canonical product

↑ **Parent:** [Weierstrass factorization theorem](#weierstrass-factorization-theorem)

A canonical product builds a prescribed discrete zero set from [Weierstrass elementary factors](real-analysis.md#weierstrass-elementary-factor). Choose the orders $p_n$ so that the logarithms of tail factors converge uniformly on each compact subset. [Infinite product convergence from logarithmic tails](real-analysis.md#infinite-product-convergence-from-logarithmic-tails) then gives an [entire function](#entire-function) with exactly those zeros, counted with the prescribed multiplicities. When $\sum_n|a_n|^{-1}<\infty$, factors of order zero suffice.

###### Canonical product construction for zeros escaping to the disk boundary

↑ **Parent:** [Canonical product](#canonical-product)

For nonzero prescribed zeros $a_n$ with $|a_n|\to1$, the [Weierstrass elementary factors](real-analysis.md#weierstrass-elementary-factor) of increasing order give the displayed [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc); $m$ handles finitely many zeros at zero. On any compact disc, eventually $|z/a_n|\le q<1$, and $|\log E_n(z/a_n)|\le q^{n+1}/[(n+1)(1-q)]$. The [infinite product convergence from logarithmic tails](real-analysis.md#infinite-product-convergence-from-logarithmic-tails) gives a nonvanishing tail. The finite initial factors supply exactly the prescribed zeros and [multiplicities](polynomial.md#multiplicity-mathematics). No [Blaschke condition](#blaschke-condition) is required unless boundedness is imposed.

###### Boundary-adapted holomorphic zero factor

↑ **Parent:** [Canonical product](#canonical-product)

For a proper plane [domain](topology.md#domain-mathematical-analysis) $D$, choose $a\in D$ and $w\notin D$ attaining $\delta(a)=\operatorname{dist}(a,\mathbb C\setminus D)$. The [holomorphic function](#holomorphic-function)

$$
E_{a,w,K}(z)=\frac{z-a}{z-w}\exp\left(\sum_{k=1}^K\frac1k\left(\frac{a-w}{z-w}\right)^k\right)
$$

has exactly one zero in $D$, a simple zero at $a$. For $|z-w|>2\delta(a)$ its zero-free [holomorphic logarithm](#holomorphic-logarithm) satisfies

$$
\left|\log E_{a,w,K}(z)\right|\leq\sum_{k>K}\frac{2^{-k}}k\leq\frac{2^{-K}}{K+1}.
$$

Thus products of such factors can realize prescribed zeros approaching the boundary. If the zero has multiplicity $m$, choose the logarithmic error smaller by a factor $m$ before taking the $m$th power. On a compact subset of $D$, eventual uniform summability of these logarithms gives a nonvanishing product tail and a [holomorphic function](#holomorphic-function) with precisely the requested zeros.

##### Hadamard factorization theorem

↑ **Parent:** [Weierstrass factorization theorem](#weierstrass-factorization-theorem)

An [entire function](#entire-function) of finite order factors as its canonical zero product times the exponential of a [polynomial](polynomial.md). For order at most one and nonzero value at zero, it has the form $f(z)=f(0)e^{Bz}\prod_j(1-z/a_j)e^{z/a_j}$. Genus-one factors converge when $\sum_j|a_j|^{-2}<\infty$. A zero-free function of this order is therefore the exponential of an affine [polynomial](polynomial.md).

##### Entire functions with the same zero divisor

↑ **Parent:** [Weierstrass factorization theorem](#weierstrass-factorization-theorem)

If two nonzero [entire functions](#entire-function) have identical zeros and orders, their quotient extends to a nowhere-zero [entire function](#entire-function). Its logarithmic derivative has a primitive on the simply connected plane, producing a [holomorphic logarithm](#holomorphic-logarithm) $h$ and the displayed relation. Any two choices differ by one constant integer multiple of $2\pi i$. On a multiply connected domain the logarithm can fail to exist globally.

#### Pointwise vanishing derivative criterion for a polynomial

↑ **Parent:** [Entire function](#entire-function)

Suppose that for every $z\in\mathbb C$, at least one derivative $f^{(n)}(z)$ of an [entire function](#entire-function) vanishes. The closed sets $E_n=\{z:f^{(n)}(z)=0\}$ cover $\mathbb C$. By the [Baire category theorem](topological-analysis.md#baire-category-theorem), some $E_N$ has nonempty interior. The [identity theorem](#identity-theorem) gives $f^{(N)}=0$ everywhere, so $f$ is a [polynomial](polynomial.md) of degree below $N$.

#### Picard theorem

↑ **Parent:** [Entire function](#entire-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Picard_theorem)

The Picard theorems concern omitted values of [holomorphic functions](#holomorphic-function). The [Little Picard theorem](#little-picard-theorem) permits at most one omitted value for a nonconstant [entire function](#entire-function); the [Great Picard theorem](#great-picard-theorem) gives infinitely many occurrences of all but at most one value near an [essential singularity](isolated-singularity.md#essential-singularity).

##### Little Picard theorem

↑ **Parent:** [Picard theorem](#picard-theorem)

Every nonconstant entire function takes every complex value with at most one exception.

###### Great Picard theorem

↑ **Parent:** [Little Picard theorem](#little-picard-theorem)

Near an essential singularity, a holomorphic function takes every complex value, with at most one exception, infinitely often.

### Analytic function with image in an affine real line

↑ **Parent:** [Holomorphic function](#holomorphic-function)

If $f=u+iv$ is a [holomorphic function](#holomorphic-function) on a connected domain and

$$
au+bv=c,\qquad a^2+b^2\ne0,
$$

then the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) force both components of $f'$ to vanish. Hence $f$ is constant.

## Simply connected domain

↑ **Parent:** [Complex analysis](complex-analysis.md)

A domain is simply connected when every closed path in it can be continuously contracted to a point while remaining in the domain.

Such a domain is a [simply connected space](algebraic-topology.md#simply-connected-space).

### Crosscut

↑ **Parent:** [Simply connected domain](#simply-connected-domain)

A crosscut of a planar domain is a simple open arc inside the domain whose two endpoints are distinct boundary points, interpreted as [prime ends](geometry-and-topology.md#prime-end) when necessary. In a [simply connected domain](#simply-connected-domain) it divides the domain into two components. In the half-plane, a bounded crosscut joining two real points separates the intervening real interval from infinity; a [Loewner chain](stochastic-process.md#loewner-chain) completing that crosscut swallows this interval.

### Primitive of a holomorphic function on a simply connected domain

↑ **Parent:** [Simply connected domain](#simply-connected-domain)

Every [holomorphic function](#holomorphic-function) $f$ on a [simply connected domain](#simply-connected-domain) has a single-valued [antiderivative](calculus.md#antiderivative). Fixing $z_0$ and setting

$$
F(z)=\int_{z_0}^z f(t)\,dt
$$

gives a path-independent function with $F'=f$, because the [Cauchy integral theorem](#cauchy-s-integral-theorem) makes the integral around every closed path zero.

## Complex inverse sine

↑ **Parent:** [Complex analysis](complex-analysis.md)

The principal complex inverse sine on

$$
\mathbb C\setminus\bigl((-\infty,-1]\cup[1,\infty)\bigr)
$$

is the branch

$$
\arcsin z=\int_0^z\frac{dt}{\sqrt{1-t^2}}
$$

whose derivative equals one at zero.

It is the complex sine member of the [inverse trigonometric functions](geometry-and-topology.md#inverse-trigonometric-functions).

### Branches of the complex inverse sine

↑ **Parent:** [Complex inverse sine](#complex-inverse-sine)

If $G$ is the principal [complex inverse sine](#complex-inverse-sine), all values reached by [analytic continuation](#analytic-continuation) are

$$
2n\pi+G(z)
\quad\hbox{or}\quad
(2n+1)\pi-G(z),
\qquad n\in\mathbb Z.
$$

This follows from the [monodromy reflections](#monodromy-reflection-at-a-square-root-branch-point) about the branch values $-\pi/2$ and $\pi/2$.

#### Monodromy of the complex inverse sine

↑ **Parent:** [Branches of the complex inverse sine](#branches-of-the-complex-inverse-sine)

Let $w$ be a local value of the [complex inverse sine](#complex-inverse-sine). Since the limiting values at the two [branch points](#branch-point) are $\pi/2$ at $z=1$ and $-\pi/2$ at $z=-1$, [monodromy reflection at a square-root branch point](#monodromy-reflection-at-a-square-root-branch-point) gives

$$
R_+(w)=\pi-w,
\qquad
R_-(w)=-\pi-w.
$$

Following a counterclockwise loop that encloses both branch points in the convention where $\sqrt{1-z^2}$ is positive just above $(-1,1)$ applies the two reflections in the order that gives

$$
R_-\circ R_+(w)=w-2\pi.
$$

The reverse orientation gives $w+2\pi$. Thus the translational part of the monodromy is generated by $2\pi$.

<h2 id="morera-s-theorem">Morera's theorem</h2>

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morera's_theorem)

If a continuous complex-valued function on a domain has zero integral around the boundary of every triangle contained in that domain, then it is holomorphic.

<h2 id="cauchy-s-integral-theorem">Cauchy's integral theorem</h2>

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy's_integral_theorem)

If a function is holomorphic on a simply connected domain, its integral around every closed piecewise smooth contour in that domain vanishes. In particular, contours with common endpoints may be deformed through the domain without changing the integral.

### Cauchy theorem for a triangle

↑ **Parent:** [Cauchy's integral theorem](#cauchy-s-integral-theorem)

A [holomorphic function](#holomorphic-function) on an open neighbourhood of a closed triangle has zero [contour integral](#contour-integral) around its boundary. Goursat's subdivision proof uses complex differentiability alone: repeatedly choose a quarter-size triangle carrying at least one quarter of the integral, and subtract the affine expansion at the limiting point. No continuity of the derivative is assumed.

### Contour deformation

↑ **Parent:** [Cauchy's integral theorem](#cauchy-s-integral-theorem)

A contour deformation changes the path of a [contour integral](#contour-integral) through a region where its integrand is a [holomorphic function](#holomorphic-function). The [Cauchy integral theorem](#cauchy-s-integral-theorem) preserves the integral when the endpoints are fixed and the connecting boundary terms vanish. Crossing a [pole](isolated-singularity.md#pole) instead contributes the appropriately oriented [residue](analysis.md#residue); a [branch cut](analysis.md#branch-cut) limits which deformations are permitted on one analytic sheet.

### Gaussian contour translation

↑ **Parent:** [Cauchy's integral theorem](#cauchy-s-integral-theorem)

For $a>0$ and real $c$, integrate $e^{-az^2}$ around a wide rectangle between the real axis and $\operatorname{Im}z=c$. The vertical contributions vanish as the width tends to infinity, so

$$
\int_{\mathbb R+ic}e^{-az^2}\,dz
=\int_{\mathbb R}e^{-ax^2}\,dx.
$$

## Cauchy principal value

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_principal_value)

The principal value uses symmetric truncation at infinity and symmetric deletion around real singularities.

### Principal-value beta integral

↑ **Parent:** [Cauchy principal value](#cauchy-principal-value)

For $0<s<a$,

$$
\operatorname{PV}\int_0^\infty\frac{x^{s-1}}{1-x^a}dx=\frac\pi a\cot\frac{\pi s}{a}.
$$

## Principal-value residue rule

↑ **Parent:** [Complex analysis](complex-analysis.md)

For real $a$ and nonzero real $\omega$,

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{i\omega x}}{x-a}\,dx
=i\pi\operatorname{sgn}(\omega)e^{i\omega a}.
$$

## Exponential integral

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_integral)

For real $x>0$, the decaying exponential integral is

$$
E_1(x)=\int_x^\infty\frac{e^{-t}}t\,dt,\qquad E_1'(x)=-\frac{e^{-x}}x.
$$

The other standard real convention satisfies $\operatorname{Ei}(-x)=-E_1(x)$. The [NIST definitions](https://dlmf.nist.gov/6.2) specify the analytic continuation and branch conventions.

### Logarithmic expansion of a symmetric exponential integral

↑ **Parent:** [Exponential integral](#exponential-integral)

For $J(\varepsilon)=\int_0^\infty e^{-x-\varepsilon/x}dx/x$, reciprocity $x\mapsto\varepsilon/x$ and the [small-argument expansion of the exponential integral](#small-argument-expansion-of-the-exponential-integral) give $J=-\log\varepsilon-2\gamma+o(1)$. Differentiation and [integration by parts](calculus.md#integration-by-parts) give $\varepsilon J''+J'=J$. Its [Frobenius method](#frobenius-method) yields

$$
J=-\log\varepsilon-2\gamma+\varepsilon[-\log\varepsilon+2-2\gamma]+O(\varepsilon^2|\log\varepsilon|).
$$

The logarithm is a singular contribution that a naive termwise expansion at $x=0$ misses.

#### Moving-cutoff correction to a symmetric exponential integral

↑ **Parent:** [Logarithmic expansion of a symmetric exponential integral](#logarithmic-expansion-of-a-symmetric-exponential-integral)

For $I=\int_\varepsilon^\infty e^{-x-\varepsilon/x}dx/x$, the omitted interval becomes $J-I=\int_1^\infty e^{-t-\varepsilon/t}dt/t$. A uniform [Taylor expansion](calculus.md#taylor-expansion) gives $J-I=E_1(1)-\varepsilon[e^{-1}-E_1(1)]+O(\varepsilon^2)$. Subtracting this correction from the [logarithmic expansion of a symmetric exponential integral](#logarithmic-expansion-of-a-symmetric-exponential-integral) preserves both the constant and first-order coefficient.

### Small-argument expansion of the exponential integral

↑ **Parent:** [Exponential integral](#exponential-integral)

As $x\downarrow0$, the [exponential integral](#exponential-integral) has

$$
E_1(x)=-\gamma-\log x+x-\frac{x^2}4+O(x^3),
$$

where $\gamma$ is the [Euler--Mascheroni constant](#euler-s-constant). Integrating the [Taylor series](calculus.md#taylor-series) of $E_1'(x)=-e^{-x}/x$ gives every nonconstant coefficient; the constant follows from the limiting definition of $\gamma$. A logarithm of a stretched variable can create a [switchback term](differential-equation.md#switchback-term) in a [matched asymptotic expansion](differential-equation.md#matched-asymptotic-expansion).

## Gamma function

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gamma_function)

$\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}\,dt$ for $\Re z>0$, and $\Gamma(z+1)=z\Gamma(z)$ gives meromorphic continuation.

### Derivative of the gamma function

↑ **Parent:** [Gamma function](#gamma-function)

For positive real $a$, differentiating the [gamma function](#gamma-function) integral under the integral sign gives the displayed formula; successive [derivatives](calculus.md#derivative) insert higher powers of $\log t$. Dominated differentiation on compact positive-$a$ intervals is justified by exponential decay at infinity and integrability of $t^{a-1}|\log t|^n$ at zero. At $a=1$, these derivatives give moments used in logarithmic endpoint [asymptotic expansions](analysis.md#asymptotic-expansion).

### Gamma function has no zeros

↑ **Parent:** [Gamma function](#gamma-function)

The [beta--gamma identity](#beta-gamma-identity) gives $\Gamma(z/2)^2=B(z/2,z/2)\Gamma(z)$ for $\operatorname{Re}z>0$. A zero of $\Gamma(z)$ would therefore force zeros at every $z/2^m$. But $w\Gamma(w)=\Gamma(1+w)\to1$ as $w\to0$ in the right half-plane, a contradiction. The [Gamma function recurrence](#gamma-function-recurrence) then extends nonvanishing to every point where the meromorphic gamma function is finite. Nonpositive integers are poles, not zeros.

### Imaginary-argument gamma asymptotic

↑ **Parent:** [Gamma function](#gamma-function)

Rotating the integral defining the [Gamma function](#gamma-function) toward the positive imaginary axis introduces the factor $ie^{-\pi n/2}$. After scaling by $n$, the remaining phase is $\log s-s$, whose unique stationary point is $s=1$ with second derivative $-1$. The [stationary phase method](analysis.md#stationary-phase-method) gives $e^{-in-i\pi/4}\sqrt{2\pi/n}$ for this scaled integral, producing the displayed asymptotic. The boundary contour integral must be Abel-regularized; its off-saddle tails are smaller by integration by parts.

### Gamma function residue at a nonpositive integer

↑ **Parent:** [Gamma function](#gamma-function)

The [Gamma function recurrence](#gamma-function-recurrence) and $\Gamma(z)\sim1/z$ at zero imply a [simple pole](isolated-singularity.md#simple-pole) at every $z=-n$, $n\geq0$, with [residue](analysis.md#residue) $(-1)^n/n!$.

### Euler product for the gamma function

↑ **Parent:** [Gamma function](#gamma-function)

For $z$ away from the poles, the [gamma function](#gamma-function) satisfies

$$
\Gamma(z)=\frac1z\prod_{n=1}^\infty(1+1/n)^z(1+z/n)^{-1}.
$$

Its finite product is $m!(m+1)^z/[z(z+1)\cdots(z+m)]$. Splitting even and odd factors gives the [gamma duplication formula](#gamma-duplication-formula).

### Residues of the Gamma function

↑ **Parent:** [Gamma function](#gamma-function)

The [Gamma function recurrence](#gamma-function-recurrence) gives $\Gamma(s)=\Gamma(s+j+1)/(s(s+1)\cdots(s+j))$. Its numerator equals one at $s=-j$, so the [residue](analysis.md#residue) there is $(-1)^j/j!$ for every nonnegative integer $j$.

### Gamma integral

↑ **Parent:** [Gamma function](#gamma-function)

For $a,s>0$, the change of variable $u=at$ in the defining integral for the [Gamma function](#gamma-function) gives

$$
\int_0^\infty t^{s-1}e^{-at}\,dt=a^{-s}\Gamma(s).
$$

In particular, $\Gamma(1/2)=\sqrt\pi$ implies

$$
u^{-1/2}=\frac1{\sqrt\pi}\int_0^\infty t^{-1/2}e^{-ut}\,dt.
$$

#### Cubic oscillatory Gamma integral

↑ **Parent:** [Gamma integral](#gamma-integral)

For $t>0$, contour rotation through angle $-\pi/6$ gives

$$
\int_0^\infty e^{-itu^3}du
=e^{-i\pi/6}t^{-1/3}\Gamma\left(\frac43\right).
$$

Taking real parts yields

$$
\int_0^\infty\cos(u^3)du
=\Gamma\left(\frac43\right)\cos\frac\pi6.
$$

### Gamma function recurrence

↑ **Parent:** [Gamma function](#gamma-function)

Integration by parts gives

$$
\Gamma(z+1)=z\Gamma(z).
$$

### Bose integral

↑ **Parent:** [Gamma function](#gamma-function)

For $\operatorname{Re}s>1$, expansion of $(e^x-1)^{-1}$ as a [geometric series](real-analysis.md#geometric-series) and termwise integration give

$$
\int_0^\infty\frac{x^{s-1}}{e^x-1}\,dx
=\Gamma(s)\zeta(s).
$$

<h3 id="euler-s-constant">Euler's constant</h3>

↑ **Parent:** [Gamma function](#gamma-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_constant)

The Euler--Mascheroni constant is

$$
\gamma=\lim_{n\to\infty}\left(\sum_{k=1}^n\frac1k-\log n\right).
$$

### Weierstrass product for the reciprocal gamma function

↑ **Parent:** [Gamma function](#gamma-function)

The reciprocal gamma function has the entire-product representation

$$
\frac1{\Gamma(z)}
=ze^{\gamma z}\prod_{k=1}^{\infty}
\left(1+\frac zk\right)e^{-z/k}.
$$

This is a particular application of the [Weierstrass factorization theorem](#weierstrass-factorization-theorem).

### Digamma function

↑ **Parent:** [Gamma function](#gamma-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Digamma_function)

The digamma function is the logarithmic derivative

$$
\psi(z)=\frac{\Gamma'(z)}{\Gamma(z)}.
$$

Logarithmically differentiating the Weierstrass product gives

$$
\psi(z)=-\gamma-\frac1z
+z\sum_{k=1}^{\infty}\frac1{k(z+k)}.
$$

#### Trigamma function

↑ **Parent:** [Digamma function](#digamma-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trigamma_function)

The trigamma function is $\psi'(z)$. For real $z>0$,

$$
\psi'(z)=\frac1{z^2}+\sum_{k=1}^{\infty}\frac1{(z+k)^2}>0.
$$

#### Positive zero of the digamma function

↑ **Parent:** [Digamma function](#digamma-function)

The digamma function is strictly increasing on the positive real axis, while

$$
\psi(1)=-\gamma<0,
\qquad
\psi(2)=1-\gamma>0.
$$

It therefore has exactly one positive zero, and that zero lies in $(1,2)$.

### Gamma reflection formula

↑ **Parent:** [Gamma function](#gamma-function)

$$
\Gamma(z)\Gamma(1-z)=\frac{\pi}{\sin\pi z}.
$$

### Gamma duplication formula

↑ **Parent:** [Gamma function](#gamma-function)



$$
\Gamma(z)\Gamma(z+\tfrac12)=2^{1-2z}\sqrt\pi\,\Gamma(2z).
$$

It follows by making the logarithm of the quotient entire and periodic; growth forces its periodic remainder to be constant.

### Beta function

↑ **Parent:** [Gamma function](#gamma-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beta_function)

For $\operatorname{Re}p,\operatorname{Re}q>0$, Euler's beta function is

$$
B(p,q)=\int_0^1t^{q-1}(1-t)^{p-1}\,dt.
$$

#### Incomplete beta function

↑ **Parent:** [Beta function](#beta-function)

For real $p,q>0$ and $0\leq z\leq1$, the displayed integral is the incomplete [beta function](#beta-function). The regularized version is $I_z(p,q)=B_z(p,q)/B_1(p,q)$, the [cumulative distribution function](probability-theory.md#cumulative-distribution-function) of the [Beta distribution](probability-theory.md#beta-distribution). It has endpoint values zero and one and derivative $z^{p-1}(1-z)^{q-1}/B_1(p,q)$. This is a useful explicit [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) when the scale density has two power-law endpoint singularities.

#### Complex beta integral

↑ **Parent:** [Beta function](#beta-function)

For $c=1-a-b$ with positive real parts $\operatorname{Re}a,\operatorname{Re}b,\operatorname{Re}c$, the integral converges at its two finite singularities and at infinity, and equals

$$
\pi\frac{\Gamma(a)\Gamma(b)\Gamma(c)}{\Gamma(1-a)\Gamma(1-b)\Gamma(1-c)}.
$$

To prove it, use [Schwinger parameterization](perturbative-quantum-field-theory.md#schwinger-parameterization) with exponents $1-a$ and $1-b$. Integrating the resulting planar [Gaussian integral](calculus.md#gaussian-integral) gives $\pi/(\lambda+\rho)$ times $\exp[-\lambda\rho/(\lambda+\rho)]$. Set $q=\lambda+\rho$ and $x=\lambda/q$; the $q$ integral is a [gamma function](#gamma-function) and the $x$ integral is $B(a,b)$, giving the stated ratio. This domain justifies the interchanges; elsewhere the answer is interpreted by [analytic continuation](#analytic-continuation). The string measure $d^2z=2dx\,dy$ multiplies the answer by two.

<h4 id="beta-gamma-identity">Beta--gamma identity</h4>

↑ **Parent:** [Beta function](#beta-function)

The sum-and-ratio change of variables in a product of gamma integrals gives

$$
B(p,q)=\frac{\Gamma(p)\Gamma(q)}{\Gamma(p+q)}.
$$

##### Sum-and-ratio substitution for gamma integrals

↑ **Parent:** [Beta--gamma identity](#beta-gamma-identity)

For $s,t>0$, put $r=s+t$ and $u=t/(s+t)$. Then $(s,t)=(r(1-u),ru)$ and $ds\,dt=r\,dr\,du$, separating radial gamma and ratio beta integrals.

#### Beta-function recurrence

↑ **Parent:** [Beta function](#beta-function)

The [Beta function](#beta-function) obeys

$$
B(x+1,y)=\frac{x}{x+y}B(x,y),
\qquad
B(x,y+1)=\frac{y}{x+y}B(x,y).
$$

These identities follow immediately from the [beta--gamma identity](#beta-gamma-identity) and the [Gamma function recurrence](#gamma-function-recurrence).

#### Logarithmic moments of the Cauchy kernel

↑ **Parent:** [Beta function](#beta-function)

For $0<a<2$,

$$
I(a)=\int_0^\infty\frac{x^{a-1}}{1+x^2}\,dx
=\frac\pi2\csc\frac{\pi a}{2}.
$$

Differentiating at $a=1$ and expanding the secant gives

$$
\int_0^\infty\frac{(\log x)^2}{1+x^2}\,dx=\frac{\pi^3}{8},
\qquad
\int_0^\infty\frac{(\log x)^4}{1+x^2}\,dx=\frac{5\pi^5}{32}.
$$

### Gamma function asymptotic at zero

↑ **Parent:** [Gamma function](#gamma-function)

The functional equation and $\Gamma(1)=1$ give $\Gamma(z)\sim1/z$ as $z\to0$ away from the negative real axis.

#### Diagonal beta-function asymptotic at zero

↑ **Parent:** [Gamma function asymptotic at zero](#gamma-function-asymptotic-at-zero)

The beta--gamma identity gives $B(z,z)=\Gamma(z)^2/\Gamma(2z)\sim2/z$ as $z\to0$ through the right half-plane.

## Riemann surfaces

↑ **Parent:** [Complex analysis](complex-analysis.md)

### Meromorphic differential on a Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A meromorphic differential is specified in each holomorphic chart by a meromorphic coefficient $f(z)$, with the coefficients transforming by the coordinate derivative so that the one-form agrees on overlaps. The derivative of a meromorphic function gives such a differential, and the ratio of two nonzero differentials is a meromorphic function. Orders of zeros and poles are independent of chart because coordinate derivatives are nonvanishing holomorphic factors. On a compact connected surface the sum of orders of a nonzero differential is $2g-2$, allowing its divisor to determine the genus.

### Hyperbolic Riemann surface in potential theory

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A noncompact [Riemann surface](#riemann-surfaces) is hyperbolic in potential theory when its Green-function exhaustion has a finite limit, equivalently when it admits a positive [Green function on a Riemann surface](analysis.md#green-function-on-a-riemann-surface). This definition does not assume a disk uniformization. The [unit disk](geometry-and-topology.md#unit-disk) is an example, since $-\log|z|$ is its positive Green function with pole zero. For simply connected surfaces this is equivalent to being conformally equivalent to the disk. For general surfaces, potential-theoretic hyperbolicity should not be conflated with the condition that the universal cover is the disk: some surfaces with disk universal cover have no positive Green function.

### Compact Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A [Riemann surface](#riemann-surfaces) which is compact as a topological space. For a connected one of genus $g$, the [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) gives $g$ independent [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form). The [Riemann bilinear relations for a compact surface](#riemann-bilinear-relations-for-a-compact-surface) make their normalized periods a full lattice in $\mathbb C^g$, and the [Abel-Jacobi map of a compact Riemann surface](#abel-jacobi-map-of-a-compact-riemann-surface) turns this lattice into a complex torus encoding [divisor classes](algebraic-geometry.md#divisor-class).

### Abel-Jacobi map of a compact Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

Integration of [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form) along cycles embeds the first [homology group](homology.md#homology-group) as a full [Euclidean lattice](fourier-analysis.md#euclidean-lattice) in $H^0(C,K_C)^\vee$. Fixing a base point, sum the path integrals to the points of an effective [complex analytic divisor](complex-geometry.md#divisor-on-a-complex-manifold). Different path choices differ by that lattice. The [Abel theorem for divisors](#abel-theorem-for-divisors) identifies the fibres with [linear equivalence of divisors](algebraic-geometry.md#linear-equivalence-of-divisors).

#### Abel theorem for divisors

↑ **Parent:** [Abel-Jacobi map of a compact Riemann surface](#abel-jacobi-map-of-a-compact-riemann-surface)

A degree-zero [complex analytic divisor](complex-geometry.md#divisor-on-a-complex-manifold) $E$ on a [compact Riemann surface](#compact-riemann-surface) is principal exactly when its [Abel-Jacobi map of a compact Riemann surface](#abel-jacobi-map-of-a-compact-riemann-surface) is zero. Normalize a [differential of the third kind](#differential-of-the-third-kind) with residues equal to the coefficients of $E$. The [Riemann bilinear relations for a compact surface](#riemann-bilinear-relations-for-a-compact-surface) express its $b$-periods as $2\pi i$ times the Abel integrals. If those integrals are in the period lattice, subtract a suitable integral multiple of the normalized [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form); all periods then lie in $2\pi i\mathbb Z$, so exponentiation gives the required [meromorphic function](isolated-singularity.md#meromorphic-function). Conversely, the logarithmic differential of a [meromorphic function](isolated-singularity.md#meromorphic-function) has integer residues and periods in $2\pi i\mathbb Z$, giving a zero Abel class by the same calculation.

### Differential of the third kind

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A meromorphic one-form on a [compact Riemann surface](#compact-riemann-surface) with only simple poles is a differential of the third kind. Prescribed residues can be realized exactly when their sum is zero: in the residue exact sequence for $K_C(S)$, the obstruction in $H^1(C,K_C)\cong\mathbb C$ is the sum of residues. Subtracting a [holomorphic differential form](complex-geometry.md#holomorphic-differential-form) normalizes its $a$-periods. Integer residues and periods in $2\pi i\mathbb Z$ make the exponential of its integral a single-valued [meromorphic function](isolated-singularity.md#meromorphic-function) with those orders of zeros and poles.

### Riemann bilinear relations for a compact surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

For a [compact Riemann surface](#compact-riemann-surface) with a [symplectic basis](linear-algebra.md#symplectic-basis) $a_i,b_i$ of its first [homology group](homology.md#homology-group), cutting along that basis and integrating a primitive gives

$$
\int_C\omega\wedge\eta=\sum_i\left(\int_{a_i}\omega\int_{b_i}\eta-\int_{b_i}\omega\int_{a_i}\eta\right)
$$

for closed smooth one-forms. For a [holomorphic differential form](complex-geometry.md#holomorphic-differential-form) $\omega$ and a [differential of the third kind](#differential-of-the-third-kind) $\eta$, the corresponding boundary calculation gives

$$
\sum_i\left(\int_{a_i}\omega\int_{b_i}\eta-\int_{b_i}\omega\int_{a_i}\eta\right)=2\pi i\sum_P\operatorname{res}_P(\eta)\int_{P_0}^P\omega.
$$

The paths and representatives of the cycles are chosen in the same cut surface. Normalized [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form) consequently have a symmetric period matrix with positive definite imaginary part.

### Three-branch-point regular surface cover

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

For a finite group generated by $A,B$, glue sheets labeled by the group over the three-punctured [Riemann sphere](#riemann-sphere) using left monodromy multiplication. Fill the punctures by the local power charts dictated by the orders $m,n,r$ of $A,B,AB$. Right multiplication by inverses defines the commuting deck action. Its nontrivial stabilizers are conjugates of the corresponding cyclic [subgroups](group.md#subgroup). The [Riemann-Hurwitz formula](#riemann-hurwitz-formula) gives the displayed [Euler characteristic](homology.md#euler-characteristic). A compatible metric can be averaged over the group; in genus at least two the invariant hyperbolic metric is canonical by the [uniformization theorem](#uniformization-theorem).

#### Orientation-reversing equivalence of branched-cover monodromy

↑ **Parent:** [Three-branch-point regular surface cover](#three-branch-point-regular-surface-cover)

For covers branched over three real points with a real base point, choose the two generating loops so complex conjugation reverses each. A sheet permutation satisfying the displayed identities lifts that conjugation to an anticonformal equivalence of the covers, including the filled branch points. For closed hyperbolic [Riemann surfaces](#riemann-surfaces) this is a [Riemannian isometry](differential-geometry.md#riemannian-isometry). Such an isometry need not come from conjugating the [subgroups](group.md#subgroup) inside the original deck group, so a [Gassmann equivalent](representation-theory.md#gassmann-equivalence) pair can be isometric despite nonconjugacy there.

### Quasiconformal mapping

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasiconformal_mapping)

An [orientation](algebraic-topology.md#orientation-of-a-simplex)-preserving [homeomorphism](topology.md#homeomorphism) with locally $L^2$ [weak derivatives](distribution-theory.md#weak-derivative) and essentially bounded infinitesimal distortion. In [holomorphic coordinates](complex-geometry.md#holomorphic-coordinate), its [Beltrami coefficient](#beltrami-coefficient) satisfies $\|\mu\|_\infty<1$, and the [maximal dilatation](#maximal-dilatation) is $(1+\|\mu\|_\infty)/(1-\|\mu\|_\infty)$.

#### Maximal dilatation

↑ **Parent:** [Quasiconformal mapping](#quasiconformal-mapping)

The essential supremum of the ratio of the largest to the smallest infinitesimal [singular value](linear-algebra.md#singular-value) of a [quasiconformal map](#quasiconformal-mapping). It equals $(1+\|\mu_f\|_\infty)/(1-\|\mu_f\|_\infty)$ in terms of the [Beltrami coefficient](#beltrami-coefficient).

#### Beltrami coefficient

↑ **Parent:** [Quasiconformal mapping](#quasiconformal-mapping)

For an [orientation](algebraic-topology.md#orientation-of-a-simplex)-preserving [quasiconformal map](#quasiconformal-mapping), the almost-everywhere coefficient $\mu_f=f_{\bar z}/f_z$. It is a coordinate-dependent representative of a tensor; the modulus and the resulting [maximal dilatation](#maximal-dilatation) are coordinate-independent.

##### Beltrami equation

↑ **Parent:** [Beltrami coefficient](#beltrami-coefficient)

The equation $f_{\bar z}=\mu f_z$ prescribing the [Beltrami coefficient](#beltrami-coefficient) of a [quasiconformal map](#quasiconformal-mapping). Two homeomorphic solutions on the same source differ by a [biholomorphism](#biholomorphism) between their targets.

### Conformal metric

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

In a [holomorphic coordinate](complex-geometry.md#holomorphic-coordinate), a length element $\rho(z)|dz|$. [Smooth](analysis.md#smooth-function) positive densities define ordinary [Riemannian metrics](differential-geometry.md#riemannian-metric); [extremal length](#extremal-length) also permits nonnegative measurable densities with finite positive area $\int\rho^2\,dx\,dy$.

### Translation surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Translation_surface)

A surface with an atlas outside finitely many cone points whose changes of coordinate are [translations](geometry-and-topology.md#translation-geometry). On a [compact](topology.md#compact-space) surface it is equivalent to a nonzero [holomorphic one-form](complex-geometry.md#holomorphic-one-form). A zero of order $m$ has [cone angle](differential-geometry.md#cone-angle) $2\pi(m+1)$.

#### Slit connected sum of translation tori

↑ **Parent:** [Translation surface](#translation-surface)

Cut equal straight slits in two [translation surfaces](#translation-surface) of [genus](topology.md#genus-of-a-surface) one and cross-glue their banks by translation. The [connected sum of oriented manifolds](differential-geometry.md#connected-sum-of-oriented-manifolds) has [genus](topology.md#genus-of-a-surface) two and two cone points of angle $4\pi$, hence two simple zeros of its [holomorphic one-form](complex-geometry.md#holomorphic-one-form). Choosing one [torus](topology.md#torus) of side $\delta$ and a slit of length $\delta^2$ creates a flat-small handle without forcing its generator to have small [extremal length](#extremal-length).

<h3 id="teichmuller-theory">Teichmüller theory</h3>

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

The study of deformations and markings of [Riemann surfaces](#riemann-surfaces), using [quasiconformal maps](#quasiconformal-mapping), [holomorphic quadratic differentials](complex-geometry.md#holomorphic-quadratic-differential), [extremal length](#extremal-length) and the [mapping class group](topology.md#mapping-class-group).

<h4 id="teichmuller-map">Teichmüller map</h4>

↑ **Parent:** [Teichmüller theory](#teichmuller-theory)

A [quasiconformal map](#quasiconformal-mapping) whose [Beltrami coefficient](#beltrami-coefficient) is $k|q|/q$ for an integrable nonzero [holomorphic quadratic differential](complex-geometry.md#holomorphic-quadratic-differential) and constant $0<k<1$. In a [flat coordinate](complex-geometry.md#natural-coordinate-of-a-holomorphic-differential) for $q$, it stretches the horizontal and vertical directions with ratio $K=(1+k)/(1-k)$. Positive multiples of $q$ define the same coefficient.

<h5 id="teichmuller-s-uniqueness-theorem">Teichmüller's uniqueness theorem</h5>

↑ **Parent:** [Teichmüller map](#teichmuller-map)

On a closed [genus](topology.md#genus-of-a-surface)-at-least-two [Riemann surface](#riemann-surfaces), a [Teichmüller map](#teichmuller-map) uniquely minimizes [maximal dilatation](#maximal-dilatation) in its [homotopy class](algebraic-topology.md#homotopy-class) among maps to the same target. The [Reich–Strebel inequality](#reich-strebel-inequality) forces equality of [Beltrami coefficients](#beltrami-coefficient) for an extremal competitor; their conformal difference is [homotopic](algebraic-topology.md#homotopy) to the identity and hence is the identity. In [genus](topology.md#genus-of-a-surface) one, translations must be factored out.

<h5 id="reich-strebel-inequality">Reich–Strebel inequality</h5>

↑ **Parent:** [Teichmüller map](#teichmuller-map)

On closed [Riemann surfaces](#riemann-surfaces) of [genus](topology.md#genus-of-a-surface) at least two, if a [Teichmüller map](#teichmuller-map) $f_0:X\to Y$ has unit-area source differential $q$ and dilatation $K_0$, any [quasiconformal map](#quasiconformal-mapping) $f:X\to Y$ in the same [homotopy class](algebraic-topology.md#homotopy-class) satisfies $K_0\leq\int_X|q|\,|1+\mu_fq/|q||^2/(1-|\mu_f|^2)$. The plus sign corresponds to a [Teichmüller map](#teichmuller-map) with $\mu_{f_0}=k_0|q|/q$ and $K_0=(1+k_0)/(1-k_0)$. This fundamental inequality yields [Teichmüller's uniqueness theorem](#teichmuller-s-uniqueness-theorem) by the pointwise [triangle inequality](topological-analysis.md#triangle-inequality) and its equality case. See [Gardiner and Hu, §5, equation (11)](https://userhome.brooklyn.cuny.edu/gardiner/A%20short%20course%20on%20Teichmuller%27s%20theorem.pdf).

#### Extremal length

↑ **Parent:** [Teichmüller theory](#teichmuller-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extremal_length)

For a [path family](geometry-and-topology.md#path-family) $\Gamma$ on a [Riemann surface](#riemann-surfaces), take the supremum of $L_\rho(\Gamma)^2/A_\rho$ over measurable [conformal metrics](#conformal-metric) of finite positive area. This is unchanged under [conformal equivalence](geometry-and-topology.md#conformal-equivalence), and a [quasiconformal map](#quasiconformal-mapping) of [maximal dilatation](#maximal-dilatation) $K$ changes it by a factor between $K^{-1}$ and $K$.

##### Extremal length lower bound from a closed one-form

↑ **Parent:** [Extremal length](#extremal-length)

Let $\alpha$ be a real [closed differential form](differential-form.md#closed-differential-form) on a [Riemann surface](#riemann-surfaces), of finite positive conformal energy $E=\int|\alpha|^2\,dA$. If its period on a loop [homotopy class](algebraic-topology.md#homotopy-class) $\gamma$ is $p$, then $\lambda(\gamma,X)\geq p^2/E$. Indeed the [conformal metric](#conformal-metric) $\rho=|\alpha|$ has area $E$ and each loop in the class has length at least $|\int\alpha|=|p|$. Energy is independent of the auxiliary [smooth](analysis.md#smooth-function) [conformal metric](#conformal-metric) used to compute the pointwise norm: the inverse scaling of the squared norm cancels the area scaling.

##### Conformal modulus of an annulus

↑ **Parent:** [Extremal length](#extremal-length)

The height divided by circumference in a conformal Euclidean cylinder model of an [annulus](topology.md#annulus-mathematics). For $r<|z|<R$, it is $(2\pi)^{-1}\log(R/r)$. The [extremal length](#extremal-length) of winding-one core curves is $1/M$, whereas that of curves joining the two boundary components is $M$.

###### Conformal cylinder

↑ **Parent:** [Conformal modulus of an annulus](#conformal-modulus-of-an-annulus)

The quotient of a horizontal strip by a horizontal translation. The model $(\mathbb R/\mathbb Z)\times(0,M)$ has [conformal modulus of an annulus](#conformal-modulus-of-an-annulus) $M$. Averaging horizontal loop lengths and applying [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) proves that the core-loop [extremal length](#extremal-length) equals $1/M$.

#### SL2R action on differentials

↑ **Parent:** [Teichmüller theory](#teichmuller-theory)

For nonzero [holomorphic one-forms](complex-geometry.md#holomorphic-one-form) and [holomorphic quadratic differentials](complex-geometry.md#holomorphic-quadratic-differential), apply $A\in\mathrm{SL}_2(\mathbb R)$ to every [flat coordinate](complex-geometry.md#natural-coordinate-of-a-holomorphic-differential). Translation and sign transition maps remain of the same type, defining a new [complex structure](complex-geometry.md#complex-structure) and differential. Composition gives a [group action](group-theory.md#group-action), [zero orders](complex-geometry.md#order-of-a-zero-of-a-differential) persist and area is preserved. The zero section has no such atlas; fixing it gives only a set-theoretic extension that is generally discontinuous.

<h4 id="teichmuller-space">Teichmüller space</h4>

↑ **Parent:** [Teichmüller theory](#teichmuller-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Teichmüller_space)

For a fixed closed oriented surface $S_g$, a point is a marked [Riemann surface](#riemann-surfaces) $(X,f:S_g\to X)$, modulo [biholomorphisms](#biholomorphism) intertwining the markings up to [homotopy](algebraic-topology.md#homotopy). For $g\geq2$, [Fenchel–Nielsen coordinates](geometry-and-topology.md#fenchel-nielsen-coordinates) give real dimension $6g-6$.

### Local coordinate

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A local coordinate at a point $p$ of a [Riemann surface](#riemann-surfaces) is a [biholomorphism](#biholomorphism) from a neighbourhood of $p$ to an open subset of $\mathbb C$. After translating the image, one may require that the coordinate sends $p$ to zero.

### Holomorphic map

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A map between Riemann surfaces is holomorphic when its expression in every pair of local complex coordinates is a [holomorphic function](#holomorphic-function).

#### Biholomorphism

↑ **Parent:** [Holomorphic map](#holomorphic-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biholomorphism)

A biholomorphism is a bijective [holomorphic map](#holomorphic-map) whose inverse is holomorphic. A degree-one nonconstant holomorphic map between compact connected Riemann surfaces is a biholomorphism.

### Germ of a holomorphic function

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A germ at $z\in D$ is an equivalence class $[f]_z$ of holomorphic functions defined near $z$, where two representatives are equivalent when they agree on some neighbourhood of $z$.

It is the holomorphic-function case of a [germ](function.md#germ-mathematics).

#### Function element

↑ **Parent:** [Germ of a holomorphic function](#germ-of-a-holomorphic-function)

A function element is a pair $(f,D)$ consisting of a nonempty disk and a [holomorphic function](#holomorphic-function) on that disk. Its local value determines a [germ of a holomorphic function](#germ-of-a-holomorphic-function). Elements agreeing on an overlapping neighborhood continue one another; chains of such continuations produce the [complete analytic function](#complete-analytic-function) generated by an element. An algebraic identity holding in one element persists along any continuation chain by the [identity theorem](#identity-theorem).

#### Space of germs of holomorphic functions

↑ **Parent:** [Germ of a holomorphic function](#germ-of-a-holomorphic-function)

The space $\mathcal G$ of germs over a domain $D$ has basic open sheets

$$
\{[f]_z:z\in U\}
$$

for holomorphic $f$ on open $U\subseteq D$. The projection $\pi([f]_z)=z$ restricts to a homeomorphism on each sheet, and these projections form holomorphic coordinate charts.

##### Analytic germ projection

↑ **Parent:** [Space of germs of holomorphic functions](#space-of-germs-of-holomorphic-functions)

The projection $[f]_z\mapsto z$ is a local [biholomorphism](#biholomorphism) for the sheet topology on the [space of germs of holomorphic functions](#space-of-germs-of-holomorphic-functions). It need not be a topological [covering map](algebraic-topology.md#covering-space): branches may end at singularities even when another branch remains over that base point.

###### Surjective inverse-polynomial germ projection without even covering

↑ **Parent:** [Analytic germ projection](#analytic-germ-projection)

The inverse germs of $w^3-3w$ over $\mathbb C$ form the connected surface $\mathbb C\setminus\{-1,1\}$. Its projection is surjective and locally biholomorphic, but the fibres have three points generically and one point at each critical value $\pm2$, so it is not an evenly covered topological covering.

##### Evaluation map on a space of germs

↑ **Parent:** [Space of germs of holomorphic functions](#space-of-germs-of-holomorphic-functions)

The evaluation map $\mathcal E([f]_z)=f(z)$ is holomorphic. On the sheet associated with $(U,f)$, its coordinate expression is exactly the holomorphic function $f$.

##### Germ surface of the square root of z to the eighth minus one

↑ **Parent:** [Space of germs of holomorphic functions](#space-of-germs-of-holomorphic-functions)

Over $D=\mathbb C\setminus\{z:z^8=1\}$, the two-valued square root is represented by

$$
R=\{(z,w)\in D\times\mathbb C:w^2=z^8-1\}.
$$

The maps $\pi(z,w)=z$ and $\mathcal E(z,w)=w$ identify this unbranched double cover analytically with the corresponding component of the space of germs.

### Complex structure lifted through a covering map

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

If $\pi:S\to R$ is a covering of a Riemann surface, compose every chart on an evenly covered open set with each local inverse sheet of $\pi$. The resulting transition maps are those of $R$, so they define a unique complex structure making $\pi$ a local biholomorphism.

### Uniformization theorem

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniformization_theorem)

Every simply connected Riemann surface is biholomorphic to the Riemann sphere, the complex plane, or the unit disc.

#### Thrice-punctured sphere as a modular quotient

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

The level-two [principal congruence subgroup](group-theory.md#principal-congruence-subgroup) $\Gamma(2)\subset\operatorname{PSL}_2(\mathbb R)$ consists of integer determinant-one matrices congruent to the identity modulo two, modulo the scalar sign. It acts freely and properly discontinuously on the [complex upper half-plane](#upper-half-plane-complex-analysis). An ideal quadrilateral with vertices $-1,0,1,\infty$ has its paired sides identified by $\tau\mapsto\tau+2$ and $\tau\mapsto\tau/(1-2\tau)$. The quotient has genus zero and three punctures, so it is conformally the sphere with three points removed. The invariant metric $|d\tau|/\operatorname{Im}\tau$ descends to its curvature-minus-one [hyperbolic metric](geometry-and-topology.md#hyperbolic-metric).

// Destination: analysis.bigb

#### Green-function exhaustion proof of disk uniformization

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

Exhaust a simply connected [hyperbolic Riemann surface in potential theory](#hyperbolic-riemann-surface-in-potential-theory) by compact bordered Jordan domains $R_n$. Their [Green functions on a Riemann surface](analysis.md#green-function-on-a-riemann-surface) $G_n(\cdot,p)$ have logarithmic poles and zero boundary values. Exponentiating their harmonic conjugates produces proper degree-one maps $f_n:R_n\to\mathbb D$ with $f_n(p)=0$. If $G_n=-\log|\zeta|+c_n+o(1)$, normalize $f_n'(p)=e^{-c_n}>0$. Domain monotonicity and a global positive Green function bound $c_n$ increasingly from above. Thus [Montel theorem](complex-dynamics.md#montel-s-theorem) gives a nonconstant limit $F$, which is injective by the [locally uniform limit of univalent functions](#locally-uniform-limit-of-univalent-functions) theorem. The [Schwarz lemma](analysis.md#schwarz-lemma) makes $F'(p)$ extremal among normalized disk-valued maps. If $F$ omitted $a\ne0$, taking a global [holomorphic square root](#holomorphic-square-root) of a disk automorphism applied to $F$, then renormalizing at $p$, would multiply its derivative by $(1+|a|)/(2\sqrt{|a|})>1$. Thus $F$ is onto and gives the desired [biholomorphism](#biholomorphism).

#### Riemann mapping theorem

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_mapping_theorem)

Every nonempty simply connected proper open subset of the [complex plane](#complex-plane) is [conformally equivalent](geometry-and-topology.md#conformal-equivalence) to the [unit disc](topology.md#unit-disc).

##### Square-root improvement of a normalized conformal map

↑ **Parent:** [Riemann mapping theorem](#riemann-mapping-theorem)

For a [univalent function](#univalent-function) $f:\Omega\to\mathbb D$ with $f(z_0)=0$, suppose $a\ne0$ is omitted. Apply the disk automorphism $T_a$ so the resulting image omits zero, take a [holomorphic square root](#holomorphic-square-root), then apply the disk automorphism taking the value at $z_0$ to zero. If $\Omega$ is a [simply connected domain](#simply-connected-domain), the root exists. The resulting normalized univalent map has derivative magnitude multiplied by $(1+|a|)/(2\sqrt{|a|})>1$, since $(1-\sqrt{|a|})^2>0$. Thus a map maximizing the derivative cannot omit an interior disk point.

##### Caratheodory boundary extension theorem

↑ **Parent:** [Riemann mapping theorem](#riemann-mapping-theorem)

For a bounded [simply connected domain](#simply-connected-domain) $D$ and a [conformal bijection](#biholomorphism) $f:\mathbb D\to D$, $f$ extends continuously to the closed disc if and only if $\partial D$ is a [locally connected space](topology.md#locally-connected-space). A Jordan [boundary](topology.md#boundary-of-a-set) gives a homeomorphism of closed discs, but [local connectedness](topology.md#locally-connected-space) alone need not give injectivity on the [boundary](topology.md#boundary-of-a-set): a slit has two [boundary](topology.md#boundary-of-a-set) approaches. The same statement applies on the sphere to unbounded [domains](topology.md#domain-mathematical-analysis) after a suitable change of coordinates. This [boundary](topology.md#boundary-of-a-set) theorem is different from the [Caratheodory extension theorem](measure-theory.md#caratheodory-s-extension-theorem) for measures.

##### Koebe distortion theorem

↑ **Parent:** [Riemann mapping theorem](#riemann-mapping-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koebe_distortion_theorem)

The Koebe distortion theorem gives universal upper and lower bounds on a univalent function and its derivative in terms of the distance to the boundary. In particular, derivatives at two points whose hyperbolic distance is bounded differ by at most a universal multiplicative factor.

###### Koebe quarter theorem

↑ **Parent:** [Koebe distortion theorem](#koebe-distortion-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koebe_quarter_theorem)

If $f$ is a [univalent function](#univalent-function) on the [unit disc](topology.md#unit-disc), then $B(f(0),|f'(0)|/4)\subseteq f(\mathbb D)$. The constant $1/4$ is sharp, as shown by the [Koebe function](#koebe-function). This gives useful comparisons between the [derivative](calculus.md#derivative) of a [conformal map](geometry-and-topology.md#conformal-map), its [conformal radius](geometry-and-topology.md#conformal-radius), and its distance to the [domain boundary](topology.md#boundary-of-a-domain).

###### Boundary-distance derivative bound for a conformal bijection

↑ **Parent:** [Koebe quarter theorem](#koebe-quarter-theorem)

For a [conformal bijection](#biholomorphism) $f:D\to\widetilde D$ between proper planar [domains](topology.md#domain-mathematical-analysis), put $d=\operatorname{dist}(z,\partial D)$ and $\widetilde d=\operatorname{dist}(f(z),\partial\widetilde D)$. Apply the [Koebe quarter theorem](#koebe-quarter-theorem) to $(f(z+dw)-f(z))/(df'(z))$ on the [unit disc](topology.md#unit-disc) to obtain $d|f'(z)|/4\leq\widetilde d$. Apply it again to $f^{-1}$ to get the opposite bound. Thus $\boxed{\widetilde d/(4d)\leq|f'(z)|\leq4\widetilde d/d}$. The [domains](topology.md#domain-mathematical-analysis) need not be [simply connected domains](#simply-connected-domain). For the whole plane, the [boundary](topology.md#boundary-of-a-set) distances are infinite and these ratios are undefined.

#### Automorphisms of simply connected Riemann surfaces

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

The sphere has the Möbius group $PGL_2(\mathbb C)$, the plane has the affine maps $z\mapsto az+b$ with $a\ne0$, and the disc has the maps $e^{i\theta}(z-a)/(1-\bar az)$ with $|a|<1$.

#### Riemann surfaces uniformized by the complex plane

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

The quotients of $\mathbb C$ by free properly discontinuous conformal actions are $\mathbb C$, $\mathbb C^*$, and the complex tori $\mathbb C/\Lambda$. The translation group has respectively rank zero, one, or two.

#### Plane domain with two omitted points is hyperbolic

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

Every plane domain whose complement contains at least two points is uniformized by the unit disc. A plane universal cover would give a nonconstant entire function omitting two values, contrary to the [Little Picard theorem](#little-picard-theorem).

#### Uniformization of a punctured compact Riemann surface

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

Let $R$ be a compact [Riemann surface](#riemann-surfaces) of [genus](topology.md#genus-of-a-surface) $g$, and remove $n$ distinct points. The punctured surface is uniformized by the [unit disc](topology.md#unit-disc) exactly when $2g-2+n>0$. It is uniformized by the [complex plane](#complex-plane) exactly when $2g-2+n$ is $-1$ or $0$, corresponding respectively to $\mathbb C$, and to $\mathbb C^*$ or a [complex torus](complex-geometry.md#complex-torus). The sole spherical case is $g=n=0$.

#### Compact Riemann surface containing an embedded punctured plane

↑ **Parent:** [Uniformization theorem](#uniformization-theorem)

If $\mathbb C^*$ embeds holomorphically in a compact Riemann surface $R$, the embedding extends across zero and infinity to a degree-one holomorphic map from the [Riemann sphere](#riemann-sphere) to $R$. Hence $R$ is conformally the sphere.

### Identity theorem on a Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

Two holomorphic functions on a connected Riemann surface that agree on a set with an accumulation point agree everywhere. Local charts reduce the proof to isolated zeros of a one-variable holomorphic function.

### Harmonic function on a Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A real-valued function on a Riemann surface is harmonic when its expression in every holomorphic coordinate chart has vanishing planar Laplacian.

#### Conformal invariance of harmonicity

↑ **Parent:** [Harmonic function on a Riemann surface](#harmonic-function-on-a-riemann-surface)

Under a holomorphic coordinate change $w=w(z)$,

$$
\Delta_z(H\circ w)=|w'(z)|^2(\Delta_wH)\circ w,
$$

so the condition $\Delta H=0$ is independent of the holomorphic chart.

### Regular covering map

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A covering is regular when its deck group acts transitively on each fibre, equivalently when its fundamental-group subgroup is normal.

### Complete analytic function

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A complete analytic function is the collection of all continuations of a germ. Its Riemann surface consists of these germs, with projection to their base points.

### Valency theorem

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

For a nonconstant analytic map $f:R\to S$ between compact connected Riemann surfaces, there is an integer $\deg f$ such that for every $w\in S$,

$$
\sum_{z\in f^{-1}(w)}m_f(z)=\deg f.
$$

The degree counts sheets with multiplicity of the associated [branched covering](algebraic-topology.md#branched-covering).

#### Local degree of a holomorphic map

↑ **Parent:** [Valency theorem](#valency-theorem)

If a nonconstant holomorphic map has local-coordinate expression

$$
f(z)-f(p)=a(z-p)^m+O((z-p)^{m+1}),
\qquad a\ne0,
$$

then $m=m_f(p)$ is its local degree, multiplicity, or ramification index at $p$.

#### Degree of a holomorphic map

↑ **Parent:** [Valency theorem](#valency-theorem)

For a nonconstant holomorphic map $f:X\to Y$ between compact connected Riemann surfaces, its degree is

$$
\deg f=\sum_{p\in f^{-1}(y)}m_f(p).
$$

The [valency theorem](#valency-theorem) says that this integer is independent of $y\in Y$.

##### Degree of a power map of the Riemann sphere

↑ **Parent:** [Degree of a holomorphic map](#degree-of-a-holomorphic-map)

For $k\ge1$, the power map has $k$ distinct preimages of every nonzero finite [regular value](differential-geometry.md#regular-value), all with positive local [degree of a map between oriented manifolds](homology.md#degree-of-a-map-between-oriented-manifolds). Integrating the [pullback of a differential form](differential-form.md#pullback-of-a-differential-form) of $\Omega=i\,d\zeta\wedge d\bar\zeta/(1+|\zeta|^2)^2$ gives the same answer, since $\int\Omega=2\pi$ and $\int f^*\Omega=2\pi k$. For $k=0$ use the constant extension $1$ at infinity; its [degree of a map between oriented manifolds](homology.md#degree-of-a-map-between-oriented-manifolds) is zero.

#### Degree of a rational map of the Riemann sphere

↑ **Parent:** [Valency theorem](#valency-theorem)

After cancelling common factors, the rational map $p/q$ on the Riemann sphere has degree $\max(\deg p,\deg q)$. It is an analytic isomorphism exactly when this degree is one, equivalently when it is a Möbius transformation.

##### Degree bounds for the derivative of a rational function

↑ **Parent:** [Degree of a rational map of the Riemann sphere](#degree-of-a-rational-map-of-the-riemann-sphere)

For a nonconstant [rational function](isolated-singularity.md#rational-function) of degree $n$, its derivative has degree between $n-1$ and $2n$. A finite pole of order $m$ becomes one of order $m+1$. If infinity is a pole of order $p-q>0$, it contributes $p-q-1$ to the derivative's pole count, where $p,q$ are the degrees of coprime numerator and denominator. This proves the lower bound; the quotient rule denominator $Q^2$ proves the upper bound. The functions $z^n$ and $1/(z^n-1)$ attain the bounds.

##### Degree of the derivative of a rational function

↑ **Parent:** [Degree of a rational map of the Riemann sphere](#degree-of-a-rational-map-of-the-riemann-sphere)

Let a nonconstant rational function $f$ have degree $d$, let $r$ be its number of distinct finite poles, and let $m_\infty$ be its pole order at infinity, taken as zero when infinity is not a pole. Differentiation raises each finite pole order by one and changes a pole of order $m_\infty>0$ at infinity into one of order $m_\infty-1$. Hence

$$
\deg f'=
\begin{cases}
d+r-1,&m_\infty>0,\\
d+r,&m_\infty=0.
\end{cases}
$$

In particular, $d-1\leq\deg f'\leq2d$.

#### Degree of an elliptic function

↑ **Parent:** [Valency theorem](#valency-theorem)

The degree of a nonconstant elliptic function is the sum of the orders of its poles in a fundamental parallelogram. Equivalently, it is the degree of the induced holomorphic map from its complex torus to the Riemann sphere.

##### Degree of the derivative of an elliptic function

↑ **Parent:** [Degree of an elliptic function](#degree-of-an-elliptic-function)

If an elliptic function $g$ has degree $d$ and $r$ distinct poles in a fundamental parallelogram, then each pole order increases by one under differentiation, so

$$
\deg g'=d+r.
$$

Because $1\leq r\leq d$, this gives $d+1\leq\deg g'\leq2d$.

#### Octahedral rotation orbits on the Riemann sphere

↑ **Parent:** [Valency theorem](#valency-theorem)

The rotation group of the octahedron has order $24$. Its vertex, face-centre, and edge-centre stabilizers have orders $4,3,2$, giving exceptional orbit sizes $6,8,12$; every other orbit has size $24$.

#### Degree-sized invariant separates finite-group orbits

↑ **Parent:** [Valency theorem](#valency-theorem)

Let a finite group $G$ of order $d$ act analytically on a compact Riemann surface, and let an invariant analytic map $F$ have degree $d$. At a point with stabilizer of order $e$, invariance forces the local multiplicity of $F$ to be at least $e$. Its orbit has $d/e$ points, so it already contributes at least $d$ to the fibre multiplicity. The valency theorem forces equality and shows that every fibre is exactly one orbit.

### Riemann-Hurwitz formula

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann–Hurwitz_formula)

For a degree-$d$ holomorphic map, $2g_X-2=d(2g_Y-2)+\sum(e_p-1)$.

#### Ramification index of a holomorphic map

↑ **Parent:** [Riemann-Hurwitz formula](#riemann-hurwitz-formula)

For a nonconstant holomorphic map of Riemann surfaces, choose local coordinates centred at $p$ and $f(p)$. The map has the form

$$
z\longmapsto z^{e_p}u(z),
\qquad u(0)\ne0.
$$

The positive integer $e_p$ is its ramification index. The point is ramified exactly when $e_p>1$ and contributes $e_p-1$ to the ramification divisor.

##### Ramification point of a holomorphic map

↑ **Parent:** [Ramification index of a holomorphic map](#ramification-index-of-a-holomorphic-map)

A point $p$ is ramified when its local degree $e_p$ is greater than one.

###### Critical point of a rational map

↑ **Parent:** [Ramification point of a holomorphic map](#ramification-point-of-a-holomorphic-map)

For a nonconstant rational map, choose local source and target coordinates centred at $p$ and $R(p)$. If the local expression is $a u^e+O(u^{e+1})$ with $a\ne0$, its local degree is $e$, and $p$ is critical exactly when $e\geq2$. This definition covers poles and infinity; a simple pole is not critical merely because the usual finite-coordinate expression is unbounded. Coordinate changes have nonzero first derivatives and leave $e$ unchanged.

###### Critical orbit of a rational map

↑ **Parent:** [Critical point of a rational map](#critical-point-of-a-rational-map)

A critical orbit is the forward sequence $p,R(p),R^2(p),\ldots$ starting at a [critical point of a rational map](#critical-point-of-a-rational-map). The [postcritical set](complex-dynamics.md#postcritical-set) records the forward images, usually from the first iterate onward, of all critical points; a single critical orbit and the union of all such images are distinct notions. For quadratic polynomials there is one finite critical point, zero, and its orbit controls connectedness of the filled Julia set and membership in the [Mandelbrot set](complex-dynamics.md#mandelbrot-set). A bounded orbit can be preperiodic to a repelling cycle, as $0\mapsto i\mapsto-1+i\mapsto-i\mapsto-1+i$ for $z^2+i$; boundedness then does not imply Fatou membership.

###### Critical points of iterates of a rational map

↑ **Parent:** [Critical point of a rational map](#critical-point-of-a-rational-map)

Local degrees multiply under composition: $e_p(S\circ R)=e_p(R)e_{R(p)}(S)$, directly by substituting the two local power-series expansions. Consequently

$$
\operatorname{Crit}(R^n)=\bigcup_{j=0}^{n-1}R^{-j}(\operatorname{Crit}(R)).
$$

In particular every critical point of $R$ remains critical for each positive iterate, and every critical point of an iterate reaches a critical point of $R$ in fewer than $n$ steps. This covers infinity as well as finite points. For polynomials at finite points the same conclusion follows from $(P^n)'(z)=\prod_{j=0}^{n-1}P'(P^j(z))$.

###### Critical multiplicity of a rational map

↑ **Parent:** [Critical point of a rational map](#critical-point-of-a-rational-map)

At a point of local degree $e$, the critical multiplicity is $e-1$. At an ordinary finite point this is the order of vanishing of the derivative. The invariant local-coordinate definition also works at poles and infinity. For $R(z)=z^d$, zero and infinity both have multiplicity $d-1$, so a critical-point count must count multiplicities: there are two distinct critical points but total multiplicity $2d-2$.

###### Total critical multiplicity of a rational map

↑ **Parent:** [Critical multiplicity of a rational map](#critical-multiplicity-of-a-rational-map)

A degree-$d$ rational map has total critical multiplicity $2d-2$. Here is an algebraic proof. Critical points are isolated zeros of local derivatives and are finite in number by compactness. Change domain and range Möbius coordinates so that the poles are $d$ simple finite poles and infinity is a regular point with a finite image. Write $R=P/Q$, with $\deg Q=d$, and $R(z)=a+b/z+O(z^{-2})$, $b\ne0$. Then $W=P'Q-PQ'$ has degree exactly $2d-2$, since $R'=W/Q^2\sim-b/z^2$. At a pole, $W=-PQ'\ne0$. Thus the roots of $W$ are precisely the critical points and their zero orders are the critical multiplicities. The fundamental theorem of algebra gives the count; the coordinate changes preserve it.

###### Branch value of a holomorphic map

↑ **Parent:** [Ramification point of a holomorphic map](#ramification-point-of-a-holomorphic-map)

A branch value is the image of a [ramification point of a holomorphic map](#ramification-point-of-a-holomorphic-map). Away from all branch values, a proper holomorphic map is an ordinary unramified covering.

###### Ramification at infinity of a superelliptic covering

↑ **Parent:** [Branch value of a holomorphic map](#branch-value-of-a-holomorphic-map)

In the compactified [Riemann surface](#riemann-surfaces) of $w^r=z^n-1$, a positive circuit enclosing the $n$ simple finite zeros sends the sheet label $j$ to $j+n$ modulo $r$. This permutation has $d=\gcd(n,r)$ cycles of length $r/d$. Each cycle fills in one point over infinity, with ramification index $r/d$. Hence infinity is unramified exactly when $r$ divides $n$. Each finite zero has ramification index $r$, so the base sphere has exactly $n$ branch values in that case and $n+1$ otherwise.

#### Triangulation proof of the Riemann-Hurwitz formula

↑ **Parent:** [Riemann-Hurwitz formula](#riemann-hurwitz-formula)

Triangulate the target with all branch values among its vertices. For a degree-$d$ map, every edge and face has $d$ lifts. Above a target vertex $v$, the number of lifted vertices is

$$
d-\sum_{p\mapsto v}(e_p-1),
$$

because $\sum_{p\mapsto v}e_p=d$. Thus

$$
\chi(X)=d\chi(Y)-\sum_p(e_p-1),
$$

which is equivalent to the [Riemann-Hurwitz formula](#riemann-hurwitz-formula).

#### Affine normal forms of a complex cubic polynomial

↑ **Parent:** [Riemann-Hurwitz formula](#riemann-hurwitz-formula)

Up to invertible affine changes in source and target, every complex cubic polynomial is exactly one of

$$
z^3,
\qquad
z\left(\frac{z^2}{3}-1\right).
$$

The extension to the [Riemann sphere](#riemann-sphere) has two finite units of ramification. A single finite critical point has ramification index three and gives the first form; two distinct simple critical points can be moved to $\pm1$, after which integration gives the second.

### Riemann sphere

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_sphere)

The Riemann sphere is $\mathbb C\cup\{\infty\}$ with two charts related by reciprocal coordinates.

#### Chordal metric

↑ **Parent:** [Riemann sphere](#riemann-sphere)

The chordal metric on the [Riemann sphere](#riemann-sphere) is $\chi(z,w)=|z-w|/\sqrt{(1+|z|^2)(1+|w|^2)}$ for finite points, with $\chi(z,\infty)=(1+|z|^2)^{-1/2}$. It is half the Euclidean chord distance between stereographic images on the unit sphere, so the triangle inequality follows from the Euclidean one. If $\rho$ is round spherical geodesic distance, then $\rho=2\arcsin\chi$ and $2\chi\leq\rho\leq\pi\chi$. These inequalities transfer uniform-continuity estimates between spherical and chordal distances, including at poles of meromorphic functions.

##### Rational map is Lipschitz in the chordal metric

↑ **Parent:** [Chordal metric](#chordal-metric)

A rational map is smooth as a map between compact round spheres, including at its poles in reciprocal coordinates. Its spherical differential norm therefore has a finite supremum $L$. Integrating along a shortest spherical geodesic gives $\rho(Rz,Rw)\leq L\rho(z,w)$. Since $2\chi\leq\rho\leq\pi\chi$, we obtain $\chi(Rz,Rw)\leq(\pi L/2)\chi(z,w)$. In finite coordinates the differential norm is $R^\#(z)=|R'(z)|(1+|z|^2)/(1+|R(z)|^2)$, extending continuously to the whole sphere. This uniform bound is useful for passing equicontinuity through compositions.

#### Stereographic projection

↑ **Parent:** [Riemann sphere](#riemann-sphere)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stereographic_projection)

Stereographic projection identifies a sphere minus one pole with the plane and supplies the standard charts of the Riemann sphere.

##### Circle-plane relation under stereographic projection

↑ **Parent:** [Stereographic projection](#stereographic-projection)

For north-pole [stereographic projection](#stereographic-projection) $z=(X+iY)/(1-Z)$ on the [unit sphere](topology.md#unit-sphere), substitute $|z|^2=(1+Z)/(1-Z)$ into a planar circle equation. The displayed plane equation follows, and its intersection with the sphere is a [circle](topology.md#circle). The plane contains the sphere's centre exactly when $r^2=1+|c|^2$, giving a [great circle](geometry-and-topology.md#great-circle).

###### Antipodal equatorial intersection criterion for a great circle

↑ **Parent:** [Circle-plane relation under stereographic projection](#circle-plane-relation-under-stereographic-projection)

A planar circle other than the unit circle lifts to a [great circle](geometry-and-topology.md#great-circle) exactly when it meets the unit circle at two opposite points. A great circle other than the equator intersects the equator in an [antipodal pair](geometry-and-topology.md#antipodal-pair). Conversely the plane containing a lifted circle and an antipodal pair contains their midpoint, the sphere's centre. Algebraically, adding the equations $|z-c|^2=r^2$ and $|-z-c|^2=r^2$ with $|z|=1$ gives the displayed condition.

##### Antipodal stereographic coordinate relation

↑ **Parent:** [Stereographic projection](#stereographic-projection)

For north-pole [stereographic projection](#stereographic-projection) $p=(X+iY)/(1-Z)$ on the [unit sphere](topology.md#unit-sphere), the [antipodal pair](geometry-and-topology.md#antipodal-pair) point has coordinate $q=-(X+iY)/(1+Z)$. Since $X^2+Y^2=1-Z^2$, this gives $p\overline q=-1$ when both coordinates are finite. On the whole [Riemann sphere](#riemann-sphere), write $q=-1/\overline p$, pairing zero with infinity. The two axis endpoints fixed by a sphere [rotation](riemannian-geometry.md#rotation-mathematics) obey this relation.

###### Antipodal cross-ratio and spherical distance

↑ **Parent:** [Antipodal stereographic coordinate relation](#antipodal-stereographic-coordinate-relation)

Use the north-pole [stereographic projection](#stereographic-projection) and the [cross-ratio](group-theory.md#cross-ratio) convention $[a,b;c,d]=(a-c)(b-d)/[(a-d)(b-c)]$. Antipodes have coordinates $-1/\bar u$. Rotate the first point to the south pole, whose coordinate is zero: its antipode becomes infinity, while a point at [spherical distance](geometry-and-topology.md#great-circle-distance) $d$ has projected modulus $\tan(d/2)$. [Möbius invariance of the cross-ratio](group-theory.md#mobius-invariance-of-the-cross-ratio) then gives the displayed identity. Antipodal endpoints require the extended-value interpretation.

##### Holomorphic stereographic atlas of the sphere

↑ **Parent:** [Stereographic projection](#stereographic-projection)

On the unit [sphere](geometry-and-topology.md#sphere), use $\zeta=(x+iy)/(1-z)$ away from the north pole and $\eta=(x-iy)/(1+z)$ away from the south pole. Their overlap relation $\eta=1/\zeta$ is a [holomorphic map](#holomorphic-map), giving a [holomorphic atlas](complex-geometry.md#holomorphic-atlas) for the [Riemann sphere](#riemann-sphere). The opposite sign of $iy$ in the second [manifold chart](differential-geometry.md#manifold-chart) ensures a holomorphic rather than antiholomorphic transition.

<h5 id="sphere-rotations-as-special-unitary-mobius-transformations">Sphere rotations as special-unitary Möbius transformations</h5>

↑ **Parent:** [Stereographic projection](#stereographic-projection)

Under the [stereographic projection](#stereographic-projection) $w=(x+iy)/(1-z)$, rotations about the third axis have representatives $\operatorname{diag}(e^{i\theta/2},e^{-i\theta/2})$, and rotations about the second axis have representatives

$$
\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}.
$$

These belong to the [special unitary group](topological-group.md#special-unitary-group) $SU(2)$. Euler-angle generation of the [special orthogonal group](linear-algebra.md#special-orthogonal-group) $SO(3)$ shows that every sphere rotation becomes a [Möbius transformation](group-theory.md#mobius-transformation) represented in $SU(2)$. Representatives $U$ and $-U$ induce the same transformation.

#### Local cyclic quotient of a Riemann surface

↑ **Parent:** [Riemann sphere](#riemann-sphere)

Let a finite group $H$ of conformal automorphisms of the Riemann sphere fix $p$. The derivative representation at $p$ embeds $H$ into $\mathbb C^\times$, so $H$ is cyclic. Averaging a local coordinate linearizes the action to $z\mapsto\zeta z$, and the quotient has coordinate $u=z^{|H|}$.

##### Finite conformal quotient of a Riemann surface

↑ **Parent:** [Local cyclic quotient of a Riemann surface](#local-cyclic-quotient-of-a-riemann-surface)

For a finite conformal group action, choose a disc around each point that meets only its stabilizer translates. The local cyclic quotient chart $z\mapsto z^e$, where $e$ is the stabilizer order, gives the orbit space a Riemann-surface structure and makes the quotient map holomorphic.

#### Orbit-separating invariant for the standard dihedral action on the Riemann sphere

↑ **Parent:** [Riemann sphere](#riemann-sphere)

For $r(z)=\zeta z$ and $s(z)=1/z$, where $\zeta^n=1$, the rational function

$$
z^n+z^{-n}
$$

is invariant under $D_{2n}$. Equality of two values factors as $(u-v)(uv-1)=0$ for $u=z_1^n$ and $v=z_2^n$, so every fibre is exactly one dihedral orbit.

### Punctured Riemann surface

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

Removing a closed discrete set from a Riemann surface leaves an open complex one-manifold; if connected, it is again a Riemann surface.

#### Path avoidance in a surface

↑ **Parent:** [Punctured Riemann surface](#punctured-riemann-surface)

A path in a surface can be perturbed inside coordinate discs to avoid finitely many prescribed points.

#### Punctured complex plane

↑ **Parent:** [Punctured Riemann surface](#punctured-riemann-surface)

The punctured plane $\mathbb C^*$ is a connected Riemann surface homeomorphic to a cylinder.

It is the complex plane with a point removed, a special [punctured Riemann surface](#punctured-riemann-surface).

##### Cylinder as a punctured plane

↑ **Parent:** [Punctured complex plane](#punctured-complex-plane)

Polar coordinates give $\mathbb C^*\cong S^1\times\mathbb R$ after taking logarithmic radius.

### Transport of a complex structure

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A homeomorphism to a complex manifold transports its atlas and thereby defines a complex structure on the source.

### Nodal crossing

↑ **Parent:** [Riemann surfaces](#riemann-surfaces)

A nodal crossing locally consists of two complex branches meeting transversely and is not a one-dimensional complex manifold at the intersection.

For a plane [algebraic curve](algebraic-geometry.md#algebraic-curve) this crossing is an [ordinary double point](algebraic-geometry.md#ordinary-double-point), with two distinct tangent directions.

#### Topological manifold local obstruction

↑ **Parent:** [Nodal crossing](#nodal-crossing)

If a punctured neighborhood has a different number of connected components from a punctured Euclidean ball, the point is not a manifold point.

#### Reducible complex curve

↑ **Parent:** [Nodal crossing](#nodal-crossing)

A reducible complex curve is a union of proper complex subcurves; intersecting components can create singular points.

## Elliptic integral

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_integral)

An elliptic integral is an integral of a rational function of $x$ and $\sqrt{P(x)}$, where $P$ is a cubic or quartic [polynomial](polynomial.md) with distinct roots. The standard first, second and third kinds describe the essential normal forms. Choosing the full endpoint yields complete versions such as the [complete elliptic integral of the first kind](#complete-elliptic-integral-of-the-first-kind).

### Elliptic integral of the first kind

↑ **Parent:** [Elliptic integral](#elliptic-integral)

For a parameter $k$, one form of the incomplete elliptic integral of the first kind is

$$
F(z,k)=\int_0^z\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}}.
$$

Its value depends on the choices of square-root branches and, under [analytic continuation](#analytic-continuation) around the [branch points](#branch-point), on the integration path.

#### Lemniscatic integral

↑ **Parent:** [Elliptic integral of the first kind](#elliptic-integral-of-the-first-kind)

Choose the [holomorphic square root](#holomorphic-square-root) equal to one at zero on the [unit disc](topology.md#unit-disc). The resulting [elliptic integral](#elliptic-integral) maps that disc conformally onto the [square](geometry-and-topology.md#square) with vertices $\pm B,\pm iB$, where $B=\int_0^1dt/\sqrt{1-t^4}$. For the inverse [Cayley transform between the half-plane and disk](#cayley-transform-between-the-half-plane-and-disk) $h(z)=i(1+z)/(1-z)$, the square of the [derivative](calculus.md#derivative) of $F_1\circ h$, with $F_1'(w)=1/\sqrt{w(1-w^2)}$, is $2i/(1-z^4)$. Thus the two [square](geometry-and-topology.md#square) maps differ by an affine change of coordinate.

#### Complete elliptic integral of the first kind

↑ **Parent:** [Elliptic integral of the first kind](#elliptic-integral-of-the-first-kind)

For $0<k<1$, the complete elliptic integral of the first kind is

$$
K(k)=\int_0^1\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}}.
$$

It is the complete first-kind member of the [elliptic integral](#elliptic-integral) family.

##### Logarithmic endpoint asymptotic of the complete elliptic integral

↑ **Parent:** [Complete elliptic integral of the first kind](#complete-elliptic-integral-of-the-first-kind)

Here $m$ is the parameter, equal to the squared modulus. Near $m=1$ the endpoint integrand is locally $(1-m+s^2)^{-1/2}$. Matching its integral to the outer secant integral gives $L$. The next correction is of order $(1-m)\log(1/(1-m))$. Keeping the parameter/modulus convention explicit prevents a factor-of-two error in the complementary small quantity.

##### Complementary complete elliptic integral of the first kind

↑ **Parent:** [Complete elliptic integral of the first kind](#complete-elliptic-integral-of-the-first-kind)

For the complementary modulus $k'=\sqrt{1-k^2}$,

$$
K'(k)=K(k')
=\int_1^{1/k}\frac{dt}{\sqrt{(t^2-1)(1-k^2t^2)}}.
$$

## Elliptic function

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_function)

An elliptic function is a [meromorphic function](isolated-singularity.md#meromorphic-function) with two real-linearly independent [periods](mathematics.md#period-of-a-function) $\omega_1,\omega_2$. A [fundamental cell](#fundamental-parallelogram-of-a-period-lattice) is a half-open parallelogram

$$
z_0+\{s\omega_1+t\omega_2:0\leq s,t<1\}.
$$

Opposite boundary integrals cancel. Consequently a nonconstant elliptic function has equally many zeros and poles in a cell, counted with multiplicity, and the sum of its pole residues in a cell is zero.

### Zero-pole sum of an elliptic function

↑ **Parent:** [Elliptic function](#elliptic-function)

For a nonzero [elliptic function](#elliptic-function) with [period lattice](#period-lattice) $\Lambda$, its [zeros of a function](polynomial.md#zero-of-a-function) $a_j$ and [poles](isolated-singularity.md#pole) $b_j$, repeated with their [multiplicities](polynomial.md#multiplicity-mathematics), have equal total number and satisfy $\sum_j a_j-\sum_j b_j\in\Lambda$. Choose a fundamental parallelogram avoiding all zeros and poles on its boundary. The [argument principle](#argument-principle) applied to $f'/f$ gives equality of the numbers. Applying the [residue theorem](analysis.md#residue-theorem) to $zf'/f$ gives their difference of sums. Pairing opposite edges, the extra factors are the two lattice generators multiplied by integrals of $f'/f$ along an edge. These integrals are integer multiples of $2\pi i$, because the endpoints have the same nonzero function value. Thus the difference of sums is a lattice element. This links zeros of a pulled-back line to the [chord-and-tangent group law](normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law).

### Elliptic divisor-sum identity

↑ **Parent:** [Elliptic function](#elliptic-function)

For a nonzero [elliptic function](#elliptic-function), the weighted sum of its zero positions minus its pole positions belongs to the [period lattice](#period-lattice). Integrating $zf^{\prime}/f$ around a [fundamental parallelogram](#fundamental-parallelogram-of-a-period-lattice) proves this: translating opposite edges gives a lattice-linear combination of integrals of $f^{\prime}/f$, each an integer multiple of $2\pi i$. The unweighted integral proves that the zero and pole multiplicities have equal total.

### Period lattice

↑ **Parent:** [Elliptic function](#elliptic-function)

Two real-linearly independent [periods](mathematics.md#period-of-a-function) $\omega_1,\omega_2$ generate the period lattice

$$
\Lambda=\mathbb Z\omega_1+\mathbb Z\omega_2.
$$

#### Fundamental parallelogram of a period lattice

↑ **Parent:** [Period lattice](#period-lattice)

A fundamental parallelogram for $\Lambda=\mathbb Z\omega_1+\mathbb Z\omega_2$ is a translate of

$$
\{s\omega_1+t\omega_2:0\leq s,t<1\}.
$$

Its translates tile the [complex plane](#complex-plane).

### Nonconstant elliptic function has a pole

↑ **Parent:** [Elliptic function](#elliptic-function)

If an [elliptic function](#elliptic-function) had no [poles](isolated-singularity.md#pole), it would be [entire](#entire-function). It is bounded on the closure of a [fundamental parallelogram](#fundamental-parallelogram-of-a-period-lattice), and periodicity then makes it bounded on the whole [complex plane](#complex-plane). The [Liouville theorem](#liouville-theorem) would make it constant. Thus every nonconstant elliptic function has a pole.

### Jacobi elliptic functions

↑ **Parent:** [Elliptic function](#elliptic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_elliptic_functions)

The Jacobi elliptic functions include $\operatorname{sn}(u,k)$, $\operatorname{cn}(u,k)$ and $\operatorname{dn}(u,k)$, with $\operatorname{sn}^2+\operatorname{cn}^2=1$ and $\operatorname{dn}^2+k^2\operatorname{sn}^2=1$. Their ratios give the other standard members. The [Jacobi elliptic sine](#jacobi-elliptic-sine) is the inverse of the [elliptic integral of the first kind](#elliptic-integral-of-the-first-kind).

#### Jacobi elliptic sine

↑ **Parent:** [Jacobi elliptic functions](#jacobi-elliptic-functions)

The Jacobi elliptic sine is the local inverse of the [elliptic integral of the first kind](#elliptic-integral-of-the-first-kind): if

$$
u=\int_0^z\frac{dt}{\sqrt{(1-t^2)(1-k^2t^2)}},
$$

then $z=\operatorname{sn}(u,k)$. Its analytic continuation is a meromorphic doubly periodic function.

It is the sn member of the [Jacobi elliptic functions](#jacobi-elliptic-functions).

##### Period lattice of the Jacobi elliptic sine

↑ **Parent:** [Jacobi elliptic sine](#jacobi-elliptic-sine)

For real $0<k<1$, the [period lattice](#period-lattice) of $\operatorname{sn}(u,k)$ is generated by

$$
4K(k)
\quad\hbox{and}\quad
2iK'(k).
$$

The periods arise by composing the [monodromy reflections](#monodromy-reflection-at-a-square-root-branch-point) of its inverse [elliptic integral of the first kind](#elliptic-integral-of-the-first-kind).

### Value multiplicity of an elliptic function

↑ **Parent:** [Elliptic function](#elliptic-function)

For any finite value $a$, apply the argument principle to $f-a$ around a fundamental parallelogram whose boundary avoids zeros and poles. Periodicity cancels the opposite-edge integrals, so the number of solutions of $f(z)=a$ equals the fixed number of poles of $f$, counting multiplicities.

### Weierstrass functions

↑ **Parent:** [Elliptic function](#elliptic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_functions)

Associated with a [period lattice](#period-lattice) are the Weierstrass sigma, zeta, eta and elliptic functions. They satisfy $\zeta=\sigma'/\sigma$ and $\wp=-\zeta'$; the eta constants record quasi-period increments of the [Weierstrass zeta function](#weierstrass-zeta-function).

#### Weierstrass elliptic function

↑ **Parent:** [Weierstrass functions](#weierstrass-functions)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_elliptic_function)

For a [period lattice](#period-lattice) $\Lambda\subset\mathbb C$, the Weierstrass elliptic function is the normally convergent lattice sum

$$
\wp_\Lambda(z)=\frac1{z^2}+\sum_{\omega\in\Lambda\setminus\{0\}}\left(\frac1{(z-\omega)^2}-\frac1{\omega^2}\right).
$$

It is an even [elliptic function](#elliptic-function) with a double [pole](isolated-singularity.md#pole) of principal part $(z-\omega)^{-2}$ and zero [residue](analysis.md#residue) at every point $\omega$ of the [period lattice](#period-lattice).

##### Weierstrass addition formula

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

For generic fixed $w$, regard the right side as an [elliptic function](#elliptic-function) of $z$. The apparent [pole](isolated-singularity.md#pole) at zero cancels, giving limiting value $\wp(w)$. At $z=w$ the slope ratio is finite. At $z=-w$, its squared slope has the same double principal part as $\wp(z+w)$ and no [simple pole](isolated-singularity.md#simple-pole) term. These exhaust the possible [poles](isolated-singularity.md#pole) because the [Weierstrass elliptic function](#weierstrass-elliptic-function) has degree two. The difference is therefore an entire [elliptic function](#elliptic-function), hence constant by [Liouville theorem](#liouville-theorem), and its value at zero is zero. [Meromorphic](isolated-singularity.md#meromorphic-function) continuation extends the identity to the exceptional parameters.

##### Weierstrass sigma function

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

For a [period lattice](#period-lattice), the displayed canonical product converges normally because its logarithmic tails are bounded by a constant times $|\omega|^{-3}$. It defines an odd entire function with simple zeros exactly at the lattice and derivative one at zero. Its logarithmic derivative is the [Weierstrass zeta function](#weierstrass-zeta-function), and the derivative of that logarithmic derivative is minus the [Weierstrass elliptic function](#weierstrass-elliptic-function). Sigma is quasi-periodic rather than elliptic; balanced products of its translates construct meromorphic functions with prescribed [divisors](number-theory.md#divisor) on a complex torus.

###### Legendre relation for Weierstrass quasi-periods

↑ **Parent:** [Weierstrass sigma function](#weierstrass-sigma-function)

For an oriented lattice basis with $\operatorname{Im}(\omega_2/\omega_1)>0$, write $\eta_j=\zeta(z+\omega_j)-\zeta(z)$. These differences are constant because $\zeta'=-\wp$ is periodic. Integrating zeta around a fundamental cell gives the displayed relation by its one simple pole of residue one. Oddness and the logarithmic derivative then give $\sigma(z+\omega_j)=-e^{\eta_j(z+\omega_j/2)}\sigma(z)$. This fixes both the sign and the exponent convention in sigma-product constructions.

##### Four totally ramified Weierstrass values

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The [Weierstrass elliptic function](#weierstrass-elliptic-function) has degree two on its period torus. Its three distinct half-period values $e_j$ have double local preimages, and its [pole](isolated-singularity.md#pole) is double, so these four values are totally ramified. This also follows from $\wp'^2=4\prod_j(\wp-e_j)$ and the principal part at the [pole](isolated-singularity.md#pole). A [Möbius transformation](group-theory.md#mobius-transformation) with [pole](isolated-singularity.md#pole) away from these values moves all four to finite values without changing local degrees.

##### Termwise derivative proof of Weierstrass periodicity

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The [Normal convergence of the Weierstrass elliptic-function series](#normal-convergence-of-the-weierstrass-elliptic-function-series) allows its [derivative](calculus.md#derivative) to be written as an absolutely locally uniformly convergent sum of inverse cubes. For a [period lattice](#period-lattice) $\Lambda$, this derivative sum is invariant under translation by any lattice vector, by reindexing. Consequently $\wp(z+\omega)-\wp(z)$ is constant; its apparent [poles](isolated-singularity.md#pole) cancel. The [Weierstrass elliptic function](#weierstrass-elliptic-function) is even, so for a primitive lattice generator $\omega$, evaluation at $z=-\omega/2$ makes that constant zero. Applying this to two generators proves that this is a [periodic function](function.md#periodic-function), namely $\wp$. This argument avoids separating the original convergent series into two divergent inverse-square sums.

##### Weierstrass shift-difference identity by pole cancellation

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

For $2a\notin\Lambda$, the apparent double poles at $z=\pm a$ on the left are canceled by its squared zero factor. Subtract the right side: the order-three principal parts at lattice points cancel by the even Laurent expansion of $\wp$, leaving at most a simple pole per period cell. An [elliptic function](#elliptic-function) has total residue zero in a period cell, so that possible pole is removable. The resulting entire periodic function is constant, and its oddness makes the constant zero. This proves the identity without presupposing the elliptic differential equation.

##### Elliptic collinearity determinant

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The determinant of the columns $(1,\wp(z),\wp'(z))$, $(1,\wp(w),\wp'(w))$ and $(1,\wp(-z-w),\wp'(-z-w))$ vanishes identically. Its apparent cubic poles at $z=0,-w$ have order at most two because the coefficient multiplying the cubic-pole entry vanishes linearly. Column coincidences give six zeros, unless $3w$ is a lattice point, when they give four zeros with one multiple zero. In the half-period case, the two apparent zero locations at poles are removable zeros: $\wp'(w)=0$ and the two $1/z$ terms cancel, leaving $O(z)$. Thus the zero count exceeds possible pole order in every case. The [argument principle](#argument-principle) proves the identity, which expresses collinearity of the three points on the [Weierstrass equation of an elliptic curve](normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve).

###### Confluent elliptic collinearity determinant

↑ **Parent:** [Elliptic collinearity determinant](#elliptic-collinearity-determinant)

For distinct finite point classes on a complex [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), ordinary column determinants test whether a line meets the curve at those three points. Repeated columns instead vanish for a purely linear-algebraic reason. To prescribe a tangent intersection at $u$, replace the second equal column by its derivative; to prescribe a triple intersection, use $c(u),c'(u),c''(u)$. These confluent determinants vanish exactly when the corresponding degree-three intersection divisor has point sum zero, away from the affine chart's pole. A local homogeneous lift supplies the version at the origin.

##### Elliptic function-field decomposition

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

Every [elliptic function](#elliptic-function) has a unique expression $A(\wp)+B(\wp)\wp^{\prime}$ with [rational functions](isolated-singularity.md#rational-function) $A,B$. Its even part is rational in the [Weierstrass elliptic function](#weierstrass-elliptic-function); its odd part divided by $\wp^{\prime}$ is even and meromorphic, so is also rational in $\wp$. The local even Laurent series at a half-period and at the pole justify meromorphic descent through the double cover of the [Riemann sphere](#riemann-sphere).

##### Even elliptic functions are rational in the Weierstrass function

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The [Weierstrass elliptic function](#weierstrass-elliptic-function) is the quotient map from the complex torus by $z\mapsto-z$. An even [elliptic function](#elliptic-function) descends through this map; its even Laurent series at each branch point makes the descended function meromorphic there. A [meromorphic function](isolated-singularity.md#meromorphic-function) on the [Riemann sphere](#riemann-sphere) is rational, so $f=Q(\wp)$.

###### Degree-two even elliptic function

↑ **Parent:** [Even elliptic functions are rational in the Weierstrass function](#even-elliptic-functions-are-rational-in-the-weierstrass-function)

An even [elliptic function](#elliptic-function) descends through the degree-two quotient map $\wp$ to a [rational function](isolated-singularity.md#rational-function) $R$ on the [Riemann sphere](#riemann-sphere). If the original function also has degree two, composition of map degrees gives $2=2\deg R$, so $R$ has degree one. Consequently it is a [Möbius transformation](group-theory.md#mobius-transformation) with $ad-bc\ne0$. The shift $\operatorname{sn}(z+K,k)$ is even and has degree two, providing an example for the common [period lattice](#period-lattice) of the [Jacobi elliptic sine](#jacobi-elliptic-sine) and $\wp$.

##### Normal convergence of the Weierstrass elliptic-function series

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

On every compact set disjoint from the lattice, the summand

$$
\frac1{(z-\omega)^2}-\frac1{\omega^2}
$$

is bounded by $C|\omega|^{-3}$ for all sufficiently large $|\omega|$. Since the lattice sum of $|\omega|^{-3}$ converges, the defining series for $\wp$ converges normally.

##### Half-period values of the Weierstrass elliptic function

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

At the three nonzero two-torsion points $z_i$ of $\mathbb C/\Lambda$, put $e_i=\wp(z_i)$. The values are distinct because $\wp(z)=\wp(w)$ exactly when $z\equiv\pm w\pmod\Lambda$.

###### Weierstrass half-period translation formula

↑ **Parent:** [Half-period values of the Weierstrass elliptic function](#half-period-values-of-the-weierstrass-elliptic-function)

Let $h_i$ represent a nonzero [two-torsion point of a complex torus](#two-torsion-point-of-a-complex-torus), and write $e_i=\wp(h_i)$. The product $(\wp(z+h_i)-e_i)(\wp(z)-e_i)$ is an [elliptic function](#elliptic-function) whose apparent [poles](isolated-singularity.md#pole) cancel against double [zeros](polynomial.md#zero-of-a-function). It is therefore constant by [Liouville theorem](#liouville-theorem). Its value at $z=0$ is $\wp''(h_i)/2$. The [Weierstrass elliptic differential equation](#weierstrass-elliptic-differential-equation) gives $\wp''(h_i)/2=3e_i^2-g_2/4=(e_i-e_j)(e_i-e_l)$, proving the formula.

###### Weierstrass quarter-period derivative identity

↑ **Parent:** [Weierstrass half-period translation formula](#weierstrass-half-period-translation-formula)

At $z=h_i/2$, evenness and periodicity give $\wp(z+h_i)=\wp(z)$. The [Weierstrass half-period translation formula](#weierstrass-half-period-translation-formula) therefore identifies $(\wp(h_i/2)-e_i)^2$ with $(e_i-e_j)(e_i-e_l)$. Differentiating the [Weierstrass half-period translation formula](#weierstrass-half-period-translation-formula) proves the identity, interpreted as equality of [meromorphic functions](isolated-singularity.md#meromorphic-function), including the apparent singularities of its quotients.

###### Two-torsion point of a complex torus

↑ **Parent:** [Half-period values of the Weierstrass elliptic function](#half-period-values-of-the-weierstrass-elliptic-function)

A two-torsion point satisfies $2z\in\Lambda$. The three nonzero classes are represented by half-periods $\lambda/2$, $\mu/2$, and $(\lambda+\mu)/2$.

##### Equianharmonic lattice

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equianharmonic_lattice)

The equianharmonic triangular lattice is preserved by multiplication by the cube root of unity $\omega=e^{2\pi i/3}$. On its three nonzero two-torsion classes, multiplication by $\omega$ acts as a three-cycle.

##### Weierstrass zeta function

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The Weierstrass zeta function satisfies $\zeta'=-\wp$ and is quasi-periodic: for every period $\omega$, the difference $\zeta(z+\omega)-\zeta(z)$ is constant. It has a simple pole of residue one at each lattice point. Consequently, if $\sum_jc_j=0$, then

$$
\sum_jc_j\zeta(z-a_j)
$$

is an elliptic function.

It is the quasi-periodic zeta member of the [Weierstrass functions](#weierstrass-functions).

##### Laurent coefficients of the Weierstrass elliptic function

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

Writing $G_{2r}=\sum_{\omega\ne0}\omega^{-2r}$ for the lattice Eisenstein sums, expansion about zero gives

$$
\wp(z)=\frac1{z^2}
+\sum_{r=2}^{\infty}(2r-1)G_{2r}z^{2r-2}.
$$

Thus the constant coefficient vanishes and, for $k\geq1$, the coefficient of $z^{2k}$ is $(2k+1)G_{2k+2}$.

###### Positive polynomial recurrence for lattice Eisenstein sums

↑ **Parent:** [Laurent coefficients of the Weierstrass elliptic function](#laurent-coefficients-of-the-weierstrass-elliptic-function)

Write the [Weierstrass elliptic function](#weierstrass-elliptic-function) as $\wp(z)=z^{-2}+\sum_{n\geq1}c_nz^{2n}$, with $c_1=3G_4$, $c_2=5G_6$ and $c_n=(2n+1)G_{2n+2}$. Differentiate the [Weierstrass elliptic differential equation](#weierstrass-elliptic-differential-equation) to obtain $\wp''=6\wp^2-g_2/2$. Comparing coefficients of $z^{2n-2}$ gives the displayed recurrence for $n\geq3$. Every denominator is positive, so induction expresses every higher [lattice Eisenstein series](modular-function.md#lattice-eisenstein-sum) as a polynomial in $G_4,G_6$ with positive rational coefficients on its occurring monomials. In particular $G_8=3G_4^2/7$ and $G_{10}=5G_4G_6/11$.

##### Weierstrass elliptic differential equation

↑ **Parent:** [Weierstrass elliptic function](#weierstrass-elliptic-function)

The [Weierstrass elliptic function](#weierstrass-elliptic-function) satisfies

$$
\wp'(z)^2=4\wp(z)^3-g_2\wp(z)-g_3.
$$

Writing $G_{2r}=\sum_{\omega\in\Lambda\setminus\{0\}}\omega^{-2r}$, the [Laurent coefficients of the Weierstrass elliptic function](#laurent-coefficients-of-the-weierstrass-elliptic-function) give

$$
\wp(z)=z^{-2}+3G_4z^2+5G_6z^4+O(z^6),
\qquad
\wp'(z)=-2z^{-3}+6G_4z+20G_6z^3+O(z^5).
$$

Thus $g_2=60G_4$ and $g_3=140G_6$ cancel every nonremovable term in the [Laurent series](analysis.md#laurent-series) of $\wp'^2-4\wp^3+g_2\wp+g_3$ at each point of the [period lattice](#period-lattice). The resulting [elliptic function](#elliptic-function) is an [entire function](#entire-function) and is bounded, hence is zero by [Liouville theorem](#liouville-theorem).

###### Nonvanishing discriminant of a complex lattice

↑ **Parent:** [Weierstrass elliptic differential equation](#weierstrass-elliptic-differential-equation)

The three nonzero half-period classes make the odd derivative of the [Weierstrass elliptic function](#weierstrass-elliptic-function) vanish. Their values are distinct: two equal values would force at least four zeros for a function with only one double pole. Thus they are three distinct roots of $4X^3-g_2X-g_3$, whose monic discriminant gives the displayed factor. This lattice discriminant differs by $(2\pi)^{12}$ from the normalized [modular discriminant](modular-function.md#modular-discriminant) for the lattice $\mathbb Z+\mathbb Z\tau$.

<h2 id="runge-s-theorem">Runge's theorem</h2>

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Runge's_theorem)

A holomorphic function near a compact set can be uniformly approximated by rational functions with poles in prescribed complementary components; connected complement permits polynomials.

### Uniform rational approximation algebra with prescribed poles

↑ **Parent:** [Runge's theorem](#runge-s-theorem)

Let $K\subset\mathbb C$ be compact and permit polynomial terms and finite poles in $S\subset\mathbb C\setminus K$, meeting every bounded complementary component. In the uniform closure $A$ of these rational functions, the coordinate $u(z)=z$ has spectrum exactly $K$. Indeed the set of $\lambda\notin K$ with $(u-\lambda)^{-1}\in A$ is relatively open by invertibility and relatively closed by uniform continuity of the scalar resolvent; it meets each component by a prescribed pole, or by a Neumann expansion at infinity. It is therefore all of $\mathbb C\setminus K$. [Holomorphic functional calculus](banach-algebra.md#holomorphic-functional-calculus) then places every function holomorphic near $K$ in $A$, proving prescribed-pole [Runge approximation theorem](#runge-s-theorem).

### Polynomial Runge theorem

↑ **Parent:** [Runge's theorem](#runge-s-theorem)

If $K\subset\mathbb C$ is compact with connected complement and $f$ is holomorphic near $K$, then for each $\varepsilon>0$ there is a polynomial $p$ such that $\sup_K|p-f|<\varepsilon$.

#### Runge exhaustion of a slit disk

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

For the unit disk with the nonpositive real radius removed, compact sets $K_m=\{re^{i\theta}:1/m\leq r\leq1-1/m,\ |\theta|\leq\pi-1/m\}$, $m\geq3$, exhaust the domain. Each has connected complement: its inner and outer complementary regions join through the missing angular sector. The [polynomial Runge theorem](#polynomial-runge-theorem) gives a [polynomial](polynomial.md) within $1/m$ of a given [holomorphic function](#holomorphic-function) on $K_m$. Every compact subset lies in some $K_m$, so these polynomials converge uniformly on compact subsets.

#### Pointwise polynomial approximation of a half-plane sign

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

There is a sequence of complex [polynomials](polynomial.md) converging pointwise on the whole plane to the sign of the imaginary part, with value zero on the real axis. For each $n$, take the [compact](topology.md#compact-space) union of the upper rectangle $[-n,n]+i[1/n,n]$, its lower reflection and the real segment $[-n,n]$. Its complement is [connected](geometry-and-topology.md#connected-space). The function equal to one, minus one and zero on disjoint [neighborhoods](topology.md#neighbourhood-mathematics) of the three components is [holomorphic](#complex-differentiability-at-a-point). The [polynomial Runge theorem](#polynomial-runge-theorem) provides a [polynomial](polynomial.md) within $1/n$ of it on the union. Every fixed point lies in its corresponding component for all large $n$, proving [pointwise convergence](real-analysis.md#pointwise-convergence). The limit is discontinuous, so the convergence cannot be locally uniform near the real axis. This illustrates how pointwise approximation by [holomorphic functions](#holomorphic-function) differs from locally uniform approximation.

#### Pole-moving polynomial approximation

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

Let the uniform closure of polynomials on a compact set be an algebra. A reciprocal at a sufficiently distant pole belongs to it by a geometric series. A path of poles avoiding the compact set can be divided into short steps; expanding each reciprocal in powers of the previous one transfers polynomial approximability along the path.

#### Polynomially approximable resolvent point

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

For a closed set $K\subsetneq\mathbb C$, a point $\lambda\notin K$ is a polynomially approximable resolvent point when $z\mapsto(z-\lambda)^{-1}$ is a [uniform limit](real-analysis.md#uniform-limit) on $K$ of complex polynomials.

##### Resolvent propagation across a complementary component

↑ **Parent:** [Polynomially approximable resolvent point](#polynomially-approximable-resolvent-point)

The polynomially approximable resolvent points form a subset that is both open and closed relative to $\mathbb C\setminus K$. Openness follows from the uniformly convergent expansion

$$
\frac1{z-\mu}
=\sum_{n=0}^{\infty}\frac{(\mu-\lambda)^n}{(z-\lambda)^{n+1}}
$$

when $|\mu-\lambda|<\operatorname{dist}(\lambda,K)$; relative closedness follows from the uniform continuity of the resolvent as its pole varies away from $K$. Hence approximability at one point propagates throughout its connected component of $\mathbb C\setminus K$.

#### Elementary polynomial approximation on a square

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

Let $S$ be a closed square and let $f$ be holomorphic on a neighbourhood of a slightly larger square. The [Cauchy integral formula](analysis.md#cauchy-integral-formula) on the larger boundary is uniformly approximated on $S$ by Riemann sums of resolvents whose poles lie outside $S$. Far-away resolvents have convergent geometric-series expansions in $z$, and [resolvent propagation across a complementary component](#resolvent-propagation-across-a-complementary-component) moves this polynomial approximability to every pole outside the square. Approximating the finitely many resolvents in each Riemann sum by polynomials proves polynomial approximation on $S$ without invoking the general [Runge theorem](#runge-s-theorem).

#### Polynomial approximation of the reciprocal on a proper circular arc

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

A proper closed arc $S$ of a circle centered at zero has connected complement and stays away from zero. The polynomial Runge theorem therefore gives polynomials converging uniformly to $1/z$ on $S$.

##### Explicit polynomial approximation of the reciprocal on the left semicircle

↑ **Parent:** [Polynomial approximation of the reciprocal on a proper circular arc](#polynomial-approximation-of-the-reciprocal-on-a-proper-circular-arc)

On $K=\{z:|z|=1,\operatorname{Re}z\leq0\}$, the polynomials

$$
p_n(z)=-\frac14\sum_{j=0}^n\sum_{k=0}^{n^2}\binom{j+k}{k}\left(\frac z4\right)^k
$$

converge uniformly to $1/z$. Expand $1/z$ first in powers of $4/(z-4)$, whose modulus is at most $4/\sqrt{17}$ on $K$, and then expand each $(z-4)^{-j-1}$ in powers of $z/4$. The estimate $\binom{j+k}{k}\leq2^{j+k}$ controls the diagonal truncation.

#### Polynomial approximation obstruction on a punctured circle

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

Polynomials cannot converge uniformly to $1/z$ on $\{z:|z|=1,z\ne1\}$. Uniform convergence there makes the polynomials uniformly Cauchy on the full circle because deleting one point does not change the supremum of a continuous function. They would therefore converge uniformly to $1/z$ on the full circle, contradicting

$$
\oint p(z)\,dz=0,
\qquad
\oint\frac{dz}{z}=2\pi i.
$$

#### Pointwise approximation by a Runge exhaustion

↑ **Parent:** [Polynomial Runge theorem](#polynomial-runge-theorem)

To approximate a piecewise constant function pointwise, exhaust each of its separated regions by compact subsets whose finite union has connected complement. Apply polynomial Runge approximation to the locally constant holomorphic function on each stage, with errors tending to zero. Every fixed point eventually lies in all later stages, so the uniform stagewise estimates imply pointwise convergence.

## Winding number

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Winding_number)

For a closed piecewise smooth curve $\gamma$ avoiding $w$,

$$
\operatorname{wind}(\gamma,w)
=\frac1{2\pi i}\int_\gamma\frac{dz}{z-w}.
$$

It is the net change of a continuous argument divided by $2\pi$ and is an integer.

### Winding number of a continuous closed path

↑ **Parent:** [Winding number](#winding-number)

If $\gamma:[0,1]\to\mathbb C\setminus\{0\}$ is [continuous](calculus.md#continuous-function) and closed, choose a continuous lift $\theta$ such that

$$
\frac{\gamma(t)}{|\gamma(t)|}=e^{2\pi i\theta(t)}.
$$

Then $\operatorname{wind}(\gamma,0)=\theta(1)-\theta(0)\in\mathbb Z$. This agrees with the contour-integral definition when the path is piecewise smooth.

#### Continuous logarithm lifting criterion

↑ **Parent:** [Winding number of a continuous closed path](#winding-number-of-a-continuous-closed-path)

On a locally [path-connected](geometry-and-topology.md#path-connected-space) space, on each path component choose a value of a [complex logarithm](analysis.md#complex-logarithm) of $f$ at a base point. Continue it along paths using local logarithms. Independence of the path is exactly vanishing of the [winding number of a continuous closed path](#winding-number-of-a-continuous-closed-path) for all loops. This constructs a [continuous function](calculus.md#continuous-function) $g$ with $f=e^g$. The implication from a logarithm to zero winding requires no local connectivity. For applications to arbitrary planar [compact](topology.md#compact-space) sets, apply the criterion on polygonal neighborhoods rather than assuming the [compact](topology.md#compact-space) set is locally [path-connected](geometry-and-topology.md#path-connected-space).

## Homotopy invariance of winding number

↑ **Parent:** [Complex analysis](complex-analysis.md)

A homotopy through closed paths avoiding the base point cannot change the integer winding number.

### Dominated perturbation preserves winding number

↑ **Parent:** [Homotopy invariance of winding number](#homotopy-invariance-of-winding-number)

If closed continuous paths $\gamma,\phi$ satisfy $|\gamma(t)|>|\phi(t)|$ for every $t$, then $H(s,t)=\gamma(t)+s\phi(t)$ never vanishes. It is therefore a homotopy through closed paths in $\mathbb C\setminus\{0\}$, and

$$
\operatorname{wind}(\gamma+\phi,0)=\operatorname{wind}(\gamma,0).
$$

### Winding-number proof of the fundamental theorem of algebra

↑ **Parent:** [Homotopy invariance of winding number](#homotopy-invariance-of-winding-number)

For a polynomial $P(z)=a_nz^n+\cdots+a_0$ of positive degree, on a sufficiently large circle its leading term dominates the remaining terms. The [dominated-perturbation lemma](#dominated-perturbation-preserves-winding-number) therefore gives winding number $n$ to the loop $P(Re^{2\pi it})$. If $P$ had no zero, radial contraction of the input circle would map under $P$ to a homotopy with a constant loop in $\mathbb C\setminus\{0\}$, which has winding number zero. This contradiction proves the [Fundamental theorem of algebra](algebra.md#fundamental-theorem-of-algebra).

### Winding-number proof of the no-retraction theorem

↑ **Parent:** [Homotopy invariance of winding number](#homotopy-invariance-of-winding-number)

If a continuous retraction from a closed disc to its boundary existed, applying it to a contraction of the boundary circle inside the disc would give a homotopy in $\mathbb C\setminus\{0\}$ from a loop of winding number one to a constant loop of winding number zero. [Homotopy invariance of winding number](#homotopy-invariance-of-winding-number) rules this out.

## Bromwich contour

↑ **Parent:** [Complex analysis](complex-analysis.md)

A Bromwich contour is a vertical line in the complex frequency plane lying to the right of the singularities in the inverse Laplace integral.

### Bromwich inversion with a square-root branch cut

↑ **Parent:** [Bromwich contour](#bromwich-contour)

When an inverse Laplace integrand contains $p^{-1/2}$ on the principal branch, closing the Bromwich contour to the left encloses isolated poles and wraps a branch cut along the negative real axis. Pole residues give persistent oscillatory terms, while the jump across the two sides of the cut gives a real decaying integral.

## Branch point

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Branch_point)

A branch point is a point around which analytic continuation of a multivalued function returns a different value.

### Algebraic branch point

↑ **Parent:** [Branch point](#branch-point)

At an algebraic [branch point](#branch-point), a local solution becomes [meromorphic](isolated-singularity.md#meromorphic-function) after the finite substitution $z-a=t^k$. The displayed convergent expansion has only finitely many negative terms. A square-root [branch point](#branch-point) corresponds to $k=2$; an [essential singularity](isolated-singularity.md#essential-singularity) or [logarithmic singularity](analysis.md#logarithmic-singularity) need not become meromorphic under any such finite substitution.

### Branch of a multivalued function

↑ **Parent:** [Branch point](#branch-point)

A branch of a multivalued analytic expression is a single-valued holomorphic choice on a domain obtained by excluding suitable branch cuts.

### Monodromy reflection at a square-root branch point

↑ **Parent:** [Branch point](#branch-point)

Let

$$
W(z)=\int_{z_0}^z\frac{q(t)}{\sqrt{P(t)}}\,dt,
$$

where $P$ has a simple zero at $a$, and let $A$ be the limiting value of $W$ at $a$ on one sheet. [Analytic continuation](#analytic-continuation) once around $a$ changes the sign of the square root and hence of $W'$. The continued primitive agrees at $a$ with the original one, so it is

$$
W\longmapsto 2A-W.
$$

#### Translation generated by two square-root monodromy reflections

↑ **Parent:** [Monodromy reflection at a square-root branch point](#monodromy-reflection-at-a-square-root-branch-point)

If continuation around two square-root branch points acts on a primitive as $R_A(W)=2A-W$ and $R_B(W)=2B-W$, then

$$
R_B\circ R_A(W)=W+2(B-A).
$$

Thus pairs of branch-point loops generate additive periods of an inverse function.

## Complex number

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_number)

A complex number has the form $x+iy$, with conjugate $x-iy$ and [modulus](#modulus) $\sqrt{x^2+y^2}$.

### Polar form of a complex number

↑ **Parent:** [Complex number](#complex-number)

A nonzero [complex number](#complex-number) has the form $z=re^{i\theta}$ with $r=|z|>0$ and an argument determined modulo $2\pi$. Multiplication multiplies moduli and adds arguments. This makes powers and [roots of a complex number](#root-of-a-complex-number) particularly transparent.

#### Root of a complex number

↑ **Parent:** [Polar form of a complex number](#polar-form-of-a-complex-number)

For $z=re^{i\theta}\ne0$ and a positive integer $n$, all solutions of $w^n=z$ are $r^{1/n}e^{i(\theta+2\pi k)/n}$ for $k=0,\ldots,n-1$. They differ by multiplication by [roots of unity](algebra.md#root-of-unity) and are distinct. If $z=0$, the sole root is zero.

### Complex modulus

↑ **Parent:** [Complex number](#complex-number)

The [complex modulus](#complex-modulus) of $z=x+iy$ is $|z|=\sqrt{x^2+y^2}=\sqrt{z\overline z}$. It is the [Euclidean norm](functional-analysis.md#euclidean-norm) of $(x,y)$ in the [complex plane](#complex-plane), and satisfies $|zw|=|z||w|$ and the [triangle inequality](topological-analysis.md#triangle-inequality).

### Imaginary unit

↑ **Parent:** [Complex number](#complex-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Imaginary_unit)

The imaginary unit is the complex number $i$ satisfying $i^2=-1$. Its integer powers repeat with period four.

### Real part

↑ **Parent:** [Complex number](#complex-number)

For a [complex number](#complex-number) $z=x+iy$, its real part is $\operatorname{Re}z=x$.

### Imaginary part

↑ **Parent:** [Complex number](#complex-number)

For a [complex number](#complex-number) $z=x+iy$, its imaginary part is $\operatorname{Im}z=y$.

<h3 id="euler-s-formula">Euler's formula</h3>

↑ **Parent:** [Complex number](#complex-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_formula)

Euler's formula states that $e^{i\theta}=\cos\theta+i\sin\theta$.

### Modulus

↑ **Parent:** [Complex number](#complex-number)

The modulus of a [complex number](#complex-number) $z=x+iy$ is $|z|=\sqrt{x^2+y^2}$.

For $z=x+iy$, its modulus is $|z|=\sqrt{x^2+y^2}$, the complex case of [absolute value](real-analysis.md#absolute-value).

### Complex conjugate

↑ **Parent:** [Complex number](#complex-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_conjugate)

The complex conjugate of $z=x+iy$ is $\overline z=x-iy$. It satisfies $z\overline z=|z|^2$.

#### Complex conjugation

↑ **Parent:** [Complex conjugate](#complex-conjugate)

Complex conjugation sends a [complex number](#complex-number) $z=a+ib$ to its [complex conjugate](#complex-conjugate) $\overline z=a-ib$. It is an involution and a [field automorphism](galois-theory.md#field-automorphism) of $\mathbb C$, with fixed field $\mathbb R$. Applied componentwise to a complex vector, it produces the conjugated vector appearing in a [Choi state](quantum-information-theory.md#choi-state) for a rank-one [Kraus operator](quantum-information-theory.md#kraus-operator).

##### Schwarz conjugation of a spectral function

↑ **Parent:** [Complex conjugation](#complex-conjugation)

This operation reflects a [holomorphic function](#holomorphic-function) across the real axis while preserving holomorphic dependence on the new argument. A transform of real data with real kernel coefficients satisfies $F^\sharp=F$. In a polygonal [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem), complex rotation factors are conjugated as well; an explicit prefactor $i$ changes sign.

### Argument (complex analysis)

↑ **Parent:** [Complex number](#complex-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Argument_(complex_analysis))

An argument of a nonzero [complex number](#complex-number) $z$ is any angle $\theta$ for which $z=|z|e^{i\theta}$. Arguments differ by integer multiples of $2\pi$; choosing one representative defines a branch of the argument.

### Complex plane

↑ **Parent:** [Complex number](#complex-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_plane)

The complex plane identifies the [complex number](#complex-number) $x+iy$ with the point $(x,y)$ in the real plane.

#### Finite-hole neighborhoods of a planar compact set

↑ **Parent:** [Complex plane](#complex-plane)

Given a [compact](topology.md#compact-space) planar set $K$ and an [open](topology.md#open-set) neighborhood $V$, a finite square-grid construction gives a [compact](topology.md#compact-space) polygonal neighborhood inside $V$ with finitely many complementary components. Remove thin polygonal corridors disjoint from $K$ joining holes that lie in the same component of $\mathbb C\setminus K$, and joining holes in its unbounded component to the exterior. Corridors can also include a prescribed point from each of finitely many specified bounded components. There remains a neighborhood whose bounded holes lie in distinct bounded components of $\mathbb C\setminus K$, each containing its chosen point. Standard small polygonal rounding gives a finite union of planar surfaces with [boundary](topology.md#boundary-of-a-set). The index map from its first integral [homology group](homology.md#homology-group) to one integer per bounded hole is an isomorphism. Triangulate a surrounding disc: a one-cycle bounds a two-chain whose coefficients are constant in each complementary component. Zero hole coefficients give a filling supported inside the neighborhood; the face chain of each hole supplies a dual cycle. The cycles can be sums of boundary curves in different components. This uses finite triangulation, not the general [Jordan curve theorem](topology.md#jordan-curve-theorem).

#### Complex coordinate

↑ **Parent:** [Complex plane](#complex-plane)

Represent Cartesian coordinates $(x,y)$ in the plane by the [complex number](#complex-number) $z=x+iy$, whose [real part](#real-part) and [imaginary part](#imaginary-part) recover them. Multiplication by $e^{i\theta}$ rotates the coordinates through angle $\theta$, so a rotating-frame calculation becomes a complex exponential change of variable.

#### Real linear equation of a line in the complex plane

↑ **Parent:** [Complex plane](#complex-plane)

For $c\ne0$ and real $r$, this equation defines a [straight line](geometry-and-topology.md#straight-line). Writing $z=x+iy$ and $c=u+iv$ gives $2ux+2vy+r=0$, so $c$ supplies a normal direction. Conversely every real affine line $Ax+By+C=0$ has this representation with $c=(A+iB)/2$ and $r=C$. The condition $c\ne0$ excludes an empty set or the entire [complex plane](#complex-plane).

#### Imaginary axis

↑ **Parent:** [Complex plane](#complex-plane)

The imaginary axis is the set of [complex numbers](#complex-number) $iy$ with $y\in\mathbb R$. It is the vertical coordinate axis in the [complex plane](#complex-plane).

#### Complex unit circle

↑ **Parent:** [Complex plane](#complex-plane)

The complex unit circle is the subgroup $\{z\in\mathbb C:|z|=1\}$ under multiplication.

## Isolated singularity

↑ **Parent:** [Complex analysis](complex-analysis.md)

[This section is present in another page, follow this link to view it.](isolated-singularity.md)

## Contour integration

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Contour_integration)

Contour integration integrates complex functions along oriented curves and evaluates many real integrals through residues.

### Cauchy transform

↑ **Parent:** [Contour integration](#contour-integration)

This [contour integral](#contour-integral) defines an analytic function away from the oriented integration curve, under the relevant integrability assumptions. Its limiting values across the curve are related by the [Sokhotski–Plemelj theorem](#sokhotski-plemelj-theorem). On an oriented real axis, with $Hf(\rho)=\pi^{-1}\operatorname{PV}\int f(s)/(\rho-s)\,ds$, the [signed Cauchy boundary operators](#signed-cauchy-boundary-operators) are $C^\pm f=\pm f/2+iHf/2$.

#### Paired radial jump of a continuous Cauchy transform

↑ **Parent:** [Cauchy transform](#cauchy-transform)

For continuous boundary data on the counterclockwise unit circle and its [Cauchy transform](#cauchy-transform) $\Phi$, $\Phi(r\omega)-\Phi(r^{-1}\omega)=P\phi(r\omega)$ for $0<r<1$. This follows by subtracting the two Cauchy kernels and obtaining the [Poisson kernel on the circle](partial-differential-equation.md#poisson-kernel-on-the-circle). Consequently the paired interior-minus-exterior difference tends to $\phi(\omega)$ as $r\uparrow1$. For $r\downarrow1$ from above, the same written difference has the opposite sign. This paired limit does not require each individual boundary value of the transform to exist.

// Destination: analysis.bigb

### Pochhammer contour

↑ **Parent:** [Contour integration](#contour-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pochhammer_contour)

A commutator contour around two branch points cancels the total [monodromy](#monodromy) of its integrand. For the contour circling $1,0$ clockwise and then $1,0$ anticlockwise, with initial positive-real branches, the [Beta function](#beta-function) obeys

$$
\int_Pt^{z-1}(1-t)^{b-1}\,dt=(1-e^{-2\pi iz})(1-e^{-2\pi ib})B(z,b).
$$

The contour integral is [entire](#entire-function) in $z$, giving a [meromorphic continuation](#meromorphic-continuation) of the [Beta function](#beta-function).

### Complex integration contour

↑ **Parent:** [Contour integration](#contour-integration)

A complex integration [contour](#complex-integration-contour) is an oriented piecewise continuously differentiable [curve](topology.md#curve) in the [complex plane](#complex-plane). For a parametrization $\gamma(s)$, its [contour integral](#contour-integral) is $\int_\Gamma f(z)\,dz=\int f(\gamma(s))\gamma'(s)\,ds$. Reversing orientation changes the sign. Unbounded [contours](#complex-integration-contour) require a convergent improper or explicitly regularized limit.

### Complex contour

↑ **Parent:** [Contour integration](#contour-integration)

An oriented piecewise differentiable path in the complex plane, used as the domain of a [contour integral](#contour-integral). Its orientation controls the signs of residues in the [residue theorem](analysis.md#residue-theorem).

### Contour rotation

↑ **Parent:** [Contour integration](#contour-integration)

An integration ray can be rotated through an analytic sector when endpoint and connecting-arc contributions vanish. Complex powers gain a phase from the rotated differential and power. This relates conditionally convergent oscillatory gamma integrals to decaying Laplace integrals.

### Keyhole contour

↑ **Parent:** [Contour integration](#contour-integration)

A contour encircling a branch cut travels on its two sides and joins them by small and large circles. It converts the phase change of a complex power into a real integral through the [residue theorem](analysis.md#residue-theorem). The two circular contributions must be bounded before taking their limiting radii.

### Contour integral

↑ **Parent:** [Contour integration](#contour-integration)

For a piecewise [differentiable](analysis.md#differentiable-function) parametrized contour $z(t)$, the contour integral is $\int f(z(t))z'(t)\,dt$. It depends on the orientation of the contour. For a [holomorphic function](#holomorphic-function), the [Cauchy integral theorem](#cauchy-s-integral-theorem) allows a [contour deformation](#contour-deformation) through regions without singularities.

### Estimation lemma

↑ **Parent:** [Contour integration](#contour-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Estimation_lemma)

If $|f(z)|\leq M$ along a contour of length $L$, then

$$
\left|\int_C f(z)\,dz\right|\leq ML.
$$

### Uniform convergence and contour integration

↑ **Parent:** [Contour integration](#contour-integration)

If continuous functions $f_n$ converge uniformly to $f$ on the image of a rectifiable curve $\gamma$, then

$$
\int_\gamma f_n(z)\,dz\longrightarrow\int_\gamma f(z)\,dz.
$$

Indeed, the absolute difference is at most the length of $\gamma$ times $\sup_\gamma|f_n-f|$.

### Contour shifting

↑ **Parent:** [Contour integration](#contour-integration)

Contour shifting deforms a complex integration path through a region where the integrand is [meromorphic](isolated-singularity.md#meromorphic-function). The [residue theorem](analysis.md#residue-theorem) says that the change equals $2\pi i$ times the sum of residues of the poles crossed.

### Period obstruction to a holomorphic antiderivative

↑ **Parent:** [Contour integration](#contour-integration)

A holomorphic function has an antiderivative on a domain only if its integral around every closed curve vanishes. Thus a single nonzero period, such as $\int_{|z|=1}dz/z=2\pi i$, prevents a global antiderivative.

<h3 id="jordan-s-lemma">Jordan's lemma</h3>

↑ **Parent:** [Contour integration](#contour-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan's_lemma)

Jordan's lemma controls exponential contour integrals on large semicircles and makes their arc contributions vanish.

#### Alternating sine series with a quadratic denominator

↑ **Parent:** [Jordan's lemma](#jordan-s-lemma)

For real $a\ne0$ and $|x|<\pi$, integrate $z\sin(xz)/((a^2+z^2)\sin\pi z)$ around a thin positively oriented strip containing the integers. Its integer [residues](analysis.md#residue) give the series. Closing the two strip sides outward instead gives minus the sum of the residues at $z=\pm ia$, each $\sinh(ax)/(2\sinh(a\pi))$. The factor $|x|<\pi$ ensures exponential decay on those closures. The bilateral series is interpreted by symmetric partial sums; at $a=0$ its continuous extension is $-x$ with the zero-index summand defined to be zero.

### Complex line integral estimate

↑ **Parent:** [Contour integration](#contour-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_line_integral_estimate)

Integrating along a straight segment bounds a complex integral by segment length times the supremum of the integrand.

### Hankel contour

↑ **Parent:** [Contour integration](#contour-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hankel_contour)

A Hankel contour runs along both banks of a branch cut and circles its branch point, converting the jump of a complex power into a sine factor.

#### Hankel analytic continuation

↑ **Parent:** [Hankel contour](#hankel-contour)

Subtracting the local Taylor expansion at the encircled branch point extends a Hankel integral successively across left half-planes; prefactors often remove the introduced poles.

#### Residue extraction by a Hankel contour

↑ **Parent:** [Hankel contour](#hankel-contour)

When the complex power becomes an integer power, a collapsed Hankel contour extracts the coefficient of $t^{-1}$ in the local Laurent series.

##### Cancellation of positive-integer gamma singularities on a Hankel contour

↑ **Parent:** [Residue extraction by a Hankel contour](#residue-extraction-by-a-hankel-contour)

Keep the circular portion of a [Hankel contour](#hankel-contour) at fixed nonzero radius. Its numerator $I(z)=\int_Ht^{z-1}e^t\,dt$ is an [entire function](#entire-function) of $z$, because the contour avoids zero and its tails decay exponentially, uniformly on compact parameter sets. At a positive integer $n$, the integrand is single-valued and entire in $t$, so the bank integrals cancel and the circular integral is zero. Thus $I(n)=0$, canceling the simple zero of $2i\sin(\pi z)$ in the Hankel representation of the [gamma function](#gamma-function). At a nonpositive integer $-n$, the circular integral instead gives $2\pi i/n!$, yielding residue $(-1)^n/n!$.

## Univalent function

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Univalent_function)

A univalent function is a holomorphic injective function.

### Area theorem (conformal mapping)

↑ **Parent:** [Univalent function](#univalent-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Area_theorem_(conformal_mapping))

For a [univalent](#univalent-function) exterior map $G(\zeta)=\zeta+b_0+\sum_{n\ge1}b_n\zeta^{-n}$, the image of $|\zeta|=R>1$ is a positively oriented Jordan curve. [Green's theorem](calculus.md#green-theorem) gives its enclosed area as $\pi(R^2-\sum_{n\ge1}n|b_n|^2R^{-2n})$. Nonnegativity and $R\downarrow1$ give the displayed bound. Laurent-series differentiation and integration on a [circle](topology.md#circle) of radius greater than one are justified by [uniform convergence](real-analysis.md#uniform-convergence) there.

### Normalized univalent function

↑ **Parent:** [Univalent function](#univalent-function)

A [normalized univalent function](#normalized-univalent-function) is a [holomorphic function](#holomorphic-function) on the [unit disc](topology.md#unit-disc) which is [injective](algebra.md#injective-function) and has the displayed normalization. Its [Taylor series](calculus.md#taylor-series) begins $z+a_2z^2+\cdots$. Normalization makes coefficient bounds and image-size estimates independent of translation and dilation; the [Koebe quarter theorem](#koebe-quarter-theorem) is the sharp universal image bound.

#### Second coefficient bound for normalized univalent functions

↑ **Parent:** [Normalized univalent function](#normalized-univalent-function)

The [odd square-root transform of a normalized univalent function](#odd-square-root-transform-of-a-normalized-univalent-function) has reciprocal exterior expansion $1/h(1/\zeta)=\zeta-(a_2/2)\zeta^{-1}+\cdots$. Its first negative Laurent coefficient has modulus at most one by the [area theorem for univalent functions](#area-theorem-conformal-mapping), proving the bound. If $w$ is omitted by $f$, the normalized map $wf/(w-f)$ has second coefficient $a_2+1/w$. Applying the bound twice gives $|1/w|\le4$, the [Koebe quarter theorem](#koebe-quarter-theorem).

#### Odd square-root transform of a normalized univalent function

↑ **Parent:** [Normalized univalent function](#normalized-univalent-function)

Because $f(z)/z$ is holomorphic and nowhere zero on the [unit disc](topology.md#unit-disc), its [square root](algebra.md#square-root) with value one at zero exists. Defining $h(z)=z\sqrt{f(z^2)/z^2}$ gives an odd normalized [univalent function](#univalent-function). If $h(z)=h(w)$, squaring gives $z^2=w^2$; the possibility $z=-w$ and oddness force both to be zero. Applying the [area theorem for univalent functions](#area-theorem-conformal-mapping) to $1/h(1/\zeta)$ yields $|a_2|\le2$.

### A univalent function has nonzero derivative

↑ **Parent:** [Univalent function](#univalent-function)

For an [injective](algebra.md#injective-function) [holomorphic function](#holomorphic-function) $f$ on an [open subset](topology.md#open-set) of $\mathbb C$, $f'(z)$ is nowhere zero. If $f(z)-f(z_0)=(z-z_0)^m h(z)$ with $h(z_0)\ne0$, choose a small [circle](topology.md#circle) where both $h$ and $mh+(z-z_0)h'$ have no zeros. The [argument principle](#argument-principle) counts $m$ zeros of $f(z)-f(z_0)-w$ inside that [circle](topology.md#circle) for sufficiently small $w\ne0$: deforming $w$ to zero cannot change the count. All these zeros are simple, since $f'$ only vanishes at $z_0$ inside the [circle](topology.md#circle) and $z_0$ is not a zero when $w\ne0$. Injectivity forces $m=1$, and hence $f'(z_0)\ne0$.

### Locally uniform limit of univalent functions

↑ **Parent:** [Univalent function](#univalent-function)

A [locally uniform convergence](real-analysis.md#locally-uniform-convergence) limit of [univalent functions](#univalent-function) on a domain is either constant or univalent. For a nonconstant limit $f$, suppose distinct $x,y$ satisfy $f(x)=f(y)$. Choose a small closed disk around $x$ excluding $y$ with $f-f(y)$ nonzero on its boundary. The [Rouche theorem](#rouche-s-theorem) then forces $f_j-f_j(y)$ to have a zero in that disk for large $j$, contradicting injectivity of $f_j$. This supplies the injectivity step in an extremal proof of the [Riemann mapping theorem](#riemann-mapping-theorem) without assuming it as a special lemma.

### Koebe function

↑ **Parent:** [Univalent function](#univalent-function)

The Koebe function $k(z)=z/(1-z)^2$ is a [univalent function](#univalent-function) from the [unit disc](topology.md#unit-disc) onto $\mathbb C\setminus(-\infty,-1/4]$. To see the image, $(1+z)/(1-z)$ maps the disc onto the right half-plane and $k(z)=(((1+z)/(1-z))^2-1)/4$. Its normalization $k(0)=0$, $k'(0)=1$ proves sharpness of the [Koebe quarter theorem](#koebe-quarter-theorem).

### Boundary logarithmic mean of a univalent function

↑ **Parent:** [Univalent function](#univalent-function)

If $\phi$ maps the unit disc conformally to a proper simply connected domain, the nonvanishing holomorphic quotient $F(w)=(\phi(w)-\phi(0))/w$ has harmonic log modulus. Its radial mean equals $\log|\phi'(0)|$. Boundary values are understood as radial limits: the standard integral-mean bound $\sup_{r<1}\int|\phi(re^{i\theta})|^p\,d\theta<\infty$ for $0<p<1/2$, together with the [Koebe distortion theorem](#koebe-distortion-theorem) lower bound $|F(w)|\geq|\phi'(0)|/4$, gives [uniform integrability](convergence-of-random-variables.md#uniform-integrability) of these logarithms. Hence

$$
\log|\phi'(0)|=\frac1{2\pi}\int_0^{2\pi}\log|\phi(e^{i\theta})-\phi(0)|\,d\theta.
$$

## Liouville theorem

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liouville_theorem)

Every bounded entire function is constant.

### Entire function confined to a half-plane is constant

↑ **Parent:** [Liouville theorem](#liouville-theorem)

If an [entire function](#entire-function) $g$ satisfies $\operatorname{Re}(cg)\ge b$ for constants $c\ne0$ and real $b$, then $e^{-cg}$ is entire and has modulus at most $e^{-b}$. The [Liouville theorem](#liouville-theorem) makes it constant, and differentiating gives $g'=0$ since the exponential never vanishes. The conclusion also applies after rotating and translating any containing half-plane; separate bounds on the real and imaginary parts are unnecessary.

### One-sided product bound for an entire function

↑ **Parent:** [Liouville theorem](#liouville-theorem)

If an [entire function](#entire-function) $f=u+iv$ has $uv$ bounded above, then $f$ is constant. Indeed $F=\exp(-if^2)$ is entire and $|F|=\exp(2uv)$ is bounded, so the [Liouville theorem](#liouville-theorem) makes $F$ constant. Differentiating gives $ff'=0$. The derivative of $f^2$ is therefore zero, and continuity on the connected complex plane makes $f$ itself constant. No separate boundedness of $u$ or $v$ is required.

### Dense image of a nonconstant entire function

↑ **Parent:** [Liouville theorem](#liouville-theorem)

The image of every nonconstant entire function is dense in $\mathbb C$. If a disc about $w$ were omitted, then $1/(f-w)$ would be bounded and entire, so Liouville's theorem would make $f$ constant.

### Entire function under a horizontal inverse-square-root bound

↑ **Parent:** [Liouville theorem](#liouville-theorem)

If an entire function satisfies $|h(z)|\leq|\operatorname{Re}z|^{-1/2}$ away from the imaginary axis, then $h=0$. Cauchy's formula on $|z|=R$ bounds every Taylor coefficient by a constant times

$$
R^{-n-1/2}\int_0^{2\pi}|\cos\theta|^{-1/2}\,d\theta,
$$

which tends to zero as $R\to\infty$.

### Polynomial growth theorem for entire functions

↑ **Parent:** [Liouville theorem](#liouville-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_growth_theorem_for_entire_functions)

An entire function bounded by a polynomial in the radius is itself a polynomial, by Cauchy estimates.

## Cauchy derivative formula

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_derivative_formula)

Cauchy’s derivative formula expresses derivatives as contour integrals with higher-order Cauchy kernels.

### Recovering an analytic derivative from the boundary real part

↑ **Parent:** [Cauchy derivative formula](#cauchy-derivative-formula)

For a [holomorphic function](#holomorphic-function) on a neighbourhood of a closed disc, parametrize the [Cauchy derivative formula](#cauchy-derivative-formula) on its boundary. The conjugate [Cauchy integral theorem](#cauchy-s-integral-theorem) gives $\int\overline{f(re^{i\theta})}e^{-i\theta}\,d\theta=0$. Replacing $f$ in the derivative integral by $f+\bar f=2\operatorname{Re}f$ therefore gives the displayed identity. The boundary real part determines every nonconstant analytic coefficient; only an imaginary additive constant is lost.

### Lipschitz bound inside a bounded analytic half-plane

↑ **Parent:** [Cauchy derivative formula](#cauchy-derivative-formula)

If $f$ is analytic and bounded by $K$ on $\operatorname{Re}z>0$, then Cauchy's derivative estimate gives

$$
|f'(z)|\leq K/c
$$

on $\operatorname{Re}z>c$. Integrating along line segments gives a Lipschitz bound with the same constant in that smaller half-plane.

## Locally uniform convergence of holomorphic functions

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_uniform_convergence_of_holomorphic_functions)

Locally uniform limits of holomorphic functions are holomorphic and their derivatives converge locally uniformly.

## Schwarz reflection principle

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarz_reflection_principle)

A holomorphic function real on a boundary interval extends across it by conjugate reflection.

## Upper half-plane self-map

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_half-plane_self-map)

An upper-half-plane self-map is holomorphic and has positive imaginary part in the upper half-plane.

## Argument principle

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Argument_principle)

If a meromorphic function has no zeros or poles on a positively oriented boundary $\gamma$, then

$$
\frac1{2\pi i}\int_\gamma\frac{f'}f\,dz=N-P,
$$

with zeros and poles counted by multiplicity.

### Radial crossing test for polynomial root counts

↑ **Parent:** [Argument principle](#argument-principle)

If $p(z(t))=t$ and $p'(z)\ne0$, implicit differentiation gives $z'(t)=1/p'(z)$. At a crossing of the [unit circle](#complex-unit-circle), the displayed radial derivative determines whether the root enters or leaves the [disk](topology.md#disk-mathematics) as the real parameter increases. Root counts are constant between such boundary crossings, including multiplicities. At the crossing parameter itself, boundary roots are excluded from an open-disk count. This complements the [winding number](#winding-number) form of the [argument principle](#argument-principle) and handles a self-intersecting [image](set-theory.md#image-of-a-function) [contour](#complex-integration-contour) without guessing its enclosed regions.

### Quarter-sector winding test for a real quartic

↑ **Parent:** [Argument principle](#argument-principle)

Suppose a monic real [quartic polynomial](polynomial.md#quartic-polynomial) has no nonnegative real zero and its real part on the imaginary axis is everywhere positive. For sufficiently large $R$, its image of the quarter-circle arc from $R$ to $iR$, closed by the straight chord from $p(iR)$ to $p(R)$, has [winding number](#winding-number) one: compare with $z^4$ on the arc and its constant image on the chord. The rest of the actual sector boundary maps into the right half-plane, so its replacement by that chord preserves the winding number. The [argument principle](#argument-principle) then counts exactly one root in the open first quadrant, including multiplicity.

<h3 id="rouche-s-theorem">Rouché's theorem</h3>

↑ **Parent:** [Argument principle](#argument-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rouché's_theorem)

If $f,g$ are holomorphic near the closure of a bounded domain and $|g|<|f|$ on its boundary, then $f$ and $f+g$ have the same number of interior zeros, counted with multiplicity. Apply the argument principle to the zero-free boundary homotopy $f+tg$.

<h4 id="rouche-localization-of-polynomial-roots">Rouché localization of polynomial roots</h4>

↑ **Parent:** [Rouché's theorem](#rouche-s-theorem)

Let $P(z)=\prod_\ell(z-r_\ell)$ have distinct roots. Choose a disc around $r_j$ with radius $\delta$ smaller than every separation from $r_j$. On its boundary, $|P(z)|\geq\delta\prod_{\ell\ne j}(|r_j-r_\ell|-\delta)$. If a [holomorphic](#complex-differentiability-at-a-point) perturbation $H$ satisfies the displayed inequality, [Rouché's theorem](#rouche-s-theorem) shows that $P+H$ has exactly one root in that disc, counted with multiplicity. Discs confined to specified half-planes or quadrants give direct geometric root-location proofs without needing a global root-continuation argument.

<h4 id="hurwitz-s-theorem">Hurwitz's theorem</h4>

↑ **Parent:** [Rouché's theorem](#rouche-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hurwitz's_theorem_(complex_analysis))

A locally uniform limit of nonvanishing holomorphic functions on a connected open set is either nonvanishing or identically zero. More generally, isolated zeros persist nearby with their multiplicity.

#### Open mapping theorem (complex analysis)

↑ **Parent:** [Rouché's theorem](#rouche-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Open_mapping_theorem_(complex_analysis))

A nonconstant holomorphic function on a domain maps open sets to open sets. Around any point, isolate its zero relative to the value there and use [Rouché's theorem](#rouche-s-theorem) to show that every sufficiently nearby value has a preimage.

##### Maximum modulus principle from the complex open mapping theorem

↑ **Parent:** [Open mapping theorem (complex analysis)](#open-mapping-theorem-complex-analysis)

If a nonconstant holomorphic function had a local maximum of its modulus, its open image near that point would contain values of larger modulus. Hence no such local maximum exists.

#### Unit-disc image from a boundary modulus lower bound

↑ **Parent:** [Rouché's theorem](#rouche-s-theorem)

If $f$ is holomorphic near the closed unit disc, $|f|\geq1$ on its boundary, and $|f(z_0)|<1$ at one interior point, then $f$ maps the open unit disc onto a set containing the open unit disc. Rouché's theorem first shows that $f$ has a zero and then that every $f-w$ with $|w|<1$ has one.

### Integer residue of a logarithmic derivative

↑ **Parent:** [Argument principle](#argument-principle)

If $g$ is holomorphic and nonvanishing on a punctured disc, then

$$
\operatorname{res}_0\frac{g'}g
=\frac1{2\pi i}\int_C\frac{g'}g\,dz
$$

is the integer winding number of $g(C)$ about zero. If it equals $k$, the logarithmic derivative of $z^{-k}g(z)$ has a removable singularity at zero.

## Meromorphic function with prescribed zeros and poles

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meromorphic_function_with_prescribed_zeros_and_poles)

A meromorphic function with finitely many specified simple zeros and poles is a rational product up to a nonzero holomorphic factor.

## Maximum modulus principle

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_modulus_principle)

A nonconstant holomorphic function on a connected domain cannot attain a local maximum of its modulus at an interior point.

### Hadamard three-circle theorem

↑ **Parent:** [Maximum modulus principle](#maximum-modulus-principle)

For a holomorphic scalar function on a neighborhood of a closed annulus, $M(r)$ is the maximum modulus on its radius-$r$ circle. The logarithm of its modulus is [subharmonic](partial-differential-equation.md#subharmonic-function); compare it with the harmonic function affine in $\log|z|$ which takes the logarithms of the two boundary maxima. The [maximum principle for subharmonic functions](partial-differential-equation.md#maximum-principle-for-subharmonic-functions) proves the displayed bound. Zero boundary maxima are handled by adding a positive bound and taking its limit. The same bound holds for the norm of a [Banach space](banach-space.md)-valued holomorphic function by applying scalar functionals and the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem).

<h3 id="phragmen-lindelof-principle">Phragmén–Lindelöf principle</h3>

↑ **Parent:** [Maximum modulus principle](#maximum-modulus-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phragmén–Lindelöf_principle)

A maximum-modulus extension for unbounded domains with suitable growth restrictions. In its polynomial-growth vertical-strip form, bounds $|F(a+it)|\ll(1+|t|)^u$ and $|F(b+it)|\ll(1+|t|)^v$ for a [holomorphic function](#holomorphic-function) imply the interpolated exponent $((b-\sigma)u+(\sigma-a)v)/(b-a)$. It is the strip-convexity tool used to move [subpower zeta bounds to the right of the critical line](analytic-number-theory.md#subpower-zeta-bound-to-the-right-of-the-critical-line) back onto that line.

### Maximum modulus principle on a bounded domain

↑ **Parent:** [Maximum modulus principle](#maximum-modulus-principle)

If a function is continuous on the closure of a bounded plane domain and holomorphic inside, the compact closure supplies a point of maximum modulus. Unless the function is constant, the [maximum modulus principle](#maximum-modulus-principle) places every maximum on the boundary.

#### Bounded half-plane maximum principle

↑ **Parent:** [Maximum modulus principle on a bounded domain](#maximum-modulus-principle-on-a-bounded-domain)

Let $f$ be bounded and holomorphic on a half-plane and continuous on its closure. A bound $|f|\leq M$ on the boundary line propagates throughout the half-plane. Apply the bounded-domain principle to $f(z)z^{-1/n}$ on expanding truncated half-discs, then let $n\to\infty$.

## Mean value property for holomorphic functions

↑ **Parent:** [Complex analysis](complex-analysis.md)

The value of a holomorphic function at the center of a closed disc equals its average around every concentric circle lying in the domain.

The real and imaginary parts are [harmonic functions](partial-differential-equation.md#harmonic-function), whose mean-value property explains this average identity.

## Dirichlet beta function

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_beta_function)

The Dirichlet beta function is $\beta(s)=\sum_{n\geq0}(-1)^n(2n+1)^{-s}$ and is the Dirichlet L-function for the nontrivial character modulo four.

### Special values of the Dirichlet beta function

↑ **Parent:** [Dirichlet beta function](#dirichlet-beta-function)

Hankel residue extraction gives $\beta(0)=1/2$, $\beta(-2)=-1/2$, and values at other nonpositive integers from the Taylor coefficients of $1/(2\cosh t)$.

### Dirichlet beta reflection formula

↑ **Parent:** [Dirichlet beta function](#dirichlet-beta-function)

The functional equation may be written

$$
\beta(1-s)=\Gamma(s)(\pi/2)^{-s}\sin(\pi s/2)\beta(s).
$$

## Identity theorem

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Identity_theorem)

Two holomorphic functions on a connected domain that agree on a set with an interior accumulation point agree everywhere.

## Residue at infinity from an asymptotic constant

↑ **Parent:** [Complex analysis](complex-analysis.md)

If $F(z)=L+O(1/z)$ uniformly on large circles, then $F(z)/z$ has residue $L$ at infinity in the large-contour sense and its counterclockwise large-circle integral tends to $2\pi iL$.

## Large-circle contour estimate

↑ **Parent:** [Complex analysis](complex-analysis.md)

On a circle of radius $R$, an integrand uniformly of order $R^{-2}$ has contour integral of order $R^{-1}$ by the estimation lemma.

## Fuchsian differential equation

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fuchsian_differential_equation)

A Fuchsian differential equation has only regular singular points, including possibly the point at infinity.

### Accessory parameter

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

An accessory parameter is a coefficient not determined by the singular points and their [indicial exponents](differential-equation.md#indicial-exponent). A second-order [Fuchsian differential equation](#fuchsian-differential-equation) with exactly three regular singular points has no such independent parameter.

### Regular singular point

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_singular_point)

A regular singular point is a singularity at which solutions of a linear differential equation have at worst controlled power and logarithmic behavior after a Frobenius reduction.

#### Logarithmically divergent derivative at a regular singular endpoint

↑ **Parent:** [Regular singular point](#regular-singular-point)

For $xy''+a(x)y=0$ with analytic coefficient and a continuous solution having $a(0)y(0)\ne0$, the equation gives $y''\sim-a(0)y(0)/x$. Integrating towards the endpoint gives the displayed logarithmic divergence of the [derivative](calculus.md#derivative). A bounded solution value therefore does not imply a finite [derivative](calculus.md#derivative) at a [regular singular point](#regular-singular-point).

#### Frobenius method

↑ **Parent:** [Regular singular point](#regular-singular-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius_method)

Near a regular singular point $x_0$, the Frobenius method seeks

$$
y=(x-x_0)^r\sum_{n\geq0}a_n(x-x_0)^n.
$$

The lowest power gives the indicial equation for $r$, and the remaining powers give a coefficient recurrence.

##### Undetermined coefficient at Frobenius resonance

↑ **Parent:** [Frobenius method](#frobenius-method)

When two [indicial roots](differential-equation.md#indicial-root) differ by a positive integer, the recurrence for the smaller-root [Frobenius solution](#frobenius-solution) can have a zero coefficient at the index of the larger root. If the corresponding right-hand side also vanishes, that coefficient is free and adds the larger-root solution; if it does not vanish, a pure Frobenius series is obstructed and a logarithmic term may be required. For $x^2y''-2xy'-x^2y=0$, the recurrence $n(n-3)a_n=a_{n-2}$ has $a_1=0$ and leaves $a_3$ free. Choosing $a_3=0$ selects the even solution, not the only solution with exponent zero.

##### Square-root reduction of a regular-singular differential equation

↑ **Parent:** [Frobenius method](#frobenius-method)

With $s=\sqrt z$ and $Y(s)=y(s^2)$, the displayed [linear differential equation](differential-equation.md#linear-differential-equation) becomes $Y_{ss}+Y=0$ away from zero. Its [Frobenius solutions](#frobenius-solution) have exponents $0$ and $1/2$: $\cos\sqrt z=\sum_{n\geq0}(-1)^nz^n/(2n)!$ and $\sin\sqrt z=z^{1/2}\sum_{n\geq0}(-1)^nz^n/(2n+1)!$. The first is an entire function of $z$; the second needs a local square-root branch. This illustrates how a [regular singular point](#regular-singular-point) can arise from a degenerate change of independent variable.

##### Frobenius solution

↑ **Parent:** [Frobenius method](#frobenius-method)

A local series solution at a regular singular point, with exponent $r$ satisfying the indicial equation. Resonant exponents can require a logarithmic companion solution.

##### Hyperbolic reduction of a regular-singular differential equation

↑ **Parent:** [Frobenius method](#frobenius-method)

The equation $x^2y''-2xy'+(2-x^2)y=0$ has a [regular singular point](#regular-singular-point) at zero. Factoring $y=xu$ cancels the Euler derivative terms and leaves $u''-u=0$ away from zero. Its analytic solutions $x\cosh x$ and $x\sinh x$ extend across zero. Their coefficient recurrence $(n-1)(n-2)c_n=c_{n-2}$ has independent free coefficients $c_1,c_2$, giving two entire solutions without a logarithmic branch despite integer-separated indicial roots.

##### Terminating Frobenius series

↑ **Parent:** [Frobenius method](#frobenius-method)

A terminating Frobenius series is a [Frobenius method](#frobenius-method) solution whose analytic [power series](real-analysis.md#power-series) factor has only finitely many nonzero coefficients. Its coefficient [linear recurrence relation](algebra.md#linear-recurrence-relation) must allow the first omitted coefficient and all following coefficients to be zero. At an integer separation of [characteristic exponents at a regular singular point](#characteristic-exponent-at-a-regular-singular-point), a resonant coefficient equation can become $0=0$, permitting such a choice rather than forcing a logarithmic term. With exponent zero, termination produces a [polynomial](polynomial.md) solution.

### Ordinary point criterion for a second-order equation

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

For $y''+P(z)y'+Q(z)y=0$, the finite point $z_0$ is ordinary when $P$ and $Q$ are [holomorphic](#holomorphic-function) at $z_0$.

### Characteristic exponent at a regular singular point

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

Substitution of a Frobenius behavior $(z-z_0)^\rho$ into the leading singular terms gives the indicial equation and its characteristic exponents.

### Regular singular point criterion for a second-order equation

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

For

$$
y''+P(z)y'+Q(z)y=0,
$$

$z_0$ is a regular singular point when $(z-z_0)P(z)$ and $(z-z_0)^2Q(z)$ are analytic at $z_0$.

#### Regular singular point at infinity

↑ **Parent:** [Regular singular point criterion for a second-order equation](#regular-singular-point-criterion-for-a-second-order-equation)

Under $\zeta=1/z$, the point $z=\infty$ is regular singular for

$$
y''+P(z)y'+Q(z)y=0
$$

exactly when $zP(z)$ and $z^2Q(z)$ are [holomorphic](#holomorphic-function) functions of $1/z$ near $1/z=0$.

#### Logarithmic solution from a repeated Frobenius exponent

↑ **Parent:** [Regular singular point criterion for a second-order equation](#regular-singular-point-criterion-for-a-second-order-equation)

When a second-order equation has a repeated indicial root and only one independent Frobenius series, a second solution has the local form

$$
y_2(z)=y_1(z)\log(z-z_0)+\text{a Frobenius series}.
$$

### Irregular singular point

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

A singular point of a linear differential equation is irregular when it fails the regular-singular criterion. For $y''+P(x)y'+Q(x)y=0$, a pole of order greater than one in $P$ or greater than two in $Q$ makes the point irregular.

<h4 id="poincare-rank">Poincaré rank</h4>

↑ **Parent:** [Irregular singular point](#irregular-singular-point)

For a first-order meromorphic [linear ordinary differential equation](differential-equation.md#linear-ordinary-differential-equation) $Y_t=A(t)Y$, with a coefficient [pole](isolated-singularity.md#pole) of order $p>1$ in a fixed local coordinate and gauge, its Poincaré rank is $p-1$. At infinity one must transform the differential system, not just the [matrix](vector-space.md#matrix)-valued function: $Y_\lambda=A_0\lambda^mY+\cdots$ becomes $Y_t=-A_0t^{-m-2}Y+\cdots$ under $t=1/\lambda$, giving rank $m+1$. A singular gauge can lower an apparent rank; distinct leading [eigenvalues](linear-operator-theory.md#eigenvalue) prevent the elementary degeneracy in the unramified setting.

<h3 id="riemann-s-differential-equation">Riemann's differential equation</h3>

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann's_differential_equation)

Riemann's differential equation is a second-order [ordinary differential equation](differential-equation.md#ordinary-differential-equation) with three [regular singular points](#regular-singular-point), normalized to zero, one and infinity by a [Möbius transformation](group-theory.md#mobius-transformation). Its local characteristic exponents are encoded by the [Papperitz symbol](#papperitz-symbol) and constrained by the [Fuchs relation](#fuchs-relation).

#### Papperitz symbol

↑ **Parent:** [Riemann's differential equation](#riemann-s-differential-equation)

A Papperitz or P-symbol lists the three regular singular points of a second-order equation and the two characteristic exponents at each.

This symbol records the local exponents of [Riemann's differential equation](#riemann-s-differential-equation).

##### Fuchs relation

↑ **Parent:** [Papperitz symbol](#papperitz-symbol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fuchs_relation)

For a second-order equation with three regular singular points, the sum of all six characteristic exponents is one.

For an order-$n$ [Fuchsian differential equation](#fuchsian-differential-equation) with $r$ finite singular points and infinity, the sum of all characteristic exponents is $n(n-1)(r-1)/2$. The three-singularity second-order case has $n=2$ and $r=2$.

<h5 id="mobius-transformation-of-a-papperitz-symbol">Möbius transformation of a Papperitz symbol</h5>

↑ **Parent:** [Papperitz symbol](#papperitz-symbol)

A Möbius change of independent variable permutes the singular points while carrying their characteristic exponent pairs with them.

##### Dependent-variable rescaling of a Papperitz symbol

↑ **Parent:** [Papperitz symbol](#papperitz-symbol)

Multiplying a solution by $(z-z_0)^\lambda$ adds $\lambda$ to both exponents at the finite point $z_0$ and subtracts $\lambda$ from both exponents at infinity, under the convention that an exponent $\rho$ at infinity corresponds to behavior $z^{-\rho}$.

### Gauss hypergeometric equation

↑ **Parent:** [Fuchsian differential equation](#fuchsian-differential-equation)

The Gauss equation has singularities at $0,1,\infty$ and normalized exponent-zero solution $F(A,B;C;u)$ at the origin.

<h4 id="euler-s-hypergeometric-transformation">Euler's hypergeometric transformation</h4>

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

Multiply a solution with parameters $(c-a,c-b;c)$ by $(1-z)^{c-a-b}$. Its local exponents become exactly those of the [Gauss hypergeometric equation](#gauss-hypergeometric-equation) with parameters $(a,b;c)$: those at one shift by $c-a-b$, and those at infinity shift by its negative. Direct differentiation gives the same [differential](differential-geometry.md#differential-of-a-smooth-map) equation. Near zero, choose the factor with value one; uniqueness of the analytic normalized solution, for $c$ not a nonpositive integer, gives the identity. Compatible analytic continuation extends it to other domains and parameters where the normalized functions are defined.

#### Hypergeometric connection formula at one

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

Put $d=c-a-b\notin\mathbb Z$ and choose a branch of $(1-z)^d$. The solution regular at zero is

$$
{}_2F_1(a,b;c;z)=\frac{\Gamma(c)\Gamma(d)}{\Gamma(c-a)\Gamma(c-b)}{}_2F_1(a,b;1-d;1-z)+\frac{\Gamma(c)\Gamma(-d)}{\Gamma(a)\Gamma(b)}(1-z)^d{}_2F_1(c-a,c-b;1+d;1-z).
$$

The two [characteristic exponents at a regular singular point](#characteristic-exponent-at-a-regular-singular-point) are $0,d$. The [Euler integral for the hypergeometric function](#euler-integral-for-the-hypergeometric-function) determines the first coefficient by a finite endpoint limit and the second by scaling the singular endpoint; [analytic continuation](#analytic-continuation) extends the parameter ranges.

#### Hypergeometric function

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypergeometric_function)

The Gauss hypergeometric function is the normalized analytic solution at zero,

$$
{}_2F_1(a,b;c;z)
=\sum_{n=0}^{\infty}\frac{(a)_n(b)_n}{(c)_n}\frac{z^n}{n!},
$$

initially for $|z|<1$ and $c\notin\{0,-1,-2,\ldots\}$, followed by [analytic continuation](#analytic-continuation) where possible.

The ordinary [hypergeometric function](#hypergeometric-function) is ${}_2F_1(a,b;c;z)=\sum_{n\geq0}(a)_n(b)_nz^n/((c)_n n!)$ near zero for admissible $c$. It solves the [Gauss hypergeometric equation](#gauss-hypergeometric-equation) and extends by [analytic continuation](#analytic-continuation).

##### Euler integral for the hypergeometric function

↑ **Parent:** [Hypergeometric function](#hypergeometric-function)

For $\Re c>\Re b>0$ and a fixed branch away from the cut,

$$
{}_2F_1(a,b;c;z)=\frac{\Gamma(c)}{\Gamma(b)\Gamma(c-b)}\int_0^1s^{b-1}(1-s)^{c-b-1}(1-zs)^{-a}\,ds.
$$

Expand $(1-zs)^{-a}$ for $|z|<1$ and integrate termwise using the [beta function](#beta-function) to recover the [Gauss hypergeometric function](#hypergeometric-function) series. [Analytic continuation](#analytic-continuation) extends the identity in $z$.

#### Pfaff transformation

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

With compatible branches and initially near $z=0$,

$$
F\left(a,c-b;c;\frac{z}{z-1}\right)
=(1-z)^aF(a,b;c;z).
$$

It follows by applying a Möbius transformation and a dependent-variable rescaling to the same [Papperitz symbol](#papperitz-symbol), then matching the normalized analytic solution at zero.

#### Second local hypergeometric solution

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

When $C$ is not an integer, a second local solution at zero is $u^{1-C}F(A-C+1,B-C+1;2-C;u)$.

#### Hypergeometric connection formula at infinity

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

Away from resonant parameter cases, two independent local solutions at infinity are

$$
z^{-a}F(a,1+a-c;1+a-b;z^{-1})
$$

and the expression obtained by exchanging $a$ and $b$. Every analytic continuation of a hypergeometric solution into their common domain is a constant linear combination of this basis.

#### Hypergeometric cancellation identity

↑ **Parent:** [Gauss hypergeometric equation](#gauss-hypergeometric-equation)

The binomial series gives $F(A,C;C;u)=(1-u)^{-A}$ wherever the defining series converges, followed by analytic continuation.

##### Elementary specialization of a hypergeometric solution

↑ **Parent:** [Hypergeometric cancellation identity](#hypergeometric-cancellation-identity)

Special parameter choices can identify a hypergeometric solution with an elementary solution of the same second-order differential equation by matching its local normalization.

###### Hypergeometric cosine identity

↑ **Parent:** [Elementary specialization of a hypergeometric solution](#elementary-specialization-of-a-hypergeometric-solution)

For compatible local branches near $x=0$,

$$
F\left(\frac{k}{2},-\frac{k}{2};\frac12;\sin^2x\right)=\cos(kx).
$$

It follows by transforming the [harmonic oscillator equation](classical-mechanics.md#simple-harmonic-motion) $y''+k^2y=0$ into the [Gauss hypergeometric equation](#gauss-hypergeometric-equation) and selecting the solution with value one and derivative zero at the origin.

###### Hypergeometric sine identity

↑ **Parent:** [Elementary specialization of a hypergeometric solution](#elementary-specialization-of-a-hypergeometric-solution)

For $k\ne0$ and compatible local branches near $x=0$,

$$
F\left(\frac{1+k}{2},\frac{1-k}{2};\frac32;\sin^2x\right)
=\frac{\sin(kx)}{k\sin x}.
$$

This is obtained from the [second local hypergeometric solution](#second-local-hypergeometric-solution) at zero and its normalization.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Analytic number theory](analytic-number-theory.md)
- [Domain (mathematical analysis)](topology.md#domain-mathematical-analysis)
- [Resolvent formalism](functional-analysis.md#resolvent-formalism)
