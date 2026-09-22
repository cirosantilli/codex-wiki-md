# Modular function

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_function)

A modular function of weight $k$ for a subgroup $\Gamma\leq SL_2(\mathbb Z)$ is a meromorphic function on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) that satisfies

$$
f(\gamma\tau)=(c\tau+d)^k f(\tau)
$$

for $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma$ and is meromorphic at every cusp.

**Table of contents**

- [Modular lambda function](#modular-lambda-function)
  - [Universal covering by the modular lambda function](#universal-covering-by-the-modular-lambda-function)
- [Modular curve](#modular-curve)
  - [Elliptic point of a modular curve](#elliptic-point-of-a-modular-curve)
  - [Modular symbol](#modular-symbol)
    - [Manin symbol](#manin-symbol)
  - [X0 2 modular curve](#x0-2-modular-curve)
    - [Discriminant-ratio coordinate on X0 2](#discriminant-ratio-coordinate-on-x0-2)
  - [Compactified modular curve](#compactified-modular-curve)
  - [Level-two modular curve](#level-two-modular-curve)
  - [Genus formula for a modular curve](#genus-formula-for-a-modular-curve)
    - [Principal congruence modular curve genus](#principal-congruence-modular-curve-genus)
      - [Elliptic and cusp ramification for principal level](#elliptic-and-cusp-ramification-for-principal-level)
    - [Modular curve X0 3](#modular-curve-x0-3)
- [Cusp of a modular group](#cusp-of-a-modular-group)
  - [Width of a cusp](#width-of-a-cusp)
  - [Holomorphic at a cusp](#holomorphic-at-a-cusp)
    - [Cusp holomorphy under rational slash operators](#cusp-holomorphy-under-rational-slash-operators)
- [Modular form](#modular-form)
  - [Weight of a modular form](#weight-of-a-modular-form)
  - [Mellin continuation of a noncuspidal modular form](#mellin-continuation-of-a-noncuspidal-modular-form)
  - [Dimension of level-one modular forms](#dimension-of-level-one-modular-forms)
    - [Polynomial ring of level-one modular forms](#polynomial-ring-of-level-one-modular-forms)
      - [Graded weights separate analytic polynomial relations](#graded-weights-separate-analytic-polynomial-relations)
      - [Rational structure of level-one modular forms](#rational-structure-of-level-one-modular-forms)
  - [Modular forms as meromorphic differentials on X(1)](#modular-forms-as-meromorphic-differentials-on-x-1)
  - [Integral triangular basis of level-one modular forms](#integral-triangular-basis-of-level-one-modular-forms)
  - [Modular form on a finite-index subgroup](#modular-form-on-a-finite-index-subgroup)
    - [Nebentypus character](#nebentypus-character)
    - [Coset norm of a modular form](#coset-norm-of-a-modular-form)
  - [Serre derivative](#serre-derivative)
    - [First Rankin-Cohen bracket](#first-rankin-cohen-bracket)
  - [Oldform by argument dilation](#oldform-by-argument-dilation)
    - [Prime stabilization of an oldform](#prime-stabilization-of-an-oldform)
    - [Weight-four modular forms on Gamma 0 3](#weight-four-modular-forms-on-gamma-0-3)
  - [Weak modular form](#weak-modular-form)
    - [Derivative transformation of a weak modular form](#derivative-transformation-of-a-weak-modular-form)
      - [Bol identity for modular forms](#bol-identity-for-modular-forms)
  - [Fricke involution](#fricke-involution)
    - [Fricke sign from a nonvanishing fixed-point value](#fricke-sign-from-a-nonvanishing-fixed-point-value)
  - [Modular group](#modular-group)
    - [Modular-invariant function](#modular-invariant-function)
    - [Rational conjugation of finite-index modular subgroups](#rational-conjugation-of-finite-index-modular-subgroups)
    - [Standard fundamental domain of the modular group](#standard-fundamental-domain-of-the-modular-group)
      - [Fundamental region of a modular subgroup](#fundamental-region-of-a-modular-subgroup)
      - [Elliptic stabilizers of the modular group](#elliptic-stabilizers-of-the-modular-group)
      - [Reduction to the standard modular region](#reduction-to-the-standard-modular-region)
  - [Slash operator for modular forms](#slash-operator-for-modular-forms)
    - [Double-coset operator on modular forms](#double-coset-operator-on-modular-forms)
    - [Hecke-normalized rational slash operator](#hecke-normalized-rational-slash-operator)
    - [Determinant-normalized slash operator](#determinant-normalized-slash-operator)
    - [Automorphy factor](#automorphy-factor)
  - [Fourier expansion of a modular form](#fourier-expansion-of-a-modular-form)
    - [Cusp form](#cusp-form)
      - [Old subspace of cusp forms](#old-subspace-of-cusp-forms)
        - [Degeneracy map for cusp forms](#degeneracy-map-for-cusp-forms)
          - [Prime-level cusp orders of discriminant degeneracy forms](#prime-level-cusp-orders-of-discriminant-degeneracy-forms)
        - [Prime-power old block at a bad prime](#prime-power-old-block-at-a-bad-prime)
      - [New subspace of cusp forms](#new-subspace-of-cusp-forms)
        - [Newform](#newform)
          - [Bad-prime eigenvalue of a trivial-character newform](#bad-prime-eigenvalue-of-a-trivial-character-newform)
          - [Newform multiplicity-one theorem](#newform-multiplicity-one-theorem)
      - [L-function of a cusp form](#l-function-of-a-cusp-form)
        - [Additive twist of a cusp-form L-function](#additive-twist-of-a-cusp-form-l-function)
          - [Functional equation of an additive cusp-form twist](#functional-equation-of-an-additive-cusp-form-twist)
          - [Rational-cusp inversion of a level-one cusp form](#rational-cusp-inversion-of-a-level-one-cusp-form)
      - [Character twist by rational translations of a cusp form](#character-twist-by-rational-translations-of-a-cusp-form)
        - [Primitive twist at coprime level](#primitive-twist-at-coprime-level)
          - [Fricke transform of a primitive coprime twist](#fricke-transform-of-a-primitive-coprime-twist)
      - [Invariant norm of a modular form](#invariant-norm-of-a-modular-form)
        - [Bounded invariant norm characterization of cusp forms](#bounded-invariant-norm-characterization-of-cusp-forms)
        - [Fourier coefficient bound for a cusp form](#fourier-coefficient-bound-for-a-cusp-form)
      - [Fourier coefficient growth criterion for a level-one cusp form](#fourier-coefficient-growth-criterion-for-a-level-one-cusp-form)
      - [Dimension of level-one cusp forms](#dimension-of-level-one-cusp-forms)
      - [Mellin transform of a cusp-form L-function](#mellin-transform-of-a-cusp-form-l-function)
        - [Phase-normalized Fricke functional equation](#phase-normalized-fricke-functional-equation)
      - [Modular discriminant](#modular-discriminant)
        - [Multiplication by the modular discriminant](#multiplication-by-the-modular-discriminant)
        - [Weight-two discriminant root at level eleven](#weight-two-discriminant-root-at-level-eleven)
        - [Integrality identity for the modular discriminant](#integrality-identity-for-the-modular-discriminant)
        - [Ramanujan tau function](#ramanujan-tau-function)
          - [Ramanujan tau congruence modulo five](#ramanujan-tau-congruence-modulo-five)
          - [Ramanujan congruence modulo 691](#ramanujan-congruence-modulo-691)
        - [Mellin transform of the modular discriminant](#mellin-transform-of-the-modular-discriminant)
      - [Petersson inner product](#petersson-inner-product)
        - [Hecke operators are self-adjoint for the Petersson inner product](#hecke-operators-are-self-adjoint-for-the-petersson-inner-product)
        - [Rankin–Selberg method](#rankin-selberg-method)
          - [Rankin–Selberg integral for holomorphic cusp forms](#rankin-selberg-integral-for-holomorphic-cusp-forms)
            - [Positive unfolding of a cusp-form square](#positive-unfolding-of-a-cusp-form-square)
              - [Absolute convergence of cusp-form L-series from square coefficients](#absolute-convergence-of-cusp-form-l-series-from-square-coefficients)
          - [Rankin–Selberg convolution](#rankin-selberg-convolution)
            - [Euler factor of a coefficientwise product of Hecke eigenforms](#euler-factor-of-a-coefficientwise-product-of-hecke-eigenforms)
            - [Zeta-completed Rankin-Selberg coefficient series](#zeta-completed-rankin-selberg-coefficient-series)
            - [Rankin–Selberg unfolding identity for a holomorphic Eisenstein series](#rankin-selberg-unfolding-identity-for-a-holomorphic-eisenstein-series)
  - [Eisenstein series](#eisenstein-series)
    - [Lattice Eisenstein sum](#lattice-eisenstein-sum)
      - [A complex lattice is determined by its fourth and sixth Eisenstein sums](#a-complex-lattice-is-determined-by-its-fourth-and-sixth-eisenstein-sums)
    - [Weight-four Eisenstein basis at level two](#weight-four-eisenstein-basis-at-level-two)
    - [Character-twisted Eisenstein series](#character-twisted-eisenstein-series)
      - [Fourier expansion of a character-twisted Eisenstein series](#fourier-expansion-of-a-character-twisted-eisenstein-series)
    - [Fourier expansion of a normalized Eisenstein series](#fourier-expansion-of-a-normalized-eisenstein-series)
      - [Divisor-sum convolution identity of weights four and eight](#divisor-sum-convolution-identity-of-weights-four-and-eight)
    - [Integral echelon basis of level-one modular forms](#integral-echelon-basis-of-level-one-modular-forms)
      - [Eisenstein congruence from a denominator prime](#eisenstein-congruence-from-a-denominator-prime)
        - [Weight-sixteen Eisenstein congruence](#weight-sixteen-eisenstein-congruence)
    - [Congruence-class Eisenstein series](#congruence-class-eisenstein-series)
    - [Orthogonality of cusp forms and holomorphic Eisenstein series](#orthogonality-of-cusp-forms-and-holomorphic-eisenstein-series)
    - [Eisenstein series of weight two](#eisenstein-series-of-weight-two)
      - [Almost holomorphic weight-two Eisenstein series](#almost-holomorphic-weight-two-eisenstein-series)
        - [Weight-two transformation from an invariant Eisenstein limit](#weight-two-transformation-from-an-invariant-eisenstein-limit)
        - [Cancellation of weight-two Eisenstein anomalies](#cancellation-of-weight-two-eisenstein-anomalies)
      - [Iterated Eisenstein summation in weight two](#iterated-eisenstein-summation-in-weight-two)
    - [Nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series)
      - [Completed nonholomorphic Eisenstein series](#completed-nonholomorphic-eisenstein-series)
        - [Kronecker limit formula](#kronecker-limit-formula)
      - [Primitive real-analytic Eisenstein series](#primitive-real-analytic-eisenstein-series)
      - [Constant term of a nonholomorphic Eisenstein series](#constant-term-of-a-nonholomorphic-eisenstein-series)
      - [Hecke eigenvalue of a nonholomorphic Eisenstein series](#hecke-eigenvalue-of-a-nonholomorphic-eisenstein-series)
    - [Weight-k real-analytic Eisenstein series](#weight-k-real-analytic-eisenstein-series)
      - [Analytic continuation of a weight-k real-analytic Eisenstein series](#analytic-continuation-of-a-weight-k-real-analytic-eisenstein-series)
      - [Absolute convergence of a weight-k real-analytic Eisenstein series](#absolute-convergence-of-a-weight-k-real-analytic-eisenstein-series)
      - [Invariant product with a weight-k real-analytic Eisenstein series](#invariant-product-with-a-weight-k-real-analytic-eisenstein-series)
  - [Hecke operator](#hecke-operator)
    - [Modular Hecke algebra](#modular-hecke-algebra)
      - [Eisenstein ideal](#eisenstein-ideal)
    - [Hecke eigenform](#hecke-eigenform)
      - [Prime-power coefficients of a level-one eigenform are often large and positive](#prime-power-coefficients-of-a-level-one-eigenform-are-often-large-and-positive)
      - [Euler product of a Hecke eigenform](#euler-product-of-a-hecke-eigenform)
      - [Hecke eigenvalues are algebraic integers](#hecke-eigenvalues-are-algebraic-integers)
    - [Hecke multiplication relations](#hecke-multiplication-relations)
      - [Hecke prime-power recurrence from q-shift operators](#hecke-prime-power-recurrence-from-q-shift-operators)
    - [Noncuspidal level-one Hecke eigenform](#noncuspidal-level-one-hecke-eigenform)
    - [Integral Hecke algebra of level-one cusp forms](#integral-hecke-algebra-of-level-one-cusp-forms)
      - [Perfect integral Hecke pairing](#perfect-integral-hecke-pairing)
    - [Fourier coefficients of a composite-index Hecke operator](#fourier-coefficients-of-a-composite-index-hecke-operator)
    - [Determinant-n matrix representatives for Hecke operators](#determinant-n-matrix-representatives-for-hecke-operators)
    - [Finite Hecke orbit criterion for holomorphy at a cusp](#finite-hecke-orbit-criterion-for-holomorphy-at-a-cusp)
  - [Meromorphic modular form](#meromorphic-modular-form)
    - [Cusp-form divisor presentation](#cusp-form-divisor-presentation)
    - [Regular-cusp valence formula on a torsion-free modular curve](#regular-cusp-valence-formula-on-a-torsion-free-modular-curve)
    - [Valence formula for the modular group](#valence-formula-for-the-modular-group)
      - [Vanishing of weight-fourteen level-one cusp forms](#vanishing-of-weight-fourteen-level-one-cusp-forms)
      - [Vanishing of weight-two level-one modular forms](#vanishing-of-weight-two-level-one-modular-forms)
      - [Dimension bound for modular forms on a finite-index subgroup](#dimension-bound-for-modular-forms-on-a-finite-index-subgroup)
    - [Klein j-invariant](#klein-j-invariant)
      - [Klein j-invariant classifies complex lattice homothety](#klein-j-invariant-classifies-complex-lattice-homothety)
      - [Level-two modular ratio of Klein j-invariants](#level-two-modular-ratio-of-klein-j-invariants)
  - [Theta function](#theta-function)
    - [Riemann theta function](#riemann-theta-function)
    - [Gaussian theta sum](#gaussian-theta-sum)
      - [Theta series of a Euclidean lattice](#theta-series-of-a-euclidean-lattice)
      - [Small-parameter asymptotic of a lattice theta sum](#small-parameter-asymptotic-of-a-lattice-theta-sum)
      - [Covolume-one theta function of a fractional ideal](#covolume-one-theta-function-of-a-fractional-ideal)
    - [Lattice theta functional equation](#lattice-theta-functional-equation)
      - [Anisotropic theta functional equation](#anisotropic-theta-functional-equation)
    - [Jacobi theta function](#jacobi-theta-function)
      - [Jacobi derivative formula](#jacobi-derivative-formula)
      - [Theta function with characteristics](#theta-function-with-characteristics)
        - [Theta constant](#theta-constant)
        - [Period lattice of theta3 over theta4](#period-lattice-of-theta3-over-theta4)
        - [Jacobi theta duplication identity](#jacobi-theta-duplication-identity)
        - [Modular transformations of theta characteristics](#modular-transformations-of-theta-characteristics)
        - [Heat equation for theta functions with characteristics](#heat-equation-for-theta-functions-with-characteristics)
        - [Zeros of theta functions with characteristics](#zeros-of-theta-functions-with-characteristics)
      - [Jacobi abstruse identity](#jacobi-abstruse-identity)
      - [Theta-constant inversion and translation laws](#theta-constant-inversion-and-translation-laws)
      - [Theta series of integer squares](#theta-series-of-integer-squares)
        - [Eight-square representation formula](#eight-square-representation-formula)
      - [Jacobi triple product](#jacobi-triple-product)
        - [Jacobi cubic product identity](#jacobi-cubic-product-identity)
        - [Euler pentagonal identity](#euler-pentagonal-identity)
      - [Theta group](#theta-group)
      - [Nonvanishing of the Jacobi theta function](#nonvanishing-of-the-jacobi-theta-function)
  - [Lattice model of a modular form](#lattice-model-of-a-modular-form)
    - [Gamma 1 level structure on a complex lattice](#gamma-1-level-structure-on-a-complex-lattice)
      - [Diamond operator](#diamond-operator)
      - [Hecke operator on marked lattices](#hecke-operator-on-marked-lattices)
        - [Good-prime and bad-prime Hecke coefficient formula](#good-prime-and-bad-prime-hecke-coefficient-formula)
      - [Marked-lattice model of a modular form](#marked-lattice-model-of-a-modular-form)
      - [Prime-index overlattices preserving a Gamma 1 level structure](#prime-index-overlattices-preserving-a-gamma-1-level-structure)
    - [Weighted Gaussian theta sum of a complex lattice](#weighted-gaussian-theta-sum-of-a-complex-lattice)
    - [Hecke operator on lattice functions](#hecke-operator-on-lattice-functions)

## Modular lambda function

↑ **Parent:** [Modular function](modular-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_lambda_function)

The nonzero even theta constants and the [Jacobi abstruse identity](#jacobi-abstruse-identity) give $\lambda(-1/\tau)=1-\lambda(\tau)$ and $\lambda(\tau+1)=\lambda(\tau)/(\lambda(\tau)-1)$. It is invariant under the principal [congruence subgroup](group-theory.md#congruence-subgroup) of level two. This parameter puts the associated complex [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) in Legendre form $y^2=x(x-1)(x-\lambda)$; its [Klein j-invariant](#klein-j-invariant) is $256(1-\lambda+\lambda^2)^3/[\lambda^2(1-\lambda)^2]$.

### Universal covering by the modular lambda function

↑ **Parent:** [Modular lambda function](#modular-lambda-function)

The [modular lambda function](#modular-lambda-function) is invariant under the projective level-two [principal congruence subgroup](group-theory.md#principal-congruence-subgroup). That group acts freely, and its quotient is the [level-two modular curve](#level-two-modular-curve). Adding its three [modular cusps](#cusp-of-a-modular-group) gives a sphere, and $\lambda$ has cusp values $0,1,\infty$, with simple orders in exponential cusp coordinates. Therefore it identifies the quotient with the sphere minus those three points. Since the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) is simply connected, this is a [universal covering map](algebraic-topology.md#universal-cover), with the projective level-two group as its [deck transformation group](algebraic-topology.md#deck-transformation-group).

## Modular curve

↑ **Parent:** [Modular function](modular-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_curve)

For a congruence subgroup $\Gamma$, the compact modular curve is

$$
X(\Gamma)=\Gamma\backslash\bigl(\mathfrak h\cup\mathbb P^1(\mathbb Q)\bigr).
$$

At an ordinary point it inherits a coordinate from $\mathfrak h$; at an elliptic point of stabilizer order $e$ a coordinate is the $e$th power of a local disk coordinate; and at a cusp of width $h$ a coordinate is $e^{2\pi i\tau/h}$.

### Elliptic point of a modular curve

↑ **Parent:** [Modular curve](#modular-curve)

An [elliptic point of a modular curve](#elliptic-point-of-a-modular-curve) is the image of a point of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) with a nontrivial [stabilizer subgroup](group-theory.md#stabilizer-subgroup) in the effective modular subgroup. For the full [modular group](#modular-group) the [stabilizer subgroup](group-theory.md#stabilizer-subgroup) orders are two and three, represented by $i$ and $e^{2\pi i/3}$. A local disk coordinate $u$ upstairs descends as $u^e$ when the [stabilizer subgroup](group-theory.md#stabilizer-subgroup) order is $e$. The central [matrices](vector-space.md#matrix) $\pm I$ are factored out before counting this order.

### Modular symbol

↑ **Parent:** [Modular curve](#modular-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_symbol)

A modular symbol is the [relative homology class](homology.md#relative-homology-class) of a path between two [modular cusps](#cusp-of-a-modular-group). Oriented paths satisfy $\{\alpha,\beta\}+\{\beta,\gamma\}=\{\alpha,\gamma\}$. [Continued fractions](number-theory.md#continued-fraction) subdivide rational-endpoint paths into unimodular edges, giving a finite presentation through [Manin symbols](#manin-symbol). The [Hecke operators](#hecke-operator) act by finite sums of transformed paths, so their matrices can be computed by rational linear algebra.

#### Manin symbol

↑ **Parent:** [Modular symbol](#modular-symbol)

For a finite-index modular subgroup, a Manin symbol records a coset and its associated oriented unimodular edge. Over the rationals the presentation has the relations $[g]+[gS]=0$ and $[g]+[gST]+[g(ST)^2]=0$, for inversion $S$ and translation $T$. They express reversing an edge and the boundary of a triangle. Integral computation also removes torsion caused by elliptic stabilizers. The boundary map sends the symbol to its terminal cusp minus its initial cusp; its kernel is absolute [homology](homology.md).

### X0 2 modular curve

↑ **Parent:** [Modular curve](#modular-curve)

The compact quotient for the [Gamma 0 congruence subgroup](group-theory.md#gamma-0-congruence-subgroup) at level two has projective index three, two [modular cusps](#cusp-of-a-modular-group) of [cusp widths](#width-of-a-cusp) one and two, one order-two elliptic orbit and no order-three elliptic orbit. It has genus zero. It differs from the level-two principal-congruence curve for $\Gamma(2)$, which has three [modular cusps](#cusp-of-a-modular-group).

#### Discriminant-ratio coordinate on X0 2

↑ **Parent:** [X0 2 modular curve](#x0-2-modular-curve)

The ratio of [modular discriminants](#modular-discriminant) has weight zero and level $\Gamma_0(2)$. It has one [simple pole](isolated-singularity.md#simple-pole) at infinity and one simple zero at the zero [modular cusp](#cusp-of-a-modular-group), with no zeros or [poles](isolated-singularity.md#pole) in the half-plane. It is a spherical coordinate by the [single-pole criterion for a spherical coordinate](isolated-singularity.md#single-pole-criterion-for-a-spherical-coordinate). The [Klein j-invariant](#klein-j-invariant) is $(t+256)^3/t^2$, with $t(e^{2\pi i/3})=-256$.

### Compactified modular curve

↑ **Parent:** [Modular curve](#modular-curve)

For a finite-index subgroup of the [modular group](#modular-group), the quotient of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) becomes a compact [Riemann surface](complex-analysis.md#riemann-surfaces) after adjoining its cusp classes. At an elliptic fixed point use the quotient coordinate for the finite stabilizer; at a cusp use its exponential local parameter. Weight-zero [modular forms](#modular-form) descend to [holomorphic functions](complex-analysis.md#holomorphic-function) on this compact surface, and hence are constant by the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle).

### Level-two modular curve

↑ **Parent:** [Modular curve](#modular-curve)

The quotient $\mathbb H/\Gamma(2)$ is a [genus](topology.md#genus-of-a-surface)-zero [Riemann surface](complex-analysis.md#riemann-surfaces) with three cusps and no [elliptic Möbius transformations](geometry-and-topology.md#elliptic-element-of-psl2-r), hence is [biholomorphic](complex-analysis.md#biholomorphism) to $\mathbb C\setminus\{0,1\}$. The integer level-two [principal congruence subgroup](group-theory.md#principal-congruence-subgroup) has projective index six; reduction modulo two gives three cusp classes.

### Genus formula for a modular curve

↑ **Parent:** [Modular curve](#modular-curve)

Let $\mu=[PSL_2(\mathbb Z):\overline\Gamma]$, let $e_2,e_3$ count elliptic orbits of orders two and three, and let $c$ be the number of cusps. Then

$$
g(X(\Gamma))=1+\frac{\mu}{12}-\frac{e_2}{4}-\frac{e_3}{3}-\frac c2.
$$

#### Principal congruence modular curve genus

↑ **Parent:** [Genus formula for a modular curve](#genus-formula-for-a-modular-curve)

For $N\geq3$, the [principal congruence subgroup](group-theory.md#principal-congruence-subgroup) has projective index $\mu=\frac12N^3\prod_{p\mid N}(1-p^{-2})$, no effective elliptic stabilizers, and all [cusp widths](#width-of-a-cusp) equal to $N$. Hence the number of cusps is $\mu/N$, and the [genus formula for a modular curve](#genus-formula-for-a-modular-curve) gives the displayed formula. The exceptional levels one and two both have genus zero; the full genus-zero list is $N=1,2,3,4,5$. Level six has genus one and every larger level has positive genus.

##### Elliptic and cusp ramification for principal level

↑ **Parent:** [Principal congruence modular curve genus](#principal-congruence-modular-curve-genus)

For $N\geq2$, the effective [principal congruence subgroup](group-theory.md#principal-congruence-subgroup) is torsion-free. Its [modular curve](#modular-curve) cover of $X(1)$ has [analytic ramification indices](complex-analysis.md#ramification-index-of-a-holomorphic-map) $2,3,N$ above the two elliptic orbits and the [modular cusp](#cusp-of-a-modular-group). If $\mu$ is its projective index, the numbers of points above these three values are $\mu/2,\mu/3,\mu/N$. Applying the [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) gives $2g-2=\mu(1/6-1/N)$. Here $\mu=6$ for $N=2$ and $\mu=N^3\prod_{p\mid N}(1-p^{-2})/2$ for $N\geq3$; level one is the identity cover.

#### Modular curve X0 3

↑ **Parent:** [Genus formula for a modular curve](#genus-formula-for-a-modular-curve)

The modular curve $X_0(3)$ has index four, two cusps, no elliptic orbit of order two, and one elliptic orbit of order three. Its genus is therefore zero.

## Cusp of a modular group

↑ **Parent:** [Modular function](modular-function.md)

A cusp of a finite-index subgroup $\Gamma\leq SL_2(\mathbb Z)$ is an orbit in $\Gamma\backslash\mathbb P^1(\mathbb Q)$. If $\sigma\in SL_2(\mathbb Z)$ sends infinity to a cusp, behavior there is studied through $f|_k\sigma$.

### Width of a cusp

↑ **Parent:** [Cusp of a modular group](#cusp-of-a-modular-group)

The width of a cusp represented by $\sigma\in SL_2(\mathbb Z)$ is the least positive $h$ such that $\sigma T^h\sigma^{-1}$ lies in the subgroup, up to its center. Its local parameter is $q_h=e^{2\pi i\tau/h}$.

### Holomorphic at a cusp

↑ **Parent:** [Cusp of a modular group](#cusp-of-a-modular-group)

A modular function is holomorphic at a cusp when its expansion in the corresponding local parameter has no negative powers. It vanishes at the cusp when that expansion has zero constant term.

#### Cusp holomorphy under rational slash operators

↑ **Parent:** [Holomorphic at a cusp](#holomorphic-at-a-cusp)

If $f$ is a [modular form on a finite-index subgroup](#modular-form-on-a-finite-index-subgroup) and $\gamma$ is rational with positive [determinant](linear-algebra.md#determinant), then $f|_k\gamma$ is bounded near infinity. Choose $\sigma\in SL_2(\mathbb Z)$ with $\sigma\infty=\gamma\infty$. The [matrix](vector-space.md#matrix) $\sigma^{-1}\gamma$ is upper triangular and sends $z$ to $Az+B$ with $A>0$. Thus the existing cusp expansion of $f|_k\sigma$ stays bounded under this substitution. [Rational conjugation of finite-index modular subgroups](#rational-conjugation-of-finite-index-modular-subgroups) gives a positive period for the translate, so boundedness gives a [removable singularity](isolated-singularity.md#removable-singularity) in its cusp parameter. Apply this to $\gamma\rho$ for every $\rho\in SL_2(\mathbb Z)$ to obtain holomorphy at every cusp of the new subgroup. Vanishing at the cusps is preserved too.

## Modular form

↑ **Parent:** [Modular function](modular-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_form)

A modular form is a [holomorphic function](complex-analysis.md#holomorphic-function) on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) that transforms with a fixed weight under a [congruence subgroup](group-theory.md#congruence-subgroup) and is [holomorphic at every cusp](#holomorphic-at-a-cusp).

### Weight of a modular form

↑ **Parent:** [Modular form](#modular-form)

The modular [modular weight](#weight-of-a-modular-form) specifies the power $(cz+d)^k$ in a [modular form](#modular-form)'s transformation law. Multiplication adds [modular weights](#weight-of-a-modular-form). At level one, the central [matrix](vector-space.md#matrix) $-I$ excludes nonzero odd-weight forms; a [nebentypus character](#nebentypus-character) at higher level changes this condition to $\psi(-1)=(-1)^k$.

### Mellin continuation of a noncuspidal modular form

↑ **Parent:** [Modular form](#modular-form)

For a level-one [modular form](#modular-form) of positive even weight $k$ and constant coefficient $a_0$, put $I_f(s)=\int_1^\infty(f(iy)-a_0)y^{s-1}\,dy$. This is an [entire function](complex-analysis.md#entire-function). Splitting the [Mellin transform](analysis.md#mellin-transform) at one and using $f(iy)=i^k y^{-k}f(i/y)$ proves the displayed continuation of $(2\pi)^{-s}\Gamma(s)L(f,s)$. It obeys $\Lambda_f(s)=i^k\Lambda_f(k-s)$ and has possible simple [poles](isolated-singularity.md#pole) only at zero and $k$, with residues $-a_0,i^ka_0$. For a [cusp form](#cusp-form) both disappear.

### Dimension of level-one modular forms

↑ **Parent:** [Modular form](#modular-form)

For even nonnegative weight, the displayed dimension follows from [multiplication by the modular discriminant](#multiplication-by-the-modular-discriminant) and the constant-coefficient map. Every nonnegative even weight except two has a product $E_4^aE_6^b$ of [Eisenstein series](#eisenstein-series) with constant term one, so $\dim M_k=1+\dim M_{k-12}$ for even $k\geq4$. The initial dimensions are one in weight zero and zero in weight two; negative and odd weights have no nonzero level-one [modular forms](#modular-form).

#### Polynomial ring of level-one modular forms

↑ **Parent:** [Dimension of level-one modular forms](#dimension-of-level-one-modular-forms)

Subtract the constant term of a [modular form](#modular-form) times a same-weight monomial in $E_4,E_6$. The remainder is a [cusp form](#cusp-form), hence divisible by the [modular discriminant](#modular-discriminant). Induction on weight and $1728\Delta=E_4^3-E_6^2$ express every form as a weighted homogeneous polynomial in these two [Eisenstein series](#eisenstein-series). The number of monomials of a given weight equals the [dimension of level-one modular forms](#dimension-of-level-one-modular-forms), so they form a basis and the graded ring has no polynomial relation.

##### Graded weights separate analytic polynomial relations

↑ **Parent:** [Polynomial ring of level-one modular forms](#polynomial-ring-of-level-one-modular-forms)

Let $P_w(E_4,E_6)$ be weighted homogeneous of [modular weight](#weight-of-a-modular-form) $w$, and suppose $\sum_wP_w(z)=0$ as a [holomorphic function](complex-analysis.md#holomorphic-function). Apply the [modular group](#modular-group) [matrices](vector-space.md#matrix) $\begin{pmatrix}1&0\\n&1\end{pmatrix}$. At a fixed point $z$ in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), this gives $\sum_w(nz+1)^wP_w(z)=0$ for every integer $n$. A [polynomial](polynomial.md) with infinitely many roots vanishes identically, so every $P_w(z)=0$. Within one [modular weight](#weight-of-a-modular-form), the monomials reduce to powers of $E_4^3/E_6^2$, after taking out a common factor. This ratio is nonconstant, as its [Fourier expansion](fourier-series.md) begins $1+1728q+\cdots$, so its powers are linearly independent. This proves [algebraic independence](algebra.md#algebraic-independence) even when the generators are regarded as analytic functions rather than elements of a formal [graded ring](commutative-algebra.md#graded-ring).

##### Rational structure of level-one modular forms

↑ **Parent:** [Polynomial ring of level-one modular forms](#polynomial-ring-of-level-one-modular-forms)

A level-one [modular form](#modular-form) with rational [Fourier coefficients](fourier-series.md#fourier-coefficient) is a weighted homogeneous polynomial with rational coefficients in the normalized [Eisenstein series](#eisenstein-series) $E_4,E_6$. Subtract its constant coefficient times a same-weight monomial. The remainder is a [cusp form](#cusp-form); divide it by $\Delta_0=(E_4^3-E_6^2)/1728=q+O(q^2)$. The [valence formula for the modular group](#valence-formula-for-the-modular-group) shows that $\Delta_0$ has no interior zeros, so this quotient is holomorphic and has rational coefficients. Induction on weight proves the assertion. Euler's [Bernoulli number](number-theory.md#bernoulli-number) formula for even zeta values then gives the corresponding rational weighted polynomial in the unnormalized [lattice Eisenstein sums](#lattice-eisenstein-sum) $G_4,G_6$.

<h3 id="modular-forms-as-meromorphic-differentials-on-x-1">Modular forms as meromorphic differentials on X(1)</h3>

↑ **Parent:** [Modular form](#modular-form)

A weight-$2k$ [modular form](#modular-form) descends as an invariant tensor differential. At an elliptic point of order $e$, a local invariant coordinate is $w=u^e$, so its descended coefficient has a pole of order at most $\lfloor k(e-1)/e\rfloor$. At infinity, $d\tau=dq/(2\pi iq)$ gives a pole of order at most $k$. Thus $D=k[\infty]+\lfloor k/2\rfloor[i]+\lfloor2k/3\rfloor[\rho]$ bounds the poles. Conversely these bounds give holomorphic pullbacks. The [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) on the compactified modular curve proves finite-dimensionality; since $X(1)$ is the [Riemann sphere](complex-analysis.md#riemann-sphere), the dimension is $\max(0,1-k+\lfloor k/2\rfloor+\lfloor2k/3\rfloor)$.

### Integral triangular basis of level-one modular forms

↑ **Parent:** [Modular form](#modular-form)

Choose $4a_j+6b_j=k-12j$ with nonnegative exponents, for every $j$ with $k-12j\ge0$ and $k-12j\ne2$. The [Eisenstein series](#eisenstein-series) and the [modular discriminant](#modular-discriminant) give [modular forms](#modular-form) with integer coefficients and distinct first powers of $q$. The [valence formula for the modular group](#valence-formula-for-the-modular-group) shows that these form a basis. Successively subtracting their leading terms proves that integral coefficients up to the greatest such $j$ force all coefficients to be integral. This is more precise than merely spanning by arbitrary monomials in $E_4,E_6$.

### Modular form on a finite-index subgroup

↑ **Parent:** [Modular form](#modular-form)

A [modular form](#modular-form) on an arbitrary [finite-index subgroup](group.md#finite-index-subgroup) $\Gamma\leq SL_2(\mathbb Z)$ is a [holomorphic function](complex-analysis.md#holomorphic-function) on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), invariant under the weight-$k$ [slash operator for modular forms](#slash-operator-for-modular-forms), and [holomorphic at a cusp](#holomorphic-at-a-cusp) at every [cusp of a modular group](#cusp-of-a-modular-group) for $\Gamma$. If $\sigma\in SL_2(\mathbb Z)$ maps infinity to a cusp, choose a genuine translation period $h>0$ with $\sigma T^h\sigma^{-1}\in\Gamma$. Then $f|_k\sigma$ has a convergent series in $e^{2\pi iz/h}$ with nonnegative exponents. A [cusp form](#cusp-form) has zero constant term at every cusp. This definition allows noncongruence subgroups and avoids sign ambiguities in odd weights when a smaller width is defined only modulo the center.

#### Nebentypus character

↑ **Parent:** [Modular form on a finite-index subgroup](#modular-form-on-a-finite-index-subgroup)

A [Dirichlet character](algebraic-number-theory.md#dirichlet-character) $\psi$ modulo $N$ specifying the displayed transformation law is the [nebentypus](#nebentypus-character) of a [modular form](#modular-form). The action of $-I$ forces $\psi(-1)=(-1)^k$ for a nonzero form. It describes a character eigenspace of the diamond action rather than an additional analytic condition at [modular cusps](#cusp-of-a-modular-group).

#### Coset norm of a modular form

↑ **Parent:** [Modular form on a finite-index subgroup](#modular-form-on-a-finite-index-subgroup)

For a finite-index inclusion of modular groups and a form with trivial multiplier, multiply its [slash operator for modular forms](#slash-operator-for-modular-forms) translates over left coset representatives. Right multiplication permutes the factors, producing a form of weight $k[\Gamma':\Gamma]$ for the larger group. [modular cusp](#cusp-of-a-modular-group) [cusp widths](#width-of-a-cusp) determine the orders contributed by the factors; the product is nonzero if the original form is nonzero.

### Serre derivative

↑ **Parent:** [Modular form](#modular-form)

The Serre derivative sends a level-one weight-$k$ [modular form](#modular-form) to weight $k+2$. Differentiating $f(-1/z)=z^kf(z)$ produces the extra term $kz^{k+1}f/(2\pi i)$; the anomalous transformation of the [Eisenstein series of weight two](#eisenstein-series-of-weight-two) cancels it. Translation invariance and the [Fourier expansion of a modular form](#fourier-expansion-of-a-modular-form) verify the remaining holomorphy conditions. For $k>0$, its constant coefficient is $-ka_0(f)/12$, so it is a [cusp form](#cusp-form) exactly when $f$ is.

#### First Rankin-Cohen bracket

↑ **Parent:** [Serre derivative](#serre-derivative)

For [modular forms](#modular-form) $f,g$ of weights $k,\ell$, respectively, the displayed combination cancels the anomaly in [derivative transformation of a weak modular form](#derivative-transformation-of-a-weak-modular-form) and is a weight-$k+\ell+2$ [cusp form](#cusp-form). Equivalently, for weights $k,\ell$ in the order $f,g$, a conventional first bracket is $k fDg-\ell gDf$; its negative is equally modular. Differentiation kills each constant [Fourier coefficient](fourier-series.md#fourier-coefficient), proving cusp vanishing.

### Oldform by argument dilation

↑ **Parent:** [Modular form](#modular-form)

If $N_1D\mid N$ and $f\in M_k(\Gamma_0(N_1))$, then $f(Dz)\in M_k(\Gamma_0(N))$. Conjugating by $\operatorname{diag}(D,1)$ changes a lower-left matrix entry $c$ to $c/D$, which is divisible by $N_1$. A rational upper-triangular factorization at every cusp preserves boundedness and hence cusp holomorphy.

#### Prime stabilization of an oldform

↑ **Parent:** [Oldform by argument dilation](#oldform-by-argument-dilation)

For a nonzero positive-weight eigenform at a good prime, the two oldforms $f(\tau),f(p\tau)$ are independent. At level multiplied by $p$, the [Hecke operator](#hecke-operator) is the bad-prime operator, with [matrix](vector-space.md#matrix) $\begin{pmatrix}\lambda&1\\-\chi(p)p^{k-1}&0\end{pmatrix}$. Distinct roots $\alpha,\beta$ of its [characteristic polynomial](linear-operator-theory.md#characteristic-polynomial) give eigenforms $f-\beta f(p\tau)$ and $f-\alpha f(p\tau)$. Weight-zero constants are an exception to the independence assertion.

#### Weight-four modular forms on Gamma 0 3

↑ **Parent:** [Oldform by argument dilation](#oldform-by-argument-dilation)

The group $\Gamma_0(3)$ has index four. The [dimension bound for modular forms on a finite-index subgroup](#dimension-bound-for-modular-forms-on-a-finite-index-subgroup) gives dimension at most two in weight four. The [Eisenstein series](#eisenstein-series) $E_4(z)$ and its [oldform by argument dilation](#oldform-by-argument-dilation) $E_4(3z)$ are independent, since their constant coefficients agree while their $q$ coefficients are $240$ and zero.

### Weak modular form

↑ **Parent:** [Modular form](#modular-form)

Here a weak modular form is a [holomorphic function](complex-analysis.md#holomorphic-function) on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) satisfying the weight-$k$ transformation law, with no growth condition at any [cusp of a modular group](#cusp-of-a-modular-group). This convention differs from weakly holomorphic modular forms, which are required to be meromorphic at the cusps. At level one, translation invariance gives a Laurent expansion on the punctured unit disc, possibly with infinitely many negative powers.

#### Derivative transformation of a weak modular form

↑ **Parent:** [Weak modular form](#weak-modular-form)

For a weight-$k$ [weak modular form](#weak-modular-form) of level one,

$$
f^{(\ell)}(-1/z)=\sum_{j=0}^{\ell}\binom\ell j(k+j)_{\ell-j}z^{k+\ell+j}f^{(j)}(z),
$$

where $(a)_r=a(a+1)\cdots(a+r-1)$ and $(a)_0=1$. Differentiate and multiply by $z^2$ to obtain the coefficient recurrence $C_{\ell+1,j}=(k+\ell+j)C_{\ell,j}+C_{\ell,j-1}$.

##### Bol identity for modular forms

↑ **Parent:** [Derivative transformation of a weak modular form](#derivative-transformation-of-a-weak-modular-form)

For integer $k<0$, the operator $D=(2\pi i)^{-1}d/dz=q\,d/dq$ sends a weight-$k$ level-one [weak modular form](#weak-modular-form) to a weight-$2-k$ one after $1-k$ iterations. In the [derivative transformation of a weak modular form](#derivative-transformation-of-a-weak-modular-form), every lower derivative coefficient then contains a zero factor. This also holds on the subspace $M_k^!$ of forms meromorphic at the cusp.

### Fricke involution

↑ **Parent:** [Modular form](#modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fricke_involution)

The Fricke matrix $W_N=\begin{pmatrix}0&-1\\N&0\end{pmatrix}$ normalizes $\Gamma_1(N)$ and $\Gamma_0(N)$ under the appropriate determinant-normalized slash action. It exchanges the cusps zero and infinity.

#### Fricke sign from a nonvanishing fixed-point value

↑ **Parent:** [Fricke involution](#fricke-involution)

If a one-dimensional [modular cusp](#cusp-of-a-modular-group) space is stable under the phase-normalized [Fricke involution](#fricke-involution), its scalar action is determined by evaluation at the fixed point. The phase-normalized prefactor is one there; if the form is nonzero at that point, the [eigenvalue](linear-operator-theory.md#eigenvalue) is $+1$. A product with strictly positive convergent factors on the imaginary axis supplies such a value and also makes the central completed [L-function of a cusp form](#l-function-of-a-cusp-form) positive when its central Mellin integral has real positive kernel.

### Modular group

↑ **Parent:** [Modular form](#modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_group)

The modular group is $SL_2(\mathbb Z)$ acting on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). Its central element $-I$ acts trivially on points but contributes the factor $(-1)^k$ in weight $k$.

#### Modular-invariant function

↑ **Parent:** [Modular group](#modular-group)

A function on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) is modular invariant if it is unchanged by the fractional-linear action of the [modular group](#modular-group). This does not imply holomorphicity: a [nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series) is modular invariant, whereas a [modular function](modular-function.md) additionally satisfies meromorphicity and cusp conditions.

#### Rational conjugation of finite-index modular subgroups

↑ **Parent:** [Modular group](#modular-group)

For any [finite-index subgroup](group.md#finite-index-subgroup) $\Gamma\leq SL_2(\mathbb Z)$ and rational positive-determinant $\gamma$, the intersection $SL_2(\mathbb Z)\cap\gamma^{-1}\Gamma\gamma$ has finite index. Multiply $\gamma$ by a positive rational scalar to obtain an integral [matrix](vector-space.md#matrix) $A$ with positive integer [determinant](linear-algebra.md#determinant) $D$. For $h=I+DB\in\Gamma(D)$, $AhA^{-1}=I+AB\operatorname{adj}(A)$ is integral, so $\Gamma(D)$ lies in $SL_2(\mathbb Z)\cap\gamma^{-1}SL_2(\mathbb Z)\gamma$. This intersection has finite index. Its further intersection with $\gamma^{-1}\Gamma\gamma$ has relative index at most $[SL_2(\mathbb Z):\Gamma]$. No assumption that $\Gamma$ itself is a [congruence subgroup](group-theory.md#congruence-subgroup) is needed.

#### Standard fundamental domain of the modular group

↑ **Parent:** [Modular group](#modular-group)

The standard fundamental domain is

$$
\mathcal F=\{\tau\in\mathfrak h:|\tau|\geq1,\ -1/2\leq\operatorname{Re}\tau\leq1/2\}.
$$

Every orbit of the modular group meets $\mathcal F$.

##### Fundamental region of a modular subgroup

↑ **Parent:** [Standard fundamental domain of the modular group](#standard-fundamental-domain-of-the-modular-group)

For a finite-index [subgroup](group.md#subgroup) of the [modular group](#modular-group), take the union of translates of the [standard fundamental domain of the modular group](#standard-fundamental-domain-of-the-modular-group) over left coset representatives. Boundary identifications are inherited from the [subgroup](group.md#subgroup) action. The truncated region is compact, and its finitely many cusp ends have exponential parameters; this proves compactness of the [compactified modular curve](#compactified-modular-curve) and boundedness of invariant cusp-form norms.

##### Elliptic stabilizers of the modular group

↑ **Parent:** [Standard fundamental domain of the modular group](#standard-fundamental-domain-of-the-modular-group)

For the boundary convention $-1/2<\operatorname{Re}z\leq1/2$, retaining only the right half of the unit circle, the exceptional points are $i$ and $\rho_+=e^{i\pi/3}$. Their stabilizers in $SL_2(\mathbb Z)$ are the cyclic groups generated by $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and $\begin{pmatrix}1&-1\\1&0\end{pmatrix}$, of orders four and six. Every other stabilizer is $\{I,-I\}$.

##### Reduction to the standard modular region

↑ **Parent:** [Standard fundamental domain of the modular group](#standard-fundamental-domain-of-the-modular-group)

Given $\tau\in\mathfrak h$, choose a primitive pair $(c,d)$ minimizing $|c\tau+d|$ and apply a modular matrix with bottom row $(c,d)$. This maximizes the imaginary part within the orbit. Translation puts the real part in $[-1/2,1/2]$, and inversion then shows that the imaginary part is at least $\sqrt3/2$.

### Slash operator for modular forms

↑ **Parent:** [Modular form](#modular-form)

For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, the weight-$k$ slash operator is

$$
(f|_k\gamma)(\tau)=(c\tau+d)^{-k}f(\gamma\tau).
$$

A modular form of weight $k$ and level $\Gamma$ satisfies $f|_k\gamma=f$ for every $\gamma\in\Gamma$.

#### Double-coset operator on modular forms

↑ **Parent:** [Slash operator for modular forms](#slash-operator-for-modular-forms)

Decompose $A\alpha B=\coprod_j A\alpha_j$ for finite-index congruence subgroups $A,B$. The sum is independent of representative choices because $f$ is invariant under $A$. Right multiplication by $B$ permutes these left cosets, so the sum is invariant under $B$. Each summand is holomorphic in the half-plane; [cusp holomorphy under rational slash operators](#cusp-holomorphy-under-rational-slash-operators) proves holomorphy at every new cusp. The same reasoning preserves vanishing at cusps. With the [Hecke-normalized rational slash operator](#hecke-normalized-rational-slash-operator), no extra scalar is needed in the defining sum.

#### Hecke-normalized rational slash operator

↑ **Parent:** [Slash operator for modular forms](#slash-operator-for-modular-forms)

For a rational [matrix](vector-space.md#matrix) of positive determinant, this slash normalization differs from the [determinant-normalized slash operator](#determinant-normalized-slash-operator) by $(\det\alpha)^{k/2-1}$. Both are right actions, by the [automorphy factor](#automorphy-factor) identity. For a positive scalar $t$, the displayed action of $tI$ is multiplication by $t^{k-2}$. On determinant-one matrices it agrees with the ordinary [slash operator for modular forms](#slash-operator-for-modular-forms). This normalization makes a good-prime [Hecke operator](#hecke-operator) a plain sum over its double-coset representatives.

#### Determinant-normalized slash operator

↑ **Parent:** [Slash operator for modular forms](#slash-operator-for-modular-forms)

For a rational [matrix](vector-space.md#matrix) $\gamma$ of positive [determinant](linear-algebra.md#determinant), use the positive real power of $\det\gamma$ in the displayed [slash operator for modular forms](#slash-operator-for-modular-forms). It satisfies $(f|_k\gamma)|_k\eta=f|_k(\gamma\eta)$ by the [automorphy factor](#automorphy-factor) identity and multiplicativity of the [determinant](linear-algebra.md#determinant). It agrees with the usual operator on the [modular group](#modular-group). The determinant factor is essential for the stated normalization of the [Hecke operators](#hecke-operator).

#### Automorphy factor

↑ **Parent:** [Slash operator for modular forms](#slash-operator-for-modular-forms)

For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, the automorphy factor is $j(\gamma,\tau)=c\tau+d$. It obeys the cocycle identity

$$
j(\gamma\delta,\tau)=j(\gamma,\delta\tau)j(\delta,\tau).
$$

### Fourier expansion of a modular form

↑ **Parent:** [Modular form](#modular-form)

Translation invariance at a cusp gives a Fourier expansion in its local parameter $q$. Holomorphy at the cusp excludes negative powers; vanishing of the constant term defines a cusp form.

#### Cusp form

↑ **Parent:** [Fourier expansion of a modular form](#fourier-expansion-of-a-modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cusp_form)

A cusp form is a modular form that vanishes at every cusp. At the cusp at infinity for the full modular group it has an expansion $\sum_{n\geq1}a_nq^n$.

##### Old subspace of cusp forms

↑ **Parent:** [Cusp form](#cusp-form)

The old subspace is spanned by $h(tz)$ for [cusp forms](#cusp-form) $h$ of level $M<N$, where $M\mid N$ and $t\mid N/M$. It is stable under the [Hecke operators](#hecke-operator), but need not have a basis of eigenvectors for every bad-prime operator. Its [Petersson inner product](#petersson-inner-product) [orthogonal complement](hilbert-space.md#orthogonal-complement) is the [new subspace of cusp forms](#new-subspace-of-cusp-forms).

###### Degeneracy map for cusp forms

↑ **Parent:** [Old subspace of cusp forms](#old-subspace-of-cusp-forms)

If $M\mid N$ and $D\mid N/M$, conjugating $\Gamma_0(N)$ by $\operatorname{diag}(D,1)$ gives matrices $\begin{pmatrix}a&Db\\c/D&d\end{pmatrix}$ in $\Gamma_0(M)$. This proves the weight transformation of $f(D\tau)$. At any rational [modular cusp](#cusp-of-a-modular-group), factor the rational change of variable into an integral cusp representative followed by an upper-triangular rational matrix of positive slope. The original cusp expansion then stays holomorphic and has zero constant term. Thus this map takes [cusp forms](#cusp-form) of level $M$ to those of level $N$.

###### Prime-level cusp orders of discriminant degeneracy forms

↑ **Parent:** [Degeneracy map for cusp forms](#degeneracy-map-for-cusp-forms)

For prime $p$, the two cusps of $\Gamma_0(p)$ have widths one and $p$. At infinity the [modular discriminant](#modular-discriminant) product gives the first pair of orders. At zero use $S\tau=-1/\tau$ and the parameter $q_0=e^{2\pi i\tau/p}$. The weight-twelve transforms are $\Delta|_{12}S=\Delta(\tau)$ and $\Delta(p\tau)|_{12}S=p^{-12}\Delta(\tau/p)$, giving orders $p$ and one in $q_0$.

###### Prime-power old block at a bad prime

↑ **Parent:** [Old subspace of cusp forms](#old-subspace-of-cusp-forms)

If $p$ divides the primitive level $M$ of a trivial-character [newform](#newform) and $N=Mp^r$, put $e_j=p^{jk/2}f(p^jz)$. Then $U_pe_0=a_pe_0$ and $U_pe_j=p^{k/2}e_{j-1}$ for $j\ge1$. The normalized [Fricke involution](#fricke-involution) acts by $e_j\mapsto\varepsilon e_{r-j}$, where $W_Mf=\varepsilon f$. These two operators act irreducibly: a nonzero invariant subspace contains an eigenvector of $U_p$; its eigenvalue is $a_p$ or zero. Either it contains $e_0$ immediately or applying the reversal and a power of $U_p$ produces $e_0$, using $a_p^2\ne p^k$. Reversal then produces $e_r$, and its successive images produce every basis vector.

##### New subspace of cusp forms

↑ **Parent:** [Cusp form](#cusp-form)

The new subspace is the [orthogonal complement](hilbert-space.md#orthogonal-complement) of the [old subspace of cusp forms](#old-subspace-of-cusp-forms) for the [Petersson inner product](#petersson-inner-product). A form belongs to it precisely when the adjoints of all lower-level [oldform by argument dilation](#oldform-by-argument-dilation) maps annihilate it.

###### Newform

↑ **Parent:** [New subspace of cusp forms](#new-subspace-of-cusp-forms)

A newform is a normalized [Hecke eigenform](#hecke-eigenform) in the [new subspace of cusp forms](#new-subspace-of-cusp-forms). Its weight, level and [Dirichlet character](algebraic-number-theory.md#dirichlet-character) are part of its specification. For a [newform](#newform), its [Fourier coefficients](fourier-series.md#fourier-coefficient) equal its [eigenvalues](linear-operator-theory.md#eigenvalue) of [Hecke operators](#hecke-operator).

###### Bad-prime eigenvalue of a trivial-character newform

↑ **Parent:** [Newform](#newform)

For a [newform](#newform) of weight $k\ge2$, level $M$ and trivial [Dirichlet character](algebraic-number-theory.md#dirichlet-character), the bad-prime [Hecke operator](#hecke-operator) $U_p$ has the displayed possibilities. The local trace relation on the [new subspace of cusp forms](#new-subspace-of-cusp-forms) gives $U_p=-p^{k/2-1}W_p$ when $p\parallel M$, where the normalized local Atkin-Lehner operator squares to one; if $p^2\mid M$, the new-vector relation gives $U_p=0$. In particular $|a_p|<p^{k/2}$, a strict inequality useful for proving irreducibility of old blocks.

###### Newform multiplicity-one theorem

↑ **Parent:** [Newform](#newform)

On the [new subspace of cusp forms](#new-subspace-of-cusp-forms), a common [eigenspace](linear-operator-theory.md#eigenspace) for the [Hecke operators](#hecke-operator) away from the level has dimension one. Distinct [newforms](#newform), even at different primitive levels, have different systems of these [eigenvalues](linear-operator-theory.md#eigenvalue). Consequently the commuting bad-prime operators also act by scalars on these lines. This is the multiplicity-one part of Atkin-Lehner-Li theory, not a consequence of [normal operator](hilbert-space.md#normal-operator) diagonalization alone. See [Stein's statement of the theorem](https://wstein.org/books/modform/modform/newforms.html#atkin-lehner-li-theory).

##### L-function of a cusp form

↑ **Parent:** [Cusp form](#cusp-form)

For $f=\sum_{n\geq1}a_nq^n$, define $L(f,s)=\sum_{n\geq1}a_nn^{-s}$ in a right half-plane. Its completion $(2\pi)^{-s}\Gamma(s)L(f,s)$ is the [Mellin transform](analysis.md#mellin-transform) of $f(iy)$. The modular inversion and exponential cusp decay continue this completion to an entire function and give its reflection $s\mapsto k-s$. A normalized [Hecke eigenform](#hecke-eigenform) also has an [Euler product of a Hecke eigenform](#euler-product-of-a-hecke-eigenform).

###### Additive twist of a cusp-form L-function

↑ **Parent:** [L-function of a cusp form](#l-function-of-a-cusp-form)

For a [cusp form](#cusp-form) $f=\sum c_nq^n$ and coprime integers $a,N$, the additive twist inserts the additive character $e^{2\pi ian/N}$. It is the [Dirichlet series](analytic-number-theory.md#dirichlet-series) associated with the rational translate $f(a/N+\tau)$. Its completed [Mellin transform](analysis.md#mellin-transform) uses the scale $N^s$ and the [Gamma function](complex-analysis.md#gamma-function).

###### Functional equation of an additive cusp-form twist

↑ **Parent:** [Additive twist of a cusp-form L-function](#additive-twist-of-a-cusp-form-l-function)

For even weight $k$, complete the [additive twist of a cusp-form L-function](#additive-twist-of-a-cusp-form-l-function) as $M(f,a/N,s)=(N/(2\pi))^s\Gamma(s)L(f,a/N,s)$. Split its [Mellin transform](analysis.md#mellin-transform) at $y=1/N$ and use [rational-cusp inversion of a level-one cusp form](#rational-cusp-inversion-of-a-level-one-cusp-form) in the lower integral. The resulting two integrals over $[1/N,\infty)$ converge locally uniformly for every complex $s$, giving an entire continuation and the displayed [functional equation](analysis.md#functional-equation). The relation $ad\equiv1\pmod N$ identifies the opposite cusp.

###### Rational-cusp inversion of a level-one cusp form

↑ **Parent:** [Additive twist of a cusp-form L-function](#additive-twist-of-a-cusp-form-l-function)

If $ad\equiv1\pmod N$, the determinant-one [matrix](vector-space.md#matrix) with rows $(a,(ad-1)/N)$ and $(N,d)$ sends $\tau-d/N$ to $a/N-1/(N^2\tau)$. The transformation of the [cusp form](#cusp-form) gives the displayed identity. It turns the small-height portion of an additive-twist [Mellin transform](analysis.md#mellin-transform) into exponentially decaying values at the inverse rational cusp.

##### Character twist by rational translations of a cusp form

↑ **Parent:** [Cusp form](#cusp-form)

For a level-one [cusp form](#cusp-form) and any [Dirichlet character](algebraic-number-theory.md#dirichlet-character) modulo $N>1$, this translation sum is a [cusp form](#cusp-form) on $\Gamma_1(N)\cap\Gamma_0(N^2)$. Conjugating that subgroup by $\begin{pmatrix}1&j/N\\0&1\end{pmatrix}$ yields integral determinant-one [matrices](vector-space.md#matrix); [cusp holomorphy under rational slash operators](#cusp-holomorphy-under-rational-slash-operators) supplies all cusp conditions. Its exact [Fourier coefficients](fourier-series.md#fourier-coefficient) at positive indices are $a_n(f)\sum_{j\in(\mathbb Z/N\mathbb Z)^\times}\chi(j)^{-1}e^{2\pi inj/N}$. For a [primitive Dirichlet character](algebraic-number-theory.md#primitive-dirichlet-character) they equal $g(\overline\chi)\chi(n)a_n(f)$, by the [finite Fourier transform of a primitive Dirichlet character](algebraic-number-theory.md#finite-fourier-transform-of-a-primitive-dirichlet-character). For imprimitive characters the sum can be nonzero at nonunits, so the simplified twist formula need not hold.

###### Primitive twist at coprime level

↑ **Parent:** [Character twist by rational translations of a cusp form](#character-twist-by-rational-translations-of-a-cusp-form)

For a [primitive Dirichlet character](algebraic-number-theory.md#primitive-dirichlet-character) $\chi$ modulo $D$, its [Gauss sum of a Dirichlet character](algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) gives $f_\chi=\tau(\overline\chi)^{-1}\sum_u\overline\chi(u)f|U_u$, with $U_u=\begin{pmatrix}1&u/D\\0&1\end{pmatrix}$. If $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(ND^2)$, take $v\equiv d^2u\pmod D$. Then $U_u\gamma U_v^{-1}\in\Gamma_0(N)$ and its lower-right entry is congruent to $d$ modulo $N$. Reindexing the sum yields the character $\psi(d)\chi(d)^2$. Rational translations preserve vanishing at [modular cusps](#cusp-of-a-modular-group), proving the stated cuspidality as well as the transformation law.

###### Fricke transform of a primitive coprime twist

↑ **Parent:** [Primitive twist at coprime level](#primitive-twist-at-coprime-level)

Use the [determinant-normalized slash operator](#determinant-normalized-slash-operator) and $W_M=\begin{pmatrix}0&-1\\M&0\end{pmatrix}$. For units $u,v$ with $Nuv\equiv-1\pmod D$, the [matrix](vector-space.md#matrix) identity $U_uW_{ND^2}=D\gamma_uW_NU_v$ has $\gamma_u=\begin{pmatrix}(1+Nuv)/D&u\\Nv&D\end{pmatrix}\in\Gamma_0(N)$. A positive scalar [matrix](vector-space.md#matrix) acts trivially. The [nebentypus](#nebentypus-character) supplies $\psi(D)$; reindexing gives $\overline\chi(u)=\chi(-N)\chi(v)$. Thus the factor is initially $\psi(D)\chi(-N)\tau(\chi)/\tau(\overline\chi)$. The primitive [Gauss sum of a Dirichlet character](algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) identity $\tau(\chi)\tau(\overline\chi)=\chi(-1)D$ gives the displayed equivalent factor. No assumption that $f$ itself is a Fricke eigenform is needed.

##### Invariant norm of a modular form

↑ **Parent:** [Cusp form](#cusp-form)

For a weight-$k$ modular form on the full modular group, the quantity

$$
(\operatorname{Im}\tau)^{k/2}|f(\tau)|
$$

is modular invariant. For a cusp form it tends to zero at the cusp and is therefore bounded on a fundamental domain.

###### Bounded invariant norm characterization of cusp forms

↑ **Parent:** [Invariant norm of a modular form](#invariant-norm-of-a-modular-form)

For $k>0$, a meromorphic function satisfying the modular transformation law is a [cusp form](#cusp-form) exactly when its invariant norm is bounded. The bound first excludes interior poles. At each cusp a genuine periodic slash translate is bounded by $Cy^{-k/2}$, which tends to zero. Its punctured-disk expression therefore has a removable singularity with zero value. Conversely cusp Fourier expansions decay exponentially, and finitely many compact core regions control the rest. Positive weight is essential: a nonzero constant in weight zero satisfies the bound but is not a cusp form.

###### Fourier coefficient bound for a cusp form

↑ **Parent:** [Invariant norm of a modular form](#invariant-norm-of-a-modular-form)

If $f(\tau)=\sum_{n\geq1}a_nq^n$ is a weight-$k$ level-one cusp form, boundedness of its [invariant norm](#invariant-norm-of-a-modular-form) gives

$$
|a_n|=O(n^{k/2}).
$$

Integrate $f(x+iy)e^{-2\pi inx}$ over one period and choose $y=1/n$.

##### Fourier coefficient growth criterion for a level-one cusp form

↑ **Parent:** [Cusp form](#cusp-form)

Let even $k\geq4$ and let $g(\tau)=\sum_{n\geq0}b_nq^n$ be a level-one modular form of weight $k$. If $b_n=O(n^{k/2})$, then $b_0=0$ and $g$ is a cusp form. Otherwise subtract the matching Eisenstein series; its coefficients grow like $\sigma_{k-1}(n)$, contradicting the bound at prime indices.

##### Dimension of level-one cusp forms

↑ **Parent:** [Cusp form](#cusp-form)

For even $k\geq12$,

$$
\dim S_k(\Gamma(1))=
\begin{cases}
\lfloor k/12\rfloor-1,&k\equiv2\pmod{12},\\
\lfloor k/12\rfloor,&k\not\equiv2\pmod{12}.
\end{cases}
$$

The dimension is zero for odd $k$ and for $k<12$.

##### Mellin transform of a cusp-form L-function

↑ **Parent:** [Cusp form](#cusp-form)

For $f(\tau)=\sum_{n\geq1}a_nq^n$, termwise integration initially gives

$$
(2\pi)^{-s}\Gamma(s)L(f,s)
=\int_0^\infty f(iy)y^{s-1}\,dy.
$$

A Fricke transformation converts the behavior near zero into cusp decay at infinity, giving analytic continuation and a functional equation for the completed L-function.

###### Phase-normalized Fricke functional equation

↑ **Parent:** [Mellin transform of a cusp-form L-function](#mellin-transform-of-a-cusp-form-l-function)

With the [determinant-normalized slash operator](#determinant-normalized-slash-operator), the map $Jf=i^kf|_kW_N$ satisfies $J^2=1$. The scaled imaginary-axis functions satisfy $F(y)=y^{-k}G(1/y)$, and their [Mellin transforms](analysis.md#mellin-transform) give the displayed entire functional equation. The phase must be specified; omitting it changes the sign in odd or twice-odd weights.

##### Modular discriminant

↑ **Parent:** [Cusp form](#cusp-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_discriminant)

The modular discriminant is the normalized weight-twelve level-one cusp form

$$
\Delta(\tau)=q\prod_{n\geq1}(1-q^n)^{24}.
$$

###### Multiplication by the modular discriminant

↑ **Parent:** [Modular discriminant](#modular-discriminant)

The [modular discriminant](#modular-discriminant) has a simple zero at infinity and no zero in the [upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), by the [valence formula for the modular group](#valence-formula-for-the-modular-group). Multiplication by it identifies weight-$k$ [modular forms](#modular-form) with weight-$(k+12)$ [cusp forms](#cusp-form). Conversely dividing a cusp form by it preserves interior holomorphy and removes one order of vanishing at infinity.

###### Weight-two discriminant root at level eleven

↑ **Parent:** [Modular discriminant](#modular-discriminant)

The effective group $\Gamma_0(11)$ is torsion-free, has index twelve and has two regular cusps. If its weight-two [cusp form](#cusp-form) space is one-dimensional, any nonzero member has order one at each cusp and no interior zeros by the [regular-cusp valence formula on a torsion-free modular curve](#regular-cusp-valence-formula-on-a-torsion-free-modular-curve). Its twelfth power and $\Delta(\tau)\Delta(11\tau)$ have the same weight and divisor. Their ratio is a holomorphic function without poles on the [compactified modular curve](#compactified-modular-curve), hence a nonzero constant. Normalizing the leading Fourier coefficient to one proves the displayed formula, with the holomorphic root chosen to start with $q$. It equals $q\prod_{n\geq1}(1-q^n)^2(1-q^{11n})^2$.

###### Integrality identity for the modular discriminant

↑ **Parent:** [Modular discriminant](#modular-discriminant)

Put $S_j=\sum_{n\geq1}\sigma_j(n)q^n$. Expanding $E_4=1+240S_3$ and $E_6=1-504S_5$ gives $\Delta=(5S_3+7S_5)/12+100S_3^2+8000S_3^3-147S_5^2$. For every integer $d$, $5d^3+7d^5$ is divisible by twelve, by separate congruences modulo three and four. Consequently every coefficient of the [modular discriminant](#modular-discriminant) is integral, without using a product expansion.

###### Ramanujan tau function

↑ **Parent:** [Modular discriminant](#modular-discriminant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramanujan_tau_function)

The Ramanujan tau function gives the [Fourier coefficients](fourier-series.md#fourier-coefficient) at positive indices of the [modular discriminant](#modular-discriminant): $\Delta(z)=\sum_{n\geq1}\tau(n)q^n$, with $\tau(1)=1$. The [Serre derivative](#serre-derivative) and [vanishing of weight-fourteen level-one cusp forms](#vanishing-of-weight-fourteen-level-one-cusp-forms) give $q\,d\Delta/dq=E_2\Delta$ and hence the convolution recurrence

$$
(1-n)\tau(n)=24\sum_{r=1}^{n-1}\sigma_1(r)\tau(n-r).
$$

###### Ramanujan tau congruence modulo five

↑ **Parent:** [Ramanujan tau function](#ramanujan-tau-function)

The [modular discriminant](#modular-discriminant) satisfies $1728\Delta=E_4^3-E_6^2$, while the [Serre derivative](#serre-derivative) gives $2\Theta E_6=E_2E_6-E_4^2$. Their integral Fourier expansions have $E_4\equiv1$ and $E_2\equiv E_6\pmod5$, because $d^5\equiv d\pmod5$. Reducing the two identities gives $\Delta\equiv\Theta E_6\pmod5$. The coefficient of $q^n$ in $\Theta E_6$ is $-504n\sigma_5(n)\equiv n\sigma_5(n)$.

###### Ramanujan congruence modulo 691

↑ **Parent:** [Ramanujan tau function](#ramanujan-tau-function)

The [Fourier expansion of a normalized Eisenstein series](#fourier-expansion-of-a-normalized-eisenstein-series) and the one-dimensional weight-twelve [cusp form](#cusp-form) space give $691E_{12}=691E_4^3-432000\Delta$. The coefficient of $q^n$, for $n\geq1$, reduces modulo $691$ to $566\sigma_{11}(n)=566\tau(n)$. Since $566$ is invertible modulo $691$, this proves the congruence. Integrality follows from $E_4=1+240\sum\sigma_3(n)q^n$ and the product $\Delta=q\prod_{n\geq1}(1-q^n)^{24}$.

###### Mellin transform of the modular discriminant

↑ **Parent:** [Modular discriminant](#modular-discriminant)

For every real $s$, the rapidly convergent integral

$$
\int_0^\infty\Delta(it)t^{s-1}\,dt
$$

is the analytic continuation of $(2\pi)^{-s}\Gamma(s)L(\Delta,s)$. The product for $\Delta$ makes the integrand positive, so $L(\Delta,s)>0$ for real $s>0$.

##### Petersson inner product

↑ **Parent:** [Cusp form](#cusp-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Petersson_inner_product)

For weight-$k$ cusp forms on $\Gamma$, the Petersson inner product is

$$
\langle f,g\rangle=\int_{\Gamma\backslash\mathfrak h}f(\tau)\overline{g(\tau)}y^k\frac{dx\,dy}{y^2}.
$$

Cusp decay makes the integral convergent.

###### Hecke operators are self-adjoint for the Petersson inner product

↑ **Parent:** [Petersson inner product](#petersson-inner-product)

On level-one [cusp forms](#cusp-form), determinant-normalized [Hecke operators](#hecke-operator) satisfy $\langle T_nf,g\rangle=\langle f,T_ng\rangle$. Unfolding their finite correspondences transfers a matrix to its inverse; its adjugate has the same determinant and reverses the correspondence. Since these operators commute, the cusp space has a common [orthonormal basis](linear-algebra.md#orthonormal-basis) of [Hecke eigenforms](#hecke-eigenform), with real eigenvalues.

<h6 id="rankin-selberg-method">Rankin–Selberg method</h6>

↑ **Parent:** [Petersson inner product](#petersson-inner-product)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rankin–Selberg_method)

The Rankin–Selberg method represents Dirichlet series built from automorphic forms as integrals against Eisenstein series and studies them by unfolding those integrals.

<h6 id="rankin-selberg-integral-for-holomorphic-cusp-forms">Rankin–Selberg integral for holomorphic cusp forms</h6>

↑ **Parent:** [Rankin–Selberg method](#rankin-selberg-method)

For two weight-$k$ level-one [cusp forms](#cusp-form), use the [primitive real-analytic Eisenstein series](#primitive-real-analytic-eisenstein-series) and $d\mu=dx\,dy/y^2$. The [Rankin–Selberg unfolding](#rankin-selberg-method) identity is

$$
I(f,g,w)=\frac{\Gamma(w+k-1)}{(4\pi)^{w+k-1}}\sum_{n\geq1}\frac{a_n\overline{b_n}}{n^{w+k-1}}.
$$

Initially this follows by absolute convergence, unfolding to $0\leq x<1$, and integrating the [Fourier series](fourier-series.md) in $x$. Exponential cusp decay and polynomial growth of the [primitive real-analytic Eisenstein series](#primitive-real-analytic-eisenstein-series) make the integral [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) for $\operatorname{Re}w>1$, continuing the [Dirichlet series](analytic-number-theory.md#dirichlet-series) to $\operatorname{Re}s>k$.

###### Positive unfolding of a cusp-form square

↑ **Parent:** [Rankin–Selberg integral for holomorphic cusp forms](#rankin-selberg-integral-for-holomorphic-cusp-forms)

For real $w>1$, the finite [Rankin–Selberg integral](#rankin-selberg-integral-for-holomorphic-cusp-forms) $I(f,f,w)$ has a nonnegative integrand. [Tonelli theorem](measure-theory.md#tonelli-theorem) unfolds it without an a priori bound on the [Dirichlet series](analytic-number-theory.md#dirichlet-series). Integration over $x$ gives $\int_0^1|f(x+iy)|^2dx=\sum_{n\geq1}|a_n|^2e^{-4\pi ny}$. A second application of [Tonelli theorem](measure-theory.md#tonelli-theorem) gives the finite sum in the displayed identity with $s=w+k-1$. Positivity, rather than analytic continuation alone, proves absolute convergence.

###### Absolute convergence of cusp-form L-series from square coefficients

↑ **Parent:** [Positive unfolding of a cusp-form square](#positive-unfolding-of-a-cusp-form-square)

By [positive unfolding of a cusp-form square](#positive-unfolding-of-a-cusp-form-square), $\sum|a_n|^2n^{-\beta}<\infty$ for $\beta>k$. Choose $k<\beta<2\sigma-1$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds the absolute sum for the [L-function of a cusp form](#l-function-of-a-cusp-form) by

$$
\left(\sum_{n\geq1}|a_n|^2n^{-\beta}\right)^{1/2}\left(\sum_{n\geq1}n^{-(2\sigma-\beta)}\right)^{1/2}<\infty.
$$

<h6 id="rankin-selberg-convolution">Rankin–Selberg convolution</h6>

↑ **Parent:** [Rankin–Selberg method](#rankin-selberg-method)

For cusp forms $f=\sum a_nq^n$ and $g=\sum b_nq^n$, their Rankin–Selberg convolution in the elementary normalization is $L(f,g,s)=\sum_{n\geq1}a_n\overline{b_n}n^{-s}$.

###### Euler factor of a coefficientwise product of Hecke eigenforms

↑ **Parent:** [Rankin–Selberg convolution](#rankin-selberg-convolution)

For normalized level-one [Hecke eigenforms](#hecke-eigenform), let $\alpha_p+\beta_p=a_p$, $\alpha_p\beta_p=p^{k-1}$, and similarly $\gamma_p+\delta_p=b_p$, $\gamma_p\delta_p=p^{k-1}$. The [Hecke multiplication relations](#hecke-multiplication-relations) give $a_{p^r}=(\alpha_p^{r+1}-\beta_p^{r+1})/(\alpha_p-\beta_p)$, with the repeated-root case obtained by continuity. Multiplying the two expressions and summing four geometric series proves the displayed local factor. Multiplicativity gives an [Euler product](analytic-number-theory.md#euler-product); multiplying by $\zeta(2s-2k+2)$ cancels its local numerator and produces the degree-four convolution factors.

###### Zeta-completed Rankin-Selberg coefficient series

↑ **Parent:** [Rankin–Selberg convolution](#rankin-selberg-convolution)

For two level-one weight-$k$ [cusp forms](#cusp-form), $F(s)=\sum a_n\overline b_n n^{-s}$. Unfolding against the nonholomorphic lattice sum normalized by $\pi^{-w}\Gamma(w)$ gives the displayed completion as the integral of $f\overline g y^k$ against that [Eisenstein series](#eisenstein-series). Its [functional equation](analysis.md#functional-equation) is $\mathcal R(s)=\mathcal R(2k-1-s)$, and its only possible simple poles are at $k-1,k$. The raw series is obtained by dividing out the gamma and zeta factors, so it does not inherit the same unqualified pole statement; zeros of the denominator zeta factor can yield additional possible poles. The raw series is regular at $k-1$ and can have a simple pole at $k$.

<h6 id="rankin-selberg-unfolding-identity-for-a-holomorphic-eisenstein-series">Rankin–Selberg unfolding identity for a holomorphic Eisenstein series</h6>

↑ **Parent:** [Rankin–Selberg convolution](#rankin-selberg-convolution)

If $f$ and $g$ have respective weights $k$ and $l$, and $r=k-l>2$, unfolding the weight-$r$ Eisenstein series gives

$$
\langle f,gG_r\rangle
=\frac{2\zeta(r)\Gamma(k-1)}{(4\pi)^{k-1}}L(f,g,k-1).
$$

### Eisenstein series

↑ **Parent:** [Modular form](#modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eisenstein_series)

An Eisenstein series is a modular form constructed by summing a weight factor over a parabolic coset space. For even $k>2$, the level-one holomorphic Eisenstein series is a scalar multiple of $\sum_{(m,n)\ne(0,0)}(m\tau+n)^{-k}$.

#### Lattice Eisenstein sum

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For a [period lattice](complex-analysis.md#period-lattice) $\Lambda\subset\mathbb C$ and an integer $k>2$, this sum converges absolutely. Pairing $\omega$ and $-\omega$ makes it zero when $k$ is odd. For even weights it supplies the [Laurent coefficients of the Weierstrass elliptic function](complex-analysis.md#laurent-coefficients-of-the-weierstrass-elliptic-function). Scaling the [period lattice](complex-analysis.md#period-lattice) gives $G_k(a\Lambda)=a^{-k}G_k(\Lambda)$.

##### A complex lattice is determined by its fourth and sixth Eisenstein sums

↑ **Parent:** [Lattice Eisenstein sum](#lattice-eisenstein-sum)

Equal sums give equal [Klein j-invariants](#klein-j-invariant), hence the [complex lattices](fourier-analysis.md#complex-lattice) are homothetic. If both sums are nonzero, the scaling factor obeys $a^4=a^6=1$ and is $\pm1$. If only $G_6$ vanishes, the lattice is homothetic to the square lattice and the possible fourth roots of unity already preserve it. If only $G_4$ vanishes, it is homothetic to the hexagonal lattice and the possible sixth roots of unity preserve it. The two sums cannot vanish together because the elliptic discriminant is nonzero.

#### Weight-four Eisenstein basis at level two

↑ **Parent:** [Eisenstein series](#eisenstein-series)

There are no weight-four [cusp forms](#cusp-form) at level two. A nonzero form would have a weight-twelve [coset norm of a modular form](#coset-norm-of-a-modular-form) with [modular cusp](#cusp-of-a-modular-group) order at least two, contradicting the simple [modular cusp](#cusp-of-a-modular-group) order and interior nonvanishing of the [modular discriminant](#modular-discriminant). The two independent displayed [Eisenstein series](#eisenstein-series) span the weight-four space, since its cusp-constant map embeds it in a two-dimensional space.

#### Character-twisted Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For $k>2$ and a [Dirichlet character](algebraic-number-theory.md#dirichlet-character) modulo $N$ with $\chi(-1)=(-1)^k$, define $G_k(\chi,z)=\sum_{m,n\in\mathbb Z,\ (n,N)=1}\chi(n)(mz+n)^{-k}$. This series converges absolutely and locally uniformly on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) and has period $N$.

##### Fourier expansion of a character-twisted Eisenstein series

↑ **Parent:** [Character-twisted Eisenstein series](#character-twisted-eisenstein-series)

With $S_\chi(r)$ the finite Fourier transform in [Gauss sum of a Dirichlet character](algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character), the constant coefficient of $G_k(\chi,z)$ in $e^{2\pi iz/N}$ is $2L(\chi,k)$, and its positive coefficients are

$$
c_n=\frac{2(-2\pi i)^k}{(k-1)!N^k}\sum_{r\mid n}r^{k-1}S_\chi(r).
$$

For a [primitive Dirichlet character](algebraic-number-theory.md#primitive-dirichlet-character) this simplifies to $2(-2\pi i)^kg(\chi)((k-1)!N^k)^{-1}\sum_{r\mid n}\overline\chi(r)r^{k-1}$. Without primitivity the simplified formula is generally false.

#### Fourier expansion of a normalized Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For even $k\geq4$, the normalized level-one Eisenstein series has expansion

$$
E_k(\tau)=1+\frac{2}{\zeta(1-k)}\sum_{n\geq1}\sigma_{k-1}(n)q^n
=1-\frac{2k}{B_k}\sum_{n\geq1}\sigma_{k-1}(n)q^n.
$$

##### Divisor-sum convolution identity of weights four and eight

↑ **Parent:** [Fourier expansion of a normalized Eisenstein series](#fourier-expansion-of-a-normalized-eisenstein-series)

The identity $E_8=E_4^2$ gives

$$
\sigma_7(n)=\sigma_3(n)+120\sum_{i=1}^{n-1}\sigma_3(i)\sigma_3(n-i).
$$

#### Integral echelon basis of level-one modular forms

↑ **Parent:** [Eisenstein series](#eisenstein-series)

If $N+1=\dim M_k(SL_2(\mathbb Z))$, there is a basis $f_0,\ldots,f_N$ with integral Fourier coefficients and

$$
f_i=q^i+\sum_{n\geq N+1}a_n(f_i)q^n.
$$

Start from the integral forms $\Delta^iE_4^aE_6^b$ and use integer elimination on their unitriangular leading coefficients.

##### Eisenstein congruence from a denominator prime

↑ **Parent:** [Integral echelon basis of level-one modular forms](#integral-echelon-basis-of-level-one-modular-forms)

If the first nonconstant coefficient of $E_k$ has reduced denominator divisible by a prime $p$, the integral echelon basis produces an integral cusp form whose Fourier coefficients are congruent modulo $p$ to $\sigma_{k-1}(n)$.

###### Weight-sixteen Eisenstein congruence

↑ **Parent:** [Eisenstein congruence from a denominator prime](#eisenstein-congruence-from-a-denominator-prime)

The weight-sixteen [cusp form](#cusp-form) space is spanned by $E_4\Delta$. Its leading coefficient and the [Fourier expansion of a normalized Eisenstein series](#fourier-expansion-of-a-normalized-eisenstein-series) give $3617E_{16}=3617E_4^4-3456000E_4\Delta$. The coefficient multiplier $-3456000$ is congruent to $16320$ modulo $3617$, and is invertible there. Coefficient comparison gives the displayed [modular congruence](number-theory.md#modular-congruence). Integrality of $E_4\Delta$ follows from the [modular discriminant](#modular-discriminant) product.

#### Congruence-class Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For $k>2$ and $(x,y)\in(\mathbb Z/N\mathbb Z)^2$,

$$
G_k^{(x,y)}(\tau)=
\sum_{(c,d)\ne(0,0)\atop(c,d)\equiv(x,y)\bmod N}(c\tau+d)^{-k}
$$

is a modular form of weight $k$ for the principal congruence subgroup $\Gamma(N)$. Right multiplication of $(x,y)$ by $\gamma\in SL_2(\mathbb Z)$ describes its slash transformation.

#### Orthogonality of cusp forms and holomorphic Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For the full modular group, a cusp form is orthogonal under the [Petersson inner product](#petersson-inner-product) to every holomorphic Eisenstein series of the same weight. Unfolding reduces the integral to the constant Fourier coefficient of the cusp form, which is zero.

#### Eisenstein series of weight two

↑ **Parent:** [Eisenstein series](#eisenstein-series)

The series

$$
E_2(\tau)=1-24\sum_{n\geq1}\sigma_1(n)q^n
$$

is quasimodular: $E_2(-1/\tau)=\tau^2E_2(\tau)+6\tau/(\pi i)$.

##### Almost holomorphic weight-two Eisenstein series

↑ **Parent:** [Eisenstein series of weight two](#eisenstein-series-of-weight-two)

The [logarithmic derivative](analytic-number-theory.md#logarithmic-derivative) of the [modular discriminant](#modular-discriminant) gives $E_2=\Delta'/(2\pi i\Delta)$. Differentiating its weight-twelve transformation yields the anomalous term $6c(c\tau+d)/(\pi i)$. Subtracting the displayed inverse-height term cancels that anomaly. The result transforms with weight two under the [modular group](#modular-group) but is not holomorphic, so it is not a holomorphic [modular form](#modular-form).

###### Weight-two transformation from an invariant Eisenstein limit

↑ **Parent:** [Almost holomorphic weight-two Eisenstein series](#almost-holomorphic-weight-two-eisenstein-series)

The finite Laurent coefficient $C(z)$ in the [Kronecker limit formula](#kronecker-limit-formula) is invariant under the [modular group](#modular-group). Its Wirtinger derivative satisfies $\partial_z C=-\pi i(E_2(z)-3/(\pi y))/12$, by differentiating the convergent product in that formula. Differentiating $C(\gamma z)=C(z)$ gives weight-two covariance for $E_2^*$. Since $\Im(\gamma z)=y/|cz+d|^2$, substitution gives the displayed transformation law. This proof needs no prior modularity assertion for the eta product.

###### Cancellation of weight-two Eisenstein anomalies

↑ **Parent:** [Almost holomorphic weight-two Eisenstein series](#almost-holomorphic-weight-two-eisenstein-series)

For a [matrix](vector-space.md#matrix) in the [Gamma 0 congruence subgroup](group-theory.md#gamma-0-congruence-subgroup), argument dilation conjugates its action to an integral determinant-one matrix for each divisor $M$ of $N$. The anomaly of $E_2(M\tau)$ is $6c(c\tau+d)/(M\pi i)$, so the displayed linear condition cancels it. Necessity follows by testing the matrix with rows $(1,0)$ and $(N,1)$. The combinations $E_2(\tau)-ME_2(M\tau)$, with $M>1$ dividing $N$, span this space.

##### Iterated Eisenstein summation in weight two

↑ **Parent:** [Eisenstein series of weight two](#eisenstein-series-of-weight-two)

In the displayed iterated order, with the $n$ sum evaluated first, $G_2(z)=(\pi^2/3)E_2(z)$. The [cosecant partial-fraction identity](fourier-series.md#cosecant-partial-fraction-identity) $\sum_n(w+n)^{-2}=\pi^2\csc^2(\pi w)$ gives the positive-$m$ contribution $-4\pi^2\sum_{r\geq1}r q^{mr}$; negative $m$ gives the same contribution. Including the $m=0$ term yields $\pi^2/3-8\pi^2\sum_{n\geq1}\sigma_1(n)q^n$. The full lattice series does not have [absolute convergence](real-analysis.md#absolute-convergence), so this order must not be replaced by arbitrary rearrangement.

#### Nonholomorphic Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For $\operatorname{Re}s>1$,

$$
G(\tau,s)=\sum_{(m,n)\ne(0,0)}\frac{\operatorname{Im}(\tau)^s}{|m\tau+n|^{2s}}
$$

is an absolutely convergent modular-invariant function.

##### Completed nonholomorphic Eisenstein series

↑ **Parent:** [Nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series)

This [modular-invariant function](#modular-invariant-function), initially defined for $\Re s>1$, has [Fourier expansion](fourier-series.md)

$$
\mathcal E(z,s)=\Xi(2s)y^s+\Xi(2s-1)y^{1-s}+2\sqrt y\sum_{n\ne0}|n|^{s-1/2}\sigma_{1-2s}(|n|)K_{s-1/2}(2\pi|n|y)e^{2\pi inx},
$$

where $\Xi(u)=\pi^{-u/2}\Gamma(u/2)\zeta(u)$ is the [completed Riemann zeta function](analytic-number-theory.md#completed-riemann-zeta-function), without the entire-xi polynomial factor. [Poisson summation](fourier-analysis.md#poisson-summation-formula) and the [integral representation of the modified Bessel function of the second kind](analysis.md#integral-representation-of-the-modified-bessel-function-of-the-second-kind) prove the expansion. It gives [meromorphic continuation](complex-analysis.md#meromorphic-continuation), $\mathcal E(z,s)=\mathcal E(z,1-s)$, and simple [poles](isolated-singularity.md#pole) at zero and one with residues $-1/2,1/2$. Apparent poles at $s=1/2$ cancel between the two constant terms.

###### Kronecker limit formula

↑ **Parent:** [Completed nonholomorphic Eisenstein series](#completed-nonholomorphic-eisenstein-series)

This normalization of the first Kronecker limit formula follows from the [Fourier expansion](fourier-series.md) of the [completed nonholomorphic Eisenstein series](#completed-nonholomorphic-eisenstein-series). At $s=1$, $K_{1/2}(t)=\sqrt{\pi/(2t)}e^{-t}$, so the nonconstant terms sum to $-2\log|\prod_{m\geq1}(1-q^m)|$. The constant terms supply $\pi y/6-(\log y)/2+(\gamma-\log(4\pi))/2$. Combining them gives the [Dedekind eta function](string-theory.md#dedekind-eta-function) expression, with $\gamma$ the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant).

##### Primitive real-analytic Eisenstein series

↑ **Parent:** [Nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series)

For $\operatorname{Re}s>1$ this [Eisenstein series](#eisenstein-series) also equals $\sum_{\gamma\in\Gamma_\infty\backslash SL_2(\mathbb Z)}(\operatorname{Im}\gamma\tau)^s$, where $\Gamma_\infty$ consists of translations and their negatives. It is [modular invariant](#modular-invariant-function). The [nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series) summed over all nonzero integer pairs instead equals $2\zeta(2s)E(\tau,s)$: separate each pair into a positive integer times a primitive pair. This normalization matters in [Rankin–Selberg unfolding](#rankin-selberg-method).

##### Constant term of a nonholomorphic Eisenstein series

↑ **Parent:** [Nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series)

For the series over all nonzero integer pairs, the constant [Fourier coefficient](fourier-series.md#fourier-coefficient) is $2\zeta(2s)y^s+2\sqrt\pi\,\Gamma(s-1/2)\zeta(2s-1)y^{1-s}/\Gamma(s)$. Integrating over one real period unfolds the translated intervals and then uses the [Gaussian integral](calculus.md#gaussian-integral). Multiplication by $\pi^{-s}\Gamma(s)$ expresses it as $2\Lambda(2s)y^s+2\Lambda(2s-1)y^{1-s}$ in terms of the [completed Riemann zeta function](analytic-number-theory.md#completed-riemann-zeta-function).

##### Hecke eigenvalue of a nonholomorphic Eisenstein series

↑ **Parent:** [Nonholomorphic Eisenstein series](#nonholomorphic-eisenstein-series)

For the normalization $(T_pf)(\tau)=p^{-1}(f(p\tau)+\sum_{b\bmod p}f((\tau+b)/p))$, one has

$$
T_pG(\tau,s)=(p^{s-1}+p^{-s})G(\tau,s).
$$

#### Weight-k real-analytic Eisenstein series

↑ **Parent:** [Eisenstein series](#eisenstein-series)

For even $k$ and $\operatorname{Re}s>(2-k)/2$, define

$$
E_{k,s}(\tau)=
\sum_{\gamma\in\Gamma_\infty\backslash\Gamma(1)}
\operatorname{Im}(\gamma\tau)^s j(\gamma,\tau)^{-k}.
$$

It is generally nonholomorphic and transforms with weight $k$.

##### Analytic continuation of a weight-k real-analytic Eisenstein series

↑ **Parent:** [Weight-k real-analytic Eisenstein series](#weight-k-real-analytic-eisenstein-series)

For fixed $\tau$, Mellin transformation of a weighted Gaussian theta series expresses $G_k(\tau,s)$ as a gamma factor times a Mellin integral. Splitting at one and applying Poisson summation to the small-time part continues it to all $s\in\mathbb C$; for positive even $k$, the reciprocal gamma factor cancels the apparent poles.

##### Absolute convergence of a weight-k real-analytic Eisenstein series

↑ **Parent:** [Weight-k real-analytic Eisenstein series](#weight-k-real-analytic-eisenstein-series)

The absolute value of the summand indexed by a primitive bottom row $(c,d)$ is

$$
y^{\operatorname{Re}s}|c\tau+d|^{-2\operatorname{Re}s-k}.
$$

The exponent exceeds two, so comparison with the lattice sum over $(c,d)\in\mathbb Z^2\setminus\{0\}$ proves absolute and locally uniform convergence.

##### Invariant product with a weight-k real-analytic Eisenstein series

↑ **Parent:** [Weight-k real-analytic Eisenstein series](#weight-k-real-analytic-eisenstein-series)

If $f$ is a weight-$k$ modular form, then

$$
f(\tau)\overline{E_{k,s}(\tau)}(\operatorname{Im}\tau)^k
$$

is modular invariant. The factors transform by $j(\gamma,\tau)^k$, $\overline{j(\gamma,\tau)}^k$, and $|j(\gamma,\tau)|^{-2k}$.

### Hecke operator

↑ **Parent:** [Modular form](#modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hecke_operator)

For a prime $p$, one normalization of the weight-$k$ Hecke operator at level one is

$$
(T_pf)(\tau)=p^{k-1}f(p\tau)
+\frac1p\sum_{b=0}^{p-1}f\left(\frac{\tau+b}{p}\right).
$$

If $f=\sum_na_nq^n$, then

$$
T_pf=\sum_n\left(a_{pn}+p^{k-1}a_{n/p}\right)q^n,
$$

where $a_{n/p}=0$ unless $p$ divides $n$.

#### Modular Hecke algebra

↑ **Parent:** [Hecke operator](#hecke-operator)

A modular Hecke algebra is the algebra generated by [Hecke operators](#hecke-operator) acting on a specified space of [modular forms](#modular-form), with level, weight and coefficient ring fixed. Its [Eisenstein ideal](#eisenstein-ideal) encodes congruences with Eisenstein eigenvalues. This arithmetic algebra should not be confused with the generic Hecke algebra of a Coxeter group.

##### Eisenstein ideal

↑ **Parent:** [Modular Hecke algebra](#modular-hecke-algebra)

The Eisenstein ideal in a [modular Hecke algebra](#modular-hecke-algebra) imposes the eigenvalue relations of an Eisenstein series, such as $T_\ell-(1+\ell)$ in an appropriate weight-two trivial-character setting. Congruences modulo this ideal connect [modular forms](#modular-form) and class-field constructions in the [Mazur-Wiles theorem](algebraic-number-theory.md#mazur-wiles-theorem). Other weights and characters require adjusted eigenvalues.

#### Hecke eigenform

↑ **Parent:** [Hecke operator](#hecke-operator)

A Hecke eigenform is a nonzero [modular form](#modular-form) that is an [eigenvector](linear-operator-theory.md#eigenvector) for every [Hecke operator](#hecke-operator). A cuspidal eigenform has nonzero first [Fourier coefficient](fourier-series.md#fourier-coefficient): $a_1(T_nf)=a_n(f)$ proves this. Normalize $a_1=1$, and then $T_nf=a_n(f)f$. The [Hecke multiplication relations](#hecke-multiplication-relations) give multiplicativity and the prime-power recurrence of the coefficients.

##### Prime-power coefficients of a level-one eigenform are often large and positive

↑ **Parent:** [Hecke eigenform](#hecke-eigenform)

For a normalized level-one [cusp form](#cusp-form) [Hecke eigenform](#hecke-eigenform) of weight $k$, fix a [prime number](number-theory.md#prime-number) $p$ whose local quadratic has distinct roots. [Hecke multiplication relations](#hecke-multiplication-relations) give $b_e=x b_{e-1}-b_{e-2}$ for $b_e=a_{p^e}/p^{e(k-1)/2}$ and real $x=a_p/p^{(k-1)/2}$. If $|x|<2$, write $x=2\cos\theta$; then $b_e=\sin((e+1)\theta)/\sin\theta$. Periodicity when $\theta/(2\pi)$ is rational, and density of irrational rotations otherwise, give infinitely many $b_e\ge1/2$. If $|x|>2$, the distinct real reciprocal roots give positive unbounded even-index terms. Reality follows from [Hecke operators are self-adjoint for the Petersson inner product](#hecke-operators-are-self-adjoint-for-the-petersson-inner-product).

##### Euler product of a Hecke eigenform

↑ **Parent:** [Hecke eigenform](#hecke-eigenform)

For a normalized weight-$k$ cuspidal [Hecke eigenform](#hecke-eigenform), the local recurrence gives $\sum_{r\geq0}a_{p^r}X^r=(1-a_pX+p^{k-1}X^2)^{-1}$. Multiplicativity therefore gives $L(f,s)=\prod_p(1-a_pp^{-s}+p^{k-1-2s})^{-1}$ in a right half-plane. Each degree-two local factor packages all the prime-power [Fourier coefficients](fourier-series.md#fourier-coefficient).

##### Hecke eigenvalues are algebraic integers

↑ **Parent:** [Hecke eigenform](#hecke-eigenform)

The rational space of level-one [cusp forms](#cusp-form) has a full lattice of forms with integral [Fourier coefficients](fourier-series.md#fourier-coefficient). It has finite rank by the [valence formula for the modular group](#valence-formula-for-the-modular-group), and is preserved by the [Fourier coefficients of a composite-index Hecke operator](#fourier-coefficients-of-a-composite-index-hecke-operator) formula. Thus every [Hecke operator](#hecke-operator) has a monic integral characteristic polynomial on this lattice, and its [eigenvalues](linear-operator-theory.md#eigenvalue) are [algebraic integers](algebraic-number-theory.md#algebraic-integer). The common eigenvalue field is totally real by the [Petersson inner product](#petersson-inner-product) self-adjointness.

#### Hecke multiplication relations

↑ **Parent:** [Hecke operator](#hecke-operator)

For level-one weight-$k$ [modular forms](#modular-form), $T_mT_n=\sum_{d\mid\gcd(m,n)}d^{k-1}T_{mn/d^2}$. Thus coprime indices multiply directly, and $T_pT_{p^r}=T_{p^{r+1}}+p^{k-1}T_{p^{r-1}}$. The [Fourier coefficients of a composite-index Hecke operator](#fourier-coefficients-of-a-composite-index-hecke-operator) prove these relations by regrouping divisors. They show that the [Hecke algebra of modular forms](#integral-hecke-algebra-of-level-one-cusp-forms) is commutative and generated by prime operators.

##### Hecke prime-power recurrence from q-shift operators

↑ **Parent:** [Hecke multiplication relations](#hecke-multiplication-relations)

On a [Fourier series](fourier-series.md) put $U_p(\sum a_nq^n)=\sum a_{pn}q^n$ and $V_pf(q)=f(q^p)$. These auxiliary operators need not individually preserve the level-one [modular form](#modular-form) space. Nevertheless $U_pV_p=1$, and the [Fourier coefficients of a composite-index Hecke operator](#fourier-coefficients-of-a-composite-index-hecke-operator) give $T_{p^r}=\sum_{j=0}^rp^{j(k-1)}V_p^jU_p^{r-j}$. Multiplication by $T_p=U_p+p^{k-1}V_p$, using $U_pV_p=1$, gives the displayed recurrence. In particular the distinction between $U_pV_p=1$ and $V_pU_p\ne1$ is essential.

#### Noncuspidal level-one Hecke eigenform

↑ **Parent:** [Hecke operator](#hecke-operator)

A simultaneous eigenfunction of all normalized level-one [Hecke operators](#hecke-operator) in positive even weight, with nonzero constant [Fourier coefficient](fourier-series.md#fourier-coefficient), is a multiple of the normalized [Eisenstein series](#eisenstein-series). The constant coefficient forces its $T_n$ eigenvalue to be $\sigma_{k-1}(n)$, and $a_1(T_nf)=a_n(f)$ forces $a_n(f)=a_1(f)\sigma_{k-1}(n)$. Subtracting the matching constant multiple of the [Eisenstein series](#eisenstein-series) leaves a [cusp form](#cusp-form). Unless every coefficient vanishes, its prime-index coefficients grow like $p^{k-1}$, contradicting the [Fourier coefficient bound for a cusp form](#fourier-coefficient-bound-for-a-cusp-form) $O(p^{k/2})$ when $k\geq4$. Weight two has no nonzero [modular forms](#modular-form), by [vanishing of weight-two level-one modular forms](#vanishing-of-weight-two-level-one-modular-forms).

#### Integral Hecke algebra of level-one cusp forms

↑ **Parent:** [Hecke operator](#hecke-operator)

This is the subring generated by the [Hecke operators](#hecke-operator) $T_n$ and the integer scalars acting on level-one [cusp forms](#cusp-form). It preserves the lattice of [cusp forms](#cusp-form) with integral [Fourier coefficients of a composite-index Hecke operator](#fourier-coefficients-of-a-composite-index-hecke-operator). It is distinct from the generic [Hecke algebra](lie-theory.md#hecke-algebra) attached to a [Coxeter system](lie-theory.md#coxeter-system).

##### Perfect integral Hecke pairing

↑ **Parent:** [Integral Hecke algebra of level-one cusp forms](#integral-hecke-algebra-of-level-one-cusp-forms)

The pairing $(T,f)\mapsto a_1(Tf)$ identifies the [integral Hecke algebra of level-one cusp forms](#integral-hecke-algebra-of-level-one-cusp-forms) with the integral dual of the cusp-form lattice. An integral basis beginning $q,q^2,\ldots,q^m$ gives a unitriangular first-$m$ coefficient matrix, so $a_1,\ldots,a_m$ form a dual basis. Commutativity of the [Hecke operators](#hecke-operator) proves nondegeneracy on the algebra, and $T_1,\ldots,T_m$ then form its integral basis.

#### Fourier coefficients of a composite-index Hecke operator

↑ **Parent:** [Hecke operator](#hecke-operator)

For the determinant-normalized [slash operator for modular forms](#slash-operator-for-modular-forms), $T_nf=n^{k/2-1}\sum_{\gamma\in\Pi_n}f|_k\gamma$. If $f=\sum_{r\geq0}a_rq^r$, then $a_r(T_nf)=\sum_{a\mid\gcd(n,r)}a^{k-1}a_{nr/a^2}(f)$, with $\gcd(n,0)=n$. In particular $a_1(T_nf)=a_n(f)$, integer coefficients are preserved, and [cusp forms](#cusp-form) remain cusp forms.

#### Determinant-n matrix representatives for Hecke operators

↑ **Parent:** [Hecke operator](#hecke-operator)

Left $SL_2(\mathbb Z)$-orbits of integral matrices of positive determinant $n$ have unique representatives $\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $a,d>0$, $ad=n$ and $0\leq b<d$. Bezout's identity reduces the first column to $(a,0)$; a row shear reduces $b$ modulo $d$.

#### Finite Hecke orbit criterion for holomorphy at a cusp

↑ **Parent:** [Hecke operator](#hecke-operator)

Let a level-one modular function be holomorphic on the upper half-plane. If the span of $f,T_pf,T_p^2f,\ldots$ is finite-dimensional, then $f$ is holomorphic at infinity. Indeed, a pole of order $N$ would make $T_p^rf$ have pole order $p^rN$, producing linearly independent functions.

### Meromorphic modular form

↑ **Parent:** [Modular form](#modular-form)

A meromorphic modular form obeys the modular transformation law and is meromorphic on the upper half-plane and at the cusps.

#### Cusp-form divisor presentation

↑ **Parent:** [Meromorphic modular form](#meromorphic-modular-form)

For a torsion-free modular curve with regular [modular cusps](#cusp-of-a-modular-group), let $f$ be a nonzero meromorphic weight-$k$ form and $C$ the reduced sum of [modular cusp](#cusp-of-a-modular-group) points. The local-order divisor of $f$, minus $C$, imposes exactly holomorphy in the interior and vanishing at every [modular cusp](#cusp-of-a-modular-group) on the product $f\varphi$. Dividing any [cusp form](#cusp-form) by $f$ gives the reverse identification with a [Riemann-Roch space](algebraic-geometry.md#riemann-roch-space). The [regular-cusp valence formula on a torsion-free modular curve](#regular-cusp-valence-formula-on-a-torsion-free-modular-curve) and [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) compute the dimension when the resulting divisor has degree greater than the canonical degree.

#### Regular-cusp valence formula on a torsion-free modular curve

↑ **Parent:** [Meromorphic modular form](#meromorphic-modular-form)

For a torsion-free effective modular group with genuine, untwisted [modular cusp](#cusp-of-a-modular-group) periods, a meromorphic weight-$k$ form has integer local orders. The tensor differential $f^{12}(d\tau)^{6k}$ has interior order $12\operatorname{ord}f$ and [modular cusp](#cusp-of-a-modular-group) order $12\operatorname{ord}f-6k$. Its canonical degree and the [genus formula for a modular curve](#genus-formula-for-a-modular-curve) yield the displayed valence formula, with $d$ the projective index. Regular [modular cusp](#cusp-of-a-modular-group) periods are important in odd weights.

#### Valence formula for the modular group

↑ **Parent:** [Meromorphic modular form](#meromorphic-modular-form)

For a nonzero meromorphic modular form $f$ of weight $k$,

$$
v_\infty(f)+\frac12v_i(f)+\frac13v_\rho(f)
+\sum_{z\ne i,\rho}v_z(f)=\frac{k}{12},
\qquad \rho=e^{2\pi i/3},
$$

where the sum takes one representative from each modular-group orbit.

##### Vanishing of weight-fourteen level-one cusp forms

↑ **Parent:** [Valence formula for the modular group](#valence-formula-for-the-modular-group)

A nonzero weight-fourteen [cusp form](#cusp-form) would have order at infinity at least one and order at $i$ at least one, since $i^{14}=-1$. The [valence formula for the modular group](#valence-formula-for-the-modular-group) would then give $1+1/2\leq14/12$, which is impossible.

##### Vanishing of weight-two level-one modular forms

↑ **Parent:** [Valence formula for the modular group](#valence-formula-for-the-modular-group)

A weight-two [modular form](#modular-form) obeys $f(i)=i^2f(i)=-f(i)$, so it vanishes at $i$. The [valence formula for the modular group](#valence-formula-for-the-modular-group) would then have left side at least $1/2$, but right side $2/12=1/6$. All orders are nonnegative by holomorphy, giving a contradiction for nonzero $f$.

##### Dimension bound for modular forms on a finite-index subgroup

↑ **Parent:** [Valence formula for the modular group](#valence-formula-for-the-modular-group)

For nonnegative integer $k$ and a finite-index subgroup $\Gamma$, a nonzero [modular form](#modular-form) has order at infinity, measured in a genuine periodic cusp parameter, at most $k[SL_2(\mathbb Z):\Gamma]/12$. The product of its slash translates over the left cosets is a nonzero level-one form; the translates along the infinity-cusp orbit contribute its full local order to this product. The [valence formula for the modular group](#valence-formula-for-the-modular-group) gives the bound. Initial coefficients through that bound therefore give an injective linear map.

#### Klein j-invariant

↑ **Parent:** [Meromorphic modular form](#meromorphic-modular-form)

The Klein j-invariant is the weight-zero level-one modular function

$$
j(\tau)=\frac{E_4(\tau)^3}{\Delta(\tau)}
=q^{-1}+744+O(q).
$$

It is holomorphic on the upper half-plane and has a simple pole at infinity.

##### Klein j-invariant classifies complex lattice homothety

↑ **Parent:** [Klein j-invariant](#klein-j-invariant)

The [valence formula for the modular group](#valence-formula-for-the-modular-group) shows that $\Delta=(E_4^3-E_6^2)/1728$ has no zeros in the half-plane. For every $a\in\mathbb C$, the weight-twelve form $E_4^3-a\Delta$ has total weighted zero order one. At $a=0$ its sole zero is the order-three zero at the cubic elliptic orbit; at $a=1728$ its sole zero is the order-two zero at the quadratic elliptic orbit. Otherwise it has one simple ordinary zero orbit. Thus each value of the [Klein j-invariant](#klein-j-invariant) occurs on exactly one modular orbit and classifies one [homothety of complex lattices](fourier-analysis.md#homothety-of-complex-lattices).

##### Level-two modular ratio of Klein j-invariants

↑ **Parent:** [Klein j-invariant](#klein-j-invariant)

The function $j(\tau)/j(2\tau)$ has weight zero and level $\Gamma_1(2)=\Gamma_0(2)$. It has a simple zero at the cusp at infinity and a simple pole at the cusp zero.

### Theta function

↑ **Parent:** [Modular form](#modular-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theta_function)

A theta function is a holomorphic function formed by summing an exponential quadratic form over a lattice.

#### Riemann theta function

↑ **Parent:** [Theta function](#theta-function)

For a symmetric matrix $B$ with positive definite imaginary part, this [theta function](#theta-function) converges normally on [compact](topology.md#compact-space) subsets of $\mathbb C^g$. It obeys $\theta(z+m+Bn,B)=e^{-\pi i n^tBn-2\pi i n^tz}\theta(z,B)$, so its zeros define a [divisor](number-theory.md#divisor) on the associated [complex torus](complex-geometry.md#complex-torus). If $B$ is a curve's normalized period matrix, its zero [divisor](number-theory.md#divisor) is a translate of the effective degree-$g-1$ locus, by the [Riemann vanishing theorem](abelian-variety.md#riemann-vanishing-theorem). A general symmetric positive period matrix need not come from a curve.

#### Gaussian theta sum

↑ **Parent:** [Theta function](#theta-function)

For a full [Euclidean lattice](fourier-analysis.md#euclidean-lattice) $\Lambda$ and a positive definite real symmetric matrix $A$, the Gaussian theta sum is $\theta_\Lambda(A)=\sum_{\lambda\in\Lambda}e^{-\pi\lambda^TA\lambda}$. Its absolute convergence follows from Gaussian decay and the polynomial growth of the number of lattice points in a ball. The [Poisson summation formula for a Euclidean lattice](fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) gives its [anisotropic theta functional equation](#anisotropic-theta-functional-equation).

##### Theta series of a Euclidean lattice

↑ **Parent:** [Gaussian theta sum](#gaussian-theta-sum)

The [lattice theta series](#theta-series-of-a-euclidean-lattice) of a full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice) records the multiset of squared lengths of lattice vectors. The Gaussian form shown here converges for $t>0$. For a [flat torus](second-fundamental-form.md#flat-torus) $\mathbb R^d/\Lambda$, its [heat trace](riemannian-geometry.md#heat-trace) is $\Theta_{\Lambda^*}(4\pi t)$, by the [spectrum of a flat torus](second-fundamental-form.md#spectrum-of-a-flat-torus). Equal theta series do not in general imply orthogonal equivalence of lattices.

##### Small-parameter asymptotic of a lattice theta sum

↑ **Parent:** [Gaussian theta sum](#gaussian-theta-sum)

If every eigenvalue of a positive definite symmetric matrix $A$ tends to zero, then the [anisotropic theta functional equation](#anisotropic-theta-functional-equation) and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) show that $(\det A)^{1/2}\theta_\Lambda(A)\to\operatorname{covol}(\Lambda)^{-1}$. Indeed all eigenvalues of $A^{-1}$ tend to infinity, the zero term of the dual [Gaussian theta sum](#gaussian-theta-sum) is one, and its remaining terms tend to zero while being dominated by a fixed summable Gaussian. Merely requiring $\det A\to0$ is insufficient.

##### Covolume-one theta function of a fractional ideal

↑ **Parent:** [Gaussian theta sum](#gaussian-theta-sum)

Let $C=\sqrt{|D_K|}N(\mathfrak b)$ and $n=[K:\mathbb Q]$. Normalize the [Minkowski embedding of a number field](algebraic-number-theory.md#minkowski-embedding-of-a-number-field) to the [covolume](fourier-analysis.md#covolume)-one [Euclidean lattice](fourier-analysis.md#euclidean-lattice) $\Lambda_{\mathfrak b}=C^{-1/n}j(\mathfrak b)$, using the metric with complex coordinates weighted by $2$. Its theta function is

$$
\Theta(y,\mathfrak b)=\sum_{a\in\mathfrak b}\exp\left(-\pi C^{-2/n}\sum_v[K_v:\mathbb R]y_v|\sigma_v(a)|^2\right).
$$

Writing $\|y\|=\prod_v y_v^{[K_v:\mathbb R]}$ and using the [trace dual of a fractional ideal](algebraic-number-theory.md#trace-dual-of-a-fractional-ideal) gives $\Theta(y,\mathfrak b)=\|y\|^{-1/2}\Theta(y^{-1},\mathfrak b^\vee)$. Its [small-parameter asymptotic of a lattice theta sum](#small-parameter-asymptotic-of-a-lattice-theta-sum) has leading coefficient one. For the unscaled ideal lattice, the leading coefficient is instead $C^{-1}$; one must specify the normalization when quoting this limit.

#### Lattice theta functional equation

↑ **Parent:** [Theta function](#theta-function)

For a full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice), $\Theta_\Lambda(\tau)=\sum_{x\in\Lambda}e^{\pi i|x|^2\tau}$ obeys $\Theta_\Lambda(\tau)=(-i\tau)^{-n/2}m(\Lambda)^{-1}\Theta_{\Lambda^\vee}(-1/\tau)$. Apply the [Poisson summation formula for a Euclidean lattice](fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice) and the [complex Gaussian Fourier transform](fourier-analysis.md#complex-gaussian-fourier-transform). The identity holds without assuming an integral or self-dual lattice.

##### Anisotropic theta functional equation

↑ **Parent:** [Lattice theta functional equation](#lattice-theta-functional-equation)

For a full [Euclidean lattice](fourier-analysis.md#euclidean-lattice) and a positive definite real symmetric matrix $A$, the [Gaussian theta sum](#gaussian-theta-sum) obeys

$$
\theta_\Lambda(A)=\operatorname{covol}(\Lambda)^{-1}(\det A)^{-1/2}\theta_{\Lambda^*}(A^{-1}).
$$

Use the [Fourier transform](analysis.md#fourier-transform) kernel $e^{-2\pi i x\cdot z}$, the identity $\widehat{e^{-\pi x^TAx}}(z)=(\det A)^{-1/2}e^{-\pi z^TA^{-1}z}$, and the [Poisson summation formula for a Euclidean lattice](fourier-analysis.md#poisson-summation-formula-for-a-euclidean-lattice). No integrality or self-duality of the [Euclidean lattice](fourier-analysis.md#euclidean-lattice) is assumed.

#### Jacobi theta function

↑ **Parent:** [Theta function](#theta-function)

The Jacobi theta function

$$
\theta(\tau)=\sum_{n\in\mathbb Z}e^{\pi in^2\tau}
$$

satisfies $\theta(\tau+2)=\theta(\tau)$ and $\theta(-1/\tau)=(-i\tau)^{1/2}\theta(\tau)$.

##### Jacobi derivative formula

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

Use period-one spatial normalization and $Q=e^{\pi i\tau}$. The conventional odd function is $\theta_1=-\theta[1/2,1/2]$ with the characteristic convention of [theta function with characteristics](#theta-function-with-characteristics). Differentiating its [Jacobi triple product](#jacobi-triple-product) gives $\theta_1'(0)=2\pi Q^{1/4}\prod_{m\geq1}(1-Q^{2m})^3$. The three even constant products have product $2Q^{1/4}\prod_{m\geq1}(1-Q^{2m})^3$, proving the identity. The sign changes if one instead calls the characteristic series itself theta1.

##### Theta function with characteristics

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

For real characteristics $\alpha,\beta$ and $\operatorname{Im}\tau>0$, Gaussian decay gives normal convergence, an entire function of $z$ and holomorphic dependence on $\tau$. Integer shifts of alpha leave the function unchanged; a unit shift of beta multiplies it by $e^{2\pi i\alpha}$. Its spatial quasi-periods are $\theta(z+1)=e^{2\pi i\alpha}\theta(z)$ and $\theta(z+\tau)=e^{-\pi i\tau-2\pi i(z+\beta)}\theta(z)$. Binary characteristic labels often mean alpha and beta divided by two, so the convention must be stated.

###### Theta constant

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

A [theta function with characteristics](#theta-function-with-characteristics) evaluated at spatial argument zero. Its dependence on $\tau\in\mathbb H$ remains [holomorphic](complex-analysis.md#complex-differentiability-at-a-point). Among the four half-integer characteristic choices, the odd one vanishes identically, whereas the three even constants are nonzero on the half-plane. The [zeros of theta functions with characteristics](#zeros-of-theta-functions-with-characteristics) locate their spatial zero away from the origin. Ratios of equal powers of even constants yield the [modular lambda function](#modular-lambda-function) and other [modular-invariant functions](#modular-invariant-function).

###### Period lattice of theta3 over theta4

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

Use the radian spatial convention $\theta_3(z,\tau)=\sum_n e^{\pi in^2\tau+2inz}$ and $\theta_4(z,\tau)=\theta_3(z+\pi/2,\tau)$. Their ratio is unchanged by $\pi$ and changes sign under $\pi\tau$. The numerator has simple zeros at $\pi(1+\tau)/2+\pi\mathbb Z+\pi\tau\mathbb Z$, while the denominator has simple zeros at $\pi\tau/2+\pi\mathbb Z+\pi\tau\mathbb Z$. The two sets are disjoint, so any period must lie in $\pi\mathbb Z+\pi\tau\mathbb Z$, by translating the [zero set](polynomial.md#zero-set). The sign rule then gives the displayed exact lattice. Squaring the ratio removes that sign and has precisely the smaller lattice $\pi\mathbb Z+\pi\tau\mathbb Z$.

###### Jacobi theta duplication identity

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

For the binary characteristic convention, each [theta function with characteristics](#theta-function-with-characteristics) has one simple zero per lattice cell. The four zeros of the numerator, at the four half-periods, cancel those of $\vartheta_{11}(2z)$. Their quotient is an entire [elliptic function](complex-analysis.md#elliptic-function), hence constant. Taking the limit at zero determines the factor one half. The product identity remains valid at the zeros, where the initial quotient requires removable extension.

###### Modular transformations of theta characteristics

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

Translation of tau by one gives $\theta[\alpha,\beta](z,\tau+1)=e^{-\pi i\alpha(\alpha-1)}\theta[\alpha,\beta+\alpha-1/2](z,\tau)$. Gaussian [Poisson summation](fourier-analysis.md#poisson-summation-formula) gives $\theta[\alpha,\beta](z/\tau,-1/\tau)=\sqrt{-i\tau}\,e^{\pi iz^2/\tau+2\pi i\alpha\beta}\theta[\beta,-\alpha](z,\tau)$. The square root is the holomorphic branch positive at tau=i. These formulas keep the characteristic phase, which is lost if one states only the transformation of unshifted theta constants.

###### Heat equation for theta functions with characteristics

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

Normal convergence allows termwise differentiation of the defining [theta function with characteristics](#theta-function-with-characteristics). A tau derivative multiplies a summand by $\pi i(n+\alpha)^2$, while its second spatial derivative multiplies it by $-4\pi^2(n+\alpha)^2$. This proves the displayed [heat equation](diffusion-equation.md#heat-equation), linking its lattice-sum construction with diffusion and analytic continuation.

###### Zeros of theta functions with characteristics

↑ **Parent:** [Theta function with characteristics](#theta-function-with-characteristics)

The logarithmic derivative is periodic under one and decreases by $2\pi i$ under tau. Integrating around a fundamental cell and applying the [argument principle](complex-analysis.md#argument-principle) counts exactly one zero, with multiplicity. The displayed zero follows from translating the zero of $\theta[0,0]$ at $(1+\tau)/2$. It is consequently simple. For half-integer characteristics only the odd characteristic $(1/2,1/2)$ vanishes at the origin; the other three theta constants are nonzero.

##### Jacobi abstruse identity

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

The identity between [Jacobi theta functions](#jacobi-theta-function) has the oscillator-product form $\prod_{r\in\mathbb N-1/2}(1+q^r)^8-\prod_{r\in\mathbb N-1/2}(1-q^r)^8=16q^{1/2}\prod_{n\ge1}(1+q^n)^8$ for $|q|<1$. In a critical [RNS string](string-theory.md#spinning-string), dividing this identity by the eight-boson oscillator product proves equality of [GSO projection](string-theory.md#gso-projection)-retained [Neveu–Schwarz sector](string-theory.md#neveu-schwarz-sector) and [Ramond sector](string-theory.md#ramond-sector) state multiplicities at every mass level.

##### Theta-constant inversion and translation laws

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

In the $e^{\pi iz}$ convention, [Poisson summation](fourier-analysis.md#poisson-summation-formula) gives $\Theta_3(-1/z)=\sqrt{-iz}\Theta_3(z)$ and interchanges $\Theta_2,\Theta_4$ with the same factor. Translation by one sends $\Theta_2$ to $e^{\pi i/4}\Theta_2$ and interchanges $\Theta_3,\Theta_4$. Eighth powers remove every phase and square-root ambiguity when proving integral-weight modularity.

##### Theta series of integer squares

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

This convention for the [Jacobi theta function](#jacobi-theta-function) is the usual theta constant evaluated at twice the argument. The [Poisson summation formula](fourier-analysis.md#poisson-summation-formula) gives $\theta(-1/(4\tau))=\sqrt{-2i\tau}\,\theta(\tau)$, with the square root holomorphic on the half-plane and positive on the imaginary axis after evaluating its positive real argument.

###### Eight-square representation formula

↑ **Parent:** [Theta series of integer squares](#theta-series-of-integer-squares)

The number of ordered integer eight-tuples with square sum $n$ satisfies the displayed divisor formula for positive $n$, with $r_8(0)=1$ separately. The eighth power of the shifted [theta series of integer squares](#theta-series-of-integer-squares) is $(16E_4(2\tau)-E_4(\tau))/15$. Its coefficient sign is $(-1)^n$, because squares and their integer roots have the same parity.

##### Jacobi triple product

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_triple_product)

For $|q|<1$ and $z\ne0$, the Jacobi triple product is

$$
\sum_{n\in\mathbb Z}z^nq^{n^2}
=\prod_{m\geq1}(1-q^{2m})(1+zq^{2m-1})(1+z^{-1}q^{2m-1}).
$$

###### Jacobi cubic product identity

↑ **Parent:** [Jacobi triple product](#jacobi-triple-product)

The odd [Dirichlet character](algebraic-number-theory.md#dirichlet-character) modulo four has $\chi_4(2r+1)=(-1)^r$. The series $B=\tfrac12\sum_n n\chi_4(n)q^{n^2/8}$ is therefore $q^{1/8}$ times the displayed sum. The [character theta proof of the eta product](algebraic-number-theory.md#character-theta-proof-of-the-eta-product) gives $B=\eta^3$, proving the identity.

###### Euler pentagonal identity

↑ **Parent:** [Jacobi triple product](#jacobi-triple-product)

The identity holds for $|q|<1$, with both sides locally uniformly convergent. In the [character theta proof of the eta product](algebraic-number-theory.md#character-theta-proof-of-the-eta-product), pair the terms indexed by $n$ and $-n$ and then select $n=6r+1$; their [Dirichlet character](algebraic-number-theory.md#dirichlet-character) signs are $(-1)^r$. Removing $q^{1/24}$ gives the displayed product identity.

##### Theta group

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

The theta group is $\Gamma_\theta=\Gamma(2)\cup\Gamma(2)S$. It is generated by $T^2$ and $S$ and has index three in the [modular group](#modular-group).

##### Nonvanishing of the Jacobi theta function

↑ **Parent:** [Jacobi theta function](#jacobi-theta-function)

The [Jacobi triple product](#jacobi-triple-product) gives

$$
\theta(\tau)=\prod_{n\geq1}(1-q^{2n})(1+q^{2n-1})^2,
\qquad q=e^{\pi i\tau}.
$$

Every factor is nonzero for $|q|<1$, and the product converges to a nonzero limit, so $\theta$ has no zero in the upper half-plane.

### Lattice model of a modular form

↑ **Parent:** [Modular form](#modular-form)

Let $\mathcal L$ be the set of complex lattices. A weight-$k$ lattice function satisfies $F(\lambda\Lambda)=\lambda^{-k}F(\Lambda)$. Evaluating at $\Lambda_\tau=\mathbb Z\tau+\mathbb Z$ identifies such functions with weight-$k$ modular-invariant functions on the upper half-plane.

#### Gamma 1 level structure on a complex lattice

↑ **Parent:** [Lattice model of a modular form](#lattice-model-of-a-modular-form)

A Gamma 1 level structure on a complex lattice $\Lambda$ is a point of exact order $N$ in $\mathbb C/\Lambda$. Similarity classes of such pairs are parametrized by $\Gamma_1(N)\backslash\mathfrak h$.

##### Diamond operator

↑ **Parent:** [Gamma 1 level structure on a complex lattice](#gamma-1-level-structure-on-a-complex-lattice)

Multiplication of a marked point by a unit modulo $N$ gives the diamond action. In modular coordinates this is the slash action of a lift in $\Gamma_0(N)$ with lower-right entry $d$. Its [Dirichlet character](algebraic-number-theory.md#dirichlet-character) eigenspaces give nebentypus [modular forms](#modular-form). For a nonzero form, the action of $-1$ imposes $\chi(-1)=(-1)^k$.

##### Hecke operator on marked lattices

↑ **Parent:** [Gamma 1 level structure on a complex lattice](#gamma-1-level-structure-on-a-complex-lattice)

Sum over index-$p$ overlattices in which the marked point retains exact order $N$. There are $p+1$ summands at good primes and $p$ at bad primes. With homogeneity $F(uL,ut)=u^{-k}F(L,t)$, the coefficient $1/p$ is the normalization giving the standard [Hecke operator](#hecke-operator) Fourier action. [Cusp holomorphy under rational slash operators](#cusp-holomorphy-under-rational-slash-operators) proves preservation of [modular forms](#modular-form).

###### Good-prime and bad-prime Hecke coefficient formula

↑ **Parent:** [Hecke operator on marked lattices](#hecke-operator-on-marked-lattices)

At a prime not dividing the level, the root-of-unity average contributes $a_{pn}$ and the scaling overlattice contributes the second term. At a prime dividing the level that overlattice loses the marked point's exact order and is excluded. Extending the [Dirichlet character](algebraic-number-theory.md#dirichlet-character) by zero gives a uniform formula, with $a_{n/p}=0$ unless $p\mid n$. The bad-prime operator is $U_p$.

##### Marked-lattice model of a modular form

↑ **Parent:** [Gamma 1 level structure on a complex lattice](#gamma-1-level-structure-on-a-complex-lattice)

Choose an oriented lattice basis with $t=\omega_2/N$ modulo the lattice. Changing such a basis is exactly the [Gamma 1 congruence subgroup](group-theory.md#gamma-1-congruence-subgroup) action, so the weight law makes the displayed function independent of the choice. It satisfies $F(uL,ut)=u^{-k}F(L,t)$. Holomorphy on the half-plane and at all [modular cusp](#cusp-of-a-modular-group) degenerations identifies the functions coming from [modular forms](#modular-form).

##### Prime-index overlattices preserving a Gamma 1 level structure

↑ **Parent:** [Gamma 1 level structure on a complex lattice](#gamma-1-level-structure-on-a-complex-lattice)

A lattice has $p+1$ index-$p$ overlattices. All preserve the exact order of a Gamma 1 level structure of order $N$ when $p\nmid N$; exactly $p$ do so when $p\mid N$.

#### Weighted Gaussian theta sum of a complex lattice

↑ **Parent:** [Lattice model of a modular form](#lattice-model-of-a-modular-form)

For an even nonnegative integer $k$,

$$
\theta_k(\Lambda)=\sum_{\lambda\in\Lambda}\lambda^ke^{-\pi|\lambda|^2}.
$$

Poisson summation and the Fourier eigenfunction identity for $(x+iy)^ke^{-\pi(x^2+y^2)}$ give

$$
\theta_k(\Lambda)=(-i)^k m(\Lambda)^{-1}\theta_k(\Lambda^\vee).
$$

#### Hecke operator on lattice functions

↑ **Parent:** [Lattice model of a modular form](#lattice-model-of-a-modular-form)

One standard normalization is

$$
(T_nF)(\Lambda)=\frac1n\sum_{\Lambda'\supset\Lambda\atop[\Lambda':\Lambda]=n}F(\Lambda').
$$

With [lattice model of a modular form](#lattice-model-of-a-modular-form) homogeneity $F(uL)=u^{-k}F(L)$, the factor $1/n$ gives the usual weight-$k$ [Hecke operator](#hecke-operator). For prime $p$, the overlattices contribute $f((\tau+b)/p)$ and $p^kf(p\tau)$; division by $p$ produces the standard Fourier coefficients.

## ↑ Ancestors (4)

1. [Number theory](number-theory.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Modular-invariant function](#modular-invariant-function)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-8.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-88.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-137.md#2/a/solution)
