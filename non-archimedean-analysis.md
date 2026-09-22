# Non-Archimedean analysis

↑ **Parent:** [Arithmetic](arithmetic.md)

Non-Archimedean analysis studies fields whose distance is induced by an ultrametric absolute value, especially local fields and valued function fields.

**Table of contents**

- [Continuous functions on the p-adic integers](#continuous-functions-on-the-p-adic-integers)
  - [Mahler's theorem](#mahler-s-theorem)
    - [Discrete antidifferentiation on the p-adic integers](#discrete-antidifferentiation-on-the-p-adic-integers)
      - [Translation-invariant linear forms on p-adic continuous functions vanish](#translation-invariant-linear-forms-on-p-adic-continuous-functions-vanish)
    - [Mahler coefficient](#mahler-coefficient)
      - [Mahler coefficient exponential generating function](#mahler-coefficient-exponential-generating-function)
      - [Mahler expansion of the parity function](#mahler-expansion-of-the-parity-function)
      - [Automatic decay of Mahler coefficients](#automatic-decay-of-mahler-coefficients)
- [Non-Archimedean ordered field](#non-archimedean-ordered-field)
- [Absolute value (algebra)](#absolute-value-algebra)
  - [Weak approximation for inequivalent absolute values](#weak-approximation-for-inequivalent-absolute-values)
  - [Bounded comparison forces equality of multiplicative absolute values](#bounded-comparison-forces-equality-of-multiplicative-absolute-values)
  - [Completion of a valued field](#completion-of-a-valued-field)
    - [Algebraic closure of the p-adic numbers is not complete](#algebraic-closure-of-the-p-adic-numbers-is-not-complete)
  - [Trivial absolute value](#trivial-absolute-value)
  - [Non-Archimedean absolute value](#non-archimedean-absolute-value)
    - [Integer criterion for a non-Archimedean absolute value](#integer-criterion-for-a-non-archimedean-absolute-value)
    - [Bounded-integer criterion for a non-Archimedean absolute value](#bounded-integer-criterion-for-a-non-archimedean-absolute-value)
    - [Ultrametric inequality](#ultrametric-inequality)
      - [Ultrametric space](#ultrametric-space)
        - [Totally disconnected space](#totally-disconnected-space)
  - [Equivalent absolute values](#equivalent-absolute-values)
  - [Extension of an absolute value](#extension-of-an-absolute-value)
    - [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)
      - [Finite-dimensional non-Archimedean norm equivalence over a complete field](#finite-dimensional-non-archimedean-norm-equivalence-over-a-complete-field)
      - [Compact-sphere proof of finite-dimensional non-Archimedean norm equivalence](#compact-sphere-proof-of-finite-dimensional-non-archimedean-norm-equivalence)
      - [Pure-power reduction of a monic irreducible polynomial](#pure-power-reduction-of-a-monic-irreducible-polynomial)
      - [Equal absolute values of algebraic conjugates](#equal-absolute-values-of-algebraic-conjugates)
      - [Integral closure in a finite extension of a complete discretely valued field](#integral-closure-in-a-finite-extension-of-a-complete-discretely-valued-field)
    - [Conjugacy of extensions of a valuation to a normal extension](#conjugacy-of-extensions-of-a-valuation-to-a-normal-extension)
    - [Valuation ring need not equal the integral closure over a noncomplete field](#valuation-ring-need-not-equal-the-integral-closure-over-a-noncomplete-field)
    - [Local factorization and extended absolute values](#local-factorization-and-extended-absolute-values)
      - [Local prime decomposition of T5 plus 6T3 plus 252T2 plus 126](#local-prime-decomposition-of-t5-plus-6t3-plus-252t2-plus-126)
      - [Prime ideals and local embedding orbits](#prime-ideals-and-local-embedding-orbits)
      - [Completion of a number field at a prime ideal](#completion-of-a-number-field-at-a-prime-ideal)
        - [p-adic tensor decomposition of a number field](#p-adic-tensor-decomposition-of-a-number-field)
        - [Transitivity of the Galois action on primes](#transitivity-of-the-galois-action-on-primes)
          - [Decomposition group](#decomposition-group)
            - [Surjectivity of decomposition group reduction](#surjectivity-of-decomposition-group-reduction)
            - [Primes in an intermediate field as double cosets](#primes-in-an-intermediate-field-as-double-cosets)
              - [Complete splitting is preserved by Galois closure](#complete-splitting-is-preserved-by-galois-closure)
            - [Decomposition group of a prime and local Galois group](#decomposition-group-of-a-prime-and-local-galois-group)
        - [Completion preserves ramification and residue data](#completion-preserves-ramification-and-residue-data)
      - [Local factorization of X3 plus 25X2 minus 50X plus 40](#local-factorization-of-x3-plus-25x2-minus-50x-plus-40)
- [Hahn series](#hahn-series)
  - [Hahn series field](#hahn-series-field)
- [P-adic number](#p-adic-number)
  - [3-adic number](#3-adic-number)
  - [p-adic absolute value](#p-adic-absolute-value)
    - [p-adic metric](#p-adic-metric)
    - [2-adic absolute value](#2-adic-absolute-value)
      - [2-adic metric](#2-adic-metric)
    - [Ostrowski's theorem](#ostrowski-s-theorem)
      - [Non-Archimedean part of Ostrowski theorem](#non-archimedean-part-of-ostrowski-theorem)
      - [Non-Archimedean absolute values on a number field](#non-archimedean-absolute-values-on-a-number-field)
- [Local field](#local-field)
  - [p-adic field](#p-adic-field)
    - [Integral lattice in a p-adic vector space](#integral-lattice-in-a-p-adic-vector-space)
  - [Residue degree](#residue-degree)
    - [Absolute residue degree](#absolute-residue-degree)
  - [Local compactness criterion for a complete non-Archimedean field](#local-compactness-criterion-for-a-complete-non-archimedean-field)
    - [Digit expansion with a nonuniformizer](#digit-expansion-with-a-nonuniformizer)
    - [Completeness of locally compact nontrivially valued fields](#completeness-of-locally-compact-nontrivially-valued-fields)
    - [Discrete valuation from nontrivial local compactness](#discrete-valuation-from-nontrivial-local-compactness)
    - [Nontrivial valuation in the local compactness criterion](#nontrivial-valuation-in-the-local-compactness-criterion)
  - [Multiplicative group of a non-Archimedean local field](#multiplicative-group-of-a-non-archimedean-local-field)
    - [Principal-unit filtration of a local field](#principal-unit-filtration-of-a-local-field)
    - [Principal-unit group of a mixed-characteristic local field](#principal-unit-group-of-a-mixed-characteristic-local-field)
  - [Hensel's lemma](#hensel-s-lemma)
    - [Hensel lifting](#hensel-lifting)
    - [Coprime-factor Hensel lifting](#coprime-factor-hensel-lifting)
    - [Simple-root Hensel lifting by successive residues](#simple-root-hensel-lifting-by-successive-residues)
    - [Coprime factor lifting from valuation-extension uniqueness](#coprime-factor-lifting-from-valuation-extension-uniqueness)
    - [Elements that are powers of infinitely many degrees in a local field](#elements-that-are-powers-of-infinitely-many-degrees-in-a-local-field)
    - [Factorization of X4 plus 9X2 minus 2 over the 2-adic numbers](#factorization-of-x4-plus-9x2-minus-2-over-the-2-adic-numbers)
    - [Strong form of Hensel lemma](#strong-form-of-hensel-lemma)
      - [Newton iteration over a valued field](#newton-iteration-over-a-valued-field)
  - [Krasner's lemma](#krasner-s-lemma)
    - [Closest-root descent in a Galois extension](#closest-root-descent-in-a-galois-extension)
    - [Finiteness of fixed-degree extensions of a p-adic field](#finiteness-of-fixed-degree-extensions-of-a-p-adic-field)
    - [Continuity of roots over a non-Archimedean field](#continuity-of-roots-over-a-non-archimedean-field)
    - [Local realization as a completion of a number field](#local-realization-as-a-completion-of-a-number-field)
    - [Completion of an algebraic closure of a p-adic field is algebraically closed](#completion-of-an-algebraic-closure-of-a-p-adic-field-is-algebraically-closed)
  - [Weierstrass preparation theorem](#weierstrass-preparation-theorem)
    - [Distinguished polynomial](#distinguished-polynomial)
  - [Laurent series field](#laurent-series-field)
    - [Prescribed ramification and residue degree for a Laurent series field](#prescribed-ramification-and-residue-degree-for-a-laurent-series-field)
    - [Finite extensions of the complex Laurent series field](#finite-extensions-of-the-complex-laurent-series-field)
      - [Absolute Galois group of the complex Laurent series field](#absolute-galois-group-of-the-complex-laurent-series-field)
    - [Completion at an irreducible polynomial over a finite field](#completion-at-an-irreducible-polynomial-over-a-finite-field)
  - [p-adic exponential function](#p-adic-exponential-function)
    - [2-adic exponential](#2-adic-exponential)
    - [Radius of convergence of the p-adic exponential](#radius-of-convergence-of-the-p-adic-exponential)
    - [p-adic logarithm](#p-adic-logarithm)
      - [2-adic logarithm](#2-adic-logarithm)
      - [Logarithm isomorphism on deep principal units](#logarithm-isomorphism-on-deep-principal-units)
  - [Teichmüller character](#teichmuller-character)
    - [Teichmuller representative](#teichmuller-representative)
      - [Finite prime-power Teichmuller representative](#finite-prime-power-teichmuller-representative)
      - [Approximation of Teichmuller lifts by iterated pth powers](#approximation-of-teichmuller-lifts-by-iterated-pth-powers)
      - [Teichmuller lift properties](#teichmuller-lift-properties)
      - [Teichmuller expansion](#teichmuller-expansion)
        - [Equal-characteristic complete discretely valued field](#equal-characteristic-complete-discretely-valued-field)
          - [Finite coefficient field in positive-characteristic local fields](#finite-coefficient-field-in-positive-characteristic-local-fields)
  - [Unramified extension](#unramified-extension)
    - [Unramified extensions remain unramified under base change](#unramified-extensions-remain-unramified-under-base-change)
    - [Lifting residue-field embeddings of unramified extensions](#lifting-residue-field-embeddings-of-unramified-extensions)
    - [Unramified generator criterion with separable reduction](#unramified-generator-criterion-with-separable-reduction)
      - [Unramified residue generator integral basis](#unramified-residue-generator-integral-basis)
        - [Residue-basis norm formula for an unramified extension](#residue-basis-norm-formula-for-an-unramified-extension)
    - [Existence and uniqueness of unramified local extensions](#existence-and-uniqueness-of-unramified-local-extensions)
    - [Frobenius automorphism](#frobenius-automorphism)
      - [Frobenius conjugacy class](#frobenius-conjugacy-class)
        - [Frobenius permutation and roots modulo a prime](#frobenius-permutation-and-roots-modulo-a-prime)
    - [Maximal unramified extension](#maximal-unramified-extension)
    - [Maximal unramified subextension of a local field extension](#maximal-unramified-subextension-of-a-local-field-extension)
  - [Ramification group](#ramification-group)
    - [Positive ramification quotients are elementary abelian](#positive-ramification-quotients-are-elementary-abelian)
    - [Ramification of the splitting field of X3 plus pX plus p](#ramification-of-the-splitting-field-of-x3-plus-px-plus-p)
    - [Lower ramification filtration of a prime-power cyclotomic extension](#lower-ramification-filtration-of-a-prime-power-cyclotomic-extension)
    - [Lower ramification numbering](#lower-ramification-numbering)
      - [Herbrand function](#herbrand-function)
        - [Upper ramification numbering](#upper-ramification-numbering)
          - [Upper ramification groups commute with quotients](#upper-ramification-groups-commute-with-quotients)
    - [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)
      - [Ramification groups of the splitting field of T3 minus 2 over Q3](#ramification-groups-of-the-splitting-field-of-t3-minus-2-over-q3)
      - [Ramification groups of the eighth-root cyclotomic extension of the 2-adic field](#ramification-groups-of-the-eighth-root-cyclotomic-extension-of-the-2-adic-field)
      - [Ramification break of an Artin–Schreier pole](#ramification-break-of-an-artin-schreier-pole)
      - [Ramification groups of the splitting field of T3 minus 3T plus 3 over Q3](#ramification-groups-of-the-splitting-field-of-t3-minus-3t-plus-3-over-q3)
      - [Ramification groups of the splitting field of Xp minus p over the p-adic numbers](#ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers)
        - [Eisenstein sextic presentation of the splitting field of X3 minus 3 over Q3](#eisenstein-sextic-presentation-of-the-splitting-field-of-x3-minus-3-over-q3)
    - [Tame inertia quotient](#tame-inertia-quotient)
      - [Branch-cycle conjugacy class](#branch-cycle-conjugacy-class)
        - [Quadratic branch parity criterion](#quadratic-branch-parity-criterion)
      - [Uniformizer character of inertia](#uniformizer-character-of-inertia)
    - [Different ideal](#different-ideal)
      - [Different exponent](#different-exponent)
        - [Cyclotomic local different exponent](#cyclotomic-local-different-exponent)
        - [Different exponent and tame ramification](#different-exponent-and-tame-ramification)
      - [Inverse different](#inverse-different)
      - [Different in a tower](#different-in-a-tower)
      - [Different exponent from ramification groups](#different-exponent-from-ramification-groups)
    - [Inertia group](#inertia-group)
      - [Wild inertia group](#wild-inertia-group)
    - [Tamely ramified extension](#tamely-ramified-extension)
      - [Discriminant exponent of a tame Galois extension](#discriminant-exponent-of-a-tame-galois-extension)
    - [Ramification-group sum for a monogenic integer ring](#ramification-group-sum-for-a-monogenic-integer-ring)
  - [Eisenstein polynomial](#eisenstein-polynomial)
    - [Shifted Eisenstein polynomial](#shifted-eisenstein-polynomial)
    - [Ramification polynomial](#ramification-polynomial)
      - [Reduced ramification polynomial](#reduced-ramification-polynomial)
        - [Ramification breaks from a reduced ramification polygon](#ramification-breaks-from-a-reduced-ramification-polygon)
  - [Newton polygon](#newton-polygon)
    - [Reflected Newton polygon convention](#reflected-newton-polygon-convention)
    - [Newton polygon root valuation theorem](#newton-polygon-root-valuation-theorem)
    - [Denominator criterion for Newton polygon irreducibility](#denominator-criterion-for-newton-polygon-irreducibility)
  - [Ramification index](#ramification-index)
    - [Ramification forced by a coprime root valuation](#ramification-forced-by-a-coprime-root-valuation)
    - [Residue-field degree](#residue-field-degree)
    - [Totally ramified extension](#totally-ramified-extension)
      - [Unramified base change preserves total ramification](#unramified-base-change-preserves-total-ramification)
        - [Cyclic quartic local extension without a totally ramified complement](#cyclic-quartic-local-extension-without-a-totally-ramified-complement)
      - [Eisenstein generator of a totally ramified extension](#eisenstein-generator-of-a-totally-ramified-extension)
  - [p-adic unit](#p-adic-unit)
    - [Unit square classes of the p-adic integers](#unit-square-classes-of-the-p-adic-integers)
    - [2-adic unit](#2-adic-unit)
      - [Digit lifting for square roots of 2-adic units](#digit-lifting-for-square-roots-of-2-adic-units)
      - [Square-class group of the 2-adic numbers](#square-class-group-of-the-2-adic-numbers)
        - [Quadratic extensions of the 2-adic numbers](#quadratic-extensions-of-the-2-adic-numbers)
          - [Ramification in the quadratic extension generated by the square root of two](#ramification-in-the-quadratic-extension-generated-by-the-square-root-of-two)
    - [pth-power criterion for p-adic units](#pth-power-criterion-for-p-adic-units)
    - [Principal unit](#principal-unit)
      - [Prime-to-residue-characteristic power map on principal units](#prime-to-residue-characteristic-power-map-on-principal-units)
      - [Higher principal-unit group](#higher-principal-unit-group)
        - [Successive quotients of principal-unit groups](#successive-quotients-of-principal-unit-groups)
        - [Cube map on 3-adic principal units](#cube-map-on-3-adic-principal-units)
      - [Principal-unit logarithm](#principal-unit-logarithm)
    - [Cube-class group of the 3-adic numbers](#cube-class-group-of-the-3-adic-numbers)
  - [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)
    - [Valuation of a primitive p-power root of unity](#valuation-of-a-primitive-p-power-root-of-unity)
      - [Roots of unity at the tame ramification boundary](#roots-of-unity-at-the-tame-ramification-boundary)
    - [Ramification bound for a primitive pth root of unity](#ramification-bound-for-a-primitive-pth-root-of-unity)
    - [Roots of unity in the p-adic numbers](#roots-of-unity-in-the-p-adic-numbers)
    - [Unit decomposition of the 2-adic Gaussian field](#unit-decomposition-of-the-2-adic-gaussian-field)
    - [Unit group of Q3 zeta3](#unit-group-of-q3-zeta3)
  - [Lubin–Tate formal group](#lubin-tate-formal-group)
    - [Lubin–Tate series](#lubin-tate-series)
    - [Lubin–Tate change of series](#lubin-tate-change-of-series)
      - [Lubin–Tate functional equation lemma](#lubin-tate-functional-equation-lemma)
    - [Lubin–Tate torsion](#lubin-tate-torsion)
      - [Lubin–Tate extension](#lubin-tate-extension)
        - [Lubin–Tate cyclotomic example](#lubin-tate-cyclotomic-example)
        - [Lubin–Tate tower](#lubin-tate-tower)
        - [Lubin–Tate Galois action on primitive torsion](#lubin-tate-galois-action-on-primitive-torsion)
      - [Eisenstein layers of Lubin–Tate torsion](#eisenstein-layers-of-lubin-tate-torsion)
      - [First Lubin–Tate torsion fields for the p-adic numbers](#first-lubin-tate-torsion-fields-for-the-p-adic-numbers)
  - [Maximal abelian extension](#maximal-abelian-extension)
    - [Weil group](#weil-group)
      - [Relative Weil group](#relative-weil-group)
        - [Weil-group topology](#weil-group-topology)
    - [Cyclotomic extension of a p-adic field](#cyclotomic-extension-of-a-p-adic-field)
      - [Total ramification criterion for local cyclotomic extensions](#total-ramification-criterion-for-local-cyclotomic-extensions)
    - [Local Kronecker-Weber theorem](#local-kronecker-weber-theorem)
    - [Local class field theory](#local-class-field-theory)
      - [Existence theorem of local class field theory](#existence-theorem-of-local-class-field-theory)
      - [Local Artin reciprocity](#local-artin-reciprocity)
        - [Hilbert norm residue symbol](#hilbert-norm-residue-symbol)
          - [Quadratic Hilbert symbol](#quadratic-hilbert-symbol)
            - [Explicit quadratic Hilbert symbols over the p-adic numbers](#explicit-quadratic-hilbert-symbols-over-the-p-adic-numbers)
            - [Hilbert-symbol annihilators of units and unramified square classes](#hilbert-symbol-annihilators-of-units-and-unramified-square-classes)
            - [Hilbert reciprocity law](#hilbert-reciprocity-law)
        - [Local Artin map](#local-artin-map)
          - [Cup-product construction of local reciprocity](#cup-product-construction-of-local-reciprocity)
          - [Lubin–Tate description of local reciprocity](#lubin-tate-description-of-local-reciprocity)
        - [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)
          - [Surjectivity of unit norms in unramified extensions](#surjectivity-of-unit-norms-in-unramified-extensions)
          - [Cyclic local norm index](#cyclic-local-norm-index)
          - [Norm-unit index in an abelian local extension](#norm-unit-index-in-an-abelian-local-extension)
          - [Norm units in a tamely totally ramified extension](#norm-units-in-a-tamely-totally-ramified-extension)
          - [Norm subgroup of a 2-power cyclotomic extension of the 2-adic numbers](#norm-subgroup-of-a-2-power-cyclotomic-extension-of-the-2-adic-numbers)

## Continuous functions on the p-adic integers

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)

The [continuous functions](calculus.md#continuous-function) from the [p-adic integers](number-theory.md#p-adic-integer) to the [P-adic numbers](#p-adic-number) form a [Banach space](banach-space.md) over $\mathbb Q_p$ with [supremum norm](normed-vector-space.md#supremum-norm) $\|f\|_\infty=\sup_{x\in\mathbb Z_p}|f(x)|_p$. Compactness of the domain bounds the norm, and [uniform convergence](sequence-and-series.md#uniform-convergence) in the complete codomain proves completeness. Translation and the [forward difference operator](finite-difference.md#forward-difference-operator) $\Delta f(x)=f(x+1)-f(x)$ are bounded operators, with $\|\Delta f\|_\infty\leq\|f\|_\infty$.

<h3 id="mahler-s-theorem">Mahler's theorem</h3>

↑ **Parent:** [Continuous functions on the p-adic integers](#continuous-functions-on-the-p-adic-integers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mahler's_theorem)

Every function in [continuous functions on the p-adic integers](#continuous-functions-on-the-p-adic-integers) has a unique uniformly convergent expansion in the [binomial polynomials](commutative-algebra.md#binomial-polynomial), with $a_n\to0$ and $a_n=(\Delta^nf)(0)$. Conversely, any coefficient sequence tending to zero defines such a [continuous function](calculus.md#continuous-function). To prove the expansion once $a_n\to0$ is known, use $|\binom xn|_p\leq1$ for uniform convergence. Finite binomial inversion gives agreement with $f$ at each nonnegative integer, and density gives agreement everywhere. The coefficients recover successively from these integer values, proving uniqueness. Moreover $\|f\|_\infty=\sup_n|a_n|_p$, because finite differences bound each coefficient by the norm and the expansion gives the reverse inequality.

#### Discrete antidifferentiation on the p-adic integers

↑ **Parent:** [Mahler's theorem](#mahler-s-theorem)

The [Mahler coefficients](#mahler-coefficient) tend to zero, so the displayed series defines a [continuous function](calculus.md#continuous-function) and has value zero at zero. The [Pascal's identity](binomial-coefficient.md#pascal-s-rule) and uniform convergence give $\Delta Jf=f$. Thus the [forward difference operator](finite-difference.md#forward-difference-operator) is surjective on [continuous functions on the p-adic integers](#continuous-functions-on-the-p-adic-integers). Its kernel consists of constants: period one implies agreement on the dense nonnegative integers, and [continuity](calculus.md#continuous-function) then implies constancy. This selects the unique [discrete antiderivative](finite-difference.md#discrete-antiderivative) vanishing at zero.

There is also a direct construction on [locally constant functions](calculus.md#locally-constant-function). If $h$ has period $M=p^r$, put $a_j=h(j)$, $S=\sum_{i=0}^{M-1}a_i$, and $P_j=\sum_{i<j}a_i$. For $x=j+My$ with $0\le j<M$ and $y\in\mathbb Z_p$, set

$$
Jh(x)=yS+P_j.
$$

This is a [continuous function](calculus.md#continuous-function) on each residue class. Increasing $j$ gives $Jh(x+1)-Jh(x)=a_j$; at $j=M-1$, the next point has residue zero and quotient $y+1$, giving the same identity. The [ultrametric inequality](#ultrametric-inequality) gives $\|Jh\|_\infty\le\|h\|_\infty$, and $Jh(0)=0$. The construction is independent of the chosen period, since two normalized [discrete antiderivatives](finite-difference.md#discrete-antiderivative) agree on the nonnegative integers and then on the [p-adic integers](number-theory.md#p-adic-integer) by [continuity](calculus.md#continuous-function). It is linear on the [locally constant functions](calculus.md#locally-constant-function), which form a [dense subset](topology.md#dense-set) in the [supremum norm](normed-vector-space.md#supremum-norm). Completeness therefore extends it to every [continuous function](calculus.md#continuous-function), retaining $\Delta J=I$ and the norm bound. This proves surjectivity without first using the [Mahler theorem](#mahler-s-theorem).

##### Translation-invariant linear forms on p-adic continuous functions vanish

↑ **Parent:** [Discrete antidifferentiation on the p-adic integers](#discrete-antidifferentiation-on-the-p-adic-integers)

Let $T:\mathcal C(\mathbb Z_p,\mathbb Q_p)\to\mathbb Q_p$ be linear and invariant under translation by one. For any $f$, choose its continuous [discrete antiderivative](finite-difference.md#discrete-antiderivative) $Jf$. Then $T(f)=T(\Delta Jf)=T(Jf(\cdot+1))-T(Jf)=0$. No [continuity](calculus.md#continuous-function) or boundedness of $T$ is assumed. In particular this applies to a form invariant under every translation by a [p-adic integer](number-theory.md#p-adic-integer).

#### Mahler coefficient

↑ **Parent:** [Mahler's theorem](#mahler-s-theorem)

For a [continuous function](calculus.md#continuous-function) $f:\mathbb Z_p\to\mathbb Q_p$, its nth Mahler coefficient is

$$
a_n=\sum_{j=0}^n(-1)^{n-j}\binom nj f(j).
$$

This is the explicit iterate of the [forward difference operator](finite-difference.md#forward-difference-operator). These coefficients are exactly those of its [Mahler expansion](#mahler-s-theorem).

##### Mahler coefficient exponential generating function

↑ **Parent:** [Mahler coefficient](#mahler-coefficient)

For the [Mahler coefficients](#mahler-coefficient) of a [continuous function](calculus.md#continuous-function) on the [p-adic integers](number-theory.md#p-adic-integer), finite [binomial inversion](binomial-coefficient.md#binomial-inversion) gives $c_n=\sum_{j=0}^n(-1)^{n-j}\binom njf(j)$. Equivalently their exponential generating function is the displayed identity in the formal power-series ring $\mathbb Q_p[[T]]$. Each coefficient involves only finitely many terms; no claim of convergence for every $p$-adic value of $T$ is needed.

##### Mahler expansion of the parity function

↑ **Parent:** [Mahler coefficient](#mahler-coefficient)

The [locally constant function](calculus.md#locally-constant-function) equal to one on $2\mathbb Z_2$ and minus one on its other coset has [Mahler coefficients](#mahler-coefficient) $a_n=(-2)^n$: at nonnegative integers its values are $(-1)^j$, so the [forward difference operator](finite-difference.md#forward-difference-operator) multiplies it by $-2$. Since $|a_n|_2=2^{-n}$ and the [binomial polynomials](commutative-algebra.md#binomial-polynomial) have absolute value at most one on the [2-adic integers](number-theory.md#2-adic-integer), the series converges uniformly. The [binomial theorem](binomial-coefficient.md#binomial-theorem) verifies its values on the nonnegative integers, and [continuity](calculus.md#continuous-function) extends the identity to the entire domain.

##### Automatic decay of Mahler coefficients

↑ **Parent:** [Mahler coefficient](#mahler-coefficient)

Approximate a [continuous function](calculus.md#continuous-function) on $\mathbb Z_p$ uniformly by a function constant on residue classes modulo $p^r$. On this finite space, translation $S$ satisfies $S^{p^r}=I$, so $\Delta^{p^r}=(S-I)^{p^r}$ has every matrix coefficient divisible by $p$. Hence $\|\Delta^{jp^r}\|\leq p^{-j}$, and the [Mahler coefficients](#mahler-coefficient) of a locally constant function tend to zero. Since $|a_n(f)-a_n(g)|_p\leq\|f-g\|_\infty$, uniform approximation proves the assertion for every [continuous function](calculus.md#continuous-function). This completes the coefficient-decay part of the [Mahler theorem](#mahler-s-theorem).

## Non-Archimedean ordered field

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-Archimedean_ordered_field)

A non-Archimedean ordered field contains elements larger than every positive integer, equivalently positive infinitesimals smaller than every positive rational number.

## Absolute value (algebra)

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolute_value_(algebra))

An absolute value on a field is a nonnegative multiplicative function that vanishes only at zero and satisfies the triangle inequality.

### Weak approximation for inequivalent absolute values

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

For finitely many pairwise inequivalent nontrivial [absolute values on a field](#absolute-value-algebra), an element of the field can approximate independently prescribed targets in the associated [completion of a valued field](#completion-of-a-valued-field) at each place to arbitrary positive accuracies. Equivalently the diagonal map has dense image in the finite product. Requiring finitely many inequivalent places is essential; the conclusion controls finitely many inequalities, not infinitely many independently prescribed bounds at once, or incompatible targets at one place. [Weak approximation for number fields](algebraic-number-theory.md#weak-approximation-for-number-fields) is the class-field-theoretic instance.

### Bounded comparison forces equality of multiplicative absolute values

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

If two multiplicative [absolute values on a field](#absolute-value-algebra) satisfy a comparison with fixed positive constants $c,C$, apply it to $x^n$ and take $n$th roots. Letting $n\to\infty$ eliminates both constants. This stronger bounded comparison differs from equivalence merely as topologies: replacing an absolute value by its square generally preserves topology but not equality.

### Completion of a valued field

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

The metric completion of a [field](algebra.md#field) for an [absolute value on a field](#absolute-value-algebra) is formed from Cauchy sequences modulo sequences tending to zero. Addition and multiplication extend continuously, and every nonzero completed element is invertible, so the result remains a [field](algebra.md#field). The [absolute value on a field](#absolute-value-algebra) extends uniquely. A place of a [number field](algebraic-number-theory.md#number-field) determines the corresponding completion $K_v$.

#### Algebraic closure of the p-adic numbers is not complete

↑ **Parent:** [Completion of a valued field](#completion-of-a-valued-field)

Choose compatible primitive [roots of unity](algebra.md#root-of-unity) $\zeta_{p^{n+1}}$. The partial sums $A_N=\sum_{n=0}^Np^{2n}\zeta_{p^{n+1}}$ form a [Cauchy sequence](sequence-and-series.md#cauchy-sequence). Each $A_N$ generates $\mathbb Q_p(\zeta_{p^{N+1}})$: for a nonidentity cyclotomic automorphism with $r=v_p(a-1)$, the first changed term has valuation $2r+1/(p-1)$, strictly below every later changed term. Thus the conjugate distance is at least $p^{-2N-1/(p-1)}$. The tail bound is $p^{-2N-2}$, strictly smaller. If the limit were algebraic, [Krasner's lemma](#krasner-s-lemma) would place every one of these unbounded-degree cyclotomic fields in one finite extension, a contradiction.

### Trivial absolute value

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

The trivial [absolute value on a field](#absolute-value-algebra) is zero at zero and one elsewhere. Its metric [topology](topology.md) is discrete. Its [valuation ring](commutative-algebra.md#valuation-ring) and [residue field](commutative-algebra.md#residue-field) are both the field itself. This is why rational absolute-value classification and nontrivial discrete-value compactness criteria need a nontriviality hypothesis.

### Non-Archimedean absolute value

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

A non-Archimedean absolute value satisfies the ultrametric inequality $|x+y|\leq\max(|x|,|y|)$.

#### Integer criterion for a non-Archimedean absolute value

↑ **Parent:** [Non-Archimedean absolute value](#non-archimedean-absolute-value)

An [absolute value on a field](#absolute-value-algebra) is non-Archimedean if and only if $|n\cdot1|\le1$ for every positive integer $n$. Necessity follows from the [ultrametric inequality](#ultrametric-inequality). Conversely the binomial theorem gives $|x+y|^m\le(m+1)\max(|x|,|y|)^m$, since every binomial coefficient has absolute value at most one. Take $m$th roots and let $m\to\infty$. In particular an [extension of an absolute value](#extension-of-an-absolute-value) that is non-Archimedean stays non-Archimedean.

#### Bounded-integer criterion for a non-Archimedean absolute value

↑ **Parent:** [Non-Archimedean absolute value](#non-archimedean-absolute-value)

An absolute value on a field is non-Archimedean exactly when its values on the image of $\mathbb Z$ are bounded. The reverse implication follows by applying the ordinary triangle inequality to the binomial expansion of $(x+y)^n$ and taking $n$th roots as $n\to\infty$.

#### Ultrametric inequality

↑ **Parent:** [Non-Archimedean absolute value](#non-archimedean-absolute-value)

The ultrametric inequality, also called the strong [triangle inequality](topological-analysis.md#triangle-inequality), bounds a direct distance by the larger of the two distances through an intermediate point:

$$
d(x,z)\leq\max\{d(x,y),d(y,z)\}.
$$

A [metric space](topological-analysis.md#metric-space) satisfying this rule is an [ultrametric space](#ultrametric-space). For a [Non-Archimedean absolute value](#non-archimedean-absolute-value), the corresponding [inequality](arithmetic.md#inequality-mathematics) is $|a+b|\leq\max\{|a|,|b|\}$, and the associated [metric](topological-analysis.md#metric) is $d(x,y)=|x-y|$. The ordinary [triangle inequality](topological-analysis.md#triangle-inequality) follows because the maximum of two nonnegative [real numbers](arithmetic.md#real-number) is at most their [sum](arithmetic.md#sum).

For example, the [2-adic absolute value](#2-adic-absolute-value) gives the three points $0,1,8$ distances

$$
d_2(0,1)=1,\qquad d_2(1,8)=|-7|_2=1,\qquad d_2(0,8)=\frac18.
$$

Each distance is bounded by the maximum of the other two. The two largest distances are equal: every triangle in an [ultrametric space](#ultrametric-space) has this property. Otherwise its unique longest side would exceed the maximum of the other two, contradicting the [ultrametric inequality](#ultrametric-inequality). The drawn lengths of a triangle on paper need not represent these distances.

The [ultrametric inequality](#ultrametric-inequality) gives a useful exact rule when $|a|\ne|b|$:

$$
|a+b|=\max\{|a|,|b|\}.
$$

To see why, suppose $|a|>|b|$. The upper bound is $|a+b|\leq|a|$; applying the [ultrametric inequality](#ultrametric-inequality) to $a=(a+b)-b$ forces the reverse bound. Equal sizes can instead cancel: $|1|_2=|1|_2=1$, but $|1+1|_2=1/2$. This makes a uniquely largest term decisive in a [sum](arithmetic.md#sum), a principle used in the [Newton polygon](#newton-polygon) and in arguments about [roots of a polynomial](polynomial.md#root-of-a-polynomial).

##### Ultrametric space

↑ **Parent:** [Ultrametric inequality](#ultrametric-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrametric_space)

An ultrametric space is a [metric space](topological-analysis.md#metric-space) whose [metric](topological-analysis.md#metric) satisfies the [ultrametric inequality](#ultrametric-inequality). The [rational numbers](number-theory.md#rational-number) with $d_p(x,y)=|x-y|_p$, and their [P-adic number](#p-adic-number) completion, are examples. Their geometry organizes points into nested clusters rather than measuring separation along a [number line](arithmetic.md#number-line).

For [integers](integer.md) $a,b$ and $k\geq0$, the definition of the [P-adic valuation](number-theory.md#p-adic-valuation) gives

$$
d_p(a,b)\leq p^{-k}\quad\Longleftrightarrow\quad a\equiv b\pmod{p^k}.
$$

Thus a [closed ball](topological-analysis.md#closed-ball) of radius $p^{-k}$ in the [integers](integer.md) is a [congruence class](modular-arithmetic.md#congruence-class) modulo $p^k$. In the [p-adic integers](number-theory.md#p-adic-integer) the same [closed ball](topological-analysis.md#closed-ball) is $a+p^k\mathbb Z_p$. More shared low-order digits mean a smaller [p-adic absolute value](#p-adic-absolute-value) of the difference.

<a id="image-the-integers-from-zero-to-fifteen-form-nested-congruence-classes-modulo-powers-of-two-in-the-2-adic-absolute-value"></a>
![](two-adic-congruence-clusters.png)

**[Figure 1](#image-the-integers-from-zero-to-fifteen-form-nested-congruence-classes-modulo-powers-of-two-in-the-2-adic-absolute-value). The integers from zero to fifteen form nested congruence classes modulo powers of two in the 2-adic absolute value**.

The [binary tree](data-structure.md#binary-tree) first splits the sixteen [integers](integer.md) into even and odd [congruence classes](modular-arithmetic.md#congruence-class), then refines modulo $4$, $8$, and $16$. Each node fixes one more low-order digit. The leaves $5$ and $13$ share the class $5$ modulo $8$, then separate modulo $16$, so their distance is exactly $1/8$. The leaves are deliberately ordered by their low-order digits; horizontal spacing and edge lengths are layout choices, not the [metric](topological-analysis.md#metric). The singleton leaves describe this finite sample; a [congruence class](modular-arithmetic.md#congruence-class) modulo $16$ in all [p-adic integers](number-theory.md#p-adic-integer) remains infinite.

The [ultrametric inequality](#ultrametric-inequality) also explains the unusual behavior of [balls](topological-analysis.md#ball-mathematics). Every point of an [open ball](topology.md#open-ball) can serve as its center: if $d(a,b)<r$, then $d(a,x)<r$ if and only if $d(b,x)<r$. Two [open balls](topology.md#open-ball) that intersect are nested, since a point of their [intersection](set.md#set-intersection) serves as a common center and their radii can be compared. The same nesting rule holds for [closed balls](topological-analysis.md#closed-ball) and for a pair consisting of one [open ball](topology.md#open-ball) and one [closed ball](topological-analysis.md#closed-ball).

Every [open ball](topology.md#open-ball) is a [clopen set](topology.md#clopen-set). For a point $y$ outside $B(a,r)$, the [open ball](topology.md#open-ball) $B(y,d(a,y))$ stays outside $B(a,r)$: if $d(y,z)<d(a,y)$, the [ultrametric inequality](#ultrametric-inequality) forces $d(a,z)=d(a,y)\geq r$. Hence the complement is an [open set](topology.md#open-set). Also every [closed ball](topological-analysis.md#closed-ball) of positive radius is an [open set](topology.md#open-set), because $B(b,r)$ lies in the [closed ball](topological-analysis.md#closed-ball) of radius $r$ around $a$ whenever $d(a,b)\leq r$. A radius-zero [closed ball](topological-analysis.md#closed-ball) is a singleton and need not be an [open set](topology.md#open-set). Distinct points can therefore be separated by a [clopen set](topology.md#clopen-set), proving that an [ultrametric space](#ultrametric-space) is [totally disconnected](#totally-disconnected-space). These ball properties turn distance thresholds into a hierarchy of compatible clusters. [Andrew V. Sutherland, Number Theory I, Lecture 8, section 8.1.1](https://math.mit.edu/classes/18.785/2021fa/LectureNotes8.pdf)

###### Totally disconnected space

↑ **Parent:** [Ultrametric space](#ultrametric-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_disconnected_space)

A topological space is totally disconnected when its only connected subsets are singletons.

### Equivalent absolute values

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

Two nontrivial [absolute values on a field](#absolute-value-algebra) are equivalent when they induce the same [topology](topology.md). Equivalently, one is a positive real power of the other.

### Extension of an absolute value

↑ **Parent:** [Absolute value (algebra)](#absolute-value-algebra)

For a [field extension](algebra.md#field-extension) $L/K$, an extension of an absolute value $|\cdot|$ on $K$ is an absolute value on $L$ whose restriction to $K$ is $|\cdot|$.

#### Unique extension of an absolute value to a finite extension

↑ **Parent:** [Extension of an absolute value](#extension-of-an-absolute-value)

If $K$ is complete and $L/K$ is finite, an absolute value on $K$ extends uniquely to $L$. With the normalization that it restricts exactly to the given absolute value,

$$
|x|_L=|N_{L/K}(x)|^{1/[L:K]}.
$$

Every $K$-automorphism of $L$ preserves this extended absolute value.

##### Finite-dimensional non-Archimedean norm equivalence over a complete field

↑ **Parent:** [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)

Let $K$ be complete for a [Non-Archimedean absolute value](#non-archimedean-absolute-value) and let $V$ be a finite-dimensional [vector space](vector-space.md) with a norm satisfying $\|av\|=|a|\|v\|$ and the [ultrametric inequality](#ultrametric-inequality). All such norms are equivalent to the maximum of coordinates in any [basis](vector-space.md#basis). The upper bound is immediate. For the lower bound, induct on dimension. The span $W$ of all but the last [basis](vector-space.md#basis) vector is complete by induction, hence closed for the given norm. Thus $\delta=\inf_{w\in W}\|e_n-w\|>0$. For $v=w+ae_n$, $\|v\|\geq |a|\delta$; also $\|w\|\leq\max(\|v\|,|a|\|e_n\|)$. The induction bound on coordinates of $w$ now bounds all coordinates by a constant times $\|v\|$. This proof needs no [local compactness](topology.md#locally-compact-space).

##### Compact-sphere proof of finite-dimensional non-Archimedean norm equivalence

↑ **Parent:** [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)

On a finite-dimensional vector space over $\mathbb Q_p$, the triangle inequality gives an upper bound by a coordinate maximum norm. The coordinate unit sphere is compact. The other norm is continuous and nonzero there, so has a positive minimum. Scaling by powers of $p$ gives the lower bound. The resulting [equivalence of norms in finite dimensions](topological-vector-space.md#equivalence-of-norms-in-finite-dimensions) proves completeness of finite extensions, and applying the comparison to powers of a field element proves equality of two extending multiplicative [absolute values on a field](#absolute-value-algebra).

##### Pure-power reduction of a monic irreducible polynomial

↑ **Parent:** [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)

Suppose a [Non-Archimedean absolute value](#non-archimedean-absolute-value) extends uniquely to every finite extension. If $f\in\mathcal O_K[X]$ is [monic](polynomial.md#monic-polynomial) and irreducible, every root has absolute value at most one: otherwise its leading power dominates all lower terms, contradicting $f(\alpha)=0$ by the [ultrametric inequality](#ultrametric-inequality). In a [splitting field](galois-theory.md#splitting-field), let $\varphi$ be the [minimal polynomial of an algebraic element](galois-theory.md#minimal-polynomial-of-an-algebraic-element) of the residue of one root. Lift its coefficients to $\mathcal O_K$. The lift has absolute value less than one at that root and hence, by [equal absolute values of algebraic conjugates](#equal-absolute-values-of-algebraic-conjugates), at every root. Consequently every root residue is a zero of $\varphi$. Since reduction preserves the product of the linear factors with multiplicities, every irreducible factor of $\overline f$ is $\varphi$, proving the displayed identity for some $m\geq1$.

##### Equal absolute values of algebraic conjugates

↑ **Parent:** [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)

Suppose a [Non-Archimedean absolute value](#non-archimedean-absolute-value) on $K$ has a unique extension to every finite [field extension](algebra.md#field-extension). Any K-isomorphism $K(\alpha_i)\to K(\alpha_j)$ between conjugate roots pulls the absolute value back to an extension on the source field, which must be the given one. Thus $|h(\alpha_i)|=|h(\alpha_j)|$ for every $h\in K[X]$. This argument includes inseparable [irreducible polynomials](polynomial.md#irreducible-polynomial): no transitive Galois action or completeness assumption is needed.

##### Integral closure in a finite extension of a complete discretely valued field

↑ **Parent:** [Unique extension of an absolute value to a finite extension](#unique-extension-of-an-absolute-value-to-a-finite-extension)

Let $K$ be complete for a discrete valuation and let $L/K$ be finite. The valuation ring $\mathcal O_L$ is exactly the integral closure of $\mathcal O_K$ in $L$. One direction follows from a monic integral equation; for the other, the coefficients of the minimal polynomial are elementary symmetric polynomials in conjugates of absolute value at most one.

#### Conjugacy of extensions of a valuation to a normal extension

↑ **Parent:** [Extension of an absolute value](#extension-of-an-absolute-value)

If $L/K$ is a finite normal extension, the Galois group acts transitively on the absolute values of $L$ extending a fixed absolute value of $K$. For number fields, this is equivalent to transitivity on the prime ideals above a fixed prime.

#### Valuation ring need not equal the integral closure over a noncomplete field

↑ **Parent:** [Extension of an absolute value](#extension-of-an-absolute-value)

Give $\mathbb Q$ its $5$-adic valuation, take $L=\mathbb Q(i)$, and choose the extension associated with the prime $(2+i)$. Then $(2+i)/(2-i)$ lies in the chosen valuation ring but has negative valuation at the conjugate prime. It is therefore not in the integral closure of $\mathbb Z_{(5)}$ in $L$.

#### Local factorization and extended absolute values

↑ **Parent:** [Extension of an absolute value](#extension-of-an-absolute-value)

If $L=K(\alpha)$ is a finite separable extension and $v$ is an absolute value on $K$, the extensions of $v$ to $L$ correspond to the irreducible factors of the minimal polynomial of $\alpha$ over the completion of $K$ at $v$.

##### Local prime decomposition of T5 plus 6T3 plus 252T2 plus 126

↑ **Parent:** [Local factorization and extended absolute values](#local-factorization-and-extended-absolute-values)

This polynomial is [Eisenstein](commutative-algebra.md#eisenstein-criterion) at $2$. Over $\mathbb Q_3$, its [Newton polygon](#newton-polygon) has a single slope $-2/5$, so it is irreducible and a root generates a totally ramified extension of degree five. Over $\mathbb Q_7$, its factor degrees are $1,1,3$: the simple residue roots $1,-1$ lift, and the remaining roots have valuation $1/3$. Thus the degree-five [number field](algebraic-number-theory.md#number-field) generated by a root has one prime above $3$ and three above $7$.

##### Prime ideals and local embedding orbits

↑ **Parent:** [Local factorization and extended absolute values](#local-factorization-and-extended-absolute-values)

For a finite extension of [number fields](algebraic-number-theory.md#number-field) $L/K$ and a nonzero [prime ideal](commutative-algebra.md#prime-ideal) $\mathfrak p$ of $K$, the primes of $L$ above $\mathfrak p$ correspond to the orbits of

$$
\operatorname{Gal}(\overline K_{\mathfrak p}/K_{\mathfrak p})\quad\text{on}\quad\operatorname{Hom}_K(L,\overline K_{\mathfrak p}).
$$

An embedding determines a prime by pulling back the local [absolute value on a field](#absolute-value-algebra). Embeddings with the same prime extend to embeddings of the same completion and are conjugate. If $L=K(\alpha)$, these orbits are the irreducible factors of its [minimal polynomial](linear-operator-theory.md#minimal-polynomial) over $K_{\mathfrak p}$.

##### Completion of a number field at a prime ideal

↑ **Parent:** [Local factorization and extended absolute values](#local-factorization-and-extended-absolute-values)

For a [number field](algebraic-number-theory.md#number-field) $K$ and a nonzero [prime ideal](commutative-algebra.md#prime-ideal) $\mathfrak p\subset\mathcal O_K$, the completion $K_{\mathfrak p}$ is the completion for the $\mathfrak p$-adic absolute value. It is a finite extension of $\mathbb Q_p$, where $p\mathbb Z=\mathfrak p\cap\mathbb Z$.

###### p-adic tensor decomposition of a number field

↑ **Parent:** [Completion of a number field at a prime ideal](#completion-of-a-number-field-at-a-prime-ideal)

For a [number field](algebraic-number-theory.md#number-field) $K$ and a rational prime $p$, the natural diagonal map gives an isomorphism of $\mathbb Q_p$-algebras

$$
K\otimes_{\mathbb Q}\mathbb Q_p\cong\prod_{\mathfrak p\mid p}K_{\mathfrak p}.
$$

###### Transitivity of the Galois action on primes

↑ **Parent:** [Completion of a number field at a prime ideal](#completion-of-a-number-field-at-a-prime-ideal)

If $L/K$ is a finite Galois extension of number fields, its Galois group acts transitively on the prime ideals of $\mathcal O_L$ lying above a fixed prime ideal of $\mathcal O_K$.

###### Decomposition group

↑ **Parent:** [Transitivity of the Galois action on primes](#transitivity-of-the-galois-action-on-primes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decomposition_group)

For a prime $\mathcal P$ of a finite Galois extension $L/K$ above $\mathfrak p$, the decomposition group is the stabilizer

$$
G_{\mathcal P/\mathfrak p}
=\{\sigma\in\operatorname{Gal}(L/K):\sigma\mathcal P=\mathcal P\}.
$$

###### Surjectivity of decomposition group reduction

↑ **Parent:** [Decomposition group](#decomposition-group)

For a finite [Galois extension](galois-theory.md#finite-galois-extension) of [number fields](algebraic-number-theory.md#number-field), choose a nonzero [residue field](commutative-algebra.md#residue-field) generator at $\mathfrak q$ and lift it to an integral element $a$ whose residues at the other primes above $\mathfrak p$ are zero, using the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem). The orbit polynomial $\prod_{\sigma\in G}(T-\sigma a)$ has coefficients in the base [ring of integers](algebraic-number-theory.md#ring-of-integers). Modulo $\mathfrak q$, its nonzero roots are precisely the orbit of $\overline a$ under the [decomposition group](#decomposition-group). Its coefficients belong to $k_{\mathfrak p}$, so [finite-field Frobenius automorphism](algebra.md#finite-field-frobenius-automorphism) permutes these roots. Consequently some decomposition-group element acts as Frobenius on the generator, and therefore on the entire [residue field](commutative-algebra.md#residue-field). Frobenius generates the finite-field [Galois group](galois-theory.md#galois-group), proving surjectivity.

###### Primes in an intermediate field as double cosets

↑ **Parent:** [Decomposition group](#decomposition-group)

Let $M/K$ be a finite [Galois extension](galois-theory.md#finite-galois-extension), $L=M^H$, and $D$ the [decomposition group](#decomposition-group) of a prime $\mathfrak P$ above $\mathfrak p$. The bijection

$$
H\backslash G/D\longrightarrow\{\mathfrak q\subset\mathcal O_L:\mathfrak q\mid\mathfrak p\},\qquad HgD\longmapsto g\mathfrak P\cap\mathcal O_L
$$

follows from transitivity on primes for both $M/K$ and $M/L$.

###### Complete splitting is preserved by Galois closure

↑ **Parent:** [Primes in an intermediate field as double cosets](#primes-in-an-intermediate-field-as-double-cosets)

If $M/K$ is the [Galois closure](galois-theory.md#galois-closure-of-a-field-extension) of a finite extension $L/K$, a prime splits completely in $L$ exactly when it splits completely in $M$. Complete splitting means every right action of $D$ on $H\backslash G$ fixes each coset, so $D$ lies in the [subgroup core](group-theory.md#core-group-theory) of $H$. That core is trivial because the conjugates of $L$ generate $M$.

###### Decomposition group of a prime and local Galois group

↑ **Parent:** [Decomposition group](#decomposition-group)

Restriction to completions gives a canonical isomorphism

$$
G_{\mathcal P/\mathfrak p}\cong
\operatorname{Gal}(L_{\mathcal P}/K_{\mathfrak p}).
$$

Consequently the number of primes above $\mathfrak p$ is the index of the decomposition group.

###### Completion preserves ramification and residue data

↑ **Parent:** [Completion of a number field at a prime ideal](#completion-of-a-number-field-at-a-prime-ideal)

For a prime $\mathfrak q$ of a finite separable extension $L/K$ above $\mathfrak p$, completion preserves the [ramification index](#ramification-index) and [residue-field extension](commutative-algebra.md#residue-field-extension):

$$
e(L_{\mathfrak q}/K_{\mathfrak p})=e_{\mathfrak q/\mathfrak p},
\qquad
k_{L_{\mathfrak q}}=k_{\mathfrak q}.
$$

##### Local factorization of X3 plus 25X2 minus 50X plus 40

↑ **Parent:** [Local factorization and extended absolute values](#local-factorization-and-extended-absolute-values)

The polynomial

$$
F(X)=X^3+25X^2-50X+40
$$

splits into three linear factors over $\mathbb Q_2$. Over $\mathbb Q_5$ it is an [Eisenstein polynomial](#eisenstein-polynomial), so adjoining a root gives a totally ramified cubic extension. Its splitting field over $\mathbb Q_5$ has [decomposition group](#decomposition-group) $S_3$ and [inertia group](#inertia-group) $A_3\cong C_3$.

## Hahn series

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hahn_series)

A [Hahn series](#hahn-series) over a [field](algebra.md#field) $k$ with exponents in an ordered abelian group $\Gamma$ is a formal sum $\sum_{\gamma}a_\gamma t^\gamma$ whose nonzero exponents form a well-ordered set. Such series form the [Hahn series field](#hahn-series-field).

### Hahn series field

↑ **Parent:** [Hahn series](#hahn-series)

For an ordered abelian group $\Gamma$, the Hahn series field $k((t^\Gamma))$ consists of formal sums with well-ordered support in $\Gamma$. The least exponent defines a valuation with value group $\Gamma$.

## P-adic number

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P-adic_number)

For a [prime number](prime-number.md) $p$, a p-adic number is an element of the [field](algebra.md#field) $\mathbb Q_p$ obtained by completing the [rational numbers](number-theory.md#rational-number) for the [metric](topological-analysis.md#metric) $d_p(x,y)=|x-y|_p$. Here $|\cdot|_p$ is the [p-adic absolute value](#p-adic-absolute-value). The [Cauchy-sequence construction of a metric completion](topological-analysis.md#cauchy-sequence-construction-of-a-metric-completion) supplies limits for every [Cauchy sequence](sequence-and-series.md#cauchy-sequence), and [addition](arithmetic.md#addition), [multiplication](arithmetic.md#multiplication), and the [p-adic absolute value](#p-adic-absolute-value) extend to this [complete metric space](topological-analysis.md#complete-metric-space). The [rational numbers](number-theory.md#rational-number) form a [dense subset](topology.md#dense-set). [Stephen William Semmes, Notes on p-adic numbers, pages 4-5](https://arxiv.org/pdf/math/0502560)

For a concrete example with $p=2$, consider the [partial sums](sequence-and-series.md#partial-sum) of a [geometric series](sequence-and-series.md#geometric-series):

$$
s_n=\sum_{k=0}^{n-1}2^k=2^n-1,\qquad |s_n-(-1)|_2=|2^n|_2=2^{-n}.
$$

The first values $1,3,7,15,31$ have distances $1/2,1/4,1/8,1/16,1/32$ from $-1$ in the [2-adic absolute value](#2-adic-absolute-value). Consequently

$$
-1=\sum_{k=0}^{\infty}2^k\qquad\text{in }\mathbb Q_2.
$$

This is a statement about [convergence in a metric space](topological-analysis.md#convergence-in-a-metric-space) with the [2-adic absolute value](#2-adic-absolute-value). In the ordinary [real number](arithmetic.md#real-number) [absolute value](real-analysis.md#absolute-value), the same [partial sums](sequence-and-series.md#partial-sum) grow without bound. Choosing a [metric](topological-analysis.md#metric) changes which approximation errors shrink.

More generally every nonzero [P-adic number](#p-adic-number) has a unique digit expansion

$$
x=\sum_{k=m}^{\infty}a_kp^k,\qquad m\in\mathbb Z,\quad a_m\ne0,\quad a_k\in\{0,1,\ldots,p-1\}.
$$

Only finitely many negative powers occur, while positive powers can continue indefinitely. Written with the highest powers on the left, the digits extend infinitely to the left; for example the [P-adic number](#p-adic-number) $-1$ at $p=2$ is written $\ldots111_2$. The [p-adic integers](number-theory.md#p-adic-integer) are exactly the elements with $|x|_p\leq1$, whose digit expansions use only nonnegative powers. [Andrew V. Sutherland, Number Theory I, Lecture 8, section 8.2, Proposition 8.17](https://math.mit.edu/classes/18.785/2021fa/LectureNotes8.pdf)

The construction can be understood through [modular arithmetic](modular-arithmetic.md). Successively choose the low-order digits to agree modulo $p$, $p^2$, and higher powers. After fixing digits below $p^n$, the remaining error has [p-adic absolute value](#p-adic-absolute-value) at most $p^{-n}$; the [partial sums](sequence-and-series.md#partial-sum) form a [Cauchy sequence](sequence-and-series.md#cauchy-sequence), so completeness supplies a limit. If two expansions first differ at position $j$, their difference has [P-adic valuation](number-theory.md#p-adic-valuation) $j$, proving uniqueness. This turns compatible finite [congruence classes](modular-arithmetic.md#congruence-class) into one exact [number](arithmetic.md#number). In particular, [Hensel's lemma](#hensel-s-lemma) upgrades suitable approximate [roots of a polynomial](polynomial.md#root-of-a-polynomial) modulo powers of $p$ into roots in the [p-adic integers](number-theory.md#p-adic-integer).

### 3-adic number

↑ **Parent:** [P-adic number](#p-adic-number)

A 3-adic number belongs to the completion of $\mathbb Q$ for the [p-adic absolute value](#p-adic-absolute-value) with prime three. Its nonzero elements have the form $3^k u$, with $k\in\mathbb Z$ and $u\in\mathbb Z_3^\times$. The [cube-class group of the 3-adic numbers](#cube-class-group-of-the-3-adic-numbers) is generated by the classes of $3$ and $4$.

### p-adic absolute value

↑ **Parent:** [P-adic number](#p-adic-number)

Fix a [prime number](prime-number.md) $p$. Write a nonzero [rational number](number-theory.md#rational-number) as $x=p^k a/b$, where $k\in\mathbb Z$ and the nonzero [integers](integer.md) $a,b$ are not divisible by $p$. The exponent $k$ is uniquely determined. Its [P-adic valuation](number-theory.md#p-adic-valuation) is this signed exponent $v_p(x)=k$: equivalently, for any nonzero integer [numerator](number-theory.md#numerator) $A$ and [denominator](number-theory.md#denominator) $B$,

$$
v_p(A/B)=v_p(A)-v_p(B),\qquad |x|_p=p^{-v_p(x)},\qquad |0|_p=0.
$$

Factors of $p$ in the [numerator](number-theory.md#numerator) decrease the [p-adic absolute value](#p-adic-absolute-value); factors in the [denominator](number-theory.md#denominator) increase it. For $p=2$ the computations are:

| [Rational number](number-theory.md#rational-number) $x$ | Factorization | [P-adic valuation](number-theory.md#p-adic-valuation) $v_2(x)$ | [2-adic absolute value](#2-adic-absolute-value) $|x|_2$ |
| --- | --- | --- | --- |
| $8$ | $2^3$ | $3$ | $1/8$ |
| $12$ | $2^2\cdot3$ | $2$ | $1/4$ |
| $3/8$ | $2^{-3}\cdot3$ | $-3$ | $8$ |
| $-7$ | $2^0\cdot(-7)$ | $0$ | $1$ |
| $0$ | Not applicable | $+\infty$ by convention | $0$ |

This is an [absolute value on a field](#absolute-value-algebra) measuring [divisibility](divisibility.md), rather than the magnitude on a [real number](arithmetic.md#real-number) [number line](arithmetic.md#number-line). It satisfies

$$
|xy|_p=|x|_p|y|_p,\qquad |x+y|_p\leq\max\{|x|_p,|y|_p\}.
$$

The proof comes directly from [P-adic valuations](number-theory.md#p-adic-valuation): exponents add in a [product of numbers](arithmetic.md#product-of-numbers), and extracting a common power of $p$ from a [sum](arithmetic.md#sum) gives $v_p(x+y)\geq\min\{v_p(x),v_p(y)\}$. If the two [P-adic valuations](number-theory.md#p-adic-valuation) differ, the remaining term with smaller exponent cannot cancel modulo $p$, so equality holds. Thus the [p-adic absolute value](#p-adic-absolute-value) is a [Non-Archimedean absolute value](#non-archimedean-absolute-value). [Stephen William Semmes, Notes on p-adic numbers, page 1](https://arxiv.org/pdf/math/0502560)

The [metric](topological-analysis.md#metric) $d_p(x,y)=|x-y|_p$ makes two [rational numbers](number-theory.md#rational-number) close when their difference contains a high power of $p$. This packages successive [modular congruences](modular-arithmetic.md#modular-congruence) into a numerical error estimate, allowing [convergence in a metric space](topological-analysis.md#convergence-in-a-metric-space) and [convergent series](sequence-and-series.md#convergent-series) to encode exact [arithmetic](arithmetic.md) information.

#### p-adic metric

↑ **Parent:** [p-adic absolute value](#p-adic-absolute-value)

The [p-adic metric](#p-adic-metric) on the [P-adic numbers](#p-adic-number) is induced by the [p-adic absolute value](#p-adic-absolute-value). Its [ultrametric inequality](#ultrametric-inequality) is $d_p(x,z)\leq\max(d_p(x,y),d_p(y,z))$. On [p-adic integers](number-theory.md#p-adic-integer), [digit agreement and p-adic distance](number-theory.md#digit-agreement-and-p-adic-distance) expresses metric precision as shared low-order digits.

#### 2-adic absolute value

↑ **Parent:** [p-adic absolute value](#p-adic-absolute-value)

The 2-adic absolute value is the [p-adic absolute value](#p-adic-absolute-value) for the [prime number](prime-number.md) $p=2$. It is defined on the [rational numbers](number-theory.md#rational-number) by $|x|_2=2^{-v_2(x)}$ for $x\ne0$ and $|0|_2=0$, and extends to their [P-adic number](#p-adic-number) completion $\mathbb Q_2$. For a nonzero [integer](integer.md), count factors of two until the remaining factor is odd; for a [rational number](number-theory.md#rational-number), subtract the [denominator](number-theory.md#denominator)'s count from the [numerator](number-theory.md#numerator)'s count.

The associated [metric](topological-analysis.md#metric) reverses a familiar comparison:

$$
d_2(5,13)=|5-13|_2=|-8|_2=\frac18,\qquad d_2(5,6)=|-1|_2=1.
$$

Although $13$ is eight units from $5$ on the ordinary [number line](arithmetic.md#number-line), it agrees with $5$ modulo $8$, whereas $6$ already disagrees modulo $2$. The [2-adic absolute value](#2-adic-absolute-value) measures that agreement. The value $|3/8|_2=8$ also shows why this [Non-Archimedean absolute value](#non-archimedean-absolute-value) must be distinguished from the ordinary [absolute value](real-analysis.md#absolute-value) $|3/8|=3/8$.

<a id="image-ordinary-absolute-value-and-2-adic-absolute-value-give-different-distance-patterns-for-the-same-sixteen-integers"></a>
![](two-adic-distance-comparison.png)

**[Figure 2](#image-ordinary-absolute-value-and-2-adic-absolute-value-give-different-distance-patterns-for-the-same-sixteen-integers). Ordinary absolute value and 2-adic absolute value give different distance patterns for the same sixteen integers**.

In the left panel, differences farther from the diagonal grow in ordinary [absolute value](real-analysis.md#absolute-value). In the right panel, nonzero even differences are closer than odd differences, and each further factor of two halves the [2-adic absolute value](#2-adic-absolute-value). The highlighted pairs have opposite distance rankings. The repeated pattern is the nested [congruence class](modular-arithmetic.md#congruence-class) structure of an [ultrametric space](#ultrametric-space), visible without adding any new points.

##### 2-adic metric

↑ **Parent:** [2-adic absolute value](#2-adic-absolute-value)

The 2-adic metric is $d_2(x,y)=|x-y|_2$, where $|x|_2=2^{-v_2(x)}$ for $x\ne0$ and $|0|_2=0$. Closeness means divisibility of the difference by a large power of two.

<h4 id="ostrowski-s-theorem">Ostrowski's theorem</h4>

↑ **Parent:** [p-adic absolute value](#p-adic-absolute-value)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ostrowski's_theorem)

Every nontrivial absolute value on $\mathbb Q$ is equivalent either to the usual absolute value or to one $p$-adic absolute value.

##### Non-Archimedean part of Ostrowski theorem

↑ **Parent:** [Ostrowski's theorem](#ostrowski-s-theorem)

For a nontrivial [Non-Archimedean absolute value](#non-archimedean-absolute-value) on $\mathbb Q$, every integer has absolute value at most one. Some prime $p$ must have value less than one, or the value would be trivial on every rational number. Two distinct such primes are impossible by a [Bezout identity](algebra.md#bezout-s-identity). Prime factorization then gives the displayed formula. Distinct primes give inequivalent topologies, since powers of $p$ tend to zero only for the $p$-adic absolute value among these values.

##### Non-Archimedean absolute values on a number field

↑ **Parent:** [Ostrowski's theorem](#ostrowski-s-theorem)

The nontrivial non-Archimedean absolute values on a [number field](algebraic-number-theory.md#number-field) $K$, up to equivalence, are indexed by the nonzero [prime ideals](commutative-algebra.md#prime-ideal) $\mathfrak p$ of its ring of integers. The value associated with $\mathfrak p$ is a fixed exponential of the discrete valuation $v_{\mathfrak p}$.

## Local field

↑ **Parent:** [Non-Archimedean analysis](non-archimedean-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_field)

A local field is a nondiscrete locally compact topological field. A non-Archimedean local field is a finite extension of $\mathbb Q_p$ or of $\mathbb F_p((t))$.

### p-adic field

↑ **Parent:** [Local field](#local-field)

A p-adic field is a finite extension of the [P-adic number](#p-adic-number) field $\mathbb Q_p$, equipped with its extended [p-adic absolute value](#p-adic-absolute-value). Conversely every characteristic-zero, nontrivially valued, non-Archimedean locally compact field is such an extension. A finite quotient $\mathcal O/p\mathcal O$ supplies finitely many generators of $\mathcal O$ over $\mathbb Z_p$ by repeated reduction and completeness.

#### Integral lattice in a p-adic vector space

↑ **Parent:** [P-adic field](#p-adic-field)

An integral lattice in a finite-dimensional $\mathbb Q_p$-vector space is a free $\mathbb Z_p$-submodule of full rank. Any two such lattices are commensurable: their intersection has finite index in each, because a sufficiently large power of $p$ multiplies either into the other. A finite group acting on the space admits invariant lattices by taking a sum of translates. This allows [Herbrand quotient](group-cohomology.md#herbrand-quotient) comparisons via finite quotient modules.

### Residue degree

↑ **Parent:** [Local field](#local-field)

The degree of the [residue field](commutative-algebra.md#residue-field) extension induced by a finite extension of complete discretely valued fields. Along with the [ramification index](#ramification-index), it satisfies $[L:K]=ef$. An [unramified extension](#unramified-extension) additionally has separable residue extension; a [totally ramified extension](#totally-ramified-extension) has residue degree one.

#### Absolute residue degree

↑ **Parent:** [Residue degree](#residue-degree)

The absolute [residue degree](#residue-degree) is the degree of the [residue field](commutative-algebra.md#residue-field) over its prime field. For a tower above $p$, degrees multiply: $[k_{\mathfrak q}:\mathbb F_p]=[k_{\mathfrak q}:k_{\mathfrak p}][k_{\mathfrak p}:\mathbb F_p]$. In a [Galois extension](galois-theory.md#finite-galois-extension) over $\mathbb Q$, the [decomposition group](#decomposition-group) has a cyclic [quotient group](group-theory.md#quotient-group) of this order by its [inertia group](#inertia-group). This can exclude [residue degrees](#residue-degree) even when the whole extension has that degree: $S_3$ has no cyclic [quotient group](group-theory.md#quotient-group) of order six.

### Local compactness criterion for a complete non-Archimedean field

↑ **Parent:** [Local field](#local-field)

A complete field with a nontrivial [Non-Archimedean absolute value](#non-archimedean-absolute-value) is locally compact exactly when its [valuation](algebra.md#valuation) is discrete and its [residue field](commutative-algebra.md#residue-field) is finite. In that case its [valuation ring](commutative-algebra.md#valuation-ring) is the [inverse limit](module-theory.md#inverse-limit) of the finite rings $\mathcal O/\mathfrak m^n$ and is compact. The [nontrivial valuation in the local compactness criterion](#nontrivial-valuation-in-the-local-compactness-criterion) is essential.

#### Digit expansion with a nonuniformizer

↑ **Parent:** [Local compactness criterion for a complete non-Archimedean field](#local-compactness-criterion-for-a-complete-non-archimedean-field)

Let a nontrivially valued [local field](#local-field) have compact [valuation ring](commutative-algebra.md#valuation-ring) $\mathcal O$, and choose any $t$ with $0<|t|<1$. The quotient $\mathcal O/t\mathcal O$ is finite. A fixed set of representatives containing zero gives every field element a unique convergent digit expansion, with finitely many nonzero negative-index terms. Recursive reduction modulo $t\mathcal O$ gives existence; comparing the first differing digit modulo this ideal gives uniqueness. The element $t$ need not be a [uniformizer](commutative-algebra.md#uniformizer).

#### Completeness of locally compact nontrivially valued fields

↑ **Parent:** [Local compactness criterion for a complete non-Archimedean field](#local-compactness-criterion-for-a-complete-non-archimedean-field)

In a locally compact nontrivially valued field, the [valuation ring](commutative-algebra.md#valuation-ring) is compact. A Cauchy sequence has a tail inside a translate of this compact set, hence a convergent subsequence. The Cauchy property forces the full sequence to converge.

#### Discrete valuation from nontrivial local compactness

↑ **Parent:** [Local compactness criterion for a complete non-Archimedean field](#local-compactness-criterion-for-a-complete-non-archimedean-field)

For a locally compact field with a nontrivial [Non-Archimedean absolute value](#non-archimedean-absolute-value), scaling a compact neighborhood makes its [valuation ring](commutative-algebra.md#valuation-ring) compact. Its open [maximal ideal](commutative-algebra.md#maximal-ideal) gives a finite discrete [residue field](commutative-algebra.md#residue-field), so that ideal is also closed and compact. A nonzero element of maximal absolute value in the ideal generates it. Successive division by this [uniformizer](commutative-algebra.md#uniformizer) makes the value group discrete.

#### Nontrivial valuation in the local compactness criterion

↑ **Parent:** [Local compactness criterion for a complete non-Archimedean field](#local-compactness-criterion-for-a-complete-non-archimedean-field)

An infinite field with the trivial [absolute value on a field](#absolute-value-algebra) is discrete, hence locally compact, but its [residue field](commutative-algebra.md#residue-field) is the original infinite field. Thus local compactness forces a finite [residue field](commutative-algebra.md#residue-field) and a discrete nontrivial value group only when the [valuation](algebra.md#valuation) is assumed nontrivial.

### Multiplicative group of a non-Archimedean local field

↑ **Parent:** [Local field](#local-field)

If a non-Archimedean [local field](#local-field) $K$ has [uniformizer](commutative-algebra.md#uniformizer) $\pi$, [valuation ring](commutative-algebra.md#valuation-ring) $\mathcal O_K$, maximal ideal $\mathfrak m_K$ and residue field $\mathbb F_q$, then

$$
K^\times\cong\pi^{\mathbb Z}\times\mu_{q-1}\times(1+\mathfrak m_K).
$$

The first factor records the [discrete valuation](commutative-algebra.md#discrete-valuation), the [Teichmuller representatives](#teichmuller-representative) split reduction $\mathcal O_K^\times\to\mathbb F_q^\times$, and $1+\mathfrak m_K$ is the group of [principal units](#principal-unit).

#### Principal-unit filtration of a local field

↑ **Parent:** [Multiplicative group of a non-Archimedean local field](#multiplicative-group-of-a-non-archimedean-local-field)

The groups $U_m$ form a compact-open neighbourhood basis at one inside the units of a non-Archimedean [local field](#local-field). A [smooth character](representation-theory.md#smooth-character) trivial on $U_{i+1}$ but nontrivial on $U_i$ cannot have a nonzero fixed vector under $U_m$ for $m\le i$. This elementary conductor comparison controls admissibility and smooth duals of direct sums.

#### Principal-unit group of a mixed-characteristic local field

↑ **Parent:** [Multiplicative group of a non-Archimedean local field](#multiplicative-group-of-a-non-archimedean-local-field)

If $K/\mathbb Q_p$ is finite of degree $d$, then as a topological [abelian group](group.md#abelian-group)

$$
1+\mathfrak m_K\cong\mu_{p^a}(K)\times\mathbb Z_p^d,
$$

where $\mu_{p^a}(K)$ is the finite group of all [roots of unity](algebra.md#root-of-unity) in $K$ whose orders are [prime powers](prime-number.md#prime-power) dividing a power of $p$.

<h3 id="hensel-s-lemma">Hensel's lemma</h3>

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hensel's_lemma)

For a complete discrete valuation ring $R$, a simple root of a polynomial modulo the maximal ideal lifts uniquely to a root in $R$.

#### Hensel lifting

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

#### Coprime-factor Hensel lifting

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

A monic [polynomial](polynomial.md) over a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) factors with prescribed coprime monic residue factors. Given monic lifts $g_r,h_r$ correct modulo $\pi^r$, the degree-bounded map $(u,v)\mapsto u\bar h_r+v\bar g_r$ is a bijection over the [residue field](commutative-algebra.md#residue-field), by coprimality and equality of dimensions. Solve it for the error $(f-g_rh_r)/\pi^r$, and replace the lifts by $g_r+\pi^ru,h_r+\pi^rv$. Their coefficients converge by completeness and the limiting product is $f$. The completeness assumption cannot be replaced just by localization.

#### Simple-root Hensel lifting by successive residues

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

For a [complete discrete valuation ring](commutative-algebra.md#complete-discrete-valuation-ring) $R$, let $f(a_1)\in(\pi)$ and let $f'(a_1)$ be a [unit](algebra.md#unit-in-a-ring). If $f(a_n)\in(\pi^n)$, choose $c$ modulo $\pi$ solving $f(a_n)/\pi^n+c f'(a_n)\equiv0$ and put $a_{n+1}=a_n+c\pi^n$. Taylor expansion gives $f(a_{n+1})\in(\pi^{n+1})$. The sequence is [Cauchy](sequence-and-series.md#cauchy-sequence) and its limit is a root. If two roots lift the same residue, factoring $f(x)-f(y)$ leaves $x-y$ times a unit, proving uniqueness.

#### Coprime factor lifting from valuation-extension uniqueness

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

Suppose a [Non-Archimedean absolute value](#non-archimedean-absolute-value) on $K$ has a unique [extension of an absolute value](#extension-of-an-absolute-value) to every finite extension. Factor a [monic](polynomial.md#monic-polynomial) $g\in\mathcal O_K[X]$ into [monic](polynomial.md#monic-polynomial) irreducible factors over $K$. All factors have integral coefficients because their roots have absolute value at most one. By [pure-power reduction of a monic irreducible polynomial](#pure-power-reduction-of-a-monic-irreducible-polynomial), each factor reduces to a power of a single irreducible [polynomial](polynomial.md). If $\overline g=\overline g_1\overline g_2$ is a [coprime](divisibility.md#coprime-integers) [monic](polynomial.md#monic-polynomial) factorization, assign each whole irreducible factor of $g$, with its multiplicity, to the unique side containing its residue factor. The resulting [monic](polynomial.md#monic-polynomial) $g_1,g_2\in\mathcal O_K[X]$ satisfy $g=g_1g_2$ and reduce to the prescribed factors. Completeness of $K$ is not required for this proof.

#### Elements that are powers of infinitely many degrees in a local field

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

For a non-Archimedean local field $K$, an element of $K^\times$ is an $m$th power for infinitely many positive integers $m$ exactly when it belongs to $\mathcal O_K^\times$. Valuations prove necessity; for sufficiency, choose infinitely many $m$ coprime to the residue characteristic and to $|k^\times|$, for which exponentiation by $m$ is an automorphism of the unit group.

#### Factorization of X4 plus 9X2 minus 2 over the 2-adic numbers

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

The polynomial $X^4+9X^2-2$ has three irreducible factors over $\mathbb Q_2$, of degrees one, one, and two. Its quadratic in $X^2$ has one unit root congruent to one modulo eight, hence a square, and one root of valuation one, whose associated quadratic factor is Eisenstein.

#### Strong form of Hensel lemma

↑ **Parent:** [Hensel's lemma](#hensel-s-lemma)

Let $K$ be complete for a [discrete valuation](commutative-algebra.md#discrete-valuation) $v$. If $f\in\mathcal O_K[X]$ and

$$
v(f(a))>2v(f'(a)),
$$

then [Newton iteration over a valued field](#newton-iteration-over-a-valued-field) converges to a root $\alpha\in\mathcal O_K$ with $v(\alpha-a)>v(f'(a))$.

##### Newton iteration over a valued field

↑ **Parent:** [Strong form of Hensel lemma](#strong-form-of-hensel-lemma)

Starting from $a_0$, Newton iteration sets $a_{n+1}=a_n-f(a_n)/f'(a_n)$. Under the [strong form of Hensel lemma](#strong-form-of-hensel-lemma) inequality, the correction valuations grow at least geometrically, so $(a_n)$ is a [Cauchy sequence](sequence-and-series.md#cauchy-sequence) converging to a root.

<h3 id="krasner-s-lemma">Krasner's lemma</h3>

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krasner's_lemma)

Let $K$ be complete, let $\alpha$ be separable over $K$, and let $\beta$ be algebraic over $K$. If $\beta$ is closer to $\alpha$ than any other $K$-conjugate of $\alpha$, then

$$
K(\alpha)\subseteq K(\beta).
$$

#### Closest-root descent in a Galois extension

↑ **Parent:** [Krasner's lemma](#krasner-s-lemma)

Let $L/K$ be a finite [Galois extension](galois-theory.md#finite-galois-extension) of a field complete for a [Non-Archimedean absolute value](#non-archimedean-absolute-value). Suppose $\alpha$ is uniquely closest to $\beta$ among the roots of a polynomial over $K$ lying in $L$. Every element of $\operatorname{Gal}(L/K(\beta))$ preserves [absolute values on a field](#absolute-value-algebra) and permutes these roots. It sends $\alpha$ to an equally close root, hence fixes $\alpha$. The [Fundamental theorem of Galois theory](galois-theory.md#fundamental-theorem-of-galois-theory) gives $K(\alpha)\subseteq K(\beta)$. The converse inclusion need not hold: for roots $0,\sqrt p,-\sqrt p$, the element $p\sqrt p$ is uniquely closest to zero but does not belong to $\mathbb Q_p$.

#### Finiteness of fixed-degree extensions of a p-adic field

↑ **Parent:** [Krasner's lemma](#krasner-s-lemma)

A [p-adic field](#p-adic-field) has only finitely many extensions of a fixed degree up to isomorphism. There are finitely many possible residue degrees and a unique [unramified extension](#unramified-extension) of each such degree. Over each maximal unramified subfield, a [totally ramified extension](#totally-ramified-extension) is generated by a root of an [Eisenstein polynomial](#eisenstein-polynomial). The coefficient space of these polynomials of fixed degree is compact. [Hensel lemma](#hensel-s-lemma) and [Krasner's lemma](#krasner-s-lemma) show that sufficiently close polynomials generate isomorphic extensions, giving a finite cover by neighborhoods of a constant extension type.

#### Continuity of roots over a non-Archimedean field

↑ **Parent:** [Krasner's lemma](#krasner-s-lemma)

The roots of a separable polynomial over a complete non-Archimedean field vary continuously with its coefficients after the roots are suitably matched. In particular, a sufficiently close coefficientwise approximation has one root in each sufficiently small disjoint ball around an original root.

#### Local realization as a completion of a number field

↑ **Parent:** [Krasner's lemma](#krasner-s-lemma)

Every finite extension of $\mathbb Q_p$ is isomorphic to the completion $F_{\mathfrak p}$ of some number field $F$ at a prime $\mathfrak p$ above $p$. Approximate a primitive element's minimal polynomial by a polynomial over $\mathbb Q$ and use [Krasner's lemma](#krasner-s-lemma) to preserve the generated local field.

#### Completion of an algebraic closure of a p-adic field is algebraically closed

↑ **Parent:** [Krasner's lemma](#krasner-s-lemma)

The completion $\mathbb C_p$ of an [algebraic closure](algebra.md#algebraic-closure) of $\mathbb Q_p$ is an [algebraically closed field](algebra.md#algebraically-closed-field). Approximate a polynomial over $\mathbb C_p$ by one over $\overline{\mathbb Q}_p$, use [continuity of roots over a non-Archimedean field](#continuity-of-roots-over-a-non-archimedean-field) to obtain a nearby algebraic root, and then use [Krasner's lemma](#krasner-s-lemma) to show that the original root already belongs to $\mathbb C_p$.

### Weierstrass preparation theorem

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weierstrass_preparation_theorem)

Over a complete local ring, a power series whose first unit coefficient has index $d$ is a unit times a unique monic distinguished polynomial of degree $d$. Consequently its sufficiently small zeros, counted with multiplicity, are the zeros of that polynomial.

#### Distinguished polynomial

↑ **Parent:** [Weierstrass preparation theorem](#weierstrass-preparation-theorem)

A distinguished polynomial over $\mathbb Z_p$ is monic and has every non-leading coefficient divisible by $p$. The [Weierstrass preparation theorem](#weierstrass-preparation-theorem) expresses any nonzero element of $\mathbb Z_p[[T]]$ as a power of $p$ times a unit times a distinguished polynomial.

### Laurent series field

↑ **Parent:** [Local field](#local-field)

The Laurent series field $k((t))$ consists of [formal series](commutative-algebra.md#formal-power-series) $\sum_{n\geq N}a_nt^n$ with finitely many negative-degree terms. Its $t$-adic valuation is the least exponent with nonzero coefficient.

#### Prescribed ramification and residue degree for a Laurent series field

↑ **Parent:** [Laurent series field](#laurent-series-field)

For arbitrary positive integers $e,f$, the displayed extension has degree $ef$, [ramification index](#ramification-index) $e$, and [residue degree](#residue-degree) $f$. If $|t|=p^{-1}$, its unique extended [absolute value on a field](#absolute-value-algebra) is $|\sum a_nu^n|=p^{-\min\{n:a_n\ne0\}/e}$. A basis consists of $\gamma_i u^j$, where the $\gamma_i$ form an [basis](vector-space.md#basis) of $\mathbb F_{p^f}$ and $0\le j<e$. Regrouping a Laurent series by its exponent modulo $e$ proves the basis assertion. When $p$ divides $e$ the extension can be inseparable; the valuation calculation still applies.

#### Finite extensions of the complex Laurent series field

↑ **Parent:** [Laurent series field](#laurent-series-field)

A finite extension of the complete discretely valued field $\mathbb C((t))$ has residue field $\mathbb C$, hence is totally ramified. If $\pi$ is its uniformizer, write $t=u\pi^n$. A root of the residue of $u$ lifts by [Hensel lemma](#hensel-s-lemma) to an $n$th root $v$ of $u$, since the residue characteristic is zero. Then $s=v\pi$ satisfies $s^n=t$. Distinct valuations modulo $n$ make $1,s,\ldots,s^{n-1}$ linearly independent over the base, so $L=\mathbb C((t))(s)$. Expanding in $s$ with constant coefficients identifies it with $\mathbb C((s))$. Its automorphisms are $s\mapsto\zeta_ns$, giving a cyclic Galois group.

##### Absolute Galois group of the complex Laurent series field

↑ **Parent:** [Finite extensions of the complex Laurent series field](#finite-extensions-of-the-complex-laurent-series-field)

Inside an algebraic closure, choose compatible roots $t^{1/n}$. The fields $\mathbb C((t^{1/n}))$ exhaust all finite extensions by [finite extensions of the complex Laurent series field](#finite-extensions-of-the-complex-laurent-series-field). Restriction from a degree-$m$ field to a degree-$n$ field for $n\mid m$ sends an exponent modulo $m$ to its reduction modulo $n$. The [absolute Galois group](galois-theory.md#absolute-galois-group) is their [inverse limit](module-theory.md#inverse-limit), namely the [profinite completion](topological-group.md#profinite-completion) of $\mathbb Z$. This is a procyclic group, rather than the direct-limit torsion group of all complex roots of unity.

#### Completion at an irreducible polynomial over a finite field

↑ **Parent:** [Laurent series field](#laurent-series-field)

For an irreducible polynomial $h\in\mathbb F_p[t]$ of degree $d$, the $h$-adic completion of $\mathbb F_p(t)$ is isomorphic to $\mathbb F_{p^d}((T))$. Its residue field is $\mathbb F_p[t]/(h)$ and $h$ is a uniformizer.

### p-adic exponential function

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/p-adic_exponential_function)

The $p$-adic exponential $\exp(x)=\sum_{n\geq0}x^n/n!$ converges near zero.

#### 2-adic exponential

↑ **Parent:** [p-adic exponential function](#p-adic-exponential-function)

#### Radius of convergence of the p-adic exponential

↑ **Parent:** [p-adic exponential function](#p-adic-exponential-function)

On $\mathbb C_p$, the power series $\exp(x)=\sum_{n\geq0}x^n/n!$ has radius of convergence

$$
p^{-1/(p-1)}.
$$

Indeed, [Legendre formula](number-theory.md#legendre-s-formula) gives $v_p(n!)/n\to1/(p-1)$, and the [Cauchy-Hadamard theorem](sequence-and-series.md#cauchy-hadamard-theorem) gives the stated radius.

#### p-adic logarithm

↑ **Parent:** [p-adic exponential function](#p-adic-exponential-function)

The $p$-adic logarithm is the convergent series $\log(1+x)=\sum_{n\geq1}(-1)^{n+1}x^n/n$ on a sufficiently small group of principal units.  
It is locally inverse to the [p-adic exponential function](#p-adic-exponential-function).

##### 2-adic logarithm

↑ **Parent:** [p-adic logarithm](#p-adic-logarithm)

##### Logarithm isomorphism on deep principal units

↑ **Parent:** [p-adic logarithm](#p-adic-logarithm)

For a mixed-characteristic [local field](#local-field) with [residue characteristic](commutative-algebra.md#residue-characteristic) $\ell$, the [p-adic logarithm](#p-adic-logarithm) and [p-adic exponential function](#p-adic-exponential-function) are mutually inverse continuous group homomorphisms on these domains. Bounds on the [valuations](algebra.md#valuation) of the denominators show that higher terms have greater [valuation](algebra.md#valuation) than the linear term. Dividing the logarithm by $\pi^r$ identifies the multiplicative [higher principal-unit group](#higher-principal-unit-group) with the additive integer ring; in particular it is torsion-free.

<h3 id="teichmuller-character">Teichmüller character</h3>

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Teichmüller_character)

The Teichmuller character sends a nonzero residue class to its unique root-of-unity lift in the valuation ring.

#### Teichmuller representative

↑ **Parent:** [Teichmüller character](#teichmuller-character)

The Teichmuller representative of a nonzero residue class $\bar a\in\mathbb F_q^*$ is the unique lift $\omega$ satisfying $\omega^{q-1}=1$ and $\omega\equiv a$ modulo the maximal ideal.

##### Finite prime-power Teichmuller representative

↑ **Parent:** [Teichmuller representative](#teichmuller-representative)

For a prime $p$ and $n\geq1$, the unique residue $y$ modulo $p^n$ satisfying $y\equiv x\pmod p$ and $y^p\equiv y\pmod{p^n}$ is the displayed residue. Existence follows from [Fermat's little theorem](number-theory.md#fermat-little-theorem) and [prime-power contraction under pth powers](modular-arithmetic.md#prime-power-contraction-under-pth-powers). Uniqueness follows by raising any other such residue repeatedly to the $p$th power and applying the same contraction to its congruence with $x$. This is the finite-modulus version of a [Teichmuller representative](#teichmuller-representative), including the zero class.

##### Approximation of Teichmuller lifts by iterated pth powers

↑ **Parent:** [Teichmuller representative](#teichmuller-representative)

For $K/\mathbb Q_p$ finite, let $x_n^{p^n}=x$ in its finite [residue field](commutative-algebra.md#residue-field), and choose arbitrary lifts $y_n\in\mathcal O_K$. With normalized [discrete valuation](commutative-algebra.md#discrete-valuation),

$$
v_K(u^p-v^p)\geq\min\{v_K(p)+r,pr\}\geq r+1\quad\text{if }v_K(u-v)\geq r\geq1.
$$

Applying this binomial estimate repeatedly to $y_n$ and $[x_n]$ proves the displayed bound, and hence convergence to $[x]$.

##### Teichmuller lift properties

↑ **Parent:** [Teichmuller representative](#teichmuller-representative)

For residue field $\mathbb F_q$, these two properties characterize the [Teichmuller lift](#teichmuller-representative) on every residue class, including zero. The [Hensel lemma](#hensel-s-lemma) applies to $T^q-T$, whose derivative reduces to $-1$. Uniqueness implies $[ab]=[a][b]$, $[0]=0$, $[1]=1$, and $[a^p]=[a]^p$. In mixed characteristic this multiplicative section need not be additive.

##### Teichmuller expansion

↑ **Parent:** [Teichmuller representative](#teichmuller-representative)

If $K$ is a complete [discretely valued field](commutative-algebra.md#discretely-valued-field) whose residue field $k$ is a [perfect field](algebra.md#perfect-field), and $\pi$ is a [uniformizer](commutative-algebra.md#uniformizer), the multiplicative Teichmuller lift $[\mathord\cdot]:k\to\mathcal O_K$ gives each $x\in\mathcal O_K$ a unique expansion

$$
x=\sum_{i=0}^{\infty}[a_i]\pi^i,
\qquad a_i\in k.
$$

###### Equal-characteristic complete discretely valued field

↑ **Parent:** [Teichmuller expansion](#teichmuller-expansion)

If a complete discretely valued field $K$ has positive characteristic and perfect residue field $k$, its [Teichmuller lift](#teichmuller-representative) is the unique ring section $k\to\mathcal O_K$. A choice of [uniformizer](commutative-algebra.md#uniformizer) $t$ then gives

$$
\mathcal O_K\cong k[[t]],
\qquad K\cong k((t)).
$$

###### Finite coefficient field in positive-characteristic local fields

↑ **Parent:** [Equal-characteristic complete discretely valued field](#equal-characteristic-complete-discretely-valued-field)

For a characteristic-p [local field](#local-field) with [residue field](commutative-algebra.md#residue-field) $\mathbb F_q$, the simple roots of $X^q-X$ lift uniquely by [Hensel lemma](#hensel-s-lemma). Their lifts form a copy of $\mathbb F_q$, since qth powers preserve addition and multiplication. Choose a [uniformizer](commutative-algebra.md#uniformizer) $\pi$. Repeatedly subtracting the lifted residue and dividing by $\pi$ produces a unique convergent expansion $\sum_{i\ge0}a_i\pi^i$ for each integral element. Allowing finitely many negative powers gives a valued-field isomorphism $K\cong\mathbb F_q((T))$, $T\mapsto\pi$.

### Unramified extension

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unramified_extension)

A finite extension of local fields is unramified when its ramification index is one and its residue-field degree equals the field degree. A local field has a unique unramified extension of each positive degree inside a fixed algebraic closure.

#### Unramified extensions remain unramified under base change

↑ **Parent:** [Unramified extension](#unramified-extension)

For non-Archimedean [local fields](#local-field), let $L/K$ be an [unramified extension](#unramified-extension) of degree $f$, and let $E/K$ be finite. The degree-$f$ [unramified extension](#unramified-extension) of $E$ has a [residue field](commutative-algebra.md#residue-field) containing the degree-$f$ residue extension of $K$. Lift an integral residue generator of $L$ into that field by [Hensel lemma](#hensel-s-lemma). This embeds $L$ into an [unramified extension](#unramified-extension) of $E$, so $LE/E$ is an [unramified](#unramified-extension) subextension. Applying this argument to each [completion of a number field at a prime ideal](#completion-of-a-number-field-at-a-prime-ideal) proves the finite-prime assertion for [number fields](algebraic-number-theory.md#number-field), even when $E/K$ is ramified.

#### Lifting residue-field embeddings of unramified extensions

↑ **Parent:** [Unramified extension](#unramified-extension)

For an [unramified extension](#unramified-extension) $L/K$ of non-Archimedean [local fields](#local-field) and any finite extension $M/K$, reduction is a bijection between $K$-[field homomorphisms](galois-theory.md#field-homomorphism) $L\to M$ and $k_K$-[field homomorphisms](galois-theory.md#field-homomorphism) $k_L\to k_M$. Choose an integral generator with separable irreducible reduction. Each specified residue image lifts uniquely to a root in $M$ by [Hensel lemma](#hensel-s-lemma). Conversely a $K$-embedding preserves the unique extended [valuation](algebra.md#valuation) and therefore induces the residue embedding. The same argument applies when $M$ is any non-Archimedean local extension with the given compatible embedding of $K$.

#### Unramified generator criterion with separable reduction

↑ **Parent:** [Unramified extension](#unramified-extension)

A finite extension of complete discretely valued fields is [unramified](#unramified-extension) exactly when it has an integral generator whose reduced [minimal polynomial of an algebraic element](galois-theory.md#minimal-polynomial-of-an-algebraic-element) is separable. In one direction, lift a residue-field primitive element. In the other, the factorization form of [Hensel's lemma](#hensel-s-lemma) makes the separable reduction irreducible, forcing residue degree to equal the entire extension degree.

##### Unramified residue generator integral basis

↑ **Parent:** [Unramified generator criterion with separable reduction](#unramified-generator-criterion-with-separable-reduction)

For an [unramified extension](#unramified-extension) of [local fields](#local-field) $L/K$, an integral element whose residue generates $k_L/k_K$ generates $L/K$: its degree is at least the [residue degree](#residue-degree) $f=[L:K]$. The reduced powers $1,\bar\alpha,\ldots,\bar\alpha^{f-1}$ are a [basis](vector-space.md#basis) of the [residue field](commutative-algebra.md#residue-field) extension. If $x=\sum c_j\alpha^j$, factor out a coefficient of least [valuation](algebra.md#valuation). Reduction of the remaining sum is nonzero by that residue [basis](vector-space.md#basis), so $v_L(x)=\min_j v_K(c_j)$. Consequently $x$ is integral exactly when all $c_j$ are integral.

###### Residue-basis norm formula for an unramified extension

↑ **Parent:** [Unramified residue generator integral basis](#unramified-residue-generator-integral-basis)

Let $L/K$ be a finite [unramified extension](#unramified-extension) of complete fields with a [Non-Archimedean absolute value](#non-archimedean-absolute-value), with separable residue extension and $[L:K]=[k_L:k_K]=n$. If $x$ is integral and its residue generates $k_L/k_K$, then $1,x,\ldots,x^{n-1}$ form a $K$-basis. Divide any nonzero combination by a coefficient of largest absolute value. Its remaining coefficients are integral, at least one is a unit, and the residue-basis independence makes the reduction nonzero. The displayed norm formula follows. In particular, the combination is integral exactly when every coefficient is integral, proving $\mathcal O_L=\mathcal O_K[x]$ without requiring a discrete valuation.

#### Existence and uniqueness of unramified local extensions

↑ **Parent:** [Unramified extension](#unramified-extension)

For a non-Archimedean [local field](#local-field) $K$, every finite extension $\ell/k_K$ of its [residue field](commutative-algebra.md#residue-field) is realized by an [unramified extension](#unramified-extension) of $K$, unique up to $K$-isomorphism. Lift the irreducible polynomial of a residue generator to a monic integral polynomial and adjoin a root. Its residue degree equals its field degree, forcing ramification index one. In any other such extension the [Hensel lemma](#hensel-s-lemma) lifts the same simple residue root, giving an isomorphism.

#### Frobenius automorphism

↑ **Parent:** [Unramified extension](#unramified-extension)

For a finite residue field $k$ of cardinality $q$, arithmetic Frobenius is $x\mapsto x^q$. Its lift generates the Galois group of a finite unramified extension; geometric Frobenius is its inverse.

##### Frobenius conjugacy class

↑ **Parent:** [Frobenius automorphism](#frobenius-automorphism)

In a finite [Galois extension](galois-theory.md#finite-galois-extension) $L/K$, choose a [prime ideal](commutative-algebra.md#prime-ideal) $\mathfrak P$ above an unramified $\mathfrak p$. The [Frobenius automorphism](#frobenius-automorphism) at $\mathfrak P$ is characterized on its residue field by $x\mapsto x^{N\mathfrak p}$. Changing $\mathfrak P$ conjugates this element, so its [conjugacy class](group-action.md#conjugacy-class) is well-defined. It is the identity class exactly at a [completely split prime](algebraic-number-theory.md#completely-split-prime).

###### Frobenius permutation and roots modulo a prime

↑ **Parent:** [Frobenius conjugacy class](#frobenius-conjugacy-class)

Let a monic integer [polynomial](polynomial.md) have distinct roots in its [splitting field](galois-theory.md#splitting-field). Outside the finitely many primes dividing its [polynomial discriminant](galois-theory.md#polynomial-discriminant) or ramifying in that field, its roots reduce to distinct residue roots. The [Frobenius automorphism](#frobenius-automorphism) permutes them by $a\mapsto a^p$; a reduced root belongs to $\mathbb F_p$ exactly when it is fixed. Distinctness of reduction identifies this with a fixed root of the Galois permutation itself. Combining this observation with a [derangement in a transitive group action](group-action.md#derangement-in-a-transitive-group-action) and the [Chebotarev density theorem](algebraic-number-theory.md#chebotarev-density-theorem) proves that an irreducible polynomial of degree at least two has rootless reduction at a positive [Dirichlet density](algebraic-number-theory.md#dirichlet-density) of primes. The degree bound is essential: every monic linear integer polynomial has a root modulo every prime.

#### Maximal unramified extension

↑ **Parent:** [Unramified extension](#unramified-extension)

The maximal unramified extension $K^{\mathrm{nr}}$ is the union of all finite unramified extensions of a non-Archimedean local field $K$. Its Galois group is canonically $\widehat{\mathbb Z}$, generated topologically by [Frobenius](#frobenius-automorphism).

#### Maximal unramified subextension of a local field extension

↑ **Parent:** [Unramified extension](#unramified-extension)

Every finite extension $L/K$ of non-Archimedean [local fields](#local-field) has a unique intermediate field $K_0$ whose residue field is $k_L$ and for which $K_0/K$ is unramified. The extension $L/K_0$ is totally ramified.

### Ramification group

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramification_group)

For a finite Galois extension of local fields, the lower ramification groups measure how closely automorphisms fix the valuation ring. The inertia group is $G_0$, and $G_1$ is the wild inertia group.

#### Positive ramification quotients are elementary abelian

↑ **Parent:** [Ramification group](#ramification-group)

For $\sigma\in G_i$, the residue of $(\sigma\pi_L-\pi_L)/\pi_L^{i+1}$ gives a homomorphism to the additive residue field with kernel $G_{i+1}$. On composing two automorphisms, their leading displacement coefficients add because each fixes residues and changes the uniformizer only in degree at least two. These successive quotients are [elementary abelian groups](group.md#elementary-abelian-group) in residue characteristic $p$. The filtration terminates, so the [wild inertia group](#wild-inertia-group) is a finite $p$-group.

#### Ramification of the splitting field of X3 plus pX plus p

↑ **Parent:** [Ramification group](#ramification-group)

For an odd prime $p$, this [Eisenstein polynomial](#eisenstein-polynomial) generates a totally ramified cubic root field. Its [discriminant](polynomial.md#discriminant) is $-p^2(4p+27)$. For $p>3$ the unit part is a square exactly when $p\equiv1\pmod3$. The [splitting field](galois-theory.md#splitting-field) then has cyclic [Galois group](galois-theory.md#galois-group) of order three; otherwise it has [symmetric group](finite-group-theory.md#symmetric-group) $S_3$, with an [unramified extension](#unramified-extension) of degree two and [inertia group](#inertia-group) $C_3$. Both cases are [tamely ramified](#tamely-ramified-extension), so all positive [ramification groups](#ramification-group) are trivial.

At $p=3$, adjoining $\beta=\sqrt{-39}$ gives a ramified quadratic subfield, and the [splitting field](galois-theory.md#splitting-field) has total [ramification index](#ramification-index) six. A root $\alpha$ has normalized [valuation](algebra.md#valuation) two, while $\beta$ has [valuation](algebra.md#valuation) three, so $\pi=\beta/\alpha$ is a [uniformizer](commutative-algebra.md#uniformizer). The derivative $3\alpha^2+3$ has [valuation](algebra.md#valuation) six, and all distinct root differences have [valuation](algebra.md#valuation) three. A three-cycle fixes $\beta$, giving $v_L(\sigma\pi-\pi)=2$. A transposition fixing $\alpha$ negates $\beta$, giving [valuation](algebra.md#valuation) one; conjugation handles the other transpositions. Hence $G_0=S_3$, $G_1=C_3$, and $G_i=1$ for $i\ge2$. The [different exponent](#different-exponent) is seven.

#### Lower ramification filtration of a prime-power cyclotomic extension

↑ **Parent:** [Ramification group](#ramification-group)

For $L=\mathbb Q_p(\zeta_{p^n})$, the [uniformiser](commutative-algebra.md#uniformizer) $\zeta_{p^n}-1$ and the [uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups) give the displayed [valuation](algebra.md#valuation) for $a\ne1$. Thus $G_0$ is the full unit group modulo $p^n$, and $G_i$ consists of units congruent to one modulo $p^j$ when $p^{j-1}\leq i\leq p^j-1$, $1\leq j<n$. All groups are trivial for $i\geq p^{n-1}$. The formula includes $p=2$, where the first congruence subgroup is already the full group.

#### Lower ramification numbering

↑ **Parent:** [Ramification group](#ramification-group)

For all real $s\geq0$, this definition uses the normalized integral valuation on $L$. Equivalently $G_s=G_{\lceil s\rceil}$. The group $G_0$ is the [inertia group](#inertia-group) and $G_1$ is the [wild inertia group](#wild-inertia-group).

##### Herbrand function

↑ **Parent:** [Lower ramification numbering](#lower-ramification-numbering)

The Herbrand function is a continuous strictly increasing piecewise linear function on the nonnegative reals. Its inverse is denoted $\psi_{L/K}$. It reparametrizes the [lower ramification numbering](#lower-ramification-numbering) to the [upper ramification numbering](#upper-ramification-numbering).

###### Upper ramification numbering

↑ **Parent:** [Herbrand function](#herbrand-function)

The upper numbering is obtained by applying the inverse [Herbrand function](#herbrand-function) to the index in the [lower ramification numbering](#lower-ramification-numbering). It is compatible with quotient Galois groups, whereas lower numbering is compatible with subgroups.

###### Upper ramification groups commute with quotients

↑ **Parent:** [Upper ramification numbering](#upper-ramification-numbering)

For a normal subgroup $H$ of a finite local [Galois group](galois-theory.md#galois-group), the [upper ramification numbering](#upper-ramification-numbering) on its quotient is obtained by projecting the upper groups. The [Herbrand function](#herbrand-function) is the change of variable that ensures this compatibility. In contrast, the [lower ramification numbering](#lower-ramification-numbering) restricts directly to subgroups.

#### Uniformizer criterion for lower ramification groups

↑ **Parent:** [Ramification group](#ramification-group)

If $L/K$ is a finite totally ramified Galois extension and $\pi_L$ is a [uniformizer](commutative-algebra.md#uniformizer), then

$$
G_i=\{\sigma:v_L(\sigma(\pi_L)-\pi_L)\geq i+1\}
$$

for every $i\geq0$.

##### Ramification groups of the splitting field of T3 minus 2 over Q3

↑ **Parent:** [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)

For $L=\mathbb Q_3(\zeta_3,\alpha)$ with $\alpha^3=2$, the shifted cubic for $\alpha+1$ and quadratic for $\zeta_3-1$ are [Eisenstein](commutative-algebra.md#eisenstein-criterion). Their compositum is totally ramified of degree six. The element $\pi=(\zeta_3-1)/(\alpha+1)$ has [valuation](algebra.md#valuation) one. Order-three automorphisms move it with [valuation](algebra.md#valuation) two and transpositions with [valuation](algebra.md#valuation) one. The lower breaks are zero and one, the upper breaks zero and one-half, and the [different exponent from ramification groups](#different-exponent-from-ramification-groups) is seven.

##### Ramification groups of the eighth-root cyclotomic extension of the 2-adic field

↑ **Parent:** [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)

For $\mathbb Q_2(\zeta_8)/\mathbb Q_2$, the shifted polynomial $(1+T)^4+1$ is [Eisenstein](commutative-algebra.md#eisenstein-criterion) and $\zeta_8-1$ is a [uniformizer](commutative-algebra.md#uniformizer). The three nonidentity automorphisms have displacement [valuations](algebra.md#valuation) two, four and two. Thus the lower breaks are one and three, the upper breaks one and two, and the [different exponent from ramification groups](#different-exponent-from-ramification-groups) is eight.

<h5 id="ramification-break-of-an-artin-schreier-pole">Ramification break of an Artin–Schreier pole</h5>

↑ **Parent:** [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)

Let $K$ be an equal-characteristic-p [local field](#local-field) and let $c\in K$ have $v_K(c)=-m<0$, with $p\nmid m$. If $\alpha^p-\alpha=c$, the [Artin–Schreier extension](galois-theory.md#artin-schreier-extension) $L=K(\alpha)$ has degree $p$ and is totally ramified: a root in $K$ would force the pole order to be divisible by $p$, and $p v_L(\alpha)=-m e(L/K)$ forces $e=p$. Choose $1\leq s<p$ and an integer $r$ with $rp-sm=1$. For a base [uniformizer](commutative-algebra.md#uniformizer) $t$, the element $\pi_L=t^r\alpha^s$ has [valuation](algebra.md#valuation) one. Under $\sigma_a(\alpha)=\alpha+a$, $a\in\mathbb F_p^\times$, the leading term in $\sigma_a(\pi_L)-\pi_L$ has [valuation](algebra.md#valuation) $rp-(s-1)m=m+1$. The [uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups) therefore gives the single lower break $m$. The [Herbrand function](#herbrand-function) is the identity up to that break, so the upper break is also $m$.

##### Ramification groups of the splitting field of T3 minus 3T plus 3 over Q3

↑ **Parent:** [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)

For the splitting field $M/\mathbb Q_3$ of $T^3-3T+3$, the cubic is [Eisenstein](commutative-algebra.md#eisenstein-criterion) and its discriminant is $-135$. The quadratic subfield is $\mathbb Q_3(\sqrt3)$, and the degree-six extension is totally ramified. If $\alpha$ is a root and $s=\sqrt3$, then $\pi=\alpha^2/s$ is a [uniformizer](commutative-algebra.md#uniformizer). Transpositions have $v_M(\sigma\pi-\pi)=1$, while three-cycles have value $2$, giving the displayed [ramification groups](#ramification-group). Its [different exponent from ramification groups](#different-exponent-from-ramification-groups) is $7$.

##### Ramification groups of the splitting field of Xp minus p over the p-adic numbers

↑ **Parent:** [Uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups)

For odd $p$, the splitting field $K=\mathbb Q_p(\zeta_p,\sqrt[p]{p})$ is totally ramified of degree $p(p-1)$. With

$$
\varpi=\frac{\zeta_p-1}{\sqrt[p]{p}},
$$

the lower ramification groups are

$$
G_0=\operatorname{Gal}(K/\mathbb Q_p),\qquad
G_i\cong\mathbb Z/p\mathbb Z\ (1\leq i\leq p),\qquad
G_i=1\ (i\geq p+1).
$$

To verify the filtration, write $\alpha^p=p$ and $\lambda=\zeta_p-1$. The [Eisenstein polynomials](#eisenstein-polynomial) for $\alpha$ and $\lambda$ give coprime degrees $p$ and $p-1$, so their compositum has degree $p(p-1)$. Its element $\varpi=\lambda/\alpha$ has $p$-adic [valuation](algebra.md#valuation) $1/[p(p-1)]$, forcing total ramification. For an automorphism $\sigma_{a,b}$ with $\alpha\mapsto\zeta_p^a\alpha$ and $\zeta_p\mapsto\zeta_p^b$,

$$
\frac{\sigma_{a,b}(\varpi)}{\varpi}=\zeta_p^{-a}\frac{\zeta_p^b-1}{\zeta_p-1}.
$$

Its residue is $b$, so the normalized displacement [valuation](algebra.md#valuation) is one if $b\ne1$. If $b=1$ and $a\ne0$, that valuation is $1+v_K(\zeta_p^{-a}-1)=p+1$. The [uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups) now gives every group displayed above.

###### Eisenstein sextic presentation of the splitting field of X3 minus 3 over Q3

↑ **Parent:** [Ramification groups of the splitting field of Xp minus p over the p-adic numbers](#ramification-groups-of-the-splitting-field-of-xp-minus-p-over-the-p-adic-numbers)

If $a^3=3$ and $\zeta_3$ is a primitive cube root of unity, then $\pi^3=1+2\zeta_3$ and $\pi^6=-3$. The [Eisenstein polynomial](#eisenstein-polynomial) $X^6+3$ therefore presents the entire degree-six [splitting field](galois-theory.md#splitting-field), and $\pi$ is a [uniformizer](commutative-algebra.md#uniformizer). Its normalised [valuation](algebra.md#valuation) gives $v_L(3)=6$, $v_L(a)=2$ and $v_L(\zeta_3-1)=3$. The order-three automorphisms displace $\pi$ with [valuation](algebra.md#valuation) four, whereas transpositions displace it with [valuation](algebra.md#valuation) one.

#### Tame inertia quotient

↑ **Parent:** [Ramification group](#ramification-group)

For a finite totally ramified Galois extension, the map

$$
\sigma\longmapsto\overline{\sigma(\pi_L)/\pi_L}
$$

induces an injection $G_0/G_1\hookrightarrow k_L^\times$. In particular, the tame inertia quotient is cyclic and has order prime to the residue characteristic.

##### Branch-cycle conjugacy class

↑ **Parent:** [Tame inertia quotient](#tame-inertia-quotient)

For a [Finite Galois extension](galois-theory.md#finite-galois-extension) of $K(T)$ with algebraically closed characteristic-zero constants, the local decomposition and inertia groups coincide and are cyclic. A fixed compatible choice of primitive [roots of unity](algebra.md#root-of-unity) selects a generator through its [uniformizer character of inertia](#uniformizer-character-of-inertia). Changing the prime above a base point conjugates this generator, and changing the [uniformizer](commutative-algebra.md#uniformizer) does not change its character. Without the roots-of-unity convention, only the inertia-subgroup [conjugacy class](group-action.md#conjugacy-class) is intrinsic. Over $\mathbb C$, positive local orientation gives the standard convention.

###### Quadratic branch parity criterion

↑ **Parent:** [Branch-cycle conjugacy class](#branch-cycle-conjugacy-class)

In [characteristic zero](algebra.md#characteristic-zero) with algebraically closed constants, a local unit has a square root. Thus $K(T)(\sqrt a)$ near a point is equivalent to adjoining the square root of the local parameter to the power $v_p(a)$. Even order is unramified; odd order gives [ramification index](#ramification-index) two. For a [polynomial](polynomial.md) $a$, its order at infinity is minus its degree, so infinity branches exactly for odd degree.

##### Uniformizer character of inertia

↑ **Parent:** [Tame inertia quotient](#tame-inertia-quotient)

For a finite Galois extension of non-Archimedean [local fields](#local-field), this is a homomorphism from the [inertia group](#inertia-group) to $k_L^\times$ with kernel the [wild inertia group](#wild-inertia-group). Inertia acts trivially on residue units, which proves multiplicativity and independence of the chosen [uniformizer](commutative-algebra.md#uniformizer). Passing to the maximal unramified subextension reduces the kernel calculation to a totally ramified extension. Hence it embeds the [tame inertia quotient](#tame-inertia-quotient) into the cyclic multiplicative group of the residue field.

#### Different ideal

↑ **Parent:** [Ramification group](#ramification-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Different_ideal)

For a finite separable extension of local fields, the different is the inverse fractional ideal of the codifferent. If $\mathcal O_L=\mathcal O_K[\alpha]$ and $f$ is the minimal polynomial of $\alpha$, then $\mathfrak D_{L/K}=(f'(\alpha))$.

##### Different exponent

↑ **Parent:** [Different ideal](#different-ideal)

The different exponent at a [prime ideal](commutative-algebra.md#prime-ideal) $\mathfrak P$ is its exponent in the [prime ideal factorization](algebraic-number-theory.md#prime-ideal-factorization) of the [different ideal](#different-ideal). It equals the local different exponent of the corresponding extension of completions. The [different exponent and tame ramification](#different-exponent-and-tame-ramification) theorem detects unramified, tame, and wild behavior without assuming a [Galois extension](galois-theory.md#finite-galois-extension).

###### Cyclotomic local different exponent

↑ **Parent:** [Different exponent](#different-exponent)

For $K_r=\mathbb Q_p(\zeta_{p^r})$, the [uniformizer](commutative-algebra.md#uniformizer) $\zeta_{p^r}-1$ has [different exponent](#different-exponent) $p^{r-1}(r(p-1)-1)$. Differentiate the [cyclotomic polynomial](galois-theory.md#cyclotomic-polynomial) at $\zeta_{p^r}$: the numerator contributes $r p^{r-1}(p-1)$ to the [valuation](algebra.md#valuation), while the denominator $\zeta_p-1$ contributes $p^{r-1}$.

###### Different exponent and tame ramification

↑ **Parent:** [Different exponent](#different-exponent)

For a finite extension of [number fields](algebraic-number-theory.md#number-field), the [different exponent](#different-exponent) satisfies $d_{\mathfrak P}\geq e_{\mathfrak P}-1$, with equality exactly when the extension at $\mathfrak P$ is [tamely ramified](#tamely-ramified-extension). The finite residue fields are perfect, so tameness is equivalent to the residue characteristic not dividing the [ramification index](#ramification-index). Thus unramified primes have exponent zero and wildly ramified primes have exponent at least $e_{\mathfrak P}$. No [Galois extension](galois-theory.md#finite-galois-extension) hypothesis is needed.

##### Inverse different

↑ **Parent:** [Different ideal](#different-ideal)

For a finite separable extension of number fields or local fields,

$$
\mathfrak D_{L/K}^{-1}
=\{x\in L:\operatorname{Tr}_{L/K}(x\mathcal O_L)\subseteq\mathcal O_K\}.
$$

It is also called the codifferent. If $\mathcal O_L=\mathcal O_K[\alpha]$ with minimal polynomial $g$, it equals $g'(\alpha)^{-1}\mathcal O_L$.

##### Different in a tower

↑ **Parent:** [Different ideal](#different-ideal)

For finite separable extensions $L/E/K$,

$$
\mathfrak D_{L/K}
=\mathfrak D_{L/E}\mathfrak D_{E/K}\mathcal O_L.
$$

For normalized valuations this says

$$
d(L/K)=d(L/E)+e(L/E)d(E/K).
$$

##### Different exponent from ramification groups

↑ **Parent:** [Different ideal](#different-ideal)

For a finite Galois extension of local fields,

$$
d(L/K)=\sum_{i\geq0}(|G_i|-1).
$$

#### Inertia group

↑ **Parent:** [Ramification group](#ramification-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertia_group)

The inertia group of a finite [Galois extension](galois-theory.md#finite-galois-extension) of local fields is the kernel of the action of its [Galois group](galois-theory.md#galois-group) on the residue field. In lower numbering it is the zeroth [ramification group](#ramification-group) $G_0$.

##### Wild inertia group

↑ **Parent:** [Inertia group](#inertia-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wild_inertia_group)

The wild inertia group is the first [ramification group](#ramification-group) $G_1$. It is the unique Sylow subgroup of the [inertia group](#inertia-group) for the residue characteristic.

#### Tamely ramified extension

↑ **Parent:** [Ramification group](#ramification-group)

A finite extension of local fields is tamely ramified when its residue-field extension is separable and its [ramification index](#ramification-index) is coprime to the residue characteristic. For a finite Galois extension this is equivalent to trivial [wild inertia group](#wild-inertia-group) $G_1$.

##### Discriminant exponent of a tame Galois extension

↑ **Parent:** [Tamely ramified extension](#tamely-ramified-extension)

If $L/K$ is a finite tamely ramified [Galois extension](galois-theory.md#finite-galois-extension) of local fields with degree $n$ and [ramification index](#ramification-index) $e$, then its different exponent is $e-1$ and the discriminant exponent is

$$
v_K(\operatorname{disc}(L/K))=n\left(1-\frac1e\right).
$$

#### Ramification-group sum for a monogenic integer ring

↑ **Parent:** [Ramification group](#ramification-group)

If $L/K$ is a finite [Galois extension](galois-theory.md#finite-galois-extension) of local fields, $\mathcal O_L=\mathcal O_K[\alpha]$, and $f$ is the [minimal polynomial](linear-operator-theory.md#minimal-polynomial) of $\alpha$, then

$$
v_L(f'(\alpha))
=\sum_{1\ne\sigma\in\operatorname{Gal}(L/K)}v_L(\sigma(\alpha)-\alpha)
=\sum_{s\geq0}(|G_s|-1).
$$

### Eisenstein polynomial

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eisenstein_polynomial)

For a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) with [uniformizer](commutative-algebra.md#uniformizer) $\pi$, an Eisenstein polynomial is a monic polynomial whose nonleading coefficients are divisible by $\pi$ and whose constant coefficient is not divisible by $\pi^2$. It is [irreducible](polynomial.md#irreducible-polynomial), and adjoining one of its roots gives a totally ramified extension.

#### Shifted Eisenstein polynomial

↑ **Parent:** [Eisenstein polynomial](#eisenstein-polynomial)

A [polynomial](polynomial.md) may fail the [Eisenstein polynomial](#eisenstein-polynomial) test while a translate $f(T+a)$ passes it. Translation does not change the generated extension: if $f(\alpha)=0$, then $f(T+a)$ vanishes at $\alpha-a$. For $f(T)=T^3-m$, the translate by $m$ is Eisenstein at $3$ whenever $3\nmid m$ and $m\not\equiv\pm1\pmod9$.

#### Ramification polynomial

↑ **Parent:** [Eisenstein polynomial](#eisenstein-polynomial)

The ramification [polynomial](polynomial.md) records the normalised differences of conjugates of a [uniformizer](commutative-algebra.md#uniformizer), including the zero difference from the identity automorphism. Its quotient by $X$ is the [reduced ramification polynomial](#reduced-ramification-polynomial). In the usual coefficient-index convention, the finite slopes of its lower [Newton polygon](#newton-polygon) are negatives of the [valuations](algebra.md#valuation) of its nonzero roots; the coefficient at the zero root is treated as having infinite [valuation](algebra.md#valuation).

##### Reduced ramification polynomial

↑ **Parent:** [Ramification polynomial](#ramification-polynomial)

For a degree-$n$ totally ramified [Galois extension](galois-theory.md#finite-galois-extension) and a [uniformizer](commutative-algebra.md#uniformizer) $\pi$, let $f$ be its [minimal polynomial](linear-operator-theory.md#minimal-polynomial). Dividing the ramification [polynomial](polynomial.md) $f(\pi(1+X))/\pi^n$ by its known factor $X$ gives the reduced ramification [polynomial](polynomial.md). It is monic of degree $n-1$, integral over the extension's [valuation ring](commutative-algebra.md#valuation-ring), and has roots $(\sigma(\pi)-\pi)/\pi$ for nonidentity automorphisms. Its constant coefficient is nonzero in a separable extension. Removing the zero root allows the usual [Newton polygon root valuation theorem](#newton-polygon-root-valuation-theorem) to apply directly.

###### Ramification breaks from a reduced ramification polygon

↑ **Parent:** [Reduced ramification polynomial](#reduced-ramification-polynomial)

In a totally ramified [Galois extension](galois-theory.md#finite-galois-extension), the [uniformizer criterion for lower ramification groups](#uniformizer-criterion-for-lower-ramification-groups) gives $\sigma\in G_m\setminus G_{m+1}$ exactly when $v_L((\sigma(\pi)-\pi)/\pi)=m$. The [Newton polygon root valuation theorem](#newton-polygon-root-valuation-theorem) therefore identifies a slope $-m$ in the coefficient-index convention with a lower ramification jump at $m$. Its horizontal length is the number of automorphisms in that difference. Under the [reflected Newton polygon convention](#reflected-newton-polygon-convention) the same jump has slope $+m$.

### Newton polygon

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton_polygon)

The Newton polygon of a polynomial over a valued field is the lower convex hull of the points formed from coefficient indices and valuations. Its slopes determine the valuations of roots, counted with multiplicity.

#### Reflected Newton polygon convention

↑ **Parent:** [Newton polygon](#newton-polygon)

For a degree-$d$ [polynomial](polynomial.md), reflecting the usual coefficient-index axis replaces $(j,v(a_j))$ by $(d-j,v(a_j))$. The reflected lower polygon has slopes equal to root [valuations](algebra.md#valuation), rather than their negatives. Horizontal lengths, and therefore multiplicities, are unchanged. This convention makes positive lower [ramification groups](#ramification-group) breaks appear as positive slopes of a reduced ramification polygon.

#### Newton polygon root valuation theorem

↑ **Parent:** [Newton polygon](#newton-polygon)

For a [polynomial](polynomial.md) with nonzero constant coefficient over a complete [discretely valued field](commutative-algebra.md#discretely-valued-field), plot coefficient exponents against their [valuations](algebra.md#valuation). A lower [Newton polygon](#newton-polygon) segment of slope $s$ and horizontal length $r$ accounts for exactly $r$ roots of [valuation](algebra.md#valuation) $-s$, counted with multiplicity in an [algebraic closure](algebra.md#algebraic-closure). Zero coefficients are omitted. Reflecting the horizontal axis changes the sign of every slope, so slope conventions must be fixed before reading root [valuations](algebra.md#valuation).

#### Denominator criterion for Newton polygon irreducibility

↑ **Parent:** [Newton polygon](#newton-polygon)

If a monic degree-$n$ polynomial over a discretely valued field with normalized valuation has all its roots of valuation $a/n$, where $\gcd(a,n)=1$, then it is irreducible. Each irreducible factor of degree $d$ has constant term of valuation $da/n\in\mathbb Z$, forcing $n\mid d$. Equivalently, a single [Newton polygon](#newton-polygon) segment of relatively prime horizontal and vertical lengths gives irreducibility.

### Ramification index

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramification_index)

For a finite extension $L/K$ of non-Archimedean local fields, the ramification index $e(L/K)$ is the index of the value group of $K$ in that of $L$. Normalized valuations satisfy $v_L|_K=e(L/K)v_K$.

#### Ramification forced by a coprime root valuation

↑ **Parent:** [Ramification index](#ramification-index)

Suppose $\alpha^m=a\in\mathbb Q^\times$ in a [number field](algebraic-number-theory.md#number-field) and $\mathfrak p$ lies above $p$. Its normalized integral [valuation](algebra.md#valuation) satisfies $m v_{\mathfrak p}(\alpha)=e_{\mathfrak p/p}v_p(a)$. If $m$ and $v_p(a)$ are coprime, then $m\mid e_{\mathfrak p/p}$. In a degree-$m$ field the [fundamental identity for prime decomposition](algebraic-number-theory.md#fundamental-identity-for-prime-decomposition) forces a unique prime, [ramification index](#ramification-index) $m$, and [residue degree](#residue-degree) one. This detects total [ramification of a prime](algebraic-number-theory.md#ramification-of-a-prime) even when the displayed defining polynomial is not [Eisenstein](commutative-algebra.md#eisenstein-criterion) at $p$.

// Target: algebra.bigb

#### Residue-field degree

↑ **Parent:** [Ramification index](#ramification-index)

The residue-field degree of a finite extension of local fields is $f(L/K)=[k_L:k_K]$, and $[L:K]=e(L/K)f(L/K)$.

#### Totally ramified extension

↑ **Parent:** [Ramification index](#ramification-index)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_ramified_extension)

A finite extension of local fields is totally ramified when its [residue-field degree](#residue-field-degree) is one, equivalently when its [ramification index](#ramification-index) equals its field degree.

##### Unramified base change preserves total ramification

↑ **Parent:** [Totally ramified extension](#totally-ramified-extension)

If $L/K$ is an [unramified extension](#unramified-extension) and $M/K$ is a [totally ramified extension](#totally-ramified-extension) of non-Archimedean [local fields](#local-field) inside a fixed [algebraic closure](algebra.md#algebraic-closure), then $LM/L$ is totally ramified of degree $[M:K]$. A [uniformizer](commutative-algebra.md#uniformizer) of $M$ has an [Eisenstein polynomial](#eisenstein-polynomial) over $K$. Since a [uniformizer](commutative-algebra.md#uniformizer) of $K$ remains a [uniformizer](commutative-algebra.md#uniformizer) in $L$, that polynomial remains Eisenstein over $L$ and generates $LM$.

###### Cyclic quartic local extension without a totally ramified complement

↑ **Parent:** [Unramified base change preserves total ramification](#unramified-base-change-preserves-total-ramification)

Let $K=\mathbb Q_3$, $L=K(i)$ with $i^2=-1$, and $\alpha^2=3(1+i)$. The extension $L/K$ is [unramified](#unramified-extension) quadratic, whereas $N=L(\alpha)$ is [totally ramified](#totally-ramified-extension) quadratic over $L$, by the [Eisenstein polynomial](#eisenstein-polynomial) $T^2-3(1+i)$. Also $i=\alpha^2/3-1$, so $N=K(\alpha)$. The [Hensel lemma](#hensel-s-lemma) gives $r\in K$ with $r^2=-2$. Put $\beta=(1+i)/r$; then $\beta^2=-i$ and $\beta\overline\beta=-1$. Consequently $i\mapsto-i$, $\alpha\mapsto\beta\alpha$ defines an automorphism whose square fixes $i$ and negates $\alpha$. It generates the cyclic [Galois group](galois-theory.md#galois-group) of order four. Its unique quadratic subfield is $L$, which is unramified. A decomposition as an unramified field and a totally ramified field would require a totally ramified quadratic subfield, and therefore cannot exist.

##### Eisenstein generator of a totally ramified extension

↑ **Parent:** [Totally ramified extension](#totally-ramified-extension)

A finite extension $L/K$ of complete discretely valued fields is totally ramified exactly when $L=K(\alpha)$ for a root $\alpha$ of an [Eisenstein polynomial](#eisenstein-polynomial) over $\mathcal O_K$. In the reverse direction one may take $\alpha$ to be any [uniformizer](commutative-algebra.md#uniformizer) of $L$.

### p-adic unit

↑ **Parent:** [Local field](#local-field)

A [p-adic unit](#p-adic-unit) is an invertible element of the [ring](commutative-algebra.md#ring) $\mathbb Z_p$. For a [p-adic integer](number-theory.md#p-adic-integer) $x$, this is equivalent to $v_p(x)=0$, $|x|_p=1$, or a nonzero initial [p-adic digit](number-theory.md#p-adic-digit) $b_0$. A [rational number](number-theory.md#rational-number) $a/b$ is a [p-adic unit](#p-adic-unit) when neither its reduced [numerator](number-theory.md#numerator) nor its [denominator](number-theory.md#denominator) is divisible by $p$.

Thus $3$ and $1/3$ are [p-adic units](#p-adic-unit) at $p=2$, while $2$ is a [p-adic integer](number-theory.md#p-adic-integer) with no inverse inside $\mathbb Z_2$. The [modular inversion converges to a p-adic inverse](number-theory.md#modular-inversion-converges-to-a-p-adic-inverse) construction computes the inverse of an integer unit to arbitrary finite precision.

#### Unit square classes of the p-adic integers

↑ **Parent:** [P-adic unit](#p-adic-unit)

For odd $p$, a [p-adic unit](#p-adic-unit) is a square exactly when its residue is a square, by the [Hensel lemma](#hensel-s-lemma). Its unit square-class group is $C_2$. For $p=2$, a unit is a square exactly when it is congruent to one modulo eight, by the [strong form of Hensel lemma](#strong-form-of-hensel-lemma). The four [square classes](galois-theory.md#square-class) are represented by $1,3,5,7$, giving $C_2\times C_2$.

#### 2-adic unit

↑ **Parent:** [P-adic unit](#p-adic-unit)

A 2-adic unit is an odd element of $\mathbb Z_2$. It is a square in $\mathbb Z_2^\times$ exactly when it is congruent to $1$ modulo $8$.

##### Digit lifting for square roots of 2-adic units

↑ **Parent:** [2-adic unit](#2-adic-unit)

An odd square is congruent to one modulo eight. Conversely, for $u\equiv1\pmod8$, begin with $x_3=1$ and $x_n^2\equiv u\pmod{2^n}$. For $n\ge3$, adding $\varepsilon_n2^{n-1}$ changes the square by $\varepsilon_n2^nx_n$ modulo $2^{n+1}$. Since $x_n$ is odd, one choice of $\varepsilon_n\in\{0,1\}$ gives the next congruence. The corrections tend to zero 2-adically, so completeness produces an odd square root. This directly proves the unit square criterion without needing a unit derivative in [Hensel lemma](#hensel-s-lemma).

##### Square-class group of the 2-adic numbers

↑ **Parent:** [2-adic unit](#2-adic-unit)

An odd $2$-adic unit is a square exactly when it is congruent to $1$ modulo $8$. Valuation parity and the four odd residue classes modulo $8$ therefore give

$$
\mathbb Q_2^\times/(\mathbb Q_2^\times)^2
\cong(\mathbb Z/2\mathbb Z)^3,
$$

with generators represented by $-1$, $2$, and $5$.

###### Quadratic extensions of the 2-adic numbers

↑ **Parent:** [Square-class group of the 2-adic numbers](#square-class-group-of-the-2-adic-numbers)

The three generators $-1,2,5$ of the [square-class group of the 2-adic numbers](#square-class-group-of-the-2-adic-numbers) give these seven distinct extensions. In characteristic different from two, completing the square shows every quadratic extension is of this form, and comparing coefficients in $\sqrt e=a+b\sqrt d$ proves that two such fields coincide precisely when $e/d$ is a square. The only unramified member is $\mathbb Q_2(\sqrt5)$: $(1+\sqrt5)/2$ is integral with irreducible reduction $X^2+X+1$. Conversely any unramified quadratic extension has that residue field, and [Hensel lemma](#hensel-s-lemma) lifts a residue root of $X^2-X-1$, recovering the same field.

###### Ramification in the quadratic extension generated by the square root of two

↑ **Parent:** [Quadratic extensions of the 2-adic numbers](#quadratic-extensions-of-the-2-adic-numbers)

In $L=\mathbb Q_2(\sqrt2)$, set $\pi=\sqrt2$ and normalize $v_L(\pi)=1$, so $v_L(2)=2$. The two terms of $a+b\pi$ have valuations of opposite parity, giving $\mathcal O_L=\mathbb Z_2\oplus\mathbb Z_2\pi$. The nonidentity automorphism sends $\pi$ to $-\pi$, and $v_L(-2\pi)=3$. The [lower ramification numbering](#lower-ramification-numbering) therefore gives the displayed groups. The different exponent is three.

#### pth-power criterion for p-adic units

↑ **Parent:** [P-adic unit](#p-adic-unit)

For an odd prime $p$ and $\alpha\in\mathbb Z_p^\times$,

$$
\alpha\in(\mathbb Z_p^\times)^p
\quad\Longleftrightarrow\quad
\alpha\bmod p^2\in((\mathbb Z/p^2\mathbb Z)^\times)^p.
$$

This follows from $\mathbb Z_p^\times\cong\mu_{p-1}\times(1+p\mathbb Z_p)$ and $(1+p\mathbb Z_p)^p=1+p^2\mathbb Z_p$.

#### Principal unit

↑ **Parent:** [P-adic unit](#p-adic-unit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_unit)

For a non-Archimedean local field $K$ with maximal ideal $\mathfrak m_K$, a principal unit is an element of $1+\mathfrak m_K$. The higher principal-unit groups are $1+\mathfrak m_K^n$.

##### Prime-to-residue-characteristic power map on principal units

↑ **Parent:** [Principal unit](#principal-unit)

In a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) of residue characteristic $p$, the power map $u\mapsto u^m$ is a bijection on $1+\mathfrak m$ when $p\nmid m$. For a [principal unit](#principal-unit) $a$, the [Hensel lemma](#hensel-s-lemma) lifts the simple residue root one of $T^m-a$ uniquely. This can absorb principal-unit factors in tame radical descriptions of [local fields](#local-field).

##### Higher principal-unit group

↑ **Parent:** [Principal unit](#principal-unit)

For a non-Archimedean local field $K$, the $n$th higher principal-unit group is $1+\mathfrak m_K^n$. These groups form a decreasing filtration of the [principal units](#principal-unit).

###### Successive quotients of principal-unit groups

↑ **Parent:** [Higher principal-unit group](#higher-principal-unit-group)

For $r\geq1$, the map $1+\pi^r a\mapsto\bar a$ is a surjective group homomorphism to the additive [residue field](commutative-algebra.md#residue-field) with kernel $U_{r+1}$. The extra product term is divisible by $\pi^{r+1}$. Thus each quotient has cardinality $|k|$, a useful count when splitting the [unit group](algebra.md#unit-group) by roots of unity.

###### Cube map on 3-adic principal units

↑ **Parent:** [Higher principal-unit group](#higher-principal-unit-group)

The cube of $1+3t$ is $1+9(t+3t^2+3t^3)$. Conversely the [polynomial](polynomial.md) $T+3T^2+3T^3-a$ has a unique simple residue root modulo three for each $a\in\mathbb Z_3$, so [Hensel lemma](#hensel-s-lemma) produces a cube root of every $1+9a$. Thus the [principal units](#principal-unit) modulo their cubes have order three. The change of variable removes the derivative obstruction that prevents direct simple-root lifting for $X^3-u$.

##### Principal-unit logarithm

↑ **Parent:** [Principal unit](#principal-unit)

For a finite extension $K/\mathbb Q_p$ and all sufficiently large $r$, the [p-adic logarithm](#p-adic-logarithm) and [p-adic exponential](#p-adic-exponential-function) are inverse group isomorphisms

$$
1+\mathfrak m_K^r\cong(\mathfrak m_K^r,+).
$$

#### Cube-class group of the 3-adic numbers

↑ **Parent:** [P-adic unit](#p-adic-unit)

The valuation and first principal-unit digit give

$$
\mathbb Q_3^\times/(\mathbb Q_3^\times)^3
\cong\mathbb Z/3\mathbb Z\times\mathbb Z/3\mathbb Z.
$$

### Roots of unity in a p-adic field

↑ **Parent:** [Local field](#local-field)

The roots of unity in a finite extension $K/\mathbb Q_p$ form a finite group. Each element of their prime-to-$p$ part is a [Teichmuller representative](#teichmuller-representative), while any $p$-power part lies among the [principal units](#principal-unit).

#### Valuation of a primitive p-power root of unity

↑ **Parent:** [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)

In a mixed-characteristic [discretely valued field](commutative-algebra.md#discretely-valued-field), a primitive $p^a$th [root of unity](algebra.md#root-of-unity) reduces to one. For every $j$ prime to $p$, the ratio $(\zeta^j-1)/(\zeta-1)$ is a unit, so all factors of $\Phi_{p^a}(1)=p$ have the same valuation. Taking valuations gives the formula. Because the left side is a positive integer for a normalized valuation, the existence of such a root forces $p^{a-1}(p-1)\mid v(p)$, bounding the possible $p$-power torsion.

##### Roots of unity at the tame ramification boundary

↑ **Parent:** [Valuation of a primitive p-power root of unity](#valuation-of-a-primitive-p-power-root-of-unity)

For odd $p$, both possibilities occur at $v(p)=p-1$: $\mathbb Q_p(\zeta_p)$ contains $p$-torsion, while $\mathbb Q_p(\sqrt[p-1]{p})$ does not. Both extensions are totally ramified of degree $p-1$ by the [Eisenstein criterion](commutative-algebra.md#eisenstein-criterion). In the second field, if $\zeta_p=1+u\pi$ with $\pi^{p-1}=p$, the cyclotomic equation reduced after division by $p$ would give $1+\bar u^{p-1}=0$ in $\mathbb F_p$, contradicting $\bar u^{p-1}=1$. For $p=2$, $v(2)=1$ always permits the root $-1$, so the torsion exponent is exactly one and the zero-exponent alternative is impossible.

#### Ramification bound for a primitive pth root of unity

↑ **Parent:** [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)

If a finite extension of the [P-adic numbers](#p-adic-number) contains a primitive $p$th [root of unity](algebra.md#root-of-unity) $\zeta$, the identity $p=\prod_{j=1}^{p-1}(1-\zeta^j)$ gives $e=(p-1)v_L(1-\zeta)\geq p-1$. The ratios of these factors reduce to the nonzero integers $j$ in the [residue field](commutative-algebra.md#residue-field). Thus an extension with $e<p-1$ has only roots of unity of order prime to $p$.

#### Roots of unity in the p-adic numbers

↑ **Parent:** [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)

For odd $p$, [Teichmuller representatives](#teichmuller-representative) provide the $p-1$ prime-to-$p$ roots, while the [logarithm isomorphism on deep principal units](#logarithm-isomorphism-on-deep-principal-units) makes $1+p\mathbb Z_p$ torsion-free. At two, the decomposition $\mathbb Z_2^\times=\{1,-1\}\times(1+4\mathbb Z_2)$ leaves exactly two roots.

#### Unit decomposition of the 2-adic Gaussian field

↑ **Parent:** [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)

The [Eisenstein polynomial](#eisenstein-polynomial) of $1-i$ is $T^2-2T+2$, so $\mathbb Q_2(i)$ has [residue field](commutative-algebra.md#residue-field) $\mathbb F_2$ and [ramification index](#ramification-index) two. The four roots $1,i,-1,-i$ have distinct cosets modulo $U_3$, which has index four by the [successive quotients of principal-unit groups](#successive-quotients-of-principal-unit-groups). The [logarithm isomorphism on deep principal units](#logarithm-isomorphism-on-deep-principal-units) gives $U_3\cong(\mathbb Z_2[i],+)$. Hence these four roots split the full unit group, and are all its torsion.

#### Unit group of Q3 zeta3

↑ **Parent:** [Roots of unity in a p-adic field](#roots-of-unity-in-a-p-adic-field)

For $K=\mathbb Q_3(\zeta_3)$, the element $\pi=\zeta_3-1$ is a [uniformizer](commutative-algebra.md#uniformizer) and

$$
\mathcal O_K^\times\cong\mu_6\times(\mathcal O_K,+).
$$

<h3 id="lubin-tate-formal-group">Lubin–Tate formal group</h3>

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lubin–Tate_formal_group)

A [Lubin–Tate formal group](#lubin-tate-formal-group) associated with a [Lubin–Tate series](#lubin-tate-series) $f$ is the unique one-dimensional commutative [formal group law](normalization-of-an-algebraic-curve.md#formal-group-law) $\mathcal F_f$ over the [valuation ring](commutative-algebra.md#valuation-ring) $\mathcal O_K$ for which $f$ is an [endomorphism](algebra.md#endomorphism) with linear coefficient the chosen [uniformizer](commutative-algebra.md#uniformizer) $\pi$. The [Lubin–Tate functional equation lemma](#lubin-tate-functional-equation-lemma) constructs the law and the [endomorphisms](algebra.md#endomorphism) $[a]_f$ for every $a\in\mathcal O_K$, with linear term $aX$. Their addition is given by the law, and their multiplication by composition. Thus the [valuation ring](commutative-algebra.md#valuation-ring) acts on the group; $[\pi]_f=f$.

<h4 id="lubin-tate-series">Lubin–Tate series</h4>

↑ **Parent:** [Lubin–Tate formal group](#lubin-tate-formal-group)

For a [uniformizer](commutative-algebra.md#uniformizer) $\pi$ of a non-Archimedean [local field](#local-field) $K$ with [residue field](commutative-algebra.md#residue-field) of cardinality $q$, a [Lubin–Tate series](#lubin-tate-series) is a series $f(T)\in\mathcal O_K[[T]]$ satisfying

$$
f(T)\equiv\pi T\pmod{T^2},\qquad f(T)\equiv T^q\pmod\pi.
$$

It determines the associated two-variable [Lubin–Tate formal group](#lubin-tate-formal-group). A useful example is $f(T)=\pi T+T^q$. For $K=\mathbb Q_p$ and $\pi=p$, the choice $(1+T)^p-1$ gives the [formal multiplicative group](normalization-of-an-algebraic-curve.md#formal-multiplicative-group) and the [Lubin–Tate cyclotomic example](#lubin-tate-cyclotomic-example).

<h4 id="lubin-tate-change-of-series">Lubin–Tate change of series</h4>

↑ **Parent:** [Lubin–Tate formal group](#lubin-tate-formal-group)

If $f$ and $g$ are Lubin–Tate series for the same [uniformizer](commutative-algebra.md#uniformizer), there is a unique strict isomorphism $h:\mathcal F_f\to\mathcal F_g$ satisfying $h\circ f=g\circ h$ and $h(X)\equiv X\pmod{X^2}$.

<h5 id="lubin-tate-functional-equation-lemma">Lubin–Tate functional equation lemma</h5>

↑ **Parent:** [Lubin–Tate change of series](#lubin-tate-change-of-series)

Given Lubin–Tate series $f,g$ for $\pi$ and a linear form $L=\sum a_iX_i$, there is a unique power series $F\equiv L$ modulo terms of degree two satisfying

$$
f(F(X_1,\ldots,X_n))=F(g(X_1),\ldots,g(X_n)).
$$

Comparison degree by degree determines each homogeneous term; the Lubin–Tate congruences provide the required divisibility by $\pi$.

<h4 id="lubin-tate-torsion">Lubin–Tate torsion</h4>

↑ **Parent:** [Lubin–Tate formal group](#lubin-tate-formal-group)

The $\pi^n$-torsion of a [Lubin–Tate formal group](#lubin-tate-formal-group) is

$$
\mu_{f,n}=\{x\in\overline{\mathfrak m}: [\pi^n]_f(x)=0\}.
$$

It is a free rank-one module over $\mathcal O_K/\pi^n\mathcal O_K$.

<h5 id="lubin-tate-extension">Lubin–Tate extension</h5>

↑ **Parent:** [Lubin–Tate torsion](#lubin-tate-torsion)

Fix a [uniformizer](commutative-algebra.md#uniformizer) $\pi$ of a [local field](#local-field) $K$ and a [Lubin–Tate formal group](#lubin-tate-formal-group) $\mathcal F$. Its nth torsion field is generated by all its $\pi^n$-torsion points. A primitive point $\lambda_n$ generates the [Lubin–Tate torsion](#lubin-tate-torsion) as a free rank-one $\mathcal O_K/\pi^n$-[module](module-theory.md#module-mathematics); therefore $K_{\pi,n}=K(\lambda_n)$. If the residue field has size $q$, the [Eisenstein layers of Lubin–Tate torsion](#eisenstein-layers-of-lubin-tate-torsion) give $[K_{\pi,n}:K]=(q-1)q^{n-1}$ and total ramification.

<h6 id="lubin-tate-cyclotomic-example">Lubin–Tate cyclotomic example</h6>

↑ **Parent:** [Lubin–Tate extension](#lubin-tate-extension)

For $K=\mathbb Q_p$ and $\pi=p$, choose the [Lubin–Tate series](#lubin-tate-series) $f(T)=(1+T)^p-1$. The associated [formal group law](normalization-of-an-algebraic-curve.md#formal-group-law) is the [formal multiplicative group](normalization-of-an-algebraic-curve.md#formal-multiplicative-group). Its torsion points are $\zeta-1$ for $\zeta^{p^n}=1$, so its [Lubin–Tate extension](#lubin-tate-extension) is the [cyclotomic extension of a p-adic field](#cyclotomic-extension-of-a-p-adic-field) $\mathbb Q_p(\mu_{p^n})$. The Galois action $\zeta\mapsto\zeta^a$ gives $(\mathbb Z/p^n\mathbb Z)^{\times}$, including the trivial first layer when $p=2$.

<h6 id="lubin-tate-tower">Lubin–Tate tower</h6>

↑ **Parent:** [Lubin–Tate extension](#lubin-tate-extension)

Choose compatible primitive [Lubin–Tate torsion](#lubin-tate-torsion) points with $[\pi]\lambda_{n+1}=\lambda_n$. Restriction of the [Lubin–Tate Galois action on primitive torsion](#lubin-tate-galois-action-on-primitive-torsion) is reduction of [unit](algebra.md#unit-in-a-ring) classes modulo $\pi^n$. The [inverse limit](module-theory.md#inverse-limit) gives

$$
\operatorname{Gal}(K_\pi/K)\simeq\varprojlim_n(\mathcal O_K/\pi^n)^{\times}\simeq\mathcal O_K^{\times}
$$

as topological groups. This describes the [Galois group](galois-theory.md#galois-group) without invoking local reciprocity.

<h6 id="lubin-tate-galois-action-on-primitive-torsion">Lubin–Tate Galois action on primitive torsion</h6>

↑ **Parent:** [Lubin–Tate extension](#lubin-tate-extension)

For a primitive [Lubin–Tate torsion](#lubin-tate-torsion) point $\lambda_n$, every Galois automorphism has $\sigma(\lambda_n)=[a_\sigma](\lambda_n)$ for a unique [unit](algebra.md#unit-in-a-ring) class $a_\sigma\pmod{\pi^n}$. All torsion points lie in $K(\lambda_n)$ because the integral endomorphism series converge there; hence the torsion field is Galois. The displayed map is an injective homomorphism. Its domain has order $(q-1)q^{n-1}$ by the primitive Eisenstein [polynomial](polynomial.md), equal to the number of [unit](algebra.md#unit-in-a-ring) classes, so it is an isomorphism.

<h5 id="eisenstein-layers-of-lubin-tate-torsion">Eisenstein layers of Lubin–Tate torsion</h5>

↑ **Parent:** [Lubin–Tate torsion](#lubin-tate-torsion)

For $f(X)=\pi X+X^q$ and its iterates $f_n$, the quotient

$$
\Phi_n(X)=\frac{f_n(X)}{f_{n-1}(X)}
=\pi+f_{n-1}(X)^{q-1}
$$

is Eisenstein. A nonzero root of exact level $n$ therefore generates a totally ramified separable extension.

<h5 id="first-lubin-tate-torsion-fields-for-the-p-adic-numbers">First Lubin–Tate torsion fields for the p-adic numbers</h5>

↑ **Parent:** [Lubin–Tate torsion](#lubin-tate-torsion)

The two Lubin–Tate series $(1+X)^p-1$ and $X^p+pX$ for $\mathbb Q_p$ have respective nonzero $p$-torsion points $\zeta_p-1$ and the roots of $X^{p-1}=-p$. A [Lubin–Tate change of series](#lubin-tate-change-of-series) identifies their torsion fields, so

$$
\mathbb Q_p(\zeta_p)=\mathbb Q_p(\sqrt[p-1]{-p}).
$$

### Maximal abelian extension

↑ **Parent:** [Local field](#local-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximal_abelian_extension)

The maximal abelian extension $K^{\mathrm{ab}}$ of a field $K$ is the compositum in a fixed separable closure of all finite abelian extensions of $K$.

#### Weil group

↑ **Parent:** [Maximal abelian extension](#maximal-abelian-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weil_group)

For a non-Archimedean local field $K$, the Weil group is the inverse image of the infinite cyclic subgroup generated by Frobenius under $\operatorname{Gal}(\overline K/K)\to\operatorname{Gal}(\overline k/k)\cong\widehat{\mathbb Z}$. It is dense in the absolute Galois group with its profinite topology.

##### Relative Weil group

↑ **Parent:** [Weil group](#weil-group)

For a Galois extension $L/K$ of non-Archimedean local fields, the relative Weil group consists of the automorphisms whose residue action is an integral power of [Frobenius](#frobenius-automorphism). It fits into

$$
1\longrightarrow I(L/K)\longrightarrow W(L/K)\longrightarrow\mathbb Z\longrightarrow1
$$

when the residue extension is the full algebraic extension.

###### Weil-group topology

↑ **Parent:** [Relative Weil group](#relative-weil-group)

The Weil-group topology makes the [inertia group](#inertia-group) open with its profinite topology and makes the quotient by inertia discrete. It is generally finer than the topology induced from the ambient Galois group.

#### Cyclotomic extension of a p-adic field

↑ **Parent:** [Maximal abelian extension](#maximal-abelian-extension)

The cyclotomic extension $\mathbb Q_p(\zeta_{p^n})/\mathbb Q_p$ is generated by a primitive $p^n$th root of unity. It is totally ramified and has Galois group $(\mathbb Z/p^n\mathbb Z)^\times$.

##### Total ramification criterion for local cyclotomic extensions

↑ **Parent:** [Cyclotomic extension of a p-adic field](#cyclotomic-extension-of-a-p-adic-field)

Here $a\geq0$ and $p\nmid m$. The prime-to-$p$ [roots of unity](algebra.md#root-of-unity) generate an [unramified extension](#unramified-extension) of degree equal to the multiplicative order of $p$ modulo $m$; for $m=1$ this degree is one. Indeed, their distinct residues lift uniquely by [Hensel lemma](#hensel-s-lemma), and the [Frobenius automorphism](#frobenius-automorphism) acts by raising them to $p$. The $p$-power [roots of unity](algebra.md#root-of-unity) generate a [totally ramified extension](#totally-ramified-extension), because the translated [cyclotomic polynomial](galois-theory.md#cyclotomic-polynomial) $\Phi_{p^a}(1+T)$ is Eisenstein. The two fields have trivial intersection and their compositum has the same residue degree as the prime-to-$p$ field, by [unramified base change preserves total ramification](#unramified-base-change-preserves-total-ramification). Thus total ramification is equivalent to $p\equiv1\pmod m$.

#### Local Kronecker-Weber theorem

↑ **Parent:** [Maximal abelian extension](#maximal-abelian-extension)

The local Kronecker-Weber theorem states that every finite abelian extension of $\mathbb Q_p$ is contained in an extension obtained by adjoining roots of unity.

#### Local class field theory

↑ **Parent:** [Maximal abelian extension](#maximal-abelian-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_class_field_theory)

Local class field theory describes the abelian extensions of a local field $K$ through its multiplicative group $K^\times$.

##### Existence theorem of local class field theory

↑ **Parent:** [Local class field theory](#local-class-field-theory)

The finite-index open subgroups of $K^\times$ are exactly the norm subgroups $N_{L/K}(L^\times)$ for finite abelian extensions $L/K$. The subgroup determines $L$ uniquely inside $K^{\mathrm{ab}}$.

##### Local Artin reciprocity

↑ **Parent:** [Local class field theory](#local-class-field-theory)

Local Artin reciprocity gives a continuous homomorphism $\operatorname{Art}_K:K^\times\to\operatorname{Gal}(K^{\mathrm{ab}}/K)$ with dense image. For every finite abelian extension $L/K$, it induces an isomorphism

$$
K^\times/N_{L/K}(L^\times)\cong\operatorname{Gal}(L/K).
$$

###### Hilbert norm residue symbol

↑ **Parent:** [Local Artin reciprocity](#local-artin-reciprocity)

For a [local field](#local-field) $F$ containing $\mu_m$, the symbol is $\operatorname{rec}_F(b)(a^{1/m})/a^{1/m}\in\mu_m$, after fixing a convention for [Local Artin reciprocity](#local-artin-reciprocity). It is independent of the chosen root and bilinear. Its kernel in the second variable is the norm subgroup of $F(a^{1/m})/F$. The [quadratic Hilbert symbol](#quadratic-hilbert-symbol) is the sign-valued case relevant to quadratic forms.

###### Quadratic Hilbert symbol

↑ **Parent:** [Hilbert norm residue symbol](#hilbert-norm-residue-symbol)

The symbol is one exactly when $b$ is a norm from $K_v(\sqrt a)$, and is always one if $a$ is square. Equivalently the conic $z^2=ax^2+by^2$ is isotropic. This proves symmetry. The [cyclic local norm index](#cyclic-local-norm-index) makes the norm subgroup have index two for nonsquare $a$, proving bilinearity and nondegeneracy on local square classes. Also $(a,-a)_v=1$ and $(a,a)_v=(a,-1)_v$.

###### Explicit quadratic Hilbert symbols over the p-adic numbers

↑ **Parent:** [Quadratic Hilbert symbol](#quadratic-hilbert-symbol)

For odd $p$ and [p-adic units](#p-adic-unit) $u,v$, the [quadratic Hilbert symbol](#quadratic-hilbert-symbol) is

$$
(p^\alpha u,p^\beta v)_p=(-1)^{\alpha\beta(p-1)/2}\left(\frac up\right)^\beta\left(\frac vp\right)^\alpha.
$$

The [Legendre symbols](quadratic-residue.md#legendre-symbol) record the two unit [square classes](galois-theory.md#square-class). For $p=2$, put $\epsilon(u)=(u-1)/2\bmod2$ and $\omega(u)=(u^2-1)/8\bmod2$. Then

$$
(2^\alpha u,2^\beta v)_2=(-1)^{\epsilon(u)\epsilon(v)+\alpha\omega(v)+\beta\omega(u)}.
$$

The basis $-1,2,5$ of the [square-class group of the 2-adic numbers](#square-class-group-of-the-2-adic-numbers) gives this formula: its only negative basis pairings are $(-1,-1)_2$ and $(2,5)_2=(5,2)_2$. The first is obstructed by sums of squares modulo four, the second by $x^2-2y^2$ modulo eight; the remaining pairings have explicit [field norm](algebraic-number-theory.md#field-norm) representatives.

###### Hilbert-symbol annihilators of units and unramified square classes

↑ **Parent:** [Quadratic Hilbert symbol](#quadratic-hilbert-symbol)

In the [square-class group of a p-adic field](galois-theory.md#square-class-group-of-a-p-adic-field), the unit [subgroup](group.md#subgroup) consists of classes of even [valuation](algebra.md#valuation). The unramified [subgroup](group.md#subgroup) consists of the trivial class and the unique nonsquare class defining an [unramified extension](#unramified-extension) of degree two. For odd $p$, the two [subgroups](group.md#subgroup) coincide with $\{1,u\}$ for a nonsquare unit $u$. For $p=2$, they are $\{1,-1,5,-5\}$ and $\{1,5\}$. Norms from an unramified quadratic [local field](#local-field) extension have even [valuation](algebra.md#valuation), and every unit is a norm. The norm characterization of the [quadratic Hilbert symbol](#quadratic-hilbert-symbol) therefore gives both displayed annihilator identities. Over $\mathbb Q_2$, the unramified class is $5$ because $(1+\sqrt5)/2$ satisfies $T^2-T-1$, whose reduction modulo two is irreducible and separable.

###### Hilbert reciprocity law

↑ **Parent:** [Quadratic Hilbert symbol](#quadratic-hilbert-symbol)

For nonzero $a,b$ in a [number field](algebraic-number-theory.md#number-field), the product of their [quadratic Hilbert symbols](#quadratic-hilbert-symbol) over all places is one. All but finitely many symbols are one. Over $\mathbb Q$, this is equivalent to quadratic reciprocity with its supplementary laws. It supplies the compatibility relation between the local invariants of a global quadratic form.

###### Local Artin map

↑ **Parent:** [Local Artin reciprocity](#local-artin-reciprocity)

The local Artin map is the reciprocity homomorphism of [Local Artin reciprocity](#local-artin-reciprocity). Its normalization is fixed by choosing whether a [uniformizer](commutative-algebra.md#uniformizer) maps to arithmetic or geometric Frobenius.

###### Cup-product construction of local reciprocity

↑ **Parent:** [Local Artin map](#local-artin-map)

For $G=\operatorname{Gal}(L/K)$, [Tate cohomology of a finite group](group-cohomology.md#tate-cohomology-of-a-finite-group) identifies the source as $\widehat H^{-2}(G,\mathbb Z)$ and the target as $\widehat H^0(G,L^\times)$. Cup product with the [local fundamental class](associative-algebra.md#local-fundamental-class) is an isomorphism; its inverse is the finite [Local Artin map](#local-artin-map). The algebraic cup-product isomorphism applies because every subgroup has first cohomology zero by [Hilbert theorem 90](galois-theory.md#hilbert-s-theorem-90), and second cohomology cyclic of order equal to its size by the [local Brauer invariant](associative-algebra.md#local-brauer-invariant). Compatibility with restriction and corestriction yields the tower and norm compatibility of [Local Artin reciprocity](#local-artin-reciprocity).

<h6 id="lubin-tate-description-of-local-reciprocity">Lubin–Tate description of local reciprocity</h6>

↑ **Parent:** [Local Artin map](#local-artin-map)

With the [arithmetic Frobenius](#frobenius-automorphism) normalization, a chosen [uniformizer](commutative-algebra.md#uniformizer) $\pi$ and [Lubin–Tate formal group](#lubin-tate-formal-group) give these actions on the [Lubin–Tate tower](#lubin-tate-tower) and the [maximal unramified extension](#maximal-unramified-extension). The two fields are linearly disjoint and their compositum is the [maximal abelian extension](#maximal-abelian-extension). The inverse on units is essential: using geometric Frobenius would invert the entire [Local Artin map](#local-artin-map). The finite kernels on a compositum of residue degree $d$ and torsion level $r$ are $\pi^{d\mathbb Z}(1+\pi^r\mathcal O_K)$. They are a basis of finite-index open subgroups, yielding the [profinite completion](topological-group.md#profinite-completion) of $K^\times$ as the abelian [Galois group](galois-theory.md#galois-group).

###### Norm subgroup of a local field extension

↑ **Parent:** [Local Artin reciprocity](#local-artin-reciprocity)

For a finite extension of local fields $L/K$, its norm subgroup is the image of the [field norm](algebraic-number-theory.md#field-norm) $N_{L/K}:L^\times\to K^\times$. For an abelian extension, it is the kernel of the induced local Artin map to $\operatorname{Gal}(L/K)$.

###### Surjectivity of unit norms in unramified extensions

↑ **Parent:** [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)

For a finite [unramified extension](#unramified-extension) of non-Archimedean [local fields](#local-field), the [field norm](algebraic-number-theory.md#field-norm) on residue units is surjective: on a cyclic group of order $q^n-1$ it is exponentiation by $(q^n-1)/(q-1)$ and has image of order $q-1$. For a common [uniformizer](commutative-algebra.md#uniformizer) $\pi$ and $r\geq1$, expansion of the conjugate product gives

$$
N_{L/K}(1+\pi^r a)\equiv1+\pi^r\operatorname{Tr}_{k_L/k_K}(\bar a)\pmod{\pi^{r+1}}.
$$

The [field trace](algebraic-number-theory.md#field-trace) of a finite [finite field](algebra.md#finite-field) extension is onto: its polynomial $X+X^q+\cdots+X^{q^{n-1}}$ is nonzero of degree below $q^n$, so defines a nonzero linear map to the base field. Lift a residue norm and correct successively with elements of $1+\pi^r\mathcal O_L$. The infinite product converges by [completeness](topological-analysis.md#completeness), and its norm is the prescribed unit. This argument also works in positive characteristic and when $p$ divides $n$.

###### Cyclic local norm index

↑ **Parent:** [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)

For a cyclic extension of [p-adic fields](#p-adic-field), the [Herbrand quotient of the local multiplicative group](group-cohomology.md#herbrand-quotient-of-the-local-multiplicative-group) together with [Hilbert theorem 90](galois-theory.md#hilbert-s-theorem-90) gives this index. If the ramification index and residue degree are $e,f$, the norm valuation formula $v_K(Nx)=f v_L(x)$ then gives the unit norm index $e$. In particular all units are norms in an [unramified extension](#unramified-extension).

###### Norm-unit index in an abelian local extension

↑ **Parent:** [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)

If $L/K$ is a finite abelian extension of local fields, then

$$
[\mathcal O_K^\times:N_{L/K}(\mathcal O_L^\times)]=e(L/K).
$$

Indeed, [Local Artin reciprocity](#local-artin-reciprocity) gives total norm index $[L:K]=ef$, while the valuation image of the norm subgroup is $f\mathbb Z$.

###### Norm units in a tamely totally ramified extension

↑ **Parent:** [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)

For a tamely totally ramified extension of degree $q-1$ of a local field with residue field $\mathbb F_q$, the unit norms are exactly the principal units. Reduction sends a unit norm to its $(q-1)$st power, and the [norm-unit index in an abelian local extension](#norm-unit-index-in-an-abelian-local-extension) shows that this containment has the correct index.

###### Norm subgroup of a 2-power cyclotomic extension of the 2-adic numbers

↑ **Parent:** [Norm subgroup of a local field extension](#norm-subgroup-of-a-local-field-extension)

For every positive integer $n$,

$$
N_{\mathbb Q_2(\zeta_{2^n})/\mathbb Q_2}
\bigl(\mathbb Q_2(\zeta_{2^n})^\times\bigr)
=2^{\mathbb Z}(1+2^n\mathbb Z_2).
$$

Under [Local Artin reciprocity](#local-artin-reciprocity), the cyclotomic character identifies the quotient with $(\mathbb Z/2^n\mathbb Z)^\times$: a [uniformizer](commutative-algebra.md#uniformizer) acts trivially on the totally ramified extension, while a [2-adic unit](#2-adic-unit) acts through its residue class modulo $2^n$.

## ↑ Ancestors (4)

1. [Arithmetic](arithmetic.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
