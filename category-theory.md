# Category theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Category_theory)

**Table of contents**

- [Bicategory](#bicategory)
- [Coreflexive pair](#coreflexive-pair)
- [Coherent category](#coherent-category)
  - [Coherent functor](#coherent-functor)
  - [Coherent topology](#coherent-topology)
  - [Unions of subobjects are pushouts](#unions-of-subobjects-are-pushouts)
- [Right lifting property](#right-lifting-property)
- [Model category](#model-category)
  - [Small object argument](#small-object-argument)
    - [Relative cell complex](#relative-cell-complex)
    - [Sequentially small object](#sequentially-small-object)
  - [Projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes)
    - [Generating cofibrations for nonnegative chain complexes](#generating-cofibrations-for-nonnegative-chain-complexes)
      - [Lifting characterization of an acyclic chain-complex fibration](#lifting-characterization-of-an-acyclic-chain-complex-fibration)
    - [Acyclic fibration in the projective chain-complex model structure](#acyclic-fibration-in-the-projective-chain-complex-model-structure)
  - [Model cofibration](#model-cofibration)
  - [Model fibration](#model-fibration)
  - [Model weak equivalence](#model-weak-equivalence)
- [Monoidal category](#monoidal-category)
  - [Product and coproduct monoidal structures on sets](#product-and-coproduct-monoidal-structures-on-sets)
  - [Triangle identity for a monoidal category](#triangle-identity-for-a-monoidal-category)
  - [Pentagon identity for a monoidal category](#pentagon-identity-for-a-monoidal-category)
  - [Unit identities derived from the monoidal pentagon and triangle](#unit-identities-derived-from-the-monoidal-pentagon-and-triangle)
  - [Yang–Baxter operator](#yang-baxter-operator)
  - [Dual pair in a monoidal category](#dual-pair-in-a-monoidal-category)
    - [Quantum dimension](#quantum-dimension)
    - [Snake identity](#snake-identity)
    - [Coevaluation morphism](#coevaluation-morphism)
    - [Evaluation morphism](#evaluation-morphism)
  - [Left closed monoidal category](#left-closed-monoidal-category)
  - [Comonoid](#comonoid)
    - [Counit](#counit)
    - [Comultiplication](#comultiplication)
    - [Comonoid morphism](#comonoid-morphism)
  - [Monoid object](#monoid-object)
    - [Frobenius monoid](#frobenius-monoid)
    - [Bimonoid](#bimonoid)
      - [Coquasitriangular structure](#coquasitriangular-structure)
    - [Monoid morphism](#monoid-morphism)
  - [Braided monoidal category](#braided-monoidal-category)
    - [Free braided monoidal category on one object](#free-braided-monoidal-category-on-one-object)
    - [Braid category](#braid-category)
    - [Braided monoidal functor](#braided-monoidal-functor)
    - [Braiding](#braiding)
  - [Opmonoidal functor](#opmonoidal-functor)
    - [Opmonoidal natural transformation](#opmonoidal-natural-transformation)
  - [Monoidal functor](#monoidal-functor)
    - [Frobenius monoidal functor](#frobenius-monoidal-functor)
    - [Strong monoidal functor](#strong-monoidal-functor)
      - [Strict monoidal functor](#strict-monoidal-functor)
  - [Strict monoidal category](#strict-monoidal-category)
  - [Monoidal coherence theorem](#monoidal-coherence-theorem)
    - [Termination proof of monoidal coherence](#termination-proof-of-monoidal-coherence)
    - [Word normalization proof of monoidal coherence](#word-normalization-proof-of-monoidal-coherence)
  - [Unitor](#unitor)
  - [Associator](#associator)
  - [Monoidal unit object](#monoidal-unit-object)
  - [Monoidal tensor product](#monoidal-tensor-product)
- [Category of groups](#category-of-groups)
- [Injective object](#injective-object)
- [Universal property](#universal-property)
- [Category](category.md)
  - [Duality (category theory)](category.md#duality-category-theory)
  - [Morphism in a category](category.md#morphism-in-a-category)
  - [Small projective object](category.md#small-projective-object)
  - [Category of small categories](category.md#category-of-small-categories)
    - [Indiscrete category](category.md#indiscrete-category)
    - [Discrete category](category.md#discrete-category)
    - [Free category on independent arrows](category.md#free-category-on-independent-arrows)
  - [Preadditive category](category.md#preadditive-category)
  - [Coreflective subcategory](category.md#coreflective-subcategory)
  - [Generating set in a category](category.md#generating-set-in-a-category)
  - [Composition in a category](category.md#composition-in-a-category)
  - [Object of a category](category.md#object-of-a-category)
  - [Terminal category](category.md#terminal-category)
  - [Nested partial unary operation category](category.md#nested-partial-unary-operation-category)
    - [Free extension of nested partial unary operations](category.md#free-extension-of-nested-partial-unary-operations)
      - [Split-coequalizer lifting for a fixed-point-domain operation](category.md#split-coequalizer-lifting-for-a-fixed-point-domain-operation)
  - [Coseparator](category.md#coseparator)
    - [Cogenerating set](category.md#cogenerating-set)
      - [Evaluation embedding into cogenerator products](category.md#evaluation-embedding-into-cogenerator-products)
    - [Equalizer presentation by powers of a coseparator](category.md#equalizer-presentation-by-powers-of-a-coseparator)
  - [Category of rings](category.md#category-of-rings)
  - [Skeletal category](category.md#skeletal-category)
    - [Skeleton of a category](category.md#skeleton-of-a-category)
  - [Subcategory](category.md#subcategory)
    - [Replete subcategory](category.md#replete-subcategory)
    - [Full subcategory](category.md#full-subcategory)
  - [Groupoid](category.md#groupoid)
  - [Functor](category.md#functor)
    - [Bifunctor](category.md#bifunctor)
    - [Discrete opfibration](category.md#discrete-opfibration)
      - [Connected components of discrete-opfibration pullbacks](category.md#connected-components-of-discrete-opfibration-pullbacks)
    - [Full functor](category.md#full-functor)
    - [Flat functor](category.md#flat-functor)
      - [Flat functor and finite-limit preservation](category.md#flat-functor-and-finite-limit-preservation)
    - [Kan extension](category.md#kan-extension)
    - [Finite-limit-preserving functor](category.md#finite-limit-preserving-functor)
      - [Regular functor](category.md#regular-functor)
    - [Conservative functor](category.md#conservative-functor)
    - [Limit-reflecting functor](category.md#limit-reflecting-functor)
      - [Limits reflected by full and faithful functors](category.md#limits-reflected-by-full-and-faithful-functors)
      - [Limit-creating functor](category.md#limit-creating-functor)
        - [Creation of limits up to isomorphism](category.md#creation-of-limits-up-to-isomorphism)
    - [Colimit-preserving functor](category.md#colimit-preserving-functor)
    - [Limit-preserving functor](category.md#limit-preserving-functor)
      - [Equalizer preservation by pullback-preserving functors](category.md#equalizer-preservation-by-pullback-preserving-functors)
    - [Forgetful functor](category.md#forgetful-functor)
    - [Endofunctor](category.md#endofunctor)
      - [Comonad](category.md#comonad)
        - [Cartesian comonad](category.md#cartesian-comonad)
        - [Idempotent comonad](category.md#idempotent-comonad)
        - [Coalgebra for a comonad](category.md#coalgebra-for-a-comonad)
          - [Category of coalgebras for a comonad](category.md#category-of-coalgebras-for-a-comonad)
            - [Cartesian closure for a finite-limit-preserving comonad](category.md#cartesian-closure-for-a-finite-limit-preserving-comonad)
            - [Subobject classifier of a coalgebra topos](category.md#subobject-classifier-of-a-coalgebra-topos)
            - [Exponentials in a coalgebra topos](category.md#exponentials-in-a-coalgebra-topos)
            - [Cofree coalgebra](category.md#cofree-coalgebra)
    - [Finite-limit-preserving set-valued functor](category.md#finite-limit-preserving-set-valued-functor)
    - [Equivalence of categories](category.md#equivalence-of-categories)
      - [Essential surjectivity](category.md#essential-surjectivity)
      - [Isomorphism of categories](category.md#isomorphism-of-categories)
    - [Functor category](category.md#functor-category)
      - [Pointwise monomorphism in a set-valued functor category](category.md#pointwise-monomorphism-in-a-set-valued-functor-category)
      - [Pointwise limits in a functor category](category.md#pointwise-limits-in-a-functor-category)
      - [Constant diagram functor](category.md#constant-diagram-functor)
        - [Adjoints to constant presheaves on open sets](category.md#adjoints-to-constant-presheaves-on-open-sets)
          - [Five adjoints for constant presheaves on open sets](category.md#five-adjoints-for-constant-presheaves-on-open-sets)
      - [Presheaf (category theory)](category.md#presheaf-category-theory)
      - [Presheaf category](category.md#presheaf-category)
        - [Canonical colimit presentation of a presheaf](category.md#canonical-colimit-presentation-of-a-presheaf)
        - [Free cocompletion](category.md#free-cocompletion)
        - [Grothendieck topology](category.md#grothendieck-topology)
          - [Double-negation topology](category.md#double-negation-topology)
            - [Separating tower site with vanishing product](category.md#separating-tower-site-with-vanishing-product)
          - [Zariski coverage on finitely presented rings](category.md#zariski-coverage-on-finitely-presented-rings)
          - [Coverage on a category](category.md#coverage-on-a-category)
            - [Rigid coverage](category.md#rigid-coverage)
            - [J-irreducible object of a site](category.md#j-irreducible-object-of-a-site)
          - [Site (category theory)](category.md#site-category-theory)
          - [Atomic topology](category.md#atomic-topology)
            - [Atomic finite-surjection site](category.md#atomic-finite-surjection-site)
              - [Primitive element of an atomic finite-surjection sheaf](category.md#primitive-element-of-an-atomic-finite-surjection-sheaf)
                - [Primitive decomposition of an atomic finite-surjection sheaf](category.md#primitive-decomposition-of-an-atomic-finite-surjection-sheaf)
                - [Primitive-element kernel rigidity lemma](category.md#primitive-element-kernel-rigidity-lemma)
              - [Descent identities for the atomic finite-surjection site](category.md#descent-identities-for-the-atomic-finite-surjection-site)
            - [Common-refinement condition for nonempty-sieve coverage](category.md#common-refinement-condition-for-nonempty-sieve-coverage)
          - [Subcanonical topology](category.md#subcanonical-topology)
          - [Sheaf on a site](category.md#sheaf-on-a-site)
        - [Sieve (category theory)](category.md#sieve-category-theory)
          - [Dense sieve](category.md#dense-sieve)
          - [J-closed sieve](category.md#j-closed-sieve)
        - [Presheaf topos](category.md#presheaf-topos)
          - [Slice-small presheaf construction](category.md#slice-small-presheaf-construction)
          - [Exponential in a presheaf category](category.md#exponential-in-a-presheaf-category)
      - [Arrow category](category.md#arrow-category)
        - [Adjoint chain for evaluation in an arrow category](category.md#adjoint-chain-for-evaluation-in-an-arrow-category)
        - [Category of injective functions](category.md#category-of-injective-functions)
      - [Representable functor](category.md#representable-functor)
        - [Representable retract criterion](category.md#representable-retract-criterion)
        - [Representability from a solution set](category.md#representability-from-a-solution-set)
        - [Left adjoint to a covariant representable functor](category.md#left-adjoint-to-a-covariant-representable-functor)
        - [Covariant representables preserve limits](category.md#covariant-representables-preserve-limits)
        - [Colimit criterion for representability of a presheaf](category.md#colimit-criterion-for-representability-of-a-presheaf)
          - [Small-limit preservation is insufficient for the large elements-colimit criterion](category.md#small-limit-preservation-is-insufficient-for-the-large-elements-colimit-criterion)
        - [Canonical colimit presentation of a covariant set-valued functor](category.md#canonical-colimit-presentation-of-a-covariant-set-valued-functor)
        - [Representation of a functor](category.md#representation-of-a-functor)
          - [Uniqueness of functor representations](category.md#uniqueness-of-functor-representations)
          - [Functoriality of chosen representations](category.md#functoriality-of-chosen-representations)
          - [Universal element of a set-valued functor](category.md#universal-element-of-a-set-valued-functor)
        - [Yoneda lemma](category.md#yoneda-lemma)
          - [Density formula for presheaves](category.md#density-formula-for-presheaves)
          - [Yoneda embedding](category.md#yoneda-embedding)
            - [Yoneda embedding detects split epimorphisms](category.md#yoneda-embedding-detects-split-epimorphisms)
            - [Yoneda embedding preserves exponentials](category.md#yoneda-embedding-preserves-exponentials)
            - [Covariant Yoneda embedding](category.md#covariant-yoneda-embedding)
      - [Pointwise epimorphism in a functor category](category.md#pointwise-epimorphism-in-a-functor-category)
        - [Pushout witness for failure of pointwise surjectivity](category.md#pushout-witness-for-failure-of-pointwise-surjectivity)
    - [Monofunctor](category.md#monofunctor)
    - [Natural transformation](category.md#natural-transformation)
      - [Dinatural transformation](category.md#dinatural-transformation)
      - [Natural isomorphism](category.md#natural-isomorphism)
        - [Natural bijection](category.md#natural-bijection)
      - [Naturality](category.md#naturality)
    - [Full and faithful functor](category.md#full-and-faithful-functor)
    - [Faithful functor](category.md#faithful-functor)
  - [Balanced category](category.md#balanced-category)
  - [Reflective subcategory](category.md#reflective-subcategory)
    - [Compact Hausdorff reflection](category.md#compact-hausdorff-reflection)
    - [Limits in a reflective subcategory](category.md#limits-in-a-reflective-subcategory)
    - [Left-exact reflective subcategory](category.md#left-exact-reflective-subcategory)
      - [Exponentials in a left-exact reflective subcategory](category.md#exponentials-in-a-left-exact-reflective-subcategory)
    - [Reflector](category.md#reflector)
    - [Closure operation induced by a left-exact reflector](category.md#closure-operation-induced-by-a-left-exact-reflector)
  - [Congruence on a category](category.md#congruence-on-a-category)
    - [Category of partial maps localized at subterminal objects](category.md#category-of-partial-maps-localized-at-subterminal-objects)
  - [Small category](category.md#small-category)
  - [Locally small category](category.md#locally-small-category)
    - [Hom-set](category.md#hom-set)
  - [Opposite category](category.md#opposite-category)
  - [Connected category](category.md#connected-category)
    - [Connected component of a category](category.md#connected-component-of-a-category)
  - [Category of sets](category.md#category-of-sets)
    - [Category of finite sets](category.md#category-of-finite-sets)
    - [Category of pointed sets](category.md#category-of-pointed-sets)
    - [Category of partial functions](category.md#category-of-partial-functions)
    - [Finite-limit-and-colimit preserving endofunctor of sets](category.md#finite-limit-and-colimit-preserving-endofunctor-of-sets)
      - [Ultrapower endofunctor of sets](category.md#ultrapower-endofunctor-of-sets)
  - [Category of ordinals in reverse order](category.md#category-of-ordinals-in-reverse-order)
  - [Pointed category](category.md#pointed-category)
    - [Pseudo-epimorphism](category.md#pseudo-epimorphism)
      - [Pseudo-epimorphism factorization through the kernel of a cokernel](category.md#pseudo-epimorphism-factorization-through-the-kernel-of-a-cokernel)
    - [Zero object](category.md#zero-object)
      - [Zero morphism](category.md#zero-morphism)
    - [Kernel in a category](category.md#kernel-in-a-category)
    - [Cokernel in a category](category.md#cokernel-in-a-category)
      - [Cokernel invariance under pushout](category.md#cokernel-invariance-under-pushout)
    - [Normal monomorphism](category.md#normal-monomorphism)
      - [Closure of normal monomorphisms forces abelianness](category.md#closure-of-normal-monomorphisms-forces-abelianness)
    - [Conormal epimorphism](category.md#conormal-epimorphism)
  - [Monomorphism](category.md#monomorphism)
    - [Extremal monomorphism](category.md#extremal-monomorphism)
    - [Split monomorphism](category.md#split-monomorphism)
      - [Absolute monomorphism](category.md#absolute-monomorphism)
      - [Retract in a category](category.md#retract-in-a-category)
    - [Strong monomorphism](category.md#strong-monomorphism)
      - [Four-object strong nonregular monomorphism](category.md#four-object-strong-nonregular-monomorphism)
      - [Balanced categories with pullbacks have strong monomorphisms](category.md#balanced-categories-with-pullbacks-have-strong-monomorphisms)
      - [Strict monomorphism](category.md#strict-monomorphism)
      - [Regular monomorphism](category.md#regular-monomorphism)
      - [Intersection of strong subobjects](category.md#intersection-of-strong-subobjects)
    - [Anodyne morphism in a category](category.md#anodyne-morphism-in-a-category)
      - [Saturated object with respect to anodyne morphisms](category.md#saturated-object-with-respect-to-anodyne-morphisms)
        - [Saturated reflection from a strong-subobject intersection](category.md#saturated-reflection-from-a-strong-subobject-intersection)
  - [Epimorphism](category.md#epimorphism)
    - [Extremal epimorphism](category.md#extremal-epimorphism)
      - [Nonregular extremal epimorphism in the category of categories](category.md#nonregular-extremal-epimorphism-in-the-category-of-categories)
    - [Split epimorphism](category.md#split-epimorphism)
    - [Regular epimorphism](category.md#regular-epimorphism)
      - [Regular epimorphisms are strong epimorphisms](category.md#regular-epimorphisms-are-strong-epimorphisms)
    - [Strong epimorphism](category.md#strong-epimorphism)
      - [Left lifting property against monomorphisms](category.md#left-lifting-property-against-monomorphisms)
        - [Binary-product criterion for lifting-only strong epimorphisms](category.md#binary-product-criterion-for-lifting-only-strong-epimorphisms)
        - [Right-factor cancellation for lifting-only strong morphisms](category.md#right-factor-cancellation-for-lifting-only-strong-morphisms)
        - [Monic lifting-only strong morphisms are invertible](category.md#monic-lifting-only-strong-morphisms-are-invertible)
      - [Regular-epimorphism-monomorphism factorization from kernel pairs](category.md#regular-epimorphism-monomorphism-factorization-from-kernel-pairs)
      - [Strong epimorphism in the category of small categories](category.md#strong-epimorphism-in-the-category-of-small-categories)
      - [Strong quotient](category.md#strong-quotient)
  - [Subobject](category.md#subobject)
    - [Well-pointed object in a category](category.md#well-pointed-object-in-a-category)
    - [Intersection of subobjects](category.md#intersection-of-subobjects)
      - [Minimal supported subobject](category.md#minimal-supported-subobject)
    - [Well-copowered category](category.md#well-copowered-category)
    - [Image factorization](category.md#image-factorization)
      - [Image factorization in an abelian category](category.md#image-factorization-in-an-abelian-category)
        - [Pullback stability of abelian image factorization](category.md#pullback-stability-of-abelian-image-factorization)
        - [Functoriality of abelian image factorization](category.md#functoriality-of-abelian-image-factorization)
      - [Frobenius reciprocity for subobjects](category.md#frobenius-reciprocity-for-subobjects)
    - [Well-powered category](category.md#well-powered-category)
  - [Projective object](category.md#projective-object)
    - [Projectivity detected by all first left derived functors](category.md#projectivity-detected-by-all-first-left-derived-functors)
    - [Covariant representables are projective](category.md#covariant-representables-are-projective)
    - [Coproducts of projective objects are projective](category.md#coproducts-of-projective-objects-are-projective)
    - [Indecomposable projective object](category.md#indecomposable-projective-object)
    - [Irreducible projective in a set-valued functor category](category.md#irreducible-projective-in-a-set-valued-functor-category)
    - [Projective cover of a set-valued functor by representables](category.md#projective-cover-of-a-set-valued-functor-by-representables)
  - [Terminal object](category.md#terminal-object)
    - [Weakly terminal set](category.md#weakly-terminal-set)
    - [Subterminal object](category.md#subterminal-object)
      - [Subterminal sheaf](category.md#subterminal-sheaf)
  - [Initial object](category.md#initial-object)
    - [Weakly initial set](category.md#weakly-initial-set)
      - [Initial-object lemma for complete categories with a weakly initial set](category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set)
    - [Strict initial object](category.md#strict-initial-object)
  - [Diagram (category theory)](category.md#diagram-category-theory)
    - [Cone over a diagram](category.md#cone-over-a-diagram)
      - [Categorical limit](category.md#categorical-limit)
        - [End of a functor](category.md#end-of-a-functor)
        - [Hom-set detection of categorical limits](category.md#hom-set-detection-of-categorical-limits)
        - [Limit functor](category.md#limit-functor)
        - [Finite limit](category.md#finite-limit)
          - [Finite limits from terminal objects and pullbacks](category.md#finite-limits-from-terminal-objects-and-pullbacks)
          - [Cartesian category](category.md#cartesian-category)
          - [Product (category theory)](category.md#product-category-theory)
            - [Categorical diagonal](category.md#categorical-diagonal)
          - [Equaliser](category.md#equaliser)
            - [Split equalizer](category.md#split-equalizer)
              - [Split equalizers associated with a monad](category.md#split-equalizers-associated-with-a-monad)
          - [Pullback (category theory)](category.md#pullback-category-theory)
            - [Base change of a pullback square](category.md#base-change-of-a-pullback-square)
            - [Pullback pasting lemma](category.md#pullback-pasting-lemma)
            - [Kernel pair](category.md#kernel-pair)
              - [Epimorphisms in an abelian category are coequalizers of their kernel pairs](category.md#epimorphisms-in-an-abelian-category-are-coequalizers-of-their-kernel-pairs)
        - [Construction of small limits from products and equalizers](category.md#construction-of-small-limits-from-products-and-equalizers)
        - [Complete category](category.md#complete-category)
        - [Initial functor](category.md#initial-functor)
          - [Representable test for initial functors](category.md#representable-test-for-initial-functors)
          - [Cone restriction along an initial functor](category.md#cone-restriction-along-an-initial-functor)
    - [Cocone under a diagram](category.md#cocone-under-a-diagram)
  - [Colimit](category.md#colimit)
    - [Coend of a functor](category.md#coend-of-a-functor)
    - [Pushout](category.md#pushout)
    - [Construction of finite colimits from coproducts and reflexive coequalizers](category.md#construction-of-finite-colimits-from-coproducts-and-reflexive-coequalizers)
    - [Pushout in a category](category.md#pushout-in-a-category)
      - [Pushout of groups](category.md#pushout-of-groups)
    - [Cocomplete category](category.md#cocomplete-category)
    - [Coproduct](category.md#coproduct)
      - [Countable coproduct](category.md#countable-coproduct)
    - [Coequalizer](category.md#coequalizer)
      - [Split coequalizer](category.md#split-coequalizer)
        - [Functor-split coequalizer pair](category.md#functor-split-coequalizer-pair)
    - [Multicolimit](category.md#multicolimit)
    - [Commutation of limits and colimits](category.md#commutation-of-limits-and-colimits)
      - [Commutation of iterated categorical limits](category.md#commutation-of-iterated-categorical-limits)
      - [Common quotient obstruction to commutation of fixed points and orbits](category.md#common-quotient-obstruction-to-commutation-of-fixed-points-and-orbits)
      - [Commutation of fixed points and orbit quotients for coprime groups](category.md#commutation-of-fixed-points-and-orbit-quotients-for-coprime-groups)
    - [Filtered category](category.md#filtered-category)
      - [Filtered colimit in a category](category.md#filtered-colimit-in-a-category)
        - [Directed colimits created by the abelian-group forgetful functor](category.md#directed-colimits-created-by-the-abelian-group-forgetful-functor)
      - [Weakly filtered category](category.md#weakly-filtered-category)
      - [Filtered colimits commute with finite limits in sets](category.md#filtered-colimits-commute-with-finite-limits-in-sets)
        - [Finite-stage equality in a filtered set colimit](category.md#finite-stage-equality-in-a-filtered-set-colimit)
        - [Cofiltered limits need not commute with finite colimits in sets](category.md#cofiltered-limits-need-not-commute-with-finite-colimits-in-sets)
    - [Sifted category](category.md#sifted-category)
    - [Local state classifier](category.md#local-state-classifier)
  - [Idempotent morphism](category.md#idempotent-morphism)
    - [Splitting of an idempotent morphism](category.md#splitting-of-an-idempotent-morphism)
      - [Idempotent splitting through a coequalizer](category.md#idempotent-splitting-through-a-coequalizer)
    - [Cauchy-complete category](category.md#cauchy-complete-category)
      - [Idempotent ideal in a finite category](category.md#idempotent-ideal-in-a-finite-category)
    - [Karoubi envelope](category.md#karoubi-envelope)
  - [Regular category](category.md#regular-category)
    - [Regular-logic separation of a proper subobject](category.md#regular-logic-separation-of-a-proper-subobject)
    - [Capital regular category](category.md#capital-regular-category)
      - [Power of sets as a capital regular category](category.md#power-of-sets-as-a-capital-regular-category)
        - [Conservativity of set products on totally supported families](category.md#conservativity-of-set-products-on-totally-supported-families)
      - [Capitalization of a small regular category](category.md#capitalization-of-a-small-regular-category)
      - [Global sections of a capital regular category](category.md#global-sections-of-a-capital-regular-category)
    - [Support of an object in a regular category](category.md#support-of-an-object-in-a-regular-category)
      - [Almost total support for a regular category](category.md#almost-total-support-for-a-regular-category)
        - [Conservative regular representation in sets](category.md#conservative-regular-representation-in-sets)
      - [Well-supported object](category.md#well-supported-object)
    - [Regular coverage](category.md#regular-coverage)
      - [Irreducible representable sheaf for the regular coverage](category.md#irreducible-representable-sheaf-for-the-regular-coverage)
      - [Local membership closure for the regular coverage](category.md#local-membership-closure-for-the-regular-coverage)
    - [Glued ring categories counterexample to regularity](category.md#glued-ring-categories-counterexample-to-regularity)
    - [Left-exact reflective subcategory of a regular category](category.md#left-exact-reflective-subcategory-of-a-regular-category)
    - [Image of a morphism in a regular category](category.md#image-of-a-morphism-in-a-regular-category)
    - [Category of relations](category.md#category-of-relations)
      - [Category of relations (sets)](category.md#category-of-relations-sets)
      - [Total functional relations define morphisms](category.md#total-functional-relations-define-morphisms)
      - [Graph of a morphism as a relation](category.md#graph-of-a-morphism-as-a-relation)
  - [Comma category](category.md#comma-category)
    - [Slice category](category.md#slice-category)
      - [Slice of a set-valued functor category](category.md#slice-of-a-set-valued-functor-category)
      - [Finite completeness of slice categories](category.md#finite-completeness-of-slice-categories)
    - [Limits in a comma category of a limit-preserving functor](category.md#limits-in-a-comma-category-of-a-limit-preserving-functor)
    - [Solution-set condition](category.md#solution-set-condition)
    - [Universal arrow from an object to a functor](category.md#universal-arrow-from-an-object-to-a-functor)
      - [Representability through the category of elements](category.md#representability-through-the-category-of-elements)
    - [Category of elements](category.md#category-of-elements)
      - [Covariant density presentation](category.md#covariant-density-presentation)
  - [Adjoint functors](category.md#adjoint-functors)
    - [Preservation obstructions to extending an adjoint chain](category.md#preservation-obstructions-to-extending-an-adjoint-chain)
    - [Adjoint chain for the objects of a category](category.md#adjoint-chain-for-the-objects-of-a-category)
    - [Discrete-indiscrete adjunction](category.md#discrete-indiscrete-adjunction)
    - [Boolean ultrafilter-power-set adjunction](category.md#boolean-ultrafilter-power-set-adjunction)
    - [Idempotent adjunction](category.md#idempotent-adjunction)
    - [Adjoint functor theorem](category.md#adjoint-functor-theorem)
    - [Left Kan extension](category.md#left-kan-extension)
      - [Left Kan extension as a comma-category colimit](category.md#left-kan-extension-as-a-comma-category-colimit)
      - [Bounded subfunctor solution set for precomposition](category.md#bounded-subfunctor-solution-set-for-precomposition)
    - [Freyd general adjoint functor theorem](category.md#freyd-general-adjoint-functor-theorem)
    - [Right-adjoint criterion using comma-category colimits](category.md#right-adjoint-criterion-using-comma-category-colimits)
    - [Mate correspondence](category.md#mate-correspondence)
    - [Galois connection](category.md#galois-connection)
      - [Adjoints of inverse image on power sets](category.md#adjoints-of-inverse-image-on-power-sets)
    - [Unit and counit of an adjunction](category.md#unit-and-counit-of-an-adjunction)
      - [Counit of an adjunction](category.md#counit-of-an-adjunction)
      - [Unit of an adjunction](category.md#unit-of-an-adjunction)
      - [Triangle identities for an adjunction](category.md#triangle-identities-for-an-adjunction)
        - [One-triangle adjunction idempotent](category.md#one-triangle-adjunction-idempotent)
          - [Splitting a one-triangle adjunction idempotent](category.md#splitting-a-one-triangle-adjunction-idempotent)
      - [Fully faithful adjoint criterion](category.md#fully-faithful-adjoint-criterion)
        - [Double-adjoint comparison transformation](category.md#double-adjoint-comparison-transformation)
      - [Faithful left adjoint criterion](category.md#faithful-left-adjoint-criterion)
      - [Pointwise-monic unit-and-counit criterion](category.md#pointwise-monic-unit-and-counit-criterion)
        - [Pointwise-monic adjunction over a non-balanced poset](category.md#pointwise-monic-adjunction-over-a-non-balanced-poset)
    - [Adjoint functor theorem for complete lattices](category.md#adjoint-functor-theorem-for-complete-lattices)
    - [Right Kan extension](category.md#right-kan-extension)
    - [Special adjoint functor theorem](category.md#special-adjoint-functor-theorem)
      - [Limit form of the special adjoint functor theorem](category.md#limit-form-of-the-special-adjoint-functor-theorem)
        - [Cogenerator bound for comma-category solution sets](category.md#cogenerator-bound-for-comma-category-solution-sets)
    - [Cartesian closed category](category.md#cartesian-closed-category)
      - [Locally Cartesian closed category](category.md#locally-cartesian-closed-category)
      - [Cartesian closed monoid](category.md#cartesian-closed-monoid)
      - [Extensional reflexive object](category.md#extensional-reflexive-object)
      - [Exponential object](category.md#exponential-object)
        - [Exponential of covariant set-valued functors](category.md#exponential-of-covariant-set-valued-functors)
        - [Currying](category.md#currying)
        - [Evaluation map of an exponential object](category.md#evaluation-map-of-an-exponential-object)
        - [Exponential of monoid sets](category.md#exponential-of-monoid-sets)
          - [Nondecidable exponential of decidable monoid sets](category.md#nondecidable-exponential-of-decidable-monoid-sets)
          - [Monoid condition for decidable exponentials](category.md#monoid-condition-for-decidable-exponentials)
        - [Currying adjunction for small categories](category.md#currying-adjunction-for-small-categories)
      - [Exponential ideal](category.md#exponential-ideal)
        - [Reflector product criterion for an exponential ideal](category.md#reflector-product-criterion-for-an-exponential-ideal)
      - [Exponentiable object](category.md#exponentiable-object)
        - [Exponentiability test using a coseparator](category.md#exponentiability-test-using-a-coseparator)
        - [Product of exponentiable objects is exponentiable](category.md#product-of-exponentiable-objects-is-exponentiable)
        - [Zero object is the only exponentiable object in a pointed category](category.md#zero-object-is-the-only-exponentiable-object-in-a-pointed-category)
        - [Exponentiability criterion in the category of T0 spaces](category.md#exponentiability-criterion-in-the-category-of-t0-spaces)
      - [Cartesian closed category of posets](category.md#cartesian-closed-category-of-posets)
      - [Tiny object](category.md#tiny-object)
        - [Tiny covariant functor on a Cauchy-complete category with an initial object is representable](category.md#tiny-covariant-functor-on-a-cauchy-complete-category-with-an-initial-object-is-representable)
        - [Tiny covariant representable functor on a category with binary coproducts](category.md#tiny-covariant-representable-functor-on-a-category-with-binary-coproducts)
        - [Tiny objects are closed under finite products](category.md#tiny-objects-are-closed-under-finite-products)
        - [Representable presheaves are the tiny objects of an idempotent-complete finite-product category](category.md#representable-presheaves-are-the-tiny-objects-of-an-idempotent-complete-finite-product-category)
  - [Category of metric spaces and non-expansive maps](category.md#category-of-metric-spaces-and-non-expansive-maps)
    - [Non-expansive map](category.md#non-expansive-map)
    - [Category of bounded metric spaces and non-expansive maps](category.md#category-of-bounded-metric-spaces-and-non-expansive-maps)
      - [Metric exponential candidate](category.md#metric-exponential-candidate)
        - [Interpolating metric space](category.md#interpolating-metric-space)
    - [Quotient metric](category.md#quotient-metric)
  - [Final functor](category.md#final-functor)
    - [Finality of a functor](category.md#finality-of-a-functor)
    - [Cocone extension along a final functor](category.md#cocone-extension-along-a-final-functor)
  - [Discrete fibration](category.md#discrete-fibration)
    - [Unique lifting property of a discrete fibration](category.md#unique-lifting-property-of-a-discrete-fibration)
    - [Orthogonality of final functors and discrete fibrations](category.md#orthogonality-of-final-functors-and-discrete-fibrations)
    - [Final-discrete-fibration factorization](category.md#final-discrete-fibration-factorization)
      - [Uniqueness of a final-discrete-fibration factorization](category.md#uniqueness-of-a-final-discrete-fibration-factorization)
      - [Connected-component presheaf of a functor](category.md#connected-component-presheaf-of-a-functor)
  - [Category of fields](category.md#category-of-fields)
  - [Compact object (mathematics)](category.md#compact-object-mathematics)
- [Symmetric monoidal category](#symmetric-monoidal-category)
- [Complete join-semilattice](#complete-join-semilattice)
  - [Category of complete join-semilattices](#category-of-complete-join-semilattices)
    - [Biproducts of complete join-semilattices](#biproducts-of-complete-join-semilattices)
- [Enriched category](#enriched-category)
  - [Commutative-monoid enrichment](#commutative-monoid-enrichment)
    - [Transported addition on the multiplicative natural-number monoid](#transported-addition-on-the-multiplicative-natural-number-monoid)
  - [Underlying category of an enriched category](#underlying-category-of-an-enriched-category)
  - [Self-enrichment of a closed symmetric monoidal category](#self-enrichment-of-a-closed-symmetric-monoidal-category)
  - [Poset-enriched adjunction](#poset-enriched-adjunction)
    - [Left adjoint relation is a function](#left-adjoint-relation-is-a-function)
  - [Semi-additive category](#semi-additive-category)
    - [Biproduct](#biproduct)
      - [Biproduct-induced addition of morphisms](#biproduct-induced-addition-of-morphisms)
      - [Countable biproducts in an additive category force triviality](#countable-biproducts-in-an-additive-category-force-triviality)
    - [Additive category](#additive-category)
      - [Semisimple category](#semisimple-category)
      - [Additive category with truncated primary torsion](#additive-category-with-truncated-primary-torsion)
      - [Additive functor](#additive-functor)
        - [Right-exact additive functor](#right-exact-additive-functor)
      - [Abelian category](#abelian-category)
        - [Cofinitary abelian category](#cofinitary-abelian-category)
        - [Finitary abelian category](#finitary-abelian-category)
          - [Coproduct-to-product comparison in a finitary abelian category](#coproduct-to-product-comparison-in-a-finitary-abelian-category)
        - [Category of abelian groups](#category-of-abelian-groups)
        - [Abelian category with enough projectives](#abelian-category-with-enough-projectives)
        - [Hereditary abelian category with enough projectives](#hereditary-abelian-category-with-enough-projectives)
        - [Kernel squares in an abelian category](#kernel-squares-in-an-abelian-category)
        - [Zero-cokernel criterion for epimorphisms](#zero-cokernel-criterion-for-epimorphisms)
        - [Pullback stability of epimorphisms in an abelian category](#pullback-stability-of-epimorphisms-in-an-abelian-category)
          - [Pullback of an epimorphism is a pushout in an abelian category](#pullback-of-an-epimorphism-is-a-pushout-in-an-abelian-category)
        - [Every abelian category is regular](#every-abelian-category-is-regular)
        - [Image and coimage in an abelian category](#image-and-coimage-in-an-abelian-category)
          - [Coimage](#coimage)
        - [Exact sequence in an abelian category](#exact-sequence-in-an-abelian-category)
          - [Short exact sequence in an abelian category](#short-exact-sequence-in-an-abelian-category)
            - [Schanuel lemma in an abelian category](#schanuel-lemma-in-an-abelian-category)
            - [Pullback of a short exact sequence in an abelian category](#pullback-of-a-short-exact-sequence-in-an-abelian-category)
          - [Five lemma](#five-lemma)
            - [Five lemma via image factorization](#five-lemma-via-image-factorization)
          - [Snake lemma](#snake-lemma)
        - [Complex in an abelian category](#complex-in-an-abelian-category)
          - [Additive indexing category for chain complexes](#additive-indexing-category-for-chain-complexes)
          - [Homology object](#homology-object)
            - [Self-duality of homology](#self-duality-of-homology)
- [Monad](#monad)
  - [Square reader monad](#square-reader-monad)
  - [Equalizer submonad of a monad](#equalizer-submonad-of-a-monad)
  - [Monad morphism](#monad-morphism)
    - [Restriction of monad algebras](#restriction-of-monad-algebras)
  - [List monad](#list-monad)
    - [List-monad algebras are monoids](#list-monad-algebras-are-monoids)
  - [Unit and multiplication of a monad](#unit-and-multiplication-of-a-monad)
  - [Opmonoidal monad](#opmonoidal-monad)
  - [Shift monad on order-preserving maps of natural numbers](#shift-monad-on-order-preserving-maps-of-natural-numbers)
  - [Idempotent monad](#idempotent-monad)
  - [Monad structure on a terminal endofunctor](#monad-structure-on-a-terminal-endofunctor)
    - [Ultrafilter monad](#ultrafilter-monad)
  - [Monad induced by an adjunction](#monad-induced-by-an-adjunction)
    - [Category of adjunctions inducing a fixed monad](#category-of-adjunctions-inducing-a-fixed-monad)
  - [Algebra for a monad](#algebra-for-a-monad)
    - [Reflexive free-algebra presentation of a monad algebra](#reflexive-free-algebra-presentation-of-a-monad-algebra)
    - [Unit law for a monad algebra](#unit-law-for-a-monad-algebra)
    - [Free algebra functor](#free-algebra-functor)
    - [Morphism of algebras for a monad](#morphism-of-algebras-for-a-monad)
  - [Eilenberg-Moore category](#eilenberg-moore-category)
    - [Monad algebra forgetful functor creates split coequalizers](#monad-algebra-forgetful-functor-creates-split-coequalizers)
    - [Monad algebra forgetful functor creates limits](#monad-algebra-forgetful-functor-creates-limits)
    - [Free-forgetful Eilenberg-Moore adjunction](#free-forgetful-eilenberg-moore-adjunction)
    - [Adjoint lifting theorem for monad algebra functors](#adjoint-lifting-theorem-for-monad-algebra-functors)
    - [Coproduct presentation for monad algebras](#coproduct-presentation-for-monad-algebras)
      - [Finite colimits of monad algebras from reflexive coequalizers](#finite-colimits-of-monad-algebras-from-reflexive-coequalizers)
    - [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor)
      - [Full faithfulness from counit coequalizers](#full-faithfulness-from-counit-coequalizers)
        - [Full comparison and reflection of split coequalizers](#full-comparison-and-reflection-of-split-coequalizers)
      - [Terminality of the Eilenberg-Moore adjunction](#terminality-of-the-eilenberg-moore-adjunction)
      - [Left adjoint to the Eilenberg-Moore comparison functor](#left-adjoint-to-the-eilenberg-moore-comparison-functor)
        - [Comparison-adjunction unit criterion](#comparison-adjunction-unit-criterion)
      - [Monadic length](#monadic-length)
        - [Monadic tower for nested partial unary operations](#monadic-tower-for-nested-partial-unary-operations)
    - [Monadic adjunction](#monadic-adjunction)
      - [Crude monadicity theorem](#crude-monadicity-theorem)
      - [Comonadic adjunction](#comonadic-adjunction)
        - [Beck comonadicity theorem](#beck-comonadicity-theorem)
      - [Beck's monadicity theorem](#beck-s-monadicity-theorem)
  - [Monad on a left adjoint induces a comonad on its right adjoint](#monad-on-a-left-adjoint-induces-a-comonad-on-its-right-adjoint)
  - [Kleisli category](#kleisli-category)
    - [Initiality of the Kleisli adjunction](#initiality-of-the-kleisli-adjunction)
    - [Kleisli comparison functor](#kleisli-comparison-functor)
    - [Free functor into a Kleisli category](#free-functor-into-a-kleisli-category)
  - [Pointwise monad on a functor category](#pointwise-monad-on-a-functor-category)
  - [Precomposition monad on a functor category](#precomposition-monad-on-a-functor-category)
- [Lawvere theory](#lawvere-theory)
- [Finitary monad](#finitary-monad)
- [Complete Heyting algebra](#complete-heyting-algebra)
  - [Subframe](#subframe)
  - [Completely prime filter](#completely-prime-filter)
  - [Preframe](#preframe)
    - [Preframe tensor product](#preframe-tensor-product)
      - [Frame coreflection of a preframe monoid](#frame-coreflection-of-a-preframe-monoid)
  - [Nucleus on a frame](#nucleus-on-a-frame)
    - [Relative nucleus assembly](#relative-nucleus-assembly)
    - [Closed nucleus](#closed-nucleus)
    - [Open nucleus](#open-nucleus)
  - [Locale](#locale)
    - [Connected locale](#connected-locale)
    - [Well-inside relation](#well-inside-relation)
      - [Regular locale](#regular-locale)
    - [Extremally disconnected locale](#extremally-disconnected-locale)
      - [Gleason cover of a compact regular locale](#gleason-cover-of-a-compact-regular-locale)
    - [Open locale](#open-locale)
      - [Totally connected locale](#totally-connected-locale)
      - [Positive open of a locale](#positive-open-of-a-locale)
    - [Totally unordered locale](#totally-unordered-locale)
    - [Hausdorff locale](#hausdorff-locale)
    - [Compact locale](#compact-locale)
      - [Localic Tychonoff theorem](#localic-tychonoff-theorem)
    - [Sublocale](#sublocale)
      - [Booleanization of a locale](#booleanization-of-a-locale)
      - [Flat sublocale](#flat-sublocale)
        - [Joyal extension lemma](#joyal-extension-lemma)
      - [Dense sublocale](#dense-sublocale)
      - [Closed sublocale](#closed-sublocale)
  - [Frame-point adjunction](#frame-point-adjunction)
  - [Open-set frame](#open-set-frame)
  - [Point of a frame](#point-of-a-frame)
  - [Frame homomorphism](#frame-homomorphism)
  - [Category of matrices valued in a frame](#category-of-matrices-valued-in-a-frame)
- [Reflexive pair](#reflexive-pair)
  - [Reflexive coequalizer](#reflexive-coequalizer)
  - [Coequalizer of a reflexive pair from a pushout](#coequalizer-of-a-reflexive-pair-from-a-pushout)
  - [Internal groupoid](#internal-groupoid)
    - [Reflexive-pair groupoid formula in a preadditive category](#reflexive-pair-groupoid-formula-in-a-preadditive-category)
    - [Reflexive pair in an additive category is an internal groupoid](#reflexive-pair-in-an-additive-category-is-an-internal-groupoid)
- [Elementary topos](#elementary-topos)
  - [Two-valued topos](#two-valued-topos)
  - [Irreducible object in a topos](#irreducible-object-in-a-topos)
  - [Boolean topos](#boolean-topos)
  - [Logical functor](#logical-functor)
  - [Power object](#power-object)
    - [Power objects in a slice category](#power-objects-in-a-slice-category)
    - [Power object of a subobject](#power-object-of-a-subobject)
    - [Contravariant power-object functor](#contravariant-power-object-functor)
      - [Power-object monadicity](#power-object-monadicity)
        - [Products and coproducts of fixed cardinality in a topos](#products-and-coproducts-of-fixed-cardinality-in-a-topos)
      - [Power objects turn coreflexive equalizers into coequalizers](#power-objects-turn-coreflexive-equalizers-into-coequalizers)
  - [Atom in a topos](#atom-in-a-topos)
  - [Global sections functor](#global-sections-functor)
  - [Geometric morphism](#geometric-morphism)
    - [Hyperconnected-localic factorization](#hyperconnected-localic-factorization)
    - [Hyperconnected geometric morphism](#hyperconnected-geometric-morphism)
    - [Localic geometric morphism](#localic-geometric-morphism)
    - [Diaconescu equivalence for geometric morphisms](#diaconescu-equivalence-for-geometric-morphisms)
    - [Global sections geometric morphism](#global-sections-geometric-morphism)
    - [Inverse image functor of a geometric morphism](#inverse-image-functor-of-a-geometric-morphism)
    - [Essential geometric morphism](#essential-geometric-morphism)
    - [Surjection-embedding factorization of a geometric morphism](#surjection-embedding-factorization-of-a-geometric-morphism)
    - [Geometric embedding](#geometric-embedding)
      - [Subtopos](#subtopos)
    - [Surjective geometric morphism](#surjective-geometric-morphism)
      - [Surjectivity detected by the subobject classifier](#surjectivity-detected-by-the-subobject-classifier)
    - [Local topos](#local-topos)
      - [Open cover criterion for a local sheaf topos](#open-cover-criterion-for-a-local-sheaf-topos)
      - [Initial object criterion for a covariant local topos](#initial-object-criterion-for-a-covariant-local-topos)
    - [Geometric morphism induced by a functor](#geometric-morphism-induced-by-a-functor)
      - [Full-faithfulness criterion for presheaf geometric embeddings](#full-faithfulness-criterion-for-presheaf-geometric-embeddings)
      - [Retract criterion for surjective presheaf geometric morphisms](#retract-criterion-for-surjective-presheaf-geometric-morphisms)
  - [Grothendieck topos](#grothendieck-topos)
    - [Classifying topos](#classifying-topos)
      - [Generic local ring](#generic-local-ring)
        - [Kock-Lawvere axiom for the generic local ring](#kock-lawvere-axiom-for-the-generic-local-ring)
      - [Classifying topos of strict linear orders](#classifying-topos-of-strict-linear-orders)
      - [Classifying topos of linear orders](#classifying-topos-of-linear-orders)
      - [Classifying topos of strict partial orders](#classifying-topos-of-strict-partial-orders)
      - [Classifying topos of partial orders](#classifying-topos-of-partial-orders)
      - [Duality between geometric quotients and subtoposes](#duality-between-geometric-quotients-and-subtoposes)
      - [Morita equivalence of geometric theories](#morita-equivalence-of-geometric-theories)
      - [Classifying topos of integral domains](#classifying-topos-of-integral-domains)
        - [Finite-tuple weak-field property of the generic integral domain](#finite-tuple-weak-field-property-of-the-generic-integral-domain)
        - [Empty-cover criterion for the domain-classifying site](#empty-cover-criterion-for-the-domain-classifying-site)
      - [Quotient-theory coverage](#quotient-theory-coverage)
      - [Generic model of an algebraic theory](#generic-model-of-an-algebraic-theory)
  - [Decidable object in a topos](#decidable-object-in-a-topos)
    - [Decidability in a set-valued functor category](#decidability-in-a-set-valued-functor-category)
    - [Quotients of decidable objects](#quotients-of-decidable-objects)
  - [Internal logic of a topos](#internal-logic-of-a-topos)
  - [Subobject classifier](#subobject-classifier)
    - [Shift epimorphism of the natural-number presheaf classifier](#shift-epimorphism-of-the-natural-number-presheaf-classifier)
    - [Monic endomorphism of a subobject classifier](#monic-endomorphism-of-a-subobject-classifier)
    - [Internal Heyting algebra of truth values](#internal-heyting-algebra-of-truth-values)
  - [Lawvere-Tierney topology](#lawvere-tierney-topology)
    - [Dense monomorphism classifier](#dense-monomorphism-classifier)
    - [Quasi-closed local operator](#quasi-closed-local-operator)
      - [Boolean cover by a generic quasi-closed subtopos](#boolean-cover-by-a-generic-quasi-closed-subtopos)
    - [Closed local operator](#closed-local-operator)
    - [Open local operator](#open-local-operator)
      - [Least dense truth characterizes an open local operator](#least-dense-truth-characterizes-an-open-local-operator)
      - [Complementary open and closed local operators](#complementary-open-and-closed-local-operators)
    - [Closure operation of a local operator](#closure-operation-of-a-local-operator)
      - [j-closed monomorphism](#j-closed-monomorphism)
      - [j-dense monomorphism](#j-dense-monomorphism)
    - [j-sheaf](#j-sheaf)
      - [j-separated object](#j-separated-object)
      - [Closed-subobject classifier](#closed-subobject-classifier)
      - [Sheaf reflector for a local operator](#sheaf-reflector-for-a-local-operator)
        - [Subobject-classifier preservation criterion for a sheaf reflector](#subobject-classifier-preservation-criterion-for-a-sheaf-reflector)

## Bicategory

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bicategory)

A bicategory has objects, hom-categories, composition functors and identity 1-cells. Associativity and unit laws hold through coherent invertible 2-cells, satisfying pentagon and triangle identities. A [monoidal category](#monoidal-category) is exactly a bicategory with a single object: its objects are the 1-cells, its morphisms the 2-cells, and its tensor product the horizontal composition.

## Coreflexive pair

↑ **Parent:** [Category theory](category-theory.md)

A coreflexive pair $f,g:B\rightrightarrows A$ has a common retraction $r:A\to B$ with $rf=rg=1_B$. It is the dual of a [reflexive pair](#reflexive-pair). Both $f$ and $g$ are [split monomorphisms](category.md#split-monomorphism).

## Coherent category

↑ **Parent:** [Category theory](category-theory.md)

A coherent category has [finite limits](category.md#finite-limit), pullback-stable regular-epi/mono image factorizations, and finite unions of subobjects stable under pullback. Each subobject lattice is distributive. These structures interpret all constructors of [coherent logic](mathematical-logic.md#coherent-logic).

### Coherent functor

↑ **Parent:** [Coherent category](#coherent-category)

A [functor](category.md#functor) between [coherent categories](#coherent-category) is coherent when it preserves [finite limits](category.md#finite-limit), image factorizations and finite unions of [subobjects](category.md#subobject), including the empty union. It consequently preserves the interpretation of every [coherent formula](mathematical-logic.md#coherent-formula). A [coherent functor](#coherent-functor) from a [coherent syntactic category](mathematical-logic.md#coherent-syntactic-category) to a [topos](#elementary-topos) is equivalent to a model of the corresponding [coherent theory](mathematical-logic.md#coherent-theory); [natural transformations](category.md#natural-transformation) correspond to ordinary model homomorphisms.

### Coherent topology

↑ **Parent:** [Coherent category](#coherent-category)

The coherent topology on a small [coherent category](#coherent-category) is generated by finite families of arrows whose image subobjects have union equal to the whole target. Pullback stability of images and unions and closure under composition make these a coverage. On a [coherent syntactic category](mathematical-logic.md#coherent-syntactic-category), this is the site topology used to construct the [classifying topos](#classifying-topos) of its [coherent theory](mathematical-logic.md#coherent-theory).

### Unions of subobjects are pushouts

↑ **Parent:** [Coherent category](#coherent-category)

In a [coherent category](#coherent-category), maps $A\to Y$ and $B\to Y$ agreeing on the intersection define a relation from $A\cup B$ to $Y$ by taking the union of their graphs. It is total because the two subobjects cover their union, and single-valued because the maps agree on overlap. [Total functional relations define morphisms](category.md#total-functional-relations-define-morphisms), giving a unique glued map. This is the [pushout](category.md#pushout) universal property without assuming a general supply of pushouts.

## Right lifting property

↑ **Parent:** [Category theory](category-theory.md)

A map $p$ has the right lifting property against $i:A\to B$ when every commutative square with $i$ on the left and $p$ on the right has a diagonal $B\to\operatorname{dom}p$ making both triangles commute. Lifting against a family of maps gives a class of right-injective maps.

## Model category

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Model_category)

A complete and cocomplete [category](category.md) with designated [model weak equivalences](#model-weak-equivalence), [model fibrations](#model-fibration) and [model cofibrations](#model-cofibration), closed under retracts. Weak equivalences satisfy two-out-of-three; maps admit the two cofibration/fibration factorizations, and either acyclic class has the required lifting property against the opposite class. These axioms organize homotopy-theoretic calculations abstractly.

### Small object argument

↑ **Parent:** [Model category](#model-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Small_object_argument)

Attach cells for all lifting squares at each successive stage, then take a suitable colimit. Smallness of the generating domains makes every eventual lifting square occur at an earlier stage. This factors a map into a [relative cell complex](#relative-cell-complex) followed by a map with the prescribed [right lifting property](#right-lifting-property).

#### Relative cell complex

↑ **Parent:** [Small object argument](#small-object-argument)

A composite built by successive pushouts of coproducts of prescribed generating maps. In nonnegative chain complexes, attaching a sphere-to-disk generator adds a free element with a specified existing cycle as boundary. The resulting inclusion has a degreewise free cokernel.

#### Sequentially small object

↑ **Parent:** [Small object argument](#small-object-argument)

Mapping out of the object preserves sequential colimits. A map factors through a finite stage, and two finite-stage maps agreeing in the colimit agree at a later stage. Relative sequential smallness restricts the diagrams to a stated class of morphisms.

### Projective model structure on nonnegative chain complexes

↑ **Parent:** [Model category](#model-category)

The [model category](#model-category) of nonnegative complexes of left modules has [quasi-isomorphisms](homology.md#quasi-isomorphism) as [model weak equivalences](#model-weak-equivalence), positive-degree surjections as [model fibrations](#model-fibration), and degreewise injections with projective cokernel as [model cofibrations](#model-cofibration). All objects are fibrant; cofibrant objects are degreewise projective.

#### Generating cofibrations for nonnegative chain complexes

↑ **Parent:** [Projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes)

The [sphere chain complex](homology.md#sphere-chain-complex) inclusions into [disk chain complexes](homology.md#disk-chain-complex), together with the separate degree-zero cell, generate the [model cofibrations](#model-cofibration) by cell attachment and retracts. Their right-injective class is exactly the [acyclic fibration in the projective chain-complex model structure](#acyclic-fibration-in-the-projective-chain-complex-model-structure).

##### Lifting characterization of an acyclic chain-complex fibration

↑ **Parent:** [Generating cofibrations for nonnegative chain complexes](#generating-cofibrations-for-nonnegative-chain-complexes)

The [right lifting property](#right-lifting-property) for each sphere-to-disk map fills a prescribed cycle and a compatible target element. The degree-zero generator supplies initial surjectivity; all other fillers force an acyclic kernel and the remaining degreewise surjections.

#### Acyclic fibration in the projective chain-complex model structure

↑ **Parent:** [Projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes)

A map that is both a [model fibration](#model-fibration) and a [quasi-isomorphism](homology.md#quasi-isomorphism). The homology isomorphism together with degree-one surjectivity forces surjectivity in degree zero. Equivalently it has the [right lifting property](#right-lifting-property) against the [generating cofibrations for nonnegative chain complexes](#generating-cofibrations-for-nonnegative-chain-complexes).

### Model cofibration

↑ **Parent:** [Model category](#model-category)

A morphism in the chosen cofibration class of a [model category](#model-category). In the [projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes) it is a degreewise split injection with degreewise projective cokernel. This usage is distinguished from the topological [cofibration](algebraic-topology.md#cofibration).

### Model fibration

↑ **Parent:** [Model category](#model-category)

A morphism in the chosen fibration class of a [model category](#model-category). In the [projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes), it is surjective in strictly positive degrees; degree zero is not required.

### Model weak equivalence

↑ **Parent:** [Model category](#model-category)

A morphism in the chosen weak-equivalence class of a [model category](#model-category). In the [projective model structure on nonnegative chain complexes](#projective-model-structure-on-nonnegative-chain-complexes) these are [quasi-isomorphisms](homology.md#quasi-isomorphism).

## Monoidal category

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monoidal_category)

A [category](category.md) equipped with a [monoidal tensor product](#monoidal-tensor-product), a [monoidal unit object](#monoidal-unit-object), and natural [associators](#associator) and [unitors](#unitor) satisfying the pentagon and triangle axioms.

### Product and coproduct monoidal structures on sets

↑ **Parent:** [Monoidal category](#monoidal-category)

Cartesian product with singleton unit and disjoint union with empty unit each make the [Category of sets](category.md#category-of-sets) monoidal. Associators and unitors simply retag or rebracket the same elements, so the pentagon and triangle identities hold elementwise. These structures differ even up to monoidal equivalence: any category equivalence preserves initial and terminal objects, so it cannot identify the empty unit with the singleton unit.

### Triangle identity for a monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)

The [associator](#associator) and [unitors](#unitor) of a [monoidal category](#monoidal-category) satisfy

$$
(1_X\otimes\lambda_Y)a_{X,I,Y}=\rho_X\otimes1_Y.
$$

Thus the two ways to remove a unit between two tensor factors agree. Together with the [pentagon identity for a monoidal category](#pentagon-identity-for-a-monoidal-category) this implies all [unit identities derived from the monoidal pentagon and triangle](#unit-identities-derived-from-the-monoidal-pentagon-and-triangle) and the [monoidal coherence theorem](#monoidal-coherence-theorem).

### Pentagon identity for a monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)

For an [associator](#associator) $a$ in a [monoidal category](#monoidal-category), the two paths from $((W\otimes X)\otimes Y)\otimes Z$ to $W\otimes(X\otimes(Y\otimes Z))$ agree:

$$
a_{W,X,Y\otimes Z}a_{W\otimes X,Y,Z}=(1_W\otimes a_{X,Y,Z})a_{W,X\otimes Y,Z}(a_{W,X,Y}\otimes1_Z).
$$

This five-vertex diagram is the basic compatibility for reassociating four tensor factors. The [monoidal coherence theorem](#monoidal-coherence-theorem) extends it to arbitrary finite tensor expressions.

### Unit identities derived from the monoidal pentagon and triangle

↑ **Parent:** [Monoidal category](#monoidal-category)

The [associator](#associator) $a$ and [unitors](#unitor) of a [monoidal category](#monoidal-category) satisfy

$$
\rho_{X\otimes Y}=(1_X\otimes\rho_Y)a_{X,Y,I},\qquad
\lambda_{X\otimes Y}a_{I,X,Y}=\lambda_X\otimes1_Y,\qquad
\lambda_I=\rho_I.
$$

For the first identity, postcompose the pentagon on $X,Y,I,Z$ by $1_X\otimes(1_Y\otimes\lambda_Z)$, then use the triangle twice and cancel $a_{X,Y,Z}$. This gives the first equality after tensoring with $1_Z$; set $Z=I$ and cancel using the natural invertible right unitor. Reversing tensor order proves the second identity. Naturality of the left unitor at $\lambda_X$ gives $\lambda_{I\otimes X}=1_I\otimes\lambda_X$; comparing the second identity with the triangle on $I,I,X$ gives $(\lambda_I\otimes1_X)=(\rho_I\otimes1_X)$ and hence the last identity. These are consequences of the axioms, not extra axioms imported from the [monoidal coherence theorem](#monoidal-coherence-theorem).

<h3 id="yang-baxter-operator">Yang–Baxter operator</h3>

↑ **Parent:** [Monoidal category](#monoidal-category)

An invertible [morphism](algebra.md#morphism) $y:X\otimes X\to X\otimes X$ satisfying $(y\otimes1)(1\otimes y)(y\otimes1)=(1\otimes y)(y\otimes1)(1\otimes y)$ with coherent parentheses. It produces representations of the [braid groups](group.md#braid-group); a self-[braiding](#braiding) is an example.

### Dual pair in a monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)

Objects $X,Y$ with an [evaluation morphism](#evaluation-morphism) $e:X\otimes Y\to I$ and a [coevaluation morphism](#coevaluation-morphism) $n:I\to Y\otimes X$ satisfying both [snake identities](#snake-identity). These are categorical duality data, distinct from the locally convex [dual pair](topological-vector-space.md#dual-pair).

#### Quantum dimension

↑ **Parent:** [Dual pair in a monoidal category](#dual-pair-in-a-monoidal-category)

Closing an identity strand using compatible [evaluation morphisms](#evaluation-morphism) and [coevaluation morphisms](#coevaluation-morphism) gives the categorical dimension in a pivotal or ribbon setting. For the standard two-dimensional [quantum enveloping algebra of sl2](algebra.md#quantum-enveloping-algebra-of-sl2) [module](module-theory.md#module-mathematics), the weighted contraction has diagonal coefficients $q^{-1},q$, giving [quantum dimension](#quantum-dimension) $q+q^{-1}=[2]_q$. The chosen duality and framing conventions matter.

#### Snake identity

↑ **Parent:** [Dual pair in a monoidal category](#dual-pair-in-a-monoidal-category)

The two triangular identities $(e\otimes1_X)(1_X\otimes n)=1_X$ and $(1_Y\otimes e)(n\otimes1_Y)=1_Y$, with canonical [associators](#associator) and [unitors](#unitor) inserted, for a [dual pair in a monoidal category](#dual-pair-in-a-monoidal-category).

#### Coevaluation morphism

↑ **Parent:** [Dual pair in a monoidal category](#dual-pair-in-a-monoidal-category)

The unit-valued duality map $n:I\to Y\otimes X$ of a [dual pair in a monoidal category](#dual-pair-in-a-monoidal-category), constrained together with evaluation by both [snake identities](#snake-identity).

#### Evaluation morphism

↑ **Parent:** [Dual pair in a monoidal category](#dual-pair-in-a-monoidal-category)

For a [dual pair in a monoidal category](#dual-pair-in-a-monoidal-category), the contraction $e:X\otimes Y\to I$. In a [left closed monoidal category](#left-closed-monoidal-category), evaluation also denotes the adjunction map $[M,N]\otimes M\to N$.

### Left closed monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)

Using the convention $-\otimes M\dashv[M,-]$, every tensoring-on-the-right functor has a right [adjoint functor](category.md#adjoint-functors). Evaluation is $[M,N]\otimes M\to N$. Naming left and right closure varies in the literature, so the adjunction fixes the convention.

### Comonoid

↑ **Parent:** [Monoidal category](#monoidal-category)

The categorical dual of a [monoid object](#monoid-object): an object with coassociative [comultiplication](#comultiplication) and a [counit](#counit), with the ambient constraints included.

#### Counit

↑ **Parent:** [Comonoid](#comonoid)

The structure map $\varepsilon:C\to I$ of a [comonoid](#comonoid), with $(\varepsilon\otimes1)\Delta$ and $(1\otimes\varepsilon)\Delta$ equal to the inverse [unitors](#unitor). This is distinct from the counit of an [adjunction](category.md#adjoint-functors).

#### Comultiplication

↑ **Parent:** [Comonoid](#comonoid)

The structure map $\Delta:C\to C\otimes C$ of a [comonoid](#comonoid); it is coassociative up to the ambient [associator](#associator).

#### Comonoid morphism

↑ **Parent:** [Comonoid](#comonoid)

A [morphism](algebra.md#morphism) $f:C\to D$ satisfying $\Delta_Df=(f\otimes f)\Delta_C$ and $\varepsilon_Df=\varepsilon_C$.

### Monoid object

↑ **Parent:** [Monoidal category](#monoidal-category)

An object with multiplication $m:A\otimes A\to A$ and unit $j:I\to A$ satisfying associativity and unit diagrams using the ambient [associators](#associator) and [unitors](#unitor).

#### Frobenius monoid

↑ **Parent:** [Monoid object](#monoid-object)

A [monoid object](#monoid-object) $A$ with a [morphism](algebra.md#morphism) $\varepsilon:A\to I$ such that $\varepsilon m$ and a suitable coevaluation make $(A,A)$ a [dual pair in a monoidal category](#dual-pair-in-a-monoidal-category). In a category of [vector spaces](vector-space.md) this is a [Frobenius algebra](associative-algebra.md#frobenius-algebra). This condition alone is not the usual separability condition.

#### Bimonoid

↑ **Parent:** [Monoid object](#monoid-object)

An object that is both a [monoid object](#monoid-object) and a [comonoid](#comonoid) in a [braided monoidal category](#braided-monoidal-category), with $\Delta,\varepsilon$ preserving multiplication and unit. The product on its tensor square uses the ambient [braiding](#braiding).

##### Coquasitriangular structure

↑ **Parent:** [Bimonoid](#bimonoid)

In a [symmetric monoidal category](#symmetric-monoidal-category), a convolution-invertible scalar pairing $\gamma:H\otimes H\to I$ on a [bimonoid](#bimonoid) inducing the [comodule](linear-algebra.md#comodule) braiding $u\otimes v\mapsto\sum v_{(0)}\otimes u_{(0)}\gamma(u_{(1)},v_{(1)})$. Its multiplicativity, normalization and commutation axioms express the hexagon, unit and colinearity conditions. The notation abbreviates morphisms and ambient symmetries, not a requirement for elements.

#### Monoid morphism

↑ **Parent:** [Monoid object](#monoid-object)

A [morphism](algebra.md#morphism) $f:A\to B$ satisfying $fm_A=m_B(f\otimes f)$ and $fj_A=j_B$.

### Braided monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Braided_monoidal_category)

A [monoidal category](#monoidal-category) with natural invertible [braidings](#braiding) $c_{X,Y}:X\otimes Y\to Y\otimes X$ satisfying the two hexagon axioms. The equation $c_{Y,X}c_{X,Y}=1$ is an additional symmetric condition, not a braided axiom.

#### Free braided monoidal category on one object

↑ **Parent:** [Braided monoidal category](#braided-monoidal-category)

The [braided monoidal category](#braided-monoidal-category) generated by one object: objects are parenthesized tensor expressions in that object and the unit, and [morphisms](algebra.md#morphism) are structural isomorphisms and crossings subject to precisely the [monoidal category](#monoidal-category) and [braiding](#braiding) axioms.

#### Braid category

↑ **Parent:** [Braided monoidal category](#braided-monoidal-category)

The [braided monoidal category](#braided-monoidal-category) with objects $n\geq0$, endomorphism [groups](group.md) $B_n$, no arrows between unequal objects, tensor given by juxtaposition, and block-crossing [braiding](#braiding). Its tensor is strict.

#### Braided monoidal functor

↑ **Parent:** [Braided monoidal category](#braided-monoidal-category)

A [monoidal functor](#monoidal-functor) between [braided monoidal categories](#braided-monoidal-category) compatible with their [braidings](#braiding): $F(c_{X,Y})F_2(X,Y)=F_2(Y,X)c_{FX,FY}$.

#### Braiding

↑ **Parent:** [Braided monoidal category](#braided-monoidal-category)

The natural tensor interchange isomorphism in a [braided monoidal category](#braided-monoidal-category), constrained by the two hexagon axioms.

### Opmonoidal functor

↑ **Parent:** [Monoidal category](#monoidal-category)

A [functor](category.md#functor) with natural maps $F_2:F(X\otimes Y)\to FX\otimes FY$ and $F_0:FI\to I$ satisfying the reversed [monoidal functor](#monoidal-functor) associativity and unit diagrams. No invertibility is required.

#### Opmonoidal natural transformation

↑ **Parent:** [Opmonoidal functor](#opmonoidal-functor)

A [natural transformation](category.md#natural-transformation) $\tau:F\Rightarrow G$ satisfying $G_2\tau_{X\otimes Y}=(\tau_X\otimes\tau_Y)F_2$ and $G_0\tau_I=F_0$.

### Monoidal functor

↑ **Parent:** [Monoidal category](#monoidal-category)

Here the unqualified term allows lax comparison maps $F_2:FX\otimes FY\to F(X\otimes Y)$ and $F_0:I\to FI$, natural and compatible with [associators](#associator) and [unitors](#unitor). Invertible comparison maps give a [strong monoidal functor](#strong-monoidal-functor). The opposite direction gives an [opmonoidal functor](#opmonoidal-functor).

#### Frobenius monoidal functor

↑ **Parent:** [Monoidal functor](#monoidal-functor)

A [lax monoidal functor](#monoidal-functor) $\varphi$ and [opmonoidal functor](#opmonoidal-functor) $\psi$ on the same underlying [functor](category.md#functor), satisfying $\psi_{A\otimes B,C}\varphi_{A,B\otimes C}=(\varphi_{A,B}\otimes1)(1\otimes\psi_{B,C})$ and $\psi_{A,B\otimes C}\varphi_{A\otimes B,C}=(1\otimes\varphi_{B,C})(\psi_{A,B}\otimes1)$ in coherent notation. It transports [dual pairs in a monoidal category](#dual-pair-in-a-monoidal-category) and [Frobenius monoids](#frobenius-monoid).

#### Strong monoidal functor

↑ **Parent:** [Monoidal functor](#monoidal-functor)

A [monoidal functor](#monoidal-functor) whose tensor and unit comparison maps are isomorphisms.

##### Strict monoidal functor

↑ **Parent:** [Strong monoidal functor](#strong-monoidal-functor)

A [strong monoidal functor](#strong-monoidal-functor) whose comparison maps are identities. It preserves the tensor, unit and structural constraints exactly; its source need not be a [strict monoidal category](#strict-monoidal-category).

### Strict monoidal category

↑ **Parent:** [Monoidal category](#monoidal-category)

A [monoidal category](#monoidal-category) whose [associators](#associator) and [unitors](#unitor) are identities; the tensor and unit laws are then equalities of objects and [morphisms](algebra.md#morphism).

### Monoidal coherence theorem

↑ **Parent:** [Monoidal category](#monoidal-category)

Every diagram formed solely from the canonical [associators](#associator), [unitors](#unitor) and their inverses commutes. Consequently structural reparenthesizations can be suppressed in calculations; this statement does not make distinct [braidings](#braiding) equal.

#### Termination proof of monoidal coherence

↑ **Parent:** [Monoidal coherence theorem](#monoidal-coherence-theorem)

Orient associativity towards right association and unit maps towards deletion of unit symbols. A lexicographic measure consisting of the number of leaves and the sum of the sizes of left subtrees decreases at every step. All overlapping reductions have commuting completions: the essential cases are the [pentagon identity for a monoidal category](#pentagon-identity-for-a-monoidal-category), the [triangle identity for a monoidal category](#triangle-identity-for-a-monoidal-category), and the derived left and right unit identities. Induction on the decreasing measure makes every normalization arrow equal, proving that every structural arrow is determined by its endpoints.

#### Word normalization proof of monoidal coherence

↑ **Parent:** [Monoidal coherence theorem](#monoidal-coherence-theorem)

Associate to a finite ordered word $w$ the right-associated tensor $N(w)$, retaining a terminal unit: $N(\varnothing)=I$ and $N(Aw)=A\otimes N(w)$. Define concatenation maps recursively by

$$
c_{\varnothing,v}=\lambda_{N(v)},\qquad
c_{Au,v}=(1_A\otimes c_{u,v})a_{A,N(u),N(v)}.
$$

The [unit identities derived from the monoidal pentagon and triangle](#unit-identities-derived-from-the-monoidal-pentagon-and-triangle) give $c_{u,\varnothing}=\rho_{N(u)}$. Induction on $u$, using the pentagon in the induction step and left-unitor compatibility in the base case, gives

$$
c_{uv,w}(c_{u,v}\otimes1)=c_{u,vw}(1\otimes c_{v,w})a_{N(u),N(v),N(w)}.
$$

Normalize a letter by $\rho_A^{-1}$, a formal unit by $1_I$, and a tensor expression recursively using $c$. The displayed identities show that normalization commutes with each generating [associator](#associator) or [unitor](#unitor), and therefore also with inverses, tensor products and composites of them. Every structural arrow from expression $S$ to expression $T$ is consequently $\nu_T^{-1}\nu_S$, proving [monoidal coherence](#monoidal-coherence-theorem) without presupposing it.

### Unitor

↑ **Parent:** [Monoidal category](#monoidal-category)

The natural isomorphisms $\lambda_X:I\otimes X\to X$ and $\rho_X:X\otimes I\to X$ in a [monoidal category](#monoidal-category). Together with the [associator](#associator) they satisfy the triangle axiom.

### Associator

↑ **Parent:** [Monoidal category](#monoidal-category)

The natural isomorphism $\alpha_{X,Y,Z}:(X\otimes Y)\otimes Z\to X\otimes(Y\otimes Z)$ in a [monoidal category](#monoidal-category). It satisfies the pentagon axiom.

### Monoidal unit object

↑ **Parent:** [Monoidal category](#monoidal-category)

The distinguished object $I$ in a [monoidal category](#monoidal-category), with the natural [unitors](#unitor) $I\otimes X\cong X\cong X\otimes I$.

### Monoidal tensor product

↑ **Parent:** [Monoidal category](#monoidal-category)

The bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$ in a [monoidal category](#monoidal-category). Its associativity is expressed by the [associator](#associator), rather than equality in general.

## Category of groups

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Category_of_groups)

The category of groups has [groups](group.md) as objects and [group homomorphisms](group-theory.md#group-homomorphism) as morphisms. Its product is the [direct product of groups](group-theory.md#direct-product-of-groups), and its coproduct is the [free product](algebraic-topology.md#free-product), as expressed by the [universal property of a free product](algebraic-topology.md#universal-property-of-a-free-product).

## Injective object

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Injective_object)

An object $I$ is injective when every morphism $A\to I$ extends across every [monomorphism](category.md#monomorphism) $A\hookrightarrow B$ to a morphism $B\to I$. This is the categorical extension property of an [injective module](noncommutative-algebra.md#injective-module) or an [injective sheaf](algebraic-geometry.md#injective-sheaf); it is dual to the lifting property of a [projective object in a category](category.md#projective-object).

## Universal property

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universal_property)

A universal property characterizes an object by a prescribed family of [morphisms](algebra.md#morphism) and a unique factorization of every competing family. It determines that object up to a unique compatible [isomorphism](algebra.md#isomorphism). Examples include the [pushout in a category](category.md#pushout-in-a-category) and the [universal property of the tensor product of modules](module-theory.md#universal-property-of-the-tensor-product-of-modules).

## Category

↑ **Parent:** [Category theory](category-theory.md)

[This section is present in another page, follow this link to view it.](category.md)

## Symmetric monoidal category

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_monoidal_category)

A symmetric monoidal category has a tensor product, unit object, coherent associativity and unit isomorphisms, and a coherent symmetry $A\otimes B\cong B\otimes A$.

## Complete join-semilattice

↑ **Parent:** [Category theory](category-theory.md)

A complete join-semilattice is a poset with joins of all families, including the empty family. A morphism preserves arbitrary joins.

### Category of complete join-semilattices

↑ **Parent:** [Complete join-semilattice](#complete-join-semilattice)

The category $\mathbf{CSLat}$ has complete join-semilattices as objects and arbitrary-join-preserving maps as morphisms. Taking opposite orders and right adjoints gives an involutive self-duality.

#### Biproducts of complete join-semilattices

↑ **Parent:** [Category of complete join-semilattices](#category-of-complete-join-semilattices)

In the [category of complete join-semilattices](#category-of-complete-join-semilattices), hom-sets have pointwise join as addition and the constant-bottom map as zero, making it a [semi-additive category](#semi-additive-category). For any family $A_i$, the cartesian product with coordinatewise joins is also its coproduct. The injections put an element in one coordinate and bottom in all others. A family of maps $f_i:A_i\to B$ extends uniquely by $(a_i)\mapsto\bigvee_i f_i(a_i)$, since each tuple is the join of its coordinate injections. Thus all set-indexed canonical product-coproduct comparisons are invertible. The two-element chain has distinct identity and zero morphisms, so this category is not trivial and not additive.

## Enriched category

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enriched_category)

For a monoidal category $(\mathcal V,\otimes,I)$, a $\mathcal V$-enriched category has hom-objects in $\mathcal V$, composition morphisms $\mathcal C(B,C)\otimes\mathcal C(A,B)\to\mathcal C(A,C)$, and unit morphisms $I\to\mathcal C(A,A)$ satisfying associativity and unit laws.

### Commutative-monoid enrichment

↑ **Parent:** [Enriched category](#enriched-category)

A commutative-monoid enrichment gives each hom-set a [commutative monoid](algebra.md#commutative-monoid) structure, with zero and addition, so that composition distributes over addition in both variables and annihilates zero. This is called a semi-additive structure in some conventions, including Cambridge Part III paper 119 of 2017. Other conventions reserve [semi-additive category](#semi-additive-category) for categories with this enrichment and finite [biproducts](#biproduct). A one-object category arising from a [semiring](algebra.md#semiring) has the enrichment without generally having those finite products.

#### Transported addition on the multiplicative natural-number monoid

↑ **Parent:** [Commutative-monoid enrichment](#commutative-monoid-enrichment)

For a multiplicative [monoid automorphism](algebra.md#monoid-automorphism) $\phi:\mathbb N\to\mathbb N$ fixing $0$, define $a\oplus b=\phi^{-1}(\phi(a)+\phi(b))$. This transports a [semiring](algebra.md#semiring) structure to the fixed underlying multiplication, hence a [commutative-monoid enrichment](#commutative-monoid-enrichment) on its one-object category. Swapping prime $2$ with an [odd prime](number-theory.md#odd-prime) $p$ gives $1\oplus1=p$. Infinitely many such primes therefore give infinitely many distinct additions, although the transported enriched categories are isomorphic.

### Underlying category of an enriched category

↑ **Parent:** [Enriched category](#enriched-category)

The underlying ordinary category has the same objects and hom-sets $\mathcal V(I,\mathcal C(A,B))$.

### Self-enrichment of a closed symmetric monoidal category

↑ **Parent:** [Enriched category](#enriched-category)

A closed symmetric monoidal category enriches over itself using its internal hom objects. Composition is adjoint to the composite of evaluation morphisms.

### Poset-enriched adjunction

↑ **Parent:** [Enriched category](#enriched-category)

In a category whose hom-sets are posets, $f:A\to B$ is left adjoint to $g:B\to A$ when $fg\leq1_B$ and $1_A\leq gf$. Left adjoints are closed under identities and composition.

#### Left adjoint relation is a function

↑ **Parent:** [Poset-enriched adjunction](#poset-enriched-adjunction)

In the inclusion-ordered category of sets and relations, a relation has a right adjoint exactly when it is the graph of a total single-valued function; its right adjoint is the converse relation.

### Semi-additive category

↑ **Parent:** [Enriched category](#enriched-category)

A semi-additive category has a [commutative-monoid enrichment](#commutative-monoid-enrichment) and finite [products in a category](category.md#product-category-theory) and [coproducts in a category](category.md#coproduct). Composition preserves addition and zero in each variable. Every finite [product in a category](category.md#product-category-theory) is canonically a [coproduct in a category](category.md#coproduct) and conversely, producing finite [biproducts](#biproduct). Some authors use "semi-additive structure" for the [commutative-monoid enrichment](#commutative-monoid-enrichment) alone; that weaker convention also permits one-object [categories](category.md) without finite [products in a category](category.md#product-category-theory).

A [preadditive category](category.md#preadditive-category) instead has abelian-group-valued hom sets. Semi-additivity alone does not require additive inverses.

#### Biproduct

↑ **Parent:** [Semi-additive category](#semi-additive-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biproduct)

A biproduct $A\oplus B$ is simultaneously a [product in a category](category.md#product-category-theory) and a [coproduct in a category](category.md#coproduct), with projections $p_i$ and injections $i_i$ satisfying

$$
p_ii_j=\delta_{ij},
\qquad
i_1p_1+i_2p_2=1_{A\oplus B}.
$$

##### Biproduct-induced addition of morphisms

↑ **Parent:** [Biproduct](#biproduct)

In a [pointed category](category.md#pointed-category) with finite [product in a category](category.md#product-category-theory) and [coproducts in a category](category.md#coproduct) and invertible canonical maps $c:A+B\to A\times B$, the unique [commutative-monoid enrichment](#commutative-monoid-enrichment) is $f+g=[1_B,1_B]c_{B,B}^{-1}\langle f,g\rangle$. Associativity and commutativity follow by comparing fold maps on triple and swapped coproduct injections. Composition distributes by the universal properties. For uniqueness, bilinearity forces $i_1p_1+i_2p_2=1$ on each biproduct, and composing with the fold and the paired morphism forces the addition formula.

##### Countable biproducts in an additive category force triviality

↑ **Parent:** [Biproduct](#biproduct)

Suppose a [semi-additive category](#semi-additive-category) has countable products and coproducts and the canonical comparison between them is always invertible. For countably many copies of $A$, let $q:A\to\coprod_iA$ correspond under that comparison to the diagonal into the product, and let $\sigma:\coprod_iA\to A$ be the fold map. If $s$ shifts the summands by one, coordinatewise comparison proves $q=\nu_1+sq$ and $\sigma s=\sigma$. Thus $z=\sigma q$ satisfies $z=1_A+z$. In an [additive category](#additive-category), cancellation gives $1_A=0$, forcing every hom-set to contain only its zero morphism. The category is equivalent to the one-object, one-arrow category.

#### Additive category

↑ **Parent:** [Semi-additive category](#semi-additive-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_category)

An additive category is enriched in abelian groups, has a zero object and finite biproducts, and has bilinear composition.

##### Semisimple category

↑ **Parent:** [Additive category](#additive-category)

In the finite-dimensional setting, a semisimple category is an [additive category](#additive-category) over a [field](algebra.md#field) in which every object is a finite [biproduct](#biproduct) of simple objects, different simple objects have zero [morphism](algebra.md#morphism) spaces, and the [endomorphism](algebra.md#endomorphism) algebra of each simple object is a [division algebra](algebra.md#division-algebra). Such categories have finite [matrix](vector-space.md#matrix) blocks and all their [idempotents](commutative-algebra.md#idempotent) split. The [semisimplicity of the reduced Temperley-Lieb category](knot-theory.md#semisimplicity-of-the-reduced-temperley-lieb-category) gives an example whose simple objects are the surviving [Jones-Wenzl colors](knot-theory.md#jones-wenzl-color).

##### Additive category with truncated primary torsion

↑ **Parent:** [Additive category](#additive-category)

Fix a [prime number](number-theory.md#prime-number) $p$. Take the full [subcategory](category.md#subcategory) of [finitely generated abelian groups](group.md#finitely-generated-abelian-group) with no element of order $p^2$. It is closed under finite [direct sums](vector-space.md#direct-sum) and [subgroups](group.md#subgroup). If $t_p(G)$ is the $p$-primary [torsion subgroup](group-theory.md#torsion-subgroup), the map $G\to R(G)=G/(p\,t_p(G))$ is a [reflection](linear-algebra.md#reflection-mathematics) into this subcategory: every map to an allowed group kills $p\,t_p(G)$. Therefore ordinary [kernels in a category](category.md#kernel-in-a-category) and reflected [cokernels in a category](category.md#cokernel-in-a-category) supply all finite [categorical limits](category.md#categorical-limit) and [colimits](category.md#colimit). No nonzero finitely generated group has zero reflection, so the [epimorphisms](category.md#epimorphism) are precisely surjections and are all [conormal epimorphisms](category.md#conormal-epimorphism). Multiplication by $p^2$ on $\mathbb Z$ is a [monomorphism](category.md#monomorphism) but not a [normal monomorphism](category.md#normal-monomorphism): its cokernel here is $\mathbb Z/p\mathbb Z$, whose kernel is $p\mathbb Z$, not $p^2\mathbb Z$. Multiplication by $p$ is normal; composing it with itself gives this nonnormal monomorphism.

##### Additive functor

↑ **Parent:** [Additive category](#additive-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_functor)

An additive functor between additive categories induces a group homomorphism on every hom-group. It therefore preserves zero morphisms and finite biproducts.

###### Right-exact additive functor

↑ **Parent:** [Additive functor](#additive-functor)

An [additive functor](#additive-functor) between [abelian categories](#abelian-category) is [right exact functor](#right-exact-additive-functor) when it sends every exact sequence $X\to Y\to Z\to0$ to an exact sequence $FX\to FY\to FZ\to0$. Equivalently, it preserves [cokernels in a category](category.md#cokernel-in-a-category), since additivity already preserves finite [biproducts](#biproduct). This is the convention used in constructing [left derived functors](algebra.md#left-derived-functor). Left exactness preserves the initial part $0\to X\to Y\to Z$ instead. Contravariant Hom becomes a [right exact functor](#right-exact-additive-functor) covariant [functor](category.md#functor) with target the opposite [abelian category](#abelian-category).

An [additive functor](#additive-functor) between [abelian categories](#abelian-category) is [right exact](#right-exact-additive-functor) when it preserves [categorical cokernels](category.md#cokernel-in-a-category), equivalently when it sends every exact sequence ending in zero to an exact sequence ending in zero. Additivity and preservation of [cokernels in a category](category.md#cokernel-in-a-category) imply preservation of finite [colimits](category.md#colimit). The additivity assumption is part of the ordinary [left derived functor](algebra.md#left-derived-functor) construction.

##### Abelian category

↑ **Parent:** [Additive category](#additive-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelian_category)

An abelian category is an additive category with all kernels and cokernels in which every monomorphism and epimorphism is normal.

###### Cofinitary abelian category

↑ **Parent:** [Abelian category](#abelian-category)

A complete [abelian category](#abelian-category) is cofinitary when its [opposite category](category.md#opposite-category) is a [finitary abelian category](#finitary-abelian-category). Thus a cone of epimorphisms over an inverse directed diagram induces an epimorphism from its vertex to the limit.

###### Finitary abelian category

↑ **Parent:** [Abelian category](#abelian-category)

A cocomplete [abelian category](#abelian-category) is finitary in the directed-union sense if every [cocone under a diagram](category.md#cocone-under-a-diagram) indexed by a nonempty directed [poset](set.md#partially-ordered-set), with all its legs [monomorphisms](category.md#monomorphism), induces a monomorphism from the colimit to the cocone vertex. The [category of abelian groups](#category-of-abelian-groups) has this property: two colimit representatives mapped to the same vertex become equal at a common upper index because that cocone leg is injective. This use of finitary concerns directed unions, rather than the preservation-of-filtered-colimits meaning used for [finitary monads](#finitary-monad).

###### Coproduct-to-product comparison in a finitary abelian category

↑ **Parent:** [Finitary abelian category](#finitary-abelian-category)

In a complete [finitary abelian category](#finitary-abelian-category), the comparison $j$ with diagonal matrix entries the identity and off-diagonal entries zero is monic. Express its source as the directed colimit of finite [biproducts](#biproduct). Their maps into the product have finite-coordinate retractions and are therefore [split monomorphisms](category.md#split-monomorphism); the finitary axiom applies to this cocone. If the category is also [cofinitary abelian category](#cofinitary-abelian-category), duality makes $j$ epic and hence invertible. For countably many copies of any object, the shift-and-fold argument in [countable biproducts in an additive category force triviality](#countable-biproducts-in-an-additive-category-force-triviality) then forces the identity to be zero, so every object is a zero object.

###### Category of abelian groups

↑ **Parent:** [Abelian category](#abelian-category)

Objects are [abelian groups](group.md#abelian-group) and morphisms are [group homomorphisms](group-theory.md#group-homomorphism). Addition on hom-sets is pointwise, kernels are subgroup kernels, and cokernels are quotients by images. Thus this is an [abelian category](#abelian-category). Products are Cartesian products; coproducts are direct sums of finite-support families. The underlying-set [functor](category.md#functor) creates directed colimits, giving a concrete description of their elements by eventual equality of representatives.

###### Abelian category with enough projectives

↑ **Parent:** [Abelian category](#abelian-category)

An [abelian category](#abelian-category) has enough projectives when every object admits an [epimorphism](category.md#epimorphism) from a [projective object in a category](category.md#projective-object). Repeating this on the [kernel in a category](category.md#kernel-in-a-category) constructs a [projective resolution](algebra.md#projective-resolution) of every object. Finite direct sums of projective objects remain projective and give the degreewise split horseshoe construction.

###### Hereditary abelian category with enough projectives

↑ **Parent:** [Abelian category](#abelian-category)

An [abelian category](#abelian-category) with enough projectives is hereditary when every [subobject](category.md#subobject) of a projective object is projective. For $0\to K\to P\to A\to0$ with $P$ projective, dimension shifting gives $L_2F(A)\cong L_1F(K)$. Hence hereditaryness is equivalent to vanishing of $L_2F$ for every additive [right exact functor](#right-exact-additive-functor) into any abelian [category](category.md), by [projectivity detected by all first left derived functors](category.md#projectivity-detected-by-all-first-left-derived-functors). It is also equivalent to left exactness of every $L_1F$: the derived long exact sequence gives injectivity of $L_1F(K)\to L_1F(P)$ when $L_2F$ vanishes, and applying left exactness to the displayed sequence proves the converse.

###### Kernel squares in an abelian category

↑ **Parent:** [Abelian category](#abelian-category)

In a commutative diagram of two kernel rows, a monic arrow between the final objects makes the square between their kernels and middle objects a [pullback in a category](category.md#pullback-category-theory). The kernel [universal property](#universal-property) factors any [categorical cone](category.md#cone-over-a-diagram) uniquely. Conversely, if the square between middle and final objects is a pullback, the induced arrow between their [kernels in a category](category.md#kernel-in-a-category) is an [isomorphism](algebra.md#isomorphism), since both kernels have the same [universal property](#universal-property) after pullback.

###### Zero-cokernel criterion for epimorphisms

↑ **Parent:** [Abelian category](#abelian-category)

In an [abelian category](#abelian-category), a morphism is an [epimorphism](category.md#epimorphism) if and only if its [categorical cokernel](category.md#cokernel-in-a-category) object is zero. For the reverse implication, any difference of maps annihilating the morphism factors through its cokernel and is therefore zero. The [cokernel invariance under pushout](category.md#cokernel-invariance-under-pushout) then proves both preservation and reflection of epimorphisms by pushout.

###### Pullback stability of epimorphisms in an abelian category

↑ **Parent:** [Abelian category](#abelian-category)

In an [abelian category](#abelian-category), the [pullback in a category](category.md#pullback-category-theory) of an [epimorphism](category.md#epimorphism) $p:B\to C$ along $k:C'\to C$ is the kernel of the epimorphism $[p,-k]:B\oplus C'\to C$. If $v:C'\to D$ annihilates its projection, $[0,v]$ annihilates that kernel and therefore factors through $[p,-k]$. Restriction to $B$ forces the factor to vanish, giving $v=0$ and proving the projection epic. This uses the definition's normality of epimorphisms.

###### Pullback of an epimorphism is a pushout in an abelian category

↑ **Parent:** [Pullback stability of epimorphisms in an abelian category](#pullback-stability-of-epimorphisms-in-an-abelian-category)

In an [abelian category](#abelian-category), suppose a commutative square $gf=kh$ is a [pullback in a category](category.md#pullback-category-theory) and $g$ is an [epimorphism](category.md#epimorphism). Then $(f,h):A\to B\oplus C$ is the [categorical kernel](category.md#kernel-in-a-category) of the epimorphism $[g,-k]$. Since an epimorphism is the cokernel of its kernel, any compatible pair $u:B\to X$, $v:C\to X$ induces a unique map $D\to X$ by factoring $[u,-v]$. Hence the square is also a [pushout in a category](category.md#pushout-in-a-category).

###### Every abelian category is regular

↑ **Parent:** [Abelian category](#abelian-category)

An abelian category has finite limits, and every morphism factors through its image as an epimorphism followed by a monomorphism. Every epimorphism is the cokernel of its kernel, hence a [regular epimorphism](category.md#regular-epimorphism), and epimorphisms in an abelian category are stable under pullback. Therefore every abelian category is a [regular category](category.md#regular-category).

###### Image and coimage in an abelian category

↑ **Parent:** [Abelian category](#abelian-category)

For $f:A\to B$ in an abelian category,

$$
\operatorname{im}f=\ker(\operatorname{coker}f),
\qquad
\operatorname{coim}f=\operatorname{coker}(\ker f).
$$

The canonical morphism $\operatorname{coim}f\to\operatorname{im}f$ is an isomorphism, giving the canonical epimorphism--isomorphism--monomorphism factorization of $f$.

###### Coimage

↑ **Parent:** [Image and coimage in an abelian category](#image-and-coimage-in-an-abelian-category)

In an [abelian category](#abelian-category), the coimage of a [morphism](algebra.md#morphism) is its domain modulo its [kernel in a category](category.md#kernel-in-a-category), expressed as a [cokernel in a category](category.md#cokernel-in-a-category). The canonical arrow from the coimage to the image is an [isomorphism](algebra.md#isomorphism), giving the [image factorization in an abelian category](category.md#image-factorization-in-an-abelian-category).

###### Exact sequence in an abelian category

↑ **Parent:** [Abelian category](#abelian-category)

A sequence is exact at an object when the image of the incoming morphism equals the kernel of the outgoing morphism. It is exact when this holds everywhere.

###### Short exact sequence in an abelian category

↑ **Parent:** [Exact sequence in an abelian category](#exact-sequence-in-an-abelian-category)

A short [exact sequence in an abelian category](#exact-sequence-in-an-abelian-category) has one nonzero morphism entering the middle object and one leaving it: $0\to A\xrightarrow{i}B\xrightarrow{p}C\to0$. Equivalently, $i$ is the [kernel in a category](category.md#kernel-in-a-category) of the [epimorphism](category.md#epimorphism) $p$. It splits if $p$ has a section; in that case the [additive category](#additive-category) splitting argument identifies $B$ with the [biproduct](#biproduct) $A\oplus C$. Categories of [modules](module-theory.md#module-mathematics) give familiar examples.

###### Schanuel lemma in an abelian category

↑ **Parent:** [Short exact sequence in an abelian category](#short-exact-sequence-in-an-abelian-category)

Two projective presentations of the same object in an [abelian category](#abelian-category), with kernels $K,K'$ and middle objects $P,P'$, satisfy $K\oplus P'\cong K'\oplus P$. Form their [pullback in a category](category.md#pullback-category-theory). Its two induced [short exact sequences in an abelian category](#short-exact-sequence-in-an-abelian-category) split because each quotient is a [projective object in a category](category.md#projective-object). The two resulting [biproduct](#biproduct) descriptions of the pullback give the isomorphism.

###### Pullback of a short exact sequence in an abelian category

↑ **Parent:** [Short exact sequence in an abelian category](#short-exact-sequence-in-an-abelian-category)

Pulling back the final arrow of a [short exact sequence in an abelian category](#short-exact-sequence-in-an-abelian-category) preserves its kernel object and yields another [short exact sequence in an abelian category](#short-exact-sequence-in-an-abelian-category). The new kernel inclusion is specified by its old kernel component and zero component into the new quotient. The [pullback stability of epimorphisms in an abelian category](#pullback-stability-of-epimorphisms-in-an-abelian-category) ensures the new final arrow remains epic.

###### Five lemma

↑ **Parent:** [Exact sequence in an abelian category](#exact-sequence-in-an-abelian-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Five_lemma)

In a commutative diagram of two exact five-term sequences, if the first and fourth vertical maps are epimorphisms and the second and fifth are monomorphisms, then an isomorphism in the middle follows; in particular, four surrounding isomorphisms force the fifth.

###### Five lemma via image factorization

↑ **Parent:** [Five lemma](#five-lemma)

For commuting five-term [exact sequences](homology.md#exact-sequence) in an [abelian category](#abelian-category), the first vertical map being epic and the second invertible give an invertible induced map on the images entering the middle objects, because these images are the cokernels of the first horizontal maps. The fourth vertical map being invertible and the fifth monic similarly give an invertible map on the images leaving the middle objects, because these are the kernels of the last horizontal maps. The [image factorization in an abelian category](category.md#image-factorization-in-an-abelian-category) packages each middle object between these two images in a [short exact sequence](module-theory.md#short-exact-sequence). The [short five lemma](module-theory.md#short-five-lemma) then makes the middle vertical map invertible. The proof is categorical and does not require an embedding into a category of modules.

###### Snake lemma

↑ **Parent:** [Exact sequence in an abelian category](#exact-sequence-in-an-abelian-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Snake_lemma)

A morphism between two short exact sequences in an abelian category induces an exact sequence

$$
\ker f'\to\ker f\to\ker f''\xrightarrow{\partial}
\operatorname{coker}f'\to\operatorname{coker}f\to\operatorname{coker}f''.
$$

###### Complex in an abelian category

↑ **Parent:** [Abelian category](#abelian-category)

A complex in an abelian category is a sequence $\cdots\to A_{n+1}\xrightarrow{d_{n+1}}A_n\xrightarrow{d_n}A_{n-1}\to\cdots$ with $d_nd_{n+1}=0$.

###### Additive indexing category for chain complexes

↑ **Parent:** [Complex in an abelian category](#complex-in-an-abelian-category)

Let $\mathbf Z$ have the [integers](number-theory.md#integer) as objects, with $\mathbf Z(n,p)=\mathbb Z$ for $p=n$ or $p=n-1$ and zero otherwise. Composition is bilinear, the generator of $\mathbf Z(n,n)$ is the identity, and the composite of two degree-lowering generators is zero. Additive functors $\mathbf Z\to\mathcal A$ are exactly chain complexes in the additive category $\mathcal A$.

###### Homology object

↑ **Parent:** [Complex in an abelian category](#complex-in-an-abelian-category)

The homology object is $H_n=\ker d_n/\operatorname{im}d_{n+1}$, formed categorically as the cokernel of the image-to-kernel monomorphism.

###### Self-duality of homology

↑ **Parent:** [Homology object](#homology-object)

Let $q:C_n\to\operatorname{coker}d_{n+1}$. Since $d_nd_{n+1}=0$, there is an induced $\bar d_n:\operatorname{coker}d_{n+1}\to C_{n-1}$. In an [abelian category](#abelian-category),

$$
\operatorname{coker}\bigl(\operatorname{im}d_{n+1}\to\ker d_n\bigr)
\cong
\ker\bar d_n.
$$

The left side is the usual homology construction and the right side is its construction in the [opposite category](category.md#opposite-category), so the definition of homology is self-dual.

## Monad

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monad_(category_theory))

A monad is an endofunctor $T$ with unit and multiplication satisfying associativity and unit laws.

### Square reader monad

↑ **Parent:** [Monad](#monad)

The unit repeats an element and multiplication selects the two outer diagonal entries. Both unit laws hold directly, and the associativity law selects the same two diagonal entries of an eight-entry array. Its [algebras for a monad](#algebra-for-a-monad) are precisely [rectangular bands](algebra.md#rectangular-band), including the empty algebra.

### Equalizer submonad of a monad

↑ **Parent:** [Monad](#monad)

In a [category](category.md) with [equalizers](category.md#equaliser), the equalizer of $\eta_{TA},T\eta_A$ defines a [functor](category.md#functor) $R$ by $\beta_BRf=Tf\beta_A$. It has unit $\alpha$ and multiplication $\theta$ characterized by

$$
\beta_A\alpha_A=\eta_A,\qquad \beta_A\theta_A=\mu_AT\beta_A\beta_{RA}.
$$

Cancelling the monomorphisms $\beta_A$ reduces its unit and associativity laws to those of $T$, so $\beta:R\Rightarrow T$ is a [monad morphism](#monad-morphism). The [split equalizers associated with a monad](category.md#split-equalizers-associated-with-a-monad) show that $\alpha_{TA}$ is invertible. If every $T\beta_A$ is monic, then every $T\alpha_A$ is invertible, the naturality square of $\beta$ at $\beta_A$ is a [pullback in a category](category.md#pullback-category-theory), and $R$ is an [idempotent monad](#idempotent-monad). This monicity hypothesis is essential to this last argument; arbitrary [functors](category.md#functor) need not preserve monomorphisms.

### Monad morphism

↑ **Parent:** [Monad](#monad)

A [morphism](algebra.md#morphism) of [monads](#monad) on one [category](category.md) is a [natural transformation](category.md#natural-transformation) $\alpha:S\Rightarrow T$ with $\alpha\eta^S=\eta^T$ and $\alpha\mu^S=\mu^T(T\alpha)(\alpha S)$. These equations preserve the unit and multiplication. A terminal [endofunctor](category.md#endofunctor) in a full composition-closed subcategory containing the identity receives a unique such [morphism](algebra.md#morphism) from every [monad](#monad) whose [functor](category.md#functor) belongs to that subcategory.

#### Restriction of monad algebras

↑ **Parent:** [Monad morphism](#monad-morphism)

A [monad morphism](#monad-morphism) $\alpha:S\Rightarrow T$ induces a [functor](category.md#functor) $\mathcal C^T\to\mathcal C^S$ between [Eilenberg-Moore categories](#eilenberg-moore-category), identical on underlying objects and arrows. Its unit equation gives the restricted algebra's unit law. Naturality and the multiplication equation give $(a\alpha_A)S(a\alpha_A)=aTa\,\alpha_{TA}S\alpha_A=a\mu_A^T T\alpha_A\alpha_{SA}=a\alpha_A\mu_A^S$. Naturality also preserves algebra [morphisms](algebra.md#morphism).

### List monad

↑ **Parent:** [Monad](#monad)

On the [Category of sets](category.md#category-of-sets), the list [monad](#monad) sends $X$ to all finite ordered lists of elements of $X$, including the empty list. Its unit inserts a singleton list and its multiplication concatenates a list of lists. Functoriality is entrywise application of functions. Ordered flattening proves the monad laws. This is the free-[monoid](algebra.md#monoid) monad, so order must not be discarded.

#### List-monad algebras are monoids

↑ **Parent:** [List monad](#list-monad)

An [algebra for a monad](#algebra-for-a-monad) for the [list monad](#list-monad) is precisely a [monoid](algebra.md#monoid). For an action $a$, the identity is $a([])$ and multiplication is $a([x,y])$. The algebra laws force the unit and associativity laws and determine $a$ as ordered multiplication. Conversely ordered multiplication defines a list action. Algebra morphisms are exactly [monoid homomorphisms](algebra.md#monoid-homomorphism), giving an isomorphism of categories $\mathbf{Set}^{\mathrm{List}}\cong\mathbf{Mon}$.

### Unit and multiplication of a monad

↑ **Parent:** [Monad](#monad)

The natural maps $\eta:1\Rightarrow T$ and $\mu:T^2\Rightarrow T$ defining a [monad](#monad), subject to the associativity and two unit identities.

### Opmonoidal monad

↑ **Parent:** [Monad](#monad)

A [monad](#monad) whose endofunctor is an [opmonoidal functor](#opmonoidal-functor) and whose unit and multiplication are [opmonoidal natural transformations](#opmonoidal-natural-transformation). Its [Eilenberg-Moore category](#eilenberg-moore-category) has a tensor of algebras $(X,a)\otimes(Y,b)=(X\otimes Y,(a\otimes b)T_2)$ and unit $(I,T_0)$.

### Shift monad on order-preserving maps of natural numbers

↑ **Parent:** [Monad](#monad)

Let $M$ be the [monoid](algebra.md#monoid) of [order-preserving functions](set.md#order-preserving-function) $\mathbb N\to\mathbb N$, with $\mathbb N=\{0,1,\ldots\}$, regarded as a one-object [category](category.md). The endofunctor $T$ fixes that object and sends $f$ to $Tf(0)=0$, $Tf(n+1)=f(n)+1$. The displayed maps give its [monad](#monad) unit and multiplication. The multiplication is not injective, so this is not an [idempotent monad](#idempotent-monad). Its only [algebra for a monad](#algebra-for-a-monad) is $\mu$, because $a\eta=1$ forces $a(n+1)=n$ and monotonicity forces $a(0)=0$. Algebra endomorphisms are exactly the functions fixing zero. The [Kleisli comparison functor](#kleisli-comparison-functor) sends $f$ to the function which is zero at zero and equals $f(n)$ at $n+1$; its inverse sends $h$ to $n\mapsto h(n+1)$. Thus the comparison is an isomorphism of categories even though the monad is not idempotent.

### Idempotent monad

↑ **Parent:** [Monad](#monad)

A monad is idempotent when its multiplication is invertible. Then $T\eta=\eta T=\mu^{-1}$. If $(A,a)$ is an [algebra for a monad](#algebra-for-a-monad), its unit law and naturality give $a\eta_A=1_A$ and $\eta_Aa=Ta\,\eta_{TA}=T(a\eta_A)=1_{TA}$. Thus every algebra is isomorphic to a free algebra, and the [Kleisli comparison functor](#kleisli-comparison-functor) into the [Eilenberg-Moore category](#eilenberg-moore-category) is an equivalence.

### Monad structure on a terminal endofunctor

↑ **Parent:** [Monad](#monad)

Let a full subcategory of the endofunctor category contain the identity, be closed under composition, and have terminal object $T$. Then $T$ has a unique monad structure: the unit $1\to T$ and multiplication $T^2\to T$ are the unique maps to the terminal object. The monad laws hold because each compares two maps with codomain $T$ from the same object.

#### Ultrafilter monad

↑ **Parent:** [Monad structure on a terminal endofunctor](#monad-structure-on-a-terminal-endofunctor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrafilter_monad)

The [ultrafilter functor](set-theory.md#ultrafilter-functor) carries the monad structure obtained from its terminality among finite-coproduct-preserving endofunctors of sets. Its unit sends a point to its [principal ultrafilter](set-theory.md#principal-ultrafilter); its multiplication sends an ultrafilter of ultrafilters to the ultrafilter of subsets whose corresponding basic set of ultrafilters is large.

### Monad induced by an adjunction

↑ **Parent:** [Monad](#monad)

An adjunction $F\dashv G$ with unit $\eta$ and counit $\varepsilon$ induces the monad

$$
T=GF,\qquad \mu=G\varepsilon F,
$$

with unit $\eta$.

#### Category of adjunctions inducing a fixed monad

↑ **Parent:** [Monad induced by an adjunction](#monad-induced-by-an-adjunction)

Fix a [monad](#monad) on $\mathcal C$. Objects are [adjunctions](category.md#adjoint-functors) with left-hand [category](category.md) $\mathcal C$ whose induced monads are identified with the fixed monad. A [morphism](algebra.md#morphism) between two such adjunctions is a [functor](category.md#functor) between their right-hand [categories](category.md) commuting with both adjoints and respecting the specified units and counits. Strict identifications give a [category](category.md); coherent identifications give the analogous [universal property](#universal-property) up to compatible [natural isomorphism](category.md#natural-isomorphism).

### Algebra for a monad

↑ **Parent:** [Monad](#monad)

An algebra for a monad $(T,\eta,\mu)$ is an object $A$ with a morphism $a:TA\to A$ satisfying $a\eta_A=1_A$ and $aT(a)=a\mu_A$.

#### Reflexive free-algebra presentation of a monad algebra

↑ **Parent:** [Algebra for a monad](#algebra-for-a-monad)

Every [algebra for a monad](#algebra-for-a-monad) $(A,a)$ is the [coequalizer](category.md#coequalizer), in the [Eilenberg-Moore category](#eilenberg-moore-category), of $F(TA)\rightrightarrows F(A)$ with underlying arrows $\mu_A$ and $Ta$, followed by $a:F(A)\to(A,a)$. The pair has common section $F\eta_A$. If an algebra morphism $h:F(A)\to(B,b)$ equalizes the pair, the unique induced algebra morphism is $h\eta_A:(A,a)\to(B,b)$. This explicit proof does not require general colimits of algebras.

#### Unit law for a monad algebra

↑ **Parent:** [Algebra for a monad](#algebra-for-a-monad)

For an [algebra for a monad](#algebra-for-a-monad) $(X,a)$, its action $a:TX\to X$ satisfies $a\eta_X=1_X$.

#### Free algebra functor

↑ **Parent:** [Algebra for a monad](#algebra-for-a-monad)

For a [monad](#monad) $(T,\eta,\mu)$, the free algebra functor $F:\mathcal C\to\mathcal C^T$ sends $X$ to $(TX,\mu_X)$ and $f$ to $Tf$. It is a [left adjoint](category.md#adjoint-functors) to the forgetful [functor](category.md#functor) $U$, via $h\mapsto h\eta_X$ and $u\mapsto\gamma Tu$ between $\mathcal C^T(FX,(C,\gamma))$ and $\mathcal C(X,C)$.

#### Morphism of algebras for a monad

↑ **Parent:** [Algebra for a monad](#algebra-for-a-monad)

A morphism $f:(A,a)\to(B,b)$ of algebras for a monad satisfies $fa=bT(f)$. Such morphisms are the morphisms of the [Eilenberg-Moore category](#eilenberg-moore-category).

### Eilenberg-Moore category

↑ **Parent:** [Monad](#monad)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eilenberg-Moore_category)

The Eilenberg-Moore category $\mathcal C^T$ consists of algebras for a monad $T$ and their structure-preserving morphisms.

#### Monad algebra forgetful functor creates split coequalizers

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

For algebra maps $f,g:(A,a)\rightrightarrows(B,b)$ whose underlying maps have a [split coequalizer](category.md#split-coequalizer) $q:B\to Q$, every functor preserves the split diagram, including $T$ and $T^2$. Since $qb$ equalizes $Tf,Tg$, it factors uniquely to the displayed action $c:TQ\to Q$. Cancellation of the epimorphisms $q,Tq,T^2q$ proves the unit and multiplication laws. Any algebra-valued map equalizing the pair factors through $q$, and cancelling $Tq$ proves that its factor preserves the action. This establishes creation of that coequalizer.

#### Monad algebra forgetful functor creates limits

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

Given a diagram of [algebras for a monad](#algebra-for-a-monad), take any chosen limit $L$ of its underlying diagram. The displayed equations uniquely determine $a:TL\to L$, because their right-hand sides form a cone. Joint monicity of the limit projections proves $a\eta_L=1$ and $aT(a)=a\mu_L$. The same projection argument proves that every induced mediating map preserves the algebra action. Thus the forgetful functor strictly creates this limit with the prescribed underlying cone, without assuming the monad preserves limits.

#### Free-forgetful Eilenberg-Moore adjunction

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

For a [monad](#monad) $(T,\eta,\mu)$, the [free algebra functor](#free-algebra-functor) sends $X$ to $(TX,\mu_X)$ and is a [left adjoint](category.md#adjoint-functors) to the [forgetful functor](category.md#forgetful-functor) from the [Eilenberg-Moore category](#eilenberg-moore-category). The transpose [bijection](function.md#bijection) sends an [monad algebra morphism](#morphism-of-algebras-for-a-monad) $h:TX\to A$ to $h\eta_X$; its inverse sends $k:X\to A$ to $aT(k)$, where $a:TA\to A$ is the algebra structure. The [monad](#monad) and algebra laws make these inverse and natural. The [adjunction unit](category.md#unit-of-an-adjunction) is $\eta$ and the [adjunction counit](category.md#counit-of-an-adjunction) at $(A,a)$ is $a$, so the induced [monad](#monad) has exactly the original endofunctor, unit and multiplication.

#### Adjoint lifting theorem for monad algebra functors

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

For a functor between [Eilenberg-Moore categories](#eilenberg-moore-category) lying over a right adjoint on the base categories and compatible with the monad structures, an adjoint lifting theorem constructs a left adjoint when the required reflexive coequalizers of algebra presentations exist. Applied through [power-object monadicity](#power-object-monadicity), this converts a left adjoint of a [logical functor](#logical-functor) into a right adjoint of that logical functor. The coequalizer hypotheses are part of the theorem; commutation with the forgetful functors alone is insufficient.

#### Coproduct presentation for monad algebras

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

For [algebras for a monad](#algebra-for-a-monad) $(A,\alpha),(B,\beta)$ and underlying binary [coproducts in a category](category.md#coproduct), put $\kappa=[T\nu_1,T\nu_2]:TA+TB\to T(A+B)$. If the algebra pair $F(\alpha+\beta),\mu_{A+B}F\kappa:F(TA+TB)\rightrightarrows F(A+B)$ has a [coequalizer](category.md#coequalizer), that coequalizer is their algebra coproduct. An algebra map from $F(A+B)$ transposes to $[a,b]:A+B\to C$; equalizing the pair is exactly the two algebra-morphism equations for $a,b$. The pair is reflexive through $F(\eta_A+\eta_B)$.

##### Finite colimits of monad algebras from reflexive coequalizers

↑ **Parent:** [Coproduct presentation for monad algebras](#coproduct-presentation-for-monad-algebras)

If $\mathcal C$ has finite [colimits](category.md#colimit) and a [monad](#monad) $T$ preserves [reflexive coequalizers](#reflexive-coequalizer), its [Eilenberg-Moore category](#eilenberg-moore-category) has finite colimits. The forgetful [functor](category.md#functor) creates reflexive coequalizers preserved by $T$. The [coproduct presentation for monad algebras](#coproduct-presentation-for-monad-algebras) yields binary coproducts, and $F0$ is initial. Any pair $a,b:X\rightrightarrows Y$ can then be replaced by the [reflexive pair](#reflexive-pair) $[a,1],[b,1]:X+Y\rightrightarrows Y$, with identical coequalizers. Finite coproducts and coequalizers give all finite colimits.

#### Eilenberg-Moore comparison functor

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

For $F\dashv G:\mathcal D\to\mathcal C$ with induced monad $T=GF$, the Eilenberg-Moore comparison functor is

$$
K:\mathcal D\to\mathcal C^T,
\qquad K(D)=(GD,G\varepsilon_D).
$$

##### Full faithfulness from counit coequalizers

↑ **Parent:** [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor)

If each standard counit presentation is a [coequalizer](category.md#coequalizer), the [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor) is [full and faithful](category.md#full-and-faithful-functor). An [monad algebra morphism](#morphism-of-algebras-for-a-monad) $\alpha:GB\to GC$ makes $\varepsilon_CF\alpha$ equalize $FG\varepsilon_B$ and $\varepsilon_{FGB}$; its unique descent is the required [morphism](algebra.md#morphism) $B\to C$. The [triangle identities for an adjunction](category.md#triangle-identities-for-an-adjunction) make $G\varepsilon_B$ a [split epimorphism](category.md#split-epimorphism), so descent has underlying arrow exactly $\alpha$. Epimorphic cancellation at $\varepsilon_B$ proves faithfulness.

###### Full comparison and reflection of split coequalizers

↑ **Parent:** [Full faithfulness from counit coequalizers](#full-faithfulness-from-counit-coequalizers)

For an adjunction $F\dashv G$, applying $G$ to its standard counit presentation gives $T^2GD\rightrightarrows TGD\to GD$, split by the monad units. Reflection therefore makes every counit presentation a coequalizer and gives full faithfulness by descent. Conversely, [monad algebra forgetful functor creates split coequalizers](#monad-algebra-forgetful-functor-creates-split-coequalizers) makes an existing G-split quotient a coequalizer in the Eilenberg-Moore category. Fullness and faithfulness of the comparison lift its universal factorization back to the original category.

##### Terminality of the Eilenberg-Moore adjunction

↑ **Parent:** [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor)

The free-forgetful [adjunction](category.md#adjoint-functors) for the [Eilenberg-Moore category](#eilenberg-moore-category) is terminal in the [category of adjunctions inducing a fixed monad](#category-of-adjunctions-inducing-a-fixed-monad). The unique [morphism](algebra.md#morphism) into it is the [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor) $B\mapsto(GB,G\varepsilon_B)$. Its underlying objects and arrows are forced by the forgetful [functor](category.md#functor), and counit compatibility forces its algebra actions.

##### Left adjoint to the Eilenberg-Moore comparison functor

↑ **Parent:** [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor)

If $F\dashv G:\mathcal D\to\mathcal C$ induces $T=GF$ and $\mathcal D$ has coequalizers of reflexive pairs, then the comparison $K:\mathcal D\to\mathcal C^T$ has a left adjoint. On a $T$-algebra $(A,a)$ it is the coequalizer

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA\longrightarrow L(A,a).
$$

The pair is reflexive through $F\eta_A$, and its universal property gives $L\dashv K$.

###### Comparison-adjunction unit criterion

↑ **Parent:** [Left adjoint to the Eilenberg-Moore comparison functor](#left-adjoint-to-the-eilenberg-moore-comparison-functor)

For $F\dashv G$ inducing $T=GF$, the [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor) has a [left adjoint](category.md#adjoint-functors) exactly when every algebra $(A,a)$ has a [coequalizer](category.md#coequalizer) $q_a:FA\to L(A,a)$ of $Fa,\varepsilon_{FA}:FTA\rightrightarrows FA$. Transposition identifies maps equalizing this pair with [monad algebra morphisms](#morphism-of-algebras-for-a-monad) $(A,a)\to K(D)$, proving both directions of the criterion. The unit is $\lambda=Gq_a\eta_A$ and satisfies $Gq_a=\lambda a$. In the base category, $a:TA\to A$ is a [split coequalizer](category.md#split-coequalizer) of $Ta,\mu_A:T^2A\rightrightarrows TA$, split by $\eta_A$ and $\eta_{TA}$. Consequently $\lambda$ is invertible exactly when $Gq_a$ is also a coequalizer. The unit is invertible everywhere precisely when $G$ preserves all these specified coequalizers; preservation of arbitrary coequalizers is not required.

##### Monadic length

↑ **Parent:** [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor)

When each comparison functor has a left adjoint, iterating the [Eilenberg-Moore comparison functor](#eilenberg-moore-comparison-functor) produces the monadic tower. Its monadic length is the least number of comparison steps needed to reach an equivalence; an equivalence has length zero and a non-equivalence that is already monadic has length one.

###### Monadic tower for nested partial unary operations

↑ **Parent:** [Monadic length](#monadic-length)

For the [nested partial unary operation category](category.md#nested-partial-unary-operation-category) tower, each one-step forgetful [functor](category.md#functor) is a [monadic adjunction](#monadic-adjunction) right adjoint: it reflects [isomorphisms](algebra.md#isomorphism) and creates its split [coequalizers](category.md#coequalizer). The [Beck monadicity theorem](#beck-s-monadicity-theorem) identifies the first [Eilenberg-Moore category](#eilenberg-moore-category) with the next category in the tower. A long composite has that same first [monad](#monad) because [free extension of nested partial unary operations](category.md#free-extension-of-nested-partial-unary-operations) leaves no new top fixed points. Repeating the comparison forgets one fewer operation at each step. The remaining forgetful functor is not full until no operation remains to forget, giving [monadic length](#monadic-length) $m-n$.

#### Monadic adjunction

↑ **Parent:** [Eilenberg-Moore category](#eilenberg-moore-category)

An adjunction is monadic when its comparison functor from the right-hand category to the Eilenberg-Moore category of the induced monad is an equivalence.

The induced [monad](#monad) determines this comparison; [Beck's monadicity theorem](#beck-s-monadicity-theorem) gives a criterion for it to be an [equivalence of categories](category.md#equivalence-of-categories).

##### Crude monadicity theorem

↑ **Parent:** [Monadic adjunction](#monadic-adjunction)

A useful form of the crude monadicity theorem says that a right adjoint is monadic if it reflects isomorphisms and its source has and the functor preserves coequalizers of reflexive pairs.

##### Comonadic adjunction

↑ **Parent:** [Monadic adjunction](#monadic-adjunction)

An adjunction is comonadic when the comparison from its left-hand category to coalgebras for the induced comonad is an equivalence. The dual Beck theorem tests this using reflected isomorphisms and suitable equalizers.

The relevant criterion is the [Beck comonadicity theorem](#beck-comonadicity-theorem), dual to [Beck's monadicity theorem](#beck-s-monadicity-theorem).

###### Beck comonadicity theorem

↑ **Parent:** [Comonadic adjunction](#comonadic-adjunction)

The Beck comonadicity theorem, dual to the [Beck monadicity theorem](#beck-s-monadicity-theorem), says that a left adjoint is comonadic when it reflects isomorphisms and preserves the required equalizers of pairs whose images admit split equalizers. A stronger convenient hypothesis is that it preserves all equalizers.

<h5 id="beck-s-monadicity-theorem">Beck's monadicity theorem</h5>

↑ **Parent:** [Monadic adjunction](#monadic-adjunction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beck's_monadicity_theorem)

The precise monadicity theorem says that a right adjoint is monadic exactly when it reflects isomorphisms and creates coequalizers of the pairs whose images have split coequalizers.

### Monad on a left adjoint induces a comonad on its right adjoint

↑ **Parent:** [Monad](#monad)

If an endofunctor $F$ has a right adjoint $G$ and $(F,\eta,\mu)$ is a [monad](#monad), the [mate correspondence](category.md#mate-correspondence) turns $\eta:1\to F$ and $\mu:F^2\to F$ into a counit $G\to1$ and comultiplication $G\to G^2$. The reversed mate correspondence turns the monad laws into the comonad laws and identifies $F$-algebras with $G$-coalgebras.

### Kleisli category

↑ **Parent:** [Monad](#monad)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kleisli_category)

For a monad $(T,\eta,\mu)$ on $\mathcal C$, the Kleisli category $\mathcal C_T$ has the objects of $\mathcal C$ and morphisms

$$
\mathcal C_T(A,B)=\mathcal C(A,TB).
$$

Its identity on $A$ is $\eta_A$, and the composite of $f:A\to TB$ and $g:B\to TC$ is $\mu_C\,T(g)f:A\to TC$.

#### Initiality of the Kleisli adjunction

↑ **Parent:** [Kleisli category](#kleisli-category)

For a [monad](#monad) $(T,\eta,\mu)$, the free functor $J:\mathcal C\to\mathcal C_T$ and functor $U:\mathcal C_T\to\mathcal C$ with $UA=TA$ and $U(f)=\mu_B T(f)$ form an [adjunction](category.md#adjoint-functors) inducing that monad. Every other adjunction inducing the same monad receives the unique [Kleisli comparison functor](#kleisli-comparison-functor) commuting with its left and right adjoints and preserving the adjunction structure. This is initiality among adjunctions inducing the specified monad, with morphisms required to respect that structure.

#### Kleisli comparison functor

↑ **Parent:** [Kleisli category](#kleisli-category)

If $L\dashv R$ induces a [monad](#monad) $T=RL$, the comparison maps $A$ to $LA$ and maps a [Kleisli category](#kleisli-category) arrow $f:A\to TB$ to $\varepsilon_{LB}L(f)$. It is [full and faithful](category.md#full-and-faithful-functor), by the adjunction bijection $\mathcal D(LA,LB)\cong\mathcal C(A,TB)$. Consequently it is part of an [equivalence of categories](category.md#equivalence-of-categories) precisely when every object of $\mathcal D$ is isomorphic to some $LA$.

#### Free functor into a Kleisli category

↑ **Parent:** [Kleisli category](#kleisli-category)

The free functor $F_T:\mathcal C\to\mathcal C_T$ is the identity on objects and sends $f:A\to B$ to $\eta_Bf:A\to TB$. A functor $G:\mathcal C\to\mathcal D$ carries an algebra for the precomposition monad $G\mapsto GT$ exactly when it factors through $F_T$.

### Pointwise monad on a functor category

↑ **Parent:** [Monad](#monad)

For a monad $T$ on $\mathcal C$ and a category $\mathcal D$, postcomposition defines a monad $T_*:[\mathcal D,\mathcal C]\to[\mathcal D,\mathcal C]$ whose unit and multiplication are pointwise. Its Eilenberg-Moore category is canonically equivalent to $[\mathcal D,\mathcal C^T]$.

### Precomposition monad on a functor category

↑ **Parent:** [Monad](#monad)

Precomposition defines a monad $T^*:[\mathcal C,\mathcal D]\to[\mathcal C,\mathcal D]$ by $G\mapsto GT$, with unit $G\eta$ and multiplication $G\mu$. Its Eilenberg-Moore category is canonically equivalent to $[\mathcal C_T,\mathcal D]$.

## Lawvere theory

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lawvere_theory)

A Lawvere theory is a small category with finite products generated by one object: every object is a finite power $[n]=[1]^n$. A model in a finite-product category is a finite-product-preserving functor from the theory.

## Finitary monad

↑ **Parent:** [Category theory](category-theory.md)

A monad on sets is finitary when its underlying functor preserves filtered colimits. Its operations on finite free algebras form a Lawvere theory.

## Complete Heyting algebra

↑ **Parent:** [Category theory](category-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_Heyting_algebra)

A frame is a complete lattice in which finite meets distribute over arbitrary joins:

$$
a\wedge\bigvee S=\bigvee_{s\in S}(a\wedge s).
$$

### Subframe

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A subframe is a subset of a [frame](#complete-heyting-algebra) closed under arbitrary ambient joins and finite ambient meets, including $0$ and $1$. The inclusion is a [frame homomorphism](#frame-homomorphism). In contrast, the fixed elements of a [nucleus on a frame](#nucleus-on-a-frame) usually need their own regularized joins and are not a subframe.

### Completely prime filter

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

An upward-closed subset of a [frame](#complete-heyting-algebra) containing $1$, excluding $0$ and closed under finite meets is completely prime if membership of an arbitrary join implies membership of some summand. Its characteristic map is a [point of a frame](#point-of-a-frame). Constructively the map takes values in the [frame](#complete-heyting-algebra) of truth values.

### Preframe

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A preframe is a [partially ordered set](set.md#partially-ordered-set) with finite meets and nonempty directed joins, with finite meets distributing over directed joins. Its homomorphisms preserve these operations. Forgetting the arbitrary joins of a [frame](#complete-heyting-algebra) leaves a preframe.

#### Preframe tensor product

↑ **Parent:** [Preframe](#preframe)

The tensor represents maps $P\times Q\to R$ preserving finite meets and directed joins in each variable separately. Its pure generators $p\#q$ satisfy the corresponding relations in each variable. The unit is the free [preframe](#preframe) on one generator, the bottom of the [frame](#complete-heyting-algebra) of truth values. For [frames](#complete-heyting-algebra), this tensor is their [coproduct](category.md#coproduct), with $p\#q=i(p)\vee j(q)$; it must not be confused with the rectangle $i(p)\wedge j(q)$.

##### Frame coreflection of a preframe monoid

↑ **Parent:** [Preframe tensor product](#preframe-tensor-product)

For a commutative [monoid object](#monoid-object) $(M,*,e)$ in [preframes](#preframe), the indicated subset is a [frame](#complete-heyting-algebra). Its bottom is $e$, its binary join is $*$, and its directed joins and finite meets are inherited. Every homomorphism from a [frame](#complete-heyting-algebra) regarded as a join monoid factors uniquely through this subset. This gives a [coreflective subcategory](category.md#coreflective-subcategory).

### Nucleus on a frame

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A nucleus is an inflationary, idempotent, finite-meet-preserving map on a [frame](#complete-heyting-algebra). Its fixed elements form a [frame](#complete-heyting-algebra), whose joins are obtained by applying $j$ to ambient joins. The induced [locale](#locale) is a [sublocale](#sublocale). The [nuclei on a frame](#nucleus-on-a-frame) themselves form a [frame](#complete-heyting-algebra) in pointwise order; their meets are pointwise, but their joins usually are not.

#### Relative nucleus assembly

↑ **Parent:** [Nucleus on a frame](#nucleus-on-a-frame)

For a [frame homomorphism](#frame-homomorphism) $h:B\to A$, nuclei are equivalent when their restrictions to $h(B)$ agree. The least representative of the class of $j$ is

$$
r_h(j)=\bigvee_{b\in B}\bigl(o(hb)\wedge c(j(hb))\bigr).
$$

The least representatives form a [frame](#complete-heyting-algebra) generated by $c(A)$ and $o(h(B))$. To see minimality, each summand is below $j$ and its value at $hb$ is $j(hb)$; any equivalent nucleus therefore bounds every summand. This construction gives the [pushout](category.md#pushout) of $B\to N(B)$ along $h$.

#### Closed nucleus

↑ **Parent:** [Nucleus on a frame](#nucleus-on-a-frame)

This [nucleus on a frame](#nucleus-on-a-frame) determines the [closed sublocale](#closed-sublocale) complementary to the open determined by $a$. It is the least [nucleus on a frame](#nucleus-on-a-frame) taking $0$ to $a$. In the [frame](#complete-heyting-algebra) of [nuclei on a frame](#nucleus-on-a-frame), $c(a)$ and the [open nucleus](#open-nucleus) $o(a)$ are complements.

#### Open nucleus

↑ **Parent:** [Nucleus on a frame](#nucleus-on-a-frame)

The [Heyting implication](mathematical-logic.md#heyting-implication) defines a [nucleus on a frame](#nucleus-on-a-frame) whose [sublocale](#sublocale) is the open determined by $a$. It is the least [nucleus on a frame](#nucleus-on-a-frame) sending $a$ to $1$.

### Locale

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A locale is an object of the opposite of the [category](category.md) of [frames](#complete-heyting-algebra). A map $f:X\to Y$ is specified by a [frame homomorphism](#frame-homomorphism) $f^*:\mathcal O(Y)\to\mathcal O(X)$. This makes open-set algebra primary and allows spaces without enough ordinary points. A [point of a frame](#point-of-a-frame) is the inverse-image map of a point of a locale.

#### Connected locale

↑ **Parent:** [Locale](#locale)

Under classical logic a positive [locale](#locale) is connected when it cannot be written as the union of two disjoint nonzero opens. Equivalently its only complemented opens are $0$ and $1$. An open sublocale uses this criterion relative to its own top element. Positivity of the whole locale excludes the empty locale. This definition is stated with its logical convention; replacing positivity by negated nonemptiness is not a constructive step.

#### Well-inside relation

↑ **Parent:** [Locale](#locale)

This relation says that the closure of the open $u$ is contained in $v$. A [regular locale](#regular-locale) has $a=\bigvee_{u\prec a}u$ for every $a$. If $u\prec a$, then $\neg\neg u\leq a$ and $\neg\neg u\prec a$.

##### Regular locale

↑ **Parent:** [Well-inside relation](#well-inside-relation)

A [locale](#locale) is regular when every open is the join of opens [well inside](#well-inside-relation) it. This expresses regularity without reference to points.

#### Extremally disconnected locale

↑ **Parent:** [Locale](#locale)

A [locale](#locale) is extremally disconnected when the closure of every open is open. Equivalently its [regular open elements](mathematical-logic.md#regular-element-of-a-heyting-algebra) are complemented, or double negation preserves binary joins, or its [Booleanization of a locale](#booleanization-of-a-locale) is a [flat sublocale](#flat-sublocale).

##### Gleason cover of a compact regular locale

↑ **Parent:** [Extremally disconnected locale](#extremally-disconnected-locale)

For a compact [regular locale](#regular-locale) $X$, put $B=\mathcal O(X)_{\neg\neg}$ and $\mathcal O(\gamma X)=\operatorname{Idl}(B)$. This [locale](#locale) is extremally disconnected. Its natural surjection to $X$ has inverse image

$$
a\longmapsto\bigvee_{u\prec a}\mathord\downarrow(\neg\neg u).
$$

The [Joyal extension lemma](#joyal-extension-lemma) gives the [frame homomorphism](#frame-homomorphism); its injectivity follows by recovering $a$ as the join of the regular opens in this ideal.

#### Open locale

↑ **Parent:** [Locale](#locale)

An open, or overt, [locale](#locale) has a positivity map $\operatorname{Pos}:\mathcal O(X)\to\Omega$ left adjoint to the scalar inverse image $!^*:\Omega\to\mathcal O(X)$, satisfying Frobenius reciprocity. Thus $a\leq !^*\operatorname{Pos}(a)$ and positivity preserves arbitrary joins. Classically every locale is overt, with positivity meaning $a\ne0$.

##### Totally connected locale

↑ **Parent:** [Open locale](#open-locale)

A positive [open locale](#open-locale) is totally connected when every [positive open of a locale](#positive-open-of-a-locale) is connected. Under classical logic its positive opens form a [completely prime filter](#completely-prime-filter), hence specify a dense point. Positivity of the whole locale is essential: the empty locale satisfies the condition on positive opens vacuously but has no point.

##### Positive open of a locale

↑ **Parent:** [Open locale](#open-locale)

An open is positive when its positivity truth value holds. Positivity gives a constructive witness of inhabitedness and must not be replaced by double-negated nonemptiness.

#### Totally unordered locale

↑ **Parent:** [Locale](#locale)

A [locale](#locale) is totally unordered when $f^*\leq g^*$ for two maps into it implies $f=g$, for every common domain. This tests generalized points rather than just ordinary points. Every [Hausdorff locale](#hausdorff-locale) has this property: comparable maps annihilate the complement of the diagonal and hence factor through the diagonal.

#### Hausdorff locale

↑ **Parent:** [Locale](#locale)

A [locale](#locale) is Hausdorff when its diagonal into its localic square is a [closed sublocale](#closed-sublocale). Its complement is the join of rectangles $a\times b$ with $a\wedge b=0$. This is stronger than the underlying space being a [Hausdorff space](topology.md#hausdorff-space), because the localic square need not be spatial.

#### Compact locale

↑ **Parent:** [Locale](#locale)

A [locale](#locale) is compact when every directed family of opens whose join is $1$ contains $1$. Equivalently every open cover has a finite subcover. The truth-valued test $a\mapsto[a=1]$ is a [preframe](#preframe) homomorphism exactly when the locale is compact.

##### Localic Tychonoff theorem

↑ **Parent:** [Compact locale](#compact-locale)

An arbitrary product of [compact locales](#compact-locale) is compact. Finite products correspond to [preframe tensor products](#preframe-tensor-product), whose compactness follows by tensoring the top tests. An arbitrary product is obtained by the filtered colimit of finite [frame](#complete-heyting-algebra) coproducts; the eventual-top test proves that filtered colimits preserve compactness. No choice of points is required.

#### Sublocale

↑ **Parent:** [Locale](#locale)

A sublocale is determined by a [nucleus on a frame](#nucleus-on-a-frame) $j$ on $\mathcal O(X)$. Its [frame](#complete-heyting-algebra) consists of the fixed elements of $j$, with inherited meets and regularized joins. Increasing the nucleus makes the sublocale smaller.

##### Booleanization of a locale

↑ **Parent:** [Sublocale](#sublocale)

The double-negation [nucleus on a frame](#nucleus-on-a-frame) gives a [dense sublocale](#dense-sublocale) whose [frame](#complete-heyting-algebra) is a [complete Boolean algebra](mathematical-logic.md#complete-boolean-algebra). Its elements are [regular open elements](mathematical-logic.md#regular-element-of-a-heyting-algebra), with Boolean joins $\neg\neg\bigvee_i a_i$.

##### Flat sublocale

↑ **Parent:** [Sublocale](#sublocale)

A [sublocale](#sublocale) is flat when its [nucleus on a frame](#nucleus-on-a-frame) preserves finite joins, including $0$. Equivalently its fixed elements are closed under ambient finite joins. In particular every flat sublocale is a [dense sublocale](#dense-sublocale).

###### Joyal extension lemma

↑ **Parent:** [Flat sublocale](#flat-sublocale)

Every map from a [flat sublocale](#flat-sublocale) $A_j$ of $A$ to a [compact locale](#compact-locale) that is also a [regular locale](#regular-locale) extends uniquely to $A$. On [frames](#complete-heyting-algebra) the extension is

$$
g^*(a)=\bigvee_{u\prec a}^{\mathcal O(A)}f^*(u),
$$

where the terms are first regarded as fixed elements in the ambient frame. Regularity proves agreement after applying $j$; compactness reduces arbitrary covers to finite subcovers on a well-inside open, and flatness identifies those finite joins with ambient joins. These facts prove that $g^*$ preserves arbitrary joins and finite meets.

##### Dense sublocale

↑ **Parent:** [Sublocale](#sublocale)

A [sublocale](#sublocale) is dense when its closure is the whole [locale](#locale). For a map $f$, its image is dense when $f^*(a)=0$ implies $a=0$. Classically, a dense point belongs to every nonzero open.

##### Closed sublocale

↑ **Parent:** [Sublocale](#sublocale)

The [closed nucleus](#closed-nucleus) $c(a)$ determines the complement of the open $a$. A [sublocale](#sublocale) with nucleus $j$ is dense precisely when $j(0)=0$, since its closure is the [closed sublocale](#closed-sublocale) defined by $j(0)$.

### Frame-point adjunction

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

There is a natural [bijection](function.md#bijection) between [continuous maps](topology.md#continuous-map) $X\to P(A)$ and [frame homomorphisms](#frame-homomorphism) $A\to O(X)$. It sends $f$ to $a\mapsto f^{-1}(U_a)$; the inverse sends $x$ to the point $a\mapsto1_{\{x\in h(a)\}}$. Its [adjunction unit](category.md#unit-of-an-adjunction) sends a point of $X$ to its open-neighbourhood membership map. The counit is represented by $a\mapsto U_a$. Every open of $P(A)$ is such a $U_a$, and every [point of a frame](#point-of-a-frame) $O(P(A))$ is uniquely evaluation at a point of $A$. Consequently $P(A)\to P(O(P(A)))$ is a [homeomorphism](topology.md#homeomorphism), and this is an [idempotent adjunction](category.md#idempotent-adjunction).

### Open-set frame

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

The [open subsets](topology.md#open-set) of a [topological space](topology.md#topological-space) form a [frame](#complete-heyting-algebra). Arbitrary joins are unions, finite meets are intersections, and an arbitrary meet is the interior of an intersection. A [continuous map](topology.md#continuous-map) induces a [frame homomorphism](#frame-homomorphism) in the opposite direction by inverse image.

### Point of a frame

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A point is a [frame homomorphism](#frame-homomorphism) to the two-element [frame](#complete-heyting-algebra) $\mathbf 2=\{0<1\}$. Its inverse image of $1$ is a completely prime filter: membership of an arbitrary join forces membership of one term. The point space $P(A)$ has opens $U_a=\{p:p(a)=1\}$. Indeed $U_{a\wedge b}=U_a\cap U_b$ and $U_{\bigvee_i a_i}=\bigcup_iU_{a_i}$, so these sets already form a [topology](topology.md).

### Frame homomorphism

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

A map between [frames](#complete-heyting-algebra) preserving every [join](set.md#least-upper-bound-in-a-partially-ordered-set) and every finite [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set), including the empty join $0$ and empty meet $1$. Such a map is automatically order-preserving. Inverse image under a [continuous map](topology.md#continuous-map) is an example.

### Category of matrices valued in a frame

↑ **Parent:** [Complete Heyting algebra](#complete-heyting-algebra)

For a [frame](#complete-heyting-algebra) $L$, an $L$-valued matrix $f:A\rightsquigarrow B$ is a function $A\times B\to L$. Composition is matrix multiplication with join as addition and meet as multiplication.

## Reflexive pair

↑ **Parent:** [Category theory](category-theory.md)

A reflexive pair is a pair $f,g:A\rightrightarrows B$ with a common splitting $r:B\to A$, so $fr=gr=1_B$.

### Reflexive coequalizer

↑ **Parent:** [Reflexive pair](#reflexive-pair)

A reflexive coequalizer is a [coequalizer](category.md#coequalizer) of a [reflexive pair](#reflexive-pair), meaning a parallel pair $r,s:X\rightrightarrows Y$ with a common section $t:Y\to X$ satisfying $rt=st=1_Y$. A [functor](category.md#functor) preserves reflexive coequalizers when it takes every such coequalizer to a coequalizer of the image pair.

### Coequalizer of a reflexive pair from a pushout

↑ **Parent:** [Reflexive pair](#reflexive-pair)

For a [reflexive pair](#reflexive-pair) $f,g:A\rightrightarrows B$ with common section $r$, form the [pushout in a category](category.md#pushout-in-a-category) of $f$ and $g$, with maps $j_1,j_2:B\to P$. The equation $j_1f=j_2g$, composed with $r$, gives $j_1=j_2=q$. This common map is a [coequalizer](category.md#coequalizer) of $f,g$: every map equalizing them defines a commuting pair into the pushout and hence factors uniquely through $q$.

### Internal groupoid

↑ **Parent:** [Reflexive pair](#reflexive-pair)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Internal_groupoid)

An internal groupoid in a category is a groupoid object: its objects, arrows, source, target, identity, composition, and inversion are objects and morphisms in the ambient category and satisfy the groupoid identities diagrammatically.

#### Reflexive-pair groupoid formula in a preadditive category

↑ **Parent:** [Internal groupoid](#internal-groupoid)

For a [reflexive pair](#reflexive-pair) $f,g:A\rightrightarrows B$ with section $r$ in a [preadditive category](category.md#preadditive-category), each hom-set diagram defines a [groupoid](category.md#groupoid). Arrows $a,b:C\to A$ compose when $ga=fb$, by $b\circ a=a+b-rga$. Identity at $x:C\to B$ is $rx$, and the inverse of $a$ is $rfa+rga-a$. Bilinearity proves the endpoint, identity and associativity laws and compatibility with precomposition in $C$. In the hom-set formulation this does not assume that the composable-arrow pullback exists.

#### Reflexive pair in an additive category is an internal groupoid

↑ **Parent:** [Internal groupoid](#internal-groupoid)

If $f,g:A\rightrightarrows B$ have common splitting $r$ in an [additive category](#additive-category), define the composite of $x,y:C\to A$ with $gx=fy$ by

$$
x\circledast y=x+y-rgx.
$$

The identity at $b:C\to B$ is $rb$, and the inverse of $x$ is $rfx+rgx-x$. These formulas make the reflexive pair an [internal groupoid](#internal-groupoid).

## Elementary topos

↑ **Parent:** [Category theory](category-theory.md)

An elementary topos is a category with finite limits, a [cartesian-closed](category.md#cartesian-closed-category) structure, and a [subobject classifier](#subobject-classifier). These axioms support an internal intuitionistic higher-order logic.

### Two-valued topos

↑ **Parent:** [Elementary topos](#elementary-topos)

A nondegenerate [elementary topos](#elementary-topos) is two-valued when its [terminal object](category.md#terminal-object) has exactly the empty and whole subobjects. This is a global-truth property, distinct from being a [Boolean topos](#boolean-topos), which requires complements for all subobjects of all objects.

### Irreducible object in a topos

↑ **Parent:** [Elementary topos](#elementary-topos)

A noninitial object is irreducible, or supercompact, when every family of subobjects with union the whole object contains the whole object as one member. This concerns unions of subobjects rather than disjoint coproduct decompositions. [Irreducible representable sheaves for the regular coverage](category.md#irreducible-representable-sheaf-for-the-regular-coverage) follow from the one-arrow nature of that coverage.

### Boolean topos

↑ **Parent:** [Elementary topos](#elementary-topos)

A Boolean topos is an elementary topos in which every subobject has a complement, equivalently its internal truth-value [Heyting algebra](mathematical-logic.md#heyting-algebra) satisfies excluded middle. Its internal first-order logic is classical. Being Boolean alone does not imply that it has enough set-valued points.

### Logical functor

↑ **Parent:** [Elementary topos](#elementary-topos)

A logical functor between elementary toposes preserves [finite limits](category.md#finite-limit), [exponential objects](category.md#exponential-object) and the [subobject classifier](#subobject-classifier), with their canonical comparison maps. It therefore preserves [power objects](#power-object) and the double-power-object monad. If it has a left adjoint, [power-object monadicity](#power-object-monadicity) and the [adjoint lifting theorem for monad algebra functors](#adjoint-lifting-theorem-for-monad-algebra-functors) give it a right adjoint as well.

### Power object

↑ **Parent:** [Elementary topos](#elementary-topos)

A power object $PA$ represents parameterized [subobjects](category.md#subobject) of $A$: $\mathcal E(X,PA)\cong\operatorname{Sub}(X\times A)$. In an [elementary topos](#elementary-topos), it is $\Omega^A$, with the membership subobject supplied by evaluation at the [subobject classifier](#subobject-classifier).

#### Power objects in a slice category

↑ **Parent:** [Power object](#power-object)

If a [Cartesian category](category.md#cartesian-category) has [power objects](#power-object), its [slice categories](category.md#slice-category) do too. In $\mathcal E/A$, the constant family $A\times X\to A$ has power object $A\times PX\to A$, since its product with a family $Y\to A$ is $X\times Y$. An arbitrary family $p:X\to A$ is a subobject of the constant family through its graph $(p,1_X)$, so the [power object of a subobject](#power-object-of-a-subobject) construction applies in the slice.

#### Power object of a subobject

↑ **Parent:** [Power object](#power-object)

For a [monomorphism](category.md#monomorphism) $Y\hookrightarrow X$ in a [Cartesian category](category.md#cartesian-category), intersect the universal membership relation on $X\times PX$ with $Y\times PX$. The resulting [subobject](category.md#subobject) is classified by $r:PX\to PX$, and $r^2=r$. The [equalizer](category.md#equaliser) of $r$ and the identity represents precisely families of subobjects of $X$ contained in $Y$, hence is a [power object](#power-object) for $Y$. This construction only requires the power object of $X$ and finite limits.

#### Contravariant power-object functor

↑ **Parent:** [Power object](#power-object)

An arrow $f:A\to B$ induces $Pf:PB\to PA$ by inverse image of predicates. Transposition of predicates on $A\times B$ gives $\mathcal E(A,PB)\cong\mathcal E(B,PA)$ and the adjunction $P^{\mathrm{op}}\dashv P$. The induced monad on the topos is double power-object formation; it is distinct from the covariant powerset monad on sets.

##### Power-object monadicity

↑ **Parent:** [Contravariant power-object functor](#contravariant-power-object-functor)

The [contravariant power-object functor](#contravariant-power-object-functor) of an [elementary topos](#elementary-topos) is monadic. Its double-power unit $\eta_A(a)(S)=(a\in S)$ is monic, which helps prove that $P$ reflects isomorphisms. Finite equalizers and the fact that [power objects turn coreflexive equalizers into coequalizers](#power-objects-turn-coreflexive-equalizers-into-coequalizers) give the remaining hypotheses of the [crude monadicity theorem](#crude-monadicity-theorem).

###### Products and coproducts of fixed cardinality in a topos

↑ **Parent:** [Power-object monadicity](#power-object-monadicity)

For an [elementary topos](#elementary-topos), existence of [products in a category](category.md#product-category-theory) indexed by a fixed set is equivalent to existence of the corresponding [coproducts in a category](category.md#coproduct). The [power-object monadicity](#power-object-monadicity) equivalence $\mathcal E^{\mathrm{op}}\simeq\mathcal E^{PP}$ gives the forward direction because [Eilenberg-Moore categories](#eilenberg-moore-category) create limits. For the converse, the diagonal into the pointwise product category is a [logical functor](#logical-functor). A coproduct is its [left adjoint](category.md#adjoint-functors); the [adjoint lifting theorem for monad algebra functors](#adjoint-lifting-theorem-for-monad-algebra-functors), applied through power-object monadicity, then gives its [right adjoint](category.md#adjoint-functors), namely the product. The required reflexive coequalizers on the algebra side are opposites of finite equalizers in the topos.

##### Power objects turn coreflexive equalizers into coequalizers

↑ **Parent:** [Contravariant power-object functor](#contravariant-power-object-functor)

For a [coreflexive pair](#coreflexive-pair) $f,g:B\rightrightarrows A$ with equalizer $e:E\hookrightarrow B$, direct image along the mono $f$ satisfies $Pf\,\exists_f=1$ and $Pg\,\exists_f=\exists_e Pe$. Thus any map $h:PB\to Z$ equalizing $Pf,Pg$ obeys $h=h\exists_e Pe$. Since $Pe\exists_e=1$, the map $Pe$ is their [coequalizer](category.md#coequalizer). These identities hold for parameterized subobjects in any [elementary topos](#elementary-topos).

### Atom in a topos

↑ **Parent:** [Elementary topos](#elementary-topos)

An atom is a noninitial object with only the empty and whole subobject. In the [atomic finite-surjection site](category.md#atomic-finite-surjection-site), the sheaf component generated by one primitive class is an atom: membership of one descendant in a subobject descends to its primitive ancestor and then propagates to all descendants. A decomposition into atoms makes subobjects selections of components.

### Global sections functor

↑ **Parent:** [Elementary topos](#elementary-topos)

Global sections are the maps from the terminal object: $\Gamma(X)=\operatorname{Hom}(1,X)$. For a [Grothendieck topos](#grothendieck-topos), this is the direct image of its geometric morphism to sets. In a [presheaf category](category.md#presheaf-category), it is right adjoint to the constant-presheaf functor.

### Geometric morphism

↑ **Parent:** [Elementary topos](#elementary-topos)

A geometric morphism $f:\mathcal E\to\mathcal F$ is an [adjunction](category.md#adjoint-functors) $f^*\dashv f_*$ with finite-limit-preserving inverse image $f^*:\mathcal F\to\mathcal E$. Inverse image also preserves colimits as a left adjoint. An extra left adjoint $f_!\dashv f^*$ makes it essential.

#### Hyperconnected-localic factorization

↑ **Parent:** [Geometric morphism](#geometric-morphism)

For a [geometric morphism](#geometric-morphism) $f:\mathcal E\to\mathcal F$, the displayed internal [frame](#complete-heyting-algebra) represents $X\mapsto\operatorname{Sub}_{\mathcal E}(f^*X)$. The localic part is $\operatorname{Sh}_{\mathcal F}(L)\to\mathcal F$. Its basic open families pull back to the subobjects of $f^*X$ they represent; gluing these gives a full faithful, subobject-closed inverse image, hence the [hyperconnected geometric morphism](#hyperconnected-geometric-morphism) part. The represented subobject functor recovers the internal frame, proving uniqueness up to equivalence over $\mathcal F$.

#### Hyperconnected geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A [geometric morphism](#geometric-morphism) $h$ is hyperconnected when its [inverse image functor of a geometric morphism](#inverse-image-functor-of-a-geometric-morphism) is [full and faithful](category.md#full-and-faithful-functor) and its essential image is closed under [subobjects](category.md#subobject). It then identifies all subobjects of $h^*X$ with subobjects of $X$, and its image is closed under quotients as well, by descending the kernel-pair relation.

#### Localic geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A [geometric morphism](#geometric-morphism) $p:\mathcal D\to\mathcal F$ is localic when $\mathcal D$ is, over $\mathcal F$, the topos of sheaves on an internal [locale](#locale) of $\mathcal F$. Equivalently, subobjects of the objects $p^*X$, with $X\in\mathcal F$, form a separating family in $\mathcal D$.

#### Diaconescu equivalence for geometric morphisms

↑ **Parent:** [Geometric morphism](#geometric-morphism)

[Geometric morphisms](#geometric-morphism) into a sheaf topos correspond to continuous [flat functors](category.md#flat-functor) from its [site](category.md#site-category-theory) into the domain topos, with continuity meaning that covers become jointly epimorphic families. Pulling back sheafified representables gives the [functor](category.md#functor); the tensor construction gives the inverse image in the other direction. This representation theorem should not be confused with the separately named Diaconescu theorem about choice and excluded middle.

#### Global sections geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

Every [Grothendieck topos](#grothendieck-topos) has a unique [geometric morphism](#geometric-morphism) to sets, up to isomorphism. Its inverse image is $\Delta S=\coprod_{s\in S}1$ and its direct image is $\Gamma A=\operatorname{Hom}(1,A)$. A geometric inverse image out of sets must have this form because it preserves [coproducts](category.md#coproduct) and the [terminal object](category.md#terminal-object). A [local topos](#local-topos) is one for which $\Gamma$ itself is an inverse image.

#### Inverse image functor of a geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

The inverse image is a finite-limit-preserving [left adjoint](category.md#adjoint-functors) with [right adjoint](category.md#adjoint-functors) $f_*$. It preserves arbitrary [colimits](category.md#colimit), and hence images as well as [finite limits](category.md#finite-limit). These properties preserve the interpretation of [geometric formulas](mathematical-logic.md#geometric-formula). It need not preserve Heyting implication or every universal quantifier.

#### Essential geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A [geometric morphism](#geometric-morphism) is essential when its inverse image has an additional [left adjoint](category.md#adjoint-functors). For a [functor](category.md#functor) of small categories, precomposition on presheaves has [left Kan extension](category.md#left-kan-extension) and [Right Kan extension](category.md#right-kan-extension) as its two adjoints. Precomposition preserves [finite limits](category.md#finite-limit) pointwise, so this is an essential [geometric morphism](#geometric-morphism).

#### Surjection-embedding factorization of a geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

For $f:\mathcal E\to\mathcal F$, the comonad $G=f^*f_*$ is Cartesian, and its coalgebra topos $\mathcal D$ gives a factorization $f=i\circ p$. Here $p^*$ is the faithful forgetful functor and $i^*$ is the comparison functor. Its right adjoint sends $(A,a)$ to $\operatorname{Eq}(f_*a,\eta_{f_*A})$; applying $f^*$ identifies the comparison counit with the equalizer $a:A\to GA$ of $Ga,\delta_A$, proving that $i_*$ is full and faithful.

#### Geometric embedding

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A geometric embedding is a [geometric morphism](#geometric-morphism) whose direct-image functor is [full and faithful](category.md#full-and-faithful-functor). Its inverse image presents a left-exact reflective subcategory of the target topos. It is the second part of the [surjection-embedding factorization of a geometric morphism](#surjection-embedding-factorization-of-a-geometric-morphism).

##### Subtopos

↑ **Parent:** [Geometric embedding](#geometric-embedding)

A [subtopos](#subtopos) is a [Grothendieck topos](#grothendieck-topos) embedded by a [geometric embedding](#geometric-embedding), considered up to equivalence over the ambient topos. On a [site](category.md#site-category-theory) $(\mathcal C,J)$, [subtoposes](#subtopos) correspond to Grothendieck topologies $J'\supseteq J$. On a [classifying topos](#classifying-topos) this is the [duality between geometric quotients and subtoposes](#duality-between-geometric-quotients-and-subtoposes).

#### Surjective geometric morphism

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A geometric morphism is surjective when its inverse-image functor is faithful, equivalently conservative for geometric inverse images. Reflection of isomorphisms of subobjects already proves faithfulness by applying the inverse image to equalizers of parallel arrows. The [surjection-embedding factorization of a geometric morphism](#surjection-embedding-factorization-of-a-geometric-morphism) separates this property from a fully faithful direct image.

##### Surjectivity detected by the subobject classifier

↑ **Parent:** [Surjective geometric morphism](#surjective-geometric-morphism)

For a [geometric morphism](#geometric-morphism), the characteristic map of $f^*\top$ induces a comparison $f^*\Omega_{\mathcal E}\to\Omega_{\mathcal F}$ whose adjoint transpose is $\lambda$. Composing with a characteristic map classifies the inverse-image subobject. Thus monicity of $\lambda$ is equivalent to reflection of equality of subobjects under $f^*$, and hence to faithfulness of the inverse image: apply reflection to equalizers of parallel arrows. Conversely faithfulness reflects when a pulled-back monomorphism is an isomorphism, by comparing its characteristic map with truth; intersections then reflect equality of arbitrary subobjects.

#### Local topos

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A topos over sets is local when its [global sections functor](#global-sections-functor) is itself an inverse image functor. For an idempotent-complete small indexing category, its [presheaf topos](category.md#presheaf-topos) is local exactly when the indexing category has a terminal object: then global sections are evaluation at that object.

##### Open cover criterion for a local sheaf topos

↑ **Parent:** [Local topos](#local-topos)

Equivalently every open cover of $X$ contains $X$ as a member, so the top element of its open-set lattice is supercompact in the frame sense. Necessity follows from preservation of [coproducts](category.md#coproduct) and [epimorphisms](category.md#epimorphism) by global sections. Conversely the union of all proper opens misses a point $x$, and the [stalk functor](ringed-space.md#stalk-functor-for-presheaves-of-sets) there equals global sections. Its [right adjoint](category.md#adjoint-functors) is a [skyscraper sheaf of sets](algebraic-geometry.md#skyscraper-sheaf-of-sets). Empty spaces fail; a T1 space satisfies the condition exactly when it is a singleton.

##### Initial object criterion for a covariant local topos

↑ **Parent:** [Local topos](#local-topos)

The constant singleton [functor](category.md#functor) must be a [retract in a category](category.md#retract-in-a-category) of a covariant [representable functor](category.md#representable-functor). Necessity follows by applying a colimit-preserving global-sections [functor](category.md#functor) to the canonical [coproduct](category.md#coproduct) of representables onto the terminal [functor](category.md#functor). Conversely its Hom [functor](category.md#functor) is a retract of evaluation, preserves [colimits](category.md#colimit) and has a [right adjoint](category.md#adjoint-functors). Such a retract is represented by an [initial object](category.md#initial-object) in the [idempotent completion](category.md#karoubi-envelope). For an idempotent-complete category an actual [initial object](category.md#initial-object) suffices; without this hypothesis an absorbing-zero [monoid](algebra.md#monoid) gives a counterexample to the unqualified claim.

#### Geometric morphism induced by a functor

↑ **Parent:** [Geometric morphism](#geometric-morphism)

A functor $F:\mathcal C\to\mathcal D$ induces a [geometric morphism](#geometric-morphism) from the presheaf topos on $\mathcal C$ to that on $\mathcal D$. Its inverse image is precomposition with $F^{\mathrm{op}}$, its direct image is [Right Kan extension](category.md#right-kan-extension) and its extra left adjoint is [left Kan extension](category.md#left-kan-extension). The extra left adjoint sends $yC$ to $y(FC)$.

##### Full-faithfulness criterion for presheaf geometric embeddings

↑ **Parent:** [Geometric morphism induced by a functor](#geometric-morphism-induced-by-a-functor)

The [geometric morphism](#geometric-morphism) induced by $T:\mathcal C\to\mathcal D$ is a [geometric embedding](#geometric-embedding) exactly when $T$ is [full and faithful](category.md#full-and-faithful-functor). Its right adjoint has $(f_*H)(d)=\operatorname{Nat}(\mathcal D(T-,d),H)$. The counit at $c$ is precomposition with $\mathcal C(-,c)\to\mathcal D(T-,Tc)$. It is invertible for all $H$ precisely when that comparison presheaf is an isomorphism, by the [Yoneda lemma](category.md#yoneda-lemma), which is precisely full faithfulness of $T$.

##### Retract criterion for surjective presheaf geometric morphisms

↑ **Parent:** [Geometric morphism induced by a functor](#geometric-morphism-induced-by-a-functor)

For a [functor](category.md#functor) $T:\mathcal C\to\mathcal D$, restriction of [presheaves](algebraic-geometry.md#presheaf-of-sets-on-a-topological-space) is faithful exactly when every $d$ is a [retract in a category](category.md#retract-in-a-category) of some $Tc$. Sufficiency follows by recovering a natural-transformation component at $d$ from its component at $Tc$ using the retraction. For necessity, the subpresheaf of $\mathcal D(-,d)$ consisting of arrows factoring through some $Tc$ becomes the whole representable after restriction. Faithfulness of a geometric inverse image reflects such a monomorphism being an isomorphism. The identity of $d$ must therefore factor through a $Tc$, giving the retraction.

### Grothendieck topos

↑ **Parent:** [Elementary topos](#elementary-topos)

A Grothendieck topos is a category equivalent to the [sheaves on a site](category.md#sheaf-on-a-site) for a small [Grothendieck topology](category.md#grothendieck-topology). It is an [elementary topos](#elementary-topos) with all small colimits and a small generating family. Small disjoint coproducts, effective quotients and the set of subobjects of any fixed object allow many constructions by unions.

#### Classifying topos

↑ **Parent:** [Grothendieck topos](#grothendieck-topos)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classifying_topos)

A topos classifies a geometric theory when geometric morphisms into it from any [Grothendieck topos](#grothendieck-topos) correspond naturally to internal models of that theory. Pulling back one generic model gives the corresponding model. For a finitary [algebraic theory](foundations-of-mathematics.md#algebraic-theory), the classifying topos is the covariant functor category on finitely presented models.

##### Generic local ring

↑ **Parent:** [Classifying topos](#classifying-topos)

In the [sheaf topos](#grothendieck-topos) for the [Zariski coverage on finitely presented rings](category.md#zariski-coverage-on-finitely-presented-rings), the universal [local ring](commutative-algebra.md#local-ring) is represented by the polynomial ring $\mathbb Z[t]$. At the stage of a finitely presented ring $A$, its section set is $A$, and restriction along $A\to B$ is that ring map. It is internally local because the localizations at $x$ and $1-x$ cover each stage. Its square-zero infinitesimals are represented by $\mathbb Z[\varepsilon]/(\varepsilon^2)$. Stage rings need not themselves be local or reduced; their variation supplies the internal local and infinitesimal semantics.

###### Kock-Lawvere axiom for the generic local ring

↑ **Parent:** [Generic local ring](#generic-local-ring)

For $D=\{d\in R:d^2=0\}$ in the [generic local ring](#generic-local-ring), every internal map $D\to R$ has a unique affine expression $d\mapsto a+bd$. At the stage $A$, such maps are elements of $A[\varepsilon]/(\varepsilon^2)$, which is freely $A\oplus A\varepsilon$ as an $A$-module. This decomposition is natural under ring maps and proves the isomorphism. Testing only on ordinary fields loses the generic infinitesimal and would give an incorrect uniqueness argument.

##### Classifying topos of strict linear orders

↑ **Parent:** [Classifying topos](#classifying-topos)

Finite [strict total orders](set.md#strict-total-order) and increasing injections, including the empty order, give a presheaf classifier for strict total orders. Trichotomy locally merges two finite sorted tuples, identifying equal entries. A strict map from a chain is injective, so parallel maps admitting the same realization are already equal. Reflexification gives a geometric morphism to the [classifying topos of linear orders](#classifying-topos-of-linear-orders); pulling back weak totality gives exactly strict trichotomy.

##### Classifying topos of linear orders

↑ **Parent:** [Classifying topos](#classifying-topos)

With empty objects allowed, finite [totally ordered sets](set.md#totally-ordered-set) and all weak [order-preserving functions](set.md#order-preserving-function) give a presheaf classifier for weak total orders. Finite tuples in a model can locally be merged into a sorted tuple using finitely many totality disjunctions. Equalizing two maps between finite chains amounts to collapsing the convex intervals forced equal. These two constructions give the flatness conditions without assuming decidable equality.

##### Classifying topos of strict partial orders

↑ **Parent:** [Classifying topos](#classifying-topos)

Let $\mathbf{FinSPos}$ contain finite [strict partial orders](set.md#strict-partial-order) and [strict order-preserving functions](set.md#strict-order-preserving-function). Its covariant set-valued functor category classifies the strict theory. A finite presentation with a strict cycle is contradictory; every other finite diagram gives a finite strict partial order. Equalizing finitely many element identifications either gives such an order or forces a forbidden cycle, so the internal model-to-flat-functor construction remains valid. The [reflexification of a strict partial order](set.md#reflexification-of-a-strict-partial-order) induces a surjective geometric morphism to the weak-order classifier, but not a geometric embedding because strict maps exclude collapse of comparable elements.

##### Classifying topos of partial orders

↑ **Parent:** [Classifying topos](#classifying-topos)

Let $\mathbf{FinPos}$ contain finite [partially ordered sets](set.md#partially-ordered-set) and all [order-preserving functions](set.md#order-preserving-function), including the empty object. The covariant functor category $[\mathbf{FinPos},\mathbf{Set}]$ classifies weak [partial orders](set.md#partially-ordered-set). Finite positive presentations reduce to finite preorders with mutually comparable cycles identified. An internal model $M$ gives a flat functor $P\mapsto\operatorname{Hom}(P,M)$ on $\mathbf{FinPos}^{\rm op}$; conversely the corresponding filtered presentation by finite models recovers its carrier and order relation.

##### Duality between geometric quotients and subtoposes

↑ **Parent:** [Classifying topos](#classifying-topos)

Each [geometric quotient theory](mathematical-logic.md#geometric-quotient-theory) is classified by the corresponding [subtopos](#subtopos) of the original [classifying topos](#classifying-topos). Extra axioms impose extra covers on the [geometric syntactic topology](mathematical-logic.md#geometric-syntactic-topology). Conversely additional definable covers give the corresponding deductively closed quotient. Under [Morita equivalence of geometric theories](#morita-equivalence-of-geometric-theories), transporting a [subtopos](#subtopos) produces a corresponding quotient of the other theory, with equivalent classifiers. Stronger axioms correspond to smaller [subtoposes](#subtopos) under inclusion.

##### Morita equivalence of geometric theories

↑ **Parent:** [Classifying topos](#classifying-topos)

[Geometric theories](mathematical-logic.md#geometric-theory) are Morita-equivalent when their [classifying toposes](#classifying-topos) are equivalent. This gives equivalent internal model categories pseudonaturally in every [Grothendieck topos](#grothendieck-topos). A common [classifying topos](#classifying-topos) transports intrinsic invariants between different presentations; agreement of set-valued model categories alone is insufficient. The [duality between geometric quotients and subtoposes](#duality-between-geometric-quotients-and-subtoposes) transfers [geometric theory](mathematical-logic.md#geometric-theory) extensions along such an equivalence.

##### Classifying topos of integral domains

↑ **Parent:** [Classifying topos](#classifying-topos)

On the opposite of finitely presented commutative rings, cover the zero ring by the empty family and cover $A$ by $A/(a),A/(b)$ whenever $ab=0$. The generated topology classifies nontrivial integral domains, with generic model the sheafified tautological ring. It is not subcanonical: at $\mathbb Z/4$, the covering quotient to $\mathbb Z/2$ identifies the distinct sections $0$ and $2$ of the polynomial-ring representable.

###### Finite-tuple weak-field property of the generic integral domain

↑ **Parent:** [Classifying topos of integral domains](#classifying-topos-of-integral-domains)

In the generic domain, negation of simultaneous invertibility of finitely many elements implies that one is zero. At a ring stage, localize at their product $t$. All become units, so a tuple satisfying the negation makes the localized stage empty. The [empty-cover criterion for the domain-classifying site](#empty-cover-criterion-for-the-domain-classifying-site) then says $A[1/t]=0$, hence $t$ is nilpotent. Repeated zero-product covers force one factor to vanish locally. The two-variable property conversely forces the integral-domain axiom in any nontrivial internal ring.

###### Empty-cover criterion for the domain-classifying site

↑ **Parent:** [Classifying topos of integral domains](#classifying-topos-of-integral-domains)

For a finitely presented ring $A$, its sheafified representable is initial exactly when $A$ is the zero ring. The zero ring has a generating empty cover. Every nonzero ring maps to a field by quotienting by a maximal ideal, and that set-based domain gives a point at which the representable has a section, precluding initiality.

##### Quotient-theory coverage

↑ **Parent:** [Classifying topos](#classifying-topos)

Adding coherent or geometric axioms to a theory determines a coverage on a site for its [classifying topos](#classifying-topos). The antecedent presentation is covered by presentations where its consequent disjuncts and witnesses hold. Sheafification imposes those axioms on the generic model. An inconsistent antecedent gets an empty cover.

##### Generic model of an algebraic theory

↑ **Parent:** [Classifying topos](#classifying-topos)

In $[\mathbb T_{fp},\mathbf{Set}]$, the generic model assigns to each finitely presented algebra its underlying set at each sort, with the algebraic operations pointwise. It is covariant on algebra homomorphisms. Pullback along a geometric morphism yields its classified internal model.

### Decidable object in a topos

↑ **Parent:** [Elementary topos](#elementary-topos)

An object is decidable when its diagonal is a complemented [subobject](category.md#subobject) of its square. Equivalently its internal equality is decidable. Pullback gives closure under subobjects; coordinatewise equality gives closure under finite products. For an existing coproduct, unequal summands together with the complements of the diagonal in each equal summand form the diagonal complement.

#### Decidability in a set-valued functor category

↑ **Parent:** [Decidable object in a topos](#decidable-object-in-a-topos)

A covariant set-valued functor $F$ is a decidable object precisely when every transition map $F(u)$ is injective. The pointwise complement of its diagonal consists of unequal pairs; it is a subfunctor exactly when transition maps preserve inequality. For left [M-sets](algebra.md#m-set), this says that every action map is injective.

#### Quotients of decidable objects

↑ **Parent:** [Decidable object in a topos](#decidable-object-in-a-topos)

In a [Grothendieck topos](#grothendieck-topos), an object is a quotient of a decidable object when it has an epic cover by one. These objects are closed under subobjects, small coproducts, quotients and finite limits. Their union inside any fixed object gives the largest subobject of this kind, defining a [coreflective subcategory](category.md#coreflective-subcategory). The induced [idempotent comonad](category.md#idempotent-comonad) is left exact, so the full subcategory is a [topos](#elementary-topos).

### Internal logic of a topos

↑ **Parent:** [Elementary topos](#elementary-topos)

The [subobject classifier](#subobject-classifier) supplies intuitionistic truth values. [Subobjects](category.md#subobject) interpret predicates, [finite limits](category.md#finite-limit) interpret finite conjunctions and equality, and suitable image and adjoint constructions interpret quantifiers. One must distinguish internal intuitionistic arguments from classical reasoning in the external category of sets.

### Subobject classifier

↑ **Parent:** [Elementary topos](#elementary-topos)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subobject_classifier)

A subobject classifier is a monomorphism $\top:1\to\Omega$ such that every monomorphism $A'\hookrightarrow A$ is, uniquely, a pullback of $\top$ along a characteristic map $\chi_{A'}:A\to\Omega$.

#### Shift epimorphism of the natural-number presheaf classifier

↑ **Parent:** [Subobject classifier](#subobject-classifier)

In the covariant [functor category](category.md#functor-category) $[\mathbb N,\mathbf{Set}]$, the classifier at $n$ consists of thresholds $k\geq n$ and the empty threshold $\infty$. Its transition to $n+1$ sends $k$ to $\max(k,n+1)$. The displayed maps commute with transitions and are all surjective, so define an [epimorphism](category.md#epimorphism). They identify $n$ and $n+1$, so the endomorphism is not an [isomorphism](algebra.md#isomorphism).

#### Monic endomorphism of a subobject classifier

↑ **Parent:** [Subobject classifier](#subobject-classifier)

In a category with [finite limits](category.md#finite-limit) and a [subobject classifier](#subobject-classifier), every monic endomorphism $f$ of $\Omega$ is an involution. The subobject $g:U\hookrightarrow\Omega$ classified by $f$ is subterminal, since $fg=\top!_U$ is monic. If $V\hookrightarrow U$ is classified by $g$, pullback uniqueness gives $f\top!_U=g$, hence $f^2g=g$. If $u$ classifies $U\hookrightarrow1$, the pullback of $g$ along $f$ is $\top!_U$, so $f^2(p)=u\wedge p$. Monicity implies $u=\top$, because $u\wedge u=u\wedge\top$, proving the displayed identity.

#### Internal Heyting algebra of truth values

↑ **Parent:** [Subobject classifier](#subobject-classifier)

The subobject classifier $\Omega$ of a topos carries internal truth, falsity, meet, join and implication. Its generalized elements over $X$ are subobjects of $X$; implication satisfies $R\leq(P\Rightarrow Q)$ exactly when $R\cap P\leq Q$. Pullback-compatible operations make this an internal [Heyting algebra](mathematical-logic.md#heyting-algebra), not merely a structure on global truth values.

### Lawvere-Tierney topology

↑ **Parent:** [Elementary topos](#elementary-topos)

A Lawvere-Tierney topology on a topos is a morphism $j:\Omega\to\Omega$ satisfying, internally,

$$
j(\top)=\top,
\qquad j(jp)=j(p),
\qquad j(p\wedge q)=j(p)\wedge j(q).
$$

It is also called a local operator.

#### Dense monomorphism classifier

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

The pullback of the truth point along a [local operator](#lawvere-tierney-topology) $j$ is the [subobject](category.md#subobject) $J\hookrightarrow\Omega$. A [monomorphism](category.md#monomorphism) with characteristic map $\chi$ is [j-dense](#j-dense-monomorphism) exactly when $\chi$ factors through $J$. Its internal order is inherited from the [Heyting algebra](mathematical-logic.md#heyting-algebra) of truth values. Having a least global element is an internal condition over all parameter objects, not just a condition on global truth values.

#### Quasi-closed local operator

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

For a subterminal truth value $u$, the quasi-closed local operator is relative double negation $q(U)(p)=((p\Rightarrow u)\Rightarrow u)$. It has bottom value $q(U)(0)=u$. Its fixed truth values are Boolean with relative bottom $u$, inherited meet, join closed by $q(U)$ and complement $p\Rightarrow u$. Therefore its sheaf topos is a [Boolean topos](#boolean-topos).

##### Boolean cover by a generic quasi-closed subtopos

↑ **Parent:** [Quasi-closed local operator](#quasi-closed-local-operator)

In $\mathcal E/\Omega$, the generic truth mono $\top:1\hookrightarrow\Omega$ defines a quasi-closed Boolean subtopos. Its composite to $\mathcal E$ is surjective. If a predicate $p(x)$ pulled back from $\mathcal E$ becomes dense, then $((p(x)\Rightarrow u)\Rightarrow u)=1$ for the generic truth $u$. Substitution $u=p(x)$ yields $p(x)=1$, proving reflection of invertible monos and hence faithfulness.

#### Closed local operator

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

For a [subterminal object](category.md#subterminal-object) classified by $u$, the closed local operator is $p\mapsto u\vee p$. Its closed monos contain the pullback of that subterminal, hence are exactly the monos dense for the corresponding [open local operator](#open-local-operator).

#### Open local operator

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

For a [subterminal object](category.md#subterminal-object) classified by $u$, the open local operator is $p\mapsto(u\Rightarrow p)$. Its dense monos are exactly those whose image contains the pullback of that subterminal. It is complementary to the corresponding [closed local operator](#closed-local-operator).

##### Least dense truth characterizes an open local operator

↑ **Parent:** [Open local operator](#open-local-operator)

For $j=o(U)$, the [dense monomorphism classifier](#dense-monomorphism-classifier) consists of the truth values above $u$, so has least element $u$. Conversely, if it has least element $u$, density of a [monomorphism](category.md#monomorphism) is exactly containment of the pulled-back subterminal $U$. For a subobject $S\subseteq X$, the mono $S\to\overline S$ is dense, so $U\cap\overline S\subseteq S$ and $j(p)\le u\Rightarrow p$. Since $j(u)=\top$, applying $j$ to $u\wedge(u\Rightarrow p)\le p$ gives $u\Rightarrow p\le j(p)$. Hence equality holds.

##### Complementary open and closed local operators

↑ **Parent:** [Open local operator](#open-local-operator)

The [open local operator](#open-local-operator) and [closed local operator](#closed-local-operator) associated with $U$ have meet the identity and join the largest local operator. The meet identity is $(u\Rightarrow p)\wedge(u\vee p)=p$. Every mono factors through its union with $U$ as a closed-operator-dense mono followed by an open-operator-dense mono, proving that their join makes every mono dense.

#### Closure operation of a local operator

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

If a subobject $A'\hookrightarrow A$ has characteristic map $\chi:A\to\Omega$, its $j$-closure is classified by $j\chi$. This closure operation is inflationary, idempotent, and stable under pullback.

##### j-closed monomorphism

↑ **Parent:** [Closure operation of a local operator](#closure-operation-of-a-local-operator)

A mono is j-closed if it equals its closure under the [local operator](#lawvere-tierney-topology) $j$. Its characteristic map factors through the [closed-subobject classifier](#closed-subobject-classifier) $\Omega_j$. A j-closed subobject of a [j-sheaf](#j-sheaf) is a j-sheaf; a mono that is both closed and [j-dense](#j-dense-monomorphism) is an isomorphism.

##### j-dense monomorphism

↑ **Parent:** [Closure operation of a local operator](#closure-operation-of-a-local-operator)

A monomorphism is $j$-dense when its $j$-closure is its whole codomain. It is $j$-closed when it equals its closure. Dense monomorphisms are stable under pullback, and a monomorphism that is both dense and closed is an isomorphism.

#### j-sheaf

↑ **Parent:** [Lawvere-Tierney topology](#lawvere-tierney-topology)

An object $X$ is a $j$-sheaf when every map $A'\to X$ defined on the domain of a [j-dense monomorphism](#j-dense-monomorphism) $A'\hookrightarrow A$ extends uniquely to a map $A\to X$.

##### j-separated object

↑ **Parent:** [J-sheaf](#j-sheaf)

An object is j-separated when two maps into it which agree on a [j-dense monomorphism](#j-dense-monomorphism) are equal. Equivalently its diagonal is [j-closed](#j-closed-monomorphism). Quotienting an arbitrary object by the j-closure of its diagonal gives its separated reflection, used in constructing the [sheaf reflector for a local operator](#sheaf-reflector-for-a-local-operator).

##### Closed-subobject classifier

↑ **Parent:** [J-sheaf](#j-sheaf)

The closed-subobject classifier is the equalizer

$$
\Omega_j\hookrightarrow\Omega
\mathrel{\substack{\xrightarrow{\mathrm{id}}\\[-2pt]\xrightarrow[j]{} }}\Omega.
$$

It classifies $j$-closed subobjects and is itself a [j-sheaf](#j-sheaf). The local operator factors as a split epimorphism $q:\Omega\twoheadrightarrow\Omega_j$ followed by the canonical inclusion $i:\Omega_j\hookrightarrow\Omega$.

##### Sheaf reflector for a local operator

↑ **Parent:** [J-sheaf](#j-sheaf)

The full subcategory of $j$-sheaves is reflective. Its reflector $L$ sends every $j$-dense monomorphism to an isomorphism and preserves finite limits.

###### Subobject-classifier preservation criterion for a sheaf reflector

↑ **Parent:** [Sheaf reflector for a local operator](#sheaf-reflector-for-a-local-operator)

For a [local operator](#lawvere-tierney-topology) $j$, the following are equivalent: $L$ preserves the subobject classifier; $L(q):L\Omega\to\Omega_j$ is an isomorphism; the canonical inclusion $i:\Omega_j\hookrightarrow\Omega$ is $j$-dense; and every monomorphism $A'\hookrightarrow A$ factors as a $j$-closed mono $A'\hookrightarrow A''$ followed by a $j$-dense mono $A''\hookrightarrow A$.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (6)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-23.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#2/solution)
