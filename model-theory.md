# Model theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Model_theory)

Model theory studies mathematical structures through the first-order sentences and formulas they satisfy.

**Table of contents**

- [Finite model theory](#finite-model-theory)
  - [Asymptotic equivalence of formulas](#asymptotic-equivalence-of-formulas)
  - [Partial fixed-point logic](#partial-fixed-point-logic)
  - [Gaifman graph](#gaifman-graph)
    - [Hanf locality lemma](#hanf-locality-lemma)
- [Recursive presentation of a structure](#recursive-presentation-of-a-structure)
  - [Computable isomorphism](#computable-isomorphism)
- [Algebraic theory](#algebraic-theory)
  - [Finitely presented models of an algebraic theory](#finitely-presented-models-of-an-algebraic-theory)
- [Ehrenfeucht-Fraïssé game](#ehrenfeucht-fraisse-game)
  - [Interval threshold strategy for discrete linear orders](#interval-threshold-strategy-for-discrete-linear-orders)
  - [Ehrenfeucht-Fraïssé theorem](#ehrenfeucht-fraisse-theorem)
    - [Failure of finite-round game equivalence in infinite languages](#failure-of-finite-round-game-equivalence-in-infinite-languages)
- [Theory of formally real fields](#theory-of-formally-real-fields)
- [Theory of nontrivial torsion-free divisible Abelian groups](#theory-of-nontrivial-torsion-free-divisible-abelian-groups)
  - [Theory of torsion-free divisible Abelian groups allowing the trivial group](#theory-of-torsion-free-divisible-abelian-groups-allowing-the-trivial-group)
- [Algebraically prime extension](#algebraically-prime-extension)
- [Reduced product](#reduced-product)
- [Elementary equivalence](#elementary-equivalence)
- [Monster model](#monster-model)
  - [Orbit of a definable set in a monster model](#orbit-of-a-definable-set-in-a-monster-model)
- [Complete theory](#complete-theory)
  - [Categorical theory](#categorical-theory)
    - [Omega-categorical theory](#omega-categorical-theory)
      - [Ryll-Nardzewski theorem](#ryll-nardzewski-theorem)
        - [Reduct of an aleph-zero-categorical theory](#reduct-of-an-aleph-zero-categorical-theory)
    - [Morley categoricity theorem](#morley-categoricity-theorem)
    - [Reduct need not preserve uncountable categoricity](#reduct-need-not-preserve-uncountable-categoricity)
    - [Nonstandard model of the additive integers](#nonstandard-model-of-the-additive-integers)
    - [Aleph-zero-categoricity of an infinite-dimensional vector space over a finite field](#aleph-zero-categoricity-of-an-infinite-dimensional-vector-space-over-a-finite-field)
- [Diagram (mathematical logic)](#diagram-mathematical-logic)
  - [Elementary diagram of a structure](#elementary-diagram-of-a-structure)
  - [Method of diagrams](#method-of-diagrams)
    - [Diagram embedding criterion for universal theories](#diagram-embedding-criterion-for-universal-theories)
    - [Finitely satisfiable type is realized in an elementary extension](#finitely-satisfiable-type-is-realized-in-an-elementary-extension)
- [Inductive first-order theory](#inductive-first-order-theory)
- [Model-complete theory](#model-complete-theory)
  - [Model companion](#model-companion)
  - [Theory of real closed fields](#theory-of-real-closed-fields)
    - [Quantifier elimination for ordered real closed fields](#quantifier-elimination-for-ordered-real-closed-fields)
    - [Non-Archimedean real closed field](#non-archimedean-real-closed-field)
    - [Model-theoretic proof of Hilbert's seventeenth problem](#model-theoretic-proof-of-hilbert-s-seventeenth-problem)
- [Ehrenfeucht-Mostowski model](#ehrenfeucht-mostowski-model)
  - [Order-indiscernible sequence](#order-indiscernible-sequence)
  - [Ehrenfeucht-Mostowski theorem](#ehrenfeucht-mostowski-theorem)
    - [Ultraproduct proof of the Ehrenfeucht-Mostowski theorem](#ultraproduct-proof-of-the-ehrenfeucht-mostowski-theorem)
    - [Models with arbitrarily large automorphism groups](#models-with-arbitrarily-large-automorphism-groups)
- [Prime model](#prime-model)
  - [Atomic model](#atomic-model)
    - [Countable atomic model without a countable saturated model](#countable-atomic-model-without-a-countable-saturated-model)
    - [Countable atomic model is prime](#countable-atomic-model-is-prime)
    - [One-point extension between atomic models](#one-point-extension-between-atomic-models)
- [Quantifier elimination](#quantifier-elimination)
  - [Extension axioms for an unrestricted binary relation](#extension-axioms-for-an-unrestricted-binary-relation)
  - [Common-substructure test for quantifier elimination](#common-substructure-test-for-quantifier-elimination)
    - [Existential common-substructure test for quantifier elimination](#existential-common-substructure-test-for-quantifier-elimination)
      - [Algebraically prime extension test for quantifier elimination](#algebraically-prime-extension-test-for-quantifier-elimination)
  - [Partial embedding](#partial-embedding)
  - [Quantifier elimination for algebraically closed fields](#quantifier-elimination-for-algebraically-closed-fields)
    - [Type space of an algebraically closed field over a subfield](#type-space-of-an-algebraically-closed-field-over-a-subfield)
  - [Theory of the random graph](#theory-of-the-random-graph)
    - [Quantifier elimination for the random graph](#quantifier-elimination-for-the-random-graph)
    - [Algebraic and definable closure in the random graph](#algebraic-and-definable-closure-in-the-random-graph)
    - [Three-type space of the random graph](#three-type-space-of-the-random-graph)
  - [Back-and-forth method](#back-and-forth-method)
    - [Effective back-and-forth construction](#effective-back-and-forth-construction)
  - [Dense linear order without endpoints](#dense-linear-order-without-endpoints)
    - [Ehrenfeucht theory of an increasing named sequence](#ehrenfeucht-theory-of-an-increasing-named-sequence)
    - [Suslin line](#suslin-line)
      - [Suslin hypothesis](#suslin-hypothesis)
    - [Quantifier elimination for dense linear orders without endpoints](#quantifier-elimination-for-dense-linear-orders-without-endpoints)
- [Ultraproduct](#ultraproduct)
  - [Countable saturation of an ultraproduct over omega](#countable-saturation-of-an-ultraproduct-over-omega)
  - [Ultrapower](#ultrapower)
    - [Model-theoretic ultralimit](#model-theoretic-ultralimit)
      - [Alternating ultrapowers give isomorphic ultralimits](#alternating-ultrapowers-give-isomorphic-ultralimits)
      - [Frayne embedding lemma](#frayne-embedding-lemma)
    - [Diagonal argument for ultrapower cardinality](#diagonal-argument-for-ultrapower-cardinality)
  - [Łoś theorem](#los-theorem)
    - [Dense-extension filter semantics](#dense-extension-filter-semantics)
    - [Infinite field of positive characteristic from an ultraproduct](#infinite-field-of-positive-characteristic-from-an-ultraproduct)
- [Elementary extension](#elementary-extension)
  - [Saturated model](#saturated-model)
    - [Omega-saturated model](#omega-saturated-model)
    - [Saturated elementary extension theorem](#saturated-elementary-extension-theorem)
    - [Countable saturation of a nonprincipal ultraproduct over omega](#countable-saturation-of-a-nonprincipal-ultraproduct-over-omega)
    - [Saturation implies homogeneity](#saturation-implies-homogeneity)
    - [Homogeneity plus realization of empty-set types implies saturation](#homogeneity-plus-realization-of-empty-set-types-implies-saturation)
    - [Universal model](#universal-model)
    - [Homogeneous model](#homogeneous-model)
    - [Universal homogeneous model is saturated](#universal-homogeneous-model-is-saturated)
    - [Small elementary submodel meeting every definable equivalence class](#small-elementary-submodel-meeting-every-definable-equivalence-class)
  - [Elementary chain theorem](#elementary-chain-theorem)
    - [Directed limit of elementary embeddings](#directed-limit-of-elementary-embeddings)
  - [Complete type](#complete-type)
    - [Algebraic type](#algebraic-type)
    - [Type space](#type-space)
      - [Stone topology on a type space](#stone-topology-on-a-type-space)
      - [Isolated type](#isolated-type)
        - [Density of isolated types from a prime model](#density-of-isolated-types-from-a-prime-model)
      - [Omitted type](#omitted-type)
        - [Omitting types theorem](#omitting-types-theorem)
          - [Henkin omission extension lemma](#henkin-omission-extension-lemma)
      - [Realization of a type in an elementary extension](#realization-of-a-type-in-an-elementary-extension)
      - [Total disconnectedness of a type space](#total-disconnectedness-of-a-type-space)
      - [One-types over the natural numbers in the rational order](#one-types-over-the-natural-numbers-in-the-rational-order)
    - [Aleph-zero-homogeneous model](#aleph-zero-homogeneous-model)
- [Stable theory](#stable-theory)
  - [Fundamental theorem of stability](#fundamental-theorem-of-stability)
    - [Definable type](#definable-type)
      - [Stable trace of a definable set](#stable-trace-of-a-definable-set)
  - [Omega-stability implies stability in every infinite cardinal](#omega-stability-implies-stability-in-every-infinite-cardinal)
  - [Order property](#order-property)
    - [Order property implies instability](#order-property-implies-instability)
- [Strongly minimal theory](#strongly-minimal-theory)
  - [Model-theoretic algebraic closure](#model-theoretic-algebraic-closure)
    - [Model-theoretic definable closure](#model-theoretic-definable-closure)
    - [Pregeometry](#pregeometry)
      - [Basis of a pregeometry](#basis-of-a-pregeometry)
        - [Dimension of a pregeometry](#dimension-of-a-pregeometry)
      - [Generic type in a strongly minimal theory](#generic-type-in-a-strongly-minimal-theory)
      - [Independent set in a strongly minimal theory](#independent-set-in-a-strongly-minimal-theory)
  - [Homogeneity of models of a countable strongly minimal theory](#homogeneity-of-models-of-a-countable-strongly-minimal-theory)

## Finite model theory

↑ **Parent:** [Model theory](model-theory.md)

Finite model theory studies logical definability and equivalence on finite [first-order structures](mathematical-logic.md#first-order-structure). Unlike unrestricted model theory, first-order compactness is unavailable when models are required to be finite. Locality, bounded-variable games and descriptive characterizations of [complexity classes](theoretical-computer-science.md#complexity-class) are central tools.

### Asymptotic equivalence of formulas

↑ **Parent:** [Finite model theory](#finite-model-theory)

Two formulas with the same free variables are asymptotically equivalent when the probability of their universal equivalence tends to one over the chosen finite-structure distribution. If a quantifier-eliminating extension theory has all its axioms of asymptotic probability one, compactness makes every formula asymptotically equivalent to a quantifier-free one: each particular equivalence follows from finitely many axioms, whose conjunction still has limiting probability one.

### Partial fixed-point logic

↑ **Parent:** [Finite model theory](#finite-model-theory)

Extend [first-order logic](mathematical-logic.md#first-order-logic) by iterating definable relation operators from the empty relation. If iteration reaches a fixed point, use that relation; if it enters a nontrivial cycle, the partial fixed point is the empty relation. For a fixed arity on a finite universe, a relation requires polynomially many bits and there are exponentially many states, so iteration is evaluable in [PSPACE](theoretical-computer-science.md#pspace). On finite ordered structures this logic captures PSPACE.

### Gaifman graph

↑ **Parent:** [Finite model theory](#finite-model-theory)

For a relational structure, the Gaifman graph has the same universe. Two distinct elements are adjacent if they occur together in some tuple of some interpreted relation. A tuple's radius-$r$ neighbourhood is the induced structure on the union of its radius-$r$ graph balls, with the tuple marked by constants.

#### Hanf locality lemma

↑ **Parent:** [Gaifman graph](#gaifman-graph)

For a finite relational signature and quantifier rank $q$, matching the numbers of all marked radius-$3^q$ one-point neighbourhood types suffices for two finite structures to satisfy the same first-order sentences of rank at most $q$. Equivalently, a bijection can match the isomorphism types of these marked neighbourhoods point by point. On bounded-degree structures, a threshold version permits large neighbourhood-type counts to differ once both exceed a fixed bound. Long cycles of equal total size give useful exact-count applications.

## Recursive presentation of a structure

↑ **Parent:** [Model theory](model-theory.md)

A recursive presentation identifies the domain of a countable structure with a [computable set](computability-theory.md#computable-set), with its basic operations given by [total computable functions](computability-theory.md#total-computable-function) and its basic relations decidable. In a fixed finite signature this makes evaluation of [atomic formulas](mathematical-logic.md#atomic-formula) effective. A countable structure may have a [recursive presentation of a structure](#recursive-presentation-of-a-structure) only for some choices of presentation, or none at all.

### Computable isomorphism

↑ **Parent:** [Recursive presentation of a structure](#recursive-presentation-of-a-structure)

A computable isomorphism is an [isomorphism](algebra.md#isomorphism) between presented structures whose underlying map is a [total computable function](computability-theory.md#total-computable-function). For presentations on $\mathbb N$, its inverse is computable too: enumerate inputs until the required output occurs. Two abstractly [isomorphic](algebra.md#isomorphism) structures with a [recursive presentation of a structure](#recursive-presentation-of-a-structure) need not admit a [computable isomorphism](#computable-isomorphism) between the chosen presentations.

## Algebraic theory

↑ **Parent:** [Model theory](model-theory.md)

A finitary algebraic theory specifies sorts, finite-arity operations and equations between terms. Its internal models can be interpreted in any category with finite products. Finitely presented set-based models generate arbitrary models under filtered colimits and determine its [classifying topos](category-theory.md#classifying-topos).

### Finitely presented models of an algebraic theory

↑ **Parent:** [Algebraic theory](#algebraic-theory)

A finitely presented model is described by finitely many generators and finitely many equations. Model homomorphisms from it commute with filtered colimits. A small skeleton of these models is equivalent to the opposite of the finite-equation part of the algebraic syntactic category.

<h2 id="ehrenfeucht-fraisse-game">Ehrenfeucht-Fraïssé game</h2>

↑ **Parent:** [Model theory](model-theory.md)

In each round the Spoiler selects an element from either structure and the Duplicator responds in the other. The paired selected elements must preserve all atomic information and equality, giving a [partial isomorphism of structures](#partial-embedding). In the infinite game the Duplicator wins by avoiding failure at every finite stage. In a timed game the Spoiler first announces the number of rounds, allowing a different response strategy for each horizon.

### Interval threshold strategy for discrete linear orders

↑ **Parent:** [Ehrenfeucht-Fraïssé game](#ehrenfeucht-fraisse-game)

With $k$ moves remaining, preserve corresponding gap sizes exactly when smaller than $2^k-1$, and otherwise require both gaps to have at least that many points. One move splits a gap; $2^k-1=2(2^{k-1}-1)+1$ permits matching both smaller gaps. This strategy proves that $(\mathbb N,<)$ and $(\mathbb N+\mathbb Z,<)$ agree at every finite quantifier rank despite the second order containing points with infinitely many predecessors.

<h3 id="ehrenfeucht-fraisse-theorem">Ehrenfeucht-Fraïssé theorem</h3>

↑ **Parent:** [Ehrenfeucht-Fraïssé game](#ehrenfeucht-fraisse-game)

For a finite relational [first-order language](mathematical-logic.md#first-order-language), with finitely many constants allowed, the Duplicator wins the $n$-round game exactly when the structures are [rank-n equivalent](mathematical-logic.md#rank-n-equivalence-of-structures). Game-winning implies rank equivalence in arbitrary languages; the converse needs a finiteness condition and can fail even for an infinite unary vocabulary. Over a finite relational vocabulary, winning every announced finite horizon is equivalent to [elementary equivalence](#elementary-equivalence).

#### Failure of finite-round game equivalence in infinite languages

↑ **Parent:** [Ehrenfeucht-Fraïssé theorem](#ehrenfeucht-fraisse-theorem)

For countably many unary predicates $P_i$, let $M$ contain infinitely many copies of each finite membership pattern and let $N$ add an element satisfying all predicates. Every finite vocabulary reduct has infinitely many elements in every Boolean cell in both structures, so $M\equiv N$. The Spoiler nevertheless wins the one-round full-language game by selecting the new element, whose complete atomic pattern has no counterpart in $M$.

## Theory of formally real fields

↑ **Parent:** [Model theory](model-theory.md)

The theory of formally real fields consists of the [field](algebra.md#field) axioms and all sentences asserting that $-1$ is not a sum of $m$ squares, one for each positive integer $m$. The [real closure theorem](algebra.md#real-closure-theorem) and model completeness make the [Theory of real closed fields](#theory-of-real-closed-fields) its [model companion](#model-companion).

## Theory of nontrivial torsion-free divisible Abelian groups

↑ **Parent:** [Model theory](model-theory.md)

This [first-order theory](mathematical-logic.md#first-order-theory) has as models the nonzero [torsion-free divisible Abelian groups](group.md#torsion-free-divisible-abelian-group). Rational division equips them with the structure of [vector spaces over the rational numbers](vector-space.md#vector-space-over-the-rational-numbers). A [rational divisible hull](group.md#rational-divisible-hull) gives an [algebraically prime extension](#algebraically-prime-extension) of each nonzero torsion-free base, while the zero base uses a one-dimensional rational space.

### Theory of torsion-free divisible Abelian groups allowing the trivial group

↑ **Parent:** [Theory of nontrivial torsion-free divisible Abelian groups](#theory-of-nontrivial-torsion-free-divisible-abelian-groups)

Remove the nonzero-model axiom from [DAG](#theory-of-nontrivial-torsion-free-divisible-abelian-groups). The inclusion $\{0\}\subseteq\mathbb Q$ is then an inclusion of models but is not a [simple closure](mathematical-logic.md#simple-closure), because $x\ne0$ has a witness only in the larger model. The theory does not have [quantifier elimination](#quantifier-elimination): all closed group terms are zero, so no quantifier-free sentence distinguishes the two models.

## Algebraically prime extension

↑ **Parent:** [Model theory](model-theory.md)

For a [first-order theory](mathematical-logic.md#first-order-theory) $T$ and $A\models T_\forall$, an algebraically prime extension is a [structure embedding](mathematical-logic.md#structure-embedding) $i:A\to P\models T$ such that every embedding $j:A\to N\models T$ factors as $j=h\circ i$ for some [structure embedding](mathematical-logic.md#structure-embedding) $h:P\to N$. The embeddings need not be elementary or unique. A theory has algebraically prime models when every such $A$ has an extension of this kind.

## Reduced product

↑ **Parent:** [Model theory](model-theory.md)

Given nonempty [first-order structures](mathematical-logic.md#first-order-structure) $\mathcal M_i$ and a proper [filter on a set](set-theory.md#filter-set-theory) $F$, a reduced product identifies product functions $f,g$ when $\{i:f(i)=g(i)\}\in F$. Operations are interpreted coordinatewise, and relations hold when their coordinate truth sets belong to $F$. For an [ultrafilter](set-theory.md#ultrafilter) this is an [ultraproduct](#ultraproduct). [Primitive positive formulas](mathematical-logic.md#primitive-positive-formula) transfer through an arbitrary proper filter, whereas [logical disjunction](mathematical-logic.md#logical-disjunction) and [logical negation](theoretical-computer-science.md#negation) can fail to transfer.

## Elementary equivalence

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elementary_equivalence)

Two [first-order structures](mathematical-logic.md#first-order-structure) are elementarily equivalent when they satisfy the same [first-order sentences](mathematical-logic.md#first-order-sentence). They need not be isomorphic or embed into one another. Every [elementary embedding](set-theory.md#elementary-embedding) implies [elementary equivalence](#elementary-equivalence) of its source and target.

## Monster model

↑ **Parent:** [Model theory](model-theory.md)

A monster model is a fixed sufficiently saturated and strongly homogeneous model of a complete theory, of a cardinality much larger than every parameter set under discussion.

### Orbit of a definable set in a monster model

↑ **Parent:** [Monster model](#monster-model)

If $\mathcal D=\phi(\mathcal U,b)$, its automorphism orbit consists of the sets $\phi(\mathcal U,f(b))$. If this orbit is infinite, saturation constructs $|\mathcal U|$ pairwise distinct conjugates, so $|O(\mathcal D)|=|\mathcal U|$.

## Complete theory

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_theory)

A consistent first-order theory is complete when it decides every sentence in its language.

### Categorical theory

↑ **Parent:** [Complete theory](#complete-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Categorical_theory)

A theory is $\kappa$-categorical when all of its models of cardinality $\kappa$ are isomorphic.

#### Omega-categorical theory

↑ **Parent:** [Categorical theory](#categorical-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Omega-categorical_theory)

An aleph-zero-categorical theory has, up to isomorphism, exactly one countably infinite model.

##### Ryll-Nardzewski theorem

↑ **Parent:** [Omega-categorical theory](#omega-categorical-theory)

For a complete theory with infinite models in a countable language, the following are equivalent: the theory is aleph-zero-categorical; every type space $S_n(T)$ is finite; and for every $n$ there are only finitely many formulas in $n$ variables modulo the theory.

###### Reduct of an aleph-zero-categorical theory

↑ **Parent:** [Ryll-Nardzewski theorem](#ryll-nardzewski-theorem)

Every reduct of an aleph-zero-categorical theory to a sublanguage is aleph-zero-categorical. There can only be fewer formulas in each arity, so the finite-formula characterization in the [Ryll-Nardzewski theorem](#ryll-nardzewski-theorem) is preserved.

#### Morley categoricity theorem

↑ **Parent:** [Categorical theory](#categorical-theory)

This theorem is the uncountable categoricity theorem for a [categorical theory](#categorical-theory). If a countable first-order theory is categorical in one uncountable cardinal, then it is categorical in every uncountable cardinal.

#### Reduct need not preserve uncountable categoricity

↑ **Parent:** [Categorical theory](#categorical-theory)

Let a language partition the universe into two infinite unary predicates and include a bijection between them. Its complete theory is categorical in every infinite cardinal. The reduct forgetting the bijection is not categorical in any uncountable cardinal, because the two infinite parts can have different cardinalities.

#### Nonstandard model of the additive integers

↑ **Parent:** [Categorical theory](#categorical-theory)

Compactness gives a countable model elementarily equivalent to $(\mathbb Z,+,0)$ that contains a nonzero element divisible by every positive standard integer. It is not isomorphic to $\mathbb Z$, so $\operatorname{Th}(\mathbb Z,+,0)$ is not aleph-zero-categorical.

#### Aleph-zero-categoricity of an infinite-dimensional vector space over a finite field

↑ **Parent:** [Categorical theory](#categorical-theory)

The complete theory of infinite-dimensional vector spaces over a fixed finite field is aleph-zero-categorical: every countably infinite model has countably infinite dimension and is therefore isomorphic to every other such model.

## Diagram (mathematical logic)

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diagram_(mathematical_logic))

The diagram of $M$ is the set of atomic and negated atomic sentences true in the expansion by constants naming every element of $M$. Its elementary diagram contains every sentence true in that expansion. Models of these diagrams correspond respectively to embeddings and elementary embeddings of $M$.

### Elementary diagram of a structure

↑ **Parent:** [Diagram (mathematical logic)](#diagram-mathematical-logic)

The elementary diagram of $M$ is the set of all first-order sentences true in the expansion of $M$ by a constant symbol for each element. A model of the elementary diagram contains an elementary copy of $M$.

### Method of diagrams

↑ **Parent:** [Diagram (mathematical logic)](#diagram-mathematical-logic)

The method of diagrams adds the diagram or elementary diagram of a structure to a theory and applies compactness. A resulting model supplies an embedding or elementary embedding of the named structure.

#### Diagram embedding criterion for universal theories

↑ **Parent:** [Method of diagrams](#method-of-diagrams)

A [first-order structure](mathematical-logic.md#first-order-structure) $A$ embeds into a model of $T$ exactly when $A\models T_\forall$. For the nontrivial direction apply the [compactness theorem](mathematical-logic.md#compactness-theorem) to $T\cup\operatorname{Diag}(A)$. If a finite diagram conjunction were inconsistent with $T$, its universal negation after replacing the new constants by variables would belong to $T_\forall$ and contradict its truth in $A$.

#### Finitely satisfiable type is realized in an elementary extension

↑ **Parent:** [Method of diagrams](#method-of-diagrams)

If a type $p(x)$ over a structure $M$ is finitely satisfiable in $M$, then the elementary diagram of $M$ together with $p(c)$ is finitely satisfiable. Compactness gives an elementary extension of $M$ realizing $p$.

## Inductive first-order theory

↑ **Parent:** [Model theory](model-theory.md)

A first-order theory is inductive when unions of chains of its models under embeddings remain models. A theory is inductive exactly when it has an axiomatization by sentences of the form $\forall\bar x\,\exists\bar y\,\varphi(\bar x,\bar y)$ with quantifier-free $\varphi$.

## Model-complete theory

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Model-complete_theory)

A theory is model-complete when every embedding between its models is elementary. Every model-complete theory is inductive and hence admits a forall-exists axiomatization.

### Model companion

↑ **Parent:** [Model-complete theory](#model-complete-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Model_companion)

A model companion of $T$ is a [model-complete theory](#model-complete-theory) $T^*$ in the same language with $T^*_\forall=T_\forall$. Equivalently each model of either theory embeds into a model of the other. Alternating these embeddings and using the [elementary chain theorem](#elementary-chain-theorem) proves uniqueness up to logical equivalence. A model companion need not be a syntactic extension of its original theory.

### Theory of real closed fields

↑ **Parent:** [Model-complete theory](#model-complete-theory)

This is the complete [first-order theory](mathematical-logic.md#first-order-theory) of [real closed fields](algebra.md#real-closed-field).

The theory of real closed fields is complete and model-complete. In the language of ordered rings it eliminates quantifiers; in the pure language of rings its definable order prevents quantifier elimination.

#### Quantifier elimination for ordered real closed fields

↑ **Parent:** [Theory of real closed fields](#theory-of-real-closed-fields)

In the language of ordered rings, the [Theory of real closed fields](#theory-of-real-closed-fields) has [quantifier elimination](#quantifier-elimination). In its pure ring reduct the order is definable by nonzero squares, so model completeness survives, although quantifier elimination does not. Keeping these two language conventions separate is essential when constructing a [model companion](#model-companion).

#### Non-Archimedean real closed field

↑ **Parent:** [Theory of real closed fields](#theory-of-real-closed-fields)

A non-Archimedean real closed field contains a positive element larger than every standard integer. Compactness constructs one by adjoining a constant $c$ and the formulas $c>n$ for all natural numbers $n$.

<h4 id="model-theoretic-proof-of-hilbert-s-seventeenth-problem">Model-theoretic proof of Hilbert's seventeenth problem</h4>

↑ **Parent:** [Theory of real closed fields](#theory-of-real-closed-fields)

Model completeness of real closed fields transfers positivity of a rational function from $\mathbb R$ to real closed extensions of $\mathbb R$. If the function were not a sum of squares, the Artin-Schreier ordering criterion would produce a real closure in which it is negative, giving a contradiction.

## Ehrenfeucht-Mostowski model

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ehrenfeucht-Mostowski_model)

An Ehrenfeucht-Mostowski model is generated, often as a Skolem hull, by a sequence of order indiscernibles whose finite order types determine their types.

### Order-indiscernible sequence

↑ **Parent:** [Ehrenfeucht-Mostowski model](#ehrenfeucht-mostowski-model)

A sequence $(a_i)_{i\in I}$ indexed by a [total order](set.md#total-order) is order-indiscernible when any two increasing finite subsequences of the same length satisfy the same first-order formulas.

### Ehrenfeucht-Mostowski theorem

↑ **Parent:** [Ehrenfeucht-Mostowski model](#ehrenfeucht-mostowski-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ehrenfeucht–Mostowski_theorem)

Let $M$ be an infinite [first-order structure](mathematical-logic.md#first-order-structure) and $I$ a [total order](set.md#total-order). After choosing a [Skolem expansion](mathematical-logic.md#skolem-expansion) of $M$, an [elementary extension](#elementary-extension) contains distinct elements $(a_i)_{i\in I}$ forming an [order-indiscernible sequence](#order-indiscernible-sequence) in that expanded language. Their [Skolem hull](mathematical-logic.md#skolem-hull) is an [elementary substructure](mathematical-logic.md#elementary-substructure) in the expanded language, and its reduct is a [first-order model](mathematical-logic.md#model-of-a-first-order-theory) of $\operatorname{Th}(M)$. Every [order automorphism](set.md#order-automorphism) of $I$ extends uniquely to a [structure automorphism](mathematical-logic.md#automorphism-of-a-first-order-structure) of the hull preserving the chosen [Skolem expansion](mathematical-logic.md#skolem-expansion), by transporting terms in the generators.

Uniqueness need not hold among all [structure automorphisms](mathematical-logic.md#automorphism-of-a-first-order-structure) of the reduct. For an infinite structure in the pure [logical equality](mathematical-logic.md#logical-equality) language, take two distinct nullary [Skolem function](mathematical-logic.md#skolem-function) values $c_0,c_1$ in the hull. For an infinite [order-indiscernible sequence](#order-indiscernible-sequence), neither can equal a generator: the expanded formula $x=c_j$ would otherwise hold at every generator, contradicting their distinctness. Swapping $c_0,c_1$ fixes every generator and preserves the pure [logical equality](mathematical-logic.md#logical-equality) reduct, while failing to preserve the [Skolem expansion](mathematical-logic.md#skolem-expansion). Thus the identity [order automorphism](set.md#order-automorphism) already has two extensions in that reduct.

#### Ultraproduct proof of the Ehrenfeucht-Mostowski theorem

↑ **Parent:** [Ehrenfeucht-Mostowski theorem](#ehrenfeucht-mostowski-theorem)

Expand an infinite [first-order structure](mathematical-logic.md#first-order-structure) by [Skolem functions](mathematical-logic.md#skolem-function), choose distinct elements $b_n$, and fix a [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) $\mathcal U$ on $\mathbb N$. For each finite subset $F$ of the required index order, form the [ultrapower](#ultrapower) over $\mathbb N^F$ using the ordered [Fubini product of ultrafilters](set-theory.md#fubini-product-of-ultrafilters). Pullback along coordinate projections gives coherent elementary maps by the [Łoś theorem](#los-theorem). In their [directed limit of elementary embeddings](#directed-limit-of-elementary-embeddings), the classes of the coordinate [functions](function.md) $\mathbf n\mapsto b_{n_i}$ are distinct and form an [order-indiscernible sequence](#order-indiscernible-sequence); every [first-order formula](mathematical-logic.md#first-order-formula) on increasing coordinates has the same nested [ultrafilter](set-theory.md#ultrafilter) test. Their [Skolem hull](mathematical-logic.md#skolem-hull) gives an [Ehrenfeucht-Mostowski model](#ehrenfeucht-mostowski-model). An index-[order automorphism](set.md#order-automorphism) sends a term in the generators to the same term in the transported generators; indiscernibility makes this well defined. Uniqueness is in the specified [Skolem expansion](mathematical-logic.md#skolem-expansion), not necessarily in its reduct. If generators must respect a definable infinite order, first produce an increasing [sequence](sequence-and-series.md#sequence) by an [ultrapower](#ultrapower) of finite increasing chains.

#### Models with arbitrarily large automorphism groups

↑ **Parent:** [Ehrenfeucht-Mostowski theorem](#ehrenfeucht-mostowski-theorem)

Every first-order theory with an infinite model has models whose [automorphism groups](mathematical-logic.md#automorphism-group-of-a-first-order-structure) have arbitrarily large cardinality. Choose a total order with many order automorphisms and apply the [Ehrenfeucht-Mostowski theorem](#ehrenfeucht-mostowski-theorem).

## Prime model

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_model)

A prime model of a complete theory elementarily embeds into every model of that theory.

### Atomic model

↑ **Parent:** [Prime model](#prime-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Atomic_model)

A model is atomic when the complete type over the empty set of every finite tuple is isolated. For a complete theory in a countable language, a model is prime exactly when it is countable and atomic.

#### Countable atomic model without a countable saturated model

↑ **Parent:** [Atomic model](#atomic-model)

Take a countable structure with countably many independent unary predicates, every finite predicate pattern realized infinitely often, and a constant naming every element. Its complete theory has an [atomic model](#atomic-model): tuples of named elements have types isolated by equations to their names. But every infinite binary predicate pattern, together with inequalities to every named element, is consistent. There are uncountably many such one-types, so no countable [omega-saturated model](#omega-saturated-model) exists. Thus existence of a countable atomic model does not imply existence of a countable saturated one.

#### Countable atomic model is prime

↑ **Parent:** [Atomic model](#atomic-model)

A countable atomic model of a complete theory elementarily embeds into every model. Enumerate it and recursively extend a finite partial elementary map; an isolating formula for the next joint type guarantees a realization in the target.

#### One-point extension between atomic models

↑ **Parent:** [Atomic model](#atomic-model)

If $M,N$ are infinite atomic models of a complete theory and a finite partial elementary map sends $\bar a$ to $\bar b$, then for every $c\in M$ there is $d\in N$ extending it by $c\mapsto d$. An isolating formula for $\operatorname{tp}(\bar a,c)$ supplies $d$. Back-and-forth therefore makes any two countable atomic models isomorphic.

## Quantifier elimination

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantifier_elimination)

A theory has quantifier elimination when every formula is equivalent modulo the theory to a quantifier-free formula.

### Extension axioms for an unrestricted binary relation

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)

For a binary relation with no symmetry or loop restrictions, an extension axiom demands a fresh element realizing any prescribed choices of incoming edges, outgoing edges and its own loop relative to a finite list of distinct parameters. All such axioms together eliminate quantifiers: the quantifier-free type of a parameter tuple determines which witness patterns can occur. These axioms differ from the undirected loop-free [theory of the random graph](#theory-of-the-random-graph).

### Common-substructure test for quantifier elimination

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)

A theory $T$ eliminates quantifiers if, whenever two models of $T$ contain isomorphic copies of the same substructure $A$, they satisfy the same formulas over $A$. Equivalently, $T\cup D(A)$ is complete for every substructure of a model of $T$.

#### Existential common-substructure test for quantifier elimination

↑ **Parent:** [Common-substructure test for quantifier elimination](#common-substructure-test-for-quantifier-elimination)

For a [first-order theory](mathematical-logic.md#first-order-theory) $T$, suppose every existential [quantifier-free formula](mathematical-logic.md#quantifier-free-formula) over a common [substructure](mathematical-logic.md#substructure-of-a-first-order-structure) has a witness in either of two $T$-models exactly when it has one in the other. Then $T$ has [quantifier elimination](#quantifier-elimination). One may test a single quantified variable, since elimination of these formulas inductively eliminates all quantifiers. A language with a constant avoids empty-generated-substructure and quantifier-free-sentence conventions.

##### Algebraically prime extension test for quantifier elimination

↑ **Parent:** [Existential common-substructure test for quantifier elimination](#existential-common-substructure-test-for-quantifier-elimination)

If $T$ has [algebraically prime models](#algebraically-prime-extension) and every inclusion between models of $T$ is a [simple closure](mathematical-logic.md#simple-closure), then $T$ has [quantifier elimination](#quantifier-elimination). For a common base $A$, embed its algebraically prime extension into both models. Simple closure transfers a witness into that extension; the second embedding transfers it to the other model.

### Partial embedding

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)

A partial embedding is an injective map between subsets of structures that preserves and reflects atomic formulas. It therefore preserves every quantifier-free formula.

### Quantifier elimination for algebraically closed fields

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)

The theory of algebraically closed fields of a fixed characteristic eliminates quantifiers in the language of rings. Over a parameter field $F$, the complete type of a tuple is determined by the prime ideal of polynomial relations it satisfies.

#### Type space of an algebraically closed field over a subfield

↑ **Parent:** [Quantifier elimination for algebraically closed fields](#quantifier-elimination-for-algebraically-closed-fields)

Complete $n$-types over a subfield $F$ of an algebraically closed field correspond to prime ideals of $F[X_1,\ldots,X_n]$, or equivalently to generic points of irreducible affine varieties over $F$. The Stone topology corresponds to the constructible topology: polynomial equalities and inequalities define basic clopen sets.

### Theory of the random graph

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)

The theory of the random graph says that the edge relation is irreflexive and symmetric and that, for every two finite disjoint vertex sets, a new vertex is adjacent to every vertex of the first and none of the second.

#### Quantifier elimination for the random graph

↑ **Parent:** [Theory of the random graph](#theory-of-the-random-graph)

Every small partial embedding of a monster random graph extends by back-and-forth to an automorphism, using saturation and the extension axioms. It is therefore elementary, and the theory of the random graph eliminates quantifiers.

#### Algebraic and definable closure in the random graph

↑ **Parent:** [Theory of the random graph](#theory-of-the-random-graph)

For every small set $A$ in a monster random graph,

$$
\operatorname{acl}(A)=\operatorname{dcl}(A)=A.
$$

Any vertex outside $A$ has infinitely many conjugates over $A$ with the same adjacency pattern.

#### Three-type space of the random graph

↑ **Parent:** [Theory of the random graph](#theory-of-the-random-graph)

The three-types of the random graph are determined by equality and adjacency among three variables. There is one all-equal type, six types with exactly two variables equal, and eight types with all variables distinct, for a total of fifteen.

### Back-and-forth method

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Back-and-forth_method)

The back-and-forth method constructs an isomorphism by alternately extending finite partial isomorphisms to include elements from each structure.

#### Effective back-and-forth construction

↑ **Parent:** [Back-and-forth method](#back-and-forth-method)

An effective back-and-forth construction alternately extends a finite [partial isomorphism of structures](#partial-embedding) to include the least unused domain and range elements, searching computably for a compatible extension. If extension always exists and its finite compatibility conditions are decidable, the union is a [computable isomorphism](#computable-isomorphism). Decidable presentations of a [dense linear order without endpoints](#dense-linear-order-without-endpoints) provide a basic example.

### Dense linear order without endpoints

↑ **Parent:** [Quantifier elimination](#quantifier-elimination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dense_linear_order_without_endpoints)

A dense linear order without endpoints is a linear order in which a third point lies strictly between every two distinct points and every point has points both below and above it.

#### Ehrenfeucht theory of an increasing named sequence

↑ **Parent:** [Dense linear order without endpoints](#dense-linear-order-without-endpoints)

Add constants $c_0<c_1<\cdots$ to the theory of [dense linear orders without endpoints](#dense-linear-order-without-endpoints). The three countable models have respectively a least upper bound for the named sequence, no upper bound, or upper bounds with no least one. The unbounded model is an [atomic model](#atomic-model); the bounded model with no least upper bound is an [omega-saturated model](#omega-saturated-model). The remaining model omits the type $c_i<x<d$ over its least-upper-bound parameter $d$.

#### Suslin line

↑ **Parent:** [Dense linear order without endpoints](#dense-linear-order-without-endpoints)

A complete [dense linear order without endpoints](#dense-linear-order-without-endpoints) with the [countable chain condition for a linear order](set.md#countable-chain-condition-for-a-linear-order), but with no countable [order-dense subset](set.md#order-dense-subset).

##### Suslin hypothesis

↑ **Parent:** [Suslin line](#suslin-line)

The assertion that there is no [Suslin line](#suslin-line), equivalently that every complete dense linear order without endpoints satisfying the interval countable chain condition is separable. A [Suslin tree](set.md#suslin-tree) gives a counterexample.

#### Quantifier elimination for dense linear orders without endpoints

↑ **Parent:** [Dense linear order without endpoints](#dense-linear-order-without-endpoints)

The theory of dense linear orders without endpoints eliminates quantifiers. A finite partial order isomorphism extends by placing each new point in the corresponding interval or ray.

## Ultraproduct

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultraproduct)

An ultraproduct identifies two sequences when they agree on a set belonging to an ultrafilter and interprets symbols coordinatewise.

### Countable saturation of an ultraproduct over omega

↑ **Parent:** [Ultraproduct](#ultraproduct)

An [ultraproduct](#ultraproduct) over a [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) on $\omega$ realizes each countable finitely satisfiable type. For the first $n$ formulas, their coordinate simultaneous-witness set $E_n$ belongs to the ultrafilter by the [Łoś theorem](#los-theorem). Replace it by $E_n\cap[n,\infty)$ and choose at coordinate $i$ a witness to as many initial formulas as that coordinate permits. This finite number tends to infinity modulo the ultrafilter, so the resulting product class realizes every formula. More generally countably incomplete ultrafilters admit the same descending-set diagonalization. This statement does not assert saturation at every larger cardinal.

### Ultrapower

↑ **Parent:** [Ultraproduct](#ultraproduct)

An ultrapower is an [ultraproduct](#ultraproduct) whose factors are all one structure $M$. Its elements are equivalence classes $[f]$ of functions $f:I\to M$, where $f\sim g$ exactly when $\{i\in I:f(i)=g(i)\}$ belongs to the chosen [ultrafilter](set-theory.md#ultrafilter) $\mathcal U$.

#### Model-theoretic ultralimit

↑ **Parent:** [Ultrapower](#ultrapower)

An ultralimit is the direct limit of a chain of structures formed by taking successive [ultrapowers](#ultrapower) along their diagonal [elementary embeddings](set-theory.md#elementary-embedding). At limit stages use the [elementary chain theorem](#elementary-chain-theorem). This is a different concept from a topological [ultrafilter limit](set-theory.md#ultralimit). Alternating relative ultrapower embeddings constructs isomorphic ultralimits of any two elementarily equivalent structures, without requiring the stronger single-ultrapower isomorphism theorem.

##### Alternating ultrapowers give isomorphic ultralimits

↑ **Parent:** [Model-theoretic ultralimit](#model-theoretic-ultralimit)

The [Frayne embedding lemma](#frayne-embedding-lemma) embeds $B$ into an [ultrapower](#ultrapower) $A_1$ of $A$. Its relative version embeds $A_1$ into an ultrapower $B_1$ of $B$, fixing the diagonal copy of $B$. Continue alternately over the previously fixed elementary substructure. After coherent identifications one has $B\preceq A_1\preceq B_1\preceq A_2\preceq B_2\preceq\cdots$, while each $A_{n+1}$ is an ultrapower of $A_n$ along its diagonal map, and similarly for $B$. The two cofinal subsequences have the same elementary union. This proves the ultralimit assertion without the stronger single-ultrapower isomorphism theorem.

##### Frayne embedding lemma

↑ **Parent:** [Model-theoretic ultralimit](#model-theoretic-ultralimit)

If $A\equiv B$, the elementary diagram of $B$ is finitely satisfiable by interpreting its finitely many named elements in $A$. Choose those finite realizations as coordinates, extend the filter of diagram cones to an [ultrafilter](set-theory.md#ultrafilter), and use the [Łoś theorem](#los-theorem) to embed $B$ elementarily into an [ultrapower](#ultrapower) of $A$. If $A\prec B$, work over the named elements of $A$ and keep their coordinates constant. The resulting embedding extends the diagonal map of $A$. This relative assertion allows an alternating chain of ultrapowers to keep every previously embedded substructure fixed.

#### Diagonal argument for ultrapower cardinality

↑ **Parent:** [Ultrapower](#ultrapower)

If $U$ is a [kappa-complete](set-theory.md#kappa-complete-filter) [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) on $\kappa$ and $|M|\geq\kappa$, then $|M^\kappa/U|>\kappa$. Otherwise enumerate representatives $f_\alpha$ for its classes and choose $g(i)\notin\{f_\alpha(i):\alpha<i\}$. Every tail of $\kappa$ belongs to $U$, so $g$ differs modulo $U$ from every representative. The [small set is absent from a complete nonprincipal ultrafilter](set-theory.md#small-set-is-absent-from-a-complete-nonprincipal-ultrafilter) lemma supplies the tail property.

<h3 id="los-theorem">Łoś theorem</h3>

↑ **Parent:** [Ultraproduct](#ultraproduct)

This theorem characterizes truth in an [ultraproduct](#ultraproduct). Łoś's theorem says that a first-order formula holds in an ultraproduct exactly when it holds in a set of factors belonging to the ultrafilter.

#### Dense-extension filter semantics

↑ **Parent:** [Łoś theorem](#los-theorem)

For a family of [first-order structures](mathematical-logic.md#first-order-structure), take [free filters](set-theory.md#free-filter) on the index set as worlds, ordered by inclusion, and product sequences as parameters. Force an atom when its coordinate truth set belongs to the filter. Conjunction is local, implication and negation quantify over filter extensions, and a disjunction is forced when every extension has a further extension forcing one disjunct. Existence is witnessed by a product sequence and universality holds for all sequences at all extensions. With the [axiom of choice](set-theory.md#axiom-of-choice), induction on formulas identifies forcing with membership of the classical coordinate truth set. Equivalently, every ultrafilter extension satisfies the formula in its [ultraproduct](#ultraproduct). Thus the semantics validates classical logic. A local disjunction rule would fail this identification: a set and its complement can both be absent from a free filter, while their union is the whole index set.

#### Infinite field of positive characteristic from an ultraproduct

↑ **Parent:** [Łoś theorem](#los-theorem)

For a [prime number](prime-number.md) $p$, a [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) on $\mathbb N$ gives

$$
K=\prod_{n\geq1}\mathbb F_{p^n}/\mathcal U.
$$

The [Łoś theorem](#los-theorem) makes $K$ a [field](algebra.md#field) of [characteristic](algebra.md#characteristic-of-a-field) $p$. For every natural number $m$, almost all factors have at least $m$ elements, so $K$ is infinite.

## Elementary extension

↑ **Parent:** [Model theory](model-theory.md)

An [elementary extension](#elementary-extension) is an extension preserving all first-order truth with parameters, hence giving [elementary equivalence](#elementary-equivalence). An extension $N\supseteq M$ is elementary when every formula with parameters from $M$ has the same truth value in both structures.

### Saturated model

↑ **Parent:** [Elementary extension](#elementary-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Saturated_model)

A model $N$ is $\kappa$-saturated when every complete type over a subset of size less than $\kappa$ is realized in $N$.

#### Omega-saturated model

↑ **Parent:** [Saturated model](#saturated-model)

A model is omega-saturated when it realizes every complete finite-tuple type over any finite parameter set. Realizing all one-variable types over finite parameter sets suffices by successively adjoining coordinates. This is weaker than saturation over every countable parameter set.

#### Saturated elementary extension theorem

↑ **Parent:** [Saturated model](#saturated-model)

For every infinite regular [cardinal](cardinal-number.md) $\kappa$, every [first-order structure](mathematical-logic.md#first-order-structure) has a $\kappa$-saturated [elementary extension](#elementary-extension). At one stage use the [compactness theorem](mathematical-logic.md#compactness-theorem) with the [elementary diagram](#elementary-diagram-of-a-structure) to realize all [complete types](#complete-type) over [subsets](set.md#subset) of the stage having size less than $\kappa$. There is a [set](set.md) of such types; finite [subsets](set.md#subset) of the enlarged theory are satisfiable because their finitely many witnesses are independent. Iterate for $\kappa$ stages, taking elementary [unions](set.md#set-union) at limits. Regularity puts any parameter [set](set.md) of size less than $\kappa$ inside one stage, and its type is realized at the next one. Passing to a larger [regular cardinal](cardinal-number.md#regular-cardinal) covers singular requested degrees of saturation as well.

#### Countable saturation of a nonprincipal ultraproduct over omega

↑ **Parent:** [Saturated model](#saturated-model)

In a [countable](cardinal-number.md#countable-set) language, an [ultraproduct](#ultraproduct) over a [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) on $\omega$ realizes every [countable](cardinal-number.md#countable-set) finitely satisfiable type, including types over countably many parameters. Enumerate the type $\varphi_1,\varphi_2,\ldots$, and let $A_n$ be the ultrafilter-large [set](set.md) of coordinates where the first $n$ [first-order formulas](mathematical-logic.md#first-order-formula) have a simultaneous witness. Put $B_n=\{i:i\geq n\}\cap\bigcap_{j\leq n}A_j$. At coordinate $i$, choose a witness for the largest $n\leq i$ with $i\in B_n$, or an arbitrary element when there is none. For each fixed $n$, the resulting [function](function.md) satisfies the first $n$ [first-order formulas](mathematical-logic.md#first-order-formula) on $B_n$. The [Łoś theorem](#los-theorem) then realizes the entire type. Countability of the language and parameter [set](set.md) makes the enumeration possible.

#### Saturation implies homogeneity

↑ **Parent:** [Saturated model](#saturated-model)

A $\kappa$-saturated model has the one-point extension property for partial elementary maps of size below $\kappa$: transport the type of the new element through the map and realize it by saturation. This is $\kappa$-homogeneity; back-and-forth gives the corresponding automorphisms when cardinalities permit.

#### Homogeneity plus realization of empty-set types implies saturation

↑ **Parent:** [Saturated model](#saturated-model)

If an aleph-zero-homogeneous model realizes every finite type over the empty set, it is aleph-zero-saturated. Realize the joint empty-set type of the parameters and a desired element, then use homogeneity to move the realized parameter tuple to the given one.

#### Universal model

↑ **Parent:** [Saturated model](#saturated-model)

A model $N$ of cardinality $\kappa$ is universal when every model of the same complete theory having cardinality less than $\kappa$ admits an elementary embedding into $N$.

#### Homogeneous model

↑ **Parent:** [Saturated model](#saturated-model)

A model $N$ of cardinality $\kappa$ is homogeneous when every partial elementary map between subsets of size less than $\kappa$ extends to an automorphism of $N$.

#### Universal homogeneous model is saturated

↑ **Parent:** [Saturated model](#saturated-model)

A universal homogeneous model realizes every type over a small parameter set. Embed a small model containing a realization into the universal model, then use homogeneity to move the embedded parameters back to the original ones.

#### Small elementary submodel meeting every definable equivalence class

↑ **Parent:** [Saturated model](#saturated-model)

Let $N$ be uncountable and saturated, and let a formula define an equivalence relation. If every small elementary submodel of $N$ meets every class, then there are only finitely many classes. Otherwise a small elementary submodel $M$ yields the finitely satisfiable type $\{\neg E(x,m):m\in M\}$, contradicting saturation.

### Elementary chain theorem

↑ **Parent:** [Elementary extension](#elementary-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elementary_chain_theorem)

The union of an elementary chain of structures has a unique induced structure, and every member of the chain is an elementary substructure of the union.

#### Directed limit of elementary embeddings

↑ **Parent:** [Elementary chain theorem](#elementary-chain-theorem)

A directed system of [first-order structures](mathematical-logic.md#first-order-structure) and coherent [elementary embeddings](set-theory.md#elementary-embedding) has a direct limit into which every member embeds elementarily. Represent an element by a pair consisting of a stage and an element at that stage; identify two representatives when their images agree at a common later stage. Interpret [functions](function.md) and relations at a common stage. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on [first-order formulas](mathematical-logic.md#first-order-formula) proves elementarity: for an existential [first-order formula](mathematical-logic.md#first-order-formula) true at the limit, its witness and parameters occur at a common stage, and elementarity pulls truth back to the stage containing the original parameters. This generalizes the [elementary chain theorem](#elementary-chain-theorem) beyond linearly ordered diagrams.

### Complete type

↑ **Parent:** [Elementary extension](#elementary-extension)

The complete type of a tuple over parameters records every formula over those parameters that the tuple satisfies.

#### Algebraic type

↑ **Parent:** [Complete type](#complete-type)

A complete type is algebraic when it contains a formula having finitely many realizations in a model of the theory. A one-element example is the type containing $x=c$ for a named constant. Such a type cannot gain infinitely many realizations in an [elementarily equivalent](#elementary-equivalence) structure. An [isolated type](#isolated-type) need not be algebraic: the unique empty-set one-type in a [dense linear order without endpoints](#dense-linear-order-without-endpoints) is isolated by $x=x$ and has infinitely many realizations.

#### Type space

↑ **Parent:** [Complete type](#complete-type)

With its standard topology, this [type space](#type-space) is a [Stone space](topology.md#stone-space). The type space $S_n^M(A)$ is the set of complete $n$-types over a parameter set $A$ that are consistent with the complete theory of $M$ together with its diagram over $A$.

##### Stone topology on a type space

↑ **Parent:** [Type space](#type-space)

For a [type space](#type-space) $S_n^M(A)$, the basic open set $[\varphi]$ consists of complete types containing the formula $\varphi$. These sets are clopen, satisfy $[\varphi]\cap[\psi]=[\varphi\wedge\psi]$, and distinguish distinct types. The [compactness theorem](mathematical-logic.md#compactness-theorem) makes this topology compact; it is Hausdorff and has a basis of clopen sets.

##### Isolated type

↑ **Parent:** [Type space](#type-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isolated_type)

A complete type $p\in S_n(A)$ is isolated when some formula $\varphi\in p$ belongs to no other complete type in $S_n(A)$. Equivalently, the basic open set determined by $\varphi$ is the singleton $\{p\}$.

###### Density of isolated types from a prime model

↑ **Parent:** [Isolated type](#isolated-type)

If a complete countable theory has a prime model, isolated types are dense in every finite-arity type space. Every nonempty basic open set is realized in the prime model, whose finite tuples have isolated types.

##### Omitted type

↑ **Parent:** [Type space](#type-space)

A type $p(x_1,\ldots,x_n)$ is omitted in a structure $M$ when no tuple from $M^n$ realizes every formula in $p$.

###### Omitting types theorem

↑ **Parent:** [Omitted type](#omitted-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Omitting_types_theorem)

Let $T$ be a consistent theory in a countable first-order language. For every countable family of nonisolated finite-arity types of $T$, there is a countable model of $T$ that omits every type in the family.

###### Henkin omission extension lemma

↑ **Parent:** [Omitting types theorem](#omitting-types-theorem)

Let $p(\mathbf x)$ be a [nonprincipal partial type](mathematical-logic.md#nonprincipal-partial-type) over a consistent [first-order theory](mathematical-logic.md#first-order-theory) $T$. Suppose $T\cup\{\sigma(\mathbf c)\}$ is consistent, with $\sigma$ a finite condition in finitely many new constants, and let $\mathbf t(\mathbf c)$ be a tuple of closed terms. Some $\psi\in p$ leaves $T\cup\{\sigma(\mathbf c),\neg\psi(\mathbf t(\mathbf c))\}$ consistent. Otherwise the original-language [first-order formula](mathematical-logic.md#first-order-formula)

$$
\theta(\mathbf x)=\exists\mathbf z\bigl(\sigma(\mathbf z)\land\mathbf x=\mathbf t(\mathbf z)\bigr)
$$

is consistent with $T$ and entails every member of $p$, contradicting nonprincipality. Replace all new constants occurring in the condition or terms by variables. This lemma makes the omission requirements dense in a countable [Henkin construction](mathematical-logic.md#henkin-construction).

##### Realization of a type in an elementary extension

↑ **Parent:** [Type space](#type-space)

Every complete type over parameters from $M$ is realized in some elementary extension of $M$. Apply compactness to the elementary diagram of $M$ together with a new tuple of constants satisfying the type.

##### Total disconnectedness of a type space

↑ **Parent:** [Type space](#type-space)

Distinct complete types contain opposite choices $\varphi$ and $\neg\varphi$. The corresponding basic clopen sets partition the type space, so every type space is totally disconnected.

##### One-types over the natural numbers in the rational order

↑ **Parent:** [Type space](#type-space)

Quantifier elimination for dense linear orders shows that the one-types over $\mathbb N\subset\mathbb Q$ are determined by cuts: equality to a natural number, one of the intervals between consecutive natural numbers, the ray below zero, or the cut above every natural number. Only the last type is non-isolated.

#### Aleph-zero-homogeneous model

↑ **Parent:** [Complete type](#complete-type)

A model is aleph-zero-homogeneous when every finite partial elementary map extends by one more element.

## Stable theory

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stable_theory)

A complete theory is $\kappa$-stable when $|S_1(A)|\leq\kappa$ for every parameter set $A$ of cardinality $\kappa$. It is omega-stable when this holds for $\kappa=\aleph_0$.

### Fundamental theorem of stability

↑ **Parent:** [Stable theory](#stable-theory)

For a complete theory, the following are equivalent: the theory is stable; no formula has the [order property](#order-property); and every complete type over every model is definable.

#### Definable type

↑ **Parent:** [Fundamental theorem of stability](#fundamental-theorem-of-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Definable_type)

A type $p(x)$ over a model $M$ is definable when, for every formula $\varphi(x;y)$, there is an $M$-formula $d_p\varphi(y)$ such that

$$
\varphi(x;b)\in p
\quad\Longleftrightarrow\quad
M\models d_p\varphi(b)
$$

for every tuple $b$ from $M$.

##### Stable trace of a definable set

↑ **Parent:** [Definable type](#definable-type)

If $T$ is stable, $M\preccurlyeq N\models T$, and $X\subseteq N^n$ is definable with parameters from $N$, then $X\cap M^n$ is definable with parameters from $M$. Apply definability of the type over $M$ of the parameter defining $X$.

### Omega-stability implies stability in every infinite cardinal

↑ **Parent:** [Stable theory](#stable-theory)

For a countable theory, omega-stability implies $|S_n(A)|\leq|A|+\aleph_0$ for every parameter set $A$. Total transcendence gives each type a finite base and a definition over it; counting finite bases and formulas proves the bound.

### Order property

↑ **Parent:** [Stable theory](#stable-theory)

A formula $\phi(\bar x,\bar y)$ has the order property for $T$ when arbitrarily long tuples $(a_i),(b_j)$ exist with $\phi(a_i,b_j)$ exactly when $i<j$. Compactness realizes this pattern along every linear order.

#### Order property implies instability

↑ **Parent:** [Order property](#order-property)

If a theory has the order property, a linear order with more than $\kappa$ cuts over a dense subset of size at most $\kappa$ produces more than $\kappa$ distinct types over that subset. Hence a theory with the order property is not $\kappa$-stable for any $\kappa\geq|T|$.

## Strongly minimal theory

↑ **Parent:** [Model theory](model-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strongly_minimal_theory)

A complete theory is strongly minimal when every definable one-variable subset of every model is finite or cofinite.

### Model-theoretic algebraic closure

↑ **Parent:** [Strongly minimal theory](#strongly-minimal-theory)

An element belongs to $\operatorname{acl}(A)$ when it lies in a finite set definable with parameters from $A$.

#### Model-theoretic definable closure

↑ **Parent:** [Model-theoretic algebraic closure](#model-theoretic-algebraic-closure)

An element belongs to $\operatorname{dcl}(A)$ when it is the unique realization of some formula with parameters from $A$. Equivalently, it is fixed by every automorphism fixing $A$ pointwise.

#### Pregeometry

↑ **Parent:** [Model-theoretic algebraic closure](#model-theoretic-algebraic-closure)

A [pregeometry](#pregeometry) is a finitary closure structure with the exchange axiom, extending the closure description of a [matroid](combinatorics.md#matroid) to possibly infinite underlying sets. A pregeometry is a closure operator with finite character and exchange. Algebraic closure in a strongly minimal theory is a pregeometry.

##### Basis of a pregeometry

↑ **Parent:** [Pregeometry](#pregeometry)

A basis of a pregeometry is a maximal independent set. Every element lies in the closure of a basis, and the exchange property implies that all bases have the same cardinality.

###### Dimension of a pregeometry

↑ **Parent:** [Basis of a pregeometry](#basis-of-a-pregeometry)

The dimension of a closed set over a smaller closed set is the cardinality of any basis of the larger set over the smaller one. The exchange property makes this cardinality independent of the chosen basis.

##### Generic type in a strongly minimal theory

↑ **Parent:** [Pregeometry](#pregeometry)

Over an algebraically closed parameter set in a strongly minimal theory, there is a unique nonalgebraic one-type. It is called the generic type: its realizations are precisely the elements outside the algebraic closure of the parameters.

##### Independent set in a strongly minimal theory

↑ **Parent:** [Pregeometry](#pregeometry)

A set is independent when no element lies in the algebraic closure of the others. Every bijection between independent sets in a strongly minimal monster model is elementary because successive independent elements realize the unique generic type over the algebraic closure of their predecessors.

### Homogeneity of models of a countable strongly minimal theory

↑ **Parent:** [Strongly minimal theory](#strongly-minimal-theory)

In a countable strongly minimal theory, every model is homogeneous. Extend a finite partial elementary map over algebraic closures, choose bases of equal dimension for the remaining pregeometry, map one basis bijectively to the other, and extend over algebraic closure.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Mathematical logic](mathematical-logic.md)
