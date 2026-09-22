# Functor

↑ **Parent:** [Category](category.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functor)

A functor assigns an [object of a category](category.md#object-of-a-category) $F(A)$ to each object $A$ and a [categorical morphism](category.md#morphism-in-a-category) $F(f):F(A)\to F(B)$ to each arrow $f:A\to B$. It preserves the rules for composing arrows:

$$
F(1_A)=1_{F(A)},\qquad F(g\circ f)=F(g)\circ F(f).
$$

For example, the [forgetful functor](#forgetful-functor) from the [category of groups](category-theory.md#category-of-groups) to the [Category of sets](category.md#category-of-sets) keeps the underlying [sets](set.md) and maps of elements while forgetting the group operations. A [group homomorphism](group-theory.md#group-homomorphism) remains a [function](function.md), and composing the underlying [functions](function.md) gives the underlying map of the composite [group homomorphism](group-theory.md#group-homomorphism).

Another example sends a [set](set.md) $X$ to its [power set](set.md#power-set) $\mathcal P(X)$. It sends a [function](function.md) $f:X\to Y$ to the [function](function.md) $\mathcal P(f):\mathcal P(X)\to\mathcal P(Y)$ defined by $S\mapsto f(S)$, the [image](set-theory.md#image-of-a-function) of the [subset](set.md#subset) $S$. For $f(x)=x+1$ and $g(x)=2x$, the subset $\{0,2\}$ goes to $\{1,3\}$ and then $\{2,6\}$; applying the composite $g\circ f$ directly also gives $\{2,6\}$. The equality of these routes expresses preservation of [composition in a category](category.md#composition-in-a-category).

**Table of contents**

- [Bifunctor](#bifunctor)
- [Discrete opfibration](#discrete-opfibration)
  - [Connected components of discrete-opfibration pullbacks](#connected-components-of-discrete-opfibration-pullbacks)
- [Full functor](#full-functor)
- [Flat functor](#flat-functor)
  - [Flat functor and finite-limit preservation](#flat-functor-and-finite-limit-preservation)
- [Kan extension](#kan-extension)
- [Finite-limit-preserving functor](#finite-limit-preserving-functor)
  - [Regular functor](#regular-functor)
- [Conservative functor](#conservative-functor)
- [Limit-reflecting functor](#limit-reflecting-functor)
  - [Limits reflected by full and faithful functors](#limits-reflected-by-full-and-faithful-functors)
  - [Limit-creating functor](#limit-creating-functor)
    - [Creation of limits up to isomorphism](#creation-of-limits-up-to-isomorphism)
- [Colimit-preserving functor](#colimit-preserving-functor)
- [Limit-preserving functor](#limit-preserving-functor)
  - [Equalizer preservation by pullback-preserving functors](#equalizer-preservation-by-pullback-preserving-functors)
- [Forgetful functor](#forgetful-functor)
- [Endofunctor](#endofunctor)
  - [Comonad](#comonad)
    - [Cartesian comonad](#cartesian-comonad)
    - [Idempotent comonad](#idempotent-comonad)
    - [Coalgebra for a comonad](#coalgebra-for-a-comonad)
      - [Category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad)
        - [Cartesian closure for a finite-limit-preserving comonad](#cartesian-closure-for-a-finite-limit-preserving-comonad)
        - [Subobject classifier of a coalgebra topos](#subobject-classifier-of-a-coalgebra-topos)
        - [Exponentials in a coalgebra topos](#exponentials-in-a-coalgebra-topos)
        - [Cofree coalgebra](#cofree-coalgebra)
- [Finite-limit-preserving set-valued functor](#finite-limit-preserving-set-valued-functor)
- [Equivalence of categories](#equivalence-of-categories)
  - [Essential surjectivity](#essential-surjectivity)
  - [Isomorphism of categories](#isomorphism-of-categories)
- [Functor category](#functor-category)
  - [Pointwise monomorphism in a set-valued functor category](#pointwise-monomorphism-in-a-set-valued-functor-category)
  - [Pointwise limits in a functor category](#pointwise-limits-in-a-functor-category)
  - [Constant diagram functor](#constant-diagram-functor)
    - [Adjoints to constant presheaves on open sets](#adjoints-to-constant-presheaves-on-open-sets)
      - [Five adjoints for constant presheaves on open sets](#five-adjoints-for-constant-presheaves-on-open-sets)
  - [Presheaf (category theory)](#presheaf-category-theory)
  - [Presheaf category](#presheaf-category)
    - [Canonical colimit presentation of a presheaf](#canonical-colimit-presentation-of-a-presheaf)
    - [Free cocompletion](#free-cocompletion)
    - [Grothendieck topology](#grothendieck-topology)
      - [Double-negation topology](#double-negation-topology)
        - [Separating tower site with vanishing product](#separating-tower-site-with-vanishing-product)
      - [Zariski coverage on finitely presented rings](#zariski-coverage-on-finitely-presented-rings)
      - [Coverage on a category](#coverage-on-a-category)
        - [Rigid coverage](#rigid-coverage)
        - [J-irreducible object of a site](#j-irreducible-object-of-a-site)
      - [Site (category theory)](#site-category-theory)
      - [Atomic topology](#atomic-topology)
        - [Atomic finite-surjection site](#atomic-finite-surjection-site)
          - [Primitive element of an atomic finite-surjection sheaf](#primitive-element-of-an-atomic-finite-surjection-sheaf)
            - [Primitive decomposition of an atomic finite-surjection sheaf](#primitive-decomposition-of-an-atomic-finite-surjection-sheaf)
            - [Primitive-element kernel rigidity lemma](#primitive-element-kernel-rigidity-lemma)
          - [Descent identities for the atomic finite-surjection site](#descent-identities-for-the-atomic-finite-surjection-site)
        - [Common-refinement condition for nonempty-sieve coverage](#common-refinement-condition-for-nonempty-sieve-coverage)
      - [Subcanonical topology](#subcanonical-topology)
      - [Sheaf on a site](#sheaf-on-a-site)
    - [Sieve (category theory)](#sieve-category-theory)
      - [Dense sieve](#dense-sieve)
      - [J-closed sieve](#j-closed-sieve)
    - [Presheaf topos](#presheaf-topos)
      - [Slice-small presheaf construction](#slice-small-presheaf-construction)
      - [Exponential in a presheaf category](#exponential-in-a-presheaf-category)
  - [Arrow category](#arrow-category)
    - [Adjoint chain for evaluation in an arrow category](#adjoint-chain-for-evaluation-in-an-arrow-category)
    - [Category of injective functions](#category-of-injective-functions)
  - [Representable functor](#representable-functor)
    - [Representable retract criterion](#representable-retract-criterion)
    - [Representability from a solution set](#representability-from-a-solution-set)
    - [Left adjoint to a covariant representable functor](#left-adjoint-to-a-covariant-representable-functor)
    - [Covariant representables preserve limits](#covariant-representables-preserve-limits)
    - [Colimit criterion for representability of a presheaf](#colimit-criterion-for-representability-of-a-presheaf)
      - [Small-limit preservation is insufficient for the large elements-colimit criterion](#small-limit-preservation-is-insufficient-for-the-large-elements-colimit-criterion)
    - [Canonical colimit presentation of a covariant set-valued functor](#canonical-colimit-presentation-of-a-covariant-set-valued-functor)
    - [Representation of a functor](#representation-of-a-functor)
      - [Uniqueness of functor representations](#uniqueness-of-functor-representations)
      - [Functoriality of chosen representations](#functoriality-of-chosen-representations)
      - [Universal element of a set-valued functor](#universal-element-of-a-set-valued-functor)
    - [Yoneda lemma](#yoneda-lemma)
      - [Density formula for presheaves](#density-formula-for-presheaves)
      - [Yoneda embedding](#yoneda-embedding)
        - [Yoneda embedding detects split epimorphisms](#yoneda-embedding-detects-split-epimorphisms)
        - [Yoneda embedding preserves exponentials](#yoneda-embedding-preserves-exponentials)
        - [Covariant Yoneda embedding](#covariant-yoneda-embedding)
  - [Pointwise epimorphism in a functor category](#pointwise-epimorphism-in-a-functor-category)
    - [Pushout witness for failure of pointwise surjectivity](#pushout-witness-for-failure-of-pointwise-surjectivity)
- [Monofunctor](#monofunctor)
- [Natural transformation](#natural-transformation)
  - [Dinatural transformation](#dinatural-transformation)
  - [Natural isomorphism](#natural-isomorphism)
    - [Natural bijection](#natural-bijection)
  - [Naturality](#naturality)
- [Full and faithful functor](#full-and-faithful-functor)
- [Faithful functor](#faithful-functor)

## Bifunctor

↑ **Parent:** [Functor](functor.md)

A [bifunctor](#bifunctor) is a [functor](functor.md) on the product of two [categories](category.md). It assigns $F(c,d)$ to each pair of objects and $F(u,v)$ to a pair of [morphisms](algebra.md#morphism), preserving [identity morphisms](algebra.md#identity-morphism) and [composition in a category](category.md#composition-in-a-category). Equivalently, it is functorial separately in each argument, with the two actions commuting: $F(1,v)F(u,1)=F(u,1)F(1,v)$ whenever the expressions have the corresponding sources and targets. The product [category](category.md) has pairs as objects, pairs of [morphisms](algebra.md#morphism) as arrows, and componentwise [composition in a category](category.md#composition-in-a-category). A [monoidal tensor product](category-theory.md#monoidal-tensor-product) is a [bifunctor](#bifunctor) from a [category](category.md) times itself.

## Discrete opfibration

↑ **Parent:** [Functor](functor.md)

A [functor](functor.md) with a unique lift, from each specified object $c$, of every arrow $Fc\to d$. The lifted arrow's target is part of the uniqueness requirement. This is dual to a [discrete fibration](category.md#discrete-fibration). Lifting a [cocone](category.md#cocone-under-a-diagram) of a finite [connected category](category.md#connected-category) gives a cocone upstairs: lifts of its legs have a common target because uniqueness identifies targets along every diagram arrow. Thus a discrete opfibration over a [weakly filtered category](category.md#weakly-filtered-category) has weakly filtered domain, including the possibility of an empty domain.

### Connected components of discrete-opfibration pullbacks

↑ **Parent:** [Discrete opfibration](#discrete-opfibration)

For [discrete opfibrations](#discrete-opfibration) $A\to D\leftarrow B$ with [weakly filtered categories](category.md#weakly-filtered-category), the map taking a pair to its [connected components of a category](category.md#connected-component-of-a-category) is a [bijection](function.md#bijection). For surjectivity, send two base objects in the same component to a common target and lift both arrows. For injectivity, choose common targets upstairs for two representatives; a cocone over the resulting finite connected diagram downstairs makes their lifted composites agree. Hence the representatives have a common target in the [pullback in a category](category.md#pullback-category-theory). Over a [filtered category](category.md#filtered-category), the component functor on the slice of discrete opfibrations preserves all finite [categorical limits](category.md#categorical-limit): it preserves pullbacks and takes the terminal object to a singleton.

## Full functor

↑ **Parent:** [Functor](functor.md)

A [functor](functor.md) $F:\mathcal C\to\mathcal D$ is full when each function $\mathcal C(A,B)\to\mathcal D(FA,FB)$ is surjective. It is a [faithful functor](#faithful-functor) when each is injective. A [full and faithful functor](#full-and-faithful-functor) identifies its source, up to equivalence, with a [full subcategory](category.md#full-subcategory) of the target. Fullness only concerns morphisms between image objects; it does not require every target object to lie in the image.

## Flat functor

↑ **Parent:** [Functor](functor.md)

A covariant [functor](functor.md) into a [Grothendieck topos](category-theory.md#grothendieck-topos) is flat when its tensor extension from presheaves preserves [finite limits](category.md#finite-limit). For set values, its [category of elements](category.md#category-of-elements) with arrows carrying source elements to target elements is cofiltered; equivalently the [functor](functor.md) is a filtered [colimit](category.md#colimit) of covariant representables. If the indexing category has [finite limits](category.md#finite-limit), flatness is equivalent to preservation of [finite limits](category.md#finite-limit). For a [site](#site-category-theory), cover-to-joint-epimorphism continuity adds the condition needed by the [Diaconescu equivalence for geometric morphisms](category-theory.md#diaconescu-equivalence-for-geometric-morphisms).

### Flat functor and finite-limit preservation

↑ **Parent:** [Flat functor](#flat-functor)

For a [small category](category.md#small-category) with [finite limits](category.md#finite-limit), a set-valued [functor](functor.md) preserving them has a [category of elements](category.md#category-of-elements) with finite limits, so its opposite is a [filtered category](category.md#filtered-category). The [covariant density presentation](category.md#covariant-density-presentation) is therefore a filtered [colimit](category.md#colimit) of [representable functors](#representable-functor). Conversely, representable functors preserve [categorical limits](category.md#categorical-limit), and [filtered colimits commute with finite limits in sets](category.md#filtered-colimits-commute-with-finite-limits-in-sets), proving the criterion.

## Kan extension

↑ **Parent:** [Functor](functor.md)

A [left Kan extension](category.md#left-kan-extension) is [left adjoint](category.md#adjoint-functors) to precomposition, when it exists; a [Right Kan extension](category.md#right-kan-extension) is [right adjoint](category.md#adjoint-functors). For small indexing categories and set-valued [functors](functor.md), both exist by comma-category [colimit](category.md#colimit) and limit formulas. These two adjoints give the [essential geometric morphism](category-theory.md#essential-geometric-morphism) induced by a [functor](functor.md) between presheaf indexing categories.

## Finite-limit-preserving functor

↑ **Parent:** [Functor](functor.md)

A finite-limit-preserving functor preserves a terminal object and pullbacks, equivalently all finite limits. It is also called left exact. Such functors from a [Cartesian syntactic category](mathematical-logic.md#cartesian-syntactic-category) to a finite-limit category correspond to models of the associated [Cartesian theory](mathematical-logic.md#cartesian-theory).

### Regular functor

↑ **Parent:** [Finite-limit-preserving functor](#finite-limit-preserving-functor)

A [functor](functor.md) between [regular categories](category.md#regular-category) is regular if it preserves [finite limits](category.md#finite-limit) and [regular epimorphisms](category.md#regular-epimorphism). It then preserves [image factorizations](category.md#image-factorization), since finite-limit preservation preserves [monomorphisms](category.md#monomorphism). A [representable functor](#representable-functor) $\mathcal C(P,-)$ is regular exactly when $P$ is projective with respect to regular epimorphisms. Regularity of a functor does not alone imply faithfulness or reflection of isomorphisms.

## Conservative functor

↑ **Parent:** [Functor](functor.md)

A [functor](functor.md) is conservative when it reflects [isomorphisms](algebra.md#isomorphism): if $F(f)$ is invertible then $f$ is invertible. It need not be full or [faithful functor](#faithful-functor). The [crude monadicity theorem](category-theory.md#crude-monadicity-theorem) uses this reflection property to lift invertibility of the comparison-adjunction counit from the base [category](category.md).

## Limit-reflecting functor

↑ **Parent:** [Functor](functor.md)

For a specified diagram shape, a [functor](functor.md) reflects [categorical limits](category.md#categorical-limit) when a [cone over a diagram](category.md#cone-over-a-diagram) is limiting whenever its image is limiting. This condition tests an existing [categorical cone](category.md#cone-over-a-diagram). It does not assert that every limiting [categorical cone](category.md#cone-over-a-diagram) in the codomain has a lift.

### Limits reflected by full and faithful functors

↑ **Parent:** [Limit-reflecting functor](#limit-reflecting-functor)

A [full and faithful functor](#full-and-faithful-functor) reflects every existing shape of [categorical limit](category.md#categorical-limit). If the image of a cone is limiting, apply its universal property to the image of any competing cone. Fullness lifts the unique mediating morphism; faithfulness proves the cone equations and uniqueness of the lift. No essential-surjectivity hypothesis is needed.

### Limit-creating functor

↑ **Parent:** [Limit-reflecting functor](#limit-reflecting-functor)

A [functor](functor.md) creates [categorical limits](category.md#categorical-limit) of a specified shape when every given limiting [categorical cone](category.md#cone-over-a-diagram) over an image diagram uniquely lifts to a [categorical cone](category.md#cone-over-a-diagram) over the original diagram, and the lift is limiting. This is stronger than just being a [limit-reflecting functor](#limit-reflecting-functor). Forgetting arrows from a [functor category](#functor-category) creates its [pointwise limits in a functor category](#pointwise-limits-in-a-functor-category).

#### Creation of limits up to isomorphism

↑ **Parent:** [Limit-creating functor](#limit-creating-functor)

An equivalence-invariant lifting property permits the underlying cone of the lift to be identified with the chosen cone by an isomorphism, rather than requiring literal equality. Lifts are unique up to a unique isomorphism compatible with that identification. A [monadic adjunction](category-theory.md#monadic-adjunction) defined by equivalence of its comparison functor has this property by [monad algebra forgetful functor creates limits](category-theory.md#monad-algebra-forgetful-functor-creates-limits). Literal creation follows if the comparison is an isomorphism over the base, or suitable strict transport of objects is part of the convention. An equivalence alone does not guarantee a literally prescribed underlying object lies in the image.

## Colimit-preserving functor

↑ **Parent:** [Functor](functor.md)

Relative to a specified class of diagram shapes, a functor preserves colimits when it takes each existing [colimit](category.md#colimit) cocone of those shapes to a [colimit](category.md#colimit) cocone. A [left adjoint](category.md#adjoint-functors) preserves all existing colimits, including large ones when their universal properties are meaningful. Small-colimit preservation alone does not imply preservation of a class-indexed colimit.

## Limit-preserving functor

↑ **Parent:** [Functor](functor.md)

Relative to a specified class of diagram shapes, a functor preserves limits when it takes each existing [categorical limit](category.md#categorical-limit) cone of those shapes to a [categorical limit](category.md#categorical-limit) cone. The usual completeness and [general adjoint functor theorem](category.md#freyd-general-adjoint-functor-theorem) hypotheses refer to small shapes; a possibly large diagram requires an explicit preservation hypothesis covering its shape.

### Equalizer preservation by pullback-preserving functors

↑ **Parent:** [Limit-preserving functor](#limit-preserving-functor)

If $\mathcal C$ has finite [categorical limits](category.md#categorical-limit), every [functor](functor.md) $F:\mathcal C\to\mathcal D$ preserving [pullbacks in a category](category.md#pullback-category-theory) also preserves [equalizers](category.md#equaliser), even when it does not preserve a [terminal object](category.md#terminal-object). Factor it through the [slice category](category.md#slice-category) $\mathcal D/F1$ by sending $A$ to $F(A\to1)$. This lifted functor preserves pullbacks because the slice [forgetful functor](#forgetful-functor) reflects them; it also preserves the terminal object, so it preserves finite limits. The slice forgetful functor preserves equalizers, completing the proof.

## Forgetful functor

↑ **Parent:** [Functor](functor.md)

A [functor](functor.md) discarding some structure, for example an action on a [module](module-theory.md#module-mathematics). It need not be full or faithful in general.

## Endofunctor

↑ **Parent:** [Functor](functor.md)

An endofunctor is a [functor](functor.md) from a [category](category.md) to itself. A [monad](category-theory.md#monad) adds a unit and multiplication to an endofunctor, satisfying the unit and associativity laws.

### Comonad

↑ **Parent:** [Endofunctor](#endofunctor)

A comonad is an [endofunctor](#endofunctor) $G$ with [natural transformations](#natural-transformation) $\epsilon:G\to1$ and $\delta:G\to G^2$ satisfying $G\epsilon\,\delta=\epsilon_G\delta=1_G$ and $G\delta\,\delta=\delta_G\delta$. It is the categorical dual of a [monad](category-theory.md#monad). Its [coalgebras for a comonad](#coalgebra-for-a-comonad) carry compatible maps into their image under $G$.

#### Cartesian comonad

↑ **Parent:** [Comonad](#comonad)

In the finite-limit setting, a Cartesian comonad is a [comonad](#comonad) whose underlying endofunctor preserves [finite limits](category.md#finite-limit). Its [category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad) has finite limits created by the [forgetful functor](#forgetful-functor). On an [elementary topos](category-theory.md#elementary-topos), equalizer constructions of [exponentials in a coalgebra topos](#exponentials-in-a-coalgebra-topos) and the [subobject classifier of a coalgebra topos](#subobject-classifier-of-a-coalgebra-topos) make that coalgebra category an elementary topos.

#### Idempotent comonad

↑ **Parent:** [Comonad](#comonad)

A [comonad](#comonad) is idempotent when its comultiplication $G\to G^2$ is invertible. Its coalgebra category identifies with the [coreflective subcategory](category.md#coreflective-subcategory) of objects on which the counit is invertible. A coreflective inclusion produces such a comonad.

#### Coalgebra for a comonad

↑ **Parent:** [Comonad](#comonad)

For a [comonad](#comonad), a coalgebra is a map $a:A\to GA$ satisfying $\epsilon_Aa=1_A$ and $\delta_Aa=Ga\,a$. A morphism $f:(A,a)\to(B,b)$ obeys $bf=Gf\,a$. This is distinct from the tensor-based notion of a [coalgebra](multilinear-algebra.md#coalgebra) in algebra.

##### Category of coalgebras for a comonad

↑ **Parent:** [Coalgebra for a comonad](#coalgebra-for-a-comonad)

The category $\mathcal E^G$ consists of [coalgebras for a comonad](#coalgebra-for-a-comonad) and their structure-preserving morphisms. Its [forgetful functor](#forgetful-functor) has the [cofree coalgebra](#cofree-coalgebra) as right adjoint. If $\mathcal E$ is a [topos](category-theory.md#elementary-topos) and $G$ preserves [finite limits](category.md#finite-limit), those limits are created by the forgetful functor, while [exponentials in a coalgebra topos](#exponentials-in-a-coalgebra-topos) and the [subobject classifier of a coalgebra topos](#subobject-classifier-of-a-coalgebra-topos) can be constructed as equalizers inside cofree objects.

###### Cartesian closure for a finite-limit-preserving comonad

↑ **Parent:** [Category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad)

Let $G$ be a [Cartesian comonad](#cartesian-comonad) on a [Cartesian category](category.md#cartesian-category) that is [Cartesian closed](category.md#cartesian-closed-category). Its [forgetful functor](#forgetful-functor) creates finite limits. For coalgebras $(A,a)$ and $(B,b)$, set $D=B^A$, $W=(GB)^A$. Transpose $G D\times A\xrightarrow{1\times a}GD\times GA\cong G(D\times A)\xrightarrow{G\operatorname{ev}}GB$ to $q:GD\to W$, and put $p=b^A\epsilon_D:GD\to W$. Their [cofree coalgebra](#cofree-coalgebra) transposes $Gp\delta_D,Gq\delta_D:R(D)\rightrightarrows R(W)$ have a coalgebra equalizer. A map into this equalizer is exactly a map $C\times A\to B$ respecting coalgebra structures, so it is the required [exponential object](category.md#exponential-object). No subobject classifier on the base category is needed.

###### Subobject classifier of a coalgebra topos

↑ **Parent:** [Category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad)

Let $\kappa:G\Omega\to\Omega$ classify $G\top:1\hookrightarrow G\Omega$. In the [cofree coalgebra](#cofree-coalgebra) $R\Omega$, equalize the identity and $G\kappa\,\delta_\Omega$. A map $\chi:X\to\Omega$ classifies a subcoalgebra exactly when $\chi=\kappa G\chi\,x$, since this says the subobject equals the inverse image of its image under $G$. Transposition gives precisely the displayed equalizer condition.

###### Exponentials in a coalgebra topos

↑ **Parent:** [Category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad)

For a finite-limit-preserving [comonad](#comonad) on a [topos](category-theory.md#elementary-topos), start with the cofree coalgebra on the ambient exponential $B^A$. Its underlying evaluation is $e=\operatorname{ev}(\epsilon\times1)$. Transpose the two expressions $be$ and $Ge(\delta\times a)$ first using the ambient exponential and then the cofree adjunction. Their coalgebra equalizer represents exactly the maps whose evaluations respect coalgebra structure. Thus coalgebra exponentials need not be the underlying ambient exponentials.

###### Cofree coalgebra

↑ **Parent:** [Category of coalgebras for a comonad](#category-of-coalgebras-for-a-comonad)

For a [comonad](#comonad), the cofree coalgebra on $X$ is $(GX,\delta_X)$. A map $UA\to X$ transposes to the coalgebra morphism $Gf\,a:A\to GX$. This gives the [adjunction](category.md#adjoint-functors) $U\dashv R$ with the [forgetful functor](#forgetful-functor).

## Finite-limit-preserving set-valued functor

↑ **Parent:** [Functor](functor.md)

A [functor](functor.md) $F:\mathcal C\to\mathbf{Set}$ is finite-limit-preserving if it carries each [finite limit](category.md#finite-limit) cone to a limiting cone. When $\mathcal C$ is a [small category](category.md#small-category) with [finite limits](category.md#finite-limit), this is equivalent to $F$ being a [filtered colimit in a category](category.md#filtered-colimit-in-a-category) of covariant [representable functors](#representable-functor), and to the opposite of its [category of elements](category.md#category-of-elements) being a [filtered category](category.md#filtered-category). It is also equivalent to every [comma category](category.md#comma-category) $(S\downarrow F)$ having [finite limits](category.md#finite-limit), for all sets $S$.

## Equivalence of categories

↑ **Parent:** [Functor](functor.md)

An equivalence consists of [functors](functor.md) $F:\mathcal C\to\mathcal D$ and $G:\mathcal D\to\mathcal C$ with [natural transformation](#natural-transformation) isomorphisms $GF\cong1_{\mathcal C}$ and $FG\cong1_{\mathcal D}$. A [full and faithful functor](#full-and-faithful-functor) which is essentially surjective, meaning every target object is isomorphic to an image object, is part of an equivalence under the usual choice convention. An isomorphism of categories is stronger: it has a strictly inverse functor.

### Essential surjectivity

↑ **Parent:** [Equivalence of categories](#equivalence-of-categories)

A [functor](functor.md) $F:\mathcal C\to\mathcal D$ is essentially surjective when every object of $\mathcal D$ is isomorphic to $FA$ for some $A\in\mathcal C$. Together with [full and faithful](#full-and-faithful-functor), this characterizes an [equivalence of categories](#equivalence-of-categories) under the appropriate [axiom of choice](set-theory.md#axiom-of-choice) convention. For large categories, choosing a quasi-inverse on all objects requires a universe or a class-choice convention.

### Isomorphism of categories

↑ **Parent:** [Equivalence of categories](#equivalence-of-categories)

An isomorphism of [categories](category.md) is a [functor](functor.md) with a strictly inverse [functor](functor.md). It is equivalently bijective on objects and on each hom-set. An [equivalence of categories](#equivalence-of-categories) only requires inverse composites up to invertible [natural transformations](#natural-transformation). For example, the [category of partial functions](category.md#category-of-partial-functions) and the [category of pointed sets](category.md#category-of-pointed-sets) are equivalent but their actual object collections prevent an isomorphism: the former has one [zero object](category.md#zero-object), the empty [set](set.md), while the latter has distinct singleton [pointed set](set.md#pointed-set) objects that are all zero objects.

## Functor category

↑ **Parent:** [Functor](functor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functor_category)

The functor category has functors $\mathcal C\to\mathcal D$ as objects and natural transformations as morphisms.

### Pointwise monomorphism in a set-valued functor category

↑ **Parent:** [Functor category](#functor-category)

A [natural transformation](#natural-transformation) between [functors](functor.md) to the [Category of sets](category.md#category-of-sets) is a [monomorphism](category.md#monomorphism) in the [functor category](#functor-category) exactly when every component is an [injective function](algebra.md#injective-function). Componentwise cancellation proves sufficiency. For necessity, the [Yoneda lemma](#yoneda-lemma) converts two elements with equal component images into two transformations from a covariant [representable functor](#representable-functor); monicity cancels these transformations, forcing the elements to coincide. The argument remains valid for a [locally small category](category.md#locally-small-category) in an ambient universe where the functor category is formed.

### Pointwise limits in a functor category

↑ **Parent:** [Functor category](#functor-category)

For small diagrams with complete codomain, choose each objectwise [categorical limit](category.md#categorical-limit). For $u:d\to d'$, its projections uniquely define the arrow $L(u)$ through $p_j(d')L(u)=H_j(u)p_j(d)$. The [universal property](category-theory.md#universal-property) proves identity and composition laws. The same projection calculation makes every [categorical cone](category.md#cone-over-a-diagram) factorization a [natural transformation](#natural-transformation). Hence these are genuine [categorical limits](category.md#categorical-limit) in the [functor category](#functor-category), and the objectwise [forgetful functor](#forgetful-functor) is a [limit-creating functor](#limit-creating-functor).

### Constant diagram functor

↑ **Parent:** [Functor category](#functor-category)

The constant diagram functor sends $C$ to the [functor](functor.md) on $J$ with constant object value $C$ and identity arrow values; a morphism $f$ becomes the [natural transformation](#natural-transformation) with every component $f$. When all $J$-shaped [categorical limits](category.md#categorical-limit) exist, it is a [left adjoint](category.md#adjoint-functors) to the [limit functor](category.md#limit-functor).

#### Adjoints to constant presheaves on open sets

↑ **Parent:** [Constant diagram functor](#constant-diagram-functor)

For a [topological space](topology.md#topological-space) $S$, let $\Delta A$ be the [constant presheaf of sets](algebraic-geometry.md#constant-presheaf-of-sets) on its open-set category, with identity restriction maps, including the value at the empty open set. A [natural transformation](#natural-transformation) $P\to\Delta A$ is determined by its map $P(\varnothing)\to A$; its component at $U$ composes with $P(U)\to P(\varnothing)$. A transformation $\Delta A\to P$ is determined by $A\to P(S)$; its component at $U$ restricts sections from $S$. These two bijections prove the displayed [adjunctions](category.md#adjoint-functors). This concerns presheaves, so no sheafification is involved.

##### Five adjoints for constant presheaves on open sets

↑ **Parent:** [Adjoints to constant presheaves on open sets](#adjoints-to-constant-presheaves-on-open-sets)

For a nonempty [topological space](topology.md#topological-space) $S$, the [constant diagram functor](#constant-diagram-functor) on its open-set [presheaf category](#presheaf-category) lies in this five-term [adjunction](category.md#adjoint-functors) chain. The leftmost [functor](functor.md) sends $A$ to the [categorical presheaf](#presheaf-category-theory) equal to $A$ at the empty open set and empty elsewhere. The rightmost sends $A$ to the presheaf equal to $A$ at $S$ and a singleton elsewhere. A [natural transformation](#natural-transformation) from the former is determined by its empty-open component; a transformation into the latter is determined by its whole-space component. The middle [adjunctions](category.md#adjoint-functors) follow from restriction maps to the empty open set and from the whole space. Neither endpoint extends: the leftmost functor fails to preserve the [terminal object](category.md#terminal-object), and the rightmost fails to preserve the [initial object](category.md#initial-object).

### Presheaf (category theory)

↑ **Parent:** [Functor category](#functor-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Presheaf_(category_theory))

A presheaf on a [category](category.md) $\mathcal C$ is a [functor](functor.md) $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$. A [morphism](algebra.md#morphism) $f:C\to D$ induces the restriction map $X(f):X(D)\to X(C)$, reversing direction. The indexing [category](category.md) need not be small. For the [category](category.md) of open subsets of a [topological space](topology.md#topological-space), this specializes to a [presheaf of sets on a topological space](algebraic-geometry.md#presheaf-of-sets-on-a-topological-space).

### Presheaf category

↑ **Parent:** [Functor category](#functor-category)

The presheaf category on a [small category](category.md#small-category) $\mathcal C$ is the [functor category](#functor-category) $[\mathcal C^{\mathrm{op}},\mathbf{Set}]$. Its limits and colimits are computed pointwise.

Each object is a [presheaf on a category](#presheaf-category-theory), and its morphisms are [natural transformations](#natural-transformation).

#### Canonical colimit presentation of a presheaf

↑ **Parent:** [Presheaf category](#presheaf-category)

For a [categorical presheaf](#presheaf-category-theory) $P$ on a [small category](category.md#small-category), its [category of elements](category.md#category-of-elements) has objects $(c,x)$ with $x\in P(c)$ and arrows $u:(c,x)\to(d,y)$ satisfying $P(u)y=x$. The canonical [natural transformation](#natural-transformation) $H_c\to P$ sends $v:a\to c$ to $P(v)x$. These maps exhibit $P$ as the displayed [colimit](category.md#colimit). At $a$, a representative $(c,x,v)$ maps to $P(v)x$, with inverse $z\mapsto(a,z,1_a)$. The arrow $v:(a,P(v)x)\to(c,x)$ identifies every representative with its canonical inverse image, proving the bijection and the colimit universal property.

#### Free cocompletion

↑ **Parent:** [Presheaf category](#presheaf-category)

For a [small category](category.md#small-category) $\mathcal C$, its [presheaf category](#presheaf-category) is the free enlargement under small [colimits](category.md#colimit). Each [categorical presheaf](#presheaf-category-theory) $P$ is the colimit of the diagram sending $(C,x)\in\int P$ to the [representable presheaf](#representable-functor) $yC$. The map at $(C,x)$ sends $f:A\to C$ to $P(f)x$. It is surjective at each $A$ because $z\in P(A)$ is the image of $1_A$ at $(A,z)$. If two representatives have the same image $z$, they are both identified with the representative $1_A$ at $(A,z)$ by arrows in the [category of elements](category.md#category-of-elements), proving injectivity. Thus $P\cong\operatorname{colim}_{(C,x)\in\int P}yC$. For a cocomplete target, a functor on $\mathcal C$ extends by these colimits, uniquely up to natural isomorphism among colimit-preserving extensions.

#### Grothendieck topology

↑ **Parent:** [Presheaf category](#presheaf-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grothendieck_topology)

A Grothendieck topology assigns covering sieves to each object. The maximal sieve covers; pulling back a covering sieve gives a covering sieve; and a sieve locally covering along all arrows of a covering sieve itself covers. It defines the [sheaves on a site](#sheaf-on-a-site). Families of arrows generate sieves and can be used to generate the topology.

##### Double-negation topology

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

The dense sieves form the double-negation [Grothendieck topology](#grothendieck-topology). Its sheaf topos is a [Boolean topos](category-theory.md#boolean-topos): the union of a subobject with its pseudocomplement is dense and thus becomes the whole object after sheafification. This need not be the [atomic topology](#atomic-topology), which requires every nonempty sieve to be dense.

###### Separating tower site with vanishing product

↑ **Parent:** [Double-negation topology](#double-negation-topology)

Consider a site indexed by natural-number objects with arrows only downwards, the cancellation condition $fh=gk\Rightarrow f=g$ for equally typed $f,g$, and the separation condition that arrows $f:m\to n$, $g:m\to n+1$ admit $h,k:m+1\to m$ with $fh=fk$ but $gh\ne gk$. Its dense-sieve sheaf topos is a [Boolean topos](category-theory.md#boolean-topos) and a [two-valued topos](category-theory.md#two-valued-topos). The representables are separated. No nonempty partial map $y_n\to y_{n+1}$ exists, by the separation condition and naturality. The associated sheaves $A_n$ consequently admit no maps $y_n\to A_{n+1}$. Each has nonzero support and maps epimorphically to one, but their product has an empty value at every stage $m$, because its $A_{m+1}$ factor does.

##### Zariski coverage on finitely presented rings

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

On the opposite of the category of finitely presented unital [commutative rings](commutative-algebra.md#commutative-ring), a basic covering family is $A\to A[f_i^{-1}]$, where finitely many $f_i$ generate the [unit ideal](commutative-algebra.md#unit-ideal). Include the empty cover of the zero ring. Localization commutes with [base change](locally-ringed-space.md#base-change-of-a-morphism-of-schemes), so these families define a [coverage on a category](#coverage-on-a-category). Their [sheaf topos](category-theory.md#grothendieck-topos) classifies the [coherent theory of local rings](mathematical-logic.md#coherent-theory-of-local-rings). This coverage is subcanonical: representable functors obey the usual localization gluing equations.

##### Coverage on a category

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

A coverage specifies covering families on a [small category](category.md#small-category), stable under refinement along arrows: for a covering family into $C$ and $f:B\to C$, there is a covering family into $B$ whose composites with $f$ factor through the original family. Passing to generated sieves and imposing maximality and local transitivity gives its associated [Grothendieck topology](#grothendieck-topology), with the same [sheaves on a site](#sheaf-on-a-site). One can equivalently specify the saturated covering sieves directly. Rigidity refers to these covering sieves, so it is unchanged by replacing a family presentation by its generated topology.

###### Rigid coverage

↑ **Parent:** [Coverage on a category](#coverage-on-a-category)

A [coverage on a category](#coverage-on-a-category) is rigid when each object is covered by the sieve generated by arrows from [J-irreducible objects of a site](#j-irreducible-object-of-a-site). Restriction to their full subcategory identifies the [sheaves on a site](#sheaf-on-a-site) with its [presheaf category](#presheaf-category). A presheaf on that subcategory extends by the right Kan extension $C\mapsto\operatorname{Nat}(yC|_{\mathcal D},F)$: every covering sieve restricts to the full representable on $\mathcal D$, which proves the sheaf condition directly.

###### J-irreducible object of a site

↑ **Parent:** [Coverage on a category](#coverage-on-a-category)

An object of a [site](#site-category-theory) is J-irreducible when its only covering [sieve on a category](#sieve-category-theory) is the maximal sieve. In particular the empty sieve cannot cover it. Every arrow from a J-irreducible object belongs to any covering sieve on its codomain: the pulled-back sieve must contain the identity. This makes the induced topology on the full subcategory of J-irreducible objects trivial.

##### Site (category theory)

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

A [site](#site-category-theory) is a category equipped with a [Grothendieck topology](#grothendieck-topology), specifying which sieves are covering. The [sheaves on a site](#sheaf-on-a-site) satisfy unique amalgamation of matching families on those sieves. A small [site](#site-category-theory) presents a [Grothendieck topos](category-theory.md#grothendieck-topos).

##### Atomic topology

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

The atomic topology declares exactly the nonempty sieves covering. It exists precisely when arrows with a common codomain admit a common refinement. On nonempty finite sets and surjections this follows from the fiber product. Its J-closed sieves are only the empty and maximal sieves.

###### Atomic finite-surjection site

↑ **Parent:** [Atomic topology](#atomic-topology)

Use a small skeleton of nonempty finite sets and surjections, with every nonempty sieve covering. Fiber-product projections are surjections, so the atomic coverage exists. Surjections are effective quotients of their kernel pairs, making the site [subcanonical](#subcanonical-topology). Its sheaves admit the [primitive decomposition of an atomic finite-surjection sheaf](#primitive-decomposition-of-an-atomic-finite-surjection-sheaf).

###### Primitive element of an atomic finite-surjection sheaf

↑ **Parent:** [Atomic finite-surjection site](#atomic-finite-surjection-site)

An element $x\in F(n)$ is primitive if it does not descend along any surjection $n\to n-1$. All elements at cardinality one are primitive. Repeated descent reaches a primitive ancestor in finitely many steps, and the [primitive-element kernel rigidity lemma](#primitive-element-kernel-rigidity-lemma) makes the ancestor unique up to bijection.

###### Primitive decomposition of an atomic finite-surjection sheaf

↑ **Parent:** [Primitive element of an atomic finite-surjection sheaf](#primitive-element-of-an-atomic-finite-surjection-sheaf)

Partition the elements of a sheaf by their primitive-ancestor equivalence classes under bijection. Each class gives a sheaf subfunctor, because its membership is preserved and reflected along covering surjections. A representative primitive element names an epic representable map onto its class component. Thus every sheaf is the coproduct of these components, each an [atom in a topos](category-theory.md#atom-in-a-topos).

###### Primitive-element kernel rigidity lemma

↑ **Parent:** [Primitive element of an atomic finite-surjection sheaf](#primitive-element-of-an-atomic-finite-surjection-sheaf)

If primitive elements have equal restrictions along $\alpha:P\to m$ and $\beta:P\to n$, then these surjections have equal kernels. To rule out $\alpha(a)=\alpha(b)$ with unequal $\beta$ images, identify those two images by $q:n\to n-1$. The set of pairs equal under $\alpha$ and $q\beta$ maps surjectively both to $P$ by projection and to the kernel pair of $q$ by applying $\beta$. Injective restrictions force the kernel-pair matching condition on the primitive element, contradicting descent along $q$.

###### Descent identities for the atomic finite-surjection site

↑ **Parent:** [Atomic finite-surjection site](#atomic-finite-surjection-site)

For any sheaf $F$ and surjection $q:n\to k$, $F(k)\to F(n)\rightrightarrows F(n\times_kn)$ is an equalizer. In particular every $F(q)$ is injective. These follow from the sheaf condition on the sieve generated by the covering arrow $q$ and control primitive elements.

###### Common-refinement condition for nonempty-sieve coverage

↑ **Parent:** [Atomic topology](#atomic-topology)

For each pair $f:V\to U$, $g:W\to U$, require $fh=gk$ for some arrows $h:T\to V$, $k:T\to W$. This is necessary and sufficient for stability of nonempty sieves under pullback; the other topology axioms then follow. Nonempty finite sets with arbitrary functions fail it at distinct singleton-to-two-point maps.

##### Subcanonical topology

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

A Grothendieck topology is subcanonical when every [representable functor](#representable-functor) is a [sheaf on a site](#sheaf-on-a-site). It is also called standard in some topos-theory terminology. A nontrivial covering quotient can fail this condition by identifying distinct sections of a representable.

##### Sheaf on a site

↑ **Parent:** [Grothendieck topology](#grothendieck-topology)

A [categorical presheaf](#presheaf-category-theory) is a sheaf for $J$ if every matching family on a covering sieve has a unique amalgamation. Equivalently restriction $\operatorname{Nat}(yU,F)\to\operatorname{Nat}(S,F)$ is bijective for each covering sieve $S\hookrightarrow yU$. Sheaves on a small site form a [Grothendieck topos](category-theory.md#grothendieck-topos).

#### Sieve (category theory)

↑ **Parent:** [Presheaf category](#presheaf-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sieve_(category_theory))

A sieve on $U$ is a subfunctor of the [representable functor](#representable-functor) $yU$, equivalently a family of arrows into $U$ closed under precomposition. For $f:V\to U$, the pullback sieve consists of arrows $g$ into $V$ for which $fg$ belongs to the original sieve.

##### Dense sieve

↑ **Parent:** [Sieve (category theory)](#sieve-category-theory)

A sieve $R$ on $A$ is dense when every arrow $f:B\to A$ has a further composite $fh$ in $R$. Equivalently, every pullback sieve $f^*R$ is nonempty. This condition is stable under pullback and transitive refinement and defines the [double-negation topology](#double-negation-topology).

##### J-closed sieve

↑ **Parent:** [Sieve (category theory)](#sieve-category-theory)

A sieve is J-closed when membership is local with respect to the [Grothendieck topology](#grothendieck-topology) $J$. Pullback preserves J-closedness. Their presheaf is the [subobject classifier](category-theory.md#subobject-classifier) of the sheaf topos: a section of a sheaf is sent to the sieve of arrows on which it belongs to the chosen subsheaf.

#### Presheaf topos

↑ **Parent:** [Presheaf category](#presheaf-category)

Every [presheaf category](#presheaf-category) is a [topos](category-theory.md#elementary-topos). Finite limits are pointwise; the exponential is

$$
(G^F)(C)=\operatorname{Nat}(yC\times F,G),
$$

and the [subobject classifier](category-theory.md#subobject-classifier) assigns to $C$ the set of sieves on $C$.

##### Slice-small presheaf construction

↑ **Parent:** [Presheaf topos](#presheaf-topos)

If every [slice category](category.md#slice-category) $\mathcal C/A$ is essentially small, the displayed [exponential object](category.md#exponential-object) and the set of [sieves on a category](#sieve-category-theory) at each $A$ are small even when $\mathcal C$ is large. Together with pointwise [finite limits](category.md#finite-limit), they give the elementary-topos constructions in a universe admitting the large diagrams. This does not force the entire functor category to be locally small in the original universe: a large discrete category has terminal slices, but maps between its constant-one and constant-two presheaves are arbitrary class-indexed binary families.

##### Exponential in a presheaf category

↑ **Parent:** [Presheaf topos](#presheaf-topos)

For [categorical presheaves](#presheaf-category-theory) $P,Q$ on a [small category](category.md#small-category), restrictions in the displayed [exponential object](category.md#exponential-object) act by precomposition with $H_u\times1_P$. Evaluation sends $(\alpha,x)$ at $c$ to $\alpha_c(1_c,x)$. The [currying](category.md#currying) of $t:R\times P\to Q$ sends $z\in R(c)$ to the natural transformation whose value on $(v:a\to c,x\in P(a))$ is $t_a(R(v)z,x)$. Evaluation and currying are inverse and natural, proving the [Cartesian closed category](category.md#cartesian-closed-category) structure.

### Arrow category

↑ **Parent:** [Functor category](#functor-category)

The arrow category of $\mathcal C$ has morphisms $A_0\to A_1$ of $\mathcal C$ as objects and commutative squares as morphisms. It is the [functor category](#functor-category) $[\mathbf 2,\mathcal C]$, where $\mathbf 2$ is the category with one nonidentity arrow.

It is also the [comma category](category.md#comma-category) $(\operatorname{id}_{\mathcal C}\downarrow\operatorname{id}_{\mathcal C})$.

#### Adjoint chain for evaluation in an arrow category

↑ **Parent:** [Arrow category](#arrow-category)

Write a presheaf on $0\to1$ as an arrow $r:B\to A$. Evaluation $\Gamma(r)=B$ has the displayed chain, where $\Pi(r)=A$, $\Delta(S)=(S\xrightarrow1 S)$, $\nabla(S)=(S\to1)$ and $\Lambda(S)=(\varnothing\to S)$. The Hom-set bijections follow by solving the commuting-square equation. The functor $\nabla$ has no right adjoint because it fails to preserve the initial object: $\nabla(\varnothing)=(\varnothing\to1)$ is not $(\varnothing\to\varnothing)$.

#### Category of injective functions

↑ **Parent:** [Arrow category](#arrow-category)

The category of injective functions is the full subcategory of $[\mathbf 2,\mathbf{Set}]$ whose objects are [injective functions](algebra.md#injective-function). It is cartesian closed: products are computed pointwise, and exponentiating an injection by any arrow again gives an injection.

### Representable functor

↑ **Parent:** [Functor category](#functor-category)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Representable_functor)

A covariant functor is representable when it is naturally isomorphic to $\mathcal C(A,-)$ for some object $A$; a contravariant functor is representable when it is naturally isomorphic to $\mathcal C(-,A)$.

#### Representable retract criterion

↑ **Parent:** [Representable functor](#representable-functor)

Suppose a [small category](category.md#small-category) has [equalizers](category.md#equaliser). If a [categorical presheaf](#presheaf-category-theory) $P$ is a retract $P\xrightarrow{i}H_B\xrightarrow{p}P$, with $pi=1_P$, then $i$ equalizes $ip$ and $1_{H_B}$. The [Yoneda lemma](#yoneda-lemma) writes $ip=H_b$ for an endomorphism $b:B\to B$. An equalizer $A\to B$ of $b$ and $1_B$ gives the same presheaf equalizer, since the [Yoneda embedding](#yoneda-embedding) preserves [categorical limits](category.md#categorical-limit). Uniqueness of equalizers gives $P\cong H_A$.

#### Representability from a solution set

↑ **Parent:** [Representable functor](#representable-functor)

On a [complete category](category.md#complete-category) that is [locally small](category.md#locally-small-category), a set-valued [functor](functor.md) is representable exactly when it preserves small [categorical limits](category.md#categorical-limit) and its [category of elements](category.md#category-of-elements) has a [weakly initial set](category.md#weakly-initial-set). [Categorical limit](category.md#categorical-limit) preservation makes that comma [category](category.md) complete. The [initial-object lemma for complete categories with a weakly initial set](category.md#initial-object-lemma-for-complete-categories-with-a-weakly-initial-set) then supplies a [universal element](#universal-element-of-a-set-valued-functor), hence a [representation of a functor](#representation-of-a-functor).

#### Left adjoint to a covariant representable functor

↑ **Parent:** [Representable functor](#representable-functor)

If $\mathcal C$ has small [coproducts in a category](category.md#coproduct) and $U\cong\mathcal C(R,-)$, then $F(S)=\coprod_{s\in S}R$ is a [left adjoint](category.md#adjoint-functors) to $U$. Maps from this coproduct to $X$ are families of maps $R\to X$, naturally equivalent to functions $S\to UX$. Conversely, a set-valued [right adjoint](category.md#adjoint-functors) $U$ is represented by $F(1)$, because maps from a singleton evaluate to elements.

#### Covariant representables preserve limits

↑ **Parent:** [Representable functor](#representable-functor)

A [representable functor](#representable-functor) $\mathcal C(R,-)$ preserves every small [categorical limit](category.md#categorical-limit) that exists. A map from $R$ into a limit is exactly a compatible family of maps from $R$ to the diagram objects, and such a family is exactly an element of the corresponding limit of sets. The comparison bijection is the one induced by the limit projections.

#### Colimit criterion for representability of a presheaf

↑ **Parent:** [Representable functor](#representable-functor)

A [categorical presheaf](#presheaf-category-theory) is [representable](#representable-functor) if its elements projection has a [colimit](category.md#colimit) and the presheaf preserves the opposite-indexed [categorical limit](category.md#categorical-limit) of that projection. Compatibility of all distinguished elements then supplies a [universal element](#universal-element-of-a-set-valued-functor) at the colimit object. The preservation requirement must cover this diagram even when its indexing [category](category.md) is large.

##### Small-limit preservation is insufficient for the large elements-colimit criterion

↑ **Parent:** [Colimit criterion for representability of a presheaf](#colimit-criterion-for-representability-of-a-presheaf)

Let $\mathcal C$ be the ordered [category](category.md) of all [ordinals](ordinal.md) with an added greatest object $\infty$. The [categorical presheaf](#presheaf-category-theory) with $X(\alpha)=\{*\}$ at ordinals and $X(\infty)=\varnothing$ preserves every small [categorical limit](category.md#categorical-limit): a small supremum is an ordinal unless its diagram contains $\infty$. Its [category of elements](category.md#category-of-elements) consists of all ordinals, and their projection has the large [colimit](category.md#colimit) $\infty$. Nevertheless $X$ is not [representable](#representable-functor): an ordinal representer has bounded support, while the representer $\infty$ has a nonempty value at $\infty$. Thus preservation must include the possibly large opposite elements diagram. The dual functor $X^{\mathrm{op}}:\mathcal C\to\mathbf{Set}^{\mathrm{op}}$ also disproves the comma-projection criterion for a right adjoint under small-colimit preservation alone.

#### Canonical colimit presentation of a covariant set-valued functor

↑ **Parent:** [Representable functor](#representable-functor)

Every [functor](functor.md) $F:\mathcal C\to\mathbf{Set}$ on a [small category](category.md#small-category) is the [colimit](category.md#colimit) of the covariant [representable functors](#representable-functor) $\mathcal C(A,-)$ indexed by the opposite of its [category of elements](category.md#category-of-elements). The cocone indexed by $(A,x)$ sends $f:A\to B$ to $F(f)(x)$. By the [Yoneda lemma](#yoneda-lemma), a compatible cocone into $G$ is exactly a [natural transformation](#natural-transformation) $F\to G$. The opposite indexing direction is essential because precomposition reverses the representing-object arrow.

#### Representation of a functor

↑ **Parent:** [Representable functor](#representable-functor)

A representation of $F:\mathcal C\to\mathbf{Set}$ is an object $A$ together with a universal element $a\in F(A)$ such that

$$
\mathcal C(A,B)\longrightarrow F(B),
\qquad f\longmapsto F(f)(a)
$$

is a bijection for every $B$, naturally in $B$. Equivalently, it is a specified natural isomorphism $\mathcal C(A,-)\cong F$.

##### Uniqueness of functor representations

↑ **Parent:** [Representation of a functor](#representation-of-a-functor)

Two [representations of a functor](#representation-of-a-functor) have unique mutually inverse [morphisms](algebra.md#morphism) carrying their specified [universal elements](#universal-element-of-a-set-valued-functor) to one another. Composing those [morphisms](algebra.md#morphism) preserves each [universal element](#universal-element-of-a-set-valued-functor), so injectivity of the representing [bijection](function.md#bijection) makes the composites identities. Arbitrary [isomorphisms](algebra.md#isomorphism) of the underlying objects need not preserve the specified elements.

##### Functoriality of chosen representations

↑ **Parent:** [Representation of a functor](#representation-of-a-functor)

If $H:\mathcal A^{\mathrm{op}}\times\mathcal B\to\mathbf{Set}$ has chosen representations $\psi_B:\mathcal A(-,GB)\cong H(-,B)$, the [Yoneda lemma](#yoneda-lemma) determines a unique [functor](functor.md) $G$ on morphisms by $\mathcal A(-,Gb)=\psi_{B'}^{-1}H(-,b)\psi_B$. This makes the representing [natural isomorphisms](#natural-isomorphism) natural in $B$.

##### Universal element of a set-valued functor

↑ **Parent:** [Representation of a functor](#representation-of-a-functor)

The universal element in a [representation of a functor](#representation-of-a-functor) is the image of $1_A$ under the representing natural isomorphism. Any two universal elements induce unique mutually inverse maps between their representing objects, so representations are unique up to unique compatible isomorphism.

#### Yoneda lemma

↑ **Parent:** [Representable functor](#representable-functor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Yoneda_lemma)

The Yoneda lemma gives natural bijections

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A)
$$

and their contravariant analogues.

##### Density formula for presheaves

↑ **Parent:** [Yoneda lemma](#yoneda-lemma)

For a [presheaf on a category](#presheaf-category-theory), the [categorical coend](category.md#coend-of-a-functor) identifies $(fh,x)$ with $(h,X(f)x)$. The displayed isomorphism sends the class of $(h:U\to W,x\in X(W))$ to $X(h)x$, with inverse $y\mapsto[1_U,y]$. The coend relation makes these inverse and natural. Consequently every presheaf is the [colimit](category.md#colimit) of representables indexed by its [category of elements](category.md#category-of-elements).

##### Yoneda embedding

↑ **Parent:** [Yoneda lemma](#yoneda-lemma)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Yoneda_embedding)

The Yoneda embedding sends $A$ to $\mathcal C(-,A)$. The [Yoneda lemma](#yoneda-lemma) identifies natural transformations $yA\to yB$ with morphisms $A\to B$, so the embedding is [full and faithful](#full-and-faithful-functor). It preserves every limit that exists in $\mathcal C$.

###### Yoneda embedding detects split epimorphisms

↑ **Parent:** [Yoneda embedding](#yoneda-embedding)

For $f:A\to B$, the [Yoneda embedding](#yoneda-embedding) sends $f$ to postcomposition $\mathcal C(-,A)\to\mathcal C(-,B)$. If this is epic in the [presheaf category](#presheaf-category), its component at $B$ is surjective, so $1_B=fg$ for some $g:B\to A$. Conversely such a section makes the natural transformation split epic. Pointwise surjectivity follows directly by doubling the target presheaf along the image subpresheaf: the two inclusions agree on the image but differ on any element outside it.

###### Yoneda embedding preserves exponentials

↑ **Parent:** [Yoneda embedding](#yoneda-embedding)

For a small [Cartesian closed category](category.md#cartesian-closed-category), the [Yoneda embedding](#yoneda-embedding) into its [presheaf category](#presheaf-category) preserves [exponential objects](category.md#exponential-object). At $C$, the [exponential in a presheaf category](#exponential-in-a-presheaf-category) has value $\operatorname{Nat}(YC\times YA,YB)$. Since $YC\times YA\cong Y(C\times A)$, the [Yoneda lemma](#yoneda-lemma) identifies this with $\mathcal C(C\times A,B)\cong\mathcal C(C,B^A)$. Every identification is natural in all three objects.

###### Covariant Yoneda embedding

↑ **Parent:** [Yoneda embedding](#yoneda-embedding)

The covariant version of the [Yoneda embedding](#yoneda-embedding) sends an object to its outgoing [representable functor](#representable-functor). Precomposition reverses arrows. The [Yoneda lemma](#yoneda-lemma) gives $\operatorname{Nat}(Y(A),Y(B))\cong\mathcal C(B,A)$, so it is [full and faithful](#full-and-faithful-functor). It carries existing [colimits](category.md#colimit) in $\mathcal C$ to pointwise [categorical limits](category.md#categorical-limit).

### Pointwise epimorphism in a functor category

↑ **Parent:** [Functor category](#functor-category)

A natural transformation in a set-valued [functor category](#functor-category) is an [epimorphism](category.md#epimorphism) exactly when every component is a [surjective function](algebra.md#surjective-function). More generally, limits and colimits in a functor category are computed pointwise whenever they exist in the codomain.

#### Pushout witness for failure of pointwise surjectivity

↑ **Parent:** [Pointwise epimorphism in a functor category](#pointwise-epimorphism-in-a-functor-category)

For a [natural transformation](#natural-transformation) $a:X\to Y$ of set-valued [functors](functor.md), form the [pushout](category.md#pushout) by taking two copies of each $Y(C)$ and identifying the two copies of every element in the image of $a_C$. [Naturality](#naturality) makes all induced maps well-defined. If $y\in Y(C)$ is outside that image, its two copies remain distinct. Thus the two maps $Y\rightrightarrows Y\amalg_XY$ agree after $a$ but differ at $y$, proving $a$ is not an [epimorphism](category.md#epimorphism). Conversely, componentwise [surjective functions](algebra.md#surjective-function) allow cancellation at every object, proving that $a$ is an epimorphism. This argument does not assume a natural choice of preimages.

## Monofunctor

↑ **Parent:** [Functor](functor.md)

A functor $F:\mathcal C\to\mathbf{Set}$ is a monofunctor when $F(f)$ is an [injective function](algebra.md#injective-function) for every [morphism](algebra.md#morphism) $f$ of $\mathcal C$.

## Natural transformation

↑ **Parent:** [Functor](functor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_transformation)

A natural transformation between [functors](functor.md) $F,G:\mathcal C\to\mathcal D$ assigns a [categorical morphism](category.md#morphism-in-a-category) $\alpha_A:F(A)\to G(A)$ to every [object of a category](category.md#object-of-a-category) $A$, with

$$
G(f)\circ\alpha_A=\alpha_B\circ F(f)\qquad\text{for every }f:A\to B.
$$

This [naturality](#naturality) condition says that transforming the input before transporting it gives the same result as transporting it first and transforming the output. It constrains the whole family of arrows, so unrelated choices of a map for each object generally fail it.

For a concrete example, compare the [functor](functor.md) that leaves every [set](set.md) and [function](function.md) unchanged with the [power set](set.md#power-set) [functor](functor.md) using images of [subsets](set.md#subset). The maps $\eta_X:X\to\mathcal P(X)$ given by $x\mapsto\{x\}$ form a [natural transformation](#natural-transformation): for any [function](function.md) $f:X\to Y$,

$$
\mathcal P(f)(\eta_X(x))=f(\{x\})=\{f(x)\}=\eta_Y(f(x)).
$$

The right-hand panel of the [category](category.md) illustration checks the square at $x=3$ with $f(x)=x+1$: both routes end at $\{4\}$. The statement works for every [function](function.md), rather than depending on a preferred labeling of a particular [set](set.md).

### Dinatural transformation

↑ **Parent:** [Natural transformation](#natural-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dinatural_transformation)

For $F,G:\mathcal C^{\mathrm{op}}\times\mathcal C\to\mathcal D$, a dinatural transformation has components $\alpha_C:F(C,C)\to G(C,C)$ satisfying, for $f:C\to D$,

$$
G(1_C,f)\alpha_CF(f,1_C)=G(f,1_D)\alpha_DF(1_D,f).
$$

Both composites have domain $F(D,C)$ and codomain $G(C,D)$. It is the compatibility used for [categorical ends](category.md#end-of-a-functor) and [categorical coends](category.md#coend-of-a-functor), rather than ordinary naturality on just one variance.

### Natural isomorphism

↑ **Parent:** [Natural transformation](#natural-transformation)

A [natural transformation](#natural-transformation) all of whose components are isomorphisms. Their inverses form the inverse [natural transformation](#natural-transformation).

#### Natural bijection

↑ **Parent:** [Natural isomorphism](#natural-isomorphism)

A natural bijection between set-valued [functors](functor.md) is a [natural transformation](#natural-transformation) whose component functions are [bijections](function.md#bijection). Their inverse functions are automatically natural, so it is a [natural isomorphism](#natural-isomorphism).

### Naturality

↑ **Parent:** [Natural transformation](#natural-transformation)

For a [natural transformation](#natural-transformation) $\theta:F\Rightarrow G$, naturality is the equation $G(f)\theta_A=\theta_BF(f)$ for each [morphism](algebra.md#morphism) $f:A\to B$. Thus transforming and then applying a [functor](functor.md) gives the same result as applying that functor and then transforming. It makes the component maps a coherent transformation of [functors](functor.md).

## Full and faithful functor

↑ **Parent:** [Functor](functor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Full_and_faithful_functor)

A functor $F:\mathcal C\to\mathcal D$ is full and faithful when every map

$$
\mathcal C(A,B)\longrightarrow\mathcal D(FA,FB)
$$

is a bijection.

## Faithful functor

↑ **Parent:** [Functor](functor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faithful_functor)

A functor is faithful when each induced map on hom-sets is injective, and full when each such map is surjective. Every faithful functor reflects monomorphisms and epimorphisms.

## ↑ Ancestors (6)

1. [Category](category.md)
2. [Category theory](category-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (227)

- [Adjoint functor theorem](category.md#adjoint-functor-theorem)
- [Base change of invertible modules](module-theory.md#base-change-of-invertible-modules)
- [Bifunctor](#bifunctor)
- [Bounded subfunctor solution set for precomposition](category.md#bounded-subfunctor-solution-set-for-precomposition)
- [Brown's representability theorem](homotopy.md#brown-s-representability-theorem)
- [Canonical colimit presentation of a covariant set-valued functor](#canonical-colimit-presentation-of-a-covariant-set-valued-functor)
- [Category of abelian groups](category-theory.md#category-of-abelian-groups)
- [Category of adjunctions inducing a fixed monad](category-theory.md#category-of-adjunctions-inducing-a-fixed-monad)
- [Category of small categories](category.md#category-of-small-categories)
- [Category theory](category-theory.md)
- [Coherent functor](category-theory.md#coherent-functor)
- [Commutation of iterated categorical limits](category.md#commutation-of-iterated-categorical-limits)
- [Connected component of a category](category.md#connected-component-of-a-category)
- [Connected-component presheaf of a functor](category.md#connected-component-presheaf-of-a-functor)
- [Conservative functor](#conservative-functor)
- [Conservativity of set products on totally supported families](category.md#conservativity-of-set-products-on-totally-supported-families)
- [Constant diagram functor](#constant-diagram-functor)
- [Corestriction functor for comodules](multilinear-algebra.md#corestriction-functor-for-comodules)
- [Coseparator](category.md#coseparator)
- [Covariant density presentation](category.md#covariant-density-presentation)
- [Currying adjunction for small categories](category.md#currying-adjunction-for-small-categories)
- [Diaconescu equivalence for geometric morphisms](category-theory.md#diaconescu-equivalence-for-geometric-morphisms)
- [Discrete opfibration](#discrete-opfibration)
- [Endofunctor](#endofunctor)
- [Equalizer preservation by pullback-preserving functors](#equalizer-preservation-by-pullback-preserving-functors)
- [Equalizer submonad of a monad](category-theory.md#equalizer-submonad-of-a-monad)
- [Equivalence of categories](#equivalence-of-categories)
- [Essential geometric morphism](category-theory.md#essential-geometric-morphism)
- [Essential surjectivity](#essential-surjectivity)
- [Finality of a functor](category.md#finality-of-a-functor)
- [Finite colimits of monad algebras from reflexive coequalizers](category-theory.md#finite-colimits-of-monad-algebras-from-reflexive-coequalizers)
- [Finite-limit-preserving set-valued functor](#finite-limit-preserving-set-valued-functor)
- [Five adjoints for constant presheaves on open sets](#five-adjoints-for-constant-presheaves-on-open-sets)
- [Fixed point of a group action](group-action.md#fixed-point-of-a-group-action)
- [Flat functor](#flat-functor)
- [Flat functor and finite-limit preservation](#flat-functor-and-finite-limit-preservation)
- [Forgetful functor](#forgetful-functor)
- [Free algebra functor](category-theory.md#free-algebra-functor)
- [Free category on independent arrows](category.md#free-category-on-independent-arrows)
- [Freyd general adjoint functor theorem](category.md#freyd-general-adjoint-functor-theorem)
- [Frobenius monoidal functor](category-theory.md#frobenius-monoidal-functor)
- [Full functor](#full-functor)
- [Full subcategory](category.md#full-subcategory)
- [Functoriality of abelian image factorization](category.md#functoriality-of-abelian-image-factorization)
- [Functoriality of chosen representations](#functoriality-of-chosen-representations)
- [Geometric syntactic category](mathematical-logic.md#geometric-syntactic-category)
- [Groupoid](category.md#groupoid)
- [Hilbert functor](algebraic-geometry.md#hilbert-functor)
- [Hom-set detection of categorical limits](category.md#hom-set-detection-of-categorical-limits)
- [Horn theory](mathematical-logic.md#horn-theory)
- [Initial object criterion for a covariant local topos](category-theory.md#initial-object-criterion-for-a-covariant-local-topos)
- [Isomorphism of categories](#isomorphism-of-categories)
- [Kan extension](#kan-extension)
- [Left derived functor](homological-algebra.md#left-derived-functor)
- [Left derived functors on an abelian category](homological-algebra.md#left-derived-functors-on-an-abelian-category)
- [Left Kan extension as a comma-category colimit](category.md#left-kan-extension-as-a-comma-category-colimit)
- [Limit-creating functor](#limit-creating-functor)
- [Limit form of the special adjoint functor theorem](category.md#limit-form-of-the-special-adjoint-functor-theorem)
- [Limit-reflecting functor](#limit-reflecting-functor)
- [Minimal supported subobject](category.md#minimal-supported-subobject)
- [Monad morphism](category-theory.md#monad-morphism)
- [Monadic tower for nested partial unary operations](category-theory.md#monadic-tower-for-nested-partial-unary-operations)
- [Morphism in a category](category.md#morphism-in-a-category)
- [Natural bijection](#natural-bijection)
- [Natural transformation](#natural-transformation)
- [Naturality](#naturality)
- [Nonregular extremal epimorphism in the category of categories](category.md#nonregular-extremal-epimorphism-in-the-category-of-categories)
- [Opmonoidal functor](category-theory.md#opmonoidal-functor)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#7/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-17.md#9/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-4.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#11/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#7/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-20.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#8/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#8/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#8/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-18.md#9/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-23.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-23.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-23.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-24.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-23.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-26.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#8/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-23.md#8/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-24.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-24.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-24.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-24.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-21.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-23.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-25.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-18.md#8/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-74.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-74.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-18.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-18.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-18.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-18.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-18.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-22.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-119.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-119.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-119.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-119.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-165.md#1/i/solution)
- [Picard functor of a curve](sheaf-of-modules.md#picard-functor-of-a-curve)
- [Pointwise monomorphism in a set-valued functor category](#pointwise-monomorphism-in-a-set-valued-functor-category)
- [Preservation obstructions to extending an adjoint chain](category.md#preservation-obstructions-to-extending-an-adjoint-chain)
- [Presheaf (category theory)](#presheaf-category-theory)
- [Presheaf classifier of a Horn theory](mathematical-logic.md#presheaf-classifier-of-a-horn-theory)
- [Projective space represents invertible quotients](projective-space.md#projective-space-represents-invertible-quotients)
- [Projectivity detected by all first left derived functors](category.md#projectivity-detected-by-all-first-left-derived-functors)
- [Pushout witness for failure of pointwise surjectivity](#pushout-witness-for-failure-of-pointwise-surjectivity)
- [Reflexive coequalizer](category-theory.md#reflexive-coequalizer)
- [Regular functor](#regular-functor)
- [Representability from a solution set](#representability-from-a-solution-set)
- [Representable test for initial functors](category.md#representable-test-for-initial-functors)
- [Restriction of monad algebras](category-theory.md#restriction-of-monad-algebras)
- [Retract criterion for surjective presheaf geometric morphisms](category-theory.md#retract-criterion-for-surjective-presheaf-geometric-morphisms)
- [Right-adjoint criterion using comma-category colimits](category.md#right-adjoint-criterion-using-comma-category-colimits)
- [Right-exact additive functor](category-theory.md#right-exact-additive-functor)
- [Right monoid action](algebraic-operation.md#right-monoid-action)
- [Simplicial set](homotopy.md#simplicial-set)
- [Slice category](category.md#slice-category)
- [Slice of a set-valued functor category](category.md#slice-of-a-set-valued-functor-category)
- [Split coequalizer](category.md#split-coequalizer)
- [Split epimorphism](category.md#split-epimorphism)
- [Split equalizer](category.md#split-equalizer)
- [Split monomorphism](category.md#split-monomorphism)
- [Subterminal sheaf](category.md#subterminal-sheaf)
- [Terminal category](category.md#terminal-category)
- [Terminality of the Eilenberg-Moore adjunction](category-theory.md#terminality-of-the-eilenberg-moore-adjunction)
- [Topological half-exact functor](homotopy.md#topological-half-exact-functor)
- [Uniqueness of a final-discrete-fibration factorization](category.md#uniqueness-of-a-final-discrete-fibration-factorization)
