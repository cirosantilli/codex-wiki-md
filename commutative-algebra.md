# Commutative algebra

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutative_algebra)

Commutative algebra studies commutative rings, ideals, modules, and their spectra.

**Table of contents**

- [Norm for a finite free ring extension](#norm-for-a-finite-free-ring-extension)
- [Finite-type integer algebra](#finite-type-integer-algebra)
  - [Finite-field theorem for finitely generated integer algebras](#finite-field-theorem-for-finitely-generated-integer-algebras)
- [Algebraic differential operator ring](#algebraic-differential-operator-ring)
  - [Order of an algebraic differential operator](#order-of-an-algebraic-differential-operator)
    - [First-order algebraic differential operator decomposition](#first-order-algebraic-differential-operator-decomposition)
- [Algebra over a commutative ring](#algebra-over-a-commutative-ring)
  - [Bialgebra](#bialgebra)
    - [Cobraided bialgebra](#cobraided-bialgebra)
    - [Bialgebra scalar cocycle](#bialgebra-scalar-cocycle)
      - [Bialgebra cocycle twist](#bialgebra-cocycle-twist)
    - [Diagonal bialgebra action](#diagonal-bialgebra-action)
- [Ring extension](#ring-extension)
  - [Module-finite ring extension](#module-finite-ring-extension)
  - [Fiber ring](#fiber-ring)
    - [Fiber of the map on spectra](#fiber-of-the-map-on-spectra)
- [Localization of a ring](#localization-of-a-ring)
  - [Total ring of fractions](#total-ring-of-fractions)
  - [Localization commutes with tensor products](#localization-commutes-with-tensor-products)
  - [Localization detects zero elements](#localization-detects-zero-elements)
  - [Multiplicatively closed set](#multiplicatively-closed-set)
    - [Saturated multiplicative subset](#saturated-multiplicative-subset)
      - [Units with no finite prime-union complement](#units-with-no-finite-prime-union-complement)
      - [Saturated complement as a union of prime ideals](#saturated-complement-as-a-union-of-prime-ideals)
  - [Universal property of localization](#universal-property-of-localization)
    - [Localization away from one plus an ideal lies in the Jacobson radical](#localization-away-from-one-plus-an-ideal-lies-in-the-jacobson-radical)
  - [Localization of a module](#localization-of-a-module)
    - [Vanishing criterion in a module localization](#vanishing-criterion-in-a-module-localization)
    - [Exactness of localization](#exactness-of-localization)
      - [Injectivity of a module map is detected at maximal localizations](#injectivity-of-a-module-map-is-detected-at-maximal-localizations)
    - [Kernel of localization away from one plus an ideal](#kernel-of-localization-away-from-one-plus-an-ideal)
      - [Non-Noetherian failure of the intersection formula for localization](#non-noetherian-failure-of-the-intersection-formula-for-localization)
  - [Integer localization at a set of primes](#integer-localization-at-a-set-of-primes)
    - [Finite quotients of the integers localized away from one prime](#finite-quotients-of-the-integers-localized-away-from-one-prime)
  - [Prime ideal correspondence for localization](#prime-ideal-correspondence-for-localization)
    - [Spectrum of localization away from one plus an ideal](#spectrum-of-localization-away-from-one-plus-an-ideal)
  - [Localization of a Noetherian ring](#localization-of-a-noetherian-ring)
    - [Localization of a Dedekind domain](#localization-of-a-dedekind-domain)
  - [Localization at a prime ideal](#localization-at-a-prime-ideal)
    - [Domain prime localizations do not imply a domain](#domain-prime-localizations-do-not-imply-a-domain)
- [Integral element](#integral-element)
  - [Finite-module criterion for integrality](#finite-module-criterion-for-integrality)
  - [Integral extension](#integral-extension)
    - [Integral field extension forces the base domain to be a field](#integral-field-extension-forces-the-base-domain-to-be-a-field)
    - [Localization of an integral extension at a prime need not be integral](#localization-of-an-integral-extension-at-a-prime-need-not-be-integral)
    - [Integral extensions preserve Krull dimension](#integral-extensions-preserve-krull-dimension)
      - [Krull dimension of rings of algebraic integers](#krull-dimension-of-rings-of-algebraic-integers)
      - [Dimension of a monic plane hypersurface](#dimension-of-a-monic-plane-hypersurface)
    - [Lying-over theorem](#lying-over-theorem)
    - [Going up and going down](#going-up-and-going-down)
      - [Going-up theorem](#going-up-theorem)
      - [Going-down theorem](#going-down-theorem)
    - [Incomparability theorem for integral extensions](#incomparability-theorem-for-integral-extensions)
    - [Ideal contraction rigidity under an integral extension](#ideal-contraction-rigidity-under-an-integral-extension)
    - [Contraction of a maximal ideal under an integral extension](#contraction-of-a-maximal-ideal-under-an-integral-extension)
    - [Fiber primes of an integral extension](#fiber-primes-of-an-integral-extension)
    - [Subalgebra generated by finitely many integral elements](#subalgebra-generated-by-finitely-many-integral-elements)
    - [Integrally closed domain](#integrally-closed-domain)
    - [Integral closure](#integral-closure)
      - [Finiteness of integral closure in a finite separable extension](#finiteness-of-integral-closure-in-a-finite-separable-extension)
      - [Integral field basis by denominator clearing](#integral-field-basis-by-denominator-clearing)
      - [Integral closure as an intersection of valuation rings](#integral-closure-as-an-intersection-of-valuation-rings)
      - [Integral closure of a graded ring is graded](#integral-closure-of-a-graded-ring-is-graded)
- [Krull dimension](#krull-dimension)
  - [Prime chain](#prime-chain)
  - [Noether normalization lemma](#noether-normalization-lemma)
    - [Noether normalization by weighted substitutions](#noether-normalization-by-weighted-substitutions)
      - [Finite flat Noether normalization of an affine hypersurface](#finite-flat-noether-normalization-of-an-affine-hypersurface)
    - [Noether normalization of the quadratic surface xy plus yz plus zx](#noether-normalization-of-the-quadratic-surface-xy-plus-yz-plus-zx)
  - [Height of an ideal](#height-of-an-ideal)
    - [Height of a prime ideal](#height-of-a-prime-ideal)
      - [Polynomial-ring height and dimension formula](#polynomial-ring-height-and-dimension-formula)
    - [Prime avoidance](#prime-avoidance)
    - [Krull principal ideal theorem](#krull-principal-ideal-theorem)
      - [Principal prime in a Noetherian local ring lemma](#principal-prime-in-a-noetherian-local-ring-lemma)
      - [Krull height theorem](#krull-height-theorem)
        - [Generator bound for primary-ideal length](#generator-bound-for-primary-ideal-length)
      - [Prime ideals between a three-prime chain](#prime-ideals-between-a-three-prime-chain)
        - [Infinitude of intermediate-height prime ideals](#infinitude-of-intermediate-height-prime-ideals)
  - [Dimension theorem for Noetherian local rings](#dimension-theorem-for-noetherian-local-rings)
    - [System of parameters](#system-of-parameters)
    - [Dimension drop by a non-zero-divisor](#dimension-drop-by-a-non-zero-divisor)
- [Polynomial ring](#polynomial-ring)
  - [Skew polynomial ring of an automorphism](#skew-polynomial-ring-of-an-automorphism)
    - [Skew Laurent polynomial ring](#skew-laurent-polynomial-ring)
      - [Skew Laurent extensions of domains are domains](#skew-laurent-extensions-of-domains-are-domains)
      - [Integral Heisenberg group algebra as a skew Laurent ring](#integral-heisenberg-group-algebra-as-a-skew-laurent-ring)
  - [Laurent polynomial ring](#laurent-polynomial-ring)
    - [Unit of a Laurent polynomial ring](#unit-of-a-laurent-polynomial-ring)
    - [Laurent normalization by a monomial change of variables](#laurent-normalization-by-a-monomial-change-of-variables)
    - [Noetherianity of subalgebras of a one-variable Laurent polynomial ring](#noetherianity-of-subalgebras-of-a-one-variable-laurent-polynomial-ring)
    - [Separating finite Laurent support by an integer weight](#separating-finite-laurent-support-by-an-integer-weight)
  - [Integer-valued polynomial](#integer-valued-polynomial)
    - [Binomial polynomial](#binomial-polynomial)
  - [Automorphism of a polynomial ring](#automorphism-of-a-polynomial-ring)
  - [Reduction of an integer polynomial modulo a prime](#reduction-of-an-integer-polynomial-modulo-a-prime)
  - [Unit in a polynomial ring](#unit-in-a-polynomial-ring)
  - [McCoy theorem](#mccoy-theorem)
- [Maximal ideal](#maximal-ideal)
  - [Residue field](#residue-field)
    - [Residue-field extension](#residue-field-extension)
    - [Residue characteristic](#residue-characteristic)
  - [Maximal spectrum](#maximal-spectrum)
  - [Maximal ideal quotient criterion](#maximal-ideal-quotient-criterion)
- [Local ring](#local-ring)
  - [Local homomorphism of local rings](#local-homomorphism-of-local-rings)
  - [Local integral domain](#local-integral-domain)
  - [Cotangent space of a local ring](#cotangent-space-of-a-local-ring)
    - [Embedding dimension](#embedding-dimension)
  - [Regular local ring](#regular-local-ring)
    - [Regular system of parameters](#regular-system-of-parameters)
      - [Formal expansion at a smooth point](#formal-expansion-at-a-smooth-point)
    - [Formal power series preserve regular local rings](#formal-power-series-preserve-regular-local-rings)
    - [Associated graded ring of a regular local ring](#associated-graded-ring-of-a-regular-local-ring)
  - [Valuation ring](#valuation-ring)
    - [Principal ideal criterion for a nontrivial rank-one valuation ring](#principal-ideal-criterion-for-a-nontrivial-rank-one-valuation-ring)
    - [Valuation domination lemma](#valuation-domination-lemma)
    - [Valuation rings are integrally closed](#valuation-rings-are-integrally-closed)
    - [Discrete valuation ring](#discrete-valuation-ring)
      - [Complete discretely valued field](#complete-discretely-valued-field)
      - [Digit expansion in a discretely valued field](#digit-expansion-in-a-discretely-valued-field)
      - [One-dimensional normal local rings are discrete valuation rings](#one-dimensional-normal-local-rings-are-discrete-valuation-rings)
      - [Complete discrete valuation ring](#complete-discrete-valuation-ring)
      - [Discrete valuation](#discrete-valuation)
        - [Discretely valued field](#discretely-valued-field)
        - [Value group](#value-group)
      - [Uniformizer](#uniformizer)
- [Dedekind domain](#dedekind-domain)
  - [Two generators for an ideal in a Dedekind domain](#two-generators-for-an-ideal-in-a-dedekind-domain)
  - [Unique factorization of ideals in a Dedekind domain](#unique-factorization-of-ideals-in-a-dedekind-domain)
    - [Prime-ideal valuation in a Dedekind domain](#prime-ideal-valuation-in-a-dedekind-domain)
  - [Principal maximal ideal in a one-dimensional normal local domain](#principal-maximal-ideal-in-a-one-dimensional-normal-local-domain)
- [Ring](#ring)
  - [Zero ring](#zero-ring)
  - [Perfect ring of characteristic p](#perfect-ring-of-characteristic-p)
  - [Opposite ring](#opposite-ring)
  - [Subring](#subring)
  - [Topological ring](#topological-ring)
    - [Pro-p ring](#pro-p-ring)
    - [Adic topology](#adic-topology)
      - [Completed localization of an adic ring](#completed-localization-of-an-adic-ring)
      - [Adic completion of a module](#adic-completion-of-a-module)
        - [Power-series presentation of an adic completion](#power-series-presentation-of-an-adic-completion)
        - [Surjectivity on adic completions](#surjectivity-on-adic-completions)
  - [Von Neumann regular ring](#von-neumann-regular-ring)
  - [Direct product of rings](#direct-product-of-rings)
  - [Characteristic of a ring](#characteristic-of-a-ring)
  - [Division ring](#division-ring)
  - [Simple ring](#simple-ring)
  - [Semisimple ring](#semisimple-ring)
  - [Group ring](#group-ring)
    - [Group rings of poly-(cyclic or finite) groups are Noetherian](#group-rings-of-poly-cyclic-or-finite-groups-are-noetherian)
    - [Augmentation ideal](#augmentation-ideal)
      - [Cyclic finite quotients of the p-adic augmentation filtration](#cyclic-finite-quotients-of-the-p-adic-augmentation-filtration)
      - [Nilpotence of a p-group augmentation ideal](#nilpotence-of-a-p-group-augmentation-ideal)
      - [Augmentation ideal of the infinite cyclic group](#augmentation-ideal-of-the-infinite-cyclic-group)
  - [Noncommutative ring](#noncommutative-ring)
  - [Nilpotent](#nilpotent)
  - [Commutative ring](#commutative-ring)
    - [Associate element](#associate-element)
    - [Regular sequence](#regular-sequence)
      - [Depth of a Noetherian local ring](#depth-of-a-noetherian-local-ring)
    - [Dual number](#dual-number)
      - [Periodic resolution over dual numbers](#periodic-resolution-over-dual-numbers)
    - [Formal power series](#formal-power-series)
      - [Noetherianity of formal power series rings](#noetherianity-of-formal-power-series-rings)
      - [Topologies on integral formal power series](#topologies-on-integral-formal-power-series)
      - [Compositional inverse of a formal power series](#compositional-inverse-of-a-formal-power-series)
        - [Recursive construction of a compositional inverse](#recursive-construction-of-a-compositional-inverse)
      - [Formal power series over a local ring](#formal-power-series-over-a-local-ring)
        - [Cotangent space of a formal power series ring](#cotangent-space-of-a-formal-power-series-ring)
      - [Reducedness of a formal power series ring](#reducedness-of-a-formal-power-series-ring)
      - [Formal power series module](#formal-power-series-module)
      - [Noetherianity of a formal power series ring](#noetherianity-of-a-formal-power-series-ring)
        - [Coefficient ideals of a formal power series ideal](#coefficient-ideals-of-a-formal-power-series-ideal)
      - [Ordinary generating function](#ordinary-generating-function)
    - [Reduced ring](#reduced-ring)
      - [Reducedness is detected by prime localizations](#reducedness-is-detected-by-prime-localizations)
  - [Graded ring](#graded-ring)
    - [Graded module](#graded-module)
      - [Super vector space](#super-vector-space)
      - [Degree-one localization of a graded module](#degree-one-localization-of-a-graded-module)
      - [Graded shift](#graded-shift)
    - [Graded algebra](#graded-algebra)
      - [Indecomposable quotient of an augmented algebra](#indecomposable-quotient-of-an-augmented-algebra)
      - [Graded tensor product](#graded-tensor-product)
      - [Graded commutator](#graded-commutator)
      - [Differential graded algebra](#differential-graded-algebra)
        - [Commutative differential graded algebra](#commutative-differential-graded-algebra)
      - [Divided power algebra](#divided-power-algebra)
      - [Graded derivation](#graded-derivation)
      - [Graded commutative algebra](#graded-commutative-algebra)
        - [Graded symmetric algebra](#graded-symmetric-algebra)
      - [Homogeneous element of a graded algebra](#homogeneous-element-of-a-graded-algebra)
      - [Gerstenhaber algebra](#gerstenhaber-algebra)
      - [Graded Leibniz rule](#graded-leibniz-rule)
      - [Standard graded algebra](#standard-graded-algebra)
    - [Associated graded ring](#associated-graded-ring)
      - [Associated graded module](#associated-graded-module)
        - [Exactness of associated graded modules for induced filtrations](#exactness-of-associated-graded-modules-for-induced-filtrations)
      - [Pole dimension of an associated graded ring](#pole-dimension-of-an-associated-graded-ring)
      - [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial)
        - [Hilbert–Samuel growth dimension](#hilbert-samuel-growth-dimension)
          - [Prime-chain lower bound for local length](#prime-chain-lower-bound-for-local-length)
        - [Hilbert–Samuel function](#hilbert-samuel-function)
          - [Hilbert–Samuel multiplicity](#hilbert-samuel-multiplicity)
    - [Hilbert series and Hilbert polynomial](#hilbert-series-and-hilbert-polynomial)
      - [Hilbert series](#hilbert-series)
        - [Hilbert function](#hilbert-function)
          - [Quasipolynomial](#quasipolynomial)
        - [Hilbert-Serre theorem](#hilbert-serre-theorem)
          - [Hilbert-Serre theorem for an additive coefficient function](#hilbert-serre-theorem-for-an-additive-coefficient-function)
          - [Hilbert series multiplication exact sequence](#hilbert-series-multiplication-exact-sequence)
          - [Growth of a finitely generated commutative algebra](#growth-of-a-finitely-generated-commutative-algebra)
            - [Growth of the two-variable Laurent polynomial algebra](#growth-of-the-two-variable-laurent-polynomial-algebra)
        - [Poincare series of a graded module](#poincare-series-of-a-graded-module)
  - [Ideal](#ideal)
    - [Monomial ideal](#monomial-ideal)
      - [Reverse-inclusion well-quasi-ordering of monomial ideals](#reverse-inclusion-well-quasi-ordering-of-monomial-ideals)
    - [Pure ideal](#pure-ideal)
    - [Zero ideal](#zero-ideal)
    - [Ideal quotient](#ideal-quotient)
    - [Unit ideal](#unit-ideal)
      - [Unit-ideal identity for powers](#unit-ideal-identity-for-powers)
    - [Union of three incomparable nonprime ideals](#union-of-three-incomparable-nonprime-ideals)
    - [Conormal module](#conormal-module)
    - [Irreducible ideal](#irreducible-ideal)
      - [Irreducible ideals are primary in Noetherian rings](#irreducible-ideals-are-primary-in-noetherian-rings)
    - [Radical ideal](#radical-ideal)
    - [Colon ideal](#colon-ideal)
    - [Nilpotent ideal](#nilpotent-ideal)
      - [Nilpotence index of an ideal](#nilpotence-index-of-an-ideal)
    - [Oka family](#oka-family)
      - [Prime ideal principle for an Oka family](#prime-ideal-principle-for-an-oka-family)
    - [Two-sided ideal](#two-sided-ideal)
      - [Square-zero ideal](#square-zero-ideal)
        - [Square-zero extension of an algebra](#square-zero-extension-of-an-algebra)
        - [Square-zero unit subgroup](#square-zero-unit-subgroup)
    - [Primary ideal](#primary-ideal)
      - [Primary ideals can need more generators than the maximal ideal](#primary-ideals-can-need-more-generators-than-the-maximal-ideal)
      - [Radical of a primary ideal](#radical-of-a-primary-ideal)
      - [Minimal primary decomposition](#minimal-primary-decomposition)
        - [First uniqueness theorem for primary decomposition](#first-uniqueness-theorem-for-primary-decomposition)
        - [Embedded primary component](#embedded-primary-component)
        - [Isolated prime of a primary decomposition](#isolated-prime-of-a-primary-decomposition)
        - [Second uniqueness theorem for primary decomposition](#second-uniqueness-theorem-for-primary-decomposition)
    - [Generating set of an ideal](#generating-set-of-an-ideal)
    - [Principal ideal](#principal-ideal)
    - [Product of ideals](#product-of-ideals)
      - [Idempotent ideal](#idempotent-ideal)
    - [Intersection of ideals](#intersection-of-ideals)
    - [Comaximal ideals](#comaximal-ideals)
    - [Prime-power ideal](#prime-power-ideal)
    - [Ideal approximation theorem](#ideal-approximation-theorem)
    - [Reduction modulo an ideal](#reduction-modulo-an-ideal)
      - [Quotient ring](#quotient-ring)
        - [Congruence modulo an ideal](#congruence-modulo-an-ideal)
    - [Homogeneous ideal](#homogeneous-ideal)
    - [Radical of an ideal](#radical-of-an-ideal)
      - [Finite prime-intersection representation of a radical](#finite-prime-intersection-representation-of-a-radical)
      - [Nilradical](#nilradical)
        - [Nilradical that is not nilpotent](#nilradical-that-is-not-nilpotent)
        - [Nilradical as the intersection of prime ideals](#nilradical-as-the-intersection-of-prime-ideals)
  - [Ring homomorphism](#ring-homomorphism)
    - [Ring endomorphism](#ring-endomorphism)
      - [Ring automorphism](#ring-automorphism)
    - [Kernel of a ring homomorphism](#kernel-of-a-ring-homomorphism)
    - [Extension and contraction of ideals](#extension-and-contraction-of-ideals)
      - [Extension of an ideal](#extension-of-an-ideal)
      - [Contraction of an ideal](#contraction-of-an-ideal)
    - [Evaluation homomorphism](#evaluation-homomorphism)
    - [First isomorphism theorem for rings](#first-isomorphism-theorem-for-rings)
  - [Idempotent](#idempotent)
    - [Orthogonal idempotent](#orthogonal-idempotent)
    - [Primitive idempotent](#primitive-idempotent)
      - [Triangular primitive-idempotent decomposition](#triangular-primitive-idempotent-decomposition)
      - [Primitive idempotents under a surjection of commutative Artinian ideals](#primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals)
    - [Idempotent lifting](#idempotent-lifting)
      - [Idempotent refinement theorem](#idempotent-refinement-theorem)
- [Integral domain](#integral-domain)
  - [Fractional ideal](#fractional-ideal)
    - [Invertible fractional ideal](#invertible-fractional-ideal)
    - [Principal fractional ideal](#principal-fractional-ideal)
    - [Integral ideal](#integral-ideal)
  - [Finite integral domain is a field](#finite-integral-domain-is-a-field)
  - [Prime element](#prime-element)
  - [Irreducible element](#irreducible-element)
  - [Atomic domain](#atomic-domain)
  - [Greatest-common-divisor domain](#greatest-common-divisor-domain)
    - [Euclid lemma in a greatest-common-divisor domain](#euclid-lemma-in-a-greatest-common-divisor-domain)
  - [Field of fractions](#field-of-fractions)
  - [Principal ideal domain](#principal-ideal-domain)
    - [Nonprincipal coordinate ideal in two variables](#nonprincipal-coordinate-ideal-in-two-variables)
    - [Every principal ideal domain is a unique factorization domain](#every-principal-ideal-domain-is-a-unique-factorization-domain)
    - [Submodule theorem for free modules over a principal ideal domain](#submodule-theorem-for-free-modules-over-a-principal-ideal-domain)
    - [Euclidean domain](#euclidean-domain)
      - [Norm-Euclidean integers of discriminant minus seven](#norm-euclidean-integers-of-discriminant-minus-seven)
      - [Euclidean function](#euclidean-function)
      - [Gaussian integer](#gaussian-integer)
        - [Primary Gaussian integer](#primary-gaussian-integer)
        - [Finite residue-field theorem for Gaussian integer orders](#finite-residue-field-theorem-for-gaussian-integer-orders)
      - [Eisenstein integer](#eisenstein-integer)
        - [Eisenstein-integer norm](#eisenstein-integer-norm)
        - [Euclidean norm on the Eisenstein integers](#euclidean-norm-on-the-eisenstein-integers)
  - [Bézout domain](#bezout-domain)
- [Ring product decomposition by an idempotent](#ring-product-decomposition-by-an-idempotent)
- [Fiber product of rings](#fiber-product-of-rings)
- [Unit modulo a prime power](#unit-modulo-a-prime-power)
- [Nilpotent element modulo a prime power](#nilpotent-element-modulo-a-prime-power)
- [Reduction map on unit groups](#reduction-map-on-unit-groups)
- [Polynomial content](#polynomial-content)
  - [Primitive polynomial](#primitive-polynomial)
    - [Gauss lemma for polynomials](#gauss-lemma-for-polynomials)
      - [Multiplicativity of the nonarchimedean polynomial norm](#multiplicativity-of-the-nonarchimedean-polynomial-norm)
      - [Polynomial ring over a unique factorization domain](#polynomial-ring-over-a-unique-factorization-domain)
        - [Integer polynomial ring is not a principal ideal domain](#integer-polynomial-ring-is-not-a-principal-ideal-domain)
      - [Symmetric rational function in two variables](#symmetric-rational-function-in-two-variables)
- [Eisenstein criterion](#eisenstein-criterion)
  - [Total ramification from an Eisenstein polynomial](#total-ramification-from-an-eisenstein-polynomial)
  - [Geometric-sum irreducibility criterion](#geometric-sum-irreducibility-criterion)
- [Odd-valuation obstruction to a rational-function square](#odd-valuation-obstruction-to-a-rational-function-square)
- [Module theory](module-theory.md)
  - [Finite representation type](module-theory.md#finite-representation-type)
  - [Auslander–Reiten quiver](module-theory.md#auslander-reiten-quiver)
    - [Stable Auslander–Reiten quiver](module-theory.md#stable-auslander-reiten-quiver)
  - [Topological group module](module-theory.md#topological-group-module)
  - [Character module](module-theory.md#character-module)
  - [Representation of an associative algebra](module-theory.md#representation-of-an-associative-algebra)
    - [Representation of a Banach algebra](module-theory.md#representation-of-a-banach-algebra)
      - [Algebraically irreducible representation of a Banach algebra](module-theory.md#algebraically-irreducible-representation-of-a-banach-algebra)
        - [Countable annihilation sequence in an irreducible Banach module](module-theory.md#countable-annihilation-sequence-in-an-irreducible-banach-module)
        - [Quotient norm on an irreducible Banach module](module-theory.md#quotient-norm-on-an-irreducible-banach-module)
      - [Normed representation of a Banach algebra](module-theory.md#normed-representation-of-a-banach-algebra)
        - [Johnson's continuity theorem for irreducible normed representations](module-theory.md#johnson-s-continuity-theorem-for-irreducible-normed-representations)
  - [Degeneration of a module](module-theory.md#degeneration-of-a-module)
  - [Hereditary ring](module-theory.md#hereditary-ring)
    - [Basic hereditary algebra path-algebra theorem](module-theory.md#basic-hereditary-algebra-path-algebra-theorem)
    - [Path algebras are hereditary](module-theory.md#path-algebras-are-hereditary)
  - [Regular sequence on a module](module-theory.md#regular-sequence-on-a-module)
  - [Composition series of a module](module-theory.md#composition-series-of-a-module)
    - [Composition factor](module-theory.md#composition-factor)
  - [Uniform module](module-theory.md#uniform-module)
    - [Uniform dimension](module-theory.md#uniform-dimension)
    - [Finite uniform decomposition of a Noetherian module](module-theory.md#finite-uniform-decomposition-of-a-noetherian-module)
  - [Indecomposable module](module-theory.md#indecomposable-module)
    - [Top of an indecomposable projective module](module-theory.md#top-of-an-indecomposable-projective-module)
  - [Fitting lemma](module-theory.md#fitting-lemma)
  - [Krull–Schmidt theorem](module-theory.md#krull-schmidt-theorem)
    - [Krull-Schmidt decomposition](module-theory.md#krull-schmidt-decomposition)
  - [Dual module](module-theory.md#dual-module)
    - [Double dual module](module-theory.md#double-dual-module)
  - [Finitely generated module](module-theory.md#finitely-generated-module)
    - [Minimal number of generators of a module](module-theory.md#minimal-number-of-generators-of-a-module)
    - [Clearing denominators relative to an independent module subset](module-theory.md#clearing-denominators-relative-to-an-independent-module-subset)
    - [Finite generation as a quotient of a finite free module](module-theory.md#finite-generation-as-a-quotient-of-a-finite-free-module)
  - [Artinian module](module-theory.md#artinian-module)
    - [Artinian modules are co-Hopfian](module-theory.md#artinian-modules-are-co-hopfian)
    - [Artinian modules in a short exact sequence](module-theory.md#artinian-modules-in-a-short-exact-sequence)
  - [Filtered colimit of modules](module-theory.md#filtered-colimit-of-modules)
    - [Direct system of abelian groups](module-theory.md#direct-system-of-abelian-groups)
      - [Direct limit of abelian groups](module-theory.md#direct-limit-of-abelian-groups)
        - [Sequential direct limit of multiplication maps on the integers](module-theory.md#sequential-direct-limit-of-multiplication-maps-on-the-integers)
          - [Rational group with square-free denominators](module-theory.md#rational-group-with-square-free-denominators)
  - [Bimodule](module-theory.md#bimodule)
  - [Invariant submodule](module-theory.md#invariant-submodule)
  - [Coinvariant module](module-theory.md#coinvariant-module)
    - [Abelianization over a Zp-extension](module-theory.md#abelianization-over-a-zp-extension)
  - [Support of a module](module-theory.md#support-of-a-module)
  - [Tensor product of modules](module-theory.md#tensor-product-of-modules)
    - [Right exactness of the tensor product](module-theory.md#right-exactness-of-the-tensor-product)
    - [Change-of-rings tensor quotient](module-theory.md#change-of-rings-tensor-quotient)
    - [Tensor product of commutative algebras](module-theory.md#tensor-product-of-commutative-algebras)
      - [Tensor product of field extensions is nonzero](module-theory.md#tensor-product-of-field-extensions-is-nonzero)
    - [Pure tensor](module-theory.md#pure-tensor)
    - [Projectivity of factors of a nonzero finite free tensor product](module-theory.md#projectivity-of-factors-of-a-nonzero-finite-free-tensor-product)
    - [Tensor-nilpotent module](module-theory.md#tensor-nilpotent-module)
    - [Balanced map](module-theory.md#balanced-map)
    - [Universal property of the tensor product of modules](module-theory.md#universal-property-of-the-tensor-product-of-modules)
    - [Tensor-hom adjunction](module-theory.md#tensor-hom-adjunction)
    - [Tensor product and infinite direct product](module-theory.md#tensor-product-and-infinite-direct-product)
  - [Flat module](module-theory.md#flat-module)
    - [Flatness criterion over dual numbers](module-theory.md#flatness-criterion-over-dual-numbers)
    - [Equational criterion for flatness](module-theory.md#equational-criterion-for-flatness)
    - [Free modules are flat](module-theory.md#free-modules-are-flat)
    - [Direct summands of flat modules are flat](module-theory.md#direct-summands-of-flat-modules-are-flat)
    - [Flatness criterion using ideals](module-theory.md#flatness-criterion-using-ideals)
    - [Lambek theorem](module-theory.md#lambek-theorem)
    - [Faithfully flat module](module-theory.md#faithfully-flat-module)
    - [Flatness is local](module-theory.md#flatness-is-local)
    - [Torsion-free module over a principal ideal domain is flat](module-theory.md#torsion-free-module-over-a-principal-ideal-domain-is-flat)
    - [Flat extension preserves finite ideal intersections](module-theory.md#flat-extension-preserves-finite-ideal-intersections)
    - [Local tensor nonvanishing criterion](module-theory.md#local-tensor-nonvanishing-criterion)
  - [Determinant trick](module-theory.md#determinant-trick)
  - [Short exact sequence](module-theory.md#short-exact-sequence)
    - [Module extension](module-theory.md#module-extension)
      - [Extension of trivial modules for an infinite cyclic group](module-theory.md#extension-of-trivial-modules-for-an-infinite-cyclic-group)
      - [Pushout of a module extension](module-theory.md#pushout-of-a-module-extension)
      - [Equivalence of module extensions](module-theory.md#equivalence-of-module-extensions)
    - [Split short exact sequence](module-theory.md#split-short-exact-sequence)
    - [Short five lemma](module-theory.md#short-five-lemma)
  - [Inverse system](module-theory.md#inverse-system)
    - [Inverse limit](module-theory.md#inverse-limit)
      - [Universal property of an inverse limit](module-theory.md#universal-property-of-an-inverse-limit)
      - [Nonemptiness theorem for inverse limits of finite sets](module-theory.md#nonemptiness-theorem-for-inverse-limits-of-finite-sets)
  - [Filtration of a module](module-theory.md#filtration-of-a-module)
    - [Quotient filtration](module-theory.md#quotient-filtration)
    - [Subspace filtration](module-theory.md#subspace-filtration)
    - [Ascending filtration](module-theory.md#ascending-filtration)
    - [Good filtration of a module](module-theory.md#good-filtration-of-a-module)
      - [Dimension of a filtered module](module-theory.md#dimension-of-a-filtered-module)
        - [Multiplicity of a filtered module](module-theory.md#multiplicity-of-a-filtered-module)
          - [Dimension and multiplicity in a filtered exact sequence](module-theory.md#dimension-and-multiplicity-in-a-filtered-exact-sequence)
    - [Equivalent filtrations of a module](module-theory.md#equivalent-filtrations-of-a-module)
    - [I-adic topology](module-theory.md#i-adic-topology)
      - [I-adic filtration](module-theory.md#i-adic-filtration)
        - [Krull intersection theorem](module-theory.md#krull-intersection-theorem)
        - [x-adic filtration](module-theory.md#x-adic-filtration)
        - [Stable I-filtration](module-theory.md#stable-i-filtration)
        - [Rees algebra](module-theory.md#rees-algebra)
          - [Rees module](module-theory.md#rees-module)
        - [Artin-Rees lemma](module-theory.md#artin-rees-lemma)
    - [Filtered algebra](module-theory.md#filtered-algebra)
      - [Rees ring of a filtered algebra](module-theory.md#rees-ring-of-a-filtered-algebra)
      - [Almost commutative algebra](module-theory.md#almost-commutative-algebra)
        - [Degree-one almost commutative algebra](module-theory.md#degree-one-almost-commutative-algebra)
      - [Filtered ring](module-theory.md#filtered-ring)
        - [Filtration of a ring](module-theory.md#filtration-of-a-ring)
          - [Complete negative filtration](module-theory.md#complete-negative-filtration)
            - [Complete negative filtered-graded transfer of Noetherianity](module-theory.md#complete-negative-filtered-graded-transfer-of-noetherianity)
        - [Ascending filtered-graded transfer of Noetherianity](module-theory.md#ascending-filtered-graded-transfer-of-noetherianity)
        - [Filtered-graded transfer for complete rings](module-theory.md#filtered-graded-transfer-for-complete-rings)
  - [Length of a module](module-theory.md#length-of-a-module)
  - [Primary decomposition theorem for finitely generated modules over a principal ideal domain](module-theory.md#primary-decomposition-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)
  - [Module (mathematics)](module-theory.md#module-mathematics)
    - [Finitely presented module](module-theory.md#finitely-presented-module)
      - [Fitting ideal](module-theory.md#fitting-ideal)
    - [Locally free module](module-theory.md#locally-free-module)
    - [Finite presentation of a module](module-theory.md#finite-presentation-of-a-module)
    - [Change of rings](module-theory.md#change-of-rings)
      - [Coextension of scalars](module-theory.md#coextension-of-scalars)
      - [Extension of scalars](module-theory.md#extension-of-scalars)
      - [Restriction of scalars](module-theory.md#restriction-of-scalars)
    - [Module isomorphism](module-theory.md#module-isomorphism)
    - [Torsion module](module-theory.md#torsion-module)
      - [Torsion submodule](module-theory.md#torsion-submodule)
        - [Torsion element of a module](module-theory.md#torsion-element-of-a-module)
    - [Module homomorphism](module-theory.md#module-homomorphism)
      - [Module endomorphism](module-theory.md#module-endomorphism)
        - [Module automorphism](module-theory.md#module-automorphism)
      - [Module retraction](module-theory.md#module-retraction)
      - [Endomorphism ring](module-theory.md#endomorphism-ring)
        - [Local endomorphism ring](module-theory.md#local-endomorphism-ring)
        - [Semisimple quotient of a module endomorphism algebra](module-theory.md#semisimple-quotient-of-a-module-endomorphism-algebra)
        - [Brick module](module-theory.md#brick-module)
          - [Ringel lemma on bricks](module-theory.md#ringel-lemma-on-bricks)
            - [Proof of Ringel lemma on bricks](module-theory.md#proof-of-ringel-lemma-on-bricks)
    - [Submodule](module-theory.md#submodule)
      - [Essential submodule](module-theory.md#essential-submodule)
        - [Essential right ideal](module-theory.md#essential-right-ideal)
          - [A regular principal right ideal in a right Noetherian ring is essential](module-theory.md#a-regular-principal-right-ideal-in-a-right-noetherian-ring-is-essential)
        - [Essential extension](module-theory.md#essential-extension)
      - [Primary decomposition](module-theory.md#primary-decomposition)
        - [Lasker–Noether theorem](module-theory.md#lasker-noether-theorem)
        - [Primary submodule](module-theory.md#primary-submodule)
  - [Quotient module](module-theory.md#quotient-module)
    - [Universal property of a quotient module](module-theory.md#universal-property-of-a-quotient-module)
  - [Free module](module-theory.md#free-module)
    - [Vector-space freeness from maximal independence](module-theory.md#vector-space-freeness-from-maximal-independence)
    - [Linear independence in a module](module-theory.md#linear-independence-in-a-module)
    - [Finite free module](module-theory.md#finite-free-module)
    - [Basis of a module](module-theory.md#basis-of-a-module)
    - [Universal property of a free module](module-theory.md#universal-property-of-a-free-module)
    - [Rank of a free module](module-theory.md#rank-of-a-free-module)
      - [Rank inequality for an injection of finite free modules](module-theory.md#rank-inequality-for-an-injection-of-finite-free-modules)
    - [Invariant basis number](module-theory.md#invariant-basis-number)
      - [Invariant basis number for a commutative ring](module-theory.md#invariant-basis-number-for-a-commutative-ring)
  - [Torsion-free module](module-theory.md#torsion-free-module)
    - [Embedding a finitely generated torsion-free module in a finite free module](module-theory.md#embedding-a-finitely-generated-torsion-free-module-in-a-finite-free-module)
    - [Maximal torsion-free quotient](module-theory.md#maximal-torsion-free-quotient)
    - [Reflexive module](module-theory.md#reflexive-module)
      - [Reflexive-module second-syzygy criterion](module-theory.md#reflexive-module-second-syzygy-criterion)
  - [Projective module](module-theory.md#projective-module)
    - [Projective modules are flat](module-theory.md#projective-modules-are-flat)
    - [Projective modules are direct summands of free modules](module-theory.md#projective-modules-are-direct-summands-of-free-modules)
    - [Principal indecomposable module](module-theory.md#principal-indecomposable-module)
    - [Finite projective module](module-theory.md#finite-projective-module)
    - [Invertible module](module-theory.md#invertible-module)
      - [Base change of invertible modules](module-theory.md#base-change-of-invertible-modules)
    - [Projective dimension](module-theory.md#projective-dimension)
      - [Top Ext detects finite projective dimension](module-theory.md#top-ext-detects-finite-projective-dimension)
        - [Top Ext detects finite projective dimension over a left Noetherian ring](module-theory.md#top-ext-detects-finite-projective-dimension-over-a-left-noetherian-ring)
        - [Vanishing top Ext without finite generation](module-theory.md#vanishing-top-ext-without-finite-generation)
      - [Global dimension](module-theory.md#global-dimension)
        - [Global dimension zero and split exact sequences](module-theory.md#global-dimension-zero-and-split-exact-sequences)
    - [Free modules are projective](module-theory.md#free-modules-are-projective)
    - [Projective cover](module-theory.md#projective-cover)
      - [Head of a module](module-theory.md#head-of-a-module)
  - [Cyclic module](module-theory.md#cyclic-module)
  - [Uniserial module](module-theory.md#uniserial-module)
  - [Semisimple module](module-theory.md#semisimple-module)
    - [Isotypic decomposition](module-theory.md#isotypic-decomposition)
      - [Isotypic component](module-theory.md#isotypic-component)
  - [Radical of a module](module-theory.md#radical-of-a-module)
    - [Radical series of a module](module-theory.md#radical-series-of-a-module)
  - [Socle (mathematics)](module-theory.md#socle-mathematics)
    - [Socle series of a module](module-theory.md#socle-series-of-a-module)
  - [Loewy length](module-theory.md#loewy-length)
    - [Radical and socle series of a direct sum](module-theory.md#radical-and-socle-series-of-a-direct-sum)
  - [Irreducible module](module-theory.md#irreducible-module)
    - [Simple modules over an algebra finite over its center](module-theory.md#simple-modules-over-an-algebra-finite-over-its-center)
    - [Simple module over a commutative ring](module-theory.md#simple-module-over-a-commutative-ring)
  - [Annihilator (ring theory)](module-theory.md#annihilator-ring-theory)
    - [Right annihilator](module-theory.md#right-annihilator)
    - [Associated prime of a module](module-theory.md#associated-prime-of-a-module)
      - [Localization of associated primes](module-theory.md#localization-of-associated-primes)
      - [Embedded associated prime](module-theory.md#embedded-associated-prime)
      - [Minimal primes are associated primes](module-theory.md#minimal-primes-are-associated-primes)
    - [Annihilator of a module](module-theory.md#annihilator-of-a-module)
      - [Maximal annihilator of a module element is prime](module-theory.md#maximal-annihilator-of-a-module-element-is-prime)
  - [Structure theorem for finitely generated modules over a principal ideal domain](module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)
    - [Invariant factor of a finitely generated module](module-theory.md#invariant-factor-of-a-finitely-generated-module)
    - [Finitely generated torsion-free module over a principal ideal domain](module-theory.md#finitely-generated-torsion-free-module-over-a-principal-ideal-domain)
      - [Classification of integral matrices satisfying the third cyclotomic polynomial](module-theory.md#classification-of-integral-matrices-satisfying-the-third-cyclotomic-polynomial)
    - [Elementary divisor](module-theory.md#elementary-divisor)
    - [Indecomposable finite abelian groups](module-theory.md#indecomposable-finite-abelian-groups)
- [Prime ideal](#prime-ideal)
  - [Minimal prime ideal](#minimal-prime-ideal)
    - [Minimal prime over an ideal](#minimal-prime-over-an-ideal)
    - [Existence of minimal primes over a proper ideal](#existence-of-minimal-primes-over-a-proper-ideal)
    - [Unique minimal prime does not imply primary](#unique-minimal-prime-does-not-imply-primary)
  - [Prime ideal avoiding a multiplicative subset](#prime-ideal-avoiding-a-multiplicative-subset)
  - [Symbolic power](#symbolic-power)
  - [Prime ideal quotient criterion](#prime-ideal-quotient-criterion)
- [Boolean ring](#boolean-ring)
  - [Prime ideals of a Boolean ring are maximal](#prime-ideals-of-a-boolean-ring-are-maximal)
- [Coefficientwise quotient of a polynomial ring](#coefficientwise-quotient-of-a-polynomial-ring)
- [Irreducible real polynomial](#irreducible-real-polynomial)
- [Kummer irreducibility criterion](#kummer-irreducibility-criterion)

## Norm for a finite free ring extension

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

If $B$ is a commutative $A$-algebra which is a [finite free module](module-theory.md#finite-free-module) over $A$, its norm sends $b$ to the [determinant](linear-algebra.md#determinant) of multiplication $m_b:B\to B$. The [determinant](linear-algebra.md#determinant) is independent of the chosen [basis](vector-space.md#basis) and is multiplicative because $m_{bc}=m_bm_c$. It commutes with scalar extension. On a separable [field](algebra.md#field) extension it becomes the product over embeddings, recovering the [field norm](algebraic-number-theory.md#field-norm). An invertible $b$ has invertible norm.

## Finite-type integer algebra

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

A unital commutative [ring](#ring) generated by finitely many elements under addition and multiplication, starting from the image of the integers. Equivalently it is a quotient of a finite-variable [polynomial ring](#polynomial-ring) over $\mathbb Z$. [localization of a ring](#localization-of-a-ring) at one element remains finite type, since $R[1/r]\cong R[T]/(rT-1)$. Generation here is as an algebra, not merely as a [field extension](algebra.md#field-extension) when the [ring](#ring) happens to be a [field](algebra.md#field).

### Finite-field theorem for finitely generated integer algebras

↑ **Parent:** [Finite-type integer algebra](#finite-type-integer-algebra)

A [field](algebra.md#field) that is a [finite-type integer algebra](#finite-type-integer-algebra) has prime characteristic or zero. Prime characteristic and [Zariski lemma](algebraic-geometry.md#zariski-s-lemma) make it a finite algebraic extension of a finite prime [field](algebra.md#field). In characteristic zero, the same lemma makes it a number [field](algebra.md#field); clearing finitely many coefficient denominators makes it integral over $\mathbb Z[1/N]$. The [integral field extension forces the base domain to be a field](#integral-field-extension-forces-the-base-domain-to-be-a-field), but a prime not dividing $N$ is not invertible there. This contradiction excludes characteristic zero.

## Algebraic differential operator ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

For a [commutative algebra](commutative-algebra.md) $R$ over $k$, put $D_k^{-1}(R)=0$ and define $D_k^j(R)$ to be the $k$-linear [endomorphisms](algebra.md#endomorphism) $\theta$ with $[\theta,m_a]\in D_k^{j-1}(R)$ for every multiplication map $m_a$. The union is a ring under composition, with $D_k^0(R)=R$ and $D_k^rD_k^s\subseteq D_k^{r+s}$. This commutator definition applies to singular rings and [fields](algebra.md#field) of arbitrary characteristic, unlike a definition restricted to polynomial coefficients and partial derivatives.

### Order of an algebraic differential operator

↑ **Parent:** [Algebraic differential operator ring](#algebraic-differential-operator-ring)

The least index in the commutator filtration of the [algebraic differential operator ring](#algebraic-differential-operator-ring) containing a nonzero operator. The zero operator has order $-\infty$ by convention. Equivalently every $(j+1)$-fold iterated commutator with multiplication maps vanishes for an operator of order at most $j$.

#### First-order algebraic differential operator decomposition

↑ **Parent:** [Order of an algebraic differential operator](#order-of-an-algebraic-differential-operator)

If $\theta$ has order at most one, set $c=\theta(1)$ and $\delta=\theta-m_c$. Then $\delta(1)=0$ and $[\delta,m_a]=m_{\delta(a)}$, which is the [Leibniz rule](calculus.md#leibniz-rule). Thus $\delta$ is a [derivation of an algebra](associative-algebra.md#derivation-of-an-algebra). Conversely any derivation satisfies this commutator identity. The sum is direct because a derivation that is multiplication must vanish at $1$.

## Algebra over a commutative ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

An algebra over a [commutative ring](#commutative-ring) $R$ is a [ring](#ring) $A$ with a specified unital [ring homomorphism](#ring-homomorphism) $R\to A$ whose image commutes with every element of $A$. Scalar multiplication is $r\cdot a=\varphi(r)a$. For commutative $A$, the commutation requirement is automatic.

### Bialgebra

↑ **Parent:** [Algebra over a commutative ring](#algebra-over-a-commutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bialgebra)

An [algebra over a commutative ring](#algebra-over-a-commutative-ring) that is also a [coalgebra](linear-algebra.md#coalgebra), whose [comultiplication](category-theory.md#comultiplication) and [counit](category-theory.md#counit) preserve the multiplication and unit. Equivalently it is a [bimonoid](category-theory.md#bimonoid) in $k$-modules.

#### Cobraided bialgebra

↑ **Parent:** [Bialgebra](#bialgebra)

A [bialgebra](#bialgebra) equipped with a [coquasitriangular structure](category-theory.md#coquasitriangular-structure), namely a convolution-invertible scalar form $r:H\otimes H\to k$ satisfying $r(ab,c)=\sum r(a,c_{(1)})r(b,c_{(2)})$, $r(a,bc)=\sum r(a_{(1)},c)r(a_{(2)},b)$ and $\sum r(a_{(1)},b_{(1)})a_{(2)}b_{(2)}=\sum b_{(1)}a_{(1)}r(a_{(2)},b_{(2)})$, with unit normalization. The induced right-[comodule](linear-algebra.md#comodule) [braiding](category-theory.md#braiding) is $v\otimes w\mapsto\sum w_{(0)}\otimes v_{(0)}r(v_{(1)},w_{(1)})$.

#### Bialgebra scalar cocycle

↑ **Parent:** [Bialgebra](#bialgebra)

A normalized scalar map $\gamma:H\otimes H\to k$ satisfying $\sum\gamma(a_{(1)},b_{(1)})\gamma(a_{(2)}b_{(2)},c)=\sum\gamma(b_{(1)},c_{(1)})\gamma(a,b_{(2)}c_{(2)})$, and $\gamma(1,a)=\varepsilon(a)=\gamma(a,1)$. Some conventions require convolution invertibility; that extra hypothesis distinguishes strong from lax tensor transformations.

##### Bialgebra cocycle twist

↑ **Parent:** [Bialgebra scalar cocycle](#bialgebra-scalar-cocycle)

With the convention $m*\gamma=\gamma*n$ and invertible [bialgebra scalar cocycle](#bialgebra-scalar-cocycle) $\gamma$ for $n$, the same [coalgebra](linear-algebra.md#coalgebra) has $n=\bar\gamma*m*\gamma$, or equivalently $m=\gamma*n*\bar\gamma$. Thus $n(a,b)=\sum\bar\gamma(a_{(1)},b_{(1)})m(a_{(2)},b_{(2)})\gamma(a_{(3)},b_{(3)})$. Specifying the equation prevents opposite twist conventions from being conflated.

#### Diagonal bialgebra action

↑ **Parent:** [Bialgebra](#bialgebra)

The tensor of left [modules](module-theory.md#module-mathematics) over a [bialgebra](#bialgebra) has action $h(u\otimes v)=\sum(h_{(1)}u)\otimes(h_{(2)}v)$. The unit module $k$ has action through the [counit](category-theory.md#counit).

## Ring extension

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ring_extension)

A ring extension $A\subseteq B$ is an inclusion of rings that makes $B$ an $A$-algebra.

### Module-finite ring extension

↑ **Parent:** [Ring extension](#ring-extension)

A ring extension $A\subseteq B$ is module-finite, or finite, when $B$ is a finitely generated $A$-module. Every module-finite extension is integral.

### Fiber ring

↑ **Parent:** [Ring extension](#ring-extension)

For a ring homomorphism $A\to B$ and a prime $\mathfrak p\subset A$, the fiber ring at $\mathfrak p$ is

$$
B\otimes_A\kappa(\mathfrak p).
$$

Its prime ideals correspond to the primes of $B$ whose contraction is $\mathfrak p$.

#### Fiber of the map on spectra

↑ **Parent:** [Fiber ring](#fiber-ring)

The fiber over $\mathfrak p\in\operatorname{Spec}A$ of $\operatorname{Spec}B\to\operatorname{Spec}A$ is the set of primes $\mathfrak q\subset B$ satisfying $\mathfrak q\cap A=\mathfrak p$. It is naturally the spectrum of the fiber ring $B\otimes_A\kappa(\mathfrak p)$.

## Localization of a ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

For a multiplicatively closed set $S$, the localization $S^{-1}R$ formally makes every element of $S$ invertible. Elements are represented by fractions $r/s$.

### Total ring of fractions

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_ring_of_fractions)

Here $S$ consists of the [non-zero-divisors](mathematics.md#non-zero-divisor) of a [commutative ring](#commutative-ring) $A$. The [localization](#localization-of-a-ring) map $A\to Q(A)$ is [injective](algebra.md#injective-function): a fraction $a/1$ is zero only if some $s\in S$ annihilates $a$. For a [reduced ring](#reduced-ring) with finitely many [minimal prime ideals](#minimal-prime-ideal), its [zero divisors](mathematics.md#zero-divisor) form the union of these primes. Indeed, if $ab=0$ and $a$ avoids every minimal prime, reduction to each domain quotient forces $b$ into their intersection, which is zero. Conversely, for $a$ in a minimal prime $\mathfrak p_i$, choose $b$ in every other minimal prime but outside $\mathfrak p_i$, using their incomparability and multiplying suitable elements. Then $b\ne0$ and $ab=0$.

### Localization commutes with tensor products

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

For a multiplicatively closed set $T$ in a commutative ring $A$, the map sends $(m\otimes n)/t$ to $(m/t)\otimes(n/1)$. An inverse sends $(m/s)\otimes(n/t)$ to $(m\otimes n)/(st)$. The fraction relations and the [tensor product of modules](module-theory.md#tensor-product-of-modules) balancing relation make these maps well-defined and mutually inverse.

### Localization detects zero elements

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

An element $a$ of a [commutative ring](#commutative-ring) $R$ is zero if and only if its image in every [localization at a prime ideal](#localization-at-a-prime-ideal) is zero. If $a\ne0$, its proper [annihilator](module-theory.md#annihilator-ring-theory) lies in a [maximal ideal](#maximal-ideal) $\mathfrak m$. No element outside $\mathfrak m$ can annihilate $a$, so $a/1\ne0$ in $R_{\mathfrak m}$. This also applies to elements of an $R$-[module](module-theory.md#module-mathematics) using [localization of a module](#localization-of-a-module).

### Multiplicatively closed set

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplicatively_closed_set)

A multiplicative subset $S$ of a ring contains $1$ and is closed under multiplication. It may contain zero, in which case its localization is the zero ring.

#### Saturated multiplicative subset

↑ **Parent:** [Multiplicatively closed set](#multiplicatively-closed-set)

A [multiplicative subset](#multiplicatively-closed-set) is saturated if every factor of a product in the subset also lies in it. We include $1$ in a [multiplicative subset](#multiplicatively-closed-set). A saturated subset containing $0$ is the whole ring. The units form a saturated subset in a [commutative ring](#commutative-ring).

##### Units with no finite prime-union complement

↑ **Parent:** [Saturated multiplicative subset](#saturated-multiplicative-subset)

In $\mathbb Z$, the [saturated multiplicative subset](#saturated-multiplicative-subset) $\{-1,1\}$ has complement equal to the union of $(p)$ over all positive primes. No finite subcollection of [prime ideals](#prime-ideal) covers this complement: a prime outside the finite list is a nonunit not in any listed [ideal](#ideal).

##### Saturated complement as a union of prime ideals

↑ **Parent:** [Saturated multiplicative subset](#saturated-multiplicative-subset)

The complement of a [multiplicative subset](#multiplicatively-closed-set) is a union of [prime ideals](#prime-ideal) exactly when the subset is saturated. If $a\notin S$, saturation ensures $(a)\cap S=\varnothing$; extend this to a [prime ideal avoiding a multiplicative subset](#prime-ideal-avoiding-a-multiplicative-subset). Conversely, a product in $S$ cannot have a factor in a [prime ideal](#prime-ideal) contained in the complement.

### Universal property of localization

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

The localization map $\iota:R\to S^{-1}R$ sends every element of $S$ to a unit. If a ring homomorphism $f:R\to T$ also sends every element of $S$ to a unit, there is a unique homomorphism $\widetilde f:S^{-1}R\to T$ with $\widetilde f(r/s)=f(r)f(s)^{-1}$ and $\widetilde f\iota=f$.

#### Localization away from one plus an ideal lies in the Jacobson radical

↑ **Parent:** [Universal property of localization](#universal-property-of-localization)

For a [commutative ring](#commutative-ring) $R$ and [ideal](#ideal) $I$, the set $S=1+I$ is a [multiplicative subset](#multiplicatively-closed-set). For $i\in I$ and $s,t\in S$, the numerator $st-ri$ of $1-(r/t)(i/s)$ again lies in $S$. Thus this difference is a [unit](algebra.md#unit-in-a-ring) in the [localization of a ring](#localization-of-a-ring). The [unit criterion for the Jacobson radical](noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) proves $S^{-1}I\subseteq J(S^{-1}R)$. This requires no [Noetherian](algebra.md#noetherian-ring) hypothesis.

### Localization of a module

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

For a [multiplicative subset](#multiplicatively-closed-set) $S\subseteq R$ and an $R$-module $M$, the localization $S^{-1}M$ consists of fractions $m/s$, with $m/s=m'/s'$ when some $u\in S$ satisfies $u(s'm-sm')=0$. It is an $S^{-1}R$-module, and the canonical map is $m\mapsto m/1$. If $M$ is finitely generated over a [Noetherian ring](algebra.md#noetherian-ring), then $S^{-1}M$ is a [Noetherian module](algebra.md#noetherian-module) over $S^{-1}R$.

#### Vanishing criterion in a module localization

↑ **Parent:** [Localization of a module](#localization-of-a-module)

The fraction relation defining [localization of a module](#localization-of-a-module) gives this criterion. For localization at powers of a single element $f$, a fraction vanishes exactly when some power of $f$ annihilates its numerator. Finitely many such vanishing relations can be cleared with one common exponent. This is distinct from detecting global zero by localizing at every prime ideal.

#### Exactness of localization

↑ **Parent:** [Localization of a module](#localization-of-a-module)

For a [multiplicative subset](#multiplicatively-closed-set) $S$ of a [commutative ring](#commutative-ring) $A$, localization preserves [short exact sequences](module-theory.md#short-exact-sequence) of $A$-modules. Surjectivity follows by lifting a numerator. If a fraction maps to zero, some element of $S$ annihilates its image, so multiplying its numerator by that element puts it into the original kernel. For an injective original map, the same criterion shows its localized kernel is zero. Thus $S^{-1}A$ is a [flat module](module-theory.md#flat-module) over $A$.

##### Injectivity of a module map is detected at maximal localizations

↑ **Parent:** [Exactness of localization](#exactness-of-localization)

For a [module homomorphism](module-theory.md#module-homomorphism) $f:M\to N$ over a [commutative ring](#commutative-ring) $A$, $f$ is [injective](algebra.md#injective-function) if and only if every $f_{\mathfrak m}$ is [injective](algebra.md#injective-function), with $\mathfrak m$ ranging over [maximal ideals](#maximal-ideal). In a [localization of a module](#localization-of-a-module), $x/s$ maps to zero exactly when some denominator $t$ satisfies $tf(x)=0$. If $f$ is [injective](algebra.md#injective-function) this gives $tx=0$, so the original fraction is zero. In general it identifies $\ker(f_{\mathfrak m})$ with $(\ker f)_{\mathfrak m}$. A nonzero element of $\ker f$ has a proper [annihilator](module-theory.md#annihilator-ring-theory), contained in some [maximal ideal](#maximal-ideal); it remains nonzero in that [localization](#localization-of-a-ring). Thus vanishing of all localized kernels forces $\ker f=0$. No finiteness or [Noetherian](algebra.md#noetherian-ring) assumption is required.

#### Kernel of localization away from one plus an ideal

↑ **Parent:** [Localization of a module](#localization-of-a-module)

Let $R$ be [Noetherian](algebra.md#noetherian-ring), $I\subseteq R$ an ideal, $S=1+I$, and $M$ a finitely generated $R$-module. Then

$$
\ker(M\longrightarrow S^{-1}M)=\bigcap_{j\geq1}I^jM.
$$

If $(1+a)m=0$ with $a\in I$, then $m=(-a)^jm\in I^jM$ for every $j$. Conversely, apply the [Artin-Rees lemma](module-theory.md#artin-rees-lemma) to $Rm\subseteq M$. For sufficiently large $c$ it gives

$$
m\in I^{c+1}M\cap Rm=I(I^cM\cap Rm)\subseteq I(Rm),
$$

so $m=am$ for some $a\in I$ and $(1-a)m=0$.

##### Non-Noetherian failure of the intersection formula for localization

↑ **Parent:** [Kernel of localization away from one plus an ideal](#kernel-of-localization-away-from-one-plus-an-ideal)

Let

$$
R=k[t^q:q\in\mathbb Q_{\geq0}]
$$

be the semigroup algebra inside $k[t^{\mathbb Q}]$, and let $I$ be generated by the $t^q$ with $q>0$. This [integral domain](#integral-domain) is not Noetherian, since

$$
(t)\subsetneq(t^{1/2})\subsetneq(t^{1/4})\subsetneq\cdots.
$$

Moreover $I^2=I$, because $t^q=(t^{q/2})^2$. Thus $\bigcap_{j\geq1}I^j=I\ne0$, whereas the map $R\to(1+I)^{-1}R$ is injective because $R$ is a domain.

### Integer localization at a set of primes

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

For a set $\pi$ of [prime numbers](number-theory.md#prime-number), the integer localization

$$
A_\pi=\mathbb Z[q^{-1}:q\in\pi]\subseteq\mathbb Q
$$

consists of fractions whose denominator has prime factors only in $\pi$. As an additive group it is divisible by every prime in $\pi$.

#### Finite quotients of the integers localized away from one prime

↑ **Parent:** [Integer localization at a set of primes](#integer-localization-at-a-set-of-primes)

If $A_{\neg p}=\mathbb Z[q^{-1}:q\ne p]$, its finite quotients are exactly the cyclic $p$-groups $\mathbb Z/p^n\mathbb Z$. Divisibility by every $q\ne p$ excludes other prime torsion, while a quotient of exponent $p^n$ factors through $A_{\neg p}/p^nA_{\neg p}\cong\mathbb Z/p^n\mathbb Z$.

### Prime ideal correspondence for localization

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

Extension and contraction give inverse inclusion-preserving bijections between prime ideals of $S^{-1}R$ and prime ideals of $R$ disjoint from $S$:

$$
\mathfrak p\longmapsto S^{-1}\mathfrak p,
\qquad
\mathfrak q\longmapsto\iota^{-1}(\mathfrak q).
$$

#### Spectrum of localization away from one plus an ideal

↑ **Parent:** [Prime ideal correspondence for localization](#prime-ideal-correspondence-for-localization)

For $S=1+I$, the [prime ideal correspondence for localization](#prime-ideal-correspondence-for-localization) identifies $\operatorname{Spec}S^{-1}R$ with

$$
\{\mathfrak p\in\operatorname{Spec}R:\mathfrak p+I\ne R\}.
$$

Indeed, $\mathfrak p\cap(1+I)=\varnothing$ exactly when no element of $I$ is congruent to $-1$ modulo $\mathfrak p$, which is exactly $\mathfrak p+I\ne R$.

### Localization of a Noetherian ring

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

Every localization of a Noetherian ring is Noetherian. Each ideal $J\subseteq S^{-1}R$ is the extension of its contraction to $R$, whose finite generating set consequently generates $J$.

#### Localization of a Dedekind domain

↑ **Parent:** [Localization of a Noetherian ring](#localization-of-a-noetherian-ring)

If $R$ is a Dedekind domain and $0\notin S$, then $S^{-1}R$ is an integrally closed Noetherian domain of dimension at most one. It is therefore either a Dedekind domain or, when its dimension is zero, a field.

### Localization at a prime ideal

↑ **Parent:** [Localization of a ring](#localization-of-a-ring)

Localization at a prime ideal $\mathfrak p$ means inverting $R\setminus\mathfrak p$. The resulting local ring $R_{\mathfrak p}$ has maximal ideal $\mathfrak pR_{\mathfrak p}$.

#### Domain prime localizations do not imply a domain

↑ **Parent:** [Localization at a prime ideal](#localization-at-a-prime-ideal)

The [ring](#ring) $k\times k$, for a [field](algebra.md#field) $k$, has two [prime ideals](#prime-ideal), $0\times k$ and $k\times0$. Their [localizations at a prime ideal](#localization-at-a-prime-ideal) are both isomorphic to $k$. Nevertheless $(1,0)(0,1)=0$ is a product of nonzero elements, so $A$ is not an [integral domain](#integral-domain). Nonzero orthogonal [idempotents](#idempotent) separate the two components of its [spectrum of a commutative ring](ringed-space.md#spectrum-of-a-commutative-ring).

## Integral element

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_element)

An element $a$ of an $R$-algebra is integral over $R$ when it satisfies a monic polynomial with coefficients in $R$.

### Finite-module criterion for integrality

↑ **Parent:** [Integral element](#integral-element)

An element $x$ of an $A$-algebra is an [integral element](#integral-element) precisely when $A[x]$ is a finite $A$-[module](module-theory.md#module-mathematics). More generally, a finite $A$-submodule containing one and stable under multiplication by $x$ proves integrality by the [determinant trick](module-theory.md#determinant-trick). Conversely a [monic polynomial](polynomial.md#monic-polynomial) equation reduces all powers of $x$ to finitely many generators.

### Integral extension

↑ **Parent:** [Integral element](#integral-element)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_extension)

An extension $R\subseteq A$ is integral when every element of $A$ is integral over $R$.

#### Integral field extension forces the base domain to be a field

↑ **Parent:** [Integral extension](#integral-extension)

If a [field](algebra.md#field) $L$ is integral over a subdomain $A$, every nonzero $a\in A$ has an inverse in $L$ satisfying a monic equation over $A$. Multiplying that equation by $a^{r-1}$ expresses $a^{-1}$ as a polynomial in $a$ with coefficients in $A$. Hence $a^{-1}\in A$, and $A$ is itself a [field](algebra.md#field). The embedding and integrality assumptions are essential; a [fraction field](#field-of-fractions) is not generally integral over its source domain.

#### Localization of an integral extension at a prime need not be integral

↑ **Parent:** [Integral extension](#integral-extension)

An [integral extension](#integral-extension) $A\subset B$ need not give an [integral extension](#integral-extension) $A_{P\cap A}\subset B_P$. For example, take $\mathbb Z\subset\mathbb Z[i]$ and $P=(2+i)$, whose contraction is $(5)$. The element $1/(2-i)$ belongs to $\mathbb Z[i]_P$ but is not integral over $\mathbb Z_{(5)}$: multiplying a hypothetical monic equation by a power of $2-i$ and reducing modulo the other Gaussian [prime ideal](#prime-ideal) $(2-i)$ gives $1=0$ in $\mathbb F_5$. Localizing both rings by the same [multiplicative subset](#multiplicatively-closed-set) does preserve integrality.

#### Integral extensions preserve Krull dimension

↑ **Parent:** [Integral extension](#integral-extension)

If $A\subseteq B$ is an [integral extension](#integral-extension), then $\dim A=\dim B$. The [incomparability theorem for integral extensions](#incomparability-theorem-for-integral-extensions) contracts every strict prime chain in $B$ to a strict chain in $A$, giving $\dim B\leq\dim A$. Conversely, the [Lying-over theorem](#lying-over-theorem) starts over the bottom of any prime chain in $A$, and repeated use of the [going-up theorem](#going-up-theorem) lifts the whole chain to $B$.

##### Krull dimension of rings of algebraic integers

↑ **Parent:** [Integral extensions preserve Krull dimension](#integral-extensions-preserve-krull-dimension)

For any algebraic field extension $K/\mathbb Q$, including an infinite one, its ring $\mathcal O_K$ of elements integral over $\mathbb Z$ is an [integral extension](#integral-extension) of $\mathbb Z$. The [Lying-over theorem](#lying-over-theorem), [going-up theorem](#going-up-theorem) and [incomparability theorem for integral extensions](#incomparability-theorem-for-integral-extensions) give $\dim\mathcal O_K=\dim\mathbb Z=1$. The argument does not require that $\mathcal O_K$ be Noetherian or finitely generated over $\mathbb Z$.

##### Dimension of a monic plane hypersurface

↑ **Parent:** [Integral extensions preserve Krull dimension](#integral-extensions-preserve-krull-dimension)

If $f\in k[Y][X]$ is monic of positive degree in $X$, monic division makes $k[Y][X]/(f)$ free of rank $\deg_Xf$ over $k[Y]$. The inclusion of $k[Y]$ is injective and the quotient is an [integral extension](#integral-extension), so its [Krull dimension](#krull-dimension) is one. This argument applies even when the polynomial factors or the [field](algebra.md#field) has positive characteristic.

#### Lying-over theorem

↑ **Parent:** [Integral extension](#integral-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lying-over_theorem)

If $A\subseteq B$ is an [integral extension](#integral-extension), then every [prime ideal](#prime-ideal) $\mathfrak p$ of $A$ is the contraction of a prime ideal $\mathfrak q$ of $B$. Thus the contraction map $\operatorname{Spec}B\to\operatorname{Spec}A$ is surjective.

#### Going up and going down

↑ **Parent:** [Integral extension](#integral-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Going_up_and_going_down)

Going up and going down concern lifting inclusions of [prime ideals](#prime-ideal) through a [ring extension](#ring-extension). [Going-up theorem](#going-up-theorem) lifts upward from a chosen lower prime for an [integral extension](#integral-extension). [Going-down theorem](#going-down-theorem) lifts downward from a chosen upper prime under additional hypotheses, including an integrally closed base domain for integral extensions of domains.

##### Going-up theorem

↑ **Parent:** [Going up and going down](#going-up-and-going-down)

For an integral extension $A\subseteq B$, primes $\mathfrak p_1\subseteq\mathfrak p_2$ of $A$, and a prime $\mathfrak q_1$ of $B$ over $\mathfrak p_1$, there is a prime $\mathfrak q_2\supseteq\mathfrak q_1$ over $\mathfrak p_2$.

##### Going-down theorem

↑ **Parent:** [Going up and going down](#going-up-and-going-down)

Let $R\subseteq A$ be an integral extension of domains with $R$ integrally closed. Given primes $\mathfrak p_0\subseteq\mathfrak p_1$ of $R$ and a prime $\mathfrak q_1$ of $A$ over $\mathfrak p_1$, there is a prime $\mathfrak q_0\subseteq\mathfrak q_1$ over $\mathfrak p_0$.

#### Incomparability theorem for integral extensions

↑ **Parent:** [Integral extension](#integral-extension)

If $A\subseteq B$ is integral and $\mathfrak q_1\subseteq\mathfrak q_2$ are primes of $B$ with equal contractions to $A$, then $\mathfrak q_1=\mathfrak q_2$. Consequently strict prime chains remain strict under contraction.

#### Ideal contraction rigidity under an integral extension

↑ **Parent:** [Integral extension](#integral-extension)

Let $A\subseteq B$ be integral and let $I\subseteq J$ be ideals of $B$. If $I$ is prime and $I\cap A=J\cap A$, then $I=J$. After quotienting by $I$, a nonzero element of $J/I$ has an integral equation of least degree whose nonzero constant term lies in $(J/I)\cap(A/(I\cap A))$, a contradiction.

#### Contraction of a maximal ideal under an integral extension

↑ **Parent:** [Integral extension](#integral-extension)

If $A\subseteq B$ is integral and $\mathfrak n$ is a maximal ideal of $B$, then $\mathfrak n\cap A$ is maximal in $A$. Indeed, $B/\mathfrak n$ is an integral domain integral over $A/(\mathfrak n\cap A)$, and a subring over which a field is integral is itself a field.

#### Fiber primes of an integral extension

↑ **Parent:** [Integral extension](#integral-extension)

For an integral extension $A\subseteq B$ and $\mathfrak p\in\operatorname{Spec}A$, localization gives a bijection

$$
\{\mathfrak q\in\operatorname{Spec}B:\mathfrak q\cap A=\mathfrak p\}
\longleftrightarrow
\operatorname{MaxSpec}((A\setminus\mathfrak p)^{-1}B).
$$

It combines the [prime ideal correspondence for localization](#prime-ideal-correspondence-for-localization) with the [contraction of a maximal ideal under an integral extension](#contraction-of-a-maximal-ideal-under-an-integral-extension).

#### Subalgebra generated by finitely many integral elements

↑ **Parent:** [Integral extension](#integral-extension)

If $a_1,\ldots,a_n$ are integral over $R$, then $R[a_1,\ldots,a_n]$ is a finitely generated $R$-module. In particular, every element of this subalgebra is integral over $R$.

#### Integrally closed domain

↑ **Parent:** [Integral extension](#integral-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integrally_closed_domain)

An integral domain is integrally closed when every element of its fraction field that is integral over the domain already belongs to the domain.

#### Integral closure

↑ **Parent:** [Integral extension](#integral-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_closure)

The integral closure of $R$ in an $R$-algebra $A$ is the subring of elements of $A$ integral over $R$.

##### Finiteness of integral closure in a finite separable extension

↑ **Parent:** [Integral closure](#integral-closure)

For a normal [Noetherian ring](algebra.md#noetherian-ring) $A$ that is an [integral domain](#integral-domain), the [integral closure](#integral-closure) in a finite [separable field extension](galois-theory.md#separable-extension) of its [fraction field](#field-of-fractions) is finite as an $A$-[module](module-theory.md#module-mathematics). An [integral field basis by denominator clearing](#integral-field-basis-by-denominator-clearing) gives a finite lattice. Integral traces place the closure in its finite [trace-dual lattice](algebraic-number-theory.md#trace-dual-lattice); [Noetherianity](algebra.md#noetherian-ring) makes that submodule finitely generated.

##### Integral field basis by denominator clearing

↑ **Parent:** [Integral closure](#integral-closure)

If $A$ is an [integral domain](#integral-domain) with [fraction field](#field-of-fractions) $K$ and $L/K$ is finite, a $K$-basis of $L$ can be rescaled to consist of [integral elements](#integral-element) over $A$. For a monic algebraic equation, choose $a\in A$ clearing the coefficient denominators; replacing $u$ by $au$ multiplies the coefficient of degree $r-j$ by $a^j$, putting it in $A$.

##### Integral closure as an intersection of valuation rings

↑ **Parent:** [Integral closure](#integral-closure)

For a domain $R$ with [fraction field](#field-of-fractions) $K$, its [integral closure](#integral-closure) is the intersection of all [valuation rings](#valuation-ring) of $K$ containing $R$. Integral elements belong to every such [ring](#ring) because [valuation rings are integrally closed](#valuation-rings-are-integrally-closed). For a nonintegral $x$, the [ideal](#ideal) $x^{-1}R[x^{-1}]$ is proper, since its containing $1$ would give a monic equation for $x$. Localize at a [maximal ideal](#maximal-ideal) containing $x^{-1}$ and apply the [valuation domination lemma](#valuation-domination-lemma). The resulting [ring](#ring) contains $R$ but not $x$, proving the reverse inclusion.

##### Integral closure of a graded ring is graded

↑ **Parent:** [Integral closure](#integral-closure)

If a graded ring $A$ is a graded extension of a graded subring $R$, then the integral closure of $R$ in $A$ is graded: every homogeneous component of an integral element is integral. This follows by separating the extremal degrees in a monic integral equation and inducting on the number of nonzero homogeneous components.

## Krull dimension

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull_dimension)

The Krull dimension of a commutative ring is the supremum of the lengths of strict chains of prime ideals.

### Prime chain

↑ **Parent:** [Krull dimension](#krull-dimension)

A strictly increasing finite sequence of [prime ideals](#prime-ideal). Its length is the number of strict inclusions, so the displayed chain has length $s$. The [Krull dimension](#krull-dimension) of a ring is the supremum of such lengths; the [height of a prime ideal](#height-of-a-prime-ideal) restricts to chains ending at that prime.

### Noether normalization lemma

↑ **Parent:** [Krull dimension](#krull-dimension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noether_normalization_lemma)

If $A$ is a finitely generated algebra over a field $k$, then there are algebraically independent elements $y_1,\ldots,y_d\in A$ such that $A$ is finite, hence integral, over $k[y_1,\ldots,y_d]$.

#### Noether normalization by weighted substitutions

↑ **Parent:** [Noether normalization lemma](#noether-normalization-lemma)

To normalize $k[a_1,\ldots,a_n]$ over an arbitrary [field](algebra.md#field), choose a nonzero polynomial relation and a base $M$ larger than all its exponents. The substitutions $b_i=a_i-a_n^{M^i}$ give distinct top weights to its monomials, so its highest power of $a_n$ has a nonzero scalar coefficient. It becomes a [monic polynomial](polynomial.md#monic-polynomial) equation, making the algebra finite over $k[b_1,\ldots,b_{n-1}]$. Induction proves the [Noether normalization lemma](#noether-normalization-lemma), including over finite fields.

##### Finite flat Noether normalization of an affine hypersurface

↑ **Parent:** [Noether normalization by weighted substitutions](#noether-normalization-by-weighted-substitutions)

For a nonconstant polynomial over any [field](algebra.md#field), use triangular substitutions $x_i=y_i+y_n^{B^i}$, $x_n=y_n$, where $B$ exceeds every exponent in its support. Base-$B$ weights distinguish all original [monomials](polynomial.md#monomial), so the transformed polynomial has a unique highest $y_n$ power with coefficient in $k^\times$. Rescale to make it monic. The [monic polynomial quotient is finite free](polynomial.md#monic-polynomial-quotient-is-finite-free) over $k[y_1,\ldots,y_{n-1}]$, yielding a finite flat projection. The nonlinear substitution works over [finite fields](algebra.md#finite-field) as well as infinite ones; a generic linear-direction argument alone would not do so.

#### Noether normalization of the quadratic surface xy plus yz plus zx

↑ **Parent:** [Noether normalization lemma](#noether-normalization-lemma)

Let

$$
T=k[x,y,z]/(xy+yz+zx)
$$

over a field in which $3$ is invertible. Put $u=x-z$ and $v=y-z$. Then

$$
xy+yz+zx=uv+2(u+v)z+3z^2,
$$

so

$$
T\cong k[u,v][z]\big/\left(z^2+\frac23(u+v)z+\frac13uv\right).
$$

Division by this monic quadratic makes $T$ a free $k[u,v]$-module with basis $1,z$. Thus $k[u,v]$ is a polynomial algebra and $T$ is integral over it.

### Height of an ideal

↑ **Parent:** [Krull dimension](#krull-dimension)

Height measures prime-chain length within [Krull dimension](#krull-dimension) theory.

The height of an ideal $I$ is the infimum of the heights of prime ideals containing it:

$$
\operatorname{ht}(I)=\inf_{\mathfrak p\supseteq I}\operatorname{ht}(\mathfrak p).
$$

The height of a prime is the supremum of the lengths of strict prime chains ending at that prime.

#### Height of a prime ideal

↑ **Parent:** [Height of an ideal](#height-of-an-ideal)

The height of a [prime ideal](#prime-ideal) is the supremum of lengths of strict [prime chains](#prime-chain) ending at it, equivalently the [Krull dimension](#krull-dimension) of its [localization at a prime ideal](#localization-at-a-prime-ideal). The [Krull height theorem](#krull-height-theorem) bounds the height of a minimal prime over an $n$-generated [ideal](#ideal) by $n$.

##### Polynomial-ring height and dimension formula

↑ **Parent:** [Height of a prime ideal](#height-of-a-prime-ideal)

For a [prime ideal](#prime-ideal) $P$ of a [polynomial ring](#polynomial-ring) over a [field](algebra.md#field), the quotient's [Krull dimension](#krull-dimension) is the transcendence degree of its [fraction field](#field-of-fractions), and its height is $n$ minus that degree. This dimension theorem identifies algebraic codimension with the length of prime chains. It must not be applied indiscriminately to every Noetherian [ring](#ring) without its polynomial-ring hypotheses.

#### Prime avoidance

↑ **Parent:** [Height of an ideal](#height-of-an-ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_avoidance)

If an ideal $I$ is contained in a finite union of prime ideals $\mathfrak p_1\cup\cdots\cup\mathfrak p_r$, then $I$ is contained in one of the $\mathfrak p_i$. Equivalently, if none of the primes contains $I$, one can choose an element of $I$ outside all of them.

#### Krull principal ideal theorem

↑ **Parent:** [Height of an ideal](#height-of-an-ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull_principal_ideal_theorem)

In a [Noetherian ring](algebra.md#noetherian-ring), every [prime ideal](#prime-ideal) minimal over a proper principal ideal has height at most one.

For a proof, suppose instead that $\mathfrak p_0\subsetneq\mathfrak q\subsetneq\mathfrak p$ and that $\mathfrak p$ is minimal over $(a)$. Quotient by $\mathfrak p_0$ and localize at $\mathfrak p$; one may assume that $R$ is a Noetherian local domain, $0\subsetneq\mathfrak q\subsetneq\mathfrak p$ with $\mathfrak p$ maximal, and $\mathfrak p$ is the only prime containing $(a)$. For the symbolic powers

$$
\mathfrak q^{(n)}=\mathfrak q^nR_{\mathfrak q}\cap R,
$$

each $\mathfrak q^{(n)}$ is $\mathfrak q$-primary. The quotient $R/(a)$ is a zero-dimensional [Noetherian ring](algebra.md#noetherian-ring) and hence [Artinian](algebra.md#artinian-ring), so the descending chain $(\mathfrak q^{(n)}+(a))/(a)$ stabilizes. For large $n$, writing an element of $\mathfrak q^{(n)}$ modulo $\mathfrak q^{(n+1)}$ and using $a\notin\mathfrak q$ gives

$$
\mathfrak q^{(n)}=\mathfrak q^{(n+1)}+a\mathfrak q^{(n)}.
$$

The [Nakayama lemma](mathematics.md#nakayama-lemma) applied to $\mathfrak q^{(n)}/\mathfrak q^{(n+1)}$ gives $\mathfrak q^{(n)}=\mathfrak q^{(n+1)}$. Localizing at $\mathfrak q$ would therefore make the powers of the nonzero maximal ideal $\mathfrak qR_{\mathfrak q}$ stabilize at a nonzero ideal, contradicting the [Krull intersection theorem](module-theory.md#krull-intersection-theorem) for the Noetherian local domain $R_{\mathfrak q}$.

##### Principal prime in a Noetherian local ring lemma

↑ **Parent:** [Krull principal ideal theorem](#krull-principal-ideal-theorem)

If a principal prime ideal $(x)$ in a Noetherian local ring has positive height, then the ring is a domain. Localizing at $(x)$ shows that every annihilator of a power of $x$ lies in $(x)$; stabilization of the annihilator chain then proves that $x$ is a nonzerodivisor and that zero is prime.

##### Krull height theorem

↑ **Parent:** [Krull principal ideal theorem](#krull-principal-ideal-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull_height_theorem)

If an ideal of a [Noetherian ring](algebra.md#noetherian-ring) is generated by $n$ elements, every prime ideal minimal over it has height at most $n$. The proof inducts on $n$, using the [Krull principal ideal theorem](#krull-principal-ideal-theorem) in a quotient and [prime avoidance](#prime-avoidance) to choose a prime chain compatible with the induction.

###### Generator bound for primary-ideal length

↑ **Parent:** [Krull height theorem](#krull-height-theorem)

If $I$ is an $\mathfrak m$-primary [ideal](#ideal) generated by $n>0$ elements in a [Noetherian local ring](algebra.md#noetherian-local-ring) and $L=\operatorname{length}(R/I)$, then $I^j/I^{j+1}$ is a quotient of $\binom{j+n-1}{n-1}$ copies of $R/I$. Summing their lengths gives the displayed bound. Since $I\subseteq\mathfrak m$, it also bounds $\operatorname{length}(R/\mathfrak m^t)$. Together with the [prime-chain lower bound for local length](#prime-chain-lower-bound-for-local-length), localization at a minimal prime proves the [Krull height theorem](#krull-height-theorem).

##### Prime ideals between a three-prime chain

↑ **Parent:** [Krull principal ideal theorem](#krull-principal-ideal-theorem)

If $R$ is Noetherian and $\mathfrak p_0\subsetneq\mathfrak p_1\subsetneq\mathfrak p_2$ are prime ideals, there are infinitely many primes strictly between $\mathfrak p_0$ and $\mathfrak p_2$. After quotienting by $\mathfrak p_0$ and localizing at $\mathfrak p_2$, this reduces to a local Noetherian domain of dimension at least two. If it had only finitely many height-one primes, [prime avoidance](#prime-avoidance) would give a nonzero element of the maximal ideal outside all of them, contradicting the [Krull principal ideal theorem](#krull-principal-ideal-theorem).

###### Infinitude of intermediate-height prime ideals

↑ **Parent:** [Prime ideals between a three-prime chain](#prime-ideals-between-a-three-prime-chain)

If a Noetherian ring has finite [Krull dimension](#krull-dimension) $d$, then it has infinitely many prime ideals of each height $n$ with $0<n<d$. In a prime chain of maximal length, apply [prime ideals between a three-prime chain](#prime-ideals-between-a-three-prime-chain) to the terms of heights $n-1$, $n$, and $n+1$.

### Dimension theorem for Noetherian local rings

↑ **Parent:** [Krull dimension](#krull-dimension)

For a Noetherian local ring $(A,\mathfrak m)$, the Krull dimension of $A$, the Krull dimension of the [associated graded ring](#associated-graded-ring) $\operatorname{gr}_{\mathfrak m}(A)$, and the order of the pole at $t=1$ of its [Hilbert series](#hilbert-series) are equal.

#### System of parameters

↑ **Parent:** [Dimension theorem for Noetherian local rings](#dimension-theorem-for-noetherian-local-rings)

In a [Noetherian local ring](algebra.md#noetherian-local-ring) $(R,\mathfrak m)$ of dimension $d$, a list $x_1,\ldots,x_d\in\mathfrak m$ whose generated ideal has radical $\mathfrak m$. Such lists exist, by successively avoiding the finitely many top-dimensional minimal primes. No list shorter than $d$ can generate a maximal-primary ideal, by the [Krull height theorem](#krull-height-theorem).

#### Dimension drop by a non-zero-divisor

↑ **Parent:** [Dimension theorem for Noetherian local rings](#dimension-theorem-for-noetherian-local-rings)

If $x$ is a non-zero-divisor in a finite-dimensional Noetherian ring $A$, then

$$
\dim(A/(x))\leq\dim A-1.
$$

Every prime chain above $(x)$ can be extended downward by a minimal prime of $A$, because a non-zero-divisor belongs to no minimal prime.

## Polynomial ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_ring)

The polynomial ring $R[X]$ consists of polynomials in an indeterminate $X$ with coefficients in a ring $R$.

### Skew polynomial ring of an automorphism

↑ **Parent:** [Polynomial ring](#polynomial-ring)

For an [automorphism](algebra.md#automorphism) $\sigma$ of a unital [ring](#ring) $A$, this [ring](#ring) consists of finite sums $\sum_{j\geq0}a_jt^j$, with multiplication determined by $ta=\sigma(a)t$. Both left and right coefficient normal forms are available because $\sigma$ is invertible. The [noncommutative Hilbert basis theorem](noncommutative-algebra.md#noncommutative-hilbert-basis-theorem) implies that it is a [right Noetherian ring](noncommutative-algebra.md#right-noetherian-ring) when $A$ is, and a [left Noetherian ring](noncommutative-algebra.md#left-noetherian-ring) when $A$ is. Invertibility of $\sigma$ matters in this two-sided formulation.

#### Skew Laurent polynomial ring

↑ **Parent:** [Skew polynomial ring of an automorphism](#skew-polynomial-ring-of-an-automorphism)

Adjoining an inverse of $t$ to the [skew polynomial ring of an automorphism](#skew-polynomial-ring-of-an-automorphism) allows finite sums $\sum_{j\in\mathbb Z}a_jt^j$, with $ta=\sigma(a)t$. Every element can be moved into the polynomial subring by multiplying by a sufficiently large power of $t$. Consequently, for a [right ideal](associative-algebra.md#right-ideal) $I$ of this [ring](#ring), $I$ is generated by its intersection with the polynomial subring: if $ft^N$ lies there, then $f=(ft^N)t^{-N}$. This proves transfer of right [Noetherianity](algebra.md#noetherian-ring) from the polynomial subring, and multiplication on the left proves the left-handed version.

##### Skew Laurent extensions of domains are domains

↑ **Parent:** [Skew Laurent polynomial ring](#skew-laurent-polynomial-ring)

Let $A$ have no zero divisors and $\sigma$ be an [automorphism](algebra.md#automorphism). For nonzero [Laurent polynomials](polynomial.md#laurent-polynomial) $f=\sum a_ix^i$ and $g=\sum b_jx^j$ with greatest exponents $m,n$, the coefficient of $x^{m+n}$ in $fg$ is $a_m\sigma^m(b_n)$. No other exponent pair contributes to that highest degree. Both factors are nonzero, so their product is nonzero, proving the [noncommutative domain](noncommutative-algebra.md#noncommutative-domain) property in every characteristic.

##### Integral Heisenberg group algebra as a skew Laurent ring

↑ **Parent:** [Skew Laurent polynomial ring](#skew-laurent-polynomial-ring)

For the [Integer Heisenberg group](lie-algebra.md#integer-heisenberg-group), choose $x=I+E_{12}$, $y=I+E_{23}$ and central $z=I+E_{13}$. Every element has a unique form $y^cz^bx^a$, and $xy=zyx$. The [group algebra](associative-algebra.md#group-algebra) is therefore the displayed [skew Laurent polynomial ring](#skew-laurent-polynomial-ring), with $\sigma(z)=z$. The base is a commutative [Laurent polynomial ring](#laurent-polynomial-ring) and an [integral domain](#integral-domain); the [skew Hilbert basis theorem](noncommutative-algebra.md#skew-hilbert-basis-theorem) gives both-sided Noetherianity and the [leading coefficient](polynomial.md#leading-coefficient-of-a-polynomial) of a product proves that there are no zero divisors.

### Laurent polynomial ring

↑ **Parent:** [Polynomial ring](#polynomial-ring)

A Laurent polynomial ring is the [localization of a ring](#localization-of-a-ring) $k[X_1,\ldots,X_r]$ obtained by inverting all variables. Its elements are finite sums of [Laurent polynomials](polynomial.md#laurent-polynomial) with exponent vectors in $\mathbb Z^r$. It is a [Noetherian ring](algebra.md#noetherian-ring) by the [Hilbert basis theorem](algebra.md#hilbert-basis-theorem) and [Localization of a Noetherian ring](#localization-of-a-noetherian-ring).

#### Unit of a Laurent polynomial ring

↑ **Parent:** [Laurent polynomial ring](#laurent-polynomial-ring)

For an [integral domain](#integral-domain) $R$, the [breadth of a Laurent polynomial](polynomial.md#breadth-of-a-laurent-polynomial) adds under multiplication. If two Laurent [polynomials](polynomial.md) multiply to one, both therefore have breadth zero: they are [monomials](polynomial.md#monomial), and their coefficients must be [units](algebra.md#unit-in-a-ring) of $R$. Conversely every displayed monomial is invertible. For $R=\mathbb Z$ the units are precisely $\pm t^k$, explaining the normalization ambiguity of an [Alexander polynomial](knot-theory.md#alexander-polynomial).

#### Laurent normalization by a monomial change of variables

↑ **Parent:** [Laurent polynomial ring](#laurent-polynomial-ring)

A nonzero quotient of an $r$-variable [Laurent polynomial ring](#laurent-polynomial-ring) is finite over an embedded [Laurent polynomial ring](#laurent-polynomial-ring) in $m\leq r$ variables. Given a nonzero Laurent relation, choose $N$ so that weights $(N,N^2,\ldots,N^{r-1},1)$ separate its finite exponent support. The displayed invertible [monomial](polynomial.md#monomial) substitution makes its extreme $Y_r$ coefficients units in the remaining Laurent variables. Normalize the relation to a [monic polynomial](polynomial.md#monic-polynomial) with unit constant term; both $Y_r$ and $Y_r^{-1}$ are integral over the image of the $(r-1)$-variable subring. Induction and transitivity of finite extensions prove the assertion, over finite [fields](algebra.md#field) as well as infinite [fields](algebra.md#field). An infinite-dimensional quotient has $m\geq1$.

#### Noetherianity of subalgebras of a one-variable Laurent polynomial ring

↑ **Parent:** [Laurent polynomial ring](#laurent-polynomial-ring)

Every unital $k$-[subalgebra](algebra.md#subalgebra) $A\subseteq k[T,T^{-1}]$ is a [Noetherian ring](algebra.md#noetherian-ring). If $A\subseteq k[T]$ or $k[T^{-1}]$, a nonconstant element $f\in A$ makes that ambient [polynomial ring](#polynomial-ring) a [finitely generated module](module-theory.md#finitely-generated-module) over $k[f]$. Otherwise $A$ contains an $f$ with both positive and negative exponents, and both $T$ and $T^{-1}$ are [integral elements](#integral-element) over $k[f]$. In either case $A$ is a [submodule](module-theory.md#submodule) of a finite module over the [Noetherian ring](algebra.md#noetherian-ring) $k[f]$, and every [ideal](#ideal) of $A$ is finitely generated over $k[f]$, hence over $A$.

#### Separating finite Laurent support by an integer weight

↑ **Parent:** [Laurent polynomial ring](#laurent-polynomial-ring)

Given a finite set $F\subset\mathbb Z^r$ of exponent vectors, there is $w\in\mathbb Z^r$ for which the integers $w\cdot m$, $m\in F$, are pairwise distinct. For $r=2$, take $w=(1,N)$ with $N$ larger than every first-coordinate difference in $F$. In higher dimensions take $w=(1,N,\ldots,N^{r-1})$ with $N$ sufficiently large. This proves that a nonzero [Laurent polynomial](polynomial.md#laurent-polynomial) can be detected by a substitution $X_i=T^{w_i}$ without cancellation of its distinct terms.

### Integer-valued polynomial

↑ **Parent:** [Polynomial ring](#polynomial-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer-valued_polynomial)

For an [integral domain](#integral-domain) $R$, an integer-valued [polynomial](polynomial.md) is a [polynomial](polynomial.md) over its [fraction field](#field-of-fractions) that maps $R$ into itself. Its coefficients need not lie in $R$: $X(X-1)/2$ maps $\mathbb Z$ into $\mathbb Z$. These [polynomials](polynomial.md) form a [ring](#ring) containing $R[X]$.

#### Binomial polynomial

↑ **Parent:** [Integer-valued polynomial](#integer-valued-polynomial)

For $n\geq0$, define $B_0(X)=1$ and $B_n(X)=X(X-1)\cdots(X-n+1)/n!$. The [binomial coefficient](combinatorics.md#binomial-coefficient) formula shows $B_n(m)\in\mathbb Z$ for every nonnegative integer $m$. Since these integers are dense in the [p-adic integers](number-theory.md#p-adic-integer), [continuity](calculus.md#continuous-function) of the [polynomial](polynomial.md) implies $B_n(\mathbb Z_p)\subseteq\mathbb Z_p$, so it is an [integer-valued polynomial](#integer-valued-polynomial) there and $\|B_n\|_\infty=1$. The [Pascal's identity](combinatorics.md#pascal-s-rule) gives $\Delta B_{n+1}=B_n$ for the [forward difference operator](finite-difference.md#forward-difference-operator).

### Automorphism of a polynomial ring

↑ **Parent:** [Polynomial ring](#polynomial-ring)

An automorphism of a polynomial ring is an invertible ring homomorphism from the ring to itself. For example, $f(X)\mapsto f(X+a)$ has inverse $f(X)\mapsto f(X-a)$, so translating the variable preserves reducibility.

### Reduction of an integer polynomial modulo a prime

↑ **Parent:** [Polynomial ring](#polynomial-ring)

Coefficientwise reduction defines a [ring homomorphism](#ring-homomorphism)

$$
\mathbb Z[X]\longrightarrow\mathbb F_p[X].
$$

It preserves sums, products, and divisibility. The [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) gives $\overline{g(X^p)}=\bar g(X)^p$.

### Unit in a polynomial ring

↑ **Parent:** [Polynomial ring](#polynomial-ring)

If $R$ is an integral domain, the units of $R[x]$ are precisely the constant polynomials whose values are units of $R$.

### McCoy theorem

↑ **Parent:** [Polynomial ring](#polynomial-ring)

A polynomial $f\in R[t]$ is a zero divisor exactly when some nonzero scalar $a\in R$ annihilates it. One proof chooses a nonzero polynomial $g$ of minimal degree with $fg=0$ and successively kills its leading coefficient.

## Maximal ideal

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximal_ideal)

A proper ideal $\mathfrak m$ of a commutative ring $R$ is maximal when no proper ideal lies strictly between $\mathfrak m$ and $R$. Equivalently, $R/\mathfrak m$ is a field.

### Residue field

↑ **Parent:** [Maximal ideal](#maximal-ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residue_field)

The residue field at a maximal ideal $\mathfrak m$ is the quotient field $\kappa(\mathfrak m)=R/\mathfrak m$. At a prime ideal $\mathfrak p$, the residue field is the fraction field of $R/\mathfrak p$.

#### Residue-field extension

↑ **Parent:** [Residue field](#residue-field)

A local homomorphism of local rings $(R,\mathfrak m)\to(S,\mathfrak n)$ induces the residue-field extension $R/\mathfrak m\to S/\mathfrak n$. For an extension of non-Archimedean local fields, its degree is the [residue-field degree](arithmetic.md#residue-field-degree).

#### Residue characteristic

↑ **Parent:** [Residue field](#residue-field)

The residue characteristic of a local ring is the [characteristic of a ring](#characteristic-of-a-ring) of its [residue field](#residue-field). A finite extension of $\mathbb Q_p$ has residue characteristic $p$.

### Maximal spectrum

↑ **Parent:** [Maximal ideal](#maximal-ideal)

The maximal spectrum $\operatorname{MaxSpec}R$ is the set of maximal ideals of a commutative ring $R$.

### Maximal ideal quotient criterion

↑ **Parent:** [Maximal ideal](#maximal-ideal)

An ideal $\mathfrak m$ of a commutative unital ring $R$ is maximal exactly when $R/\mathfrak m$ is a field.

## Local ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_ring)

A local ring is a [commutative ring](#commutative-ring) with exactly one maximal ideal.

### Local homomorphism of local rings

↑ **Parent:** [Local ring](#local-ring)

A homomorphism $\varphi:(A,\mathfrak m)\to(B,\mathfrak n)$ of [local rings](#local-ring) is local if $\varphi(\mathfrak m)\subseteq\mathfrak n$, equivalently $\varphi^{-1}(\mathfrak n)=\mathfrak m$. The equivalence uses the fact that all elements outside $\mathfrak m$ are [units](algebra.md#unit-in-a-ring). It induces an embedding of [residue fields](#residue-field) $A/\mathfrak m\to B/\mathfrak n$.

### Local integral domain

↑ **Parent:** [Local ring](#local-ring)

A [local ring](#local-ring) that is also an [integral domain](#integral-domain). Multiplication by any nonzero element is injective. This permits cancellation in [Artin-Rees lemma](module-theory.md#artin-rees-lemma) length-growth arguments.

### Cotangent space of a local ring

↑ **Parent:** [Local ring](#local-ring)

For a [local ring](#local-ring) $(R,\mathfrak m)$ with [residue field](#residue-field) $\kappa=R/\mathfrak m$, its cotangent space is the $\kappa$-[vector space](vector-space.md) $\mathfrak m/\mathfrak m^2$. In a [Noetherian local ring](algebra.md#noetherian-local-ring), its [dimension](vector-space.md#dimension-vector-space) is the minimal number of generators of $\mathfrak m$, by the [Nakayama lemma](mathematics.md#nakayama-lemma). Equality of this [dimension](vector-space.md#dimension-vector-space) with the [Krull dimension](#krull-dimension) defines a [regular local ring](#regular-local-ring).

#### Embedding dimension

↑ **Parent:** [Cotangent space of a local ring](#cotangent-space-of-a-local-ring)

The embedding dimension of a [Noetherian local ring](algebra.md#noetherian-local-ring) $(R,\mathfrak m)$ is $\dim_{R/\mathfrak m}(\mathfrak m/\mathfrak m^2)$. It counts the smallest number of local generators needed for the [maximal ideal](#maximal-ideal). It is at least the [Krull dimension](#krull-dimension); equality characterizes a [regular local ring](#regular-local-ring).

### Regular local ring

↑ **Parent:** [Local ring](#local-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_local_ring)

A Noetherian local ring $(R,\mathfrak m)$ is regular when the minimal number of generators of its [maximal ideal](#maximal-ideal) equals its [Krull dimension](#krull-dimension). Every regular local ring is an [integral domain](#integral-domain) and a [unique factorization domain](algebra.md#unique-factorization-domain).

#### Regular system of parameters

↑ **Parent:** [Regular local ring](#regular-local-ring)

In a regular local ring of dimension $d$, a regular system of parameters is a list in the maximal ideal whose images form a residue-field basis of $\mathfrak m/\mathfrak m^2$. The [Nakayama lemma](mathematics.md#nakayama-lemma) shows that it generates the maximal ideal. At a smooth closed point over an algebraically closed field, these are the local parameters in all dimensions, extending the single [local parameter on a smooth algebraic curve](projective-space.md#local-parameter-on-a-smooth-algebraic-curve).

##### Formal expansion at a smooth point

↑ **Parent:** [Regular system of parameters](#regular-system-of-parameters)

A chosen [regular system of parameters](#regular-system-of-parameters) gives the displayed completion isomorphism by sending $T_i$ to $t_i$. The [associated graded ring of a regular local ring](#associated-graded-ring-of-a-regular-local-ring) is the polynomial ring on their initial forms. Successively removing the homogeneous initial form of each remainder gives a unique formal series for every local function. The [Krull intersection theorem](module-theory.md#krull-intersection-theorem) embeds the local ring in its completion. The power-series characterization is also given in [Stacks Project Lemma 10.160.10](https://stacks.math.columbia.edu/tag/0C0S).

#### Formal power series preserve regular local rings

↑ **Parent:** [Regular local ring](#regular-local-ring)

Let $(A,\mathfrak m)$ be a [regular local ring](#regular-local-ring) of [Krull dimension](#krull-dimension) $d$. Its [formal power series ring](#formal-power-series) $B=A[[x]]$ is [Noetherian](algebra.md#noetherian-ring) and local, with [maximal ideal](#maximal-ideal) $I=\mathfrak mB+(x)$ and [embedding dimension](#embedding-dimension) $d+1$. Since $I$ is generated by $d+1$ elements, the [Krull height theorem](#krull-height-theorem) gives $\dim B\leq d+1$. For the reverse inequality choose a strict prime chain $\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_d=\mathfrak m$ in $A$. Finite generation of each $\mathfrak p_i$ gives $B/\mathfrak p_iB\cong(A/\mathfrak p_i)[[x]]$, an [integral domain](#integral-domain), so each extended [ideal](#ideal) is prime. The inclusions remain strict by contraction to $A$, and $\mathfrak mB\subsetneq I$ adds one more step since $x\notin\mathfrak mB$. This proves $\dim B=d+1$, equal to its [embedding dimension](#embedding-dimension), and hence regularity.

#### Associated graded ring of a regular local ring

↑ **Parent:** [Regular local ring](#regular-local-ring)

For a [regular local ring](#regular-local-ring) of [embedding dimension](#embedding-dimension) $e$, a minimal maximal-[ideal](#ideal) generating set induces the displayed polynomial-algebra isomorphism. It is surjective in every degree. A nonzero homogeneous kernel relation would bound the cumulative Hilbert function by $O(t^{e-1})$, contradicting the [prime-chain lower bound for local length](#prime-chain-lower-bound-for-local-length) at $\dim R=e$. The [graded ring](#graded-ring) is a domain; the [Krull intersection theorem](module-theory.md#krull-intersection-theorem) then shows the original ring is a domain by multiplying nonzero initial forms.

### Valuation ring

↑ **Parent:** [Local ring](#local-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Valuation_ring)

A valuation ring is an [integral domain](#integral-domain) $R$ such that, for every nonzero element $x$ of its [fraction field](#field-of-fractions) $K$, either $x\in R$ or $x^{-1}\in R$. Equivalently, its ideals are totally ordered by inclusion.

#### Principal ideal criterion for a nontrivial rank-one valuation ring

↑ **Parent:** [Valuation ring](#valuation-ring)

A [valuation ring](#valuation-ring) for a nontrivial real-valued rank-one [valuation](algebra.md#valuation) is a [principal ideal domain](#principal-ideal-domain) exactly when its value group is discrete. A least positive value makes the value group cyclic and lets every nonzero ideal be generated by an element of smallest valuation. Conversely, if the maximal ideal is principal, its generator has the least positive value. Nontriviality matters: a field with the trivial valuation is a principal ideal domain, but not a [discrete valuation ring](#discrete-valuation-ring) in the usual nontrivial convention.

#### Valuation domination lemma

↑ **Parent:** [Valuation ring](#valuation-ring)

Every local subring $A$ of a [field](algebra.md#field) $K$ is dominated by a [valuation ring](#valuation-ring) with [fraction field](#field-of-fractions) $K$. Order local overrings by inclusion and contraction of their maximal [ideals](#ideal); chain unions are local, so [Zorn's lemma](set-theory.md#zorn-s-lemma) gives a maximal one. For each $z\in K^\times$, at least one of the extensions of its [maximal ideal](#maximal-ideal) to $V[z]$ and $V[z^{-1}]$ is proper: otherwise two least-degree relations for $1$ with maximal-ideal coefficients reduce one another to a smaller-degree relation. Localizing the proper extension gives a dominating overring, so maximality forces either $z$ or $z^{-1}$ into $V$.

#### Valuation rings are integrally closed

↑ **Parent:** [Valuation ring](#valuation-ring)

If an element $x$ of the [fraction field](#field-of-fractions) is absent from a [valuation ring](#valuation-ring) $V$, its inverse $y$ belongs to the [maximal ideal](#maximal-ideal). A monic equation for $x$, multiplied by a power of $y$, would put $1$ in that [maximal ideal](#maximal-ideal). Thus $V$ is an [integrally closed domain](#integrally-closed-domain), without a discrete or [Noetherian](algebra.md#noetherian-ring) hypothesis.

#### Discrete valuation ring

↑ **Parent:** [Valuation ring](#valuation-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_valuation_ring)

A discrete valuation ring is a [principal ideal domain](#principal-ideal-domain) with exactly one nonzero maximal ideal. Every nonzero element of its [fraction field](#field-of-fractions) is a unit times a unique integer power of a uniformizer.

##### Complete discretely valued field

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)

A [field](algebra.md#field) with a surjective discrete [valuation](algebra.md#valuation), complete for the associated non-Archimedean metric. Its [valuation ring](#valuation-ring) is a [discrete valuation ring](#discrete-valuation-ring), and its [maximal ideal](#maximal-ideal) is generated by a [uniformizer](#uniformizer). [Completeness](topological-analysis.md#completeness) allows successive congruence solutions to converge to actual roots, which underlies the [Hensel lemma](arithmetic.md#hensel-s-lemma). Non-Archimedean [local fields](arithmetic.md#local-field) are examples; [completeness](topological-analysis.md#completeness) alone does not require the [residue field](#residue-field) to be finite.

##### Digit expansion in a discretely valued field

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)

For a normalized [discrete valuation](#discrete-valuation), a [uniformizer](#uniformizer) $\pi$, and a chosen set $A$ of representatives of the [residue field](#residue-field), every existing nonzero element has a unique displayed expansion, with its first digit not in the maximal ideal. Starting from $y_0=\pi^{-v(x)}x$, choose $a_j$ representing $y_j$ modulo the maximal ideal and put $y_{j+1}=(y_j-a_j)/\pi$. The error after $r$ digits has valuation at least $v(x)+r$, so the sums converge to $x$ even without [completeness](topological-analysis.md#completeness). Conversely arbitrary digit sequences need not converge in an incomplete field: in $\mathbb Q$ with its three-adic valuation, the digits of $\sqrt{10}\in\mathbb Q_3$ give a counterexample. [Hensel lemma](arithmetic.md#hensel-s-lemma) gives this square root, but it is not rational.

##### One-dimensional normal local rings are discrete valuation rings

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)

Let $R$ be a one-dimensional normal Noetherian local domain. Choose $0\ne x$ in its maximal ideal $\mathfrak m$ and a minimal $n$ with $\mathfrak m^n\subseteq(x)$. If $n>1$, choose $y\in\mathfrak m^{n-1}\setminus(x)$ and put $z=y/x$. Then $z\notin R$ but $z\mathfrak m\subseteq R$. If $z\mathfrak m\subseteq\mathfrak m$, the [determinant trick](module-theory.md#determinant-trick) makes $z$ integral, contrary to normality. Thus $zu$ is a unit for some $u\in\mathfrak m$, and $v=u(zv)/(zu)$ for every $v\in\mathfrak m$ proves $\mathfrak m=(u)$. The case $n=1$ is already principal. Such a local domain is a [discrete valuation ring](#discrete-valuation-ring).

##### Complete discrete valuation ring

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)

A complete discrete [valuation](algebra.md#valuation) ring is a [discrete valuation ring](#discrete-valuation-ring) complete for its maximal-ideal-adic topology. Equivalently, the canonical map to the [inverse limit](module-theory.md#inverse-limit) of the residue rings is an isomorphism: compatible residue classes determine a Cauchy sequence, and completeness gives its unique limit. Standard examples are $\mathbb Z_p$ and $k[[t]]$. This completeness is the hypothesis that makes [Newton iteration over a valued field](arithmetic.md#newton-iteration-over-a-valued-field) converge in the ring in the usual [Hensel lemma](arithmetic.md#hensel-s-lemma).

##### Discrete valuation

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_valuation)

A discrete valuation on a field $K$ is a surjective group homomorphism $v:K^\times\to\mathbb Z$ satisfying $v(x+y)\geq\min(v(x),v(y))$ whenever $x+y\ne0$. Its valuation ring is $\{0\}\cup\{x:v(x)\geq0\}$.

###### Discretely valued field

↑ **Parent:** [Discrete valuation](#discrete-valuation)

A discretely valued field is a field equipped with a [discrete valuation](#discrete-valuation). It is complete when every [Cauchy sequence](real-analysis.md#cauchy-sequence) for the induced metric converges.

###### Value group

↑ **Parent:** [Discrete valuation](#discrete-valuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Value_group)

The value group of a valued field is the ordered abelian group formed by the values of its nonzero elements. A valuation is discrete when its value group is infinite cyclic with the order inherited from $\mathbb Z$.

##### Uniformizer

↑ **Parent:** [Discrete valuation ring](#discrete-valuation-ring)

A uniformizer of a [discrete valuation ring](#discrete-valuation-ring) $R$ is a generator $\pi$ of its unique nonzero [maximal ideal](#maximal-ideal). Every nonzero $x$ in the [fraction field](#field-of-fractions) has a unique expression $x=u\pi^n$ with $u$ a unit and $n\in\mathbb Z$.

## Dedekind domain

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dedekind_domain)

A Dedekind domain is a Noetherian integrally closed domain of Krull dimension one. Equivalently, every localization at a nonzero prime ideal is a discrete valuation ring.

### Two generators for an ideal in a Dedekind domain

↑ **Parent:** [Dedekind domain](#dedekind-domain)

Every [ideal](#ideal) of a [Dedekind domain](#dedekind-domain) is generated by at most two elements. Given a nonzero [ideal](#ideal) $I$ and any prescribed nonzero $a\in I$, the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) supplies $b\in I$ with $v_P((b))=v_P(I)$ at every [prime ideal](#prime-ideal) dividing $(a)$. The [prime-ideal valuation in a Dedekind domain](#prime-ideal-valuation-in-a-dedekind-domain) then gives $I=(a,b)$.

### Unique factorization of ideals in a Dedekind domain

↑ **Parent:** [Dedekind domain](#dedekind-domain)

Every nonzero proper [ideal](#ideal) of a [Dedekind domain](#dedekind-domain) has a unique factorization, up to reordering, as a finite product of positive powers of distinct nonzero [prime ideals](#prime-ideal). The unit [ideal](#ideal) is the empty product. This is distinct from unique factorization of elements.

#### Prime-ideal valuation in a Dedekind domain

↑ **Parent:** [Unique factorization of ideals in a Dedekind domain](#unique-factorization-of-ideals-in-a-dedekind-domain)

For a nonzero [ideal](#ideal) $I$ in a [Dedekind domain](#dedekind-domain), $v_P(I)$ is the exponent of the nonzero [prime ideal](#prime-ideal) $P$ in the [unique factorization of ideals in a Dedekind domain](#unique-factorization-of-ideals-in-a-dedekind-domain). Then $I\subseteq J$ if and only if $v_P(I)\geq v_P(J)$ for every $P$, and $v_P(I+J)=\min(v_P(I),v_P(J))$.

### Principal maximal ideal in a one-dimensional normal local domain

↑ **Parent:** [Dedekind domain](#dedekind-domain)

The maximal ideal of an integrally closed Noetherian local domain of Krull dimension one is principal. Hence every such local ring is a [discrete valuation ring](#discrete-valuation-ring).

## Ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ring_(mathematics))

A ring has addition and multiplication, with an abelian group under addition and multiplication distributive over addition.

### Zero ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zero_ring)

The ring with a single element, which is both its additive and multiplicative identity. If a unital [ring](#ring) has $0=1$, then every element $r$ equals $r1=r0=0$, so it is this ring. Under the usual definition it is excluded from [integral domains](#integral-domain) and [fields](algebra.md#field). The [quotient ring](#quotient-ring) $\mathbb Z/(1)$ is an example.

### Perfect ring of characteristic p

↑ **Parent:** [Ring](#ring)

A [commutative ring](#commutative-ring) of prime characteristic $p$ is perfect in the Frobenius sense when its [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) is an automorphism. It is necessarily reduced: if $a$ is nilpotent, some $p$-power iterate is zero, and injectivity gives $a=0$. This use of perfect is distinct from the homological notion of a perfect ring. The [Absolute Frobenius morphism](ringed-space.md#absolute-frobenius-morphism) of a [scheme](ringed-space.md#scheme) is an [isomorphism](algebra.md#isomorphism) exactly when all its [local rings](#local-ring) are perfect in this sense, because it is the identity on points and is an isomorphism on every stalk.

### Opposite ring

↑ **Parent:** [Ring](#ring)

The opposite ring has the same additive group and identity as a [ring](#ring) $R$, with multiplication $a\cdot_{\mathrm{op}}b=ba$. Left [modules](module-theory.md#module-mathematics) over it are right [modules](module-theory.md#module-mathematics) over $R$. Forming the opposite exchanges left and right chain conditions and reverses the order of composition when interpreting endomorphisms as right multiplications. For an [associative algebra](associative-algebra.md) with its scalar action retained, this construction gives the [opposite algebra](associative-algebra.md#opposite-algebra).

### Subring

↑ **Parent:** [Ring](#ring)

A subset closed under addition, additive inverses and multiplication, with the induced operations. Under the unital convention used here it also contains the identity of $R$. A subring of an [integral domain](#integral-domain) is again an integral domain. The [ring of invariants](group-theory.md#ring-of-invariants) is one example: fixed elements remain fixed under all ring operations.

### Topological ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_ring)

A topological ring is a [ring](#ring) equipped with a [topology](topology.md) making addition, additive inversion and multiplication [continuous functions](calculus.md#continuous-function). An [adic topology](#adic-topology) is obtained from powers of an [ideal](#ideal).

#### Pro-p ring

↑ **Parent:** [Topological ring](#topological-ring)

A pro-$p$ ring is a topological ring with continuous ring operations whose underlying additive [group](group.md) is a [pro-p group](topological-group.md#pro-p-group). Standard local analytic examples are complete Noetherian local rings with finite [residue field](#residue-field) of characteristic $p$, such as $\mathbb Z_p$ and $\mathbb F_p[[t]]$. The [topology](topology.md) is essential to the convergence of [power series](real-analysis.md#power-series) used for analytic [group](group.md) operations.

#### Adic topology

↑ **Parent:** [Topological ring](#topological-ring)

For a two-sided [ideal](#ideal) $I$ of a [ring](#ring) $R$, the powers $I^n$ form a neighborhood base at zero for the adic topology. For an $R$-[module](module-theory.md#module-mathematics) $M$, use $I^nM$ on the left or $MI^n$ on the right. Convergence means that for every $n$ the differences eventually belong to the corresponding submodule. The [formal power series ring](#formal-power-series) $k[[t]]$ and [formal power series module](#formal-power-series-module) $M[[t]]$ are complete for $I=(t)$; convergence fixes each finite list of coefficients eventually. This is formal convergence, without an analytic condition on the size of coefficients.

##### Completed localization of an adic ring

↑ **Parent:** [Adic topology](#adic-topology)

For a complete Noetherian [ring](#ring) with ideal of definition $I$, completed localization is the completion of the [localization of a ring](#localization-of-a-ring) $A_f$ in the induced [adic topology](#adic-topology). It gives the sections of the [formal spectrum](ringed-space.md#formal-spectrum) over $D(f)$. For $A=k[t][[q]]$, its completed localization at $t$ is $k[t,t^{-1}][[q]]$. Ordinary localization allows a bounded pole order in $t$ across all coefficients; the latter [ring](#ring) also contains $\sum_{n\geq0}q^nt^{-n}$, whose pole orders are unbounded.

// Target: ringed-space.bigb

##### Adic completion of a module

↑ **Parent:** [Adic topology](#adic-topology)

The adic completion is the [inverse limit](module-theory.md#inverse-limit) of the [quotient modules](module-theory.md#quotient-module) $M/I^nM$. An element is a compatible family of residue classes at every order. For $R=k[t]$ and $M=V\otimes_k k[t]$, this gives the [formal power series module](#formal-power-series-module) $V[[t]]$. The canonical map from $M$ need not be injective in general: its [kernel](linear-algebra.md#kernel-of-a-linear-map) is $\bigcap_n I^nM$. It is injective for this polynomial example because a nonzero polynomial has finite degree. Successive changes of coordinates in [formal rigidity from vanishing second Hochschild cohomology](associative-algebra.md#formal-rigidity-from-vanishing-second-hochschild-cohomology) converge in this completion because the order-$r$ change is the identity modulo $t^r$.

###### Power-series presentation of an adic completion

↑ **Parent:** [Adic completion of a module](#adic-completion-of-a-module)

If $I=(a_1,\ldots,a_s)$, evaluation $X_i\mapsto a_i$ gives a ring map to the $I$-adic completion, with each series evaluated modulo $I^r$ using only terms of total degree below $r$. It is surjective: successively represent the residual class in $I^r/I^{r+1}$ by a homogeneous degree-$r$ polynomial in the $a_i$. If $R$ is a commutative [Noetherian ring](algebra.md#noetherian-ring), [Noetherianity of formal power series rings](#noetherianity-of-formal-power-series-rings) therefore makes its completion Noetherian.

###### Surjectivity on adic completions

↑ **Parent:** [Adic completion of a module](#adic-completion-of-a-module)

For any ideal $I$ and surjective module map $f:M\to N$, compatible representatives $n_r$ modulo $I^rN$ can be lifted recursively. Having chosen $f(m_r)=n_r$, lift $n_{r+1}-n_r\in I^rN$ to $\delta_r\in I^rM$ and put $m_{r+1}=m_r+\delta_r$. These define the required element of the [adic completion of a module](#adic-completion-of-a-module). No finite-generation hypothesis on the modules is required.

### Von Neumann regular ring

↑ **Parent:** [Ring](#ring)

A ring is von Neumann regular if every element $a$ has an element $b$ with $a=aba$. In a [commutative ring](#commutative-ring), this is $a=a^2b$. An arbitrary [direct product of rings](#direct-product-of-rings) whose factors are [fields](algebra.md#field) has this property by taking inverses in each nonzero coordinate. Every [localization at a prime ideal](#localization-at-a-prime-ideal) of a commutative von Neumann regular ring is a [field](algebra.md#field).

### Direct product of rings

↑ **Parent:** [Ring](#ring)

The direct product of a family of [rings](#ring) consists of all tuples of their elements, with coordinatewise addition and multiplication. Unlike a direct sum, tuples may have infinitely many nonzero coordinates.

### Characteristic of a ring

↑ **Parent:** [Ring](#ring)

The characteristic of a [ring](#ring) $R$ is the least positive integer $n$ satisfying $n\cdot1_R=0$, or zero if no such integer exists. A nonzero ring of positive characteristic has prime characteristic when it is an [integral domain](#integral-domain).

### Division ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Division_ring)

A division ring is a nonzero [ring](#ring) in which every nonzero element has a multiplicative inverse. Its multiplication need not be [commutative](#commutative-ring).

### Simple ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_ring)

A nonzero ring is simple when its only two-sided ideals are zero and the whole ring.

### Semisimple ring

↑ **Parent:** [Ring](#ring)

A semisimple ring is a ring that is semisimple as a module over itself. Equivalently, every module over it is semisimple, so every short exact sequence of modules splits.

### Group ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_ring)

The [group ring](#group-ring) $R[G]$ consists of finite formal sums $\sum_{g\in G}r_gg$ with coefficients in a [ring](#ring) $R$. Addition is coefficientwise and multiplication extends the [group operation](group.md#group-operation) and multiplication in $R$ distributively. A [group algebra](associative-algebra.md#group-algebra) is the case in which $R$ is a [field](algebra.md#field).

#### Group rings of poly-(cyclic or finite) groups are Noetherian

↑ **Parent:** [Group ring](#group-ring)

If $A$ is a [left Noetherian ring](noncommutative-algebra.md#left-noetherian-ring) and a [right Noetherian ring](noncommutative-algebra.md#right-noetherian-ring), and $G$ is a [poly-(cyclic or finite) group](group.md#poly-cyclic-or-finite-group), then $A[G]$ satisfies both chain conditions. Induct along the [subnormal series](group-theory.md#subnormal-series). A finite factor gives a finite free extension on each side, handled by [finite-module extension preserves Noetherianity](noncommutative-algebra.md#finite-module-extension-preserves-noetherianity). An infinite cyclic factor gives a [skew Laurent polynomial ring](#skew-laurent-polynomial-ring), with the twisting [automorphism](algebra.md#automorphism) induced by conjugation by a lift of the cyclic generator. The [noncommutative Hilbert basis theorem](noncommutative-algebra.md#noncommutative-hilbert-basis-theorem) and clearing negative powers prove the required chain conditions at that step. In particular $\mathbb Z[G]$ is [Noetherian](algebra.md#noetherian-ring).

#### Augmentation ideal

↑ **Parent:** [Group ring](#group-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Augmentation_ideal)

The augmentation homomorphism $\varepsilon:R[G]\to R$ sends $\sum_gr_gg$ to $\sum_gr_g$. Its kernel is the augmentation ideal.

##### Cyclic finite quotients of the p-adic augmentation filtration

↑ **Parent:** [Augmentation ideal](#augmentation-ideal)

In the ordinary [group algebra](associative-algebra.md#group-algebra) of the additive [p-adic integers](number-theory.md#p-adic-integer), let $I$ be the [augmentation ideal](#augmentation-ideal). The [kernel](linear-algebra.md#kernel-of-a-linear-map) of the map to the [group algebra](associative-algebra.md#group-algebra) of $\mathbb Z_p/p^r\mathbb Z_p$ is generated by $[p^rh]-1=([h]-1)^{p^r}$, so it is contained in $I^{p^r}$. The quotient is the cyclic-group algebra $\mathbb F_p[T]/(T^{p^r})$, so its [augmentation ideal](#augmentation-ideal) has zero $p^r$th power and the reverse inclusion holds. Every finite degree of the [associated graded ring](#associated-graded-ring) can be read from such a quotient, giving $\operatorname{gr}_I\mathbb F_p[\mathbb Z_p]\cong\mathbb F_p[X]$. The completion is $\mathbb F_p[[T]]$, but completion is not needed for the graded calculation.

##### Nilpotence of a p-group augmentation ideal

↑ **Parent:** [Augmentation ideal](#augmentation-ideal)

In characteristic $p$, the [augmentation ideal](#augmentation-ideal) $I$ of the [group algebra](associative-algebra.md#group-algebra) of a finite $p$-group is nilpotent. Choose a central element $z$ of order $p$ and put $t=z-1$, so $t^p=0$. The quotient by $t$ is the group algebra of the smaller quotient group. Induction gives $I^m\subseteq t kP$ for some $m$, hence $I^{mp}=0$. For a normal $p$-subgroup $P$ of $G$, conjugation stability gives $(I kG)^m=I^m kG$, proving nilpotence of the kernel of $kG\to k(G/P)$.

##### Augmentation ideal of the infinite cyclic group

↑ **Parent:** [Augmentation ideal](#augmentation-ideal)

The [group ring](#group-ring) of an [infinite cyclic group](group.md#infinite-cyclic-group) is the Laurent polynomial ring $R=\mathbb Z[t,t^{-1}]$, with augmentation $\varepsilon(t)=1$. Multiply any element in the kernel by a power of $t$ to obtain a polynomial vanishing at one. The [factor theorem](polynomial.md#factor-theorem) makes it divisible by $t-1$. Thus the [augmentation ideal](#augmentation-ideal) is $(t-1)R$. Since $R$ is an [integral domain](#integral-domain), multiplication by $t-1$ is an injective module map, so this ideal is a free $R$-module of rank one, even though its additive group has infinite rank.

### Noncommutative ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noncommutative_ring)

A noncommutative ring is a [ring](#ring) whose multiplication is not required to be commutative.

### Nilpotent

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent)

An element $x$ of a ring is nilpotent when $x^n=0$ for some positive integer $n$. A field has no nonzero nilpotent elements.

### Commutative ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Commutative_ring)

A commutative ring is a [ring](#ring) whose multiplication satisfies $ab=ba$.

#### Associate element

↑ **Parent:** [Commutative ring](#commutative-ring)

#### Regular sequence

↑ **Parent:** [Commutative ring](#commutative-ring)

A regular sequence in a [commutative ring](#commutative-ring) $A$ is a finite list such that $(f_1,\ldots,f_r)$ is proper and $f_j$ is a [non-zero-divisor](mathematics.md#non-zero-divisor) on $A/(f_1,\ldots,f_{j-1})$ for each $j$. In a graded ring with homogeneous $f_j$, injectivity can be checked on homogeneous elements because components of distinct degrees cannot cancel. It gives [short exact sequences](module-theory.md#short-exact-sequence) $0\to R_{j-1}(-\deg f_j)\to R_{j-1}\to R_j\to0$ for the successive graded quotients.

##### Depth of a Noetherian local ring

↑ **Parent:** [Regular sequence](#regular-sequence)

The depth of a [Noetherian local ring](algebra.md#noetherian-local-ring) is the maximal length of an $R$-regular sequence in its maximal ideal. It is at most its [Krull dimension](#krull-dimension). Quotienting by a nonzero divisor lowers depth by one. This invariant measures how many independent successive nonzero-divisor equations the local algebra supports.

#### Dual number

↑ **Parent:** [Commutative ring](#commutative-ring)

The dual-number ring over a [field](algebra.md#field) $k$ consists of elements $a+b\varepsilon$ with $\varepsilon^2=0$. The element $\varepsilon$ is a nonzero [nilpotent element](#nilpotent); its ideal is the ring's only [prime ideal](#prime-ideal). Hence its [affine scheme](ringed-space.md#affine-scheme) has the same one-point topology as $\operatorname{Spec}k$ while its [structure sheaf](ringed-space.md#structure-sheaf-of-a-scheme) differs.

##### Periodic resolution over dual numbers

↑ **Parent:** [Dual number](#dual-number)

For $A=k[\varepsilon]/(\varepsilon^2)$ and $k=A/(\varepsilon)$, the kernel and image of multiplication by $\varepsilon$ both equal $(\varepsilon)$. Thus the displayed sequence is a [free resolution](algebra.md#free-resolution). Applying $\operatorname{Hom}_A(-,k)$ makes every differential zero, so $\operatorname{Ext}_A^i(k,k)\cong k$ for every $i\ge0$. The module $k$ therefore has infinite [projective dimension](module-theory.md#projective-dimension).

#### Formal power series

↑ **Parent:** [Commutative ring](#commutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_power_series)

The [formal power series ring](#formal-power-series) $R[[T]]$ consists of all expressions $\sum_{n\geq0}a_nT^n$ with $a_n\in R$. Addition is coefficientwise, while multiplication uses the [Cauchy product](real-analysis.md#cauchy-product); no analytic convergence is required.

##### Noetherianity of formal power series rings

↑ **Parent:** [Formal power series](#formal-power-series)

For a commutative [Noetherian ring](algebra.md#noetherian-ring), the ideals of lowest possible coefficients of an ideal in $R[[X]]$ form an ascending chain. Choose lifts of finite generating sets through the stabilization degree. Successive coefficient cancellation expresses any series in the ideal using these finitely many lifts. The multiplier series converge coefficientwise, so this generates the actual ideal without first assuming it is closed. Iterating gives the result for finitely many variables.

##### Topologies on integral formal power series

↑ **Parent:** [Formal power series](#formal-power-series)

The [formal power series ring](#formal-power-series) $R=\mathbb Z_p[[T]]$ is complete for two useful [topologies](topology.md). In the $p$-adic topology, convergence means that all coefficient errors are uniformly divisible by arbitrarily large powers of $p$. In the $(p,T)$-adic topology, only finitely many coefficients are controlled at each precision. The latter topology is compact, since $R/(p,T)^n$ is finite and $R$ is its [inverse limit](module-theory.md#inverse-limit). The former is finer and is not compact: the series $T^n$ converge to zero in the latter but remain pairwise separated modulo $p$ in the former. [Coleman norm contraction](algebraic-number-theory.md#coleman-norm-contraction) uses the former; compact interpolation arguments use the latter.

##### Compositional inverse of a formal power series

↑ **Parent:** [Formal power series](#formal-power-series)

A [formal power series](#formal-power-series) with zero constant coefficient has a compositional inverse over $R$ exactly when its linear coefficient is a unit. Starting with $b_1=a_1^{-1}$, the degree-$k$ coefficient of $f(b_1T+\cdots+b_kT^k)$ is $a_1b_k$ plus an expression already determined by lower coefficients, so recursion gives a unique inverse. For a homomorphism of [formal group laws](normalization-of-an-algebraic-curve.md#formal-group-law), cancellation in the homomorphism identity proves that this inverse is also a formal-group homomorphism.

###### Recursive construction of a compositional inverse

↑ **Parent:** [Compositional inverse of a formal power series](#compositional-inverse-of-a-formal-power-series)

Let $R$ be a commutative unital [ring](#ring) and $f(T)=a_1T+a_2T^2+\cdots$ with $a_1$ a [unit](algebra.md#unit-in-a-ring). Set $g(T)=\sum_{n\ge1}b_nT^n$. The coefficient of $T$ in $f(g(T))$ gives $b_1=a_1^{-1}$. At every degree $n>1$, the coefficient is $a_1b_n$ plus an expression involving only $b_1,\ldots,b_{n-1}$; choose $b_n$ to cancel that expression. This gives a unique right [compositional inverse of a formal power series](#compositional-inverse-of-a-formal-power-series).

Similarly, the coefficient of $T^n$ in $h(f(T))$ is $a_1^n h_n$ plus previously fixed terms, so the same recursion gives a left inverse $h$. Composition of zero-constant-term [formal power series](#formal-power-series) is associative, since every coefficient involves finitely many terms. Therefore $h=h\circ(f\circ g)=(h\circ f)\circ g=g$, proving $f\circ g=g\circ f=T$.

##### Formal power series over a local ring

↑ **Parent:** [Formal power series](#formal-power-series)

If $(A,\mathfrak m)$ is a [local ring](#local-ring), then $B=A[[x]]$ is local with [maximal ideal](#maximal-ideal) $I=\mathfrak mB+xB$ and [residue field](#residue-field) $A/\mathfrak m$. A series $f=\sum a_nx^n$ is a [unit](algebra.md#unit-in-a-ring) if and only if $a_0$ is a [unit](algebra.md#unit-in-a-ring). Necessity follows by taking constant coefficients of an inverse; sufficiency follows from the recursion $b_0=a_0^{-1}$ and $b_n=-a_0^{-1}\sum_{i=1}^na_ib_{n-i}$ for its inverse. Thus the nonunits are precisely series with $a_0\in\mathfrak m$, which is exactly $I$, since $f=a_0+xg$. The constant-coefficient map followed by reduction modulo $\mathfrak m$ has [kernel](linear-algebra.md#kernel-of-a-linear-map) $I$ and image $A/\mathfrak m$.

###### Cotangent space of a formal power series ring

↑ **Parent:** [Formal power series over a local ring](#formal-power-series-over-a-local-ring)

For a [local ring](#local-ring) $(A,\mathfrak m)$ with [residue field](#residue-field) $k$, put $B=A[[x]]$ and $I=\mathfrak mB+xB$. There is a natural $k$-[vector space](vector-space.md) [isomorphism](algebra.md#isomorphism) $I/I^2\cong(\mathfrak m/\mathfrak m^2)\oplus k$. The inverse sends $(\bar a,\bar b)$ to the class of $a+bx$. It is well-defined because changing $a$ by $\mathfrak m^2$ or $b$ by $\mathfrak m$ changes the result by $I^2$. It is [surjective](algebra.md#surjective-function) since every $f\in I$ is congruent modulo $x^2B\subseteq I^2$ to its constant and linear terms. As $I^2=\mathfrak m^2B+x\mathfrak mB+x^2B$, those coefficients of an element of $I^2$ lie in $\mathfrak m^2$ and $\mathfrak m$, respectively. This proves injectivity. Thus adjoining one formal variable increases finite [embedding dimension](#embedding-dimension) by one.

##### Reducedness of a formal power series ring

↑ **Parent:** [Formal power series](#formal-power-series)

A [formal power series ring](#formal-power-series) is a [reduced ring](#reduced-ring) if and only if its coefficient ring is reduced. A nonzero constant nilpotent proves one direction. In the other direction, a nonzero series with first nonzero coefficient $a_r$ has first coefficient $a_r^m$ in its $m$th power; this is nonzero over a [reduced ring](#reduced-ring).

##### Formal power series module

↑ **Parent:** [Formal power series](#formal-power-series)

For a [vector space](vector-space.md) $M$ over a [field](algebra.md#field) $k$, its formal power series module is $M[[t]]=\varprojlim_n M\otimes_k k[t]/(t^n)$. It is complete for the filtration by $t^nM[[t]]$. The ordinary [tensor product](linear-algebra.md#tensor-product) $M\otimes_k k[[t]]$ embeds in it and consists of series whose coefficients span a finite-dimensional [vector subspace](vector-space.md#vector-subspace); it equals $M[[t]]$ if $M$ is finite-dimensional. The inclusion is proper for infinite-dimensional $M$, as shown by a series with linearly independent coefficients.

##### Noetherianity of a formal power series ring

↑ **Parent:** [Formal power series](#formal-power-series)

A [formal power series ring](#formal-power-series) $R[[x]]$ is [Noetherian](algebra.md#noetherian-ring) if and only if $R$ is [Noetherian](algebra.md#noetherian-ring). In the forward direction, use the [quotient ring](#quotient-ring) $R[[x]]/(x)\cong R$. In the reverse direction, for an [ideal](#ideal) $I$ consider the ascending sequence of [ideals](#ideal) of $R$ formed by the coefficient of $x^n$ in $I\cap x^nR[[x]]$. Stabilization and finite generation give a finite list of series that generate $I$ by successive coefficient cancellation.

###### Coefficient ideals of a formal power series ideal

↑ **Parent:** [Noetherianity of a formal power series ring](#noetherianity-of-a-formal-power-series-ring)

For an [ideal](#ideal) $H\subseteq R[[X]]$, let $A_n$ consist of coefficients of $X^n$ in members of $H$ with all lower coefficients zero. These are [ideals](#ideal) of $R$ and $A_n\subseteq A_{n+1}$, by multiplication by $X$. If $R$ is [Noetherian](algebra.md#noetherian-ring), this chain stabilizes. Choose series whose leading coefficients generate the finitely many distinct coefficient [ideals](#ideal), then cancel coefficients successively. The accumulated multipliers are [formal power series](#formal-power-series), giving an ordinary finite [ideal](#ideal) generating set for $H$, rather than merely a dense subideal.

##### Ordinary generating function

↑ **Parent:** [Formal power series](#formal-power-series)

This is the power-series specialization of a [generating function](real-analysis.md#generating-function).

The ordinary generating function of a sequence $(a_n)_{n\geq0}$ is the [formal power series](#formal-power-series) $A(z)=\sum_{n\geq0}a_nz^n$. Algebraic identities for $A$ encode recurrences and counting constructions for the coefficients.

#### Reduced ring

↑ **Parent:** [Commutative ring](#commutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_ring)

A reduced ring is a [commutative ring](#commutative-ring) with no nonzero [nilpotent element](#nilpotent). Equivalently, its [nilradical](#nilradical) is zero.

##### Reducedness is detected by prime localizations

↑ **Parent:** [Reduced ring](#reduced-ring)

If a nonzero [nilpotent element](#nilpotent) $a$ existed in $A$, its proper [annihilator](module-theory.md#annihilator-ring-theory) would lie in a [maximal ideal](#maximal-ideal) $\mathfrak m$. No element outside $\mathfrak m$ annihilates $a$, so $a/1$ is nonzero in the [localization at a prime ideal](#localization-at-a-prime-ideal) $A_{\mathfrak m}$. Conversely, if $(a/s)^n=0$ in a localization, some $u$ in the [multiplicative subset](#multiplicatively-closed-set) satisfies $ua^n=0$. Then $(ua)^n=0$, so reducedness of $A$ gives $ua=0$ and hence $a/s=0$.

### Graded ring

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graded_ring)

A graded ring is a direct sum $R=\bigoplus_{n\geq0}R_n$ with $R_mR_n\subseteq R_{m+n}$.

#### Graded module

↑ **Parent:** [Graded ring](#graded-ring)

A graded module over a [graded ring](#graded-ring) $R=\bigoplus_iR_i$ is an $R$-[module](module-theory.md#module-mathematics) with a [direct sum](vector-space.md#direct-sum) decomposition $M=\bigoplus_dM_d$ satisfying $R_iM_d\subseteq M_{i+d}$. A graded homomorphism preserves these degrees. Over a [polynomial ring](#polynomial-ring) with positive variable degrees, a [finitely generated module](module-theory.md#finitely-generated-module) of this kind is bounded below and has finite-dimensional graded components over the coefficient [field](algebra.md#field).

##### Super vector space

↑ **Parent:** [Graded module](#graded-module)

A super vector space is a [vector space](vector-space.md) graded by the two-element group. Degree-preserving maps and the usual graded tensor product form a [monoidal category](category-theory.md#monoidal-category). Over a field of characteristic different from two, this category has two different symmetries: ordinary interchange of tensor factors and interchange multiplied by $(-1)^{pq}$ on homogeneous factors of degrees $p,q$. The latter is the [Koszul sign rule](homology.md#koszul-sign-rule).

##### Degree-one localization of a graded module

↑ **Parent:** [Graded module](#graded-module)

If $f$ is homogeneous of degree one, multiplication by powers of the invertible element $f$ identifies every homogeneous component of $M_f$ with $(M_f)_0$. A homogeneous element $m$ of degree $a$ is written $f^a(f^{-a}m)$. Thus the displayed map is an isomorphism of [graded modules](#graded-module). In particular, the degree-zero part of a tensor product of localized graded modules is the tensor product of their degree-zero parts over $(S_f)_0$. This proves [tensor compatibility of graded sheafification on degree-one-generated Proj](ringed-space.md#tensor-compatibility-of-graded-sheafification-on-degree-one-generated-proj).

##### Graded shift

↑ **Parent:** [Graded module](#graded-module)

The graded shift $M(-a)$ is the same underlying [module](module-theory.md#module-mathematics) with $M(-a)_d=M_{d-a}$. Thus $S(-a)$ has a free generator in degree $a$. Its [Hilbert series](#hilbert-series) is $t^aH_M(t)$, and multiplication by a homogeneous element of degree $a$ becomes a degree-preserving map $M(-a)\to M$.

#### Graded algebra

↑ **Parent:** [Graded ring](#graded-ring)

A graded algebra over a field $k$ is a $k$-algebra $A=\bigoplus_{n\geq0}A_n$ whose multiplication satisfies $A_iA_j\subseteq A_{i+j}$.

##### Indecomposable quotient of an augmented algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

For an augmented graded algebra $A$, its positive augmentation ideal $A^+$ has indecomposable quotient $Q(A)=A^+/(A^+)^2$. For a [Sullivan minimal model](algebraic-topology.md#sullivan-minimal-model) $(\Lambda V,d)$, this quotient is $V$ with zero differential because every $dv$ is decomposable. The map $H^+(\Lambda V,d)\to V$ induced by projection is dual to the rational [Hurewicz homomorphism](algebraic-topology.md#hurewicz-homomorphism) under the finite-type model identification.

##### Graded tensor product

↑ **Parent:** [Graded algebra](#graded-algebra)

The tensor product of graded algebras uses the displayed multiplication, incorporating the sign for interchanging homogeneous factors. This is the algebra structure in the cohomological [Künneth theorem](cohomology.md#kunneth-theorem), and explains the signs of mixed intersection products on product manifolds.

##### Graded commutator

↑ **Parent:** [Graded algebra](#graded-algebra)

The bracket of homogeneous elements in a parity-graded associative algebra. It is a commutator if at least one element is even and an [anticommutator](vector-space.md#anticommutator) if both are odd. This is the natural bracket for the action of an odd [BRST charge](relativistic-quantum-field.md#brst-charge) on quantum operators.

##### Differential graded algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

A graded algebra equipped with a degree-one differential satisfying $d(ab)=d(a)b+(-1)^{|a|}a\,d(b)$ and $d^2=0$. Its [cohomology](cohomology.md) inherits a graded algebra structure. In rational [homotopy](algebraic-topology.md#homotopy), a [Sullivan minimal model](algebraic-topology.md#sullivan-minimal-model) is a free graded-commutative differential graded algebra with decomposable generator differentials.

###### Commutative differential graded algebra

↑ **Parent:** [Differential graded algebra](#differential-graded-algebra)

A commutative [differential graded algebra](#differential-graded-algebra) has multiplication $ab=(-1)^{|a||b|}ba$ and a degree-one differential with $d^2=0$ and $d(ab)=d(a)b+(-1)^{|a|}a\,d(b)$. Over $\mathbb Q$, its free algebra on graded generators is polynomial on even-degree generators and exterior on odd-degree generators. Rational [rational polynomial differential forms](algebraic-topology.md#rational-polynomial-differential-forms) on a space supply such an algebra, modelled up to [quasi-isomorphism](homology.md#quasi-isomorphism) by a [Sullivan minimal model](algebraic-topology.md#sullivan-minimal-model).

##### Divided power algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

For an even-degree generator, take a free graded $R$-module with basis $a_k$, $k\geq0$, and multiplication $a_i a_j=\binom{i+j}{i}a_{i+j}$, with $a_0=1$ and $|a_k|=k|a|$. Associativity follows from the multinomial identity. Over $\mathbb Z$, $a_1^k=k!a_k$, so the algebra need not be polynomial on $a_1$.

##### Graded derivation

↑ **Parent:** [Graded algebra](#graded-algebra)

An odd graded derivation satisfies $Q(ab)=(Qa)b+(-1)^{|a|}a(Qb)$ for homogeneous $a$. Its square is an even derivation; consequently checking $Q^2=0$ on algebra generators establishes nilpotence everywhere.

##### Graded commutative algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

A [graded algebra](#graded-algebra) is a graded commutative algebra if $uv=(-1)^{pq}vu$ for [homogeneous elements of a graded algebra](#homogeneous-element-of-a-graded-algebra) of degrees $p,q$. In [characteristic](algebra.md#characteristic-of-a-field) not equal to two, every odd-degree element then squares to zero. The [exterior algebra](linear-algebra.md#exterior-algebra) and [Hochschild cohomology](associative-algebra.md#hochschild-cohomology) with the [Hochschild cup product](associative-algebra.md#hochschild-cup-product) are examples.

###### Graded symmetric algebra

↑ **Parent:** [Graded commutative algebra](#graded-commutative-algebra)

For a graded vector space $V$, $\operatorname{Sym}(V)$ is the quotient of the tensor algebra by $uv-(-1)^{|u||v|}vu$. Over $\mathbb Q$ it is polynomial on even-degree basis elements and exterior on odd-degree ones. With each generator primitive, it is a graded cocommutative Hopf algebra. Its primitive subspace is exactly $V$: applying the diagonal to a polynomial of symmetric length greater than one produces mixed terms, or equivalently the polynomial's formal derivatives cannot all vanish in characteristic zero. This is the associated graded algebra in the [graded Poincaré–Birkhoff–Witt theorem](lie-algebra.md#graded-poincare-birkhoff-witt-theorem).

##### Homogeneous element of a graded algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

An element of a single graded component $A_n$ of a [graded algebra](#graded-algebra) is homogeneous of degree $n$. The degree sign rules for an [exterior product](linear-algebra.md#exterior-product) or a [graded Lie bracket](lie-algebra.md#graded-lie-bracket) apply first to homogeneous elements, then extend by [linearity](vector-space.md#linearity).

##### Gerstenhaber algebra

↑ **Parent:** [Graded algebra](#graded-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gerstenhaber_algebra)

A Gerstenhaber algebra has an associative product making it a [graded commutative algebra](#graded-commutative-algebra) and a degree-minus-one [graded Lie bracket](lie-algebra.md#graded-lie-bracket). In the left convention, $[u,vw]=[u,v]w+(-1)^{(|u|-1)|v|}v[u,w]$. The shifted degrees $|u|-1$ determine the signs of antisymmetry and the [Jacobi identity](lie-algebra.md#jacobi-identity). [Hochschild cohomology](associative-algebra.md#hochschild-cohomology) and the [exterior algebra](linear-algebra.md#exterior-algebra) of polynomial [derivations](associative-algebra.md#derivation-of-an-algebra) are examples.

##### Graded Leibniz rule

↑ **Parent:** [Graded algebra](#graded-algebra)

On a [graded algebra](#graded-algebra), a left derivation of degree $r$ satisfies the displayed rule for homogeneous $a$. A right derivation of degree $r$ satisfies $R(ab)=aR(b)+(-1)^{r|b|}R(a)b$. For odd $r$, these reduce to the familiar parity sign rules. The left [Gerstenhaber bracket](associative-algebra.md#gerstenhaber-bracket) makes $[u,-]$ a left derivation of degree $|u|-1$ on [Hochschild cohomology](associative-algebra.md#hochschild-cohomology); this rule holds for the induced [cohomology](cohomology.md) operations, not necessarily for their cochain representatives.

##### Standard graded algebra

↑ **Parent:** [Graded algebra](#graded-algebra)

A standard graded algebra over a field $k$ has $A_0=k$ and is generated as a $k$-algebra by finitely many elements of degree one. Its Hilbert function agrees eventually with a polynomial.

#### Associated graded ring

↑ **Parent:** [Graded ring](#graded-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Associated_graded_ring)

For an ideal $I$, the associated graded ring is

$$
\operatorname{gr}_I(R)=\bigoplus_{n\ge0}I^n/I^{n+1}.
$$

##### Associated graded module

↑ **Parent:** [Associated graded ring](#associated-graded-ring)

For an increasing [filtration of a module](module-theory.md#filtration-of-a-module) $M_n$ compatible with a [filtered algebra](module-theory.md#filtered-algebra) $A$, set $\operatorname{gr}M=\bigoplus_n M_n/M_{n-1}$. Multiplication on the quotients makes it a graded [module](module-theory.md#module-mathematics) over $\operatorname{gr}A$. Its cumulative homogeneous dimensions equal $\dim M_n$ for a finite-dimensional exhaustive nonnegative [filtration of a module](module-theory.md#filtration-of-a-module).

###### Exactness of associated graded modules for induced filtrations

↑ **Parent:** [Associated graded module](#associated-graded-module)

Give $N$ the [subspace filtration](module-theory.md#subspace-filtration) and $M/N$ the [quotient filtration](module-theory.md#quotient-filtration). If the degree-$i$ class of $m\in F_iM$ maps to zero, then $m=n+m'$ with $n\in N$ and $m'\in F_{i-1}M$. Thus $n\in N\cap F_iM$ and the class comes from $\operatorname{gr}N$. Inclusion is [injective](algebra.md#injective-function) in every degree and the quotient map is [surjective](algebra.md#surjective-function), proving the displayed [short exact sequence](module-theory.md#short-exact-sequence) of [associated graded modules](#associated-graded-module). Exactness can fail for arbitrarily chosen incompatible filtrations.

##### Pole dimension of an associated graded ring

↑ **Parent:** [Associated graded ring](#associated-graded-ring)

For a Noetherian local ring $(A,\mathfrak m)$, the pole dimension $d(\operatorname{gr}_{\mathfrak m}(A))$ is the order of the pole at $t=1$ of

$$
\sum_{n\geq0}\dim_{A/\mathfrak m}(\mathfrak m^n/\mathfrak m^{n+1})t^n.
$$

The Hilbert-Serre theorem makes this series rational, so the order is defined.

##### Hilbert-Samuel polynomial

↑ **Parent:** [Associated graded ring](#associated-graded-ring)

For an $\mathfrak m$-primary ideal $I$ in a Noetherian local ring, $\operatorname{length}(R/I^n)$ agrees for all sufficiently large $n$ with the Hilbert-Samuel polynomial of $I$.

<h6 id="hilbert-samuel-growth-dimension">Hilbert–Samuel growth dimension</h6>

↑ **Parent:** [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial)

For a [Noetherian local ring](algebra.md#noetherian-local-ring) $(R,\mathfrak m)$, let $H_R(t)=\operatorname{length}(R/\mathfrak m^t)$. Its eventual [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial) has degree $d(R)$, equivalently the pole order at $1$ of the [Hilbert series](#hilbert-series) of $\operatorname{gr}_{\mathfrak m}R$. This is the local length-growth invariant, not the [embedding dimension](#embedding-dimension). The [prime-chain lower bound for local length](#prime-chain-lower-bound-for-local-length) proves $\dim R\leq d(R)$; the full local dimension theorem gives equality.

###### Prime-chain lower bound for local length

↑ **Parent:** [Hilbert–Samuel growth dimension](#hilbert-samuel-growth-dimension)

A [prime chain](#prime-chain) of length $s$ in a [Noetherian local ring](algebra.md#noetherian-local-ring) forces its maximal-[ideal](#ideal) length function to be at least $ct^s$ for large $t$. Quotient by the initial prime to reduce to a domain, choose a nonzero $a$ in the next prime, and use the [Artin-Rees lemma](module-theory.md#artin-rees-lemma) to obtain $H_R(t)\geq H_R(t-c_0)+H_{R/(a)}(t)$. Induction on chain length and summing about $t/(2c_0)$ terms prove the bound. This yields $\dim R\leq d(R)$ without assuming the [Krull height theorem](#krull-height-theorem).

<h6 id="hilbert-samuel-function">Hilbert–Samuel function</h6>

↑ **Parent:** [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert–Samuel_function)

For an [ideal of definition](algebra.md#ideal-of-definition) $I$ of a [Noetherian local ring](algebra.md#noetherian-local-ring) and a [finitely generated module](module-theory.md#finitely-generated-module) $M$, the Hilbert–Samuel function is

$$
\chi(M,I;n)=\operatorname{length}(M/I^nM).
$$

For sufficiently large $n$, it equals the [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial).

<h6 id="hilbert-samuel-multiplicity">Hilbert–Samuel multiplicity</h6>

↑ **Parent:** [Hilbert–Samuel function](#hilbert-samuel-function)

If $M$ has [Krull dimension](#krull-dimension) $d$, the coefficient of $n^d$ in its [Hilbert-Samuel polynomial](#hilbert-samuel-polynomial) is $e_I(M)/d!$. The positive integer $e_I(M)$ is the Hilbert–Samuel multiplicity of $M$ with respect to $I$.

#### Hilbert series and Hilbert polynomial

↑ **Parent:** [Graded ring](#graded-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_series_and_Hilbert_polynomial)

For a finitely generated graded module over a standard graded algebra over a [field](algebra.md#field), with finite-dimensional graded pieces, the [Hilbert function](#hilbert-function) $h(n)=\dim M_n$ is eventually a polynomial in $n$. Its generating series is the [Hilbert series](#hilbert-series). Thus the polynomial describes eventual graded growth, while the series records all graded pieces.

##### Hilbert series

↑ **Parent:** [Hilbert series and Hilbert polynomial](#hilbert-series-and-hilbert-polynomial)

For a graded module $M=\bigoplus_{n\ge0}M_n$ whose pieces have finite length, its Hilbert series is

$$
H_M(z)=\sum_{n\ge0}\operatorname{length}(M_n)z^n.
$$

###### Hilbert function

↑ **Parent:** [Hilbert series](#hilbert-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_function)

The Hilbert function of a graded module $M=\bigoplus_nM_n$ over a field is $n\mapsto\dim_kM_n$. Its generating function is the [Hilbert series](#hilbert-series).

###### Quasipolynomial

↑ **Parent:** [Hilbert function](#hilbert-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasipolynomial)

A quasipolynomial is a function $f:\mathbb Z\to\mathbb C$ for which there are [polynomials](polynomial.md) $P_0,\ldots,P_{m-1}$ such that $f(n)=P_r(n)$ whenever $n\equiv r\pmod m$. The least possible positive $m$ is its period.

###### Hilbert-Serre theorem

↑ **Parent:** [Hilbert series](#hilbert-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert-Serre_theorem)

Let $S=k[x_1,\ldots,x_r]$ be graded with positive degrees $d_i=\deg x_i$, and let $M$ be a finitely generated graded $S$-module with finite-dimensional graded pieces. Then

$$
H_M(t)=\frac{P(t)}{\prod_{i=1}^r(1-t^{d_i})}
$$

for a Laurent polynomial $P(t)\in\mathbb Z[t,t^{-1}]$. For a standard grading, $\dim_kM_n$ consequently agrees with a polynomial for all sufficiently large $n$.

The proof is by induction on $r$. For $x=x_r$ of degree $d$, the exact sequence of graded modules

$$
0\longrightarrow(0:_Mx)(-d)\longrightarrow M(-d)
\xrightarrow{x}M\longrightarrow M/xM\longrightarrow0
$$

gives

$$
(1-t^d)H_M(t)=H_{M/xM}(t)-t^dH_{(0:_Mx)}(t).
$$

Both modules on the right are finitely generated over $k[x_1,\ldots,x_{r-1}]$, so induction supplies the asserted denominator.

###### Hilbert-Serre theorem for an additive coefficient function

↑ **Parent:** [Hilbert-Serre theorem](#hilbert-serre-theorem)

Let $S_0$ be a commutative [Noetherian ring](algebra.md#noetherian-ring), let a graded $S$ be generated over it by finitely many positive-degree homogeneous elements, and let $M$ be a finitely generated [graded module](#graded-module). For an integer-valued function $\lambda$ additive on exact sequences of finitely generated $S_0$-modules, its graded-piece series has the displayed form. The exact sequence for multiplication by the last variable gives $(1-t^d)P_M=P_{M/xM}-t^dP_{(0:_Mx)}$. Those two [modules](module-theory.md#module-mathematics) are finite over the [ring](#ring) with one fewer variable, and induction proves rationality. Finite graded pieces and the finite-generation assumptions cannot simply be omitted.

###### Hilbert series multiplication exact sequence

↑ **Parent:** [Hilbert-Serre theorem](#hilbert-serre-theorem)

For a homogeneous element $x$ of degree $e>0$ acting on a finite [graded module](#graded-module), set $N=(0:_Mx)$ and $C=M/xM$. The multiplication exact sequence $0\to N(-e)\to M(-e)\to M\to C\to0$ and additivity of component lengths give $(1-t^e)P_M=P_C-t^eP_N$. This is the inductive step in the [Hilbert-Serre theorem](#hilbert-serre-theorem); the [annihilator](module-theory.md#annihilator-ring-theory) term must be kept unless multiplication by $x$ is injective.

###### Growth of a finitely generated commutative algebra

↑ **Parent:** [Hilbert-Serre theorem](#hilbert-serre-theorem)

Let a commutative $k$-algebra $R$ be generated by $x_1,\ldots,x_n$, and let $R_j$ be the span of words of total degree at most $j$ in those generators. The [associated graded ring](#associated-graded-ring) of this filtration is a [standard graded algebra](#standard-graded-algebra), and

$$
\dim_kR_j=\sum_{i=0}^j\dim_k(R_i/R_{i-1}).
$$

The [Hilbert-Serre theorem](#hilbert-serre-theorem) therefore makes $\dim_kR_j$ eventually a polynomial in $j$. Its degree is $\dim R$; this follows by applying the Rees-ring deformation, whose special fibers are $R$ and the associated graded ring, so they have the same [Krull dimension](#krull-dimension).

###### Growth of the two-variable Laurent polynomial algebra

↑ **Parent:** [Growth of a finitely generated commutative algebra](#growth-of-a-finitely-generated-commutative-algebra)

For

$$
R=k[Y_1,Y_1^{-1},Y_2,Y_2^{-1}]
$$

with the four displayed generators, $R_j$ has basis $Y_1^aY_2^b$ with $|a|+|b|\leq j$. The number of integer lattice points in this diamond is

$$
1+4\sum_{r=1}^jr=2j^2+2j+1.
$$

Its quadratic growth agrees with $\dim R=2$.

###### Poincare series of a graded module

↑ **Parent:** [Hilbert series](#hilbert-series)

For a chosen additive function such as module length, the Poincare series of a graded module is the generating function of that function on its homogeneous components. In this usage it is a Hilbert series.

### Ideal

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_(ring_theory))

An ideal is an additive subgroup of a [ring](#ring) that absorbs multiplication by ring elements.

#### Monomial ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monomial_ideal)

An [ideal](#ideal) in a [polynomial ring](#polynomial-ring) generated by [monomials](polynomial.md#monomial). Its exponent vectors form an upward-closed subset of $\mathbb N^r$ under the componentwise order. The [Dickson lemma](combinatorics.md#dickson-s-lemma) makes the minimal exponent set finite. This description permits [Maclagan's theorem](#reverse-inclusion-well-quasi-ordering-of-monomial-ideals) to compare ideals by reverse inclusion independently of the coefficient field.

##### Reverse-inclusion well-quasi-ordering of monomial ideals

↑ **Parent:** [Monomial ideal](#monomial-ideal)

Upward-closed subsets of $\mathbb N^r$, including the empty subset, form a [well-quasi-ordering](set.md#well-quasi-ordering) by reverse inclusion. For $r=1$, tails correspond to the well-order $\mathbb N\cup\{\infty\}$. Inductively slice in the last coordinate. The slices increase and eventually stabilize: their union has a finite minimal basis by the [Dickson lemma](combinatorics.md#dickson-s-lemma), all of which has appeared in one finite slice. Encode an upset by the word of its pre-stabilization slices and its final slice. The [Higman lemma](set.md#higman-s-lemma) and [finite product closure of well-quasi-orderings](set.md#finite-product-closure-of-well-quasi-orderings) compare these encodings in the reverse-inclusion slice order. A subsequence map $f$ has $f(k)\ge k$, so containment of the matched later slice implies containment of the slice at $k$; the final-slice comparison handles the tail. The entire earlier upset therefore contains the later upset.

#### Pure ideal

↑ **Parent:** [Ideal](#ideal)

An [ideal](#ideal) $I$ is pure when the quotient is a [flat module](module-theory.md#flat-module). Equivalently every $a\in I$ satisfies $a=ab$ for some $b\in I$. The latter condition makes $I$ vanish after localizing at primes containing it, while at primes not containing it the quotient is zero. Pure ideals need not be finitely generated. They describe [flat morphisms](ringed-space.md#flat-morphism) that are [closed immersions](ringed-space.md#closed-immersion) on affine charts.

#### Zero ideal

↑ **Parent:** [Ideal](#ideal)

The [ideal](#ideal) consisting only of zero. It is the [principal ideal](#principal-ideal) generated by zero.

#### Ideal quotient

↑ **Parent:** [Ideal](#ideal)

For [ideals](#ideal) $I,J$ in a commutative [ring](#ring), the ideal quotient is $(I:J)=\{r\in R:rJ\subseteq I\}$. Closure under subtraction and multiplication by arbitrary ring elements proves it is an [ideal](#ideal). If $I\subseteq J=(a)$, then $I=a(I:J)$: write $x=ar\in I$ and observe that $rJ=xR\subseteq I$. Consequently, if also $(I:J)=(b)$, then $I=(ab)$ is a [principal ideal](#principal-ideal).

#### Unit ideal

↑ **Parent:** [Ideal](#ideal)

The whole [ring](#ring) $R$, viewed as an [ideal](#ideal). Elements $f_1,\dots,f_r$ generate the [unit ideal](#unit-ideal) exactly when coefficients $g_i\in R$ give $\sum_i g_if_i=1$.

##### Unit-ideal identity for powers

↑ **Parent:** [Unit ideal](#unit-ideal)

If $\sum_i g_if_i=1$, expand its power $r(N-1)+1$. By the [pigeonhole principle](algebra.md#pigeonhole-principle), each monomial contains some $f_i^N$. Collecting terms expresses $1$ as a [linear combination](vector-space.md#linear-combination) of these powers. This lets one use a common denominator exponent in [localization](#localization-of-a-ring) arguments.

#### Union of three incomparable nonprime ideals

↑ **Parent:** [Ideal](#ideal)

In $\mathbb F_2[u,v]/(u,v)^2$, the [ideals](#ideal) $(u)$, $(v)$ and $(u+v)$ are pairwise incomparable and nonprime. Their union is the [ideal](#ideal) $(u,v)$: the three lines cover its two-dimensional [vector space](vector-space.md) over $\mathbb F_2$. This shows why a primality hypothesis matters in [prime avoidance](#prime-avoidance).

#### Conormal module

↑ **Parent:** [Ideal](#ideal)

For an [ideal](#ideal) $I\subseteq R$, its conormal module is $I/I^2$, naturally an $R/I$-[module](module-theory.md#module-mathematics). It records generators and relations to first order along the quotient $R/I$. If $I$ is the [maximal ideal](#maximal-ideal) of a [local ring](#local-ring), it is the [cotangent space of a local ring](#cotangent-space-of-a-local-ring) over the [residue field](#residue-field). For the augmentation ideal $(X_1-1,\ldots,X_r-1)$ of $A[X_1^{\pm1},\ldots,X_r^{\pm1}]$, reduction modulo $I^2$ gives $I/I^2\cong A^r$, with basis the classes of $X_i-1$.

#### Irreducible ideal

↑ **Parent:** [Ideal](#ideal)

A proper [ideal](#ideal) $I$ is irreducible if $I=J\cap K$ implies $I=J$ or $I=K$. In a [Noetherian ring](algebra.md#noetherian-ring), every irreducible ideal is a [primary ideal](#primary-ideal); every proper [ideal](#ideal) is a finite intersection of irreducible ideals.

##### Irreducible ideals are primary in Noetherian rings

↑ **Parent:** [Irreducible ideal](#irreducible-ideal)

In a [Noetherian ring](algebra.md#noetherian-ring), an [irreducible ideal](#irreducible-ideal) is a [primary ideal](#primary-ideal). In its quotient, if $xy=0$ and $x\ne0$, choose $r$ after the [annihilators](module-theory.md#annihilator-ring-theory) of powers of $y$ stabilize. Then $(x)\cap(y^r)=0$, so irreducibility forces $y^r=0$. Combined with finite decomposition into irreducible ideals, this proves the [Lasker–Noether theorem](module-theory.md#lasker-noether-theorem).

#### Radical ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radical_ideal)

An ideal $I$ is radical when $f^m\in I$ for some positive integer $m$ implies $f\in I$. Over an algebraically closed field, the [Hilbert Nullstellensatz](algebraic-geometry.md#hilbert-nullstellensatz) identifies the vanishing ideal of $V(I)$ with the radical $\sqrt I$.

#### Colon ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colon_ideal)

For an ideal $I$ and an element $a$ of a commutative ring,

$$
(I:a)=\{x:xa\in I\}.
$$

#### Nilpotent ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_ideal)

An ideal $I$ is nilpotent when $I^r=0$ for some positive integer $r$.

##### Nilpotence index of an ideal

↑ **Parent:** [Nilpotent ideal](#nilpotent-ideal)

For a [nilpotent ideal](#nilpotent-ideal) $I$, its [nilpotence index of an ideal](#nilpotence-index-of-an-ideal) is the least positive integer $n$ for which $I^n=0$. In $k[X]/(g^e)$, with $g$ an [irreducible polynomial](polynomial.md#irreducible-polynomial), the unique [maximal ideal](#maximal-ideal) $(g)$ has index $e$. In a [discrete valuation ring](#discrete-valuation-ring) with $p=u\pi^e$, the [maximal ideal](#maximal-ideal) of its reduction modulo $p$ has the same index. Comparing these indices under a [quotient ring](#quotient-ring) isomorphism recovers the ramification exponent in the [Kummer-Dedekind theorem](algebraic-number-theory.md#kummer-dedekind-theorem).

#### Oka family

↑ **Parent:** [Ideal](#ideal)

An Oka family of ideals is a family $\mathcal G$ such that $I+(a)\in\mathcal G$ and $(I:a)\in\mathcal G$ imply $I\in\mathcal G$.

##### Prime ideal principle for an Oka family

↑ **Parent:** [Oka family](#oka-family)

Every ideal maximal outside an Oka family is prime. If $xy\in I$ while $x,y\notin I$, both $I+(x)$ and $(I:x)$ properly contain $I$, contradicting the Oka condition.

#### Two-sided ideal

↑ **Parent:** [Ideal](#ideal)

A two-sided ideal $I$ of a [noncommutative ring](#noncommutative-ring) satisfies $RI\subseteq I$ and $IR\subseteq I$.

##### Square-zero ideal

↑ **Parent:** [Two-sided ideal](#two-sided-ideal)

A square-zero ideal is an [ideal](#ideal) $I$ satisfying $I^2=0$, so every product of two elements of $I$ vanishes.

###### Square-zero extension of an algebra

↑ **Parent:** [Square-zero ideal](#square-zero-ideal)

For a unital [associative algebra](associative-algebra.md) $A$ and prescribed $A$-[bimodule](module-theory.md#bimodule) $M$, an extension is $0\to M\to E\to A\to0$ where $E$ is unital, $E\to A$ is unital, $M$ is a [square-zero ideal](#square-zero-ideal), and the induced actions are the prescribed ones. Equivalences induce the identity on $A$ and $M$. A unital linear section produces a normalized [Hochschild cocycle](associative-algebra.md#hochschild-cocycle) $\mu(a,b)=s(a)s(b)-s(ab)$. Conversely, $(a,m)(b,n)=(ab,an+mb+\mu(a,b))$ on $A\oplus M$ defines the extension. Changing section changes $\mu$ by a coboundary, giving classification by $HH^2(A,M)$.

###### Square-zero unit subgroup

↑ **Parent:** [Square-zero ideal](#square-zero-ideal)

If $I^2=0$, then $1+I=\{1+a:a\in I\}$ is an abelian subgroup of the [unit group](algebra.md#unit-group). Multiplication satisfies $(1+a)(1+b)=1+a+b$, and $(1+a)^{-1}=1-a$, so $a\mapsto1+a$ identifies the [additive group](group.md#additive-group) of $I$ with $1+I$.

#### Primary ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primary_ideal)

An ideal $I$ is primary when $ab\in I$ and $a\notin I$ imply $b^n\in I$ for some positive integer $n$.

##### Primary ideals can need more generators than the maximal ideal

↑ **Parent:** [Primary ideal](#primary-ideal)

In the [Noetherian local ring](algebra.md#noetherian-local-ring) $A=k[[u,v]]$ with [maximal ideal](#maximal-ideal) $\mathfrak m=(u,v)$, the [embedding dimension](#embedding-dimension) is two but $\mathfrak m^r$ needs $r+1$ generators for every $r\geq1$. The degree-$r$ monomials $u^r,u^{r-1}v,\ldots,v^r$ generate $\mathfrak m^r$, and their images form a [basis](vector-space.md#basis) of $\mathfrak m^r/\mathfrak m^{r+1}$, so no smaller generating list exists. These [ideals](#ideal) are $\mathfrak m$-primary: if $ab\in\mathfrak m^r$ and $a\notin\mathfrak m^r$, then $b$ cannot be a [unit](algebra.md#unit-in-a-ring); hence $b\in\mathfrak m$ and $b^r\in\mathfrak m^r$. Consequently [embedding dimension](#embedding-dimension) bounds the minimum over all maximal-primary [ideals](#ideal), because the [maximal ideal](#maximal-ideal) itself is eligible, but does not bound the number of generators of each such [ideal](#ideal).

##### Radical of a primary ideal

↑ **Parent:** [Primary ideal](#primary-ideal)

The radical $\sqrt I=\{x:x^n\in I\text{ for some }n\geq1\}$ of a primary ideal is prime. In a number ring this forces a nonzero primary ideal to have only one prime in its unique factorization.

##### Minimal primary decomposition

↑ **Parent:** [Primary ideal](#primary-ideal)

A minimal primary decomposition of an ideal $I$ is an irredundant finite intersection $I=\bigcap_iQ_i$ of primary ideals whose radicals are pairwise distinct.

###### First uniqueness theorem for primary decomposition

↑ **Parent:** [Minimal primary decomposition](#minimal-primary-decomposition)

The distinct radicals in a [minimal primary decomposition](#minimal-primary-decomposition) are exactly the [associated primes of a module](module-theory.md#associated-prime-of-a-module) $R/I$, and hence are invariant. The injection into the sum of primary quotients proves one inclusion; an element supported on one component, supplied by irredundancy, proves the other. This does not imply uniqueness of [embedded primary components](#embedded-primary-component).

###### Embedded primary component

↑ **Parent:** [Minimal primary decomposition](#minimal-primary-decomposition)

A component in a [minimal primary decomposition](#minimal-primary-decomposition) is embedded if its [radical of an ideal](#radical-of-an-ideal) strictly contains another radical occurring in that decomposition. Such components need not be unique. For example,

$$
(x^2,xy)=(x)\cap(x^2,y)=(x)\cap(x^2,y-x)
$$

in $k[x,y]$ gives different $(x,y)$-[primary ideals](#primary-ideal) as embedded components, with the same isolated component $(x)$.

###### Isolated prime of a primary decomposition

↑ **Parent:** [Minimal primary decomposition](#minimal-primary-decomposition)

An isolated prime of a minimal primary decomposition is a minimal member of the set of radicals of its primary components.

###### Second uniqueness theorem for primary decomposition

↑ **Parent:** [Minimal primary decomposition](#minimal-primary-decomposition)

In a Noetherian ring, the primary component belonging to each isolated prime $\mathfrak p$ is uniquely determined by

$$
Q(\mathfrak p)=IR_{\mathfrak p}\cap R.
$$

Embedded primary components need not be unique.

#### Generating set of an ideal

↑ **Parent:** [Ideal](#ideal)

A set $S\subseteq I$ generates an ideal $I$ when every element of $I$ is a finite sum of ring multiples of elements of $S$.

#### Principal ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_ideal)

A principal ideal is generated by one element: $(a)=\{ra:r\in R\}$.

#### Product of ideals

↑ **Parent:** [Ideal](#ideal)

The product $IJ$ consists of finite sums of products $xy$ with $x\in I$ and $y\in J$.

##### Idempotent ideal

↑ **Parent:** [Product of ideals](#product-of-ideals)

An [ideal](#ideal) $I$ is idempotent when $I^2=I$. Then $I^j=I$ for every $j\ge1$, so a nonzero idempotent ideal gives a nonzero intersection of all its powers. A [semigroup algebra](algebra.md#semigroup-algebra) with arbitrarily divisible positive exponents supplies examples in a non-Noetherian [integral domain](#integral-domain). If $I$ is finitely generated, the [determinant trick](module-theory.md#determinant-trick) applied to $I=I^2$ produces $r\in I$ such that $(1+r)I=0$.

#### Intersection of ideals

↑ **Parent:** [Ideal](#ideal)

The set-theoretic intersection of any family of ideals is again an ideal.

#### Comaximal ideals

↑ **Parent:** [Ideal](#ideal)

Ideals $I$ and $J$ are comaximal when $I+J=R$.

#### Prime-power ideal

↑ **Parent:** [Ideal](#ideal)

A prime-power ideal has the form $\mathfrak p^m$ for a [prime ideal](#prime-ideal) $\mathfrak p$ and positive integer $m$.

#### Ideal approximation theorem

↑ **Parent:** [Ideal](#ideal)

For finitely many distinct prime ideals, one can prescribe finite valuation data simultaneously by the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem).

#### Reduction modulo an ideal

↑ **Parent:** [Ideal](#ideal)

Reduction modulo an ideal $I$ is the quotient homomorphism $R\to R/I$.

##### Quotient ring

↑ **Parent:** [Reduction modulo an ideal](#reduction-modulo-an-ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_ring)

For a [two-sided ideal](#two-sided-ideal) $I$ of a [ring](#ring) $R$, the quotient $R/I$ has addition and multiplication induced from $R$.

###### Congruence modulo an ideal

↑ **Parent:** [Quotient ring](#quotient-ring)

Two elements of a [commutative ring](#commutative-ring) are congruent modulo an [ideal](#ideal) if their difference lies in that [ideal](#ideal), equivalently if their images in the [quotient ring](#quotient-ring) agree. This is an [equivalence relation](set-theory.md#equivalence-relation) compatible with [addition](arithmetic.md#addition) and [multiplication](arithmetic.md#multiplication). For $R=\mathbb Z_p[[T]]$ and $I=p^kR$, it means every coefficient difference is divisible by $p^k$.

#### Homogeneous ideal

↑ **Parent:** [Ideal](#ideal)

An [ideal](#ideal) in a [graded ring](#graded-ring) is homogeneous when it is generated by [homogeneous elements](algebra.md#homogeneous-polynomial), equivalently when every homogeneous component of each of its elements also belongs to the ideal.

#### Radical of an ideal

↑ **Parent:** [Ideal](#ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radical_of_an_ideal)

The radical of an [ideal](#ideal) $I$ is

$$
\sqrt I=\{f:f^m\in I\text{ for some }m\geq1\}.
$$

An ideal equal to its radical is a radical ideal.

##### Finite prime-intersection representation of a radical

↑ **Parent:** [Radical of an ideal](#radical-of-an-ideal)

In a [Noetherian ring](algebra.md#noetherian-ring), every [radical of an ideal](#radical-of-an-ideal) is an intersection of finitely many [prime ideals](#prime-ideal). A maximal counterexample [ideal](#ideal) $J$ cannot be prime. Choose $a,b\notin J$ with $ab\in J$; the strictly larger [ideals](#ideal) $J+(a)$ and $J+(b)$ satisfy the result, and $\sqrt J=\sqrt{J+(a)}\cap\sqrt{J+(b)}$. This contradicts maximality. The unit [ideal](#ideal) uses an empty intersection.

##### Nilradical

↑ **Parent:** [Radical of an ideal](#radical-of-an-ideal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilradical)

The nilradical of a [commutative ring](#commutative-ring) is its [ideal](#ideal) of [nilpotent elements](#nilpotent), equivalently the [radical of an ideal](#radical-of-an-ideal) applied to its zero ideal.

###### Nilradical that is not nilpotent

↑ **Parent:** [Nilradical](#nilradical)

In $R=k[t_1,t_2,\ldots]/(t_1^2,t_2^2,\ldots)$, the [nilradical](#nilradical) is generated by all $\bar t_i$. Every element uses finitely many variables and is nilpotent, while each square-free product $\bar t_1\cdots\bar t_j$ is nonzero. Thus this [nilradical](#nilradical) is not a [nilpotent ideal](#nilpotent-ideal). A [Noetherian ring](algebra.md#noetherian-ring) cannot have this behavior: finitely many nilpotent generators give a nilpotent [ideal](#ideal).

###### Nilradical as the intersection of prime ideals

↑ **Parent:** [Nilradical](#nilradical)

For every [commutative ring](#commutative-ring) $R$,

$$
\operatorname{Nil}(R)=\bigcap_{P\in\operatorname{Spec}R}P.
$$

Every [nilpotent element](#nilpotent) lies in every [prime ideal](#prime-ideal). If $a$ is not nilpotent, an [ideal](#ideal) maximal among those disjoint from $\{1,a,a^2,\ldots\}$ is a [prime ideal](#prime-ideal) avoiding $a$, by the [Zorn lemma](set-theory.md#zorn-s-lemma) and the maximality argument.

### Ring homomorphism

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ring_homomorphism)

A ring homomorphism preserves addition, multiplication, and, under the convention used here, the multiplicative identity.

#### Ring endomorphism

↑ **Parent:** [Ring homomorphism](#ring-homomorphism)

A [ring homomorphism](#ring-homomorphism) from a ring to itself. Surjectivity need not imply injectivity in general, but a surjective [ring endomorphism](#ring-endomorphism) of a [Noetherian ring](algebra.md#noetherian-ring) is a [ring automorphism](#ring-automorphism).

##### Ring automorphism

↑ **Parent:** [Ring endomorphism](#ring-endomorphism)

A bijective [ring endomorphism](#ring-endomorphism). Its inverse is again a [ring homomorphism](#ring-homomorphism), so it preserves the ring structure in both directions.

#### Kernel of a ring homomorphism

↑ **Parent:** [Ring homomorphism](#ring-homomorphism)

The kernel of a [ring homomorphism](#ring-homomorphism) $\varphi:R\to S$ is the [ideal](#ideal) $\{r\in R:\varphi(r)=0\}$. The [ring homomorphism](#ring-homomorphism) is [injective](algebra.md#injective-function) exactly when this [ideal](#ideal) is zero.

#### Extension and contraction of ideals

↑ **Parent:** [Ring homomorphism](#ring-homomorphism)

For a [ring homomorphism](#ring-homomorphism) $f:R\to S$, extension sends an [ideal](#ideal) $I\subseteq R$ to the ideal $S f(I)$ generated by its image. Contraction sends an ideal $J\subseteq S$ to $f^{-1}(J)$. These are distinct forward and inverse-image operations.

##### Extension of an ideal

↑ **Parent:** [Extension and contraction of ideals](#extension-and-contraction-of-ideals)

For a ring homomorphism $f:R\to A$ and an ideal $I\subseteq R$, the extension $I^e=IA$ is the ideal of $A$ generated by $f(I)$.

##### Contraction of an ideal

↑ **Parent:** [Extension and contraction of ideals](#extension-and-contraction-of-ideals)

For a ring homomorphism $f:R\to A$ and an ideal $J\subseteq A$, its contraction is $J^c=f^{-1}(J)$.

#### Evaluation homomorphism

↑ **Parent:** [Ring homomorphism](#ring-homomorphism)

For an element $a$ of a commutative $R$-algebra, evaluation on a [polynomial ring](#polynomial-ring) is the ring homomorphism

$$
R[X]\longrightarrow R[a],\qquad f\longmapsto f(a).
$$

#### First isomorphism theorem for rings

↑ **Parent:** [Ring homomorphism](#ring-homomorphism)

Every ring homomorphism $\phi:R\to S$ induces an isomorphism

$$
R/\ker\phi\cong\operatorname{im}\phi,
\qquad r+\ker\phi\longmapsto\phi(r).
$$

### Idempotent

↑ **Parent:** [Ring](#ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Idempotent_(ring_theory))

An element $e$ is idempotent when $e^2=e$.

#### Orthogonal idempotent

↑ **Parent:** [Idempotent](#idempotent)

Distinct [idempotents](#idempotent) are orthogonal when their products in both orders vanish. A finite family summing to one gives a decomposition $M=\bigoplus_ie_iM$ of every left [module](module-theory.md#module-mathematics) as a vector space; the summands need not be submodules unless the idempotents are central. Vertex idempotents of a [path algebra](algebra.md#path-algebra) supply the spaces of its [quiver representation](algebra.md#representation-of-a-quiver).

#### Primitive idempotent

↑ **Parent:** [Idempotent](#idempotent)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_idempotent)

A nonzero idempotent is primitive when it cannot be written as a sum of two nonzero orthogonal idempotents. For a finite-dimensional algebra $A$, the left module $Ae$ is indecomposable projective exactly when $e$ is primitive.

##### Triangular primitive-idempotent decomposition

↑ **Parent:** [Primitive idempotent](#primitive-idempotent)

If [idempotents](#idempotent) $e_1,\ldots,e_N$ satisfy $e_ie_j=0$ for $i>j$, then the [left ideals](associative-algebra.md#left-ideal) $Ae_i$ have an internal [direct sum](vector-space.md#direct-sum). Multiply a relation $\sum z_i=0$ by $e_1$ on the right to obtain $z_1=0$, and continue in order. Pairwise orthogonality in both directions is unnecessary. If the sum has dimension $\dim A$, it is the whole algebra.

##### Primitive idempotents under a surjection of commutative Artinian ideals

↑ **Parent:** [Primitive idempotent](#primitive-idempotent)

Let $A,B$ be finite-dimensional commutative [algebras](algebra.md), let $I\subset A$ and $J\subset B$ be [ideals](#ideal), and let $f:I\to J$ be a surjective algebra homomorphism. The ideals need not have identities. Then $f$ gives a bijection between the [primitive idempotents](#primitive-idempotent) of $A$ lying in $I$ with nonzero image and the primitive idempotents of $J$.

Decompose $A$ into its commutative [Artinian local rings](algebra.md#artinian-local-ring) $A_i$, with identities $e_i$. Each $I\cap A_i$ is either all of $A_i$, in which case $e_i\in I$, or a proper ideal and therefore a [nilpotent ideal](#nilpotent-ideal). The sum of the latter ideals is nilpotent, so its image contributes no idempotents. Each nonzero $f(e_i)$ has local corner algebra $f(e_i)J=f(A_i)$, a quotient of $A_i$, so is primitive. These idempotents are orthogonal, and the remaining part of $J$ is nilpotent; hence they are exactly its primitive idempotents. This statement does not require the entire kernel of $f$ to be nilpotent.

#### Idempotent lifting

↑ **Parent:** [Idempotent](#idempotent)

If a ring is complete with respect to an ideal contained in its [Jacobson radical](noncommutative-algebra.md#jacobson-radical), every idempotent in the quotient lifts to an idempotent of the ring. Consequently direct-sum decompositions of a modular reduction lift to a complete integral lattice.

##### Idempotent refinement theorem

↑ **Parent:** [Idempotent lifting](#idempotent-lifting)

In a finite-dimensional algebra, or a complete finite coefficient-ring algebra, primitive [idempotents](#idempotent) lift modulo a nilpotent ideal or the coefficient maximal ideal. Orthogonal decompositions of the identity lift, and equivalent primitive idempotents have isomorphic associated projective modules. Two lifts of the same idempotent modulo such an ideal are conjugate by a unit congruent to one. This is an [idempotent lifting](#idempotent-lifting) and refinement result; it does not assert that every central idempotent lifts centrally through an arbitrary nilpotent quotient.

## Integral domain

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_domain)

An integral domain is a nonzero commutative ring with identity and without zero divisors.

### Fractional ideal

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fractional_ideal)

For an [integral domain](#integral-domain) $A$ with [fraction field](#field-of-fractions) $K$, a fractional ideal is a nonzero $A$-submodule $I\subseteq K$ for which $dI\subseteq A$ for some $0\ne d\in A$. A finitely generated submodule of $K$ has a common denominator and is therefore a fractional ideal. The product is generated by pairwise products of elements. An [invertible fractional ideal](#invertible-fractional-ideal) has a multiplicative inverse and is finitely generated; arbitrary fractional ideals need not be finitely generated over a non-Noetherian domain. The familiar fractional ideals of a [number field](algebraic-number-theory.md#number-field) are the special case $A=\mathcal O_K$. This general definition also applies to the ideals representing [Cartier divisors](cartier-divisor.md) on affine integral schemes.

#### Invertible fractional ideal

↑ **Parent:** [Fractional ideal](#fractional-ideal)

Over an [integral domain](#integral-domain) $A$ with [fraction field](#field-of-fractions) $K$, an [invertible fractional ideal](#invertible-fractional-ideal) is a finitely generated nonzero $A$-submodule $I\subseteq K$ for which another fractional ideal $J$ satisfies $IJ=A$. Here $I^{-1}=\{x\in K:xI\subseteq A\}$ equals $J$. Choose $1=\sum u_iv_i$ with $u_i\in I$, $v_i\in J$. On the distinguished open where $u_iv_i$ is invertible, $I$ is generated by $u_i$, since $x/u_i=(xv_i)/(u_iv_i)$. The maps $x\mapsto v_ix$ form a finite dual basis and prove that $I$ is a rank-one [projective module](module-theory.md#projective-module). Conversely, a finitely generated rank-one [projective module](module-theory.md#projective-module) embeds in $K$ after choosing a basis over $K$; its dual identifies with $I^{-1}$, and local evaluation shows $II^{-1}=A$.

#### Principal fractional ideal

↑ **Parent:** [Fractional ideal](#fractional-ideal)

A principal fractional ideal of an [integral domain](#integral-domain) $A$ with [fraction field](#field-of-fractions) $K$ is $aA$ for a nonzero $a\in K$. Its generators differ by a [unit in a ring](algebra.md#unit-in-a-ring) in $A$. For a [number field](algebraic-number-theory.md#number-field), taking $A=\mathcal O_K$ and quotienting nonzero [fractional ideals](#fractional-ideal) by [principal fractional ideals](#principal-fractional-ideal) gives the [ideal class group](algebraic-number-theory.md#ideal-class-group); requiring congruences and signs of the generators instead gives a [ray class group](algebraic-number-theory.md#ray-class-group).

#### Integral ideal

↑ **Parent:** [Fractional ideal](#fractional-ideal)

An integral ideal is a [fractional ideal](#fractional-ideal) of an [integral domain](#integral-domain) $A$ that is contained in $A$. For a [number field](algebraic-number-theory.md#number-field), take $A$ to be its [ring of integers](algebraic-number-theory.md#ring-of-integers) $\mathcal O_K$.

### Finite integral domain is a field

↑ **Parent:** [Integral domain](#integral-domain)

Multiplication by a nonzero element of an [integral domain](#integral-domain) is injective. If the ring is finite, that map is surjective, so its image contains one and the multiplier has a multiplicative inverse. Hence every nonzero element is invertible and the ring is a [field](algebra.md#field).

### Prime element

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_element)

A nonzero nonunit $p$ in an integral domain is prime when $p\mid ab$ implies $p\mid a$ or $p\mid b$.

### Irreducible element

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irreducible_element)

A nonzero nonunit $p$ in an integral domain is irreducible when every factorization $p=ab$ has at least one unit factor.

### Atomic domain

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Atomic_domain)

An atomic domain is an [integral domain](#integral-domain) in which every nonzero nonunit is a finite product of [irreducible elements](#irreducible-element). Every [unique factorization domain](algebra.md#unique-factorization-domain) is atomic, but atomicity alone does not imply uniqueness.

### Greatest-common-divisor domain

↑ **Parent:** [Integral domain](#integral-domain)

A greatest-common-divisor domain is an integral domain in which every two nonzero elements have a greatest common divisor, defined up to multiplication by a unit.

#### Euclid lemma in a greatest-common-divisor domain

↑ **Parent:** [Greatest-common-divisor domain](#greatest-common-divisor-domain)

If $\gcd(a,b)=1$ and $a\mid bc$ in a greatest-common-divisor domain, then $a\mid c$. Indeed, the least common multiple of $a$ and $b$ is associate to $ab$ and divides every common multiple; applying this to $bc$ and cancelling $b$ proves the claim.

### Field of fractions

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_of_fractions)

The fraction field of an [integral domain](#integral-domain) $R$ consists of fractions $a/b$ with $a,b\in R$ and $b\ne0$, modulo the usual equivalence relation.

### Principal ideal domain

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Principal_ideal_domain)

A principal ideal domain is an integral domain whose every ideal has one generator.

#### Nonprincipal coordinate ideal in two variables

↑ **Parent:** [Principal ideal domain](#principal-ideal-domain)

Over a [field](algebra.md#field) $F$, the [ideal](#ideal) $(X,Y)$ in a two-variable [polynomial ring](#polynomial-ring) is not principal. A proposed generator would divide both $X$ and $Y$. Any nonconstant divisor of the degree-one polynomial $X$ is a scalar multiple of $X$, which does not divide $Y$; therefore the generator would have to be a unit. But every element of $(X,Y)$ vanishes at $(0,0)$, so the ideal cannot contain one. This contrasts with $F[X]$, where the division algorithm makes every ideal principal.

#### Every principal ideal domain is a unique factorization domain

↑ **Parent:** [Principal ideal domain](#principal-ideal-domain)

The [ascending chain condition](algebra.md#ascending-chain-condition) supplies existence of factorizations into [irreducible elements](#irreducible-element). The [Bezout identity](algebra.md#bezout-identity) makes every irreducible element prime, which supplies uniqueness up to order and multiplication by units.

#### Submodule theorem for free modules over a principal ideal domain

↑ **Parent:** [Principal ideal domain](#principal-ideal-domain)

Every submodule of a finite-rank free module over a principal ideal domain is free. Induction on rank splits off a generator of the image under one coordinate projection and applies the result to the kernel.

#### Euclidean domain

↑ **Parent:** [Principal ideal domain](#principal-ideal-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_domain)

A Euclidean domain admits division with remainder measured by a decreasing Euclidean function.

##### Norm-Euclidean integers of discriminant minus seven

↑ **Parent:** [Euclidean domain](#euclidean-domain)

The [ring of integers](algebraic-number-theory.md#ring-of-integers) $\mathbb Z[(1+\sqrt{-7})/2]$ is a [Euclidean domain](#euclidean-domain) for $N(z)=z\overline z$. In its lattice choose the nearest row, whose imaginary-coordinate error is at most $\sqrt7/4$, then the nearest point on that row, whose real-coordinate error is at most $1/2$. Every complex number is thus within squared distance $11/16<1$ of a lattice point, giving Euclidean division. The suborder $\mathbb Z[\sqrt{-7}]$ has the nonprincipal [ideal](#ideal) $(2,1+\sqrt{-7})$ and consequently is not a [Euclidean domain](#euclidean-domain) for any Euclidean function.

##### Euclidean function

↑ **Parent:** [Euclidean domain](#euclidean-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_function)

A Euclidean function on an integral domain $R$ assigns a nonnegative integer to every nonzero element so that, for $a,b\in R$ with $b\ne0$, there are $q,r\in R$ satisfying $a=bq+r$ and either $r=0$ or $d(r)<d(b)$.

##### Gaussian integer

↑ **Parent:** [Euclidean domain](#euclidean-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_integer)

A Gaussian integer has the form $a+bi$ with $a,b\in\mathbb Z$. Its multiplicative norm is $N(a+bi)=a^2+b^2$, which makes $\mathbb Z[i]$ a Euclidean domain.

###### Primary Gaussian integer

↑ **Parent:** [Gaussian integer](#gaussian-integer)

An odd [Gaussian integer](#gaussian-integer) is primary when it satisfies the displayed congruence. The four units have distinct images in $(\mathbb Z[i]/(1+i)^3)^\times$, a group of order four; hence every odd ideal has a unique primary generator. Indeed $v_{1+i}(-2)=2$ and $v_{1+i}(i-1)=v_{1+i}(-i-1)=1$.

###### Finite residue-field theorem for Gaussian integer orders

↑ **Parent:** [Gaussian integer](#gaussian-integer)

If $\alpha=a+bi$ is a [Gaussian integer](#gaussian-integer) and $P$ is a nonzero [prime ideal](#prime-ideal) of $R=\mathbb Z[\alpha]$, then $R/P$ is a finite field. Complex conjugation preserves $R$, so a nonzero $\beta\in P$ gives the positive integer $\beta\bar\beta\in P$. Primality supplies a rational prime $p\in P$. Since $\alpha$ satisfies the monic polynomial $t^2-2at+a^2+b^2$, the ring $R/P$ is a quotient of $\mathbb F_p[t]/(\bar F)$ and has at most $p^2$ elements. It is a finite [integral domain](#integral-domain), hence a field. The proof does not require $R$ to be a [principal ideal domain](#principal-ideal-domain).

##### Eisenstein integer

↑ **Parent:** [Euclidean domain](#euclidean-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eisenstein_integer)

For a primitive cube root of unity $\omega$, the Eisenstein integers form the triangular lattice

$$
\mathbb Z[\omega]=\{a+b\omega:a,b\in\mathbb Z\}.
$$

Their multiplicative norm is $N(a+b\omega)=a^2-ab+b^2$.

###### Eisenstein-integer norm

↑ **Parent:** [Eisenstein integer](#eisenstein-integer)

The Eisenstein-integer norm is $N(z)=z\overline z$. It is multiplicative and takes $a+b\omega$ to $a^2-ab+b^2$.

###### Euclidean norm on the Eisenstein integers

↑ **Parent:** [Eisenstein integer](#eisenstein-integer)

Every complex number is within squared distance at most $3/4$ of an Eisenstein integer: write it as $x+y\omega$ and round $x$ and $y$ to integers. Therefore, for nonzero $\beta$ and arbitrary $\alpha$, a nearest lattice point $q$ to $\alpha/\beta$ gives

$$
N(\alpha-q\beta)<N(\beta).
$$

The norm makes the Eisenstein integers a [Euclidean domain](#euclidean-domain).

<h3 id="bezout-domain">Bézout domain</h3>

↑ **Parent:** [Integral domain](#integral-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bézout_domain)

A Bézout domain is an integral domain in which every finitely generated ideal is principal. Equivalently, every pair $a,b$ has a greatest common divisor $d$ satisfying a Bézout identity $d=ra+sb$. A Noetherian Bézout domain is a principal ideal domain because all its ideals are finitely generated.

## Ring product decomposition by an idempotent

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

A commutative ring $R$ has a nontrivial idempotent $e$ exactly when it decomposes as a product of two nontrivial rings. The isomorphism determined by $e$ is

$$
R\longrightarrow eR\times(1-e)R,
\qquad r\longmapsto(er,(1-e)r),
$$

with inverse $(x,y)\mapsto x+y$.

## Fiber product of rings

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fiber_product_of_rings)

A fiber product of rings consists of pairs having the same image in a third ring.

## Unit modulo a prime power

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unit_modulo_a_prime_power)

Modulo a prime power, a class is a unit exactly when it is not divisible by that prime.

## Nilpotent element modulo a prime power

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nilpotent_element_modulo_a_prime_power)

Modulo p^e, a class is nilpotent exactly when its reduction modulo p is zero.

## Reduction map on unit groups

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduction_map_on_unit_groups)

Reduction between quotient rings sends units to units and is surjective when every target unit avoids the same prime factors.

## Polynomial content

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_content)

The content of a polynomial is a greatest common divisor of its coefficients, up to a unit.

### Primitive polynomial

↑ **Parent:** [Polynomial content](#polynomial-content)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_polynomial)

A primitive polynomial has unit content.

#### Gauss lemma for polynomials

↑ **Parent:** [Primitive polynomial](#primitive-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss_lemma_for_polynomials)

Over a UFD, products of primitive polynomials are primitive and factorization over the fraction field descends after content is removed.

##### Multiplicativity of the nonarchimedean polynomial norm

↑ **Parent:** [Gauss lemma for polynomials](#gauss-lemma-for-polynomials)

For a [field](algebra.md#field) with a [Non-Archimedean absolute value](arithmetic.md#non-archimedean-absolute-value), define the coefficient norm $\|f\|_G=\max_i|a_i|$ for $f(T)=\sum_i a_iT^i$. Then $\|fg\|_G=\|f\|_G\|g\|_G$. For nonzero [polynomials](polynomial.md), scale each by one of its coefficients of maximum absolute value; the resulting [polynomials](polynomial.md) have integral coefficients and at least one [unit](algebra.md#unit-in-a-ring) coefficient. Their reductions in the [residue field](#residue-field) are nonzero, so their product is nonzero. The product therefore also has coefficient norm $1$, proving the formula after reversing the scaling. This compares binary-polynomial coefficient heights with the heights of their roots.

##### Polynomial ring over a unique factorization domain

↑ **Parent:** [Gauss lemma for polynomials](#gauss-lemma-for-polynomials)

If $R$ is a [unique factorization domain](algebra.md#unique-factorization-domain) with fraction field $F$, then $R[X]$ is a unique factorization domain. A primitive polynomial irreducible in $R[X]$ remains irreducible, hence prime, in the principal ideal domain $F[X]$; [Gauss lemma for polynomials](#gauss-lemma-for-polynomials) brings divisibility back to $R[X]$.

###### Integer polynomial ring is not a principal ideal domain

↑ **Parent:** [Polynomial ring over a unique factorization domain](#polynomial-ring-over-a-unique-factorization-domain)

The [polynomial ring](#polynomial-ring) $\mathbb Z[X]$ is a [unique factorization domain](algebra.md#unique-factorization-domain) by [Gauss lemma for polynomials](#gauss-lemma-for-polynomials), but its [ideal](#ideal) $(2,X)$ is not principal. Any generator would divide both 2 and $X$, hence be a unit: a divisor of 2 has degree zero, and a constant dividing $X$ is $\pm1$. Yet evaluation at zero followed by reduction modulo 2 annihilates the ideal and not 1. It embeds in the [principal ideal domain](#principal-ideal-domain) $\mathbb Q[X]$, illustrating that the property need not pass to a subring.

##### Symmetric rational function in two variables

↑ **Parent:** [Gauss lemma for polynomials](#gauss-lemma-for-polynomials)

Every rational function in $\mathbb C(X,Y)$ fixed by exchanging $X$ and $Y$ is a quotient of coprime symmetric polynomials. In a coprime presentation $p/q$, symmetry gives

$$
pq^*=p^*q.
$$

Unique factorization implies $p^*=\lambda p$ and $q^*=\lambda q$. The alternative $\lambda=-1$ would make both divisible by $X-Y$, contradicting coprimality, so $\lambda=1$.

## Eisenstein criterion

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eisenstein_criterion)

For a primitive polynomial

$$
F(X)=a_nX^n+\cdots+a_0\in\mathbb Z[X],
$$

if a prime $p$ does not divide $a_n$, divides every $a_j$ for $j<n$, and has $p^2\nmid a_0$, then $F$ is irreducible. If $F=GH$, reduction modulo $p$ forces both $\overline G$ and $\overline H$ to be positive-degree monomials. Their constant terms are consequently divisible by $p$, making $p^2\mid F(0)$, a contradiction. [Gauss lemma for polynomials](#gauss-lemma-for-polynomials) transfers the result between $\mathbb Z[X]$ and $\mathbb Q[X]$.

### Total ramification from an Eisenstein polynomial

↑ **Parent:** [Eisenstein criterion](#eisenstein-criterion)

If an algebraic integer $\alpha$ has a degree-$n$ minimal polynomial that is Eisenstein at $p$, then $p$ has a unique prime ideal $P$ above it in $\mathbb Q(\alpha)$, with

$$
(p)=P^n,\qquad v_P(\alpha)=1.
$$

This conclusion concerns the full [ring of integers of a number field](algebraic-number-theory.md#ring-of-integers) and does not assume that it equals $\mathbb Z[\alpha]$.

### Geometric-sum irreducibility criterion

↑ **Parent:** [Eisenstein criterion](#eisenstein-criterion)

For $n>1$,

$$
1+X+\cdots+X^{n-1}
$$

is irreducible over the integers exactly when $n$ is prime. Composite $n$ gives a geometric factorization; for prime $p$, translation $X\mapsto X+1$ makes the polynomial Eisenstein at $p$.

## Odd-valuation obstruction to a rational-function square

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

Every zero and pole of a square in $K(Y)$ has even order. Thus a rational function with a zero or pole of odd order cannot be a square. For characteristic different from two, this proves that $1-Y^2$ is not a square in $K(Y)$.

## Module theory

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

[This section is present in another page, follow this link to view it.](module-theory.md)

## Prime ideal

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_ideal)

An ideal $\mathfrak p$ is prime when $ab\in\mathfrak p$ implies $a\in\mathfrak p$ or $b\in\mathfrak p$, equivalently when the quotient is an integral domain.

### Minimal prime ideal

↑ **Parent:** [Prime ideal](#prime-ideal)

A minimal prime ideal is a [prime ideal](#prime-ideal) containing no strictly smaller prime ideal. If $A$ is a [reduced ring](#reduced-ring) and $\mathfrak p$ is minimal, the [localization at a prime ideal](#localization-at-a-prime-ideal) $A_{\mathfrak p}$ is a field: its only prime is its maximal ideal, and reducedness makes that ideal its zero [nilradical](#nilradical). Every nonzero commutative ring has a minimal prime.

#### Minimal prime over an ideal

↑ **Parent:** [Minimal prime ideal](#minimal-prime-ideal)

A [prime ideal](#prime-ideal) $P$ is minimal over an [ideal](#ideal) $I$ if $I\subseteq P$ and no smaller [prime ideal](#prime-ideal) contains $I$. The definition also applies to two-sided [prime ideals of a noncommutative ring](noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring).

#### Existence of minimal primes over a proper ideal

↑ **Parent:** [Minimal prime ideal](#minimal-prime-ideal)

Every proper [ideal](#ideal) of a unital commutative [ring](#ring) is contained in a minimal prime over that [ideal](#ideal). A [maximal ideal](#maximal-ideal) supplies a prime containing it, and an intersection of a decreasing chain of primes is still prime. [Zorn's lemma](set-theory.md#zorn-s-lemma), with reverse inclusion, therefore supplies a minimal member. No [Noetherian](algebra.md#noetherian-ring) assumption is needed.

#### Unique minimal prime does not imply primary

↑ **Parent:** [Minimal prime ideal](#minimal-prime-ideal)

In $k[u,v]$, the [ideal](#ideal) $I=(u^2,uv)$ has [radical of an ideal](#radical-of-an-ideal) $(u)$, a [prime ideal](#prime-ideal), and hence a unique [minimal prime ideal](#minimal-prime-ideal). Nevertheless $uv\in I$, $u\notin I$, and $v^j\notin I$ for all $j\ge1$, so $I$ is not a [primary ideal](#primary-ideal). The same example works after adjoining inverses of $1+u$ and $1+v$; thus it also gives an example in a two-variable [Laurent polynomial ring](#laurent-polynomial-ring).

### Prime ideal avoiding a multiplicative subset

↑ **Parent:** [Prime ideal](#prime-ideal)

In a [Noetherian ring](algebra.md#noetherian-ring), an [ideal](#ideal) $I$ disjoint from a nonempty [multiplicative subset](#multiplicatively-closed-set) $S$ extends to an ideal $P$ maximal among those disjoint from $S$, by the [ascending chain condition](algebra.md#ascending-chain-condition). It is proper. If $ab\in P$ but neither factor belongs to $P$, both $P+(a)$ and $P+(b)$ meet $S$. Multiplying such representatives puts an element of $S$ in $P$, a contradiction. Thus $P$ is a [prime ideal](#prime-ideal). For a general [commutative ring](#commutative-ring) the same argument follows after applying the [Zorn lemma](set-theory.md#zorn-s-lemma) to disjoint ideals; the union of a chain is disjoint from $S$.

### Symbolic power

↑ **Parent:** [Prime ideal](#prime-ideal)

The $n$th symbolic power of a [prime ideal](#prime-ideal) $P\subset R$ is

$$
P^{(n)}=P^nR_P\cap R,
$$

where the intersection denotes [contraction of an ideal](#contraction-of-an-ideal). It is always a $P$-[primary ideal](#primary-ideal). The ordinary power $P^n$ equals $P^{(n)}$ precisely when $P^n$ is $P$-primary; this assertion does not require $R$ to be [Noetherian](algebra.md#noetherian-ring).

### Prime ideal quotient criterion

↑ **Parent:** [Prime ideal](#prime-ideal)

For a commutative unital ring $R$, an ideal $I$ is prime exactly when $R/I$ is an integral domain. The zero-product condition in the quotient translates directly to $ab\in I$.

## Boolean ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boolean_ring)

A Boolean ring satisfies $r^2=r$ for every element. Expanding $(r+1)^2=r+1$ shows that it has characteristic two.

### Prime ideals of a Boolean ring are maximal

↑ **Parent:** [Boolean ring](#boolean-ring)

A nonzero Boolean integral domain has only the elements zero and one, so it is $\mathbb F_2$. The quotient criterion then makes every prime quotient of a Boolean ring a field, and every prime ideal maximal.

## Coefficientwise quotient of a polynomial ring

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

For an ideal $I$ of a commutative ring $R$, reducing coefficients modulo $I$ is a surjection $R[X]\to(R/I)[X]$ with kernel $I[X]$. Hence

$$
R[X]/I[X]\cong(R/I)[X].
$$

## Irreducible real polynomial

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

The irreducible polynomials over $\mathbb R$ have degree one, or degree two with negative discriminant.

## Kummer irreducibility criterion

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

Over a field containing the relevant roots of unity, $X^n-a$ is irreducible when the valuation data prevent $a$ from being a proper prime-divisor power, with the standard fourth-power exception.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Algebraic differential operator ring](#algebraic-differential-operator-ring)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-2.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-2.md#5/solution)
