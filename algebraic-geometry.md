# Algebraic geometry

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_geometry)

**Table of contents**

- [GAGA theorem](#gaga-theorem)
- [Very general point of an algebraic parameter space](#very-general-point-of-an-algebraic-parameter-space)
- [Hilbert scheme](#hilbert-scheme)
  - [Hilbert functor](#hilbert-functor)
    - [First-order embedded deformation](#first-order-embedded-deformation)
      - [Zariski tangent space of a Hilbert scheme](#zariski-tangent-space-of-a-hilbert-scheme)
  - [Fano scheme](#fano-scheme)
    - [Fano scheme of lines](#fano-scheme-of-lines)
      - [Incidence proof that a cubic surface contains a line](#incidence-proof-that-a-cubic-surface-contains-a-line)
        - [Cubic surface line incidence variety](#cubic-surface-line-incidence-variety)
      - [Finiteness of lines on a smooth surface of degree at least three](#finiteness-of-lines-on-a-smooth-surface-of-degree-at-least-three)
- [Étale cohomology](#etale-cohomology)
- [Algebraic set](#algebraic-set)
- [Complex multiplication](#complex-multiplication)
  - [CM period](#cm-period)
  - [CM reciprocity theorem](#cm-reciprocity-theorem)
  - [CM elliptic curve](#cm-elliptic-curve)
- [Birational geometry](#birational-geometry)
  - [Blowing up (algebraic geometry)](#blowing-up-algebraic-geometry)
    - [Strict transform of an algebraic subvariety](#strict-transform-of-an-algebraic-subvariety)
    - [Algebraic exceptional divisor](#algebraic-exceptional-divisor)
- [Zariski topology](#zariski-topology)
  - [Zariski dense subset](#zariski-dense-subset)
- [Presheaf of sets on a topological space](#presheaf-of-sets-on-a-topological-space)
  - [Constant presheaf of sets](#constant-presheaf-of-sets)
  - [Morphism of presheaves](#morphism-of-presheaves)
  - [Sheaf (mathematics)](#sheaf-mathematics)
    - [Skyscraper sheaf of sets](#skyscraper-sheaf-of-sets)
    - [Étale space of a presheaf](#etale-space-of-a-presheaf)
    - [Constant sheaf of sets](#constant-sheaf-of-sets)
    - [Morphism of sheaves](#morphism-of-sheaves)
      - [Cokernel sheaf](#cokernel-sheaf)
      - [f-morphism of sheaves](#f-morphism-of-sheaves)
      - [Surjective morphism of sheaves](#surjective-morphism-of-sheaves)
      - [Kernel sheaf](#kernel-sheaf)
    - [Sheaf of abelian groups](#sheaf-of-abelian-groups)
      - [Direct sum of sheaves](#direct-sum-of-sheaves)
      - [Injective sheaf](#injective-sheaf)
      - [Exact sequence of sheaves](#exact-sequence-of-sheaves)
        - [Short exact sequence of sheaves](#short-exact-sequence-of-sheaves)
      - [Constant sheaf](#constant-sheaf)
        - [Constant sheaves on irreducible spaces are flasque](#constant-sheaves-on-irreducible-spaces-are-flasque)
    - [Sheaf gluing axiom](#sheaf-gluing-axiom)
- [Ringed space](ringed-space.md)
  - [Morphism of ringed spaces](ringed-space.md#morphism-of-ringed-spaces)
  - [Sheaf of rings](ringed-space.md#sheaf-of-rings)
    - [Sheaf of topological rings](ringed-space.md#sheaf-of-topological-rings)
  - [Sheaf of modules](ringed-space.md#sheaf-of-modules)
    - [Internal Hom sheaf](ringed-space.md#internal-hom-sheaf)
    - [Local system](ringed-space.md#local-system)
    - [Rational section of a sheaf of modules](ringed-space.md#rational-section-of-a-sheaf-of-modules)
      - [Rational principal part](ringed-space.md#rational-principal-part)
        - [Rational principal-parts resolution on an algebraic curve](ringed-space.md#rational-principal-parts-resolution-on-an-algebraic-curve)
          - [Affine principal-parts interpolation for a locally free sheaf](ringed-space.md#affine-principal-parts-interpolation-for-a-locally-free-sheaf)
      - [Stalk inclusion into rational sections of a locally free sheaf](ringed-space.md#stalk-inclusion-into-rational-sections-of-a-locally-free-sheaf)
    - [Coherent analytic sheaf](ringed-space.md#coherent-analytic-sheaf)
    - [Dual of a sheaf](ringed-space.md#dual-of-a-sheaf)
    - [Injective sheaf of modules](ringed-space.md#injective-sheaf-of-modules)
      - [Injective module sheaves are flasque](ringed-space.md#injective-module-sheaves-are-flasque)
    - [Stalk of a sheaf](ringed-space.md#stalk-of-a-sheaf)
      - [Costalk](ringed-space.md#costalk)
      - [Stalk functor for presheaves of sets](ringed-space.md#stalk-functor-for-presheaves-of-sets)
        - [Joint stalk functor on sheaves of sets](ringed-space.md#joint-stalk-functor-on-sheaves-of-sets)
      - [Skyscraper sheaf](ringed-space.md#skyscraper-sheaf)
        - [Skyscraper sheaf cohomology](ringed-space.md#skyscraper-sheaf-cohomology)
      - [Germ of a sheaf section](ringed-space.md#germ-of-a-sheaf-section)
        - [Support of a sheaf section](ringed-space.md#support-of-a-sheaf-section)
    - [Sheafification](ringed-space.md#sheafification)
      - [Universal property of sheafification](ringed-space.md#universal-property-of-sheafification)
      - [Sheafification by locally representable germs](ringed-space.md#sheafification-by-locally-representable-germs)
    - [Extension by zero](ringed-space.md#extension-by-zero)
    - [Quasi-coherent sheaf](ringed-space.md#quasi-coherent-sheaf)
      - [Kernels of quasi-coherent sheaf morphisms](ringed-space.md#kernels-of-quasi-coherent-sheaf-morphisms)
      - [Affine module sheaf](ringed-space.md#affine-module-sheaf)
        - [Coherence of an affine module sheaf](ringed-space.md#coherence-of-an-affine-module-sheaf)
      - [Quasi-coherent sheaves are closed under extensions](ringed-space.md#quasi-coherent-sheaves-are-closed-under-extensions)
      - [Global-section localization for quasi-coherent sheaves](ringed-space.md#global-section-localization-for-quasi-coherent-sheaves)
      - [Affine module-sheaf equivalence](ringed-space.md#affine-module-sheaf-equivalence)
      - [Torsion-free sheaf](ringed-space.md#torsion-free-sheaf)
      - [Vanishing of quasi-coherent cohomology on an affine scheme](ringed-space.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme)
      - [Coherent sheaf](ringed-space.md#coherent-sheaf)
        - [Globally generated sheaf](ringed-space.md#globally-generated-sheaf)
        - [Stalkwise isomorphic coherent sheaves need not be isomorphic](ringed-space.md#stalkwise-isomorphic-coherent-sheaves-need-not-be-isomorphic)
        - [Coherent ideal sheaf](ringed-space.md#coherent-ideal-sheaf)
        - [Finite twisting resolution of a coherent sheaf on projective space](ringed-space.md#finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space)
        - [Support dimension of a coherent sheaf](ringed-space.md#support-dimension-of-a-coherent-sheaf)
        - [Associated point of a coherent sheaf](ringed-space.md#associated-point-of-a-coherent-sheaf)
        - [Direct image of a coherent sheaf under a closed immersion](ringed-space.md#direct-image-of-a-coherent-sheaf-under-a-closed-immersion)
    - [Tensor product of sheaves](ringed-space.md#tensor-product-of-sheaves)
    - [Direct image sheaf](ringed-space.md#direct-image-sheaf)
      - [Derived direct image of sheaves](ringed-space.md#derived-direct-image-of-sheaves)
        - [Proper base change for sheaves](ringed-space.md#proper-base-change-for-sheaves)
      - [Projective direct image need not preserve surjections](ringed-space.md#projective-direct-image-need-not-preserve-surjections)
      - [Coherence reflected by finite direct image](ringed-space.md#coherence-reflected-by-finite-direct-image)
      - [Direct image from an open restriction](ringed-space.md#direct-image-from-an-open-restriction)
      - [Direct-image tensor comparison](ringed-space.md#direct-image-tensor-comparison)
      - [Sheaf cohomology under a closed inclusion](ringed-space.md#sheaf-cohomology-under-a-closed-inclusion)
      - [Direct image of a quasi-coherent sheaf under an affine morphism](ringed-space.md#direct-image-of-a-quasi-coherent-sheaf-under-an-affine-morphism)
        - [Acyclic direct image from an affine chart of the projective line](ringed-space.md#acyclic-direct-image-from-an-affine-chart-of-the-projective-line)
      - [Quasi-coherence of direct image under a quasi-compact quasi-separated morphism](ringed-space.md#quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism)
    - [Inverse image sheaf](ringed-space.md#inverse-image-sheaf)
      - [Inverse-image direct-image adjunction](ringed-space.md#inverse-image-direct-image-adjunction)
      - [Universal property of an inverse image sheaf](ringed-space.md#universal-property-of-an-inverse-image-sheaf)
      - [Pullback of a sheaf of modules](ringed-space.md#pullback-of-a-sheaf-of-modules)
        - [Restriction of a module sheaf to a closed subvariety](ringed-space.md#restriction-of-a-module-sheaf-to-a-closed-subvariety)
        - [Pullback-direct-image adjunction unit](ringed-space.md#pullback-direct-image-adjunction-unit)
        - [Projection formula](ringed-space.md#projection-formula)
    - [Locally free sheaf](ringed-space.md#locally-free-sheaf)
      - [Free sheaf](ringed-space.md#free-sheaf)
      - [Saturated line subbundle on a smooth curve](ringed-space.md#saturated-line-subbundle-on-a-smooth-curve)
        - [Unbounded negative degrees of line subbundles](ringed-space.md#unbounded-negative-degrees-of-line-subbundles)
        - [Upper degree bound for line subbundles on a smooth curve](ringed-space.md#upper-degree-bound-for-line-subbundles-on-a-smooth-curve)
      - [Local splitting when a quotient sheaf is locally free](ringed-space.md#local-splitting-when-a-quotient-sheaf-is-locally-free)
      - [Line bundle](ringed-space.md#line-bundle)
        - [Degree of a line bundle](ringed-space.md#degree-of-a-line-bundle)
        - [Half-density](ringed-space.md#half-density)
        - [Orientation line bundle](ringed-space.md#orientation-line-bundle)
          - [Orientable total space of the orientation line bundle](ringed-space.md#orientable-total-space-of-the-orientation-line-bundle)
        - [Homogeneous line-bundle representations on the two-sphere](ringed-space.md#homogeneous-line-bundle-representations-on-the-two-sphere)
        - [Line bundles trivialized by an open cover](ringed-space.md#line-bundles-trivialized-by-an-open-cover)
        - [Globally generated line bundle](ringed-space.md#globally-generated-line-bundle)
          - [Globally generated line bundle without finite generators](ringed-space.md#globally-generated-line-bundle-without-finite-generators)
          - [Finite global generation on a quasi-compact scheme](ringed-space.md#finite-global-generation-on-a-quasi-compact-scheme)
          - [Tensor product of globally generated line bundles](ringed-space.md#tensor-product-of-globally-generated-line-bundles)
        - [Rational section of a line bundle](ringed-space.md#rational-section-of-a-line-bundle)
        - [Twisting sheaf on projective space](ringed-space.md#twisting-sheaf-on-projective-space)
          - [Homogeneous rational sections of a twisting sheaf](ringed-space.md#homogeneous-rational-sections-of-a-twisting-sheaf)
          - [Laurent-monomial description of top cohomology on projective space](ringed-space.md#laurent-monomial-description-of-top-cohomology-on-projective-space)
          - [Canonical bundle of projective space](ringed-space.md#canonical-bundle-of-projective-space)
            - [Canonical-form transition on projective space](ringed-space.md#canonical-form-transition-on-projective-space)
          - [Hyperplane exact sequence for twisting sheaves](ringed-space.md#hyperplane-exact-sequence-for-twisting-sheaves)
            - [Top-twist vanishing by hyperplane induction](ringed-space.md#top-twist-vanishing-by-hyperplane-induction)
        - [Picard group](ringed-space.md#picard-group)
          - [Picard group of the projective line](ringed-space.md#picard-group-of-the-projective-line)
          - [Degree-zero Picard group of a curve](ringed-space.md#degree-zero-picard-group-of-a-curve)
            - [Rational points need not generate the degree-zero Picard group](ringed-space.md#rational-points-need-not-generate-the-degree-zero-picard-group)
            - [Abel map of a pointed smooth projective curve](ringed-space.md#abel-map-of-a-pointed-smooth-projective-curve)
          - [Picard functor of a curve](ringed-space.md#picard-functor-of-a-curve)
            - [Picard scheme of a curve](ringed-space.md#picard-scheme-of-a-curve)
              - [Picard charts from nonspecial divisors](ringed-space.md#picard-charts-from-nonspecial-divisors)
          - [Picard group of a ring](ringed-space.md#picard-group-of-a-ring)
          - [Holomorphic Picard group](ringed-space.md#holomorphic-picard-group)
            - [Picard injection for holomorphic projective bundles](ringed-space.md#picard-injection-for-holomorphic-projective-bundles)
          - [Picard-group localization on a smooth variety](ringed-space.md#picard-group-localization-on-a-smooth-variety)
          - [Cartier-divisor description of the Picard group](ringed-space.md#cartier-divisor-description-of-the-picard-group)
          - [Néron-Severi group](ringed-space.md#neron-severi-group)
        - [Very ample line bundle](ringed-space.md#very-ample-line-bundle)
        - [Ample line bundle](ringed-space.md#ample-line-bundle)
          - [Ampleness on reduced components](ringed-space.md#ampleness-on-reduced-components)
          - [Finite pullback of an ample line bundle](ringed-space.md#finite-pullback-of-an-ample-line-bundle)
          - [High ample twist is very ample](ringed-space.md#high-ample-twist-is-very-ample)
        - [Kodaira map](ringed-space.md#kodaira-map)
    - [Global section functor](ringed-space.md#global-section-functor)
      - [Localization of global sections on a principal open](ringed-space.md#localization-of-global-sections-on-a-principal-open)
      - [Global section](ringed-space.md#global-section)
      - [Section functor with support](ringed-space.md#section-functor-with-support)
        - [Local cohomology](ringed-space.md#local-cohomology)
          - [Long exact sequence for local cohomology](ringed-space.md#long-exact-sequence-for-local-cohomology)
          - [Local cohomology of the affine plane supported at the origin](ringed-space.md#local-cohomology-of-the-affine-plane-supported-at-the-origin)
    - [Sheaf cohomology](ringed-space.md#sheaf-cohomology)
      - [Coherent cohomology](ringed-space.md#coherent-cohomology)
        - [Finiteness of coherent cohomology on projective varieties](ringed-space.md#finiteness-of-coherent-cohomology-on-projective-varieties)
      - [Cohomology sheaf](ringed-space.md#cohomology-sheaf)
        - [Cohomology-sheaf exact sequence](ringed-space.md#cohomology-sheaf-exact-sequence)
      - [Grauert base change theorem](ringed-space.md#grauert-base-change-theorem)
      - [Hypercohomology](ringed-space.md#hypercohomology)
      - [Acyclic resolution theorem](ringed-space.md#acyclic-resolution-theorem)
      - [Locally vanishing principle for sheaf cohomology](ringed-space.md#locally-vanishing-principle-for-sheaf-cohomology)
      - [Holomorphic first cohomology of punctured complex two-space](ringed-space.md#holomorphic-first-cohomology-of-punctured-complex-two-space)
      - [Castelnuovo–Mumford regularity](ringed-space.md#castelnuovo-mumford-regularity)
      - [Injective resolution of sheaves](ringed-space.md#injective-resolution-of-sheaves)
      - [Euler characteristic of a coherent sheaf](ringed-space.md#euler-characteristic-of-a-coherent-sheaf)
        - [Asymptotic Riemann–Roch](ringed-space.md#asymptotic-riemann-roch)
      - [Serre vanishing](ringed-space.md#serre-vanishing)
        - [Uniform high-degree vanishing on a smooth projective curve](ringed-space.md#uniform-high-degree-vanishing-on-a-smooth-projective-curve)
        - [Uniform Serre vanishing for two ample twists](ringed-space.md#uniform-serre-vanishing-for-two-ample-twists)
          - [Higher cohomology vanishing from an ample hyperplane restriction](ringed-space.md#higher-cohomology-vanishing-from-an-ample-hyperplane-restriction)
        - [Fujita vanishing](ringed-space.md#fujita-vanishing)
          - [Cohomology growth for nef twists](ringed-space.md#cohomology-growth-for-nef-twists)
            - [Top cohomology boundedness for nef twists](ringed-space.md#top-cohomology-boundedness-for-nef-twists)
      - [Grothendieck vanishing](ringed-space.md#grothendieck-vanishing)
      - [Resolution principle for sheaf cohomology](ringed-space.md#resolution-principle-for-sheaf-cohomology)
      - [Leray spectral sequence](ringed-space.md#leray-spectral-sequence)
      - [Flasque sheaf](ringed-space.md#flasque-sheaf)
        - [Sheafification of an injective module is flasque](ringed-space.md#sheafification-of-an-injective-module-is-flasque)
        - [Flasque-kernel section-lifting lemma](ringed-space.md#flasque-kernel-section-lifting-lemma)
        - [Flasque resolution](ringed-space.md#flasque-resolution)
          - [Godement resolution](ringed-space.md#godement-resolution)
      - [Čech cohomology](ringed-space.md#cech-cohomology)
        - [Cohomology of twists on projective space](ringed-space.md#cohomology-of-twists-on-projective-space)
        - [Čech cohomology of the punctured affine plane](ringed-space.md#cech-cohomology-of-the-punctured-affine-plane)
        - [Čech cohomology of twists on the projective line](ringed-space.md#cech-cohomology-of-twists-on-the-projective-line)
          - [Holomorphic Laurent-series cohomology of twists on the projective line](ringed-space.md#holomorphic-laurent-series-cohomology-of-twists-on-the-projective-line)
        - [Čech cohomology of an affine cover can differ from sheaf cohomology](ringed-space.md#cech-cohomology-of-an-affine-cover-can-differ-from-sheaf-cohomology)
        - [Čech-de Rham double complex](ringed-space.md#cech-de-rham-double-complex)
        - [Čech lifting below the first possible local cohomology degree](ringed-space.md#cech-lifting-below-the-first-possible-local-cohomology-degree)
        - [Čech cochain complex](ringed-space.md#cech-cochain-complex)
          - [Čech differential](ringed-space.md#cech-differential)
          - [Čech resolution on a semi-separated scheme](ringed-space.md#cech-resolution-on-a-semi-separated-scheme)
          - [Exactness of the unit-ideal localization Čech complex](ringed-space.md#exactness-of-the-unit-ideal-localization-cech-complex)
          - [Čech cochain group](ringed-space.md#cech-cochain-group)
          - [Čech cocycle condition](ringed-space.md#cech-cocycle-condition)
          - [Čech coboundary](ringed-space.md#cech-coboundary)
        - [Leray's theorem](ringed-space.md#leray-s-theorem)
          - [Cohomology under a closed immersion](ringed-space.md#cohomology-under-a-closed-immersion)
          - [Cohomological dimension bound from an affine cover](ringed-space.md#cohomological-dimension-bound-from-an-affine-cover)
      - [Fine sheaf](ringed-space.md#fine-sheaf)
      - [Mayer-Vietoris sequence for sheaf cohomology](ringed-space.md#mayer-vietoris-sequence-for-sheaf-cohomology)
      - [Long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology)
      - [Serre duality](ringed-space.md#serre-duality)
        - [Dualizing sheaf on a smooth projective curve](ringed-space.md#dualizing-sheaf-on-a-smooth-projective-curve)
          - [Residue trace on a smooth projective curve](ringed-space.md#residue-trace-on-a-smooth-projective-curve)
        - [Residue duality on the projective line](ringed-space.md#residue-duality-on-the-projective-line)
        - [Failure of ordinary sheaf-dual Serre duality for a skyscraper sheaf](ringed-space.md#failure-of-ordinary-sheaf-dual-serre-duality-for-a-skyscraper-sheaf)
        - [Serre duality for compact complex manifolds](ringed-space.md#serre-duality-for-compact-complex-manifolds)
  - [Locally ringed space](ringed-space.md#locally-ringed-space)
    - [Morphism of locally ringed spaces](ringed-space.md#morphism-of-locally-ringed-spaces)
    - [Scheme](ringed-space.md#scheme)
      - [Functor represented by a scheme](ringed-space.md#functor-represented-by-a-scheme)
      - [Gluing of schemes along open subschemes](ringed-space.md#gluing-of-schemes-along-open-subschemes)
      - [Formal scheme](ringed-space.md#formal-scheme)
        - [Formal completion of a scheme](ringed-space.md#formal-completion-of-a-scheme)
          - [Formal completion commutes with restriction to an open subscheme](ringed-space.md#formal-completion-commutes-with-restriction-to-an-open-subscheme)
        - [Formal spectrum](ringed-space.md#formal-spectrum)
      - [Smooth morphism](ringed-space.md#smooth-morphism)
      - [Étale morphism](ringed-space.md#etale-morphism)
        - [Finite étale morphism](ringed-space.md#finite-etale-morphism)
      - [Quasi-compact scheme](ringed-space.md#quasi-compact-scheme)
      - [Open subscheme](ringed-space.md#open-subscheme)
      - [Irreducible scheme](ringed-space.md#irreducible-scheme)
      - [Dimension of a scheme](ringed-space.md#dimension-of-a-scheme)
      - [Structure morphism](ringed-space.md#structure-morphism)
      - [Scheme of characteristic p](ringed-space.md#scheme-of-characteristic-p)
        - [Absolute Frobenius morphism](ringed-space.md#absolute-frobenius-morphism)
          - [Frobenius factorization through a finite normal cover](ringed-space.md#frobenius-factorization-through-a-finite-normal-cover)
      - [Structure sheaf of a scheme](ringed-space.md#structure-sheaf-of-a-scheme)
        - [Idempotent–clopen correspondence](ringed-space.md#idempotent-clopen-correspondence)
        - [Sheaf of units of the structure sheaf](ringed-space.md#sheaf-of-units-of-the-structure-sheaf)
        - [Regular function](ringed-space.md#regular-function)
          - [Global regular function](ringed-space.md#global-regular-function)
            - [Global regular functions on an irreducible projective variety](ringed-space.md#global-regular-functions-on-an-irreducible-projective-variety)
            - [Regular functions on the punctured affine plane](ringed-space.md#regular-functions-on-the-punctured-affine-plane)
      - [Reduced scheme](ringed-space.md#reduced-scheme)
        - [Generic reducedness with no embedded components](ringed-space.md#generic-reducedness-with-no-embedded-components)
        - [Integral scheme](ringed-space.md#integral-scheme)
          - [Generic-point embedding of regular functions](ringed-space.md#generic-point-embedding-of-regular-functions)
      - [Group scheme](ringed-space.md#group-scheme)
        - [Homomorphism of group schemes](ringed-space.md#homomorphism-of-group-schemes)
        - [Multiplication-by-n morphism](ringed-space.md#multiplication-by-n-morphism)
      - [Nonreduced scheme](ringed-space.md#nonreduced-scheme)
        - [Nonreduced double point](ringed-space.md#nonreduced-double-point)
      - [Punctual scheme](ringed-space.md#punctual-scheme)
      - [Spectrum of a commutative ring](ringed-space.md#spectrum-of-a-commutative-ring)
        - [Spectrum map for the complexification of a real polynomial ring](ringed-space.md#spectrum-map-for-the-complexification-of-a-real-polynomial-ring)
        - [Disconnected reduced spectrum product decomposition](ringed-space.md#disconnected-reduced-spectrum-product-decomposition)
        - [Affine scheme](ringed-space.md#affine-scheme)
          - [Affine gluing along closed subschemes](ringed-space.md#affine-gluing-along-closed-subschemes)
          - [Cohomological criterion for affineness](ringed-space.md#cohomological-criterion-for-affineness)
            - [Unit-ideal certificate from a principal affine cover](ringed-space.md#unit-ideal-certificate-from-a-principal-affine-cover)
            - [Affine principal neighbourhoods from ideal-sheaf vanishing](ringed-space.md#affine-principal-neighbourhoods-from-ideal-sheaf-vanishing)
            - [Ideal-sheaf vanishing for a coherent submodule of a trivial bundle](ringed-space.md#ideal-sheaf-vanishing-for-a-coherent-submodule-of-a-trivial-bundle)
          - [Affine scheme reconstruction from global sections](ringed-space.md#affine-scheme-reconstruction-from-global-sections)
          - [Affine open subscheme](ringed-space.md#affine-open-subscheme)
            - [Affine chart of a variety](ringed-space.md#affine-chart-of-a-variety)
          - [Principal open subscheme](ringed-space.md#principal-open-subscheme)
            - [Dense principal open inside a dense open subset](ringed-space.md#dense-principal-open-inside-a-dense-open-subset)
          - [Affine line](ringed-space.md#affine-line)
          - [Affine plane](ringed-space.md#affine-plane)
            - [Real affine plane scheme points](ringed-space.md#real-affine-plane-scheme-points)
            - [Punctured affine plane](ringed-space.md#punctured-affine-plane)
              - [Nonaffineness of a punctured affine plane](ringed-space.md#nonaffineness-of-a-punctured-affine-plane)
          - [Affine three-space](ringed-space.md#affine-three-space)
            - [Punctured affine three-space](ringed-space.md#punctured-affine-three-space)
      - [Noetherian scheme](ringed-space.md#noetherian-scheme)
        - [Regular scheme](ringed-space.md#regular-scheme)
          - [Regular in codimension one](ringed-space.md#regular-in-codimension-one)
        - [Normal scheme](ringed-space.md#normal-scheme)
          - [Normalization of an integral scheme](ringed-space.md#normalization-of-an-integral-scheme)
          - [Normal variety](ringed-space.md#normal-variety)
            - [Normal surface singularity](ringed-space.md#normal-surface-singularity)
              - [Rational double point](ringed-space.md#rational-double-point)
            - [Normality of a quadratic cone](ringed-space.md#normality-of-a-quadratic-cone)
          - [Codimension-two extension of regular functions on a normal variety](ringed-space.md#codimension-two-extension-of-regular-functions-on-a-normal-variety)
          - [Serre's criterion for normality](ringed-space.md#serre-s-criterion-for-normality)
      - [Morphism of schemes](ringed-space.md#morphism-of-schemes)
        - [Graph morphism of schemes](ringed-space.md#graph-morphism-of-schemes)
        - [Affine-target adjunction for schemes](ringed-space.md#affine-target-adjunction-for-schemes)
        - [Stein factorization](ringed-space.md#stein-factorization)
        - [Isomorphism of schemes](ringed-space.md#isomorphism-of-schemes)
        - [Fiber product of schemes](ringed-space.md#fiber-product-of-schemes)
          - [Scheme-theoretic intersection](ringed-space.md#scheme-theoretic-intersection)
          - [Point-lifting property of a scheme fibre product](ringed-space.md#point-lifting-property-of-a-scheme-fibre-product)
          - [Scheme-theoretic fibre](ringed-space.md#scheme-theoretic-fibre)
            - [Nonaffine special fibre obtained by blowing up](ringed-space.md#nonaffine-special-fibre-obtained-by-blowing-up)
            - [Real fourth-power fibre classification](ringed-space.md#real-fourth-power-fibre-classification)
            - [Nonreduced reducible fibre between integral schemes](ringed-space.md#nonreduced-reducible-fibre-between-integral-schemes)
            - [Integrality of the generic fibre of an affine dominant morphism](ringed-space.md#integrality-of-the-generic-fibre-of-an-affine-dominant-morphism)
          - [Universal property of a fibre product](ringed-space.md#universal-property-of-a-fibre-product)
          - [Base change of a morphism of schemes](ringed-space.md#base-change-of-a-morphism-of-schemes)
            - [Global-section base-change failure in a flat projective family](ringed-space.md#global-section-base-change-failure-in-a-flat-projective-family)
            - [Complexification fibres of a real scheme](ringed-space.md#complexification-fibres-of-a-real-scheme)
            - [Surjectivity is preserved by base change](ringed-space.md#surjectivity-is-preserved-by-base-change)
        - [Locally closed immersion](ringed-space.md#locally-closed-immersion)
          - [Open immersion](ringed-space.md#open-immersion)
          - [Diagonal morphism](ringed-space.md#diagonal-morphism)
            - [Coincidence locus of two scheme morphisms](ringed-space.md#coincidence-locus-of-two-scheme-morphisms)
        - [Kähler differential](ringed-space.md#kahler-differential)
          - [Kähler differentials under a separable field extension](ringed-space.md#kahler-differentials-under-a-separable-field-extension)
          - [Base change for Kähler differentials](ringed-space.md#base-change-for-kahler-differentials)
          - [Localization of Kähler differentials](ringed-space.md#localization-of-kahler-differentials)
          - [Kähler differentials of a polynomial algebra](ringed-space.md#kahler-differentials-of-a-polynomial-algebra)
          - [Universal property of Kähler differentials](ringed-space.md#universal-property-of-kahler-differentials)
          - [Conormal module of the diagonal](ringed-space.md#conormal-module-of-the-diagonal)
          - [Conormal exact sequence for Kähler differentials](ringed-space.md#conormal-exact-sequence-for-kahler-differentials)
            - [Conormal sheaf](ringed-space.md#conormal-sheaf)
              - [Normal sheaf](ringed-space.md#normal-sheaf)
                - [Normal sheaf of a projective complete intersection](ringed-space.md#normal-sheaf-of-a-projective-complete-intersection)
              - [Conormal injectivity for a generically smooth Cartier divisor](ringed-space.md#conormal-injectivity-for-a-generically-smooth-cartier-divisor)
          - [Transitivity exact sequence for Kähler differentials](ringed-space.md#transitivity-exact-sequence-for-kahler-differentials)
          - [Sheaf of relative Kähler differentials](ringed-space.md#sheaf-of-relative-kahler-differentials)
            - [Tangent sheaf of a scheme](ringed-space.md#tangent-sheaf-of-a-scheme)
            - [Cotangent-sheaf cohomology of projective space](ringed-space.md#cotangent-sheaf-cohomology-of-projective-space)
            - [Sheaf of Kähler differentials over a field](ringed-space.md#sheaf-of-kahler-differentials-over-a-field)
              - [Algebraic cotangent bundle](ringed-space.md#algebraic-cotangent-bundle)
              - [Local freeness of differentials on a smooth variety](ringed-space.md#local-freeness-of-differentials-on-a-smooth-variety)
            - [Canonical line bundle of a smooth variety](ringed-space.md#canonical-line-bundle-of-a-smooth-variety)
              - [Canonical divisor of a smooth variety](ringed-space.md#canonical-divisor-of-a-smooth-variety)
                - [Plurigenus](ringed-space.md#plurigenus)
                  - [Blowup invariance of plurigenera](ringed-space.md#blowup-invariance-of-plurigenera)
        - [Affine morphism](ringed-space.md#affine-morphism)
          - [Cohomology under an affine morphism](ringed-space.md#cohomology-under-an-affine-morphism)
        - [Flat morphism](ringed-space.md#flat-morphism)
          - [Finite flat rank over an irreducible scheme](ringed-space.md#finite-flat-rank-over-an-irreducible-scheme)
        - [Morphism of finite type](ringed-space.md#morphism-of-finite-type)
          - [Quasi-finite morphism](ringed-space.md#quasi-finite-morphism)
        - [Universally closed morphism](ringed-space.md#universally-closed-morphism)
          - [Projective line with a doubled point](ringed-space.md#projective-line-with-a-doubled-point)
        - [Separated morphism](ringed-space.md#separated-morphism)
          - [Separated scheme](ringed-space.md#separated-scheme)
            - [Separated variety](ringed-space.md#separated-variety)
          - [Valuative criterion for separatedness](ringed-space.md#valuative-criterion-for-separatedness)
        - [Proper morphism](ringed-space.md#proper-morphism)
          - [Complete variety](ringed-space.md#complete-variety)
          - [Proper affine morphisms are finite](ringed-space.md#proper-affine-morphisms-are-finite)
          - [Properness descends from a surjective source](ringed-space.md#properness-descends-from-a-surjective-source)
          - [Properness cancels through a separated morphism](ringed-space.md#properness-cancels-through-a-separated-morphism)
          - [Properness is local on the target](ringed-space.md#properness-is-local-on-the-target)
          - [Proper closed-point fibers do not imply properness](ringed-space.md#proper-closed-point-fibers-do-not-imply-properness)
          - [Finite complex computing cohomology in a proper flat family](ringed-space.md#finite-complex-computing-cohomology-in-a-proper-flat-family)
            - [Cohomology and base change for line bundles on a curve](ringed-space.md#cohomology-and-base-change-for-line-bundles-on-a-curve)
            - [Semicontinuity theorem for coherent cohomology](ringed-space.md#semicontinuity-theorem-for-coherent-cohomology)
              - [Constancy of line bundle degree in a family](ringed-space.md#constancy-of-line-bundle-degree-in-a-family)
          - [Valuative criterion for properness](ringed-space.md#valuative-criterion-for-properness)
          - [Projective morphism](ringed-space.md#projective-morphism)
            - [Closedness of projection from projective space](ringed-space.md#closedness-of-projection-from-projective-space)
              - [Rational-point projection need not be Zariski closed](ringed-space.md#rational-point-projection-need-not-be-zariski-closed)
          - [Projective scheme](ringed-space.md#projective-scheme)
            - [Proj construction](ringed-space.md#proj-construction)
              - [Degree-one generation condition for Proj](ringed-space.md#degree-one-generation-condition-for-proj)
              - [Sheaf associated with a graded module](ringed-space.md#sheaf-associated-with-a-graded-module)
                - [Tensor compatibility of graded sheafification on degree-one-generated Proj](ringed-space.md#tensor-compatibility-of-graded-sheafification-on-degree-one-generated-proj)
                - [Twisting sheaf on Proj](ringed-space.md#twisting-sheaf-on-proj)
              - [Irrelevant ideal of a graded ring](ringed-space.md#irrelevant-ideal-of-a-graded-ring)
              - [Standard affine open of Proj](ringed-space.md#standard-affine-open-of-proj)
                - [Morphism on Proj induced by a graded ring homomorphism](ringed-space.md#morphism-on-proj-induced-by-a-graded-ring-homomorphism)
                  - [Invariance of Proj under an eventual graded isomorphism](ringed-space.md#invariance-of-proj-under-an-eventual-graded-isomorphism)
              - [Relative Proj construction](ringed-space.md#relative-proj-construction)
              - [Veronese subring](ringed-space.md#veronese-subring)
                - [Veronese embedding](ringed-space.md#veronese-embedding)
        - [Closed immersion](ringed-space.md#closed-immersion)
          - [Flat closed immersion of finite presentation](ringed-space.md#flat-closed-immersion-of-finite-presentation)
          - [Closed immersion criterion for affine schemes](ringed-space.md#closed-immersion-criterion-for-affine-schemes)
          - [Nilpotent thickening](ringed-space.md#nilpotent-thickening)
          - [Closed subscheme](ringed-space.md#closed-subscheme)
            - [Infinitesimal neighbourhood of a closed subscheme](ringed-space.md#infinitesimal-neighbourhood-of-a-closed-subscheme)
            - [Projective complete intersection](ringed-space.md#projective-complete-intersection)
              - [Unmixedness of a complete intersection](ringed-space.md#unmixedness-of-a-complete-intersection)
              - [Global regular functions on a positive-dimensional projective complete intersection](ringed-space.md#global-regular-functions-on-a-positive-dimensional-projective-complete-intersection)
              - [Intermediate cohomology vanishing for a projective complete intersection](ringed-space.md#intermediate-cohomology-vanishing-for-a-projective-complete-intersection)
            - [Construction of a closed subscheme from a quasi-coherent ideal](ringed-space.md#construction-of-a-closed-subscheme-from-a-quasi-coherent-ideal)
            - [Ideal sheaf of a closed subscheme](ringed-space.md#ideal-sheaf-of-a-closed-subscheme)
              - [Ideal sheaf of a closed point](ringed-space.md#ideal-sheaf-of-a-closed-point)
                - [Ideal sheaf of two closed points](ringed-space.md#ideal-sheaf-of-two-closed-points)
              - [Rank bound for locally free ideals on reduced schemes](ringed-space.md#rank-bound-for-locally-free-ideals-on-reduced-schemes)
            - [Structure-sheaf sequence of a hypersurface](ringed-space.md#structure-sheaf-sequence-of-a-hypersurface)
            - [Reduced induced subscheme](ringed-space.md#reduced-induced-subscheme)
            - [Scheme-theoretic image](ringed-space.md#scheme-theoretic-image)
      - [Affine plane with doubled origin](ringed-space.md#affine-plane-with-doubled-origin)
      - [Semi-separated scheme](ringed-space.md#semi-separated-scheme)
        - [Exact direct image from an affine open in a semi-separated scheme](ringed-space.md#exact-direct-image-from-an-affine-open-in-a-semi-separated-scheme)
  - [Direct image functor](ringed-space.md#direct-image-functor)
  - [Inverse image functor](ringed-space.md#inverse-image-functor)
  - [Valuative criterion](ringed-space.md#valuative-criterion)
- [Weil divisor](#weil-divisor)
  - [Q-Cartier divisor](#q-cartier-divisor)
  - [Linear system of divisors](#linear-system-of-divisors)
    - [Bertini smoothness theorem](#bertini-smoothness-theorem)
    - [Genus-two quartic from a degree-four complete linear system](#genus-two-quartic-from-a-degree-four-complete-linear-system)
    - [Base-point-free linear system](#base-point-free-linear-system)
      - [Very ample linear system](#very-ample-linear-system)
        - [Length-two criterion for a very ample linear system](#length-two-criterion-for-a-very-ample-linear-system)
  - [Support of a Weil divisor](#support-of-a-weil-divisor)
  - [Linear equivalence of Weil divisors](#linear-equivalence-of-weil-divisors)
    - [Unavoidable support at a non-Cartier point](#unavoidable-support-at-a-non-cartier-point)
  - [Divisorial ideal](#divisorial-ideal)
  - [Principal Weil divisor](#principal-weil-divisor)
  - [Prime Weil divisor](#prime-weil-divisor)
  - [Divisor class group](#divisor-class-group)
    - [Divisor class groups of products of projective spaces](#divisor-class-groups-of-products-of-projective-spaces)
    - [Divisor class group of a plane-curve complement](#divisor-class-group-of-a-plane-curve-complement)
    - [Divisor class group and Picard group of a smooth curve](#divisor-class-group-and-picard-group-of-a-smooth-curve)
      - [Nonfinite generation of elliptic-curve divisor class groups](#nonfinite-generation-of-elliptic-curve-divisor-class-groups)
    - [Divisor-class criterion for unique factorization](#divisor-class-criterion-for-unique-factorization)
    - [Localization sequence for the divisor class group](#localization-sequence-for-the-divisor-class-group)
      - [Nagata theorem for divisor class groups](#nagata-theorem-for-divisor-class-groups)
        - [Divisor class group of the three-dimensional affine quadric cone](#divisor-class-group-of-the-three-dimensional-affine-quadric-cone)
      - [Divisor class group of a projective-space bundle with trivial vector bundle](#divisor-class-group-of-a-projective-space-bundle-with-trivial-vector-bundle)
    - [Divisor class group of an A-type surface singularity](#divisor-class-group-of-an-a-type-surface-singularity)
- [Cartier divisor](cartier-divisor.md)
  - [Pullback of a Cartier divisor](cartier-divisor.md#pullback-of-a-cartier-divisor)
  - [Cartier divisor exact sequence for an integral domain](cartier-divisor.md#cartier-divisor-exact-sequence-for-an-integral-domain)
  - [Divisor line bundle](cartier-divisor.md#divisor-line-bundle)
  - [Real Cartier divisor](cartier-divisor.md#real-cartier-divisor)
    - [Ample real divisor](cartier-divisor.md#ample-real-divisor)
    - [Real linear equivalence of divisors](cartier-divisor.md#real-linear-equivalence-of-divisors)
  - [Positivity of divisors](cartier-divisor.md#positivity-of-divisors)
    - [Semiample divisor](cartier-divisor.md#semiample-divisor)
      - [Semiampleness of a square-zero rational curve](cartier-divisor.md#semiampleness-of-a-square-zero-rational-curve)
      - [Semiample and curve-positive ampleness criterion](cartier-divisor.md#semiample-and-curve-positive-ampleness-criterion)
      - [Restriction ampleness implies semiampleness for an effective divisor](cartier-divisor.md#restriction-ampleness-implies-semiampleness-for-an-effective-divisor)
    - [Big divisor](cartier-divisor.md#big-divisor)
      - [Algebraic Morse inequality for ample divisors](cartier-divisor.md#algebraic-morse-inequality-for-ample-divisors)
      - [Bigness under finite normalization](cartier-divisor.md#bigness-under-finite-normalization)
      - [Big real divisor](cartier-divisor.md#big-real-divisor)
        - [Negative curves of a big real divisor lie in finitely many divisors](cartier-divisor.md#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors)
          - [Uniform ample subtraction from a big divisor with ample exceptional restrictions](cartier-divisor.md#uniform-ample-subtraction-from-a-big-divisor-with-ample-exceptional-restrictions)
        - [Componentwise bigness on a projective scheme](cartier-divisor.md#componentwise-bigness-on-a-projective-scheme)
        - [Rational approximation of an ample-plus-effective real divisor](cartier-divisor.md#rational-approximation-of-an-ample-plus-effective-real-divisor)
        - [Big cone](cartier-divisor.md#big-cone)
      - [Birational linear system criterion for bigness](cartier-divisor.md#birational-linear-system-criterion-for-bigness)
      - [Kodaira's lemma](cartier-divisor.md#kodaira-s-lemma)
      - [Section subtraction lemma for big divisors](cartier-divisor.md#section-subtraction-lemma-for-big-divisors)
    - [Numerical equivalence of divisors](cartier-divisor.md#numerical-equivalence-of-divisors)
      - [Real numerical divisor classes](cartier-divisor.md#real-numerical-divisor-classes)
        - [Nef cone](cartier-divisor.md#nef-cone)
          - [Ample cone](cartier-divisor.md#ample-cone)
            - [Nef-plus-ample ampleness lemma](cartier-divisor.md#nef-plus-ample-ampleness-lemma)
        - [Closed cone of curves](cartier-divisor.md#closed-cone-of-curves)
    - [Nef line bundle](cartier-divisor.md#nef-line-bundle)
      - [Volume of a nef divisor](cartier-divisor.md#volume-of-a-nef-divisor)
    - [Ample Cartier divisor](cartier-divisor.md#ample-cartier-divisor)
      - [Toric ampleness criterion](cartier-divisor.md#toric-ampleness-criterion)
      - [Vanishing-section ampleness criterion](cartier-divisor.md#vanishing-section-ampleness-criterion)
      - [Euler-characteristic ampleness criterion](cartier-divisor.md#euler-characteristic-ampleness-criterion)
      - [Kleiman's criterion](cartier-divisor.md#kleiman-s-criterion)
      - [Nakai–Moishezon criterion](cartier-divisor.md#nakai-moishezon-criterion)
        - [Real Nakai–Moishezon criterion](cartier-divisor.md#real-nakai-moishezon-criterion)
  - [Linear equivalence of Cartier divisors](cartier-divisor.md#linear-equivalence-of-cartier-divisors)
    - [Principal Cartier divisor](cartier-divisor.md#principal-cartier-divisor)
  - [Effective Cartier divisor](cartier-divisor.md#effective-cartier-divisor)
    - [Relative effective Cartier divisor on a curve](cartier-divisor.md#relative-effective-cartier-divisor-on-a-curve)
    - [Locally principal subvariety](cartier-divisor.md#locally-principal-subvariety)
    - [Divisor restriction exact sequence](cartier-divisor.md#divisor-restriction-exact-sequence)
  - [Complete linear system of a divisor](cartier-divisor.md#complete-linear-system-of-a-divisor)
    - [Iitaka dimension](cartier-divisor.md#iitaka-dimension)
    - [Movable part of a linear system](cartier-divisor.md#movable-part-of-a-linear-system)
    - [Fixed part of a linear system](cartier-divisor.md#fixed-part-of-a-linear-system)
      - [Fixed component](cartier-divisor.md#fixed-component)
    - [Basepoint-free divisor](cartier-divisor.md#basepoint-free-divisor)
      - [Toric basepoint-free criterion](cartier-divisor.md#toric-basepoint-free-criterion)
    - [Very ample divisor](cartier-divisor.md#very-ample-divisor)
      - [High-degree divisor is very ample on a smooth projective curve](cartier-divisor.md#high-degree-divisor-is-very-ample-on-a-smooth-projective-curve)
  - [Hyperplane divisor](cartier-divisor.md#hyperplane-divisor)
    - [Hyperplane section](cartier-divisor.md#hyperplane-section)
      - [Bertini's theorem](cartier-divisor.md#bertini-s-theorem)
      - [Hyperplane-section divisor of a projective plane curve](cartier-divisor.md#hyperplane-section-divisor-of-a-projective-plane-curve)
  - [Line bundle associated to a divisor](cartier-divisor.md#line-bundle-associated-to-a-divisor)
  - [Cartier class group](cartier-divisor.md#cartier-class-group)
- [Algebraic variety](#algebraic-variety)
  - [Rational map of algebraic varieties](#rational-map-of-algebraic-varieties)
  - [Ring of rational functions on a reduced variety](#ring-of-rational-functions-on-a-reduced-variety)
    - [Local ring embeds in rational functions on incident components](#local-ring-embeds-in-rational-functions-on-incident-components)
  - [Rational function on an algebraic variety](#rational-function-on-an-algebraic-variety)
  - [Quasi-projective algebraic set](#quasi-projective-algebraic-set)
    - [Quasi-projective variety](#quasi-projective-variety)
  - [Irreducible variety](#irreducible-variety)
  - [Constructible subset of a variety](#constructible-subset-of-a-variety)
    - [Chevalley constructibility theorem](#chevalley-constructibility-theorem)
  - [Rational point](#rational-point)
  - [Smooth algebraic variety](#smooth-algebraic-variety)
    - [Smoothness of an algebraic variety](#smoothness-of-an-algebraic-variety)
  - [Normalization of an algebraic variety](#normalization-of-an-algebraic-variety)
  - [Closed subvariety](#closed-subvariety)
  - [Algebraic curve](#algebraic-curve)
    - [Integral projective curve](#integral-projective-curve)
    - [Nonsingular point of an algebraic curve](#nonsingular-point-of-an-algebraic-curve)
    - [Affine algebraic curve](#affine-algebraic-curve)
    - [Cuspidal cubic](#cuspidal-cubic)
      - [Unique smooth flex of a cuspidal cubic](#unique-smooth-flex-of-a-cuspidal-cubic)
      - [Cusp with two isolated-point components](#cusp-with-two-isolated-point-components)
    - [Symmetric product of a curve](#symmetric-product-of-a-curve)
    - [Monomial curve](#monomial-curve)
      - [Monomial curve with exponents three, four and five](#monomial-curve-with-exponents-three-four-and-five)
    - [Rational parametrization of an algebraic curve](#rational-parametrization-of-an-algebraic-curve)
    - [Arithmetic genus](#arithmetic-genus)
      - [Genus of a complete-intersection space curve](#genus-of-a-complete-intersection-space-curve)
  - [Prevariety](#prevariety)
  - [Algebraic group](#algebraic-group)
    - [Isogeny](#isogeny)
    - [Multiplicative group scheme](#multiplicative-group-scheme)
    - [Multiplicative algebraic group](#multiplicative-algebraic-group)
    - [Algebraic group action](#algebraic-group-action)
    - [Dimension formula for an algebraic group homomorphism](#dimension-formula-for-an-algebraic-group-homomorphism)
    - [Constructible subgroup is closed](#constructible-subgroup-is-closed)
    - [Homomorphism of group varieties](#homomorphism-of-group-varieties)
    - [Abelian variety](abelian-variety.md)
      - [Prime-to-characteristic torsion of an abelian variety](abelian-variety.md#prime-to-characteristic-torsion-of-an-abelian-variety)
      - [Jacobian variety](abelian-variety.md#jacobian-variety)
        - [Torelli theorem](abelian-variety.md#torelli-theorem)
        - [Universal property of the Jacobian variety](abelian-variety.md#universal-property-of-the-jacobian-variety)
        - [Theta divisor](abelian-variety.md#theta-divisor)
          - [Riemann vanishing theorem](abelian-variety.md#riemann-vanishing-theorem)
            - [Theta pullback zero-divisor identity](abelian-variety.md#theta-pullback-zero-divisor-identity)
            - [Vector of Riemann constants](abelian-variety.md#vector-of-riemann-constants)
          - [Gauss map of a theta divisor](abelian-variety.md#gauss-map-of-a-theta-divisor)
            - [Branch locus of the theta Gauss map](abelian-variety.md#branch-locus-of-the-theta-gauss-map)
          - [Riemann singularity theorem](abelian-variety.md#riemann-singularity-theorem)
            - [Schur complement presentation of a theta singularity](abelian-variety.md#schur-complement-presentation-of-a-theta-singularity)
            - [Tangent cone to a theta divisor](abelian-variety.md#tangent-cone-to-a-theta-divisor)
          - [Theta autoduality of a Jacobian](abelian-variety.md#theta-autoduality-of-a-jacobian)
          - [Restriction of the theta divisor to an Abel curve](abelian-variety.md#restriction-of-the-theta-divisor-to-an-abel-curve)
          - [Determinant description of the theta divisor](abelian-variety.md#determinant-description-of-the-theta-divisor)
            - [Invertible cup-product direction for a line bundle on a curve](abelian-variety.md#invertible-cup-product-direction-for-a-line-bundle-on-a-curve)
            - [Evaluation determinant on a product of curves](abelian-variety.md#evaluation-determinant-on-a-product-of-curves)
              - [Torsion trivialization in a determinant quotient](abelian-variety.md#torsion-trivialization-in-a-determinant-quotient)
        - [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve)
          - [Derivative of the Abelian sum map](abelian-variety.md#derivative-of-the-abelian-sum-map)
            - [Repeated-point Abel differential formula](abelian-variety.md#repeated-point-abel-differential-formula)
      - [Curve generation criterion for an abelian variety](abelian-variety.md#curve-generation-criterion-for-an-abelian-variety)
      - [Dual abelian variety](abelian-variety.md#dual-abelian-variety)
        - [Weil pairing for an abelian variety](abelian-variety.md#weil-pairing-for-an-abelian-variety)
        - [Poincaré line bundle](abelian-variety.md#poincare-line-bundle)
      - [Mumford rigidity lemma](abelian-variety.md#mumford-rigidity-lemma)
      - [Invariant differential on a group scheme](abelian-variety.md#invariant-differential-on-a-group-scheme)
      - [Theorem of the Cube](abelian-variety.md#theorem-of-the-cube)
        - [Arithmetic cube identity for Weil heights](abelian-variety.md#arithmetic-cube-identity-for-weil-heights)
        - [Cohomological proof of the cube theorem for elliptic curves](abelian-variety.md#cohomological-proof-of-the-cube-theorem-for-elliptic-curves)
        - [Bilinear cross-effect of a line bundle on an abelian variety](abelian-variety.md#bilinear-cross-effect-of-a-line-bundle-on-an-abelian-variety)
        - [Theorem of the square](abelian-variety.md#theorem-of-the-square)
          - [Homomorphism associated to a line bundle on an abelian variety](abelian-variety.md#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)
            - [Line bundle translation stabilizer](abelian-variety.md#line-bundle-translation-stabilizer)
            - [Identity component of the Picard group](abelian-variety.md#identity-component-of-the-picard-group)
              - [Seesaw theorem](abelian-variety.md#seesaw-theorem)
  - [Smooth algebraic curve](#smooth-algebraic-curve)
    - [Product dimension bound for sections on a curve](#product-dimension-bound-for-sections-on-a-curve)
  - [Affine algebraic set](#affine-algebraic-set)
    - [Affineness from a unit-ideal principal affine cover](#affineness-from-a-unit-ideal-principal-affine-cover)
    - [Morphism of affine varieties](#morphism-of-affine-varieties)
    - [Coordinate ring of a product of affine varieties](#coordinate-ring-of-a-product-of-affine-varieties)
    - [Vanishing ideal](#vanishing-ideal)
    - [Coordinate ring](#coordinate-ring)
      - [Irreducibility and prime vanishing ideal](#irreducibility-and-prime-vanishing-ideal)
      - [Dominant morphism of affine varieties](#dominant-morphism-of-affine-varieties)
    - [Vanishing loci of ideal sums and intersections](#vanishing-loci-of-ideal-sums-and-intersections)
    - [Irreducible components of two intersecting complex hyperbolas](#irreducible-components-of-two-intersecting-complex-hyperbolas)
  - [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)
    - [Sheaf of nonzero rational functions on an irreducible variety](#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety)
    - [Dimension from the function field](#dimension-from-the-function-field)
    - [Projective model of a finitely generated field](#projective-model-of-a-finitely-generated-field)
  - [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)
    - [Morphism of algebraic curves](#morphism-of-algebraic-curves)
    - [Conic bundle](#conic-bundle)
      - [Conic discriminant](#conic-discriminant)
        - [Reduced singular fibres of a smooth conic bundle](#reduced-singular-fibres-of-a-smooth-conic-bundle)
    - [Generically finite morphism](#generically-finite-morphism)
    - [Isomorphic local rings determine isomorphic neighborhoods](#isomorphic-local-rings-determine-isomorphic-neighborhoods)
    - [Degree of a morphism of curves](#degree-of-a-morphism-of-curves)
    - [Algebraic quotient by a finite group](#algebraic-quotient-by-a-finite-group)
    - [Affine-target adjunction for varieties](#affine-target-adjunction-for-varieties)
    - [Ramification index of a morphism of curves](#ramification-index-of-a-morphism-of-curves)
    - [Fiber of a morphism](#fiber-of-a-morphism)
      - [Local fibre dimension](#local-fibre-dimension)
        - [Upper semicontinuity of local fibre dimension](#upper-semicontinuity-of-local-fibre-dimension)
      - [Fiber dimension theorem](#fiber-dimension-theorem)
        - [Dimension of image of a morphism](#dimension-of-image-of-a-morphism)
          - [Isolated fibre point forces dominance in equal dimensions](#isolated-fibre-point-forces-dominance-in-equal-dimensions)
        - [Generic equidimensionality of fibres](#generic-equidimensionality-of-fibres)
        - [Closed-fibre lower bound by finite normalization](#closed-fibre-lower-bound-by-finite-normalization)
      - [Scheme-theoretic fiber](#scheme-theoretic-fiber)
        - [Fibre of absolute Frobenius over a rational point of the affine line](#fibre-of-absolute-frobenius-over-a-rational-point-of-the-affine-line)
    - [Isomorphism of algebraic varieties](#isomorphism-of-algebraic-varieties)
    - [Finite morphism](#finite-morphism)
      - [Trace-dual module of a finite curve map](#trace-dual-module-of-a-finite-curve-map)
      - [Finite morphisms are proper](#finite-morphisms-are-proper)
  - [Projective space](projective-space.md)
    - [Projective space represents invertible quotients](projective-space.md#projective-space-represents-invertible-quotients)
    - [Morphisms from projective space to smaller projective space are constant](projective-space.md#morphisms-from-projective-space-to-smaller-projective-space-are-constant)
    - [Dual projective space](projective-space.md#dual-projective-space)
      - [Projective dual variety](projective-space.md#projective-dual-variety)
        - [Projective biduality theorem](projective-space.md#projective-biduality-theorem)
    - [Projective coordinates over a local ring](projective-space.md#projective-coordinates-over-a-local-ring)
    - [Quaternionic projective space](projective-space.md#quaternionic-projective-space)
      - [Complex cobordism ring of the quaternionic projective plane](projective-space.md#complex-cobordism-ring-of-the-quaternionic-projective-plane)
      - [Complex inclusion into quaternionic projective space](projective-space.md#complex-inclusion-into-quaternionic-projective-space)
      - [Cohomology ring of quaternionic projective space](projective-space.md#cohomology-ring-of-quaternionic-projective-space)
    - [General linear position](projective-space.md#general-linear-position)
    - [Veronese map](projective-space.md#veronese-map)
    - [Top cohomology of projective space](projective-space.md#top-cohomology-of-projective-space)
    - [Cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space)
      - [Nonnegative hyperplane twist cohomology by restriction](projective-space.md#nonnegative-hyperplane-twist-cohomology-by-restriction)
      - [Infinite negative-twist sum with zero global sections](projective-space.md#infinite-negative-twist-sum-with-zero-global-sections)
      - [Global regular functions on projective space](projective-space.md#global-regular-functions-on-projective-space)
    - [Projective point](projective-space.md#projective-point)
      - [Homogeneous coordinate](projective-space.md#homogeneous-coordinate)
      - [Coordinate point](projective-space.md#coordinate-point)
    - [Projective plane](projective-space.md#projective-plane)
      - [Point-line duality](projective-space.md#point-line-duality)
        - [Dual arrangement of a planar point set](projective-space.md#dual-arrangement-of-a-planar-point-set)
          - [Good edge of a dual line arrangement](projective-space.md#good-edge-of-a-dual-line-arrangement)
            - [Safe edge of a dual line arrangement](projective-space.md#safe-edge-of-a-dual-line-arrangement)
              - [Bounded-radius propagation of edge defects](projective-space.md#bounded-radius-propagation-of-edge-defects)
          - [Euler defect identity for a projective line arrangement](projective-space.md#euler-defect-identity-for-a-projective-line-arrangement)
      - [Fano plane](projective-space.md#fano-plane)
        - [Fano plane duality group](projective-space.md#fano-plane-duality-group)
        - [Fano point-line stabilizer intersection](projective-space.md#fano-point-line-stabilizer-intersection)
    - [Projective linear transformation](projective-space.md#projective-linear-transformation)
    - [Projective variety](projective-space.md#projective-variety)
      - [Veronese surface](projective-space.md#veronese-surface)
      - [Projective embedding](projective-space.md#projective-embedding)
      - [Pole divisor avoiding a fiber](projective-space.md#pole-divisor-avoiding-a-fiber)
      - [Projective completion](projective-space.md#projective-completion)
        - [Homogenization (algebra)](projective-space.md#homogenization-algebra)
      - [Projective dimension theorem](projective-space.md#projective-dimension-theorem)
      - [Projective curve](projective-space.md#projective-curve)
        - [Rational normal curve](projective-space.md#rational-normal-curve)
        - [Smooth projective curve](projective-space.md#smooth-projective-curve)
          - [Two-affine cover of a smooth projective curve](projective-space.md#two-affine-cover-of-a-smooth-projective-curve)
          - [Genus of a smooth projective curve](projective-space.md#genus-of-a-smooth-projective-curve)
            - [Rationality of a smooth projective genus-zero curve](projective-space.md#rationality-of-a-smooth-projective-genus-zero-curve)
          - [Smooth plane cubic in characteristic three](projective-space.md#smooth-plane-cubic-in-characteristic-three)
          - [Smooth rational curve](projective-space.md#smooth-rational-curve)
          - [Local ring of a smooth algebraic curve](projective-space.md#local-ring-of-a-smooth-algebraic-curve)
            - [Local parameter on a smooth algebraic curve](projective-space.md#local-parameter-on-a-smooth-algebraic-curve)
          - [Extension of a rational map from a smooth projective curve](projective-space.md#extension-of-a-rational-map-from-a-smooth-projective-curve)
            - [Failure of rational-map extension on a singular curve](projective-space.md#failure-of-rational-map-extension-on-a-singular-curve)
      - [Homogeneous coordinate ring](projective-space.md#homogeneous-coordinate-ring)
      - [Product of projective varieties](projective-space.md#product-of-projective-varieties)
        - [Coordinate projection](projective-space.md#coordinate-projection)
        - [Segre embedding](projective-space.md#segre-embedding)
        - [Smooth quadric surface](projective-space.md#smooth-quadric-surface)
          - [Projection from a point on a smooth quadric](projective-space.md#projection-from-a-point-on-a-smooth-quadric)
          - [Picard group of a smooth affine quadric surface](projective-space.md#picard-group-of-a-smooth-affine-quadric-surface)
          - [Segre description of a smooth quadric surface](projective-space.md#segre-description-of-a-smooth-quadric-surface)
          - [Rulings of a smooth quadric surface](projective-space.md#rulings-of-a-smooth-quadric-surface)
            - [Disjoint curves on a smooth quadric surface](projective-space.md#disjoint-curves-on-a-smooth-quadric-surface)
- [Irreducible topological space](#irreducible-topological-space)
  - [Irreducible closed subset](#irreducible-closed-subset)
  - [Dimension of a topological space by irreducible chains](#dimension-of-a-topological-space-by-irreducible-chains)
    - [Dimension of an algebraic set](#dimension-of-an-algebraic-set)
      - [Equidimensional algebraic variety](#equidimensional-algebraic-variety)
      - [Local dimension of an algebraic variety](#local-dimension-of-an-algebraic-variety)
      - [Codimension of an algebraic subvariety](#codimension-of-an-algebraic-subvariety)
  - [Generic point](#generic-point)
  - [Irreducible component](#irreducible-component)
  - [Noetherian Zariski topology](#noetherian-zariski-topology)
- [Zariski-closed set](#zariski-closed-set)
- [Zariski-open set](#zariski-open-set)
  - [Distinguished open set](#distinguished-open-set)
- [Noether normalization](#noether-normalization)
  - [Norm detects proper closed subsets under finite normalization](#norm-detects-proper-closed-subsets-under-finite-normalization)
  - [Linear Noether normalization for a hypersurface](#linear-noether-normalization-for-a-hypersurface)
- [Hilbert Nullstellensatz](#hilbert-nullstellensatz)
  - [Radical ideals and closed subsets of the maximal spectrum](#radical-ideals-and-closed-subsets-of-the-maximal-spectrum)
  - [Weak Hilbert Nullstellensatz](#weak-hilbert-nullstellensatz)
    - [Zariski's lemma](#zariski-s-lemma)
  - [Strong Hilbert Nullstellensatz](#strong-hilbert-nullstellensatz)
    - [Spreading out of an affine zero-set inclusion](#spreading-out-of-an-affine-zero-set-inclusion)
    - [Rabinowitsch trick](#rabinowitsch-trick)
  - [Complex affine algebraic set cardinality dichotomy](#complex-affine-algebraic-set-cardinality-dichotomy)
  - [Projective Nullstellensatz](#projective-nullstellensatz)
    - [Graded multiplication map for a projective fiber](#graded-multiplication-map-for-a-projective-fiber)
    - [Irrelevant ideal of projective space](#irrelevant-ideal-of-projective-space)
  - [Quasi-compactness of an affine variety](#quasi-compactness-of-an-affine-variety)
- [Zariski density of the complex exponential graph](#zariski-density-of-the-complex-exponential-graph)
- [Degree of an algebraic variety](#degree-of-an-algebraic-variety)
  - [Degree of a projective curve](#degree-of-a-projective-curve)
    - [Homological degree of a smooth complex plane curve](#homological-degree-of-a-smooth-complex-plane-curve)
    - [Genus bound for a nonplanar degree-five curve](#genus-bound-for-a-nonplanar-degree-five-curve)
    - [Bézout's theorem](#bezout-s-theorem)
      - [Resultant bound for intersections of plane curves](#resultant-bound-for-intersections-of-plane-curves)
      - [Projective plane curve](#projective-plane-curve)
        - [Plane conic](#plane-conic)
        - [Plane quartic](#plane-quartic)
        - [Multiplicity of a plane curve at a point](#multiplicity-of-a-plane-curve-at-a-point)
        - [Cohomology of a projective plane hypersurface](#cohomology-of-a-projective-plane-hypersurface)
        - [An irreducible plane cubic has at most one singular point](#an-irreducible-plane-cubic-has-at-most-one-singular-point)
        - [Cayley-Bacharach theorem](#cayley-bacharach-theorem)
          - [Eight-point cubic completion for two triples of lines](#eight-point-cubic-completion-for-two-triples-of-lines)
            - [Cubic propagation along a triangular strip](#cubic-propagation-along-a-triangular-strip)
        - [Smooth plane conic](#smooth-plane-conic)
          - [Dual conic](#dual-conic)
            - [Genus one tangent incidence curve of two conics](#genus-one-tangent-incidence-curve-of-two-conics)
              - [Poncelet porism](#poncelet-porism)
          - [Homology of the complement of a smooth conic](#homology-of-the-complement-of-a-smooth-conic)
        - [Plane cubic](#plane-cubic)
          - [Degenerate cubic containing a line](#degenerate-cubic-containing-a-line)
        - [Real conic without real rational points](#real-conic-without-real-rational-points)
        - [Genus-degree formula](#genus-degree-formula)
          - [Plane curve singularity multiplicity bound](#plane-curve-singularity-multiplicity-bound)
            - [Rationality of a plane quartic with three double points](#rationality-of-a-plane-quartic-with-three-double-points)
      - [Intersection multiplicity](#intersection-multiplicity)
        - [Inflection point of an algebraic plane curve](#inflection-point-of-an-algebraic-plane-curve)
          - [Hessian criterion for a flex](#hessian-criterion-for-a-flex)
            - [Hessian curve of a plane cubic](#hessian-curve-of-a-plane-cubic)
    - [Hilbert polynomial](#hilbert-polynomial)
      - [Polynomial bound for sections of a fixed divisor](#polynomial-bound-for-sections-of-a-fixed-divisor)
    - [Generic hyperplane section of a projective curve](#generic-hyperplane-section-of-a-projective-curve)
    - [Degree under a linear projective embedding](#degree-under-a-linear-projective-embedding)
    - [Embedding dependence of projective degree](#embedding-dependence-of-projective-degree)
- [Twisted cubic](#twisted-cubic)
  - [Standard monomials of the twisted cubic](#standard-monomials-of-the-twisted-cubic)
  - [Nondegenerate projective variety](#nondegenerate-projective-variety)
  - [Degree obstruction to the twisted cubic being a complete intersection](#degree-obstruction-to-the-twisted-cubic-being-a-complete-intersection)
- [Genus distinguishes equal-degree projective curves](#genus-distinguishes-equal-degree-projective-curves)
- [Zariski tangent space](#zariski-tangent-space)
  - [Projective tangent plane](#projective-tangent-plane)
  - [Embedding dimension distinguishes three-branch curves](#embedding-dimension-distinguishes-three-branch-curves)
  - [Algebraic cotangent space](#algebraic-cotangent-space)
  - [Dimension from minimum tangent dimension](#dimension-from-minimum-tangent-dimension)
  - [Smooth locus of a variety](#smooth-locus-of-a-variety)
    - [Singular locus](#singular-locus)
    - [Smooth point of a variety](#smooth-point-of-a-variety)
    - [Singular point of an algebraic variety](#singular-point-of-an-algebraic-variety)
      - [Cusp (algebraic geometry)](#cusp-algebraic-geometry)
      - [Hypersurface singularity](#hypersurface-singularity)
        - [Secant line through singular points of a cubic hypersurface](#secant-line-through-singular-points-of-a-cubic-hypersurface)
      - [Ordinary double point](#ordinary-double-point)
    - [Density of the smooth locus](#density-of-the-smooth-locus)
      - [Jacobian criterion](#jacobian-criterion)
  - [Singular locus of a product with a smooth variety](#singular-locus-of-a-product-with-a-smooth-variety)
  - [Tangent spaces of a product of two nodal line pairs](#tangent-spaces-of-a-product-of-two-nodal-line-pairs)
  - [Tangent-space obstruction between two unions of three lines](#tangent-space-obstruction-between-two-unions-of-three-lines)
- [Krull dimension of an affine variety](#krull-dimension-of-an-affine-variety)
  - [Closed-point dimension lemma for affine domains](#closed-point-dimension-lemma-for-affine-domains)
    - [Principal hypersurface dimension lemma](#principal-hypersurface-dimension-lemma)
  - [Dimension of an irreducible affine variety by transcendence degree](#dimension-of-an-irreducible-affine-variety-by-transcendence-degree)
- [Affine hypersurface](#affine-hypersurface)
  - [Smooth point on an irreducible hypersurface in positive characteristic](#smooth-point-on-an-irreducible-hypersurface-in-positive-characteristic)
  - [Smoothness of a nonzero homogeneous level set](#smoothness-of-a-nonzero-homogeneous-level-set)
  - [Tangent hyperplane section](#tangent-hyperplane-section)
  - [Singular points of an irreducible affine plane cubic](#singular-points-of-an-irreducible-affine-plane-cubic)
  - [Singular cylinder over a nodal curve](#singular-cylinder-over-a-nodal-curve)
- [Projective hypersurface](#projective-hypersurface)
  - [Plane section](#plane-section)
  - [Quadric (algebraic geometry)](#quadric-algebraic-geometry)
  - [Plane quartic with exactly two nodes](#plane-quartic-with-exactly-two-nodes)
  - [Projective gradient criterion in characteristic dividing the degree](#projective-gradient-criterion-in-characteristic-dividing-the-degree)
  - [Ideal-sheaf sequence of a projective hypersurface](#ideal-sheaf-sequence-of-a-projective-hypersurface)
  - [Affine cone](#affine-cone)
    - [Three-dimensional affine quadric cone](#three-dimensional-affine-quadric-cone)
    - [Ruling morphism of the punctured three-dimensional affine quadric cone](#ruling-morphism-of-the-punctured-three-dimensional-affine-quadric-cone)
  - [Pencil of plane curves](#pencil-of-plane-curves)
    - [Fermat cubic curve](#fermat-cubic-curve)
    - [Cubic pencil with a triangular member](#cubic-pencil-with-a-triangular-member)
  - [Affine cone over a projective hypersurface](#affine-cone-over-a-projective-hypersurface)
  - [Projective quadric cone with one singular vertex](#projective-quadric-cone-with-one-singular-vertex)
    - [Projective variety with a prescribed-dimensional singular locus](#projective-variety-with-a-prescribed-dimensional-singular-locus)
- [Determinantal variety](#determinantal-variety)
  - [Smooth projective surface from overlapping rank-one coordinates](#smooth-projective-surface-from-overlapping-rank-one-coordinates)
  - [Rank-one determinantal variety](#rank-one-determinantal-variety)
- [Birational variety](#birational-variety)
  - [Blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface)
    - [Canonical divisor formula for a surface blowup](#canonical-divisor-formula-for-a-surface-blowup)
  - [Birational morphism](#birational-morphism)
  - [Birational map](#birational-map)
  - [Blowup of the affine plane at the origin](#blowup-of-the-affine-plane-at-the-origin)
- [Normalization of an algebraic curve](normalization-of-an-algebraic-curve.md)
  - [Finite normalization model of a one-variable function field](normalization-of-an-algebraic-curve.md#finite-normalization-model-of-a-one-variable-function-field)
  - [Flat normalization is an isomorphism](normalization-of-an-algebraic-curve.md#flat-normalization-is-an-isomorphism)
  - [Geometric genus](normalization-of-an-algebraic-curve.md#geometric-genus)
    - [Genus one curve](normalization-of-an-algebraic-curve.md#genus-one-curve)
      - [Elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve)
        - [Galois cohomology of an elliptic curve](normalization-of-an-algebraic-curve.md#galois-cohomology-of-an-elliptic-curve)
        - [Diagonal cubic elliptic curve](normalization-of-an-algebraic-curve.md#diagonal-cubic-elliptic-curve)
          - [Rational pairs of cubes summing to seven](normalization-of-an-algebraic-curve.md#rational-pairs-of-cubes-summing-to-seven)
          - [Rational torsion of a diagonal cubic](normalization-of-an-algebraic-curve.md#rational-torsion-of-a-diagonal-cubic)
          - [Flexes of a diagonal cubic](normalization-of-an-algebraic-curve.md#flexes-of-a-diagonal-cubic)
        - [Elliptic curve group law from Riemann-Roch](normalization-of-an-algebraic-curve.md#elliptic-curve-group-law-from-riemann-roch)
        - [Three-torsion points are flexes of a plane cubic](normalization-of-an-algebraic-curve.md#three-torsion-points-are-flexes-of-a-plane-cubic)
        - [Complex uniformization of an elliptic curve](normalization-of-an-algebraic-curve.md#complex-uniformization-of-an-elliptic-curve)
        - [Weierstrass uniformization by half-period values](normalization-of-an-algebraic-curve.md#weierstrass-uniformization-by-half-period-values)
        - [Nonparametrizability of an elliptic curve](normalization-of-an-algebraic-curve.md#nonparametrizability-of-an-elliptic-curve)
        - [j-invariant of an elliptic curve](normalization-of-an-algebraic-curve.md#j-invariant-of-an-elliptic-curve)
        - [Abel-Jacobi map of a genus-one curve](normalization-of-an-algebraic-curve.md#abel-jacobi-map-of-a-genus-one-curve)
          - [Involution of a degree-two map from a genus one curve](normalization-of-an-algebraic-curve.md#involution-of-a-degree-two-map-from-a-genus-one-curve)
        - [Chord-and-tangent group law](normalization-of-an-algebraic-curve.md#chord-and-tangent-group-law)
          - [Torsion multiples in a two-parameter Weierstrass family](normalization-of-an-algebraic-curve.md#torsion-multiples-in-a-two-parameter-weierstrass-family)
          - [Associativity of the chord-and-tangent law via divisor classes](normalization-of-an-algebraic-curve.md#associativity-of-the-chord-and-tangent-law-via-divisor-classes)
          - [Translation on an elliptic curve](normalization-of-an-algebraic-curve.md#translation-on-an-elliptic-curve)
          - [Smooth-locus group of a singular Weierstrass cubic](normalization-of-an-algebraic-curve.md#smooth-locus-group-of-a-singular-weierstrass-cubic)
          - [Elliptic-curve addition formula](normalization-of-an-algebraic-curve.md#elliptic-curve-addition-formula)
            - [Symmetric-coordinate identity for elliptic-curve addition](normalization-of-an-algebraic-curve.md#symmetric-coordinate-identity-for-elliptic-curve-addition)
        - [Weierstrass equation of an elliptic curve](normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve)
          - [Legendre form of an elliptic curve](normalization-of-an-algebraic-curve.md#legendre-form-of-an-elliptic-curve)
          - [Pole orders on a smooth cubic in Weierstrass form](normalization-of-an-algebraic-curve.md#pole-orders-on-a-smooth-cubic-in-weierstrass-form)
          - [Weierstrass construction from Riemann-Roch in genus one](normalization-of-an-algebraic-curve.md#weierstrass-construction-from-riemann-roch-in-genus-one)
          - [Elliptic-curve discriminant](normalization-of-an-algebraic-curve.md#elliptic-curve-discriminant)
          - [Admissible change of Weierstrass coordinates](normalization-of-an-algebraic-curve.md#admissible-change-of-weierstrass-coordinates)
          - [Short Weierstrass form](normalization-of-an-algebraic-curve.md#short-weierstrass-form)
          - [Invariant differential on an elliptic curve](normalization-of-an-algebraic-curve.md#invariant-differential-on-an-elliptic-curve)
            - [Translation invariance of a Weierstrass differential](normalization-of-an-algebraic-curve.md#translation-invariance-of-a-weierstrass-differential)
          - [Minimal Weierstrass equation](normalization-of-an-algebraic-curve.md#minimal-weierstrass-equation)
            - [Reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#reduction-of-an-elliptic-curve)
              - [Good reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve)
                - [Good-reduction map respects elliptic addition](normalization-of-an-algebraic-curve.md#good-reduction-map-respects-elliptic-addition)
                - [Supersingular reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#supersingular-reduction-of-an-elliptic-curve)
                - [Ordinary reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#ordinary-reduction-of-an-elliptic-curve)
                - [Surjectivity of good reduction over a local field](normalization-of-an-algebraic-curve.md#surjectivity-of-good-reduction-over-a-local-field)
                - [Kernel of reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#kernel-of-reduction-of-an-elliptic-curve)
                  - [Reduction certificate for a nonintegral elliptic point](normalization-of-an-algebraic-curve.md#reduction-certificate-for-a-nonintegral-elliptic-point)
                  - [Reduction exponent obstruction to integral multiples](normalization-of-an-algebraic-curve.md#reduction-exponent-obstruction-to-integral-multiples)
              - [Bad reduction of an elliptic curve](normalization-of-an-algebraic-curve.md#bad-reduction-of-an-elliptic-curve)
                - [Discriminant valuation obstruction to good reduction](normalization-of-an-algebraic-curve.md#discriminant-valuation-obstruction-to-good-reduction)
                - [Bad primes of a congruent number curve with odd parameter](normalization-of-an-algebraic-curve.md#bad-primes-of-a-congruent-number-curve-with-odd-parameter)
              - [Reduction of torsion points on an elliptic curve](normalization-of-an-algebraic-curve.md#reduction-of-torsion-points-on-an-elliptic-curve)
                - [Torsion exclusion from good reduction counts](normalization-of-an-algebraic-curve.md#torsion-exclusion-from-good-reduction-counts)
                - [Two-prime bound on rational elliptic torsion](normalization-of-an-algebraic-curve.md#two-prime-bound-on-rational-elliptic-torsion)
                - [Prime-to-p torsion lifts uniquely at good reduction](normalization-of-an-algebraic-curve.md#prime-to-p-torsion-lifts-uniquely-at-good-reduction)
                - [Prime-two torsion bound for good reduction](normalization-of-an-algebraic-curve.md#prime-two-torsion-bound-for-good-reduction)
        - [Quadratic twist of an elliptic curve](normalization-of-an-algebraic-curve.md#quadratic-twist-of-an-elliptic-curve)
        - [Twist of an elliptic curve](normalization-of-an-algebraic-curve.md#twist-of-an-elliptic-curve)
        - [Inflection point of a plane cubic](normalization-of-an-algebraic-curve.md#inflection-point-of-a-plane-cubic)
          - [Hessian criterion for flexes of a plane cubic](normalization-of-an-algebraic-curve.md#hessian-criterion-for-flexes-of-a-plane-cubic)
            - [Flexes of a Hesse cubic](normalization-of-an-algebraic-curve.md#flexes-of-a-hesse-cubic)
        - [Formal group law](normalization-of-an-algebraic-curve.md#formal-group-law)
          - [Invariant differential of a formal group law](normalization-of-an-algebraic-curve.md#invariant-differential-of-a-formal-group-law)
          - [Isomorphism of formal group laws](normalization-of-an-algebraic-curve.md#isomorphism-of-formal-group-laws)
          - [Formal inverse](normalization-of-an-algebraic-curve.md#formal-inverse)
          - [Formal additive group](normalization-of-an-algebraic-curve.md#formal-additive-group)
          - [Formal multiplicative group](normalization-of-an-algebraic-curve.md#formal-multiplicative-group)
            - [Exponential isomorphism between the additive and multiplicative formal groups](normalization-of-an-algebraic-curve.md#exponential-isomorphism-between-the-additive-and-multiplicative-formal-groups)
          - [Invertible morphism criterion for formal group laws](normalization-of-an-algebraic-curve.md#invertible-morphism-criterion-for-formal-group-laws)
            - [Multiplication isomorphism of a formal group law](normalization-of-an-algebraic-curve.md#multiplication-isomorphism-of-a-formal-group-law)
              - [Prime-to-residue-characteristic multiplication on a formal group](normalization-of-an-algebraic-curve.md#prime-to-residue-characteristic-multiplication-on-a-formal-group)
          - [Formal logarithm](normalization-of-an-algebraic-curve.md#formal-logarithm)
            - [Valuation bound for coefficients of an integral formal logarithm](normalization-of-an-algebraic-curve.md#valuation-bound-for-coefficients-of-an-integral-formal-logarithm)
            - [Deep logarithm subgroup of a formal group](normalization-of-an-algebraic-curve.md#deep-logarithm-subgroup-of-a-formal-group)
              - [Torsion test using a deep formal logarithm subgroup](normalization-of-an-algebraic-curve.md#torsion-test-using-a-deep-formal-logarithm-subgroup)
              - [Topological structure of a formal group on twice the 2-adic integers](normalization-of-an-algebraic-curve.md#topological-structure-of-a-formal-group-on-twice-the-2-adic-integers)
            - [Torsion-freeness of the formal group over Qp for odd p](normalization-of-an-algebraic-curve.md#torsion-freeness-of-the-formal-group-over-qp-for-odd-p)
            - [Formal group exponential](normalization-of-an-algebraic-curve.md#formal-group-exponential)
          - [Formal group of an elliptic curve](normalization-of-an-algebraic-curve.md#formal-group-of-an-elliptic-curve)
            - [Initial coefficients of the elliptic formal group at infinity](normalization-of-an-algebraic-curve.md#initial-coefficients-of-the-elliptic-formal-group-at-infinity)
            - [Formal kernel of a minimal Weierstrass equation](normalization-of-an-algebraic-curve.md#formal-kernel-of-a-minimal-weierstrass-equation)
              - [Two-prime formal-kernel test for nontorsion](normalization-of-an-algebraic-curve.md#two-prime-formal-kernel-test-for-nontorsion)
            - [Torsion-free formal subgroup for a short Weierstrass equation](normalization-of-an-algebraic-curve.md#torsion-free-formal-subgroup-for-a-short-weierstrass-equation)
            - [Formal coordinates on a short Weierstrass curve](normalization-of-an-algebraic-curve.md#formal-coordinates-on-a-short-weierstrass-curve)
            - [Formal-group morphism induced by an isogeny](normalization-of-an-algebraic-curve.md#formal-group-morphism-induced-by-an-isogeny)
            - [Filtration of elliptic-curve points over a local field](normalization-of-an-algebraic-curve.md#filtration-of-elliptic-curve-points-over-a-local-field)
        - [Isogeny of elliptic curves](normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves)
          - [Division point of an elliptic curve](normalization-of-an-algebraic-curve.md#division-point-of-an-elliptic-curve)
          - [Homomorphism group of elliptic curves](normalization-of-an-algebraic-curve.md#homomorphism-group-of-elliptic-curves)
          - [Isogenous elliptic curves can have different rational point groups](normalization-of-an-algebraic-curve.md#isogenous-elliptic-curves-can-have-different-rational-point-groups)
            - [Eight-point isogenous elliptic curves over F5](normalization-of-an-algebraic-curve.md#eight-point-isogenous-elliptic-curves-over-f5)
          - [Endomorphism ring of an elliptic curve](normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve)
          - [Degree of an isogeny](normalization-of-an-algebraic-curve.md#degree-of-an-isogeny)
            - [Positive definiteness of degree on elliptic-curve homomorphisms](normalization-of-an-algebraic-curve.md#positive-definiteness-of-degree-on-elliptic-curve-homomorphisms)
              - [Bilinear degree pairing for elliptic-curve homomorphisms](normalization-of-an-algebraic-curve.md#bilinear-degree-pairing-for-elliptic-curve-homomorphisms)
            - [Quadratic degree recursion for elliptic multiplication](normalization-of-an-algebraic-curve.md#quadratic-degree-recursion-for-elliptic-multiplication)
            - [Divisor proof of the degree parallelogram law](normalization-of-an-algebraic-curve.md#divisor-proof-of-the-degree-parallelogram-law)
            - [Degree of an isogeny from its x-coordinate map](normalization-of-an-algebraic-curve.md#degree-of-an-isogeny-from-its-x-coordinate-map)
          - [Separable isogeny](normalization-of-an-algebraic-curve.md#separable-isogeny)
            - [Differential criterion for separability of an isogeny](normalization-of-an-algebraic-curve.md#differential-criterion-for-separability-of-an-isogeny)
            - [Vélu's formulas](normalization-of-an-algebraic-curve.md#velu-s-formulas)
          - [Kernel of an isogeny](normalization-of-an-algebraic-curve.md#kernel-of-an-isogeny)
          - [Dual isogeny](normalization-of-an-algebraic-curve.md#dual-isogeny)
          - [Trace of an elliptic-curve endomorphism](normalization-of-an-algebraic-curve.md#trace-of-an-elliptic-curve-endomorphism)
            - [Trace of the square of an elliptic-curve endomorphism](normalization-of-an-algebraic-curve.md#trace-of-the-square-of-an-elliptic-curve-endomorphism)
          - [Frobenius isogeny of an elliptic curve](normalization-of-an-algebraic-curve.md#frobenius-isogeny-of-an-elliptic-curve)
            - [Anticommuting Frobenius isogenies give opposite traces](normalization-of-an-algebraic-curve.md#anticommuting-frobenius-isogenies-give-opposite-traces)
            - [Trace of Frobenius](normalization-of-an-algebraic-curve.md#trace-of-frobenius)
              - [Coefficient formula for trace of Frobenius modulo p](normalization-of-an-algebraic-curve.md#coefficient-formula-for-trace-of-frobenius-modulo-p)
            - [Elliptic-curve point count over a finite field](normalization-of-an-algebraic-curve.md#elliptic-curve-point-count-over-a-finite-field)
              - [Frobenius trace recurrence](normalization-of-an-algebraic-curve.md#frobenius-trace-recurrence)
              - [Vanishing trace criterion for a congruent number curve](normalization-of-an-algebraic-curve.md#vanishing-trace-criterion-for-a-congruent-number-curve)
              - [Two generators for elliptic curves over finite fields](normalization-of-an-algebraic-curve.md#two-generators-for-elliptic-curves-over-finite-fields)
              - [Point-count criterion for y squared equals x cubed plus k x](normalization-of-an-algebraic-curve.md#point-count-criterion-for-y-squared-equals-x-cubed-plus-k-x)
              - [Prime-square point-count formula](normalization-of-an-algebraic-curve.md#prime-square-point-count-formula)
              - [Point count for y squared equals x cubed minus x minus one over finite extensions of F3](normalization-of-an-algebraic-curve.md#point-count-for-y-squared-equals-x-cubed-minus-x-minus-one-over-finite-extensions-of-f3)
            - [Hasse's theorem on elliptic curves](normalization-of-an-algebraic-curve.md#hasse-s-theorem-on-elliptic-curves)
              - [Degree-form proof of the Hasse bound](normalization-of-an-algebraic-curve.md#degree-form-proof-of-the-hasse-bound)
              - [Zeta function of an elliptic curve over a finite field](normalization-of-an-algebraic-curve.md#zeta-function-of-an-elliptic-curve-over-a-finite-field)
                - [Riemann hypothesis for an elliptic curve over a finite field](normalization-of-an-algebraic-curve.md#riemann-hypothesis-for-an-elliptic-curve-over-a-finite-field)
        - [Torsion point of an elliptic curve](normalization-of-an-algebraic-curve.md#torsion-point-of-an-elliptic-curve)
          - [Prime-to-characteristic geometric torsion](normalization-of-an-algebraic-curve.md#prime-to-characteristic-geometric-torsion)
          - [Rational torsion in the family x times x plus one times x plus m squared](normalization-of-an-algebraic-curve.md#rational-torsion-in-the-family-x-times-x-plus-one-times-x-plus-m-squared)
          - [Rational torsion on y squared equals x cubed plus positive k x](normalization-of-an-algebraic-curve.md#rational-torsion-on-y-squared-equals-x-cubed-plus-positive-k-x)
          - [2-torsion](normalization-of-an-algebraic-curve.md#2-torsion)
          - [Division polynomials](normalization-of-an-algebraic-curve.md#division-polynomials)
          - [Nagell–Lutz theorem](normalization-of-an-algebraic-curve.md#nagell-lutz-theorem)
            - [Divisibility proof in the Nagell–Lutz theorem](normalization-of-an-algebraic-curve.md#divisibility-proof-in-the-nagell-lutz-theorem)
          - [Division field of an elliptic curve](normalization-of-an-algebraic-curve.md#division-field-of-an-elliptic-curve)
            - [Uniform unramified division field over a local field](normalization-of-an-algebraic-curve.md#uniform-unramified-division-field-over-a-local-field)
            - [Mod-three Galois representation of an elliptic curve](normalization-of-an-algebraic-curve.md#mod-three-galois-representation-of-an-elliptic-curve)
          - [Weil pairing](normalization-of-an-algebraic-curve.md#weil-pairing)
        - [Naive height on the projective line](normalization-of-an-algebraic-curve.md#naive-height-on-the-projective-line)
          - [Height growth under a morphism of the projective line](normalization-of-an-algebraic-curve.md#height-growth-under-a-morphism-of-the-projective-line)
          - [Canonical height of an elliptic curve](normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve)
            - [Height parallelogram identity](normalization-of-an-algebraic-curve.md#height-parallelogram-identity)
              - [Symmetric-square proof of the naive height parallelogram estimate](normalization-of-an-algebraic-curve.md#symmetric-square-proof-of-the-naive-height-parallelogram-estimate)
              - [Biquadratic morphism for elliptic sums and differences](normalization-of-an-algebraic-curve.md#biquadratic-morphism-for-elliptic-sums-and-differences)
            - [Canonical height pairing](normalization-of-an-algebraic-curve.md#canonical-height-pairing)
              - [Rank certificate from rounded canonical heights](normalization-of-an-algebraic-curve.md#rank-certificate-from-rounded-canonical-heights)
            - [Canonical-height lattice-point growth](normalization-of-an-algebraic-curve.md#canonical-height-lattice-point-growth)
            - [Regulator of an elliptic curve](normalization-of-an-algebraic-curve.md#regulator-of-an-elliptic-curve)
        - [Mordell-Weil group](normalization-of-an-algebraic-curve.md#mordell-weil-group)
          - [Mordell-Weil saturation](normalization-of-an-algebraic-curve.md#mordell-weil-saturation)
          - [Rank of an elliptic curve](normalization-of-an-algebraic-curve.md#rank-of-an-elliptic-curve)
          - [Weak Mordell-Weil theorem](normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem)
            - [Kummer-theoretic proof of the weak Mordell-Weil theorem](normalization-of-an-algebraic-curve.md#kummer-theoretic-proof-of-the-weak-mordell-weil-theorem)
              - [Kummer exact sequence of an elliptic curve](normalization-of-an-algebraic-curve.md#kummer-exact-sequence-of-an-elliptic-curve)
                - [Unramified division torsors at good primes](normalization-of-an-algebraic-curve.md#unramified-division-torsors-at-good-primes)
                - [n-Selmer group](normalization-of-an-algebraic-curve.md#n-selmer-group)
                  - [Selmer exact sequence and rank bound](normalization-of-an-algebraic-curve.md#selmer-exact-sequence-and-rank-bound)
                  - [Prime-primary Selmer group of a CM elliptic curve](normalization-of-an-algebraic-curve.md#prime-primary-selmer-group-of-a-cm-elliptic-curve)
                  - [Tate–Shafarevich group](normalization-of-an-algebraic-curve.md#tate-shafarevich-group)
          - [Height descent lemma](normalization-of-an-algebraic-curve.md#height-descent-lemma)
            - [Naive height contraction in elliptic halving descent](normalization-of-an-algebraic-curve.md#naive-height-contraction-in-elliptic-halving-descent)
            - [Canonical-height proof of Mordell-Weil finite generation](normalization-of-an-algebraic-curve.md#canonical-height-proof-of-mordell-weil-finite-generation)
          - [Kummer map of an elliptic curve](normalization-of-an-algebraic-curve.md#kummer-map-of-an-elliptic-curve)
            - [Isogeny Selmer group](normalization-of-an-algebraic-curve.md#isogeny-selmer-group)
              - [Local-to-global gap in isogeny descent](normalization-of-an-algebraic-curve.md#local-to-global-gap-in-isogeny-descent)
            - [Two-torsion square-class homomorphism](normalization-of-an-algebraic-curve.md#two-torsion-square-class-homomorphism)
            - [Two-descent on an elliptic curve](normalization-of-an-algebraic-curve.md#two-descent-on-an-elliptic-curve)
            - [Kummer pairing](normalization-of-an-algebraic-curve.md#kummer-pairing)
              - [Halving cocycle with rational two-torsion](normalization-of-an-algebraic-curve.md#halving-cocycle-with-rational-two-torsion)
                - [Unramified halving fields for a split cubic](normalization-of-an-algebraic-curve.md#unramified-halving-fields-for-a-split-cubic)
                  - [Rational halving quotient bound from root size](normalization-of-an-algebraic-curve.md#rational-halving-quotient-bound-from-root-size)
              - [Finite-extension kernel of a Kummer map](normalization-of-an-algebraic-curve.md#finite-extension-kernel-of-a-kummer-map)
              - [S-unramified power class group](normalization-of-an-algebraic-curve.md#s-unramified-power-class-group)
                - [Finiteness of S-unramified Kummer classes](normalization-of-an-algebraic-curve.md#finiteness-of-s-unramified-kummer-classes)
            - [Two-isogeny descent](normalization-of-an-algebraic-curve.md#two-isogeny-descent)
              - [Rank-zero elliptic curve with roots zero three and four](normalization-of-an-algebraic-curve.md#rank-zero-elliptic-curve-with-roots-zero-three-and-four)
              - [Rank-two elliptic curve with cubic x cubed minus seventeen x](normalization-of-an-algebraic-curve.md#rank-two-elliptic-curve-with-cubic-x-cubed-minus-seventeen-x)
              - [Rank-one elliptic curve with cubic x cubed minus twice x](normalization-of-an-algebraic-curve.md#rank-one-elliptic-curve-with-cubic-x-cubed-minus-twice-x)
              - [Rank-zero elliptic curve with cubic x cubed plus x](normalization-of-an-algebraic-curve.md#rank-zero-elliptic-curve-with-cubic-x-cubed-plus-x)
              - [Rank-one elliptic curve with coefficients eight and minus seven](normalization-of-an-algebraic-curve.md#rank-one-elliptic-curve-with-coefficients-eight-and-minus-seven)
              - [Rank-one elliptic curve with roots zero two and ten](normalization-of-an-algebraic-curve.md#rank-one-elliptic-curve-with-roots-zero-two-and-ten)
              - [Unit square-class bound for two-isogeny descent](normalization-of-an-algebraic-curve.md#unit-square-class-bound-for-two-isogeny-descent)
              - [Two-isogeny index formula over a number field](normalization-of-an-algebraic-curve.md#two-isogeny-index-formula-over-a-number-field)
              - [Two-isogeny formula](normalization-of-an-algebraic-curve.md#two-isogeny-formula)
              - [Prime-support bound in two-isogeny descent](normalization-of-an-algebraic-curve.md#prime-support-bound-in-two-isogeny-descent)
              - [Square-class index formula for two-isogeny descent](normalization-of-an-algebraic-curve.md#square-class-index-formula-for-two-isogeny-descent)
              - [Quartic covering in a two-isogeny descent](normalization-of-an-algebraic-curve.md#quartic-covering-in-a-two-isogeny-descent)
                - [Negative unit obstruction for the fourteen-coefficient isogeny cover](normalization-of-an-algebraic-curve.md#negative-unit-obstruction-for-the-fourteen-coefficient-isogeny-cover)
                - [Modulo-sixteen obstruction for the negative unit descent class](normalization-of-an-algebraic-curve.md#modulo-sixteen-obstruction-for-the-negative-unit-descent-class)
                - [Five-adic obstructions for the congruent-number isogeny covers](normalization-of-an-algebraic-curve.md#five-adic-obstructions-for-the-congruent-number-isogeny-covers)
                - [Five-adic obstruction to square class two on the curve with coefficient one hundred](normalization-of-an-algebraic-curve.md#five-adic-obstruction-to-square-class-two-on-the-curve-with-coefficient-one-hundred)
                - [Signed divisor-two obstruction for an isogeny covering](normalization-of-an-algebraic-curve.md#signed-divisor-two-obstruction-for-an-isogeny-covering)
                - [Modulo-thirty-two obstruction for a congruent-number descent class](normalization-of-an-algebraic-curve.md#modulo-thirty-two-obstruction-for-a-congruent-number-descent-class)
                - [Odd-prime obstructions for the congruent-number isogeny coverings](normalization-of-an-algebraic-curve.md#odd-prime-obstructions-for-the-congruent-number-isogeny-coverings)
                - [Modulo-eight obstruction to a two-isogeny descent class](normalization-of-an-algebraic-curve.md#modulo-eight-obstruction-to-a-two-isogeny-descent-class)
            - [Three-isogeny descent](normalization-of-an-algebraic-curve.md#three-isogeny-descent)
        - [Congruent number elliptic curve](normalization-of-an-algebraic-curve.md#congruent-number-elliptic-curve)
          - [Rank bound for a prime congruent-number elliptic curve](normalization-of-an-algebraic-curve.md#rank-bound-for-a-prime-congruent-number-elliptic-curve)
          - [Rational torsion of a congruent number curve](normalization-of-an-algebraic-curve.md#rational-torsion-of-a-congruent-number-curve)
          - [Congruent number](normalization-of-an-algebraic-curve.md#congruent-number)
            - [Two is not a congruent number](normalization-of-an-algebraic-curve.md#two-is-not-a-congruent-number)
            - [Fermat right triangle theorem](normalization-of-an-algebraic-curve.md#fermat-right-triangle-theorem)
            - [Infinitely many rational right triangles from a nontorsion point](normalization-of-an-algebraic-curve.md#infinitely-many-rational-right-triangles-from-a-nontorsion-point)
            - [Noncongruent primes congruent to three modulo eight](normalization-of-an-algebraic-curve.md#noncongruent-primes-congruent-to-three-modulo-eight)
          - [Mordell-Weil group of the congruent number curve for five](normalization-of-an-algebraic-curve.md#mordell-weil-group-of-the-congruent-number-curve-for-five)
        - [Mordell-Weil group of y squared equals x times x plus one times x plus four](normalization-of-an-algebraic-curve.md#mordell-weil-group-of-y-squared-equals-x-times-x-plus-one-times-x-plus-four)
          - [Euler theorem on four squares in arithmetic progression](normalization-of-an-algebraic-curve.md#euler-theorem-on-four-squares-in-arithmetic-progression)
  - [Normalization of a nodal curve](normalization-of-an-algebraic-curve.md#normalization-of-a-nodal-curve)
    - [Normalization of y squared equals x times x minus one squared](normalization-of-an-algebraic-curve.md#normalization-of-y-squared-equals-x-times-x-minus-one-squared)
- [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)
  - [Riemann-Roch space](#riemann-roch-space)
    - [Rational functions with prescribed poles](#rational-functions-with-prescribed-poles)
  - [Degree of a divisor](#degree-of-a-divisor)
  - [Linear equivalence of divisors](#linear-equivalence-of-divisors)
    - [Divisor class](#divisor-class)
  - [Principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve)
    - [Principality criterion on a complex elliptic curve](#principality-criterion-on-a-complex-elliptic-curve)
    - [Divisor class on the projective line](#divisor-class-on-the-projective-line)
    - [Principal divisor with one simple zero and one simple pole](#principal-divisor-with-one-simple-zero-and-one-simple-pole)
    - [Principal divisor criterion on an elliptic curve](#principal-divisor-criterion-on-an-elliptic-curve)
  - [Riemann-Roch theorem](#riemann-roch-theorem)
    - [Riemann-Roch via elementary modifications](#riemann-roch-via-elementary-modifications)
    - [Cohomological proof of Riemann-Roch for curves](#cohomological-proof-of-riemann-roch-for-curves)
    - [Clifford inequality for curves](#clifford-inequality-for-curves)
    - [Weierstrass gap](#weierstrass-gap)
      - [Weierstrass gap theorem](#weierstrass-gap-theorem)
        - [Genus-two Weierstrass gap sequence](#genus-two-weierstrass-gap-sequence)
    - [Canonical divisor](#canonical-divisor)
      - [Rational differential on an algebraic curve](#rational-differential-on-an-algebraic-curve)
        - [Algebraic residue of a rational differential](#algebraic-residue-of-a-rational-differential)
      - [Valuation of a rational differential](#valuation-of-a-rational-differential)
      - [Canonical Riemann-Roch space](#canonical-riemann-roch-space)
      - [Canonical divisor of the projective line](#canonical-divisor-of-the-projective-line)
      - [Genus of a smooth plane curve](#genus-of-a-smooth-plane-curve)
        - [No smooth plane curve has genus two](#no-smooth-plane-curve-has-genus-two)
        - [Smooth plane quartic](#smooth-plane-quartic)
          - [Projective closure of y cubed equals x to the fourth plus one](#projective-closure-of-y-cubed-equals-x-to-the-fourth-plus-one)
          - [Klein quartic](#klein-quartic)
            - [Plane model y plus x cubed plus xy cubed equals zero of the Klein quartic](#plane-model-y-plus-x-cubed-plus-xy-cubed-equals-zero-of-the-klein-quartic)
            - [Ramification of the x-coordinate on the Klein quartic](#ramification-of-the-x-coordinate-on-the-klein-quartic)
          - [Line section of a smooth plane quartic](#line-section-of-a-smooth-plane-quartic)
          - [Gonality of a smooth plane quartic](#gonality-of-a-smooth-plane-quartic)
      - [Canonical map](#canonical-map)
        - [Canonical genus-four curve as a quadric-cubic intersection](#canonical-genus-four-curve-as-a-quadric-cubic-intersection)
- [Gonality](#gonality)
  - [Trigonal curve](#trigonal-curve)
    - [Canonical scroll of a trigonal curve](#canonical-scroll-of-a-trigonal-curve)
      - [Maroni invariant](#maroni-invariant)
  - [Gonality bound from Riemann-Roch](#gonality-bound-from-riemann-roch)
- [Hyperelliptic curve](#hyperelliptic-curve)
  - [Even-degree hyperelliptic model](#even-degree-hyperelliptic-model)
    - [Compactification of y squared equals x to the eighth minus one](#compactification-of-y-squared-equals-x-to-the-eighth-minus-one)
    - [Canonical divisor of an even-degree hyperelliptic curve](#canonical-divisor-of-an-even-degree-hyperelliptic-curve)
      - [Canonical map of a hyperelliptic curve](#canonical-map-of-a-hyperelliptic-curve)
- [Rational map of projective varieties](#rational-map-of-projective-varieties)
  - [Indeterminacy locus](#indeterminacy-locus)
  - [Projective Cremona transformation](#projective-cremona-transformation)
- [Nonsingular plane cubic](#nonsingular-plane-cubic)
  - [Flex coordinates for a smooth plane cubic](#flex-coordinates-for-a-smooth-plane-cubic)
- [Plane curve](#plane-curve)
  - [Lemniscate of Bernoulli](#lemniscate-of-bernoulli)
  - [Astroid](#astroid)
  - [Plane cusp of type (2,5)](#plane-cusp-of-type-2-5)
    - [Resolution of the (2,5) cusp by two blowups](#resolution-of-the-2-5-cusp-by-two-blowups)
  - [Archimedean spiral](#archimedean-spiral)
  - [Superelliptic curve](#superelliptic-curve)
  - [Canonical map of a smooth plane curve](#canonical-map-of-a-smooth-plane-curve)
  - [Semicubical parabola](#semicubical-parabola)
    - [Coordinate ring and singularity of the semicubical parabola](#coordinate-ring-and-singularity-of-the-semicubical-parabola)
- [Ramification (mathematics)](#ramification-mathematics)
  - [Ramification divisor](#ramification-divisor)
- [Product surface without low-genus curves](#product-surface-without-low-genus-curves)
- [Algebraic surface](#algebraic-surface)
  - [Cubic surface](#cubic-surface)
    - [Smooth cubic surface](#smooth-cubic-surface)
      - [Rational parametrization of a cubic surface from two skew lines](#rational-parametrization-of-a-cubic-surface-from-two-skew-lines)
      - [Conic bundle from a line on a smooth cubic surface](#conic-bundle-from-a-line-on-a-smooth-cubic-surface)
        - [Discriminant quintic of a cubic surface conic bundle](#discriminant-quintic-of-a-cubic-surface-conic-bundle)
      - [Lines through a point of a smooth cubic surface](#lines-through-a-point-of-a-smooth-cubic-surface)
  - [Exceptional curve of a surface resolution](#exceptional-curve-of-a-surface-resolution)
  - [Smooth algebraic surface](#smooth-algebraic-surface)
    - [Arithmetic adjunction formula on a smooth surface](#arithmetic-adjunction-formula-on-a-smooth-surface)
      - [Arithmetic genus drop under a point blowup](#arithmetic-genus-drop-under-a-point-blowup)
    - [Smooth projective surface](#smooth-projective-surface)
      - [Noether–Lefschetz theorem](#noether-lefschetz-theorem)
        - [Very general surface of degree at least four has no smooth rational curve](#very-general-surface-of-degree-at-least-four-has-no-smooth-rational-curve)
      - [Negative curve on a projective surface](#negative-curve-on-a-projective-surface)
        - [Countability of negative curves](#countability-of-negative-curves)
        - [Rigidity of a negative curve](#rigidity-of-a-negative-curve)
      - [Castelnuovo contraction criterion](#castelnuovo-contraction-criterion)
  - [Riemann–Roch theorem for algebraic surfaces](#riemann-roch-theorem-for-algebraic-surfaces)
    - [Noether formula](#noether-formula)
  - [Intersection pairing on the Picard group of a surface](#intersection-pairing-on-the-picard-group-of-a-surface)
    - [Hodge index theorem for algebraic surfaces](#hodge-index-theorem-for-algebraic-surfaces)
      - [Contracted curve has negative self-intersection](#contracted-curve-has-negative-self-intersection)
      - [Isotropic orthogonality consequence of the Hodge index theorem](#isotropic-orthogonality-consequence-of-the-hodge-index-theorem)
    - [Picard lattice of a Hirzebruch surface](#picard-lattice-of-a-hirzebruch-surface)
  - [Intersection formula for blowing up a surface](#intersection-formula-for-blowing-up-a-surface)
    - [Isotropic divisor from a nontrivial birational morphism to the projective plane](#isotropic-divisor-from-a-nontrivial-birational-morphism-to-the-projective-plane)
    - [Self-intersection after blowing up points on a smooth curve](#self-intersection-after-blowing-up-points-on-a-smooth-curve)
  - [Morphism from the projective plane contracting a line](#morphism-from-the-projective-plane-contracting-a-line)
  - [Exceptional curve of the first kind](#exceptional-curve-of-the-first-kind)
    - [Minimal algebraic surface](#minimal-algebraic-surface)
      - [Abelian surface](#abelian-surface)
        - [Ample curve on an abelian surface generates the surface](#ample-curve-on-an-abelian-surface-generates-the-surface)
      - [Minimal Hirzebruch surface](#minimal-hirzebruch-surface)
  - [Elliptic surface](#elliptic-surface)
    - [Elliptic surface of Kodaira dimension minus infinity](#elliptic-surface-of-kodaira-dimension-minus-infinity)
  - [Kodaira dimension](#kodaira-dimension)
    - [Surface of general type](#surface-of-general-type)
      - [Double plane of general type](#double-plane-of-general-type)
  - [Irregularity of an algebraic surface](#irregularity-of-an-algebraic-surface)
    - [Irregularity of a product of curves](#irregularity-of-a-product-of-curves)
    - [Smooth projective hypersurface has zero irregularity](#smooth-projective-hypersurface-has-zero-irregularity)
      - [Product of positive-genus curves is not a projective hypersurface](#product-of-positive-genus-curves-is-not-a-projective-hypersurface)
  - [Geometric genus of an algebraic surface](#geometric-genus-of-an-algebraic-surface)
    - [Birational invariance of the geometric genus of a surface](#birational-invariance-of-the-geometric-genus-of-a-surface)
  - [Albanese variety](#albanese-variety)
    - [Irregularity from a smooth Albanese curve image](#irregularity-from-a-smooth-albanese-curve-image)
- [Projection of a plane curve from an exterior point](#projection-of-a-plane-curve-from-an-exterior-point)
- [Projection from a point on a plane curve](#projection-from-a-point-on-a-plane-curve)
- [Toric geometry](toric-geometry.md)
  - [Lattice in toric geometry](toric-geometry.md#lattice-in-toric-geometry)
    - [Basis of a toric lattice](toric-geometry.md#basis-of-a-toric-lattice)
  - [Toric scheme over a base ring](toric-geometry.md#toric-scheme-over-a-base-ring)
    - [Semistable infinite chain from a toric fan](toric-geometry.md#semistable-infinite-chain-from-a-toric-fan)
      - [Cyclic formal quotient of the infinite toric chain](toric-geometry.md#cyclic-formal-quotient-of-the-infinite-toric-chain)
  - [Algebraic torus](toric-geometry.md#algebraic-torus)
    - [Maximal algebraic torus](toric-geometry.md#maximal-algebraic-torus)
      - [Rational maximal torus](toric-geometry.md#rational-maximal-torus)
        - [Elliptic maximal torus](toric-geometry.md#elliptic-maximal-torus)
    - [Character lattice of an algebraic torus](toric-geometry.md#character-lattice-of-an-algebraic-torus)
      - [Algebraic torus character](toric-geometry.md#algebraic-torus-character)
    - [Cocharacter lattice of an algebraic torus](toric-geometry.md#cocharacter-lattice-of-an-algebraic-torus)
  - [Fan in toric geometry](toric-geometry.md#fan-in-toric-geometry)
    - [Infinite fan in toric geometry](toric-geometry.md#infinite-fan-in-toric-geometry)
    - [Normal fan of a polytope](toric-geometry.md#normal-fan-of-a-polytope)
    - [Cone in toric geometry](toric-geometry.md#cone-in-toric-geometry)
      - [Face of a polyhedral cone](toric-geometry.md#face-of-a-polyhedral-cone)
        - [Ray of a fan](toric-geometry.md#ray-of-a-fan)
      - [Dual cone](toric-geometry.md#dual-cone)
        - [Face duality for polyhedral cones](toric-geometry.md#face-duality-for-polyhedral-cones)
        - [Affine semigroup of a rational cone](toric-geometry.md#affine-semigroup-of-a-rational-cone)
          - [Gordan lemma](toric-geometry.md#gordan-lemma)
          - [Hilbert basis of a rational cone](toric-geometry.md#hilbert-basis-of-a-rational-cone)
      - [Simplicial polyhedral cone](toric-geometry.md#simplicial-polyhedral-cone)
    - [Complete fan](toric-geometry.md#complete-fan)
      - [Star of a cone in a fan](toric-geometry.md#star-of-a-cone-in-a-fan)
      - [Simplex fan](toric-geometry.md#simplex-fan)
    - [Fan subdivision](toric-geometry.md#fan-subdivision)
      - [Star subdivision](toric-geometry.md#star-subdivision)
        - [Toric blowup along an orbit closure](toric-geometry.md#toric-blowup-along-an-orbit-closure)
        - [Toric blowup at a torus-fixed point](toric-geometry.md#toric-blowup-at-a-torus-fixed-point)
          - [Ample divisor after blowing up a torus-fixed point](toric-geometry.md#ample-divisor-after-blowing-up-a-torus-fixed-point)
          - [Blowup of affine space at the origin](toric-geometry.md#blowup-of-affine-space-at-the-origin)
        - [Toric resolution of singularities](toric-geometry.md#toric-resolution-of-singularities)
          - [Two minimal toric resolutions of a four-ray threefold cone](toric-geometry.md#two-minimal-toric-resolutions-of-a-four-ray-threefold-cone)
          - [Multiplicity descent in toric desingularization](toric-geometry.md#multiplicity-descent-in-toric-desingularization)
          - [Hirzebruch–Jung resolution](toric-geometry.md#hirzebruch-jung-resolution)
          - [Self-intersection formula for a toric surface divisor](toric-geometry.md#self-intersection-formula-for-a-toric-surface-divisor)
            - [Toric contraction of a minus-one curve](toric-geometry.md#toric-contraction-of-a-minus-one-curve)
    - [Product fan](toric-geometry.md#product-fan)
    - [Fan of the affine line](toric-geometry.md#fan-of-the-affine-line)
    - [Fan of the projective line](toric-geometry.md#fan-of-the-projective-line)
  - [Toric variety](toric-geometry.md#toric-variety)
    - [Complete three-ray toric surfaces with at most one singular point](toric-geometry.md#complete-three-ray-toric-surfaces-with-at-most-one-singular-point)
    - [Toric surface](toric-geometry.md#toric-surface)
    - [Weighted projective space](toric-geometry.md#weighted-projective-space)
      - [Well-formed weighted projective space](toric-geometry.md#well-formed-weighted-projective-space)
        - [Class-group generator of a well-formed weighted projective space](toric-geometry.md#class-group-generator-of-a-well-formed-weighted-projective-space)
          - [Divisorial section ring of a well-formed weighted projective space](toric-geometry.md#divisorial-section-ring-of-a-well-formed-weighted-projective-space)
      - [Weighted projective plane](toric-geometry.md#weighted-projective-plane)
        - [Divisor class and Picard groups of a weighted projective plane](toric-geometry.md#divisor-class-and-picard-groups-of-a-weighted-projective-plane)
    - [Projective toric variety of a lattice polytope](toric-geometry.md#projective-toric-variety-of-a-lattice-polytope)
    - [Affine toric variety](toric-geometry.md#affine-toric-variety)
      - [Cyclic quotient surface singularity](toric-geometry.md#cyclic-quotient-surface-singularity)
        - [Four-ray completion criterion for a cyclic quotient surface singularity](toric-geometry.md#four-ray-completion-criterion-for-a-cyclic-quotient-surface-singularity)
      - [Dense torus of an affine toric variety](toric-geometry.md#dense-torus-of-an-affine-toric-variety)
      - [Coordinate ring of an affine toric variety](toric-geometry.md#coordinate-ring-of-an-affine-toric-variety)
      - [Diagonal cyclic quotient singularity of order three](toric-geometry.md#diagonal-cyclic-quotient-singularity-of-order-three)
    - [Orbit-cone correspondence](toric-geometry.md#orbit-cone-correspondence)
      - [Monomial support face of a toric point](toric-geometry.md#monomial-support-face-of-a-toric-point)
      - [Complement of an affine toric face chart](toric-geometry.md#complement-of-an-affine-toric-face-chart)
      - [Orbit closure in a toric variety](toric-geometry.md#orbit-closure-in-a-toric-variety)
        - [Monomial zero locus in an affine toric variety](toric-geometry.md#monomial-zero-locus-in-an-affine-toric-variety)
      - [Torus-invariance of the singular locus of a toric variety](toric-geometry.md#torus-invariance-of-the-singular-locus-of-a-toric-variety)
    - [Proper toric variety](toric-geometry.md#proper-toric-variety)
    - [Smoothness criterion for a toric variety](toric-geometry.md#smoothness-criterion-for-a-toric-variety)
    - [Hirzebruch surface](toric-geometry.md#hirzebruch-surface)
      - [Negative section of a Hirzebruch surface](toric-geometry.md#negative-section-of-a-hirzebruch-surface)
      - [Fiber class of a Hirzebruch surface](toric-geometry.md#fiber-class-of-a-hirzebruch-surface)
        - [Multiples of a fiber on the first Hirzebruch surface](toric-geometry.md#multiples-of-a-fiber-on-the-first-hirzebruch-surface)
    - [Toric morphism](toric-geometry.md#toric-morphism)
      - [No nonconstant toric morphism from the projective plane to the product of projective lines](toric-geometry.md#no-nonconstant-toric-morphism-from-the-projective-plane-to-the-product-of-projective-lines)
    - [Rational map of toric varieties from a lattice homomorphism](toric-geometry.md#rational-map-of-toric-varieties-from-a-lattice-homomorphism)
    - [Toric divisor](toric-geometry.md#toric-divisor)
      - [Principal divisor on a toric variety](toric-geometry.md#principal-divisor-on-a-toric-variety)
      - [Toric divisor class sequence](toric-geometry.md#toric-divisor-class-sequence)
      - [Lattice polytope of a toric divisor](toric-geometry.md#lattice-polytope-of-a-toric-divisor)
    - [Cox construction](toric-geometry.md#cox-construction)
      - [Toric irrelevant ideal](toric-geometry.md#toric-irrelevant-ideal)
      - [Cox ring](toric-geometry.md#cox-ring)
      - [Geometric quotient](toric-geometry.md#geometric-quotient)
- [Intersection theory](#intersection-theory)
  - [Intersection dimension bound on a smooth variety](#intersection-dimension-bound-on-a-smooth-variety)
  - [Intersection product of Cartier divisors](#intersection-product-of-cartier-divisors)
    - [Projection formula for algebraic cycles](#projection-formula-for-algebraic-cycles)
  - [Intersection number of a Cartier divisor with a curve](#intersection-number-of-a-cartier-divisor-with-a-curve)
    - [Self-intersection of an algebraic curve](#self-intersection-of-an-algebraic-curve)
  - [Algebraic cycle](#algebraic-cycle)
    - [Rational equivalence](#rational-equivalence)
      - [Chow group](#chow-group)
        - [Chow class](#chow-class)
        - [Cycle class map](#cycle-class-map)
          - [Cycle class](#cycle-class)
        - [Chow ring](#chow-ring)
          - [External product of Chow classes](#external-product-of-chow-classes)
            - [Chow Künneth failure for an elliptic self-product](#chow-kunneth-failure-for-an-elliptic-self-product)
        - [Localization sequence for Chow groups](#localization-sequence-for-chow-groups)
        - [Cellular decomposition of a scheme](#cellular-decomposition-of-a-scheme)
          - [Chow ring of projective space](#chow-ring-of-projective-space)
        - [Projective bundle formula for Chow groups](#projective-bundle-formula-for-chow-groups)
          - [Homotopy invariance of Chow groups](#homotopy-invariance-of-chow-groups)
  - [Chern class](#chern-class)
    - [Chern class axioms in the Chow ring](#chern-class-axioms-in-the-chow-ring)
      - [Chern classes of a smooth hypersurface cotangent bundle](#chern-classes-of-a-smooth-hypersurface-cotangent-bundle)
    - [Todd class](#todd-class)
    - [Chern class in complex cobordism](#chern-class-in-complex-cobordism)
      - [Projective bundle relation in complex cobordism](#projective-bundle-relation-in-complex-cobordism)
    - [Chern number](#chern-number)
    - [Whitney sum formula for Chern classes](#whitney-sum-formula-for-chern-classes)
    - [Projective bundle definition of Chern classes](#projective-bundle-definition-of-chern-classes)
    - [Total Chern class](#total-chern-class)
    - [Euler sequence](#euler-sequence)
      - [Cotangent Euler sequence in homogeneous coordinates](#cotangent-euler-sequence-in-homogeneous-coordinates)
        - [Vanishing of global sections of the once-twisted projective cotangent bundle](#vanishing-of-global-sections-of-the-once-twisted-projective-cotangent-bundle)
  - [Degree of a projective scheme](#degree-of-a-projective-scheme)
  - [Normal bundle](#normal-bundle)
    - [Normal bundle of a smooth plane conic](#normal-bundle-of-a-smooth-plane-conic)
    - [Normal bundle of a linear complex-projective embedding](#normal-bundle-of-a-linear-complex-projective-embedding)
    - [Normal bundle of a transverse intersection](#normal-bundle-of-a-transverse-intersection)
    - [Self-intersection number](#self-intersection-number)
      - [Self-intersection of the diagonal of a curve](#self-intersection-of-the-diagonal-of-a-curve)
    - [Self-intersection formula](#self-intersection-formula)
      - [Euler number equals self-intersection](#euler-number-equals-self-intersection)
    - [Framing of an embedded sphere](#framing-of-an-embedded-sphere)

## GAGA theorem

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

For a projective variety over the complex numbers, analytification gives an equivalence between algebraic and analytic [coherent sheaves](ringed-space.md#coherent-sheaf), preserves their cohomology, and is fully faithful on their morphisms. In particular, a holomorphic isomorphism between algebraic [line bundles](ringed-space.md#line-bundle) is algebraic. This allows a complex-torus proof of a line-bundle identity to establish the corresponding algebraic identity on a projective [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve).

## Very general point of an algebraic parameter space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A property holds at a very general point of an irreducible complex algebraic parameter space if it holds outside a countable union of proper [Zariski-closed subsets](#zariski-closed-set). This permits countably many exceptional conditions. Over $\mathbb C$ that complement is nonempty and dense, for example by the [Baire category theorem](topological-analysis.md#baire-category-theorem) on a local smooth analytic chart.

## Hilbert scheme

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_scheme)

For a projective scheme $X$ and a fixed [Hilbert polynomial](#hilbert-polynomial) $P$, the Hilbert scheme parametrizes flat families of closed subschemes of $X$ with that polynomial. This turns a family of embedded [algebraic curves](#algebraic-curve) into an algebraic parameter space.

### Hilbert functor

↑ **Parent:** [Hilbert scheme](#hilbert-scheme)

For a [projective scheme](ringed-space.md#projective-scheme) $X$ over a [field](algebra.md#field) $k$, the Hilbert functor assigns to a $k$-scheme $T$ the set of closed subschemes $W\subseteq X\times_kT$ which are of finite presentation, proper and flat over $T$. Pullback of families makes it a contravariant [functor](category.md#functor). After choosing a very ample [line bundle](ringed-space.md#line-bundle), requiring a fixed fibre [Hilbert polynomial](#hilbert-polynomial) $P$ gives the subfunctor represented by $\operatorname{Hilb}^P(X)$. The unrestricted functor is represented by the disjoint union of these [Hilbert schemes](#hilbert-scheme).

#### First-order embedded deformation

↑ **Parent:** [Hilbert functor](#hilbert-functor)

A first-order embedded deformation of a [closed subscheme](ringed-space.md#closed-subscheme) $Z\subseteq X$ is a closed subscheme $Z_\varepsilon\subseteq X\times_k\operatorname{Spec}(k[\varepsilon]/(\varepsilon^2))$ flat over the [dual numbers](commutative-algebra.md#dual-number) and with special fibre equal to the given embedded $Z$. It is a tangent vector of the [Hilbert scheme](#hilbert-scheme), not a deformation modulo arbitrary automorphisms of the ambient scheme. These deformations are naturally the [global sections](ringed-space.md#global-section) of the [normal sheaf](ringed-space.md#normal-sheaf).

##### Zariski tangent space of a Hilbert scheme

↑ **Parent:** [First-order embedded deformation](#first-order-embedded-deformation)

For a [closed subscheme](ringed-space.md#closed-subscheme) $Z\subseteq X$ with [ideal sheaf](ringed-space.md#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$, one has $T_{[Z]}\operatorname{Hilb}(X)\cong\operatorname{Hom}_{\mathcal O_X}(\mathcal I,i_*\mathcal O_Z)\cong H^0(Z,\mathcal N_{Z/X})$. Locally a flat deformation ideal $J\subseteq A[\varepsilon]/(\varepsilon^2)$ satisfies $J\cap\varepsilon A=\varepsilon I$. Lifting $f\in I$ to $f+\varepsilon g\in J$ gives a well-defined map $f\mapsto g\bmod I$ killing $I^2$. Conversely the graph condition $g\bmod I=\phi(f)$ defines an ideal with flat quotient by the [flatness criterion over dual numbers](module-theory.md#flatness-criterion-over-dual-numbers). These operations commute with restriction and are inverse, giving the global identification without a smoothness assumption.

### Fano scheme

↑ **Parent:** [Hilbert scheme](#hilbert-scheme)

The closed subscheme of the [Grassmannian](differential-geometry.md#grassmannian) parametrizing projective $k$-planes contained in an embedded projective variety $X$.

#### Fano scheme of lines

↑ **Parent:** [Fano scheme](#fano-scheme)

The [Fano scheme](#fano-scheme) for projective lines. For $X\subseteq\mathbb P^3$, it is a closed subscheme of $\operatorname{Gr}(2,4)$ and hence is projective. Requiring the defining homogeneous polynomials of $X$ to vanish along a line gives its closed defining conditions.

##### Incidence proof that a cubic surface contains a line

↑ **Parent:** [Fano scheme of lines](#fano-scheme-of-lines)

Cubic forms in four variables form $\mathbb P^{19}$. Lines form the four-dimensional [Grassmannian](differential-geometry.md#grassmannian) $G=\operatorname{Gr}(2,4)$. The incidence pairs $(\ell,[F])$ with $F|_\ell=0$ form a projective-space bundle with fibre $\mathbb P^{15}$ over $G$, since restriction to a line imposes four independent linear conditions. Hence the incidence variety is irreducible of dimension 19. For $F=x_0^2x_2+x_1^2x_3$, a nearby line written $x_2=a_0x_0+a_1x_1$, $x_3=b_0x_0+b_1x_1$ lies on $F$ precisely when all four parameters vanish. This is an isolated point of that fibre. The [fiber dimension theorem](#fiber-dimension-theorem) forces the image to have dimension 19, and projectivity makes the image closed. It is therefore all of $\mathbb P^{19}$, proving geometric existence over an [algebraically closed field](algebra.md#algebraically-closed-field).

###### Cubic surface line incidence variety

↑ **Parent:** [Incidence proof that a cubic surface contains a line](#incidence-proof-that-a-cubic-surface-contains-a-line)

A [projective bundle](fiber-bundle.md#projective-bundle) with fibre $\mathbb P^{15}$ over the four-dimensional [Grassmannian](differential-geometry.md#grassmannian) $\operatorname{Gr}(2,4)$. The condition of containing a fixed line imposes four independent linear conditions on the twenty cubic coefficients. The projection to $\mathbb P^{19}$ is proper. The line $\{x_2=x_3=0\}$ is an isolated point over $x_0^2x_2+x_1^2x_3$; [isolated fibre point forces dominance in equal dimensions](#isolated-fibre-point-forces-dominance-in-equal-dimensions) then proves that every cubic surface contains a line.

##### Finiteness of lines on a smooth surface of degree at least three

↑ **Parent:** [Fano scheme of lines](#fano-scheme-of-lines)

For a line $L$ on a degree-$d$ smooth surface in $\mathbb P^3$, the [adjunction formula](complex-geometry.md#adjunction-formula) gives $L^2=2-d$. If $d\geq3$, all lines are [negative curves](#negative-curve-on-a-projective-surface), hence there are only countably many by [countability of negative curves](#countability-of-negative-curves). Their projective [Fano scheme of lines](#fano-scheme-of-lines) cannot have a positive-dimensional complex component, since such a component has uncountably many points. A zero-dimensional projective scheme of finite type has finitely many points, proving the assertion.

<h2 id="etale-cohomology">Étale cohomology</h2>

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Étale_cohomology)

Étale cohomology is [sheaf cohomology](ringed-space.md#sheaf-cohomology) on the site whose objects are [étale morphisms](ringed-space.md#etale-morphism) $Y\to X$ and whose coverings are jointly surjective families of such morphisms. It provides cohomological invariants for [algebraic varieties](#algebraic-variety) over fields of positive characteristic. In [Deligne-Lusztig theory](lie-theory.md#deligne-lusztig-theory), compactly supported groups with $\ell$-adic coefficients, for $\ell$ different from the field characteristic, give finite-dimensional representations of the finite groups acting on the varieties.

## Algebraic set

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

An algebraic set is a zero locus of polynomial equations, allowing reducible sets. An [affine algebraic set](#affine-algebraic-set) uses ordinary polynomial equations; a projective algebraic set uses homogeneous equations in projective coordinates. On affine or projective space, closed sets in the [Zariski topology](#zariski-topology) are algebraic sets, and an irreducible algebraic set is an [algebraic variety](#algebraic-variety) in the classical convention.

## Complex multiplication

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_multiplication)

An [abelian variety](abelian-variety.md) of dimension $g$ has complex multiplication when its rational [endomorphism ring](module-theory.md#endomorphism-ring) contains a commutative semisimple $\mathbb Q$-algebra of dimension $2g$. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) in characteristic zero, this means its geometric [endomorphism ring of an elliptic curve](normalization-of-an-algebraic-curve.md#endomorphism-ring-of-an-elliptic-curve) is an order in an [imaginary quadratic field](algebraic-number-theory.md#imaginary-quadratic-field). The resulting rank-one [Tate module](representation-theory.md#tate-module) representations connect torsion points to [class field theory](algebraic-number-theory.md#class-field-theory).

### CM period

↑ **Parent:** [Complex multiplication](#complex-multiplication)

A complex CM period compares an algebraic invariant differential on a [CM elliptic curve](#cm-elliptic-curve) with its analytic lattice coordinate. At an ordinary prime, a $p$-adic CM period compares the same differential with the invariant differential of the multiplicative formal group: an isomorphism $\eta$ is normalized by $\log_{\widehat E}\eta(T)=\Omega_p\log(1+T)$. Matched periods make normalized critical [Hecke L-function](analytic-number-theory.md#hecke-l-function) values algebraic and give precise [p-adic L-function](analytic-number-theory.md#p-adic-l-function) interpolation.

### CM reciprocity theorem

↑ **Parent:** [Complex multiplication](#complex-multiplication)

For a complex CM torus $\mathbb C/\mathfrak a$ and an idele $s$ of its CM field, the automorphism corresponding to $s$ by [Artin reciprocity](algebraic-number-theory.md#artin-reciprocity-law) takes its lattice to $s^{-1}\mathfrak a$ and acts on torsion through the adelic scalar $s^{-1}$. When the curve is defined over a larger field, use the idelic norm to the CM field. Comparison with the original curve gives a scalar in the CM field, producing the [Hecke character of a CM elliptic curve](algebraic-number-theory.md#hecke-character-of-a-cm-elliptic-curve).

### CM elliptic curve

↑ **Parent:** [Complex multiplication](#complex-multiplication)

An [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) with [complex multiplication](#complex-multiplication) is called a CM elliptic curve. Distinguish geometric [endomorphisms](algebra.md#endomorphism) from [endomorphisms](algebra.md#endomorphism) defined over the base [field](algebra.md#field). In characteristic zero, adjoining the [imaginary quadratic field](algebraic-number-theory.md#imaginary-quadratic-field) selected by the tangent action makes all geometric [endomorphisms](algebra.md#endomorphism) defined over the base. Good split primes have [ordinary reduction](normalization-of-an-algebraic-curve.md#ordinary-reduction-of-an-elliptic-curve); good inert primes have [supersingular reduction](normalization-of-an-algebraic-curve.md#supersingular-reduction-of-an-elliptic-curve).

## Birational geometry

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birational_geometry)

### Blowing up (algebraic geometry)

↑ **Parent:** [Birational geometry](#birational-geometry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Blowing_up)

The [projective morphism](ringed-space.md#projective-morphism) $\operatorname{Proj}_X\bigoplus_{j\ge0}\mathcal I^j\to X$ associated to the powers of the ideal sheaf of a closed centre. Off that centre it is an [isomorphism](algebra.md#isomorphism). Blowing up a smooth point of an $n$-dimensional smooth variety replaces the point by a [projective space](projective-space.md) $\mathbb P^{n-1}$, the [algebraic exceptional divisor](#algebraic-exceptional-divisor).

#### Strict transform of an algebraic subvariety

↑ **Parent:** [Blowing up (algebraic geometry)](#blowing-up-algebraic-geometry)

For a [blowup of an algebraic variety](#blowing-up-algebraic-geometry) $\pi:\widetilde X\to X$ with centre $Z$, the [strict transform of an algebraic subvariety](#strict-transform-of-an-algebraic-subvariety) of a subvariety $Y$ not contained in $Z$ is the closure of $\pi^{-1}(Y\setminus Z)$. It excludes components supported entirely in the [algebraic exceptional divisor](#algebraic-exceptional-divisor).

#### Algebraic exceptional divisor

↑ **Parent:** [Blowing up (algebraic geometry)](#blowing-up-algebraic-geometry)

The divisor contracted by a [blowup of an algebraic variety](#blowing-up-algebraic-geometry) to its centre. For the blowup of a smooth point on an $n$-dimensional smooth variety it is $\mathbb P^{n-1}$. Being a closed projective subvariety of positive dimension, it can obstruct affineness of a fibre containing it.

## Zariski topology

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zariski_topology)

The Zariski topology on an affine scheme $\operatorname{Spec}A$ has closed sets $V(I)=\{\mathfrak p:I\subseteq\mathfrak p\}$ for ideals $I\subseteq A$. Its basic open sets are the [principal open subschemes](ringed-space.md#principal-open-subscheme) $D(f)$.

### Zariski dense subset

↑ **Parent:** [Zariski topology](#zariski-topology)

A subset of an algebraic variety is Zariski dense when its closure in the [Zariski topology](#zariski-topology) is the whole variety. For an affine variety, this is equivalent to saying that every regular function vanishing on the subset vanishes on the entire variety.

## Presheaf of sets on a topological space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A presheaf of sets on a [topological space](topology.md#topological-space) $X$ is a contravariant functor from the inclusion-ordered category $\mathcal O(X)$ of open subsets to $\mathbf{Set}$. Its maps $F(U)\to F(V)$ for $V\subseteq U$ are restriction maps.

### Constant presheaf of sets

↑ **Parent:** [Presheaf of sets on a topological space](#presheaf-of-sets-on-a-topological-space)

Every restriction is the identity. Its stalk at each point is $T$, and its [étale space of a presheaf](#etale-space-of-a-presheaf) is $X\times T$ with $T$ discrete. It is generally not a sheaf; in particular its value on the empty open set is $T$. Its [sheafification](ringed-space.md#sheafification) is the [constant sheaf of sets](#constant-sheaf-of-sets).

### Morphism of presheaves

↑ **Parent:** [Presheaf of sets on a topological space](#presheaf-of-sets-on-a-topological-space)

A [natural transformation](category.md#natural-transformation) between [presheaves](#presheaf-of-sets-on-a-topological-space) assigns maps $F(U)\to G(U)$ commuting with every restriction. For [presheaves](#presheaf-of-sets-on-a-topological-space) of abelian groups or [modules](module-theory.md#module-mathematics), those maps preserve the specified algebraic structure.

### Sheaf (mathematics)

↑ **Parent:** [Presheaf of sets on a topological space](#presheaf-of-sets-on-a-topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sheaf_(mathematics))

A sheaf of sets is a presheaf in which compatible sections on any open cover glue to one unique section on the union.

A sheaf may additionally carry [abelian group](group.md#abelian-group) or [module](module-theory.md#module-mathematics) structure on its sections, with restriction and gluing preserving that structure. The underlying [sheaf of sets](#sheaf-mathematics) retains the same local-to-global axiom.

#### Skyscraper sheaf of sets

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

For inclusion of a point $i:\{x\}\to X$, this is the direct-image sheaf of a set. It is [right adjoint](category.md#adjoint-functors) to the [stalk functor](ringed-space.md#stalk-functor-for-presheaves-of-sets). It uses the singleton terminal set on opens omitting $x$, rather than the zero [group](group.md) used for abelian-group skyscraper sheaves.

<h4 id="etale-space-of-a-presheaf">Étale space of a presheaf</h4>

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

The space of [germs](ringed-space.md#germ-of-a-sheaf-section) of a presheaf has basic opens given by the germs of one section over an open set. Projection to its base point is a local homeomorphism. Continuous sections of this projection give [sheafification](ringed-space.md#sheafification). For the [constant presheaf of sets](#constant-presheaf-of-sets), the basic opens are $U\times\{t\}$, giving the ordinary product with a discrete fibre.

#### Constant sheaf of sets

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

The sections are [locally constant functions](calculus.md#locally-constant-function) into a discrete set $T$, with ordinary restriction. It is the [sheafification](ringed-space.md#sheafification) of the [constant presheaf of sets](#constant-presheaf-of-sets). Its value on an empty open set is a singleton, even if $T$ is empty. For a topological space, this construction is [left adjoint](category.md#adjoint-functors) to the [global sections functor](category-theory.md#global-sections-functor): a map from it to a sheaf is a family of global sections indexed by $T$.

#### Morphism of sheaves

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

A morphism of [sheaves](#sheaf-mathematics) assigns a map $\mathcal F(U)\to\mathcal G(U)$ on every [open set](topology.md#open-set), commuting with all restriction maps. For [sheaves of abelian groups](#sheaf-of-abelian-groups), [sheaves of rings](ringed-space.md#sheaf-of-rings) or [sheaves of modules](ringed-space.md#sheaf-of-modules), the maps must also preserve the relevant algebraic structure. It induces maps on every [stalk](ringed-space.md#stalk-of-a-sheaf), and equality of sheaf morphisms can be checked there.

##### Cokernel sheaf

↑ **Parent:** [Morphism of sheaves](#morphism-of-sheaves)

For a [morphism of sheaves](#morphism-of-sheaves) $\phi:\mathcal F\to\mathcal G$ of abelian groups or modules, the cokernel sheaf is the [sheafification](ringed-space.md#sheafification) of the [presheaf](#presheaf-of-sets-on-a-topological-space) $U\mapsto\mathcal G(U)/\phi(\mathcal F(U))$. Its [stalk](ringed-space.md#stalk-of-a-sheaf) at $x$ is $\operatorname{coker}(\mathcal F_x\to\mathcal G_x)$. The presheaf quotient itself need not satisfy the [sheaf gluing axiom](#sheaf-gluing-axiom), which explains why a surjective [morphism of sheaves](#morphism-of-sheaves) need not be surjective on [global sections](ringed-space.md#global-section).

##### f-morphism of sheaves

↑ **Parent:** [Morphism of sheaves](#morphism-of-sheaves)

For a continuous map $f:X\to Y$, an f-morphism from a [sheaf](#sheaf-mathematics) on $Y$ to a [sheaf](#sheaf-mathematics) on $X$ is a family of the displayed maps commuting with restrictions. It is equivalently a [morphism of sheaves](#morphism-of-sheaves) $\mathcal G\to f_*\mathcal F$. For each $x\in X$ it induces a map $\mathcal G_{f(x)}\to\mathcal F_x$ on [stalks](ringed-space.md#stalk-of-a-sheaf), by pulling back the neighbourhood representing a [germ](ringed-space.md#germ-of-a-sheaf-section).

##### Surjective morphism of sheaves

↑ **Parent:** [Morphism of sheaves](#morphism-of-sheaves)

A morphism of [sheaves of modules](ringed-space.md#sheaf-of-modules) is surjective when the induced map on every [stalk](ringed-space.md#stalk-of-a-sheaf) is onto. Equivalently every target section can locally be lifted. It need not be onto on [global sections](ringed-space.md#global-section); the [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology) describes that obstruction.

##### Kernel sheaf

↑ **Parent:** [Morphism of sheaves](#morphism-of-sheaves)

For a [morphism of sheaves](#morphism-of-sheaves) of abelian groups or modules, the kernel sheaf has sections $\ker(\mathcal F(U)\to\mathcal G(U))$. These already satisfy the [sheaf gluing axiom](#sheaf-gluing-axiom). Its [stalk](ringed-space.md#stalk-of-a-sheaf) at $x$ is the kernel of $\mathcal F_x\to\mathcal G_x$, since filtered colimits of modules preserve exactness. A sheaf morphism is injective exactly when its kernel sheaf is zero.

#### Sheaf of abelian groups

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

A sheaf of abelian groups is a [sheaf of sets](#sheaf-mathematics) whose sections on each open set form an [abelian group](group.md#abelian-group) and whose restriction maps are group homomorphisms. Its [stalk of a sheaf](ringed-space.md#stalk-of-a-sheaf) is the corresponding group of germs. Kernels are computed on sections, whereas cokernels are obtained by [sheafification](ringed-space.md#sheafification) of the sectionwise cokernel. An [exact sequence](homology.md#exact-sequence) can therefore be checked on stalks.

##### Direct sum of sheaves

↑ **Parent:** [Sheaf of abelian groups](#sheaf-of-abelian-groups)

The direct sum of sheaves of abelian groups is the sheafification of the presheaf $U\mapsto\bigoplus_i\mathcal F_i(U)$. It need not equal that presheaf: sections are locally represented using finitely many summands, while globally infinitely many can occur. For point-supported [skyscraper sheaves](ringed-space.md#skyscraper-sheaf) at closed points, allowable point supports are a [locally finite family of subsets](topology.md#locally-finite-family-of-subsets).

##### Injective sheaf

↑ **Parent:** [Sheaf of abelian groups](#sheaf-of-abelian-groups)

A sheaf of abelian groups is injective if every morphism to it from a subsheaf extends to the containing sheaf. Every such sheaf embeds in an injective sheaf. Injective sheaves are [flasque](ringed-space.md#flasque-sheaf): the inclusion of [extension by zero](ringed-space.md#extension-by-zero) constant-integer sheaves associated to $U\subseteq V$ turns the extension property into surjectivity of restriction from $V$ to $U$.

##### Exact sequence of sheaves

↑ **Parent:** [Sheaf of abelian groups](#sheaf-of-abelian-groups)

An [exact sequence](homology.md#exact-sequence) of [sheaves of abelian groups](#sheaf-of-abelian-groups) is a sequence of sheaf homomorphisms for which the image of each map equals the kernel of the next. Exactness can be checked on every [stalk of a sheaf](ringed-space.md#stalk-of-a-sheaf). Exactness of the associated sequences of sections on every open set is a stronger condition: a surjective sheaf homomorphism need only admit lifts locally.

###### Short exact sequence of sheaves

↑ **Parent:** [Exact sequence of sheaves](#exact-sequence-of-sheaves)

A sequence $0\to\mathcal F'\to\mathcal F\to\mathcal F''\to0$ of sheaves is exact exactly when the induced sequence on every stalk is exact.

##### Constant sheaf

↑ **Parent:** [Sheaf of abelian groups](#sheaf-of-abelian-groups)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constant_sheaf)

For an abelian group $A$, the constant sheaf has sections over an open set given by its locally constant $A$-valued functions. It is the sheafification of the constant presheaf, and its sections on a disconnected open set need not have a single common value.

###### Constant sheaves on irreducible spaces are flasque

↑ **Parent:** [Constant sheaf](#constant-sheaf)

Every nonempty open subset of an irreducible space is connected. A locally constant function into a fixed abelian group $D$ is therefore constant on that open set. Restrictions between nonempty opens identify with the identity of $D$, and restrictions to the empty set are surjective onto zero. Thus the constant sheaf is flasque, with global sections $D$ and zero higher sheaf cohomology on a nonempty irreducible space. For an integral scheme its constant function-field sheaf has its natural structure-sheaf action by regular functions viewed in the function field.

#### Sheaf gluing axiom

↑ **Parent:** [Sheaf (mathematics)](#sheaf-mathematics)

The sheaf gluing axiom says that sections $s_i$ on an [open cover](topology.md#open-cover) $(U_i)$ that agree on every overlap $U_i\cap U_j$ glue to a unique section on $\bigcup_iU_i$.

## Ringed space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

[This section is present in another page, follow this link to view it.](ringed-space.md)

## Weil divisor

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weil_divisor)

A Weil divisor on a Noetherian integral scheme is a finite integer combination of integral codimension-one closed subschemes.

### Q-Cartier divisor

↑ **Parent:** [Weil divisor](#weil-divisor)

A [Weil divisor](#weil-divisor) is Q-Cartier if some positive integer multiple is a [Cartier divisor](cartier-divisor.md). Its Cartier index is the smallest such integer. It is ample in the Q-Cartier sense when such a multiple is an [ample Cartier divisor](cartier-divisor.md#ample-cartier-divisor). This need not make the original divisor itself Cartier.

### Linear system of divisors

↑ **Parent:** [Weil divisor](#weil-divisor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_system_of_divisors)

A [linear system of divisors](#linear-system-of-divisors) is a projective family of effective [Weil divisors](#weil-divisor) linearly equivalent to a fixed divisor. A [complete linear system of a divisor](cartier-divisor.md#complete-linear-system-of-a-divisor) contains every effective representative of that class; a projective subspace gives a subsystem. For a [Cartier divisor](cartier-divisor.md), the family is obtained from global sections of its associated [line bundle](ringed-space.md#line-bundle). The [algebraic curve](#algebraic-curve) case recovers the usual moving family of effective divisors.

#### Bertini smoothness theorem

↑ **Parent:** [Linear system of divisors](#linear-system-of-divisors)

On a smooth variety over a field of characteristic zero, a general member of a basepoint-free [linear system of divisors](#linear-system-of-divisors) is smooth. More generally it is smooth outside the base locus. Irreducibility is a separate assertion and requires suitable hypotheses on the associated morphism; a pencil composed with a map to a curve can have disconnected general divisors.

#### Genus-two quartic from a degree-four complete linear system

↑ **Parent:** [Linear system of divisors](#linear-system-of-divisors)

On a smooth projective curve of genus two, $D=K+P+Q$ has three sections and no base points by the [Riemann-Roch theorem](#riemann-roch-theorem). Its map to $\mathbb P^2$ is nondegenerate and has mapping degree times image degree four. The only nonbirational possibility is a double cover of a conic. Every degree-two divisor with two sections is canonical, again by [Riemann-Roch theorem](#riemann-roch-theorem), so that possibility forces $D\sim2K$, or $P+Q\sim K$. If this equivalence fails, the image is a quartic and the map is birational. The quartic is singular because a smooth plane quartic has genus three.

#### Base-point-free linear system

↑ **Parent:** [Linear system of divisors](#linear-system-of-divisors)

A linear system is base-point-free if its sections have no common zero. Their ratios then define an everywhere-defined morphism to projective space whose hyperplane pullbacks are members of the original system.

##### Very ample linear system

↑ **Parent:** [Base-point-free linear system](#base-point-free-linear-system)

A very ample linear system defines an embedding into projective space. On a smooth projective curve this means it has no base points and separates both distinct points and tangent directions; the complete system of a [very ample divisor](cartier-divisor.md#very-ample-divisor) is an example.

###### Length-two criterion for a very ample linear system

↑ **Parent:** [Very ample linear system](#very-ample-linear-system)

For a finite generating space $V\subseteq H^0(X,\mathcal L)$ on a projective scheme, its map to [projective space](projective-space.md) is a [closed immersion](ringed-space.md#closed-immersion) exactly when, after algebraic closure of the ground field, the displayed evaluation is surjective for every length-two [closed subscheme](ringed-space.md#closed-subscheme) $E$. Two distinct points test point separation; a double point tests a direction in the [Zariski tangent space](#zariski-tangent-space). For the complete section space, this characterizes a [very ample line bundle](ringed-space.md#very-ample-line-bundle).

### Support of a Weil divisor

↑ **Parent:** [Weil divisor](#weil-divisor)

For $D=\sum_P a_PP$, its support is the union of the prime divisors $P$ with $a_P\ne0$. Negative as well as positive coefficients contribute. A point outside the support has a neighbourhood on which the divisor is zero.

### Linear equivalence of Weil divisors

↑ **Parent:** [Weil divisor](#weil-divisor)

Two [Weil divisors](#weil-divisor) are linearly equivalent when their difference is a [principal Weil divisor](#principal-weil-divisor). This is the equivalence relation defining the [divisor class group](#divisor-class-group), and applies to normal varieties of any dimension, not just curves.

#### Unavoidable support at a non-Cartier point

↑ **Parent:** [Linear equivalence of Weil divisors](#linear-equivalence-of-weil-divisors)

If a [Weil divisor](#weil-divisor) $D$ on a [normal variety](ringed-space.md#normal-variety) is not Cartier at $x$, every linearly equivalent divisor has $x$ in its [support of a Weil divisor](#support-of-a-weil-divisor). Otherwise that representative would vanish near $x$, expressing $D$ as a [principal Weil divisor](#principal-weil-divisor) there. On $V(ac-b^2)$ the prime divisor $V(a,b)$ is not Cartier at the origin: its ideal has two independent generators modulo the [maximal ideal](commutative-algebra.md#maximal-ideal) times that ideal. This gives an unavoidable support point even for representatives with negative coefficients.

### Divisorial ideal

↑ **Parent:** [Weil divisor](#weil-divisor)

For a [normal variety](ringed-space.md#normal-variety) with affine [coordinate ring](#coordinate-ring) $A$ and a [Weil divisor](#weil-divisor) $D$, the fractional ideal of functions whose principal [Weil divisor](#weil-divisor) is at least $D$ is

$$
I_D=\{q\in\operatorname{Frac}(A):\operatorname{ord}_P(q)\ge\operatorname{coeff}_P D\text{ for all prime divisors }P\}\cup\{0\}.
$$

For an effective prime divisor this is its height-one [prime ideal](commutative-algebra.md#prime-ideal). If the divisor is Cartier locally, this ideal is locally principal. A nonprincipal height-one [prime ideal](commutative-algebra.md#prime-ideal) in a normal [local ring](commutative-algebra.md#local-ring) can therefore detect a non-Cartier divisor.

### Principal Weil divisor

↑ **Parent:** [Weil divisor](#weil-divisor)

On a normal integral Noetherian scheme, a nonzero rational function defines the displayed [Weil divisor](#weil-divisor), with the sum over codimension-one prime divisors. The [local ring](commutative-algebra.md#local-ring) at each such divisor is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), so the order is well defined. The [divisor class group](#divisor-class-group) is the group of [Weil divisors](#weil-divisor) modulo principal Weil divisors. On a smooth curve this agrees with a [principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve).

### Prime Weil divisor

↑ **Parent:** [Weil divisor](#weil-divisor)

A prime Weil divisor is one integral codimension-one closed subscheme. At its generic point, regularity in codimension one supplies a discrete valuation and hence an order of vanishing.

### Divisor class group

↑ **Parent:** [Weil divisor](#weil-divisor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisor_class_group)

The divisor class group is the group of Weil divisors modulo principal divisors of rational functions.

#### Divisor class groups of products of projective spaces

↑ **Parent:** [Divisor class group](#divisor-class-group)

For positive $n,m$, $\operatorname{Cl}(\mathbb P^n\times\mathbb P^m)=\mathbb Z^2$, generated freely by the pullbacks of coordinate hyperplanes. Restrict a divisor to the standard affine chart, where [unique factorization](algebra.md#unique-factorization-in-an-integral-domain) makes it principal, and subtract this [principal Weil divisor](#principal-weil-divisor) to leave only the two boundary hyperplanes. Any principal relation between them would be given by a rational function whose divisor vanishes on the chart; [unique factorization](algebra.md#unique-factorization-in-an-integral-domain) then makes that function a constant, proving independence. The same argument gives $\operatorname{Cl}(\mathbb P^r)=\mathbb Z$.

#### Divisor class group of a plane-curve complement

↑ **Parent:** [Divisor class group](#divisor-class-group)

If $C$ is an irreducible plane curve of degree $d$, the [localization sequence for the divisor class group](#localization-sequence-for-the-divisor-class-group) quotients $\operatorname{Cl}(\mathbb P^2)=\mathbb Z[H]$ by the class $[C]=d[H]$. Nonsingularity of the removed curve is not required; irreducibility makes it a single removed [prime Weil divisor](#prime-weil-divisor).

#### Divisor class group and Picard group of a smooth curve

↑ **Parent:** [Divisor class group](#divisor-class-group)

For a smooth irreducible [algebraic curve](#algebraic-curve), send a [divisor on an algebraic curve](#divisor-on-an-algebraic-curve) $D=\sum_P n_PP$ to the [line bundle associated to a divisor](cartier-divisor.md#line-bundle-associated-to-a-divisor) defined locally by $\mathcal O_X(D)_P=t_P^{-n_P}\mathcal O_{X,P}$. A nonzero rational section of a [line bundle](ringed-space.md#line-bundle) gives its inverse construction, and changing that section changes its divisor by a [principal divisor](#principal-divisor-on-an-algebraic-curve). Thus the [divisor class group](#divisor-class-group) is the [Picard group](ringed-space.md#picard-group). The quotient of the [sheaf of nonzero rational functions on an irreducible variety](#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety) by the [sheaf of units of the structure sheaf](ringed-space.md#sheaf-of-units-of-the-structure-sheaf) has stalk $\mathbb Z$ at each closed point, via the [discrete valuation](commutative-algebra.md#discrete-valuation). Its global sections are finite sums of points. The corresponding [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology), and the vanishing for the rational-function sheaf, identify both groups with $H^1(X,\mathcal O_X^*)$.

##### Nonfinite generation of elliptic-curve divisor class groups

↑ **Parent:** [Divisor class group and Picard group of a smooth curve](#divisor-class-group-and-picard-group-of-a-smooth-curve)

For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) over an [algebraically closed field](algebra.md#algebraically-closed-field), $\operatorname{Pic}^0(E)\cong E(k)$ via $P\mapsto[P-O]$. This group is infinite and divisible by any prime $\ell$ different from the characteristic, since $[\ell]:E\to E$ has nonzero derivative and is a surjective morphism of projective curves. A [finitely generated abelian group](group.md#finitely-generated-abelian-group) divisible by $\ell$ has zero free rank and is finite. Hence $E(k)$, and therefore $\operatorname{Cl}(E)$, cannot be finitely generated. This proof applies to countable algebraically closed fields as well.

#### Divisor-class criterion for unique factorization

↑ **Parent:** [Divisor class group](#divisor-class-group)

A [Noetherian ring](algebra.md#noetherian-ring) that is an [integrally closed domain](commutative-algebra.md#integrally-closed-domain) is a [unique factorization domain](algebra.md#unique-factorization-domain) exactly when its [divisor class group](#divisor-class-group) vanishes. Indeed, vanishing says every [prime Weil divisor](#prime-weil-divisor), equivalently every height-one prime ideal, is principal.

#### Localization sequence for the divisor class group

↑ **Parent:** [Divisor class group](#divisor-class-group)

Let $X$ be a Noetherian integral scheme that is regular in codimension one, and let $U=X\setminus\bigcup_{j=1}^r Z_j$, where the $Z_j$ are the codimension-one irreducible components of the complement. Restriction gives an exact sequence

$$
\bigoplus_{j=1}^r\mathbb Z[Z_j]\longrightarrow\operatorname{Cl}(X)\longrightarrow\operatorname{Cl}(U)\longrightarrow0.
$$

##### Nagata theorem for divisor class groups

↑ **Parent:** [Localization sequence for the divisor class group](#localization-sequence-for-the-divisor-class-group)

If $A$ is a Noetherian normal domain and $S$ is a multiplicative set, then $\operatorname{Cl}(S^{-1}A)$ is the quotient of $\operatorname{Cl}(A)$ by the classes of height-one primes meeting $S$. Tracking the units of $S^{-1}A$ determines the relations among those prime divisors.

###### Divisor class group of the three-dimensional affine quadric cone

↑ **Parent:** [Nagata theorem for divisor class groups](#nagata-theorem-for-divisor-class-groups)

For the three-dimensional affine quadric cone

$$
X=\operatorname{Spec}k[x,y,z,w]/(xy-zw),
$$

the [divisor class group](#divisor-class-group) is infinite cyclic. A generator is either ruling plane $V(x,z)$ or $V(x,w)$, and the [principal divisor](#principal-divisor-on-an-algebraic-curve) of $x$ gives the relation $[V(x,z)]+[V(x,w)]=0$.

##### Divisor class group of a projective-space bundle with trivial vector bundle

↑ **Parent:** [Localization sequence for the divisor class group](#localization-sequence-for-the-divisor-class-group)

For a Noetherian integral scheme $X$ that is regular in codimension one,

$$
\operatorname{Cl}(X\times\mathbb P^n)\cong\operatorname{Cl}(X)\oplus\mathbb Z[H],
$$

where $H=X\times\mathbb P^{n-1}$ is a [hyperplane divisor](cartier-divisor.md#hyperplane-divisor). Restriction to $X\times\mathbb A^n$ gives the first summand, while restriction to the generic projective-space fiber detects the coefficient of $H$.

#### Divisor class group of an A-type surface singularity

↑ **Parent:** [Divisor class group](#divisor-class-group)

For $n\geq2$, the normal affine surface

$$
X_n=\operatorname{Spec}k[x,y,z]/(xy-z^n)
$$

has $\operatorname{Cl}(X_n)\cong\mathbb Z/n\mathbb Z$. The class of the prime divisor $D=V(x,z)$ generates: localization at $x$ is a unique factorization domain, so the divisor-class localization sequence leaves only $D$, while $\operatorname{div}(x)=nD$ gives its exact order.

## Cartier divisor

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

[This section is present in another page, follow this link to view it.](cartier-divisor.md)

## Algebraic variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_variety)

An algebraic variety is a geometric space locally described by polynomial equations, together with its regular functions.

### Rational map of algebraic varieties

↑ **Parent:** [Algebraic variety](#algebraic-variety)

A rational map is a [morphism of algebraic varieties](#morphism-of-algebraic-varieties) defined on a dense [open subset](topology.md#open-set), with representatives identified when they agree on a smaller dense [open subset](topology.md#open-set). For an integral source and a [separated variety](ringed-space.md#separated-variety) as target, agreement on a dense open determines a morphism uniquely. This definition also permits nonprojective sources.

### Ring of rational functions on a reduced variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

For a possibly reducible [algebraic variety](#algebraic-variety) $X$, take pairs $(U,f)$ with $U$ a dense open subset and $f$ a [regular function](ringed-space.md#regular-function) on $U$. Identify pairs agreeing on a common dense open subset. Addition and multiplication on intersections make these classes a [ring](commutative-algebra.md#ring). For an [affine variety](#affine-algebraic-set) with reduced [coordinate ring](#coordinate-ring) $A$, this ring is its [total quotient ring](commutative-algebra.md#total-ring-of-fractions). For an [irreducible variety](#irreducible-variety), it is the [function field](#function-field-of-an-algebraic-variety). An [isomorphism](algebra.md#isomorphism) of dense open subsets induces an [isomorphism](algebra.md#isomorphism) of these rings.

#### Local ring embeds in rational functions on incident components

↑ **Parent:** [Ring of rational functions on a reduced variety](#ring-of-rational-functions-on-a-reduced-variety)

Let $Y$ be the reduced union of the [irreducible components](#irreducible-component) of an [affine variety](#affine-algebraic-set) $X$ containing $P$. Removing all other components leaves an open neighbourhood of $P$ on which $X$ and $Y$ agree, so their [local rings](commutative-algebra.md#local-ring) at $P$ agree. In the [coordinate ring](#coordinate-ring) $B=k[Y]$, every denominator not vanishing at $P$ avoids all minimal primes: each component of $Y$ contains $P$. Such a denominator is a [non-zero-divisor](mathematics.md#non-zero-divisor). Consequently $B_{\mathfrak m_P}$ injects into the [total quotient ring](commutative-algebra.md#total-ring-of-fractions) $Q(B)=\operatorname{Rat}(Y)$. One cannot generally replace $Y$ by a single component through an intersection point.

### Rational function on an algebraic variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

On an integral algebraic variety, a rational function is an equivalence class of regular functions on nonempty open subsets, with equality on a common dense open subset. These form the function field $k(X)$. On an affine open $\operatorname{Spec}A$, this field is the fraction field of $A$.

// Target: geometry-and-topology.bigb

### Quasi-projective algebraic set

↑ **Parent:** [Algebraic variety](#algebraic-variety)

A locally closed [affine algebraic set](#affine-algebraic-set) in a [projective space](projective-space.md), equivalently an [open subset](topology.md#open-set) of a closed subset of [projective space](projective-space.md) cut out by homogeneous polynomials. Reducibility is allowed for an algebraic set; an [irreducible variety](#irreducible-variety) with such an embedding is a [quasi-projective variety](#quasi-projective-variety).

#### Quasi-projective variety

↑ **Parent:** [Quasi-projective algebraic set](#quasi-projective-algebraic-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-projective_variety)

An [irreducible variety](#irreducible-variety) which admits a locally closed embedding into [projective space](projective-space.md). Open subsets of [affine varieties](#affine-algebraic-set) and [blowups of algebraic varieties](#blowing-up-algebraic-geometry) along closed centres give important examples.

### Irreducible variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

An [algebraic variety](#algebraic-variety) whose underlying [topological space](topology.md#topological-space) with its [Zariski topology](#zariski-topology) is an [irreducible topological space](#irreducible-topological-space): it is nonempty and cannot be a union of two proper closed subsets. For a reduced affine variety, this is equivalent to its [coordinate ring](#coordinate-ring) being an [integral domain](commutative-algebra.md#integral-domain).

### Constructible subset of a variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

A constructible subset is a finite union of locally closed subsets in the [Zariski topology](#zariski-topology). A dense constructible subset contains a dense open subset. Constructibility alone is weaker than closedness, but a [constructible subgroup is closed](#constructible-subgroup-is-closed).

#### Chevalley constructibility theorem

↑ **Parent:** [Constructible subset of a variety](#constructible-subset-of-a-variety)

The image of a morphism of algebraic varieties is constructible. This replaces the generally false assertion that all morphisms have closed image. Group structure adds the fact that a [constructible subgroup is closed](#constructible-subgroup-is-closed).

### Rational point

↑ **Parent:** [Algebraic variety](#algebraic-variety)

For an [algebraic variety](#algebraic-variety) $X$ defined over a [field](algebra.md#field) $K$, a K-[rational point](#rational-point) is a morphism $\operatorname{Spec}K\to X$ over $K$. In affine coordinates it is a solution of the defining equations with every coordinate in $K$; in projective coordinates it is a nonzero coordinate vector over $K$, considered up to common nonzero scaling. The set is denoted $X(K)$. Over a [number field](algebraic-number-theory.md#number-field), having points over every completion need not imply having a [rational point](#rational-point); for genus-one coverings this failure is recorded by the [Tate–Shafarevich group](normalization-of-an-algebraic-curve.md#tate-shafarevich-group).

### Smooth algebraic variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

An algebraic variety is smooth over its ground field when its structural morphism is smooth. Over an algebraically closed field its local rings are regular; on an irreducible variety its tangent spaces all have the variety's [dimension of a scheme](ringed-space.md#dimension-of-a-scheme).

#### Smoothness of an algebraic variety

↑ **Parent:** [Smooth algebraic variety](#smooth-algebraic-variety)

Over a [perfect field](algebra.md#perfect-field), a point of an [algebraic variety](#algebraic-variety) is smooth exactly when its [local ring](commutative-algebra.md#local-ring) is a [regular local ring](commutative-algebra.md#regular-local-ring). The [smooth locus of a variety](#smooth-locus-of-a-variety) is open; its closed complement is the [singular locus](#singular-locus).

### Normalization of an algebraic variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

The normalization of an integral [algebraic variety](#algebraic-variety) is obtained by taking the integral closure of its affine coordinate rings in its [function field](#function-field-of-an-algebraic-variety). Its natural morphism is finite and birational, and its source is normal. For [Cartier divisors](cartier-divisor.md), [bigness under finite normalization](cartier-divisor.md#bigness-under-finite-normalization) compares section growth on the two varieties.

### Closed subvariety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

A closed subvariety is an integral closed subscheme of an [algebraic variety](#algebraic-variety). It supplies the lower-dimensional loci on which positivity is tested by the [Nakai–Moishezon criterion](cartier-divisor.md#nakai-moishezon-criterion).

### Algebraic curve

↑ **Parent:** [Algebraic variety](#algebraic-variety)

An algebraic curve is a one-dimensional [algebraic variety](#algebraic-variety). On a [smooth algebraic curve](#smooth-algebraic-curve), the local ring at every closed point is a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), which allows orders of zeros and poles to be recorded as a [divisor on an algebraic curve](#divisor-on-an-algebraic-curve).

#### Integral projective curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

An [algebraic curve](#algebraic-curve) which is projective, [reduced](commutative-algebra.md#reduced-ring) and [irreducible](representation-theory.md#irreducible-representation). Over an [algebraically closed field](algebra.md#algebraically-closed-field), its only [global regular functions](ringed-space.md#global-regular-function) are constants and its [arithmetic genus](#arithmetic-genus) is $h^1(\mathcal O_C)\ge0$.

#### Nonsingular point of an algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

For an affine plane [algebraic curve](#algebraic-curve) $F(x,y)=0$, a point over an [algebraic closure](algebra.md#algebraic-closure) is nonsingular when the displayed condition holds. Its [Zariski tangent space](#zariski-tangent-space) has dimension one, and a local coordinate can be chosen in the direction of a nonzero [partial derivative](calculus.md#partial-derivative). A [smooth algebraic curve](#smooth-algebraic-curve) has all points nonsingular. Over a complete [local field](arithmetic.md#local-field), the [Hensel lemma](arithmetic.md#hensel-s-lemma) lifts a nonsingular residue point by solving for a coordinate with unit [partial derivative](calculus.md#partial-derivative).

#### Affine algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

An affine algebraic curve is an [affine variety](#affine-algebraic-set) of [Krull dimension](commutative-algebra.md#krull-dimension) one. An irreducible affine curve has a finitely generated one-dimensional domain as its [coordinate ring](#coordinate-ring). Quotienting this ring by a nonzero element gives a zero-dimensional [Noetherian ring](algebra.md#noetherian-ring), hence an [Artinian ring](algebra.md#artinian-ring). Consequently a nonzero regular function has finitely many zeros. No nonsingularity assumption is part of the definition.

#### Cuspidal cubic

↑ **Parent:** [Algebraic curve](#algebraic-curve)

The projective [algebraic curve](#algebraic-curve) $D=\{y^2z=x^3\}\subset\mathbb P^2$ is an irreducible cubic with a [cusp](#cusp-algebraic-geometry) at $[0:0:1]$. In the chart $z=1$, its equation is $y^2=x^3$, with parametrization $(x,y)=(t^2,t^3)$. Its affine version $y^2=z^3$, used below, differs only by renaming a coordinate. At the point $[0:1:0]$, the chart $y=1$ gives $z=x^3$, which is smooth and exhibits its [unique smooth flex of a cuspidal cubic](#unique-smooth-flex-of-a-cuspidal-cubic).

##### Unique smooth flex of a cuspidal cubic

↑ **Parent:** [Cuspidal cubic](#cuspidal-cubic)

For $D=\{y^2z=x^3\}$, the determinant of the homogeneous [Hessian matrix](calculus.md#hessian-matrix) is $24xy^2$. Its intersections with $D$ are the cusp $[0:0:1]$ and the smooth point $[0:1:0]$. The [Hessian criterion for a flex](#hessian-criterion-for-a-flex) therefore gives a unique smooth [flex](#inflection-point-of-an-algebraic-plane-curve), with tangent $z=0$ and contact order three. Consequently every pair consisting of a triple line and a cuspidal cubic meeting only at a smooth point is projectively equivalent to $(3\{z=0\},D)$.

##### Cusp with two isolated-point components

↑ **Parent:** [Cuspidal cubic](#cuspidal-cubic)

The algebraic set in $\mathbb A^3$ defined by

$$
xy=0,
\qquad y^2-z^3+xz=0,
\qquad x(x+y+2z+1)=0
$$

is the disjoint union of the cuspidal cubic $V(x,y^2-z^3)$ and the two reduced points $(-1,0,0)$ and $(1,0,-1)$. Its radical vanishing ideal is the intersection of the three corresponding prime ideals.

#### Symmetric product of a curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

The [scheme](ringed-space.md#scheme) $C^{(d)}$ parametrizes effective degree-$d$ [Cartier divisors](cartier-divisor.md) on a smooth [algebraic curve](#algebraic-curve). Near a [Cartier divisor](cartier-divisor.md) $\sum m_iP_i$, its completed local ring is a power-series ring in the elementary symmetric coordinates of $m_i$ local parameters at each $P_i$. It is therefore smooth of dimension $d$, even when the [characteristic of a field](algebra.md#characteristic-of-a-field) divides $d!$. For projective $C$ it is projective.

#### Monomial curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

Over a [field](algebra.md#field) $k$, an affine curve parametrized by positive integer powers of one parameter. Its coordinate [ring](commutative-algebra.md#ring) is the subalgebra generated by those powers, and its defining [prime ideal](commutative-algebra.md#prime-ideal) is the kernel of $k[x_1,\ldots,x_n]\to k[t]$ sending $x_i$ to $t^{a_i}$. Equal exponent sums yield binomial relations. Studying those relations connects an additive semigroup of exponents to the geometry of the curve.

##### Monomial curve with exponents three, four and five

↑ **Parent:** [Monomial curve](#monomial-curve)

The kernel of $x\mapsto t^3$, $y\mapsto t^4$, $z\mapsto t^5$ is generated by $y^2-xz$, $yz-x^3$, $z^2-x^2y$. Reducing these three relations leaves a unique normal form $A_0(x)+A_1(x)y+A_2(x)z$: its images have distinct exponents modulo three. The curve [ring](commutative-algebra.md#ring) is therefore finite free of rank three over $k[x]$ and has dimension one. In a three-variable [polynomial ring](commutative-algebra.md#polynomial-ring) its [ideal](commutative-algebra.md#ideal) has height two, but its three independent quadratic initial forms force at least three generators. This is a concrete failure of generation by codimension many equations.

#### Rational parametrization of an algebraic curve

↑ **Parent:** [Algebraic curve](#algebraic-curve)

A rational parametrization expresses the coordinates of an [algebraic curve](#algebraic-curve) as [rational functions](isolated-singularity.md#rational-function) of a parameter, with a rational inverse on a dense open subset. It identifies the [function field](#function-field-of-an-algebraic-variety) with $K(t)$ and the smooth projective [normalization of an algebraic curve](normalization-of-an-algebraic-curve.md) with the [projective line](finite-group-theory.md#projective-line). A nonconstant parametrizing map without an inverse is a weaker notion; even this cannot exist for an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) in characteristic zero.

#### Arithmetic genus

↑ **Parent:** [Algebraic curve](#algebraic-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arithmetic_genus)

The [arithmetic genus](#arithmetic-genus) of a proper curve $C$ is $p_a(C)=1-\chi(C,\mathcal O_C)$. For an integral projective curve over an algebraically closed field, $H^0(C,\mathcal O_C)=k$, so $p_a=h^1\ge0$. Its finite normalization has $p_a(C)=g(C^\nu)+\operatorname{length}(\nu_*\mathcal O_{C^\nu}/\mathcal O_C)$. Hence [arithmetic genus](#arithmetic-genus) zero forces the curve to be smooth and rational.

##### Genus of a complete-intersection space curve

↑ **Parent:** [Arithmetic genus](#arithmetic-genus)

For a [projective complete intersection](ringed-space.md#projective-complete-intersection) curve cut out by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of positive degrees $a,b$ in $\mathbb P^3_k$, the [Koszul resolution](algebra.md#koszul-resolution) gives [Hilbert polynomial](#hilbert-polynomial) $ab\,m+ab(4-a-b)/2$. Hence its [arithmetic genus](#arithmetic-genus) is $1+ab(a+b-4)/2$. The same resolution shows $H^0(C,\mathcal O_C)=k$, and the [dimension of a scheme](ringed-space.md#dimension-of-a-scheme) is one, so this genus equals $\dim_kH^1(C,\mathcal O_C)$. Smoothness and irreducibility of the curve are not required. For degrees five and seven, the value is $141$.

### Prevariety

↑ **Parent:** [Algebraic variety](#algebraic-variety)

In the classical convention over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$, a prevariety is an [irreducible topological space](#irreducible-topological-space) with a [sheaf of rings](ringed-space.md#sheaf-of-rings) which has a finite [open cover](topology.md#open-cover) by [affine varieties](#affine-algebraic-set), with compatible local identifications. A prevariety need not be separated. A classical [algebraic variety](#algebraic-variety) is a separated prevariety: its [diagonal morphism](ringed-space.md#diagonal-morphism) has closed image. Some authors allow reducible prevarieties and varieties; the separation criterion and product construction remain the same under that convention.

### Algebraic group

↑ **Parent:** [Algebraic variety](#algebraic-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_group)

A group variety is an [algebraic variety](#algebraic-variety) whose multiplication and inversion are morphisms.

#### Isogeny

↑ **Parent:** [Algebraic group](#algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isogeny)

An isogeny is a surjective [morphism](algebra.md#morphism) of [algebraic groups](#algebraic-group) with finite kernel. For [abelian varieties](abelian-variety.md) it is a finite surjective group morphism. An [isogeny of elliptic curves](normalization-of-an-algebraic-curve.md#isogeny-of-elliptic-curves) is its one-dimensional abelian-variety specialization.

#### Multiplicative group scheme

↑ **Parent:** [Algebraic group](#algebraic-group)

The multiplicative group [scheme](ringed-space.md#scheme) represents [units](algebra.md#unit-in-a-ring): its $R$-points are $R^\times$. Multiplication is specified by $t\mapsto t\otimes t$ on the coordinate [ring](commutative-algebra.md#ring). It is the [principal open subset](ringed-space.md#principal-open-subscheme) $D(t)$ of the [affine line](ringed-space.md#affine-line) and the one-dimensional split [algebraic torus](toric-geometry.md#algebraic-torus).

// Target: ringed-space.bigb

#### Multiplicative algebraic group

↑ **Parent:** [Algebraic group](#algebraic-group)

The multiplicative [algebraic group](#algebraic-group) has $\mathbb G_m(K)=K^{\times}$, with multiplication as its [group operation](group.md#group-operation). Its coordinate ring is $K[z,z^{-1}]$. The [formal multiplicative group](normalization-of-an-algebraic-curve.md#formal-multiplicative-group) describes its law near the identity $z=1$.

#### Algebraic group action

↑ **Parent:** [Algebraic group](#algebraic-group)

This is a group action whose action map $G\times V\to V$ is a morphism of varieties. Orbits are locally closed: constructibility gives a relatively open piece, and its translates cover the orbit. An orbit of an irreducible group is irreducible and open in its closure. These facts control degenerations of [quiver representations](algebra.md#representation-of-a-quiver).

#### Dimension formula for an algebraic group homomorphism

↑ **Parent:** [Algebraic group](#algebraic-group)

The kernel is a closed identity fiber. The image is closed because a [constructible subgroup is closed](#constructible-subgroup-is-closed). Every nonempty fiber is a kernel translate, so the [fiber dimension theorem](#fiber-dimension-theorem) gives $\dim G=\dim\ker\varphi+\dim\operatorname{im}\varphi$, even for inseparable morphisms.

#### Constructible subgroup is closed

↑ **Parent:** [Algebraic group](#algebraic-group)

Let $S$ be constructible in an [algebraic group](#algebraic-group), and $C=\overline S$. The closure is a subgroup. Choose a dense open $U\subseteq C$ contained in $S$. For every $c\in C$, the dense opens $U,cU$ intersect, giving $u=cv$ for $u,v\in S$. Hence $c=uv^{-1}\in S$ and $S=C$. The [Chevalley constructibility theorem](#chevalley-constructibility-theorem) therefore proves closedness of homomorphism images.

#### Homomorphism of group varieties

↑ **Parent:** [Algebraic group](#algebraic-group)

A homomorphism of group varieties is a morphism of algebraic varieties that also preserves multiplication. It automatically preserves the identity and inversion.

#### Abelian variety

↑ **Parent:** [Algebraic group](#algebraic-group)

[This section is present in another page, follow this link to view it.](abelian-variety.md)

### Smooth algebraic curve

↑ **Parent:** [Algebraic variety](#algebraic-variety)

A smooth algebraic curve is a one-dimensional [algebraic variety](#algebraic-variety) whose [local ring](commutative-algebra.md#local-ring) at every point is regular.

This is the nonsingular subclass of [algebraic curves](#algebraic-curve).

#### Product dimension bound for sections on a curve

↑ **Parent:** [Smooth algebraic curve](#smooth-algebraic-curve)

For nonzero finite-dimensional spaces $V,W$ of sections of two [line bundles](ringed-space.md#line-bundle) on a smooth integral curve over an algebraically closed field, their product span in sections of the tensor product satisfies this bound. At one point choose bases with strictly increasing orders of vanishing. Multiplying every first-space basis vector by the first second-space vector, and then the last first-space vector by the remaining second-space vectors, produces distinct increasing orders and hence independent sections. This proves the dimension inequality needed for the [Clifford inequality for curves](#clifford-inequality-for-curves).

### Affine algebraic set

↑ **Parent:** [Algebraic variety](#algebraic-variety)

An affine algebraic set is the common zero set $V(I)$ of an [ideal](commutative-algebra.md#ideal) in a polynomial ring over a field.

#### Affineness from a unit-ideal principal affine cover

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

A classical [variety](#algebraic-variety) is affine if finitely many global [regular functions](ringed-space.md#regular-function) generate the [unit ideal](commutative-algebra.md#unit-ideal) and their nonvanishing opens are affine. [Localization of global sections on a principal open](ringed-space.md#localization-of-global-sections-on-a-principal-open) identifies their [coordinate rings](#coordinate-ring) with $A_{f_i}$, where $A=\Gamma(X,\mathcal O_X)$. Choose a finite-type subalgebra of $A$ containing the functions, their unit-ideal coefficients and numerators of generators of every $A_{f_i}$. Its affine variety has the same principal affine charts, whose [isomorphisms](algebra.md#isomorphism) glue globally. This avoids assuming finite generation of $A$ before affineness is known.

#### Morphism of affine varieties

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

A map between [affine varieties](#affine-algebraic-set) is a morphism when its coordinate functions are restrictions of ambient [polynomials](polynomial.md). Pullback identifies these morphisms contravariantly with homomorphisms of their [coordinate rings](#coordinate-ring).

#### Coordinate ring of a product of affine varieties

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

For [affine varieties](#affine-algebraic-set) $X,Y$ over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$, their [product in a category](category.md#product-category-theory) is affine, with [coordinate ring](#coordinate-ring) $A\otimes_k B$, where $A=k[X]$ and $B=k[Y]$. Presenting $A=k[x]/J$ and $B=k[y]/L$ identifies this ring with $k[x,y]/(J,L)$. If both varieties are irreducible, this is an [integral domain](commutative-algebra.md#integral-domain): express a nonzero tensor $F$ using linearly independent second factors. The points $x$ where its specialization $F_x$ is nonzero form a nonempty open subset of $X$. For two nonzero tensors $F,G$, choose $x$ in the intersection of these open subsets; then $F_xG_x\ne0$ in the domain $B$. The [Hilbert Nullstellensatz](#hilbert-nullstellensatz) identifies $(J,L)$ with the defining ideal of $X\times Y$. The universal property follows from the universal property of the [tensor product of modules](module-theory.md#tensor-product-of-modules) as a tensor product of commutative algebras.

#### Vanishing ideal

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

The vanishing ideal of $X\subseteq k^n$ is

$$
I(X)=\{f\in k[x_1,\ldots,x_n]:f(x)=0\text{ for every }x\in X\}.
$$

#### Coordinate ring

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coordinate_ring)

For an affine algebraic set $X\subseteq\mathbb A_k^n$, its coordinate ring is

$$
k[X]=k[x_1,\ldots,x_n]/I(X).
$$

The set $X$ is irreducible exactly when $k[X]$ is an [integral domain](commutative-algebra.md#integral-domain).

##### Irreducibility and prime vanishing ideal

↑ **Parent:** [Coordinate ring](#coordinate-ring)

For an affine algebraic set $X$ over an algebraically closed field,

$$
X\text{ is irreducible}
\quad\Longleftrightarrow\quad
I(X)\text{ is a prime ideal}.
$$

If $fg$ vanishes on $X$, then $X$ is the union of its intersections with $V(f)$ and $V(g)$. Conversely, a nontrivial decomposition into closed subsets supplies functions vanishing on each proper piece whose product vanishes on all of $X$.

##### Dominant morphism of affine varieties

↑ **Parent:** [Coordinate ring](#coordinate-ring)

A morphism $f:X\to Y$ of affine varieties is dominant when its image is [Zariski dense](#zariski-dense-subset) in $Y$. It is dominant exactly when the pullback homomorphism

$$
f^*:k[Y]\to k[X]
$$

is injective. When $X$ and $Y$ are irreducible, this injection extends to their function fields and gives $\dim X\geq\dim Y$.

This is the dense-image case of a [morphism of algebraic varieties](#morphism-of-algebraic-varieties).

#### Vanishing loci of ideal sums and intersections

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

For ideals $I,J\subseteq k[x_1,\ldots,x_n]$,

$$
V(I+J)=V(I)\cap V(J),
\qquad
V(I\cap J)=V(I)\cup V(J).
$$

The second equality also follows from $V(IJ)=V(I)\cup V(J)$ and

$$
IJ\subseteq I\cap J.
$$

#### Irreducible components of two intersecting complex hyperbolas

↑ **Parent:** [Affine algebraic set](#affine-algebraic-set)

The algebraic set

$$
V(x^2+y^2-1,x^2-z^2-1)\subseteq\mathbb A_{\mathbb C}^3
$$

has the two irreducible components

$$
V(y-iz,x^2-z^2-1)
\quad\text{and}\quad
V(y+iz,x^2-z^2-1).
$$

Each is irreducible because the linear change $u=x-z$, $v=x+z$ identifies its [coordinate ring](#coordinate-ring) with

$$
\mathbb C[u,v]/(uv-1)\cong\mathbb C[u,u^{-1}],
$$

an [integral domain](commutative-algebra.md#integral-domain).

### Function field of an algebraic variety

↑ **Parent:** [Algebraic variety](#algebraic-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Function_field_of_an_algebraic_variety)

The function field $k(X)$ of an irreducible [algebraic variety](#algebraic-variety) consists of its [rational functions](isolated-singularity.md#rational-function).

#### Sheaf of nonzero rational functions on an irreducible variety

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

For an irreducible [algebraic variety](#algebraic-variety) $X$ with [function field](#function-field-of-an-algebraic-variety) $K$, this [sheaf of abelian groups](#sheaf-of-abelian-groups) assigns $K^*$ to every nonempty open set, with identity restriction maps, and assigns the trivial group to the empty set. Irreducibility ensures that any two nonempty open subsets meet, so these sections satisfy the [sheaf gluing axiom](#sheaf-gluing-axiom). It is a [flasque sheaf](ringed-space.md#flasque-sheaf) and has zero higher [sheaf cohomology](ringed-space.md#sheaf-cohomology).

#### Dimension from the function field

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

For an irreducible variety $X$ over a field $k$,

$$
\dim X=\operatorname{trdeg}_k k(X).
$$

Consequently birational irreducible varieties have the same dimension.

#### Projective model of a finitely generated field

↑ **Parent:** [Function field of an algebraic variety](#function-field-of-an-algebraic-variety)

If $K/k$ is a finitely generated field extension, write $K=\operatorname{Frac}(A)$ for a finitely generated integral $k$-algebra $A$. The projective closure of the affine variety $\operatorname{Spec}A$ is an irreducible projective variety with function field $K$.

### Morphism of algebraic varieties

↑ **Parent:** [Algebraic variety](#algebraic-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_algebraic_varieties)

A morphism of algebraic varieties is a map given locally by regular functions. A projective-coordinate formula defines a morphism wherever its homogeneous coordinate functions do not vanish simultaneously.

#### Morphism of algebraic curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A [morphism of algebraic varieties](#morphism-of-algebraic-varieties) whose source and target are [algebraic curves](#algebraic-curve). A nonconstant morphism between [smooth projective curves](projective-space.md#smooth-projective-curve) is finite and surjective; its degree is the degree of the induced extension of [function fields](#function-field-of-an-algebraic-variety).

#### Conic bundle

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conic_bundle)

A flat proper [morphism of algebraic varieties](#morphism-of-algebraic-varieties) whose geometric fibres are [plane conics](#plane-conic), usually presented as a quadratic equation in a [projective bundle](fiber-bundle.md#projective-bundle) of relative dimension two. The generic fibre is normally required to be smooth; singular conics can occur in special fibres. A [conic bundle from a line on a smooth cubic surface](#conic-bundle-from-a-line-on-a-smooth-cubic-surface) has five reducible fibres over the [projective line](finite-group-theory.md#projective-line).

##### Conic discriminant

↑ **Parent:** [Conic bundle](#conic-bundle)

In characteristic different from two, a local equation for a [conic bundle](#conic-bundle) is $z^{\mathsf T}Mz=0$ with $M$ symmetric. A fibre is singular exactly when the [determinant](linear-algebra.md#determinant) vanishes. Changing the fibre coordinates multiplies that determinant by a nonzero square, so its zero locus is intrinsically defined even when the quadratic coefficients belong to twisting [line bundles](ringed-space.md#line-bundle).

###### Reduced singular fibres of a smooth conic bundle

↑ **Parent:** [Conic discriminant](#conic-discriminant)

Let the base be a [smooth algebraic curve](#smooth-algebraic-curve), the total surface be smooth, and the [field](algebra.md#field) be algebraically closed of characteristic different from two. At a rank-two singular fibre with kernel vector $v$, the fibre derivatives vanish at $[v]$. Smoothness requires $v^{\mathsf T}M'v\ne0$. The [adjugate matrix](linear-algebra.md#adjugate-matrix) is a nonzero multiple of $vv^{\mathsf T}$, so the determinant has a simple zero. At rank at most one, the projective kernel contains a line and the quadratic $v^{\mathsf T}M'v$ has a zero on it; that point would make the total surface singular. Thus every singular fibre is a pair of distinct [projective lines](finite-group-theory.md#projective-line) and its discriminant zero is simple.

#### Generically finite morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A dominant [morphism of varieties](#morphism-of-algebraic-varieties) is generically finite when its extension of [function fields](#function-field-of-an-algebraic-variety) is finite. Its degree is the degree of this field extension. A dominant morphism between integral varieties of equal dimension is generically finite; over a suitable nonempty open subset of the target its fibers are finite.

#### Isomorphic local rings determine isomorphic neighborhoods

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A $k$-algebra isomorphism between the local rings at closed points extends to a morphism on some neighborhoods: represent the images of finitely many affine coordinate generators by fractions, and shrink where their denominators are nonzero and their finitely many relations hold. Extend its inverse the same way. The two compositions agree with the identity as germs; finitely many coordinate equalities make them identities after shrinking again. Taking inverse images of these neighborhoods then gives mutually inverse actual neighborhood isomorphisms, not just a formal-completion isomorphism.

#### Degree of a morphism of curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

A nonconstant [morphism of algebraic varieties](#morphism-of-algebraic-varieties) $f:C\to D$ between smooth projective integral curves is finite, and its degree is the degree of the induced extension of [function fields](#function-field-of-an-algebraic-variety). It is also the degree of the pullback of a rational point, with ramification multiplicities and residue degrees included: locally the finite coordinate algebra is a torsion-free module over the target [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring), hence free of its generic rank. For $D=\mathbb P^1$ and a [rational function](isolated-singularity.md#rational-function) defining $f$, the pullback of infinity is its pole [divisor](number-theory.md#divisor), so the total pole degree equals $\deg f$. A degree-one finite map to a normal curve is an isomorphism, since a finite integral algebra inside its unchanged function field equals the integrally closed target ring.

#### Algebraic quotient by a finite group

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For an [affine variety](#affine-algebraic-set) with [coordinate ring](#coordinate-ring) $A$ acted on by a [finite group](group.md#finite-group) $G$, the affine quotient is $\operatorname{Spec}A^G$. Elements of $A$ satisfy monic orbit polynomials over $A^G$, so the quotient map is a [finite morphism](#finite-morphism). Over an [algebraically closed field](algebra.md#algebraically-closed-field), invariant functions separate finite orbits; in characteristic not dividing $|G|$, interpolate and average a function separating two orbits. The quotient fibres are consequently the orbits.

#### Affine-target adjunction for varieties

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a classical [algebraic variety](#algebraic-variety) $X$ and [affine variety](#affine-algebraic-set) $Y$, a homomorphism on the indicated rings gives a morphism by evaluating the images of affine coordinate generators at each point of $X$. The relations defining $Y$ remain zero. Local fractions pull back to local regular fractions, proving regularity; the [coordinate ring](#coordinate-ring) generators also prove uniqueness.

#### Ramification index of a morphism of curves

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a nonconstant morphism between nonsingular curves and a local target [uniformizer](commutative-algebra.md#uniformizer) $t$ at the image of $P$, the index is the [order of vanishing](isolated-singularity.md#order-of-vanishing) of its pullback. Changing $t$ multiplies it by a local [unit in a ring](algebra.md#unit-in-a-ring) and does not change that order. This is a [valuation](algebra.md#valuation) definition and remains meaningful for inseparable morphisms.

#### Fiber of a morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

For a [morphism of algebraic varieties](#morphism-of-algebraic-varieties) $f:X\to Y$ and $y\in Y$, the fiber is the inverse-image variety $X_y=f^{-1}(y)$.

For a point $y$, the underlying [fiber](function.md#fiber-of-a-function) is the inverse image $f^{-1}(y)$.

##### Local fibre dimension

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

The dimension of the [fibre of a morphism](#fiber-of-a-morphism) locally at its source point $x$: the maximum of the dimensions of the fibre's irreducible components through $x$. This differs from the [Krull dimension](commutative-algebra.md#krull-dimension) of the local ring at a nonclosed point.

###### Upper semicontinuity of local fibre dimension

↑ **Parent:** [Local fibre dimension](#local-fibre-dimension)

For a finite-type [morphism of schemes](ringed-space.md#morphism-of-schemes), local fibre dimension is upper semicontinuous on the source, in the displayed sense. If the morphism is proper, the maximal fibre dimension is also upper semicontinuous on the target. Without properness a component of a large fibre can disappear from the source over a special point, so the target statement is not valid in that generality. [The Stacks Project: dimension of fibres](https://stacks.math.columbia.edu/tag/0B2H) distinguishes these statements.

##### Fiber dimension theorem

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

For a dominant morphism of irreducible varieties, generic fiber dimension is source dimension minus target dimension, and this dimension occurs over a nonempty open subset. In particular, constant fiber dimension $d$ gives source dimension equal to target dimension plus $d$. For algebraic groups the equal-dimensional components and coset fibers allow the same dimension formula componentwise.

###### Dimension of image of a morphism

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For an irreducible source, regard the [morphism of algebraic varieties](#morphism-of-algebraic-varieties) as dominant onto the closure of its image, with generic point $\eta$. The [fiber dimension theorem](#fiber-dimension-theorem) gives the displayed formula. A [proper morphism](ringed-space.md#proper-morphism) has closed image, so the closure can then be omitted.

###### Isolated fibre point forces dominance in equal dimensions

↑ **Parent:** [Dimension of image of a morphism](#dimension-of-image-of-a-morphism)

Let $f:X\to Y$ be a [proper morphism](ringed-space.md#proper-morphism) of irreducible [algebraic varieties](#algebraic-variety) with equal dimension. If some fibre has an isolated point, its corresponding irreducible component has dimension zero. Apply the [fiber dimension theorem](#fiber-dimension-theorem) to $X\to f(X)$: $0\ge\dim X-\dim f(X)$. Thus the closed image has dimension $\dim Y$ and equals $Y$. The [incidence proof that a cubic surface contains a line](#incidence-proof-that-a-cubic-surface-contains-a-line) is an application; the entire witness fibre need not be finite.

###### Generic equidimensionality of fibres

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For a dominant [morphism of algebraic varieties](#morphism-of-algebraic-varieties) between irreducible varieties, there is a nonempty [Zariski-open subset](#zariski-open-set) of the target over which every fibre is nonempty and every irreducible component has the displayed dimension. Apply [Noether normalization](#noether-normalization) to affine source charts over the target [function field](#function-field-of-an-algebraic-variety) and clear denominators on the target to get a generic upper bound. Combine it with the closed-fibre lower bound in the [fiber dimension theorem](#fiber-dimension-theorem).

###### Closed-fibre lower bound by finite normalization

↑ **Parent:** [Fiber dimension theorem](#fiber-dimension-theorem)

For a surjective morphism of irreducible varieties, choose an affine neighborhood of the target point and a finite [Noether normalization](#noether-normalization) to affine space of target dimension $r$. On an affine source neighborhood the composite fibre is cut out by $r$ functions, so repeated [principal hypersurface dimension lemma](#principal-hypersurface-dimension-lemma) gives dimension at least source dimension minus $r$ on every component. The normalization fibre is finite. The original fibre is therefore an open-and-closed union of components of that composite fibre, proving the bound without assuming target smoothness. For a reducible source the bound must instead be applied using the dimension of each source component.

##### Scheme-theoretic fiber

↑ **Parent:** [Fiber of a morphism](#fiber-of-a-morphism)

For a morphism of schemes $f:X\to Y$ and a point $y\in Y$, the scheme-theoretic fiber is the fiber product $X\times_Y\operatorname{Spec}\kappa(y)$. It remembers multiplicities and nilpotents that the underlying set-theoretic inverse image cannot detect.

Its underlying [fiber](function.md#fiber-of-a-function) is enriched with local-ring and multiplicity information.

###### Fibre of absolute Frobenius over a rational point of the affine line

↑ **Parent:** [Scheme-theoretic fiber](#scheme-theoretic-fiber)

Over a [perfect field](algebra.md#perfect-field) $k$ of characteristic $p$, the [scheme-theoretic fiber](#scheme-theoretic-fiber) of the [Absolute Frobenius morphism](ringed-space.md#absolute-frobenius-morphism) of $\mathbb A_k^1$ over a rational point $a$ is

$$
\operatorname{Spec}\bigl(k[t]\otimes_{k[t],\,t\mapsto t^p}k\bigr)
\cong\operatorname{Spec}k[t]/(t-a)^p.
$$

Its underlying space is one point, but its coordinate ring has a nonzero [nilpotent element](commutative-algebra.md#nilpotent), so the fibre is a length-$p$ [nonreduced scheme](ringed-space.md#nonreduced-scheme).

#### Isomorphism of algebraic varieties

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)

An isomorphism of algebraic varieties is a [morphism](#morphism-of-algebraic-varieties) with a morphic inverse. It preserves all properties intrinsic to the variety.

#### Finite morphism

↑ **Parent:** [Morphism of algebraic varieties](#morphism-of-algebraic-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_morphism)

A finite morphism is a morphism whose inverse image of every affine open set is affine and whose corresponding coordinate ring is finite as a module over the base coordinate ring. A nonconstant morphism between smooth projective curves is finite, and its degree is the number of points in a generic fiber counted with multiplicity.

##### Trace-dual module of a finite curve map

↑ **Parent:** [Finite morphism](#finite-morphism)

For a finite generically separable morphism between [smooth projective curves](projective-space.md#smooth-projective-curve), the [field trace](algebraic-number-theory.md#field-trace) on [rational differentials](#rational-differential-on-an-algebraic-curve) identifies the differential sheaf with the trace-dual module. Locally, for $A=k[[s]]\subset B=k[[u]]$ with $s=f(u)$, the trace-dual fractional ideal is $f'(u)^{-1}B$. Multiplying it by $ds=f'(u)du$ gives $Bdu$. For a monogenic finite extension with monic polynomial $P$, the identity $\operatorname{Tr}(g(u)/P'(u))=[T^{e-1}](g(T)\bmod P(T))$ proves the dual-module formula: the top-coefficient pairing on the basis $1,u,\ldots,u^{e-1}$ has invertible antitriangular matrix. Tensoring locally with an [invertible sheaf](ringed-space.md#line-bundle) yields $\pi_*(\mathcal M^\vee\otimes\Omega^1_C)\cong\mathcal H om(\pi_*\mathcal M,\Omega^1_D)$.

##### Finite morphisms are proper

↑ **Parent:** [Finite morphism](#finite-morphism)

A finite morphism is of finite type and separated: on affine charts the multiplication map $B\otimes_AB\to B$ is surjective and represents its closed diagonal. Each element of a finite algebra satisfies a monic equation by the determinant trick. In a valuative lifting problem, its image in the fraction field is therefore integral over the valuation ring and belongs to that ring, since valuation rings are integrally closed. This gives a lift, unique because the valuation ring embeds in its fraction field. The [valuative criterion for properness](ringed-space.md#valuative-criterion-for-properness) proves properness.

### Projective space

↑ **Parent:** [Algebraic variety](#algebraic-variety)

[This section is present in another page, follow this link to view it.](projective-space.md)

## Irreducible topological space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A nonempty topological space is irreducible when it is not the union of two proper closed subsets. Equivalently, every two nonempty open subsets intersect.

### Irreducible closed subset

↑ **Parent:** [Irreducible topological space](#irreducible-topological-space)

A nonempty [closed subset](topology.md#closed-set) which, with its induced [topology](topology.md), is an [irreducible topological space](#irreducible-topological-space). In an [affine algebraic set](#affine-algebraic-set) these subsets correspond, with reversed inclusion, to [prime ideals](commutative-algebra.md#prime-ideal) of the [coordinate ring](#coordinate-ring).

### Dimension of a topological space by irreducible chains

↑ **Parent:** [Irreducible topological space](#irreducible-topological-space)

This is the supremum of lengths of strict chains of nonempty irreducible closed subsets. Closedness is relative to the given space. This is the relevant dimension for locally closed subsets of [algebraic varieties](#algebraic-variety), rather than a general Hausdorff-space notion of dimension.

#### Dimension of an algebraic set

↑ **Parent:** [Dimension of a topological space by irreducible chains](#dimension-of-a-topological-space-by-irreducible-chains)

The supremum of the lengths of strict chains of nonempty [irreducible closed subsets](#irreducible-closed-subset). It is the maximum of the dimensions of the [irreducible components](#irreducible-component). For an [affine algebraic set](#affine-algebraic-set) it equals the [Krull dimension](commutative-algebra.md#krull-dimension) of its [coordinate ring](#coordinate-ring); for a [quasi-projective algebraic set](#quasi-projective-algebraic-set) it is the supremum of these dimensions over [affine open subsets](ringed-space.md#affine-open-subscheme).

##### Equidimensional algebraic variety

↑ **Parent:** [Dimension of an algebraic set](#dimension-of-an-algebraic-set)

An [algebraic variety](#algebraic-variety) whose [irreducible components](#irreducible-component) all have the same [dimension of an algebraic set](#dimension-of-an-algebraic-set). The components of a generic fibre in the [fiber dimension theorem](#fiber-dimension-theorem) have this property even when that fibre is reducible.

##### Local dimension of an algebraic variety

↑ **Parent:** [Dimension of an algebraic set](#dimension-of-an-algebraic-set)

The [Krull dimension](commutative-algebra.md#krull-dimension) of $\mathcal O_{X,x}$ at a point $x$. For a closed point of an irreducible [affine variety](#affine-algebraic-set) it equals $\dim X$, by the [closed-point dimension lemma for affine domains](#closed-point-dimension-lemma-for-affine-domains). At a generic point of a codimension-one subvariety the local dimension is one.

##### Codimension of an algebraic subvariety

↑ **Parent:** [Dimension of an algebraic set](#dimension-of-an-algebraic-set)

For an irreducible closed subvariety $Y$ of an irreducible variety $X$, its codimension is $\dim X-\dim Y$. In an affine chart it also equals the height of the corresponding [prime ideal](commutative-algebra.md#prime-ideal), by the dimension formula for finite-type domains over a field.

### Generic point

↑ **Parent:** [Irreducible topological space](#irreducible-topological-space)

A generic point is a point whose closure is the whole space. An [integral scheme](ringed-space.md#integral-scheme) has a unique generic point; on an [affine scheme](ringed-space.md#affine-scheme) associated to an [integral domain](commutative-algebra.md#integral-domain), it corresponds to the zero [prime ideal](commutative-algebra.md#prime-ideal). Its [local ring](commutative-algebra.md#local-ring) is the [fraction field](commutative-algebra.md#field-of-fractions) of the domain. On every nonempty affine chart of an integral scheme these fields identify with the same function field.

### Irreducible component

↑ **Parent:** [Irreducible topological space](#irreducible-topological-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irreducible_component)

An irreducible component is a maximal irreducible closed subset. Every algebraic variety is a finite union of its irreducible components.

### Noetherian Zariski topology

↑ **Parent:** [Irreducible topological space](#irreducible-topological-space)

The Zariski topology on affine space is Noetherian because polynomial rings are Noetherian. Every closed subset is a finite union of irreducible closed subsets: a minimal counterexample would split into two smaller closed subsets, each already having such a decomposition.

## Zariski-closed set

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A Zariski-closed set is a common zero set of [polynomials](polynomial.md). Arbitrary intersections and finite unions of such sets are again Zariski closed.

## Zariski-open set

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A Zariski-open set is the complement of a [Zariski-closed set](#zariski-closed-set). A [distinguished affine open](#distinguished-open-set) has the form $D(f)=\{x:f(x)\ne0\}$.

### Distinguished open set

↑ **Parent:** [Zariski-open set](#zariski-open-set)

For a polynomial $f$, the distinguished open set $D(f)$ is the locus on which $f$ does not vanish.

## Noether normalization

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

Every finitely generated algebra $A$ over a field has algebraically independent elements $y_1,\ldots,y_d$ such that $A$ is finite as a module over the polynomial subalgebra $k[y_1,\ldots,y_d]$. The integer $d$ is the Krull dimension of $A$.

### Norm detects proper closed subsets under finite normalization

↑ **Parent:** [Noether normalization](#noether-normalization)

For a finite integral inclusion $A=k[t_1,\ldots,t_r]\subset B$ of domains, a nonzero $b\in B$ has a monic [minimal polynomial](linear-operator-theory.md#minimal-polynomial) over the fraction field with nonzero constant term $a_0\in A$. Its equation gives $a_0\in bB\cap A$. Consequently the image of $V_B(b)$ under the [finite morphism](#finite-morphism) to $\mathbb A^r$ is contained in the proper [Zariski-closed set](#zariski-closed-set) $V_A(a_0)$. Finite morphisms preserve the dimension of a closed subvariety and its image, so this proves dimension drops for proper closed subsets after [Noether normalization](#noether-normalization). A power of $a_0$, up to sign, is the [field norm](algebraic-number-theory.md#field-norm) of $b$.

### Linear Noether normalization for a hypersurface

↑ **Parent:** [Noether normalization](#noether-normalization)

For a nonconstant polynomial $f\in k[t_1,\ldots,t_n]$ over an infinite field, an invertible linear change of coordinates can make $f$ monic in the final coordinate after multiplication by a scalar. Therefore $k[t_1,\ldots,t_n]/(f)$ is integral over a polynomial algebra in the first $n-1$ new coordinates.

## Hilbert Nullstellensatz

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_Nullstellensatz)

For an [algebraically closed field](algebra.md#algebraically-closed-field) $k$ and an [ideal](commutative-algebra.md#ideal) $I\subseteq k[x_1,\ldots,x_n]$, the strong Hilbert Nullstellensatz is

$$
I(V(I))=\sqrt I.
$$

Its weak form says that an ideal with empty [affine zero set](#affine-algebraic-set) is the unit ideal. Equivalently, if finitely many [polynomials](polynomial.md) have no common zero, a polynomial combination of them equals one.

### Radical ideals and closed subsets of the maximal spectrum

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

For a [finitely generated algebra](algebra.md#finitely-generated-algebra) over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$, [radical ideals](commutative-algebra.md#radical-ideal) correspond, with inclusion reversed, to closed subsets of the [maximal spectrum](commutative-algebra.md#maximal-spectrum). If $f\notin\sqrt I$, the nonzero algebra $(A/I)[1/f]$ is still finitely generated over $k$. Its maximal residue field is $k$ by the [Zariski lemma](#zariski-s-lemma), so contracting a maximal ideal gives a maximal ideal of $A$ containing $I$ and avoiding $f$. Hence the intersection of all maximal ideals containing $I$ is $\sqrt I$. This proves the inverse correspondence, including the empty closed set and unit ideal.

### Weak Hilbert Nullstellensatz

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

For an algebraically closed field $k$, every maximal ideal of $k[x_1,\ldots,x_n]$ has the form

$$
(x_1-a_1,\ldots,x_n-a_n)
$$

for a unique point $a\in k^n$. Equivalently, every proper ideal has a common zero.

<h4 id="zariski-s-lemma">Zariski's lemma</h4>

↑ **Parent:** [Weak Hilbert Nullstellensatz](#weak-hilbert-nullstellensatz)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zariski's_lemma)

If a field $L$ is finitely generated as an algebra over a subfield $k$, then $L$ is a finite algebraic extension of $k$. Applying this to a residue field of a polynomial ring proves the [Weak Hilbert Nullstellensatz](#weak-hilbert-nullstellensatz).

### Strong Hilbert Nullstellensatz

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

For an ideal $I\subseteq k[x_1,\ldots,x_n]$ over an algebraically closed field,

$$
I(V(I))=\sqrt I.
$$

#### Spreading out of an affine zero-set inclusion

↑ **Parent:** [Strong Hilbert Nullstellensatz](#strong-hilbert-nullstellensatz)

Let $I,J\subseteq\mathbb Z[x_1,\ldots,x_n]$. If $V_{\mathbb C}(I)\subseteq V_{\mathbb C}(J)$, then

$$
V_{\overline{\mathbb F}_p}(I\bmod p)\subseteq V_{\overline{\mathbb F}_p}(J\bmod p)
$$

for all but finitely many primes $p$. The Nullstellensatz puts a power of each generator of $J$ in $I\mathbb Q[x_1,\ldots,x_n]$; clearing denominators leaves only finitely many exceptional characteristics.

#### Rabinowitsch trick

↑ **Parent:** [Strong Hilbert Nullstellensatz](#strong-hilbert-nullstellensatz)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rabinowitsch_trick)

To prove the [Strong Hilbert Nullstellensatz](#strong-hilbert-nullstellensatz) from its weak form, adjoin a variable $y$ and the equation $1-yf$. If $f$ vanishes on $V(I)$, the ideal $(I,1-yf)$ has no common zero and is therefore the unit ideal. Substituting $y=f^{-1}$ and clearing denominators yields $f^N\in I$ for some $N$.

### Complex affine algebraic set cardinality dichotomy

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

A complex affine algebraic set is either finite or has the cardinality of $\mathbb C$. One proof takes a positive-dimensional irreducible component and applies [Noether normalization](#noether-normalization): the resulting finite dominant map to a positive-dimensional affine space has a point above every closed point.

### Projective Nullstellensatz

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

Let $I\subseteq k[x_0,\ldots,x_n]$ be a [homogeneous ideal](commutative-algebra.md#homogeneous-ideal) over an [algebraically closed field](algebra.md#algebraically-closed-field), and let

$$
\mathfrak m=(x_0,\ldots,x_n)
$$

be the irrelevant ideal. Then $V_+(I)=\varnothing$ exactly when either $I=(1)$ or $\sqrt I=\mathfrak m$. For a proper homogeneous ideal this is also equivalent to $\mathfrak m^N\subseteq I$ for some $N$.

It is the homogeneous projective version of the [Hilbert Nullstellensatz](#hilbert-nullstellensatz).

#### Graded multiplication map for a projective fiber

↑ **Parent:** [Projective Nullstellensatz](#projective-nullstellensatz)

For homogeneous fiber equations $f_i$ of fixed degrees $d_i$ in $S=k[y_0,\ldots,y_n]$, put $S_j=0$ for $j<0$. The [linear map](vector-space.md#linear-map) $\mu_N((g_i)_i)=\sum_i g_if_i$ has image the degree-$N$ component of their [homogeneous ideal](commutative-algebra.md#homogeneous-ideal). Hence it is surjective exactly when that ideal contains $(y_0,\ldots,y_n)^N$: the degree-$N$ [monomials](polynomial.md#monomial) generate this power. In a family, the [matrix](vector-space.md#matrix) entries are regular functions on the base. Failure of surjectivity is therefore a closed [determinantal variety](#determinantal-variety), cut out by the maximal-size [matrix minors](vector-space.md#minor-linear-algebra).

#### Irrelevant ideal of projective space

↑ **Parent:** [Projective Nullstellensatz](#projective-nullstellensatz)

In the standard graded [homogeneous coordinate ring](projective-space.md#homogeneous-coordinate-ring) $S=k[x_0,\ldots,x_n]$ of $\mathbb P^n$, the irrelevant ideal is

$$
S_+=(x_0,\ldots,x_n).
$$

It vanishes only at the origin of the corresponding [affine cone](#affine-cone), which does not represent a [projective point](projective-space.md#projective-point).

It is the polynomial-ring instance of the [irrelevant ideal of a graded ring](ringed-space.md#irrelevant-ideal-of-a-graded-ring).

### Quasi-compactness of an affine variety

↑ **Parent:** [Hilbert Nullstellensatz](#hilbert-nullstellensatz)

Every open cover of an affine variety has a finite subcover. Refine it by distinguished opens $D(f_i)$. Their complements have no common point, so the Nullstellensatz writes $1$ as a finite combination of the $f_i$; the corresponding finite family of distinguished opens covers.

## Zariski density of the complex exponential graph

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

The graph $\{(x,e^x):x\in\mathbb C\}$ is Zariski dense in $\mathbb A^2_\mathbb C$. If $\sum_jp_j(x)e^{jx}=0$, repeated application of $D-m$ removes the largest exponential term while acting injectively on the others, proving inductively that every $p_j$ vanishes.

## Degree of an algebraic variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Degree_of_an_algebraic_variety)

The degree of a projective [algebraic variety](#algebraic-variety) of dimension $r$ is the length, with [intersection multiplicities](#intersection-multiplicity), of its intersection with a sufficiently general linear subspace of complementary codimension. Equivalently, its [Hilbert polynomial](#hilbert-polynomial) has leading coefficient $\deg X/r!$. For a [projective curve](projective-space.md#projective-curve), a general hyperplane section measures this degree.

### Degree of a projective curve

↑ **Parent:** [Degree of an algebraic variety](#degree-of-an-algebraic-variety)

If the Hilbert polynomial of the homogeneous coordinate ring of a projective curve is

$$
P_C(m)=dm+c,
$$

then $\deg C=d$. Equivalently, a sufficiently general hyperplane section has scheme-theoretic length $d$.

#### Homological degree of a smooth complex plane curve

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)

A smooth compact [Riemann surface](complex-analysis.md#riemann-surfaces) embedded in [Complex projective space](algebraic-topology.md#complex-projective-space) $\mathbb{CP}^2$ determines an integral [homology](homology.md) class $d[\mathbb{CP}^1]$. Since a projective line has self-intersection one, $d$ is the [intersection number](#intersection-number-of-a-cartier-divisor-with-a-curve) with a transverse projective line. Every transverse intersection of complex curves has positive sign, because a complex-linear change of tangent basis has positive real determinant. For the Fermat curve $x^d+y^d=z^d$, the line $y=0$ meets it transversely in the $d$ points $[\zeta:0:1]$, $\zeta^d=1$, directly verifying its homological degree.

#### Genus bound for a nonplanar degree-five curve

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)

The embedding [line bundle](ringed-space.md#line-bundle) has at least four independent [global sections](ringed-space.md#global-section). If it is nonspecial, the [Riemann-Roch theorem](#riemann-roch-theorem) gives $h^0=6-g$, so $g\leq2$. If it is special, the [Clifford inequality for curves](#clifford-inequality-for-curves) gives $h^0\leq3$, a contradiction. The [smooth projective curve](projective-space.md#smooth-projective-curve) need not span its full ambient [projective space](projective-space.md).

<h4 id="bezout-s-theorem">Bézout's theorem</h4>

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bézout's_theorem)

Two [projective plane curves](#projective-plane-curve) of degrees $m$ and $n$ with no common irreducible component have total [intersection multiplicity](#intersection-multiplicity) $mn$. In particular, two nonempty projective plane curves always intersect.

##### Resultant bound for intersections of plane curves

↑ **Parent:** [Bézout's theorem](#bezout-s-theorem)

For [projective plane curves](#projective-plane-curve) without a common [irreducible component](#irreducible-component), project from a point outside both [curves](topology.md#curve). In coordinates where that point is $[1:0:0]$, their defining [homogeneous polynomials](algebra.md#homogeneous-polynomial) have constant nonzero leading coefficients in $X$. The [resultant](polynomial.md#resultant) in $X$ is nonzero by [Gauss's lemma](riemannian-geometry.md#gauss-s-lemma-riemannian-geometry), and is homogeneous of degree $\deg C\deg D$ in the remaining two coordinates. Every intersection projects to one of its zeros. Each projection line has only finitely many intersections with the curves, so their intersection is finite. Choose the center again outside all joining lines of pairs of intersection points; the projection is now injective on that finite set, proving the bound.

##### Projective plane curve

↑ **Parent:** [Bézout's theorem](#bezout-s-theorem)

A projective plane curve is a [projective curve](projective-space.md#projective-curve) embedded in the [projective plane](projective-space.md#projective-plane), usually given by one homogeneous equation.

###### Plane conic

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

A degree-two [projective plane curve](#projective-plane-curve), allowing singular and nonreduced cases. In characteristic different from two, write its equation as $z^{\mathsf T}Mz$ with $M$ a symmetric [matrix](vector-space.md#matrix). It is smooth exactly when $M$ has [matrix rank](vector-space.md#matrix-rank) three. Over an [algebraically closed field](algebra.md#algebraically-closed-field), rank two gives two distinct [projective lines](finite-group-theory.md#projective-line), while rank one gives a double line.

###### Plane quartic

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

A degree-four [projective plane curve](#projective-plane-curve). Its [arithmetic genus](#arithmetic-genus) is three by the [genus-degree formula](#genus-degree-formula); singularities can lower the genus of its [normalization of an algebraic curve](normalization-of-an-algebraic-curve.md).

###### Multiplicity of a plane curve at a point

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

Translate the point to the origin of an affine chart and expand a local defining [polynomial](polynomial.md) as $\sum a_{ij}x^iy^j$. Its lowest nonzero total degree is the multiplicity. A [smooth point of a variety](#smooth-point-of-a-variety) has multiplicity one; a double point has multiplicity two. On a point [blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface), the total transform is the [strict transform of an algebraic subvariety](#strict-transform-of-an-algebraic-subvariety) plus this multiplicity times the [algebraic exceptional divisor](#algebraic-exceptional-divisor).

###### Cohomology of a projective plane hypersurface

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

For a nonzero homogeneous polynomial of degree $d>0$, multiplication gives $0\to\mathcal O_{\mathbb P^2}(-d)\to\mathcal O_{\mathbb P^2}\to i_*\mathcal O_X\to0$. Intermediate cohomology of the twisting sheaves vanishes. The top cohomology of $\mathcal O(-d)$ has Laurent basis $t_0^{-b_0}t_1^{-b_1}t_2^{-b_2}$ with $b_i\geq1$ and $\sum b_i=d$. There are $(d-1)(d-2)/2$ such monomials, with zero basis for $d=1,2$. The long exact sequence gives the displayed dimensions. The calculation allows singular, reducible and nonreduced hypersurfaces; it is an arithmetic-genus calculation, not an assertion about a normalization's genus.

###### An irreducible plane cubic has at most one singular point

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

Two distinct singular points would impose at least two zeros each on the restriction of the cubic to their joining line. A nonzero homogeneous polynomial of degree three cannot have total zero multiplicity four, so that restriction vanishes identically. The line would be a component, contradicting the [irreducible polynomial](polynomial.md#irreducible-polynomial) hypothesis. This argument works in every characteristic.

###### Cayley-Bacharach theorem

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

In its classical nine-point cubic form, the [Cayley-Bacharach theorem](#cayley-bacharach-theorem) says that a cubic through eight of the nine distinct intersections of two plane cubics must contain the ninth. The [eight-point cubic completion for two triples of lines](#eight-point-cubic-completion-for-two-triples-of-lines) is the elementary case needed for triangular-strip propagation in [incidence geometry](combinatorics.md#incidence-geometry). The phenomenon explains why interpolation conditions at such a complete intersection are dependent.

###### Eight-point cubic completion for two triples of lines

↑ **Parent:** [Cayley-Bacharach theorem](#cayley-bacharach-theorem)

Let two triples of projective lines meet in nine distinct points. Any [plane cubic](#plane-cubic) containing eight contains all nine. To prove this, write the triples as $F=L_1L_2L_3$ and $G=M_1M_2M_3$, with the missing point on $L_3$. The candidate cubic $H$ agrees with a scalar multiple of $G$ on $L_1$, so $H-\lambda G=L_1Q$. Its three known zeros on $L_2$ force $Q=L_2L$. Two remaining known zeros on $L_3$ force the linear factor $L$ to be a multiple of $L_3$. Hence $H=\lambda G+\mu F$ and vanishes at the missing point.

###### Cubic propagation along a triangular strip

↑ **Parent:** [Eight-point cubic completion for two triples of lines](#eight-point-cubic-completion-for-two-triples-of-lines)

A two-cell-thick strip of triangles with degree-six vertices in a [dual arrangement of a planar point set](projective-space.md#dual-arrangement-of-a-planar-point-set) produces three indexed primal point families with collinearities $a_i,b_j,c_k$ whenever $i+j+k=0$. A [plane cubic](#plane-cubic) can be fitted to nine initial points because its homogeneous coefficient space has dimension ten. Overlapping nine-point configurations then force each next point onto the same cubic by [eight-point cubic completion for two triples of lines](#eight-point-cubic-completion-for-two-triples-of-lines). Safe neighbourhoods guarantee the distinctness needed in these local completion steps. A possible seed is $a_{-1},a_0,a_1,a_2,b_{-3},b_{-2},b_{-1},c_1,c_2$. Adjacent completion blocks force $c_3,b_{-4},c_4,a_{-2}$, followed by the alternating continuation along the two long transverse families.

###### Smooth plane conic

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

A smooth complex degree-two [projective plane curve](#projective-plane-curve) is a projective linear image of the degree-two [Veronese map](projective-space.md#veronese-map) and is diffeomorphic to a [sphere](geometry-and-topology.md#sphere). Its class in $\mathbb{CP}^2$ is twice the class of a projective line. Its [self-intersection number](#self-intersection-number) is four, so its oriented [normal bundle](#normal-bundle) has [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle) evaluating to four.

###### Dual conic

↑ **Parent:** [Smooth plane conic](#smooth-plane-conic)

The tangent lines of a [smooth plane conic](#smooth-plane-conic) form a [smooth plane conic](#smooth-plane-conic) in the [dual projective space](projective-space.md#dual-projective-space). If the original equation is $v^{\mathsf T}Qv=0$, its tangent has coefficient vector $Qv$, giving the displayed equation. The matrix $Q$ is symmetric and invertible, so this correspondence is a projective linear isomorphism of the conics.

###### Genus one tangent incidence curve of two conics

↑ **Parent:** [Dual conic](#dual-conic)

If two [smooth plane conics](#smooth-plane-conic) over $\mathbb C$ meet at four distinct points, their tangent incidence curve is a smooth projective [genus one curve](normalization-of-an-algebraic-curve.md#genus-one-curve). Projection to $C_2$ is a double cover branched at those four intersections. The tangent equation becomes a quadratic whose discriminant cuts out $C_1\cap C_2$; its four simple zeros make the cover smooth and connected. The [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) then gives genus one.

###### Poncelet porism

↑ **Parent:** [Genus one tangent incidence curve of two conics](#genus-one-tangent-incidence-curve-of-two-conics)

For two [smooth plane conics](#smooth-plane-conic) meeting transversely, the operation of crossing a chord of the second conic tangent to the first and choosing the other tangent through the new endpoint acts as a [translation on an elliptic curve](normalization-of-an-algebraic-curve.md#translation-on-an-elliptic-curve) on their incidence curve. Each switch is an [involution of a degree-two map from a genus one curve](normalization-of-an-algebraic-curve.md#involution-of-a-degree-two-map-from-a-genus-one-curve). One periodic orbit means that the translating point is torsion, so every orbit is periodic with the same least period. The construction extends through coincident choices at ramification points using the regular involutions.

###### Homology of the complement of a smooth conic

↑ **Parent:** [Smooth plane conic](#smooth-plane-conic)

The complement of a closed [tubular neighborhood](differential-geometry.md#tubular-neighborhood) of a [smooth plane conic](#smooth-plane-conic) has the displayed integral [homology](homology.md). The [Excision theorem](homology.md#excision-theorem) and [Thom isomorphism theorem](fiber-bundle.md#thom-isomorphism-theorem) reduce the calculation to the relative long exact sequence: the ambient degree-four [fundamental class](cohomology.md#fundamental-class) restricts with coefficient one, while the degree-two map is intersection with the conic and has coefficient two. A [collar neighborhood](differential-geometry.md#collar-neighbourhood) identifies the open and compact exterior [homotopy equivalence](algebraic-topology.md#homotopy-equivalence) types. The boundary instead has first [homology](homology.md) $\mathbb Z/4$, from the [Gysin sequence](fiber-bundle.md#gysin-sequence-of-a-sphere-bundle) and the normal [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle) four.

###### Plane cubic

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

A plane cubic is a [projective plane curve](#projective-plane-curve) defined by a nonzero homogeneous polynomial of degree three. Its [arithmetic genus](#arithmetic-genus) is one by the [genus-degree formula](#genus-degree-formula), and its [Hilbert polynomial](#hilbert-polynomial) is $3m$. A singular cubic can have normalization of smaller genus; the Hilbert polynomial measures the arithmetic genus.

###### Degenerate cubic containing a line

↑ **Parent:** [Plane cubic](#plane-cubic)

A projective line $L=0$ is contained in the zero locus of the nonzero cubic $L^3$. The union of three lines is given by their product, and a conic together with a line is likewise a [plane cubic](#plane-cubic). Reducibility and repeated factors are permitted in polynomial coverings used in [incidence geometry](combinatorics.md#incidence-geometry); a covering by cubics need not consist of smooth irreducible curves.

###### Real conic without real rational points

↑ **Parent:** [Projective plane curve](#projective-plane-curve)

This smooth [projective plane curve](#projective-plane-curve) has no real [rational points](#rational-point): a sum of three real squares is zero only when all three coordinates vanish, which is forbidden in [projective space](projective-space.md). It is therefore not isomorphic over $\mathbb R$ to the [projective line](finite-group-theory.md#projective-line), which has rational points. Over $\mathbb C$ it becomes a nonsingular conic isomorphic to a projective line. Thus the ground field changes whether a geometric genus-zero curve admits a projective-line parametrization.

###### Genus-degree formula

↑ **Parent:** [Projective plane curve](#projective-plane-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Genus-degree_formula)

The arithmetic genus of a degree-$d$ [projective plane curve](#projective-plane-curve) is

$$
p_a=\frac{(d-1)(d-2)}2.
$$

Equivalently, its structure sheaf has Euler characteristic $\chi(\mathcal O_X)=1-p_a$.

###### Plane curve singularity multiplicity bound

↑ **Parent:** [Genus-degree formula](#genus-degree-formula)

Blow up each distinct singular point of an [integral projective curve](#integral-projective-curve) in the [projective plane](projective-space.md#projective-plane) once. The [arithmetic genus drop under a point blowup](#arithmetic-genus-drop-under-a-point-blowup) and the [genus-degree formula](#genus-degree-formula) give arithmetic genus $(d-1)(d-2)/2-\sum_Pm_P(m_P-1)/2$ for the strict transform. Its [arithmetic genus](#arithmetic-genus) is nonnegative, proving the bound in every characteristic. Infinitely near singularities need not have been resolved.

###### Rationality of a plane quartic with three double points

↑ **Parent:** [Plane curve singularity multiplicity bound](#plane-curve-singularity-multiplicity-bound)

Three distinct points of multiplicity two use the entire [arithmetic genus](#arithmetic-genus) three of an [integral projective curve](#integral-projective-curve) of degree four. One point blowup at each gives [arithmetic genus](#arithmetic-genus) zero. The [normalization of an algebraic curve](normalization-of-an-algebraic-curve.md) then has genus zero and is the [projective line](finite-group-theory.md#projective-line) over an [algebraically closed field](algebra.md#algebraically-closed-field), by [rationality of a smooth projective genus-zero curve](projective-space.md#rationality-of-a-smooth-projective-genus-zero-curve). This allows double points with one branch as well as ordinary nodes.

##### Intersection multiplicity

↑ **Parent:** [Bézout's theorem](#bezout-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_multiplicity)

Intersection multiplicity measures the local order of contact of two algebraic subvarieties. Transverse intersections have multiplicity one.

###### Inflection point of an algebraic plane curve

↑ **Parent:** [Intersection multiplicity](#intersection-multiplicity)

A smooth point of an algebraic plane curve is a flex if its tangent line has [intersection multiplicity](#intersection-multiplicity) at least three there. This definition also applies to smooth points of a singular curve.

###### Hessian criterion for a flex

↑ **Parent:** [Inflection point of an algebraic plane curve](#inflection-point-of-an-algebraic-plane-curve)

For a [plane curve](#plane-curve) defined by a [homogeneous polynomial](algebra.md#homogeneous-polynomial) $F$ of degree $d\ge2$, assume the [field characteristic](algebra.md#characteristic-of-a-field) is different from two and $d-1$ is nonzero in the [field](algebra.md#field). A [smooth point of a variety](#smooth-point-of-a-variety) is a [flex](#inflection-point-of-an-algebraic-plane-curve) exactly when the [determinant](linear-algebra.md#determinant) of the homogeneous [Hessian matrix](calculus.md#hessian-matrix) vanishes there, provided its [tangent line](calculus.md#tangent-line) is not a component. Put the point at $[0:0:1]$ with tangent $y=0$ and $F_y(p)\ne0$. The homogeneous identities give $F_{xz}(p)=F_{zz}(p)=0$ and $F_{yz}(p)=(d-1)F_y(p)$, so the determinant is $-(d-1)^2F_y(p)^2F_{xx}(p)$. In the completed [local ring](commutative-algebra.md#local-ring), write the curve as a [formal power series](commutative-algebra.md#formal-power-series) $y=h(x)$. Its linear coefficient is zero and its quadratic coefficient is $-F_{xx}(p)/(2F_y(p))$. Vanishing of that coefficient is exactly [intersection multiplicity](#intersection-multiplicity) at least three with the tangent, proving the criterion in these positive characteristics as well as in characteristic zero.

###### Hessian curve of a plane cubic

↑ **Parent:** [Hessian criterion for a flex](#hessian-criterion-for-a-flex)

For a cubic [homogeneous polynomial](algebra.md#homogeneous-polynomial) $F$, its [Hessian matrix](calculus.md#hessian-matrix) has linear entries, so its determinant is a cubic [homogeneous polynomial](algebra.md#homogeneous-polynomial), possibly zero. On a [nonsingular plane cubic](#nonsingular-plane-cubic) in characteristic different from two, its zeros are exactly the [flexes](#inflection-point-of-an-algebraic-plane-curve), by the [Hessian criterion for a flex](#hessian-criterion-for-a-flex). If the determinant is nonzero, [Bézout's theorem](#bezout-s-theorem) supplies intersections; if it is zero, the local criterion itself supplies flexes.

#### Hilbert polynomial

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert_polynomial)

The Hilbert function of a finitely generated graded algebra agrees in all sufficiently large degrees with a unique polynomial. For a projective variety of dimension $r$, its leading term is $\deg(V)m^r/r!$.

##### Polynomial bound for sections of a fixed divisor

↑ **Parent:** [Hilbert polynomial](#hilbert-polynomial)

For a [coherent sheaf](ringed-space.md#coherent-sheaf) $\mathcal F$ of support dimension $d$ on a [projective scheme](ringed-space.md#projective-scheme) and a fixed [Cartier divisor](cartier-divisor.md) $D$, $h^0(X,\mathcal F(mD))=O(m^d)$. Choose a sufficiently high ample divisor $A$ whose section avoids the [associated points](ringed-space.md#associated-point-of-a-coherent-sheaf) of $\mathcal F$ and for which $D+A$ is ample. Multiplication by the $m$th power of that section injects $\mathcal F(mD)$ into $\mathcal F(m(D+A))$. The ample [Hilbert polynomial](#hilbert-polynomial), together with [Serre vanishing](ringed-space.md#serre-vanishing), bounds the latter section space by $O(m^d)$.

#### Generic hyperplane section of a projective curve

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)

For a general linear form $\ell$ not vanishing identically on a projective curve, the exact sequence

$$
0\to A_C(-1)\xrightarrow{\ell}A_C\to A_C/(\ell)\to0
$$

shows that the hyperplane-section length is $P_C(m)-P_C(m-1)=\deg C$.

#### Degree under a linear projective embedding

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)

Adjoining projective coordinates that vanish identically does not change the homogeneous coordinate ring or Hilbert polynomial. A linear embedding of projective space therefore preserves the degree of an embedded variety.

#### Embedding dependence of projective degree

↑ **Parent:** [Degree of a projective curve](#degree-of-a-projective-curve)

Projective degree belongs to an embedding rather than to the abstract variety. A line and a smooth conic in $\mathbb P^2$ are both abstractly $\mathbb P^1$ but have degrees one and two.

## Twisted cubic

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Twisted_cubic)

The twisted cubic is the image of

$$
[s:t]\mapsto[s^3:s^2t:st^2:t^3]
$$

in $\mathbb P^3$. Its ideal is generated by the three $2\times2$ minors of

$$
\begin{pmatrix}x_0&x_1&x_2\\x_1&x_2&x_3\end{pmatrix},
$$

and it has degree three.

### Standard monomials of the twisted cubic

↑ **Parent:** [Twisted cubic](#twisted-cubic)

Modulo the three quadric relations of the [twisted cubic](#twisted-cubic), replace $x_1^2$ by $x_0x_2$, $x_2^2$ by $x_1x_3$, and $x_1x_2$ by $x_0x_3$. Each replacement reduces the total exponent of $x_1,x_2$. The resulting monomials are $x_0^ax_3^b$, $x_0^ax_1x_3^b$, and $x_0^ax_2x_3^b$. In degree $m$ their images under $x_i\mapsto s^{3-i}t^i$ are all $3m+1$ distinct monomials of degree $3m$. They are linearly independent, so the three quadrics generate the full [homogeneous ideal](commutative-algebra.md#homogeneous-ideal), not merely its radical. The quotient is the third [Veronese subring](ringed-space.md#veronese-subring) of $k[s,t]$.

### Nondegenerate projective variety

↑ **Parent:** [Twisted cubic](#twisted-cubic)

A projective variety is nondegenerate when it is contained in no hyperplane of its ambient projective space.

### Degree obstruction to the twisted cubic being a complete intersection

↑ **Parent:** [Twisted cubic](#twisted-cubic)

The twisted cubic is a [nondegenerate projective variety](#nondegenerate-projective-variety), so every hypersurface containing it has degree at least two. At least two hypersurfaces are needed to cut out a curve in $\mathbb P^3$, making their degree product at least four rather than the curve's degree three.

## Genus distinguishes equal-degree projective curves

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A twisted cubic and a smooth plane cubic embedded in $\mathbb P^3$ both have degree three, but their genera are zero and one. Thus equal projective degree does not imply isomorphism.

## Zariski tangent space

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zariski_tangent_space)

For $P\in X\subseteq\mathbb A^n$, the Zariski tangent space is the common kernel at $P$ of the differentials of all polynomials in $I(X)$.

### Projective tangent plane

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

For a [smooth algebraic surface](#smooth-algebraic-surface) defined by a [homogeneous polynomial](algebra.md#homogeneous-polynomial) $F$ in [projective space](projective-space.md) of dimension three, its tangent plane at $P$ is the displayed plane. Every [projective line](finite-group-theory.md#projective-line) on the surface through $P$ lies in this plane.

### Embedding dimension distinguishes three-branch curves

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

Three coordinate axes in affine three-space have coordinate ideal $(xy,xz,yz)$; their common point has [embedding dimension](commutative-algebra.md#embedding-dimension) three. Three distinct coplanar lines meeting at one point have embedding dimension two there. An isomorphism preserves the unique point lying on all three irreducible components and preserves the [algebraic cotangent space](#algebraic-cotangent-space), so these two configurations are not isomorphic despite identical component incidence.

### Algebraic cotangent space

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

At a [closed point](topology.md#closed-point) of a [variety](#algebraic-variety) over an [algebraically closed field](algebra.md#algebraically-closed-field), the cotangent space is $\mathfrak m_P/\mathfrak m_P^2$. The [universal property of Kähler differentials](ringed-space.md#universal-property-of-kahler-differentials) identifies its [dual vector space](linear-algebra.md#linear-functional) with $k$-derivations of the [local ring](commutative-algebra.md#local-ring) into the residue field, hence with the [Zariski tangent space](#zariski-tangent-space). The [Kähler differential sheaf](ringed-space.md#sheaf-of-kahler-differentials-over-a-field) has the same fibre because a derivation kills constants and products of two elements of the [maximal ideal](commutative-algebra.md#maximal-ideal).

### Dimension from minimum tangent dimension

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

For an affine variety, its dimension is the minimum of $\dim T_{X,P}$ over its points. A point is smooth when its tangent dimension attains this minimum and singular otherwise.

### Smooth locus of a variety

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

The smooth locus consists of points $P$ for which $\dim T_{X,P}=\dim X$. For an irreducible variety over a perfect field it is a nonempty [Zariski-open subset](#zariski-open-set) and therefore dense.

#### Singular locus

↑ **Parent:** [Smooth locus of a variety](#smooth-locus-of-a-variety)

The closed subset of points where an [algebraic variety](#algebraic-variety) is not smooth. Over a [perfect field](algebra.md#perfect-field) it is equivalently the locus whose [local rings](commutative-algebra.md#local-ring) are not [regular local rings](commutative-algebra.md#regular-local-ring). A [normal variety](ringed-space.md#normal-variety) has no singular points in codimension zero or one.

#### Smooth point of a variety

↑ **Parent:** [Smooth locus of a variety](#smooth-locus-of-a-variety)

Over a [perfect field](algebra.md#perfect-field), a point of a [variety](#algebraic-variety) is smooth when its [local ring](commutative-algebra.md#local-ring) is a [regular local ring](commutative-algebra.md#regular-local-ring). For an [irreducible variety](#irreducible-variety) of dimension $n$ at a [closed point](topology.md#closed-point), this is equivalent to its [Zariski tangent space](#zariski-tangent-space) having dimension $n$. The [Jacobian criterion](#jacobian-criterion) expresses the equality as a matrix-rank condition.

#### Singular point of an algebraic variety

↑ **Parent:** [Smooth locus of a variety](#smooth-locus-of-a-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_point_of_an_algebraic_variety)

A point $p$ of an irreducible variety $X$ is singular when $\dim T_pX>\dim X$. Equivalently, its local ring is not regular. The singular locus is the complement of the smooth locus.

##### Cusp (algebraic geometry)

↑ **Parent:** [Singular point of an algebraic variety](#singular-point-of-an-algebraic-variety)

A unibranch [singular point of an algebraic variety](#singular-point-of-an-algebraic-variety) on a plane [algebraic curve](#algebraic-curve). The ordinary cusp has local equation $y^2=x^3$ and parametrization $(x,y)=(t^2,t^3)$; its branch has a repeated tangent and a vanishing first derivative at the singular point. Higher-order cusps may have different local equations. A [cuspidal cubic](#cuspidal-cubic) gives the basic projective example.

##### Hypersurface singularity

↑ **Parent:** [Singular point of an algebraic variety](#singular-point-of-an-algebraic-variety)

A point on $F=0$ where all first partial derivatives vanish. For a reduced hypersurface this is the [Jacobian criterion](#jacobian-criterion); a nondegenerate quadratic leading part defines an [ordinary double point](#ordinary-double-point).

###### Secant line through singular points of a cubic hypersurface

↑ **Parent:** [Hypersurface singularity](#hypersurface-singularity)

Restrict a cubic equation to the affine line through two distinct singular points. At each point the equation and its first directional derivative vanish, so the restricted polynomial has two distinct double roots. A polynomial of degree at most three with this property is identically zero. Hence the whole line lies in the hypersurface. The multiplicity argument works in every characteristic.

##### Ordinary double point

↑ **Parent:** [Singular point of an algebraic variety](#singular-point-of-an-algebraic-variety)

For a reduced plane [algebraic curve](#algebraic-curve), an ordinary double point is a point whose lowest nonzero local homogeneous term has degree $2$ and factors into two distinct linear factors over an [algebraic closure](algebra.md#algebraic-closure). The two factors give distinct tangent directions. In characteristic not $2$, $x^2+y^2+\text{higher terms}$ is an example.

#### Density of the smooth locus

↑ **Parent:** [Smooth locus of a variety](#smooth-locus-of-a-variety)

If $X\subseteq\mathbb A^n$ is irreducible of dimension $d$, choose a nonzero $(n-d)$-rowed minor of a Jacobian matrix at one point of minimum tangent dimension. Its nonvanishing locus is a nonempty [Zariski-open set](#zariski-open-set) on which the Jacobian has rank $n-d$, so every point there is smooth. Irreducibility makes every nonempty [Zariski-open set](#zariski-open-set) dense.

##### Jacobian criterion

↑ **Parent:** [Density of the smooth locus](#density-of-the-smooth-locus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobian_criterion)

For an affine variety over a perfect field, the tangent-space codimension at a point is the rank of the Jacobian matrix of defining equations. The smooth locus of a pure $d$-dimensional variety in $\mathbb A^N$ is where this rank is $N-d$.

### Singular locus of a product with a smooth variety

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

Since $T_{(x,y)}(X\times Y)=T_xX\oplus T_yY$, if $Y$ is smooth then

$$
\operatorname{Sing}(X\times Y)=\operatorname{Sing}(X)\times Y.
$$

In particular, dimensions add.

### Tangent spaces of a product of two nodal line pairs

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

For

$$
X=Z(x_1^2-x_2^2,x_3^2-x_4^2)\subset\mathbb A^4
$$

in characteristic other than two,

$$
T_PX=\{v:x_1v_1-x_2v_2=0,\ x_3v_3-x_4v_4=0\}.
$$

The variety has dimension two. Its tangent dimension is two when both coordinate pairs are nonzero, three when exactly one pair vanishes, and four at the origin.

### Tangent-space obstruction between two unions of three lines

↑ **Parent:** [Zariski tangent space](#zariski-tangent-space)

The union of the three coordinate axes in $\mathbb A^3$ and a union of three distinct lines through the origin in $\mathbb A^2$ are not [isomorphic](#isomorphism-of-algebraic-varieties). Their origins are intrinsically the unique points common to all three [irreducible components](#irreducible-component), but their [Zariski tangent spaces](#zariski-tangent-space) there have dimensions three and two respectively.

## Krull dimension of an affine variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

The Krull dimension of an affine variety is the supremum of the lengths of strict chains of irreducible closed subsets, equivalently the Krull dimension of its coordinate ring. For an irreducible affine variety it equals the minimum Zariski tangent-space dimension.

### Closed-point dimension lemma for affine domains

↑ **Parent:** [Krull dimension of an affine variety](#krull-dimension-of-an-affine-variety)

If $A$ is a finite-type [integral domain](commutative-algebra.md#integral-domain) over an [algebraically closed field](algebra.md#algebraically-closed-field) and $\dim A=d$, every [maximal ideal](commutative-algebra.md#maximal-ideal) $\mathfrak m$ has [height of a prime ideal](commutative-algebra.md#height-of-a-prime-ideal) $d$. Choose a [Noether normalization](#noether-normalization) $k[z_1,\ldots,z_d]\subset A$. The contraction of $\mathfrak m$ is a [maximal ideal](commutative-algebra.md#maximal-ideal) of the [polynomial ring](commutative-algebra.md#polynomial-ring) and has height $d$; [going-down theorem](commutative-algebra.md#going-down-theorem) lifts its full chain since the [polynomial ring](commutative-algebra.md#polynomial-ring) is [integrally closed domain](commutative-algebra.md#integrally-closed-domain). The upper bound is $\dim A$. A [principal open subset](ringed-space.md#principal-open-subscheme) containing a [closed point](topology.md#closed-point) consequently has dimension $d$, because the whole chain under that point survives [localization](commutative-algebra.md#localization-of-a-ring).

#### Principal hypersurface dimension lemma

↑ **Parent:** [Closed-point dimension lemma for affine domains](#closed-point-dimension-lemma-for-affine-domains)

For an [irreducible variety](#irreducible-variety) which is an [affine variety](#affine-algebraic-set) of dimension $d$ and a nonzero nonunit [regular function](ringed-space.md#regular-function) $f$, each [irreducible component](#irreducible-component) of $V(f)$ has dimension $d-1$. Choose a closed point on just the component in question. In its [local ring](commutative-algebra.md#local-ring) $R$, $\sqrt{(f)}$ is that component's [prime ideal](commutative-algebra.md#prime-ideal). A [system of parameters](commutative-algebra.md#system-of-parameters) of $R/(f)$, lifted and supplemented by $f$, generates a maximal-primary ideal; the [Krull height theorem](commutative-algebra.md#krull-height-theorem) gives $\dim R/(f)\ge d-1$. Extending any chain above $(f)$ by the zero prime of the domain gives the reverse inequality. This proof does not identify dimension with [transcendence degree](algebra.md#transcendence-degree).

### Dimension of an irreducible affine variety by transcendence degree

↑ **Parent:** [Krull dimension of an affine variety](#krull-dimension-of-an-affine-variety)

For an irreducible affine variety $X$ over $k$, its dimension is

$$
\dim X=\operatorname{trdeg}_k k(X),
$$

where $k(X)=\operatorname{Frac}(k[X])$ is its [function field of an algebraic variety](#function-field-of-an-algebraic-variety). An inclusion $k(Y)\hookrightarrow k(X)$ therefore implies $\dim Y\leq\dim X$.

## Affine hypersurface

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

The zero set of a nonconstant polynomial in $n$ affine variables has dimension $n-1$. Passing to the square-free part gives its radical principal ideal.

This is a polynomial-defined [hypersurface](differential-geometry.md#hypersurface) in affine space.

### Smooth point on an irreducible hypersurface in positive characteristic

↑ **Parent:** [Affine hypersurface](#affine-hypersurface)

Let $k$ be algebraically closed of characteristic $p>0$ and let $f\in k[x_1,\ldots,x_n]$ be irreducible. Some partial derivative of $f$ is nonzero: otherwise every exponent is divisible by $p$, and perfection of $k$ would make $f$ a $p$th power. If the gradient vanished at every point of $Z(f)$, the [Strong Hilbert Nullstellensatz](#strong-hilbert-nullstellensatz) would put each partial derivative in $(f)$, impossible by degree. Hence $Z(f)$ has a smooth point and minimum tangent dimension $n-1$.

### Smoothness of a nonzero homogeneous level set

↑ **Parent:** [Affine hypersurface](#affine-hypersurface)

Let $f$ be homogeneous of positive degree $d$ over a field whose characteristic does not divide $d$. The [Euler homogeneous function theorem](real-analysis.md#euler-theorem-for-homogeneous-functions) gives

$$
\sum_i x_i\frac{\partial f}{\partial x_i}=df.
$$

On the level set $f=c\ne0$, the gradient cannot vanish, so $Z(f-c)$ is a smooth hypersurface.

### Tangent hyperplane section

↑ **Parent:** [Affine hypersurface](#affine-hypersurface)

At a smooth point of a hypersurface, restriction to the tangent hyperplane has zero linear term. The natural hyperplane intersection therefore has tangent dimension one larger than its expected dimension and is singular at that point.

### Singular points of an irreducible affine plane cubic

↑ **Parent:** [Affine hypersurface](#affine-hypersurface)

An irreducible affine plane cubic has at most one singular point. If two existed, restriction of its cubic polynomial to their joining line would have a zero of multiplicity at least two at each point. A polynomial of degree at most three cannot have those four zeros unless it vanishes identically, making the line a component and contradicting irreducibility.

### Singular cylinder over a nodal curve

↑ **Parent:** [Affine hypersurface](#affine-hypersurface)

The affine surface

$$
V\bigl(y^2-x(x-1)^2\bigr)\subseteq\mathbb A^3_{x,y,z}
$$

is birational to $\mathbb A^2$ and has singular locus $\{(1,0,z):z\in k\}$, an irreducible affine line.

## Projective hypersurface

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A degree-$d$ projective hypersurface $X_d\subseteq\mathbb P_k^n$ is the [closed subscheme](ringed-space.md#closed-subscheme) cut out by one nonzero homogeneous polynomial of degree $d$.

This is a homogeneous-polynomial [hypersurface](differential-geometry.md#hypersurface) in projective space.

### Plane section

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

The [scheme-theoretic intersection](ringed-space.md#scheme-theoretic-intersection) of a [projective hypersurface](#projective-hypersurface) with a projective plane. If the plane is not contained in the hypersurface, restricting the defining [homogeneous polynomial](algebra.md#homogeneous-polynomial) gives a [projective plane curve](#projective-plane-curve) of the same degree, with possible repeated components.

### Quadric (algebraic geometry)

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadric_(algebraic_geometry))

A projective hypersurface defined by a nonzero homogeneous quadratic form. Over $\mathbb C$, diagonalization identifies its rank; it is smooth when the rank is $N+1$ and otherwise is a cone with a linear vertex.

### Plane quartic with exactly two nodes

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

Over the complex numbers the displayed [projective plane curve](#projective-plane-curve) has precisely two singular points, $[1:0:1]$ and $[-1:0:1]$. At either, with $X=\pm1+u$, $Y=v$, $Z=1$, the leading quadratic term is $4u^2\pm v^2$, so they are [ordinary double points](#ordinary-double-point). The derivative equations in the chart $Y=1$ have no solution: writing $d=X^2-Z^2$ forces both $d^2=-1/16$ and $d^2=1$. The [Bézout theorem](#bezout-s-theorem) proves irreducibility, since a factorization into degrees $r,4-r$ would require at least three intersections, whereas the only possible component intersections are the two transverse [ordinary double points](#ordinary-double-point).

### Projective gradient criterion in characteristic dividing the degree

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

For a reduced [projective hypersurface](#projective-hypersurface) $X=V(f)$ over an algebraically closed field,

$$
\operatorname{Sing}(X)=X\cap V(f_{x_0},\ldots,f_{x_n}).
$$

The [Euler homogeneous function theorem](real-analysis.md#euler-theorem-for-homogeneous-functions) makes the intersection redundant only when the characteristic does not divide the degree. In characteristic $p$, the irreducible polynomial $x_0^p+x_1^{p-1}x_2$ has zero gradient at $[1:0:0]$, which is not on $X$.

### Ideal-sheaf sequence of a projective hypersurface

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

Multiplication by the defining polynomial of a degree-$d$ [projective hypersurface](#projective-hypersurface) gives the short exact sequence

$$
0\longrightarrow\mathcal O_{\mathbb P^n}(-d)
\xrightarrow{\cdot F}\mathcal O_{\mathbb P^n}
\longrightarrow i_*\mathcal O_{X_d}\longrightarrow0.
$$

Thus the ideal sheaf of $X_d$ is $\mathcal O_{\mathbb P^n}(-d)$.

### Affine cone

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_cone)

For a projective algebraic set $X\subseteq\mathbb P^n$, its affine cone is the union in $\mathbb A^{n+1}$ of the lines represented by the points of $X$, together with the origin.

#### Three-dimensional affine quadric cone

↑ **Parent:** [Affine cone](#affine-cone)

The [affine variety](#affine-algebraic-set) $X=V(xy-zw)\subset\mathbb A^4$ has dimension three and a unique [singular point of an algebraic variety](#singular-point-of-an-algebraic-variety) at the origin. The planes $V_X(x,z)$ and $V_X(y,w)$ have dimension two but intersect only at that origin. This is a basic failure of [intersection dimension estimates](#intersection-dimension-bound-on-a-smooth-variety) at singular points.

#### Ruling morphism of the punctured three-dimensional affine quadric cone

↑ **Parent:** [Affine cone](#affine-cone)

On $Y=\{xy=zw\}\setminus\{0\}$, the formulas

$$
[x:w]=[z:y]
$$

glue to a morphism $Y\to\mathbb P^1$. The inverse image of $[0:1]$ is the ruling plane $V(x,z)\cap Y$, so its divisor line bundle is the pullback of $\mathcal O_{\mathbb P^1}(1)$.

### Pencil of plane curves

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

Given homogeneous polynomials $F,G$ of the same degree, their pencil is the one-parameter family

$$
V(sF+tG)\subseteq\mathbb P^2,
\qquad [s:t]\in\mathbb P^1.
$$

Its total space is the [projective hypersurface](#projective-hypersurface) $V(sF+tG)\subseteq\mathbb P^2\times\mathbb P^1$, and projection to $[s:t]$ has these plane curves as its [fibres](#fiber-of-a-morphism).

It is a [pencil](geometry-and-topology.md#pencil-geometry) whose members are plane curves.

#### Fermat cubic curve

↑ **Parent:** [Pencil of plane curves](#pencil-of-plane-curves)

The Fermat cubic $x^3+y^3+z^3=0$ is a [smooth projective curve](projective-space.md#smooth-projective-curve): its three first partial derivatives vanish simultaneously only at the forbidden zero vector. The [genus of a smooth plane curve](#genus-of-a-smooth-plane-curve) formula gives genus one.

This is the degree-three case of a Fermat equation; in general $x^n+y^n+z^n=0$ defines a Fermat curve.

#### Cubic pencil with a triangular member

↑ **Parent:** [Pencil of plane curves](#pencil-of-plane-curves)

The pencil generated by the [Fermat cubic curve](#fermat-cubic-curve) and $xyz=0$ contains both a smooth [genus one](normalization-of-an-algebraic-curve.md#genus-one-curve) curve and the union of the three coordinate lines. Its total space in $\mathbb P^2\times\mathbb P^1$ is irreducible because the two generating cubics have no common factor.

### Affine cone over a projective hypersurface

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

If $X=V_+(F)\subseteq\mathbb P^n$, its affine cone is $Y=V(F)\subseteq\mathbb A^{n+1}$. If $X$ is smooth, every nonzero point of $Y$ is smooth; hence the vertex is the only possible singular point. The vertex is smooth for linear $F$ and singular whenever $\deg F\geq2$.

### Projective quadric cone with one singular vertex

↑ **Parent:** [Projective hypersurface](#projective-hypersurface)

Over an algebraically closed field of characteristic other than two, the rank-$r+1$ quadric

$$
V(X_0^2+\cdots+X_r^2)\subseteq\mathbb P^{r+1}
$$

is an irreducible $r$-dimensional cone for $r\geq2$, and its singular locus is the omitted-coordinate vertex $[0:\cdots:0:1]$.

#### Projective variety with a prescribed-dimensional singular locus

↑ **Parent:** [Projective quadric cone with one singular vertex](#projective-quadric-cone-with-one-singular-vertex)

For $n>k\geq0$, take an $(n-k)$-dimensional irreducible projective variety with one singular point and form its product with $\mathbb P^k$. The Segre embedding makes the product projective, and its singular locus is the singular point times $\mathbb P^k$, of dimension $k$. A quadric cone works in dimension at least two and a cuspidal cubic works in dimension one.

## Determinantal variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Determinantal_variety)

A determinantal variety is cut out by minors imposing an upper bound on matrix rank.

### Smooth projective surface from overlapping rank-one coordinates

↑ **Parent:** [Determinantal variety](#determinantal-variety)

The projective locus where

$$
\begin{pmatrix}y_0&y_1&y_2\\y_2&y_3&y_4\end{pmatrix}
$$

has rank one is cut out by its three $2\times2$ minors. It is a smooth surface: on each of the charts $y_0\ne0$, $y_1\ne0$, $y_3\ne0$, and $y_4\ne0$, the equations eliminate three coordinates and leave two free affine coordinates; these charts cover the locus.

### Rank-one determinantal variety

↑ **Parent:** [Determinantal variety](#determinantal-variety)

The variety of $m\times n$ matrices of rank at most one has dimension $m+n-1$. For $m,n\geq2$, its only singular point is the zero matrix.

## Birational variety

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

Irreducible varieties are birational exactly when they have isomorphic function fields.

This equivalence is the relation studied by [birational geometry](#birational-geometry).

### Blowup of a smooth algebraic surface

↑ **Parent:** [Birational variety](#birational-variety)

Over an algebraically closed [field](algebra.md#field), the [blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface) at a closed point replaces the point by an exceptional [smooth rational curve](projective-space.md#smooth-rational-curve) $E\cong\mathbb P^1$, with $E^2=-1$. Locally it is the [blowup of the affine plane at the origin](#blowup-of-the-affine-plane-at-the-origin). It is a proper [birational morphism](#birational-morphism), an isomorphism off the exceptional curve, and the blown-up surface is again smooth and projective when the original is projective.

#### Canonical divisor formula for a surface blowup

↑ **Parent:** [Blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface)

For a point [blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface) $\psi:\widetilde X\to X$ over an algebraically closed [field](algebra.md#field), with exceptional curve $E$, $K_{\widetilde X}=\psi^*K_X+E$ after choosing compatible representatives. In local coordinates $y=xu$, the differential $dx\wedge dy=x\,dx\wedge du$ has one additional zero along $E$. Thus the formula is valid in every characteristic.

### Birational morphism

↑ **Parent:** [Birational variety](#birational-variety)

A morphism between integral varieties is birational if it induces an isomorphism of their function fields, equivalently an isomorphism on suitable dense open subsets. A proper [birational morphism](#birational-morphism) to a normal variety satisfies $f_*\mathcal O_X=\mathcal O_Y$. For point blowups of smooth surfaces this identifies sections of pulled-back [line bundles](ringed-space.md#line-bundle) by the [projection formula for sheaves](ringed-space.md#projection-formula).

### Birational map

↑ **Parent:** [Birational variety](#birational-variety)

A [rational map](isolated-singularity.md#rational-map-complex-analysis) with a rational inverse restricts to an [isomorphism](algebra.md#isomorphism) of dense open subsets. It may identify or omit exceptional points outside those subsets.

### Blowup of the affine plane at the origin

↑ **Parent:** [Birational variety](#birational-variety)

The blowup of $\mathbb A^2$ at the origin is

$$
\operatorname{Bl}_0\mathbb A^2
=\{((X,Y),[W:Z]):XZ=WY\}\subseteq\mathbb A^2\times\mathbb P^1.
$$

Its projection to $\mathbb A^2$ is an isomorphism away from the origin, while the fiber above the origin is the exceptional curve $\mathbb P^1$.

It is an explicit example of [blowup of an algebraic variety](#blowing-up-algebraic-geometry).

## Normalization of an algebraic curve

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

[This section is present in another page, follow this link to view it.](normalization-of-an-algebraic-curve.md)

## Divisor on an algebraic curve

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A divisor is a finite formal integer combination of closed points. For a divisor $D$,

$$
L(D)=\{f\in k(X)^\times:(f)+D\geq0\}\cup\{0\},
\qquad \ell(D)=\dim_kL(D).
$$

### Riemann-Roch space

↑ **Parent:** [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)

The Riemann-Roch space of a divisor $D$ is the finite-dimensional vector space

$$
L(D)=\{f\in k(X)^\times:(f)+D\geq0\}\cup\{0\}.
$$

Its elements are the [rational functions](isolated-singularity.md#rational-function) whose poles are bounded by the negative coefficients of $D$.

#### Rational functions with prescribed poles

↑ **Parent:** [Riemann-Roch space](#riemann-roch-space)

For finitely many distinct points $P_i$ on a smooth projective genus-$g$ curve, choose $N\ge2g+1$. The [Riemann-Roch theorem](#riemann-roch-theorem) gives $\ell(NP_i)-\ell((N-1)P_i)=1$, so choose $f_i$ with a sole pole of exact order $N$ at $P_i$. Then $\sum_i f_i$ has exactly those poles with that order: all other summands are regular at each $P_i$, so no principal part can cancel. This is an explicit construction rather than an unspecified generic choice of section.

### Degree of a divisor

↑ **Parent:** [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)

For $D=\sum_Pn_PP$ on a curve over an algebraically closed field, its degree is $\deg D=\sum_Pn_P$.

### Linear equivalence of divisors

↑ **Parent:** [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)

Two divisors $D$ and $E$ are linearly equivalent, written $D\sim E$, when $D-E$ is a [principal divisor](#principal-divisor-on-an-algebraic-curve). Multiplication by a rational function whose divisor is $D-E$ gives an isomorphism between their spaces of sections, so $\ell(D)=\ell(E)$.

#### Divisor class

↑ **Parent:** [Linear equivalence of divisors](#linear-equivalence-of-divisors)

A divisor class is an equivalence class of divisors under [linear equivalence](#linear-equivalence-of-divisors). Degree descends to divisor classes because every principal divisor has degree zero.

### Principal divisor on an algebraic curve

↑ **Parent:** [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)

For a nonzero [rational function](isolated-singularity.md#rational-function) $f$ on a [smooth projective curve](projective-space.md#smooth-projective-curve) $C$, its principal divisor is

$$
(f)=\operatorname{div}(f)=\sum_{p\in C}\operatorname{ord}_p(f)p.
$$

It records the zeros of $f$ with positive multiplicity and its poles with negative multiplicity. Every principal divisor has [degree](#degree-of-a-divisor) zero.

#### Principality criterion on a complex elliptic curve

↑ **Parent:** [Principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve)

For $E=\mathbb C/\Lambda$, integrate the logarithmic derivative of an [elliptic function](complex-analysis.md#elliptic-function) and its product with $z$ around a fundamental cell. The first integral forces total degree zero; the second forces the weighted point sum to lie in the lattice. Conversely choose lifts of the points with equal zero and pole sums, and form the balanced ratio of translated [Weierstrass sigma functions](complex-analysis.md#weierstrass-sigma-function). Their quasi-period factors cancel, giving an elliptic function with exactly the prescribed divisor. Separate zero and pole divisors require disjoint support; common terms cancel when only their difference is prescribed.

#### Divisor class on the projective line

↑ **Parent:** [Principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve)

Every degree-zero divisor on the [projective line](finite-group-theory.md#projective-line) is principal. Indeed, if $D=\sum_i a_ip_i$ and $L_i$ is a homogeneous linear form vanishing at $p_i$, then $\sum_i a_i=0$ makes

$$
f=\prod_iL_i^{a_i}
$$

a degree-zero rational function with $(f)=D$. Consequently, two divisors on $\mathbb P^1$ are linearly equivalent exactly when they have the same degree.

#### Principal divisor with one simple zero and one simple pole

↑ **Parent:** [Principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve)

If distinct points $p,q$ on a [smooth projective curve](projective-space.md#smooth-projective-curve) satisfy $(f)=p-q$, then $f:C\to\mathbb P^1$ is a [finite morphism](#finite-morphism) of degree one. Such a morphism between smooth projective curves is an [isomorphism](#isomorphism-of-algebraic-varieties), so $C$ has [genus](normalization-of-an-algebraic-curve.md#geometric-genus) zero. Hence no divisor $p-q$ on a curve of positive genus is principal.

#### Principal divisor criterion on an elliptic curve

↑ **Parent:** [Principal divisor on an algebraic curve](#principal-divisor-on-an-algebraic-curve)

For an elliptic curve with identity $O$, a divisor $D=\sum_Pn_P(P)$ is principal exactly when

$$
\sum_Pn_P=0
\qquad\text{and}\qquad
\sum_P[n_P]P=O.
$$

This is the identification of the degree-zero divisor class group with the elliptic curve.

### Riemann-Roch theorem

↑ **Parent:** [Divisor on an algebraic curve](#divisor-on-an-algebraic-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann–Roch_theorem)

For a smooth projective curve of genus $g$ and a canonical divisor $K$,

$$
\ell(D)-\ell(K-D)=\deg D+1-g.
$$

#### Riemann-Roch via elementary modifications

↑ **Parent:** [Riemann-Roch theorem](#riemann-roch-theorem)

For a closed point $p$ on a [smooth projective curve](projective-space.md#smooth-projective-curve), the quotient in $0\to L(-p)\to L\to L|_p\to0$ has $k$-dimension $[k(p):k]$. Additivity of [Euler characteristic](homology.md#euler-characteristic) therefore changes $\chi(L)$ by that residue-field degree. Every [line bundle](ringed-space.md#line-bundle) is associated with a [divisor](number-theory.md#divisor), so iteration proves the displayed formula. The [dualizing sheaf on a smooth projective curve](ringed-space.md#dualizing-sheaf-on-a-smooth-projective-curve) identifies $h^1(L)$ with $h^0(\Omega^1_C\otimes L^{-1})$ and converts this Euler-characteristic formula into the usual divisor form of [Riemann-Roch theorem](#riemann-roch-theorem).

#### Cohomological proof of Riemann-Roch for curves

↑ **Parent:** [Riemann-Roch theorem](#riemann-roch-theorem)

On a [smooth projective curve](projective-space.md#smooth-projective-curve), the exact sequence $0\to\mathcal O(D-P)\to\mathcal O(D)\to k(P)\to0$ increases the Euler characteristic by one. Iteration for positive and negative coefficients gives $\chi(\mathcal O(D))=\deg D+1-g$. [Serre duality](ringed-space.md#serre-duality) identifies $h^1(\mathcal O(D))$ with $h^0(\mathcal O(K-D))$, proving $\ell(D)-\ell(K-D)=\deg D+1-g$.

#### Clifford inequality for curves

↑ **Parent:** [Riemann-Roch theorem](#riemann-roch-theorem)

If a [line bundle](ringed-space.md#line-bundle) on a [smooth projective curve](projective-space.md#smooth-projective-curve) has both $h^0(\mathcal L)>0$ and $h^0(\omega_C\otimes\mathcal L^{-1})>0$, the displayed inequality holds. Write these dimensions as $r,s$. The [product dimension bound for sections on a curve](#product-dimension-bound-for-sections-on-a-curve) gives $r+s-1\leq g$, and the [Riemann-Roch theorem](#riemann-roch-theorem) gives $r-s=\deg\mathcal L+1-g$. Adding gives $2r\leq\deg\mathcal L+2$.

#### Weierstrass gap

↑ **Parent:** [Riemann-Roch theorem](#riemann-roch-theorem)

At a point $p$ of a [smooth projective curve](projective-space.md#smooth-projective-curve), a positive integer $n$ is a Weierstrass gap when no [rational function](isolated-singularity.md#rational-function) has a pole of order exactly $n$ at $p$ and no other poles. Equivalently,

$$
\ell(np)=\ell((n-1)p).
$$

##### Weierstrass gap theorem

↑ **Parent:** [Weierstrass gap](#weierstrass-gap)

At every point of a smooth projective curve of genus $g$, exactly $g$ positive integers are [Weierstrass gap](#weierstrass-gap). Indeed, each quotient $L(np)/L((n-1)p)$ has dimension zero or one, while [Riemann--Roch](#riemann-roch-theorem) gives $\ell(np)=n+1-g$ for all $n>2g-2$.

###### Genus-two Weierstrass gap sequence

↑ **Parent:** [Weierstrass gap theorem](#weierstrass-gap-theorem)

On a genus-two smooth projective curve, the gap set at any point is either $\{1,2\}$ or $\{1,3\}$. The integer $1$ is always a gap on a positive-genus curve. If $2$ is not a gap, then $3$ must be a gap, since pole orders are closed under addition and $2,3$ would otherwise generate every integer at least two.

#### Canonical divisor

↑ **Parent:** [Riemann-Roch theorem](#riemann-roch-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_divisor)

A canonical divisor is the divisor of any nonzero rational differential. Its divisor class is independent of the differential and has degree $2g-2$.

##### Rational differential on an algebraic curve

↑ **Parent:** [Canonical divisor](#canonical-divisor)

A rational differential on a [smooth projective curve](projective-space.md#smooth-projective-curve) is a rational section of its [canonical bundle](complex-geometry.md#canonical-bundle). In a local coordinate $t$ it has the form $f(t)\,dt$ for a [rational function](isolated-singularity.md#rational-function) $f$.

###### Algebraic residue of a rational differential

↑ **Parent:** [Rational differential on an algebraic curve](#rational-differential-on-an-algebraic-curve)

At a smooth point with local parameter $u$, expand a [rational differential](#rational-differential-on-an-algebraic-curve) as $\sum_j a_j u^jdu$ in the completed local field; its residue is $a_{-1}$. Formal substitution shows this coefficient is independent of the parameter, in arbitrary characteristic. For a finite separable extension of these local fields, residues commute with the differential trace, with a sum over branches. The monogenic trace formula in the [trace-dual module of a finite curve map](#trace-dual-module-of-a-finite-curve-map) proves this compatibility by coefficient extraction.

##### Valuation of a rational differential

↑ **Parent:** [Canonical divisor](#canonical-divisor)

If $t$ is a [uniformizer](commutative-algebra.md#uniformizer) at a point $p$ of a [smooth projective curve](projective-space.md#smooth-projective-curve) and a nonzero rational differential is $\omega=f(t)\,dt$, then $\nu_p(\omega)=\nu_p(f)$. This integer is independent of the chosen uniformizer. Its positive and negative values are respectively the orders of the zero and pole of $\omega$ at $p$.

##### Canonical Riemann-Roch space

↑ **Parent:** [Canonical divisor](#canonical-divisor)

If $K_X=(\omega)$ is represented by a nonzero [rational differential](#rational-differential-on-an-algebraic-curve), multiplication by $\omega$ identifies the [Riemann-Roch space](#riemann-roch-space) $L(K_X)$ with the vector space of [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form). The [Riemann-Roch theorem](#riemann-roch-theorem) gives $\ell(K_X)=g$ for a smooth projective curve of genus $g$.

##### Canonical divisor of the projective line

↑ **Parent:** [Canonical divisor](#canonical-divisor)

For the affine coordinate $t$ on $\mathbb P^1$, put $s=t^{-1}$ at infinity. Since $dt=-s^{-2}ds$,

$$
(dt)=-2\infty,
$$

so $K_{\mathbb P^1}\sim-2\infty$. More generally,

$$
\ell(d\infty)=\max(d+1,0),
$$

because $L(d\infty)$ consists of polynomials of degree at most $d$ when $d\geq0$ and only the zero function when $d<0$.

##### Genus of a smooth plane curve

↑ **Parent:** [Canonical divisor](#canonical-divisor)

A smooth plane curve of degree $d$ has genus

$$
g=\frac{(d-1)(d-2)}2.
$$

###### No smooth plane curve has genus two

↑ **Parent:** [Genus of a smooth plane curve](#genus-of-a-smooth-plane-curve)

If a smooth degree-$d$ [projective plane curve](#projective-plane-curve) had genus two, the [genus-degree formula](#genus-degree-formula) would give $(d-1)(d-2)=4$, equivalently $d^2-3d-2=0$. Its discriminant is $17$, so it has no integral solution for the degree $d$.

###### Smooth plane quartic

↑ **Parent:** [Genus of a smooth plane curve](#genus-of-a-smooth-plane-curve)

A smooth plane quartic is a smooth degree-four curve in $\mathbb P^2$ and has genus three.

The smoothness condition excludes the singular degree-four curves considered in the general plane-quartic family.

###### Projective closure of y cubed equals x to the fourth plus one

↑ **Parent:** [Smooth plane quartic](#smooth-plane-quartic)

The [projective closure](projective-space.md#projective-completion) of the [superelliptic curve](#superelliptic-curve) $y^3=x^4+1$ is the smooth plane quartic

$$
Y^3Z=X^4+Z^4.
$$

Its unique point at infinity is $P_\infty=[0:1:0]$. The rational function $x=X/Z$ defines a degree-three morphism to $\mathbb P^1$ ramified with index three at $P_\infty$ and at the four affine points $(\alpha,0)$ with $\alpha^4=-1$. Its genus is three, and

$$
\operatorname{div}\left(\frac{dx}{y^2}\right)=4P_\infty.
$$

###### Klein quartic

↑ **Parent:** [Smooth plane quartic](#smooth-plane-quartic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klein_quartic)

The Klein quartic has the smooth projective plane model

$$
X^3Y+Y^3Z+Z^3X=0.
$$

Its affine chart $Z=1$ is $x^3y+y^3+x=0$. If $\zeta$ is a primitive seventh root of unity, the projective transformation

$$
[X:Y:Z]\longmapsto[\zeta^3X:\zeta Y:Z]
$$

is an automorphism of order seven.

###### Plane model y plus x cubed plus xy cubed equals zero of the Klein quartic

↑ **Parent:** [Klein quartic](#klein-quartic)

The [projective completion](projective-space.md#projective-completion) of

$$
y+x^3+xy^3=0
$$

is the [smooth plane quartic](#smooth-plane-quartic)

$$
X^3Z+XY^3+YZ^3=0.
$$

The coordinate relabelling $[A:B:C]=[Y:X:Z]$ turns this equation into the standard [Klein quartic](#klein-quartic) equation $A^3B+B^3C+C^3A=0$.

###### Ramification of the x-coordinate on the Klein quartic

↑ **Parent:** [Klein quartic](#klein-quartic)

The coordinate function $x$ has degree three on the Klein quartic. It has ramification index three at $(0,0)$, index two at the seven affine points satisfying $y^7=-3/8$ and $x=2y^3$, and index two at $[0:1:0]$. The total ramification is ten, so the [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) gives genus three.

###### Line section of a smooth plane quartic

↑ **Parent:** [Smooth plane quartic](#smooth-plane-quartic)

For a [smooth plane quartic](#smooth-plane-quartic) $C\subset\mathbb P^2$, the [adjunction formula](complex-geometry.md#adjunction-formula) gives $K_C\cong\mathcal O_C(1)$. Hence every line section $C\cap\ell$ is a [canonical divisor](#canonical-divisor).

###### Gonality of a smooth plane quartic

↑ **Parent:** [Smooth plane quartic](#smooth-plane-quartic)

Projection from a point of a [smooth plane quartic](#smooth-plane-quartic) gives a degree-three map to the [projective line](finite-group-theory.md#projective-line). A degree-two map would make the curve [hyperelliptic](#hyperelliptic-curve), but its [canonical map](#canonical-map-of-a-smooth-plane-curve) is its plane embedding, whereas a hyperelliptic canonical map is not an embedding. Its [gonality](#gonality) is therefore three.

##### Canonical map

↑ **Parent:** [Canonical divisor](#canonical-divisor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_map)

For $g\geq2$, a basis of the space of regular differentials defines the canonical map $X\to\mathbb P^{g-1}$. Equivalently, after choosing a differential with divisor $K$, one may use a basis of $L(K)$.

###### Canonical genus-four curve as a quadric-cubic intersection

↑ **Parent:** [Canonical map](#canonical-map)

For a nonhyperelliptic [smooth projective curve](projective-space.md#smooth-projective-curve) of [geometric genus](normalization-of-an-algebraic-curve.md#geometric-genus) four, the [canonical map](#canonical-map) is an embedding of degree six. Dimension counts $10>h^0(2K)=9$ and $20>h^0(3K)=15$ supply a quadric and a cubic not divisible by it. The quadric is irreducible because the curve is nondegenerate. Degree six and [unmixedness of a complete intersection](ringed-space.md#unmixedness-of-a-complete-intersection) then identify the intersection with the curve as a scheme.

## Gonality

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gonality)

The gonality of a smooth projective curve is the least degree of a nonconstant morphism from the curve to the projective line.

### Trigonal curve

↑ **Parent:** [Gonality](#gonality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trigonal_curve)

A [smooth projective curve](projective-space.md#smooth-projective-curve) of gonality three has a basepoint-free pencil of degree three. For a nonhyperelliptic curve, a fibre of this pencil spans a line in its [canonical map](#canonical-map): [Riemann-Roch theorem](#riemann-roch-theorem) gives $h^0(K_C-D)=g-2$. The union of these lines is a scroll of degree $g-2$ in $\mathbb P^{g-1}$. Its smooth ruled model may map to a cone in low genus.

#### Canonical scroll of a trigonal curve

↑ **Parent:** [Trigonal curve](#trigonal-curve)

The rank-two bundle of fibre spans is globally generated and splits as $\mathcal O(a_1)\oplus\mathcal O(a_2)$ with $a_1+a_2=g-2$. On its [rational normal scroll](fiber-bundle.md#rational-normal-scroll), $L|_C$ is the degree-three pencil and $M|_C=K_C$. The [adjunction formula](complex-geometry.md#adjunction-formula) then forces the displayed divisor class. Writing $a=a_2-a_1$ and $M=B+a_2L$ on the [Hirzebruch surface](toric-geometry.md#hirzebruch-surface) gives $C\in|3B+(a+a_2+2)L|$.

##### Maroni invariant

↑ **Parent:** [Canonical scroll of a trigonal curve](#canonical-scroll-of-a-trigonal-curve)

The difference between the two normalized splitting degrees of the [canonical scroll of a trigonal curve](#canonical-scroll-of-a-trigonal-curve) measures its imbalance. Since a smooth trigonal curve cannot contain the negative section, its intersection with that section is nonnegative. This gives $3a\le g+2$, and parity gives $a\equiv g\pmod2$.

### Gonality bound from Riemann-Roch

↑ **Parent:** [Gonality](#gonality)

For a point $P$ on a smooth projective genus-$g$ curve, [Riemann-Roch space](#riemann-roch-space) $L((g+1)P)$ has dimension at least two. A nonconstant function in it has only a pole at $P$, of order at most $g+1$, and extends to a finite morphism to the projective line. The degree equals the total pole order, including inseparable degree if present. This proves the bound.

## Hyperelliptic curve

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperelliptic_curve)

A hyperelliptic curve of genus at least two admits a degree-two map to $\mathbb P^1$ and can be represented in characteristic other than two by an equation $y^2=f(x)$ with $f$ square-free.

### Even-degree hyperelliptic model

↑ **Parent:** [Hyperelliptic curve](#hyperelliptic-curve)

If $y^2=f(x)$ with $\deg f=2n$, the coordinates

$$
u=x^{-1},\qquad v=yx^{-n}
$$

give the second chart

$$
v^2=u^{2n}f(u^{-1}).
$$

There are two points $P_+,P_-$ above infinity.

#### Compactification of y squared equals x to the eighth minus one

↑ **Parent:** [Even-degree hyperelliptic model](#even-degree-hyperelliptic-model)

The affine germ surface over the plane with the eight roots of unity removed is compactified by adding the eight simple branch points above those roots and two unbranched points above infinity. The degree-two map to the Riemann sphere has total ramification eight, so the [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) gives genus three.

#### Canonical divisor of an even-degree hyperelliptic curve

↑ **Parent:** [Even-degree hyperelliptic model](#even-degree-hyperelliptic-model)

For the smooth curve $y^2=f(x)$ with square-free $f$ of degree $2n$, the differential $dx/y$ has divisor

$$
(n-2)(P_++P_-).
$$

Thus the canonical degree is $2n-4$, the genus is $n-1$, and $L(K)$ has basis $1,x,\ldots,x^{n-2}$.

##### Canonical map of a hyperelliptic curve

↑ **Parent:** [Canonical divisor of an even-degree hyperelliptic curve](#canonical-divisor-of-an-even-degree-hyperelliptic-curve)

The canonical map of an even-degree hyperelliptic curve is

$$
(x,y)\longmapsto[1:x:\cdots:x^{n-2}],
$$

so it identifies the two points $(x,y)$ and $(x,-y)$ of a general fibre and is not an embedding.

## Rational map of projective varieties

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A rational map is a morphism on a dense open subset, considered up to agreement on a smaller dense open subset.

It is the projective-source-and-target case of a [rational map of algebraic varieties](#rational-map-of-algebraic-varieties).

### Indeterminacy locus

↑ **Parent:** [Rational map of projective varieties](#rational-map-of-projective-varieties)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indeterminacy_locus)

The indeterminacy locus is the set where a rational map has no regular local representative.

### Projective Cremona transformation

↑ **Parent:** [Rational map of projective varieties](#rational-map-of-projective-varieties)

A projective Cremona transformation is a birational self-map of projective space, regular on complementary dense open subsets together with its inverse.

Composition of these birational self-maps forms the Cremona group.

## Nonsingular plane cubic

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

A plane cubic is nonsingular when its homogeneous equation and all first partial derivatives have no common projective zero.

### Flex coordinates for a smooth plane cubic

↑ **Parent:** [Nonsingular plane cubic](#nonsingular-plane-cubic)

Put a [flex](#inflection-point-of-an-algebraic-plane-curve) at $[0:1:0]$ with [tangent line](calculus.md#tangent-line) $Z=0$. The tangent section has a triple zero there, so $F(X,Y,0)=aX^3$ with $a\ne0$. Smoothness gives $b\ne0$. In characteristic different from two, replacing $Y$ by $Y+(cX+eZ)/(2b)$ completes the square and produces a [Weierstrass equation of an elliptic curve](normalization-of-an-algebraic-curve.md#weierstrass-equation-of-an-elliptic-curve) using only projective linear coordinate changes.

## Plane curve

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plane_curve)

A plane curve is the zero set of a polynomial in two variables, or a one-dimensional curve embedded in a plane.

### Lemniscate of Bernoulli

↑ **Parent:** [Plane curve](#plane-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lemniscate_of_Bernoulli)

A figure-eight [plane curve](#plane-curve) with two congruent lobes and a crossing at the origin. With scale $a>0$, its polar equation is $r^2=a^2\cos2\theta$. One quarter has coordinates $x=at\sqrt{(1+t^2)/2}$, $y=at\sqrt{(1-t^2)/2}$, $0\leq t\leq1$. Differentiation gives arc element $a\,dt/\sqrt{1-t^4}$. The total [arc length](riemannian-geometry.md#arc-length) is therefore $4a\int_0^1dt/\sqrt{1-t^4}$.

### Astroid

↑ **Parent:** [Plane curve](#plane-curve)

An astroid is the four-cusped [plane curve](#plane-curve) parametrized by $x=a\cos^3t$, $y=a\sin^3t$ for $a>0$. It appears as the relative trajectory in the [astroid motion of a harmonic oscillator in a rotating frame](classical-mechanics.md#astroid-motion-of-a-harmonic-oscillator-in-a-rotating-frame). The parametrization has zero first derivative at the cusps while remaining smooth as a function of its parameter.

<h3 id="plane-cusp-of-type-2-5">Plane cusp of type (2,5)</h3>

↑ **Parent:** [Plane curve](#plane-curve)

This irreducible plane branch has parametrization $x=t^5$, $y=t^2$. Its only singular point is the origin. The [resolution of the (2,5) cusp by two blowups](#resolution-of-the-2-5-cusp-by-two-blowups) makes its [strict transform](complex-geometry.md#strict-transform) smooth in every characteristic.

<h4 id="resolution-of-the-2-5-cusp-by-two-blowups">Resolution of the (2,5) cusp by two blowups</h4>

↑ **Parent:** [Plane cusp of type (2,5)](#plane-cusp-of-type-2-5)

Blow up the origin and use the chart $x=uy$, giving the [strict transform](complex-geometry.md#strict-transform) $u^2-y^3=0$. Blow up its remaining singular point and use $u=vy$, giving $v^2-y=0$, which is smooth because its derivative in $y$ is $-1$. The complementary chart at each stage has no point of the [strict transform](complex-geometry.md#strict-transform) on its exceptional divisor. These two [blowups of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface) resolve the branch, although the smooth transform is still tangent to an exceptional divisor.

### Archimedean spiral

↑ **Parent:** [Plane curve](#plane-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Archimedean_spiral)

An Archimedean spiral has radius linear in polar angle, $r=a+b\theta$. For the special parametrization $(u\cos u,u\sin u)$, the [curvature of a plane curve](differential-geometry.md#curvature-of-a-plane-curve) is $(u^2+2)/(1+u^2)^{3/2}$. Its parameter speed is $\sqrt{1+u^2}$, so it remains a [regular curve](differential-geometry.md#regular-curve) at the origin.

### Superelliptic curve

↑ **Parent:** [Plane curve](#plane-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superelliptic_curve)

A superelliptic curve has an affine equation $y^m=f(x)$. When $f$ is square-free and the characteristic does not divide $m$, projection to the $x$-coordinate is a finite morphism whose finite ramification occurs over the roots of $f$; its behavior at infinity depends on $m$ and $\deg f$.

### Canonical map of a smooth plane curve

↑ **Parent:** [Plane curve](#plane-curve)

For a smooth plane curve of degree $d\geq4$, adjunction gives

$$
K_C\cong\mathcal O_C(d-3).
$$

Its canonical map is induced by the $(d-3)$rd Veronese map and is therefore an embedding.

### Semicubical parabola

↑ **Parent:** [Plane curve](#plane-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semicubical_parabola)

A semicubical parabola is a cusped cubic curve affinely equivalent to $y^2=x^3$.

#### Coordinate ring and singularity of the semicubical parabola

↑ **Parent:** [Semicubical parabola](#semicubical-parabola)

The homomorphism

$$
k[x,y]\to k[t],
\qquad x\mapsto t^2,\quad y\mapsto t^3
$$

has kernel $(y^2-x^3)$ and image $k[t^2,t^3]$. The quotient is therefore an [integral domain](commutative-algebra.md#integral-domain), so the curve is irreducible. In characteristic zero its gradient $(-3x^2,2y)$ vanishes at the origin, making the origin its unique [singular point of an algebraic variety](#singular-point-of-an-algebraic-variety).

## Ramification (mathematics)

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ramification_(mathematics))

Ramification is branching in a geometric or algebraic map, detected by multiplicity greater than one. For [number fields](algebraic-number-theory.md#number-field), [ramification of a prime](algebraic-number-theory.md#ramification-of-a-prime) means that some [prime ideal](commutative-algebra.md#prime-ideal) occurs with exponent greater than one in the extended prime ideal. For a map of smooth [algebraic curves](#algebraic-curve), a local parameter pulls back to a parameter with order greater than one at a ramification point.

### Ramification divisor

↑ **Parent:** [Ramification (mathematics)](#ramification-mathematics)

For a finite morphism $f:X\to Y$ of smooth curves, the ramification divisor is

$$
R_f=\sum_{P\in X}(e_P-1)P.
$$

The [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) states $2g_X-2=(\deg f)(2g_Y-2)+\deg R_f$.

The coefficients assemble the [ramification indices of a morphism of curves](#ramification-index-of-a-morphism-of-curves).

## Product surface without low-genus curves

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

If $C$ is a smooth projective curve of genus at least three, then the smooth projective surface $C\times C$ contains no curve of geometric genus below three. On the normalization of any curve in the product, at least one coordinate projection to $C$ is nonconstant, and the [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) cannot decrease genus.

## Algebraic surface

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_surface)

An algebraic surface is a two-dimensional [algebraic variety](#algebraic-variety). The birational classification of smooth projective surfaces uses their curves, divisor intersections and pluricanonical maps.

### Cubic surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cubic_surface)

A cubic surface is a degree-three [projective hypersurface](#projective-hypersurface) in the [projective space](projective-space.md) $\mathbb P^3$. Over an [algebraically closed field](algebra.md#algebraically-closed-field) every cubic surface contains a projective line. The smooth case has finitely many lines, although the incidence proof of existence does not require smoothness.

#### Smooth cubic surface

↑ **Parent:** [Cubic surface](#cubic-surface)

A [cubic surface](#cubic-surface) with empty [singular locus](#singular-locus). Over an [algebraically closed field](algebra.md#algebraically-closed-field), it is irreducible: distinct positive-degree hypersurface components would meet, and every point of their intersection would be singular in their product equation.

##### Rational parametrization of a cubic surface from two skew lines

↑ **Parent:** [Smooth cubic surface](#smooth-cubic-surface)

For two [skew lines](geometry-and-topology.md#skew-lines) $L,M$ on a [smooth cubic surface](#smooth-cubic-surface), their joining line meets the surface at a third point generically. In coordinates with $L=\{x_2=x_3=0\}$ and $M=\{x_0=x_1=0\}$, write $F(\alpha A+\beta B)=\alpha\beta(\alpha U+\beta V)$. The third point is $[VA-UB]$ whenever $UV\ne0$. Neither $U$ nor $V$ is identically zero, because that would make one of the two lines singular on the surface. The inverse records $[x_0:x_1]$ and $[x_2:x_3]$ of a general surface point. Thus the surface is [birational](#birational-variety) to $\mathbb P^1\times\mathbb P^1$, hence to $\mathbb P^2$.

##### Conic bundle from a line on a smooth cubic surface

↑ **Parent:** [Smooth cubic surface](#smooth-cubic-surface)

Write a line as $L=\{x_2=x_3=0\}$ and the surface equation as $F=x_2Q_2+x_3Q_3$. Smoothness says $A=Q_2|_L$, $B=Q_3|_L$ have no common zero. Projection $[x_2:x_3]$ extends over $L$ by $[-B:A]$. Its fibres are the residual [plane conics](#plane-conic) in the planes through $L$, since substituting $x_2=sw$, $x_3=tw$ gives $F=w(sQ_2+tQ_3)$. Different residual conics are disjoint everywhere, including their points on $L$, because they are fibres of one [morphism of algebraic varieties](#morphism-of-algebraic-varieties). The family is flat: over the smooth base curve its local rings are torsion-free over the corresponding [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring); smoothness of the total surface supplies the reduced-fibre conclusions.

###### Discriminant quintic of a cubic surface conic bundle

↑ **Parent:** [Conic bundle from a line on a smooth cubic surface](#conic-bundle-from-a-line-on-a-smooth-cubic-surface)

The matrix of the residual [plane conic](#plane-conic) in coordinates $(u,v,w)$ has coefficient degrees $\left(\begin{smallmatrix}1&1&2\\1&1&2\\2&2&3\end{smallmatrix}\right)$ in the plane parameter $(s,t)$. Every term of its [determinant](linear-algebra.md#determinant) has degree five. The [reduced singular fibres of a smooth conic bundle](#reduced-singular-fibres-of-a-smooth-conic-bundle) lemma rules out an identically zero determinant and makes each zero simple. Over an [algebraically closed field](algebra.md#algebraically-closed-field), there are therefore exactly five singular fibres, each a pair of distinct coplanar [projective lines](finite-group-theory.md#projective-line). No residual conic contains the original line, because $sA+tB\equiv0$ would make $A,B$ proportional and force a common zero. Pairs from different fibres are disjoint.

##### Lines through a point of a smooth cubic surface

↑ **Parent:** [Smooth cubic surface](#smooth-cubic-surface)

Every [projective line](finite-group-theory.md#projective-line) through $P$ on a [smooth cubic surface](#smooth-cubic-surface) lies in its [projective tangent plane](#projective-tangent-plane). Each is a distinct linear factor of the cubic [plane section](#plane-section). There can therefore be at most three. Equality occurs when the tangent section consists of three concurrent lines.

### Exceptional curve of a surface resolution

↑ **Parent:** [Algebraic surface](#algebraic-surface)

An exceptional curve of a surface resolution is an irreducible curve on the smooth resolving surface that maps to a point on the original normal surface. For an affine toric surface resolved by fan subdivision, the interior inserted rays give these proper curves. Each has a complete one-dimensional star and is isomorphic to the projective line.

### Smooth algebraic surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)

A smooth algebraic surface is a two-dimensional [smooth variety](#smooth-algebraic-variety). Its local rings are regular, and its integral curves define [Cartier divisors](cartier-divisor.md).

#### Arithmetic adjunction formula on a smooth surface

↑ **Parent:** [Smooth algebraic surface](#smooth-algebraic-surface)

For an integral curve $C$ on a [smooth projective surface](#smooth-projective-surface), $2p_a(C)-2=C\cdot(C+K_X)$. Apply [Riemann–Roch theorem for algebraic surfaces](#riemann-roch-theorem-for-algebraic-surfaces) to the [divisor restriction exact sequence](cartier-divisor.md#divisor-restriction-exact-sequence) $0\to\mathcal O_X(-C)\to\mathcal O_X\to\mathcal O_C\to0$ to derive it. This arithmetic version applies also to singular curves and in arbitrary characteristic.

##### Arithmetic genus drop under a point blowup

↑ **Parent:** [Arithmetic adjunction formula on a smooth surface](#arithmetic-adjunction-formula-on-a-smooth-surface)

For an [integral projective curve](#integral-projective-curve) on a [smooth projective surface](#smooth-projective-surface), blowing up a point of multiplicity $m$ gives $C'=\pi^*C-mE$. The [intersection formula for blowing up a surface](#intersection-formula-for-blowing-up-a-surface) and [canonical divisor formula for a surface blowup](#canonical-divisor-formula-for-a-surface-blowup) yield $C'^2=C^2-m^2$ and $K_{X'}\cdot C'=K_X\cdot C+m$. Substitute both in the [arithmetic adjunction formula on a smooth surface](#arithmetic-adjunction-formula-on-a-smooth-surface). This does not require the transformed [curve](topology.md#curve) to be smooth.

#### Smooth projective surface

↑ **Parent:** [Smooth algebraic surface](#smooth-algebraic-surface)

A [smooth projective surface](#smooth-projective-surface) is a two-dimensional [smooth variety](#smooth-algebraic-variety) admitting a closed embedding in [projective space](projective-space.md). Its integral curves are [Cartier divisors](cartier-divisor.md), and their intersections, arithmetic adjunction and point blowups control its birational geometry.

<h5 id="noether-lefschetz-theorem">Noether–Lefschetz theorem</h5>

↑ **Parent:** [Smooth projective surface](#smooth-projective-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noether–Lefschetz_theorem)

A [very general](#very-general-point-of-an-algebraic-parameter-space) smooth degree-$d$ surface $X\subset\mathbb P^3_{\mathbb C}$ with $d\geq4$ has [Picard group](ringed-space.md#picard-group) generated by its hyperplane class. The exceptional surfaces lie in a countable union of proper closed loci. A proof is given by [Griffiths and Harris, "On the Noether-Lefschetz Theorem"](https://publications.ias.edu/sites/default/files/noether.pdf).

###### Very general surface of degree at least four has no smooth rational curve

↑ **Parent:** [Noether–Lefschetz theorem](#noether-lefschetz-theorem)

The [Noether–Lefschetz theorem](#noether-lefschetz-theorem) makes any curve class a positive multiple of the hyperplane class, with positive self-intersection. But the [smooth rational-curve self-intersection on a projective hypersurface](complex-geometry.md#smooth-rational-curve-self-intersection-on-a-projective-hypersurface) formula makes every smooth rational curve have self-intersection at most $-2$ when the surface degree is at least four. Thus none exists. The smoothness condition is essential; this does not prohibit singular curves whose normalizations are rational.

##### Negative curve on a projective surface

↑ **Parent:** [Smooth projective surface](#smooth-projective-surface)

A negative curve is an irreducible [algebraic curve](#algebraic-curve) on a smooth projective surface whose [self-intersection number](#self-intersection-number) is negative. The negativity prevents it from moving in a nontrivial effective linear system and constrains how many curves can represent a fixed numerical class.

###### Countability of negative curves

↑ **Parent:** [Negative curve on a projective surface](#negative-curve-on-a-projective-surface)

Distinct [negative curves](#negative-curve-on-a-projective-surface) cannot have the same integral cohomology class: their mutual intersection would equal a negative self-intersection, contradicting nonnegative [intersection multiplicities](#intersection-multiplicity) for distinct curves. A smooth complex projective surface has finitely generated integral [cohomology groups](cohomology.md#cohomology-group), so its negative curves form an at most countable set. Zero-self-intersection curves need not obey this restriction: one ruling of $\mathbb P^1\times\mathbb P^1$ gives an uncountable family.

###### Rigidity of a negative curve

↑ **Parent:** [Negative curve on a projective surface](#negative-curve-on-a-projective-surface)

If an [effective divisor](cartier-divisor.md#effective-cartier-divisor) $D$ is [linearly equivalent](#linear-equivalence-of-weil-divisors) to a [negative curve](#negative-curve-on-a-projective-surface) $C$, then $D=C$. Otherwise $D\cdot C=C^2<0$ forces $C$ to be a component of $D$, since distinct irreducible curves have nonnegative [intersection multiplicities](#intersection-multiplicity). Write $D=C+D'$ with $D'$ effective and linearly equivalent to zero. An [ample divisor](cartier-divisor.md#ample-cartier-divisor) intersects $D'$ positively unless $D'=0$, while linear equivalence forces that intersection to vanish.

##### Castelnuovo contraction criterion

↑ **Parent:** [Smooth projective surface](#smooth-projective-surface)

A [smooth rational curve](projective-space.md#smooth-rational-curve) with self-intersection $-1$ on a [smooth projective surface](#smooth-projective-surface) over an algebraically closed field contracts to a smooth point of another [smooth projective surface](#smooth-projective-surface). The contraction is a [birational morphism](#birational-morphism) and an isomorphism off the curve, with inverse a [blowup of a smooth algebraic surface](#blowup-of-a-smooth-algebraic-surface). This algebraic criterion is valid in arbitrary characteristic and should not be confused with Castelnuovo's rationality criterion.

<h3 id="riemann-roch-theorem-for-algebraic-surfaces">Riemann–Roch theorem for algebraic surfaces</h3>

↑ **Parent:** [Algebraic surface](#algebraic-surface)

For a [Cartier divisor](cartier-divisor.md) on a smooth projective surface, the displayed formula computes its [Euler characteristic of a coherent sheaf](ringed-space.md#euler-characteristic-of-a-coherent-sheaf). Combined with [Serre duality](ringed-space.md#serre-duality), it turns [intersection numbers](#intersection-number-of-a-cartier-divisor-with-a-curve) into lower bounds for section spaces.

#### Noether formula

↑ **Parent:** [Riemann–Roch theorem for algebraic surfaces](#riemann-roch-theorem-for-algebraic-surfaces)

For a smooth compact complex surface, the degree-four part of its Todd class is $(c_1^2+c_2)/12$. Applying Riemann–Roch to its structure sheaf gives the formula. For a [K3 surface](complex-geometry.md#k3-surface), $c_1=0$ and $\chi(\mathcal O_X)=2$, so its topological Euler characteristic is $c_2=24$.

### Intersection pairing on the Picard group of a surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)

On a smooth projective surface, two [line bundles](ringed-space.md#line-bundle) are represented by divisors $D$ and $E$, and their intersection is the degree of the zero-cycle obtained after moving them into proper position. It is a symmetric bilinear form on the [Picard group](ringed-space.md#picard-group), and $D\cdot E$ equals the degree of $\mathcal O_X(D)$ restricted to $E$ when $E$ is an integral curve not contained in $D$.

#### Hodge index theorem for algebraic surfaces

↑ **Parent:** [Intersection pairing on the Picard group of a surface](#intersection-pairing-on-the-picard-group-of-a-surface)

For a smooth projective surface and an ample divisor $A$, the [intersection pairing on the Picard group of a surface](#intersection-pairing-on-the-picard-group-of-a-surface) is negative definite on the orthogonal complement of $[A]$ in $N^1(X)_{\mathbb R}$. Its signature is $(1,\rho-1)$. This is an algebraic statement valid in arbitrary characteristic, distinct from its analytic formulation for compact Kähler surfaces.

##### Contracted curve has negative self-intersection

↑ **Parent:** [Hodge index theorem for algebraic surfaces](#hodge-index-theorem-for-algebraic-surfaces)

Let a surjective morphism from a smooth projective surface to a projective surface contract an irreducible curve $C$. Pull back an [ample divisor](cartier-divisor.md#ample-cartier-divisor) $H$ from the target to obtain $L$. The [projection formula for algebraic cycles](#projection-formula-for-algebraic-cycles) gives $L\cdot C=0$ and $L^2=\deg(f)H^2>0$. The [Hodge index theorem for algebraic surfaces](#hodge-index-theorem-for-algebraic-surfaces) makes the intersection form negative definite on the orthogonal complement of this positive-square class. Since an ample divisor on the source meets $C$ positively, its numerical class is nonzero, and $C^2<0$.

##### Isotropic orthogonality consequence of the Hodge index theorem

↑ **Parent:** [Hodge index theorem for algebraic surfaces](#hodge-index-theorem-for-algebraic-surfaces)

If $D$ is nonzero numerically with $D^2=0$ and $D\cdot A>0$ for ample $A$, then $D\cdot E=0$ implies $E^2\leq0$, with equality only when $[E]$ is proportional to $[D]$. To see this, use the [Hodge index theorem for algebraic surfaces](#hodge-index-theorem-for-algebraic-surfaces) to split off the positive $A$ direction and diagonalize the remaining negative definite form. Orthogonality to a nonzero isotropic vector then leaves a negative semidefinite form whose radical is precisely that vector's span.

#### Picard lattice of a Hirzebruch surface

↑ **Parent:** [Intersection pairing on the Picard group of a surface](#intersection-pairing-on-the-picard-group-of-a-surface)

For the [Hirzebruch surface](toric-geometry.md#hirzebruch-surface) $\mathbb F_n$, the [negative section of a Hirzebruch surface](toric-geometry.md#negative-section-of-a-hirzebruch-surface) $S$ and a [fiber class of a Hirzebruch surface](toric-geometry.md#fiber-class-of-a-hirzebruch-surface) $F$ freely generate $\operatorname{Pic}(\mathbb F_n)$ and satisfy

$$
S^2=-n,\qquad S\cdot F=1,\qquad F^2=0.
$$

### Intersection formula for blowing up a surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)

If $\pi:\widetilde X\to X$ blows up a smooth point with exceptional curve $E$, then

$$
\operatorname{Pic}(\widetilde X)=\pi^*\operatorname{Pic}(X)\oplus\mathbb ZE,
\qquad E^2=-1,
\qquad \pi^*D\cdot E=0.
$$

If a curve $C$ has multiplicity $m$ at the center, its strict transform is $\widetilde C=\pi^*C-mE$ and $\widetilde C^2=C^2-m^2$.

#### Isotropic divisor from a nontrivial birational morphism to the projective plane

↑ **Parent:** [Intersection formula for blowing up a surface](#intersection-formula-for-blowing-up-a-surface)

Every nonisomorphic birational morphism from a smooth projective surface to $\mathbb P^2$ factors into point blowups. If $H$ is the pullback of a line and $E$ is the total transform of an exceptional divisor from one factor, then $H^2=1$, $E^2=-1$ and $H\cdot E=0$, so $(H+E)^2=0$.

#### Self-intersection after blowing up points on a smooth curve

↑ **Parent:** [Intersection formula for blowing up a surface](#intersection-formula-for-blowing-up-a-surface)

Blowing up $r$ distinct smooth points of a smooth curve $C$ gives a strict transform $C'$ isomorphic to $C$ with

$$
(C')^2=C^2-r.
$$

Choosing $r>C^2$ turns a curve of positive self-intersection into one of negative self-intersection without changing its abstract isomorphism type.

### Morphism from the projective plane contracting a line

↑ **Parent:** [Algebraic surface](#algebraic-surface)

Every morphism $f:\mathbb P^2\to\mathbb P^n$ satisfies $f^*\mathcal O(1)\cong\mathcal O(d)$ for some $d\geq0$. If $f$ contracts a line, restriction to that line makes $\mathcal O(d)$ trivial, hence $d=0$ and all defining sections are constant. Thus the entire morphism is constant.

### Exceptional curve of the first kind

↑ **Parent:** [Algebraic surface](#algebraic-surface)

An exceptional curve of the first kind is a smooth rational curve $E$ on a smooth surface with $E^2=-1$. It can be contracted to a smooth point.

This is precisely the curve contracted by the [Castelnuovo contraction criterion](#castelnuovo-contraction-criterion).

#### Minimal algebraic surface

↑ **Parent:** [Exceptional curve of the first kind](#exceptional-curve-of-the-first-kind)

A smooth projective surface is minimal when it contains no [exceptional curve of the first kind](#exceptional-curve-of-the-first-kind).

Minimality here is the smooth-surface condition, rather than a claim about every higher-dimensional minimal model.

##### Abelian surface

↑ **Parent:** [Minimal algebraic surface](#minimal-algebraic-surface)

An abelian surface is a two-dimensional [abelian variety](abelian-variety.md). It contains no rational curve: a morphism from $\mathbb P^1$ to an abelian variety is constant. Consequently every abelian surface is a [minimal algebraic surface](#minimal-algebraic-surface).

###### Ample curve on an abelian surface generates the surface

↑ **Parent:** [Abelian surface](#abelian-surface)

Let $C$ be a smooth connected [ample](ringed-space.md#ample-line-bundle) curve in an [abelian surface](#abelian-surface) $A$. Translate its chosen basepoint to zero and apply the [universal property of the Jacobian variety](abelian-variety.md#universal-property-of-the-jacobian-variety). The image of $J(C)\to A$ is a closed connected algebraic subgroup containing the translated curve. If it had dimension one, that curve would be the subgroup itself; a distinct coset is disjoint and numerically equivalent, forcing $C^2=0$. This contradicts ampleness, so the homomorphism is surjective.

##### Minimal Hirzebruch surface

↑ **Parent:** [Minimal algebraic surface](#minimal-algebraic-surface)

The [Hirzebruch surface](toric-geometry.md#hirzebruch-surface) $\mathbb F_n$ is minimal for $n=0$ and every $n\geq2$; $\mathbb F_1$ is not minimal because its negative section is a $(-1)$-curve. For $n>0$, the negative section is the unique irreducible curve of negative self-intersection, so its self-intersection $-n$ distinguishes the isomorphism class. The surfaces $\mathbb F_n$ for $n\geq2$ therefore give infinitely many pairwise nonisomorphic minimal rational surfaces.

### Elliptic surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptic_surface)

An elliptic surface is a smooth projective surface equipped with a surjective morphism to a smooth curve whose generic fiber is a smooth curve of genus one.

#### Elliptic surface of Kodaira dimension minus infinity

↑ **Parent:** [Elliptic surface](#elliptic-surface)

For an elliptic curve $E$, projection $\mathbb P^1\times E\to\mathbb P^1$ is an elliptic fibration. Its canonical bundle is the pullback of $K_{\mathbb P^1}$, so it has no nonzero pluricanonical sections and its [Kodaira dimension](#kodaira-dimension) is $-\infty$.

### Kodaira dimension

↑ **Parent:** [Algebraic surface](#algebraic-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kodaira_dimension)

The Kodaira dimension measures the asymptotic growth of the pluricanonical spaces $H^0(X,K_X^{\otimes m})$. For a surface it takes values $-\infty,0,1,2$.

#### Surface of general type

↑ **Parent:** [Kodaira dimension](#kodaira-dimension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_of_general_type)

A smooth projective surface is of general type when its [Kodaira dimension](#kodaira-dimension) is two, equivalently when its canonical divisor is big.

##### Double plane of general type

↑ **Parent:** [Surface of general type](#surface-of-general-type)

Let $B\subseteq\mathbb P^2$ be a smooth curve of degree $2d$, and let $\pi:X\to\mathbb P^2$ be the double cover branched along $B$. Then

$$
K_X=\pi^*(K_{\mathbb P^2}+dH)=\pi^*((d-3)H).
$$

For $d\geq4$ this canonical divisor is ample, so $X$ is a [surface of general type](#surface-of-general-type). A smooth octic branch curve gives the first such example.

### Irregularity of an algebraic surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)

The irregularity of a smooth projective complex surface is

$$
q(X)=h^1(X,\mathcal O_X)=h^0(X,\Omega_X^1).
$$

#### Irregularity of a product of curves

↑ **Parent:** [Irregularity of an algebraic surface](#irregularity-of-an-algebraic-surface)

For smooth projective curves $C$ and $D$, the [Künneth theorem](cohomology.md#kunneth-theorem) gives

$$
q(C\times D)=g(C)+g(D).
$$

#### Smooth projective hypersurface has zero irregularity

↑ **Parent:** [Irregularity of an algebraic surface](#irregularity-of-an-algebraic-surface)

A smooth surface hypersurface $X_d\subseteq\mathbb P^3$ has $q(X_d)=0$. This follows from the [structure-sheaf sequence of a hypersurface](ringed-space.md#structure-sheaf-sequence-of-a-hypersurface) and the vanishing of the intermediate cohomology of line bundles on $\mathbb P^3$.

##### Product of positive-genus curves is not a projective hypersurface

↑ **Parent:** [Smooth projective hypersurface has zero irregularity](#smooth-projective-hypersurface-has-zero-irregularity)

If $C$ and $D$ have positive genus, then $q(C\times D)=g(C)+g(D)>0$, whereas every smooth surface hypersurface in projective space lies in $\mathbb P^3$ and has irregularity zero. Hence $C\times D$ is not isomorphic to a projective hypersurface.

### Geometric genus of an algebraic surface

↑ **Parent:** [Algebraic surface](#algebraic-surface)

The geometric genus of a smooth projective surface is

$$
p_g(X)=h^0(X,K_X)=h^2(X,\mathcal O_X).
$$

#### Birational invariance of the geometric genus of a surface

↑ **Parent:** [Geometric genus of an algebraic surface](#geometric-genus-of-an-algebraic-surface)

If $\pi:\widetilde X\to X$ is the blowup of a smooth surface at a point, then $K_{\widetilde X}=\pi^*K_X+E$ and $\pi_*K_{\widetilde X}=K_X$. Pullback therefore identifies the global holomorphic two-forms and gives $p_g(\widetilde X)=p_g(X)$.

### Albanese variety

↑ **Parent:** [Algebraic surface](#algebraic-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Albanese_variety)

The Albanese variety of a smooth projective variety $X$ is the universal abelian variety receiving a morphism from $X$ after a base point is chosen. Over the complex numbers its dimension is $q(X)$.

#### Irregularity from a smooth Albanese curve image

↑ **Parent:** [Albanese variety](#albanese-variety)

If the image of the Albanese morphism of a surface is a smooth curve $C$ of genus $g$, then $q(X)=g$. Pullback of one-forms from $C$ gives $g\leq q(X)$, while the universal property gives a surjection from the Jacobian of $C$ onto $\operatorname{Alb}(X)$ and hence $q(X)\leq g$.

## Projection of a plane curve from an exterior point

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

After coordinates place $p=[0:0:1]$, projection away from $p$ is $[x:y:z]\mapsto[x:y]$. Its restriction to a plane curve avoiding $p$ is a morphism to $\mathbb P^1$ whose degree equals the degree of the curve.

## Projection from a point on a plane curve

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

For a degree-$d$ plane curve $C$ and a smooth point $p\in C$, the pencil of lines through $p$ induces a morphism $C\to\mathbb P^1$. A general line has one fixed intersection at $p$, so [Bézout theorem](#bezout-s-theorem) makes the morphism have degree $d-1$.

## Toric geometry

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)

[This section is present in another page, follow this link to view it.](toric-geometry.md)

## Intersection theory

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Intersection_theory)

Intersection theory studies algebraic cycles modulo rational equivalence and their products.

### Intersection dimension bound on a smooth variety

↑ **Parent:** [Intersection theory](#intersection-theory)

For closed irreducible subvarieties $Y,Z$ of a smooth $d$-dimensional [algebraic variety](#algebraic-variety) $X$, every [irreducible component](#irreducible-component) of their intersection has dimension at least $\dim Y+\dim Z-d$. Locally the diagonal of $X\times X$ is cut out by $d$ parameters. Intersecting it with $Y\times Z$ and applying the [Krull height theorem](commutative-algebra.md#krull-height-theorem) gives the bound. The [three-dimensional affine quadric cone](#three-dimensional-affine-quadric-cone) shows that the same lower bound can fail when $X$ is singular.

### Intersection product of Cartier divisors

↑ **Parent:** [Intersection theory](#intersection-theory)

Successive intersection with [Cartier divisors](cartier-divisor.md) gives a cycle class. On an $n$-dimensional complete scheme, its degree is multilinear and depends only on numerical divisor classes; the top product with one divisor is its [self-intersection number](#self-intersection-number).

#### Projection formula for algebraic cycles

↑ **Parent:** [Intersection product of Cartier divisors](#intersection-product-of-cartier-divisors)

For a proper [morphism of varieties](#morphism-of-algebraic-varieties) $f:X\to Y$, a [Cartier divisor](cartier-divisor.md) $D$ on $Y$, and an [algebraic cycle](#algebraic-cycle) $\alpha$ on $X$, pullback of $D$, intersection with $\alpha$, and proper pushforward satisfy the displayed identity in the [Chow group](#chow-group). In particular, for a [generically finite morphism](#generically-finite-morphism) of surfaces of degree $r$, $(f^*D)^2=rD^2$. For a curve $C$ contracted to a point, $f_*C=0$, so $f^*D\cdot C=0$.

### Intersection number of a Cartier divisor with a curve

↑ **Parent:** [Intersection theory](#intersection-theory)

The intersection number $D\cdot C$ is the degree of the restriction of $\mathcal O_X(D)$ to the complete integral curve $C$. On a smooth surface, proper effective intersections are sums of local [intersection multiplicities](#intersection-multiplicity).

#### Self-intersection of an algebraic curve

↑ **Parent:** [Intersection number of a Cartier divisor with a curve](#intersection-number-of-a-cartier-divisor-with-a-curve)

For a proper integral Cartier curve $C$ on a smooth algebraic surface, its self-intersection is $\deg\mathcal O_C(C)$. If $C$ is smooth, this is the degree of its normal line bundle. It is defined over any algebraically closed field, without requiring an associated real or complex manifold.

// Target: geometry-and-topology.bigb

### Algebraic cycle

↑ **Parent:** [Intersection theory](#intersection-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_cycle)

A $k$-cycle on a scheme $X$ is a finite integer linear combination of integral closed subschemes of dimension $k$. Their free abelian group is denoted $Z_k(X)$.

#### Rational equivalence

↑ **Parent:** [Algebraic cycle](#algebraic-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_equivalence)

Rational equivalence is generated by principal divisors $[\operatorname{div}(r)]$ of nonzero rational functions on integral subvarieties one dimension larger than the cycles.

##### Chow group

↑ **Parent:** [Rational equivalence](#rational-equivalence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chow_group)

The Chow group is $A_k(X)=Z_k(X)/\operatorname{Rat}_k(X)$, the group of $k$-dimensional algebraic cycles modulo rational equivalence.

###### Chow class

↑ **Parent:** [Chow group](#chow-group)

The equivalence class of an [algebraic cycle](#algebraic-cycle) modulo [rational equivalence](#rational-equivalence). The [Chow group](#chow-group) consists of these classes with addition induced by adding cycles.

###### Cycle class map

↑ **Parent:** [Chow group](#chow-group)

For a smooth complex projective [algebraic variety](#algebraic-variety), the cycle class map sends an [algebraic cycle](#algebraic-cycle) of codimension $r$ to the [Poincare dual](cohomology.md#poincare-dual) of its homology class. [Rational equivalence](#rational-equivalence) gives the same cohomology class, so the map descends to the [Chow group](#chow-group). It respects [intersection products](#intersection-product-of-cartier-divisors), pullback and proper pushforward; a cohomological obstruction therefore obstructs the corresponding proposed identity of [Chow classes](#chow-class).

###### Cycle class

↑ **Parent:** [Cycle class map](#cycle-class-map)

The cycle class of an [algebraic cycle](#algebraic-cycle) is its image under the [cycle class map](#cycle-class-map). For a codimension-$r$ cycle on a smooth complex projective variety, it belongs to $H^{2r}(X,\mathbb Z)$ and is the [Poincare dual](cohomology.md#poincare-dual) of its fundamental homology class. The map factors through the [Chow group](#chow-group), but a [Chow class](#chow-class) retains finer information than its cohomological cycle class.

###### Chow ring

↑ **Parent:** [Chow group](#chow-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chow_ring)

For a smooth variety, intersection of cycles gives the graded Chow ring $A^*(X)$.

###### External product of Chow classes

↑ **Parent:** [Chow ring](#chow-ring)

For smooth projective varieties $X,Y$, pull back [Chow classes](#chow-class) from the two factors and take their [intersection product](#intersection-product-of-cartier-divisors) on $X\times Y$. This gives the external product and a graded map $\operatorname{CH}^*(X)\otimes\operatorname{CH}^*(Y)\to\operatorname{CH}^*(X\times Y)$. Unlike the cohomological [Künneth theorem](cohomology.md#kunneth-theorem), it need not generate every class of the product.

<h6 id="chow-kunneth-failure-for-an-elliptic-self-product">Chow Künneth failure for an elliptic self-product</h6>

↑ **Parent:** [External product of Chow classes](#external-product-of-chow-classes)

On $E\times E$ for a complex [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), the two factor curves and the diagonal have [intersection matrix](homology.md#intersection-matrix) $\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix}$, of determinant two. Their cohomology classes are therefore independent. The degree-one image of the [external product of Chow classes](#external-product-of-chow-classes) has cohomology contained in the span of the two factor classes. The [cycle class map](#cycle-class-map) thus shows that the diagonal is outside that image, proving failure of surjectivity.

###### Localization sequence for Chow groups

↑ **Parent:** [Chow group](#chow-group)

For a closed immersion $j:Z\hookrightarrow X$ with open complement $i:U\hookrightarrow X$, restriction and proper pushforward give an exact sequence

$$
A_k(Z)\xrightarrow{j_*}A_k(X)\xrightarrow{i^*}A_k(U)\to0.
$$

###### Cellular decomposition of a scheme

↑ **Parent:** [Chow group](#chow-group)

A cellular decomposition filters a scheme by closed subschemes whose successive differences are disjoint unions of affine spaces. The closures of the cells generate its Chow groups.

###### Chow ring of projective space

↑ **Parent:** [Cellular decomposition of a scheme](#cellular-decomposition-of-a-scheme)

For the hyperplane class $H$,

$$
A^*(\mathbb P^r)\cong\mathbb Z[H]/(H^{r+1}),
$$

and $A_k(\mathbb P^r)\cong\mathbb Z$ is generated by a linear $\mathbb P^k$.

###### Projective bundle formula for Chow groups

↑ **Parent:** [Chow group](#chow-group)

For a rank-$e+1$ vector bundle $E\to X$ and $p:\mathbb P(E)\to X$, powers of $\zeta=c_1(\mathcal O(1))$ give isomorphisms

$$
\bigoplus_{i=0}^e A_{k-e+i}(X)\xrightarrow{\sim}A_k(\mathbb P(E)).
$$

###### Homotopy invariance of Chow groups

↑ **Parent:** [Projective bundle formula for Chow groups](#projective-bundle-formula-for-chow-groups)

For a rank-$r$ vector bundle $E\to X$, flat pullback is an isomorphism $A_k(X)\cong A_{k+r}(E)$.

### Chern class

↑ **Parent:** [Intersection theory](#intersection-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chern_class)

Chern classes are characteristic classes of vector bundles satisfying functoriality and the Whitney product formula $c(E)=c(E')c(E'')$ for a short exact sequence.

#### Chern class axioms in the Chow ring

↑ **Parent:** [Chern class](#chern-class)

For a [vector bundle](fiber-bundle.md#vector-bundle) $E$ of rank $r$ on a smooth [algebraic variety](#algebraic-variety), algebraic [Chern classes](#chern-class) have $c_0(E)=1$, vanish for $i>r$, commute with pullback, and obey the [Whitney sum formula for Chern classes](#whitney-sum-formula-for-chern-classes) for every short exact sequence of vector bundles. A [line bundle](ringed-space.md#line-bundle) $\mathcal O(D)$ has total class $1+[D]$. The projective-bundle splitting construction makes pullback injective and supplies a filtration by line bundles, so these axioms determine all classes as elementary symmetric functions of their first classes. In particular, $c_i(E^*)=(-1)^ic_i(E)$ and $c_1(L\otimes M)=c_1(L)+c_1(M)$ in the ordinary [Chow ring](#chow-ring).

##### Chern classes of a smooth hypersurface cotangent bundle

↑ **Parent:** [Chern class axioms in the Chow ring](#chern-class-axioms-in-the-chow-ring)

For a smooth degree-$d$ [projective hypersurface](#projective-hypersurface) $X\subset\mathbb P^n$, put $h=c_1(\mathcal O_X(1))$. The [cotangent Euler sequence in homogeneous coordinates](#cotangent-euler-sequence-in-homogeneous-coordinates) gives $c(\Omega^1_{\mathbb P^n}|_X)=(1-h)^{n+1}$. The [Conormal exact sequence for Kähler differentials](ringed-space.md#conormal-exact-sequence-for-kahler-differentials) and [Whitney sum formula for Chern classes](#whitney-sum-formula-for-chern-classes) therefore yield $c(\Omega_X^1)=(1-h)^{n+1}/(1-dh)$. In codimension $i\le n-1$, its coefficient is $c_i(\Omega_X^1)=\sum_{j=0}^i(-1)^j\binom{n+1}{j}d^{i-j}h^i$. Higher classes vanish by rank and dimension; the formal quotient is truncated in the [Chow ring](#chow-ring).

#### Todd class

↑ **Parent:** [Chern class](#chern-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Todd_class)

Here the $x_j$ are the formal Chern roots of a [vector bundle](fiber-bundle.md#vector-bundle). The degree-four term is $(c_1^2+c_2)/12$. Applied to the tangent bundle of a compact complex surface, Riemann–Roch for the structure sheaf gives the [Noether formula](#noether-formula).

#### Chern class in complex cobordism

↑ **Parent:** [Chern class](#chern-class)

The complex orientation of [complex cobordism](geometry-and-topology.md#complex-cobordism) defines Chern classes of actual complex bundles by the splitting principle and elementary symmetric expressions in the first Chern classes of line summands. For an actual rank-$n$ complex bundle, its top Chern class is its [Euler class in a generalized cohomology theory](fiber-bundle.md#euler-class-in-a-generalized-cohomology-theory). Chern classes extend stably by the Whitney formula; this stable extension must not be confused with the Euler class of a merely stably complex real bundle.

##### Projective bundle relation in complex cobordism

↑ **Parent:** [Chern class in complex cobordism](#chern-class-in-complex-cobordism)

The relation uses $x=c_1(S)$ for the tautological line on the projectivization of $E$. It follows from the rank of the complementary bundle and Whitney multiplication. The alternating signs are ring subtraction; they do not assert that the [First Chern class](complex-geometry.md#first-chern-class) of a dual line is the additive negative in [complex cobordism](geometry-and-topology.md#complex-cobordism), where duality uses the formal-group inverse.

// Target: geometry-and-topology.bigb

#### Chern number

↑ **Parent:** [Chern class](#chern-class)

On a compact oriented $2r$-manifold without boundary, an integral product of [Chern classes](#chern-class) of total complex degree $r$ pairs with the [fundamental class](cohomology.md#fundamental-class) to give a [Chern number](#chern-number). A [unitary connection](fiber-bundle.md#unitary-connection) supplies [Chern-Weil theory](geometry-and-topology.md#chern-weil-homomorphism) representatives, but the integer is independent of that connection. The [Second Chern number](geometry-and-topology.md#second-chern-number) on a four-manifold is one important example; the integral of the [First Chern class](complex-geometry.md#first-chern-class) over a closed surface is another.

#### Whitney sum formula for Chern classes

↑ **Parent:** [Chern class](#chern-class)

The [Total Chern class](#total-chern-class) of a direct sum of complex [vector bundles](fiber-bundle.md#vector-bundle) is the product of their total Chern classes. In each degree, $c_k(E\oplus F)=\sum_{i+j=k}c_i(E)\smile c_j(F)$. The degree-zero class is one, classes beyond the bundle rank vanish, and a trivial bundle has total class one.

#### Projective bundle definition of Chern classes

↑ **Parent:** [Chern class](#chern-class)

For a rank-$r$ complex [vector bundle](fiber-bundle.md#vector-bundle), let $h=c_1(S^*)$ for the tautological line $S$ on its [projective bundle](fiber-bundle.md#projective-bundle). The [Leray-Hirsch theorem](fiber-bundle.md#leray-hirsch-theorem) gives the free basis $1,h,\ldots,h^{r-1}$ over base cohomology. The uniquely determined coefficients in the displayed monic relation define the integral [Chern classes](#chern-class). The line normalization uses the [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle) of the canonically oriented underlying real two-plane bundle, and uniqueness makes this definition intrinsic and natural under pullback. No choice of a trivializing cover or classifying map remains in the definition.

#### Total Chern class

↑ **Parent:** [Chern class](#chern-class)

The total Chern class is $c(E)=1+c_1(E)+c_2(E)+\cdots$.

#### Euler sequence

↑ **Parent:** [Chern class](#chern-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_sequence)

On projective space, the Euler sequence is

$$
0\to\mathcal O\to\mathcal O(1)^{\oplus(m+1)}\to T\mathbb P^m\to0.
$$

##### Cotangent Euler sequence in homogeneous coordinates

↑ **Parent:** [Euler sequence](#euler-sequence)

For a degree-zero rational function regular on an open subset of [projective space](projective-space.md), each derivative $\partial f/\partial X_i$ is a regular homogeneous rational function of degree $-1$. These derivatives define a [derivation](associative-algebra.md#derivation-of-an-algebra) with values in $\mathcal O(-1)^{\oplus(n+1)}$, hence a map from the [Kähler differential sheaf](ringed-space.md#sheaf-of-kahler-differentials-over-a-field). The last map is $(g_i)\mapsto\sum_iX_ig_i$. On $X_i\ne0$, put $y_j=X_j/X_i$ and use frame $X_i^{-1}$. The derivative of $y_j$ has coordinate vector with $1$ at $j$, $-y_j$ at $i$ and zero elsewhere. Those vectors form a free basis of the kernel of $(b_i)\mapsto b_i+\sum_{j\ne i}y_jb_j$, proving exactness directly in every characteristic.

###### Vanishing of global sections of the once-twisted projective cotangent bundle

↑ **Parent:** [Cotangent Euler sequence in homogeneous coordinates](#cotangent-euler-sequence-in-homogeneous-coordinates)

Dualize the [Euler sequence on complex projective space](algebraic-topology.md#euler-sequence-on-complex-projective-space) and tensor by the [hyperplane line bundle](fiber-bundle.md#hyperplane-line-bundle) to obtain $0\to\Omega^1(1)\to\mathcal O^{n+1}\to\mathcal O(1)\to0$. On global sections the last map sends $(c_i)$ to $\sum_i c_iX_i$, an isomorphism onto the linear forms. Left exactness of [sheaf cohomology](ringed-space.md#sheaf-cohomology) therefore gives the asserted vanishing. No higher-cohomology assumption is needed for this final kernel calculation.

### Degree of a projective scheme

↑ **Parent:** [Intersection theory](#intersection-theory)

For a pure $k$-dimensional projective scheme $X\subseteq\mathbb P^m$, its degree is $k!$ times the leading coefficient of its Hilbert polynomial, equivalently $\int_XH^k$.

This extends [degree of an algebraic variety](#degree-of-an-algebraic-variety) to retain scheme multiplicities.

### Normal bundle

↑ **Parent:** [Intersection theory](#intersection-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_bundle)

For a smooth closed embedding $i:X\hookrightarrow Y$, the normal bundle fits into $0\to TX\to i^*TY\to N_{X/Y}\to0$.

#### Normal bundle of a smooth plane conic

↑ **Parent:** [Normal bundle](#normal-bundle)

Embed a [smooth plane conic](#smooth-plane-conic) in $\mathbf P^3$ through a plane. The plane equation and conic equation form a [regular sequence](commutative-algebra.md#regular-sequence) of degrees one and two, so its [normal sheaf](ringed-space.md#normal-sheaf) is $\mathcal O_C(1)\oplus\mathcal O_C(2)$. Under $C\cong\mathbf P^1$, hyperplane degree is two, hence this [normal bundle](#normal-bundle) is $\mathcal O_{\mathbf P^1}(2)\oplus\mathcal O_{\mathbf P^1}(4)$. The normal exact sequence splits as well because $H^1(\mathbf P^1,\mathcal O(2))=0$.

#### Normal bundle of a linear complex-projective embedding

↑ **Parent:** [Normal bundle](#normal-bundle)

Near a projective subspace, transverse directions are linear maps from the tautological line to the complementary coordinate vector space. This describes the actual complex [normal bundle](#normal-bundle). The conjugate line and the dual line are complex-isomorphic using a [Hermitian metric](complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle); neither is the original tautological line as a complex bundle in general.

// Target: geometry-and-topology.bigb

#### Normal bundle of a transverse intersection

↑ **Parent:** [Normal bundle](#normal-bundle)

For a [transverse intersection](differential-geometry.md#transverse-intersection), the quotient map $TM|_L\to\nu_1|_L\oplus\nu_2|_L$ is onto and has kernel $TL$. This gives the displayed isomorphism of actual [normal bundles](#normal-bundle). [Complex structures](complex-geometry.md#complex-structure) on the two [normal bundles](#normal-bundle) therefore induce a [complex structure](complex-geometry.md#complex-structure) on the intersection's [normal bundle](#normal-bundle).

// Target: geometry-and-topology.bigb

#### Self-intersection number

↑ **Parent:** [Normal bundle](#normal-bundle)

For an oriented submanifold of half the dimension of its ambient manifold, the self-intersection number is the intersection number with a transverse perturbation. It equals the Euler number of the [normal bundle](#normal-bundle).

##### Self-intersection of the diagonal of a curve

↑ **Parent:** [Self-intersection number](#self-intersection-number)

For a smooth projective [algebraic curve](#algebraic-curve) $C$, the [normal bundle](#normal-bundle) of its diagonal in $C\times C$ is $TC$: on the diagonal the quotient of $TC\oplus TC$ by the diagonal subbundle is identified with $TC$ by taking the difference. The [self-intersection formula](#self-intersection-formula) therefore gives $\Delta_C^2=\deg TC=2-2g(C)$.

#### Self-intersection formula

↑ **Parent:** [Normal bundle](#normal-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Self-intersection_formula)

For a regular closed embedding $i:X\hookrightarrow Y$ of codimension $d$, the self-intersection formula is $i^*i_*(\alpha)=c_d(N_{X/Y})\cap\alpha$.

##### Euler number equals self-intersection

↑ **Parent:** [Self-intersection formula](#self-intersection-formula)

For an oriented closed surface smoothly embedded in an oriented four-manifold, a transverse section of the [normal bundle](#normal-bundle) gives a homologous small push-off. Its signed zeros are exactly the signed intersections with the original surface. This identifies the evaluation of the [Euler class](fiber-bundle.md#euler-class-of-a-vector-bundle) with the [self-intersection number](#self-intersection-number).

#### Framing of an embedded sphere

↑ **Parent:** [Normal bundle](#normal-bundle)

A framing of an embedding $S^{k-1}\hookrightarrow N^{n-1}$ is a trivialization of its rank-$(n-k)$ [normal bundle](#normal-bundle), equivalently a continuously varying ordered basis of normal vectors. After fixing one framing, homotopy classes of orientation-compatible framings form a torsor for $[S^{k-1},SO(n-k)]$.

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
