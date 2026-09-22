# Ringed space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ringed_space)

A ringed space $(X,\mathcal O_X)$ is a [topological space](topology.md#topological-space) $X$ equipped with a [sheaf of rings](#sheaf-of-rings) $\mathcal O_X$. A morphism consists of a continuous map $f:X\to Y$ and a compatible morphism $f^{-1}\mathcal O_Y\to\mathcal O_X$.

**Table of contents**

- [Morphism of ringed spaces](#morphism-of-ringed-spaces)
- [Sheaf of rings](#sheaf-of-rings)
  - [Sheaf of topological rings](#sheaf-of-topological-rings)
- [Sheaf of modules](#sheaf-of-modules)
  - [Internal Hom sheaf](#internal-hom-sheaf)
  - [Local system](#local-system)
  - [Rational section of a sheaf of modules](#rational-section-of-a-sheaf-of-modules)
    - [Rational principal part](#rational-principal-part)
      - [Rational principal-parts resolution on an algebraic curve](#rational-principal-parts-resolution-on-an-algebraic-curve)
        - [Affine principal-parts interpolation for a locally free sheaf](#affine-principal-parts-interpolation-for-a-locally-free-sheaf)
    - [Stalk inclusion into rational sections of a locally free sheaf](#stalk-inclusion-into-rational-sections-of-a-locally-free-sheaf)
  - [Coherent analytic sheaf](#coherent-analytic-sheaf)
  - [Dual of a sheaf](#dual-of-a-sheaf)
  - [Injective sheaf of modules](#injective-sheaf-of-modules)
    - [Injective module sheaves are flasque](#injective-module-sheaves-are-flasque)
  - [Stalk of a sheaf](#stalk-of-a-sheaf)
    - [Costalk](#costalk)
    - [Stalk functor for presheaves of sets](#stalk-functor-for-presheaves-of-sets)
      - [Joint stalk functor on sheaves of sets](#joint-stalk-functor-on-sheaves-of-sets)
    - [Skyscraper sheaf](#skyscraper-sheaf)
      - [Skyscraper sheaf cohomology](#skyscraper-sheaf-cohomology)
    - [Germ of a sheaf section](#germ-of-a-sheaf-section)
      - [Support of a sheaf section](#support-of-a-sheaf-section)
  - [Sheafification](#sheafification)
    - [Universal property of sheafification](#universal-property-of-sheafification)
    - [Sheafification by locally representable germs](#sheafification-by-locally-representable-germs)
  - [Extension by zero](#extension-by-zero)
  - [Quasi-coherent sheaf](#quasi-coherent-sheaf)
    - [Kernels of quasi-coherent sheaf morphisms](#kernels-of-quasi-coherent-sheaf-morphisms)
    - [Affine module sheaf](#affine-module-sheaf)
      - [Coherence of an affine module sheaf](#coherence-of-an-affine-module-sheaf)
    - [Quasi-coherent sheaves are closed under extensions](#quasi-coherent-sheaves-are-closed-under-extensions)
    - [Global-section localization for quasi-coherent sheaves](#global-section-localization-for-quasi-coherent-sheaves)
    - [Affine module-sheaf equivalence](#affine-module-sheaf-equivalence)
    - [Torsion-free sheaf](#torsion-free-sheaf)
    - [Vanishing of quasi-coherent cohomology on an affine scheme](#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme)
    - [Coherent sheaf](#coherent-sheaf)
      - [Globally generated sheaf](#globally-generated-sheaf)
      - [Stalkwise isomorphic coherent sheaves need not be isomorphic](#stalkwise-isomorphic-coherent-sheaves-need-not-be-isomorphic)
      - [Coherent ideal sheaf](#coherent-ideal-sheaf)
      - [Finite twisting resolution of a coherent sheaf on projective space](#finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space)
      - [Support dimension of a coherent sheaf](#support-dimension-of-a-coherent-sheaf)
      - [Associated point of a coherent sheaf](#associated-point-of-a-coherent-sheaf)
      - [Direct image of a coherent sheaf under a closed immersion](#direct-image-of-a-coherent-sheaf-under-a-closed-immersion)
  - [Tensor product of sheaves](#tensor-product-of-sheaves)
  - [Direct image sheaf](#direct-image-sheaf)
    - [Derived direct image of sheaves](#derived-direct-image-of-sheaves)
      - [Proper base change for sheaves](#proper-base-change-for-sheaves)
    - [Projective direct image need not preserve surjections](#projective-direct-image-need-not-preserve-surjections)
    - [Coherence reflected by finite direct image](#coherence-reflected-by-finite-direct-image)
    - [Direct image from an open restriction](#direct-image-from-an-open-restriction)
    - [Direct-image tensor comparison](#direct-image-tensor-comparison)
    - [Sheaf cohomology under a closed inclusion](#sheaf-cohomology-under-a-closed-inclusion)
    - [Direct image of a quasi-coherent sheaf under an affine morphism](#direct-image-of-a-quasi-coherent-sheaf-under-an-affine-morphism)
      - [Acyclic direct image from an affine chart of the projective line](#acyclic-direct-image-from-an-affine-chart-of-the-projective-line)
    - [Quasi-coherence of direct image under a quasi-compact quasi-separated morphism](#quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism)
  - [Inverse image sheaf](#inverse-image-sheaf)
    - [Inverse-image direct-image adjunction](#inverse-image-direct-image-adjunction)
    - [Universal property of an inverse image sheaf](#universal-property-of-an-inverse-image-sheaf)
    - [Pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules)
      - [Restriction of a module sheaf to a closed subvariety](#restriction-of-a-module-sheaf-to-a-closed-subvariety)
      - [Pullback-direct-image adjunction unit](#pullback-direct-image-adjunction-unit)
      - [Projection formula](#projection-formula)
  - [Locally free sheaf](#locally-free-sheaf)
    - [Free sheaf](#free-sheaf)
    - [Saturated line subbundle on a smooth curve](#saturated-line-subbundle-on-a-smooth-curve)
      - [Unbounded negative degrees of line subbundles](#unbounded-negative-degrees-of-line-subbundles)
      - [Upper degree bound for line subbundles on a smooth curve](#upper-degree-bound-for-line-subbundles-on-a-smooth-curve)
    - [Local splitting when a quotient sheaf is locally free](#local-splitting-when-a-quotient-sheaf-is-locally-free)
    - [Line bundle](#line-bundle)
      - [Degree of a line bundle](#degree-of-a-line-bundle)
      - [Half-density](#half-density)
      - [Orientation line bundle](#orientation-line-bundle)
        - [Orientable total space of the orientation line bundle](#orientable-total-space-of-the-orientation-line-bundle)
      - [Homogeneous line-bundle representations on the two-sphere](#homogeneous-line-bundle-representations-on-the-two-sphere)
      - [Line bundles trivialized by an open cover](#line-bundles-trivialized-by-an-open-cover)
      - [Globally generated line bundle](#globally-generated-line-bundle)
        - [Globally generated line bundle without finite generators](#globally-generated-line-bundle-without-finite-generators)
        - [Finite global generation on a quasi-compact scheme](#finite-global-generation-on-a-quasi-compact-scheme)
        - [Tensor product of globally generated line bundles](#tensor-product-of-globally-generated-line-bundles)
      - [Rational section of a line bundle](#rational-section-of-a-line-bundle)
      - [Twisting sheaf on projective space](#twisting-sheaf-on-projective-space)
        - [Homogeneous rational sections of a twisting sheaf](#homogeneous-rational-sections-of-a-twisting-sheaf)
        - [Laurent-monomial description of top cohomology on projective space](#laurent-monomial-description-of-top-cohomology-on-projective-space)
        - [Canonical bundle of projective space](#canonical-bundle-of-projective-space)
          - [Canonical-form transition on projective space](#canonical-form-transition-on-projective-space)
        - [Hyperplane exact sequence for twisting sheaves](#hyperplane-exact-sequence-for-twisting-sheaves)
          - [Top-twist vanishing by hyperplane induction](#top-twist-vanishing-by-hyperplane-induction)
      - [Picard group](#picard-group)
        - [Picard group of the projective line](#picard-group-of-the-projective-line)
        - [Degree-zero Picard group of a curve](#degree-zero-picard-group-of-a-curve)
          - [Rational points need not generate the degree-zero Picard group](#rational-points-need-not-generate-the-degree-zero-picard-group)
          - [Abel map of a pointed smooth projective curve](#abel-map-of-a-pointed-smooth-projective-curve)
        - [Picard functor of a curve](#picard-functor-of-a-curve)
          - [Picard scheme of a curve](#picard-scheme-of-a-curve)
            - [Picard charts from nonspecial divisors](#picard-charts-from-nonspecial-divisors)
        - [Picard group of a ring](#picard-group-of-a-ring)
        - [Holomorphic Picard group](#holomorphic-picard-group)
          - [Picard injection for holomorphic projective bundles](#picard-injection-for-holomorphic-projective-bundles)
        - [Picard-group localization on a smooth variety](#picard-group-localization-on-a-smooth-variety)
        - [Cartier-divisor description of the Picard group](#cartier-divisor-description-of-the-picard-group)
        - [Néron-Severi group](#neron-severi-group)
      - [Very ample line bundle](#very-ample-line-bundle)
      - [Ample line bundle](#ample-line-bundle)
        - [Ampleness on reduced components](#ampleness-on-reduced-components)
        - [Finite pullback of an ample line bundle](#finite-pullback-of-an-ample-line-bundle)
        - [High ample twist is very ample](#high-ample-twist-is-very-ample)
      - [Kodaira map](#kodaira-map)
  - [Global section functor](#global-section-functor)
    - [Localization of global sections on a principal open](#localization-of-global-sections-on-a-principal-open)
    - [Global section](#global-section)
    - [Section functor with support](#section-functor-with-support)
      - [Local cohomology](#local-cohomology)
        - [Long exact sequence for local cohomology](#long-exact-sequence-for-local-cohomology)
        - [Local cohomology of the affine plane supported at the origin](#local-cohomology-of-the-affine-plane-supported-at-the-origin)
  - [Sheaf cohomology](#sheaf-cohomology)
    - [Coherent cohomology](#coherent-cohomology)
      - [Finiteness of coherent cohomology on projective varieties](#finiteness-of-coherent-cohomology-on-projective-varieties)
    - [Cohomology sheaf](#cohomology-sheaf)
      - [Cohomology-sheaf exact sequence](#cohomology-sheaf-exact-sequence)
    - [Grauert base change theorem](#grauert-base-change-theorem)
    - [Hypercohomology](#hypercohomology)
    - [Acyclic resolution theorem](#acyclic-resolution-theorem)
    - [Locally vanishing principle for sheaf cohomology](#locally-vanishing-principle-for-sheaf-cohomology)
    - [Holomorphic first cohomology of punctured complex two-space](#holomorphic-first-cohomology-of-punctured-complex-two-space)
    - [Castelnuovo–Mumford regularity](#castelnuovo-mumford-regularity)
    - [Injective resolution of sheaves](#injective-resolution-of-sheaves)
    - [Euler characteristic of a coherent sheaf](#euler-characteristic-of-a-coherent-sheaf)
      - [Asymptotic Riemann–Roch](#asymptotic-riemann-roch)
    - [Serre vanishing](#serre-vanishing)
      - [Uniform high-degree vanishing on a smooth projective curve](#uniform-high-degree-vanishing-on-a-smooth-projective-curve)
      - [Uniform Serre vanishing for two ample twists](#uniform-serre-vanishing-for-two-ample-twists)
        - [Higher cohomology vanishing from an ample hyperplane restriction](#higher-cohomology-vanishing-from-an-ample-hyperplane-restriction)
      - [Fujita vanishing](#fujita-vanishing)
        - [Cohomology growth for nef twists](#cohomology-growth-for-nef-twists)
          - [Top cohomology boundedness for nef twists](#top-cohomology-boundedness-for-nef-twists)
    - [Grothendieck vanishing](#grothendieck-vanishing)
    - [Resolution principle for sheaf cohomology](#resolution-principle-for-sheaf-cohomology)
    - [Leray spectral sequence](#leray-spectral-sequence)
    - [Flasque sheaf](#flasque-sheaf)
      - [Sheafification of an injective module is flasque](#sheafification-of-an-injective-module-is-flasque)
      - [Flasque-kernel section-lifting lemma](#flasque-kernel-section-lifting-lemma)
      - [Flasque resolution](#flasque-resolution)
        - [Godement resolution](#godement-resolution)
    - [Čech cohomology](#cech-cohomology)
      - [Cohomology of twists on projective space](#cohomology-of-twists-on-projective-space)
      - [Čech cohomology of the punctured affine plane](#cech-cohomology-of-the-punctured-affine-plane)
      - [Čech cohomology of twists on the projective line](#cech-cohomology-of-twists-on-the-projective-line)
        - [Holomorphic Laurent-series cohomology of twists on the projective line](#holomorphic-laurent-series-cohomology-of-twists-on-the-projective-line)
      - [Čech cohomology of an affine cover can differ from sheaf cohomology](#cech-cohomology-of-an-affine-cover-can-differ-from-sheaf-cohomology)
      - [Čech-de Rham double complex](#cech-de-rham-double-complex)
      - [Čech lifting below the first possible local cohomology degree](#cech-lifting-below-the-first-possible-local-cohomology-degree)
      - [Čech cochain complex](#cech-cochain-complex)
        - [Čech differential](#cech-differential)
        - [Čech resolution on a semi-separated scheme](#cech-resolution-on-a-semi-separated-scheme)
        - [Exactness of the unit-ideal localization Čech complex](#exactness-of-the-unit-ideal-localization-cech-complex)
        - [Čech cochain group](#cech-cochain-group)
        - [Čech cocycle condition](#cech-cocycle-condition)
        - [Čech coboundary](#cech-coboundary)
      - [Leray's theorem](#leray-s-theorem)
        - [Cohomology under a closed immersion](#cohomology-under-a-closed-immersion)
        - [Cohomological dimension bound from an affine cover](#cohomological-dimension-bound-from-an-affine-cover)
    - [Fine sheaf](#fine-sheaf)
    - [Mayer-Vietoris sequence for sheaf cohomology](#mayer-vietoris-sequence-for-sheaf-cohomology)
    - [Long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology)
    - [Serre duality](#serre-duality)
      - [Dualizing sheaf on a smooth projective curve](#dualizing-sheaf-on-a-smooth-projective-curve)
        - [Residue trace on a smooth projective curve](#residue-trace-on-a-smooth-projective-curve)
      - [Residue duality on the projective line](#residue-duality-on-the-projective-line)
      - [Failure of ordinary sheaf-dual Serre duality for a skyscraper sheaf](#failure-of-ordinary-sheaf-dual-serre-duality-for-a-skyscraper-sheaf)
      - [Serre duality for compact complex manifolds](#serre-duality-for-compact-complex-manifolds)
- [Locally ringed space](#locally-ringed-space)
  - [Morphism of locally ringed spaces](#morphism-of-locally-ringed-spaces)
  - [Scheme](#scheme)
    - [Functor represented by a scheme](#functor-represented-by-a-scheme)
    - [Gluing of schemes along open subschemes](#gluing-of-schemes-along-open-subschemes)
    - [Formal scheme](#formal-scheme)
      - [Formal completion of a scheme](#formal-completion-of-a-scheme)
        - [Formal completion commutes with restriction to an open subscheme](#formal-completion-commutes-with-restriction-to-an-open-subscheme)
      - [Formal spectrum](#formal-spectrum)
    - [Smooth morphism](#smooth-morphism)
    - [Étale morphism](#etale-morphism)
      - [Finite étale morphism](#finite-etale-morphism)
    - [Quasi-compact scheme](#quasi-compact-scheme)
    - [Open subscheme](#open-subscheme)
    - [Irreducible scheme](#irreducible-scheme)
    - [Dimension of a scheme](#dimension-of-a-scheme)
    - [Structure morphism](#structure-morphism)
    - [Scheme of characteristic p](#scheme-of-characteristic-p)
      - [Absolute Frobenius morphism](#absolute-frobenius-morphism)
        - [Frobenius factorization through a finite normal cover](#frobenius-factorization-through-a-finite-normal-cover)
    - [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)
      - [Idempotent–clopen correspondence](#idempotent-clopen-correspondence)
      - [Sheaf of units of the structure sheaf](#sheaf-of-units-of-the-structure-sheaf)
      - [Regular function](#regular-function)
        - [Global regular function](#global-regular-function)
          - [Global regular functions on an irreducible projective variety](#global-regular-functions-on-an-irreducible-projective-variety)
          - [Regular functions on the punctured affine plane](#regular-functions-on-the-punctured-affine-plane)
    - [Reduced scheme](#reduced-scheme)
      - [Generic reducedness with no embedded components](#generic-reducedness-with-no-embedded-components)
      - [Integral scheme](#integral-scheme)
        - [Generic-point embedding of regular functions](#generic-point-embedding-of-regular-functions)
    - [Group scheme](#group-scheme)
      - [Homomorphism of group schemes](#homomorphism-of-group-schemes)
      - [Multiplication-by-n morphism](#multiplication-by-n-morphism)
    - [Nonreduced scheme](#nonreduced-scheme)
      - [Nonreduced double point](#nonreduced-double-point)
    - [Punctual scheme](#punctual-scheme)
    - [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)
      - [Spectrum map for the complexification of a real polynomial ring](#spectrum-map-for-the-complexification-of-a-real-polynomial-ring)
      - [Disconnected reduced spectrum product decomposition](#disconnected-reduced-spectrum-product-decomposition)
      - [Affine scheme](#affine-scheme)
        - [Affine gluing along closed subschemes](#affine-gluing-along-closed-subschemes)
        - [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)
          - [Unit-ideal certificate from a principal affine cover](#unit-ideal-certificate-from-a-principal-affine-cover)
          - [Affine principal neighbourhoods from ideal-sheaf vanishing](#affine-principal-neighbourhoods-from-ideal-sheaf-vanishing)
          - [Ideal-sheaf vanishing for a coherent submodule of a trivial bundle](#ideal-sheaf-vanishing-for-a-coherent-submodule-of-a-trivial-bundle)
        - [Affine scheme reconstruction from global sections](#affine-scheme-reconstruction-from-global-sections)
        - [Affine open subscheme](#affine-open-subscheme)
          - [Affine chart of a variety](#affine-chart-of-a-variety)
        - [Principal open subscheme](#principal-open-subscheme)
          - [Dense principal open inside a dense open subset](#dense-principal-open-inside-a-dense-open-subset)
        - [Affine line](#affine-line)
        - [Affine plane](#affine-plane)
          - [Real affine plane scheme points](#real-affine-plane-scheme-points)
          - [Punctured affine plane](#punctured-affine-plane)
            - [Nonaffineness of a punctured affine plane](#nonaffineness-of-a-punctured-affine-plane)
        - [Affine three-space](#affine-three-space)
          - [Punctured affine three-space](#punctured-affine-three-space)
    - [Noetherian scheme](#noetherian-scheme)
      - [Regular scheme](#regular-scheme)
        - [Regular in codimension one](#regular-in-codimension-one)
      - [Normal scheme](#normal-scheme)
        - [Normalization of an integral scheme](#normalization-of-an-integral-scheme)
        - [Normal variety](#normal-variety)
          - [Normal surface singularity](#normal-surface-singularity)
            - [Rational double point](#rational-double-point)
          - [Normality of a quadratic cone](#normality-of-a-quadratic-cone)
        - [Codimension-two extension of regular functions on a normal variety](#codimension-two-extension-of-regular-functions-on-a-normal-variety)
        - [Serre's criterion for normality](#serre-s-criterion-for-normality)
    - [Morphism of schemes](#morphism-of-schemes)
      - [Graph morphism of schemes](#graph-morphism-of-schemes)
      - [Affine-target adjunction for schemes](#affine-target-adjunction-for-schemes)
      - [Stein factorization](#stein-factorization)
      - [Isomorphism of schemes](#isomorphism-of-schemes)
      - [Fiber product of schemes](#fiber-product-of-schemes)
        - [Scheme-theoretic intersection](#scheme-theoretic-intersection)
        - [Point-lifting property of a scheme fibre product](#point-lifting-property-of-a-scheme-fibre-product)
        - [Scheme-theoretic fibre](#scheme-theoretic-fibre)
          - [Nonaffine special fibre obtained by blowing up](#nonaffine-special-fibre-obtained-by-blowing-up)
          - [Real fourth-power fibre classification](#real-fourth-power-fibre-classification)
          - [Nonreduced reducible fibre between integral schemes](#nonreduced-reducible-fibre-between-integral-schemes)
          - [Integrality of the generic fibre of an affine dominant morphism](#integrality-of-the-generic-fibre-of-an-affine-dominant-morphism)
        - [Universal property of a fibre product](#universal-property-of-a-fibre-product)
        - [Base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes)
          - [Global-section base-change failure in a flat projective family](#global-section-base-change-failure-in-a-flat-projective-family)
          - [Complexification fibres of a real scheme](#complexification-fibres-of-a-real-scheme)
          - [Surjectivity is preserved by base change](#surjectivity-is-preserved-by-base-change)
      - [Locally closed immersion](#locally-closed-immersion)
        - [Open immersion](#open-immersion)
        - [Diagonal morphism](#diagonal-morphism)
          - [Coincidence locus of two scheme morphisms](#coincidence-locus-of-two-scheme-morphisms)
      - [Kähler differential](#kahler-differential)
        - [Kähler differentials under a separable field extension](#kahler-differentials-under-a-separable-field-extension)
        - [Base change for Kähler differentials](#base-change-for-kahler-differentials)
        - [Localization of Kähler differentials](#localization-of-kahler-differentials)
        - [Kähler differentials of a polynomial algebra](#kahler-differentials-of-a-polynomial-algebra)
        - [Universal property of Kähler differentials](#universal-property-of-kahler-differentials)
        - [Conormal module of the diagonal](#conormal-module-of-the-diagonal)
        - [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials)
          - [Conormal sheaf](#conormal-sheaf)
            - [Normal sheaf](#normal-sheaf)
              - [Normal sheaf of a projective complete intersection](#normal-sheaf-of-a-projective-complete-intersection)
            - [Conormal injectivity for a generically smooth Cartier divisor](#conormal-injectivity-for-a-generically-smooth-cartier-divisor)
        - [Transitivity exact sequence for Kähler differentials](#transitivity-exact-sequence-for-kahler-differentials)
        - [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)
          - [Tangent sheaf of a scheme](#tangent-sheaf-of-a-scheme)
          - [Cotangent-sheaf cohomology of projective space](#cotangent-sheaf-cohomology-of-projective-space)
          - [Sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field)
            - [Algebraic cotangent bundle](#algebraic-cotangent-bundle)
            - [Local freeness of differentials on a smooth variety](#local-freeness-of-differentials-on-a-smooth-variety)
          - [Canonical line bundle of a smooth variety](#canonical-line-bundle-of-a-smooth-variety)
            - [Canonical divisor of a smooth variety](#canonical-divisor-of-a-smooth-variety)
              - [Plurigenus](#plurigenus)
                - [Blowup invariance of plurigenera](#blowup-invariance-of-plurigenera)
      - [Affine morphism](#affine-morphism)
        - [Cohomology under an affine morphism](#cohomology-under-an-affine-morphism)
      - [Flat morphism](#flat-morphism)
        - [Finite flat rank over an irreducible scheme](#finite-flat-rank-over-an-irreducible-scheme)
      - [Morphism of finite type](#morphism-of-finite-type)
        - [Quasi-finite morphism](#quasi-finite-morphism)
      - [Universally closed morphism](#universally-closed-morphism)
        - [Projective line with a doubled point](#projective-line-with-a-doubled-point)
      - [Separated morphism](#separated-morphism)
        - [Separated scheme](#separated-scheme)
          - [Separated variety](#separated-variety)
        - [Valuative criterion for separatedness](#valuative-criterion-for-separatedness)
      - [Proper morphism](#proper-morphism)
        - [Complete variety](#complete-variety)
        - [Proper affine morphisms are finite](#proper-affine-morphisms-are-finite)
        - [Properness descends from a surjective source](#properness-descends-from-a-surjective-source)
        - [Properness cancels through a separated morphism](#properness-cancels-through-a-separated-morphism)
        - [Properness is local on the target](#properness-is-local-on-the-target)
        - [Proper closed-point fibers do not imply properness](#proper-closed-point-fibers-do-not-imply-properness)
        - [Finite complex computing cohomology in a proper flat family](#finite-complex-computing-cohomology-in-a-proper-flat-family)
          - [Cohomology and base change for line bundles on a curve](#cohomology-and-base-change-for-line-bundles-on-a-curve)
          - [Semicontinuity theorem for coherent cohomology](#semicontinuity-theorem-for-coherent-cohomology)
            - [Constancy of line bundle degree in a family](#constancy-of-line-bundle-degree-in-a-family)
        - [Valuative criterion for properness](#valuative-criterion-for-properness)
        - [Projective morphism](#projective-morphism)
          - [Closedness of projection from projective space](#closedness-of-projection-from-projective-space)
            - [Rational-point projection need not be Zariski closed](#rational-point-projection-need-not-be-zariski-closed)
        - [Projective scheme](#projective-scheme)
          - [Proj construction](#proj-construction)
            - [Degree-one generation condition for Proj](#degree-one-generation-condition-for-proj)
            - [Sheaf associated with a graded module](#sheaf-associated-with-a-graded-module)
              - [Tensor compatibility of graded sheafification on degree-one-generated Proj](#tensor-compatibility-of-graded-sheafification-on-degree-one-generated-proj)
              - [Twisting sheaf on Proj](#twisting-sheaf-on-proj)
            - [Irrelevant ideal of a graded ring](#irrelevant-ideal-of-a-graded-ring)
            - [Standard affine open of Proj](#standard-affine-open-of-proj)
              - [Morphism on Proj induced by a graded ring homomorphism](#morphism-on-proj-induced-by-a-graded-ring-homomorphism)
                - [Invariance of Proj under an eventual graded isomorphism](#invariance-of-proj-under-an-eventual-graded-isomorphism)
            - [Relative Proj construction](#relative-proj-construction)
            - [Veronese subring](#veronese-subring)
              - [Veronese embedding](#veronese-embedding)
      - [Closed immersion](#closed-immersion)
        - [Flat closed immersion of finite presentation](#flat-closed-immersion-of-finite-presentation)
        - [Closed immersion criterion for affine schemes](#closed-immersion-criterion-for-affine-schemes)
        - [Nilpotent thickening](#nilpotent-thickening)
        - [Closed subscheme](#closed-subscheme)
          - [Infinitesimal neighbourhood of a closed subscheme](#infinitesimal-neighbourhood-of-a-closed-subscheme)
          - [Projective complete intersection](#projective-complete-intersection)
            - [Unmixedness of a complete intersection](#unmixedness-of-a-complete-intersection)
            - [Global regular functions on a positive-dimensional projective complete intersection](#global-regular-functions-on-a-positive-dimensional-projective-complete-intersection)
            - [Intermediate cohomology vanishing for a projective complete intersection](#intermediate-cohomology-vanishing-for-a-projective-complete-intersection)
          - [Construction of a closed subscheme from a quasi-coherent ideal](#construction-of-a-closed-subscheme-from-a-quasi-coherent-ideal)
          - [Ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme)
            - [Ideal sheaf of a closed point](#ideal-sheaf-of-a-closed-point)
              - [Ideal sheaf of two closed points](#ideal-sheaf-of-two-closed-points)
            - [Rank bound for locally free ideals on reduced schemes](#rank-bound-for-locally-free-ideals-on-reduced-schemes)
          - [Structure-sheaf sequence of a hypersurface](#structure-sheaf-sequence-of-a-hypersurface)
          - [Reduced induced subscheme](#reduced-induced-subscheme)
          - [Scheme-theoretic image](#scheme-theoretic-image)
    - [Affine plane with doubled origin](#affine-plane-with-doubled-origin)
    - [Semi-separated scheme](#semi-separated-scheme)
      - [Exact direct image from an affine open in a semi-separated scheme](#exact-direct-image-from-an-affine-open-in-a-semi-separated-scheme)
- [Direct image functor](#direct-image-functor)
- [Inverse image functor](#inverse-image-functor)
- [Valuative criterion](#valuative-criterion)

## Morphism of ringed spaces

↑ **Parent:** [Ringed space](ringed-space.md)

A morphism of ringed spaces $f:(X,\mathcal O_X)\to(Y,\mathcal O_Y)$ consists of a continuous map $f:X\to Y$ and a morphism of [sheaves of rings](#sheaf-of-rings) $f^{-1}\mathcal O_Y\to\mathcal O_X$.

## Sheaf of rings

↑ **Parent:** [Ringed space](ringed-space.md)

A sheaf of rings assigns a ring $\mathcal O(U)$ to every open set, restriction homomorphisms to inclusions, and satisfies local identity and gluing. It supplies the local functions on a [ringed space](ringed-space.md).

This is a ring-valued [Sheaf (mathematics)](algebraic-geometry.md#sheaf-mathematics), with ring homomorphisms as restriction maps.

### Sheaf of topological rings

↑ **Parent:** [Sheaf of rings](#sheaf-of-rings)

A [sheaf of topological rings](#sheaf-of-topological-rings) takes values in [topological rings](commutative-algebra.md#topological-ring), with continuous restriction maps. For an open cover, the sheaf condition is an equalizer of the product of sections on the cover and the product on pairwise overlaps, in the category of [topological rings](commutative-algebra.md#topological-ring). The structure sheaf of a [formal scheme](#formal-scheme) is an [inverse limit](module-theory.md#inverse-limit) of discrete structure sheaves with this topology.

// Target: algebra.bigb

## Sheaf of modules

↑ **Parent:** [Ringed space](ringed-space.md)

For a [ringed space](ringed-space.md) $(X,\mathcal O_X)$, a sheaf of $\mathcal O_X$-modules is a sheaf $\mathcal F$ such that every $\mathcal F(U)$ is an $\mathcal O_X(U)$-module and restriction maps preserve scalar multiplication.

The underlying object is a [Sheaf (mathematics)](algebraic-geometry.md#sheaf-mathematics) with compatible local module actions.

### Internal Hom sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

For [sheaves of modules](#sheaf-of-modules) $\mathcal F,\mathcal G$ on a [ringed space](ringed-space.md), the internal Hom sheaf assigns to an open $U$ the module of [sheaf morphisms](algebraic-geometry.md#morphism-of-sheaves) $\mathcal F|_U\to\mathcal G|_U$ respecting $\mathcal O_U$. Compatible morphisms glue, so this is a sheaf. Its [global sections](#global-section) are precisely the global module-sheaf morphisms. For a [locally free sheaf](#locally-free-sheaf) $\mathcal F$ of finite rank it is $\mathcal F^\vee\otimes\mathcal G$.

### Local system

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_system)

A local system is a locally constant [sheaf](algebraic-geometry.md#sheaf-mathematics) of modules, for example the integral cohomology of fibres of a [smooth proper family of compact complex manifolds](complex-geometry.md#smooth-proper-family-of-compact-complex-manifolds). Parallel continuation around loops gives its [monodromy](complex-analysis.md#monodromy) representation.

### Rational section of a sheaf of modules

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

A rational section is a section on a dense [open subset](topology.md#open-set), with two representatives identified when they agree on a common dense [open subset](topology.md#open-set). Intersecting representatives' domains defines addition. Multiplication by a similarly represented [rational function on an algebraic variety](algebraic-geometry.md#rational-function-on-an-algebraic-variety) makes these classes a module over the ring $\operatorname{Rat}(X)$. For an [irreducible variety](algebraic-geometry.md#irreducible-variety), this ring is its [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety).

#### Rational principal part

↑ **Parent:** [Rational section of a sheaf of modules](#rational-section-of-a-sheaf-of-modules)

For a [locally free sheaf](#locally-free-sheaf) on an [irreducible variety](algebraic-geometry.md#irreducible-variety), the stalk inclusion identifies sections regular near $P$ inside its [rational sections](#rational-section-of-a-sheaf-of-modules). The quotient records the obstruction to regularity at that point. This definition does not assume a nonsingular point or a discrete valuation parameter.

##### Rational principal-parts resolution on an algebraic curve

↑ **Parent:** [Rational principal part](#rational-principal-part)

On an irreducible algebraic curve, let $\mathcal R(\mathcal F)$ be the constant rational-section sheaf and put $\mathcal P(\mathcal F)(U)=\bigoplus_{P\in U}\operatorname{Rat}(\mathcal F)/\mathcal F_P$. Every [open subset](topology.md#open-set) is [quasi-compact](topology.md#compact-space), so compatible finite-support families glue with finite support. Its stalk at $P$ is the displayed rational-principal-part quotient. A rational section is regular outside finitely many points, making its principal-part map well defined. The resulting sequence is stalkwise exact. Both right-hand sheaves are [flasque](#flasque-sheaf), and consequently $H^1(X,\mathcal F)$ is the cokernel of the global principal-part map and $H^q(X,\mathcal F)=0$ for $q\ge2$. The curve and Zariski-topology hypotheses distinguish finite support here from locally finite pole sets in complex analysis.

###### Affine principal-parts interpolation for a locally free sheaf

↑ **Parent:** [Rational principal-parts resolution on an algebraic curve](#rational-principal-parts-resolution-on-an-algebraic-curve)

Let $X$ be an irreducible [affine curve](algebraic-geometry.md#affine-algebraic-curve), $A=k[X]$, $K=\operatorname{Frac}A$, and $\mathcal F=\widetilde M$ be [locally free](#locally-free-sheaf). Given finitely many classes in $M_K/M_{\mathfrak m_P}$, choose one nonzero $a\in A$ clearing denominators of representatives. The ring $A/(a)$ is [Artinian](algebra.md#artinian-ring) and is the product of its finitely many local factors. Hence $M/aM\cong\bigoplus_{P\in V(a)}(M/aM)_{\mathfrak m_P}$. Prescribe $av_P$ modulo $aM_{\mathfrak m_P}$ at the requested points and zero at the other zeros of $a$. Lift this tuple to $w\in M$; the section $w/a$ has exactly the requested rational principal parts and no others. This proves surjectivity without assuming the curve is nonsingular.

#### Stalk inclusion into rational sections of a locally free sheaf

↑ **Parent:** [Rational section of a sheaf of modules](#rational-section-of-a-sheaf-of-modules)

On an [irreducible variety](algebraic-geometry.md#irreducible-variety), every nonempty [open subset](topology.md#open-set) is dense, so a [germ](#germ-of-a-sheaf-section) determines a [rational section](#rational-section-of-a-sheaf-of-modules). For a [locally free sheaf](#locally-free-sheaf), this map is injective: a local section which vanishes on a dense open has all its regular coefficient functions zero, hence is zero. Local freeness is important; a section of a torsion sheaf can vanish generically without having zero [germ](#germ-of-a-sheaf-section).

### Coherent analytic sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

On a [complex manifold](complex-geometry.md#complex-manifold), a sheaf of modules over the [sheaf of holomorphic functions](complex-geometry.md#structure-sheaf-of-a-complex-manifold) is coherent analytic if it is locally finitely generated and the kernel of every morphism $\mathcal O^r\to\mathcal F$ is locally finitely generated. The structure sheaf and locally free finite-rank sheaves are examples. [Cartan theorem B](complex-geometry.md#cartan-theorem-b) gives vanishing of their higher [sheaf cohomology](#sheaf-cohomology) on a [Stein manifold](complex-geometry.md#stein-manifold).

### Dual of a sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

The dual is the [sheaf of modules](#sheaf-of-modules) whose sections on $U$ are module-sheaf morphisms $\mathcal F|_U\to\mathcal O_U$. For a [locally free sheaf](#locally-free-sheaf) of finite rank, the dual is locally free of the same rank and the natural double-dual map is an isomorphism. General [coherent sheaves](#coherent-sheaf) need not have this property: a skyscraper at a point of positive-dimensional projective space has zero ordinary sheaf dual.

### Injective sheaf of modules

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

On a [ringed space](ringed-space.md) $(X,\mathcal O_X)$, an injective module sheaf is an [injective object](category-theory.md#injective-object) in the category of [sheaves of modules](#sheaf-of-modules) over $\mathcal O_X$. Its defining extension property concerns module-sheaf morphisms; it is distinct from injectivity solely in the category of [sheaves of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups).

#### Injective module sheaves are flasque

↑ **Parent:** [Injective sheaf of modules](#injective-sheaf-of-modules)

For opens $U\subseteq V\subseteq X$, there is a monomorphism between the [extensions by zero](#extension-by-zero) of $\mathcal O_U$ and $\mathcal O_V$. Morphisms from these sheaves into an [injective sheaf of modules](#injective-sheaf-of-modules) $I$ identify with sections on $U$ and $V$, respectively. The [injective object](category-theory.md#injective-object) extension property therefore makes the restriction $I(V)\to I(U)$ surjective, proving that $I$ is [flasque](#flasque-sheaf). The argument applies to any [ringed space](ringed-space.md).

### Stalk of a sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stalk_of_a_sheaf)

The stalk $\mathcal F_x$ is the direct limit of $\mathcal F(U)$ over neighborhoods $U$ of $x$. A morphism of sheaves is an isomorphism or forms an exact sequence exactly when it does so on every stalk.

#### Costalk

↑ **Parent:** [Stalk of a sheaf](#stalk-of-a-sheaf)

The derived [costalk](#costalk) at $x$ is $i_x^!E$, where $i_x:\{x\}\hookrightarrow X$. It computes local [cohomology](cohomology.md) supported at $x$. On an oriented $N$-manifold the constant [sheaf](algebraic-geometry.md#sheaf-mathematics) has [costalk](#costalk) $\mathbb Q[-N]$, whose [cohomology](cohomology.md) is in degree $N$.

#### Stalk functor for presheaves of sets

↑ **Parent:** [Stalk of a sheaf](#stalk-of-a-sheaf)

For presheaves of sets, $F_x=\varinjlim_{U\ni x}F(U)$. This functor preserves finite limits because the neighborhood system is filtered and [filtered colimits commute with finite limits in sets](category.md#filtered-colimits-commute-with-finite-limits-in-sets). Its right adjoint sends a set $S$ to the presheaf taking the value $S$ on opens containing $x$ and the singleton on other opens.

##### Joint stalk functor on sheaves of sets

↑ **Parent:** [Stalk functor for presheaves of sets](#stalk-functor-for-presheaves-of-sets)

The joint stalk functor $\mathbf{Sh}(X)\to\mathbf{Set}^X$ is faithful: equality of germs makes two images of a section locally equal, and the sheaf uniqueness axiom makes them globally equal. Its right adjoint is the product of the set-valued skyscraper sheaves at all points. The [Beck comonadicity theorem](category-theory.md#beck-comonadicity-theorem) then makes the joint stalk functor comonadic.

#### Skyscraper sheaf

↑ **Parent:** [Stalk of a sheaf](#stalk-of-a-sheaf)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skyscraper_sheaf)

For a point inclusion $i:\{x\}\hookrightarrow X$ and an [abelian group](group.md#abelian-group) $A$, the skyscraper sheaf $i_*A$ has sections $A$ on opens containing $x$ and zero on other opens. Its restriction maps are identities or maps to zero. If $A\ne0$, its nonzero [stalks](#stalk-of-a-sheaf) occur at every point of the closure $\overline{\{x\}}$: exactly those points whose every neighbourhood contains $x$. Thus the familiar assertion that only the stalk at $x$ is nonzero requires $x$ to be a [closed point](topology.md#closed-point). It is always [flasque](#flasque-sheaf), giving the stated [skyscraper sheaf cohomology](#skyscraper-sheaf-cohomology).

##### Skyscraper sheaf cohomology

↑ **Parent:** [Skyscraper sheaf](#skyscraper-sheaf)

For any point inclusion $i:\{x\}\hookrightarrow X$, the [skyscraper sheaf](#skyscraper-sheaf) $i_*A$ has restriction maps that are identities or maps to zero. It is [flasque](#flasque-sheaf), so its higher [sheaf cohomology](#sheaf-cohomology) vanishes and its [global sections](#global-section) are $A$. This requires no assumption that $x$ is closed.

#### Germ of a sheaf section

↑ **Parent:** [Stalk of a sheaf](#stalk-of-a-sheaf)

The germ $s_x$ of a section $s\in\mathcal F(U)$ is its image in the [stalk of a sheaf](#stalk-of-a-sheaf) $\mathcal F_x$. It is zero exactly when $s$ restricts to zero on some neighbourhood of $x$.

##### Support of a sheaf section

↑ **Parent:** [Germ of a sheaf section](#germ-of-a-sheaf-section)

The support of a sheaf section is the closed set

$$
\operatorname{Supp}s=\{x:s_x\ne0\}.
$$

Its complement is open because a zero [germ of a sheaf section](#germ-of-a-sheaf-section) is represented by a section that vanishes on a neighbourhood.

### Sheafification

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sheafification)

Sheafification associates a sheaf to a presheaf without changing its stalks and is universal among morphisms from that presheaf to sheaves.

#### Universal property of sheafification

↑ **Parent:** [Sheafification](#sheafification)

Every [presheaf morphism](algebraic-geometry.md#morphism-of-presheaves) from $\mathcal F$ to a [sheaf](algebraic-geometry.md#sheaf-mathematics) $\mathcal H$ factors uniquely through the canonical [sheafification](#sheafification) map. Local representatives give local images in $\mathcal H$, and the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom) makes their union unique.

#### Sheafification by locally representable germs

↑ **Parent:** [Sheafification](#sheafification)

For a [presheaf](algebraic-geometry.md#presheaf-of-sets-on-a-topological-space), take families of elements of its [stalks](#stalk-of-a-sheaf) which near each point are the [germs](#germ-of-a-sheaf-section) of one [presheaf](algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) section. Pointwise operations and restriction make these families into a [sheaf](algebraic-geometry.md#sheaf-mathematics). The map sending a section to all its [germs](#germ-of-a-sheaf-section) is its [sheafification](#sheafification) map.

### Extension by zero

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extension_by_zero)

For an open inclusion $j:U\hookrightarrow X$, extension by zero is the sheaf $j_!\mathcal F$ whose stalk equals $\mathcal F_x$ on $U$ and zero outside $U$. Its sections are local sections on $U$ whose support is closed in the ambient open set.

### Quasi-coherent sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-coherent_sheaf)

A sheaf of modules on a scheme is quasi-coherent when every affine chart $\operatorname{Spec}A$ restricts it to the sheaf associated with an $A$-module. On an affine scheme it is determined by its module of global sections.

#### Kernels of quasi-coherent sheaf morphisms

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

On an [affine scheme](#affine-scheme), a morphism between [quasi-coherent sheaves](#quasi-coherent-sheaf) is determined by the induced map on [global sections](#global-section), because its maps on [principal open subsets](#principal-open-subscheme) are their [localizations](commutative-algebra.md#localization-of-a-ring). [Exactness of localization](commutative-algebra.md#exactness-of-localization) gives the displayed identity. Thus the [kernel sheaf](algebraic-geometry.md#kernel-sheaf) of a morphism between [quasi-coherent sheaves](#quasi-coherent-sheaf) is quasi-coherent on an arbitrary scheme, by applying the affine argument locally. No finite generation is needed.

#### Affine module sheaf

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

For an [affine variety](algebraic-geometry.md#affine-algebraic-set) with [coordinate ring](algebraic-geometry.md#coordinate-ring) $A$ and an $A$-module $M$, [localization](commutative-algebra.md#localization-of-a-ring) defines sections on [principal open subsets](#principal-open-subscheme) by the displayed formula. Restrictions are the natural localization maps. Equivalently, a section is a family of [stalk](#stalk-of-a-sheaf) values which locally come from one fraction $m/f^r$. These data form a [quasi-coherent sheaf](#quasi-coherent-sheaf), with [global sections](#global-section) $M$ and stalk $M_{\mathfrak m_P}$ at $P$. Sheaf [tensor products](linear-algebra.md#tensor-product) correspond to tensor products over $A$; [pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules) corresponds to extension of scalars, and affine [direct image](#direct-image-sheaf) to restriction of scalars.

##### Coherence of an affine module sheaf

↑ **Parent:** [Affine module sheaf](#affine-module-sheaf)

For a [Noetherian ring](algebra.md#noetherian-ring) $A$, a [finitely generated module](module-theory.md#finitely-generated-module) $M$ has a [finite presentation of a module](module-theory.md#finite-presentation-of-a-module), and kernels of maps from [finite free modules](module-theory.md#finite-free-module) to $M$ are finitely generated. Its [affine module sheaf](#affine-module-sheaf) is therefore a [coherent sheaf](#coherent-sheaf). Conversely, if $\widetilde M$ is coherent, choose a finite [principal open subset](#principal-open-subscheme) cover on which its section [modules](module-theory.md#module-mathematics) are finitely generated. Lift their finitely many generators to numerators in $M$. The [submodule](module-theory.md#submodule) generated by these numerators becomes all of $M$ on every chart, and hence is all of $M$: its quotient has zero [localization](commutative-algebra.md#localization-of-a-ring) at every point. This proves finite generation without assuming that [global sections](#global-section) preserve arbitrary [sheaf](algebraic-geometry.md#sheaf-mathematics) [surjections](algebra.md#surjective-function).

#### Quasi-coherent sheaves are closed under extensions

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

In $0\to\mathcal F\to\mathcal G\to\mathcal E\to0$, assume the outer sheaves are quasi-coherent. On an affine open, any section of $\mathcal E$ has local lifts to $\mathcal G$ on a finite principal cover. Their differences are a Čech cocycle in the module defining $\mathcal F$. Exactness of the unit-ideal localization Čech complex makes this cocycle a coboundary, so adjusted lifts glue. Thus sections are exact on the affine open and on every principal open in it. Comparing the resulting sequences after localization, the outer isomorphisms force the middle localization map to be an isomorphism. Hence $\mathcal G$ is associated with its global-section module and is quasi-coherent.

#### Global-section localization for quasi-coherent sheaves

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

Choose a finite cover of an affine scheme by principal opens on which the quasi-coherent sheaf is associated with a module. The sheaf gluing axiom expresses global sections as the kernel of the difference map from the finite product of chart sections to the finite product of overlap sections. Localization commutes with kernels and finite products. Localizing at $a$ therefore gives the same kernel for the cover intersected with $D(a)$, proving the formula. The principal-open formulas identify the sheaf with that associated with its global-section module; no finite-generation hypothesis on the module is needed.

#### Affine module-sheaf equivalence

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

On an [affine variety](algebraic-geometry.md#affine-algebraic-set) or [affine scheme](#affine-scheme) with [coordinate ring](algebraic-geometry.md#coordinate-ring) $A$, the [global section functor](#global-section-functor) and $M\mapsto\widetilde M$ are inverse equivalences between [modules](module-theory.md#module-mathematics) and [quasi-coherent sheaves](#quasi-coherent-sheaf). On every [principal open subset](#principal-open-subscheme), sections are the appropriate [localization of a module](commutative-algebra.md#localization-of-a-module). [Localization](commutative-algebra.md#localization-of-a-ring) detects exactness at maximal ideals, so these functors are exact even for [modules](module-theory.md#module-mathematics) which are not finitely generated.

#### Torsion-free sheaf

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

On an integral scheme, a [quasi-coherent sheaf](#quasi-coherent-sheaf) is torsion-free when its [module](module-theory.md#module-mathematics) on every [affine chart](#affine-chart-of-a-variety) is a [torsion-free module](module-theory.md#torsion-free-module) over that chart's [integral domain](commutative-algebra.md#integral-domain). It embeds into its generic fibre. Therefore a torsion-free sheaf with zero generic fibre is zero; [locally free sheaves](#locally-free-sheaf) and their subsheaves are torsion-free.

#### Vanishing of quasi-coherent cohomology on an affine scheme

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)

Every [quasi-coherent sheaf](#quasi-coherent-sheaf) on an [affine scheme](#affine-scheme) has zero higher [sheaf cohomology](#sheaf-cohomology). Together with the equivalence between modules and quasi-coherent sheaves on an affine scheme, this makes [affine varieties](algebraic-geometry.md#affine-algebraic-set) the basic acyclic pieces for computing cohomology. An affine [open cover](topology.md#open-cover) of a [separated scheme](#separated-scheme) has affine finite intersections, so the [acyclic cover theorem](#leray-s-theorem) identifies its [Čech cohomology](#cech-cohomology) with sheaf cohomology.

#### Coherent sheaf

↑ **Parent:** [Quasi-coherent sheaf](#quasi-coherent-sheaf)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coherent_sheaf)

On a locally Noetherian scheme, a coherent sheaf is a [quasi-coherent sheaf](#quasi-coherent-sheaf) that is locally associated with a finitely generated module. Kernels, cokernels, and finite direct sums of coherent sheaves remain coherent.

##### Globally generated sheaf

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

A sheaf of modules is globally generated when the evaluation map from its [global sections](#global-section) is surjective. Equivalently, the germs of global sections span each stalk as a module over the local ring. For a [coherent sheaf](#coherent-sheaf) on a [projective variety](projective-space.md#projective-variety), every sufficiently positive twist is globally generated: embed the variety in projective space, present its direct-image sheaf as a quotient of a finite sum of $\mathcal O(-a)$, twist until those line bundles are globally generated, and restrict their generating sections to the variety.

##### Stalkwise isomorphic coherent sheaves need not be isomorphic

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

On $\mathbb P^1_k$, $\mathcal O$ and $\mathcal O(-1)$ are line bundles, so each stalk of either is a free rank-one module over the local ring. Nevertheless their spaces of global sections are $k$ and zero. Indeed a section of $\mathcal O(-1)$ on the two standard charts would require a polynomial $a(t)$ to equal $t^{-1}b(t^{-1})$, which has only strictly negative powers. Only the zero section can satisfy this. Pointwise existence of unrelated stalk isomorphisms does not supply a morphism of sheaves.

##### Coherent ideal sheaf

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

An [ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme) that is a [coherent sheaf](#coherent-sheaf) as a [module](module-theory.md#module-mathematics) over the [structure sheaf](#structure-sheaf-of-a-scheme). On a [Noetherian scheme](#noetherian-scheme), every [quasi-coherent](#quasi-coherent-sheaf) ideal sheaf is coherent.

##### Finite twisting resolution of a coherent sheaf on projective space

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

A [coherent sheaf](#coherent-sheaf) on $\mathbb P_k^n$ is the [sheaf associated with a graded module](#sheaf-associated-with-a-graded-module) for a finite graded $k[t_0,\ldots,t_n]$-module. Choose a finite graded [free resolution](algebra.md#free-resolution) by the [Hilbert syzygy theorem](algebra.md#hilbert-s-syzygy-theorem) and sheafify it; [exactness of localization](commutative-algebra.md#exactness-of-localization) preserves exactness. All terms are finite sums of [twisting sheaves on projective space](#twisting-sheaf-on-projective-space). Twisting sufficiently positively makes every term acyclic in positive degree, and dimension shifting in [long exact sequences in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) proves [Serre vanishing](#serre-vanishing). The graded-module description is supplied by [Stacks Project, Section 30.15](https://stacks.math.columbia.edu/tag/0BXE).

##### Support dimension of a coherent sheaf

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

The support dimension is the [dimension of a scheme](#dimension-of-a-scheme) of the closed support of a [coherent sheaf](#coherent-sheaf). Tensoring with a [line bundle](#line-bundle) leaves its support unchanged. Quotienting by a section that avoids its [associated points](#associated-point-of-a-coherent-sheaf) reduces the support dimension by at least one.

##### Associated point of a coherent sheaf

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

An associated point of a [coherent sheaf](#coherent-sheaf) is a point whose corresponding prime is the annihilator of an element of the module on an affine chart. There are finitely many on a [Noetherian scheme](#noetherian-scheme). A section of a [line bundle](#line-bundle) avoiding them acts injectively on the sheaf, even when the scheme is nonreduced. Over an infinite field a sufficiently ample linear system supplies such a section.

##### Direct image of a coherent sheaf under a closed immersion

↑ **Parent:** [Coherent sheaf](#coherent-sheaf)

If $i:Z\hookrightarrow X$ is a [closed immersion](#closed-immersion) of [Noetherian schemes](#noetherian-scheme) and $\mathcal F$ is a [coherent sheaf](#coherent-sheaf) on $Z$, then $i_*\mathcal F$ is coherent on $X$. Affine-locally this regards a finitely generated $A/I$-module as a finitely generated $A$-module.

### Tensor product of sheaves

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

The tensor product of two sheaves of $\mathcal O_X$-modules is the sheafification of $U\mapsto\mathcal F(U)\otimes_{\mathcal O_X(U)}\mathcal G(U)$. Its stalk at $x$ is $\mathcal F_x\otimes_{\mathcal O_{X,x}}\mathcal G_x$.

### Direct image sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

For a continuous map $f:X\to Y$ and a sheaf $\mathcal F$ on $X$, the direct image is defined by $(f_*\mathcal F)(V)=\mathcal F(f^{-1}V)$ for every open $V\subseteq Y$.

The direct image sheaf is the result of the [direct image functor](#direct-image-functor): $(f_*\mathcal F)(V)=\mathcal F(f^{-1}V)$.

#### Derived direct image of sheaves

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For a continuous map $f:X\to Y$, the derived direct image $Rf_*$ is obtained by applying $f_*$ to an injective resolution. Composition with derived global sections gives $R\Gamma(Y,Rf_*E)\cong R\Gamma(X,E)$.

##### Proper base change for sheaves

↑ **Parent:** [Derived direct image of sheaves](#derived-direct-image-of-sheaves)

For a proper map of locally compact spaces and a constructible complex $E$, the derived stalk satisfies $(Rf_*E)_y\cong R\Gamma(f^{-1}(y),E|_{f^{-1}(y)})$. In particular $(R^if_*\mathbb Q)_y\cong H^i(f^{-1}(y);\mathbb Q)$. Properness is what prevents fibre [cohomology](cohomology.md) from missing nearby sections.

#### Projective direct image need not preserve surjections

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For $f:\mathbb P^1_k\to\operatorname{Spec}k$, let $D$ consist of $0$ and infinity. Its ideal sheaf is $\mathcal O(-2)$, giving an exact coherent sequence $0\to\mathcal O(-2)\to\mathcal O\to\mathcal O_D\to0$. The map on global sections is the diagonal $k\to k\oplus k$, which is not surjective. Since direct image to the point is global sections, projectivity does not make direct image right exact.

#### Coherence reflected by finite direct image

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For a [finite morphism](algebraic-geometry.md#finite-morphism) between [Noetherian schemes](#noetherian-scheme), a [quasi-coherent sheaf](#quasi-coherent-sheaf) is coherent exactly when its [direct image sheaf](#direct-image-sheaf) is coherent. Over an affine target chart, let $B$ be the finite algebra over the target ring $A$, and let $M$ represent the sheaf on $\operatorname{Spec}B$. Finite generation of $M$ over $A$ implies finite generation over $B$, using the same generators; finite generation over $B$ implies finite generation over $A$ because $B$ is finite over $A$.

#### Direct image from an open restriction

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For an open inclusion $j:U\hookrightarrow X$, this [sheaf](algebraic-geometry.md#sheaf-mathematics) has sections $\mathcal F(V\cap U)$ on an open set $V$. Restriction defines $\mathcal F\to{}_U\mathcal F$. Its [stalks](#stalk-of-a-sheaf) outside $U$ may be nonzero, so it differs from [extension by zero](#extension-by-zero).

#### Direct-image tensor comparison

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

Tensoring sections on $f^{-1}V$ gives a balanced pairing of the two [direct image sheaves](#direct-image-sheaf) on $V$. The [universal property of the tensor product of modules](module-theory.md#universal-property-of-the-tensor-product-of-modules) and [sheafification](#sheafification) produce the displayed morphism. Composing with the [pullback-direct-image adjunction unit](#pullback-direct-image-adjunction-unit) gives the [projection formula for sheaves](#projection-formula). The comparison itself need not be an [isomorphism](algebra.md#isomorphism).

#### Sheaf cohomology under a closed inclusion

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For a closed inclusion $i:X\hookrightarrow Y$, [direct image sheaf](#direct-image-sheaf) formation is exact: stalks on $X$ are unchanged and stalks outside $X$ are zero. It also preserves [flasque sheaves](#flasque-sheaf). Pushing forward a [flasque resolution](#flasque-resolution) thus gives a resolution computing cohomology on $Y$, and its complex of [global sections](#global-section) is identical to the original one on $X$. This proves the displayed isomorphism in every nonnegative degree.

#### Direct image of a quasi-coherent sheaf under an affine morphism

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

For an [affine morphism](#affine-morphism) $f:X\to Y$, the direct image of every [quasi-coherent sheaf](#quasi-coherent-sheaf) on $X$ is quasi-coherent. On affine charts this is the fact that restriction of scalars turns the module sheaf $\widetilde M$ into the module sheaf associated with the same underlying module over the target ring.

##### Acyclic direct image from an affine chart of the projective line

↑ **Parent:** [Direct image of a quasi-coherent sheaf under an affine morphism](#direct-image-of-a-quasi-coherent-sheaf-under-an-affine-morphism)

Let $j:\mathbb A^1_k\hookrightarrow\mathbb P^1_k$ be a standard affine chart and $\mathcal G=\widetilde M$ a [quasi-coherent sheaf](#quasi-coherent-sheaf) there. Its direct image is quasi-coherent because $j$ is an [affine morphism](#affine-morphism). The standard two-chart [acyclic cover](topology.md#acyclic-cover) has [Čech cochain complex](#cech-cochain-complex) $M\oplus M_x\to M_x$ in degrees zero and one, with differential $(m,n)\mapsto n-m/1$. Surjectivity gives $H^i(\mathbb P^1_k,j_*\mathcal G)=0$ for $i>0$. This does not assert that the direct image itself is flasque.

#### Quasi-coherence of direct image under a quasi-compact quasi-separated morphism

↑ **Parent:** [Direct image sheaf](#direct-image-sheaf)

If $f:X\to Y$ is quasi-compact and quasi-separated, then the direct image of every [quasi-coherent sheaf](#quasi-coherent-sheaf) on $X$ is again a quasi-coherent sheaf. A finite affine cover of each inverse image of an affine target chart expresses the direct image as the kernel of a morphism between finite sums of quasi-coherent direct images from affine charts.

### Inverse image sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

The inverse image sheaf $f^{-1}\mathcal E$ is the sheaf associated with the presheaf whose sections near $U\subseteq X$ are obtained as a colimit of $\mathcal E(V)$ over open sets $V\supseteq f(U)$.

This is the sheaf obtained by applying the [inverse image functor](#inverse-image-functor).

#### Inverse-image direct-image adjunction

↑ **Parent:** [Inverse image sheaf](#inverse-image-sheaf)

For [sheaves of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups) and a continuous map $f:X\to Y$, there is a natural bijection $\operatorname{Hom}_X(f^{-1}\mathcal G,\mathcal F)\cong\operatorname{Hom}_Y(\mathcal G,f_*\mathcal F)$. It comes from the [universal property of an inverse image sheaf](#universal-property-of-an-inverse-image-sheaf). The inverse image of abelian [sheaves](algebraic-geometry.md#sheaf-mathematics) is different from the tensor-adjusted [pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules) on a [ringed space](ringed-space.md).

#### Universal property of an inverse image sheaf

↑ **Parent:** [Inverse image sheaf](#inverse-image-sheaf)

Every [f-morphism of sheaves](algebraic-geometry.md#f-morphism-of-sheaves) from $\mathcal G$ to $\mathcal F$ factors uniquely through the canonical f-morphism from $\mathcal G$ to its [inverse image sheaf](#inverse-image-sheaf). A local inverse-image section is represented by sections of $\mathcal G$ on image neighbourhoods; their prescribed images glue in $\mathcal F$.

#### Pullback of a sheaf of modules

↑ **Parent:** [Inverse image sheaf](#inverse-image-sheaf)

For a morphism of [ringed spaces](ringed-space.md), the pullback of an $\mathcal O_Y$-module is

$$
f^*\mathcal E=\mathcal O_X\otimes_{f^{-1}\mathcal O_Y}f^{-1}\mathcal E.
$$

The [inverse image functor](#inverse-image-functor) supplies the sheaf $f^{-1}\mathcal E$; tensoring with the source structure sheaf supplies the module scalar extension.

##### Restriction of a module sheaf to a closed subvariety

↑ **Parent:** [Pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules)

The restriction meant here is the [pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules) to the closed subvariety, including tensoring with its structure sheaf. On an [affine chart](#affine-chart-of-a-variety), tensoring $M$ with $A/I$ gives $M/IM$. This distinction matters because restricting only the underlying topological sheaf would retain the ambient ring action.

##### Pullback-direct-image adjunction unit

↑ **Parent:** [Pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules)

For a [morphism of ringed spaces](#morphism-of-ringed-spaces), the [pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules) is left adjoint to the [direct image sheaf](#direct-image-sheaf) functor. The unit sends a local section $h$ to $1\otimes h$ after inverse image. On the [structure sheaf](#structure-sheaf-of-a-scheme) it becomes the given [ring homomorphism](commutative-algebra.md#ring-homomorphism) $\mathcal O_Y\to f_*\mathcal O_X$.

##### Projection formula

↑ **Parent:** [Pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projection_formula)

For a morphism of [ringed spaces](ringed-space.md), there is a natural morphism

$$
f_*\mathcal F\otimes_{\mathcal O_Y}\mathcal E\longrightarrow f_*\bigl(\mathcal F\otimes_{\mathcal O_X}f^*\mathcal E\bigr).
$$

It is an isomorphism when $\mathcal E$ is a [locally free sheaf](#locally-free-sheaf) of finite rank, because the claim is local and then reduces to distributivity over a finite direct sum.

The same formula holds for higher direct images: $R^if_*\mathcal F\otimes\mathcal E\cong R^if_*(\mathcal F\otimes f^*\mathcal E)$ when $\mathcal E$ is locally free of finite rank.

### Locally free sheaf

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

A sheaf of $\mathcal O_X$-modules is locally free of finite rank when every point has an open neighborhood $U$ on which it is isomorphic to $\mathcal O_U^{\oplus r}$ for some finite $r$. If $X$ is connected, the rank is constant.

A sheaf of modules is locally free of rank $r$ if each point has a neighborhood $U$ on which it is isomorphic to $\mathcal O_U^r$. Finite-rank locally free sheaves correspond to [vector bundles](fiber-bundle.md#vector-bundle) in the standard geometric settings.

#### Free sheaf

↑ **Parent:** [Locally free sheaf](#locally-free-sheaf)

A free sheaf of finite rank on a [scheme](#scheme) is a [sheaf of modules](#sheaf-of-modules) globally isomorphic to $\mathcal O_X^{\oplus r}$. A [locally free sheaf](#locally-free-sheaf) only requires such an isomorphism on an open cover; its local frames need not glue to one global frame.

#### Saturated line subbundle on a smooth curve

↑ **Parent:** [Locally free sheaf](#locally-free-sheaf)

A rank-one subsheaf of a [vector bundle](fiber-bundle.md#vector-bundle) on a [smooth algebraic curve](algebraic-geometry.md#smooth-algebraic-curve) is saturated when the quotient is torsion-free. Intersecting a one-dimensional subspace of the generic fibre with each stalk constructs a saturated subsheaf. The [local ring of a smooth algebraic curve](projective-space.md#local-ring-of-a-smooth-algebraic-curve) is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), so the subsheaf and its torsion-free quotient are [locally free](#locally-free-sheaf). Saturating a nonzero map from a [line bundle](#line-bundle) enlarges that line bundle by an [effective divisor](cartier-divisor.md#effective-cartier-divisor), recording the map's zeros.

##### Unbounded negative degrees of line subbundles

↑ **Parent:** [Saturated line subbundle on a smooth curve](#saturated-line-subbundle-on-a-smooth-curve)

For a rank-two bundle $E$, the sufficiently positive twist $E(mp_0)$ is globally generated. The [nowhere-vanishing section of a globally generated bundle on a curve](fiber-bundle.md#nowhere-vanishing-section-of-a-globally-generated-bundle-on-a-curve) gives a subbundle $\mathcal O_C\subset E(mp_0)$. Twisting back produces a genuine [line subbundle](fiber-bundle.md#line-subbundle) of degree $-m$, with [locally free](#locally-free-sheaf) quotient. Thus line-subbundle degrees are bounded above but not below. Merely inserting a negative [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve) into a fixed subline would allow a torsion quotient and would not establish this stronger conclusion.

##### Upper degree bound for line subbundles on a smooth curve

↑ **Parent:** [Saturated line subbundle on a smooth curve](#saturated-line-subbundle-on-a-smooth-curve)

Choose a rational basis of the dual of a [vector bundle](fiber-bundle.md#vector-bundle) and an [effective divisor](cartier-divisor.md#effective-cartier-divisor) $D$ bounding all its poles. Evaluation gives a generically [injective](algebra.md#injective-function) map $E\to\mathcal O_C(D)^{\oplus r}$. A [line subbundle](fiber-bundle.md#line-subbundle) maps nontrivially to at least one summand, so $\mathcal O_C(D)\otimes L^{-1}$ has a nonzero regular section. Consequently $\deg L\le\deg D$. This bound depends on $E$ and the chosen rational frame, and does not require $E$ to be stable.

#### Local splitting when a quotient sheaf is locally free

↑ **Parent:** [Locally free sheaf](#locally-free-sheaf)

In a [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves) $0\to\mathcal F\to\mathcal G\to\mathcal H\to0$, if $\mathcal H$ is [locally free](#locally-free-sheaf) of finite rank, the sequence splits near every point. Trivialize $\mathcal H$, lift its finitely many basis sections locally, and shrink to one neighbourhood on which all lifts exist. The lifts define a splitting. If $\mathcal F$ is also locally free, then so is $\mathcal G$. Conversely locally free kernel and middle term need not give a locally free quotient: multiplication by $t$ on $\mathcal O_{\operatorname{Spec}k[t]}$ has quotient supported at the origin.

#### Line bundle

↑ **Parent:** [Locally free sheaf](#locally-free-sheaf)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Line_bundle)

A line bundle on a [scheme](#scheme) is a [locally free sheaf](#locally-free-sheaf) of rank one. Its global sections can define a morphism to [projective space](projective-space.md) when they have no common zero.

##### Degree of a line bundle

↑ **Parent:** [Line bundle](#line-bundle)

On a smooth projective curve, a nonzero [rational section](#rational-section-of-a-sheaf-of-modules) represents a [line bundle](#line-bundle) by its [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve). The degree is the sum of its vanishing orders minus its pole orders, including residue-field degrees over a nonclosed field. Principal [divisors on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve) have degree zero, so this number is independent of the section. A nonzero regular section gives an [effective divisor](cartier-divisor.md#effective-cartier-divisor) and therefore a nonnegative degree. Degrees add under tensor products and change sign under duality.

##### Half-density

↑ **Parent:** [Line bundle](#line-bundle)

A [half-density](#half-density) transforms by the square root of the absolute Jacobian under a coordinate change. The product of a [half-density](#half-density) with its complex conjugate is an integrable density, so its [norm](functional-analysis.md#norm) is coordinate-independent without choosing a separate volume form. [Half-densities](#half-density) provide an intrinsic configuration-space [Hilbert space](hilbert-space.md) for a real cotangent polarization.

##### Orientation line bundle

↑ **Parent:** [Line bundle](#line-bundle)

The orientation line bundle of a smooth $n$-manifold is the real line bundle $\bigwedge^nTM$. Its transition functions have the signs of the tangent-coordinate transition determinants. A nonzero continuous section specifies an [orientation](algebraic-topology.md#orientation-of-a-simplex) of the manifold. Its orientation double cover records the two possible local orientations.

###### Orientable total space of the orientation line bundle

↑ **Parent:** [Orientation line bundle](#orientation-line-bundle)

The total space of the [orientation line bundle](#orientation-line-bundle) is orientable even when its base is not: an orientation reversal in a base coordinate transition is matched by a reversal in the line coordinate, so their product has positive sign. Fiberwise multiplication by $1-t$ gives a [deformation retraction](algebraic-topology.md#deformation-retraction) onto the zero section. For the real projective plane this total space is $(S^2\times\mathbb R)/((v,t)\sim(-v,-t))$, an oriented noncompact three-manifold homotopy equivalent to the plane.

##### Homogeneous line-bundle representations on the two-sphere

↑ **Parent:** [Line bundle](#line-bundle)

On $S^2=SU(2)/U(1)$ a degree-$q$ equivariant line bundle corresponds to isotropy character $\operatorname{diag}(e^{it},e^{-it})\mapsto e^{-iqt}$. The [Peter-Weyl theorem](representation-theory.md#peter-weyl-theorem) computes its section multiplicities by the occurrence of weight $-q$ in the [SU(2) representation](representation-theory.md#representation-theory-of-su-2) $\operatorname{Sym}^n\mathbb C^2$. Its weights $n,n-2,\ldots,-n$ give the displayed multiplicity-one decomposition. The spinor lines have degrees $-1,+1$ and thus contain all odd $n$, once each.

##### Line bundles trivialized by an open cover

↑ **Parent:** [Line bundle](#line-bundle)

A [line bundle](#line-bundle) trivial on each [open set](topology.md#open-set) is determined by unit-valued transition functions on pairwise intersections. Their [cocycle](algebra.md#cocycle) identities make the local trivial bundles glue; changing frames changes the [cocycle](algebra.md#cocycle) by a [coboundary](algebra.md#coboundary). The [tensor product of sheaves](#tensor-product-of-sheaves) multiplies the transition functions, giving the displayed group [isomorphism](algebra.md#isomorphism) with [Čech cohomology](#cech-cohomology).

##### Globally generated line bundle

↑ **Parent:** [Line bundle](#line-bundle)

A [line bundle](#line-bundle) is globally generated if at each point some [global section](#global-section) has a [germ](#germ-of-a-sheaf-section) generating its [stalk](#stalk-of-a-sheaf) as a module over the [local ring](commutative-algebra.md#local-ring). Equivalently its evaluation map from global sections tensored with the [structure sheaf](#structure-sheaf-of-a-scheme) is surjective.

###### Globally generated line bundle without finite generators

↑ **Parent:** [Globally generated line bundle](#globally-generated-line-bundle)

The displayed line bundle is globally generated, but no finite family of [global sections](#global-section) generates it. A family of $N$ sections restricts to $N$ linear forms on $\mathbb P^m$; for $m\geq N$, these have a common zero. This shows why [finite global generation on a quasi-compact scheme](#finite-global-generation-on-a-quasi-compact-scheme) requires its finiteness hypothesis.

###### Finite global generation on a quasi-compact scheme

↑ **Parent:** [Globally generated line bundle](#globally-generated-line-bundle)

A [globally generated line bundle](#globally-generated-line-bundle) on a [quasi-compact](topology.md#compact-space) scheme is generated by finitely many [global sections](#global-section). Each point has a section generating on an open neighbourhood, and quasi-compactness gives a finite subcover. This supplies a map into a fixed finite-dimensional [projective space](projective-space.md) associated with that line bundle.

###### Tensor product of globally generated line bundles

↑ **Parent:** [Globally generated line bundle](#globally-generated-line-bundle)

The [tensor product](linear-algebra.md#tensor-product) of two [globally generated line bundles](#globally-generated-line-bundle) is globally generated. At a point choose generator germs arising from a global section of each factor. Their tensor is the germ of a global tensor-product section and generates the rank-one tensor-product stalk. Iteration gives the same property for every positive tensor power, on an arbitrary [scheme](#scheme).

##### Rational section of a line bundle

↑ **Parent:** [Line bundle](#line-bundle)

On an [integral scheme](#integral-scheme) with [generic point](algebraic-geometry.md#generic-point) $\eta$ and function field $K$, a rational section of a [line bundle](#line-bundle) $\mathcal L$ is an element of the one-dimensional $K$-space $\mathcal L_\eta$. A nonzero rational section writes as $a_ie_i$ in local trivializations, with $a_i\in K^*$. Ratios of these coefficients are regular units, and therefore define a [Cartier divisor](cartier-divisor.md).

##### Twisting sheaf on projective space

↑ **Parent:** [Line bundle](#line-bundle)

The twisting sheaf $\mathcal O(d)$ on $\operatorname{Proj}k[x_0,\ldots,x_n]$ is associated with the shifted graded module $k[x_0,\ldots,x_n](d)$. For $d\geq0$, its global sections are the homogeneous polynomials of degree $d$.

On projective space the twisting sheaf $\mathcal O(d)$ is the $d$th tensor power of $\mathcal O(1)$ for $d\geq0$, and the corresponding dual power for $d<0$. Twisting another sheaf means tensoring it with this line bundle.

###### Homogeneous rational sections of a twisting sheaf

↑ **Parent:** [Twisting sheaf on projective space](#twisting-sheaf-on-projective-space)

The local frame $X_i^m$ on $X_i\ne0$ identifies a section with a homogeneous rational function of degree $m$ on the punctured affine cone. Homogenizing a local rational expression and cancelling common factors writes every nonzero section as a quotient of coprime [homogeneous polynomials](algebra.md#homogeneous-polynomial) $F/G$ with $\deg F-\deg G=m$. Conversely, such a rational function regular on the cone gives local coefficients $r/X_i^m$, which glue with the twisting sheaf's [transition functions of a vector bundle](fiber-bundle.md#transition-function-of-a-vector-bundle).

###### Laurent-monomial description of top cohomology on projective space

↑ **Parent:** [Twisting sheaf on projective space](#twisting-sheaf-on-projective-space)

For $n\ge1$, the top [Čech cohomology](#cech-cohomology) of the standard affine cover of [projective space](projective-space.md) is the degree-$m$ quotient of the Laurent ring by the sum of rings in which at least one variable has not been inverted. Its basis consists of [Laurent monomials](polynomial.md#laurent-monomial) $X_0^{a_0}\cdots X_n^{a_n}$ with every $a_i<0$ and $\sum_i a_i=m$. Hence it vanishes for $m\ge-n$ and has dimension $\binom{-m-1}{n}$ for $m\le-n-1$.

###### Canonical bundle of projective space

↑ **Parent:** [Twisting sheaf on projective space](#twisting-sheaf-on-projective-space)

Over any field, the [canonical bundle](complex-geometry.md#canonical-bundle) of [projective space](projective-space.md) is $\mathcal O(-n-1)$. Indeed, dualizing the [Euler sequence](algebraic-geometry.md#euler-sequence) gives $0\to\Omega^1_{\mathbf P^n}\to\mathcal O(-1)^{\oplus(n+1)}\to\mathcal O\to0$; taking determinants gives the result. Hence [Serre duality](#serre-duality) identifies $H^i(\mathbf P^n,\mathcal O(m))$ with the dual of $H^{n-i}(\mathbf P^n,\mathcal O(-m-n-1))$.

###### Canonical-form transition on projective space

↑ **Parent:** [Canonical bundle of projective space](#canonical-bundle-of-projective-space)

On the standard charts of [projective space](projective-space.md), wedge the coordinate differentials in increasing order. The change $X_0/X_i=(X_i/X_0)^{-1}$ and $X_j/X_i=(X_j/X_0)/(X_i/X_0)$ gives the displayed [Jacobian determinant](calculus.md#jacobian-determinant). Multiplying the $i$th local generator by $(-1)^i$ removes this sign and yields the transition functions of the [twisting sheaf on projective space](#twisting-sheaf-on-projective-space) with degree $-n-1$.

###### Hyperplane exact sequence for twisting sheaves

↑ **Parent:** [Twisting sheaf on projective space](#twisting-sheaf-on-projective-space)

For a hyperplane $H\subset\mathbf P^n$ with inclusion $i$, multiplication by its defining linear [homogeneous polynomial](algebra.md#homogeneous-polynomial) gives the [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\to\mathcal O_{\mathbf P^n}(m-1)\to\mathcal O_{\mathbf P^n}(m)\to i_*\mathcal O_H(m)\to0.
$$

The [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) relates twists in consecutive degrees and consecutive dimensions. Surjectivity of restriction on global homogeneous polynomials, together with eventual positive-twist vanishing, proves vanishing of intermediate cohomology by descending induction. The top-degree dimensions satisfy $h_n(m-1)=h_n(m)+h_{n-1}(m)$ for $n\geq2$, where $h_r(m)=\dim H^r(\mathbf P^r,\mathcal O(m))$.

###### Top-twist vanishing by hyperplane induction

↑ **Parent:** [Hyperplane exact sequence for twisting sheaves](#hyperplane-exact-sequence-for-twisting-sheaves)

The [hyperplane exact sequence for twisting sheaves](#hyperplane-exact-sequence-for-twisting-sheaves) identifies consecutive top-degree groups whenever the hyperplane's preceding-degree group vanishes. Induction on dimension, starting with the surjective restriction of constants to a point on $\mathbf P^1$, propagates the degree-zero top vanishing down to $m=-n$. Its top-degree surjections also propagate vanishing to every positive twist. This proof does not apply the negative-twist global-section formula to $\mathbf P^0$.

##### Picard group

↑ **Parent:** [Line bundle](#line-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Picard_group)

The Picard group is the group of isomorphism classes of [line bundles](#line-bundle) under tensor product.

###### Picard group of the projective line

↑ **Parent:** [Picard group](#picard-group)

For any [field](algebra.md#field) $k$, degree identifies the [Picard group](#picard-group) of the [projective line](finite-group-theory.md#projective-line) with $\mathbb Z$, generated by $\mathcal O(1)$. A closed point on the affine chart is cut out by an irreducible polynomial $f(t)$, whose [divisor](number-theory.md#divisor) is that point minus $\deg(f)$ times infinity. Hence every divisor is linearly equivalent to its degree times infinity. Principal divisors have degree zero, so the degree map is injective as well as surjective. Thus a [line bundle](#line-bundle) of degree $d$ is $\mathcal O(d)$.

###### Degree-zero Picard group of a curve

↑ **Parent:** [Picard group](#picard-group)

For a [smooth projective curve](projective-space.md#smooth-projective-curve), the degree-zero Picard group consists of [line bundles](#line-bundle) of degree zero up to isomorphism, with tensor product as addition. A nonzero [rational section of a line bundle](#rational-section-of-a-line-bundle) identifies each [line bundle](#line-bundle) with $\mathcal O(D)$ for a [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve); degree is the sum of multiplicities weighted by residue-field degrees. Over an [algebraically closed field](algebra.md#algebraically-closed-field), every degree-zero [divisor](number-theory.md#divisor) is a sum of differences of points.

###### Rational points need not generate the degree-zero Picard group

↑ **Parent:** [Degree-zero Picard group of a curve](#degree-zero-picard-group-of-a-curve)

Let $C$ be the smooth projective model over $\mathbb F_2$ of $y^2+y=x^5+x+1$. Its only rational point is its unique point $p_\infty$ at infinity. At that point $x,y$ have pole orders two and five. The degree-two closed point $D$ defined by $y=0$, $x^2+x+1=0$ gives a nonzero class $[D-2p_\infty]$. Indeed a function with poles bounded by $2p_\infty$ has the form $a+bx$: in the affine coordinate ring every function is uniquely $A(x)+B(x)y$, and the two possible pole orders have opposite parity. No nonzero $a+bx$ vanishes at both roots of $x^2+x+1$. Thus the [Abel map of a pointed smooth projective curve](#abel-map-of-a-pointed-smooth-projective-curve) on rational points has trivial image here, but the [degree-zero Picard group of a curve](#degree-zero-picard-group-of-a-curve) is nontrivial. Generation by point differences needs an algebraically closed field, or closed points with their residue degrees instead of just rational points.

###### Abel map of a pointed smooth projective curve

↑ **Parent:** [Degree-zero Picard group of a curve](#degree-zero-picard-group-of-a-curve)

Given a base point $p_0$, the Abel map takes points of a [smooth projective curve](projective-space.md#smooth-projective-curve) to its [degree-zero Picard group of a curve](#degree-zero-picard-group-of-a-curve). For positive genus it is injective: equality at distinct $p,q$ would give a [principal divisor with one simple zero and one simple pole](algebraic-geometry.md#principal-divisor-with-one-simple-zero-and-one-simple-pole), forcing a degree-one map to the [projective line](finite-group-theory.md#projective-line) and genus zero. For genus one the [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) gives a unique effective degree-one representative of $L(p_0)$ for every degree-zero [line bundle](#line-bundle) $L$, making the map bijective and inducing an [abelian group](group.md#abelian-group) law on the points.

###### Picard functor of a curve

↑ **Parent:** [Picard group](#picard-group)

For a smooth projective geometrically connected [algebraic curve](algebraic-geometry.md#algebraic-curve) $C/k$, this [functor](category.md#functor) assigns to a [scheme](#scheme) $T$ the [line bundles](#line-bundle) on $C\times T$ having degree $d$ on each geometric fibre, modulo bundles pulled back from $T$. One generally takes the associated sheaf for faithfully flat covers. A rational point of $C$ permits normalization of every [line bundle](#line-bundle) along that point; normalized bundles have no automorphisms preserving their normalization and satisfy effective descent. The resulting [functor](category.md#functor) is represented by the degree-$d$ component of the [Picard scheme of a curve](#picard-scheme-of-a-curve).

###### Picard scheme of a curve

↑ **Parent:** [Picard functor of a curve](#picard-functor-of-a-curve)

For a smooth projective [algebraic curve](algebraic-geometry.md#algebraic-curve) of genus $g$, this smooth proper $g$-dimensional [scheme](#scheme) represents degree-$d$ [line bundles](#line-bundle) in families. Charts come from nonspecial degree-$g$ bundles: their first [sheaf cohomology](#sheaf-cohomology) vanishes, so the [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) gives exactly one independent [global section](#global-section), whose zero [Cartier divisor](cartier-divisor.md) varies algebraically. Twisting by fixed [line bundles](#line-bundle) gives charts covering every degree-$d$ class. For degree zero the [tensor product](linear-algebra.md#tensor-product) gives the [Jacobian variety](abelian-variety.md#jacobian-variety); other components are its torsors.

###### Picard charts from nonspecial divisors

↑ **Parent:** [Picard scheme of a curve](#picard-scheme-of-a-curve)

A degree-$g$ [line bundle](#line-bundle) with vanishing first [sheaf cohomology](#sheaf-cohomology) has exactly one section up to scale, by [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem). Its zero divisor is unique and varies in families by [cohomology and base change for line bundles on a curve](#cohomology-and-base-change-for-line-bundles-on-a-curve). For a fixed divisor $B$ of degree $N-g$, the open subset of $C^{(g)}$ where $\mathcal O(E)$ has vanishing first cohomology gives a chart in degree $N$, by $E\mapsto\mathcal O(B+E)$. Different charts are glued by the unique residual divisor of $\mathcal O(B+E-B')$ wherever that line bundle is again nonspecial. Normalizing the universal bundles along a fixed rational point gives their canonical compatible gluing and a representing [scheme](#scheme) for the [Picard functor of a curve](#picard-functor-of-a-curve).

###### Picard group of a ring

↑ **Parent:** [Picard group](#picard-group)

The [Picard group](#picard-group) of a commutative [ring](commutative-algebra.md#ring) $A$ consists of isomorphism classes of finitely generated [projective modules](module-theory.md#projective-module) that have rank one at every [prime ideal](commutative-algebra.md#prime-ideal). Tensor product is the group law, $[A]$ is the identity, and the module dual supplies the inverse. For an [integral domain](commutative-algebra.md#integral-domain), every such module can be represented by an [invertible fractional ideal](commutative-algebra.md#invertible-fractional-ideal) after choosing a basis over the [fraction field](commutative-algebra.md#field-of-fractions).

###### Holomorphic Picard group

↑ **Parent:** [Picard group](#picard-group)

The [holomorphic Picard group](#holomorphic-picard-group) consists of isomorphism classes of [holomorphic line bundles](complex-geometry.md#holomorphic-line-bundle), with [tensor product](linear-algebra.md#tensor-product) as its group law. The trivial bundle is the identity and dualization gives inverses. Transition functions identify it with $H^1(X,\mathcal O_X^*)$. On the [complex projective line](algebraic-topology.md#complex-projective-line) every class is $\mathcal O(n)$, so degree gives an isomorphism with $\mathbb Z$.

###### Picard injection for holomorphic projective bundles

↑ **Parent:** [Holomorphic Picard group](#holomorphic-picard-group)

For a rank-two [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle) on a nonempty [complex manifold](complex-geometry.md#complex-manifold), this map from $\operatorname{Pic}_{\rm hol}(X)\times\mathbb Z$ to $\operatorname{Pic}_{\rm hol}(\mathbb P(E))$ is injective. Fibre degree detects $n$. If $p^*M$ is trivial, a nonvanishing holomorphic section is constant along every compact projective fibre in a local bundle chart, so it descends to a nonvanishing section of $M$. The proof requires no global section of $p$.

###### Picard-group localization on a smooth variety

↑ **Parent:** [Picard group](#picard-group)

For a smooth integral [variety](algebraic-geometry.md#algebraic-variety), every [Weil divisor](algebraic-geometry.md#weil-divisor) is a [Cartier divisor](cartier-divisor.md), so the [Picard group](#picard-group) equals the [divisor class group](algebraic-geometry.md#divisor-class-group). If $U$ is obtained by removing irreducible [Weil divisors](algebraic-geometry.md#weil-divisor) $D_j$, the [localization sequence for the divisor class group](algebraic-geometry.md#localization-sequence-for-the-divisor-class-group) gives the displayed [exact sequence](homology.md#exact-sequence). A rational trivialization of a [line bundle](#line-bundle) on $U$ has divisor supported on the removed divisors, describing the [kernel](linear-algebra.md#kernel-of-a-linear-map) concretely.

###### Cartier-divisor description of the Picard group

↑ **Parent:** [Picard group](#picard-group)

On an [irreducible variety](algebraic-geometry.md#irreducible-variety), a [Cartier divisor](cartier-divisor.md) is a section of $\mathcal K_X^*/\mathcal O_X^*$: its local rational equations differ by regular units. Their ratios define an [invertible sheaf](#line-bundle), and a global rational equation gives the trivial class. Conversely a rational trivialization of an [invertible sheaf](#line-bundle) gives local equations. The rational-function sheaf is [flasque](#flasque-sheaf), so its [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) also identifies the quotient with $H^1(X,\mathcal O_X^*)$.

<h6 id="neron-severi-group">Néron-Severi group</h6>

↑ **Parent:** [Picard group](#picard-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Néron-Severi_group)

The Néron-Severi group is the quotient $\operatorname{Pic}(X)/\operatorname{Pic}^0(X)$ of the [Picard group](#picard-group) by line bundles algebraically equivalent to zero.

##### Very ample line bundle

↑ **Parent:** [Line bundle](#line-bundle)

A line bundle is very ample when its global sections define a closed embedding into [projective space](projective-space.md).

Over a field, a line bundle is very ample when it is the pullback of $\mathcal O(1)$ by a closed immersion into projective space. It is an [ample line bundle](#ample-line-bundle), but an ample bundle need not itself be very ample.

##### Ample line bundle

↑ **Parent:** [Line bundle](#line-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ample_line_bundle)

A [line bundle](#line-bundle) $L$ is ample when some positive [tensor power](linear-algebra.md#tensor-power) $L^{\otimes m}$ is [very ample](#very-ample-line-bundle).

###### Ampleness on reduced components

↑ **Parent:** [Ample line bundle](#ample-line-bundle)

On a [projective scheme](#projective-scheme), a [line bundle](#line-bundle) is [ample](#ample-line-bundle) exactly when its restriction to every reduced irreducible component is [ample](#ample-line-bundle). The disjoint union of those components maps finitely and surjectively to the scheme, so finite-surjective descent of the [finite pullback of an ample line bundle](#finite-pullback-of-an-ample-line-bundle) proves this. The same argument applies to restrictions to any closed subscheme. Thus nilpotent structure does not affect [ampleness](cartier-divisor.md#ample-cartier-divisor).

###### Finite pullback of an ample line bundle

↑ **Parent:** [Ample line bundle](#ample-line-bundle)

For a [finite morphism](algebraic-geometry.md#finite-morphism) $f:X\to Y$, the pullback of an [ample line bundle](#ample-line-bundle) is [ample](#ample-line-bundle). If $f$ is also surjective, [ampleness](cartier-divisor.md#ample-cartier-divisor) is equivalent in both directions. These results hold for proper schemes over a field, including nonreduced schemes. Cohomological [ampleness](cartier-divisor.md#ample-cartier-divisor) and the exact finite pushforward prove the forward direction; coherent-sheaf devissage gives finite-surjective descent. In particular, a finite map to projective space makes the pulled-back hyperplane bundle [ample](#ample-line-bundle).

###### High ample twist is very ample

↑ **Parent:** [Ample line bundle](#ample-line-bundle)

If $A$ is an [ample line bundle](#ample-line-bundle) on a [projective variety](projective-space.md#projective-variety) and $L$ is any [line bundle](#line-bundle), then $A^{\otimes m}\otimes L$ is [very ample](#very-ample-line-bundle) for all sufficiently large [integers](number-theory.md#integer) $m$. Taking $L$ to be trivial also makes $A^{\otimes m}$ very ample.

##### Kodaira map

↑ **Parent:** [Line bundle](#line-bundle)

A basepoint-free vector space of global sections $V\subseteq H^0(X,L)$ defines the Kodaira map $X\to\mathbb P(V^*)$ by evaluating the sections at each point.

### Global section functor

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)

The global section functor sends a sheaf $\mathcal F$ on $X$ to $\Gamma(X,\mathcal F)$. It is left exact, and its right derived functors are [sheaf cohomology](#sheaf-cohomology).

#### Localization of global sections on a principal open

↑ **Parent:** [Global section functor](#global-section-functor)

For a quasi-compact [separated scheme](#separated-scheme) and a global [regular function](#regular-function) $f$, [global sections](#global-section) on $X_f$ are the [localization](commutative-algebra.md#localization-of-a-ring) of [global sections](#global-section) by $f$. Choose a finite affine [open cover](topology.md#open-cover). Its intersections are affine, so the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom) describes [global sections](#global-section) as the [kernel](linear-algebra.md#kernel-of-a-linear-map) of the difference map between two finite products of affine [coordinate rings](algebraic-geometry.md#coordinate-ring). [Exactness of localization](commutative-algebra.md#exactness-of-localization) preserves this [kernel](linear-algebra.md#kernel-of-a-linear-map), and [localization](commutative-algebra.md#localization-of-a-ring) commutes with those finite products. Localizing the same cover gives the claimed [isomorphism](algebra.md#isomorphism). This applies before knowing whether $X$ itself is affine.

#### Global section

↑ **Parent:** [Global section functor](#global-section-functor)

A global section of a [sheaf of modules](#sheaf-of-modules) $\mathcal F$ is an element of $\Gamma(X,\mathcal F)$, meaning a section defined over the whole space $X$.

#### Section functor with support

↑ **Parent:** [Global section functor](#global-section-functor)

For a closed subset $Z\subseteq X$, the section functor with support is

$$
\Gamma_Z(X,\mathcal F)
=\{s\in\Gamma(X,\mathcal F):\operatorname{Supp}s\subseteq Z\}.
$$

It is left exact.

##### Local cohomology

↑ **Parent:** [Section functor with support](#section-functor-with-support)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_cohomology)

Local cohomology consists of the right derived functors of the [section functor with support](#section-functor-with-support). It measures sections and cohomology concentrated along a closed subset $Z$.

###### Long exact sequence for local cohomology

↑ **Parent:** [Local cohomology](#local-cohomology)

For $U=X\setminus Z$, local and ordinary [sheaf cohomology](#sheaf-cohomology) fit into the natural sequence

$$
\cdots\to H^{i-1}(U,\mathcal F|_U)
\to H_Z^i(X,\mathcal F)
\to H^i(X,\mathcal F)
\to H^i(U,\mathcal F|_U)
\to H_Z^{i+1}(X,\mathcal F)\to\cdots.
$$

###### Local cohomology of the affine plane supported at the origin

↑ **Parent:** [Local cohomology](#local-cohomology)

For $X=\operatorname{Spec}k[x,y]$ and $Z=V(x,y)$, the only nonzero local cohomology group of the structure sheaf is

$$
H_Z^2(X,\mathcal O_X)
\cong\frac{k[x^{\pm1},y^{\pm1}]}{k[x^{\pm1},y]+k[x,y^{\pm1}]}.
$$

It has basis $x^{-a}y^{-b}$ for $a,b\geq1$. The two-standard-open [Čech cochain complex](#cech-cochain-complex) of the [punctured affine plane](#punctured-affine-plane) proves the formula.

### Sheaf cohomology

↑ **Parent:** [Sheaf of modules](#sheaf-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sheaf_cohomology)

Sheaf cohomology consists of the right derived functors of global sections. The zeroth group is $H^0(X,\mathcal F)=\Gamma(X,\mathcal F)$, and higher groups measure obstructions to gluing local sections.

#### Coherent cohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

Coherent cohomology means [sheaf cohomology](#sheaf-cohomology) with coefficients in a [coherent sheaf](#coherent-sheaf). On a separated [Noetherian scheme](#noetherian-scheme), a finite affine cover computes it using the [Čech cochain complex](#cech-cochain-complex), because intersections of affine opens are affine and positive-degree [quasi-coherent sheaf](#quasi-coherent-sheaf) cohomology vanishes there. Short exact sequences give [long exact sequences in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology).

##### Finiteness of coherent cohomology on projective varieties

↑ **Parent:** [Coherent cohomology](#coherent-cohomology)

For a [coherent sheaf](#coherent-sheaf) $\mathcal F$ on a [projective variety](projective-space.md#projective-variety) over a field, every $H^q(X,\mathcal F)$ is finite-dimensional, and [Grothendieck vanishing](#grothendieck-vanishing) gives zero for $q>\dim X$. A closed embedding in projective space and a [finite twisting resolution of a coherent sheaf on projective space](#finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space) reduce finiteness to the explicit [cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space). The same resolution proves [Serre vanishing](#serre-vanishing) after sufficiently positive twisting.

#### Cohomology sheaf

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For a [cochain complex](algebra.md#cochain-complex) of [sheaves](algebraic-geometry.md#sheaf-mathematics) $E$, its $i$th [cohomology sheaf](#cohomology-sheaf) is $\mathcal H^i(E)=\ker(d^i)/\operatorname{im}(d^{i-1})$, where the image and quotient are taken in [sheaves](algebraic-geometry.md#sheaf-mathematics). Its stalk at $x$ is the [cohomology](cohomology.md) of the stalk complex, because taking stalks is exact.

##### Cohomology-sheaf exact sequence

↑ **Parent:** [Cohomology sheaf](#cohomology-sheaf)

A short exact sequence of [cochain complexes](algebra.md#cochain-complex) of [sheaves](algebraic-geometry.md#sheaf-mathematics) $0\to E\to F\to G\to0$ induces $\cdots\to\mathcal H^i(E)\to\mathcal H^i(F)\to\mathcal H^i(G)\to\mathcal H^{i+1}(E)\to\cdots$. Taking stalks is exact, so the construction and exactness follow from the ordinary long exact sequence of [cohomology](cohomology.md) of complexes at every stalk. The stalkwise connecting maps come from the lift-and-differentiate construction and form a [sheaf](algebraic-geometry.md#sheaf-mathematics) morphism.

#### Grauert base change theorem

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For a proper holomorphic map and a coherent sheaf flat over the base, local constancy of the fibre-cohomology dimension makes its higher direct image locally free and gives the displayed base-change identification. Applied to relative holomorphic forms in a smooth proper Kähler family, this constructs the holomorphic [cohomology](cohomology.md) bundles entering its [variation of Hodge structure](differential-geometry.md#variation-of-hodge-structure).

#### Hypercohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypercohomology)

[Hypercohomology](#hypercohomology) applies the derived global-section functor to a complex of sheaves. One may resolve the complex by an [injective](algebra.md#injective-function) double complex, take [global sections](#global-section), and take the [cohomology](cohomology.md) of its total complex. For a complex concentrated in degree zero it is ordinary [sheaf cohomology](#sheaf-cohomology). The [relative de Rham complex](differential-form.md#relative-de-rham-complex) uses this construction to compute fibre [cohomology](cohomology.md) and its [Hodge filtration](differential-geometry.md#hodge-filtration).

#### Acyclic resolution theorem

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

If $0\to\mathcal F\to\mathcal I^0\to\mathcal I^1\to\cdots$ is an exact resolution of [sheaves](algebraic-geometry.md#sheaf-mathematics) and each $\mathcal I^j$ has vanishing positive [sheaf cohomology](#sheaf-cohomology), then the cohomology of its global-section complex computes $H^q(X,\mathcal F)$. [Fine sheaves](#fine-sheaf) provide acyclic terms on a paracompact manifold, giving the analytic [Dolbeault resolution of holomorphic differential forms](complex-geometry.md#dolbeault-resolution-of-holomorphic-differential-forms).

#### Locally vanishing principle for sheaf cohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

A positive-degree [sheaf cohomology](#sheaf-cohomology) class restricts to zero on some neighbourhood of every point, because a representing cocycle in a [flasque resolution](#flasque-resolution) is locally a boundary. If a basis closed under finite intersections has vanishing local cohomology in degrees $1,\ldots,i-1$, the neighbourhoods can be chosen in that basis so that the image of the class in $H^i(X,{}_U\mathcal F)$ is zero. Here ${}_U\mathcal F$ is the [direct image from an open restriction](#direct-image-from-an-open-restriction). Lower local vanishing makes the edge map $H^i(X,{}_U\mathcal F)\to H^i(U,\mathcal F|_U)$ injective. Local vanishing of a class alone does not imply global vanishing.

#### Holomorphic first cohomology of punctured complex two-space

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For $X=\mathbb C^2\setminus\{0\}$, the cover $\mathbb C\times\mathbb C^*$ and $\mathbb C^*\times\mathbb C$ is acyclic for $\mathcal O_X$. The first [Čech cohomology](#cech-cohomology) quotient is represented uniquely by normally convergent doubly negative [Laurent series](analysis.md#laurent-series). Under $w_i=1/z_i$ it is $w_1w_2\mathcal O(\mathbb C_w^2)$, the entire functions divisible by both coordinates. This is an infinite-dimensional analytic vector space; restricting representatives to finite Laurent polynomials loses classes. The class of $1/(z_1z_2)$ is nonzero, so $X$ is not a [Stein manifold](complex-geometry.md#stein-manifold).

<h4 id="castelnuovo-mumford-regularity">Castelnuovo–Mumford regularity</h4>

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Castelnuovo–Mumford_regularity)

A [coherent sheaf](#coherent-sheaf) $\mathcal F$ on $\mathbb P^N$ is $r$-regular if $H^i(\mathbb P^N,\mathcal F(r-i))=0$ for every $i>0$. It is then $(r+1)$-regular and $\mathcal F(r)$ is globally generated. Persistence follows by induction with a hyperplane avoiding the associated points and its restriction exact sequence. A sheaf on an embedded [projective scheme](#projective-scheme) is tested after pushforward to projective space.

#### Injective resolution of sheaves

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

An injective resolution is an [exact sequence](homology.md#exact-sequence) starting with a [sheaf](algebraic-geometry.md#sheaf-mathematics) and continuing with [injective sheaves](algebraic-geometry.md#injective-sheaf). It is constructed by successively embedding each quotient in an injective sheaf. Taking [global sections](#global-section) and then cohomology computes [sheaf cohomology](#sheaf-cohomology); in particular an injective sheaf has zero higher cohomology.

#### Euler characteristic of a coherent sheaf

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

On a proper scheme over a field, the [Euler characteristic of a coherent sheaf](#euler-characteristic-of-a-coherent-sheaf) is $\chi(X,\mathcal F)=\sum_i(-1)^i\dim H^i(X,\mathcal F)$. The sum is finite by [Grothendieck vanishing](#grothendieck-vanishing), and [long exact sequences in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) make it additive in [short exact sequences of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves).

<h5 id="asymptotic-riemann-roch">Asymptotic Riemann–Roch</h5>

↑ **Parent:** [Euler characteristic of a coherent sheaf](#euler-characteristic-of-a-coherent-sheaf)

For a [Cartier divisor](cartier-divisor.md) $D$ on an $n$-dimensional [projective scheme](#projective-scheme), $\chi(X,\mathcal O_X(mD))$ is a polynomial in $m$ whose leading term is $D^nm^n/n!$. The [intersection product](algebraic-geometry.md#intersection-product-of-cartier-divisors) uses the fundamental cycle, with the generic multiplicity of each component. Thus the statement also applies to nonreduced schemes.

#### Serre vanishing

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For an [ample line bundle](#ample-line-bundle) $A$ on a [projective scheme](#projective-scheme) and a [coherent sheaf](#coherent-sheaf) $\mathcal F$, $H^i(X,\mathcal F\otimes A^m)=0$ for every $i>0$ and all sufficiently large $m$.

##### Uniform high-degree vanishing on a smooth projective curve

↑ **Parent:** [Serre vanishing](#serre-vanishing)

For a fixed [coherent sheaf](#coherent-sheaf) on a [smooth projective curve](projective-space.md#smooth-projective-curve), one degree bound works for all [divisors on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve), rather than just powers of one ample divisor. Choose a point $P$. The complement of $P$ is affine, so the surjective transition maps on the finite-dimensional groups $H^1(C,\mathcal F(nP))$ eventually kill every class. The [Euler characteristic of a coherent sheaf](#euler-characteristic-of-a-coherent-sheaf) gives $h^0(\mathcal O(A))\ge\deg A+1-g$. Every divisor of sufficiently large degree is therefore linearly equivalent to $n_0P+E$ with $E$ effective. The point-supported quotient for adding $E$ transfers vanishing to that divisor. Torsion is first removed so that the relevant inclusions are injections of [locally free sheaves](#locally-free-sheaf).

##### Uniform Serre vanishing for two ample twists

↑ **Parent:** [Serre vanishing](#serre-vanishing)

For [ample](#ample-line-bundle) [line bundles](#line-bundle) $L,B$ and a [coherent sheaf](#coherent-sheaf) $\mathcal F$ on a [projective scheme](#projective-scheme), one $M$ gives $H^i(X,\mathcal F\otimes L^m\otimes B^t)=0$ for every $i>0$, $m\ge M$ and $t\ge0$. If $B$ is [very ample](#very-ample-line-bundle), [Serre vanishing](#serre-vanishing) for the finitely many fixed twists $\mathcal F(-iB)$ makes $\mathcal F\otimes L^m$ zero-regular. Persistence of [Castelnuovo–Mumford regularity](#castelnuovo-mumford-regularity) gives all nonnegative $B$-twists. For general [ample](#ample-line-bundle) $B$, use a [very ample](#very-ample-line-bundle) power and treat finitely many residues of $t$.

###### Higher cohomology vanishing from an ample hyperplane restriction

↑ **Parent:** [Uniform Serre vanishing for two ample twists](#uniform-serre-vanishing-for-two-ample-twists)

Let $H$ be a [very ample](#very-ample-line-bundle) [effective Cartier divisor](cartier-divisor.md#effective-cartier-divisor) on a [projective scheme](#projective-scheme) $X$, and suppose $L|_H$ is [ample](#ample-line-bundle). Then $H^i(X,L^m)=0$ for $i\ge2$ and sufficiently large $m$. By [uniform Serre vanishing for two ample twists](#uniform-serre-vanishing-for-two-ample-twists), cohomology of $L^m(tH)|_H$ vanishes uniformly for $t\ge0$. The restriction sequence identifies the higher groups of $L^m(tH)$ and $L^m((t+1)H)$ for $i\ge2$. For fixed $m$, large $t$ kills them by [Serre vanishing](#serre-vanishing) for $H$; descend to $t=0$. No $H^1$ vanishing is claimed.

##### Fujita vanishing

↑ **Parent:** [Serre vanishing](#serre-vanishing)

Given a [coherent sheaf](#coherent-sheaf) $\mathcal F$ and an [ample Cartier divisor](cartier-divisor.md#ample-cartier-divisor) $A$ on a [projective scheme](#projective-scheme), one integer $a_0$ ensures $H^i(X,\mathcal F(aA+N))=0$ for all $i>0$, all $a\geq a_0$, and every [nef divisor](cartier-divisor.md#nef-line-bundle) $N$. The uniformity in $N$ is stronger than [Serre vanishing](#serre-vanishing). [Fujino's note on Fujita vanishing](https://www.math.kyoto-u.ac.jp/~fujino/fujita-vani3.pdf) states the theorem for arbitrary projective schemes over a field.

###### Cohomology growth for nef twists

↑ **Parent:** [Fujita vanishing](#fujita-vanishing)

Let $N$ be a [nef Cartier divisor](cartier-divisor.md#nef-line-bundle) and let the [coherent sheaf](#coherent-sheaf) $\mathcal F$ have support dimension $d$. Then $h^i(X,\mathcal F(mN))=O(m^{d-i})$ for $1\leq i\leq d$. This does not require reducedness or smoothness.

Choose a very ample $A$ and fix $a$ sufficiently large for [Fujita vanishing](#fujita-vanishing). Choose a section of $aA$ avoiding the [associated points](#associated-point-of-a-coherent-sheaf) of $\mathcal F$. Its multiplication gives $0\to\mathcal F\to\mathcal F(aA)\to\mathcal Q\to0$, where $\mathcal Q$ has support dimension at most $d-1$. After tensoring with $\mathcal O_X(mN)$, the middle term has zero higher [sheaf cohomology](#sheaf-cohomology), uniformly in $m$. Hence $h^i(\mathcal F(mN))\leq h^{i-1}(\mathcal Q(mN))$. Induct on support dimension: for $i=1$ use the [polynomial bound for sections of a fixed divisor](algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor), and for $i>1$ use the induction hypothesis. Degree greater than $d$ vanishes by [Grothendieck vanishing](#grothendieck-vanishing).

###### Top cohomology boundedness for nef twists

↑ **Parent:** [Cohomology growth for nef twists](#cohomology-growth-for-nef-twists)

The top-degree case of [cohomology growth for nef twists](#cohomology-growth-for-nef-twists) is bounded independently of $m$. It fills a gap when a dimension induction hypothesis only covers intermediate [sheaf cohomology](#sheaf-cohomology) degrees.

#### Grothendieck vanishing

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For a [coherent sheaf](#coherent-sheaf) on a [Noetherian scheme](#noetherian-scheme), its [sheaf cohomology](#sheaf-cohomology) vanishes in degrees greater than its support dimension. In particular, a zero-dimensional projective scheme has no positive-degree coherent cohomology.

#### Resolution principle for sheaf cohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

If $0\to\mathcal F\to\mathcal A^0\to\mathcal A^1\to\cdots$ is an [exact sequence](homology.md#exact-sequence) of [sheaves of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups) on $X$ and $H^q(X,\mathcal A^j)=0$ for every $q>0$ and $j\geq0$, then [sheaf cohomology](#sheaf-cohomology) is computed by the [cochain complex](algebra.md#cochain-complex) of global sections:

$$
H^i(X,\mathcal F)\cong H^i\bigl(\Gamma(X,\mathcal A^\bullet)\bigr).
$$

In particular a [flasque resolution](#flasque-resolution) computes sheaf cohomology. Acyclicity is required on the space on which cohomology is being computed.

#### Leray spectral sequence

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leray_spectral_sequence)

For a continuous map $f:X\to Y$ and a sheaf $\mathcal F$ on $X$, the Leray spectral sequence is

$$
E_2^{p,q}=H^p(Y,R^qf_*\mathcal F)\Longrightarrow H^{p+q}(X,\mathcal F).
$$

If every higher direct image vanishes, its edge maps identify $H^p(X,\mathcal F)$ with $H^p(Y,f_*\mathcal F)$.

#### Flasque sheaf

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flasque_sheaf)

A sheaf is flasque when every restriction map is surjective. Flasque sheaves are acyclic for global sections, so $H^i(X,\mathcal F)=0$ for $i>0$.

##### Sheafification of an injective module is flasque

↑ **Parent:** [Flasque sheaf](#flasque-sheaf)

For a [Noetherian ring](algebra.md#noetherian-ring) $A$, an [injective module](noncommutative-algebra.md#injective-module) $I$ gives a [flasque sheaf](#flasque-sheaf) on $\operatorname{Spec}A$. If $U=\operatorname{Spec}A\setminus V(\mathfrak a)$, clearing denominators on finitely many principal opens identifies $\Gamma(U,\widetilde I)$ with $\varinjlim_n\operatorname{Hom}_A(\mathfrak a^n,I)$. Each map extends to $A$ by injectivity. Thus every section on $U$ extends globally, and all restriction maps are surjective. This concerns sheafification of an injective module, rather than the different assertion that an [injective sheaf of modules](#injective-sheaf-of-modules) is flasque.

##### Flasque-kernel section-lifting lemma

↑ **Parent:** [Flasque sheaf](#flasque-sheaf)

For a [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves) with [flasque sheaf](#flasque-sheaf) kernel, every section of the quotient on any open set lifts to the middle sheaf on that set. Use the [Zorn lemma](set-theory.md#zorn-s-lemma) to choose a maximal partial lift, with chains glued by the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom). A new local lift differs from the old one on their overlap by a kernel section. Extend that difference by flasqueness, adjust the new lift, and glue, contradicting maximality unless its domain is the entire open set. Consequently a quotient of two flasque sheaves is flasque. With an [injective resolution of sheaves](#injective-resolution-of-sheaves), the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) and repeated dimension shifts prove that flasque sheaves have zero positive-degree cohomology.

##### Flasque resolution

↑ **Parent:** [Flasque sheaf](#flasque-sheaf)

A flasque resolution is an [exact sequence](homology.md#exact-sequence) of [sheaves of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups) whose terms $\mathcal I^j$ are [flasque sheaves](#flasque-sheaf). Every such sheaf embeds by its section germs into the sheaf $U\mapsto\prod_{P\in U}\mathcal F_P$. Its restriction maps are projections, so it is flasque. Apply this construction successively to the cokernels to obtain a resolution. The [sheaf cohomology](#sheaf-cohomology) of $\mathcal F$ is the cohomology of the [cochain complex](algebra.md#cochain-complex) $\Gamma(X,\mathcal I^\bullet)$. A quotient of two flasque sheaves in a [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves) is flasque: the flasque kernel allows local lifts to be glued into a section of the middle sheaf over the smaller open set; extend that lift using flasqueness of the middle sheaf, and project. Consequently the resolution's successive cokernels are flasque when $\mathcal F$ is flasque, and exactness of sections shows that all its positive-degree cohomology vanishes.

###### Godement resolution

↑ **Parent:** [Flasque resolution](#flasque-resolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Godement_resolution)

Embed a [sheaf of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups) $\mathcal F$ into the sheaf $C(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P$ by all its [germs](#germ-of-a-sheaf-section). Restrictions are projections, so $C(\mathcal F)$ is [flasque](#flasque-sheaf). Repeat on the successive sheaf [cokernels](linear-algebra.md#cokernel) to obtain a canonical [flasque resolution](#flasque-resolution). Its complex of [global sections](#global-section) computes [sheaf cohomology](#sheaf-cohomology). When $\mathcal F$ is itself [flasque](#flasque-sheaf), the flasque-kernel section-lifting lemma makes every successive quotient flasque and makes the global-section complex exact in positive degrees, proving $H^q(X,\mathcal F)=0$ for $q>0$ without assuming that vanishing in the construction.

<h4 id="cech-cohomology">Čech cohomology</h4>

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Čech_cohomology)

For an open cover $\mathcal U=(U_i)$, the Čech cochain group is

$$
\check C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}),
$$

with the alternating sum of restrictions as differential. Its cohomology is the Čech cohomology of $\mathcal F$ with respect to $\mathcal U$.

##### Cohomology of twists on projective space

↑ **Parent:** [Čech cohomology](#cech-cohomology)

For $r\ge1$, a [twisting sheaf on projective space](#twisting-sheaf-on-projective-space) has $H^0(\mathbf P_k^r,\mathcal O(n))=k[X_0,\ldots,X_r]_n$ when $n\ge0$, and top cohomology with basis the [Laurent monomials](polynomial.md#laurent-monomial) of total degree $n$ whose exponents are all negative. All intermediate [sheaf cohomology](#sheaf-cohomology) vanishes. Their dimensions are $\binom{n+r}{r}$ and $\binom{-n-1}{r}$ respectively, with the top group nonzero only for $n\le-r-1$. Decompose the standard [Čech cochain complex](#cech-cochain-complex) by exponent vector: no negative exponents gives a simplex with cohomology in degree zero; a nonempty proper negative-support set admits a contracting homotopy inserting a vertex outside that set; all negative exponents give only the top term. For $r=0$, every twist is trivial on $\operatorname{Spec}k$ and has $H^0=k$.

<h5 id="cech-cohomology-of-the-punctured-affine-plane">Čech cohomology of the punctured affine plane</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

The two affine opens $D(x),D(y)$ cover the [punctured affine plane](#punctured-affine-plane). Their intersection has ring $k[x^{\pm1},y^{\pm1}]$. The [Čech cohomology](#cech-cohomology) in degree one is the quotient by $k[x^{\pm1},y]+k[x,y^{\pm1}]$. Its basis consists precisely of the Laurent monomials whose two exponents are negative, so this [vector space](vector-space.md) is infinite-dimensional. Global functions, by contrast, form $k[x,y]$.

<h5 id="cech-cohomology-of-twists-on-the-projective-line">Čech cohomology of twists on the projective line</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

On the standard two-affine cover of the [projective line](finite-group-theory.md#projective-line), with coordinate $t$, a frame for the [twisting sheaf on projective space](#twisting-sheaf-on-projective-space) $\mathcal O(n)$ on the second chart equals $t^n$ times the frame on the first. Its [Čech cochain complex](#cech-cochain-complex) is $k[t]\oplus k[t^{-1}]\to k[t,t^{-1}]$, with map $(a,b)\mapsto t^nb-a$. The kernel has basis $1,t,\ldots,t^n$ for $n\geq0$. The cokernel has basis $t^{n+1},\ldots,t^{-1}$ for $n\leq-2$. The two-chart complex also proves vanishing in degrees at least two.

###### Holomorphic Laurent-series cohomology of twists on the projective line

↑ **Parent:** [Čech cohomology of twists on the projective line](#cech-cohomology-of-twists-on-the-projective-line)

For analytic [holomorphic sections](complex-geometry.md#holomorphic-section), the two-chart [Čech cohomology](#cech-cohomology) uses convergent [Laurent series](analysis.md#laurent-series), rather than only Laurent polynomials. A frame on the infinity chart equals $z^n$ times a finite-chart frame. Entire finite-chart functions remove Laurent powers $k\ge0$, and infinity-chart functions remove powers $k\le n$. The positive and negative tails converge to entire chart functions, so only the finite gap $n<k<0$ remains. Thus the first cohomology has basis $z^{n+1},\ldots,z^{-1}$ when $n\le-2$ and is zero when $n\ge-1$. The same transition relation gives global sections of dimension $\max(n+1,0)$.

<h5 id="cech-cohomology-of-an-affine-cover-can-differ-from-sheaf-cohomology">Čech cohomology of an affine cover can differ from sheaf cohomology</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

On $X=\mathbb A^1_k$, let $K=k(t)$ and let $\mathcal K$ be its constant sheaf. For the two closed rational points $0,1$, take skyscraper sheaves $S_0,S_1$ with value $K$, and put $\mathcal F=\ker(\mathcal K\to S_0\oplus S_1)$. The maps on the two stalks are identities, so this is a sheaf surjection. All three displayed outer sheaves are flasque. The induced global map is the diagonal $K\to K^2$, so $H^1(X,\mathcal F)=K^2/\Delta K\simeq K$. The one-member affine cover has zero positive Čech cochains. This even gives an $\mathcal O_X$-module example: let regular functions act on all copies of $K$ by multiplication as rational functions, not by evaluation at the closed point. The kernel is not quasi-coherent.

<h5 id="cech-de-rham-double-complex">Čech-de Rham double complex</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

On a good cover, combine Čech degree $p$ and differential-form degree $q$ in the double complex of forms on intersections. The Čech differential and [exterior derivative](differential-form.md#exterior-derivative) commute, so the total differential $\delta+(-1)^p d$ squares to zero. A partition of unity and the [Poincaré lemma](differential-form.md#poincare-lemma) identify its cohomology with both constant-sheaf and [de Rham cohomology](differential-form.md#de-rham-cohomology). The sign convention makes [Čech-de Rham curvature descent](complex-geometry.md#cech-de-rham-curvature-descent) explicit.

<h5 id="cech-lifting-below-the-first-possible-local-cohomology-degree">Čech lifting below the first possible local cohomology degree</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

For a finite cover whose nonempty intersections have zero [sheaf cohomology](#sheaf-cohomology) in degrees $1,\ldots,i-1$, the displayed sequence is exact for $i>0$. Apply the [Čech cochain complex](#cech-cochain-complex) to a [flasque resolution](#flasque-resolution). Local primitives and successive primitives of their overlap differences reduce a class with zero restrictions to a Čech cocycle with values in the original [sheaf](algebraic-geometry.md#sheaf-mathematics). Vanishing in degree $i$ on all intersections is not needed.

<h5 id="cech-cochain-complex">Čech cochain complex</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)

The Čech cochain complex places sections on $(p+1)$-fold intersections in degree $p$ and uses the alternating sum of restriction maps as its differential.

<h6 id="cech-differential">Čech differential</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

The Čech differential sends a cochain on $(p+1)$-fold intersections to the alternating sum of its restrictions to $(p+2)$-fold intersections. Each pair of omitted indices occurs twice with opposite signs in the composite, so $\delta^2=0$. It defines the [Čech cohomology](#cech-cohomology) of the cover.

<h6 id="cech-resolution-on-a-semi-separated-scheme">Čech resolution on a semi-separated scheme</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

For a finite affine cover of a [semi-separated scheme](#semi-separated-scheme), every finite intersection is affine. The augmented sheaf [Čech cochain complex](#cech-cochain-complex) is exact: near each point, an open of the cover contains the neighbourhood under consideration, and inserting its index contracts the complex. Its terms are acyclic for a [quasi-coherent sheaf](#quasi-coherent-sheaf), by affine cohomology vanishing and the affine-intersection property. Alternatively, apply the section-level [Čech cochain complex](#cech-cochain-complex) to a [flasque resolution](#flasque-resolution); the two computations of the resulting [double complex](homology.md#double-complex) identify [Čech cohomology](#cech-cohomology) with [sheaf cohomology](#sheaf-cohomology). Stalks of direct images from opens outside those opens need not vanish, so exactness must not be justified by treating these direct images as [extensions by zero](#extension-by-zero).

<h6 id="exactness-of-the-unit-ideal-localization-cech-complex">Exactness of the unit-ideal localization Čech complex</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

For a finite family generating the [unit ideal](commutative-algebra.md#unit-ideal) in a [commutative ring](commutative-algebra.md#commutative-ring), this augmented [Čech cochain complex](#cech-cochain-complex) of any [module](module-theory.md#module-mathematics) is exact. One proof clears the finitely many denominators and cocycle relations by powers $f_i^N$, writes $1=\sum_i a_if_i^N$, and contracts an alternating cocycle by the weighted insertions $\sum_i a_if_i^Nc_{iI}$. The argument uses [vanishing criterion in a module localization](commutative-algebra.md#vanishing-criterion-in-a-module-localization) and does not require the [module](module-theory.md#module-mathematics) to be finitely generated.

<h6 id="cech-cochain-group">Čech cochain group</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

The degree-$p$ Čech cochain group for an ordered cover is $\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p})$.

<h6 id="cech-cocycle-condition">Čech cocycle condition</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

A Čech cochain is a cocycle when its alternating coboundary vanishes. For a multiplicative one-cochain $(g_{ij})$, this says $g_{ij}g_{jk}=g_{ik}$ on triple intersections.

<h6 id="cech-coboundary">Čech coboundary</h6>

↑ **Parent:** [Čech cochain complex](#cech-cochain-complex)

A Čech coboundary is the image of a cochain in the preceding degree. Multiplicatively, a zero-cochain $(h_i)$ changes a one-cocycle by $g_{ij}\mapsto h_i^{-1}g_{ij}h_j$.

<h5 id="leray-s-theorem">Leray's theorem</h5>

↑ **Parent:** [Čech cohomology](#cech-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leray's_theorem)

If every nonempty finite intersection of members of an open cover has vanishing higher [sheaf cohomology](#sheaf-cohomology) for $\mathcal F$, then the cover's [Čech cohomology](#cech-cohomology) computes $H^p(X,\mathcal F)$. An affine open cover of a separated scheme satisfies this condition for a quasi-coherent sheaf because its finite intersections are affine.

###### Cohomology under a closed immersion

↑ **Parent:** [Leray's theorem](#leray-s-theorem)

If $i:Z\hookrightarrow X$ is a [closed immersion](#closed-immersion) of [Noetherian schemes](#noetherian-scheme), $X$ is separated, and $\mathcal F$ is [quasi-coherent](#quasi-coherent-sheaf) on $Z$, then

$$
H^q(X,i_*\mathcal F)\cong H^q(Z,\mathcal F).
$$

Indeed, an affine cover of $X$ induces an affine cover of $Z$, and the two associated [Čech cochain complexes](#cech-cochain-complex) are termwise identical.

###### Cohomological dimension bound from an affine cover

↑ **Parent:** [Leray's theorem](#leray-s-theorem)

If a [separated scheme](#separated-scheme) has an acyclic affine cover by $r$ open sets, then every [quasi-coherent sheaf](#quasi-coherent-sheaf) on it has vanishing [sheaf cohomology](#sheaf-cohomology) in degrees at least $r$. The corresponding [Čech cochain complex](#cech-cochain-complex) has no terms in those degrees.

#### Fine sheaf

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fine_sheaf)

A sheaf of modules over the sheaf of [smooth functions](analysis.md#smooth-function) is fine when every locally finite [open cover](topology.md#open-cover) admits a subordinate family of sheaf endomorphisms summing to the identity. Fine sheaves on a [paracompact space](topology.md#paracompact-space) are acyclic, so their positive-degree [sheaf cohomology](#sheaf-cohomology) vanishes.

#### Mayer-Vietoris sequence for sheaf cohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

For $X=U\cup V$, the short exact sequence of sheaves obtained by restricting to $U$, $V$, and $U\cap V$ induces a long exact sequence

$$
0\to H^0(X,\mathcal F)\to H^0(U,\mathcal F)\oplus H^0(V,\mathcal F)\to H^0(U\cap V,\mathcal F)\to H^1(X,\mathcal F)\to\cdots.
$$

#### Long exact sequence in sheaf cohomology

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)

A short exact sequence of sheaves $0\to\mathcal F'\to\mathcal F\to\mathcal F''\to0$ induces a natural long exact sequence

$$
0\to H^0(X,\mathcal F')\to H^0(X,\mathcal F)\to H^0(X,\mathcal F'')\to H^1(X,\mathcal F')\to\cdots.
$$

#### Serre duality

↑ **Parent:** [Sheaf cohomology](#sheaf-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Serre_duality)

For a smooth projective $n$-dimensional variety $X$ over a field and a coherent sheaf $\mathcal F$, Serre duality gives a perfect pairing between $H^q(X,\mathcal F)$ and $\operatorname{Ext}^{n-q}(\mathcal F,\omega_X)$, where $\omega_X$ is the canonical sheaf.

##### Dualizing sheaf on a smooth projective curve

↑ **Parent:** [Serre duality](#serre-duality)

For [vector bundles](fiber-bundle.md#vector-bundle) on a [smooth projective curve](projective-space.md#smooth-projective-curve), a dualizing sheaf is a [line bundle](#line-bundle) $D_C$ with a trace $H^1(C,D_C)\to k$ making the evaluation pairings $H^i(C,E)\times H^{1-i}(C,E^\vee\otimes D_C)\to k$ perfect for $i=0,1$. Choose a finite generically separable map to the [projective line](finite-group-theory.md#projective-line). The trace-dual module for this finite map, tensored with $\Omega^1_{\mathbb P^1}$, is $\Omega^1_C$ by the different–differential identity. Finite pushforward and [residue duality on the projective line](#residue-duality-on-the-projective-line) then prove the pairings, rather than assuming the curve-duality theorem to establish them.

###### Residue trace on a smooth projective curve

↑ **Parent:** [Dualizing sheaf on a smooth projective curve](#dualizing-sheaf-on-a-smooth-projective-curve)

Use the [rational principal-parts resolution on an algebraic curve](#rational-principal-parts-resolution-on-an-algebraic-curve) to represent a class by finitely many rational differential principal parts. Sum their [algebraic residues of a rational differential](algebraic-geometry.md#algebraic-residue-of-a-rational-differential). The sum of residues of a global rational differential is zero: trace to the [projective line](finite-group-theory.md#projective-line), where partial fractions prove the assertion. Hence the sum descends to cohomology. Pairing an [invertible sheaf](#line-bundle) with its differential-valued dual gives the perfect [Serre duality](#serre-duality) pairing. Since the global regular functions on an integral projective curve over an algebraically closed field are $k$, evaluation at the constant function $1$ identifies this trace canonically with an isomorphism to $k$.

##### Residue duality on the projective line

↑ **Parent:** [Serre duality](#serre-duality)

The coefficient of $t^{-1}dt$ gives a trace on $H^1(\mathbb P^1,\Omega^1)$. Multiplication followed by this trace pairs the Laurent bases of the [Čech cohomology of twists on the projective line](#cech-cohomology-of-twists-on-the-projective-line) perfectly: $t^a$ pairs with $t^{-a-1}$. For any [vector bundle](fiber-bundle.md#vector-bundle), evaluation into $\Omega^1$ defines the same natural pairing. Saturate a rational rank-one subspace to a [line subbundle](fiber-bundle.md#line-subbundle), and induct on rank using the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) and compatibility of evaluation with connecting maps. This proves the duality without using the later splitting theorem.

##### Failure of ordinary sheaf-dual Serre duality for a skyscraper sheaf

↑ **Parent:** [Serre duality](#serre-duality)

On $\mathbb P_k^n$ with $n>0$, let $\mathcal F=i_*k$ at a rational point. It has one-dimensional [global sections](#global-section), but its [dual of a sheaf](#dual-of-a-sheaf) is zero: a local map from the residue field into the local polynomial ring must have image annihilated by a nonzero parameter, which is impossible in an [integral domain](commutative-algebra.md#integral-domain). Thus $H^n(\mathcal F^\vee(-n-1))=0$. [Serre duality](#serre-duality) for arbitrary coherent sheaves instead uses an [Ext functor](algebra.md#ext-functor); replacing this by the ordinary dual can lose torsion information.

##### Serre duality for compact complex manifolds

↑ **Parent:** [Serre duality](#serre-duality)

For a compact complex $n$-manifold and a [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle) $E$, analytic [Serre duality](#serre-duality) gives

$$
H^q(M,E)^*\cong H^{n-q}(M,K_M\otimes E^*).
$$

The pairing integrates the wedge product of bundle-valued [Dolbeault cohomology](complex-geometry.md#dolbeault-cohomology) representatives, contracting $E$ with its dual.

## Locally ringed space

↑ **Parent:** [Ringed space](ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_ringed_space)

A locally ringed space is a [ringed space](ringed-space.md) whose stalk $\mathcal O_{X,x}$ is a [local ring](commutative-algebra.md#local-ring) at every point. Morphisms of locally ringed spaces induce local homomorphisms on stalks.

### Morphism of locally ringed spaces

↑ **Parent:** [Locally ringed space](#locally-ringed-space)

A morphism is a continuous map $f:X\to Y$ together with a homomorphism $\mathcal O_Y\to f_*\mathcal O_X$ of [sheaves of rings](#sheaf-of-rings) whose induced map on every [stalk](#stalk-of-a-sheaf) is a [local homomorphism](commutative-algebra.md#local-homomorphism-of-local-rings). Applied to [schemes](#scheme), this is exactly a [morphism of schemes](#morphism-of-schemes).

### Scheme

↑ **Parent:** [Locally ringed space](#locally-ringed-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scheme_(mathematics))

A scheme is a [locally ringed space](#locally-ringed-space) covered by open subsets isomorphic to spectra of [commutative rings](commutative-algebra.md#commutative-ring). It retains both the points defined by prime ideals and the local algebra of functions around them.

#### Functor represented by a scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functor_represented_by_a_scheme)

The functor of points describes a [scheme](#scheme) through its morphisms from test [schemes](#scheme). On [commutative rings](commutative-algebra.md#commutative-ring), it is covariant because a [ring homomorphism](commutative-algebra.md#ring-homomorphism) reverses the corresponding affine-scheme map. A functor on [rings](commutative-algebra.md#ring) is represented by $X$ in the algebraic-geometric sense when it is naturally isomorphic to $h_X$. The representing [scheme](#scheme) need not be affine; this is different from demanding a [representable functor](category.md#representable-functor) in the category of [rings](commutative-algebra.md#ring) itself.

// Target: module-theory.bigb

#### Gluing of schemes along open subschemes

↑ **Parent:** [Scheme](#scheme)

Given [schemes](#scheme) $X_i$ and [isomorphisms](algebra.md#isomorphism) between designated [open subschemes](#open-subscheme) satisfying inverse and cocycle conditions, identify the underlying open spaces and glue their structure sheaves. The resulting [locally ringed space](#locally-ringed-space) is locally one of the $X_i$, hence a [scheme](#scheme). The same construction works for [formal schemes](#formal-scheme) and topological structure sheaves. Compatible morphisms out of the charts glue uniquely.

// Target: ringed-space.bigb

#### Formal scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_scheme)

A [formal scheme](#formal-scheme) is a [locally ringed space](#locally-ringed-space) with a [sheaf of topological rings](#sheaf-of-topological-rings) that is locally a [formal spectrum](#formal-spectrum) of a complete adic [ring](commutative-algebra.md#ring). An ordinary [scheme](#scheme) is the special case of the discrete topology. A [formal completion of a scheme](#formal-completion-of-a-scheme) retains all [infinitesimal neighbourhoods](#infinitesimal-neighbourhood-of-a-closed-subscheme) of a [closed subscheme](#closed-subscheme), rather than just that subscheme.

// Target: ringed-space.bigb

##### Formal completion of a scheme

↑ **Parent:** [Formal scheme](#formal-scheme)

For a [closed subscheme](#closed-subscheme) with [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$ in a locally [Noetherian scheme](#noetherian-scheme), the completion is the [formal scheme](#formal-scheme) on $|Y|$ with topological structure sheaf $\varprojlim_n(\mathcal O_X/\mathcal I^{n+1})|_{|Y|}$. On a Noetherian [affine scheme](#affine-scheme) $\operatorname{Spec}A$, it is $\operatorname{Spf}(\varprojlim_nA/I^{n+1})$. Its [adic topology](commutative-algebra.md#adic-topology) remembers every [infinitesimal neighbourhood](#infinitesimal-neighbourhood-of-a-closed-subscheme).

// Target: commutative-algebra.bigb

###### Formal completion commutes with restriction to an open subscheme

↑ **Parent:** [Formal completion of a scheme](#formal-completion-of-a-scheme)

Restricting the topological structure sheaf of a [formal completion of a scheme](#formal-completion-of-a-scheme) to an [open subscheme](#open-subscheme) commutes with its [inverse limit](module-theory.md#inverse-limit): both sheaves are $\varprojlim_n(\mathcal O_U/(\mathcal I|_U)^{n+1})$ on $|U\cap Y|$. Equivalently, the identical [infinitesimal neighbourhoods](#infinitesimal-neighbourhood-of-a-closed-subscheme) have identical restricted structure sheaves. On formal affine charts this uses [completed localization of an adic ring](commutative-algebra.md#completed-localization-of-an-adic-ring).

// Target: toric-geometry.bigb

##### Formal spectrum

↑ **Parent:** [Formal scheme](#formal-scheme)

For a complete [ring](commutative-algebra.md#ring) with an [adic topology](commutative-algebra.md#adic-topology) defined by $I$, the [formal spectrum](#formal-spectrum) has the prime ideals containing $I$ as its points and structure sheaf $\varprojlim_n\mathcal O_{\operatorname{Spec}(A/I^{n+1})}$. On a [principal open subset](#principal-open-subscheme) $D(f)$ its sections form the [completed localization of an adic ring](commutative-algebra.md#completed-localization-of-an-adic-ring), not generally the ordinary localization $A_f$.

// Target: ringed-space.bigb

#### Smooth morphism

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smooth_morphism)

A morphism of [schemes](#scheme) is smooth when it is locally of finite presentation, flat and has geometrically regular fibres. Smooth fibres alone do not imply that a morphism is smooth: flatness and the dimension behaviour matter as well. The [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve) has smooth [projective space](projective-space.md) fibres whose dimensions can jump.

<h4 id="etale-morphism">Étale morphism</h4>

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Étale_morphism)

A morphism of [schemes](#scheme) is étale when it is flat, unramified and locally of finite presentation. For a morphism between smooth varieties of the same dimension, an invertible differential gives this property locally. A finite étale morphism over an [algebraically closed field](algebra.md#algebraically-closed-field) has reduced finite fibres, and their cardinalities equal its degree when the source and target are connected.

<h5 id="finite-etale-morphism">Finite étale morphism</h5>

↑ **Parent:** [Étale morphism](#etale-morphism)

A finite étale morphism is both a [finite morphism](algebraic-geometry.md#finite-morphism) and an [étale morphism](#etale-morphism). Affine-locally it is represented by a finite locally free algebra with zero module of [Kähler differentials](#kahler-differential). Its fibres are finite products of finite separable field extensions. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) with [good reduction](normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at a prime not dividing $m$, multiplication by $m$ on its smooth proper group model is finite étale of degree $m^2$: its differential is multiplication by the unit $m$. A division torsor of a section consequently gives an unramified local extension, the good-prime input to the [Weak Mordell-Weil theorem](normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem).

#### Quasi-compact scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is quasi-compact when its underlying [topological space](topology.md#topological-space) is [quasi-compact](topology.md#compact-space): every [open cover](topology.md#open-cover) has a finite subcover. Since [affine open subsets](#affine-open-subscheme) form a base, this is equivalent to possessing a finite [affine open cover](topology.md#affine-open-cover). Every [affine scheme](#affine-scheme) is quasi-compact.

#### Open subscheme

↑ **Parent:** [Scheme](#scheme)

An open subscheme of a [scheme](#scheme) $X$ is an [open subset](topology.md#open-set) $U$ equipped with the restriction of its [structure sheaf](#structure-sheaf-of-a-scheme). Its inclusion is an [open immersion](#open-immersion). Every scheme is covered by [affine open subschemes](#affine-open-subscheme). Any nonempty open subscheme of an [integral scheme](#integral-scheme) is integral and has the same [generic point](algebraic-geometry.md#generic-point) and [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety).

#### Irreducible scheme

↑ **Parent:** [Scheme](#scheme)

An irreducible [scheme](#scheme) is one whose underlying [topological space](topology.md#topological-space) is a nonempty [irreducible topological space](algebraic-geometry.md#irreducible-topological-space). It can have [nilpotent elements](commutative-algebra.md#nilpotent) in its [structure sheaf](#structure-sheaf-of-a-scheme); irreducibility concerns only the topology. A [reduced scheme](#reduced-scheme) is an [integral scheme](#integral-scheme) precisely when it is irreducible.

#### Dimension of a scheme

↑ **Parent:** [Scheme](#scheme)

The dimension of a [scheme](#scheme) is the supremum of the lengths of strict chains of irreducible closed subsets of its underlying topological space. On an affine scheme it is the [Krull dimension](commutative-algebra.md#krull-dimension) of its coordinate ring. Taking the reduced subscheme leaves the dimension unchanged.

#### Structure morphism

↑ **Parent:** [Scheme](#scheme)

The structure morphism of a [scheme](#scheme) $X$ is its unique morphism $X\to\operatorname{Spec}\mathbb Z$. More generally, an $S$-scheme comes equipped with a specified morphism to the base scheme $S$.

#### Scheme of characteristic p

↑ **Parent:** [Scheme](#scheme)

A [scheme](#scheme) $X$ has characteristic $p$ when $p\cdot1=0$ in its [structure sheaf of a scheme](#structure-sheaf-of-a-scheme). Equivalently, its [structure morphism](#structure-morphism) $X\to\operatorname{Spec}\mathbb Z$ factors through $\operatorname{Spec}\mathbb F_p$.

##### Absolute Frobenius morphism

↑ **Parent:** [Scheme of characteristic p](#scheme-of-characteristic-p)

The absolute Frobenius morphism of a [scheme of characteristic p](#scheme-of-characteristic-p) is the identity on the underlying topological space and raises every local function to its $p$th power. On an affine chart $\operatorname{Spec}A$ it is induced contravariantly by the [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) $A\to A$, $a\mapsto a^p$. It need not be an [isomorphism of schemes](#isomorphism-of-schemes), even when it acts invertibly on global sections.

The algebraic [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) induces this scheme map contravariantly on affine charts.

###### Frobenius factorization through a finite normal cover

↑ **Parent:** [Absolute Frobenius morphism](#absolute-frobenius-morphism)

For a finite surjective map of normal [integral schemes](#integral-scheme) with [function fields](algebraic-geometry.md#function-field-of-an-algebraic-variety) $K\subseteq L$ in characteristic $p$, the condition $L^p\subseteq K$ lets the [Absolute Frobenius morphism](#absolute-frobenius-morphism) of the source factor through the map. On an affine chart $A\subseteq B$, send $b$ to $b^p\in A$: it lies in $K$, is integral over $A$, and $A$ is integrally closed. The condition $K\subseteq L^p$ instead lets the map factor after the source Frobenius. Send $a$ to its unique $p$th root in $L$; that root lies in the normal ring $B$ because it satisfies a monic polynomial over $B$. These rules localize and glue; injectivity of Frobenius in the [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety) supplies uniqueness.

#### Structure sheaf of a scheme

↑ **Parent:** [Scheme](#scheme)

The structure sheaf $\mathcal O_X$ records the [regular functions](#regular-function) on every open subset of a [scheme](#scheme) $X$. Its stalk $\mathcal O_{X,x}$ is the [local ring](commutative-algebra.md#local-ring) of functions defined near $x$.

<h5 id="idempotent-clopen-correspondence">Idempotent–clopen correspondence</h5>

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

A global [idempotent](commutative-algebra.md#idempotent) on a [scheme](#scheme) is zero or one in every [local ring](commutative-algebra.md#local-ring). Its one-locus is both open and closed. Conversely a clopen subset determines a global [idempotent](commutative-algebra.md#idempotent) by gluing one on it and zero on its complement. Under this correspondence, decompositions into nonzero [orthogonal idempotents](commutative-algebra.md#orthogonal-idempotent) correspond to disjoint clopen decompositions. When all [connected components](geometry-and-topology.md#connected-component) are open, the [primitive idempotents](commutative-algebra.md#primitive-idempotent) correspond exactly to those components. Without orthogonality the assertion fails in characteristic two: $(1,0)=(1,1)+(0,1)$ in $\mathbb F_2\times\mathbb F_2$.

##### Sheaf of units of the structure sheaf

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

The units in the [structure sheaf of a scheme](#structure-sheaf-of-a-scheme) form a multiplicative [sheaf of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups). On a [smooth algebraic curve](algebraic-geometry.md#smooth-algebraic-curve), a nonzero [rational function](isolated-singularity.md#rational-function) is a unit at a point precisely when its [discrete valuation](commutative-algebra.md#discrete-valuation) there is zero. Its inclusion in the [sheaf of nonzero rational functions on an irreducible variety](algebraic-geometry.md#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety) relates [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve) to the [Picard group](#picard-group) through the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology).

##### Regular function

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

A regular function on an open subset $U$ of a [scheme](#scheme) $X$ is a section of $\mathcal O_X(U)$. On an affine variety it is locally a quotient of polynomial functions with a denominator that does not vanish.

On a variety, a regular function is a [regular map](algebraic-geometry.md#morphism-of-algebraic-varieties) to the [affine line](#affine-line); the arbitrary-target regular-map concept is broader.

###### Global regular function

↑ **Parent:** [Regular function](#regular-function)

A global regular function is a [global section](#global-section) of the [structure sheaf](#structure-sheaf-of-a-scheme) of a [scheme](#scheme), defined on the entire scheme. These functions form its ring $H^0(X,\mathcal O_X)$. On an [affine scheme](#affine-scheme) this recovers the defining ring; on a positive-dimensional [projective complete intersection](#projective-complete-intersection) it consists only of constants over the base [field](algebra.md#field).

###### Global regular functions on an irreducible projective variety

↑ **Parent:** [Global regular function](#global-regular-function)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), every [regular function](#regular-function) on a nonempty irreducible [projective variety](projective-space.md#projective-variety) is constant. Regard the function as a morphism to $\mathbb P^1$ avoiding infinity. Its graph is closed; the [closedness of projection from projective space](#closedness-of-projection-from-projective-space) makes its image closed in $\mathbb P^1$. A proper closed subset there is finite, and an irreducible finite image is a singleton. Irreducibility is the usual variety convention; on a disconnected projective algebraic set different components may have different constants.

###### Regular functions on the punctured affine plane

↑ **Parent:** [Global regular function](#global-regular-function)

For $W=\mathbb A_k^2\setminus\{0\}$, restriction to $D(x)$ and $D(y)$ gives

$$
\Gamma(W,\mathcal O_W)=k[x,y]_x\cap k[x,y]_y=k[x,y].
$$

The intersection is taken in $k(x,y)$ and the equality follows from [unique factorization](algebra.md#unique-factorization-in-an-integral-domain): a reduced denominator dividing powers of both $x$ and $y$ is a unit. The inclusion $W\hookrightarrow\mathbb A^2$ induces an isomorphism on global functions but is not an isomorphism, so $W$ is not an [affine variety](algebraic-geometry.md#affine-algebraic-set).

#### Reduced scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_scheme)

A scheme is reduced when every [local ring](commutative-algebra.md#local-ring) $\mathcal O_{X,x}$ is a [reduced ring](commutative-algebra.md#reduced-ring), equivalently when its structure sheaf has no nonzero [nilpotent element](commutative-algebra.md#nilpotent). The affine scheme $\operatorname{Spec}A$ is reduced exactly when $A$ is reduced.

##### Generic reducedness with no embedded components

↑ **Parent:** [Reduced scheme](#reduced-scheme)

A Noetherian scheme with no embedded [associated primes](module-theory.md#associated-prime-of-a-module) is reduced if it is reduced at all its generic points. Locally, a nonzero nilpotent ideal would have an [associated prime](module-theory.md#associated-prime-of-a-module), necessarily a minimal prime. Its localization there would be nonzero, contradicting generic reducedness. This is useful with the [unmixedness of a complete intersection](#unmixedness-of-a-complete-intersection).

##### Integral scheme

↑ **Parent:** [Reduced scheme](#reduced-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_scheme)

An integral scheme is a nonempty [scheme](#scheme) that is both [reduced](#reduced-scheme) and [irreducible](algebraic-geometry.md#irreducible-topological-space). An affine scheme $\operatorname{Spec}A$ is integral exactly when $A$ is an [integral domain](commutative-algebra.md#integral-domain).

###### Generic-point embedding of regular functions

↑ **Parent:** [Integral scheme](#integral-scheme)

On an [integral scheme](#integral-scheme) $X$, every nonempty open $U$ contains its [generic point](algebraic-geometry.md#generic-point) $\eta$. Taking a [germ](#germ-of-a-sheaf-section) gives an injective [ring homomorphism](commutative-algebra.md#ring-homomorphism) from its [regular functions](#regular-function) to the [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety) $\mathcal O_{X,\eta}$. Injectivity follows on each nonempty [affine open subscheme](#affine-open-subscheme) from the injection of an [integral domain](commutative-algebra.md#integral-domain) into its [field of fractions](commutative-algebra.md#field-of-fractions), and then from the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom). This lets regular functions on different open subsets be compared inside one field.

#### Group scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_scheme)

A group scheme over a base scheme $S$ is an $S$-scheme $G$ with multiplication $m:G\times_SG\to G$, an identity section $e:S\to G$, and inversion $i:G\to G$ satisfying the group axioms as equalities of morphisms.

##### Homomorphism of group schemes

↑ **Parent:** [Group scheme](#group-scheme)

A homomorphism of group schemes $f:H\to G$ is a morphism over the base that commutes with multiplication: $f\circ m_H=m_G\circ(f\times f)$. It consequently preserves the identity and inversion.

##### Multiplication-by-n morphism

↑ **Parent:** [Group scheme](#group-scheme)

For a commutative [group scheme](#group-scheme) $G$, the multiplication-by-$n$ morphism $[n]_G:G\to G$ adds a point to itself $n$ times. On an [abelian variety](abelian-variety.md), it is surjective for every nonzero integer $n$.

#### Nonreduced scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is nonreduced when its structure sheaf contains a nonzero [nilpotent element](commutative-algebra.md#nilpotent). For an affine scheme $\operatorname{Spec}(A/I)$, this is equivalent to the ideal $I$ not being radical.

##### Nonreduced double point

↑ **Parent:** [Nonreduced scheme](#nonreduced-scheme)

The spectrum of the [dual number](commutative-algebra.md#dual-number) ring $k[\epsilon]/(\epsilon^2)$ is a [nonreduced scheme](#nonreduced-scheme) of length two supported at one point. Its nonzero nilpotent $\epsilon$ retains first-order information that the underlying singleton topological space forgets. It differs from the disjoint union of two reduced $k$-points.

#### Punctual scheme

↑ **Parent:** [Scheme](#scheme)

A scheme over an algebraically closed field is punctual when its underlying topological space consists of one closed rational point. It may have nontrivial nilpotent structure, such as $\operatorname{Spec}k[\varepsilon]/(\varepsilon^2)$.

#### Spectrum of a commutative ring

↑ **Parent:** [Scheme](#scheme)

The spectrum $\operatorname{Spec}A$ of a [commutative ring](commutative-algebra.md#commutative-ring) $A$ is the set of its [prime ideals](commutative-algebra.md#prime-ideal), with closed sets $V(I)=\{\mathfrak p:I\subseteq\mathfrak p\}$ and a structure sheaf whose sections locally look like fractions.

##### Spectrum map for the complexification of a real polynomial ring

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)

Contraction sends the zero [prime ideal](commutative-algebra.md#prime-ideal) to zero. A complex closed point $(x-z)$ contracts to $(x-z)$ when $z$ is real, and to $((x-\operatorname{Re}z)^2+(\operatorname{Im}z)^2)$ otherwise. Thus the map on the [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) is surjective and identifies each nonreal conjugate pair. Both spectra have only finite proper [Zariski-closed sets](algebraic-geometry.md#zariski-closed-set), so this is also the topological quotient by complex conjugation.

##### Disconnected reduced spectrum product decomposition

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)

For a [reduced ring](commutative-algebra.md#reduced-ring) with a nonempty disconnected [spectrum of a commutative ring](#spectrum-of-a-commutative-ring), choose a separation $V(I)\sqcup V(J)$. Disjointness gives $I+J=R$; covering the spectrum gives $IJ\subseteq\sqrt{(0)}=0$. For [comaximal ideals](commutative-algebra.md#comaximal-ideals), $I\cap J=IJ$. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) then supplies a product of two nonzero quotient [rings](commutative-algebra.md#ring). Equivalently, if $i+j=1$ with $i\in I$, $j\in J$, then $i,j$ are nontrivial orthogonal [idempotents](commutative-algebra.md#idempotent). This connects topology of the spectrum to [ring product decomposition by an idempotent](commutative-algebra.md#ring-product-decomposition-by-an-idempotent) without a Noetherian assumption.

##### Affine scheme

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_scheme)

An affine scheme is a [scheme](#scheme) isomorphic to $\operatorname{Spec}A$ for some [commutative ring](commutative-algebra.md#commutative-ring) $A$. Homomorphisms $A\to B$ correspond contravariantly to morphisms $\operatorname{Spec}B\to\operatorname{Spec}A$.

###### Affine gluing along closed subschemes

↑ **Parent:** [Affine scheme](#affine-scheme)

Suppose a scheme is the scheme-theoretic union of affine closed subschemes $Y=\operatorname{Spec}A$ and $Z=\operatorname{Spec}B$, meaning their ideal sheaves have zero intersection. The intersection $W$ is closed in both, hence affine with coordinate ring $C$ and surjections $A\to C$, $B\to C$. Then the whole scheme is $\operatorname{Spec}(A\times_CB)$. Both projections of this fiber product are surjective; their kernels have zero intersection and product, and their quotient by the sum is $C$. Thus its spectrum has the same closed pieces, intersection and topology. The structure sheaf is the kernel of $i_*\mathcal O_Y\oplus j_*\mathcal O_Z\to k_*\mathcal O_W$ on both spaces, identifying their locally ringed structures. A reduced Noetherian scheme has finitely many irreducible components, so induction proves it is affine if and only if its reduced irreducible components are affine. The intersection $W$ need not be reduced.

###### Cohomological criterion for affineness

↑ **Parent:** [Affine scheme](#affine-scheme)

A [Noetherian scheme](#noetherian-scheme) is affine exactly when every [coherent ideal sheaf](#coherent-ideal-sheaf) has zero first [sheaf cohomology](#sheaf-cohomology). One direction is [vanishing of quasi-coherent cohomology on an affine scheme](#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme). For the converse, ideal-sheaf vanishing produces [affine principal neighbourhoods from ideal-sheaf vanishing](#affine-principal-neighbourhoods-from-ideal-sheaf-vanishing). A finite such cover yields a [unit-ideal certificate from a principal affine cover](#unit-ideal-certificate-from-a-principal-affine-cover), and those [affine charts](#affine-chart-of-a-variety) glue to the [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) of [global sections](#global-section). The criterion, including the finite-type ideal version for quasi-compact quasi-separated schemes, is recorded in [Stacks Project, Section 30.3](https://stacks.math.columbia.edu/tag/01XE).

###### Unit-ideal certificate from a principal affine cover

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

If finitely many $X_{f_i}$ cover $X$, the morphism $\mathcal O_X^r\to\mathcal O_X$ with coefficients $f_i$ is onto. If its [kernel](linear-algebra.md#kernel-of-a-linear-map) has vanishing first [sheaf cohomology](#sheaf-cohomology), the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) lifts the [global section](#global-section) $1$ to coefficients $g_i$. This turns a geometric cover into a [unit ideal](commutative-algebra.md#unit-ideal) in the ring of [global sections](#global-section).

###### Affine principal neighbourhoods from ideal-sheaf vanishing

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

Let $P$ have an affine open neighbourhood $U$, and let $Y=X\setminus U$. Evaluation gives $\mathcal I_Y\twoheadrightarrow k_P$ with [kernel](linear-algebra.md#kernel-of-a-linear-map) $\mathcal I_Y\cap\mathcal I_P$. If first [sheaf cohomology](#sheaf-cohomology) of every [coherent ideal sheaf](#coherent-ideal-sheaf) vanishes, a [global section](#global-section) $f$ of $\mathcal I_Y$ can be chosen with $f(P)=1$. Then $X_f\subseteq U$ is a [principal open subset](#principal-open-subscheme) of an [affine variety](algebraic-geometry.md#affine-algebraic-set) and is affine.

###### Ideal-sheaf vanishing for a coherent submodule of a trivial bundle

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

If $H^1(X,\mathcal I)=0$ for every [coherent ideal sheaf](#coherent-ideal-sheaf), projection to the last coordinate makes any coherent $\mathcal F\subseteq\mathcal O_X^r$ an extension of a coherent submodule of $\mathcal O_X^{r-1}$ by an ideal sheaf. The [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) proves the assertion by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $r$.

###### Affine scheme reconstruction from global sections

↑ **Parent:** [Affine scheme](#affine-scheme)

For an [affine scheme](#affine-scheme) $X=\operatorname{Spec}A$, its ring of [global sections](#global-section) is $A$. A [morphism of schemes](#morphism-of-schemes) between affine schemes is determined contravariantly by its map on these rings. Consequently a morphism between affine schemes is an [isomorphism of schemes](#isomorphism-of-schemes) exactly when that ring map is an isomorphism. The affine hypothesis is essential, as the [punctured affine plane](#punctured-affine-plane) shows.

###### Affine open subscheme

↑ **Parent:** [Affine scheme](#affine-scheme)

An affine open subscheme is an [open subset](topology.md#open-set) of a [scheme](#scheme) with its restricted [structure sheaf](#structure-sheaf-of-a-scheme), which is itself an [affine scheme](#affine-scheme). Every scheme has an [open cover](topology.md#open-cover) by such subschemes. On an affine scheme, the [principal open subschemes](#principal-open-subscheme) give an [open basis](topology.md#basis-of-a-topology).

###### Affine chart of a variety

↑ **Parent:** [Affine open subscheme](#affine-open-subscheme)

An open subset of an [algebraic variety](algebraic-geometry.md#algebraic-variety) equipped with an identification with an [affine variety](algebraic-geometry.md#affine-algebraic-set). Such charts make [quasi-coherent sheaves](#quasi-coherent-sheaf) and regular maps accessible through their local [coordinate rings](algebraic-geometry.md#coordinate-ring).

###### Principal open subscheme

↑ **Parent:** [Affine scheme](#affine-scheme)

For $f\in A$, the principal open subset $D(f)=\{\mathfrak p:f\notin\mathfrak p\}$ of $\operatorname{Spec}A$ is the [affine scheme](#affine-scheme) $\operatorname{Spec}A_f$.

###### Dense principal open inside a dense open subset

↑ **Parent:** [Principal open subscheme](#principal-open-subscheme)

In an [affine variety](algebraic-geometry.md#affine-algebraic-set) with [coordinate ring](algebraic-geometry.md#coordinate-ring) $A$, every dense open subset $U$ contains a dense [principal open subset](#principal-open-subscheme). Write its closed complement as $V(I)$. Density says that $I$ is contained in none of the finitely many [minimal prime ideals](commutative-algebra.md#minimal-prime-ideal) of the [reduced ring](commutative-algebra.md#reduced-ring) $A$. [Prime avoidance](commutative-algebra.md#prime-avoidance) supplies $s\in I$ outside all these primes. Thus $D(s)\subseteq U$, and $s$ is a [non-zero-divisor](mathematics.md#non-zero-divisor). [Noetherian Zariski topology](algebraic-geometry.md#noetherian-zariski-topology) also makes $U$ a finite union of principal opens; one can add $D(s)$ to this cover. An arbitrary existing cover need not contain a dense member when the [variety](algebraic-geometry.md#algebraic-variety) is reducible.

###### Affine line

↑ **Parent:** [Affine scheme](#affine-scheme)

The affine line over a field $k$ is $\mathbb A_k^1=\operatorname{Spec}k[t]$.

The one-dimensional scheme has an [affine space](geometry-and-topology.md#affine-space) of rational points over its base field; its scheme structure also records non-rational points and local rings.

###### Affine plane

↑ **Parent:** [Affine scheme](#affine-scheme)

The affine plane over a field $k$ is the [affine scheme](#affine-scheme) $\operatorname{Spec}k[x,y]$.

The two-dimensional scheme has an [affine space](geometry-and-topology.md#affine-space) of rational points over its base field; its scheme structure also records non-rational points and local rings.

###### Real affine plane scheme points

↑ **Parent:** [Affine plane](#affine-plane)

The points of the real [affine plane](#affine-plane) as a [scheme](#scheme) are its [prime ideals](commutative-algebra.md#prime-ideal): the zero ideal, the principal ideals of irreducible real polynomials, and its [maximal ideals](commutative-algebra.md#maximal-ideal). The latter have [residue field](commutative-algebra.md#residue-field) $\mathbb R$ or $\mathbb C$, by the [Zariski lemma](algebraic-geometry.md#zariski-s-lemma) and the [real closed field](algebra.md#real-closed-field) property. They correspond respectively to real coordinate pairs and conjugate pairs of nonreal complex coordinate pairs. Thus the scheme contains both nonclosed [generic points](algebraic-geometry.md#generic-point) and closed points absent from the real locus. Its topology is the [Zariski topology](algebraic-geometry.md#zariski-topology), and its [structure sheaf](#structure-sheaf-of-a-scheme) has sections $\mathbb R[x,y]_h$ on each [principal open subscheme](#principal-open-subscheme) $D(h)$.

###### Punctured affine plane

↑ **Parent:** [Affine plane](#affine-plane)

The punctured affine plane is obtained by deleting the closed point $(x,y)$ from $\operatorname{Spec}k[x,y]$. Its regular functions still form $k[x,y]$, while

$$
H^1(\mathbb A_k^2\setminus\{0\},\mathcal O)\cong k[x^{\pm1},y^{\pm1}]/\bigl(k[x^{\pm1},y]+k[x,y^{\pm1}]\bigr),
$$

which has basis represented by $x^{-a}y^{-b}$ for $a,b\geq1$.

###### Nonaffineness of a punctured affine plane

↑ **Parent:** [Punctured affine plane](#punctured-affine-plane)

The [punctured affine plane](#punctured-affine-plane) $U=\mathbb A_k^2\setminus\{(0,0)\}$ is not an [affine scheme](#affine-scheme). On its cover $D(x)\cup D(y)$, [global sections](#global-section) are $k[x,y]_x\cap k[x,y]_y=k[x,y]$ inside the [field of fractions](commutative-algebra.md#field-of-fractions). Coprimality of $x$ and $y$ proves this equality. If $U$ were affine, its inclusion into $\mathbb A_k^2$ would be an isomorphism by [affine scheme reconstruction from global sections](#affine-scheme-reconstruction-from-global-sections), contradicting the omitted point.

###### Affine three-space

↑ **Parent:** [Affine scheme](#affine-scheme)

Affine three-space is $\operatorname{Spec}k[x_1,x_2,x_3]$.

The three-dimensional scheme has an [affine space](geometry-and-topology.md#affine-space) of rational points over its base field; its scheme structure also records non-rational points and local rings.

###### Punctured affine three-space

↑ **Parent:** [Affine three-space](#affine-three-space)

For $U=\mathbb A_k^3\setminus\{0\}$,

$$
H^0(U,\mathcal O_U)=k[x_1,x_2,x_3],\qquad H^1(U,\mathcal O_U)=0,
$$

and

$$
H^2(U,\mathcal O_U)\cong
\frac{k[x_1^{\pm1},x_2^{\pm1},x_3^{\pm1}]}{
k[x_1^{\pm1},x_2^{\pm1},x_3]+k[x_1^{\pm1},x_2,x_3^{\pm1}]+k[x_1,x_2^{\pm1},x_3^{\pm1}]}.
$$

The last group has basis represented by $x_1^{-a}x_2^{-b}x_3^{-c}$ for $a,b,c\geq1$, and all groups in degrees at least three vanish.

#### Noetherian scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noetherian_scheme)

A Noetherian scheme has a finite cover by affine schemes $\operatorname{Spec}A_i$ with each $A_i$ a [Noetherian ring](algebra.md#noetherian-ring). Equivalently, it is quasi-compact and locally Noetherian.

##### Regular scheme

↑ **Parent:** [Noetherian scheme](#noetherian-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_scheme)

A locally Noetherian scheme is regular when every local ring $\mathcal O_{X,x}$ is a [regular local ring](commutative-algebra.md#regular-local-ring).

###### Regular in codimension one

↑ **Parent:** [Regular scheme](#regular-scheme)

A Noetherian scheme is regular in codimension one when every local ring at a codimension-one point is regular. For an integral scheme these local rings are then discrete valuation rings.

##### Normal scheme

↑ **Parent:** [Noetherian scheme](#noetherian-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_scheme)

An integral locally Noetherian scheme is normal when every local ring is an [integrally closed domain](commutative-algebra.md#integrally-closed-domain).

More generally a scheme is normal when every local ring is an integrally closed domain; the scheme need not be globally integral, for example a disjoint union of normal integral components.

###### Normalization of an integral scheme

↑ **Parent:** [Normal scheme](#normal-scheme)

For an [integral scheme](#integral-scheme), take on each [affine chart](#affine-chart-of-a-variety) the [integral closure](commutative-algebra.md#integral-closure) of its coordinate [ring](commutative-algebra.md#ring) in its [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety). [Integral closure](commutative-algebra.md#integral-closure) commutes with [localization](commutative-algebra.md#localization-of-a-ring), so these [rings](commutative-algebra.md#ring) glue to a [normal scheme](#normal-scheme) with an integral birational morphism to the original [scheme](#scheme). This is the normalization. It need not be finite without additional hypotheses; for an algebraic curve of finite type over a [field](algebra.md#field) it is finite. It is an [isomorphism](algebra.md#isomorphism) exactly when the original [scheme](#scheme) is normal.

###### Normal variety

↑ **Parent:** [Normal scheme](#normal-scheme)

An [algebraic variety](algebraic-geometry.md#algebraic-variety) whose [local rings](commutative-algebra.md#local-ring) are [integrally closed domains](commutative-algebra.md#integrally-closed-domain). In particular an [irreducible variety](algebraic-geometry.md#irreducible-variety) that is a [normal variety](#normal-variety) has normal affine [coordinate rings](algebraic-geometry.md#coordinate-ring), enabling [codimension-two extension of regular functions on a normal variety](#codimension-two-extension-of-regular-functions-on-a-normal-variety).

###### Normal surface singularity

↑ **Parent:** [Normal variety](#normal-variety)

A singular point on a normal two-dimensional [algebraic variety](algebraic-geometry.md#algebraic-variety) has an integrally closed local domain which is not a regular local ring. A [rational double point](#rational-double-point) is an important isolated example with a crepant minimal resolution.

###### Rational double point

↑ **Parent:** [Normal surface singularity](#normal-surface-singularity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_double_point)

A rational double point is a normal surface singularity whose minimal resolution has a configuration of smooth rational $(-2)$-curves of type $A$, $D$ or $E$. Birational projective models of [K3 surfaces](complex-geometry.md#k3-surface) arising from nef big systems contract orthogonal $(-2)$-curves to these singularities.

###### Normality of a quadratic cone

↑ **Parent:** [Normal variety](#normal-variety)

Over an algebraically closed field of characteristic different from two, a nondegenerate quadratic form of rank at least three is irreducible, its cone has only the vertex singular, and its hypersurface ring is Cohen-Macaulay. Thus $(R_1)$ and $(S_2)$ in the [Serre criterion for normality](#serre-s-criterion-for-normality) hold. In characteristic two, the reduced zero variety of $\sum_i t_i^2$ is instead the hyperplane $\sum_i t_i=0$, which is normal. The unreduced double-hyperplane scheme is not normal.

###### Codimension-two extension of regular functions on a normal variety

↑ **Parent:** [Normal scheme](#normal-scheme)

For an integral [normal variety](#normal-variety) that is [Noetherian](algebra.md#noetherian-ring), removing a closed subset of codimension at least two does not create new [regular functions](#regular-function). Affine-locally, a normal Noetherian domain is the intersection of its localizations at height-one primes inside its [fraction field](commutative-algebra.md#field-of-fractions). The complement still contains every height-one point, so a [regular function](#regular-function) on it lies in each such [localization](commutative-algebra.md#localization-of-a-ring) and therefore in the original ring. On projective space this also follows directly by excluding [irreducible polynomial](polynomial.md#irreducible-polynomial) factor of the denominators on each polynomial [affine chart](#affine-chart-of-a-variety).

<h6 id="serre-s-criterion-for-normality">Serre's criterion for normality</h6>

↑ **Parent:** [Normal scheme](#normal-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Serre's_criterion_for_normality)

A Noetherian ring is normal exactly when it satisfies $(R_1)$, regularity in codimension one, and $(S_2)$, depth at least $\min(2,\dim)$ at every localization.

#### Morphism of schemes

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_schemes)

A morphism of schemes is a morphism of [locally ringed spaces](#locally-ringed-space). On affine schemes it is contravariantly equivalent to a homomorphism of their coordinate rings.

##### Graph morphism of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

For [morphisms of schemes](#morphism-of-schemes) $f:X\to Y$ and $g:Y\to Z$, the graph is the displayed map. It is the pullback of the [diagonal morphism](#diagonal-morphism) $Y\to Y\times_ZY$ along $(f\circ p_X,p_Y)$. Thus a [separated morphism](#separated-morphism) $g$ makes $\Gamma_f$ a [closed immersion](#closed-immersion). If also $g\circ f$ is a [closed immersion](#closed-immersion), the projection $X\times_ZY\to Y$ is a [closed immersion](#closed-immersion) by [base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes), and its composite with $\Gamma_f$ proves that $f$ is a [closed immersion](#closed-immersion).

##### Affine-target adjunction for schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A [morphism of schemes](#morphism-of-schemes) into an [affine scheme](#affine-scheme) is uniquely determined by its homomorphism on [global sections](#global-section). Conversely, a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $A\to\Gamma(X,\mathcal O_X)$ restricts on every [affine open subscheme](#affine-open-subscheme) of $X$ to a map into $\operatorname{Spec}A$; equality on affine covers of overlaps glues these maps. No quasi-compactness or affineness assumption on $X$ is needed.

##### Stein factorization

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stein_factorization)

A proper morphism $f:X\to Y$ factors as $X\xrightarrow{g}Z\xrightarrow{h}Y$, with $h$ finite and $g_*\mathcal O_X=\mathcal O_Z$; its fibers are connected. When $X$ is normal, $Z$ is normal. For a morphism from a smooth surface onto a curve, $Z$ is therefore a smooth projective curve over an algebraically closed field.

##### Isomorphism of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

An isomorphism of schemes is a [morphism of schemes](#morphism-of-schemes) admitting a two-sided inverse morphism. It is simultaneously a homeomorphism of the underlying spaces and an isomorphism of their structure sheaves.

##### Fiber product of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fiber_product_of_schemes)

The fibre product $X\times_SY$ represents pairs of morphisms to $X$ and $Y$ with equal composites to $S$. Affine-locally,

$$
\operatorname{Spec}A\times_{\operatorname{Spec}R}\operatorname{Spec}B
=\operatorname{Spec}(A\otimes_RB).
$$

###### Scheme-theoretic intersection

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For two [closed subschemes](#closed-subscheme) of a [scheme](#scheme) $X$, their intersection is their [fiber product of schemes](#fiber-product-of-schemes) over $X$. On an affine chart, ideals $I,J$ give the quotient by $I+J$. This retains nonreduced structure and [intersection multiplicities](algebraic-geometry.md#intersection-multiplicity) which a set-theoretic intersection would lose.

###### Point-lifting property of a scheme fibre product

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For [morphisms of schemes](#morphism-of-schemes) $X\to S$, $Y\to S$, a pair of points $x,y$ lifts to a point of $X\times_SY$ exactly when their base images agree. For sufficiency use the nonempty [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) of $\kappa(x)\otimes_{\kappa(s)}\kappa(y)$, by [tensor product of field extensions is nonzero](module-theory.md#tensor-product-of-field-extensions-is-nonzero). This establishes existence, not uniqueness, of a lift.

###### Scheme-theoretic fibre

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

The fibre of a [morphism of schemes](#morphism-of-schemes) over $y\in Y$ is its base change to the [residue field](commutative-algebra.md#residue-field) $\kappa(y)$. For $\operatorname{Spec}B\to\operatorname{Spec}A$, with $y$ corresponding to $\mathfrak p$, its fibre ring is $B\otimes_A\kappa(\mathfrak p)$. Its [structure sheaf](#structure-sheaf-of-a-scheme) records nilpotents and multiplicities that the set-theoretic inverse image cannot see.

###### Nonaffine special fibre obtained by blowing up

↑ **Parent:** [Scheme-theoretic fibre](#scheme-theoretic-fibre)

Blow up $(0,1,0)$ in $\mathbb A^3_{x,y,z}$ and compose with $xy:\mathbb A^3\to\mathbb A^1$. Nonzero fibres are $\mathbb G_m\times\mathbb A^1$. The zero fibre consists of the strict transforms of the two coordinate planes and the exceptional $\mathbb P^2$, all with multiplicity one. Its plane crossings make it singular; its closed $\mathbb P^2$ makes it nonaffine. The centre is deliberately on just one component of $xy=0$, keeping the fibre reduced.

###### Real fourth-power fibre classification

↑ **Parent:** [Scheme-theoretic fibre](#scheme-theoretic-fibre)

The [scheme-theoretic fibres](#scheme-theoretic-fibre) over positive real points, negative real points, zero, and nonreal [closed points](topology.md#closed-point) have real coordinate algebras $\mathbb R^2\times\mathbb C$, $\mathbb C^2$, $\mathbb R[x]/(x^4)$, and $\mathbb C^4$, respectively. Their ordinary [irreducible component](algebraic-geometry.md#irreducible-component) counts are $3,2,1,4$, so there are four real-scheme isomorphism classes. The last case pulls back an irreducible quadratic to a squarefree degree-eight polynomial, with four conjugate pairs of nonreal roots. The zero fibre retains its nilpotents and is not a reduced point.

###### Nonreduced reducible fibre between integral schemes

↑ **Parent:** [Scheme-theoretic fibre](#scheme-theoretic-fibre)

A [morphism of schemes](#morphism-of-schemes) between [integral schemes](#integral-scheme) can have a [scheme-theoretic fibre](#scheme-theoretic-fibre) that is neither reduced nor irreducible. For the map of [affine lines](#affine-line) given by $t=x^2(x-1)^2$, the fibre at $t=0$ has ring $k[x]/(x^2(x-1)^2)$. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) identifies it with the product of two [dual number](commutative-algebra.md#dual-number) rings, so it consists of two [nonreduced double points](#nonreduced-double-point). Its nilpotent structure is invisible to the set-theoretic fibre.

###### Integrality of the generic fibre of an affine dominant morphism

↑ **Parent:** [Scheme-theoretic fibre](#scheme-theoretic-fibre)

For an injective [ring homomorphism](commutative-algebra.md#ring-homomorphism) between nonzero [integral domains](commutative-algebra.md#integral-domain) $A\to B$, the [scheme-theoretic fibre](#scheme-theoretic-fibre) over the [generic point](algebraic-geometry.md#generic-point) of $\operatorname{Spec}A$ is $\operatorname{Spec}(S^{-1}B)$ with $S=A\setminus\{0\}$. Localization at these nonzero elements is a nonzero integral domain, so the generic fibre is a nonempty [integral scheme](#integral-scheme). A surjective morphism between these affine schemes necessarily gives an injective ring map: a prime above $(0)$ contains its kernel.

###### Universal property of a fibre product

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For morphisms $X\to S$ and $Y\to S$, maps $T\to X\times_SY$ are naturally equivalent to pairs of maps $T\to X$ and $T\to Y$ whose composites to $S$ agree.

###### Base change of a morphism of schemes

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

Given $f:X\to Y$ and $g:Y'\to Y$, the base change of $f$ along $g$ is the projection

$$
X\times_YY'\longrightarrow Y'.
$$

Properties such as being [proper](#proper-morphism) and [flat](#flat-morphism) are stable under arbitrary base change.

###### Global-section base-change failure in a flat projective family

↑ **Parent:** [Base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes)

Flatness of a projective family does not by itself force global sections to commute with [base change](#base-change-of-a-morphism-of-schemes). For a discrete valuation ring with uniformizer $\pi$, glue $\operatorname{Spec}R[\pi t,t^2,t^3]$ to $\operatorname{Spec}R[t^{-1}]$ along $\operatorname{Spec}R[t,t^{-1}]$. In the projective model with coordinates $(1,\pi t,t^2,t^3)$, the global ring is $R$. The special-fibre first chart has an additional square-zero element $a$ annihilated by $t^2,t^3$; it vanishes on the overlap and therefore extends by zero to a global section. The special-fibre global ring is $k[a]/(a^2)$, and base change from $R$ reaches only its constants.

###### Complexification fibres of a real scheme

↑ **Parent:** [Base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes)

For a [scheme](#scheme) over $\mathbb R$, its [base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes) to $\mathbb C$ has [scheme-theoretic fibre](#scheme-theoretic-fibre) over a point $p$ equal to $\operatorname{Spec}(\kappa(p)\otimes_{\mathbb R}\mathbb C)$. This is the spectrum of $\kappa(p)[s]/(s^2+1)$. It has two points if $-1$ is a square in the [residue field](commutative-algebra.md#residue-field), and otherwise one point with a quadratic [field extension](algebra.md#field-extension). In both cases it is reduced, because the quadratic polynomial has no repeated root in [characteristic zero](algebra.md#characteristic-zero). The distinction applies to [generic points](algebraic-geometry.md#generic-point) as well as [closed points](topology.md#closed-point).

###### Surjectivity is preserved by base change

↑ **Parent:** [Base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes)

If $X\to Y$ is a surjective [morphism of schemes](#morphism-of-schemes), the projection $X\times_YY^{\prime}\to Y^{\prime}$ is surjective for every $Y^{\prime}\to Y$. For a point $y\prime$, choose a point $x$ over its base image and apply the [point-lifting property of a scheme fibre product](#point-lifting-property-of-a-scheme-fibre-product). No flatness assumption is necessary.

##### Locally closed immersion

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A locally closed immersion factors as a closed immersion followed by an open immersion. Equivalently, it identifies its source with a closed subscheme of an open subscheme of the target.

###### Open immersion

↑ **Parent:** [Locally closed immersion](#locally-closed-immersion)

An open immersion is a [morphism of schemes](#morphism-of-schemes) that identifies its source with an open subscheme of its target. It is an isomorphism onto that open subscheme as a [locally ringed space](#locally-ringed-space).

###### Diagonal morphism

↑ **Parent:** [Locally closed immersion](#locally-closed-immersion)

The diagonal morphism sends a point to the pair consisting of that point twice. Every diagonal of schemes is a locally closed immersion, and a morphism is separated exactly when its diagonal is a closed immersion.

###### Coincidence locus of two scheme morphisms

↑ **Parent:** [Diagonal morphism](#diagonal-morphism)

For morphisms $f,g:X\to Y$ over a base $S$, their scheme-theoretic coincidence locus is the fibre product

$$
\operatorname{Eq}(f,g)=X\times_{(f,g),\,Y\times_SY,\,\Delta_{Y/S}}Y.
$$

It is the [equalizer](category.md#equaliser) of $f$ and $g$, hence is universal among subschemes on which they agree. It is locally closed because every diagonal is an immersion, and closed when $Y\to S$ is separated.

<h5 id="kahler-differential">Kähler differential</h5>

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_differential)

For a ring map $A\to B$, the module of Kähler differentials represents $A$-derivations: $\operatorname{Hom}_B(\Omega_{B/A},M)\cong\operatorname{Der}_A(B,M)$.

For an algebra $B$ over $A$, the module $\Omega_{B/A}$ represents $A$-linear derivations: every derivation $B\to N$ factors uniquely through the universal map $d:B\to\Omega_{B/A}$.

<h6 id="kahler-differentials-under-a-separable-field-extension">Kähler differentials under a separable field extension</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

For finite separable $L/F$, every $k$-[derivation](associative-algebra.md#derivation-of-an-algebra) on $F$ into an $L$-module extends uniquely to $L$. Differentiate the minimal polynomial of each algebraic generator and divide by its nonzero derivative. Consequently the [Transitivity exact sequence for Kähler differentials](#transitivity-exact-sequence-for-kahler-differentials) identifies $\Omega_{L/k}$ with $L\otimes_F\Omega_{F/k}$, and $\Omega_{L/F}=0$.

<h6 id="base-change-for-kahler-differentials">Base change for Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

The [Kähler differentials](#kahler-differential) commute with extension of the base ring. A derivation of the base-changed algebra that kills $k'$ is determined by its restriction to $A\otimes1$, and the [Leibniz rule](calculus.md#leibniz-rule) provides its unique extension. No flatness hypothesis is required for this isomorphism.

<h6 id="localization-of-kahler-differentials">Localization of Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

[Kähler differentials](#kahler-differential) commute with [localization of a ring](commutative-algebra.md#localization-of-a-ring). The quotient rule $d(a/s)=(s\,da-a\,ds)/s^2$ uniquely extends a [derivation](associative-algebra.md#derivation-of-an-algebra) after inverting $s$; its universal property proves the displayed module isomorphism.

<h6 id="kahler-differentials-of-a-polynomial-algebra">Kähler differentials of a polynomial algebra</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

The [Kähler differentials](#kahler-differential) of a [polynomial ring](commutative-algebra.md#polynomial-ring) are free on the differentials of its variables. Assigning arbitrary values to these generators uniquely defines a [derivation](associative-algebra.md#derivation-of-an-algebra). Applying the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials) to a quotient gives its presentation by the formal derivatives of its defining equations.

<h6 id="universal-property-of-kahler-differentials">Universal property of Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

Composing an $A$-linear map with $d:A\to\Omega_{A/k}$ gives a $k$-[derivation](associative-algebra.md#derivation-of-an-algebra). Every derivation factors uniquely this way because its linearity and product rule are exactly the defining relations of the [module of Kähler differentials](#kahler-differential).

###### Conormal module of the diagonal

↑ **Parent:** [Kähler differential](#kahler-differential)

For a commutative $k$-algebra $A$, let $I$ be the kernel of multiplication $\mu:A\otimes_k A\to A$. The formula $a\mapsto[1\otimes a-a\otimes1]$ is a [derivation of an algebra](associative-algebra.md#derivation-of-an-algebra) into the [quotient module](module-theory.md#quotient-module) $I/I^2$, with $A$ acting through the first factor. It induces an isomorphism from the [module of Kähler differentials](#kahler-differential). An inverse is induced by $q(x\otimes y)=x\,dy$: the identity $q(rs)=\mu(r)q(s)+\mu(s)q(r)$ shows $q(I^2)=0$. For $z=\sum_i x_i\otimes y_i\in I$, the equality $\sum_i x_i y_i=0$ gives $[z]=\sum_i x_i[1\otimes y_i-y_i\otimes1]$, proving that the two maps are inverse. For an [affine variety](algebraic-geometry.md#affine-algebraic-set), $I$ is the defining ideal of its [diagonal morphism](#diagonal-morphism).

<h6 id="conormal-exact-sequence-for-kahler-differentials">Conormal exact sequence for Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

For $A\to B\to C=B/I$, there is a right-exact sequence

$$
I/I^2\longrightarrow\Omega_{B/A}\otimes_BC\longrightarrow\Omega_{C/A}\longrightarrow0,
$$

where $[i]\mapsto di\otimes1$ and $db\otimes c\mapsto c\,d\bar b$.

###### Conormal sheaf

↑ **Parent:** [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials)

For a closed immersion, this [quasi-coherent sheaf](#quasi-coherent-sheaf) measures the first-order equations of the subvariety. Its local [module](module-theory.md#module-mathematics) is $I/I^2$, and its map to the restricted [Kähler differential sheaf](#sheaf-of-kahler-differentials-over-a-field) sends the class of $f$ to $df$. This is the definition in [Stacks Project, Section 29.32](https://stacks.math.columbia.edu/tag/01R1).

###### Normal sheaf

↑ **Parent:** [Conormal sheaf](#conormal-sheaf)

For a [closed immersion](#closed-immersion) $i:Z\hookrightarrow X$ with [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$, the normal sheaf is $\mathcal N_{Z/X}=\mathcal Hom_{\mathcal O_Z}(\mathcal I/\mathcal I^2,\mathcal O_Z)$. It is the dual of the [conormal sheaf](#conormal-sheaf). For a regular embedding it is a [locally free sheaf](#locally-free-sheaf); in the smooth case it agrees with the [normal bundle](algebraic-geometry.md#normal-bundle). Without regularity it need not be locally free, but its [global sections](#global-section) still classify [first-order embedded deformations](algebraic-geometry.md#first-order-embedded-deformation).

###### Normal sheaf of a projective complete intersection

↑ **Parent:** [Normal sheaf](#normal-sheaf)

If a [projective complete intersection](#projective-complete-intersection) $Z\subseteq\mathbf P^n$ is cut out by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of degrees $d_1,\ldots,d_c$, then $\mathcal I/\mathcal I^2\cong\bigoplus_j\mathcal O_Z(-d_j)$ and $\mathcal N_{Z/\mathbf P^n}\cong\bigoplus_j\mathcal O_Z(d_j)$. The classes of the defining equations form the conormal basis: the first syzygies of a [regular sequence](commutative-algebra.md#regular-sequence) are the [Koszul complex](homology.md#koszul-complex) relations, whose coefficients vanish modulo the defining ideal. Thus the generator classes have no residual linear relations. Dualizing gives the stated [normal sheaf](#normal-sheaf).

###### Conormal injectivity for a generically smooth Cartier divisor

↑ **Parent:** [Conormal sheaf](#conormal-sheaf)

Let $W$ be an integral [effective Cartier divisor](cartier-divisor.md#effective-cartier-divisor) in an integral [variety](algebraic-geometry.md#algebraic-variety) $V$ over a [perfect field](algebra.md#perfect-field), and suppose $W$ is not contained in the singular locus of $V$. On a dense open subset both [varieties](algebraic-geometry.md#algebraic-variety) are smooth. The [Zariski tangent space](algebraic-geometry.md#zariski-tangent-space) of $W$ there has codimension one in that of $V$, so the differential of the local defining equation is nonzero. Thus the [conormal sheaf](#conormal-sheaf) map is injective generically. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) is a subsheaf of a [line bundle](#line-bundle) on the integral [variety](algebraic-geometry.md#algebraic-variety) $W$ and is therefore a [torsion-free sheaf](#torsion-free-sheaf); generic vanishing implies zero everywhere. Right exactness is the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials).

<h6 id="transitivity-exact-sequence-for-kahler-differentials">Transitivity exact sequence for Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

For ring maps $A\to B\to C$, the first or transitivity exact sequence is

$$
\Omega_{B/A}\otimes_BC\longrightarrow\Omega_{C/A}\longrightarrow\Omega_{C/B}\longrightarrow0.
$$

The maps send $db\otimes c$ to $c\,db$ and then kill differentials of elements coming from $B$.

<h6 id="sheaf-of-relative-kahler-differentials">Sheaf of relative Kähler differentials</h6>

↑ **Parent:** [Kähler differential](#kahler-differential)

For a morphism of schemes $X\to Y$, the sheaf of relative Kähler differentials is obtained by sheafifying the modules $\Omega_{B/A}$ on affine charts $\operatorname{Spec}B\to\operatorname{Spec}A$.

###### Tangent sheaf of a scheme

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

The relative tangent sheaf is the [dual of a sheaf](#dual-of-a-sheaf) of [Kähler differentials](#kahler-differential). Its sections are derivations of the [structure sheaf](#structure-sheaf-of-a-scheme) that kill base scalars. For a [smooth morphism](#smooth-morphism) it is [locally free](#locally-free-sheaf) and describes first-order deformations of sections into the scheme.

###### Cotangent-sheaf cohomology of projective space

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For $n\geq1$, the cotangent form of the [Euler sequence](algebraic-geometry.md#euler-sequence) is $0\to\Omega^1_{\mathbb P^n/k}\to\mathcal O(-1)^{\oplus(n+1)}\to\mathcal O\to0$. The [cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) and the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) give $H^1(\mathbb P_k^n,\Omega^1)\cong k$, with every other cohomology group zero. Therefore the [Euler characteristic of a coherent sheaf](#euler-characteristic-of-a-coherent-sheaf) is $-1$. The nonzero class is the connecting image of the constant section $1$.

<h6 id="sheaf-of-kahler-differentials-over-a-field">Sheaf of Kähler differentials over a field</h6>

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For a [variety](algebraic-geometry.md#algebraic-variety) over $k$, the [module of Kähler differentials](#kahler-differential) $\Omega_{A/k}$ on each [affine chart](#affine-chart-of-a-variety) gives a [quasi-coherent sheaf](#quasi-coherent-sheaf). Compatibility with [localization](commutative-algebra.md#localization-of-a-ring) glues these into $\Omega^1_{X/k}$. A [finite presentation of an algebra](algebra.md#finite-presentation-of-an-algebra) gives a [finite presentation of a module](module-theory.md#finite-presentation-of-a-module) for its differentials, so this is a [coherent sheaf](#coherent-sheaf) on a [variety](algebraic-geometry.md#algebraic-variety).

###### Algebraic cotangent bundle

↑ **Parent:** [Sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field)

For a smooth [algebraic variety](algebraic-geometry.md#algebraic-variety) of dimension $r$ over a field, the [sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field) is locally free of rank $r$ and defines its algebraic cotangent bundle. Its dual is the [tangent sheaf of a scheme](#tangent-sheaf-of-a-scheme). For a smooth hypersurface of degree $d$ in $\mathbb P^n$, the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials) is the short exact sequence $0\to\mathcal O_X(-d)\to\Omega^1_{\mathbb P^n}|_X\to\Omega^1_X\to0$.

###### Local freeness of differentials on a smooth variety

↑ **Parent:** [Sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field)

An invertible maximal-rank minor in the [Jacobian matrix](calculus.md#jacobian-matrix) eliminates generators and gives a local surjection from $\mathcal O_X^n$ to the [Kähler differential sheaf](#sheaf-of-kahler-differentials-over-a-field). For an integral smooth [variety](algebraic-geometry.md#algebraic-variety) the map is an [isomorphism](algebra.md#isomorphism) at the [generic point](algebraic-geometry.md#generic-point). Its [kernel](linear-algebra.md#kernel-of-a-linear-map) is a submodule of a [free module](module-theory.md#free-module) over an [integral domain](commutative-algebra.md#integral-domain), so it is a [torsion-free module](module-theory.md#torsion-free-module); vanishing generically forces it to be zero. This gives local free frames for differentials.

###### Canonical line bundle of a smooth variety

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For a smooth $n$-dimensional variety $X$ over a field, its canonical [line bundle](#line-bundle) is $\omega_X=\bigwedge^n\Omega^1_{X/k}$. It is the bundle of top-degree algebraic differential forms. A nonzero rational section defines a [canonical divisor of a smooth variety](#canonical-divisor-of-a-smooth-variety). This algebraic definition works in arbitrary characteristic and is distinct from restricting the analytic canonical-bundle definition to complex manifolds.

###### Canonical divisor of a smooth variety

↑ **Parent:** [Canonical line bundle of a smooth variety](#canonical-line-bundle-of-a-smooth-variety)

A canonical divisor $K_X$ on a smooth integral variety is the [Cartier divisor](cartier-divisor.md) of a nonzero rational top-degree differential form; $\mathcal O_X(K_X)\cong\omega_X$. Its linear-equivalence class is independent of the chosen form. The [plurigenus](#plurigenus) is the dimension of the space of sections of a positive tensor power of this bundle.

###### Plurigenus

↑ **Parent:** [Canonical divisor of a smooth variety](#canonical-divisor-of-a-smooth-variety)

For a smooth [projective variety](projective-space.md#projective-variety), its $m$th plurigenus is $P_m(X)=h^0(X,\omega_X^{\otimes m})$, for $m\ge1$. These dimensions describe pluricanonical linear systems. [Blowup invariance of plurigenera](#blowup-invariance-of-plurigenera) proves their invariance under a point blowup on a smooth surface.

###### Blowup invariance of plurigenera

↑ **Parent:** [Plurigenus](#plurigenus)

For a point [blowup of a smooth algebraic surface](algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) $\psi:\widetilde X\to X$, where $X$ is a [smooth projective surface](algebraic-geometry.md#smooth-projective-surface) over an algebraically closed [field](algebra.md#field), multiplication by the exceptional section to power $m$ identifies $H^0(\widetilde X,m\psi^*K_X)$ with $H^0(\widetilde X,mK_{\widetilde X})$. Every effective pluricanonical representative must contain $mE$, since after subtracting $j<m$ copies its intersection with $E$ is $-m+j<0$. The [projection formula for sheaves](#projection-formula) and $\psi_*\mathcal O=\mathcal O$ identify the remaining sections with those on $X$. No effectivity of $K_X$ itself is assumed.

##### Affine morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_morphism)

A morphism $f:X\to Y$ is affine when the inverse image of every affine open subscheme of $Y$ is affine. For a [quasi-coherent sheaf](#quasi-coherent-sheaf) $\mathcal F$ on $X$, one has $R^qf_*\mathcal F=0$ for $q>0$.

###### Cohomology under an affine morphism

↑ **Parent:** [Affine morphism](#affine-morphism)

For an [affine morphism](#affine-morphism) $f:X\to Y$ and a [quasi-coherent sheaf](#quasi-coherent-sheaf) $\mathcal F$ on $X$, the [direct image sheaf](#direct-image-sheaf) has the same [sheaf cohomology](#sheaf-cohomology) on $Y$ as $\mathcal F$ on $X$. To prove this, take a [flasque resolution](#flasque-resolution) $\mathcal F\to\mathcal I^\bullet$. Its direct images are [flasque sheaves](#flasque-sheaf). On each affine open $V\subset Y$, the complex of sections of the direct images is $\Gamma(f^{-1}V,\mathcal I^\bullet)$. By [vanishing of quasi-coherent cohomology on an affine scheme](#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme), this augmented complex is exact. Checking on the affine basis proves that $f_*\mathcal I^\bullet$ resolves $f_*\mathcal F$. Its global sections are identical to those of the original resolution.

##### Flat morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_morphism)

A morphism $f:X\to Y$ is flat at $x\in X$ when the local ring $\mathcal O_{X,x}$ is a [flat module](module-theory.md#flat-module) over $\mathcal O_{Y,f(x)}$. It is flat when it is flat at every point.

###### Finite flat rank over an irreducible scheme

↑ **Parent:** [Flat morphism](#flat-morphism)

For a [finite morphism](algebraic-geometry.md#finite-morphism) that is flat, its direct-image algebra is finite free at every local stalk. On an [irreducible scheme](#irreducible-scheme), every point specializes from the same generic point. Localizing each stalk further at that generic point shows that all these free ranks equal the generic rank. Hence all fibre algebras have the same dimension, even without assuming finite presentation in advance.

##### Morphism of finite type

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_finite_type)

A morphism $f:X\to Y$ is of finite type when every point of $Y$ has an affine neighborhood $V=\operatorname{Spec}A$ for which $f^{-1}V$ has a finite affine cover $\operatorname{Spec}B_i$ with each $B_i$ a finitely generated $A$-algebra.

###### Quasi-finite morphism

↑ **Parent:** [Morphism of finite type](#morphism-of-finite-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-finite_morphism)

A finite-type [morphism of schemes](#morphism-of-schemes) is quasi-finite if its fibres are finite discrete schemes. A proper quasi-finite morphism is a [finite morphism](algebraic-geometry.md#finite-morphism). In particular, a proper finite-type morphism of [projective varieties](projective-space.md#projective-variety) with no positive-dimensional fibres is finite; a positive-dimensional projective fibre would contain an integral curve.

##### Universally closed morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universally_closed_morphism)

A morphism is universally closed when every base change is a closed map on underlying topological spaces.

###### Projective line with a doubled point

↑ **Parent:** [Universally closed morphism](#universally-closed-morphism)

Glue two copies of $\mathbb P_k^1$ by the identity away from one chosen point. The resulting finite-type scheme is universally closed over $k$: after any base change, a closed subset meets each projective-line chart in a closed subset whose image is closed, and the total image is their finite union. The two copies of the chosen point cannot be separated, so the structure morphism is not separated and therefore is not proper.

##### Separated morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A morphism $f:X\to Y$ is separated when its diagonal $X\to X\times_YX$ is a [closed immersion](#closed-immersion). This is the scheme-theoretic analogue of the Hausdorff property.

A morphism of [schemes](#scheme) is separated when its diagonal is a [closed immersion](#closed-immersion). This is a property of the morphism, distinct from the broader morphism or diagonal constructions.

###### Separated scheme

↑ **Parent:** [Separated morphism](#separated-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separated_scheme)

A scheme over a base $S$ is separated when its structure morphism to $S$ is a [separated morphism](#separated-morphism). An absolute scheme is usually called separated when it is separated over $\operatorname{Spec}\mathbb Z$.

###### Separated variety

↑ **Parent:** [Separated scheme](#separated-scheme)

An [algebraic variety](algebraic-geometry.md#algebraic-variety) that is separated over its ground field. Two affine open charts have an affine intersection: their intersection is the inverse image of the closed diagonal inside the product of the two [affine charts](#affine-chart-of-a-variety). This ensures a finite affine cover is acyclic for [quasi-coherent sheaves](#quasi-coherent-sheaf).

###### Valuative criterion for separatedness

↑ **Parent:** [Separated morphism](#separated-morphism)

For a finite-type morphism of [Noetherian schemes](#noetherian-scheme), separatedness is equivalent to uniqueness in every lifting problem $\operatorname{Spec}K\to X$ over $\operatorname{Spec}R\to Y$, where $R$ is a [valuation ring](commutative-algebra.md#valuation-ring) with [fraction field](commutative-algebra.md#field-of-fractions) $K$.

This is the uniqueness part of the [valuative criterion](#valuative-criterion).

##### Proper morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_morphism)

A morphism is proper when it is separated, of finite type, and universally closed. Properness is stable under base change and composition.

###### Complete variety

↑ **Parent:** [Proper morphism](#proper-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_variety)

A [variety](algebraic-geometry.md#algebraic-variety) over a field $k$ is complete when its map to $\operatorname{Spec}k$ is [universally closed](#universally-closed-morphism): after any base change, projection sends closed subsets to closed subsets. For a separated finite-type [variety](algebraic-geometry.md#algebraic-variety), this is equivalent to being [proper](#proper-morphism). In the classical algebraically closed setting one may test projections $X\times Y\to Y$ for arbitrary [varieties](algebraic-geometry.md#algebraic-variety). Images of rational points over a non-algebraically-closed field must not replace geometric images.

###### Proper affine morphisms are finite

↑ **Parent:** [Proper morphism](#proper-morphism)

For a finite-type affine morphism of Noetherian schemes, apply its valuative lifting property to each domain quotient $B/\mathfrak q$ for a minimal prime and all valuation rings of its fraction field containing the image of $A$. The lift forces $B/\mathfrak q$ into every such valuation ring, hence makes it integral over that image. For each $b\in B$, multiply the finitely many resulting monic equations. Its value at $b$ lies in the nilradical. The nilradical of a Noetherian ring is nilpotent, so a power of this monic polynomial annihilates $b$. Thus $B$ is integral over $A$. Finitely many algebra generators, each satisfying a monic equation, have their powers reduced to finitely many monomials, proving that $B$ is a finite $A$-module. Nilpotents cannot be ignored in this proof.

###### Properness descends from a surjective source

↑ **Parent:** [Proper morphism](#proper-morphism)

Suppose $gf$ is proper, $f$ is surjective, and $g$ is separated and of finite type. Surjectivity of scheme morphisms is preserved by base change: a nonempty fiber remains nonempty after a residue-field extension. After any base change to $Z$, for a closed subset $C$ of the new target of $f$, its inverse image is closed and has image $g(C)$ under the proper composite. Thus $g(C)$ is closed. This proves universal closedness of $g$, completing the three conditions for properness.

###### Properness cancels through a separated morphism

↑ **Parent:** [Proper morphism](#proper-morphism)

If $X\xrightarrow fY\xrightarrow gZ$ has proper composite and $g$ is separated, the graph $X\to X\times_ZY$ is a closed immersion, being a base change of the diagonal of $g$. The projection $X\times_ZY\to Y$ is a base change of the proper composite. Their composition is $f$, so $f$ is proper.

###### Properness is local on the target

↑ **Parent:** [Proper morphism](#proper-morphism)

If $f:X\to Y$ is a [morphism of schemes](#morphism-of-schemes) and $(U_i)$ is an open cover of $Y$, then $f$ is [proper](#proper-morphism) exactly when every restriction $f^{-1}(U_i)\to U_i$ is proper. The three defining properties—finite type, separatedness, and universal closedness—can each be checked on an open cover of the target.

###### Proper closed-point fibers do not imply properness

↑ **Parent:** [Proper morphism](#proper-morphism)

A finite-type morphism can have a proper fiber over every closed point without being proper. Properness controls compatible specialization in families, as expressed by the [valuative criterion for properness](#valuative-criterion-for-properness), rather than only the individual closed fibers.

###### Finite complex computing cohomology in a proper flat family

↑ **Parent:** [Proper morphism](#proper-morphism)

For a proper morphism $X\to\operatorname{Spec}A$ with $A$ Noetherian and an $A$-flat coherent sheaf $\mathcal F$, locally on the base there is a bounded complex of finite free modules $K^\bullet$ such that

$$
H^p(X,\mathcal F\otimes_AM)\cong H^p(K^\bullet\otimes_AM)
$$

naturally for every $A$-module $M$.

###### Cohomology and base change for line bundles on a curve

↑ **Parent:** [Finite complex computing cohomology in a proper flat family](#finite-complex-computing-cohomology-in-a-proper-flat-family)

In a proper flat family of [algebraic curves](algebraic-geometry.md#algebraic-curve), if the first [sheaf cohomology](#sheaf-cohomology) of a [line bundle](#line-bundle) vanishes on every fibre of an open set, its direct image there is a [vector bundle](fiber-bundle.md#vector-bundle) of rank given by the [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) and commutes with arbitrary [base change](#base-change-of-a-morphism-of-schemes). Locally a finite free complex computes both fibre [sheaf cohomology](#sheaf-cohomology) groups. Vanishing of the last cokernel makes its last map surjective; splitting that map leaves a finite locally free kernel in degree zero. This is the mechanism behind charts of the [Picard scheme of a curve](#picard-scheme-of-a-curve) and evaluation descriptions of the [theta divisor](abelian-variety.md#theta-divisor).

###### Semicontinuity theorem for coherent cohomology

↑ **Parent:** [Finite complex computing cohomology in a proper flat family](#finite-complex-computing-cohomology-in-a-proper-flat-family)

For a proper morphism of Noetherian schemes and a coherent sheaf flat over the base, the fiber dimension $s\mapsto\dim_{\kappa(s)}H^p(X_s,\mathcal F_s)$ is upper semicontinuous, and the fiberwise Euler characteristic is locally constant.

###### Constancy of line bundle degree in a family

↑ **Parent:** [Semicontinuity theorem for coherent cohomology](#semicontinuity-theorem-for-coherent-cohomology)

For a [line bundle](#line-bundle) $M$ on $C\times T$, with $C$ a smooth projective curve, this function is locally constant. Twist both $M$ and $M^{-1}$ by a large power of an [ample line bundle](#ample-line-bundle) on $C$. Near a chosen fiber their first [sheaf cohomology](#sheaf-cohomology) groups vanish. The [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) and upper semicontinuity of their zeroth [sheaf cohomology](#sheaf-cohomology) groups then bound the degree from above and below by the degree on that fiber. Connectedness of $T$ is necessary for a single constant across all fibers.

###### Valuative criterion for properness

↑ **Parent:** [Proper morphism](#proper-morphism)

For a finite-type morphism of [Noetherian schemes](#noetherian-scheme), properness is equivalent to existence and uniqueness in every lifting problem from the generic point $\operatorname{Spec}K$ of a [valuation ring](commutative-algebra.md#valuation-ring) $R$ to $\operatorname{Spec}R$.

This is the existence-and-uniqueness part of the [valuative criterion](#valuative-criterion).

###### Projective morphism

↑ **Parent:** [Proper morphism](#proper-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_morphism)

A morphism $X\to S$ is projective when it factors as a [closed immersion](#closed-immersion) $X\hookrightarrow\mathbb P_S^n$ followed by the projection to $S$. Every projective morphism is proper.

###### Closedness of projection from projective space

↑ **Parent:** [Projective morphism](#projective-morphism)

Projection $X\times\mathbb P^n\to X$ sends closed subsets to closed subsets, with geometric points or schemes understood. On an affine base, choose finitely many homogeneous equations for a closed subset. Its fiber is nonempty exactly when every [graded multiplication map for a projective fiber](algebraic-geometry.md#graded-multiplication-map-for-a-projective-fiber) fails to be surjective, by the [Projective Nullstellensatz](algebraic-geometry.md#projective-nullstellensatz). The image is thus an intersection of closed rank-defect loci. An affine open cover proves the general case. This is the universally closed part of the [proper morphism](#proper-morphism) property of projective space.

###### Rational-point projection need not be Zariski closed

↑ **Parent:** [Closedness of projection from projective space](#closedness-of-projection-from-projective-space)

Over the real numbers, the closed equation $y_0^2=t y_1^2$ in $\mathbb A^1\times\mathbb P^1$ projects on real points to $\{t\ge0\}$, which is not [Zariski closed](algebraic-geometry.md#zariski-closed-set). Projective properness concerns scheme or geometric images, not the image of rational points over an arbitrary field. Similarly, $y_0^2+y_1^2$ has no real projective zero, but its [homogeneous ideal](commutative-algebra.md#homogeneous-ideal) contains no power of the [irrelevant ideal of projective space](algebraic-geometry.md#irrelevant-ideal-of-projective-space), since it has a complex projective zero.

###### Projective scheme

↑ **Parent:** [Proper morphism](#proper-morphism)

A projective scheme over a base $S$ is an $S$-scheme admitting a closed immersion into some projective space $\mathbb P_S^n$. Every projective morphism is [proper](#proper-morphism).

Projectivity is a property of the scheme over its specified base, expressed by its structural [projective morphism](#projective-morphism).

###### Proj construction

↑ **Parent:** [Projective scheme](#projective-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proj_construction)

For a graded ring $S$, $\operatorname{Proj}S$ consists of homogeneous prime ideals not containing the irrelevant ideal $S_+$. Its standard affine opens satisfy $D_+(f)\cong\operatorname{Spec}(S_f)_0$.

###### Degree-one generation condition for Proj

↑ **Parent:** [Proj construction](#proj-construction)

If a nonnegatively graded ring $S$ is generated by $S_1$ as an $S_0$-algebra, the [standard affine opens of Proj](#standard-affine-open-of-proj) $D_+(f)$ with $f\in S_1$ cover $\operatorname{Proj}S$. Indeed a homogeneous prime containing every degree-one element would contain the [irrelevant ideal of a graded ring](#irrelevant-ideal-of-a-graded-ring). This condition makes all [twisting sheaves on Proj](#twisting-sheaf-on-proj) invertible and makes graded sheafification compatible with [tensor products of sheaves](#tensor-product-of-sheaves).

###### Sheaf associated with a graded module

↑ **Parent:** [Proj construction](#proj-construction)

A [graded module](commutative-algebra.md#graded-module) $M$ over a graded ring $S$ determines a [quasi-coherent sheaf](#quasi-coherent-sheaf) on the [Proj construction](#proj-construction) $\operatorname{Proj}S$ by taking the degree-zero part of its localization on each [standard affine open of Proj](#standard-affine-open-of-proj). Localization identifies these module sheaves on overlaps. The construction is exact, by [exactness of localization](commutative-algebra.md#exactness-of-localization) and exactness of taking a fixed graded component.

###### Tensor compatibility of graded sheafification on degree-one-generated Proj

↑ **Parent:** [Sheaf associated with a graded module](#sheaf-associated-with-a-graded-module)

Under the [degree-one generation condition for Proj](#degree-one-generation-condition-for-proj), cover $X=\operatorname{Proj}S$ by degree-one charts. The [degree-one localization of a graded module](commutative-algebra.md#degree-one-localization-of-a-graded-module) identifies the two local modules in the displayed formula, using [localization commutes with tensor products](commutative-algebra.md#localization-commutes-with-tensor-products). The maps are natural and agree on overlaps, so they glue to an isomorphism of [sheaves of modules](#sheaf-of-modules). The analogous assertion can fail for general positively graded rings.

###### Twisting sheaf on Proj

↑ **Parent:** [Sheaf associated with a graded module](#sheaf-associated-with-a-graded-module)

With the [graded shift](commutative-algebra.md#graded-shift) convention $S(n)_d=S_{n+d}$, this is the [sheaf associated with a graded module](#sheaf-associated-with-a-graded-module) $S(n)$. Under the [degree-one generation condition for Proj](#degree-one-generation-condition-for-proj), it is an [invertible sheaf](#line-bundle): on $D_+(f)$ with $\deg f=1$, multiplication by $f^n$ freely generates its local module for every integer $n$. Without that hypothesis, it need not be invertible. The [twisting sheaf on projective space](#twisting-sheaf-on-projective-space) is the standard special case. [Stacks Project, Section 27.10](https://stacks.math.columbia.edu/tag/01MM) records the hypotheses and local trivializations.

###### Irrelevant ideal of a graded ring

↑ **Parent:** [Proj construction](#proj-construction)

For a nonnegatively graded ring $S=\bigoplus_{d\geq0}S_d$, the irrelevant ideal is

$$
S_+=\bigoplus_{d>0}S_d.
$$

The points of $\operatorname{Proj}S$ are precisely the homogeneous [prime ideals](commutative-algebra.md#prime-ideal) that do not contain $S_+$.

###### Standard affine open of Proj

↑ **Parent:** [Proj construction](#proj-construction)

For a positive-degree homogeneous element $f\in S$, the standard open

$$
D_+(f)=\{\mathfrak p\in\operatorname{Proj}S:f\notin\mathfrak p\}
$$

is the [affine scheme](#affine-scheme) $\operatorname{Spec}(S_f)_0$.

###### Morphism on Proj induced by a graded ring homomorphism

↑ **Parent:** [Standard affine open of Proj](#standard-affine-open-of-proj)

A graded homomorphism $S\to T$ induces a morphism to $\operatorname{Proj}S$ on the open subset of $\operatorname{Proj}T$ where the inverse image of a prime does not contain $S_+$. On $D_+(\varphi(f))$ it is induced by $(S_f)_0\to(T_{\varphi(f)})_0$.

###### Invariance of Proj under an eventual graded isomorphism

↑ **Parent:** [Morphism on Proj induced by a graded ring homomorphism](#morphism-on-proj-induced-by-a-graded-ring-homomorphism)

If a graded homomorphism $S\to T$ is an isomorphism in every sufficiently large degree, then it induces an isomorphism

$$
\operatorname{Proj}T\xrightarrow{\sim}\operatorname{Proj}S.
$$

Multiplying degree-zero localized fractions by a sufficiently large power of the chart denominator reduces the claim to the assumed high-degree isomorphisms.

###### Relative Proj construction

↑ **Parent:** [Proj construction](#proj-construction)

For a quasi-coherent graded $\mathcal O_X$-algebra $\mathcal A$, the relative Proj is obtained by gluing the schemes $\operatorname{Proj}\mathcal A(U)$ over affine open subsets $U\subseteq X$. If $\mathcal A$ is of finite type and generated in degree one, a surjection $\operatorname{Sym}(\mathcal E)\twoheadrightarrow\mathcal A$ realizes $\operatorname{Proj}_X\mathcal A$ as a closed subscheme of the projective bundle $\mathbb P_X(\mathcal E)$.

###### Veronese subring

↑ **Parent:** [Proj construction](#proj-construction)

For a nonnegatively [graded ring](commutative-algebra.md#graded-ring) $S=\bigoplus_{m\geq0}S_m$ and $d\geq1$, its $d$th Veronese subring is

$$
S^{(d)}=\bigoplus_{m\geq0}S_{dm},
$$

graded by $(S^{(d)})_m=S_{dm}$. Passing from $S$ to $S^{(d)}$ does not change its projective scheme: the standard affine charts give a canonical isomorphism $\operatorname{Proj}S\cong\operatorname{Proj}S^{(d)}$.

###### Veronese embedding

↑ **Parent:** [Veronese subring](#veronese-subring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Veronese_embedding)

The degree-$d$ Veronese embedding sends a [projective point](projective-space.md#projective-point) to all monomials of degree $d$ in its homogeneous coordinates. For example,

$$
\nu_2:\mathbb P^1\longrightarrow\mathbb P^2,
\qquad [x:y]\longmapsto[x^2:xy:y^2],
$$

is a closed immersion with image the conic $uw-v^2=0$.

##### Closed immersion

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_immersion)

A morphism $i:Z\to X$ is a closed immersion when it identifies $Z$ homeomorphically with a closed subset of $X$ and the morphism $\mathcal O_X\to i_*\mathcal O_Z$ is surjective. Affine-locally it has the form $\operatorname{Spec}(A/I)\to\operatorname{Spec}A$.

###### Flat closed immersion of finite presentation

↑ **Parent:** [Closed immersion](#closed-immersion)

A nonempty flat [closed immersion](#closed-immersion) of finite presentation into a connected [scheme](#scheme) is an [isomorphism](algebra.md#isomorphism). On a chart it is $A\to A/I$ with $I$ finitely generated. At a prime containing $I$, the quotient is a finite flat module over the [local ring](commutative-algebra.md#local-ring), hence free of rank one, so $I$ vanishes there. Finite generation extends this vanishing to a neighbourhood. Thus the image is open as well as closed; connectedness makes it all of the target, and the ideal is everywhere zero. Without finite presentation the conclusion can fail.

###### Closed immersion criterion for affine schemes

↑ **Parent:** [Closed immersion](#closed-immersion)

A surjective [ring homomorphism](commutative-algebra.md#ring-homomorphism) $A\to B=A/I$ identifies the [spectrum of a ring](#spectrum-of-a-commutative-ring) $B$ with the closed subset $V(I)$ and induces a surjective map of structure sheaves. Conversely, the [direct image sheaf](#direct-image-sheaf) of $\mathcal O_{\operatorname{Spec}B}$ under an affine morphism is the sheaf associated with the $A$-module $B$: its sections on $D(a)$ are $B_{\phi(a)}$. The cokernel of the structure-sheaf map is therefore associated with the module cokernel of $A\to B$. If the sheaf map is surjective, all localizations of that cokernel vanish and the module cokernel is zero. This proves the converse without assuming global sections preserve arbitrary sheaf surjections.

###### Nilpotent thickening

↑ **Parent:** [Closed immersion](#closed-immersion)

A nilpotent thickening is a [closed immersion](#closed-immersion) defined by a nilpotent [ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme). Its underlying topological map is a [homeomorphism](topology.md#homeomorphism), because every [prime ideal](commutative-algebra.md#prime-ideal) contains every [nilpotent element](commutative-algebra.md#nilpotent). For example, quotienting the [dual numbers](commutative-algebra.md#dual-number) by $(\varepsilon)$ changes the [structure sheaf](#structure-sheaf-of-a-scheme) without changing the single point of the spectrum.

###### Closed subscheme

↑ **Parent:** [Closed immersion](#closed-immersion)

A closed subscheme of $X$ is a [scheme](#scheme) $Z$ together with a [closed immersion](#closed-immersion) $Z\hookrightarrow X$, usually identified with its image and its quotient structure sheaf.

###### Infinitesimal neighbourhood of a closed subscheme

↑ **Parent:** [Closed subscheme](#closed-subscheme)

For a [closed subscheme](#closed-subscheme) defined by an [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$, its $n$th [infinitesimal neighbourhood](#infinitesimal-neighbourhood-of-a-closed-subscheme) has structure sheaf $\mathcal O_X/\mathcal I^{n+1}$. All these neighbourhoods have the same underlying topological space because the radicals of $\mathcal I$ and its positive powers agree. Their [inverse limit](module-theory.md#inverse-limit) of structure sheaves is the [formal completion of a scheme](#formal-completion-of-a-scheme).

// Target: ringed-space.bigb

###### Projective complete intersection

↑ **Parent:** [Closed subscheme](#closed-subscheme)

A projective complete intersection is a [closed subscheme](#closed-subscheme) of a [projective space](projective-space.md) defined by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of positive degrees. A length-$r$ sequence in $k[t_0,\ldots,t_N]$ gives dimension $N-r$ when $r\le N$. Sheafifying its successive quotient sequences gives exact restriction sequences of [twisting sheaves on projective space](#twisting-sheaf-on-projective-space), allowing computation of its [sheaf cohomology](#sheaf-cohomology). It need not be smooth or reduced.

###### Unmixedness of a complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

A [projective complete intersection](#projective-complete-intersection) defined by a [regular sequence](commutative-algebra.md#regular-sequence) in a [polynomial ring](commutative-algebra.md#polynomial-ring) has pure codimension equal to the sequence length and has no embedded [associated primes](module-theory.md#associated-prime-of-a-module). Thus its components account for the whole degree, with their generic multiplicities. This fact excludes hidden embedded points when a contained curve already has the full intersection degree.

###### Global regular functions on a positive-dimensional projective complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

For a length-$r$ homogeneous regular sequence of positive degrees in $\mathbb P^N_k$, with $r<N$, the [global regular functions](#global-regular-function) on its [projective complete intersection](#projective-complete-intersection) are exactly $k$. In the successive restriction sequences, [intermediate cohomology vanishing for a projective complete intersection](#intermediate-cohomology-vanishing-for-a-projective-complete-intersection) makes the first-cohomology group on the preceding stage zero. Inductively all negative twists have zero global sections, so at twist zero the restriction of constants is an isomorphism. The positive-dimension assumption is essential: a zero-dimensional complete intersection can have more global functions, including nilpotents.

###### Intermediate cohomology vanishing for a projective complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

For a length-$r$ [projective complete intersection](#projective-complete-intersection) $X_r\subseteq\mathbb P^N_k$, the groups $H^q(X_r,\mathcal O_{X_r}(m))$ vanish for every integer $m$ and $0<q<N-r$. Starting with [cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space), induct through $0\to\mathcal O_{X_{j-1}}(m-d_j)\to\mathcal O_{X_{j-1}}(m)\to\mathcal O_{X_j}(m)\to0$. Both adjacent groups in the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) vanish precisely in the indicated range.

###### Construction of a closed subscheme from a quasi-coherent ideal

↑ **Parent:** [Closed subscheme](#closed-subscheme)

A [quasi-coherent sheaf](#quasi-coherent-sheaf) of ideals $\mathcal I\subseteq\mathcal O_X$ gives a [closed subscheme](#closed-subscheme) by gluing $\operatorname{Spec}(A/J)$ on [affine open subschemes](#affine-open-subscheme) where $\mathcal I=\widetilde J$. Compatibility follows from [exactness of localization](commutative-algebra.md#exactness-of-localization). On the closed set $Z=\{x:\mathcal I_x\ne\mathcal O_{X,x}\}$, the [structure sheaf](#structure-sheaf-of-a-scheme) is $i^{-1}(\mathcal O_X/\mathcal I)$, where $i:Z\hookrightarrow X$ is the inclusion. Its pushforward is $\mathcal O_X/\mathcal I$.

###### Ideal sheaf of a closed subscheme

↑ **Parent:** [Closed subscheme](#closed-subscheme)

For a [closed immersion](#closed-immersion) $i:Z\hookrightarrow X$, the ideal sheaf is the kernel $\mathcal I_{Z/X}=\ker(\mathcal O_X\to i_*\mathcal O_Z)$. It therefore fits into the [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\longrightarrow\mathcal I_{Z/X}\longrightarrow\mathcal O_X\longrightarrow i_*\mathcal O_Z\longrightarrow0.
$$

###### Ideal sheaf of a closed point

↑ **Parent:** [Ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme)

For a [closed point](topology.md#closed-point) $P$ with residue field $k(P)$, evaluation gives a morphism from the [structure sheaf](#structure-sheaf-of-a-scheme) onto the [skyscraper sheaf](#skyscraper-sheaf) $k_P$. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) is the ideal sheaf of $P$. On a [Noetherian scheme](#noetherian-scheme) it is a [coherent ideal sheaf](#coherent-ideal-sheaf).

###### Ideal sheaf of two closed points

↑ **Parent:** [Ideal sheaf of a closed point](#ideal-sheaf-of-a-closed-point)

For distinct [closed points](topology.md#closed-point) over an [algebraically closed field](algebra.md#algebraically-closed-field), evaluation gives the [short exact sequence](module-theory.md#short-exact-sequence) $0\to\mathcal I_{\{P,Q\}}\to\mathcal O_X\to k_P\oplus k_Q\to0$. If all global [regular functions](#regular-function) are constant, the [long exact sequence in sheaf cohomology](#long-exact-sequence-in-sheaf-cohomology) embeds $k^2/k(1,1)$ into $H^1(X,\mathcal I_{\{P,Q\}})$. Thus this ideal detects a concrete obstruction to affineness.

###### Rank bound for locally free ideals on reduced schemes

↑ **Parent:** [Ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme)

A finite [locally free sheaf](#locally-free-sheaf) of ideals on a [reduced scheme](#reduced-scheme) has rank at most one at every point. On a nonempty [affine open subscheme](#affine-open-subscheme) where its rank is $r$, localize its inclusion into the structure sheaf at a [minimal prime ideal](commutative-algebra.md#minimal-prime-ideal). The resulting [local ring](commutative-algebra.md#local-ring) is a field $K$, giving an injection $K^r\hookrightarrow K$, hence $r\le1$. This works without a Noetherian assumption. The empty scheme is a vacuous exception to claims phrased as nonexistence of a sheaf of a prescribed rank.

###### Structure-sheaf sequence of a hypersurface

↑ **Parent:** [Closed subscheme](#closed-subscheme)

If a homogeneous polynomial $f_d$ of degree $d$ cuts out a projective hypersurface $i:X\hookrightarrow\mathbb P^n$, multiplication by $f_d$ gives the short exact sequence

$$
0\longrightarrow\mathcal O_{\mathbb P^n}(-d)\xrightarrow{\cdot f_d}\mathcal O_{\mathbb P^n}\longrightarrow i_*\mathcal O_X\longrightarrow0.
$$

###### Reduced induced subscheme

↑ **Parent:** [Closed subscheme](#closed-subscheme)

Every closed subset $Z\subseteq X$ has a canonical reduced closed-subscheme structure defined affine-locally by $\operatorname{Spec}(A/\sqrt I)$ when $Z=V(I)\subseteq\operatorname{Spec}A$. It is the smallest closed subscheme with underlying set $Z$.

###### Scheme-theoretic image

↑ **Parent:** [Closed subscheme](#closed-subscheme)

The scheme-theoretic image of $f:X\to Y$ is the smallest [closed subscheme](#closed-subscheme) of $Y$ through which $f$ factors. For an affine morphism $\operatorname{Spec}B\to\operatorname{Spec}A$ induced by $\varphi:A\to B$, it is $\operatorname{Spec}(A/\ker\varphi)$, whose underlying set is the closure of the set-theoretic image.

The construction retains the scheme structure on the [closed subscheme](#closed-subscheme), not merely the set of points in an image.

#### Affine plane with doubled origin

↑ **Parent:** [Scheme](#scheme)

The affine plane with doubled origin is formed by gluing two copies of $\mathbb A_k^2$ by the identity away from the origin. The overlap is the [punctured affine plane](#punctured-affine-plane), so this scheme is nonseparated and the two-open affine cover is not acyclic for the structure sheaf.

The gluing resembles a [non-Hausdorff manifold](topology.md#non-hausdorff-manifold) example, but this node concerns an algebraic scheme and its nonseparatedness, not a real manifold.

#### Semi-separated scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is semi-separated when the intersection of any two affine open subsets is affine, equivalently when its diagonal is affine. This condition makes affine covers acyclic for quasi-coherent sheaves.

##### Exact direct image from an affine open in a semi-separated scheme

↑ **Parent:** [Semi-separated scheme](#semi-separated-scheme)

If $U$ is an [affine open subscheme](#affine-open-subscheme) of a [semi-separated scheme](#semi-separated-scheme), its [open immersion](#open-immersion) $j:U\hookrightarrow X$ has exact [direct image](#direct-image-sheaf) on [quasi-coherent sheaves](#quasi-coherent-sheaf). Test on an affine open $V$ of $X$: the intersection $U\cap V$ is affine, and the [affine module-sheaf equivalence](#affine-module-sheaf-equivalence) makes sections on this intersection exact. The direct image is also quasi-coherent, since this open immersion is an [affine morphism](#affine-morphism).

## Direct image functor

↑ **Parent:** [Ringed space](ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_image_functor)

For a continuous map $f:X\to Y$, the direct-image functor sends a sheaf $\mathcal F$ on $X$ to the sheaf $V\mapsto\mathcal F(f^{-1}V)$ on $Y$, and sends sheaf morphisms to their induced maps on sections. Its output is a [direct image sheaf](#direct-image-sheaf).

## Inverse image functor

↑ **Parent:** [Ringed space](ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_image_functor)

For a continuous map $f:X\to Y$, the inverse-image functor takes a sheaf on $Y$ to the sheafification of its local inverse-image presheaf on $X$. It is left adjoint to the [direct image functor](#direct-image-functor). For sheaves of modules on ringed spaces, extension of scalars gives the separate [pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules).

## Valuative criterion

↑ **Parent:** [Ringed space](ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Valuative_criterion)

Valuative criteria test properties of scheme morphisms by extending a lift from the generic point of the spectrum of a valuation ring to the whole spectrum. Under the usual finiteness hypotheses, uniqueness characterizes separatedness, existence characterizes universal closedness, and existence with uniqueness characterizes properness. The [valuative criterion for separatedness](#valuative-criterion-for-separatedness) and [valuative criterion for properness](#valuative-criterion-for-properness) are the respective specific statements.

## ↑ Ancestors (5)

1. [Algebraic geometry](algebraic-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (11)

- [Injective module sheaves are flasque](#injective-module-sheaves-are-flasque)
- [Injective sheaf of modules](#injective-sheaf-of-modules)
- [Internal Hom sheaf](#internal-hom-sheaf)
- [Inverse-image direct-image adjunction](#inverse-image-direct-image-adjunction)
- [Locally ringed space](#locally-ringed-space)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-13.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-113.md#4/i/solution)
- [Projection formula](#projection-formula)
- [Pullback of a sheaf of modules](#pullback-of-a-sheaf-of-modules)
- [Sheaf of modules](#sheaf-of-modules)
- [Sheaf of rings](#sheaf-of-rings)
