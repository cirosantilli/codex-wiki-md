# Locally ringed space

↑ **Parent:** [Ringed space](ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Locally_ringed_space)

A locally ringed space is a [ringed space](ringed-space.md) whose stalk $\mathcal O_{X,x}$ is a [local ring](commutative-algebra.md#local-ring) at every point. Morphisms of locally ringed spaces induce local homomorphisms on stalks.

**Table of contents**

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

## Morphism of locally ringed spaces

↑ **Parent:** [Locally ringed space](locally-ringed-space.md)

A morphism is a continuous map $f:X\to Y$ together with a homomorphism $\mathcal O_Y\to f_*\mathcal O_X$ of [sheaves of rings](ringed-space.md#sheaf-of-rings) whose induced map on every [stalk](sheaf-of-modules.md#stalk-of-a-sheaf) is a [local homomorphism](commutative-algebra.md#local-homomorphism-of-local-rings). Applied to [schemes](#scheme), this is exactly a [morphism of schemes](#morphism-of-schemes).

## Scheme

↑ **Parent:** [Locally ringed space](locally-ringed-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scheme_(mathematics))

A scheme is a [locally ringed space](locally-ringed-space.md) covered by open subsets isomorphic to spectra of [commutative rings](commutative-algebra.md#commutative-ring). It retains both the points defined by prime ideals and the local algebra of functions around them.

### Functor represented by a scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functor_represented_by_a_scheme)

The functor of points describes a [scheme](#scheme) through its morphisms from test [schemes](#scheme). On [commutative rings](commutative-algebra.md#commutative-ring), it is covariant because a [ring homomorphism](commutative-algebra.md#ring-homomorphism) reverses the corresponding affine-scheme map. A functor on [rings](commutative-algebra.md#ring) is represented by $X$ in the algebraic-geometric sense when it is naturally isomorphic to $h_X$. The representing [scheme](#scheme) need not be affine; this is different from demanding a [representable functor](functor.md#representable-functor) in the category of [rings](commutative-algebra.md#ring) itself.

// Target: module-theory.bigb

### Gluing of schemes along open subschemes

↑ **Parent:** [Scheme](#scheme)

Given [schemes](#scheme) $X_i$ and [isomorphisms](algebra.md#isomorphism) between designated [open subschemes](#open-subscheme) satisfying inverse and cocycle conditions, identify the underlying open spaces and glue their structure sheaves. The resulting [locally ringed space](locally-ringed-space.md) is locally one of the $X_i$, hence a [scheme](#scheme). The same construction works for [formal schemes](#formal-scheme) and topological structure sheaves. Compatible morphisms out of the charts glue uniquely.

// Target: ringed-space.bigb

### Formal scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_scheme)

A [formal scheme](#formal-scheme) is a [locally ringed space](locally-ringed-space.md) with a [sheaf of topological rings](ringed-space.md#sheaf-of-topological-rings) that is locally a [formal spectrum](#formal-spectrum) of a complete adic [ring](commutative-algebra.md#ring). An ordinary [scheme](#scheme) is the special case of the discrete topology. A [formal completion of a scheme](#formal-completion-of-a-scheme) retains all [infinitesimal neighbourhoods](#infinitesimal-neighbourhood-of-a-closed-subscheme) of a [closed subscheme](#closed-subscheme), rather than just that subscheme.

// Target: ringed-space.bigb

#### Formal completion of a scheme

↑ **Parent:** [Formal scheme](#formal-scheme)

For a [closed subscheme](#closed-subscheme) with [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$ in a locally [Noetherian scheme](#noetherian-scheme), the completion is the [formal scheme](#formal-scheme) on $|Y|$ with topological structure sheaf $\varprojlim_n(\mathcal O_X/\mathcal I^{n+1})|_{|Y|}$. On a Noetherian [affine scheme](#affine-scheme) $\operatorname{Spec}A$, it is $\operatorname{Spf}(\varprojlim_nA/I^{n+1})$. Its [adic topology](commutative-algebra.md#adic-topology) remembers every [infinitesimal neighbourhood](#infinitesimal-neighbourhood-of-a-closed-subscheme).

// Target: commutative-algebra.bigb

##### Formal completion commutes with restriction to an open subscheme

↑ **Parent:** [Formal completion of a scheme](#formal-completion-of-a-scheme)

Restricting the topological structure sheaf of a [formal completion of a scheme](#formal-completion-of-a-scheme) to an [open subscheme](#open-subscheme) commutes with its [inverse limit](module-theory.md#inverse-limit): both sheaves are $\varprojlim_n(\mathcal O_U/(\mathcal I|_U)^{n+1})$ on $|U\cap Y|$. Equivalently, the identical [infinitesimal neighbourhoods](#infinitesimal-neighbourhood-of-a-closed-subscheme) have identical restricted structure sheaves. On formal affine charts this uses [completed localization of an adic ring](commutative-algebra.md#completed-localization-of-an-adic-ring).

// Target: toric-geometry.bigb

#### Formal spectrum

↑ **Parent:** [Formal scheme](#formal-scheme)

For a complete [ring](commutative-algebra.md#ring) with an [adic topology](commutative-algebra.md#adic-topology) defined by $I$, the [formal spectrum](#formal-spectrum) has the prime ideals containing $I$ as its points and structure sheaf $\varprojlim_n\mathcal O_{\operatorname{Spec}(A/I^{n+1})}$. On a [principal open subset](#principal-open-subscheme) $D(f)$ its sections form the [completed localization of an adic ring](commutative-algebra.md#completed-localization-of-an-adic-ring), not generally the ordinary localization $A_f$.

// Target: ringed-space.bigb

### Smooth morphism

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smooth_morphism)

A morphism of [schemes](#scheme) is smooth when it is locally of finite presentation, flat and has geometrically regular fibres. Smooth fibres alone do not imply that a morphism is smooth: flatness and the dimension behaviour matter as well. The [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve) has smooth [projective space](projective-space.md) fibres whose dimensions can jump.

<h3 id="etale-morphism">Étale morphism</h3>

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Étale_morphism)

A morphism of [schemes](#scheme) is étale when it is flat, unramified and locally of finite presentation. For a morphism between smooth varieties of the same dimension, an invertible differential gives this property locally. A finite étale morphism over an [algebraically closed field](algebra.md#algebraically-closed-field) has reduced finite fibres, and their cardinalities equal its degree when the source and target are connected.

<h4 id="finite-etale-morphism">Finite étale morphism</h4>

↑ **Parent:** [Étale morphism](#etale-morphism)

A finite étale morphism is both a [finite morphism](algebraic-variety.md#finite-morphism) and an [étale morphism](#etale-morphism). Affine-locally it is represented by a finite locally free algebra with zero module of [Kähler differentials](#kahler-differential). Its fibres are finite products of finite separable field extensions. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) with [good reduction](normalization-of-an-algebraic-curve.md#good-reduction-of-an-elliptic-curve) at a prime not dividing $m$, multiplication by $m$ on its smooth proper group model is finite étale of degree $m^2$: its differential is multiplication by the unit $m$. A division torsor of a section consequently gives an unramified local extension, the good-prime input to the [Weak Mordell-Weil theorem](normalization-of-an-algebraic-curve.md#weak-mordell-weil-theorem).

### Quasi-compact scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is quasi-compact when its underlying [topological space](topology.md#topological-space) is [quasi-compact](topology.md#compact-space): every [open cover](topology.md#open-cover) has a finite subcover. Since [affine open subsets](#affine-open-subscheme) form a base, this is equivalent to possessing a finite [affine open cover](topology.md#affine-open-cover). Every [affine scheme](#affine-scheme) is quasi-compact.

### Open subscheme

↑ **Parent:** [Scheme](#scheme)

An open subscheme of a [scheme](#scheme) $X$ is an [open subset](topology.md#open-set) $U$ equipped with the restriction of its [structure sheaf](#structure-sheaf-of-a-scheme). Its inclusion is an [open immersion](#open-immersion). Every scheme is covered by [affine open subschemes](#affine-open-subscheme). Any nonempty open subscheme of an [integral scheme](#integral-scheme) is integral and has the same [generic point](algebraic-geometry.md#generic-point) and [function field](algebraic-variety.md#function-field-of-an-algebraic-variety).

### Irreducible scheme

↑ **Parent:** [Scheme](#scheme)

An irreducible [scheme](#scheme) is one whose underlying [topological space](topology.md#topological-space) is a nonempty [irreducible topological space](algebraic-geometry.md#irreducible-topological-space). It can have [nilpotent elements](commutative-algebra.md#nilpotent) in its [structure sheaf](#structure-sheaf-of-a-scheme); irreducibility concerns only the topology. A [reduced scheme](#reduced-scheme) is an [integral scheme](#integral-scheme) precisely when it is irreducible.

### Dimension of a scheme

↑ **Parent:** [Scheme](#scheme)

The dimension of a [scheme](#scheme) is the supremum of the lengths of strict chains of irreducible closed subsets of its underlying topological space. On an affine scheme it is the [Krull dimension](commutative-algebra.md#krull-dimension) of its coordinate ring. Taking the reduced subscheme leaves the dimension unchanged.

### Structure morphism

↑ **Parent:** [Scheme](#scheme)

The structure morphism of a [scheme](#scheme) $X$ is its unique morphism $X\to\operatorname{Spec}\mathbb Z$. More generally, an $S$-scheme comes equipped with a specified morphism to the base scheme $S$.

### Scheme of characteristic p

↑ **Parent:** [Scheme](#scheme)

A [scheme](#scheme) $X$ has characteristic $p$ when $p\cdot1=0$ in its [structure sheaf of a scheme](#structure-sheaf-of-a-scheme). Equivalently, its [structure morphism](#structure-morphism) $X\to\operatorname{Spec}\mathbb Z$ factors through $\operatorname{Spec}\mathbb F_p$.

#### Absolute Frobenius morphism

↑ **Parent:** [Scheme of characteristic p](#scheme-of-characteristic-p)

The absolute Frobenius morphism of a [scheme of characteristic p](#scheme-of-characteristic-p) is the identity on the underlying topological space and raises every local function to its $p$th power. On an affine chart $\operatorname{Spec}A$ it is induced contravariantly by the [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) $A\to A$, $a\mapsto a^p$. It need not be an [isomorphism of schemes](#isomorphism-of-schemes), even when it acts invertibly on global sections.

The algebraic [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) induces this scheme map contravariantly on affine charts.

##### Frobenius factorization through a finite normal cover

↑ **Parent:** [Absolute Frobenius morphism](#absolute-frobenius-morphism)

For a finite surjective map of normal [integral schemes](#integral-scheme) with [function fields](algebraic-variety.md#function-field-of-an-algebraic-variety) $K\subseteq L$ in characteristic $p$, the condition $L^p\subseteq K$ lets the [Absolute Frobenius morphism](#absolute-frobenius-morphism) of the source factor through the map. On an affine chart $A\subseteq B$, send $b$ to $b^p\in A$: it lies in $K$, is integral over $A$, and $A$ is integrally closed. The condition $K\subseteq L^p$ instead lets the map factor after the source Frobenius. Send $a$ to its unique $p$th root in $L$; that root lies in the normal ring $B$ because it satisfies a monic polynomial over $B$. These rules localize and glue; injectivity of Frobenius in the [function field](algebraic-variety.md#function-field-of-an-algebraic-variety) supplies uniqueness.

### Structure sheaf of a scheme

↑ **Parent:** [Scheme](#scheme)

The structure sheaf $\mathcal O_X$ records the [regular functions](#regular-function) on every open subset of a [scheme](#scheme) $X$. Its stalk $\mathcal O_{X,x}$ is the [local ring](commutative-algebra.md#local-ring) of functions defined near $x$.

<h4 id="idempotent-clopen-correspondence">Idempotent–clopen correspondence</h4>

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

A global [idempotent](commutative-algebra.md#idempotent) on a [scheme](#scheme) is zero or one in every [local ring](commutative-algebra.md#local-ring). Its one-locus is both open and closed. Conversely a clopen subset determines a global [idempotent](commutative-algebra.md#idempotent) by gluing one on it and zero on its complement. Under this correspondence, decompositions into nonzero [orthogonal idempotents](commutative-algebra.md#orthogonal-idempotent) correspond to disjoint clopen decompositions. When all [connected components](geometry-and-topology.md#connected-component) are open, the [primitive idempotents](commutative-algebra.md#primitive-idempotent) correspond exactly to those components. Without orthogonality the assertion fails in characteristic two: $(1,0)=(1,1)+(0,1)$ in $\mathbb F_2\times\mathbb F_2$.

#### Sheaf of units of the structure sheaf

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

The units in the [structure sheaf of a scheme](#structure-sheaf-of-a-scheme) form a multiplicative [sheaf of abelian groups](algebraic-geometry.md#sheaf-of-abelian-groups). On a [smooth algebraic curve](algebraic-variety.md#smooth-algebraic-curve), a nonzero [rational function](isolated-singularity.md#rational-function) is a unit at a point precisely when its [discrete valuation](commutative-algebra.md#discrete-valuation) there is zero. Its inclusion in the [sheaf of nonzero rational functions on an irreducible variety](algebraic-variety.md#sheaf-of-nonzero-rational-functions-on-an-irreducible-variety) relates [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve) to the [Picard group](sheaf-of-modules.md#picard-group) through the [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology).

#### Regular function

↑ **Parent:** [Structure sheaf of a scheme](#structure-sheaf-of-a-scheme)

A regular function on an open subset $U$ of a [scheme](#scheme) $X$ is a section of $\mathcal O_X(U)$. On an affine variety it is locally a quotient of polynomial functions with a denominator that does not vanish.

On a variety, a regular function is a [regular map](algebraic-variety.md#morphism-of-algebraic-varieties) to the [affine line](#affine-line); the arbitrary-target regular-map concept is broader.

##### Global regular function

↑ **Parent:** [Regular function](#regular-function)

A global regular function is a [global section](sheaf-of-modules.md#global-section) of the [structure sheaf](#structure-sheaf-of-a-scheme) of a [scheme](#scheme), defined on the entire scheme. These functions form its ring $H^0(X,\mathcal O_X)$. On an [affine scheme](#affine-scheme) this recovers the defining ring; on a positive-dimensional [projective complete intersection](#projective-complete-intersection) it consists only of constants over the base [field](algebra.md#field).

###### Global regular functions on an irreducible projective variety

↑ **Parent:** [Global regular function](#global-regular-function)

Over an [algebraically closed field](algebra.md#algebraically-closed-field), every [regular function](#regular-function) on a nonempty irreducible [projective variety](projective-space.md#projective-variety) is constant. Regard the function as a morphism to $\mathbb P^1$ avoiding infinity. Its graph is closed; the [closedness of projection from projective space](#closedness-of-projection-from-projective-space) makes its image closed in $\mathbb P^1$. A proper closed subset there is finite, and an irreducible finite image is a singleton. Irreducibility is the usual variety convention; on a disconnected projective algebraic set different components may have different constants.

###### Regular functions on the punctured affine plane

↑ **Parent:** [Global regular function](#global-regular-function)

For $W=\mathbb A_k^2\setminus\{0\}$, restriction to $D(x)$ and $D(y)$ gives

$$
\Gamma(W,\mathcal O_W)=k[x,y]_x\cap k[x,y]_y=k[x,y].
$$

The intersection is taken in $k(x,y)$ and the equality follows from [unique factorization](algebra.md#unique-factorization-in-an-integral-domain): a reduced denominator dividing powers of both $x$ and $y$ is a unit. The inclusion $W\hookrightarrow\mathbb A^2$ induces an isomorphism on global functions but is not an isomorphism, so $W$ is not an [affine variety](algebraic-variety.md#affine-algebraic-set).

### Reduced scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_scheme)

A scheme is reduced when every [local ring](commutative-algebra.md#local-ring) $\mathcal O_{X,x}$ is a [reduced ring](commutative-algebra.md#reduced-ring), equivalently when its structure sheaf has no nonzero [nilpotent element](commutative-algebra.md#nilpotent). The affine scheme $\operatorname{Spec}A$ is reduced exactly when $A$ is reduced.

#### Generic reducedness with no embedded components

↑ **Parent:** [Reduced scheme](#reduced-scheme)

A Noetherian scheme with no embedded [associated primes](module-theory.md#associated-prime-of-a-module) is reduced if it is reduced at all its generic points. Locally, a nonzero nilpotent ideal would have an [associated prime](module-theory.md#associated-prime-of-a-module), necessarily a minimal prime. Its localization there would be nonzero, contradicting generic reducedness. This is useful with the [unmixedness of a complete intersection](#unmixedness-of-a-complete-intersection).

#### Integral scheme

↑ **Parent:** [Reduced scheme](#reduced-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_scheme)

An integral scheme is a nonempty [scheme](#scheme) that is both [reduced](#reduced-scheme) and [irreducible](algebraic-geometry.md#irreducible-topological-space). An affine scheme $\operatorname{Spec}A$ is integral exactly when $A$ is an [integral domain](commutative-algebra.md#integral-domain).

##### Generic-point embedding of regular functions

↑ **Parent:** [Integral scheme](#integral-scheme)

On an [integral scheme](#integral-scheme) $X$, every nonempty open $U$ contains its [generic point](algebraic-geometry.md#generic-point) $\eta$. Taking a [germ](sheaf-of-modules.md#germ-of-a-sheaf-section) gives an injective [ring homomorphism](commutative-algebra.md#ring-homomorphism) from its [regular functions](#regular-function) to the [function field](algebraic-variety.md#function-field-of-an-algebraic-variety) $\mathcal O_{X,\eta}$. Injectivity follows on each nonempty [affine open subscheme](#affine-open-subscheme) from the injection of an [integral domain](commutative-algebra.md#integral-domain) into its [field of fractions](commutative-algebra.md#field-of-fractions), and then from the [sheaf gluing axiom](algebraic-geometry.md#sheaf-gluing-axiom). This lets regular functions on different open subsets be compared inside one field.

### Group scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_scheme)

A group scheme over a base scheme $S$ is an $S$-scheme $G$ with multiplication $m:G\times_SG\to G$, an identity section $e:S\to G$, and inversion $i:G\to G$ satisfying the group axioms as equalities of morphisms.

#### Homomorphism of group schemes

↑ **Parent:** [Group scheme](#group-scheme)

A homomorphism of group schemes $f:H\to G$ is a morphism over the base that commutes with multiplication: $f\circ m_H=m_G\circ(f\times f)$. It consequently preserves the identity and inversion.

#### Multiplication-by-n morphism

↑ **Parent:** [Group scheme](#group-scheme)

For a commutative [group scheme](#group-scheme) $G$, the multiplication-by-$n$ morphism $[n]_G:G\to G$ adds a point to itself $n$ times. On an [abelian variety](abelian-variety.md), it is surjective for every nonzero integer $n$.

### Nonreduced scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is nonreduced when its structure sheaf contains a nonzero [nilpotent element](commutative-algebra.md#nilpotent). For an affine scheme $\operatorname{Spec}(A/I)$, this is equivalent to the ideal $I$ not being radical.

#### Nonreduced double point

↑ **Parent:** [Nonreduced scheme](#nonreduced-scheme)

The spectrum of the [dual number](commutative-algebra.md#dual-number) ring $k[\epsilon]/(\epsilon^2)$ is a [nonreduced scheme](#nonreduced-scheme) of length two supported at one point. Its nonzero nilpotent $\epsilon$ retains first-order information that the underlying singleton topological space forgets. It differs from the disjoint union of two reduced $k$-points.

### Punctual scheme

↑ **Parent:** [Scheme](#scheme)

A scheme over an algebraically closed field is punctual when its underlying topological space consists of one closed rational point. It may have nontrivial nilpotent structure, such as $\operatorname{Spec}k[\varepsilon]/(\varepsilon^2)$.

### Spectrum of a commutative ring

↑ **Parent:** [Scheme](#scheme)

The spectrum $\operatorname{Spec}A$ of a [commutative ring](commutative-algebra.md#commutative-ring) $A$ is the set of its [prime ideals](commutative-algebra.md#prime-ideal), with closed sets $V(I)=\{\mathfrak p:I\subseteq\mathfrak p\}$ and a structure sheaf whose sections locally look like fractions.

#### Spectrum map for the complexification of a real polynomial ring

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)

Contraction sends the zero [prime ideal](commutative-algebra.md#prime-ideal) to zero. A complex closed point $(x-z)$ contracts to $(x-z)$ when $z$ is real, and to $((x-\operatorname{Re}z)^2+(\operatorname{Im}z)^2)$ otherwise. Thus the map on the [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) is surjective and identifies each nonreal conjugate pair. Both spectra have only finite proper [Zariski-closed sets](algebraic-geometry.md#zariski-closed-set), so this is also the topological quotient by complex conjugation.

#### Disconnected reduced spectrum product decomposition

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)

For a [reduced ring](commutative-algebra.md#reduced-ring) with a nonempty disconnected [spectrum of a commutative ring](#spectrum-of-a-commutative-ring), choose a separation $V(I)\sqcup V(J)$. Disjointness gives $I+J=R$; covering the spectrum gives $IJ\subseteq\sqrt{(0)}=0$. For [comaximal ideals](commutative-algebra.md#comaximal-ideals), $I\cap J=IJ$. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) then supplies a product of two nonzero quotient [rings](commutative-algebra.md#ring). Equivalently, if $i+j=1$ with $i\in I$, $j\in J$, then $i,j$ are nontrivial orthogonal [idempotents](commutative-algebra.md#idempotent). This connects topology of the spectrum to [ring product decomposition by an idempotent](commutative-algebra.md#ring-product-decomposition-by-an-idempotent) without a Noetherian assumption.

#### Affine scheme

↑ **Parent:** [Spectrum of a commutative ring](#spectrum-of-a-commutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_scheme)

An affine scheme is a [scheme](#scheme) isomorphic to $\operatorname{Spec}A$ for some [commutative ring](commutative-algebra.md#commutative-ring) $A$. Homomorphisms $A\to B$ correspond contravariantly to morphisms $\operatorname{Spec}B\to\operatorname{Spec}A$.

##### Affine gluing along closed subschemes

↑ **Parent:** [Affine scheme](#affine-scheme)

Suppose a scheme is the scheme-theoretic union of affine closed subschemes $Y=\operatorname{Spec}A$ and $Z=\operatorname{Spec}B$, meaning their ideal sheaves have zero intersection. The intersection $W$ is closed in both, hence affine with coordinate ring $C$ and surjections $A\to C$, $B\to C$. Then the whole scheme is $\operatorname{Spec}(A\times_CB)$. Both projections of this fiber product are surjective; their kernels have zero intersection and product, and their quotient by the sum is $C$. Thus its spectrum has the same closed pieces, intersection and topology. The structure sheaf is the kernel of $i_*\mathcal O_Y\oplus j_*\mathcal O_Z\to k_*\mathcal O_W$ on both spaces, identifying their locally ringed structures. A reduced Noetherian scheme has finitely many irreducible components, so induction proves it is affine if and only if its reduced irreducible components are affine. The intersection $W$ need not be reduced.

##### Cohomological criterion for affineness

↑ **Parent:** [Affine scheme](#affine-scheme)

A [Noetherian scheme](#noetherian-scheme) is affine exactly when every [coherent ideal sheaf](sheaf-of-modules.md#coherent-ideal-sheaf) has zero first [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology). One direction is [vanishing of quasi-coherent cohomology on an affine scheme](sheaf-of-modules.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme). For the converse, ideal-sheaf vanishing produces [affine principal neighbourhoods from ideal-sheaf vanishing](#affine-principal-neighbourhoods-from-ideal-sheaf-vanishing). A finite such cover yields a [unit-ideal certificate from a principal affine cover](#unit-ideal-certificate-from-a-principal-affine-cover), and those [affine charts](#affine-chart-of-a-variety) glue to the [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) of [global sections](sheaf-of-modules.md#global-section). The criterion, including the finite-type ideal version for quasi-compact quasi-separated schemes, is recorded in [Stacks Project, Section 30.3](https://stacks.math.columbia.edu/tag/01XE).

###### Unit-ideal certificate from a principal affine cover

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

If finitely many $X_{f_i}$ cover $X$, the morphism $\mathcal O_X^r\to\mathcal O_X$ with coefficients $f_i$ is onto. If its [kernel](kernel-of-a-linear-map.md) has vanishing first [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology), the [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology) lifts the [global section](sheaf-of-modules.md#global-section) $1$ to coefficients $g_i$. This turns a geometric cover into a [unit ideal](commutative-algebra.md#unit-ideal) in the ring of [global sections](sheaf-of-modules.md#global-section).

###### Affine principal neighbourhoods from ideal-sheaf vanishing

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

Let $P$ have an affine open neighbourhood $U$, and let $Y=X\setminus U$. Evaluation gives $\mathcal I_Y\twoheadrightarrow k_P$ with [kernel](kernel-of-a-linear-map.md) $\mathcal I_Y\cap\mathcal I_P$. If first [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) of every [coherent ideal sheaf](sheaf-of-modules.md#coherent-ideal-sheaf) vanishes, a [global section](sheaf-of-modules.md#global-section) $f$ of $\mathcal I_Y$ can be chosen with $f(P)=1$. Then $X_f\subseteq U$ is a [principal open subset](#principal-open-subscheme) of an [affine variety](algebraic-variety.md#affine-algebraic-set) and is affine.

###### Ideal-sheaf vanishing for a coherent submodule of a trivial bundle

↑ **Parent:** [Cohomological criterion for affineness](#cohomological-criterion-for-affineness)

If $H^1(X,\mathcal I)=0$ for every [coherent ideal sheaf](sheaf-of-modules.md#coherent-ideal-sheaf), projection to the last coordinate makes any coherent $\mathcal F\subseteq\mathcal O_X^r$ an extension of a coherent submodule of $\mathcal O_X^{r-1}$ by an ideal sheaf. The [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology) proves the assertion by [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $r$.

##### Affine scheme reconstruction from global sections

↑ **Parent:** [Affine scheme](#affine-scheme)

For an [affine scheme](#affine-scheme) $X=\operatorname{Spec}A$, its ring of [global sections](sheaf-of-modules.md#global-section) is $A$. A [morphism of schemes](#morphism-of-schemes) between affine schemes is determined contravariantly by its map on these rings. Consequently a morphism between affine schemes is an [isomorphism of schemes](#isomorphism-of-schemes) exactly when that ring map is an isomorphism. The affine hypothesis is essential, as the [punctured affine plane](#punctured-affine-plane) shows.

##### Affine open subscheme

↑ **Parent:** [Affine scheme](#affine-scheme)

An affine open subscheme is an [open subset](topology.md#open-set) of a [scheme](#scheme) with its restricted [structure sheaf](#structure-sheaf-of-a-scheme), which is itself an [affine scheme](#affine-scheme). Every scheme has an [open cover](topology.md#open-cover) by such subschemes. On an affine scheme, the [principal open subschemes](#principal-open-subscheme) give an [open basis](topology.md#basis-of-a-topology).

###### Affine chart of a variety

↑ **Parent:** [Affine open subscheme](#affine-open-subscheme)

An open subset of an [algebraic variety](algebraic-variety.md) equipped with an identification with an [affine variety](algebraic-variety.md#affine-algebraic-set). Such charts make [quasi-coherent sheaves](sheaf-of-modules.md#quasi-coherent-sheaf) and regular maps accessible through their local [coordinate rings](algebraic-variety.md#coordinate-ring).

##### Principal open subscheme

↑ **Parent:** [Affine scheme](#affine-scheme)

For $f\in A$, the principal open subset $D(f)=\{\mathfrak p:f\notin\mathfrak p\}$ of $\operatorname{Spec}A$ is the [affine scheme](#affine-scheme) $\operatorname{Spec}A_f$.

###### Dense principal open inside a dense open subset

↑ **Parent:** [Principal open subscheme](#principal-open-subscheme)

In an [affine variety](algebraic-variety.md#affine-algebraic-set) with [coordinate ring](algebraic-variety.md#coordinate-ring) $A$, every dense open subset $U$ contains a dense [principal open subset](#principal-open-subscheme). Write its closed complement as $V(I)$. Density says that $I$ is contained in none of the finitely many [minimal prime ideals](commutative-algebra.md#minimal-prime-ideal) of the [reduced ring](commutative-algebra.md#reduced-ring) $A$. [Prime avoidance](commutative-algebra.md#prime-avoidance) supplies $s\in I$ outside all these primes. Thus $D(s)\subseteq U$, and $s$ is a [non-zero-divisor](mathematics.md#non-zero-divisor). [Noetherian Zariski topology](algebraic-geometry.md#noetherian-zariski-topology) also makes $U$ a finite union of principal opens; one can add $D(s)$ to this cover. An arbitrary existing cover need not contain a dense member when the [variety](algebraic-variety.md) is reducible.

##### Affine line

↑ **Parent:** [Affine scheme](#affine-scheme)

The affine line over a field $k$ is $\mathbb A_k^1=\operatorname{Spec}k[t]$.

The one-dimensional scheme has an [affine space](geometry-and-topology.md#affine-space) of rational points over its base field; its scheme structure also records non-rational points and local rings.

##### Affine plane

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

The [punctured affine plane](#punctured-affine-plane) $U=\mathbb A_k^2\setminus\{(0,0)\}$ is not an [affine scheme](#affine-scheme). On its cover $D(x)\cup D(y)$, [global sections](sheaf-of-modules.md#global-section) are $k[x,y]_x\cap k[x,y]_y=k[x,y]$ inside the [field of fractions](commutative-algebra.md#field-of-fractions). Coprimality of $x$ and $y$ proves this equality. If $U$ were affine, its inclusion into $\mathbb A_k^2$ would be an isomorphism by [affine scheme reconstruction from global sections](#affine-scheme-reconstruction-from-global-sections), contradicting the omitted point.

##### Affine three-space

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

### Noetherian scheme

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noetherian_scheme)

A Noetherian scheme has a finite cover by affine schemes $\operatorname{Spec}A_i$ with each $A_i$ a [Noetherian ring](algebra.md#noetherian-ring). Equivalently, it is quasi-compact and locally Noetherian.

#### Regular scheme

↑ **Parent:** [Noetherian scheme](#noetherian-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_scheme)

A locally Noetherian scheme is regular when every local ring $\mathcal O_{X,x}$ is a [regular local ring](commutative-algebra.md#regular-local-ring).

##### Regular in codimension one

↑ **Parent:** [Regular scheme](#regular-scheme)

A Noetherian scheme is regular in codimension one when every local ring at a codimension-one point is regular. For an integral scheme these local rings are then discrete valuation rings.

#### Normal scheme

↑ **Parent:** [Noetherian scheme](#noetherian-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_scheme)

An integral locally Noetherian scheme is normal when every local ring is an [integrally closed domain](commutative-algebra.md#integrally-closed-domain).

More generally a scheme is normal when every local ring is an integrally closed domain; the scheme need not be globally integral, for example a disjoint union of normal integral components.

##### Normalization of an integral scheme

↑ **Parent:** [Normal scheme](#normal-scheme)

For an [integral scheme](#integral-scheme), take on each [affine chart](#affine-chart-of-a-variety) the [integral closure](commutative-algebra.md#integral-closure) of its coordinate [ring](commutative-algebra.md#ring) in its [function field](algebraic-variety.md#function-field-of-an-algebraic-variety). [Integral closure](commutative-algebra.md#integral-closure) commutes with [localization](commutative-algebra.md#localization-of-a-ring), so these [rings](commutative-algebra.md#ring) glue to a [normal scheme](#normal-scheme) with an integral birational morphism to the original [scheme](#scheme). This is the normalization. It need not be finite without additional hypotheses; for an algebraic curve of finite type over a [field](algebra.md#field) it is finite. It is an [isomorphism](algebra.md#isomorphism) exactly when the original [scheme](#scheme) is normal.

##### Normal variety

↑ **Parent:** [Normal scheme](#normal-scheme)

An [algebraic variety](algebraic-variety.md) whose [local rings](commutative-algebra.md#local-ring) are [integrally closed domains](commutative-algebra.md#integrally-closed-domain). In particular an [irreducible variety](algebraic-variety.md#irreducible-variety) that is a [normal variety](#normal-variety) has normal affine [coordinate rings](algebraic-variety.md#coordinate-ring), enabling [codimension-two extension of regular functions on a normal variety](#codimension-two-extension-of-regular-functions-on-a-normal-variety).

###### Normal surface singularity

↑ **Parent:** [Normal variety](#normal-variety)

A singular point on a normal two-dimensional [algebraic variety](algebraic-variety.md) has an integrally closed local domain which is not a regular local ring. A [rational double point](#rational-double-point) is an important isolated example with a crepant minimal resolution.

###### Rational double point

↑ **Parent:** [Normal surface singularity](#normal-surface-singularity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_double_point)

A rational double point is a normal surface singularity whose minimal resolution has a configuration of smooth rational $(-2)$-curves of type $A$, $D$ or $E$. Birational projective models of [K3 surfaces](complex-geometry.md#k3-surface) arising from nef big systems contract orthogonal $(-2)$-curves to these singularities.

###### Normality of a quadratic cone

↑ **Parent:** [Normal variety](#normal-variety)

Over an algebraically closed field of characteristic different from two, a nondegenerate quadratic form of rank at least three is irreducible, its cone has only the vertex singular, and its hypersurface ring is Cohen-Macaulay. Thus $(R_1)$ and $(S_2)$ in the [Serre criterion for normality](#serre-s-criterion-for-normality) hold. In characteristic two, the reduced zero variety of $\sum_i t_i^2$ is instead the hyperplane $\sum_i t_i=0$, which is normal. The unreduced double-hyperplane scheme is not normal.

##### Codimension-two extension of regular functions on a normal variety

↑ **Parent:** [Normal scheme](#normal-scheme)

For an integral [normal variety](#normal-variety) that is [Noetherian](algebra.md#noetherian-ring), removing a closed subset of codimension at least two does not create new [regular functions](#regular-function). Affine-locally, a normal Noetherian domain is the intersection of its localizations at height-one primes inside its [fraction field](commutative-algebra.md#field-of-fractions). The complement still contains every height-one point, so a [regular function](#regular-function) on it lies in each such [localization](commutative-algebra.md#localization-of-a-ring) and therefore in the original ring. On projective space this also follows directly by excluding [irreducible polynomial](polynomial.md#irreducible-polynomial) factor of the denominators on each polynomial [affine chart](#affine-chart-of-a-variety).

<h5 id="serre-s-criterion-for-normality">Serre's criterion for normality</h5>

↑ **Parent:** [Normal scheme](#normal-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Serre's_criterion_for_normality)

A Noetherian ring is normal exactly when it satisfies $(R_1)$, regularity in codimension one, and $(S_2)$, depth at least $\min(2,\dim)$ at every localization.

### Morphism of schemes

↑ **Parent:** [Scheme](#scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_schemes)

A morphism of schemes is a morphism of [locally ringed spaces](locally-ringed-space.md). On affine schemes it is contravariantly equivalent to a homomorphism of their coordinate rings.

#### Graph morphism of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

For [morphisms of schemes](#morphism-of-schemes) $f:X\to Y$ and $g:Y\to Z$, the graph is the displayed map. It is the pullback of the [diagonal morphism](#diagonal-morphism) $Y\to Y\times_ZY$ along $(f\circ p_X,p_Y)$. Thus a [separated morphism](#separated-morphism) $g$ makes $\Gamma_f$ a [closed immersion](#closed-immersion). If also $g\circ f$ is a [closed immersion](#closed-immersion), the projection $X\times_ZY\to Y$ is a [closed immersion](#closed-immersion) by [base change of a morphism of schemes](#base-change-of-a-morphism-of-schemes), and its composite with $\Gamma_f$ proves that $f$ is a [closed immersion](#closed-immersion).

#### Affine-target adjunction for schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A [morphism of schemes](#morphism-of-schemes) into an [affine scheme](#affine-scheme) is uniquely determined by its homomorphism on [global sections](sheaf-of-modules.md#global-section). Conversely, a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $A\to\Gamma(X,\mathcal O_X)$ restricts on every [affine open subscheme](#affine-open-subscheme) of $X$ to a map into $\operatorname{Spec}A$; equality on affine covers of overlaps glues these maps. No quasi-compactness or affineness assumption on $X$ is needed.

#### Stein factorization

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stein_factorization)

A proper morphism $f:X\to Y$ factors as $X\xrightarrow{g}Z\xrightarrow{h}Y$, with $h$ finite and $g_*\mathcal O_X=\mathcal O_Z$; its fibers are connected. When $X$ is normal, $Z$ is normal. For a morphism from a smooth surface onto a curve, $Z$ is therefore a smooth projective curve over an algebraically closed field.

#### Isomorphism of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

An isomorphism of schemes is a [morphism of schemes](#morphism-of-schemes) admitting a two-sided inverse morphism. It is simultaneously a homeomorphism of the underlying spaces and an isomorphism of their structure sheaves.

#### Fiber product of schemes

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fiber_product_of_schemes)

The fibre product $X\times_SY$ represents pairs of morphisms to $X$ and $Y$ with equal composites to $S$. Affine-locally,

$$
\operatorname{Spec}A\times_{\operatorname{Spec}R}\operatorname{Spec}B
=\operatorname{Spec}(A\otimes_RB).
$$

##### Scheme-theoretic intersection

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For two [closed subschemes](#closed-subscheme) of a [scheme](#scheme) $X$, their intersection is their [fiber product of schemes](#fiber-product-of-schemes) over $X$. On an affine chart, ideals $I,J$ give the quotient by $I+J$. This retains nonreduced structure and [intersection multiplicities](algebraic-geometry.md#intersection-multiplicity) which a set-theoretic intersection would lose.

##### Point-lifting property of a scheme fibre product

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For [morphisms of schemes](#morphism-of-schemes) $X\to S$, $Y\to S$, a pair of points $x,y$ lifts to a point of $X\times_SY$ exactly when their base images agree. For sufficiency use the nonempty [spectrum of a commutative ring](#spectrum-of-a-commutative-ring) of $\kappa(x)\otimes_{\kappa(s)}\kappa(y)$, by [tensor product of field extensions is nonzero](module-theory.md#tensor-product-of-field-extensions-is-nonzero). This establishes existence, not uniqueness, of a lift.

##### Scheme-theoretic fibre

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

##### Universal property of a fibre product

↑ **Parent:** [Fiber product of schemes](#fiber-product-of-schemes)

For morphisms $X\to S$ and $Y\to S$, maps $T\to X\times_SY$ are naturally equivalent to pairs of maps $T\to X$ and $T\to Y$ whose composites to $S$ agree.

##### Base change of a morphism of schemes

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

#### Locally closed immersion

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A locally closed immersion factors as a closed immersion followed by an open immersion. Equivalently, it identifies its source with a closed subscheme of an open subscheme of the target.

##### Open immersion

↑ **Parent:** [Locally closed immersion](#locally-closed-immersion)

An open immersion is a [morphism of schemes](#morphism-of-schemes) that identifies its source with an open subscheme of its target. It is an isomorphism onto that open subscheme as a [locally ringed space](locally-ringed-space.md).

##### Diagonal morphism

↑ **Parent:** [Locally closed immersion](#locally-closed-immersion)

The diagonal morphism sends a point to the pair consisting of that point twice. Every diagonal of schemes is a locally closed immersion, and a morphism is separated exactly when its diagonal is a closed immersion.

###### Coincidence locus of two scheme morphisms

↑ **Parent:** [Diagonal morphism](#diagonal-morphism)

For morphisms $f,g:X\to Y$ over a base $S$, their scheme-theoretic coincidence locus is the fibre product

$$
\operatorname{Eq}(f,g)=X\times_{(f,g),\,Y\times_SY,\,\Delta_{Y/S}}Y.
$$

It is the [equalizer](category.md#equaliser) of $f$ and $g$, hence is universal among subschemes on which they agree. It is locally closed because every diagonal is an immersion, and closed when $Y\to S$ is separated.

<h4 id="kahler-differential">Kähler differential</h4>

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_differential)

For a ring map $A\to B$, the module of Kähler differentials represents $A$-derivations: $\operatorname{Hom}_B(\Omega_{B/A},M)\cong\operatorname{Der}_A(B,M)$.

For an algebra $B$ over $A$, the module $\Omega_{B/A}$ represents $A$-linear derivations: every derivation $B\to N$ factors uniquely through the universal map $d:B\to\Omega_{B/A}$.

<h5 id="kahler-differentials-under-a-separable-field-extension">Kähler differentials under a separable field extension</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

For finite separable $L/F$, every $k$-[derivation](associative-algebra.md#derivation-of-an-algebra) on $F$ into an $L$-module extends uniquely to $L$. Differentiate the minimal polynomial of each algebraic generator and divide by its nonzero derivative. Consequently the [Transitivity exact sequence for Kähler differentials](#transitivity-exact-sequence-for-kahler-differentials) identifies $\Omega_{L/k}$ with $L\otimes_F\Omega_{F/k}$, and $\Omega_{L/F}=0$.

<h5 id="base-change-for-kahler-differentials">Base change for Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

The [Kähler differentials](#kahler-differential) commute with extension of the base ring. A derivation of the base-changed algebra that kills $k'$ is determined by its restriction to $A\otimes1$, and the [Leibniz rule](calculus.md#leibniz-rule) provides its unique extension. No flatness hypothesis is required for this isomorphism.

<h5 id="localization-of-kahler-differentials">Localization of Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

[Kähler differentials](#kahler-differential) commute with [localization of a ring](commutative-algebra.md#localization-of-a-ring). The quotient rule $d(a/s)=(s\,da-a\,ds)/s^2$ uniquely extends a [derivation](associative-algebra.md#derivation-of-an-algebra) after inverting $s$; its universal property proves the displayed module isomorphism.

<h5 id="kahler-differentials-of-a-polynomial-algebra">Kähler differentials of a polynomial algebra</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

The [Kähler differentials](#kahler-differential) of a [polynomial ring](commutative-algebra.md#polynomial-ring) are free on the differentials of its variables. Assigning arbitrary values to these generators uniquely defines a [derivation](associative-algebra.md#derivation-of-an-algebra). Applying the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials) to a quotient gives its presentation by the formal derivatives of its defining equations.

<h5 id="universal-property-of-kahler-differentials">Universal property of Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

Composing an $A$-linear map with $d:A\to\Omega_{A/k}$ gives a $k$-[derivation](associative-algebra.md#derivation-of-an-algebra). Every derivation factors uniquely this way because its linearity and product rule are exactly the defining relations of the [module of Kähler differentials](#kahler-differential).

##### Conormal module of the diagonal

↑ **Parent:** [Kähler differential](#kahler-differential)

For a commutative $k$-algebra $A$, let $I$ be the kernel of multiplication $\mu:A\otimes_k A\to A$. The formula $a\mapsto[1\otimes a-a\otimes1]$ is a [derivation of an algebra](associative-algebra.md#derivation-of-an-algebra) into the [quotient module](module-theory.md#quotient-module) $I/I^2$, with $A$ acting through the first factor. It induces an isomorphism from the [module of Kähler differentials](#kahler-differential). An inverse is induced by $q(x\otimes y)=x\,dy$: the identity $q(rs)=\mu(r)q(s)+\mu(s)q(r)$ shows $q(I^2)=0$. For $z=\sum_i x_i\otimes y_i\in I$, the equality $\sum_i x_i y_i=0$ gives $[z]=\sum_i x_i[1\otimes y_i-y_i\otimes1]$, proving that the two maps are inverse. For an [affine variety](algebraic-variety.md#affine-algebraic-set), $I$ is the defining ideal of its [diagonal morphism](#diagonal-morphism).

<h5 id="conormal-exact-sequence-for-kahler-differentials">Conormal exact sequence for Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

For $A\to B\to C=B/I$, there is a right-exact sequence

$$
I/I^2\longrightarrow\Omega_{B/A}\otimes_BC\longrightarrow\Omega_{C/A}\longrightarrow0,
$$

where $[i]\mapsto di\otimes1$ and $db\otimes c\mapsto c\,d\bar b$.

###### Conormal sheaf

↑ **Parent:** [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials)

For a closed immersion, this [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf) measures the first-order equations of the subvariety. Its local [module](module-theory.md#module-mathematics) is $I/I^2$, and its map to the restricted [Kähler differential sheaf](#sheaf-of-kahler-differentials-over-a-field) sends the class of $f$ to $df$. This is the definition in [Stacks Project, Section 29.32](https://stacks.math.columbia.edu/tag/01R1).

###### Normal sheaf

↑ **Parent:** [Conormal sheaf](#conormal-sheaf)

For a [closed immersion](#closed-immersion) $i:Z\hookrightarrow X$ with [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$, the normal sheaf is $\mathcal N_{Z/X}=\mathcal Hom_{\mathcal O_Z}(\mathcal I/\mathcal I^2,\mathcal O_Z)$. It is the dual of the [conormal sheaf](#conormal-sheaf). For a regular embedding it is a [locally free sheaf](sheaf-of-modules.md#locally-free-sheaf); in the smooth case it agrees with the [normal bundle](algebraic-geometry.md#normal-bundle). Without regularity it need not be locally free, but its [global sections](sheaf-of-modules.md#global-section) still classify [first-order embedded deformations](algebraic-geometry.md#first-order-embedded-deformation).

###### Normal sheaf of a projective complete intersection

↑ **Parent:** [Normal sheaf](#normal-sheaf)

If a [projective complete intersection](#projective-complete-intersection) $Z\subseteq\mathbf P^n$ is cut out by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of degrees $d_1,\ldots,d_c$, then $\mathcal I/\mathcal I^2\cong\bigoplus_j\mathcal O_Z(-d_j)$ and $\mathcal N_{Z/\mathbf P^n}\cong\bigoplus_j\mathcal O_Z(d_j)$. The classes of the defining equations form the conormal basis: the first syzygies of a [regular sequence](commutative-algebra.md#regular-sequence) are the [Koszul complex](homology.md#koszul-complex) relations, whose coefficients vanish modulo the defining ideal. Thus the generator classes have no residual linear relations. Dualizing gives the stated [normal sheaf](#normal-sheaf).

###### Conormal injectivity for a generically smooth Cartier divisor

↑ **Parent:** [Conormal sheaf](#conormal-sheaf)

Let $W$ be an integral [effective Cartier divisor](cartier-divisor.md#effective-cartier-divisor) in an integral [variety](algebraic-variety.md) $V$ over a [perfect field](algebra.md#perfect-field), and suppose $W$ is not contained in the singular locus of $V$. On a dense open subset both [varieties](algebraic-variety.md) are smooth. The [Zariski tangent space](algebraic-geometry.md#zariski-tangent-space) of $W$ there has codimension one in that of $V$, so the differential of the local defining equation is nonzero. Thus the [conormal sheaf](#conormal-sheaf) map is injective generically. Its [kernel](kernel-of-a-linear-map.md) is a subsheaf of a [line bundle](sheaf-of-modules.md#line-bundle) on the integral [variety](algebraic-variety.md) $W$ and is therefore a [torsion-free sheaf](sheaf-of-modules.md#torsion-free-sheaf); generic vanishing implies zero everywhere. Right exactness is the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials).

<h5 id="transitivity-exact-sequence-for-kahler-differentials">Transitivity exact sequence for Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

For ring maps $A\to B\to C$, the first or transitivity exact sequence is

$$
\Omega_{B/A}\otimes_BC\longrightarrow\Omega_{C/A}\longrightarrow\Omega_{C/B}\longrightarrow0.
$$

The maps send $db\otimes c$ to $c\,db$ and then kill differentials of elements coming from $B$.

<h5 id="sheaf-of-relative-kahler-differentials">Sheaf of relative Kähler differentials</h5>

↑ **Parent:** [Kähler differential](#kahler-differential)

For a morphism of schemes $X\to Y$, the sheaf of relative Kähler differentials is obtained by sheafifying the modules $\Omega_{B/A}$ on affine charts $\operatorname{Spec}B\to\operatorname{Spec}A$.

###### Tangent sheaf of a scheme

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

The relative tangent sheaf is the [dual of a sheaf](sheaf-of-modules.md#dual-of-a-sheaf) of [Kähler differentials](#kahler-differential). Its sections are derivations of the [structure sheaf](#structure-sheaf-of-a-scheme) that kill base scalars. For a [smooth morphism](#smooth-morphism) it is [locally free](sheaf-of-modules.md#locally-free-sheaf) and describes first-order deformations of sections into the scheme.

###### Cotangent-sheaf cohomology of projective space

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For $n\geq1$, the cotangent form of the [Euler sequence](algebraic-geometry.md#euler-sequence) is $0\to\Omega^1_{\mathbb P^n/k}\to\mathcal O(-1)^{\oplus(n+1)}\to\mathcal O\to0$. The [cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space) and the [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology) give $H^1(\mathbb P_k^n,\Omega^1)\cong k$, with every other cohomology group zero. Therefore the [Euler characteristic of a coherent sheaf](sheaf-of-modules.md#euler-characteristic-of-a-coherent-sheaf) is $-1$. The nonzero class is the connecting image of the constant section $1$.

<h6 id="sheaf-of-kahler-differentials-over-a-field">Sheaf of Kähler differentials over a field</h6>

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For a [variety](algebraic-variety.md) over $k$, the [module of Kähler differentials](#kahler-differential) $\Omega_{A/k}$ on each [affine chart](#affine-chart-of-a-variety) gives a [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf). Compatibility with [localization](commutative-algebra.md#localization-of-a-ring) glues these into $\Omega^1_{X/k}$. A [finite presentation of an algebra](algebra-over-a-field.md#finite-presentation-of-an-algebra) gives a [finite presentation of a module](module-theory.md#finite-presentation-of-a-module) for its differentials, so this is a [coherent sheaf](sheaf-of-modules.md#coherent-sheaf) on a [variety](algebraic-variety.md).

###### Algebraic cotangent bundle

↑ **Parent:** [Sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field)

For a smooth [algebraic variety](algebraic-variety.md) of dimension $r$ over a field, the [sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field) is locally free of rank $r$ and defines its algebraic cotangent bundle. Its dual is the [tangent sheaf of a scheme](#tangent-sheaf-of-a-scheme). For a smooth hypersurface of degree $d$ in $\mathbb P^n$, the [Conormal exact sequence for Kähler differentials](#conormal-exact-sequence-for-kahler-differentials) is the short exact sequence $0\to\mathcal O_X(-d)\to\Omega^1_{\mathbb P^n}|_X\to\Omega^1_X\to0$.

###### Local freeness of differentials on a smooth variety

↑ **Parent:** [Sheaf of Kähler differentials over a field](#sheaf-of-kahler-differentials-over-a-field)

An invertible maximal-rank minor in the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) eliminates generators and gives a local surjection from $\mathcal O_X^n$ to the [Kähler differential sheaf](#sheaf-of-kahler-differentials-over-a-field). For an integral smooth [variety](algebraic-variety.md) the map is an [isomorphism](algebra.md#isomorphism) at the [generic point](algebraic-geometry.md#generic-point). Its [kernel](kernel-of-a-linear-map.md) is a submodule of a [free module](module-theory.md#free-module) over an [integral domain](commutative-algebra.md#integral-domain), so it is a [torsion-free module](module-theory.md#torsion-free-module); vanishing generically forces it to be zero. This gives local free frames for differentials.

###### Canonical line bundle of a smooth variety

↑ **Parent:** [Sheaf of relative Kähler differentials](#sheaf-of-relative-kahler-differentials)

For a smooth $n$-dimensional variety $X$ over a field, its canonical [line bundle](sheaf-of-modules.md#line-bundle) is $\omega_X=\bigwedge^n\Omega^1_{X/k}$. It is the bundle of top-degree algebraic differential forms. A nonzero rational section defines a [canonical divisor of a smooth variety](#canonical-divisor-of-a-smooth-variety). This algebraic definition works in arbitrary characteristic and is distinct from restricting the analytic canonical-bundle definition to complex manifolds.

###### Canonical divisor of a smooth variety

↑ **Parent:** [Canonical line bundle of a smooth variety](#canonical-line-bundle-of-a-smooth-variety)

A canonical divisor $K_X$ on a smooth integral variety is the [Cartier divisor](cartier-divisor.md) of a nonzero rational top-degree differential form; $\mathcal O_X(K_X)\cong\omega_X$. Its linear-equivalence class is independent of the chosen form. The [plurigenus](#plurigenus) is the dimension of the space of sections of a positive tensor power of this bundle.

###### Plurigenus

↑ **Parent:** [Canonical divisor of a smooth variety](#canonical-divisor-of-a-smooth-variety)

For a smooth [projective variety](projective-space.md#projective-variety), its $m$th plurigenus is $P_m(X)=h^0(X,\omega_X^{\otimes m})$, for $m\ge1$. These dimensions describe pluricanonical linear systems. [Blowup invariance of plurigenera](#blowup-invariance-of-plurigenera) proves their invariance under a point blowup on a smooth surface.

###### Blowup invariance of plurigenera

↑ **Parent:** [Plurigenus](#plurigenus)

For a point [blowup of a smooth algebraic surface](algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) $\psi:\widetilde X\to X$, where $X$ is a [smooth projective surface](algebraic-geometry.md#smooth-projective-surface) over an algebraically closed [field](algebra.md#field), multiplication by the exceptional section to power $m$ identifies $H^0(\widetilde X,m\psi^*K_X)$ with $H^0(\widetilde X,mK_{\widetilde X})$. Every effective pluricanonical representative must contain $mE$, since after subtracting $j<m$ copies its intersection with $E$ is $-m+j<0$. The [projection formula for sheaves](sheaf-of-modules.md#projection-formula) and $\psi_*\mathcal O=\mathcal O$ identify the remaining sections with those on $X$. No effectivity of $K_X$ itself is assumed.

#### Affine morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affine_morphism)

A morphism $f:X\to Y$ is affine when the inverse image of every affine open subscheme of $Y$ is affine. For a [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf) $\mathcal F$ on $X$, one has $R^qf_*\mathcal F=0$ for $q>0$.

##### Cohomology under an affine morphism

↑ **Parent:** [Affine morphism](#affine-morphism)

For an [affine morphism](#affine-morphism) $f:X\to Y$ and a [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf) $\mathcal F$ on $X$, the [direct image sheaf](sheaf-of-modules.md#direct-image-sheaf) has the same [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) on $Y$ as $\mathcal F$ on $X$. To prove this, take a [flasque resolution](sheaf-of-modules.md#flasque-resolution) $\mathcal F\to\mathcal I^\bullet$. Its direct images are [flasque sheaves](sheaf-of-modules.md#flasque-sheaf). On each affine open $V\subset Y$, the complex of sections of the direct images is $\Gamma(f^{-1}V,\mathcal I^\bullet)$. By [vanishing of quasi-coherent cohomology on an affine scheme](sheaf-of-modules.md#vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme), this augmented complex is exact. Checking on the affine basis proves that $f_*\mathcal I^\bullet$ resolves $f_*\mathcal F$. Its global sections are identical to those of the original resolution.

#### Flat morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_morphism)

A morphism $f:X\to Y$ is flat at $x\in X$ when the local ring $\mathcal O_{X,x}$ is a [flat module](module-theory.md#flat-module) over $\mathcal O_{Y,f(x)}$. It is flat when it is flat at every point.

##### Finite flat rank over an irreducible scheme

↑ **Parent:** [Flat morphism](#flat-morphism)

For a [finite morphism](algebraic-variety.md#finite-morphism) that is flat, its direct-image algebra is finite free at every local stalk. On an [irreducible scheme](#irreducible-scheme), every point specializes from the same generic point. Localizing each stalk further at that generic point shows that all these free ranks equal the generic rank. Hence all fibre algebras have the same dimension, even without assuming finite presentation in advance.

#### Morphism of finite type

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morphism_of_finite_type)

A morphism $f:X\to Y$ is of finite type when every point of $Y$ has an affine neighborhood $V=\operatorname{Spec}A$ for which $f^{-1}V$ has a finite affine cover $\operatorname{Spec}B_i$ with each $B_i$ a finitely generated $A$-algebra.

##### Quasi-finite morphism

↑ **Parent:** [Morphism of finite type](#morphism-of-finite-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-finite_morphism)

A finite-type [morphism of schemes](#morphism-of-schemes) is quasi-finite if its fibres are finite discrete schemes. A proper quasi-finite morphism is a [finite morphism](algebraic-variety.md#finite-morphism). In particular, a proper finite-type morphism of [projective varieties](projective-space.md#projective-variety) with no positive-dimensional fibres is finite; a positive-dimensional projective fibre would contain an integral curve.

#### Universally closed morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universally_closed_morphism)

A morphism is universally closed when every base change is a closed map on underlying topological spaces.

##### Projective line with a doubled point

↑ **Parent:** [Universally closed morphism](#universally-closed-morphism)

Glue two copies of $\mathbb P_k^1$ by the identity away from one chosen point. The resulting finite-type scheme is universally closed over $k$: after any base change, a closed subset meets each projective-line chart in a closed subset whose image is closed, and the total image is their finite union. The two copies of the chosen point cannot be separated, so the structure morphism is not separated and therefore is not proper.

#### Separated morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)

A morphism $f:X\to Y$ is separated when its diagonal $X\to X\times_YX$ is a [closed immersion](#closed-immersion). This is the scheme-theoretic analogue of the Hausdorff property.

A morphism of [schemes](#scheme) is separated when its diagonal is a [closed immersion](#closed-immersion). This is a property of the morphism, distinct from the broader morphism or diagonal constructions.

##### Separated scheme

↑ **Parent:** [Separated morphism](#separated-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separated_scheme)

A scheme over a base $S$ is separated when its structure morphism to $S$ is a [separated morphism](#separated-morphism). An absolute scheme is usually called separated when it is separated over $\operatorname{Spec}\mathbb Z$.

###### Separated variety

↑ **Parent:** [Separated scheme](#separated-scheme)

An [algebraic variety](algebraic-variety.md) that is separated over its ground field. Two affine open charts have an affine intersection: their intersection is the inverse image of the closed diagonal inside the product of the two [affine charts](#affine-chart-of-a-variety). This ensures a finite affine cover is acyclic for [quasi-coherent sheaves](sheaf-of-modules.md#quasi-coherent-sheaf).

##### Valuative criterion for separatedness

↑ **Parent:** [Separated morphism](#separated-morphism)

For a finite-type morphism of [Noetherian schemes](#noetherian-scheme), separatedness is equivalent to uniqueness in every lifting problem $\operatorname{Spec}K\to X$ over $\operatorname{Spec}R\to Y$, where $R$ is a [valuation ring](commutative-algebra.md#valuation-ring) with [fraction field](commutative-algebra.md#field-of-fractions) $K$.

This is the uniqueness part of the [valuative criterion](ringed-space.md#valuative-criterion).

#### Proper morphism

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_morphism)

A morphism is proper when it is separated, of finite type, and universally closed. Properness is stable under base change and composition.

##### Complete variety

↑ **Parent:** [Proper morphism](#proper-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_variety)

A [variety](algebraic-variety.md) over a field $k$ is complete when its map to $\operatorname{Spec}k$ is [universally closed](#universally-closed-morphism): after any base change, projection sends closed subsets to closed subsets. For a separated finite-type [variety](algebraic-variety.md), this is equivalent to being [proper](#proper-morphism). In the classical algebraically closed setting one may test projections $X\times Y\to Y$ for arbitrary [varieties](algebraic-variety.md). Images of rational points over a non-algebraically-closed field must not replace geometric images.

##### Proper affine morphisms are finite

↑ **Parent:** [Proper morphism](#proper-morphism)

For a finite-type affine morphism of Noetherian schemes, apply its valuative lifting property to each domain quotient $B/\mathfrak q$ for a minimal prime and all valuation rings of its fraction field containing the image of $A$. The lift forces $B/\mathfrak q$ into every such valuation ring, hence makes it integral over that image. For each $b\in B$, multiply the finitely many resulting monic equations. Its value at $b$ lies in the nilradical. The nilradical of a Noetherian ring is nilpotent, so a power of this monic polynomial annihilates $b$. Thus $B$ is integral over $A$. Finitely many algebra generators, each satisfying a monic equation, have their powers reduced to finitely many monomials, proving that $B$ is a finite $A$-module. Nilpotents cannot be ignored in this proof.

##### Properness descends from a surjective source

↑ **Parent:** [Proper morphism](#proper-morphism)

Suppose $gf$ is proper, $f$ is surjective, and $g$ is separated and of finite type. Surjectivity of scheme morphisms is preserved by base change: a nonempty fiber remains nonempty after a residue-field extension. After any base change to $Z$, for a closed subset $C$ of the new target of $f$, its inverse image is closed and has image $g(C)$ under the proper composite. Thus $g(C)$ is closed. This proves universal closedness of $g$, completing the three conditions for properness.

##### Properness cancels through a separated morphism

↑ **Parent:** [Proper morphism](#proper-morphism)

If $X\xrightarrow fY\xrightarrow gZ$ has proper composite and $g$ is separated, the graph $X\to X\times_ZY$ is a closed immersion, being a base change of the diagonal of $g$. The projection $X\times_ZY\to Y$ is a base change of the proper composite. Their composition is $f$, so $f$ is proper.

##### Properness is local on the target

↑ **Parent:** [Proper morphism](#proper-morphism)

If $f:X\to Y$ is a [morphism of schemes](#morphism-of-schemes) and $(U_i)$ is an open cover of $Y$, then $f$ is [proper](#proper-morphism) exactly when every restriction $f^{-1}(U_i)\to U_i$ is proper. The three defining properties—finite type, separatedness, and universal closedness—can each be checked on an open cover of the target.

##### Proper closed-point fibers do not imply properness

↑ **Parent:** [Proper morphism](#proper-morphism)

A finite-type morphism can have a proper fiber over every closed point without being proper. Properness controls compatible specialization in families, as expressed by the [valuative criterion for properness](#valuative-criterion-for-properness), rather than only the individual closed fibers.

##### Finite complex computing cohomology in a proper flat family

↑ **Parent:** [Proper morphism](#proper-morphism)

For a proper morphism $X\to\operatorname{Spec}A$ with $A$ Noetherian and an $A$-flat coherent sheaf $\mathcal F$, locally on the base there is a bounded complex of finite free modules $K^\bullet$ such that

$$
H^p(X,\mathcal F\otimes_AM)\cong H^p(K^\bullet\otimes_AM)
$$

naturally for every $A$-module $M$.

###### Cohomology and base change for line bundles on a curve

↑ **Parent:** [Finite complex computing cohomology in a proper flat family](#finite-complex-computing-cohomology-in-a-proper-flat-family)

In a proper flat family of [algebraic curves](algebraic-variety.md#algebraic-curve), if the first [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) of a [line bundle](sheaf-of-modules.md#line-bundle) vanishes on every fibre of an open set, its direct image there is a [vector bundle](vector-bundle.md) of rank given by the [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) and commutes with arbitrary [base change](#base-change-of-a-morphism-of-schemes). Locally a finite free complex computes both fibre [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) groups. Vanishing of the last cokernel makes its last map surjective; splitting that map leaves a finite locally free kernel in degree zero. This is the mechanism behind charts of the [Picard scheme of a curve](sheaf-of-modules.md#picard-scheme-of-a-curve) and evaluation descriptions of the [theta divisor](abelian-variety.md#theta-divisor).

###### Semicontinuity theorem for coherent cohomology

↑ **Parent:** [Finite complex computing cohomology in a proper flat family](#finite-complex-computing-cohomology-in-a-proper-flat-family)

For a proper morphism of Noetherian schemes and a coherent sheaf flat over the base, the fiber dimension $s\mapsto\dim_{\kappa(s)}H^p(X_s,\mathcal F_s)$ is upper semicontinuous, and the fiberwise Euler characteristic is locally constant.

###### Constancy of line bundle degree in a family

↑ **Parent:** [Semicontinuity theorem for coherent cohomology](#semicontinuity-theorem-for-coherent-cohomology)

For a [line bundle](sheaf-of-modules.md#line-bundle) $M$ on $C\times T$, with $C$ a smooth projective curve, this function is locally constant. Twist both $M$ and $M^{-1}$ by a large power of an [ample line bundle](sheaf-of-modules.md#ample-line-bundle) on $C$. Near a chosen fiber their first [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) groups vanish. The [Riemann-Roch theorem](algebraic-geometry.md#riemann-roch-theorem) and upper semicontinuity of their zeroth [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology) groups then bound the degree from above and below by the degree on that fiber. Connectedness of $T$ is necessary for a single constant across all fibers.

##### Valuative criterion for properness

↑ **Parent:** [Proper morphism](#proper-morphism)

For a finite-type morphism of [Noetherian schemes](#noetherian-scheme), properness is equivalent to existence and uniqueness in every lifting problem from the generic point $\operatorname{Spec}K$ of a [valuation ring](commutative-algebra.md#valuation-ring) $R$ to $\operatorname{Spec}R$.

This is the existence-and-uniqueness part of the [valuative criterion](ringed-space.md#valuative-criterion).

##### Projective morphism

↑ **Parent:** [Proper morphism](#proper-morphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_morphism)

A morphism $X\to S$ is projective when it factors as a [closed immersion](#closed-immersion) $X\hookrightarrow\mathbb P_S^n$ followed by the projection to $S$. Every projective morphism is proper.

###### Closedness of projection from projective space

↑ **Parent:** [Projective morphism](#projective-morphism)

Projection $X\times\mathbb P^n\to X$ sends closed subsets to closed subsets, with geometric points or schemes understood. On an affine base, choose finitely many homogeneous equations for a closed subset. Its fiber is nonempty exactly when every [graded multiplication map for a projective fiber](algebraic-geometry.md#graded-multiplication-map-for-a-projective-fiber) fails to be surjective, by the [Projective Nullstellensatz](algebraic-geometry.md#projective-nullstellensatz). The image is thus an intersection of closed rank-defect loci. An affine open cover proves the general case. This is the universally closed part of the [proper morphism](#proper-morphism) property of projective space.

###### Rational-point projection need not be Zariski closed

↑ **Parent:** [Closedness of projection from projective space](#closedness-of-projection-from-projective-space)

Over the real numbers, the closed equation $y_0^2=t y_1^2$ in $\mathbb A^1\times\mathbb P^1$ projects on real points to $\{t\ge0\}$, which is not [Zariski closed](algebraic-geometry.md#zariski-closed-set). Projective properness concerns scheme or geometric images, not the image of rational points over an arbitrary field. Similarly, $y_0^2+y_1^2$ has no real projective zero, but its [homogeneous ideal](commutative-algebra.md#homogeneous-ideal) contains no power of the [irrelevant ideal of projective space](algebraic-geometry.md#irrelevant-ideal-of-projective-space), since it has a complex projective zero.

##### Projective scheme

↑ **Parent:** [Proper morphism](#proper-morphism)

A projective scheme over a base $S$ is an $S$-scheme admitting a closed immersion into some projective space $\mathbb P_S^n$. Every projective morphism is [proper](#proper-morphism).

Projectivity is a property of the scheme over its specified base, expressed by its structural [projective morphism](#projective-morphism).

###### Proj construction

↑ **Parent:** [Projective scheme](#projective-scheme)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proj_construction)

For a graded ring $S$, $\operatorname{Proj}S$ consists of homogeneous prime ideals not containing the irrelevant ideal $S_+$. Its standard affine opens satisfy $D_+(f)\cong\operatorname{Spec}(S_f)_0$.

###### Degree-one generation condition for Proj

↑ **Parent:** [Proj construction](#proj-construction)

If a nonnegatively graded ring $S$ is generated by $S_1$ as an $S_0$-algebra, the [standard affine opens of Proj](#standard-affine-open-of-proj) $D_+(f)$ with $f\in S_1$ cover $\operatorname{Proj}S$. Indeed a homogeneous prime containing every degree-one element would contain the [irrelevant ideal of a graded ring](#irrelevant-ideal-of-a-graded-ring). This condition makes all [twisting sheaves on Proj](#twisting-sheaf-on-proj) invertible and makes graded sheafification compatible with [tensor products of sheaves](sheaf-of-modules.md#tensor-product-of-sheaves).

###### Sheaf associated with a graded module

↑ **Parent:** [Proj construction](#proj-construction)

A [graded module](commutative-algebra.md#graded-module) $M$ over a graded ring $S$ determines a [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf) on the [Proj construction](#proj-construction) $\operatorname{Proj}S$ by taking the degree-zero part of its localization on each [standard affine open of Proj](#standard-affine-open-of-proj). Localization identifies these module sheaves on overlaps. The construction is exact, by [exactness of localization](commutative-algebra.md#exactness-of-localization) and exactness of taking a fixed graded component.

###### Tensor compatibility of graded sheafification on degree-one-generated Proj

↑ **Parent:** [Sheaf associated with a graded module](#sheaf-associated-with-a-graded-module)

Under the [degree-one generation condition for Proj](#degree-one-generation-condition-for-proj), cover $X=\operatorname{Proj}S$ by degree-one charts. The [degree-one localization of a graded module](commutative-algebra.md#degree-one-localization-of-a-graded-module) identifies the two local modules in the displayed formula, using [localization commutes with tensor products](commutative-algebra.md#localization-commutes-with-tensor-products). The maps are natural and agree on overlaps, so they glue to an isomorphism of [sheaves of modules](sheaf-of-modules.md). The analogous assertion can fail for general positively graded rings.

###### Twisting sheaf on Proj

↑ **Parent:** [Sheaf associated with a graded module](#sheaf-associated-with-a-graded-module)

With the [graded shift](commutative-algebra.md#graded-shift) convention $S(n)_d=S_{n+d}$, this is the [sheaf associated with a graded module](#sheaf-associated-with-a-graded-module) $S(n)$. Under the [degree-one generation condition for Proj](#degree-one-generation-condition-for-proj), it is an [invertible sheaf](sheaf-of-modules.md#line-bundle): on $D_+(f)$ with $\deg f=1$, multiplication by $f^n$ freely generates its local module for every integer $n$. Without that hypothesis, it need not be invertible. The [twisting sheaf on projective space](sheaf-of-modules.md#twisting-sheaf-on-projective-space) is the standard special case. [Stacks Project, Section 27.10](https://stacks.math.columbia.edu/tag/01MM) records the hypotheses and local trivializations.

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

#### Closed immersion

↑ **Parent:** [Morphism of schemes](#morphism-of-schemes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_immersion)

A morphism $i:Z\to X$ is a closed immersion when it identifies $Z$ homeomorphically with a closed subset of $X$ and the morphism $\mathcal O_X\to i_*\mathcal O_Z$ is surjective. Affine-locally it has the form $\operatorname{Spec}(A/I)\to\operatorname{Spec}A$.

##### Flat closed immersion of finite presentation

↑ **Parent:** [Closed immersion](#closed-immersion)

A nonempty flat [closed immersion](#closed-immersion) of finite presentation into a connected [scheme](#scheme) is an [isomorphism](algebra.md#isomorphism). On a chart it is $A\to A/I$ with $I$ finitely generated. At a prime containing $I$, the quotient is a finite flat module over the [local ring](commutative-algebra.md#local-ring), hence free of rank one, so $I$ vanishes there. Finite generation extends this vanishing to a neighbourhood. Thus the image is open as well as closed; connectedness makes it all of the target, and the ideal is everywhere zero. Without finite presentation the conclusion can fail.

##### Closed immersion criterion for affine schemes

↑ **Parent:** [Closed immersion](#closed-immersion)

A surjective [ring homomorphism](commutative-algebra.md#ring-homomorphism) $A\to B=A/I$ identifies the [spectrum of a ring](#spectrum-of-a-commutative-ring) $B$ with the closed subset $V(I)$ and induces a surjective map of structure sheaves. Conversely, the [direct image sheaf](sheaf-of-modules.md#direct-image-sheaf) of $\mathcal O_{\operatorname{Spec}B}$ under an affine morphism is the sheaf associated with the $A$-module $B$: its sections on $D(a)$ are $B_{\phi(a)}$. The cokernel of the structure-sheaf map is therefore associated with the module cokernel of $A\to B$. If the sheaf map is surjective, all localizations of that cokernel vanish and the module cokernel is zero. This proves the converse without assuming global sections preserve arbitrary sheaf surjections.

##### Nilpotent thickening

↑ **Parent:** [Closed immersion](#closed-immersion)

A nilpotent thickening is a [closed immersion](#closed-immersion) defined by a nilpotent [ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme). Its underlying topological map is a [homeomorphism](topology.md#homeomorphism), because every [prime ideal](commutative-algebra.md#prime-ideal) contains every [nilpotent element](commutative-algebra.md#nilpotent). For example, quotienting the [dual numbers](commutative-algebra.md#dual-number) by $(\varepsilon)$ changes the [structure sheaf](#structure-sheaf-of-a-scheme) without changing the single point of the spectrum.

##### Closed subscheme

↑ **Parent:** [Closed immersion](#closed-immersion)

A closed subscheme of $X$ is a [scheme](#scheme) $Z$ together with a [closed immersion](#closed-immersion) $Z\hookrightarrow X$, usually identified with its image and its quotient structure sheaf.

###### Infinitesimal neighbourhood of a closed subscheme

↑ **Parent:** [Closed subscheme](#closed-subscheme)

For a [closed subscheme](#closed-subscheme) defined by an [ideal sheaf](#ideal-sheaf-of-a-closed-subscheme) $\mathcal I$, its $n$th [infinitesimal neighbourhood](#infinitesimal-neighbourhood-of-a-closed-subscheme) has structure sheaf $\mathcal O_X/\mathcal I^{n+1}$. All these neighbourhoods have the same underlying topological space because the radicals of $\mathcal I$ and its positive powers agree. Their [inverse limit](module-theory.md#inverse-limit) of structure sheaves is the [formal completion of a scheme](#formal-completion-of-a-scheme).

// Target: ringed-space.bigb

###### Projective complete intersection

↑ **Parent:** [Closed subscheme](#closed-subscheme)

A projective complete intersection is a [closed subscheme](#closed-subscheme) of a [projective space](projective-space.md) defined by a homogeneous [regular sequence](commutative-algebra.md#regular-sequence) of positive degrees. A length-$r$ sequence in $k[t_0,\ldots,t_N]$ gives dimension $N-r$ when $r\le N$. Sheafifying its successive quotient sequences gives exact restriction sequences of [twisting sheaves on projective space](sheaf-of-modules.md#twisting-sheaf-on-projective-space), allowing computation of its [sheaf cohomology](sheaf-of-modules.md#sheaf-cohomology). It need not be smooth or reduced.

###### Unmixedness of a complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

A [projective complete intersection](#projective-complete-intersection) defined by a [regular sequence](commutative-algebra.md#regular-sequence) in a [polynomial ring](commutative-algebra.md#polynomial-ring) has pure codimension equal to the sequence length and has no embedded [associated primes](module-theory.md#associated-prime-of-a-module). Thus its components account for the whole degree, with their generic multiplicities. This fact excludes hidden embedded points when a contained curve already has the full intersection degree.

###### Global regular functions on a positive-dimensional projective complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

For a length-$r$ homogeneous regular sequence of positive degrees in $\mathbb P^N_k$, with $r<N$, the [global regular functions](#global-regular-function) on its [projective complete intersection](#projective-complete-intersection) are exactly $k$. In the successive restriction sequences, [intermediate cohomology vanishing for a projective complete intersection](#intermediate-cohomology-vanishing-for-a-projective-complete-intersection) makes the first-cohomology group on the preceding stage zero. Inductively all negative twists have zero global sections, so at twist zero the restriction of constants is an isomorphism. The positive-dimension assumption is essential: a zero-dimensional complete intersection can have more global functions, including nilpotents.

###### Intermediate cohomology vanishing for a projective complete intersection

↑ **Parent:** [Projective complete intersection](#projective-complete-intersection)

For a length-$r$ [projective complete intersection](#projective-complete-intersection) $X_r\subseteq\mathbb P^N_k$, the groups $H^q(X_r,\mathcal O_{X_r}(m))$ vanish for every integer $m$ and $0<q<N-r$. Starting with [cohomology of twisting sheaves on projective space](projective-space.md#cohomology-of-twisting-sheaves-on-projective-space), induct through $0\to\mathcal O_{X_{j-1}}(m-d_j)\to\mathcal O_{X_{j-1}}(m)\to\mathcal O_{X_j}(m)\to0$. Both adjacent groups in the [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology) vanish precisely in the indicated range.

###### Construction of a closed subscheme from a quasi-coherent ideal

↑ **Parent:** [Closed subscheme](#closed-subscheme)

A [quasi-coherent sheaf](sheaf-of-modules.md#quasi-coherent-sheaf) of ideals $\mathcal I\subseteq\mathcal O_X$ gives a [closed subscheme](#closed-subscheme) by gluing $\operatorname{Spec}(A/J)$ on [affine open subschemes](#affine-open-subscheme) where $\mathcal I=\widetilde J$. Compatibility follows from [exactness of localization](commutative-algebra.md#exactness-of-localization). On the closed set $Z=\{x:\mathcal I_x\ne\mathcal O_{X,x}\}$, the [structure sheaf](#structure-sheaf-of-a-scheme) is $i^{-1}(\mathcal O_X/\mathcal I)$, where $i:Z\hookrightarrow X$ is the inclusion. Its pushforward is $\mathcal O_X/\mathcal I$.

###### Ideal sheaf of a closed subscheme

↑ **Parent:** [Closed subscheme](#closed-subscheme)

For a [closed immersion](#closed-immersion) $i:Z\hookrightarrow X$, the ideal sheaf is the kernel $\mathcal I_{Z/X}=\ker(\mathcal O_X\to i_*\mathcal O_Z)$. It therefore fits into the [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\longrightarrow\mathcal I_{Z/X}\longrightarrow\mathcal O_X\longrightarrow i_*\mathcal O_Z\longrightarrow0.
$$

###### Ideal sheaf of a closed point

↑ **Parent:** [Ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme)

For a [closed point](topology.md#closed-point) $P$ with residue field $k(P)$, evaluation gives a morphism from the [structure sheaf](#structure-sheaf-of-a-scheme) onto the [skyscraper sheaf](sheaf-of-modules.md#skyscraper-sheaf) $k_P$. Its [kernel](kernel-of-a-linear-map.md) is the ideal sheaf of $P$. On a [Noetherian scheme](#noetherian-scheme) it is a [coherent ideal sheaf](sheaf-of-modules.md#coherent-ideal-sheaf).

###### Ideal sheaf of two closed points

↑ **Parent:** [Ideal sheaf of a closed point](#ideal-sheaf-of-a-closed-point)

For distinct [closed points](topology.md#closed-point) over an [algebraically closed field](algebra.md#algebraically-closed-field), evaluation gives the [short exact sequence](module-theory.md#short-exact-sequence) $0\to\mathcal I_{\{P,Q\}}\to\mathcal O_X\to k_P\oplus k_Q\to0$. If all global [regular functions](#regular-function) are constant, the [long exact sequence in sheaf cohomology](sheaf-of-modules.md#long-exact-sequence-in-sheaf-cohomology) embeds $k^2/k(1,1)$ into $H^1(X,\mathcal I_{\{P,Q\}})$. Thus this ideal detects a concrete obstruction to affineness.

###### Rank bound for locally free ideals on reduced schemes

↑ **Parent:** [Ideal sheaf of a closed subscheme](#ideal-sheaf-of-a-closed-subscheme)

A finite [locally free sheaf](sheaf-of-modules.md#locally-free-sheaf) of ideals on a [reduced scheme](#reduced-scheme) has rank at most one at every point. On a nonempty [affine open subscheme](#affine-open-subscheme) where its rank is $r$, localize its inclusion into the structure sheaf at a [minimal prime ideal](commutative-algebra.md#minimal-prime-ideal). The resulting [local ring](commutative-algebra.md#local-ring) is a field $K$, giving an injection $K^r\hookrightarrow K$, hence $r\le1$. This works without a Noetherian assumption. The empty scheme is a vacuous exception to claims phrased as nonexistence of a sheaf of a prescribed rank.

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

### Affine plane with doubled origin

↑ **Parent:** [Scheme](#scheme)

The affine plane with doubled origin is formed by gluing two copies of $\mathbb A_k^2$ by the identity away from the origin. The overlap is the [punctured affine plane](#punctured-affine-plane), so this scheme is nonseparated and the two-open affine cover is not acyclic for the structure sheaf.

The gluing resembles a [non-Hausdorff manifold](topology.md#non-hausdorff-manifold) example, but this node concerns an algebraic scheme and its nonseparatedness, not a real manifold.

### Semi-separated scheme

↑ **Parent:** [Scheme](#scheme)

A scheme is semi-separated when the intersection of any two affine open subsets is affine, equivalently when its diagonal is affine. This condition makes affine covers acyclic for quasi-coherent sheaves.

#### Exact direct image from an affine open in a semi-separated scheme

↑ **Parent:** [Semi-separated scheme](#semi-separated-scheme)

If $U$ is an [affine open subscheme](#affine-open-subscheme) of a [semi-separated scheme](#semi-separated-scheme), its [open immersion](#open-immersion) $j:U\hookrightarrow X$ has exact [direct image](sheaf-of-modules.md#direct-image-sheaf) on [quasi-coherent sheaves](sheaf-of-modules.md#quasi-coherent-sheaf). Test on an affine open $V$ of $X$: the intersection $U\cap V$ is affine, and the [affine module-sheaf equivalence](sheaf-of-modules.md#affine-module-sheaf-equivalence) makes sections on this intersection exact. The direct image is also quasi-coherent, since this open immersion is an [affine morphism](#affine-morphism).

## ↑ Ancestors (6)

1. [Ringed space](ringed-space.md)
2. [Algebraic geometry](algebraic-geometry.md)
3. [Geometry and topology](geometry-and-topology.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Formal scheme](#formal-scheme)
- [Gluing of schemes along open subschemes](#gluing-of-schemes-along-open-subschemes)
- [Morphism of schemes](#morphism-of-schemes)
- [Open immersion](#open-immersion)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-16.md#1/solution)
- [Scheme](#scheme)
