# Module theory

↑ **Parent:** [Commutative algebra](commutative-algebra.md)

Module theory extends linear algebra by allowing scalars from a ring rather than only a field.

**Table of contents**

- [Finite representation type](#finite-representation-type)
- [Auslander–Reiten quiver](#auslander-reiten-quiver)
  - [Stable Auslander–Reiten quiver](#stable-auslander-reiten-quiver)
- [Topological group module](#topological-group-module)
- [Character module](#character-module)
- [Representation of an associative algebra](#representation-of-an-associative-algebra)
  - [Representation of a Banach algebra](#representation-of-a-banach-algebra)
    - [Algebraically irreducible representation of a Banach algebra](#algebraically-irreducible-representation-of-a-banach-algebra)
      - [Countable annihilation sequence in an irreducible Banach module](#countable-annihilation-sequence-in-an-irreducible-banach-module)
      - [Quotient norm on an irreducible Banach module](#quotient-norm-on-an-irreducible-banach-module)
    - [Normed representation of a Banach algebra](#normed-representation-of-a-banach-algebra)
      - [Johnson's continuity theorem for irreducible normed representations](#johnson-s-continuity-theorem-for-irreducible-normed-representations)
- [Degeneration of a module](#degeneration-of-a-module)
- [Hereditary ring](#hereditary-ring)
  - [Basic hereditary algebra path-algebra theorem](#basic-hereditary-algebra-path-algebra-theorem)
  - [Path algebras are hereditary](#path-algebras-are-hereditary)
- [Regular sequence on a module](#regular-sequence-on-a-module)
- [Composition series of a module](#composition-series-of-a-module)
  - [Composition factor](#composition-factor)
- [Uniform module](#uniform-module)
  - [Uniform dimension](#uniform-dimension)
  - [Finite uniform decomposition of a Noetherian module](#finite-uniform-decomposition-of-a-noetherian-module)
- [Indecomposable module](#indecomposable-module)
  - [Top of an indecomposable projective module](#top-of-an-indecomposable-projective-module)
- [Fitting lemma](#fitting-lemma)
- [Krull–Schmidt theorem](#krull-schmidt-theorem)
  - [Krull-Schmidt decomposition](#krull-schmidt-decomposition)
- [Dual module](#dual-module)
  - [Double dual module](#double-dual-module)
- [Finitely generated module](#finitely-generated-module)
  - [Minimal number of generators of a module](#minimal-number-of-generators-of-a-module)
  - [Clearing denominators relative to an independent module subset](#clearing-denominators-relative-to-an-independent-module-subset)
  - [Finite generation as a quotient of a finite free module](#finite-generation-as-a-quotient-of-a-finite-free-module)
- [Artinian module](#artinian-module)
  - [Artinian modules are co-Hopfian](#artinian-modules-are-co-hopfian)
  - [Artinian modules in a short exact sequence](#artinian-modules-in-a-short-exact-sequence)
- [Filtered colimit of modules](#filtered-colimit-of-modules)
  - [Direct system of abelian groups](#direct-system-of-abelian-groups)
    - [Direct limit of abelian groups](#direct-limit-of-abelian-groups)
      - [Sequential direct limit of multiplication maps on the integers](#sequential-direct-limit-of-multiplication-maps-on-the-integers)
        - [Rational group with square-free denominators](#rational-group-with-square-free-denominators)
- [Bimodule](#bimodule)
- [Invariant submodule](#invariant-submodule)
- [Coinvariant module](#coinvariant-module)
  - [Abelianization over a Zp-extension](#abelianization-over-a-zp-extension)
- [Support of a module](#support-of-a-module)
- [Tensor product of modules](#tensor-product-of-modules)
  - [Right exactness of the tensor product](#right-exactness-of-the-tensor-product)
  - [Change-of-rings tensor quotient](#change-of-rings-tensor-quotient)
  - [Tensor product of commutative algebras](#tensor-product-of-commutative-algebras)
    - [Tensor product of field extensions is nonzero](#tensor-product-of-field-extensions-is-nonzero)
  - [Pure tensor](#pure-tensor)
  - [Projectivity of factors of a nonzero finite free tensor product](#projectivity-of-factors-of-a-nonzero-finite-free-tensor-product)
  - [Tensor-nilpotent module](#tensor-nilpotent-module)
  - [Balanced map](#balanced-map)
  - [Universal property of the tensor product of modules](#universal-property-of-the-tensor-product-of-modules)
  - [Tensor-hom adjunction](#tensor-hom-adjunction)
  - [Tensor product and infinite direct product](#tensor-product-and-infinite-direct-product)
- [Flat module](#flat-module)
  - [Flatness criterion over dual numbers](#flatness-criterion-over-dual-numbers)
  - [Equational criterion for flatness](#equational-criterion-for-flatness)
  - [Free modules are flat](#free-modules-are-flat)
  - [Direct summands of flat modules are flat](#direct-summands-of-flat-modules-are-flat)
  - [Flatness criterion using ideals](#flatness-criterion-using-ideals)
  - [Lambek theorem](#lambek-theorem)
  - [Faithfully flat module](#faithfully-flat-module)
  - [Flatness is local](#flatness-is-local)
  - [Torsion-free module over a principal ideal domain is flat](#torsion-free-module-over-a-principal-ideal-domain-is-flat)
  - [Flat extension preserves finite ideal intersections](#flat-extension-preserves-finite-ideal-intersections)
  - [Local tensor nonvanishing criterion](#local-tensor-nonvanishing-criterion)
- [Determinant trick](#determinant-trick)
- [Short exact sequence](#short-exact-sequence)
  - [Module extension](#module-extension)
    - [Extension of trivial modules for an infinite cyclic group](#extension-of-trivial-modules-for-an-infinite-cyclic-group)
    - [Pushout of a module extension](#pushout-of-a-module-extension)
    - [Equivalence of module extensions](#equivalence-of-module-extensions)
  - [Split short exact sequence](#split-short-exact-sequence)
  - [Short five lemma](#short-five-lemma)
- [Inverse system](#inverse-system)
  - [Inverse limit](#inverse-limit)
    - [Universal property of an inverse limit](#universal-property-of-an-inverse-limit)
    - [Nonemptiness theorem for inverse limits of finite sets](#nonemptiness-theorem-for-inverse-limits-of-finite-sets)
- [Filtration of a module](#filtration-of-a-module)
  - [Quotient filtration](#quotient-filtration)
  - [Subspace filtration](#subspace-filtration)
  - [Ascending filtration](#ascending-filtration)
  - [Good filtration of a module](#good-filtration-of-a-module)
    - [Dimension of a filtered module](#dimension-of-a-filtered-module)
      - [Multiplicity of a filtered module](#multiplicity-of-a-filtered-module)
        - [Dimension and multiplicity in a filtered exact sequence](#dimension-and-multiplicity-in-a-filtered-exact-sequence)
  - [Equivalent filtrations of a module](#equivalent-filtrations-of-a-module)
  - [I-adic topology](#i-adic-topology)
    - [I-adic filtration](#i-adic-filtration)
      - [Krull intersection theorem](#krull-intersection-theorem)
      - [x-adic filtration](#x-adic-filtration)
      - [Stable I-filtration](#stable-i-filtration)
      - [Rees algebra](#rees-algebra)
        - [Rees module](#rees-module)
      - [Artin-Rees lemma](#artin-rees-lemma)
  - [Filtered algebra](#filtered-algebra)
    - [Rees ring of a filtered algebra](#rees-ring-of-a-filtered-algebra)
    - [Almost commutative algebra](#almost-commutative-algebra)
      - [Degree-one almost commutative algebra](#degree-one-almost-commutative-algebra)
    - [Filtered ring](#filtered-ring)
      - [Filtration of a ring](#filtration-of-a-ring)
        - [Complete negative filtration](#complete-negative-filtration)
          - [Complete negative filtered-graded transfer of Noetherianity](#complete-negative-filtered-graded-transfer-of-noetherianity)
      - [Ascending filtered-graded transfer of Noetherianity](#ascending-filtered-graded-transfer-of-noetherianity)
      - [Filtered-graded transfer for complete rings](#filtered-graded-transfer-for-complete-rings)
- [Length of a module](#length-of-a-module)
- [Primary decomposition theorem for finitely generated modules over a principal ideal domain](#primary-decomposition-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)
- [Module (mathematics)](#module-mathematics)
  - [Finitely presented module](#finitely-presented-module)
    - [Fitting ideal](#fitting-ideal)
  - [Locally free module](#locally-free-module)
  - [Finite presentation of a module](#finite-presentation-of-a-module)
  - [Change of rings](#change-of-rings)
    - [Coextension of scalars](#coextension-of-scalars)
    - [Extension of scalars](#extension-of-scalars)
    - [Restriction of scalars](#restriction-of-scalars)
  - [Module isomorphism](#module-isomorphism)
  - [Torsion module](#torsion-module)
    - [Torsion submodule](#torsion-submodule)
      - [Torsion element of a module](#torsion-element-of-a-module)
  - [Module homomorphism](#module-homomorphism)
    - [Module endomorphism](#module-endomorphism)
      - [Module automorphism](#module-automorphism)
    - [Module retraction](#module-retraction)
    - [Endomorphism ring](#endomorphism-ring)
      - [Local endomorphism ring](#local-endomorphism-ring)
      - [Semisimple quotient of a module endomorphism algebra](#semisimple-quotient-of-a-module-endomorphism-algebra)
      - [Brick module](#brick-module)
        - [Ringel lemma on bricks](#ringel-lemma-on-bricks)
          - [Proof of Ringel lemma on bricks](#proof-of-ringel-lemma-on-bricks)
  - [Submodule](#submodule)
    - [Essential submodule](#essential-submodule)
      - [Essential right ideal](#essential-right-ideal)
        - [A regular principal right ideal in a right Noetherian ring is essential](#a-regular-principal-right-ideal-in-a-right-noetherian-ring-is-essential)
      - [Essential extension](#essential-extension)
    - [Primary decomposition](#primary-decomposition)
      - [Lasker–Noether theorem](#lasker-noether-theorem)
      - [Primary submodule](#primary-submodule)
- [Quotient module](#quotient-module)
  - [Universal property of a quotient module](#universal-property-of-a-quotient-module)
- [Free module](#free-module)
  - [Vector-space freeness from maximal independence](#vector-space-freeness-from-maximal-independence)
  - [Linear independence in a module](#linear-independence-in-a-module)
  - [Finite free module](#finite-free-module)
  - [Basis of a module](#basis-of-a-module)
  - [Universal property of a free module](#universal-property-of-a-free-module)
  - [Rank of a free module](#rank-of-a-free-module)
    - [Rank inequality for an injection of finite free modules](#rank-inequality-for-an-injection-of-finite-free-modules)
  - [Invariant basis number](#invariant-basis-number)
    - [Invariant basis number for a commutative ring](#invariant-basis-number-for-a-commutative-ring)
- [Torsion-free module](#torsion-free-module)
  - [Embedding a finitely generated torsion-free module in a finite free module](#embedding-a-finitely-generated-torsion-free-module-in-a-finite-free-module)
  - [Maximal torsion-free quotient](#maximal-torsion-free-quotient)
  - [Reflexive module](#reflexive-module)
    - [Reflexive-module second-syzygy criterion](#reflexive-module-second-syzygy-criterion)
- [Projective module](#projective-module)
  - [Projective modules are flat](#projective-modules-are-flat)
  - [Projective modules are direct summands of free modules](#projective-modules-are-direct-summands-of-free-modules)
  - [Principal indecomposable module](#principal-indecomposable-module)
  - [Finite projective module](#finite-projective-module)
  - [Invertible module](#invertible-module)
    - [Base change of invertible modules](#base-change-of-invertible-modules)
  - [Projective dimension](#projective-dimension)
    - [Top Ext detects finite projective dimension](#top-ext-detects-finite-projective-dimension)
      - [Top Ext detects finite projective dimension over a left Noetherian ring](#top-ext-detects-finite-projective-dimension-over-a-left-noetherian-ring)
      - [Vanishing top Ext without finite generation](#vanishing-top-ext-without-finite-generation)
    - [Global dimension](#global-dimension)
      - [Global dimension zero and split exact sequences](#global-dimension-zero-and-split-exact-sequences)
  - [Free modules are projective](#free-modules-are-projective)
  - [Projective cover](#projective-cover)
    - [Head of a module](#head-of-a-module)
- [Cyclic module](#cyclic-module)
- [Uniserial module](#uniserial-module)
- [Semisimple module](#semisimple-module)
  - [Isotypic decomposition](#isotypic-decomposition)
    - [Isotypic component](#isotypic-component)
- [Radical of a module](#radical-of-a-module)
  - [Radical series of a module](#radical-series-of-a-module)
- [Socle (mathematics)](#socle-mathematics)
  - [Socle series of a module](#socle-series-of-a-module)
- [Loewy length](#loewy-length)
  - [Radical and socle series of a direct sum](#radical-and-socle-series-of-a-direct-sum)
- [Irreducible module](#irreducible-module)
  - [Simple modules over an algebra finite over its center](#simple-modules-over-an-algebra-finite-over-its-center)
  - [Simple module over a commutative ring](#simple-module-over-a-commutative-ring)
- [Annihilator (ring theory)](#annihilator-ring-theory)
  - [Right annihilator](#right-annihilator)
  - [Associated prime of a module](#associated-prime-of-a-module)
    - [Localization of associated primes](#localization-of-associated-primes)
    - [Embedded associated prime](#embedded-associated-prime)
    - [Minimal primes are associated primes](#minimal-primes-are-associated-primes)
  - [Annihilator of a module](#annihilator-of-a-module)
    - [Maximal annihilator of a module element is prime](#maximal-annihilator-of-a-module-element-is-prime)
- [Structure theorem for finitely generated modules over a principal ideal domain](#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)
  - [Invariant factor of a finitely generated module](#invariant-factor-of-a-finitely-generated-module)
  - [Finitely generated torsion-free module over a principal ideal domain](#finitely-generated-torsion-free-module-over-a-principal-ideal-domain)
    - [Classification of integral matrices satisfying the third cyclotomic polynomial](#classification-of-integral-matrices-satisfying-the-third-cyclotomic-polynomial)
  - [Elementary divisor](#elementary-divisor)
  - [Indecomposable finite abelian groups](#indecomposable-finite-abelian-groups)

## Finite representation type

↑ **Parent:** [Module theory](module-theory.md)

A finite-dimensional [algebra](algebra.md) has finite representation type when there are only finitely many isomorphism classes of finite-dimensional [indecomposable modules](#indecomposable-module). This counts module types, not the dimensions or the number of direct sums formed from them. For a [block of a group algebra](representation-theory.md#block-of-a-group-algebra), finite representation type is equivalent to a cyclic [defect group of a block](representation-theory.md#defect-group-of-a-block).

<h2 id="auslander-reiten-quiver">Auslander–Reiten quiver</h2>

↑ **Parent:** [Module theory](module-theory.md)

For a finite-dimensional [algebra](algebra.md), the Auslander–Reiten quiver has one vertex for each isomorphism class of finite-dimensional [indecomposable modules](#indecomposable-module), and its arrows record irreducible module homomorphisms. A homomorphism is irreducible when it is neither a split injection nor a split surjection and every factorization forces the first map to split injectively or the second to split surjectively.

<h3 id="stable-auslander-reiten-quiver">Stable Auslander–Reiten quiver</h3>

↑ **Parent:** [Auslander–Reiten quiver](#auslander-reiten-quiver)

For a self-injective finite-dimensional [algebra](algebra.md), remove the projective vertices from its [Auslander–Reiten quiver](#auslander-reiten-quiver). The resulting stable quiver has vertices the nonprojective indecomposable modules. Its translation sends the end term of an almost-split exact sequence to its start term. In particular a quiver of shape $\mathbb ZA_s/\langle\tau^e\rangle$ has $es$ vertices.

## Topological group module

↑ **Parent:** [Module theory](module-theory.md)

A topological [abelian group](group.md#abelian-group) $A$ with a continuous action of a [topological group](topological-group.md) $G$ by group [automorphisms](algebra.md#automorphism). Continuity means joint continuity of $G\times A\to A$. For a discrete coefficient group this is equivalent to every element of $A$ having an open stabilizer.

## Character module

↑ **Parent:** [Module theory](module-theory.md)

For a [module](#module-mathematics) $M$ over a commutative [ring](commutative-algebra.md#ring) $A$, its character module is the additive-group dual into $D=\mathbb Q/\mathbb Z$, with action $(a\phi)(m)=\phi(am)$. The group $D$ is an [injective cogenerator of abelian groups](noncommutative-algebra.md#injective-cogenerator-of-abelian-groups). The natural adjunction $\operatorname{Hom}_A(N,M^*)\cong\operatorname{Hom}_{\mathbb Z}(N\otimes_AM,D)$ sends $h$ to the balanced pairing $(n,m)\mapsto h(n)(m)$.

## Representation of an associative algebra

↑ **Parent:** [Module theory](module-theory.md)

An algebra representation is a unital [algebra homomorphism](algebra.md#algebra-homomorphism-over-a-field) into the [endomorphisms](algebra.md#endomorphism) of a [vector space](vector-space.md). It is equivalent to making that [vector space](vector-space.md) a left [module](#module-mathematics) over the algebra, with $av=\rho(a)v$.

### Representation of a Banach algebra

↑ **Parent:** [Representation of an associative algebra](#representation-of-an-associative-algebra)

A representation of a complex [Banach algebra](banach-algebra.md) is a complex-linear multiplicative action on a [vector space](vector-space.md). For a [unital](associative-algebra.md#unital-algebra) action require $\pi(1)=I$; a nonunital algebra can be handled by extending the action to its [unitization](banach-algebra.md#unitization-of-an-algebra). A nonzero action is algebraically irreducible when it has no nonzero proper invariant [vector](vector-space.md#vector) subspace, equivalently when it defines a [simple module](#irreducible-module).

#### Algebraically irreducible representation of a Banach algebra

↑ **Parent:** [Representation of a Banach algebra](#representation-of-a-banach-algebra)

Algebraic irreducibility excludes every proper nonzero invariant [vector subspace](vector-space.md#vector-subspace), including those that are not [closed](topology.md#closed-set). It is stronger than topological irreducibility, which excludes only [closed](topology.md#closed-set) [invariant subspaces](representation-theory.md#invariant-subspace). For a nonzero irreducible action, every nonzero [vector](vector-space.md#vector) is cyclic in the algebraic sense: $A\xi=X$.

##### Countable annihilation sequence in an irreducible Banach module

↑ **Parent:** [Algebraically irreducible representation of a Banach algebra](#algebraically-irreducible-representation-of-a-banach-algebra)

For countably many [linearly independent](vector-space.md#linear-independence) [vectors](vector-space.md#vector) in an infinite-dimensional irreducible complex Banach module, there are elements $a_n$ satisfying the displayed annihilation conditions while the tail images $\{\pi(a_n\cdots a_1)\xi_j:j\ge n\}$ remain [linearly independent](vector-space.md#linear-independence). Use the [quotient norm on an irreducible Banach module](#quotient-norm-on-an-irreducible-banach-module) to make each finite annihilator a [closed](topology.md#closed-set) Banach subspace. The [Jacobson density theorem](noncommutative-algebra.md#jacobson-density-theorem) makes each condition of independence of finitely many tail images [open](topology.md#open-set) and dense there; the [Baire category theorem](topological-analysis.md#baire-category-theorem) intersects these countably many conditions. This is stronger than prescribing only finitely many images once.

##### Quotient norm on an irreducible Banach module

↑ **Parent:** [Algebraically irreducible representation of a Banach algebra](#algebraically-irreducible-representation-of-a-banach-algebra)

For a [unital](associative-algebra.md#unital-algebra) irreducible action and $\xi\ne0$, the annihilator $L_\xi=\{a:\pi(a)\xi=0\}$ is a [maximal left ideal](associative-algebra.md#maximal-left-ideal) and is [closed](topology.md#closed-set). Thus $A/L_\xi$ supplies the displayed complete [norm](functional-analysis.md#norm) on the module, with contractive action. Every [module endomorphism](#module-endomorphism) is bounded for this quotient [norm](functional-analysis.md#norm): its value at the cyclic [vector](vector-space.md#vector) is $a\xi$, so it is induced by bounded right multiplication by $a$ on the quotient. The [Gelfand-Mazur theorem](banach-algebra.md#gelfand-mazur-theorem) then makes the module's commutant consist of scalar operators. This constructs one compatible [norm](functional-analysis.md#norm); it does not by itself establish [continuity](calculus.md#continuous-function) in a different preassigned [norm](functional-analysis.md#norm).

#### Normed representation of a Banach algebra

↑ **Parent:** [Representation of a Banach algebra](#representation-of-a-banach-algebra)

A normed representation acts by individually [bounded operators](topological-vector-space.md#continuous-linear-operator) on a [normed vector space](functional-analysis.md#normed-vector-space). This condition alone does not assume that $a\mapsto\pi(a)$ is [continuous](calculus.md#continuous-function) in the [operator norm](continuous-dual-space.md#operator-norm), nor that the representation space is complete. A [continuous](calculus.md#continuous-function) representation has a common bound $\|\pi(a)\|\le C\|a\|$.

<h5 id="johnson-s-continuity-theorem-for-irreducible-normed-representations">Johnson's continuity theorem for irreducible normed representations</h5>

↑ **Parent:** [Normed representation of a Banach algebra](#normed-representation-of-a-banach-algebra)

Every [algebraically irreducible representation of a Banach algebra](#algebraically-irreducible-representation-of-a-banach-algebra) that is normed is [continuous](calculus.md#continuous-function). The [continuous](calculus.md#continuous-function) orbit [vectors](vector-space.md#vector) form an [invariant subspace](representation-theory.md#invariant-subspace). If all nonzero orbit maps were discontinuous, apply the [countable annihilation sequence in an irreducible Banach module](#countable-annihilation-sequence-in-an-irreducible-banach-module) and the [gliding-hump continuity principle](functional-analysis.md#gliding-hump-continuity-principle) to right multiplication on the algebra and evaluation of the operator-valued representation. Off-diagonal maps vanish, whereas diagonal maps are discontinuous, a contradiction. Once every orbit map is [continuous](calculus.md#continuous-function), the [Uniform boundedness principle](banach-space.md#uniform-boundedness-principle) on the [Banach algebra](banach-algebra.md) gives the common operator-norm bound. Completing the original normed representation space supplies the Banach operator space needed in the argument.

## Degeneration of a module

↑ **Parent:** [Module theory](module-theory.md)

A finite-dimensional [module](#module-mathematics) $X$ degenerates to $Y$ when $Y$ has a representative in the closure of $X$'s change-of-basis orbit in the [representation variety of an associative algebra](associative-algebra.md#representation-variety-of-an-associative-algebra). The full orbit of $Y$ then lies in that closure. The relation is transitive because orbit closures are closed and invariant under change of basis. A [split extension as a degeneration](representation-theory.md#split-extension-as-a-degeneration) shows that a module degenerates to the direct sum of its composition factors.

## Hereditary ring

↑ **Parent:** [Module theory](module-theory.md)

A ring is left hereditary if every submodule of a left [projective module](#projective-module) is projective. Equivalently, every left module has a [projective resolution](algebra.md#projective-resolution) of length at most one. The [standard projective resolution of a quiver representation](algebra.md#standard-projective-resolution-of-a-quiver-representation), used also for arbitrary infinite-dimensional modules, proves that [path algebras](algebra.md#path-algebra) are left hereditary.

### Basic hereditary algebra path-algebra theorem

↑ **Parent:** [Hereditary ring](#hereditary-ring)

Let $A$ be a finite-dimensional [basic algebra](associative-algebra.md#basic-algebra) over an [algebraically closed field](algebra.md#algebraically-closed-field) and a [hereditary ring](#hereditary-ring). The radicals of its indecomposable projectives are projective and satisfy $JP_i\cong\bigoplus_jP_j^{a_{ij}}$, where $a_{ij}$ are the [Ext quiver](associative-algebra.md#ext-quiver) arrow multiplicities. Hence $\dim P_i=1+\sum_ja_{ij}\dim P_j$, forcing strict dimension decrease along arrows and therefore acyclicity. Lifting an arrow basis in $J/J^2$ gives a surjective [path algebra](algebra.md#path-algebra) homomorphism $kQ\to A$. The number of paths starting at $i$ satisfies the same dimension recursion. Equality of total dimensions proves the homomorphism is an isomorphism. Sums of vertex [idempotents](commutative-algebra.md#idempotent) over connected components are precisely the primitive [central idempotents](associative-algebra.md#central-idempotent), so components give the blocks.

### Path algebras are hereditary

↑ **Parent:** [Hereditary ring](#hereditary-ring)

The [standard projective resolution of a quiver representation](algebra.md#standard-projective-resolution-of-a-quiver-representation) has length one, even for quivers with oriented cycles. Thus every [path algebra](algebra.md#path-algebra) is a [hereditary ring](#hereditary-ring), and higher [extension groups](algebra.md#extension-group) vanish. Applying a [long exact sequence of Ext groups](algebra.md#long-exact-sequence-of-ext-groups) to $0\to I\to K\to C\to0$ gives a surjection $\operatorname{Ext}^1(K,W)\twoheadrightarrow\operatorname{Ext}^1(I,W)$, since the next term $\operatorname{Ext}^2(C,W)$ is zero. This is the hereditary step in the [Ringel lemma on bricks](#ringel-lemma-on-bricks).

## Regular sequence on a module

↑ **Parent:** [Module theory](module-theory.md)

For central elements, each multiplication map on the preceding quotient must be injective; a usual convention also requires the final quotient to be nonzero. The augmented [Koszul complex on central ring elements](homology.md#koszul-complex-on-central-ring-elements) tensored with $M$ is then a [quasi-isomorphism](homology.md#quasi-isomorphism) to the final quotient in degree zero.

## Composition series of a module

↑ **Parent:** [Module theory](module-theory.md)

A composition series of a [module](#module-mathematics) is a finite chain of [submodules](#submodule) whose nonzero successive [quotient modules](#quotient-module) are [simple modules](#irreducible-module). Every finite-dimensional [Lie algebra representation](lie-algebra.md#lie-algebra-representation) has such a chain, viewed as a [module](#module-mathematics) over the [universal enveloping algebra](lie-algebra.md#universal-enveloping-algebra).

### Composition factor

↑ **Parent:** [Composition series of a module](#composition-series-of-a-module)

A composition factor is an irreducible successive quotient in a [composition series of a module](#composition-series-of-a-module). For a central [Casimir operator](semisimple-lie-algebra.md#casimir-element), its scalar on a composition factor is an [eigenvalue](linear-operator-theory.md#eigenvalue) of the operator on the original [Lie algebra representation](lie-algebra.md#lie-algebra-representation).

## Uniform module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_module)

A nonzero [module](#module-mathematics) is uniform if every pair of nonzero [submodules](#submodule) has nonzero intersection. Equivalently, every nonzero [submodule](#submodule) is an [essential submodule](#essential-submodule). A [right Noetherian domain](noncommutative-algebra.md#right-noetherian-domain) is uniform as a right [module](#module-mathematics): if $aA\cap bA=0$ for nonzero $a,b$, the [right ideals](associative-algebra.md#right-ideal) $b^iaA$, $i\geq0$, form an infinite [direct sum](vector-space.md#direct-sum), contradicting the [ascending chain condition](algebra.md#ascending-chain-condition).

### Uniform dimension

↑ **Parent:** [Uniform module](#uniform-module)

The uniform dimension of a [module](#module-mathematics) is the supremum of the numbers of nonzero [submodules](#submodule) that can occur in an internal [direct sum](vector-space.md#direct-sum). Finite uniform dimension is equivalent to having no infinite internal [direct sum](vector-space.md#direct-sum) of nonzero [submodules](#submodule). A finite [direct sum](vector-space.md#direct-sum) of [uniform modules](#uniform-module) contained as an [essential submodule](#essential-submodule) gives that number as the dimension. The [finite uniform decomposition of a Noetherian module](#finite-uniform-decomposition-of-a-noetherian-module) therefore gives finite uniform dimension.

### Finite uniform decomposition of a Noetherian module

↑ **Parent:** [Uniform module](#uniform-module)

Every nonzero [Noetherian module](algebra.md#noetherian-module) contains a [uniform module](#uniform-module): otherwise repeatedly split a nonuniform nonzero submodule into two disjoint nonzero submodules, retaining one and collecting the other, to build an infinite direct sum. Repeatedly adding a uniform submodule disjoint from the current finite sum must likewise stop. The final finite sum is an [essential submodule](#essential-submodule), since any disjoint nonzero submodule would allow another addition.

## Indecomposable module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indecomposable_module)

A nonzero [module](#module-mathematics) is indecomposable if it cannot be expressed as a [direct sum](vector-space.md#direct-sum) of two nonzero [submodules](#submodule). The zero [module](#module-mathematics) is excluded. A [module](#module-mathematics) of finite [composition length](finite-group-theory.md#composition-length) is indecomposable exactly when its [endomorphism ring](#endomorphism-ring) has no [idempotents](commutative-algebra.md#idempotent) other than zero and one: an [idempotent](commutative-algebra.md#idempotent) splits the [module](#module-mathematics) into its image and [kernel](linear-algebra.md#kernel-of-a-linear-map).

### Top of an indecomposable projective module

↑ **Parent:** [Indecomposable module](#indecomposable-module)

For a nonzero finitely generated [indecomposable module](#indecomposable-module) $P$ that is a [projective module](#projective-module) over a [right Artinian ring](noncommutative-algebra.md#right-artinian-ring) $A$, its top $P/PJ(A)$ is a [simple module](#irreducible-module). The [Jacobson radical](noncommutative-algebra.md#jacobson-radical) $J(A)$ is a [nilpotent ideal](commutative-algebra.md#nilpotent-ideal), so the top is nonzero; the quotient is a [semisimple module](#semisimple-module) over the [semisimple ring](commutative-algebra.md#semisimple-ring) $A/J(A)$. If it decomposed, a nontrivial [idempotent](commutative-algebra.md#idempotent) of its [endomorphism ring](#endomorphism-ring) would lift by projectivity to an [endomorphism](algebra.md#endomorphism) of $P$. The [Hopkins-Levitzki theorem](noncommutative-algebra.md#hopkins-levitzki-theorem) gives finite [composition length](finite-group-theory.md#composition-length), and the [Fitting lemma](#fitting-lemma) makes the lift either invertible or nilpotent. Its induced map on the top would have the same property, impossible for that nontrivial [idempotent](commutative-algebra.md#idempotent).

## Fitting lemma

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fitting_lemma)

For an endomorphism $f$ of a finite-length module $M$, sufficiently large $n$ gives

$$
M=\ker(f^n)\oplus\operatorname{im}(f^n).
$$

If $M$ is indecomposable, every endomorphism is therefore either invertible or nilpotent, so its endomorphism ring is local.

<h2 id="krull-schmidt-theorem">Krull–Schmidt theorem</h2>

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull–Schmidt_theorem)

The Krull–Schmidt theorem says that a finite-length module decomposes as a finite direct sum of indecomposable modules, uniquely up to permutation and isomorphism of the summands.

### Krull-Schmidt decomposition

↑ **Parent:** [Krull–Schmidt theorem](#krull-schmidt-theorem)

A finite-dimensional module is $\bigoplus_aM_a^{\oplus m_a}$ with pairwise nonisomorphic indecomposables and uniquely determined multiplicities. The [Fitting lemma](#fitting-lemma) makes their endomorphism rings local. The multiplicity spaces provide the general linear factors in the [Levi decomposition of a quiver automorphism group](algebra.md#levi-decomposition-of-a-quiver-automorphism-group).

## Dual module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_module)

For an $R$-module $M$, its dual module is $M^*=\operatorname{Hom}_R(M,R)$, with pointwise addition and scalar multiplication.

### Double dual module

↑ **Parent:** [Dual module](#dual-module)

The double dual module is $M^{**}=\operatorname{Hom}_R(M^*,R)$. The [evaluation homomorphism](commutative-algebra.md#evaluation-homomorphism) sends $m\in M$ to the functional $f\mapsto f(m)$.

## Finitely generated module

↑ **Parent:** [Module theory](module-theory.md)

An $R$-module is finitely generated when there are finitely many elements $m_1,\ldots,m_r$ such that every element is an $R$-linear combination of them.

### Minimal number of generators of a module

↑ **Parent:** [Finitely generated module](#finitely-generated-module)

For a [module](#module-mathematics) $M$, $\mu_A(M)$ is the least cardinality of a generating set, equivalently the least size of a [basis](vector-space.md#basis) of a [free module](#free-module) surjecting onto $M$. If $(A,\mathfrak m)$ is a [local ring](commutative-algebra.md#local-ring) and $M$ is finitely generated, then $\mu_A(M)=\dim_{A/\mathfrak m}(M/\mathfrak mM)$. Any generating set spans this quotient, proving the lower bound. Lift a [basis](vector-space.md#basis) of the quotient and let $J$ be the [submodule](#submodule) generated by those lifts. Then $N=M/J$ is finitely generated and satisfies $N=\mathfrak mN$. For generators $n_i$ write $n_i=\sum_jc_{ij}n_j$ with $c_{ij}\in\mathfrak m$. The adjugate of $I-C$ shows that $\det(I-C)$ annihilates $N$; this determinant is one modulo $\mathfrak m$ and hence a [unit](algebra.md#unit-in-a-ring). Thus $N=0$, giving the upper bound.

### Clearing denominators relative to an independent module subset

↑ **Parent:** [Finitely generated module](#finitely-generated-module)

Let a [finitely generated module](#finitely-generated-module) over an [integral domain](commutative-algebra.md#integral-domain) have a finite generating set $S$ and a maximal independent subset $T$. For each $s\notin T$, dependence of $T\cup\{s\}$ gives a nonzero coefficient $a_s$ with $a_ss\in\langle T\rangle$. The product of those coefficients is nonzero and carries the whole [module](#module-mathematics) into $\langle T\rangle$.

### Finite generation as a quotient of a finite free module

↑ **Parent:** [Finitely generated module](#finitely-generated-module)

An [R-module](#primary-submodule) is finitely generated exactly when it is the image of a [surjection](algebra.md#surjective-function) from a finite [free module](#free-module) $R^n$. Given generators $m_i$, send $(r_i)$ to $\sum_i r_im_i$; conversely, the images of the standard free generators generate every such image. This criterion does not assert that the [module](#module-mathematics) is free: a quotient can have nontrivial relations.

## Artinian module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artinian_module)

An $R$-module is Artinian when every descending chain of submodules stabilizes. Equivalently, every nonempty family of submodules has a minimal member.

### Artinian modules are co-Hopfian

↑ **Parent:** [Artinian module](#artinian-module)

For an injective [module endomorphism](#module-endomorphism) $f:M\to M$ of an [Artinian module](#artinian-module), the chain $M\supseteq fM\supseteq f^2M\supseteq\cdots$ stabilizes. If $f^nM=f^{n+1}M$, then every $x$ satisfies $f^nx=f^{n+1}y$. Injectivity of $f^n$ gives $x=fy$, proving surjectivity. No finite-length or Noetherian hypothesis is needed.

### Artinian modules in a short exact sequence

↑ **Parent:** [Artinian module](#artinian-module)

For a [short exact sequence](#short-exact-sequence) $0\to N\to M\to Q\to0$, the middle [module](#module-mathematics) is [Artinian](algebra.md#artinian-ring) exactly when both outer [modules](#module-mathematics) are [Artinian](algebra.md#artinian-ring). Submodules and quotients inherit the [descending chain condition](algebra.md#descending-chain-condition). Conversely, for a descending chain $M_i$, both $M_i\cap N$ and its image in $Q$ eventually stabilize. If $x\in M_i$, choose $y\in M_{i+1}$ with the same image in $Q$; then $x-y\in M_i\cap N=M_{i+1}\cap N$, giving $M_i=M_{i+1}$. Induction shows that finite direct sums of [Artinian modules](#artinian-module) are [Artinian](algebra.md#artinian-ring).

## Filtered colimit of modules

↑ **Parent:** [Module theory](module-theory.md)

A filtered colimit of modules is a direct limit indexed by a filtered category. Filtered colimits preserve exact sequences, and tensor products commute with them.

### Direct system of abelian groups

↑ **Parent:** [Filtered colimit of modules](#filtered-colimit-of-modules)

A direct system indexed by a [directed set](set.md#directed-set) $A$ consists of [abelian groups](group.md#abelian-group) $G_a$ and homomorphisms $\phi_{ab}:G_a\to G_b$ for $a\leq b$, with $\phi_{aa}=1$ and $\phi_{bc}\phi_{ab}=\phi_{ac}$.

#### Direct limit of abelian groups

↑ **Parent:** [Direct system of abelian groups](#direct-system-of-abelian-groups)

The direct limit of a [direct system of abelian groups](#direct-system-of-abelian-groups) is the quotient of $\bigoplus_aG_a$ by the relations identifying $g\in G_a$ with $\phi_{ab}(g)\in G_b$ whenever $a\leq b$.

##### Sequential direct limit of multiplication maps on the integers

↑ **Parent:** [Direct limit of abelian groups](#direct-limit-of-abelian-groups)

For nonzero integers $a_i$ and $P_n=a_0\cdots a_{n-1}$, the compatible embeddings of stage $n$ into $\mathbb Q$ send $m$ to $m/P_n$. They identify the direct limit with

$$
\bigcup_{n\geq0}P_n^{-1}\mathbb Z\subseteq\mathbb Q.
$$

###### Rational group with square-free denominators

↑ **Parent:** [Sequential direct limit of multiplication maps on the integers](#sequential-direct-limit-of-multiplication-maps-on-the-integers)

The additive group $\mathbb Q_{\mathrm{sq}}$ consists of the [rational numbers](number-theory.md#rational-number) whose reduced denominators are [square-free integers](number-theory.md#square-free-integer). If $p_0,p_1,\ldots$ lists the primes without repetition, then

$$
\mathbb Q_{\mathrm{sq}}\cong\varinjlim\left(\mathbb Z\xrightarrow{p_0}\mathbb Z\xrightarrow{p_1}\mathbb Z\xrightarrow{p_2}\cdots\right).
$$

## Bimodule

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bimodule)

An $(R,S)$-bimodule is simultaneously a left $R$-module and a right $S$-module, with commuting scalar actions $(rm)s=r(ms)$.

## Invariant submodule

↑ **Parent:** [Module theory](module-theory.md)

For a group $G$ acting on a module $M$, the invariant submodule is $M^G=\{m\in M:g\cdot m=m\text{ for all }g\in G\}$.

## Coinvariant module

↑ **Parent:** [Module theory](module-theory.md)

For a group $G$ acting on a module $M$, the coinvariant module is

$$
M_G=M/\langle g\cdot m-m:g\in G,\ m\in M\rangle.
$$

### Abelianization over a Zp-extension

↑ **Parent:** [Coinvariant module](#coinvariant-module)

Suppose $1\to X\to\mathcal G\to\Gamma\to1$ is an exact sequence of [pro-p groups](topological-group.md#pro-p-group), with $X$ abelian and $\Gamma\cong\mathbb Z_p$. Conjugation gives $X$ a [compact Galois module](galois-theory.md#compact-galois-module) structure. The closed [commutator subgroup](group-theory.md#commutator-subgroup) is $(\gamma-1)X$: its image is closed by compactness, and after quotienting by it, a lift of $\gamma$ centralizes $X$ and topologically generates the remaining quotient. Hence $0\to X_\Gamma\to\mathcal G^{\mathrm{ab}}\to\Gamma\to0$ is exact.

## Support of a module

↑ **Parent:** [Module theory](module-theory.md)

The support of an $R$-module $M$ is

$$
\operatorname{Supp}_R(M)=\{\mathfrak p\in\operatorname{Spec}R:M_{\mathfrak p}\ne0\}.
$$

For a nonzero finitely generated module, the support is nonempty and contains a maximal ideal.

## Tensor product of modules

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor_product_of_modules)

The tensor product of an $R$-module $M$ and an $R$-module $N$ is an $R$-module $M\otimes_RN$ generated by pure tensors $m\otimes n$, subject to additivity in both variables and the balancing relation

$$
(rm)\otimes n=m\otimes(rn).
$$

### Right exactness of the tensor product

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

For a [short exact sequence](#short-exact-sequence) $0\to U\xrightarrow{i}V\xrightarrow{q}W\to0$ and any [module](#module-mathematics) $E$, the sequence $U\otimes_AE\to V\otimes_AE\to W\otimes_AE\to0$ is exact. The last map is surjective since every pure tensor $w\otimes e$ can be lifted using a preimage of $w$. Put $T=(V\otimes_AE)/\operatorname{im}(i\otimes1_E)$. There is a well-defined balanced map $W\times E\to T$, sending $(q(v),e)$ to the class of $v\otimes e$: replacing $v$ by $v+i(u)$ changes it by an element of the discarded image. This induces $W\otimes_AE\to T$, inverse to the map induced by $q\otimes1_E$. Thus the kernel of $q\otimes1_E$ is exactly the image of $i\otimes1_E$. Consequently a module is flat exactly when tensoring with it also preserves injections.

### Change-of-rings tensor quotient

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

For a homomorphism of [commutative rings](commutative-algebra.md#commutative-ring) $R\to A$ and two $A$-[modules](#module-mathematics), the [tensor product of modules](#tensor-product-of-modules) over $A$ is the quotient of the [tensor product of modules](#tensor-product-of-modules) over $R$ imposing all relations $am\otimes n=m\otimes an$. The quotient map is $A$-linear when $A$ acts through the first factor on the source. This expresses the extra balancing imposed by [change of rings](#change-of-rings).

### Tensor product of commutative algebras

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

For commutative $R$-algebras, their module [tensor product](linear-algebra.md#tensor-product) becomes a commutative algebra by $(a\otimes b)(a'\otimes b')=aa'\otimes bb'$. Its [universal property](category-theory.md#universal-property) is that pairs of compatible $R$-algebra maps from $A$ and $B$ into a commutative algebra $C$ correspond to maps $A\otimes_RB\to C$. This coproduct of algebras gives, contravariantly, the [fibre product of schemes](ringed-space.md#fiber-product-of-schemes) on affine charts.

#### Tensor product of field extensions is nonzero

↑ **Parent:** [Tensor product of commutative algebras](#tensor-product-of-commutative-algebras)

If $L,L^{\prime}$ are [field extensions](algebra.md#field-extension) of $K$, choose a $K$-basis of $L$ containing $1$. After tensoring with $L^{\prime}$, that basis expresses $L\otimes_KL^{\prime}$ as a nonzero direct sum of copies of $L^{\prime}$, and $1\otimes1$ is nonzero. A [prime ideal](commutative-algebra.md#prime-ideal) of this nonzero ring supplies a point used in the [point-lifting property of a scheme fibre product](ringed-space.md#point-lifting-property-of-a-scheme-fibre-product).

### Pure tensor

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pure_tensor)

A pure tensor is an element of a tensor product that can be written as $m\otimes n$. General tensors are finite sums of pure tensors and need not themselves be pure.

### Projectivity of factors of a nonzero finite free tensor product

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

If $M\otimes_RN\cong R^n$ for a positive integer $n$, then both $M$ and $N$ are [projective modules](#projective-module). Choose a finite expression for the inverse image of one basis vector. It produces a split surjection $N^r\to R$; tensoring the splitting with $M$ exhibits $M$ as a direct summand of the finite free module $(M\otimes_RN)^r$. Symmetry gives the result for $N$.

### Tensor-nilpotent module

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

An $R$-module $M$ is tensor-nilpotent when $M^{\otimes k}=0$ for some positive integer $k$. A nonzero finitely generated module cannot be tensor-nilpotent: localize at a maximal ideal in its support and reduce modulo that maximal ideal, obtaining a nonzero tensor power of a nonzero vector space.

### Balanced map

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

A map $b:M\times N\to P$ is balanced when it is additive in each variable and satisfies $b(rm,n)=b(m,rn)$.

### Universal property of the tensor product of modules

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

Every balanced map $b:M\times N\to P$ factors uniquely through an $R$-module homomorphism $\widetilde b:M\otimes_RN\to P$ satisfying $\widetilde b(m\otimes n)=b(m,n)$.

### Tensor-hom adjunction

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tensor-hom_adjunction)

For modules over a commutative ring, there is a natural isomorphism

$$
\operatorname{Hom}_R(M\otimes_RN,P)
\cong
\operatorname{Hom}_R\bigl(M,\operatorname{Hom}_R(N,P)\bigr),
$$

given by $f\mapsto(m\mapsto(n\mapsto f(m\otimes n)))$.

### Tensor product and infinite direct product

↑ **Parent:** [Tensor product of modules](#tensor-product-of-modules)

Tensor product need not commute with an infinite direct product. For example,

$$
\mathbb Q\otimes_{\mathbb Z}\prod_{n\geq2}\mathbb Z/n\mathbb Z\ne0,
\qquad
\prod_{n\geq2}\left(\mathbb Q\otimes_{\mathbb Z}\mathbb Z/n\mathbb Z\right)=0.
$$

The element $(1\bmod n)_n$ has infinite order in the product, so it survives rational localization.

## Flat module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_module)

An $R$-module $M$ is flat when tensoring with it preserves injections, equivalently when $-\otimes_RM$ is an exact functor.

### Flatness criterion over dual numbers

↑ **Parent:** [Flat module](#flat-module)

For $D=k[\varepsilon]/(\varepsilon^2)$, a [module](#module-mathematics) $M$ is a [flat module](#flat-module) exactly when $\ker(\varepsilon:M\to M)=\varepsilon M$. Flatness implies this by tensoring the exact sequence $0\to(\varepsilon)\to D\to k\to0$. Conversely lift a $k$-basis of $M/\varepsilon M$ to $M$. Every element is a finite combination of the lifts plus $\varepsilon$ times another such combination, proving generation over $D$. A relation first reduces to zero coefficients modulo $\varepsilon$; the kernel condition then reduces its remaining coefficients to zero as well. The lifts form a free $D$-basis, proving flatness.

### Equational criterion for flatness

↑ **Parent:** [Flat module](#flat-module)

For a [flat module](#flat-module) $M$ over a [commutative ring](commutative-algebra.md#commutative-ring), every finite relation among elements of $M$ is a finite combination of relations among elements of the [ring](commutative-algebra.md#ring) itself, in the displayed sense. To obtain this, tensor the kernel of the linear map $A^r\to A$, $(u_i)\mapsto\sum_i a_iu_i$, with $M$. Flatness says that this tensor maps onto the kernel in $M^r$. Writing an element of that tensor as a finite sum gives the columns $b_{ij}$ and the elements $n_j$. The converse follows by applying this condition to relations in a [tensor product](linear-algebra.md#tensor-product) to prove that tensoring preserves injections.

### Free modules are flat

↑ **Parent:** [Flat module](#flat-module)

For a [free module](#free-module) $F=\bigoplus_{i\in J}Ae_i$, the natural map $U\otimes_AF\to\bigoplus_{i\in J}U$ sends $u\otimes\sum_i a_ie_i$ to $(a_iu)_i$ and is an [isomorphism](algebra.md#isomorphism), with inverse sending the tuple $(u_i)$ to $\sum_i u_i\otimes e_i$. For any [injection](algebra.md#injective-function) $U\hookrightarrow V$, its [tensor product of modules](#tensor-product-of-modules) with $F$ is therefore the coordinatewise [injection](algebra.md#injective-function) $\bigoplus_JU\hookrightarrow\bigoplus_JV$. Thus every [free module](#free-module) is flat, including those of infinite rank.

### Direct summands of flat modules are flat

↑ **Parent:** [Flat module](#flat-module)

If $F=P\oplus Q$ is a [flat module](#flat-module), then $P$ and $Q$ are [flat](#flat-module). For an [injection](algebra.md#injective-function) $u:U\hookrightarrow V$, distributivity of the [tensor product of modules](#tensor-product-of-modules) identifies $u\otimes F$ with $(u\otimes P)\oplus(u\otimes Q)$. This map is [injective](algebra.md#injective-function) by flatness of $F$. Each component is therefore [injective](algebra.md#injective-function), proving flatness of both summands.

### Flatness criterion using ideals

↑ **Parent:** [Flat module](#flat-module)

The arrow is the canonical multiplication map, not an arbitrary abstract module isomorphism. Its inclusion into $M$ is $\mu_I:I\otimes_AM\to M$. Dualizing identifies $\mu_I^*$ with the restriction $\operatorname{Hom}_A(A,M^*)\to\operatorname{Hom}_A(I,M^*)$. All these maps are surjective precisely when $M^*$ is injective, by the [Baer criterion](noncommutative-algebra.md#baer-criterion). The [injective cogenerator of abelian groups](noncommutative-algebra.md#injective-cogenerator-of-abelian-groups) detects injectivity of $\mu_I$, and the [Lambek theorem](#lambek-theorem) gives flatness. No Noetherian or finite-generation hypothesis is needed.

### Lambek theorem

↑ **Parent:** [Flat module](#flat-module)

A [module](#module-mathematics) over a commutative [ring](commutative-algebra.md#ring) is [flat](#flat-module) exactly when its [character module](#character-module) is [injective](algebra.md#injective-function). For a submodule inclusion $N'\hookrightarrow N$, the character adjunction identifies restriction $\operatorname{Hom}_A(N,M^*)\to\operatorname{Hom}_A(N',M^*)$ with the dual of $N'\otimes_AM\to N\otimes_AM$. The [injective cogenerator of abelian groups](noncommutative-algebra.md#injective-cogenerator-of-abelian-groups) detects whether the latter map is injective. Thus the two extension/exactness conditions are equivalent.

### Faithfully flat module

↑ **Parent:** [Flat module](#flat-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faithfully_flat_module)

A flat module $M$ is faithfully flat when $N\otimes_RM=0$ implies $N=0$. Every field extension is faithfully flat over its base field.

### Flatness is local

↑ **Parent:** [Flat module](#flat-module)

An $R$-module $M$ is flat if and only if $M_{\mathfrak p}$ is flat over $R_{\mathfrak p}$ for every prime ideal $\mathfrak p$, equivalently for every maximal ideal.

### Torsion-free module over a principal ideal domain is flat

↑ **Parent:** [Flat module](#flat-module)

Over a principal ideal domain, a module is flat exactly when it is torsion-free. Hence the tensor product of two torsion-free modules over a principal ideal domain is torsion-free: both tensor functors are exact, so their composite is exact.

### Flat extension preserves finite ideal intersections

↑ **Parent:** [Flat module](#flat-module)

If an $R$-algebra $A$ is flat as an $R$-module, then for ideals $I,J\subseteq R$,

$$
IA\cap JA=(I\cap J)A.
$$

Tensor the exact sequence $0\to I\cap J\to I\oplus J\to I+J\to0$ with $A$.

### Local tensor nonvanishing criterion

↑ **Parent:** [Flat module](#flat-module)

A nonzero commutative ring $R$ has the property that $M\otimes_RN=0$ forces $M=0$ or $N=0$ exactly when $R$ is local with maximal ideal $\mathfrak m$ and $M=\mathfrak mM$ forces $M=0$ for every $R$-module. Reduction modulo $\mathfrak m$ turns a tensor product into a tensor product of vector spaces.

## Determinant trick

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Determinant_trick)

If a finitely generated faithful module $M$ over a commutative ring $R$ satisfies $xM\subseteq IM$, the determinant of a matrix presenting these relations gives a monic equation

$$
x^n+a_{n-1}x^{n-1}+\cdots+a_0=0,
\qquad a_i\in I^{n-i}.
$$

In particular, an element of an extension field that preserves a nonzero finitely generated ideal is integral over $R$.

## Short exact sequence

↑ **Parent:** [Module theory](module-theory.md)

A short exact sequence is an exact sequence

$$
0\longrightarrow L\xrightarrow{j}M\xrightarrow{q}N\longrightarrow0.
$$

Thus $j$ is injective, $q$ is surjective, and $\operatorname{im}j=\ker q$.

### Module extension

↑ **Parent:** [Short exact sequence](#short-exact-sequence)

A short exact sequence with specified kernel module $A$ and quotient module $C$. Its equivalence class is determined by the degree-one [Ext functor](algebra.md#ext-functor); equivalence must preserve both end modules.

#### Extension of trivial modules for an infinite cyclic group

↑ **Parent:** [Module extension](#module-extension)

With trivial action on both end modules, an extension has underlying abelian group $\mathbb Z^r\oplus\mathbb Z^s$ and generator action $\left(\begin{smallmatrix}I&T\\0&I\end{smallmatrix}\right)$. The integer matrix $T$ is invariant under equivalences fixing the ends. The one-element [projective resolution](algebra.md#projective-resolution) with differential $z-1$ computes the same classification over the [group ring](commutative-algebra.md#group-ring).

#### Pushout of a module extension

↑ **Parent:** [Module extension](#module-extension)

Pushing an inclusion $i:A\to B$ along $f:A\to A\prime$ gives a new [module extension](#module-extension) with kernel $A\prime$ and the same quotient. This [pushout](category.md#pushout) realizes the covariance of the degree-one [Ext functor](algebra.md#ext-functor) in its second argument.

#### Equivalence of module extensions

↑ **Parent:** [Module extension](#module-extension)

A commuting isomorphism between two [module extensions](#module-extension) that is the identity on both end modules. Classifying middle modules up to arbitrary isomorphism is a different and generally coarser problem.

### Split short exact sequence

↑ **Parent:** [Short exact sequence](#short-exact-sequence)

A short exact sequence splits when its injection has a retraction, equivalently when its surjection has a section. In that case the middle module is isomorphic to the direct sum of the two outer modules.

### Short five lemma

↑ **Parent:** [Short exact sequence](#short-exact-sequence)

The [Five lemma](category-theory.md#five-lemma) has a short form: in a commutative diagram of short exact sequences, if the maps on both outer terms are isomorphisms, then the map on the middle terms is an isomorphism.

## Inverse system

↑ **Parent:** [Module theory](module-theory.md)

An inverse system is a family $(N_i)$ with transition maps $g_{ij}:N_j\to N_i$ for $i\le j$, satisfying $g_{ii}=1$ and $g_{ik}=g_{ij}g_{jk}$.

### Inverse limit

↑ **Parent:** [Inverse system](#inverse-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_limit)

The inverse limit is the module of compatible families

$$
\varprojlim_iN_i=\{(x_i)\in\prod_iN_i:g_{ij}(x_j)=x_i\}.
$$

#### Universal property of an inverse limit

↑ **Parent:** [Inverse limit](#inverse-limit)

Maps from a module $X$ to $\varprojlim_iN_i$ correspond naturally to compatible families of maps $X\to N_i$.

#### Nonemptiness theorem for inverse limits of finite sets

↑ **Parent:** [Inverse limit](#inverse-limit)

An inverse system of nonempty finite sets over a directed index set has nonempty inverse limit. Give each set the discrete topology: the compatibility conditions are closed subsets of the compact product, and directedness gives them the [finite intersection property](topology.md#finite-intersection-property).

## Filtration of a module

↑ **Parent:** [Module theory](module-theory.md)

A decreasing filtration of a module is a chain $M=M_0\supseteq M_1\supseteq\cdots$ of submodules.

### Quotient filtration

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)

The quotient filtration records images of the filtered pieces in a [quotient module](#quotient-module). Together with the [subspace filtration](#subspace-filtration), it gives [exactness of associated graded modules for induced filtrations](commutative-algebra.md#exactness-of-associated-graded-modules-for-induced-filtrations).

### Subspace filtration

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)

A [submodule](#submodule) of a filtered [module](#module-mathematics) inherits the displayed filtration by intersection. It is also called the induced filtration.

### Ascending filtration

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)

An ascending filtration is an increasing chain of additive subgroups, or vector subspaces when a scalar field is fixed. It is exhaustive if their union is the whole object. For a [filtered ring](#filtered-ring), multiplicative compatibility means $F_iR\,F_jR\subseteq F_{i+j}R$. For an ideal $I$, intersecting each level with $I$ gives the induced filtration. Its [associated graded module](commutative-algebra.md#associated-graded-module) has components $(I\cap F_nR)/(I\cap F_{n-1}R)$.

### Good filtration of a module

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)

For a [filtered algebra](#filtered-algebra) $A$ with finite-dimensional filtration pieces, a [good filtration of a module](#good-filtration-of-a-module) on a [finitely generated module](#finitely-generated-module) is compatible with multiplication and has finitely generated [associated graded module](commutative-algebra.md#associated-graded-module) over the [associated graded ring](commutative-algebra.md#associated-graded-ring). Taking bounded-degree translates of a finite set of module generators supplies such a [filtration of a module](#filtration-of-a-module) when the [associated graded ring](commutative-algebra.md#associated-graded-ring) is [Noetherian](algebra.md#noetherian-ring).

#### Dimension of a filtered module

↑ **Parent:** [Good filtration of a module](#good-filtration-of-a-module)

For a [good filtration of a module](#good-filtration-of-a-module) over a fixed finite-dimensional [filtration of a ring](#filtration-of-a-ring) whose associated graded algebra is commutative and finitely generated, the cumulative Hilbert function is eventually a [quasipolynomial](commutative-algebra.md#quasipolynomial) by the [Hilbert-Serre theorem](commutative-algebra.md#hilbert-serre-theorem). Its leading asymptotic degree is the dimension of the nonzero filtered [module](#module-mathematics). Monotonicity forces the leading coefficients in its residue classes to agree. If the associated graded algebra is a [standard graded algebra](commutative-algebra.md#standard-graded-algebra), the Hilbert function is eventually polynomial. Two good module filtrations bound one another after fixed shifts, so they have the same growth degree. Set $d(0)=-\infty$. For the [Bernstein filtration](noncommutative-algebra.md#bernstein-filtration) this is the [Bernstein growth dimension of a Weyl algebra module](associative-algebra.md#bernstein-growth-dimension-of-a-weyl-algebra-module).

##### Multiplicity of a filtered module

↑ **Parent:** [Dimension of a filtered module](#dimension-of-a-filtered-module)

With the fixed algebra-filtration convention in [dimension of a filtered module](#dimension-of-a-filtered-module), the multiplicity is factorial times the common leading coefficient of the cumulative Hilbert function for $M\ne0$, and is zero for $M=0$. It is a positive integer with a [standard graded algebra](commutative-algebra.md#standard-graded-algebra) normalization, and can be a positive rational number for a weighted grading. Fixed shifts between [good filtrations of a module](#good-filtration-of-a-module) preserve its leading Hilbert coefficient. Rescaling the algebra filtration itself can change multiplicity, so its normalization must be specified.

###### Dimension and multiplicity in a filtered exact sequence

↑ **Parent:** [Multiplicity of a filtered module](#multiplicity-of-a-filtered-module)

The [subspace filtration](#subspace-filtration) and [quotient filtration](#quotient-filtration) in a [short exact sequence](#short-exact-sequence) are good when the associated graded algebra is [Noetherian](algebra.md#noetherian-ring). Their cumulative Hilbert functions add in every degree. Positive leading coefficients make the degree of the sum the larger degree; when both degrees agree, factorial times the leading coefficients add. Thus equal-dimensional nonzero factors consume positive [multiplicity of a filtered module](#multiplicity-of-a-filtered-module). With a [standard graded algebra](commutative-algebra.md#standard-graded-algebra) normalization these multiplicities are integral.

### Equivalent filtrations of a module

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)

Two decreasing filtrations $(M_n)$ and $(N_n)$ are equivalent when each contains a fixed shift of the other: $M_{n+a}\subseteq N_n$ and $N_{n+b}\subseteq M_n$ for fixed $a,b$ and every $n$.

### I-adic topology

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/I-adic_topology)

The $I$-adic topology on a [module](#module-mathematics) $M$ has the powers $I^nM$ as a neighbourhood basis of zero. It is generated by the [I-adic filtration](#i-adic-filtration); separatedness means $\bigcap_n I^nM=0$.

#### I-adic filtration

↑ **Parent:** [I-adic topology](#i-adic-topology)

For an ideal $I$, the $I$-adic filtration of a module $M$ is $M\supseteq IM\supseteq I^2M\supseteq\cdots$.

##### Krull intersection theorem

↑ **Parent:** [I-adic filtration](#i-adic-filtration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krull_intersection_theorem)

If $R$ is a [Noetherian local ring](algebra.md#noetherian-local-ring) with maximal ideal $\mathfrak m$ and $I\subseteq\mathfrak m$, then

$$
\bigcap_{n\geq1}I^n=0.
$$

More generally, the intersection of the powers acts trivially on every finitely generated module.

##### x-adic filtration

↑ **Parent:** [I-adic filtration](#i-adic-filtration)

The $x$-adic filtration is the filtration by powers of the principal ideal $(x)$.

##### Stable I-filtration

↑ **Parent:** [I-adic filtration](#i-adic-filtration)

An $I$-filtration $(M_n)$ is stable when $IM_n=M_{n+1}$ for all sufficiently large $n$. Every stable $I$-filtration is equivalent to the $I$-adic filtration.

##### Rees algebra

↑ **Parent:** [I-adic filtration](#i-adic-filtration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rees_algebra)

For an ideal $I\subseteq R$, the Rees ring is the graded subring

$$
\mathcal R(I)=\bigoplus_{n\geq0}I^nt^n\subseteq R[t].
$$

It packages all powers of $I$ into one algebra and turns stable filtrations into finitely generated graded modules.

###### Rees module

↑ **Parent:** [Rees algebra](#rees-algebra)

The Rees module of an $R$-[module](#module-mathematics) $M$ with respect to an [ideal](commutative-algebra.md#ideal) $I$ is $\mathcal R_I(M)=\bigoplus_{j\ge0}I^jMt^j$, a [graded module](commutative-algebra.md#graded-module) over the [Rees ring](#rees-algebra) $\mathcal R(I)$. Generators of $M$ in degree zero generate this module. For $N\subseteq M$, the graded [submodule](#submodule) $\bigoplus_j(I^jM\cap N)t^j$ is finitely generated when $R$ is a [Noetherian ring](algebra.md#noetherian-ring); a bound on its generators' degrees yields the [Artin-Rees lemma](#artin-rees-lemma).

##### Artin-Rees lemma

↑ **Parent:** [I-adic filtration](#i-adic-filtration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artin–Rees_lemma)

If $R$ is Noetherian, $I$ is an ideal, and $N\subseteq M$ are finitely generated modules, then some $k$ satisfies

$$
I^nM\cap N=I^{n-k}(I^kM\cap N)
$$

for every $n\ge k$.

### Filtered algebra

↑ **Parent:** [Filtration of a module](#filtration-of-a-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Filtered_algebra)

A filtered algebra has a nested family of vector subspaces whose index is compatible with multiplication.

#### Rees ring of a filtered algebra

↑ **Parent:** [Filtered algebra](#filtered-algebra)

For an ascending multiplicative filtration with $1\in F_0A$, its Rees ring contains the central element $h$. The quotient by $h$ is the [associated graded ring](commutative-algebra.md#associated-graded-ring), and the quotient by $h-1$ is the original algebra. If $[F_iA,F_jA]\subseteq F_{i+j-1}A$, commutators of lifts are divisible by $h$. Their first-order term defines the [Poisson bracket from a central deformation parameter](algebra.md#poisson-bracket-from-a-central-deformation-parameter) on the associated graded ring.

#### Almost commutative algebra

↑ **Parent:** [Filtered algebra](#filtered-algebra)

An almost commutative algebra over a [field](algebra.md#field) is an [algebra](algebra.md) with an exhaustive increasing nonnegative multiplicative [filtration](stochastic-process.md#filtration-probability-theory) whose [associated graded ring](commutative-algebra.md#associated-graded-ring) is commutative and finitely generated as an algebra over the field. A common presentation uses finitely many degree-one generators, scalar degree-zero part, and [commutators](lie-algebra.md#commutator) that lower degree. The finite-generation requirement is essential: an infinitely generated commutative [polynomial ring](commutative-algebra.md#polynomial-ring) has commutative associated graded algebra but need not be [Noetherian](algebra.md#noetherian-ring).

##### Degree-one almost commutative algebra

↑ **Parent:** [Almost commutative algebra](#almost-commutative-algebra)

This is the degree-one convention for an [almost commutative algebra](#almost-commutative-algebra): the exhaustive filtration is generated by a finite-dimensional first step containing $1$, the degree-zero part is $k$, and its associated graded algebra is commutative. The first step is a finite-dimensional [Lie algebra](lie-algebra.md) under commutators. Its inclusion into $A$ extends by the universal property to a surjection from its [universal enveloping algebra](lie-algebra.md#universal-enveloping-algebra). The element $1$ of the first step is retained as a central Lie generator and its image is the associative identity; quotienting the first step by $k1$ before taking the bracket can lose scalar commutators. This convention is stronger than merely requiring a finitely generated commutative associated graded algebra for an arbitrary weighted filtration.

// Destination: noncommutative-algebra.bigb

#### Filtered ring

↑ **Parent:** [Filtered algebra](#filtered-algebra)

A filtered ring is a ring with subgroups $(R_n)$ satisfying $R_mR_n\subseteq R_{m+n}$.

##### Filtration of a ring

↑ **Parent:** [Filtered ring](#filtered-ring)

A filtration of a [ring](commutative-algebra.md#ring) is an exhaustive increasing family of additive subgroups $(F_iR)_{i\in\mathbb Z}$, with $1\in F_0R$ and the displayed multiplicativity condition. Its [associated graded ring](commutative-algebra.md#associated-graded-ring) is $\bigoplus_i F_iR/F_{i-1}R$. It differs from a probabilistic [filtration](stochastic-process.md#filtration-probability-theory), which is a nested family of sigma-algebras.

###### Complete negative filtration

↑ **Parent:** [Filtration of a ring](#filtration-of-a-ring)

A negative [filtration of a ring](#filtration-of-a-ring) has $F_iR=R$ for nonnegative indices. It is complete and separated when the displayed map to the [inverse limit](#inverse-limit) is an [isomorphism](algebra.md#isomorphism). Products make $F_{-q}R$ two-sided [ideals](commutative-algebra.md#ideal). Series whose terms eventually belong to every $F_{-q}R$ converge. In particular, for $x\in F_{-1}R$ and $r\in R$, the [geometric series](real-analysis.md#geometric-series) $\sum_{j\geq0}(xr)^j$ inverts $1-xr$, so the [unit criterion for the Jacobson radical](noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) gives $F_{-1}R\subseteq J(R)$.

###### Complete negative filtered-graded transfer of Noetherianity

↑ **Parent:** [Complete negative filtration](#complete-negative-filtration)

Lift finite homogeneous generators of the [associated graded module](commutative-algebra.md#associated-graded-module) of a [right ideal](associative-algebra.md#right-ideal) $I$ to $x_i\in I$ of degrees $d_i$. Successive leading-symbol cancellations write an element $x\in F_dI$ as finite partial sums $\sum_i x_i a_i^{(q)}$ with residual in $F_{d-q}R$. The coefficient increments lie in $F_{d-q-d_i}R$ and therefore converge in the [complete negative filtration](#complete-negative-filtration). Multiplication is continuous, so their limits express $x$ as a finite sum $\sum_i x_i a_i$. This generates the actual [right ideal](associative-algebra.md#right-ideal) and does not presuppose that it is closed. The left-sided statement is analogous.

##### Ascending filtered-graded transfer of Noetherianity

↑ **Parent:** [Filtered ring](#filtered-ring)

For an exhaustive nonnegative increasing multiplicative [filtration](stochastic-process.md#filtration-probability-theory), each [left ideal](associative-algebra.md#left-ideal) $I$ induces a homogeneous [ideal](commutative-algebra.md#ideal) $\operatorname{gr}I$ in the [associated graded ring](commutative-algebra.md#associated-graded-ring). If that graded ring is a [left Noetherian ring](noncommutative-algebra.md#left-noetherian-ring), lift a finite homogeneous generating set of $\operatorname{gr}I$ to elements of $I$. For any element of $I$, subtract a combination of these lifts with the same leading symbol; the remainder has strictly lower degree. Induction on the nonnegative degree proves the lifts generate $I$. There is no completion hypothesis because the cancellation terminates in finitely many steps. The analogous result holds for [right ideals](associative-algebra.md#right-ideal).

##### Filtered-graded transfer for complete rings

↑ **Parent:** [Filtered ring](#filtered-ring)

For a complete separated multiplicatively filtered [ring](commutative-algebra.md#ring) with nonnegative integer valuations, a domain [associated graded ring](commutative-algebra.md#associated-graded-ring) makes the original ring a domain: the leading symbols of two nonzero elements have nonzero product. If the graded ring is left Noetherian, lift finitely many homogeneous generators of the graded ideal of a left ideal. Successively cancelling leading terms leaves remainders of increasing valuation. Completeness makes the coefficient series converge, expressing every ideal element as a finite sum of the chosen generators with completed coefficients. The right-handed argument is identical. Completeness is necessary for this infinite cancellation proof.

## Length of a module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Length_of_a_module)

The length of a module is the number of simple factors in a composition series. It is additive across short exact sequences.

## Primary decomposition theorem for finitely generated modules over a principal ideal domain

↑ **Parent:** [Module theory](module-theory.md)

A finitely generated module over a principal ideal domain decomposes as

$$
R^r\oplus\bigoplus_p\bigoplus_jR/(p^{e_{p,j}}),
$$

with finitely many irreducibles $p$. The free rank and primary cyclic factors are unique up to associates and ordering.

## Module (mathematics)

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Module_(mathematics))

An $R$-module is an abelian group equipped with scalar multiplication by a ring $R$, satisfying the usual distributive and associative laws.

### Finitely presented module

↑ **Parent:** [Module (mathematics)](#module-mathematics)

A [module](#module-mathematics) is finitely presented if it has finitely many generators and finitely many defining relations, equivalently an exact sequence of the displayed form with m and n finite. Over a commutative ring a relation [matrix](vector-space.md#matrix) records the presentation, and its minors define the [Fitting ideals](#fitting-ideal).

// Target: knot-theory.bigb

#### Fitting ideal

↑ **Parent:** [Finitely presented module](#finitely-presented-module)

For a [module](#module-mathematics) over a commutative ring presented by a [matrix](vector-space.md#matrix) with n generators, its zeroth Fitting ideal is generated by all n-by-n minors of the relation [matrix](vector-space.md#matrix). It is independent of the chosen finite presentation. Over a [unique factorization domain](algebra.md#unique-factorization-domain), the greatest common divisor of these minors defines the [module](#module-mathematics) order up to a unit. This does not require a Smith normal form over the ring. The square [Seifert-matrix presentation of the Alexander module](knot-theory.md#seifert-matrix-presentation-of-the-alexander-module) makes the order its determinant.

// Target: knot-theory.bigb

### Locally free module

↑ **Parent:** [Module (mathematics)](#module-mathematics)

A [locally free module](#locally-free-module) is one whose associated sheaf is locally a [free module](#free-module). In the finite constant-rank case, it becomes free of rank $r$ on a [principal open subset](ringed-space.md#principal-open-subscheme) cover of $\operatorname{Spec}A$. Equivalently it is a [finite projective module](#finite-projective-module) of constant rank $r$. A surjection onto it splits, so the [kernel](linear-algebra.md#kernel-of-a-linear-map) is also finite projective. Its associated sheaf is a [locally free sheaf](ringed-space.md#locally-free-sheaf) and defines an algebraic [vector bundle](fiber-bundle.md#vector-bundle).

// Target: algebraic-geometry.bigb

### Finite presentation of a module

↑ **Parent:** [Module (mathematics)](#module-mathematics)

A [module](#module-mathematics) is finitely presented when it admits the displayed [exact sequence](homology.md#exact-sequence) for finite integers $r,s$. Thus it has finitely many generators and finitely many relations. On a [Noetherian ring](algebra.md#noetherian-ring), every finitely generated module has a finite presentation.

### Change of rings

↑ **Parent:** [Module (mathematics)](#module-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_rings)

Changing the coefficient [ring](commutative-algebra.md#ring) of a [module](#module-mathematics) along a [ring homomorphism](commutative-algebra.md#ring-homomorphism) can mean [restriction of scalars](#restriction-of-scalars), [extension of scalars](#extension-of-scalars), or [coextension of scalars](#coextension-of-scalars). The underlying [module](#module-mathematics) may be retained with a smaller ring action, or replaced by a tensor or Hom construction with the new ring.

#### Coextension of scalars

↑ **Parent:** [Change of rings](#change-of-rings)

For a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $R\to A$ and a left $R$-[module](#module-mathematics) $M$, the left $A$-action on $\operatorname{Hom}_R(A,M)$ is $(a\cdot h)(b)=h(ba)$. This construction is right adjoint to [restriction of scalars](#restriction-of-scalars).

#### Extension of scalars

↑ **Parent:** [Change of rings](#change-of-rings)

For a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $R\to A$, tensoring an $R$-[module](#module-mathematics) with the $(A,R)$-[bimodule](#bimodule) $A$ gives an $A$-[module](#module-mathematics). This functor is left adjoint to [restriction of scalars](#restriction-of-scalars).

#### Restriction of scalars

↑ **Parent:** [Change of rings](#change-of-rings)

For a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $\theta:R\to A$, an $A$-[module](#module-mathematics) becomes an $R$-[module](#module-mathematics) by the displayed action. Its underlying [abelian group](group.md#abelian-group) stays the same.

### Module isomorphism

↑ **Parent:** [Module (mathematics)](#module-mathematics)

A [module isomorphism](#module-isomorphism) is a bijection of [modules](#module-mathematics) over the same [ring](commutative-algebra.md#ring) preserving addition and scalar multiplication. Its inverse preserves these operations too. When a [linear operator](vector-space.md#linear-operator) $T$ gives a [vector space](vector-space.md) an $F[t]$-[module](#module-mathematics) structure by $t\cdot v=T(v)$, a [module isomorphism](#module-isomorphism) is exactly an invertible [linear map](vector-space.md#linear-map) intertwining the two operators. This translates classification of [modules](#module-mathematics) into [matrix similarity](linear-algebra.md#matrix-similarity) and [rational canonical form](linear-operator-theory.md#rational-canonical-form).

### Torsion module

↑ **Parent:** [Module (mathematics)](#module-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torsion_module)

A torsion module over an [integral domain](commutative-algebra.md#integral-domain) is a module in which every element is annihilated by some nonzero scalar.

#### Torsion submodule

↑ **Parent:** [Torsion module](#torsion-module)

For a module $M$ over an [integral domain](commutative-algebra.md#integral-domain) $R$, its torsion submodule is

$$
T(M)=\{m\in M:rm=0\text{ for some }0\ne r\in R\}.
$$

The domain condition makes this a [submodule](#submodule): products of nonzero annihilators remain nonzero and annihilate sums.

##### Torsion element of a module

↑ **Parent:** [Torsion submodule](#torsion-submodule)

For a [module](#module-mathematics) over an [integral domain](commutative-algebra.md#integral-domain), a torsion element is killed by some nonzero scalar. These elements form the [torsion submodule](#torsion-submodule): the product of nonzero annihilating scalars annihilates a sum. This scalar-annihilation definition differs from saying that an element has finite order in a [group](group.md).

### Module homomorphism

↑ **Parent:** [Module (mathematics)](#module-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Module_homomorphism)

An $R$-module homomorphism is an additive map $f:M\to N$ satisfying $f(rm)=rf(m)$.

#### Module endomorphism

↑ **Parent:** [Module homomorphism](#module-homomorphism)

A module endomorphism is a [module homomorphism](#module-homomorphism) from a [module](#module-mathematics) to itself. These maps form the [endomorphism ring](#endomorphism-ring) $\operatorname{End}_R(M)$ under pointwise addition and composition. An invertible module endomorphism is a [module automorphism](#module-automorphism).

##### Module automorphism

↑ **Parent:** [Module endomorphism](#module-endomorphism)

A module automorphism is an invertible [module endomorphism](#module-endomorphism). Equivalently, it is a bijective [module homomorphism](#module-homomorphism) from a [module](#module-mathematics) to itself; its inverse is automatically a [module homomorphism](#module-homomorphism). They form a [group](group.md) under composition.

#### Module retraction

↑ **Parent:** [Module homomorphism](#module-homomorphism)

A [module retraction](#module-retraction) onto a [submodule](#submodule) $U\xrightarrow iX$ is a [module homomorphism](#module-homomorphism) $r:X\to U$ with $ri=I_U$. It gives $X=i(U)\oplus\ker r$: write $x=i(r(x))+(x-i(r(x)))$. Thus a nonzero proper submodule admitting a retraction contradicts indecomposability. Extending a projection from a larger submodule can produce such a retraction through the [long exact sequence of Ext groups](algebra.md#long-exact-sequence-of-ext-groups).

#### Endomorphism ring

↑ **Parent:** [Module homomorphism](#module-homomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Endomorphism_ring)

The endomorphism ring $\operatorname{End}_R(M)$ consists of the $R$-module homomorphisms $M\to M$, with pointwise addition and composition as multiplication.

##### Local endomorphism ring

↑ **Parent:** [Endomorphism ring](#endomorphism-ring)

An [endomorphism ring](#endomorphism-ring) is local when its nonunits form a proper two-sided [ideal](commutative-algebra.md#ideal); commutativity is not required. The [Fitting lemma](#fitting-lemma) gives this property for an indecomposable finite-length [module](#module-mathematics). If two nonunits had an invertible sum, multiplication by its inverse would give $I=f+g$ with noninvertible $f,g$. Fitting makes $f$ nilpotent, so $I-f=g$ would be invertible, a contradiction. Products with a nonunit are nonunits by finite-length injectivity/surjectivity. The quotient by the nonunit ideal is a [division ring](commutative-algebra.md#division-ring).

##### Semisimple quotient of a module endomorphism algebra

↑ **Parent:** [Endomorphism ring](#endomorphism-ring)

For a finite-dimensional module over an [algebraically closed field](algebra.md#algebraically-closed-field), write a [Krull-Schmidt decomposition](#krull-schmidt-decomposition) $X=\bigoplus_aM_a^{\oplus m_a}$ with distinct indecomposable types. Each endomorphism ring of $M_a$ is a [local endomorphism ring](#local-endomorphism-ring) with residue division algebra $k$, by the [finite-dimensional division algebra over an algebraically closed field](algebra.md#finite-dimensional-division-algebra-over-an-algebraically-closed-field) result. Modulo the [Jacobson radical](noncommutative-algebra.md#jacobson-radical) of $\operatorname{End}(X)$, the blocks of one type become $M_{m_a}(k)$ and all maps between different types vanish. A composite through a different indecomposable type cannot be invertible, since that would make one type a direct summand of the other. This yields the displayed product and the [Levi decomposition of a quiver automorphism group](algebra.md#levi-decomposition-of-a-quiver-automorphism-group).

##### Brick module

↑ **Parent:** [Endomorphism ring](#endomorphism-ring)

A nonzero module is a brick when every endomorphism is either zero or an isomorphism. Equivalently, its endomorphism ring is a division ring.

###### Ringel lemma on bricks

↑ **Parent:** [Brick module](#brick-module)

An indecomposable finite-dimensional [quiver representation](algebra.md#representation-of-a-quiver) that is not a [brick module](#brick-module) contains a brick with nonzero self-extensions. The [Ringel form](algebra.md#ringel-form) then gives $q_Q(\dim B)=1-\dim\operatorname{Ext}^1_Q(B,B)\leq0$, impossible for a positive definite [Tits form of a quiver](algebra.md#tits-form-of-a-quiver).

###### Proof of Ringel lemma on bricks

↑ **Parent:** [Ringel lemma on bricks](#ringel-lemma-on-bricks)

The [Fitting lemma](#fitting-lemma) supplies a nonzero nilpotent endomorphism $f$ of a non-brick indecomposable $X$. Minimize its nonzero rank; nilpotence and minimality give $f^2=0$. Set $I=\operatorname{im}f\subset K=\ker f=\bigoplus_jK_j$. Choose a nonzero component $u:I\to K_j$. The square-zero endomorphism $X\xrightarrow fI\xrightarrow uK_j\hookrightarrow X$ has rank at least $\dim I$, so $u$ is injective.

If $\operatorname{Ext}^1(I,K_j)=0$, the projection $K\to K_j$ extends to $X\to K_j$ by the [long exact sequence of Ext groups](algebra.md#long-exact-sequence-of-ext-groups), giving a [module retraction](#module-retraction) and contradicting indecomposability. Thus this extension group is nonzero. Since [path algebras are hereditary](#path-algebras-are-hereditary), $u$ induces a surjection $\operatorname{Ext}^1(K_j,K_j)\twoheadrightarrow\operatorname{Ext}^1(I,K_j)$. Hence $K_j$ is a proper indecomposable submodule with self-extensions. Iterate until a [brick module](#brick-module) is reached; dimensions strictly decrease.

This minimal-rank argument is given in section 2 of [William Crawley-Boevey's quiver lectures](https://www.math.uni-bielefeld.de/~wcrawley/quivlecs.pdf).

### Submodule

↑ **Parent:** [Module (mathematics)](#module-mathematics)

A submodule $N$ of a [module](#module-mathematics) $M$ is a subset closed under addition, additive inverses, and scalar multiplication by every element of $R$.

#### Essential submodule

↑ **Parent:** [Submodule](#submodule)

A [submodule](#submodule) $N\subseteq M$ is an [essential submodule](#essential-submodule) if it intersects every nonzero [submodule](#submodule) of $M$ nontrivially. A nonzero [module](#module-mathematics) is a [uniform module](#uniform-module) precisely when every nonzero [submodule](#submodule) is an [essential submodule](#essential-submodule).

##### Essential right ideal

↑ **Parent:** [Essential submodule](#essential-submodule)

An essential right ideal is an [essential submodule](#essential-submodule) of the right regular [module](#module-mathematics) of a [ring](commutative-algebra.md#ring). Every [right ideal](associative-algebra.md#right-ideal) containing an essential right ideal is essential.

###### A regular principal right ideal in a right Noetherian ring is essential

↑ **Parent:** [Essential right ideal](#essential-right-ideal)

If $c$ is a [regular element of a ring](noncommutative-algebra.md#regular-element-of-a-ring) in a [right Noetherian ring](noncommutative-algebra.md#right-noetherian-ring) and a nonzero [right ideal](associative-algebra.md#right-ideal) $B$ had $B\cap cR=0$, cancellation would make $B+cB+c^2B+\cdots$ an infinite [direct sum](vector-space.md#direct-sum) of nonzero [right ideals](associative-algebra.md#right-ideal). Its finite partial sums contradict the [ascending chain condition](algebra.md#ascending-chain-condition). Thus $cR$ is an [essential right ideal](#essential-right-ideal).

##### Essential extension

↑ **Parent:** [Essential submodule](#essential-submodule)

An extension $N\subseteq M$ is essential when $N$ is an [essential submodule](#essential-submodule) of $M$. Essentiality is transitive. It is an intersection condition, not a statement that the quotient is small in dimension or finitely generated.

#### Primary decomposition

↑ **Parent:** [Submodule](#submodule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primary_decomposition)

A primary decomposition expresses an ideal or submodule as an intersection of primary components.

<h5 id="lasker-noether-theorem">Lasker–Noether theorem</h5>

↑ **Parent:** [Primary decomposition](#primary-decomposition)

Every proper [ideal](commutative-algebra.md#ideal) in a [Noetherian ring](algebra.md#noetherian-ring) is a finite intersection of [primary ideals](commutative-algebra.md#primary-ideal). This existence theorem does not give uniqueness of the individual components: [embedded primary components](commutative-algebra.md#embedded-primary-component) may vary.

##### Primary submodule

↑ **Parent:** [Primary decomposition](#primary-decomposition)

A proper submodule $N\subsetneq M$ is primary when $rm\in N$ and $m\notin N$ imply $r^kM\subseteq N$ for some positive integer $k$.

## Quotient module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_module)

For a submodule $N\leq M$, the quotient module $M/N$ consists of additive cosets with scalar multiplication $r(m+N)=rm+N$.

### Universal property of a quotient module

↑ **Parent:** [Quotient module](#quotient-module)

If an [R-module homomorphism](#module-homomorphism) $f:M\to P$ vanishes on a [submodule](#submodule) $N$, there is a unique homomorphism $\bar f:M/N\to P$ satisfying $f=\bar f\circ q$, where $q:M\to M/N$ is the quotient map. It is given by $\bar f(m+N)=f(m)$.

## Free module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_module)

A free module has a basis: every element has a unique finite linear combination in that basis with coefficients in the scalar ring.

### Vector-space freeness from maximal independence

↑ **Parent:** [Free module](#free-module)

Order the [linearly independent](vector-space.md#linear-independence) subsets of a [vector space](vector-space.md) by inclusion. A chain's union is independent, since every finite relation is contained in one chain member. [Zorn's lemma](set-theory.md#zorn-s-lemma) gives a maximal independent subset. A vector outside its span could be adjoined while preserving independence, so it spans. Sending finite-support coefficient families to their linear combinations gives an isomorphism from the [free module](#free-module) on that subset to $V$. This supplies an arbitrary, possibly infinite-dimensional [basis](vector-space.md#basis) using the [axiom of choice](set-theory.md#axiom-of-choice); no pre-existing [basis](vector-space.md#basis) theorem is invoked.

### Linear independence in a module

↑ **Parent:** [Free module](#free-module)

Elements of a [module](#module-mathematics) are linearly independent if every finite linear relation between them has all coefficients zero. An independent finite set freely generates its span, a [finite free module](#finite-free-module). Over an [integral domain](commutative-algebra.md#integral-domain), maximal independence within a finite generating set enables [clearing denominators relative to an independent module subset](#clearing-denominators-relative-to-an-independent-module-subset).

### Finite free module

↑ **Parent:** [Free module](#free-module)

A finite free module is a free module with a finite basis, equivalently a module isomorphic to $R^n$ for some nonnegative integer $n$.

### Basis of a module

↑ **Parent:** [Free module](#free-module)

A basis $S$ of an $R$-module $M$ is a subset such that every element of $M$ has a unique expression as a finite $R$-linear combination of elements of $S$.

### Universal property of a free module

↑ **Parent:** [Free module](#free-module)

A module $F$ is free on a set $S$ exactly when every function from $S$ to any module $N$ extends uniquely to an $R$-module homomorphism $F\to N$.

### Rank of a free module

↑ **Parent:** [Free module](#free-module)

For a nonzero commutative scalar ring, every two bases of a finite-rank free module have the same cardinality. This cardinality is the rank.

#### Rank inequality for an injection of finite free modules

↑ **Parent:** [Rank of a free module](#rank-of-a-free-module)

Over a nonzero commutative ring, an injection $R^m\hookrightarrow R^n$ implies $m\leq n$. If $m>n$, appending zero coordinates gives an injective endomorphism of $R^m$ with zero determinant; the Cayley--Hamilton theorem and cancellation of that injection eventually force the identity to vanish.

### Invariant basis number

↑ **Parent:** [Free module](#free-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invariant_basis_number)

A nonzero [ring](commutative-algebra.md#ring) $R$ has invariant basis number if $R^m\cong R^n$ as [free modules](#free-module) implies $m=n$ for all positive integers $m,n$. The property is not automatic for arbitrary rings; the commutative-ring case is proved below.

#### Invariant basis number for a commutative ring

↑ **Parent:** [Invariant basis number](#invariant-basis-number)

If $R$ is a nonzero commutative ring and $R^m\cong R^n$, reduction modulo a maximal ideal produces isomorphic vector spaces of dimensions $m$ and $n$. Hence $m=n$.

## Torsion-free module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torsion-free_module)

A module $M$ over an integral domain $R$ is torsion-free when $rm=0$ with $0\ne r\in R$ implies $m=0$.

### Embedding a finitely generated torsion-free module in a finite free module

↑ **Parent:** [Torsion-free module](#torsion-free-module)

Apply [clearing denominators relative to an independent module subset](#clearing-denominators-relative-to-an-independent-module-subset) to find $0\ne a$ with $aM$ lying in a [finite free module](#finite-free-module). Multiplication by $a$ is injective on a [torsion-free module](#torsion-free-module), giving the required embedding. A submodule need not itself be free over a general [integral domain](commutative-algebra.md#integral-domain).

### Maximal torsion-free quotient

↑ **Parent:** [Torsion-free module](#torsion-free-module)

For a module $M$ over an [integral domain](commutative-algebra.md#integral-domain), the quotient $M/T(M)$ by its [torsion submodule](#torsion-submodule) is torsion-free. Every homomorphism from $M$ to a torsion-free module factors uniquely through $M/T(M)$ by the [universal property of a quotient module](#universal-property-of-a-quotient-module).

### Reflexive module

↑ **Parent:** [Torsion-free module](#torsion-free-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflexive_module)

A finitely generated module $M$ over a [commutative ring](commutative-algebra.md#commutative-ring) $A$ is reflexive when its [evaluation homomorphism](commutative-algebra.md#evaluation-homomorphism) $M\to M^{**}$ to the [double dual module](#double-dual-module) is an [isomorphism](algebra.md#isomorphism).

#### Reflexive-module second-syzygy criterion

↑ **Parent:** [Reflexive module](#reflexive-module)

Let $A$ be a [Noetherian ring](algebra.md#noetherian-ring) that is an [integral domain](commutative-algebra.md#integral-domain). If

$$
0\longrightarrow M\longrightarrow N\longrightarrow P\longrightarrow0
$$

is [exact](homology.md#exact-sequence), $N$ is a finitely generated [free module](#free-module), and $P$ is a [torsion-free module](#torsion-free-module), then $M$ is a [reflexive module](#reflexive-module). In particular, the dual of every finitely generated $A$-module is reflexive.

## Projective module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_module)

A module $P$ is projective when every map from $P$ through the target of a surjection lifts through that surjection.

### Projective modules are flat

↑ **Parent:** [Projective module](#projective-module)

A [projective module](#projective-module) is a [direct summand](vector-space.md#direct-summand) of a [free module](#free-module). [Free modules](#free-module) are flat because tensoring with a [free module](#free-module) produces a [direct sum](vector-space.md#direct-sum) of copies of the original module and map. If $F=P\oplus Q$ is flat, tensoring an [injection](algebra.md#injective-function) with $F$ is the [direct sum](vector-space.md#direct-sum) of its tensor maps with $P$ and $Q$, so each component is [injective](algebra.md#injective-function). Applying this to a [free module](#free-module) containing $P$ proves that $P$ is [flat](#flat-module).

### Projective modules are direct summands of free modules

↑ **Parent:** [Projective module](#projective-module)

Every [module](#module-mathematics) $P$ is a quotient of a [free module](#free-module) $F=\bigoplus_{p\in P}Ae_p$, via $e_p\mapsto p$. If $P$ is a [projective module](#projective-module), lift $1_P$ through this [surjection](algebra.md#surjective-function) to obtain a section $s:P\to F$. The resulting [split short exact sequence](#split-short-exact-sequence) identifies $F$ with $\ker\pi\oplus P$. Conversely, if $P$ is a summand of a [free module](#free-module), extend a prescribed map out of $P$ to the [free module](#free-module) using the summand projection, lift each [basis](vector-space.md#basis) image through the given [surjection](algebra.md#surjective-function), and restrict the lift to $P$. This proves the equivalence with the lifting definition of a [projective module](#projective-module), for arbitrary ranks.

### Principal indecomposable module

↑ **Parent:** [Projective module](#projective-module)

For a finite-dimensional [algebra](algebra.md) $A$, a principal indecomposable module is an indecomposable direct summand of the left regular [module](#module-mathematics), equivalently $Ae$ for a [primitive idempotent](commutative-algebra.md#primitive-idempotent) $e$. Its [head of a module](#head-of-a-module) is simple, and it is the [projective cover](#projective-cover) of that simple module.

### Finite projective module

↑ **Parent:** [Projective module](#projective-module)

A finite projective module is a [finitely generated module](#finitely-generated-module) that is a [projective module](#projective-module). Equivalently it is a direct summand of a finite [free module](#free-module): a finite free surjection splits by projectivity. Its [dual module](#dual-module) is finite projective and its evaluation map to its [double dual module](#double-dual-module) is an [isomorphism](algebra.md#isomorphism), since both properties hold for finite free modules and pass to direct summands. Finite generation is needed for this elementary duality argument.

### Invertible module

↑ **Parent:** [Projective module](#projective-module)

An invertible module over a [commutative ring](commutative-algebra.md#commutative-ring) $A$ is a [finitely generated module](#finitely-generated-module) that is a [projective module](#projective-module) and whose [localization at a prime ideal](commutative-algebra.md#localization-at-a-prime-ideal) is free of rank one at every prime. Its [dual module](#dual-module) $L^*=\operatorname{Hom}_A(L,A)$ is also finite projective. Evaluation $L\otimes_A L^*\to A$ is an [isomorphism](algebra.md#isomorphism) after every prime localization, hence is an isomorphism globally by [localization detects zero elements](commutative-algebra.md#localization-detects-zero-elements). The [Picard group of a ring](ringed-space.md#picard-group-of-a-ring) consists of the isomorphism classes of these modules under the [tensor product of modules](#tensor-product-of-modules).

#### Base change of invertible modules

↑ **Parent:** [Invertible module](#invertible-module)

For a [ring homomorphism](commutative-algebra.md#ring-homomorphism) $A\to B$, [extension of scalars](#extension-of-scalars) takes an [invertible module](#invertible-module) to an invertible $B$-module. A direct-summand presentation in a finite [free module](#free-module) remains a direct-summand presentation after tensoring. At a prime $\mathfrak q\subset B$ contracting to $\mathfrak p$, localization gives $B_{\mathfrak q}\otimes_{A_{\mathfrak p}}L_{\mathfrak p}\cong B_{\mathfrak q}$. Compatibility with tensor products, identities and composition makes the [Picard group of a ring](ringed-space.md#picard-group-of-a-ring) a covariant [functor](category.md#functor).

### Projective dimension

↑ **Parent:** [Projective module](#projective-module)

For a nonzero [module](#module-mathematics), the projective dimension $\operatorname{pd}_RM$ is the shortest length of a [projective resolution](algebra.md#projective-resolution) of the [module](#module-mathematics) $M$, or infinity if no finite [projective resolution](algebra.md#projective-resolution) exists. Equivalently, it is the supremum of degrees with nonzero $\operatorname{Ext}_R^n(M,N)$ as $N$ ranges over all [modules](#module-mathematics). This equivalence follows by dimension shifting and the characterization of [projective modules](#projective-module) by vanishing $\operatorname{Ext}^1$.

#### Top Ext detects finite projective dimension

↑ **Parent:** [Projective dimension](#projective-dimension)

Let $M$ be a nonzero [finitely generated module](#finitely-generated-module) over a commutative [Noetherian ring](algebra.md#noetherian-ring). Take a length-$n$ resolution with finite projective terms. If its top [Ext functor](algebra.md#ext-functor) with coefficients in $A$ vanished, the dual of its last injection would be surjective. The dual of a finite projective module is projective, so that surjection splits. Finite projective modules are isomorphic to their double duals, so dualizing gives a splitting of the original injection. The resolution then shortens, contradicting minimality of $n$. When $n=0$, a nonzero coordinate of a finite free module containing $M$ as a summand gives a nonzero map $M\to A$.

##### Top Ext detects finite projective dimension over a left Noetherian ring

↑ **Parent:** [Top Ext detects finite projective dimension](#top-ext-detects-finite-projective-dimension)

For a nonzero left [finitely generated module](#finitely-generated-module) over a [left Noetherian ring](noncommutative-algebra.md#left-noetherian-ring), take a finite [projective resolution](algebra.md#projective-resolution) with [finite projective modules](#finite-projective-module). Vanishing of its top [Ext functor](algebra.md#ext-functor) would make the dual of its final injection surjective. These duals are right [finite projective modules](#finite-projective-module), so the surjection splits. Dualizing back and using finite projective [double dual modules](#double-dual-module) splits the original injection and shortens the resolution, contradicting the definition of [projective dimension](#projective-dimension). When the dimension is zero, a coordinate map of a finite free module containing the nonzero projective summand supplies a nonzero map to $R$. The left/right distinction in the duals is essential for a noncommutative [ring](commutative-algebra.md#ring).

##### Vanishing top Ext without finite generation

↑ **Parent:** [Top Ext detects finite projective dimension](#top-ext-detects-finite-projective-dimension)

Put $A=k[[t]]$ and $K=A[1/t]$. A [free resolution](algebra.md#free-resolution) has countably many generators $e_i$ and relations $e_i-te_{i+1}$. Applying the [Hom functor](algebra.md#hom-functor) with coefficients in $A$ gives $(b_i)\mapsto(b_i-tb_{i+1})$ on sequence products. This is surjective: for prescribed $(c_i)$ use $b_i=\sum_{j\ge0}t^jc_{i+j}$, a well-defined [formal power series](commutative-algebra.md#formal-power-series). Therefore the degree-one [Ext functor](algebra.md#ext-functor) vanishes. But $\operatorname{Hom}_A(K,A)=0$, since every image is infinitely divisible by $t$. A nonzero projective module has a nonzero coordinate map into $A$, so $K$ is not projective. Its displayed resolution proves that its [projective dimension](#projective-dimension) is exactly one. The finite-generation hypothesis in [top Ext detects finite projective dimension](#top-ext-detects-finite-projective-dimension) is essential.

#### Global dimension

↑ **Parent:** [Projective dimension](#projective-dimension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Global_dimension)

The global dimension of a [ring](commutative-algebra.md#ring) is the supremum of the [projective dimensions](#projective-dimension) of all its [modules](#module-mathematics), allowing infinity. It measures the longest [projective resolution](algebra.md#projective-resolution) needed by any [module](#module-mathematics). For a [field](algebra.md#field) it is zero, since every [module](#module-mathematics) is a [vector space](vector-space.md) and hence free.

##### Global dimension zero and split exact sequences

↑ **Parent:** [Global dimension](#global-dimension)

If [global dimension](#global-dimension) is zero, every [module](#module-mathematics) is a [projective module](#projective-module). Each [short exact sequence](#short-exact-sequence) splits because its quotient is projective. Conversely, splitting every [short exact sequence](#short-exact-sequence) makes each [module](#module-mathematics) a direct summand of a [free module](#free-module) and therefore a [projective module](#projective-module). Splitting also makes every [module](#module-mathematics) an [injective module](noncommutative-algebra.md#injective-module): for $A\hookrightarrow B$ choose a retraction $B\to A$ and compose it with any prescribed map out of $A$.

### Free modules are projective

↑ **Parent:** [Projective module](#projective-module)

Lift the image of each basis element independently through the given surjection, then extend the chosen lifts linearly.

### Projective cover

↑ **Parent:** [Projective module](#projective-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_cover)

A projective cover of a module $M$ is an essential surjection $P\twoheadrightarrow M$ from a [projective module](#projective-module). For a finite-dimensional algebra, every finite-dimensional module has one; the projective cover of a simple module is indecomposable and has that simple module as its head.

#### Head of a module

↑ **Parent:** [Projective cover](#projective-cover)

The head, or top, of a finite-length module $M$ is its largest semisimple quotient. It is $M/J(M)$, where $J(M)$ is the [radical of a module](#radical-of-a-module).

## Cyclic module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_module)

A module is cyclic when one element $m$ generates it: $M=Rm$.

## Uniserial module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniserial_module)

A module is uniserial when its submodules are totally ordered by inclusion. A finite-length uniserial module has a unique composition series.

## Semisimple module

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semisimple_module)

A module is semisimple, or completely reducible, when it is a [direct sum](vector-space.md#direct-sum) of [simple modules](#irreducible-module). Equivalently, every submodule has a direct-sum complement.

### Isotypic decomposition

↑ **Parent:** [Semisimple module](#semisimple-module)

A finite-length [semisimple module](#semisimple-module) has a canonical decomposition

$$
M=\bigoplus_i M_i
$$

in which $M_i$ is the sum of all simple submodules isomorphic to a fixed simple module $S_i$. Each $M_i$ is isomorphic to a finite direct sum $S_i^{m_i}$.

The decomposition is intrinsic to the [semisimple module](#semisimple-module): the isomorphism types of its simple submodules determine the summands.

#### Isotypic component

↑ **Parent:** [Isotypic decomposition](#isotypic-decomposition)

In a complex representation of a [finite group](group.md#finite-group) $N$, the $\theta$-isotypic component is the sum of all irreducible submodules with character $\theta$. The [character idempotent](associative-algebra.md#character-idempotent) $e_\theta=\theta(1)|N|^{-1}\sum_{n\in N}\theta(n^{-1})n$ projects onto it. Every $N$-submodule is preserved by these projections and decomposes into its intersections with the isotypic components. If $N\triangleleft G$, conjugation permutes them according to $\theta^g(n)=\theta(g^{-1}ng)$.

## Radical of a module

↑ **Parent:** [Module theory](module-theory.md)

The radical $J(M)$ of a module is the intersection of its maximal submodules. For a finite-dimensional module over a finite-dimensional algebra $A$,

$$
J(M)=J(A)M,
$$

and it is the smallest submodule $N$ for which $M/N$ is a [semisimple module](#semisimple-module).

### Radical series of a module

↑ **Parent:** [Radical of a module](#radical-of-a-module)

The radical series is the descending chain

$$
M\supseteq J(M)\supseteq J^2(M)\supseteq\cdots,
$$

where $J^{i+1}(M)=J(J^i(M))$. For finite-dimensional $A$ and $M$, one has $J^i(M)=J(A)^iM$.

## Socle (mathematics)

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Socle_(mathematics))

The socle of a module is the sum of all its simple submodules, equivalently its largest [semisimple module](#semisimple-module).

### Socle series of a module

↑ **Parent:** [Socle (mathematics)](#socle-mathematics)

The socle series begins with $\operatorname{Soc}^0(M)=0$ and is defined by

$$
\operatorname{Soc}^{i+1}(M)/\operatorname{Soc}^i(M)
=\operatorname{Soc}\bigl(M/\operatorname{Soc}^i(M)\bigr).
$$

For finite-dimensional $A$ and $M$, $\operatorname{Soc}^i(M)$ consists of the elements annihilated by $J(A)^i$.

## Loewy length

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loewy_length)

The Loewy length of a finite-length module is both the least $m$ for which $J^m(M)=0$ and the least $m$ for which $\operatorname{Soc}^m(M)=M$.

### Radical and socle series of a direct sum

↑ **Parent:** [Loewy length](#loewy-length)

For finite-length modules $U,V$ and every nonnegative integer $i$,

$$
J^i(U\oplus V)=J^i(U)\oplus J^i(V),
\qquad
\operatorname{Soc}^i(U\oplus V)=\operatorname{Soc}^i(U)\oplus\operatorname{Soc}^i(V).
$$

## Irreducible module

↑ **Parent:** [Module theory](module-theory.md)

An irreducible, or simple, module is nonzero and has no submodules other than zero and itself.

### Simple modules over an algebra finite over its center

↑ **Parent:** [Irreducible module](#irreducible-module)

If $A$ is a finite [module](#module-mathematics) over a commutative central subring $R$ and $M$ is a simple left $A$-module, then $M=Am$ is finite over $R$. A central element not annihilating $M$ acts bijectively, since its kernel and image are $A$-submodules. Put $B=R/\operatorname{Ann}_R(M)$. For $0\ne r\in B$, write generators as $m_i=r\sum_jb_{ij}m_j$. The [adjugate matrix](linear-algebra.md#adjugate-matrix) identity shows $\det(I-r(b_{ij}))$ annihilates $M$, hence is zero in $B$. Since this determinant has form $1-rq$, $r$ is invertible. Thus $B$ is a [field](algebra.md#field). If $R$ is a finite-type algebra over an algebraically closed [field](algebra.md#field) $k$, the residue [field](algebra.md#field) is $k$, and every such [simple module](#irreducible-module) is finite-dimensional over $k$.

### Simple module over a commutative ring

↑ **Parent:** [Irreducible module](#irreducible-module)

Every simple module over a commutative ring $R$ is isomorphic to $R/\mathfrak m$ for a maximal ideal $\mathfrak m$; its annihilator is therefore maximal.

## Annihilator (ring theory)

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Annihilator_(ring_theory))

The annihilator records which ring elements kill a specified subset of a module.

### Right annihilator

↑ **Parent:** [Annihilator (ring theory)](#annihilator-ring-theory)

The right annihilator of a subset $X$ of a [ring](commutative-algebra.md#ring) is the [right ideal](associative-algebra.md#right-ideal) of elements killed on the left by every member of $X$. Its sidedness matters for a [noncommutative ring](commutative-algebra.md#noncommutative-ring).

### Associated prime of a module

↑ **Parent:** [Annihilator (ring theory)](#annihilator-ring-theory)

An associated prime of an $R$-[module](#module-mathematics) $M$ is a [prime ideal](commutative-algebra.md#prime-ideal) equal to the [annihilator](#annihilator-ring-theory) $\operatorname{Ann}_R(m)$ of some nonzero $m\in M$. The set of these primes is denoted $\operatorname{Ass}_R(M)$. Over a [Noetherian ring](algebra.md#noetherian-ring), any maximal member among the [annihilators](#annihilator-ring-theory) of nonzero elements is prime: if $abm=0$ and $bm\ne0$, maximality forces $\operatorname{Ann}_R(bm)=\operatorname{Ann}_R(m)$, so $am=0$. Hence every nonzero [module](#module-mathematics) has an associated prime.

#### Localization of associated primes

↑ **Parent:** [Associated prime of a module](#associated-prime-of-a-module)

For a commutative [Noetherian ring](algebra.md#noetherian-ring), an [annihilator](#annihilator-ring-theory) $Q=\operatorname{Ann}_R(m)$ contained in $P$ localizes to the [annihilator](#annihilator-ring-theory) of the nonzero $m/1$. Conversely, contract an associated prime of $M_P$ represented by $m/1$ to an [ideal](commutative-algebra.md#ideal) $Q$. Choose finitely many generators of $Q$ and one denominator outside $P$ clearing all their annihilation equations. For this denominator $s$, the element $sm$ is nonzero and has [annihilator](#annihilator-ring-theory) exactly $Q$. This proves the formula; finite generation of the contracted [ideal](commutative-algebra.md#ideal) is the key use of [Noetherianity](algebra.md#noetherian-ring).

// Destination: noncommutative-algebra.bigb

#### Embedded associated prime

↑ **Parent:** [Associated prime of a module](#associated-prime-of-a-module)

An [associated prime of a module](#associated-prime-of-a-module) $R/I$ is embedded when it is not minimal over $I$. For example, in $k[x,y]/(x^2,xy)$ the nonzero class of $x$ has [annihilator](#annihilator-ring-theory) $(x,y)$, while the unique minimal prime is $(x)$. Embedded primes record [annihilators](#annihilator-ring-theory) which are invisible if one retains only the reduced irreducible components.

#### Minimal primes are associated primes

↑ **Parent:** [Associated prime of a module](#associated-prime-of-a-module)

For a [Noetherian ring](algebra.md#noetherian-ring) and a proper [ideal](commutative-algebra.md#ideal) $I$, every minimal prime $P$ over $I$ is an [associated prime of a module](#associated-prime-of-a-module) $R/I$. The localized quotient has one prime, so its finitely generated [maximal ideal](commutative-algebra.md#maximal-ideal) is nilpotent and its [socle](#socle-mathematics) is nonzero. An element with [annihilator](#annihilator-ring-theory) $PR_P$ can be lifted to the quotient. Clearing denominators for a finite generating set of $P$ gives a nonzero element with [annihilator](#annihilator-ring-theory) exactly $P$.

### Annihilator of a module

↑ **Parent:** [Annihilator (ring theory)](#annihilator-ring-theory)

The annihilator $\operatorname{Ann}_R(M)$ is the ideal of scalars that kill every element of $M$.

#### Maximal annihilator of a module element is prime

↑ **Parent:** [Annihilator of a module](#annihilator-of-a-module)

Over a commutative unital [ring](commutative-algebra.md#ring), an ideal maximal among annihilators of nonzero elements of a [module](#module-mathematics) is a [prime ideal](commutative-algebra.md#prime-ideal). Each such ideal is the [annihilator of a module](#annihilator-of-a-module) given by the cyclic submodule generated by that element. If $P=\operatorname{Ann}(m)$ and $ab\in P$ with $b\notin P$, then $bm\ne0$ and $P\subseteq\operatorname{Ann}(bm)$. Maximality makes these annihilators equal, so $a\in P$. A [Noetherian ring](algebra.md#noetherian-ring) ensures that a nonzero module has a maximal element annihilator by the [ascending chain condition](algebra.md#ascending-chain-condition) on ideals.

## Structure theorem for finitely generated modules over a principal ideal domain

↑ **Parent:** [Module theory](module-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Structure_theorem_for_finitely_generated_modules_over_a_principal_ideal_domain)

Every finitely generated module over a PID is a direct sum of a free module and cyclic prime-power torsion modules.

### Invariant factor of a finitely generated module

↑ **Parent:** [Structure theorem for finitely generated modules over a principal ideal domain](#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)

For a [finitely generated module](#finitely-generated-module) over a [principal ideal domain](commutative-algebra.md#principal-ideal-domain), its invariant factors are nonzero nonunits $d_i$ in a decomposition $M\cong R^r\oplus\bigoplus_iR/(d_i)$, ordered by $d_i\mid d_{i+1}$. They are unique up to multiplication by units and describe the [torsion submodule](#torsion-submodule). Over $F[t]$, making $t$ act as a [linear operator](vector-space.md#linear-operator) recovers the [invariant factors of a linear operator](linear-operator-theory.md#invariant-factors-of-a-linear-operator) used in its [rational canonical form](linear-operator-theory.md#rational-canonical-form).

### Finitely generated torsion-free module over a principal ideal domain

↑ **Parent:** [Structure theorem for finitely generated modules over a principal ideal domain](#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)

Every finitely generated torsion-free module over a principal ideal domain is free. In the structure theorem, torsion-freeness removes every cyclic torsion summand and leaves only the free summand.

#### Classification of integral matrices satisfying the third cyclotomic polynomial

↑ **Parent:** [Finitely generated torsion-free module over a principal ideal domain](#finitely-generated-torsion-free-module-over-a-principal-ideal-domain)

An integral matrix satisfying $A^2+A+I=0$ makes $\mathbb Z^n$ a module over the [Eisenstein integers](commutative-algebra.md#eisenstein-integer) by letting the primitive cube root act as $A$. This module is finitely generated and torsion-free, hence free. Since the Eisenstein integers have integer rank two, such matrices exist only for $n=2m$; for that dimension every one is integrally conjugate to

$$
\begin{pmatrix}0&-1\\1&-1\end{pmatrix}^{\oplus m}.
$$

### Elementary divisor

↑ **Parent:** [Structure theorem for finitely generated modules over a principal ideal domain](#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elementary_divisor)

An elementary divisor is a prime power $p^e$ occurring in the cyclic decomposition of a finitely generated torsion module.

### Indecomposable finite abelian groups

↑ **Parent:** [Structure theorem for finitely generated modules over a principal ideal domain](#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain)

A finite abelian group is indecomposable exactly when it is cyclic of prime-power order. The structure theorem proves necessity. Conversely, every nonzero subgroup of $C_{p^n}$ contains its unique subgroup of order $p$, so two nonzero subgroups cannot be complementary direct summands.

## ↑ Ancestors (5)

1. [Commutative algebra](commutative-algebra.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
