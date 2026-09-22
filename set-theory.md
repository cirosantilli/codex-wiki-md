# Set theory

↑ **Parent:** [Foundations of mathematics](foundations-of-mathematics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Set_theory)

**Table of contents**

- [Russell's paradox](#russell-s-paradox)
- [Urelement](#urelement)
  - [Basic Fraenkel permutation model](#basic-fraenkel-permutation-model)
- [Hereditarily locally small membership model](#hereditarily-locally-small-membership-model)
- [New Foundations](#new-foundations)
  - [New Foundations with urelements](#new-foundations-with-urelements)
    - [Type-shifting automorphism](#type-shifting-automorphism)
      - [Rank-shifting automorphism construction of NFU](#rank-shifting-automorphism-construction-of-nfu)
        - [Rank-shifting NFU model with explicit set predicate](#rank-shifting-nfu-model-with-explicit-set-predicate)
          - [Rank-indiscernible construction of an NFU model](#rank-indiscernible-construction-of-an-nfu-model)
    - [Stratified formula](#stratified-formula)
- [Simple typed set theory with atoms](#simple-typed-set-theory-with-atoms)
  - [Typical ambiguity](#typical-ambiguity)
- [Axiom of pairing](#axiom-of-pairing)
- [Axiom of extensionality](#axiom-of-extensionality)
  - [Non-extensional membership model with one atom](#non-extensional-membership-model-with-one-atom)
- [Independent family of sets](#independent-family-of-sets)
  - [Fichtenholz-Kantorovich independent family](#fichtenholz-kantorovich-independent-family)
- [Almost disjoint family on a regular cardinal](#almost-disjoint-family-on-a-regular-cardinal)
  - [Essential disjointness of small subfamilies](#essential-disjointness-of-small-subfamilies)
- [Kappa-filtration](#kappa-filtration)
  - [Club agreement of countable filtrations](#club-agreement-of-countable-filtrations)
- [Almost disjoint family on omega](#almost-disjoint-family-on-omega)
  - [Maximal almost disjoint family on omega](#maximal-almost-disjoint-family-on-omega)
    - [Almost disjointness number](#almost-disjointness-number)
      - [Bounding-to-almost-disjointness inequality](#bounding-to-almost-disjointness-inequality)
- [Standard membership model of set theory](#standard-membership-model-of-set-theory)
- [Partition relation](#partition-relation)
  - [Finite-symmetric-difference colouring of infinite subsets](#finite-symmetric-difference-colouring-of-infinite-subsets)
  - [Erdős-Rado theorem for finite arities](#erdos-rado-theorem-for-finite-arities)
    - [Closed elementary-submodel construction of an end-homogeneous sequence](#closed-elementary-submodel-construction-of-an-end-homogeneous-sequence)
    - [End-homogeneous routing tree](#end-homogeneous-routing-tree)
  - [Erdős-Rado theorem for pairs](#erdos-rado-theorem-for-pairs)
    - [Ordinal partition-bound function](#ordinal-partition-bound-function)
  - [Finite-subset partition property](#finite-subset-partition-property)
    - [Small forcing preservation of finite-subset partition properties](#small-forcing-preservation-of-finite-subset-partition-properties)
  - [Infinite-arity partition relation](#infinite-arity-partition-relation)
- [Eventual domination](#eventual-domination)
  - [Eventual domination on a regular cardinal](#eventual-domination-on-a-regular-cardinal)
    - [Long chain under eventual domination](#long-chain-under-eventual-domination)
  - [Bounding number](#bounding-number)
  - [Dominating family](#dominating-family)
- [Sierpiński decomposition of the plane](#sierpinski-decomposition-of-the-plane)
- [Definable continuous hierarchy](#definable-continuous-hierarchy)
- [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)
  - [Zermelo set theory](#zermelo-set-theory)
    - [Axiom of limitation of size](#axiom-of-limitation-of-size)
  - [Intuitionistic Zermelo–Fraenkel set theory](#intuitionistic-zermelo-fraenkel-set-theory)
    - [Boolean-valued inner universe over intuitionistic set theory](#boolean-valued-inner-universe-over-intuitionistic-set-theory)
      - [Boolean-valued name](#boolean-valued-name)
      - [Collection for Boolean-valued names](#collection-for-boolean-valued-names)
  - [Rieger-Bernays permutation model](#rieger-bernays-permutation-model)
    - [Quine atom](#quine-atom)
      - [Extensional cumulative universe over Quine atoms](#extensional-cumulative-universe-over-quine-atoms)
      - [Hereditarily finite-supported Quine-atom model](#hereditarily-finite-supported-quine-atom-model)
  - [Axiom of infinity](#axiom-of-infinity)
    - [Inductive set](#inductive-set)
  - [Zermelo–Fraenkel set theory with choice](#zermelo-fraenkel-set-theory-with-choice)
- [Von Neumann hierarchy](#von-neumann-hierarchy)
  - [Countable rank-initial segment cannot model ZFC](#countable-rank-initial-segment-cannot-model-zfc)
  - [Lévy reflection theorem](#levy-reflection-theorem)
    - [Club reflection below an inaccessible cardinal](#club-reflection-below-an-inaccessible-cardinal)
    - [Reflection theorem for definable hierarchies](#reflection-theorem-for-definable-hierarchies)
    - [Ordinal described by a first-order formula](#ordinal-described-by-a-first-order-formula)
  - [Rank of a set](#rank-of-a-set)
- [Definable power set](definable-power-set.md)
  - [Finite relation closure for set-theoretic coding](definable-power-set.md#finite-relation-closure-for-set-theoretic-coding)
  - [Constructible hierarchy](definable-power-set.md#constructible-hierarchy)
    - [Constructible sets of low rank can appear at later stages](definable-power-set.md#constructible-sets-of-low-rank-can-appear-at-later-stages)
    - [Absoluteness of constructible levels](definable-power-set.md#absoluteness-of-constructible-levels)
      - [Constructible-level absoluteness over ZF](definable-power-set.md#constructible-level-absoluteness-over-zf)
    - [Constructible universe](definable-power-set.md#constructible-universe)
      - [Shepherdson's wall](definable-power-set.md#shepherdson-s-wall)
      - [Axiom of constructibility](definable-power-set.md#axiom-of-constructibility)
      - [Separation proof in the constructible universe](definable-power-set.md#separation-proof-in-the-constructible-universe)
      - [Constructible universe theorem](definable-power-set.md#constructible-universe-theorem)
      - [Diamond theorem in the constructible universe](definable-power-set.md#diamond-theorem-in-the-constructible-universe)
      - [Countability of constructible omega-one](definable-power-set.md#countability-of-constructible-omega-one)
      - [Hereditarily countable constructible sets appear below omega-one](definable-power-set.md#hereditarily-countable-constructible-sets-appear-below-omega-one)
      - [Constructible power set](definable-power-set.md#constructible-power-set)
      - [Relative constructible universe](definable-power-set.md#relative-constructible-universe)
        - [Inner models with all reals preserve omega-one](definable-power-set.md#inner-models-with-all-reals-preserve-omega-one)
        - [Relative constructible hierarchy](definable-power-set.md#relative-constructible-hierarchy)
          - [Relative condensation lemma](definable-power-set.md#relative-condensation-lemma)
          - [Relative constructible level recognition](definable-power-set.md#relative-constructible-level-recognition)
          - [Coded relative constructible stage](definable-power-set.md#coded-relative-constructible-stage)
            - [Stage histories appear below every limit constructible level](definable-power-set.md#stage-histories-appear-below-every-limit-constructible-level)
        - [Relative constructible universe can violate the continuum hypothesis](definable-power-set.md#relative-constructible-universe-can-violate-the-continuum-hypothesis)
    - [Condensation sentence for the constructible hierarchy](definable-power-set.md#condensation-sentence-for-the-constructible-hierarchy)
    - [Well-order code](definable-power-set.md#well-order-code)
    - [Coding level of the constructible hierarchy](definable-power-set.md#coding-level-of-the-constructible-hierarchy)
    - [Condensation lemma for the constructible universe](definable-power-set.md#condensation-lemma-for-the-constructible-universe)
- [Forcing](forcing.md)
  - [Forcing antichain](forcing.md#forcing-antichain)
  - [Cardinal collapse](forcing.md#cardinal-collapse)
  - [Cofinality-preserving forcing](forcing.md#cofinality-preserving-forcing)
  - [Martin's axiom](forcing.md#martin-s-axiom)
  - [Countable forcing](forcing.md#countable-forcing)
    - [One-Cohen-real preservation of GCH](forcing.md#one-cohen-real-preservation-of-gch)
    - [Countable forcing preserves Suslin trees](forcing.md#countable-forcing-preserves-suslin-trees)
    - [Ground-model uncountable subset lemma for countable forcing](forcing.md#ground-model-uncountable-subset-lemma-for-countable-forcing)
  - [Separative forcing order](forcing.md#separative-forcing-order)
  - [Forcing atom](forcing.md#forcing-atom)
    - [A forcing atom determines a ground-model generic filter](forcing.md#a-forcing-atom-determines-a-ground-model-generic-filter)
    - [Atomless forcing order](forcing.md#atomless-forcing-order)
      - [Generic filter for an atomless order is new](forcing.md#generic-filter-for-an-atomless-order-is-new)
  - [Product forcing](forcing.md#product-forcing)
    - [Mutual genericity for product forcing](forcing.md#mutual-genericity-for-product-forcing)
    - [Projection of a product-generic filter](forcing.md#projection-of-a-product-generic-filter)
  - [Infinite-reservoir stem forcing](forcing.md#infinite-reservoir-stem-forcing)
  - [Unbounded real over a model](forcing.md#unbounded-real-over-a-model)
  - [Cardinal-preserving forcing](forcing.md#cardinal-preserving-forcing)
  - [Forcing name](forcing.md#forcing-name)
    - [Forcing name rank](forcing.md#forcing-name-rank)
    - [Choice preservation by well-ordered names](forcing.md#choice-preservation-by-well-ordered-names)
    - [Nice forcing name](forcing.md#nice-forcing-name)
    - [Paired forcing name](forcing.md#paired-forcing-name)
    - [Forcing name for the complement of a generic filter](forcing.md#forcing-name-for-the-complement-of-a-generic-filter)
    - [Evaluation of a forcing name](forcing.md#evaluation-of-a-forcing-name)
    - [Canonical forcing name](forcing.md#canonical-forcing-name)
  - [Finite-function collapse to countable size](forcing.md#finite-function-collapse-to-countable-size)
    - [GCH preservation by a finite-function collapse](forcing.md#gch-preservation-by-a-finite-function-collapse)
  - [Standard notation for forcing](forcing.md#standard-notation-for-forcing)
  - [Jerusalem notation for forcing](forcing.md#jerusalem-notation-for-forcing)
  - [Compatible forcing conditions](forcing.md#compatible-forcing-conditions)
    - [Incompatible forcing conditions](forcing.md#incompatible-forcing-conditions)
  - [Dense subset of a forcing order](forcing.md#dense-subset-of-a-forcing-order)
    - [Dense above a forcing condition](forcing.md#dense-above-a-forcing-condition)
    - [Dense below a forcing condition](forcing.md#dense-below-a-forcing-condition)
      - [Dense-below generic meeting lemma](forcing.md#dense-below-generic-meeting-lemma)
  - [Generic filter](forcing.md#generic-filter)
    - [Maximal-antichain criterion for genericity](forcing.md#maximal-antichain-criterion-for-genericity)
    - [Rasiowa–Sikorski lemma](forcing.md#rasiowa-sikorski-lemma)
    - [Generic extension](forcing.md#generic-extension)
      - [Power-set failure in an increasing union of generic extensions](forcing.md#power-set-failure-in-an-increasing-union-of-generic-extensions)
      - [Power set in a generic extension](forcing.md#power-set-in-a-generic-extension)
      - [Forcing theorem](forcing.md#forcing-theorem)
        - [Forcing decision pattern](forcing.md#forcing-decision-pattern)
        - [Forcing preserves ordinals](forcing.md#forcing-preserves-ordinals)
        - [Forcing truth lemma](forcing.md#forcing-truth-lemma)
        - [Forcing definability lemma](forcing.md#forcing-definability-lemma)
        - [Semantic forcing relation](forcing.md#semantic-forcing-relation)
        - [Syntactic forcing relation](forcing.md#syntactic-forcing-relation)
          - [Atomic membership truth lemma for forcing](forcing.md#atomic-membership-truth-lemma-for-forcing)
          - [Existential clause of syntactic forcing](forcing.md#existential-clause-of-syntactic-forcing)
        - [Separation in a generic extension](forcing.md#separation-in-a-generic-extension)
  - [Countable transitive model](forcing.md#countable-transitive-model)
  - [Cohen forcing](forcing.md#cohen-forcing)
    - [Cohen forcing two-level continuum plateau](forcing.md#cohen-forcing-two-level-continuum-plateau)
  - [Eventually different forcing](forcing.md#eventually-different-forcing)
  - [Fn forcing](forcing.md#fn-forcing)
    - [Countable chain condition for finite-function forcing](forcing.md#countable-chain-condition-for-finite-function-forcing)
    - [Generic coordinate reals for finite-function forcing](forcing.md#generic-coordinate-reals-for-finite-function-forcing)
  - [Chain condition for forcing](forcing.md#chain-condition-for-forcing)
    - [Ground-model club containment lemma](forcing.md#ground-model-club-containment-lemma)
    - [Possible-values lemma for chain-condition forcing](forcing.md#possible-values-lemma-for-chain-condition-forcing)
      - [Cardinal preservation by chain-condition forcing](forcing.md#cardinal-preservation-by-chain-condition-forcing)
    - [Countable chain condition for forcing](forcing.md#countable-chain-condition-for-forcing)
      - [Knaster forcing](forcing.md#knaster-forcing)
        - [Knaster forcing preserves Suslin trees](forcing.md#knaster-forcing-preserves-suslin-trees)
  - [Closed forcing](forcing.md#closed-forcing)
    - [Closed forcing adds no short ground-valued sequences](forcing.md#closed-forcing-adds-no-short-ground-valued-sequences)
    - [Countably closed forcing](forcing.md#countably-closed-forcing)
      - [Diamond-sequence forcing](forcing.md#diamond-sequence-forcing)
      - [Countable-condition collapse](forcing.md#countable-condition-collapse)
    - [Closed forcing adds no short ordinal sequences](forcing.md#closed-forcing-adds-no-short-ordinal-sequences)
      - [Cardinal preservation by closed forcing](forcing.md#cardinal-preservation-by-closed-forcing)
  - [Antichain in a forcing order](forcing.md#antichain-in-a-forcing-order)
  - [Centered subset of a forcing order](forcing.md#centered-subset-of-a-forcing-order)
    - [Sigma-centered forcing](forcing.md#sigma-centered-forcing)
  - [Hechler forcing](forcing.md#hechler-forcing)
    - [Dominating real](forcing.md#dominating-real)
  - [Nice name for a real](forcing.md#nice-name-for-a-real)
  - [Finite-condition Lévy collapse](forcing.md#finite-condition-levy-collapse)
    - [Finite Lévy collapse to omega-one](forcing.md#finite-levy-collapse-to-omega-one)
    - [Maximal-antichain sizes in the finite Lévy collapse](forcing.md#maximal-antichain-sizes-in-the-finite-levy-collapse)
- [Delta-system lemma](#delta-system-lemma)
  - [Generalized delta-system lemma](#generalized-delta-system-lemma)
  - [Delta-system](#delta-system)
    - [Erdős–Rado sunflower lemma](#erdos-rado-sunflower-lemma)
  - [Delta-system lemma at a regular uncountable cardinal](#delta-system-lemma-at-a-regular-uncountable-cardinal)
- [Standard model (set theory)](#standard-model-set-theory)
- [Transitive set](#transitive-set)
  - [Transitive model](#transitive-model)
    - [Well-founded model of set theory](#well-founded-model-of-set-theory)
    - [Ordinal height of a model of set theory](#ordinal-height-of-a-model-of-set-theory)
      - [Uncountable transitive set model has uncountable ordinal height](#uncountable-transitive-set-model-has-uncountable-ordinal-height)
        - [Countable-ordinal correctness under constructibility](#countable-ordinal-correctness-under-constructibility)
- [Well-founded relation](#well-founded-relation)
  - [Intersection-power-set predecessor relation](#intersection-power-set-predecessor-relation)
  - [Power-set-predecessor relation](#power-set-predecessor-relation)
  - [Well-founded induction](#well-founded-induction)
  - [Well-founded recursion](#well-founded-recursion)
    - [Recursive powerset mapping](#recursive-powerset-mapping)
    - [Ordinal rank function for a relation](#ordinal-rank-function-for-a-relation)
      - [Rank of a well-founded tree](#rank-of-a-well-founded-tree)
        - [Maurey hierarchy of finite sets](#maurey-hierarchy-of-finite-sets)
  - [Set-like relation](#set-like-relation)
- [Extensional relation](#extensional-relation)
- [Set](set.md)
  - [Partition of a set](set.md#partition-of-a-set)
    - [Colouring of a set](set.md#colouring-of-a-set)
  - [Coinfinite set](set.md#coinfinite-set)
  - [Dedekind-finite set](set.md#dedekind-finite-set)
    - [Finite repetition-free sequences preserve Dedekind-finiteness](set.md#finite-repetition-free-sequences-preserve-dedekind-finiteness)
    - [Infinite Dedekind-finite set](set.md#infinite-dedekind-finite-set)
  - [Set difference](set.md#set-difference)
  - [Complement of a set](set.md#complement-of-a-set)
  - [Pointed set](set.md#pointed-set)
  - [Multiset](set.md#multiset)
  - [Nondecreasing family of sets](set.md#nondecreasing-family-of-sets)
  - [Power set](set.md#power-set)
    - [Cantor's theorem](set.md#cantor-s-theorem)
  - [Finite set](set.md#finite-set)
  - [Infinite set](set.md#infinite-set)
  - [Empty set](set.md#empty-set)
  - [Singleton (mathematics)](set.md#singleton-mathematics)
  - [Distinct elements](set.md#distinct-elements)
  - [Generating set](set.md#generating-set)
  - [Subset](set.md#subset)
  - [Set union](set.md#set-union)
    - [Countable union](set.md#countable-union)
  - [Set intersection](set.md#set-intersection)
    - [Countable intersection](set.md#countable-intersection)
  - [Symmetric difference](set.md#symmetric-difference)
    - [Finite symmetric difference](set.md#finite-symmetric-difference)
  - [Pair](set.md#pair)
    - [Ordered pair](set.md#ordered-pair)
      - [Kuratowski ordered pair](set.md#kuratowski-ordered-pair)
    - [Unordered pair](set.md#unordered-pair)
  - [Preorder](set.md#preorder)
    - [Hoare domination preorder](set.md#hoare-domination-preorder)
      - [Finite-subset lifting of a well-quasi-order](set.md#finite-subset-lifting-of-a-well-quasi-order)
    - [Well-quasi-ordering](set.md#well-quasi-ordering)
      - [Perfect subsequence lemma](set.md#perfect-subsequence-lemma)
      - [Finite product closure of well-quasi-orderings](set.md#finite-product-closure-of-well-quasi-orderings)
      - [Better-quasi-ordering](set.md#better-quasi-ordering)
        - [Power-set closure of better-quasi-orderings](set.md#power-set-closure-of-better-quasi-orderings)
        - [Continuous array in better-quasi-order theory](set.md#continuous-array-in-better-quasi-order-theory)
        - [Barrier in better-quasi-order theory](set.md#barrier-in-better-quasi-order-theory)
          - [Nash-Williams barrier partition theorem](set.md#nash-williams-barrier-partition-theorem)
      - [Rado order](set.md#rado-order)
        - [Bad barrier array for the Rado order](set.md#bad-barrier-array-for-the-rado-order)
      - [Higman's lemma](set.md#higman-s-lemma)
      - [Bad sequence](set.md#bad-sequence)
        - [Minimal bad sequence](set.md#minimal-bad-sequence)
      - [Finite bad-sequence tree](set.md#finite-bad-sequence-tree)
      - [Kruskal's tree theorem](set.md#kruskal-s-tree-theorem)
        - [Labelled version of Kruskal's tree theorem](set.md#labelled-version-of-kruskal-s-tree-theorem)
        - [Friedman's finite form of Kruskal's theorem](set.md#friedman-s-finite-form-of-kruskal-s-theorem)
  - [Partially ordered set](set.md#partially-ordered-set)
    - [Upper and lower sets](set.md#upper-and-lower-sets)
    - [Greatest element and least element](set.md#greatest-element-and-least-element)
      - [Greatest element](set.md#greatest-element)
    - [Maximal and minimal elements](set.md#maximal-and-minimal-elements)
      - [Maximal element of a partially ordered set](set.md#maximal-element-of-a-partially-ordered-set)
      - [Minimal element of a partially ordered set](set.md#minimal-element-of-a-partially-ordered-set)
    - [Upper and lower bounds](set.md#upper-and-lower-bounds)
      - [Upper bound in a partially ordered set](set.md#upper-bound-in-a-partially-ordered-set)
        - [Least upper bound in a partially ordered set](set.md#least-upper-bound-in-a-partially-ordered-set)
    - [Increasing function on a partially ordered set](set.md#increasing-function-on-a-partially-ordered-set)
    - [Szpilrajn extension theorem](set.md#szpilrajn-extension-theorem)
    - [Dilworth's theorem](set.md#dilworth-s-theorem)
    - [Lower bound in a partially ordered set](set.md#lower-bound-in-a-partially-ordered-set)
      - [Greatest lower bound in a partially ordered set](set.md#greatest-lower-bound-in-a-partially-ordered-set)
    - [Chain-complete partially ordered set](set.md#chain-complete-partially-ordered-set)
    - [Complete partial order](set.md#complete-partial-order)
      - [Directed-complete partial order](set.md#directed-complete-partial-order)
        - [Scott continuous map](set.md#scott-continuous-map)
        - [Pointed complete partial order](set.md#pointed-complete-partial-order)
          - [Embedding-projection pair](set.md#embedding-projection-pair)
            - [Inverse-limit solution of the reflexive domain equation](set.md#inverse-limit-solution-of-the-reflexive-domain-equation)
          - [Function space of complete partial orders](set.md#function-space-of-complete-partial-orders)
            - [Pointwise directed supremum](set.md#pointwise-directed-supremum)
        - [Least fixed point from a directed family of maps](set.md#least-fixed-point-from-a-directed-family-of-maps)
    - [Product order](set.md#product-order)
      - [Maximal external point](set.md#maximal-external-point)
        - [Expected number of coordinatewise maxima](set.md#expected-number-of-coordinatewise-maxima)
    - [Strict partial order](set.md#strict-partial-order)
      - [Reflexification of a strict partial order](set.md#reflexification-of-a-strict-partial-order)
    - [Chain-poset nonembedding lemma](set.md#chain-poset-nonembedding-lemma)
    - [Set-theoretic tree](set.md#set-theoretic-tree)
      - [Branching form of the tree property](set.md#branching-form-of-the-tree-property)
      - [Splitting tree](set.md#splitting-tree)
      - [Tree with unique limits](set.md#tree-with-unique-limits)
      - [Well-pruned set-theoretic tree](set.md#well-pruned-set-theoretic-tree)
        - [Unbounded-extension kernel of a regular tree](set.md#unbounded-extension-kernel-of-a-regular-tree)
      - [Kappa-tree](set.md#kappa-tree)
        - [Tree property](set.md#tree-property)
        - [Uniformly narrow regular-height tree branch theorem](set.md#uniformly-narrow-regular-height-tree-branch-theorem)
      - [Kurepa tree](set.md#kurepa-tree)
        - [Kurepa tree from an inaccessible binary tree](set.md#kurepa-tree-from-an-inaccessible-binary-tree)
        - [Kurepa hypothesis](set.md#kurepa-hypothesis)
        - [Kurepa-family hypothesis](set.md#kurepa-family-hypothesis)
      - [Aronszajn tree](set.md#aronszajn-tree)
        - [Coherent-injection Aronszajn tree](set.md#coherent-injection-aronszajn-tree)
        - [Suslin tree](set.md#suslin-tree)
          - [Suslin-tree obstruction to Martin's axiom](set.md#suslin-tree-obstruction-to-martin-s-axiom)
        - [Special Aronszajn tree](set.md#special-aronszajn-tree)
          - [Rationally labelled Aronszajn tree construction](set.md#rationally-labelled-aronszajn-tree-construction)
            - [Bounded rational extension property](set.md#bounded-rational-extension-property)
        - [Aleph-two Aronszajn tree](set.md#aleph-two-aronszajn-tree)
      - [Normal set-theoretic tree](set.md#normal-set-theoretic-tree)
      - [Cofinal branch](set.md#cofinal-branch)
      - [Tree antichain](set.md#tree-antichain)
    - [Chain in a partial order](set.md#chain-in-a-partial-order)
    - [Differential poset](set.md#differential-poset)
      - [Normal ordering identity for up and down operators](set.md#normal-ordering-identity-for-up-and-down-operators)
    - [Filter (mathematics)](set.md#filter-mathematics)
      - [Principal filter in an ordered set](set.md#principal-filter-in-an-ordered-set)
    - [Linear extension](set.md#linear-extension)
      - [Reduced adjacent-swap path between linear extensions](set.md#reduced-adjacent-swap-path-between-linear-extensions)
    - [Order-preserving function](set.md#order-preserving-function)
      - [Inflationary map](set.md#inflationary-map)
      - [Strict order-preserving function](set.md#strict-order-preserving-function)
    - [Order dimension](set.md#order-dimension)
      - [Two-dimensional partially ordered set](set.md#two-dimensional-partially-ordered-set)
        - [Finite-local characterization of two-dimensional partially ordered sets](set.md#finite-local-characterization-of-two-dimensional-partially-ordered-sets)
    - [Chain in a partially ordered set](set.md#chain-in-a-partially-ordered-set)
    - [Directed set](set.md#directed-set)
  - [Total order](set.md#total-order)
    - [Minimum of a subset of a total order](set.md#minimum-of-a-subset-of-a-total-order)
    - [Maximum of a subset of a total order](set.md#maximum-of-a-subset-of-a-total-order)
    - [Totally ordered set](set.md#totally-ordered-set)
    - [Dense order](set.md#dense-order)
    - [Aleph-one-like linear order](set.md#aleph-one-like-linear-order)
      - [Stationary encoding in an aleph-one-like dense order](set.md#stationary-encoding-in-an-aleph-one-like-dense-order)
    - [Order topology](set.md#order-topology)
      - [Lexicographic order topology on the real plane](set.md#lexicographic-order-topology-on-the-real-plane)
    - [Countable chain condition for a linear order](set.md#countable-chain-condition-for-a-linear-order)
    - [Order-dense subset](set.md#order-dense-subset)
    - [Order completeness](set.md#order-completeness)
      - [Dedekind completion](set.md#dedekind-completion)
    - [Order isomorphism](set.md#order-isomorphism)
    - [Order sum](set.md#order-sum)
    - [Order automorphism](set.md#order-automorphism)
      - [Rigid dense subset of the real line](set.md#rigid-dense-subset-of-the-real-line)
      - [Extension of an order automorphism from a dense subset](set.md#extension-of-an-order-automorphism-from-a-dense-subset)
    - [Strict total order](set.md#strict-total-order)
    - [Well-order](set.md#well-order)
      - [Decidable well-order](set.md#decidable-well-order)
    - [Empty order](set.md#empty-order)
    - [Initial segment](set.md#initial-segment)
- [Binary relation](#binary-relation)
  - [Binary relations with no empty row or column](#binary-relations-with-no-empty-row-or-column)
  - [Preference relation](#preference-relation)
    - [Closed convergence of preference relations](#closed-convergence-of-preference-relations)
      - [Uniform utility convergence need not preserve closed preference convergence](#uniform-utility-convergence-need-not-preserve-closed-preference-convergence)
    - [Indifference relation](#indifference-relation)
    - [Strict preference](#strict-preference)
  - [Composition of relations](#composition-of-relations)
  - [Reflexive relation](#reflexive-relation)
    - [Reflexive closure](#reflexive-closure)
  - [Symmetric relation](#symmetric-relation)
    - [Symmetric closure](#symmetric-closure)
  - [Antisymmetric relation](#antisymmetric-relation)
  - [Transitive relation](#transitive-relation)
    - [Transitive closure (relation)](#transitive-closure-relation)
  - [Equivalence relation](#equivalence-relation)
    - [Composition of commuting equivalence relations](#composition-of-commuting-equivalence-relations)
    - [Commuting equivalence relations](#commuting-equivalence-relations)
    - [Equivalence closure](#equivalence-closure)
    - [Union of equivalence relations](#union-of-equivalence-relations)
    - [Intersection of equivalence relations](#intersection-of-equivalence-relations)
    - [Co-computably enumerable equivalence relation](#co-computably-enumerable-equivalence-relation)
      - [Semidecidable least-representative transversal](#semidecidable-least-representative-transversal)
    - [Equivalence of partial functions modulo finite changes](#equivalence-of-partial-functions-modulo-finite-changes)
    - [Equivalence class](#equivalence-class)
    - [Equivalence relation induced by a function](#equivalence-relation-induced-by-a-function)
      - [Prime-support equivalence relation](#prime-support-equivalence-relation)
    - [Quotient set](#quotient-set)
- [Function](function.md)
  - [Germ (mathematics)](function.md#germ-mathematics)
  - [Nonnegative function](function.md#nonnegative-function)
  - [Commuting functions](function.md#commuting-functions)
  - [Finite modification of the identity on the real line](function.md#finite-modification-of-the-identity-on-the-real-line)
  - [Pointwise periodic self-map](function.md#pointwise-periodic-self-map)
    - [Uniform period criterion for pointwise periodic maps](function.md#uniform-period-criterion-for-pointwise-periodic-maps)
  - [Vector-valued function](function.md#vector-valued-function)
  - [Set function](function.md#set-function)
    - [Finite additivity of a set function](function.md#finite-additivity-of-a-set-function)
    - [Supermodular set function](function.md#supermodular-set-function)
    - [Submodular set function](function.md#submodular-set-function)
  - [Function collision](function.md#function-collision)
  - [Fiber of a function](function.md#fiber-of-a-function)
    - [Factorization through a surjection](function.md#factorization-through-a-surjection)
  - [Translation of a function](function.md#translation-of-a-function)
  - [Graph of a function](function.md#graph-of-a-function)
    - [Compact graph of a continuous map](function.md#compact-graph-of-a-continuous-map)
    - [Closed graph of a map into a Hausdorff space](function.md#closed-graph-of-a-map-into-a-hausdorff-space)
  - [Partial function](function.md#partial-function)
    - [Partial unary operation](function.md#partial-unary-operation)
    - [Composition of partial functions](function.md#composition-of-partial-functions)
  - [Domain of a function](function.md#domain-of-a-function)
    - [Domain of a partial function](function.md#domain-of-a-partial-function)
  - [Function class](function.md#function-class)
  - [Support](function.md#support)
    - [Compact support](function.md#compact-support)
  - [Identity function](function.md#identity-function)
  - [Inverse function](function.md#inverse-function)
    - [Right inverse](function.md#right-inverse)
      - [Right-inverse characterization of the axiom of choice](function.md#right-inverse-characterization-of-the-axiom-of-choice)
    - [Left inverse](function.md#left-inverse)
  - [Projection (mathematics)](function.md#projection-mathematics)
    - [Projection map](function.md#projection-map)
      - [Empty-set cases for Cartesian projections](function.md#empty-set-cases-for-cartesian-projections)
  - [Fixed point](function.md#fixed-point)
  - [Conjugate functions](function.md#conjugate-functions)
  - [Piecewise linear function](function.md#piecewise-linear-function)
    - [Linear interpolation](function.md#linear-interpolation)
  - [Bounded function](function.md#bounded-function)
    - [Unbounded function](function.md#unbounded-function)
  - [Constant function](function.md#constant-function)
  - [Real-valued function](function.md#real-valued-function)
    - [Global maximum](function.md#global-maximum)
    - [Positive part of a real-valued function](function.md#positive-part-of-a-real-valued-function)
  - [Bijection](function.md#bijection)
  - [Periodic function](function.md#periodic-function)
    - [Simply periodic function](function.md#simply-periodic-function)
    - [Cardinality of integer-periodic function spaces](function.md#cardinality-of-integer-periodic-function-spaces)
    - [Period average](function.md#period-average)
    - [Triangular wave](function.md#triangular-wave)
- [Zorn's lemma](#zorn-s-lemma)
- [Class (set theory)](#class-set-theory)
  - [Set-theoretic class function](#set-theoretic-class-function)
  - [Proper class](#proper-class)
  - [Transitive class](#transitive-class)
    - [Basic set-theoretic axioms inherited by a transitive class](#basic-set-theoretic-axioms-inherited-by-a-transitive-class)
    - [Formula relativization to a class](#formula-relativization-to-a-class)
      - [Set-theoretic absoluteness](#set-theoretic-absoluteness)
        - [Delta-one absoluteness](#delta-one-absoluteness)
        - [Absoluteness of well-foundedness](#absoluteness-of-well-foundedness)
        - [Absolute formula](#absolute-formula)
        - [Absoluteness of cardinalhood in limit ranks](#absoluteness-of-cardinalhood-in-limit-ranks)
        - [Upward absolute formula](#upward-absolute-formula)
        - [Downward absolute formula](#downward-absolute-formula)
        - [Bounded formula in set theory](#bounded-formula-in-set-theory)
          - [ZF-equivalent bounded formula](#zf-equivalent-bounded-formula)
        - [Absoluteness of infinitude between transitive models](#absoluteness-of-infinitude-between-transitive-models)
        - [Downward absoluteness of cardinalhood](#downward-absoluteness-of-cardinalhood)
        - [Upward absoluteness of countability](#upward-absoluteness-of-countability)
        - [Nonabsoluteness of singular cardinalhood](#nonabsoluteness-of-singular-cardinalhood)
        - [Cardinal nonabsoluteness in a small transitive model](#cardinal-nonabsoluteness-in-a-small-transitive-model)
        - [Strong-inaccessibility absoluteness from rank agreement](#strong-inaccessibility-absoluteness-from-rank-agreement)
        - [Lévy hierarchy](#levy-hierarchy)
          - [Delta-one formula modulo ZFC](#delta-one-formula-modulo-zfc)
          - [Pi-one formula in set theory](#pi-one-formula-in-set-theory)
          - [Sigma-one formula in set theory](#sigma-one-formula-in-set-theory)
          - [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf)
            - [Regular cardinalhood is Pi-one definable](#regular-cardinalhood-is-pi-one-definable)
            - [Cardinalhood is Pi-one definable](#cardinalhood-is-pi-one-definable)
          - [Delta-one formula in set theory](#delta-one-formula-in-set-theory)
- [Axiom schema of replacement](#axiom-schema-of-replacement)
  - [Axiom schema of collection](#axiom-schema-of-collection)
  - [Full second-order replacement rank obstruction](#full-second-order-replacement-rank-obstruction)
- [Axiom of union](#axiom-of-union)
- [Axiom of regularity](#axiom-of-regularity)
  - [Epsilon induction](#epsilon-induction)
    - [Epsilon-recursion theorem](#epsilon-recursion-theorem)
- [Axiom of power set](#axiom-of-power-set)
- [Cumulative hierarchy](#cumulative-hierarchy)
  - [Transitive closure](#transitive-closure)
    - [Transitive closure preserves set-theoretic rank](#transitive-closure-preserves-set-theoretic-rank)
    - [Hereditarily small set](#hereditarily-small-set)
      - [Power-set failure in hereditarily small sets](#power-set-failure-in-hereditarily-small-sets)
    - [Finite-power-set hereditary-small construction](#finite-power-set-hereditary-small-construction)
    - [Hereditarily countable set](#hereditarily-countable-set)
      - [Axioms satisfied by hereditarily countable sets](#axioms-satisfied-by-hereditarily-countable-sets)
      - [Countable membership coding](#countable-membership-coding)
      - [Countable-subset closure](#countable-subset-closure)
      - [Reasonable set](#reasonable-set)
  - [Hereditarily finite set](#hereditarily-finite-set)
  - [Finite von Neumann ordinal](#finite-von-neumann-ordinal)
- [Axiom schema of specification](#axiom-schema-of-specification)
  - [Restricted set comprehension](#restricted-set-comprehension)
  - [Relativized closure criterion for separation](#relativized-closure-criterion-for-separation)
- [Axiom of choice](#axiom-of-choice)
  - [Axiom of global choice](#axiom-of-global-choice)
  - [Axiom of countable choice](#axiom-of-countable-choice)
    - [Countable product compactness implies countable choice](#countable-product-compactness-implies-countable-choice)
  - [Choice function](#choice-function)
  - [Restricted axiom of choice](#restricted-axiom-of-choice)
  - [Well-ordering theorem](#well-ordering-theorem)
    - [Choice-function well-ordering construction](#choice-function-well-ordering-construction)
  - [Cardinal comparability principle](#cardinal-comparability-principle)
- [Hartogs theorem](#hartogs-theorem)
  - [Hartogs number](#hartogs-number)
    - [Hartogs numbers under choice](#hartogs-numbers-under-choice)
- [Tarski cardinal-square theorem](#tarski-cardinal-square-theorem)
- [Image and preimage of a function](#image-and-preimage-of-a-function)
  - [Image of a function](#image-of-a-function)
  - [Preimage](#preimage)
- [Cartesian product](#cartesian-product)
  - [Affine section of a planar set](#affine-section-of-a-planar-set)
    - [Universal planar set for countable real sections](#universal-planar-set-for-countable-real-sections)
  - [Universal property of Cartesian products](#universal-property-of-cartesian-products)
    - [Joint injectivity of a pair of functions](#joint-injectivity-of-a-pair-of-functions)
  - [Finite tuple](#finite-tuple)
- [Disjoint union](#disjoint-union)
- [Fiber product of sets](#fiber-product-of-sets)
- [Cantor diagonal argument](#cantor-diagonal-argument)
- [Elementary embedding](#elementary-embedding)
  - [Elementarity](#elementarity)
  - [Kunen inconsistency theorem](#kunen-inconsistency-theorem)
  - [Critical point of an elementary embedding](#critical-point-of-an-elementary-embedding)
  - [Ultrapower embedding](#ultrapower-embedding)
  - [Beta-strong elementary embedding](#beta-strong-elementary-embedding)
    - [One-strong cardinal](#one-strong-cardinal)
    - [Beta-stable cardinal property](#beta-stable-cardinal-property)
      - [Reflection by a beta-strong embedding](#reflection-by-a-beta-strong-embedding)
        - [Reflection below a cardinal](#reflection-below-a-cardinal)
  - [Kunen critical sequence](#kunen-critical-sequence)
    - [Kunen lemma](#kunen-lemma)
- [Cardinal number](#cardinal-number)
  - [Limit cardinal](#limit-cardinal)
  - [Cardinality](#cardinality)
  - [Successor cardinal](#successor-cardinal)
  - [Cofinality](#cofinality)
    - [Cofinality of a continuous cardinal hierarchy](#cofinality-of-a-continuous-cardinal-hierarchy)
    - [Cofinal map](#cofinal-map)
    - [Cofinality of an increasing ordinal supremum](#cofinality-of-an-increasing-ordinal-supremum)
    - [Singular cardinal](#singular-cardinal)
      - [Bukovský-Hechler theorem](#bukovsky-hechler-theorem)
      - [Singular cardinal enumeration](#singular-cardinal-enumeration)
        - [Cardinal fixed point of the singular cardinal enumeration](#cardinal-fixed-point-of-the-singular-cardinal-enumeration)
      - [Singular cardinals hypothesis](#singular-cardinals-hypothesis)
    - [Cofinal function](#cofinal-function)
    - [Regular cardinal](#regular-cardinal)
  - [Large cardinal](#large-cardinal)
    - [Supercompact cardinal](#supercompact-cardinal)
      - [Supercompact Sigma-two downward reflection](#supercompact-sigma-two-downward-reflection)
    - [Mahlo cardinal](#mahlo-cardinal)
      - [Mahloness is downward absolute to the constructible universe](#mahloness-is-downward-absolute-to-the-constructible-universe)
    - [Weakly inaccessible cardinal](#weakly-inaccessible-cardinal)
      - [Weakly Mahlo cardinal](#weakly-mahlo-cardinal)
      - [Model of ZFC without weakly inaccessible cardinals](#model-of-zfc-without-weakly-inaccessible-cardinals)
    - [Strong limit cardinal](#strong-limit-cardinal)
      - [Singular strong limit power-set identity](#singular-strong-limit-power-set-identity)
    - [Strongly inaccessible cardinal](#strongly-inaccessible-cardinal)
      - [Inaccessible limit of inaccessibles](#inaccessible-limit-of-inaccessibles)
        - [Rank cutoff at the first inaccessible limit of inaccessibles](#rank-cutoff-at-the-first-inaccessible-limit-of-inaccessibles)
      - [Keisler extension property](#keisler-extension-property)
    - [Worldly cardinal](#worldly-cardinal)
      - [Worldly cardinals below an inaccessible cardinal](#worldly-cardinals-below-an-inaccessible-cardinal)
      - [Nested transitive models from a worldly cardinal](#nested-transitive-models-from-a-worldly-cardinal)
      - [Arithmetic absoluteness for a rank-initial model](#arithmetic-absoluteness-for-a-rank-initial-model)
    - [Kappa-satisfiable theory](#kappa-satisfiable-theory)
    - [Least-occurrence order on cardinal properties](#least-occurrence-order-on-cardinal-properties)
      - [Nontransitivity of the least-occurrence order on cardinal properties](#nontransitivity-of-the-least-occurrence-order-on-cardinal-properties)
    - [Weakly compact cardinal](#weakly-compact-cardinal)
    - [Measurable cardinal](#measurable-cardinal)
      - [Omega-measurable cardinal](#omega-measurable-cardinal)
        - [Least omega-measurable cardinal is measurable](#least-omega-measurable-cardinal-is-measurable)
      - [Measurable cardinal is a strong limit cardinal](#measurable-cardinal-is-a-strong-limit-cardinal)
      - [Measurable cardinal is one-strong](#measurable-cardinal-is-one-strong)
      - [Two measurable cardinals under an ultrapower embedding](#two-measurable-cardinals-under-an-ultrapower-embedding)
      - [Moved critical point is not an ambient cardinal under GCH](#moved-critical-point-is-not-an-ambient-cardinal-under-gch)
    - [Strongly compact cardinal](#strongly-compact-cardinal)
  - [Countable set](#countable-set)
    - [Countability of disjoint positive-length intervals](#countability-of-disjoint-positive-length-intervals)
    - [Countability of finite subsets of a countable set](#countability-of-finite-subsets-of-a-countable-set)
    - [Cardinalities of monotone natural-number functions](#cardinalities-of-monotone-natural-number-functions)
    - [Countability of integer polynomial rings](#countability-of-integer-polynomial-rings)
    - [Countable closure under real polynomial roots](#countable-closure-under-real-polynomial-roots)
    - [Countability of pairwise disjoint open disks](#countability-of-pairwise-disjoint-open-disks)
    - [Increasing chain of countable sets](#increasing-chain-of-countable-sets)
      - [Cardinal bound for an increasing chain of countable sets](#cardinal-bound-for-an-increasing-chain-of-countable-sets)
    - [Finite Cartesian power of a countable set](#finite-cartesian-power-of-a-countable-set)
    - [Countable union of explicitly ordered finite lists without choice](#countable-union-of-explicitly-ordered-finite-lists-without-choice)
    - [Countability from vanishing averages of distinct sequences](#countability-from-vanishing-averages-of-distinct-sequences)
    - [Countably infinite set](#countably-infinite-set)
      - [Increasing enumeration of an infinite subset of natural numbers](#increasing-enumeration-of-an-infinite-subset-of-natural-numbers)
    - [Countable union of countable sets](#countable-union-of-countable-sets)
      - [Parabola obstruction to countable line coverings](#parabola-obstruction-to-countable-line-coverings)
    - [Cantor pairing function](#cantor-pairing-function)
    - [Cantor's diagonal argument](#cantor-s-diagonal-argument)
  - [Uncountable set](#uncountable-set)
    - [Uncountability of permutations of a countably infinite set](#uncountability-of-permutations-of-a-countably-infinite-set)
    - [Uncountability of surjections onto a nontrivial finite set](#uncountability-of-surjections-onto-a-nontrivial-finite-set)
  - [Initial ordinal](#initial-ordinal)
    - [Aleph number](#aleph-number)
      - [Every infinite cardinal is an aleph](#every-infinite-cardinal-is-an-aleph)
  - [Cardinal arithmetic](#cardinal-arithmetic)
    - [Gimel function](#gimel-function)
      - [Gimel recursion for cardinal exponentiation](#gimel-recursion-for-cardinal-exponentiation)
      - [Gimel hypothesis](#gimel-hypothesis)
    - [Beth number](#beth-number)
    - [Product-sum comparison lemma](#product-sum-comparison-lemma)
    - [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)
      - [Currying law for cardinal exponentiation](#currying-law-for-cardinal-exponentiation)
      - [Square of an infinite cardinal](#square-of-an-infinite-cardinal)
      - [Sum and product of two infinite cardinals](#sum-and-product-of-two-infinite-cardinals)
      - [Cardinality of a finite union of infinite sets](#cardinality-of-a-finite-union-of-infinite-sets)
      - [Countable family of distinct infinite cardinalities with a largest member](#countable-family-of-distinct-infinite-cardinalities-with-a-largest-member)
      - [Cardinal exponentiation between two and the exponent](#cardinal-exponentiation-between-two-and-the-exponent)
    - [Kőnig's theorem (set theory)](#konig-s-theorem-set-theory)
    - [Hausdorff formula for cardinal exponentiation](#hausdorff-formula-for-cardinal-exponentiation)
    - [Continuum hypothesis](#continuum-hypothesis)
      - [Freiling axiom of symmetry](#freiling-axiom-of-symmetry)
        - [Freiling theorem](#freiling-theorem)
      - [Generalized continuum hypothesis](#generalized-continuum-hypothesis)
  - [Cantor-Schröder-Bernstein theorem](#cantor-schroder-bernstein-theorem)
- [Ordinal](#ordinal)
  - [Finite ordinal](#finite-ordinal)
  - [Bounded successor characterization of finite ordinals](#bounded-successor-characterization-of-finite-ordinals)
  - [Club set](#club-set)
    - [Club of closure points for countable set-valued functions](#club-of-closure-points-for-countable-set-valued-functions)
    - [Diagonal intersection](#diagonal-intersection)
    - [Club sequence](#club-sequence)
      - [Square principle](#square-principle)
      - [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)
        - [Minimal-walk tree](#minimal-walk-tree)
        - [Trace coherence lemma for minimal walks](#trace-coherence-lemma-for-minimal-walks)
        - [First-divergence lemma for minimal walks](#first-divergence-lemma-for-minimal-walks)
    - [Stationary set](#stationary-set)
      - [Stationary partition at a successor cardinal](#stationary-partition-at-a-successor-cardinal)
      - [Non-reflecting subset](#non-reflecting-subset)
        - [Nonreflection of fixed order-type fibers](#nonreflection-of-fixed-order-type-fibers)
      - [Stationarity in a limit ordinal](#stationarity-in-a-limit-ordinal)
      - [Stationary partition by cofinal-sequence fibers](#stationary-partition-by-cofinal-sequence-fibers)
      - [Ulam matrix on omega-one](#ulam-matrix-on-omega-one)
        - [Disjoint stationary subsets of omega-one](#disjoint-stationary-subsets-of-omega-one)
      - [Diamond principle](#diamond-principle)
        - [CCC forcing cannot create diamond](#ccc-forcing-cannot-create-diamond)
        - [Stationary diamond principle](#stationary-diamond-principle)
          - [Stationary diamond at a regular cardinal](#stationary-diamond-at-a-regular-cardinal)
            - [Countable-family diamond principle](#countable-family-diamond-principle)
              - [Countable-family diamond equivalence](#countable-family-diamond-equivalence)
          - [Antichain sealing by diamond](#antichain-sealing-by-diamond)
      - [Club principle](#club-principle)
        - [Stationary-indexed club principle](#stationary-indexed-club-principle)
      - [Regressive function](#regressive-function)
        - [Fodor lemma](#fodor-lemma)
          - [Filtration form of Fodor lemma](#filtration-form-of-fodor-lemma)
      - [Stationarity of ordinals of prescribed cofinality](#stationarity-of-ordinals-of-prescribed-cofinality)
    - [Club filter](#club-filter)
      - [Stationary nonclosed member of the club filter](#stationary-nonclosed-member-of-the-club-filter)
      - [Club filter completeness](#club-filter-completeness)
    - [Closed unbounded class of ordinals](#closed-unbounded-class-of-ordinals)
  - [Successor ordinal](#successor-ordinal)
  - [Countable ordinal](#countable-ordinal)
  - [Order type](#order-type)
    - [Mostowski collapse theorem](#mostowski-collapse-theorem)
      - [Mostowski collapse](#mostowski-collapse)
      - [Transitive collapse fixes transitive subsets](#transitive-collapse-fixes-transitive-subsets)
  - [Limit ordinal](#limit-ordinal)
  - [Normal function on an ordinal](#normal-function-on-an-ordinal)
    - [Fixed point of a normal ordinal function](#fixed-point-of-a-normal-ordinal-function)
  - [Transfinite recursion](#transfinite-recursion)
    - [Natural-number recursion theorem](#natural-number-recursion-theorem)
  - [Transfinite induction](#transfinite-induction)
  - [Ordinal addition](#ordinal-addition)
    - [Associativity of ordinal addition](#associativity-of-ordinal-addition)
    - [Commuting ordinal addition](#commuting-ordinal-addition)
  - [Ordinal multiplication](#ordinal-multiplication)
    - [Ordinal division algorithm](#ordinal-division-algorithm)
    - [Commuting squares of ordinals](#commuting-squares-of-ordinals)
    - [Distributive law for ordinal multiplication](#distributive-law-for-ordinal-multiplication)
  - [Ordinal exponentiation](#ordinal-exponentiation)
    - [Epsilon zero](#epsilon-zero)
  - [Derived-set iteration of a well-order](#derived-set-iteration-of-a-well-order)
    - [Derived sets of an ordinal](#derived-sets-of-an-ordinal)
  - [Ordinal interval](#ordinal-interval)
  - [First uncountable ordinal](#first-uncountable-ordinal)
    - [First uncountable ordinal is regular](#first-uncountable-ordinal-is-regular)
    - [Tail of the first uncountable ordinal](#tail-of-the-first-uncountable-ordinal)
  - [Second uncountable ordinal](#second-uncountable-ordinal)
  - [Cantor normal form](#cantor-normal-form)
    - [Generalized Cantor normal form](#generalized-cantor-normal-form)
    - [Commensurable ordinals](#commensurable-ordinals)
    - [Computable Cantor normal form notation](#computable-cantor-normal-form-notation)
      - [Slow well-ordering below epsilon zero](#slow-well-ordering-below-epsilon-zero)
    - [Leading term of an ordinal](#leading-term-of-an-ordinal)
      - [Greatest power of omega below an ordinal](#greatest-power-of-omega-below-an-ordinal)
      - [Leading exponent of an ordinal product](#leading-exponent-of-an-ordinal-product)
  - [Additively indecomposable ordinal](#additively-indecomposable-ordinal)
    - [Additively closed ordinal](#additively-closed-ordinal)
    - [Division by an additively indecomposable ordinal](#division-by-an-additively-indecomposable-ordinal)
    - [Multiplicatively closed ordinal](#multiplicatively-closed-ordinal)
      - [Multiplicative closure criterion for a power of omega](#multiplicative-closure-criterion-for-a-power-of-omega)
  - [Ordinal arithmetic](#ordinal-arithmetic)
    - [Fundamental sequence of a limit ordinal](#fundamental-sequence-of-a-limit-ordinal)
    - [Fast-growing hierarchy](#fast-growing-hierarchy)
      - [Eventual dominance in a fast-growing hierarchy](#eventual-dominance-in-a-fast-growing-hierarchy)
    - [Hessenberg natural sum](#hessenberg-natural-sum)
      - [Shuffle bound for ordinal partitions](#shuffle-bound-for-ordinal-partitions)
        - [Ordinal partition bound](#ordinal-partition-bound)
- [Inner model](#inner-model)
  - [Constructible-universe obstruction to a uniform inner-model proof of failure of choice](#constructible-universe-obstruction-to-a-uniform-inner-model-proof-of-failure-of-choice)
- [Descriptive set theory](descriptive-set-theory.md)
  - [Baire space of sequences](descriptive-set-theory.md#baire-space-of-sequences)
  - [Infinite game of perfect information](descriptive-set-theory.md#infinite-game-of-perfect-information)
    - [Covering of an infinite game](descriptive-set-theory.md#covering-of-an-infinite-game)
      - [Depth-stabilizing inverse limit of game coverings](descriptive-set-theory.md#depth-stabilizing-inverse-limit-of-game-coverings)
      - [Unravelling of a game payoff](descriptive-set-theory.md#unravelling-of-a-game-payoff)
        - [Announcement-and-challenge covering of a closed payoff](descriptive-set-theory.md#announcement-and-challenge-covering-of-a-closed-payoff)
    - [Buchi game](descriptive-set-theory.md#buchi-game)
    - [Strategy in an infinite game](descriptive-set-theory.md#strategy-in-an-infinite-game)
      - [Winning strategy in an infinite game](descriptive-set-theory.md#winning-strategy-in-an-infinite-game)
    - [Determined infinite game](descriptive-set-theory.md#determined-infinite-game)
      - [Borel determinacy theorem](descriptive-set-theory.md#borel-determinacy-theorem)
      - [Choice diagonalization of an undetermined game](descriptive-set-theory.md#choice-diagonalization-of-an-undetermined-game)
      - [Open determinacy](descriptive-set-theory.md#open-determinacy)
        - [Clopen determinacy with terminal losses](descriptive-set-theory.md#clopen-determinacy-with-terminal-losses)
        - [Winning-position attractor in an infinite game](descriptive-set-theory.md#winning-position-attractor-in-an-infinite-game)
      - [Axiom of determinacy](descriptive-set-theory.md#axiom-of-determinacy)
        - [Projective determinacy](descriptive-set-theory.md#projective-determinacy)
    - [Quasistrategy](descriptive-set-theory.md#quasistrategy)
      - [Quasidetermined infinite game](descriptive-set-theory.md#quasidetermined-infinite-game)
        - [Choice characterization of quasideterminacy](descriptive-set-theory.md#choice-characterization-of-quasideterminacy)
  - [Uniformization of a binary relation](descriptive-set-theory.md#uniformization-of-a-binary-relation)
    - [Uniformization from determinacy](descriptive-set-theory.md#uniformization-from-determinacy)
  - [Pointclass](descriptive-set-theory.md#pointclass)
    - [Analytic set](descriptive-set-theory.md#analytic-set)
      - [Coanalytic set](descriptive-set-theory.md#coanalytic-set)
    - [Projective hierarchy](descriptive-set-theory.md#projective-hierarchy)
      - [Projective set](descriptive-set-theory.md#projective-set)
  - [Perfect set property](descriptive-set-theory.md#perfect-set-property)
  - [Suslin representation](descriptive-set-theory.md#suslin-representation)
    - [X-Suslin set](descriptive-set-theory.md#x-suslin-set)
      - [Kappa-Suslin set](descriptive-set-theory.md#kappa-suslin-set)
        - [Every set of reals is continuum-Suslin](descriptive-set-theory.md#every-set-of-reals-is-continuum-suslin)
        - [Successor-Suslin decomposition](descriptive-set-theory.md#successor-suslin-decomposition)
        - [Aleph-one-Suslin decomposition into analytic sets](descriptive-set-theory.md#aleph-one-suslin-decomposition-into-analytic-sets)
  - [Set of well-order codes](descriptive-set-theory.md#set-of-well-order-codes)
    - [Boundedness theorem for well-order codes](descriptive-set-theory.md#boundedness-theorem-for-well-order-codes)
    - [Solovay rank-comparison game](descriptive-set-theory.md#solovay-rank-comparison-game)
    - [Causal rank-raising map on well-order codes](descriptive-set-theory.md#causal-rank-raising-map-on-well-order-codes)
  - [Projectively well-ordered inner model](descriptive-set-theory.md#projectively-well-ordered-inner-model)
    - [First uncountable ordinal of an inner model](descriptive-set-theory.md#first-uncountable-ordinal-of-an-inner-model)
    - [Projective determinacy collapses the inner-model omega-one](descriptive-set-theory.md#projective-determinacy-collapses-the-inner-model-omega-one)
  - [Friedman–Moschovakis coding lemma](descriptive-set-theory.md#friedman-moschovakis-coding-lemma)
    - [Friedman–Moschovakis coding game](descriptive-set-theory.md#friedman-moschovakis-coding-game)
- [Filter (set theory)](#filter-set-theory)
  - [Pushforward filter](#pushforward-filter)
  - [Convergence of a filter](#convergence-of-a-filter)
  - [Addition of filters on the natural numbers](#addition-of-filters-on-the-natural-numbers)
  - [Filter quantifier](#filter-quantifier)
    - [Boolean failure of the cofinite-filter quantifier](#boolean-failure-of-the-cofinite-filter-quantifier)
    - [Conjunction law for filter quantifiers](#conjunction-law-for-filter-quantifiers)
  - [Free filter](#free-filter)
    - [Membership in a free filter is detected by its ultrafilter extensions](#membership-in-a-free-filter-is-detected-by-its-ultrafilter-extensions)
  - [Kappa-complete filter](#kappa-complete-filter)
    - [Cobounded filter on a regular cardinal](#cobounded-filter-on-a-regular-cardinal)
  - [Cofinite filter](#cofinite-filter)
    - [Cofinite set](#cofinite-set)
  - [Ultrafilter lemma](#ultrafilter-lemma)
    - [Ultrafilter selection from a partition-rich family](#ultrafilter-selection-from-a-partition-rich-family)
  - [Ultrafilter](#ultrafilter)
    - [Fine ultrafilter](#fine-ultrafilter)
      - [Normal ultrafilter on small subsets](#normal-ultrafilter-on-small-subsets)
    - [Normal ultrafilter on a cardinal](#normal-ultrafilter-on-a-cardinal)
    - [Ultrafilter with arithmetic-progression-rich members](#ultrafilter-with-arithmetic-progression-rich-members)
    - [Ultrafilter with finite-sums members](#ultrafilter-with-finite-sums-members)
    - [Number of ultrafilters on an infinite set](#number-of-ultrafilters-on-an-infinite-set)
    - [Pushforward ultrafilter](#pushforward-ultrafilter)
    - [Fubini product of ultrafilters](#fubini-product-of-ultrafilters)
    - [Ultrafilter functor](#ultrafilter-functor)
      - [Terminal finite-coproduct-preserving set endofunctor](#terminal-finite-coproduct-preserving-set-endofunctor)
    - [Principal ultrafilter](#principal-ultrafilter)
    - [Nonprincipal ultrafilter](#nonprincipal-ultrafilter)
      - [Small set is absent from a complete nonprincipal ultrafilter](#small-set-is-absent-from-a-complete-nonprincipal-ultrafilter)
    - [Countably complete ultrafilter](#countably-complete-ultrafilter)
    - [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers)
      - [No nontrivial convergent sequences in the Stone-Čech compactification](#no-nontrivial-convergent-sequences-in-the-stone-cech-compactification)
      - [Compact Hausdorff topology on ultrafilters](#compact-hausdorff-topology-on-ultrafilters)
      - [Addition on the Stone-Čech compactification of the natural numbers](#addition-on-the-stone-cech-compactification-of-the-natural-numbers)
        - [Idempotent ultrafilter](#idempotent-ultrafilter)
          - [Tail finite-sums semigroup](#tail-finite-sums-semigroup)
          - [Zero-residue constraint for idempotent ultrafilters](#zero-residue-constraint-for-idempotent-ultrafilters)
          - [Idempotent-ultrafilter star-set lemma](#idempotent-ultrafilter-star-set-lemma)
        - [Idempotent ultrafilter on the natural numbers](#idempotent-ultrafilter-on-the-natural-numbers)
    - [Ultralimit](#ultralimit)
      - [Ultrafilter characterization of compact Hausdorff spaces](#ultrafilter-characterization-of-compact-hausdorff-spaces)

<h2 id="russell-s-paradox">Russell's paradox</h2>

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Russell's_paradox)

Unrestricted formation of a [set](set.md) $R=\{x:x\notin x\}$ contradicts its own membership condition: substituting $R$ for $x$ gives the displayed equivalence. Thus a predicate cannot always define a [set](set.md) of all objects satisfying it. Restricted [set comprehension](#restricted-set-comprehension) forms a [subset](set.md#subset) of a previously given [set](set.md), avoiding this argument. The contradiction does not assert that a [set](set.md) whose elements happen not to contain themselves is impossible; it rules out the universal collection with exactly the specified membership condition.

## Urelement

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Urelement)

An urelement is an object permitted alongside [sets](set.md), with no members, distinguished from the [empty set](set.md#empty-set) by an atom or [set](set.md) predicate. [Extensionality](#axiom-of-extensionality) is restricted to [sets](set.md), so distinct atoms need not be equal merely because they have no members. An atom is different from a [Quine atom](#quine-atom), which is a [set](set.md) with a self-member. In [simple typed set theory with atoms](#simple-typed-set-theory-with-atoms), each sort may contain urelements in addition to the objects representing [subsets](set.md#subset) of the preceding sort.

### Basic Fraenkel permutation model

↑ **Parent:** [Urelement](#urelement)

Start with a well-founded universe of [sets](set.md) over an infinite set $A$ of [urelements](#urelement). The full [symmetric group](finite-group-theory.md#symmetric-group) of $A$ acts recursively on sets. Retain the objects all of whose descendants have a [finite support in a permutation action](group-theory.md#finite-support-in-a-permutation-action). This class satisfies set-extensionality, [foundation](#axiom-of-regularity), [infinity](mathematics.md#infinity), [pairing](#axiom-of-pairing), [union](set.md#set-union), [separation](#axiom-schema-of-specification), [replacement](#axiom-schema-of-replacement) and its internal [power set](set.md#power-set) axiom. A definable functional image has the finite union of the supports of its domain and parameters as a support; uniqueness makes the image invariant. The family of two-element subsets of $A$ has no [choice function](#choice-function): a transposition of two atoms outside the function's finite support fixes their pair and moves either possible choice. For untyped membership with extensionality merely restricted to nonempty objects, atoms are also vacuous subsets; add all atoms to each internal power-set object.

## Hereditarily locally small membership model

↑ **Parent:** [Set theory](set-theory.md)

For a strong-limit cardinal $\lambda$ of [countable](#countable-set) [cofinality](#cofinality), define

$$
B_\lambda=\{x:\forall y\in\operatorname{TC}(\{x\})\ (|y|<\lambda)\}.
$$

Here smallness bounds every individual membership extension; it does not bound the [cardinality](#cardinality) of the entire [transitive closure](#transitive-closure). The [transitive class](#transitive-class) $B_\lambda$ satisfies all [ZF](#zermelo-fraenkel-set-theory) axioms except possibly the [Axiom of union](#axiom-of-union): functional images have fewer than $\lambda$ elements, and the [power set](set.md#power-set) of a [set](set.md) of size $\mu<\lambda$ has size $2^\mu<\lambda$. These facts give [Axiom schema of replacement](#axiom-schema-of-replacement) and [Axiom of power set](#axiom-of-power-set); pairs and definable [subsets](set.md#subset) also remain locally small. For $\lambda=\beth_\omega$, the [countable](#countable-set) [set](set.md) $\{V_{\omega+n}:n<\omega\}$ belongs to $B_\lambda$, but its [union](set.md#set-union) $V_{\omega+\omega}$ has size $\lambda$ and does not. This gives an explicit relative-independence model for the [Axiom of union](#axiom-of-union).

## New Foundations

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/New_Foundations)

New Foundations uses ordinary extensionality and comprehension restricted to [stratified formulas](#stratified-formula). Its atom-permitting weakening is [New Foundations with urelements](#new-foundations-with-urelements).

### New Foundations with urelements

↑ **Parent:** [New Foundations](#new-foundations)

NFU has a universal domain, a predicate $S$ distinguishing sets from atoms, extensionality restricted to sets, and comprehension for [stratified formulas](#stratified-formula). Atoms have no members. Every stratified predicate has a set extension, including the always-false predicate, so there is a distinguished empty set even when atoms exist. Permitting atoms removes the full-extensionality obstacle in [New Foundations](#new-foundations).

#### Type-shifting automorphism

↑ **Parent:** [New Foundations with urelements](#new-foundations-with-urelements)

For an integer-indexed typed model, a type-shifting automorphism is a bijection from each type to the next preserving equality, adjacent-type membership and the set predicates. On type zero define $x\mathrel E y$ by $x\in j(y)$. Stratified formulas are translated by sending a variable of type $i$ to $j^i(x)$. Typed comprehension then gives the untyped comprehension of [NFU](#new-foundations-with-urelements). Such an automorphism is external; formulas containing it are not included in the typed comprehension scheme.

##### Rank-shifting automorphism construction of NFU

↑ **Parent:** [Type-shifting automorphism](#type-shifting-automorphism)

In a model of [ZFC](#zermelo-fraenkel-set-theory-with-choice), choose an external automorphism $j$ and an ordinal $\alpha$ with $j(\alpha)>\alpha$. Set $D_i=V_{j^i(\alpha)}$ for integer $i$, and declare the sets of type $i+1$ to be its objects that are subsets of $D_i$. Ordinary membership between successive types satisfies typed comprehension and set-extensionality. The automorphism shifts all types, yielding [NFU](#new-foundations-with-urelements) by the type-zero collapse. A [Skolem hull](mathematical-logic.md#skolem-hull) of integer-indexed increasing ordinal indiscernibles supplies such a $j$ by shifting the indices. The model is externally ill-founded; a transitive well-founded universe cannot have such an automorphism.

###### Rank-shifting NFU model with explicit set predicate

↑ **Parent:** [Rank-shifting automorphism construction of NFU](#rank-shifting-automorphism-construction-of-nfu)

Let $M$ be a membership structure satisfying [extensionality](#axiom-of-extensionality) and every pure-membership separation instance, with an external automorphism $j$ and domains $D_i=j^i(D_0)$ represented by objects of $M$. Suppose every $M$-subset of $D_i$ is an element of $D_{i+1}$. Interpret [NFU](#new-foundations-with-urelements) on the objects of $D_0$ using the displayed [set](set.md) predicate and membership, with all [subset](set.md#subset) statements evaluated in $M$. Atoms have no members, and [extensionality](#axiom-of-extensionality) applied to $j(y),j(z)\subseteq D_0$ gives [extensionality](#axiom-of-extensionality) for [sets](set.md). A [stratified formula](#stratified-formula) becomes an ordinary pure-membership formula by sending each variable of type $i$ to $j^i(x)$ and restricting its quantifier to $D_i$. A [set](set.md) predicate on sort $i$ means containment in $D_{i-1}$; adjacent-sort membership is guarded by containment in the lower domain. Separation yields the extension $X\subseteq D_i$, the closure hypothesis places it in $D_{i+1}$, and $j^{-(i+1)}(X)\in D_0$ is the required untyped [set](set.md). This proves every comprehension instance. The guard is essential: an object not contained in a lower domain can still have some ordinary members there, which must not become members of a typed atom. Internal ranks $V_{j^i(\alpha)}$ with $j(\alpha)>\alpha$ give one instance of these hypotheses; shifted rank objects in an elementary model of an expanded $V_{\omega+\omega}$ give a consistency proof without assuming Con([ZFC](#zermelo-fraenkel-set-theory-with-choice)).

###### Rank-indiscernible construction of an NFU model

↑ **Parent:** [Rank-shifting NFU model with explicit set predicate](#rank-shifting-nfu-model-with-explicit-set-predicate)

[NFU](#new-foundations-with-urelements) has a unary predicate $S$ for [sets](set.md), atoms have no members, [extensionality](#axiom-of-extensionality) applies to [sets](set.md), and comprehension applies to every [stratified formula](#stratified-formula). A stratification assigns integer types to variables so that equality uses equal types and $x\in y$ requires $\operatorname{type}(y)=\operatorname{type}(x)+1$. A unary [set](set.md) predicate adds no type difference.

Start with the actual [set](set.md) structure $B=(V_{\omega+\omega},\in)$. This structure satisfies [extensionality](#axiom-of-extensionality) and every pure-membership [separation](#axiom-schema-of-specification) instance: the [subset](set.md#subset) defined in a [set](set.md) $a$ of rank below $\omega+\omega$ still has rank below $\omega+\omega$. We do not assert that $B$ satisfies [replacement](#axiom-schema-of-replacement) or all of [ZFC](#zermelo-fraenkel-set-theory-with-choice). Expand it by [Skolem functions](mathematical-logic.md#skolem-function). In it use the [sequence](real-analysis.md#sequence) of rank objects $V_{\omega+n+6}$, $n<\omega$. For two such objects $d<e$ in [sequence](real-analysis.md#sequence) order, we have

$$
d\subsetneq e,\qquad \forall x\,(x\subseteq d\Longrightarrow x\in e),
$$

with quantifiers in $B$. The second statement holds because every [subset](set.md#subset) of $V_\alpha$ belongs to $V_{\alpha+1}$, and the later rank is at least $\alpha+1$.

Introduce constants $d_i$, $i\in\mathbb Z$, and require them to be order indiscernibles in the Skolem language, satisfying these two assertions whenever $i<j$. Also require $V_{\omega+5}\subseteq d_i$ for every $i$; this fixed rank object is first-order definable in $B$. Every finite part of these requirements together with $\operatorname{Th}(B^*)$ is satisfiable: color finite increasing tuples of the original rank [sequence](real-analysis.md#sequence) by the truth values of the finitely many formulas mentioned, and use [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem) to get a homogeneous [subsequence](real-analysis.md#subsequence). The rank assertions hold for every increasing tuple there. The [compactness theorem](mathematical-logic.md#compactness-theorem) gives a model of the full theory. In its [Skolem hull](mathematical-logic.md#skolem-hull) $N$ generated by the $d_i$, the integer shift extends to an [automorphism](algebra.md#automorphism) $j$ with $j(d_i)=d_{i+1}$, by the term-transport proof of the [Ehrenfeucht-Mostowski theorem](foundations-of-mathematics.md#ehrenfeucht-mostowski-theorem). Thus $N$ still satisfies [extensionality](#axiom-of-extensionality) and all pure-membership [separation](#axiom-schema-of-specification) instances, and

$$
N\models\forall x\,(x\subseteq d_i\Longrightarrow x\in d_{i+1})
\quad(i\in\mathbb Z).
$$

This is a set-sized [first-order model](mathematical-logic.md#model-of-a-first-order-theory); no satisfaction predicate for a proper-class universe is being assumed.

Externally let $D_i=\{x\in N:N\models x\in d_i\}$. The [automorphism](algebra.md#automorphism) bijects $D_i$ onto $D_{i+1}$. Interpret a typed structure with sort $i$ equal to $D_i$. At sort $i+1$, declare $y$ a [set](set.md) exactly when $N\models y\subseteq d_i$; otherwise it is an atom. Define adjacent-sort membership by

$$
x\in_i y\quad\Longleftrightarrow\quad N\models(y\subseteq d_i\ \land\ x\in y).
$$

The guard is necessary: a typed atom might have some ordinary $N$-members in $D_i$, and those must not become its typed members. Set-extensionality follows from [extensionality](#axiom-of-extensionality) in $N$, because the ordinary members of a typed [set](set.md) all lie in $D_i$. For any typed formula on sort $i$, its quantifiers can be restricted to the corresponding $d_l$, its [set](set.md) predicates replaced by [subset](set.md#subset) assertions, and its memberships replaced by the guarded relation. This is an ordinary pure-membership formula of $N$ with finitely many parameters. [Separation](#axiom-schema-of-specification) gives its extension $X\subseteq d_i$, and the displayed closure assertion gives $X\in d_{i+1}$. It is therefore a typed [set](set.md) witnessing comprehension. The [automorphism](algebra.md#automorphism) shifts these sorted domains and preserves the [set](set.md) flags and guarded memberships.

Collapse the types onto $D_0$. Define

$$
S(y)\quad\Longleftrightarrow\quad N\models j(y)\subseteq d_0,
\qquad x\mathrel E y\quad\Longleftrightarrow\quad S(y)\ \land\ N\models x\in j(y).
$$

Objects not satisfying $S$ have no $E$-members. If two [sets](set.md) have the same $E$-members, their images under $j$ are [subsets](set.md#subset) of $d_0$ with the same ordinary members, so are equal by [extensionality](#axiom-of-extensionality) of $N$; injectivity of $j$ gives equality of the original objects.

To verify every stratified comprehension instance, assign a variable $v$ its stratification type $t(v)$ and translate its value $a\in D_0$ to $j^{t(v)}(a)\in D_{t(v)}$. Equality is preserved. An atomic $E(x,y)$ translates to the guarded adjacent-sort membership because $t(y)=t(x)+1$; the unary predicate $S(y)$ translates to $j^{t(y)}(y)\subseteq d_{t(y)-1}$. [Induction](foundations-of-mathematics.md#mathematical-induction) on formulas, using the domain bijections for quantifiers, preserves truth. If the free variable $x$ has type $t$, typed comprehension produces its extension $X\subseteq d_t$, with $X\in d_{t+1}$. Put $b=j^{-(t+1)}(X)\in D_0$. Then $S(b)$ holds, and for every $a\in D_0$,

$$
a\mathrel E b\quad\Longleftrightarrow\quad N\models j^t(a)\in X
\quad\Longleftrightarrow\quad \varphi(a,\vec p).
$$

This is exactly the required [NFU](#new-foundations-with-urelements) [set](set.md). No formula containing the external [automorphism](algebra.md#automorphism) $j$ has been used in a [separation](#axiom-schema-of-specification) or comprehension scheme; $j$ only transports values after the pure formula is formed.

The construction also permits the usual [infinity](mathematics.md#infinity) requirement. The ordinary $\omega$ and its successor graph $f$ are definable in $N$, hence fixed by $j$, and lie below $V_{\omega+5}$, so belong to all the required domains. Under $E$, the members of $\omega$ are still its ordinary $N$-members. The new Kuratowski pair satisfies

$$
\langle x,y\rangle_E=j^{-2}(\langle x,y\rangle_N).
$$

Since $j(f)=f$, membership of this pair in $f$ under $E$ is equivalent to $\langle x,y\rangle_N\in f$. Thus $f$ is an internal injection of $\omega$ into itself omitting zero, giving a Dedekind-infinite [set](set.md).

We have built a model of [NFU](#new-foundations-with-urelements), with [infinity](mathematics.md#infinity) if it is included in the formulation, in ordinary [ZFC](#zermelo-fraenkel-set-theory-with-choice) metatheory:

$$
\boxed{\text{ZFC proves the existence of a model of NFU.}}
$$

In particular $\operatorname{Con}(\mathrm{ZFC})\Rightarrow\operatorname{Con}(\mathrm{NFU})$. This proof does not assume $\operatorname{Con}(\mathrm{ZFC})$ as an additional internal axiom: its starting structure is the [set](set.md) $V_{\omega+\omega}$, not a model of [ZFC](#zermelo-fraenkel-set-theory-with-choice).

#### Stratified formula

↑ **Parent:** [New Foundations with urelements](#new-foundations-with-urelements)

A formula is stratified if its variables can be assigned integer types so that equality relates variables of the same type and membership $x\in y$ requires $\operatorname{type}(y)=\operatorname{type}(x)+1$. Unary set predicates impose no additional difference. Stratification is a syntactic condition; it does not assert that the untyped universe actually has disjoint types. Translating a stratified formula into a typed model permits [type-shifting automorphism](#type-shifting-automorphism) to recover untyped comprehension.

## Simple typed set theory with atoms

↑ **Parent:** [Set theory](set-theory.md)

Objects have sorts $0,1,\ldots$, with membership allowed only from sort $i$ to sort $i+1$. A set predicate distinguishes sets from atoms; atoms have no members, extensionality applies to sets, and every well-typed formula defines a set in the next sort by comprehension. First-order models may have only a specified collection of subsets, as in [Henkin semantics](mathematical-logic.md#henkin-semantics). For a full finite-type model, take $D_i=V_{r_i}$ at widely separated increasing ranks, represent sets at level $i+1$ by $\mathcal P(D_i)\subseteq D_{i+1}$, and treat the remaining objects as atoms under typed membership.

### Typical ambiguity

↑ **Parent:** [Simple typed set theory with atoms](#simple-typed-set-theory-with-atoms)

Typical ambiguity is the schema asserting that every closed well-typed sentence is equivalent to its uniform type-raise. It is not an assertion that adjacent types have the same cardinality. To obtain finite satisfiability, color finite increasing rank selections by the truth values of the finitely many sentences concerned. The [Ramsey's theorem](ramsey-theory.md#ramsey-s-theorem) gives a homogeneous rank set; two overlapping windows then have equal truth vectors, yielding the desired type-raise equivalences. The [compactness theorem](mathematical-logic.md#compactness-theorem) gives a first-order model of the entire schema.

## Axiom of pairing

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_pairing)

For any two [sets](set.md) there is a set containing exactly those two members. Together with other [ZFC](#zermelo-fraenkel-set-theory-with-choice) axioms it permits ordinary ordered-pair coding. [Countable-subset closure](#countable-subset-closure) implies this axiom for the structure of [hereditarily countable sets](#hereditarily-countable-set).

## Axiom of extensionality

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_extensionality)

Two [sets](set.md) with exactly the same members are equal. In a [transitive model](#transitive-model), all actual members of its sets are available internally, so ambient extensionality gives the internal axiom as well.

### Non-extensional membership model with one atom

↑ **Parent:** [Axiom of extensionality](#axiom-of-extensionality)

Build well-founded coded sets over a single [urelement](#urelement) $a$ with no members, retaining a distinct empty set. Use the unmodified membership language, so both $a$ and the empty set have the same empty extension and [extensionality](#axiom-of-extensionality) fails. Pairs, unions, separation and functional ranges have set codes, and pure natural numbers give [infinity](mathematics.md#infinity). For the unrestricted [Axiom of power set](#axiom-of-power-set), the power-set code must contain $a$ as well as all ordinary subset codes, since the atom is vacuously a subset of every object. Rank gives [foundation](#axiom-of-regularity). Thus the other [ZF](#zermelo-fraenkel-set-theory) axioms hold.

## Independent family of sets

↑ **Parent:** [Set theory](set-theory.md)

A family of [subsets](set.md#subset) of $X$ is independent when every finite choice of distinct members and their complements has nonempty [intersection](set.md#set-intersection). Write $A^1=A$ and $A^0=X\setminus A$ in the displayed condition. Every assignment of zero or one to the family then gives a collection with the [finite intersection property](topology.md#finite-intersection-property), which can be extended to an [ultrafilter](#ultrafilter).

### Fichtenholz-Kantorovich independent family

↑ **Parent:** [Independent family of sets](#independent-family-of-sets)

For every infinite [set](set.md) $X$ there is an [independent family of sets](#independent-family-of-sets) consisting of $2^{|X|}$ subsets of $X$. One construction uses a set $D$ of pairs $(s,H)$, where $s\subseteq X$ is finite and $H\subseteq\mathcal P(s)$. For each $A\subseteq X$, let $I_A=\{(s,H):A\cap s\in H\}$. Given distinct $A_1,\ldots,A_m$, choose a finite $s$ distinguishing all their traces and choose $H$ to contain precisely the traces prescribed to have value one. This realizes every finite Boolean choice. With the [axiom of choice](#axiom-of-choice), $|D|=|X|$, so a [bijection](function.md#bijection) transports this family to $X$. Its independent assignments give $2^{2^{|X|}}$ distinct [ultrafilters](#ultrafilter).

## Almost disjoint family on a regular cardinal

↑ **Parent:** [Set theory](set-theory.md)

A family of size-$\kappa$ [subsets](set.md#subset) of a set is almost disjoint at $\kappa$ when distinct members have intersection of size less than $\kappa$. Graphs of a [long chain under eventual domination](#long-chain-under-eventual-domination) give such a family of size $\kappa^+$ on $\kappa\times\kappa$. Transport by a [bijection](function.md#bijection) gives a family on $\kappa$ itself.

### Essential disjointness of small subfamilies

↑ **Parent:** [Almost disjoint family on a regular cardinal](#almost-disjoint-family-on-a-regular-cardinal)

Any at-most-$\kappa$ subfamily of an [almost disjoint family on a regular cardinal](#almost-disjoint-family-on-a-regular-cardinal) becomes pairwise disjoint after deleting fewer than $\kappa$ points from each member. Enumerate it in length at most $\kappa$ and apply the displayed trimming. Each removed part is a union of fewer than $\kappa$ small intersections, so [regular cardinal](#regular-cardinal) arithmetic bounds it below $\kappa$.

## Kappa-filtration

↑ **Parent:** [Set theory](set-theory.md)

For a [set](set.md) $A$ of size an uncountable [regular cardinal](#regular-cardinal) $\kappa$, an increasing sequence $(A_\alpha)_{\alpha<\kappa}$ with union $A$, each $|A_\alpha|<\kappa$, and $A_\delta=\bigcup_{\alpha<\delta}A_\alpha$ at every nonzero limit stage.

### Club agreement of countable filtrations

↑ **Parent:** [Kappa-filtration](#kappa-filtration)

For two [kappa-filtrations](#kappa-filtration) at $\kappa=\omega_1$ exhausting sets of size $\aleph_1$, any bijection between the sets carries corresponding stages onto one another on a [club set](#club-set) of indices. Bound both forward and inverse images at each countable stage by a function $g:\omega_1\to\omega_1$. The limit ordinals closed under all earlier $g$-values form a club; continuity gives equality at those ordinals.

## Almost disjoint family on omega

↑ **Parent:** [Set theory](set-theory.md)

A family of infinite [subsets](set.md#subset) of $\omega$ such that any two distinct members have finite intersection.

### Maximal almost disjoint family on omega

↑ **Parent:** [Almost disjoint family on omega](#almost-disjoint-family-on-omega)

An [almost disjoint family on omega](#almost-disjoint-family-on-omega) that cannot be enlarged by another infinite [subset](set.md#subset) while retaining almost disjointness. For the [cardinal](#cardinal-number) invariant $\mathfrak a$, one requires the family itself to be infinite; finite partitions otherwise give trivial maximal families.

#### Almost disjointness number

↑ **Parent:** [Maximal almost disjoint family on omega](#maximal-almost-disjoint-family-on-omega)

The least size of an infinite [maximal almost disjoint family on omega](#maximal-almost-disjoint-family-on-omega). [Zorn lemma](#zorn-s-lemma) extends an infinite disjoint family to a maximal one; thus $\mathfrak a\le2^{\aleph_0}$. The [bounding-to-almost-disjointness inequality](#bounding-to-almost-disjointness-inequality) supplies $\mathfrak b\le\mathfrak a$.

##### Bounding-to-almost-disjointness inequality

↑ **Parent:** [Almost disjointness number](#almost-disjointness-number)

For an infinite [almost disjoint family on omega](#almost-disjoint-family-on-omega) of size less than the [bounding number](#bounding-number), select countably many members and remove their intersections with earlier selected members to obtain infinite disjoint [sets](set.md) $C_n$. Bound, eventually and simultaneously, the finite intersections of each member with $C_n$. Choose one point of each $C_n$ above its bound. The resulting infinite [set](set.md) is almost disjoint from every original member, proving the family is not maximal. A selected member has one exceptional infinite intersection, which is ignored in its bounding [function](function.md).

## Standard membership model of set theory

↑ **Parent:** [Set theory](set-theory.md)

A model whose relation symbol for membership is interpreted by actual membership restricted to its domain. If the domain is also transitive, it is a [transitive model](#transitive-model). Some conventions include this transitivity requirement in the word standard.

## Partition relation

↑ **Parent:** [Set theory](set-theory.md)

The notation $\lambda\rightarrow(\mu)^\alpha_\beta$ says that every $\beta$-coloring of the $\alpha$-element subsets of $\lambda$ has a homogeneous subset of order type $\mu$. At infinite arity one specifies whether the domain subsets have a fixed cardinality or a fixed order type; the usual finite-arity notation has no such ambiguity.

### Finite-symmetric-difference colouring of infinite subsets

↑ **Parent:** [Partition relation](#partition-relation)

Choose a representative $R$ of each class of countably infinite [sets](set.md) modulo [finite symmetric difference](set.md#finite-symmetric-difference), and colour $A$ by the parity of $|A\mathbin\triangle R|$. Removing one element stays in the same class and flips the parity. Every infinite candidate homogeneous set therefore has two countably infinite subsets of opposite colours. With [choice](#axiom-of-choice), this refutes unrestricted countably infinite-arity positive [partition relations](#partition-relation) on every infinite cardinal.

<h3 id="erdos-rado-theorem-for-finite-arities">Erdős-Rado theorem for finite arities</h3>

↑ **Parent:** [Partition relation](#partition-relation)

For an infinite cardinal $\lambda$ and finite $r\ge0$, put $\beth_0(\lambda)=\lambda$ and $\beth_{r+1}(\lambda)=2^{\beth_r(\lambda)}$. Every $\lambda$-coloring of $(r+1)$-element subsets of $\beth_r(\lambda)^+$ has a homogeneous subset of size $\lambda^+$. The case $r=1$ is the [Erdős-Rado theorem for pairs](#erdos-rado-theorem-for-pairs). For the induction, the [end-homogeneous routing tree](#end-homogeneous-routing-tree) yields a sequence of length $\beth_{r-1}(\lambda)^+$ on which the color of an $(r+1)$-tuple depends only on its first $r$ entries. The previous-arity theorem homogenizes those $r$ entries. The case $r=0$ is the infinite pigeonhole principle at a successor cardinal.

#### Closed elementary-submodel construction of an end-homogeneous sequence

↑ **Parent:** [Erdős-Rado theorem for finite arities](#erdos-rado-theorem-for-finite-arities)

Put $\theta=(2^\mu)^+$ for an infinite [cardinal](#cardinal-number) $\mu$. Choose $M\prec H_\chi$ of size $2^\mu$, containing all [ordinals](#ordinal) below $\mu^+$, and closed under externally given [sequences](real-analysis.md#sequence) of length at most $\mu$. Such a model is built by $\mu^+$ successive [Skolem hull](mathematical-logic.md#skolem-hull) closures, since $(2^\mu)^\mu=2^\mu$. For a coloring of $[\theta]^{r+1}$ with at most $\mu$ colors in $M$, put $\beta=\sup(M\cap\theta)<\theta$. Recursively choose $x_\alpha\in M\cap\theta$ for $\alpha<\mu^+$, above all earlier points, so that every earlier $r$-tuple has the same color with $x_\alpha$ as with $\beta$. There are at most $\mu$ constraints, their code belongs to $M$ by closure, and $\beta$ witnesses their consistency. The [elementary embedding](#elementary-embedding) supplies the required witness in $M$. The resulting [sequence](real-analysis.md#sequence) is end-homogeneous, providing the induction step in the [Erdős-Rado theorem for finite arities](#erdos-rado-theorem-for-finite-arities).

#### End-homogeneous routing tree

↑ **Parent:** [Erdős-Rado theorem for finite arities](#erdos-rado-theorem-for-finite-arities)

For a coloring of $(r+1)$-subsets of an ordinal, route a vertex through the least earlier vertices matching its colors on every $r$-subset of previously chosen ancestors. The path stops when the vertex itself is selected. Common path prefixes agree, yielding a [set-theoretic tree](set.md#set-theoretic-tree); a node at level $\alpha$ is determined by its color table on $[\alpha]^r$. Along a branch, the color of an $(r+1)$-tuple is independent of its last entry. If the domain has size $(2^\mu)^+$ and $\lambda\le\mu$, levels below $\mu^+$ have size at most $2^\mu$; counting all those levels forces a branch of length $\mu^+$. If the domain is a regular strong-limit cardinal $\kappa$, those levels instead have size below $\kappa$, and the [tree property](set.md#tree-property) supplies a cofinal branch when needed.

<h3 id="erdos-rado-theorem-for-pairs">Erdős-Rado theorem for pairs</h3>

↑ **Parent:** [Partition relation](#partition-relation)

For every infinite [cardinal](#cardinal-number) $\lambda$, every coloring of pairs from $(2^\lambda)^+$ by $\lambda$ colors has a [monochromatic](ramsey-theory.md#monochromatic-set) subset of size $\lambda^+$. Construct an end-homogeneous tree by routing a new vertex through the least preceding vertices that match its colors to all previously chosen ancestors. An ancestor's color to every later vertex on a branch is constant. A node at height $\alpha$ is determined by its color sequence of length $\alpha$, so levels below $\lambda^+$ have size at most $\lambda^{|\alpha|}\leq2^\lambda$. The whole tree has more than $2^\lambda$ vertices, forcing a branch of length $\lambda^+$. One of the $\lambda$ ancestor-colors occurs $\lambda^+$ times, giving the required set.

#### Ordinal partition-bound function

↑ **Parent:** [Erdős-Rado theorem for pairs](#erdos-rado-theorem-for-pairs)

The colors $\nu$ here range over nonzero cardinals. The [Erdős-Rado theorem for pairs](#erdos-rado-theorem-for-pairs) makes this function total, and target and color monotonicity make it nondecreasing, with $f(\alpha)\geq\alpha$. If an uncountable cardinal $\kappa$ is closed below itself under $f$, then it is strong limit. Indeed, coloring distinct binary strings of length $\lambda<\kappa$ by their first differing coordinate uses $\lambda$ colors and has no monochromatic triangle, so $f(\lambda+1)>2^\lambda$. If $\kappa$ also has the [tree property](set.md#tree-property), the end-homogeneous tree for any $\nu<\kappa$ has levels of size below $\kappa$ and a cofinal branch; regularity makes one color occur $\kappa$ times. Thus $f(\kappa)=\kappa$. This distinguishes function closure plus the tree property from the tree property alone.

### Finite-subset partition property

↑ **Parent:** [Partition relation](#partition-relation)

The relation $\lambda\rightarrow(\lambda)^{<\omega}_\beta$ requires a subset of size $\lambda$ homogeneous at each finite arity. The constant color may depend on the arity.

#### Small forcing preservation of finite-subset partition properties

↑ **Parent:** [Finite-subset partition property](#finite-subset-partition-property)

If inaccessible $\lambda$ has the finite-subset partition property for every color number below $\lambda$, forcing of size below $\lambda$ preserves its two-color version. Color ground-model finite sets by their full [forcing decision patterns](forcing.md#forcing-decision-pattern); strong-limit cardinal arithmetic bounds the number of patterns.

### Infinite-arity partition relation

↑ **Parent:** [Partition relation](#partition-relation)

A [partition relation](#partition-relation) whose colored subsets are infinite. For countably infinite arity, choosing representatives modulo finite [symmetric difference](set.md#symmetric-difference) and coloring its parity shows $\kappa\nrightarrow(\omega)^\omega_2$ for every infinite cardinal $\kappa$.

## Eventual domination

↑ **Parent:** [Set theory](set-theory.md)

For functions $f,g:\omega\to\omega$, write $f\leq^*g$ when $f(n)\leq g(n)$ for all sufficiently large $n$. A [dominating family](#dominating-family) is cofinal for this relation.

### Eventual domination on a regular cardinal

↑ **Parent:** [Eventual domination](#eventual-domination)

For $f,g:\kappa\to\kappa$, write $f<^*g$ when there is $\gamma<\kappa$ such that $f(\delta)<g(\delta)$ whenever $\gamma<\delta<\kappa$. For an infinite [regular cardinal](#regular-cardinal), suprema of fewer than $\kappa$ [ordinals](#ordinal) below $\kappa$ remain below it, permitting the [long chain under eventual domination](#long-chain-under-eventual-domination) construction.

#### Long chain under eventual domination

↑ **Parent:** [Eventual domination on a regular cardinal](#eventual-domination-on-a-regular-cardinal)

For every infinite [regular cardinal](#regular-cardinal) $\kappa$, there is a strictly eventually increasing sequence of $\kappa^+$ [functions](function.md) $\kappa\to\kappa$. At stage $0<\zeta<\kappa^+$ enumerate predecessors by $e:\kappa\to\zeta$ and put $f_\zeta(\delta)=\sup_{\eta<\delta}(f_{e(\eta)}(\delta)+1)$. Regularity bounds each value below $\kappa$, while any predecessor's index is eventually included in the supremum.

### Bounding number

↑ **Parent:** [Eventual domination](#eventual-domination)

The least size of a family in $\omega^\omega$ having no common bound for [eventual domination](#eventual-domination). Every countable family $(f_i)$ has the bound $g(n)=1+\max_{i\le n}f_i(n)$, so $\aleph_1\le\mathfrak b\le2^{\aleph_0}$.

### Dominating family

↑ **Parent:** [Eventual domination](#eventual-domination)

A family $C\subseteq\omega^\omega$ such that every $f\in\omega^\omega$ is eventually dominated by some $g\in C$.

<h2 id="sierpinski-decomposition-of-the-plane">Sierpiński decomposition of the plane</h2>

↑ **Parent:** [Set theory](set-theory.md)

A partition $\mathbb R^2=A\sqcup B$ in which every vertical section of $A$ and every horizontal section of $B$ is countable. Swapping the coordinate directions gives the equivalent convention.

## Definable continuous hierarchy

↑ **Parent:** [Set theory](set-theory.md)

A definable continuous hierarchy is a definable class function from the [ordinals](#ordinal) to [sets](set.md), with increasing levels $H_\alpha$ and the displayed continuity condition at nonzero [limit ordinals](#limit-ordinal). Its union is a definable [class in set theory](#class-set-theory). One often additionally requires [transitive sets](#transitive-set) as levels. Finite collections of [first-order formulas](mathematical-logic.md#first-order-formula) reflect along this hierarchy by the [reflection theorem for definable hierarchies](#reflection-theorem-for-definable-hierarchies).

<h2 id="zermelo-fraenkel-set-theory">Zermelo–Fraenkel set theory</h2>

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zermelo–Fraenkel_set_theory)

Zermelo–Fraenkel set theory is the usual first-order axiomatization of sets by extensionality, empty set, pairing, union, power set, infinity, separation, replacement and foundation.

### Zermelo set theory

↑ **Parent:** [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zermelo_set_theory)

The usual [set theory](set-theory.md) with [extensionality](#axiom-of-extensionality), [empty set](set.md#empty-set), [pairing](#axiom-of-pairing), [union](set.md#set-union), [power set](set.md#power-set), [infinity](mathematics.md#infinity) and full [separation](#axiom-schema-of-specification), before adjoining [replacement](#axiom-schema-of-replacement). Modern presentations often include [foundation](#axiom-of-regularity); the convention should be specified when comparing theories. Class-theoretic variants add classes and class comprehension, rather than treating proper classes as sets.

#### Axiom of limitation of size

↑ **Parent:** [Zermelo set theory](#zermelo-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_limitation_of_size)

Every proper class is in [bijection](function.md#bijection) with the universe. Over class-theoretic [Zermelo set theory](#zermelo-set-theory), with class-parameter [separation](#axiom-schema-of-specification), this is equivalent to [replacement](#axiom-schema-of-replacement) plus [global choice](#axiom-of-global-choice). For replacement, a proper functional image of a set would give a surjection from that set onto the universe, contradicted by diagonal separation. The proper class of ordinals supplies the global well-order. Conversely rank followed by uniformly chosen rank-segment well-orders is set-like, and every proper class in that order has order type equal to the entire ordinal class.

<h3 id="intuitionistic-zermelo-fraenkel-set-theory">Intuitionistic Zermelo–Fraenkel set theory</h3>

↑ **Parent:** [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)

Full intuitionistic Zermelo–Fraenkel set theory uses [intuitionistic first-order logic](mathematical-logic.md#intuitionistic-first-order-logic), extensionality, pairing, union, infinity, full separation, power set, collection and [epsilon induction](#epsilon-induction). Collection is stronger than replacement intuitionistically. This is distinct from predicative constructive ZF, which restricts separation and replaces full power set. The full theory supports a [Boolean-valued inner universe over intuitionistic set theory](#boolean-valued-inner-universe-over-intuitionistic-set-theory), giving the relative consistency of classical [ZF](#zermelo-fraenkel-set-theory).

#### Boolean-valued inner universe over intuitionistic set theory

↑ **Parent:** [Intuitionistic Zermelo–Fraenkel set theory](#intuitionistic-zermelo-fraenkel-set-theory)

Using the [double-negation Boolean algebra](mathematical-logic.md#double-negation-boolean-algebra), form well-founded names whose immediate subnames have truth-value weights. Define valued membership and equality by recursion on the underlying well-founded trees. Logical conjunction and universal quantification use meets; disjunction and existence use Boolean joins. Explicit names for pairs, unions and subsets verify the elementary set axioms, and [collection for Boolean-valued names](#collection-for-boolean-valued-names) handles unbounded witnesses. The resulting internal valued universe validates classical [ZF](#zermelo-fraenkel-set-theory). This is a negative inner interpretation, not an assertion that the external intuitionistic universe satisfies excluded middle.

##### Boolean-valued name

↑ **Parent:** [Boolean-valued inner universe over intuitionistic set theory](#boolean-valued-inner-universe-over-intuitionistic-set-theory)

A well-founded recursively built set code with a set of immediate subnames and a Boolean coefficient for each. The coefficient records the extent to which the corresponding subname belongs. More generally one may permit repeated coded subnames, joining their coefficients. Recursive valued equality identifies different codes representing the same valued set; external equality of codes is not the interpreted equality.

##### Collection for Boolean-valued names

↑ **Parent:** [Boolean-valued inner universe over intuitionistic set theory](#boolean-valued-inner-universe-over-intuitionistic-set-theory)

For a name $a$ and formula $\varphi$, form the set of pairs $(u,p)$ with $u$ in the immediate domain of $a$, $p$ a Boolean truth value, and some name $v$ satisfying $p\le a(u)\wedge\llbracket\varphi(u,v)\rrbracket$. Full separation makes this a set, and intuitionistic collection gives a set of witness names covering all its pairs. A name with these witnesses in its domain collects the entire Boolean value of every existential assertion over $a$, without selecting one witness whose value is top. No choice or maximum principle is used.

### Rieger-Bernays permutation model

↑ **Parent:** [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)

A definable class bijection $\pi$ of a model's universe changes membership as displayed. Images and inverse images of sets under $\pi$ remain sets by the [Axiom schema of replacement](#axiom-schema-of-replacement). The new extension of $y$ is the old set $\pi(y)$. Thus the representative of any desired extension $b$ is $\pi^{-1}(b)$. Extensionality follows from bijectivity; separation and replacement translate to old definable formulas; pairs, unions and power sets have explicit representatives. Infinity follows by iterating the new empty set and successor. Foundation need not survive: interchanging $\varnothing$ and $\{\varnothing\}$ makes the old empty set a [Quine atom](#quine-atom). A full such permutation of a model of choice still satisfies choice; failure of choice requires an additional symmetry restriction.

#### Quine atom

↑ **Parent:** [Rieger-Bernays permutation model](#rieger-bernays-permutation-model)

A Quine atom is a set whose sole member is itself. It violates the [Axiom of foundation](#axiom-of-regularity) while respecting the [axiom of extensionality](#axiom-of-extensionality). Swapping pairwise distinct old objects $a_n$ with their singletons in a [Rieger-Bernays permutation model](#rieger-bernays-permutation-model) supplies many Quine atoms, provided those transpositions have disjoint supports. For example, the old ordinals $a_n=\omega+n$ and their singletons are disjoint families.

##### Extensional cumulative universe over Quine atoms

↑ **Parent:** [Quine atom](#quine-atom)

Start with distinct formal atoms $q\in A$ with membership extensions $\{q\}$. Recursively adjoin a unique representative $S(X)$ of every [subset](set.md#subset) $X$ of a previous stage, except that $S(\{q\})=q$ uses the atom already present. Define membership by these extensions. Each set-sized collection of objects has bounded construction rank, so it has a representative at a later stage. This gives full [extensionality](#axiom-of-extensionality), unlike adjoining an ordinary singleton distinct from a [Quine atom](#quine-atom). Definable [subsets](set.md#subset) and ranges, [unions](set.md#set-union) and power [sets](set.md) are set-sized collections in the ambient model and hence have representatives. The pure finite hierarchy supplies [infinity](mathematics.md#infinity). Every permutation of the atoms extends recursively; hereditary [finite support](group-theory.md#finite-support-in-a-permutation-action) restriction gives the [hereditarily finite-supported Quine-atom model](#hereditarily-finite-supported-quine-atom-model), whose two-element atom [subsets](set.md#subset) have no [choice function](#choice-function).

##### Hereditarily finite-supported Quine-atom model

↑ **Parent:** [Quine atom](#quine-atom)

Build the cumulative universe over an infinite set $A$ of [Quine atoms](#quine-atom), and extend every permutation of $A$ recursively to its other sets. An object has finite support if every permutation fixing that finite subset of $A$ fixes the object. Retain objects whose members, recursively away from the atomic self-loops, also have finite support. Parameters and domains give finite supports for definable subsets and functional ranges; the collection of all retained subsets of a retained set is again supported. These observations verify separation, replacement and power set, and the pure natural-number hierarchy gives infinity. There is no choice function on the two-element subsets of $A$: swap two atoms outside its supposed finite support, fixing their unordered pair but interchanging either possible selected member.

### Axiom of infinity

↑ **Parent:** [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_infinity)

The axiom asserts the existence of a set containing the empty set and closed under the successor operation $x\mapsto x\cup\{x\}$:

$$
\exists I\;\bigl(\varnothing\in I\land\forall x\in I\;(x\cup\{x\}\in I)\bigr).
$$

In [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory), this supplies a set from which the set of [natural numbers](arithmetic.md#natural-number) is constructed.

#### Inductive set

↑ **Parent:** [Axiom of infinity](#axiom-of-infinity)

A [set](set.md) $I$ is inductive if it contains the [empty set](set.md#empty-set) and contains $x\cup\{x\}$ whenever it contains $x$. The [axiom of infinity](#axiom-of-infinity) asserts that an [inductive set](#inductive-set) exists. The [natural numbers](arithmetic.md#natural-number) form the least [inductive set](#inductive-set): intersect one [inductive set](#inductive-set) with the class of objects belonging to every [inductive set](#inductive-set). This use of [separation](#axiom-schema-of-specification) gives a [set](set.md), and the defining class is closed under successor.

<h3 id="zermelo-fraenkel-set-theory-with-choice">Zermelo–Fraenkel set theory with choice</h3>

↑ **Parent:** [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory)

ZFC is [Zermelo–Fraenkel set theory](#zermelo-fraenkel-set-theory) together with the [axiom of choice](#axiom-of-choice).

## Von Neumann hierarchy

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Neumann_hierarchy)

The von Neumann hierarchy is

$$
V_0=\varnothing,
\qquad
V_{\alpha+1}=\mathcal P(V_\alpha),
\qquad
V_\lambda=\bigcup_{\beta<\lambda}V_\beta.
$$

Every level is transitive, the levels are increasing, and every set belongs to some level.

### Countable rank-initial segment cannot model ZFC

↑ **Parent:** [Von Neumann hierarchy](#von-neumann-hierarchy)

If $\alpha$ is a [countable ordinal](#countable-ordinal) and $V_\alpha\models\mathsf{ZFC}$, then $\alpha$ must be a limit ordinal. Choose a countable cofinal sequence $(\alpha_n)$ in $\alpha$. The internal [axiom of choice](#axiom-of-choice) gives, for every $n$, a bijection between $V_{\alpha_n}$ and some ordinal below $\alpha$; that ordinal is externally countable, so every $V_{\alpha_n}$ is countable. Hence $V_\alpha=\bigcup_nV_{\alpha_n}$ is countable. But $V_\alpha$ contains the full [power set](set.md#power-set) $\mathcal P(\omega)$, which is uncountable by [Cantor theorem](set.md#cantor-s-theorem), a contradiction.

<h3 id="levy-reflection-theorem">Lévy reflection theorem</h3>

↑ **Parent:** [Von Neumann hierarchy](#von-neumann-hierarchy)

For every finite collection $\Phi$ of [first-order formulas](mathematical-logic.md#first-order-formula), there are arbitrarily large [ordinals](#ordinal) $\alpha$ such that, for every $\varphi\in\Phi$ and all parameters in $V_\alpha$,

$$
V_\alpha\models\varphi
\quad\Longleftrightarrow\quad
V\models\varphi.
$$

The reflecting ordinals for $\Phi$ form a closed unbounded class.

#### Club reflection below an inaccessible cardinal

↑ **Parent:** [Lévy reflection theorem](#levy-reflection-theorem)

For inaccessible $\kappa$ and any predicate $R\subseteq V_\kappa$, the ordinals $\alpha<\kappa$ with $\langle V_\alpha,\in,R\cap V_\alpha\rangle\prec\langle V_\kappa,\in,R\rangle$ form a club. Closure under ranks of existential witnesses gives unboundedness, and the [elementary chain theorem](foundations-of-mathematics.md#elementary-chain-theorem) gives closedness.

#### Reflection theorem for definable hierarchies

↑ **Parent:** [Lévy reflection theorem](#levy-reflection-theorem)

A finite collection of [first-order formulas](mathematical-logic.md#first-order-formula) has a [closed unbounded class of ordinals](#closed-unbounded-class-of-ordinals) whose levels in a [definable continuous hierarchy](#definable-continuous-hierarchy) agree with its union for all parameters in the level. Close the collection under subformulas, bound the least witness levels for existential instances on each set-sized stage by [Axiom schema of replacement](#axiom-schema-of-replacement), and iterate these bounds countably. Continuity supplies the closed stages, and induction on formulas proves agreement. The [Tarski-Vaught test](mathematical-logic.md#tarski-vaught-test) describes the same witness criterion. For a hierarchy of length an uncountable [regular cardinal](#regular-cardinal), bounds stay below that cardinal when every stage has smaller [cardinality](#cardinality).

#### Ordinal described by a first-order formula

↑ **Parent:** [Lévy reflection theorem](#levy-reflection-theorem)

A [first-order formula](mathematical-logic.md#first-order-formula) $\varphi$ describes an ordinal $\alpha$ when $\alpha$ is the least ordinal such that $V_\alpha\models\varphi$. No [strongly inaccessible cardinal](#strongly-inaccessible-cardinal) can be described: if $V_\kappa\models\varphi$, the [Lévy reflection theorem](#levy-reflection-theorem) produces some $\alpha<\kappa$ with $V_\alpha\models\varphi$.

### Rank of a set

↑ **Parent:** [Von Neumann hierarchy](#von-neumann-hierarchy)

The rank is defined by

$$
\operatorname{rank}(x)
=\sup_{y\in x}(\operatorname{rank}(y)+1).
$$

It is the least ordinal $\alpha$ for which $x\subseteq V_\alpha$.

## Definable power set

↑ **Parent:** [Set theory](set-theory.md)

[This section is present in another page, follow this link to view it.](definable-power-set.md)

## Forcing

↑ **Parent:** [Set theory](set-theory.md)

[This section is present in another page, follow this link to view it.](forcing.md)

## Delta-system lemma

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Delta-system_lemma)

Every uncountable family of finite sets has an uncountable subfamily whose distinct members have the same pairwise intersection, called the root. It is also known as the sunflower lemma.

### Generalized delta-system lemma

↑ **Parent:** [Delta-system lemma](#delta-system-lemma)

If $\mu<\theta=\operatorname{cf}(\theta)$ are infinite [cardinals](#cardinal-number) and $|[\alpha]^{<\mu}|<\theta$ for every $\alpha<\theta$, every $\theta$-sized family of sets of size less than $\mu$ has a $\theta$-sized [delta-system](#delta-system) subfamily.

### Delta-system

↑ **Parent:** [Delta-system lemma](#delta-system-lemma)

A family of sets is a Delta-system with root $r$ when any two distinct members intersect exactly in $r$. The members themselves need not be finite, although the usual [Delta-system lemma](#delta-system-lemma) applies to uncountable families of finite sets.

<h4 id="erdos-rado-sunflower-lemma">Erdős–Rado sunflower lemma</h4>

↑ **Parent:** [Delta-system](#delta-system)

A sunflower is a [delta-system](#delta-system): its pairwise [intersections](set.md#set-intersection) all equal one core, and its petals outside the core are pairwise disjoint. For an $s$-[uniform set family](extremal-set-theory.md#uniform-set-family), prove the displayed bound by [induction](foundations-of-mathematics.md#mathematical-induction) on $s$. If a maximal disjoint subfamily has $r$ members, their core is empty. Otherwise its union has at most $s(r-1)$ points and meets every member. Some point belongs to more than $(s-1)!(r-1)^{s-1}$ members. Remove it and apply the induction hypothesis; putting it back enlarges the common core. The case $s=0$ is immediate.

### Delta-system lemma at a regular uncountable cardinal

↑ **Parent:** [Delta-system lemma](#delta-system-lemma)

If $\kappa$ is a regular uncountable [cardinal number](#cardinal-number), every family of $\kappa$ finite sets has a subfamily of cardinality $\kappa$ whose distinct members have one common pairwise intersection.

## Standard model (set theory)

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_model_(set_theory))

A standard model of [set theory](set-theory.md) interprets membership by the ambient membership relation restricted to its domain. A [transitive model](#transitive-model) additionally has a [transitive set](#transitive-set) or class as its domain. Standardness alone does not impose transitivity.

## Transitive set

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transitive_set)

A set $X$ is transitive when every element of an element of $X$ is itself an element of $X$.

### Transitive model

↑ **Parent:** [Transitive set](#transitive-set)

A transitive model of set theory is a [transitive set](#transitive-set) or [transitive class](#transitive-class) whose membership relation is the ambient membership relation and which satisfies the specified set-theoretic axioms.

#### Well-founded model of set theory

↑ **Parent:** [Transitive model](#transitive-model)

A model of set theory is well-founded when its internally interpreted membership relation is a [well-founded relation](#well-founded-relation) externally. By the [Mostowski collapse theorem](#mostowski-collapse-theorem), every well-founded extensional set model is isomorphic to a transitive model.

#### Ordinal height of a model of set theory

↑ **Parent:** [Transitive model](#transitive-model)

The ordinal height of a model $M$ is its class of internal ordinals. For a transitive set model this is an ordinal $\operatorname{Ord}\cap M$.

##### Uncountable transitive set model has uncountable ordinal height

↑ **Parent:** [Ordinal height of a model of set theory](#ordinal-height-of-a-model-of-set-theory)

Let $M$ be a transitive set model of [ZFC](#zermelo-fraenkel-set-theory-with-choice). If $\operatorname{Ord}\cap M$ were countable, then every $x\in M$ would be countable: the internal [axiom of choice](#axiom-of-choice) supplies a bijection from $x$ to an ordinal of $M$, which is externally countable. For every $\alpha\in\operatorname{Ord}\cap M$, the internal rank $V_\alpha^M$ is an element of $M$ and hence countable. The [Axiom schema of replacement](#axiom-schema-of-replacement) inside $M$ gives $M=\bigcup_{\alpha\in\operatorname{Ord}\cap M}V_\alpha^M$, a countable union of countable sets. Thus every uncountable transitive set model has uncountably many ordinals.

###### Countable-ordinal correctness under constructibility

↑ **Parent:** [Uncountable transitive set model has uncountable ordinal height](#uncountable-transitive-set-model-has-uncountable-ordinal-height)

Assuming $V=L$, every uncountable [transitive model](#transitive-model) of [ZFC](#zermelo-fraenkel-set-theory-with-choice) contains all ambient [countable ordinals](#countable-ordinal) and witnesses their countability internally. Its ordinal height is at least $\omega_1$, and [absoluteness of constructible levels](definable-power-set.md#absoluteness-of-constructible-levels) puts $L_{\omega_1}$ inside it. Every countability witness for a countable ordinal can be chosen in $L_{\omega_1}$ by [hereditarily countable constructible sets appear below omega-one](definable-power-set.md#hereditarily-countable-constructible-sets-appear-below-omega-one).

## Well-founded relation

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Well-founded_relation)

A relation $r$ on $X$ is well-founded when every nonempty subset of $X$ contains an element with no $r$-predecessor in that subset.

### Intersection-power-set predecessor relation

↑ **Parent:** [Well-founded relation](#well-founded-relation)

This relation has [well-foundedness](#well-founded-relation) without [Axiom of foundation](#axiom-of-regularity) or [axiom of choice](#axiom-of-choice). If a nonempty set $S$ had no minimal member, put $b=\bigcap S$. For each $y\in S$, choose existentially an $x\in S$ with $xRy$. Since $b\subseteq x\cap y$, every subset of $b$ belongs to $y$. Thus $\mathcal P(b)\subseteq b$. But $d=\{u\in b:u\notin u\}$ is then an element of $b$, contradicting $d\in d\iff d\notin d$.

### Power-set-predecessor relation

↑ **Parent:** [Well-founded relation](#well-founded-relation)

This [well-founded relation](#well-founded-relation) is well-founded without the [axiom of choice](#axiom-of-choice) or [Axiom of foundation](#axiom-of-regularity). If a nonempty set $A$ lacked a minimal member, put $b=\bigcap A$. For each $y\in A$, some $x\in A$ has $\mathcal P(x)\subseteq y$, and $b\subseteq x$ gives $\mathcal P(b)\subseteq y$. Hence $\mathcal P(b)\subseteq b$. The [Cantor diagonal argument](#cantor-diagonal-argument) applied to $d=\{u\in b:u\notin u\}$ contradicts this inclusion.

### Well-founded induction

↑ **Parent:** [Well-founded relation](#well-founded-relation)

To prove a property at every point of a [well-founded relation](#well-founded-relation), prove that it holds at a point whenever it holds at all its predecessors.

### Well-founded recursion

↑ **Parent:** [Well-founded relation](#well-founded-relation)

A recursive definition in which the value at a point depends on its predecessor values in a [well-founded relation](#well-founded-relation). For a class relation, set-likeness allows the local set recursions to combine into a class function.

#### Recursive powerset mapping

↑ **Parent:** [Well-founded recursion](#well-founded-recursion)

A map $f:a\to\mathcal P(a)$ is recursive if every map $g:\mathcal P(b)\to b$ admits a unique $h:a\to b$ with $h(y)=g(\{h(x):x\in f(y)\})$. This holds exactly when the predecessor relation $x\in f(y)$ is a [well-founded relation](#well-founded-relation). For the forward construction, take the union of all consistent partial solutions on downward-closed domains; [well-founded induction](#well-founded-induction) proves compatibility, and a minimal missing point allows extension. Conversely, a nonempty subset with no minimal point has an upward reachability closure $T$ satisfying $y\in T$ exactly when some predecessor is in $T$. With $b=\{0,1\}$ and $g(S)=1$ exactly when $1\in S$, both the zero map and the indicator of $T$ solve the recursion, contradicting uniqueness.

#### Ordinal rank function for a relation

↑ **Parent:** [Well-founded recursion](#well-founded-recursion)

An ordinal-valued function strictly increasing along a relation. For a well-founded set relation, or a [set-like](#set-like-relation) class relation, the canonical rank is $\rho(y)=\sup\{\rho(x)+1:xRy\}$.

##### Rank of a well-founded tree

↑ **Parent:** [Ordinal rank function for a relation](#ordinal-rank-function-for-a-relation)

The rank of a terminal node is zero; the rank of any node is the supremum of the successor ranks of its immediate extensions. The rank of the empty node gives one convention for tree height. Every countable well-founded tree has countable rank. Changing between empty-root rank and successive leaf-deletion order changes harmless endpoint conventions.

###### Maurey hierarchy of finite sets

↑ **Parent:** [Rank of a well-founded tree](#rank-of-a-well-founded-tree)

This hierarchy measures the complexity of successive finite selections. Start with $\mathcal M_0=\{\varnothing\}$. At a successor stage, retain the previous family and allow one smaller integer to be prepended. At a countable limit $\lambda$, choose positive ordinals $\lambda_j\uparrow\lambda$ and admit sets in $\mathcal M_{\lambda_j}$ whose minimum is at least $j$. Each family is hereditary and spreading, has no infinite branch, and its extension-tree rank on every infinite subset is at least $\alpha$. These properties make the hierarchy useful for transfinite constructions of [unconditional basic sequences](functional-analysis.md#unconditional-basic-sequence).

### Set-like relation

↑ **Parent:** [Well-founded relation](#well-founded-relation)

A class relation for which each point has a set of predecessors. This allows the suprema in [well-founded recursion](#well-founded-recursion) to be ordinals rather than proper classes.

## Extensional relation

↑ **Parent:** [Set theory](set-theory.md)

A relation is extensional when distinct elements have distinct sets of predecessors.

This is the predecessor-set instance of the identity principle [extensionality](#axiom-of-extensionality).

## Set

↑ **Parent:** [Set theory](set-theory.md)

[This section is present in another page, follow this link to view it.](set.md)

## Binary relation

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_relation)

A binary relation on a set $X$ is a subset of $X\times X$.

### Binary relations with no empty row or column

↑ **Parent:** [Binary relation](#binary-relation)

Represent a [binary relation](#binary-relation) on an $n$-element [finite set](set.md#finite-set) by its zero-one incidence [matrix](vector-space.md#matrix). If no column may be empty, each column has $2^n-1$ choices. Apply the [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) to empty rows: fixing $k$ empty rows leaves $(2^{n-k}-1)^n$ allowed matrices. Summing over those row sets with alternating signs yields the displayed count.

### Preference relation

↑ **Parent:** [Binary relation](#binary-relation)

A weak [preference relation](#preference-relation) records that one alternative is at least as desirable as another. Rational preferences are complete and [transitive](#transitive-relation). Their [strict preference](#strict-preference) and [indifference relation](#indifference-relation) are the asymmetric and symmetric parts. On a consumption space, continuity is expressed by a [closed set](topology.md#closed-set) of weakly ranked pairs.

#### Closed convergence of preference relations

↑ **Parent:** [Preference relation](#preference-relation)

This is the [Fell topology](topology.md#fell-topology) restricted to closed graphs of complete, [transitive](#transitive-relation), continuous [preference relations](#preference-relation). Both the upper limit condition and approximation of every limiting weak comparison are needed. A large limiting indifference class can make the second requirement stronger than convergence of numerical utility differences.

##### Uniform utility convergence need not preserve closed preference convergence

↑ **Parent:** [Closed convergence of preference relations](#closed-convergence-of-preference-relations)

On $[0,\infty)$ the [utility functions](utility-function.md) $u_n(x)=x/n$ converge uniformly on every bounded set to $u(x)=0$. Their [preference relations](#preference-relation) remain the usual order, while the limiting [utility function](utility-function.md) makes all pairs indifferent. The weak comparison $0\succeq1$ in the limit cannot be approximated by comparisons from the varying graphs. Uniform convergence does guarantee the upper graph-limit condition, because convergent pairs remain in a fixed bounded set.

#### Indifference relation

↑ **Parent:** [Preference relation](#preference-relation)

For a [preorder](set.md#preorder), the [indifference relation](#indifference-relation) is an [equivalence relation](#equivalence-relation). Passing to its equivalence classes removes ties and produces a [partial order](set.md#partially-ordered-set).

#### Strict preference

↑ **Parent:** [Preference relation](#preference-relation)

The [strict preference](#strict-preference) associated with a weak [preference relation](#preference-relation) retains comparisons that do not hold in the reverse direction.

### Composition of relations

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Composition_of_relations)

This convention composes paths in their written order; some sources instead reverse that convention. [Composition of relations](#composition-of-relations) is associative. Taking inverse relations reverses the order: $(R\circ S)^{-1}=S^{-1}\circ R^{-1}$.

// Target: foundations-of-mathematics.bigb

### Reflexive relation

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflexive_relation)

A relation $\mathrel R$ on $X$ is reflexive when $x\mathrel R x$ for every $x\in X$.

#### Reflexive closure

↑ **Parent:** [Reflexive relation](#reflexive-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflexive_closure)

The reflexive closure of a [binary relation](#binary-relation) $R\subseteq A\times A$ is $R\cup\Delta_A$, where $\Delta_A=\{(a,a):a\in A\}$. Every [reflexive relation](#reflexive-relation) containing $R$ must contain the diagonal, so this is the least such extension.

### Symmetric relation

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_relation)

A relation $\mathrel R$ is symmetric when $x\mathrel R y$ implies $y\mathrel R x$.

#### Symmetric closure

↑ **Parent:** [Symmetric relation](#symmetric-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_closure)

The symmetric closure of a [binary relation](#binary-relation) $R$ is $R\cup R^{-1}$, where $(x,y)\in R^{-1}$ means $(y,x)\in R$. Every [symmetric relation](#symmetric-relation) containing $R$ contains all these reversed pairs, proving minimality.

### Antisymmetric relation

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antisymmetric_relation)

A relation $\mathrel R$ is antisymmetric when $x\mathrel R y$ and $y\mathrel R x$ together imply $x=y$.

### Transitive relation

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transitive_relation)

A relation $\mathrel R$ is transitive when $x\mathrel R y$ and $y\mathrel R z$ imply $x\mathrel R z$.

#### Transitive closure (relation)

↑ **Parent:** [Transitive relation](#transitive-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transitive_closure)

The transitive closure of a relation connects $x$ to $y$ when a finite nonempty chain of $R$-steps leads from $x$ to $y$. Concatenation proves [transitivity](#transitive-relation), and induction along a chain shows that any [transitive relation](#transitive-relation) containing $R$ contains $R^+$. This concerns closure of a relation, rather than the [transitive closure](#transitive-closure) of a set under membership.

### Equivalence relation

↑ **Parent:** [Binary relation](#binary-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivalence_relation)

An equivalence relation is a reflexive, symmetric, and transitive binary relation. It partitions a set into disjoint equivalence classes.

#### Composition of commuting equivalence relations

↑ **Parent:** [Equivalence relation](#equivalence-relation)

Using the left-to-right convention for [composition of relations](#composition-of-relations), two [equivalence relations](#equivalence-relation) $R,S$ have an equivalence-relation composite exactly when $R\circ S=S\circ R$. Its inverse is $S\circ R$. Commutation gives $(R\circ S)^2=R^2\circ S^2=R\circ S$, proving transitivity. Every equivalence relation containing $R,S$ contains their two-step composite, so this is their least common extension.

// Destination: combinatorics.bigb

#### Commuting equivalence relations

↑ **Parent:** [Equivalence relation](#equivalence-relation)

For two [equivalence relations](#equivalence-relation) on the same set, their composite contains each and is reflexive. It is symmetric exactly when the relations commute. It is transitive exactly when $S\circ R\subseteq R\circ S$, which by inversion is also equivalent to commutation. Under these conditions the composite is the smallest equivalence relation containing both. For congruences modulo $m,n$ on the integers, their composite is congruence modulo $\gcd(m,n)$.

// Target: combinatorics.bigb

#### Equivalence closure

↑ **Parent:** [Equivalence relation](#equivalence-relation)

The equivalence closure of a [binary relation](#binary-relation) $R$ is the least [equivalence relation](#equivalence-relation) containing it. Add diagonal and reversed pairs, then connect points by finite chains. Constant chains prove reflexivity, reversed chains prove symmetry, and concatenated chains prove transitivity. Any equivalence relation extending $R$ contains every such chain endpoint by induction.

#### Union of equivalence relations

↑ **Parent:** [Equivalence relation](#equivalence-relation)

A union of [equivalence relations](#equivalence-relation) on the same [set](set.md) is reflexive and symmetric, but can fail [transitivity](#transitive-relation). On a three-point [set](set.md), partitions into blocks $\{1,2\},\{3\}$ and $\{1\},\{2,3\}$ make the union relate $1$ to $2$ and $2$ to $3$ without relating $1$ to $3$. An equivalence relation containing both requires transitive closure as well.

#### Intersection of equivalence relations

↑ **Parent:** [Equivalence relation](#equivalence-relation)

The intersection of any family of [equivalence relations](#equivalence-relation) on one [set](set.md) is an [equivalence relation](#equivalence-relation). Reflexivity and symmetry hold in every component. A pair of consecutive related points belongs to every component, so each component's [transitivity](#transitive-relation) supplies the required final pair. Its [equivalence classes](#equivalence-class) refine the component partitions. The empty intersection is the universal relation.

#### Co-computably enumerable equivalence relation

↑ **Parent:** [Equivalence relation](#equivalence-relation)

An [equivalence relation](#equivalence-relation) on the [natural numbers](arithmetic.md#natural-number) is co-computably enumerable when its [complement](set.md#complement-of-a-set) as a set of pairs is [computably enumerable](foundations-of-mathematics.md#recursively-enumerable-set). Inequivalence can then be positively recognized, even when equivalence cannot be decided. This is sufficient for a [semidecidable least-representative transversal](#semidecidable-least-representative-transversal).

##### Semidecidable least-representative transversal

↑ **Parent:** [Co-computably enumerable equivalence relation](#co-computably-enumerable-equivalence-relation)

For a [co-computably enumerable equivalence relation](#co-computably-enumerable-equivalence-relation), the least element of each [equivalence class](#equivalence-class) forms a complete [transversal of a set family](extremal-set-theory.md#hitting-set). Membership is [semidecidable](foundations-of-mathematics.md#recursively-enumerable-set): run the finitely many inequivalence tests against smaller numbers in parallel and accept when all succeed. Infinitely many classes are needed only to make the resulting transversal infinite.

#### Equivalence of partial functions modulo finite changes

↑ **Parent:** [Equivalence relation](#equivalence-relation)

Two [functions](function.md) $f:A\to X$ and $g:B\to X$, whose domains lie in one ambient [set](set.md), are equivalent modulo finite changes when $A\mathbin\triangle B$ is a [finite set](set.md#finite-set) and the [functions](function.md) disagree at only finitely many points of $A\cap B$. The [symmetric difference](set.md#symmetric-difference) inclusion $A\mathbin\triangle C\subseteq(A\mathbin\triangle B)\cup(B\mathbin\triangle C)$ handles domains in a transitive chain. An exceptional [set](set.md) for values must also include points of $A\cap C$ absent from the middle domain $B$; these lie in the finite difference $A\setminus B$.

#### Equivalence class

↑ **Parent:** [Equivalence relation](#equivalence-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equivalence_class)

The equivalence class of an element $x$ under an [equivalence relation](#equivalence-relation) $R$ is the [set](set.md) of all elements related to $x$. Two such [sets](set.md) are equal or disjoint, and together they partition the original [set](set.md).

#### Equivalence relation induced by a function

↑ **Parent:** [Equivalence relation](#equivalence-relation)

Every [function](function.md) $f:X\to Y$ induces an [equivalence relation](#equivalence-relation) on $X$ by $x\sim y$ exactly when $f(x)=f(y)$. Reflexivity, symmetry, and transitivity follow from the corresponding properties of equality in $Y$; the equivalence classes are the nonempty fibers of $f$.

##### Prime-support equivalence relation

↑ **Parent:** [Equivalence relation induced by a function](#equivalence-relation-induced-by-a-function)

Positive [integers](number-theory.md#integer) are equivalent when they have the same finite set of [prime factors](number-theory.md#prime-factor). Equivalently, each divides a positive power of the other. This [equivalence relation](#equivalence-relation) is induced by the [radical of an integer](number-theory.md#radical-of-an-integer); its [equivalence classes](#equivalence-class) correspond to finite prime supports. The empty support gives the singleton $\{1\}$, and every nonempty support gives an infinite class by varying exponents.

#### Quotient set

↑ **Parent:** [Equivalence relation](#equivalence-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quotient_set)

The quotient set $X/{\sim}$ of a [set](set.md) $X$ by an [equivalence relation](#equivalence-relation) $\sim$ is the set of its equivalence classes.

## Function

↑ **Parent:** [Set theory](set-theory.md)

[This section is present in another page, follow this link to view it.](function.md)

<h2 id="zorn-s-lemma">Zorn's lemma</h2>

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zorn's_lemma)

If every chain in a nonempty partially ordered set has an upper bound, then the set has a maximal element.

## Class (set theory)

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_(set_theory))

A class is a collection of sets specified by a formula, possibly with set parameters. A class is a set when one set has exactly those members.

### Set-theoretic class function

↑ **Parent:** [Class (set theory)](#class-set-theory)

A set-theoretic class function is a definable class of ordered pairs whose relation is functional: every input in its domain has exactly one output. Its graph need not be a set.

### Proper class

↑ **Parent:** [Class (set theory)](#class-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Proper_class)

A proper class is a [class in set theory](#class-set-theory) that is not a set in the ambient universe.

### Transitive class

↑ **Parent:** [Class (set theory)](#class-set-theory)

A class $M$ is transitive when $x\in y\in M$ implies $x\in M$. Consequently, every member of a member of $M$ is available as an element of the structure $(M,\in)$.

#### Basic set-theoretic axioms inherited by a transitive class

↑ **Parent:** [Transitive class](#transitive-class)

If a transitive class $M$ contains the empty set and is closed under pairing and union, then $(M,\in)$ satisfies extensionality, empty set, pairing, and union. Transitivity makes all members of each $x\in M$ visible inside $M$, so the ambient witnesses have the same required membership relations internally.

#### Formula relativization to a class

↑ **Parent:** [Transitive class](#transitive-class)

The relativization $\varphi^M$ of a formula $\varphi$ is obtained recursively by restricting every quantifier to $M$:

$$
(\exists x\,\psi)^M=\exists x\,(x\in M\land\psi^M),
\qquad
(\forall x\,\psi)^M=\forall x\,(x\in M\mathbin\Rightarrow\psi^M).
$$

For parameters in $M$, the ambient statement $\varphi^M$ holds exactly when the structure $(M,\in)$ satisfies $\varphi$.

##### Set-theoretic absoluteness

↑ **Parent:** [Formula relativization to a class](#formula-relativization-to-a-class)

A formula is absolute between transitive classes $M\subseteq N$ when it has the same truth value in both structures for parameters from $M$.

###### Delta-one absoluteness

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

Let $M\subseteq N$ be [transitive models](#transitive-model) of a theory proving both an existential-bounded and a universal-bounded equivalent of a formula. For parameters in $M$, the existential form gives upward absoluteness and the universal form gives downward absoluteness. Consequently the models agree on the formula. The equivalences must hold in both models.

###### Absoluteness of well-foundedness

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

For a set relation in nested transitive models of [ZFC](#zermelo-fraenkel-set-theory-with-choice), well-foundedness is absolute. An inner-model ordinal rank function witnesses upward absoluteness, and a fixed nonempty subset without a minimal member witnesses failure in both models.

###### Absolute formula

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

A formula with unchanged truth value between the specified models, using parameters shared by them. Usually the models in set-theoretic applications are transitive and nested; the class of models is part of the assertion of absoluteness.

###### Absoluteness of cardinalhood in limit ranks

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

For [limit ordinals](#limit-ordinal) $\alpha\leq\beta$, the structures $V_\alpha$ and $V_\beta$ agree on whether any shared [set](set.md) is a [cardinal number](#cardinal-number). They agree on being an [ordinal](#ordinal). If $\delta<\alpha$ is not a [cardinal number](#cardinal-number), a [bijection](function.md#bijection) from some $\gamma<\delta$ onto $\delta$ has [rank of a set](#rank-of-a-set) at most $\delta+3$, hence belongs to $V_\alpha$. Its defining properties are [bounded formulas in set theory](#bounded-formula-in-set-theory). Both structures therefore see the same failure witness. This full agreement is stronger than [downward absoluteness of cardinalhood](#downward-absoluteness-of-cardinalhood) between arbitrary [transitive models](#transitive-model).

###### Upward absolute formula

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

A formula is upward absolute when its truth in a smaller transitive class implies its truth in a larger one. Existential formulas with bounded matrices are upward absolute because their witnesses remain available.

###### Downward absolute formula

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

A formula is downward absolute when its truth in a larger transitive class implies its truth in a smaller one. Universal formulas with bounded matrices are downward absolute.

###### Bounded formula in set theory

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

A bounded formula in set theory has every quantifier in one of the forms $\forall x\in y$ or $\exists x\in y$. Such formulas are absolute between transitive models containing their parameters.

###### ZF-equivalent bounded formula

↑ **Parent:** [Bounded formula in set theory](#bounded-formula-in-set-theory)

A [first-order formula](mathematical-logic.md#first-order-formula) is ZF-equivalent bounded if [ZF](#zermelo-fraenkel-set-theory) proves it equivalent, with the same free variables, to a syntactically [bounded formula in set theory](#bounded-formula-in-set-theory). It need not itself have only bounded quantifiers. Between [transitive models](#transitive-model) of [ZF](#zermelo-fraenkel-set-theory), use the bounded equivalent and the axioms in each model to prove [set-theoretic absoluteness](#set-theoretic-absoluteness). The syntactic bounded-formula result requires only transitivity; the provable-equivalence extension additionally requires the theory used for the equivalence.

###### Absoluteness of infinitude between transitive models

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

Transitive models of [ZFC](#zermelo-fraenkel-set-theory-with-choice) have the same [natural numbers](arithmetic.md#natural-number) and agree on whether a shared set is a [finite set](set.md#finite-set). Consequently they also agree on whether it is an [infinite set](set.md#infinite-set).

###### Downward absoluteness of cardinalhood

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

If a larger transitive model regards an ordinal $\kappa$ as a [cardinal number](#cardinal-number), then a smaller transitive model does too: any bijection in the smaller model witnessing otherwise would remain in the larger one. The converse can fail when the larger model contains a new bijection between $\kappa$ and a smaller ordinal.

###### Upward absoluteness of countability

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

If a smaller transitive model has a function witnessing that $x$ is a [countable set](#countable-set), the same witness exists in every larger transitive model. Downward absoluteness can fail because a larger model may contain a new enumeration of $x$.

###### Nonabsoluteness of singular cardinalhood

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

The statement that $\kappa$ is a [cardinal number](#cardinal-number) with $\operatorname{cf}(\kappa)<\kappa$ is generally neither upward nor downward absolute. Upward absoluteness can fail when a larger model collapses the cardinal; downward absoluteness can fail when a larger model adds a short cofinal sequence to a cardinal that the smaller model regards as regular.

###### Cardinal nonabsoluteness in a small transitive model

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

Let $M$ be a [transitive set](#transitive-set) of cardinality $\kappa$ that models enough set theory and contains $\kappa$. The internal [successor cardinal](#successor-cardinal) $\alpha=(\kappa^+)^M$ is an ordinal in $M$, so transitivity gives $\alpha\subseteq M$ and hence $|\alpha|\leq\kappa$ externally. Although $M$ regards $\alpha$ as a [cardinal number](#cardinal-number), an ambient rank containing a bijection between $\kappa$ and $\alpha$ does not. Cardinalhood can therefore fail to be absolute even between transitive models.

###### Strong-inaccessibility absoluteness from rank agreement

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)

If transitive models of enough set theory contain the same $V_{\alpha+1}$, then they agree on whether $\alpha$ is a [strongly inaccessible cardinal](#strongly-inaccessible-cardinal). They have the same subsets and functions on every ordinal below $\alpha$, so they agree on [cardinality](#cardinal-number), [regularity](#regular-cardinal), and the [strong limit cardinal](#strong-limit-cardinal) property.

<h6 id="levy-hierarchy">Lévy hierarchy</h6>

↑ **Parent:** [Set-theoretic absoluteness](#set-theoretic-absoluteness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lévy_hierarchy)

The Lévy hierarchy classifies formulas of set theory by their alternations of unbounded quantifiers, ignoring bounded quantifiers of the forms $\forall x\in y$ and $\exists x\in y$.

###### Delta-one formula modulo ZFC

↑ **Parent:** [Lévy hierarchy](#levy-hierarchy)

A [first-order formula](mathematical-logic.md#first-order-formula) is $\Delta_1$ modulo [ZFC](#zermelo-fraenkel-set-theory-with-choice) if that theory proves it equivalent, with the same free variables, both to a [Sigma-one formula in set theory](#sigma-one-formula-in-set-theory) and to a universal unbounded quantifier block with a [bounded formula in set theory](#bounded-formula-in-set-theory) as matrix. The theory used for provable equivalence matters: modulo [ZF](#zermelo-fraenkel-set-theory) is a stronger requirement.

###### Pi-one formula in set theory

↑ **Parent:** [Lévy hierarchy](#levy-hierarchy)

A syntactically $\Pi_1$ [first-order formula](mathematical-logic.md#first-order-formula) has an unbounded universal quantifier block followed by a [bounded formula in set theory](#bounded-formula-in-set-theory). Universal quantification makes it downward absolute between [transitive models](#transitive-model). A [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf) may have another syntax but has such an equivalent provable in [ZF](#zermelo-fraenkel-set-theory).

###### Sigma-one formula in set theory

↑ **Parent:** [Lévy hierarchy](#levy-hierarchy)

A [first-order formula](mathematical-logic.md#first-order-formula) is syntactically $\Sigma_1$ when it is an unbounded existential quantifier block followed by a [bounded formula in set theory](#bounded-formula-in-set-theory). Equivalence provable in a specified theory gives the corresponding modulo-theory notion. Existential witnesses show upward absoluteness between [transitive models](#transitive-model) containing the parameters.

###### Pi-one formula modulo ZF

↑ **Parent:** [Lévy hierarchy](#levy-hierarchy)

A [first-order formula](mathematical-logic.md#first-order-formula) is $\Pi_1^{\mathrm{ZF}}$ if [ZF](#zermelo-fraenkel-set-theory) proves it equivalent, with the same free variables, to a universal unbounded quantifier block followed by a [bounded formula in set theory](#bounded-formula-in-set-theory). Bounded quantifiers do not increase its level in the [Lévy hierarchy](#levy-hierarchy). Such properties are downward absolute between appropriate [transitive models](#transitive-model) of [ZF](#zermelo-fraenkel-set-theory).

###### Regular cardinalhood is Pi-one definable

↑ **Parent:** [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf)

An infinite [cardinal number](#cardinal-number) $\kappa$ is a [regular cardinal](#regular-cardinal) if every function from an ordinal $\delta<\kappa$ into $\kappa$ has bounded range. Write this as $\forall f\,\forall\delta\in\kappa\,(\operatorname{Map}(f,\delta,\kappa)\Rightarrow\exists\beta\in\kappa\,\forall\xi\in\delta\ f(\xi)<\beta)$. The graph predicates are [bounded formulas in set theory](#bounded-formula-in-set-theory), and [cardinalhood is Pi-one definable](#cardinalhood-is-pi-one-definable), so adding infinite cardinalhood yields a [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf).

###### Cardinalhood is Pi-one definable

↑ **Parent:** [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf)

An ordinal $\kappa$ is a [cardinal number](#cardinal-number) precisely when no smaller ordinal has a [bijection](function.md#bijection) onto it. Ordinalhood and the graph predicate for a [bijection](function.md#bijection) are [bounded formulas in set theory](#bounded-formula-in-set-theory), so $\operatorname{Ord}(\kappa)\land\forall f\,\forall\alpha\in\kappa\,\neg\operatorname{Bij}(f,\alpha,\kappa)$ is a [Pi-one formula modulo ZF](#pi-one-formula-modulo-zf). This does not assert that every set can be assigned an ordinal cardinal without the [axiom of choice](#axiom-of-choice).

###### Delta-one formula in set theory

↑ **Parent:** [Lévy hierarchy](#levy-hierarchy)

A formula is $\Delta_1^{\mathrm{ZF}}$ when ZF proves it equivalent both to a $\Sigma_1$ formula and to a $\Pi_1$ formula. Such formulas are absolute between suitable transitive models of finite fragments of ZF.

## Axiom schema of replacement

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_schema_of_replacement)

Every definable function-class maps a set-sized domain to a set-sized range. Functionality means that the defining formula assigns exactly one output to each input in the domain.

### Axiom schema of collection

↑ **Parent:** [Axiom schema of replacement](#axiom-schema-of-replacement)

For each formula, if every member of a domain set has a witness, a set contains witnesses for all those members. It permits extra members and does not require unique witnesses. For [hereditarily countable sets](#hereditarily-countable-set), use ambient [axiom of choice](#axiom-of-choice) to select one internal witness for each member of the countable domain, and use [countable-subset closure](#countable-subset-closure) to keep the resulting witness set internal.

### Full second-order replacement rank obstruction

↑ **Parent:** [Axiom schema of replacement](#axiom-schema-of-replacement)

If $V_\lambda$, for an infinite [cardinal number](#cardinal-number) $\lambda$, satisfies [Axiom schema of replacement](#axiom-schema-of-replacement) for every external functional class, then an external cofinal [function](function.md) from an [ordinal](#ordinal) below $\lambda$ cannot exist: its range would have [rank of a set](#rank-of-a-set) $\lambda$ and would have to belong to $V_\lambda$. Similarly, a [surjection](algebra.md#surjective-function) $\mathcal P(\theta)\to\lambda$ with $\theta<\lambda$ is impossible. Infinity therefore makes $\lambda$ an uncountable [regular cardinal](#regular-cardinal) and a [strong limit cardinal](#strong-limit-cardinal). [Full semantics for second-order logic](mathematical-logic.md#full-semantics-for-second-order-logic), allowing arbitrary external functional relations, is essential.

## Axiom of union

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_union)

For every set $x$, there is a set $u=\bigcup x$ whose elements are exactly the elements of members of $x$:

$$
y\in u\quad\Longleftrightarrow\quad\exists z\in x\ (y\in z).
$$

## Axiom of regularity

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_regularity)

Every nonempty set $A$ has an element $x\in A$ such that $x\cap A=\varnothing$.

### Epsilon induction

↑ **Parent:** [Axiom of regularity](#axiom-of-regularity)

The principle of epsilon induction says that every progressive class is universal: if

$$
\forall x\left[
(\forall y\in x,\ \varphi(y))\Longrightarrow\varphi(x)
\right],
$$

then $\varphi(x)$ holds for every set $x$. Over the other axioms of ZF, it is equivalent to the [Axiom of foundation](#axiom-of-regularity).

#### Epsilon-recursion theorem

↑ **Parent:** [Epsilon induction](#epsilon-induction)

Given a definable operation $G(x,h)$ on a set $x$ and a function $h$ with domain $x$, there is a unique class function $F$ satisfying

$$
F(x)=G(x,F\mathbin{\upharpoonright}x)
$$

for every set $x$. Existence and uniqueness follow by [epsilon induction](#epsilon-induction), because the value at $x$ depends only on values at members of $x$.

## Axiom of power set

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_power_set)

For every set $x$ there is a set $\mathcal P(x)$ whose members are exactly the subsets of $x$.

## Cumulative hierarchy

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cumulative_hierarchy)

The cumulative hierarchy is defined by $V_0=\varnothing$, $V_{\alpha+1}=\mathcal P(V_\alpha)$, and $V_\lambda=\bigcup_{\alpha<\lambda}V_\alpha$ at limit ordinals.

### Transitive closure

↑ **Parent:** [Cumulative hierarchy](#cumulative-hierarchy)

The transitive closure $\operatorname{TC}(x)$ is the least transitive set containing every member of $x$. It is obtained by taking the union of all finite iterates of the union operation starting from $x$. This set-theoretic construction uses the membership [binary relation](#binary-relation); [transitive closure of a relation](#transitive-closure-relation) instead closes an arbitrary [binary relation](#binary-relation) under composition.

#### Transitive closure preserves set-theoretic rank

↑ **Parent:** [Transitive closure](#transitive-closure)

Using the convention that $\operatorname{TC}(x)$ is the least [transitive set](#transitive-set) containing $x$ as a subset, put $x_0=x$, $x_{n+1}=\bigcup x_n$ and $\operatorname{TC}(x)=\bigcup_{n<\omega}x_n$. If $\operatorname{rank}x=\alpha$, every element encountered is an iterated member of an original element and has rank below $\alpha$. Thus the closure has rank at most $\alpha$, while $x\subseteq\operatorname{TC}(x)$ gives the reverse inequality. A convention requiring $x$ itself to be an element instead has rank $\alpha+1$.

#### Hereditarily small set

↑ **Parent:** [Transitive closure](#transitive-closure)

For an infinite [cardinal number](#cardinal-number) $\kappa$, $H_\kappa$ consists of the sets $x$ for which $|\operatorname{tc}(\{x\})|<\kappa$, where $\operatorname{tc}$ is [transitive closure](#transitive-closure). The entire transitive membership ancestry is bounded, not only the size of $x$. These collections are [transitive sets](#transitive-set). At $\kappa=\omega_1$ the elements are the [hereditarily countable sets](#hereditarily-countable-set).

##### Power-set failure in hereditarily small sets

↑ **Parent:** [Hereditarily small set](#hereditarily-small-set)

The [hereditarily small set](#hereditarily-small-set) structure $H_{\omega_2}$ fails the [Axiom of power set](#axiom-of-power-set) at $\omega_1$. Every subset of $\omega_1$ belongs to $H_{\omega_2}$, but their full [power set](set.md#power-set) has [cardinality](#cardinality) at least $\aleph_2$ by the [Cantor theorem](set.md#cantor-s-theorem), so cannot itself be hereditarily smaller than $\aleph_2$.

#### Finite-power-set hereditary-small construction

↑ **Parent:** [Transitive closure](#transitive-closure)

Let $z_0=\omega$ and $z_{n+1}=\mathcal P(z_n)$. Call $x$ small when it injects into some $z_n$, and let $\mathbf{HS}$ contain exactly the sets all of whose hereditary members are small. Then every $z_n$ and the set $y=\{z_n:n\in\omega\}$ belong to $\mathbf{HS}$, but $\bigcup y$ does not. Consequently $(\mathbf{HS},\in)$ fails the [Axiom of union](#axiom-of-union).

#### Hereditarily countable set

↑ **Parent:** [Transitive closure](#transitive-closure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hereditarily_countable_set)

A set is hereditarily countable when its [transitive closure](#transitive-closure) is [countable](#countable-set). These sets form the transitive set $H_{\omega_1}$ and all have rank below $\omega_1$.

##### Axioms satisfied by hereditarily countable sets

↑ **Parent:** [Hereditarily countable set](#hereditarily-countable-set)

The [transitive set](#transitive-set) of [hereditarily countable sets](#hereditarily-countable-set) satisfies every [ZFC](#zermelo-fraenkel-set-theory-with-choice) axiom except the [Axiom of power set](#axiom-of-power-set). For internal definable functions on a countable domain, ambient [Axiom schema of replacement](#axiom-schema-of-replacement) gives a countable range of hereditarily countable sets, which belongs to the structure by [countable-subset closure](#countable-subset-closure). The same closure proves [axiom schema of collection](#axiom-schema-of-collection) and retains countable choice-function graphs. All subsets of $\omega$ are elements, but their uncountable full power set is not an element, so Power Set fails.

##### Countable membership coding

↑ **Parent:** [Hereditarily countable set](#hereditarily-countable-set)

A countable [well-founded relation](#well-founded-relation) that is an [extensional relation](#extensional-relation) codes a transitive set through the [Mostowski collapse theorem](#mostowski-collapse-theorem). Adding a distinguished point selects one decoded set. Every [hereditarily countable set](#hereditarily-countable-set) has such a code by enumerating its transitive membership ancestry. There are only continuum many codes. In [ZFC](#zermelo-fraenkel-set-theory-with-choice), selecting least codes in a well-order gives an injection of the hereditarily countable sets into a set of size $2^{\aleph_0}$.

##### Countable-subset closure

↑ **Parent:** [Hereditarily countable set](#hereditarily-countable-set)

A set has countable-subset closure when every countable subset of it is one of its elements, including the empty subset. In [ZFC](#zermelo-fraenkel-set-theory-with-choice), the [hereditarily countable sets](#hereditarily-countable-set) form the least such set. First realize them as the separated subset of $V_{\omega_1}$ with countable [transitive closure](#transitive-closure). Countable unions show closure; [well-founded induction](#well-founded-induction) proves leastness because each of these sets is a countable collection of earlier members.

##### Reasonable set

↑ **Parent:** [Hereditarily countable set](#hereditarily-countable-set)

A set $x$ is reasonable when every member of $\operatorname{TC}(\{x\})$ is countable. In ZFC this is equivalent to $x$ being [hereditarily countable](#hereditarily-countable-set).

### Hereditarily finite set

↑ **Parent:** [Cumulative hierarchy](#cumulative-hierarchy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hereditarily_finite_set)

The class of hereditarily finite sets is the set

$$
V_\omega=\bigcup_{n<\omega}V_n.
$$

Equivalently, these are the sets with finite transitive closure, or the sets contained in a finite transitive set.

### Finite von Neumann ordinal

↑ **Parent:** [Cumulative hierarchy](#cumulative-hierarchy)

A finite von Neumann ordinal is obtained from $0=\varnothing$ by finitely many applications of the successor operation $S(x)=x\cup\{x\}$. Equivalently, it is an ordinal every nonempty subset of which has a greatest element. This characterization defines the individual natural numbers without quantifying over all inductive sets.

## Axiom schema of specification

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_schema_of_specification)

For each formula $\varphi$, the axiom schema of specification forms the subset

$$
\{z\in x:\varphi(z)\}
$$

of any set $x$. When interpreting the schema inside a class model, the formula must be evaluated internally.

### Restricted set comprehension

↑ **Parent:** [Axiom schema of specification](#axiom-schema-of-specification)

A predicate selects a [subset](set.md#subset) of a previously given [set](set.md) $A$. The [axiom schema of separation](#axiom-schema-of-specification) guarantees this subset for each allowed formula, with parameters. Unlike unrestricted universal set formation, the resulting set has an ambient bound. Attempting to select all sets not containing themselves without that bound leads to [Russell's paradox](#russell-s-paradox).

### Relativized closure criterion for separation

↑ **Parent:** [Axiom schema of specification](#axiom-schema-of-specification)

Let $M$ be a transitive class. If $M$ is closed under the ambient subsets defined by $\varphi^M$, then $M$ satisfies the $\varphi$-instance of separation, because

$$
\{z\in x:V\models\varphi^M(z)\}
=\{z\in x:M\models\varphi(z)\}.
$$

## Axiom of choice

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_choice)

Every family of nonempty sets has a choice function. In ZF this is equivalent to the well-ordering theorem.

### Axiom of global choice

↑ **Parent:** [Axiom of choice](#axiom-of-choice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_global_choice)

A single class [function](function.md) chooses one member of every nonempty [set](set.md). In the usual class theory with [replacement](#axiom-schema-of-replacement), it is equivalent to a set-like global [well-ordering](set.md#well-order) of the universe. Ordinary [choice](#axiom-of-choice) asserts choice only for each set-sized family separately.

### Axiom of countable choice

↑ **Parent:** [Axiom of choice](#axiom-of-choice)

The axiom of countable choice allows one to choose an element from each member of a countable family of nonempty [sets](set.md). It is a restricted form of the [axiom of choice](#axiom-of-choice). In the usual proof that a [countable union of countable sets](#countable-union-of-countable-sets) is countable, it suffices to choose one enumerating [injection](algebra.md#injective-function) for each set; if those enumerations are already supplied, that proof requires no further choice.

#### Countable product compactness implies countable choice

↑ **Parent:** [Axiom of countable choice](#axiom-of-countable-choice)

This concerns arbitrary [compact spaces](topology.md#compact-space), with no [Hausdorff](topology.md#hausdorff-space) restriction. For nonempty sets $A_j$, adjoin a distinguished point $\infty_j$ and use the four-open-set [topology](topology.md) $\{\varnothing,A_j,\{\infty_j\},A_j\cup\{\infty_j\}\}$. Each resulting space is compact without choice. The product has the canonical all-infinity point. The closed coordinate conditions $x_j\in A_j$ have the [finite intersection property](topology.md#finite-intersection-property), since finite choice is provable without the [axiom of choice](#axiom-of-choice). If the countable product is compact, their intersection is nonempty, and any point in it supplies a [choice function](#choice-function).

### Choice function

↑ **Parent:** [Axiom of choice](#axiom-of-choice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Choice_function)

A choice function on a family $\mathcal A$ of nonempty sets is a function $f$ with $f(A)\in A$ for every $A\in\mathcal A$.

### Restricted axiom of choice

↑ **Parent:** [Axiom of choice](#axiom-of-choice)

For sets $X$ and $Y$, $\mathsf{AC}_X(Y)$ says that every $X$-indexed family $(A_x)_{x\in X}$ of nonempty subsets of $Y$ has a [choice function](#choice-function) $c:X\to Y$ satisfying $c(x)\in A_x$.

### Well-ordering theorem

↑ **Parent:** [Axiom of choice](#axiom-of-choice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Well-ordering_theorem)

Every set admits a well-order. In ZF this statement is equivalent to the [axiom of choice](#axiom-of-choice).

#### Choice-function well-ordering construction

↑ **Parent:** [Well-ordering theorem](#well-ordering-theorem)

Given a choice function on all nonempty subsets of $X$, recursively choose the next point from the complement of all earlier choices. [Hartogs theorem](#hartogs-theorem) forces the recursion to exhaust $X$ before it defines an injection from $h(X)$ into $X$, producing a bijection from an ordinal to $X$.

### Cardinal comparability principle

↑ **Parent:** [Axiom of choice](#axiom-of-choice)

For any sets $X,Y$, either $X$ injects into $Y$ or $Y$ injects into $X$. Applying this to $X$ and its Hartogs ordinal proves the [well-ordering theorem](#well-ordering-theorem), so over ZF cardinal comparability is equivalent to choice.

## Hartogs theorem

↑ **Parent:** [Set theory](set-theory.md)

For every set $X$ there is a least ordinal $h(X)$ that does not inject into $X$.

The least ordinal supplied by the theorem is the [Hartogs number](#hartogs-number).

### Hartogs number

↑ **Parent:** [Hartogs theorem](#hartogs-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hartogs_number)

The least [ordinal](#ordinal) that does not admit an [injection](algebra.md#injective-function) into $X$. Its existence, supplied by [Hartogs theorem](#hartogs-theorem), does not require the [axiom of choice](#axiom-of-choice).

#### Hartogs numbers under choice

↑ **Parent:** [Hartogs number](#hartogs-number)

For infinite [sets](set.md) in [ZFC](#zermelo-fraenkel-set-theory-with-choice), the [Hartogs number](#hartogs-number) is the successor of the input cardinal. Every smaller ordinal injects into the input, whereas that successor does not. An infinite [successor cardinal](#successor-cardinal) $\kappa^+$ is regular: a cofinal family of at most $\kappa$ ordinals below it would have union of cardinal at most $\kappa\cdot\kappa=\kappa$, a contradiction. Finite inputs give finite successor cardinals, so the formulation in terms of alephs requires an infinite input. The general [Hartogs theorem](#hartogs-theorem) itself does not require [choice](#axiom-of-choice).

## Tarski cardinal-square theorem

↑ **Parent:** [Set theory](set-theory.md)

In ZF, if $X\times X\cong X$ for every infinite $X$, apply this to $X\sqcup h(X)$. The [product-sum comparison lemma](#product-sum-comparison-lemma) applied to $X$ and its Hartogs ordinal gives either an impossible injection $h(X)\to X$ or a surjection $h(X)\to X$. In the latter case, ordering each $x\in X$ by its least ordinal preimage well-orders $X$. The converse is the well-orderable-cardinal identity $\kappa^2=\kappa$.

## Image and preimage of a function

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Image_and_preimage_of_a_function)

Images send subsets of a domain forward through a function, while preimages pull subsets of the codomain back.

### Image of a function

↑ **Parent:** [Image and preimage of a function](#image-and-preimage-of-a-function)

For a [function](function.md) $f:X\to Y$, its image is $f(X)=\{f(x):x\in X\}$.

### Preimage

↑ **Parent:** [Image and preimage of a function](#image-and-preimage-of-a-function)

For a [function](function.md) $f:X\to Y$ and a [subset](set.md#subset) $B\subseteq Y$, the preimage $f^{-1}(B)$ consists of points of $X$ mapped into $B$. This notation does not require $f$ to have an [inverse function](function.md#inverse-function). Preimages preserve [unions](set.md#set-union), [intersections](set.md#set-intersection) and complements, which makes them useful in defining [continuous functions](calculus.md#continuous-function) and [measurable functions](measure-theory.md#measurable-function).

## Cartesian product

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartesian_product)

The Cartesian product $X\times Y$ is the set of ordered pairs $(x,y)$ with $x\in X$ and $y\in Y$.

### Affine section of a planar set

↑ **Parent:** [Cartesian product](#cartesian-product)

For $A\subseteq\mathbb R^2$ and a nonzero direction $\mathbf b$, its affine section is the inverse image of $A$ under the line parametrization $t\mapsto\mathbf a+t\mathbf b$. The resulting set is a subset of the parameter line, so changing a parametrization can change the section by translation or scaling. The four real parameters can be encoded by a single real using [real-number pairing by separated digits](algebra.md#real-number-pairing-by-separated-digits). Thus no fixed planar set can realize every real subset as a section, by [Cantor's theorem](set.md#cantor-s-theorem).

#### Universal planar set for countable real sections

↑ **Parent:** [Affine section of a planar set](#affine-section-of-a-planar-set)

Use [coding of real sequences by ternary digits](algebra.md#coding-of-real-sequences-by-ternary-digits) to give each real sequence a distinct column coordinate $c(s)\in[0,1/2]$. Put every term of that sequence in its column. The vertical [affine section of a planar set](#affine-section-of-a-planar-set) at $c(s)$ is exactly the sequence range. Every nonempty [countable set](#countable-set) has such an enumeration, with repetitions allowed, while any column outside the code interval gives the empty set. This realizes every countable real subset; the other sections are unrestricted.

### Universal property of Cartesian products

↑ **Parent:** [Cartesian product](#cartesian-product)

Given [functions](function.md) $f_i:Y\to X_i$, there is a unique [function](function.md) $g:Y\to X_1\times X_2$ whose coordinate [projection maps](function.md#projection-map) are $f_1,f_2$. It is the displayed pointwise pairing. Equality of ordered pairs is equality of both coordinates, which proves uniqueness and makes the [Cartesian product](#cartesian-product) a categorical product in the [Category of sets](category.md#category-of-sets).

#### Joint injectivity of a pair of functions

↑ **Parent:** [Universal property of Cartesian products](#universal-property-of-cartesian-products)

The [pairing map to a Cartesian product](#universal-property-of-cartesian-products) is [injective](algebra.md#injective-function) exactly when its coordinate [functions](function.md) are jointly injective in the displayed sense. Either coordinate being [injective](algebra.md#injective-function) is sufficient, but neither need be [injective](algebra.md#injective-function) individually. For example, pairing three points with $(0,0),(0,1),(1,0)$ distinguishes all points even though each coordinate separately identifies two of them.

### Finite tuple

↑ **Parent:** [Cartesian product](#cartesian-product)

A finite [tuple](#finite-tuple) is an ordered list of finitely many entries; coordinates can repeat, and their positions matter. A [tuple](#finite-tuple) of length $n$ from a set $M$ is an element of the [Cartesian product](#cartesian-product) $M^n$. The empty [tuple](#finite-tuple) has length zero. Finite [tuples](#finite-tuple) support [Scott formulas](mathematical-logic.md#scott-formula) in a [back-and-forth method](foundations-of-mathematics.md#back-and-forth-method) construction, where matching [tuples](#finite-tuple) determine a [partial isomorphism of structures](foundations-of-mathematics.md#partial-embedding).

## Disjoint union

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disjoint_union)

The disjoint union tags the elements of its summands, for example $X\sqcup Y=(X\times\{0\})\cup(Y\times\{1\})$.

## Fiber product of sets

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fiber_product_of_sets)

The fiber product of maps f:A to B and g:A-prime to B consists of pairs with equal images in B.

## Cantor diagonal argument

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor_diagonal_argument)

Cantor’s diagonal argument constructs an object differing from the nth listed object in its nth coordinate, proving no proposed enumeration is complete.

## Elementary embedding

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elementary_embedding)

An elementary embedding preserves every first-order formula with parameters from its domain. Its critical point $\operatorname{crit}(j)$ is the least ordinal moved by a nonidentity embedding.

### Elementarity

↑ **Parent:** [Elementary embedding](#elementary-embedding)

Preservation of all [first-order formulas](mathematical-logic.md#first-order-formula) with parameters by an embedding. For an inclusion of structures this is the condition for an [elementary substructure](mathematical-logic.md#elementary-substructure).

### Kunen inconsistency theorem

↑ **Parent:** [Elementary embedding](#elementary-embedding)

In [ZFC](#zermelo-fraenkel-set-theory-with-choice) there is no nonidentity [elementary embedding](#elementary-embedding) $j:V\to V$, understood as an ordinary class embedding whose set restrictions and critical sequence are available. Let $\lambda$ be the supremum of the [Kunen critical sequence](#kunen-critical-sequence), so $j(\lambda)=\lambda$ and $j(\lambda^+)=\lambda^+$. Partition the ordinals of cofinality $\omega$ below $\lambda^+$ into stationary sets indexed by the critical point. After applying $j$, the extra stationary cell at that critical point meets the club of ordinals closed under $j$. Such an ordinal of countable cofinality is fixed by $j$ and hence belongs both to that extra cell and an old-index cell, a contradiction.

### Critical point of an elementary embedding

↑ **Parent:** [Elementary embedding](#elementary-embedding)

If $\kappa=\operatorname{crit}(j)$, then $j$ fixes every member of $V_\kappa$ and every ordinal below $\kappa$, while $j(\kappa)>\kappa$.

### Ultrapower embedding

↑ **Parent:** [Elementary embedding](#elementary-embedding)

An ultrafilter $U$ on $I$ gives an elementary map into the well-founded collapse of an ultrapower by sending $x$ to the class of the constant function with value $x$. For a $\kappa$-complete nonprincipal ultrafilter on $\kappa$, its critical point is $\kappa$.

### Beta-strong elementary embedding

↑ **Parent:** [Elementary embedding](#elementary-embedding)

For inaccessible $\lambda$, a map $j:V_\lambda\to M$ with critical point $\kappa$ is $\beta$-strong when $M$ is transitive and $V_{\kappa+\beta}\subseteq M$.

#### One-strong cardinal

↑ **Parent:** [Beta-strong elementary embedding](#beta-strong-elementary-embedding)

A cardinal $\kappa<\lambda$ is 1-strong when it is the [critical point of an elementary embedding](#critical-point-of-an-elementary-embedding) $j:V_\lambda\to M$ into a transitive model satisfying $V_{\kappa+1}\subseteq M$.

#### Beta-stable cardinal property

↑ **Parent:** [Beta-strong elementary embedding](#beta-strong-elementary-embedding)

A formula $\Phi(x,\kappa)$ defines a $\beta$-stable property of $\kappa$ when it is absolute between the universe and every transitive $M\supseteq V_{\kappa+\beta}$.

##### Reflection by a beta-strong embedding

↑ **Parent:** [Beta-stable cardinal property](#beta-stable-cardinal-property)

If a $\beta$-strong embedding has critical point $\kappa$ and the $\beta$-stable property $\Phi(\kappa)$ holds, then $\{\mu<\kappa:\Phi(\mu)\}$ is unbounded in $\kappa$. For each $\gamma<\kappa$, the target sees $\kappa$ as a witness between $\gamma$ and $j(\kappa)$; elementarity reflects a witness between $\gamma$ and $\kappa$.

###### Reflection below a cardinal

↑ **Parent:** [Reflection by a beta-strong embedding](#reflection-by-a-beta-strong-embedding)

A property $P$ reflects below a cardinal $\kappa$ when $\{\mu<\kappa:P(\mu)\}$ is unbounded in $\kappa$. For an [elementary embedding](#elementary-embedding) with [critical point](#critical-point-of-an-elementary-embedding) $\kappa$, one often proves this by using $\kappa$ as a witness below $j(\kappa)$ in the target and then invoking elementarity.

### Kunen critical sequence

↑ **Parent:** [Elementary embedding](#elementary-embedding)

The critical sequence of $j$ starts with its critical point $\kappa$ and iterates $\kappa_{n+1}=j(\kappa_n)$. Its supremum $\widehat\kappa=\sup_{n<\omega}j^n(\kappa)$ is the least fixed point of $j$ above $\kappa$ whenever the relevant iterates lie in the domain.

#### Kunen lemma

↑ **Parent:** [Kunen critical sequence](#kunen-critical-sequence)

For an elementary embedding with critical-sequence supremum $\widehat\kappa$, the set

$$
j\mathbin{``}\widehat\kappa=\{j(\xi):\xi<\widehat\kappa\}
$$

does not belong to the transitive target model. The proof uses an omega-Jonsson function on $\widehat\kappa$.

## Cardinal number

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardinal_number)

In the presence of choice, a cardinal number may be represented by the least ordinal in its bijection class.

### Limit cardinal

↑ **Parent:** [Cardinal number](#cardinal-number)

An infinite [cardinal number](#cardinal-number) is a limit cardinal if it is not a [successor cardinal](#successor-cardinal); equivalently it is an [aleph number](#aleph-number) with zero or a [limit ordinal](#limit-ordinal) as index. Uncountable limit cardinals are either [singular cardinals](#singular-cardinal) or [weakly inaccessible cardinals](#weakly-inaccessible-cardinal). This concerns succession among cardinals, rather than merely being a [limit ordinal](#limit-ordinal).

### Cardinality

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardinality)

The cardinality $|X|$ of a [set](set.md) $X$ is the [cardinal number](#cardinal-number) shared by all sets in [bijection](function.md#bijection) with $X$. For a [finite set](set.md#finite-set), it is the number of elements.

### Successor cardinal

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successor_cardinal)

The successor cardinal $\kappa^+$ is the least [cardinal number](#cardinal-number) strictly larger than $\kappa$.

### Cofinality

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cofinality)

The cofinality of an ordinal $\alpha$ is the least [order type](#order-type) of an unbounded subset of $\alpha$, equivalently the least ordinal $\beta$ admitting a cofinal function $\beta\to\alpha$.

#### Cofinality of a continuous cardinal hierarchy

↑ **Parent:** [Cofinality](#cofinality)

At a nonzero [limit ordinal](#limit-ordinal) $\delta$, a strictly increasing continuous sequence of [cardinals](#cardinal-number) $(\kappa_\alpha)_{\alpha\le\delta}$ satisfies $\operatorname{cf}(\kappa_\delta)=\operatorname{cf}(\delta)$. A cofinal sequence of indices gives the upper bound. Conversely, bounds for a cofinal [set](set.md) of values must have cofinal indices, giving the lower bound. In particular the assertion applies to [Beth numbers](#beth-number).

#### Cofinal map

↑ **Parent:** [Cofinality](#cofinality)

A map $f:\delta\to\alpha$ whose range is cofinal: every $\xi<\alpha$ lies below or equals some $f(\eta)$. It need not be increasing.

#### Cofinality of an increasing ordinal supremum

↑ **Parent:** [Cofinality](#cofinality)

If $\alpha$ is a nonzero [limit ordinal](#limit-ordinal) and $(\gamma_\xi)_{\xi<\alpha}$ is strictly increasing, then $\operatorname{cf}(\sup_{\xi<\alpha}\gamma_\xi)=\operatorname{cf}(\alpha)$. A cofinal subsequence of the index order gives one inequality. Conversely, a cofinal family in the supremum determines a cofinal family of indices by choosing an index past each of its values. This also explains the [cofinality](#cofinality) of limit-indexed [aleph numbers](#aleph-number).

#### Singular cardinal

↑ **Parent:** [Cofinality](#cofinality)

An infinite [cardinal number](#cardinal-number) $\kappa$ is singular when $\operatorname{cf}(\kappa)<\kappa$. Thus a short [cofinal function](#cofinal-function) reaches arbitrarily high ordinals below $\kappa$. For example, $\aleph_\omega$ has [cofinality](#cofinality) $\omega$. The complementary case is a [regular cardinal](#regular-cardinal).

<h5 id="bukovsky-hechler-theorem">Bukovský-Hechler theorem</h5>

↑ **Parent:** [Singular cardinal](#singular-cardinal)

If the power-set [function](function.md) is eventually constant below a [singular cardinal](#singular-cardinal) $\kappa$, its constant value persists at $\kappa$. Writing $\theta=\operatorname{cf}(\kappa)$ gives $2^\kappa=(2^{<\kappa})^\theta$. On the plateau choose a [cardinal](#cardinal-number) $\mu\ge\theta$, so $(2^\mu)^\theta=2^{\mu\cdot\theta}=2^\mu$.

##### Singular cardinal enumeration

↑ **Parent:** [Singular cardinal](#singular-cardinal)

Write $\sigma_\alpha$ for the $\alpha$th uncountable [singular cardinal](#singular-cardinal) in increasing order. It begins with $\sigma_0=\aleph_\omega$ and $\sigma_1=\aleph_{\omega+\omega}$. At a nonzero [limit ordinal](#limit-ordinal) index it is continuous exactly when the supremum of its earlier values is singular. It can jump when that supremum is a [weakly inaccessible cardinal](#weakly-inaccessible-cardinal). The first member of uncountable [cofinality](#cofinality) occurs at index $\omega_1$, with value $\aleph_{\omega_1}$.

###### Cardinal fixed point of the singular cardinal enumeration

↑ **Parent:** [Singular cardinal enumeration](#singular-cardinal-enumeration)

There is an uncountable [cardinal number](#cardinal-number) $\kappa$ with $\sigma_\kappa=\kappa$. Iterate $\kappa_{n+1}=\sigma_{\kappa_n}$ starting with $\aleph_0$. If there is no earlier fixed point, the increasing supremum $\kappa$ has countable [cofinality](#cofinality), hence is a [singular cardinal](#singular-cardinal). The [singular cardinal enumeration](#singular-cardinal-enumeration) is cofinal in $\kappa$ below index $\kappa$, and continuity at this singular supremum gives equality.

##### Singular cardinals hypothesis

↑ **Parent:** [Singular cardinal](#singular-cardinal)

The singular cardinals hypothesis asserts that every infinite [singular cardinal](#singular-cardinal) $\kappa$ satisfies

$$
2^{\operatorname{cf}(\kappa)}<\kappa\ \Longrightarrow\ \gimel(\kappa)=\kappa^+.
$$

Equivalently, $\gimel(\kappa)=\max\{\kappa^+,2^{\operatorname{cf}(\kappa)}\}$ for every infinite [singular cardinal](#singular-cardinal). Here $\gimel$ is the [gimel function](#gimel-function). The [Generalized continuum hypothesis](#generalized-continuum-hypothesis) implies this principle, but the principle only constrains the indicated singular-cardinal exponentiation.

#### Cofinal function

↑ **Parent:** [Cofinality](#cofinality)

A function $f:\beta\to\alpha$ between ordinals is cofinal when its range is unbounded in $\alpha$: for every $\gamma<\alpha$ some $\xi<\beta$ satisfies $\gamma\leq f(\xi)$.

#### Regular cardinal

↑ **Parent:** [Cofinality](#cofinality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regular_cardinal)

An infinite cardinal $\kappa$ is regular when its cofinality is $\kappa$.

### Large cardinal

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Large_cardinal)

A large cardinal property strengthens uncountability by imposing combinatorial, logical, measure-like, or elementary-embedding structure whose existence is not provable in ZFC if ZFC is consistent.

#### Supercompact cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supercompact_cardinal)

A [cardinal](#cardinal-number) $\kappa$ is supercompact if for every cardinal $\lambda\geq\kappa$ there is an [elementary embedding](#elementary-embedding) $j:V\to M$ into a transitive class with [critical point of an elementary embedding](#critical-point-of-an-elementary-embedding) $\kappa$, $j(\kappa)>\lambda$, and $M^\lambda\subseteq M$. This closure supplies every sufficiently small rank segment needed to transfer existential witnesses into $M$.

##### Supercompact Sigma-two downward reflection

↑ **Parent:** [Supercompact cardinal](#supercompact-cardinal)

If $\kappa$ is a [supercompact cardinal](#supercompact-cardinal), each true $\Sigma_2$ statement, allowing parameters in $V_\kappa$, holds in $V_\kappa$. Write it as an existential witness followed by a $\Pi_1$ assertion. Choose a supercompact [elementary embedding](#elementary-embedding) whose transitive target contains the witness in $V_{j(\kappa)}$. Downward absoluteness of the universal bounded-matrix assertion puts the witness in that rank segment, and elementarity reflects this to $V_\kappa$.

#### Mahlo cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)

An inaccessible cardinal $\kappa$ whose inaccessible ordinals below it form a stationary set. Equivalently, every predicate expansion of $V_\kappa$ has an inaccessible elementary rank level below $\kappa$.

##### Mahloness is downward absolute to the constructible universe

↑ **Parent:** [Mahlo cardinal](#mahlo-cardinal)

If $\kappa$ is Mahlo in $V$, then it is Mahlo in $L$. Inaccessibility is downward absolute, and every club in $L$ remains a club in $V$, where it meets a $V$-inaccessible ordinal.

#### Weakly inaccessible cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)

A weakly inaccessible cardinal is an uncountable [regular cardinal](#regular-cardinal) that is a [limit cardinal](#limit-cardinal). It need not be a [strong limit cardinal](#strong-limit-cardinal). Under the [Generalized continuum hypothesis](#generalized-continuum-hypothesis), it is a [strongly inaccessible cardinal](#strongly-inaccessible-cardinal), since every smaller infinite $\lambda$ satisfies $2^\lambda=\lambda^+<\kappa$.

##### Weakly Mahlo cardinal

↑ **Parent:** [Weakly inaccessible cardinal](#weakly-inaccessible-cardinal)

A [weakly inaccessible cardinal](#weakly-inaccessible-cardinal) $\kappa$ is weakly Mahlo if $\{\alpha<\kappa:\alpha=\operatorname{cf}(\alpha)\}$ is a [stationary set](#stationary-set). Intersecting this set with the [club set](#club-set) of uncountable [limit cardinals](#limit-cardinal) shows that the weakly inaccessible cardinals below $\kappa$ are stationary, hence unbounded.

##### Model of ZFC without weakly inaccessible cardinals

↑ **Parent:** [Weakly inaccessible cardinal](#weakly-inaccessible-cardinal)

Consistency of [ZFC](#zermelo-fraenkel-set-theory-with-choice) implies consistency of [ZFC](#zermelo-fraenkel-set-theory-with-choice) with the [Generalized continuum hypothesis](#generalized-continuum-hypothesis) and no [weakly inaccessible cardinals](#weakly-inaccessible-cardinal). Pass to the [constructible universe](definable-power-set.md#constructible-universe). If it has an inaccessible, cut at its least one; that rank segment still models [ZFC](#zermelo-fraenkel-set-theory-with-choice) and the [Generalized continuum hypothesis](#generalized-continuum-hypothesis), but has no inaccessibles. In this model the [singular cardinal enumeration](#singular-cardinal-enumeration) is continuous at every nonzero [limit ordinal](#limit-ordinal) index. This is a relative-consistency construction, not a deduction of a [transitive model](#transitive-model) from bare consistency.

#### Strong limit cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_limit_cardinal)

A cardinal $\kappa$ is a strong limit when $2^\lambda<\kappa$ for every cardinal $\lambda<\kappa$.

##### Singular strong limit power-set identity

↑ **Parent:** [Strong limit cardinal](#strong-limit-cardinal)

For a singular [strong limit cardinal](#strong-limit-cardinal) $\lambda$, let $\mu=\operatorname{cf}(\lambda)$ and choose cofinal cardinals $\lambda_i<\lambda$. Subset restrictions inject $\mathcal P(\lambda)$ into $\prod_{i<\mu}\mathcal P(\lambda_i)$, whose cardinal is at most $\lambda^\mu$ by the strong-limit property. Conversely $\lambda^\mu\le(2^\lambda)^\mu=2^\lambda$. This equality alone does not imply the [singular cardinals hypothesis](#singular-cardinals-hypothesis).

#### Strongly inaccessible cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)

A strongly inaccessible cardinal is an uncountable regular strong limit cardinal.

##### Inaccessible limit of inaccessibles

↑ **Parent:** [Strongly inaccessible cardinal](#strongly-inaccessible-cardinal)

An [inaccessible cardinal](#strongly-inaccessible-cardinal) $\iota$ is an inaccessible limit of inaccessibles if the inaccessible cardinals below it are unbounded in $\iota$. A [rank cutoff at the first inaccessible limit of inaccessibles](#rank-cutoff-at-the-first-inaccessible-limit-of-inaccessibles) shows that existence of unboundedly many inaccessibles does not prove existence of such a limit, provided the former theory is consistent.

###### Rank cutoff at the first inaccessible limit of inaccessibles

↑ **Parent:** [Inaccessible limit of inaccessibles](#inaccessible-limit-of-inaccessibles)

If $\iota$ is the least [inaccessible limit of inaccessibles](#inaccessible-limit-of-inaccessibles), $V_\iota$ models [ZFC](#zermelo-fraenkel-set-theory-with-choice) and internally has unboundedly many [inaccessible cardinals](#strongly-inaccessible-cardinal), while none of its ordinals is an [inaccessible limit of inaccessibles](#inaccessible-limit-of-inaccessibles). Rank agreement makes inaccessibility below $\iota$ absolute. If a model of unboundedly many inaccessibles has no such limit in the first place, no cutoff is needed. This proves the corresponding relative-consistency nonimplication.

##### Keisler extension property

↑ **Parent:** [Strongly inaccessible cardinal](#strongly-inaccessible-cardinal)

An inaccessible cardinal $\kappa$ has the Keisler extension property when there is a proper [transitive set](#transitive-set) $X\supsetneq V_\kappa$ for which

$$
(V_\kappa,\in)\prec(X,\in).
$$

Such a $\kappa$ is not the least inaccessible cardinal: $X$ regards $\kappa$ as inaccessible, [elementarity](mathematical-logic.md#elementary-substructure) reflects the existence of an inaccessible into $V_\kappa$, and [strong-inaccessibility absoluteness from rank agreement](#strong-inaccessibility-absoluteness-from-rank-agreement) makes the resulting witness genuinely inaccessible below $\kappa$.

#### Worldly cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Worldly_cardinal)

A cardinal $\kappa$ is worldly when $V_\kappa\models\mathrm{ZFC}$. Every [strongly inaccessible cardinal](#strongly-inaccessible-cardinal) is worldly, but worldly cardinals can be singular.

##### Worldly cardinals below an inaccessible cardinal

↑ **Parent:** [Worldly cardinal](#worldly-cardinal)

Below any uncountable [strongly inaccessible cardinal](#strongly-inaccessible-cardinal) $\kappa$, the [worldly cardinals](#worldly-cardinal) contain a [closed unbounded subset](#club-set) of $\kappa$ and hence have [cardinality](#cardinality) $\kappa$. The structure $V_\kappa$ models [ZFC](#zermelo-fraenkel-set-theory-with-choice). Reflect each finite group from an enumeration of all [first-order formulas](mathematical-logic.md#first-order-formula) to a [closed unbounded subset](#club-set) of $\kappa$, using $|V_\alpha|<\kappa$ and regularity for the witness bounds. The countable intersection remains [closed unbounded](#club-set), so its ranks are [elementary substructures](mathematical-logic.md#elementary-substructure) of $V_\kappa$. Intersect with the [closed unbounded subset](#club-set) of infinite [cardinal numbers](#cardinal-number) below $\kappa$. Uncountability is essential: the regular strong limit $\omega$ has no [worldly cardinal](#worldly-cardinal) below it.

##### Nested transitive models from a worldly cardinal

↑ **Parent:** [Worldly cardinal](#worldly-cardinal)

A [worldly cardinal](#worldly-cardinal) permits a [countable transitive model](forcing.md#countable-transitive-model) $M$ of [ZFC](#zermelo-fraenkel-set-theory-with-choice) and a [transitive model](#transitive-model) $N$ of [ZFC](#zermelo-fraenkel-set-theory-with-choice) with $M\in N$, $|N|=\aleph_1$, and $(\omega_1)^N=\omega_1$. First collapse a countable [elementary substructure](mathematical-logic.md#elementary-substructure) of $V_\kappa$. Then collapse an $\aleph_1$-sized [Skolem hull](mathematical-logic.md#skolem-hull) containing every countable ordinal and every member of $M$, as well as $M$ itself. The [transitive collapse fixes transitive subsets](#transitive-collapse-fixes-transitive-subsets) lemma preserves $M$ and those ordinals.

##### Arithmetic absoluteness for a rank-initial model

↑ **Parent:** [Worldly cardinal](#worldly-cardinal)

If $V_\kappa\models\mathrm{ZFC}$, it has the standard natural numbers and standard finite proofs. Every arithmetical sentence, including a [formal consistency statement](mathematical-logic.md#formal-consistency-statement), therefore has the same truth value in $V_\kappa$ and the universe.

#### Kappa-satisfiable theory

↑ **Parent:** [Large cardinal](#large-cardinal)

A theory is $\kappa$-satisfiable when each of its subtheories of cardinality less than $\kappa$ has a model.

#### Least-occurrence order on cardinal properties

↑ **Parent:** [Large cardinal](#large-cardinal)

For cardinal properties $\Phi$ and $\Psi$ that occur, let $\iota_\Phi$ and $\iota_\Psi$ be their least witnesses. Define $\Phi<_1\Psi$ when

$$
\mathrm{ZFC}+\Phi\mathbf C+\Psi\mathbf C\vdash\iota_\Phi<\iota_\Psi.
$$

This relation need not be transitive, because the two implications can be proved under different joint existence assumptions.

##### Nontransitivity of the least-occurrence order on cardinal properties

↑ **Parent:** [Least-occurrence order on cardinal properties](#least-occurrence-order-on-cardinal-properties)

Let $I,W,M$ mean inaccessible, weakly compact, and measurable, and define

$$
\Theta(\kappa)\iff
(W\mathbf C\land M(\kappa))\lor(\neg W\mathbf C\land I(\kappa)).
$$

Then $I<_1W$ and $W<_1\Theta$. Subject to the consistency of an inaccessible without a weakly compact cardinal, there is also a model in which $\Theta=I$, so $I\not<_1\Theta$.

#### Weakly compact cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weakly_compact_cardinal)

An uncountable cardinal $\kappa$ is weakly compact when every $\kappa$-satisfiable theory in an $L_{\kappa,\kappa}$ language having at most $\kappa$ nonlogical symbols is satisfiable.

#### Measurable cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurable_cardinal)

An uncountable cardinal $\kappa$ is measurable when it carries a nonprincipal $\kappa$-complete ultrafilter.

##### Omega-measurable cardinal

↑ **Parent:** [Measurable cardinal](#measurable-cardinal)

A cardinal is omega-measurable if it carries a [countably complete ultrafilter](#countably-complete-ultrafilter) that is a [nonprincipal ultrafilter](#nonprincipal-ultrafilter). Countable completeness rules out countable underlying sets. Such a measure is weaker than the cardinal's own full completeness requirement, but the [least omega-measurable cardinal is measurable](#least-omega-measurable-cardinal-is-measurable).

###### Least omega-measurable cardinal is measurable

↑ **Parent:** [Omega-measurable cardinal](#omega-measurable-cardinal)

If $\kappa$ is the least [omega-measurable cardinal](#omega-measurable-cardinal) and $U$ witnesses it, failure of $\kappa$-completeness partitions a member of $U$ into fewer than $\kappa$ fibres, none belonging to $U$. The [pushforward ultrafilter](#pushforward-ultrafilter) under the fibre-index map is then a nonprincipal countably complete measure on a smaller cardinal, a contradiction. Thus $U$ is $\kappa$-complete and $\kappa$ is a [measurable cardinal](#measurable-cardinal).

##### Measurable cardinal is a strong limit cardinal

↑ **Parent:** [Measurable cardinal](#measurable-cardinal)

Let $U$ be a nonprincipal $\kappa$-complete ultrafilter on $\kappa$. If $\lambda<\kappa$ and $(A_\alpha)_{\alpha<\kappa}$ were distinct subsets of $\lambda$, then for every $\xi<\lambda$ choose the $U$-large side of the partition according to whether $\xi\in A_\alpha$. Their intersection is $U$-large by $\kappa$-completeness, but all its indices label the same subset of $\lambda$, so it has at most one member, contradicting nonprincipality. Thus $2^\lambda<\kappa$.

##### Measurable cardinal is one-strong

↑ **Parent:** [Measurable cardinal](#measurable-cardinal)

The [ultrapower embedding](#ultrapower-embedding) $j:V_\lambda\to M$ associated with a measure on $\kappa<\lambda$ has critical point $\kappa$. For every $A\in V_{\kappa+1}$,

$$
A=j(A)\cap V_\kappa,
$$

so $V_{\kappa+1}\subseteq M$. Hence every measurable cardinal is [1-strong](#one-strong-cardinal).

##### Two measurable cardinals under an ultrapower embedding

↑ **Parent:** [Measurable cardinal](#measurable-cardinal)

Let $\kappa_0<\kappa_1<\lambda$, where both $\kappa_i$ are measurable and $\lambda$ is inaccessible, and let $j_i:V_\lambda\to M_i$ be ultrapower embeddings by measures on $\kappa_i$. Then

$$
j_0(\kappa_1)=\kappa_1,
\qquad
j_1(\kappa_0)=\kappa_0.
$$

The second equality follows from the critical point. For the first, regularity gives continuity of $j_0$ at $\kappa_1$, while strong-limitness bounds $j_0(\beta)<\kappa_1$ for every $\beta<\kappa_1$.

##### Moved critical point is not an ambient cardinal under GCH

↑ **Parent:** [Measurable cardinal](#measurable-cardinal)

For a measure ultrapower $j:V_\lambda\to M$ with critical point $\kappa$, there are at most $2^\kappa$ equivalence classes of functions $\kappa\to\kappa$, so $|j(\kappa)|\leq2^\kappa$ in $V_\lambda$. The target $M$ regards $j(\kappa)$ as measurable and contains $V_{\kappa+1}$, so it sees $(2^\kappa)^M<j(\kappa)$. Under the [Generalized continuum hypothesis](#generalized-continuum-hypothesis), this places $j(\kappa)$ strictly above the ambient $\kappa^+$ while its ambient cardinality is at most $\kappa^+$; hence it is not an ambient cardinal.

#### Strongly compact cardinal

↑ **Parent:** [Large cardinal](#large-cardinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strongly_compact_cardinal)

An uncountable cardinal $\kappa$ is strongly compact when every $\kappa$-satisfiable theory in any $L_{\kappa,\kappa}$ language is satisfiable, with no bound on the number of nonlogical symbols.

### Countable set

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Countable_set)

A countable set is a [set](set.md) that admits an [injective function](algebra.md#injective-function) into the [natural numbers](arithmetic.md#natural-number). It is therefore either a [finite set](set.md#finite-set) or a [countably infinite set](#countably-infinite-set).

#### Countability of disjoint positive-length intervals

↑ **Parent:** [Countable set](#countable-set)

A family of pairwise disjoint real intervals of positive length is [countable](#countable-set). Each interval contains a [rational number](number-theory.md#rational-number) in its interior by the [density of the rational numbers](number-theory.md#density-of-the-rational-numbers). Fix an enumeration of the [rational numbers](number-theory.md#rational-number) and select the first member lying inside each interval. Disjointness makes this selection an [injection](algebra.md#injective-function) into a [countable set](#countable-set). The argument also applies to disjoint nonempty open subsets of the real line.

#### Countability of finite subsets of a countable set

↑ **Parent:** [Countable set](#countable-set)

A finite [subset](set.md#subset) $A$ of the [natural numbers](arithmetic.md#natural-number), numbered from one, has the binary code $\sum_{j\in A}2^{j-1}$. Distinct finite [subsets](set.md#subset) give distinct codes, because the largest differing exponent exceeds the sum of all smaller powers of two. Thus the finite [subsets](set.md#subset) form a [countable set](#countable-set), although the entire [power set](set.md#power-set) is an [uncountable set](#uncountable-set) by the [Cantor diagonal argument](#cantor-diagonal-argument). An enumeration transfers this coding to any [countable set](#countable-set).

#### Cardinalities of monotone natural-number functions

↑ **Parent:** [Countable set](#countable-set)

[Nondecreasing functions](calculus.md#nondecreasing-function) $\mathbb N\to\mathbb N$ form an uncountable set: every subset $A$ is encoded by the strictly increasing function $n+\sum_{k=1}^{n}\mathbf1_A(k)$. In contrast, [nonincreasing functions](calculus.md#nonincreasing-function) form a countable set because each is determined by a finite initial segment and its eventual constant value.

// Target: classical-mechanics.bigb

#### Countability of integer polynomial rings

↑ **Parent:** [Countable set](#countable-set)

For every fixed positive integer $d$, the [polynomial ring](commutative-algebra.md#polynomial-ring) with integer coefficients in $d$ indeterminates is countably infinite. Polynomials of bounded total degree have only finitely many possible monomials, so they are encoded by a finite Cartesian power of the [integers](number-theory.md#integer). Taking a [countable union of countable sets](#countable-union-of-countable-sets) over degree bounds proves countability; constant polynomials supply an infinite subset. Nonzero one-variable polynomials have finitely many real roots, so the real [algebraic numbers](algebra.md#algebraic-number) form a countable set as well.

#### Countable closure under real polynomial roots

↑ **Parent:** [Countable set](#countable-set)

Every [countable set](#countable-set) $B$ of [real numbers](arithmetic.md#real-number) is contained in a [countable set](#countable-set) closed under taking all real [roots of a polynomial](polynomial.md#root-of-a-polynomial) with coefficients in that set. Let $\phi(A)$ consist of these [roots of a polynomial](polynomial.md#root-of-a-polynomial), excluding the zero [polynomial](polynomial.md). There are countably many finite coefficient lists over a [countable set](#countable-set), and each nonzero [polynomial](polynomial.md) has finitely many [roots of a polynomial](polynomial.md#root-of-a-polynomial); hence $\phi(A)$ is countable. Define $B_0=B$ and $B_{n+1}=B_n\cup\phi(B_n)$. The [countable union of countable sets](#countable-union-of-countable-sets) theorem shows that $X=\bigcup_nB_n$ is countable. Every finite coefficient list in $X$ belongs to one stage $B_N$, so its real [roots of a polynomial](polynomial.md#root-of-a-polynomial) belong to $B_{N+1}\subseteq X$. Retaining $B_n$ at the next stage matters: $\phi(A)$ need not contain $A$.

#### Countability of pairwise disjoint open disks

↑ **Parent:** [Countable set](#countable-set)

Every family of pairwise disjoint nonempty open disks in the plane is countable. The [density of the rational numbers](number-theory.md#density-of-the-rational-numbers) gives each disk a point of the [countable set](#countable-set) $\mathbb Q^2$. Fixing an enumeration and taking the first point in each disk yields an [injection](algebra.md#injective-function) from disks to labels. This argument requires no countable choice of representatives and is useful when geometric separation would otherwise produce an uncountable family.

#### Increasing chain of countable sets

↑ **Parent:** [Countable set](#countable-set)

A family of countable [sets](set.md) indexed by a [linear order](algebra.md#linear-order) is increasing if $i\leq j$ implies $X_i\subseteq X_j$. Its union has [cardinality](#cardinality) at most $\aleph_1$, by the [cardinal bound for an increasing chain of countable sets](#cardinal-bound-for-an-increasing-chain-of-countable-sets). The index order need not be a [well-order](set.md#well-order).

##### Cardinal bound for an increasing chain of countable sets

↑ **Parent:** [Increasing chain of countable sets](#increasing-chain-of-countable-sets)

An [increasing chain of countable sets](#increasing-chain-of-countable-sets) has union of [cardinality](#cardinality) at most $\aleph_1$. If the union is uncountable, select $\aleph_1$ of its points and one containing member for each. Every countable member misses one selected point, so linear comparison puts it below that point's chosen member. The chosen subfamily is cofinal, and its union has size at most $\aleph_1$ by [infinite cardinal arithmetic](#infinite-cardinal-arithmetic).

#### Finite Cartesian power of a countable set

↑ **Parent:** [Countable set](#countable-set)

A finite [Cartesian product](#cartesian-product) of [countable sets](#countable-set) is countable. For a fixed finite exponent $m$, index tuples in $\mathbb N^m$ can be listed by increasing maximum coordinate, with each group finite. If $B$ is countably infinite and $m>0$, its power $B^m$ is also countably infinite.

#### Countable union of explicitly ordered finite lists without choice

↑ **Parent:** [Countable set](#countable-set)

Given finite lists $\ell_0,\ell_1,\ldots$ in a [set](set.md) $X$, their union of entries has an explicit enumeration from a subset of $\mathbb N^2$: use the existing positions in each list and a [Cantor pairing function](#cantor-pairing-function). If the union is infinite, successively take the first occurrence of an entry not previously taken, in the order of its natural-number code. The [well-order](set.md#well-order) on [natural numbers](arithmetic.md#natural-number) makes each step uniquely determined and yields an injection $\mathbb N\to X$. No [axiom of choice](#axiom-of-choice) is needed. This does not assert that an arbitrary countable family of unordered [finite sets](set.md#finite-set) has a countable union in [ZF](#zermelo-fraenkel-set-theory) without the [axiom of choice](#axiom-of-choice).

#### Countability from vanishing averages of distinct sequences

↑ **Parent:** [Countable set](#countable-set)

If every [sequence](real-analysis.md#sequence) of distinct elements of a positive-real [set](set.md) $A$ has arithmetic averages tending to zero, then $A$ is a [countable set](#countable-set). For each positive [integer](number-theory.md#integer) $n$, the threshold [set](set.md) $\{a\in A:a\ge1/n\}$ must be finite: an infinite sequence inside it would have averages at least $1/n$. The [Archimedean property](arithmetic.md#archimedean-property) makes $A$ their union, so the [countable union of countable sets](#countable-union-of-countable-sets) theorem applies. The hypothesis concerns every distinct-element sequence, not merely one enumeration.

#### Countably infinite set

↑ **Parent:** [Countable set](#countable-set)

A countably infinite set admits a [bijection](function.md#bijection) with the [natural numbers](arithmetic.md#natural-number).

##### Increasing enumeration of an infinite subset of natural numbers

↑ **Parent:** [Countably infinite set](#countably-infinite-set)

For an infinite [subset](set.md#subset) $A\subseteq\mathbb N$, repeatedly selecting the least element not yet used gives a [bijection](function.md#bijection) $f:\mathbb N\to A$. The [well-order](set.md#well-order) ensures each minimum exists, infinitude ensures the remaining [set](set.md) is nonempty, and strict increase gives injectivity. If $a\in A$ were omitted forever, all selected values would be at most $a$, impossible inside the [finite set](set.md#finite-set) $\{0,\ldots,a\}$.

#### Countable union of countable sets

↑ **Parent:** [Countable set](#countable-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Countable_union_of_countable_sets)

A countable union of countable sets is countable, using a diagonal enumeration.

##### Parabola obstruction to countable line coverings

↑ **Parent:** [Countable union of countable sets](#countable-union-of-countable-sets)

A [parabola](geometry-and-topology.md#parabola) parametrized by $(t,t^2)$ is in [bijection](function.md#bijection) with $\mathbb R$ and is an [uncountable set](#uncountable-set). Every affine line meets it in at most two points. A countable family of affine lines could therefore cover only countably many points of this [parabola](geometry-and-topology.md#parabola), and cannot cover the plane. More generally, an uncountable curve with finite intersection with every permitted member obstructs a countable covering by those members.

#### Cantor pairing function

↑ **Parent:** [Countable set](#countable-set)

The Cantor pairing function is an explicit [bijection](function.md#bijection) between $\mathbb N^2$ and $\mathbb N$, obtained by enumerating lattice points along successive diagonals.

<h4 id="cantor-s-diagonal-argument">Cantor's diagonal argument</h4>

↑ **Parent:** [Countable set](#countable-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor's_diagonal_argument)

Cantor's diagonal argument proves that the infinite binary sequences form an [uncountable set](#uncountable-set): a sequence obtained by changing the $n$th digit of the $n$th listed sequence differs from every sequence in the list.

### Uncountable set

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uncountable_set)

An uncountable set is a set for which no [bijection](function.md#bijection) with a subset of the natural numbers exists.

#### Uncountability of permutations of a countably infinite set

↑ **Parent:** [Uncountable set](#uncountable-set)

The [bijections](function.md#bijection) of a [countably infinite set](#countably-infinite-set) form an uncountable set. Partition an enumeration into disjoint pairs and encode an infinite [binary sequence](real-analysis.md#bitstream) by independently fixing or swapping each pair.

#### Uncountability of surjections onto a nontrivial finite set

↑ **Parent:** [Uncountable set](#uncountable-set)

If $B$ is a [countably infinite set](#countably-infinite-set) and $A$ is a [finite set](set.md#finite-set) with at least two elements, the set of [surjective functions](algebra.md#surjective-function) $B\to A$ is uncountable. Fix finitely many values to cover $A$, then encode an arbitrary infinite [binary sequence](real-analysis.md#bitstream) using two values of $A$ on the remaining inputs.

### Initial ordinal

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Initial_ordinal)

An initial ordinal is an ordinal not equinumerous with any smaller ordinal. It is therefore the canonical ordinal representative of a cardinal.

#### Aleph number

↑ **Parent:** [Initial ordinal](#initial-ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aleph_number)

The alephs enumerate the infinite initial ordinals: $\aleph_0=\omega$, successor indices select the next initial ordinal, and limit indices select the least initial ordinal above all earlier values.

##### Every infinite cardinal is an aleph

↑ **Parent:** [Aleph number](#aleph-number)

Assuming the [axiom of choice](#axiom-of-choice), the [well-ordering theorem](#well-ordering-theorem) makes every set equipotent to an [initial ordinal](#initial-ordinal). The infinite initial ordinals are exactly the $\aleph_\alpha$, so every infinite cardinal is $\aleph_\alpha$ for a unique ordinal $\alpha$.

### Cardinal arithmetic

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardinal_arithmetic)

Cardinal sums are cardinalities of disjoint unions, products are cardinalities of Cartesian products, and exponentials $\kappa^\lambda$ count functions from a set of size $\lambda$ to one of size $\kappa$.

#### Gimel function

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)

For an infinite [cardinal number](#cardinal-number), $\gimel(\kappa)=\kappa^{\operatorname{cf}(\kappa)}$. The [singular cardinals hypothesis](#singular-cardinals-hypothesis) predicts its value when $\kappa$ is a [singular cardinal](#singular-cardinal) and $2^{\operatorname{cf}(\kappa)}<\kappa$. For a [regular cardinal](#regular-cardinal), its value is $2^\kappa$.

##### Gimel recursion for cardinal exponentiation

↑ **Parent:** [Gimel function](#gimel-function)

The [Gimel function](#gimel-function) determines all infinite [cardinal](#cardinal-number) powers. For a regular base, $2^\kappa=\gimel(\kappa)$. For a singular base, put $s=\sup_{\rho<\kappa}2^\rho$ and $\theta=\operatorname{cf}(\kappa)$; then $2^\kappa=s^\theta$, which is $s$ if attained below $\kappa$ and $\gimel(s)$ otherwise. After these powers are known, fix an infinite exponent $\lambda$ and recurse on the base. Below $\lambda$ use $2^\lambda$; at successors use the [Hausdorff formula for cardinal exponentiation](#hausdorff-formula-for-cardinal-exponentiation). At a limit base greater than $\lambda$, put $a=\sup_{\rho<\kappa}\rho^\lambda$. The answer is $a$ if $\operatorname{cf}(\kappa)>\lambda$ or the supremum is attained, and $\gimel(a)$ otherwise. In the nonattained cases, the cofinal-index argument identifies the [cofinality](#cofinality) of the supremum.

##### Gimel hypothesis

↑ **Parent:** [Gimel function](#gimel-function)

For every singular infinite [cardinal number](#cardinal-number) $\kappa$, the [Gimel function](#gimel-function) has the smallest value permitted by [König theorem for cardinal numbers](#konig-s-theorem-set-theory) and the exponent: $\kappa^{\operatorname{cf}(\kappa)}=\max\{\kappa^+,2^{\operatorname{cf}(\kappa)}\}$. Where $2^{\operatorname{cf}(\kappa)}<\kappa$, this is the [singular cardinals hypothesis](#singular-cardinals-hypothesis). The hypothesis imposes no separate successor-power condition on regular [cardinals](#cardinal-number).

#### Beth number

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beth_number)

The [cardinal numbers](#cardinal-number) defined by $\beth_0=\aleph_0$, $\beth_{\alpha+1}=2^{\beth_\alpha}$, and $\beth_\lambda=\sup_{\alpha<\lambda}\beth_\alpha$ at [limit ordinals](#limit-ordinal) are the beth numbers. In particular $\beth_1=|\mathcal P(\omega)|$, the [cardinality](#cardinality) of the continuum. This notation distinguishes iterated [power sets](set.md#power-set) from the enumeration by [Aleph numbers](#aleph-number) of well-orderable infinite [cardinal numbers](#cardinal-number).

#### Product-sum comparison lemma

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)

In ZF, let $K,L$ be nonempty. If $K\times L$ injects into $K\sqcup L$, then there is either an injection or a surjection from $K$ to $L$.

Indeed, extend the inverse of the given injection to a surjection $p:K\sqcup L\to K\times L$ by sending points outside its range to one fixed pair $(k_*,l_*)$. If the second coordinate of $p$ restricted to the $K$-summand covers $L$, it is the required surjection. Otherwise choose $l_0$ that it misses. Every $(k,l_0)$ then has its preimage in the $L$-summand. Except possibly for the default pair, that preimage is unique, so these preimages inject $K$ into $L$. In the exceptional case they inject $K\setminus\{k_*\}$ into $L$; either their image is all of $L$, yielding a surjection from $K$, or an omitted point extends the map to an injection from $K$.

#### Infinite cardinal arithmetic

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)

For infinite cardinals, choice gives $\kappa+\kappa=\kappa\cdot\kappa=\kappa$. Exponentiation satisfies $(\kappa^\lambda)^\mu=\kappa^{\lambda\mu}$, while a countable sum of cardinals has size the maximum of $\aleph_0$ and their supremum.

##### Currying law for cardinal exponentiation

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

There is a natural [bijection](function.md#bijection) between functions $M\to K^L$ and functions $M\times L\to K$, obtained by sending $f$ to $(m,l)\mapsto f(m)(l)$. Therefore

$$
(\kappa^\lambda)^\mu=\kappa^{\lambda\mu}.
$$

##### Square of an infinite cardinal

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

Assuming the [axiom of choice](#axiom-of-choice), every infinite cardinal satisfies

$$
\kappa\cdot\kappa=\kappa.
$$

One proof takes a least counterexample $\kappa$, identifies cardinals with [initial ordinals](#initial-ordinal), and well-orders $\kappa\times\kappa$ first by $\max\{\alpha,\beta\}$. Every proper initial segment then has cardinality below $\kappa$ by minimality, so the whole order has cardinality at most $\kappa$, contradicting the choice of $\kappa$.

##### Sum and product of two infinite cardinals

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

For infinite cardinals $\kappa$ and $\lambda$, the [axiom of choice](#axiom-of-choice) and the [square of an infinite cardinal](#square-of-an-infinite-cardinal) give

$$
\kappa+\lambda=\kappa\lambda=\max\{\kappa,\lambda\}.
$$

The maximum is a lower bound for both operations, while both are bounded above by respectively $\mu+\mu$ and $\mu^2$, where $\mu=\max\{\kappa,\lambda\}$.

##### Cardinality of a finite union of infinite sets

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

For finitely many infinite sets $X_1,\ldots,X_n$, choose one whose cardinality $\kappa$ is largest. Then

$$
\kappa\leq\left|\bigcup_{i=1}^nX_i\right|
\leq\sum_{i=1}^n|X_i|
\leq n\kappa=\kappa,
$$

so the union has the same cardinality as that largest member.

##### Countable family of distinct infinite cardinalities with a largest member

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

Pairwise distinct cardinalities do not prevent a countable family from having a largest member. For example, take $X_1=\aleph_\omega$ and $X_{n+2}=\aleph_n$ for $n<\omega$, viewing cardinals as initial ordinals. Every later set is a subset of $X_1$, so

$$
\bigcup_{n\geq1}X_n=X_1
$$

although all the cardinalities are different.

##### Cardinal exponentiation between two and the exponent

↑ **Parent:** [Infinite cardinal arithmetic](#infinite-cardinal-arithmetic)

If $\lambda$ is infinite and $2\le\kappa\le\lambda$, then

$$
\kappa^\lambda=2^\lambda.
$$

Indeed,

$$
2^\lambda\le\kappa^\lambda\le\lambda^\lambda
\le(2^\lambda)^\lambda
=2^{\lambda\lambda}=2^\lambda.
$$

<h4 id="konig-s-theorem-set-theory">Kőnig's theorem (set theory)</h4>

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kőnig's_theorem_(set_theory))

If $\kappa_i<\lambda_i$ for every $i\in I$, then

$$
\sum_{i\in I}\kappa_i<\prod_{i\in I}\lambda_i.
$$

The injection uses functions supported at one coordinate. For non-surjectivity, given any map from the disjoint union to the product, choose at coordinate $i$ a value omitted by the $i$th row; the resulting diagonal element is outside its image.

#### Hausdorff formula for cardinal exponentiation

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)

For infinite cardinals $\kappa,\lambda$, Hausdorff's formula is

$$
(\kappa^+)^\lambda=\kappa^\lambda\cdot\kappa^+
=\max\{\kappa^\lambda,\kappa^+\}.
$$

#### Continuum hypothesis

↑ **Parent:** [Cardinal arithmetic](#cardinal-arithmetic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuum_hypothesis)

The continuum hypothesis asserts that every infinite subset of the real numbers is either countable or equinumerous with the real numbers, equivalently $2^{\aleph_0}=\aleph_1$.

##### Freiling axiom of symmetry

↑ **Parent:** [Continuum hypothesis](#continuum-hypothesis)

Every function $f:\mathbb R\to[\mathbb R]^{<\omega_1}$ has reals $x,y$ with $x\notin f(y)$ and $y\notin f(x)$. The values are countable [subsets](set.md#subset). Requiring distinct witnesses is equivalent, by first adjoining $x$ to $f(x)$. The [Freiling theorem](#freiling-theorem) identifies this axiom with the negation of the [Continuum hypothesis](#continuum-hypothesis) in [ZFC](#zermelo-fraenkel-set-theory-with-choice).

###### Freiling theorem

↑ **Parent:** [Freiling axiom of symmetry](#freiling-axiom-of-symmetry)

In [ZFC](#zermelo-fraenkel-set-theory-with-choice), the [Freiling axiom of symmetry](#freiling-axiom-of-symmetry) is equivalent to failure of the [Continuum hypothesis](#continuum-hypothesis). Under the hypothesis, countable initial segments of a well-order of the reals violate symmetry. When the continuum exceeds $\aleph_1$, the union of the countable values on an $\aleph_1$-sized set leaves a real outside; avoiding that real's countable value gives the two witnesses.

##### Generalized continuum hypothesis

↑ **Parent:** [Continuum hypothesis](#continuum-hypothesis)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_continuum_hypothesis)

The generalized continuum hypothesis states that $2^\kappa=\kappa^+$ for every infinite [cardinal number](#cardinal-number) $\kappa$.

<h3 id="cantor-schroder-bernstein-theorem">Cantor-Schröder-Bernstein theorem</h3>

↑ **Parent:** [Cardinal number](#cardinal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor-Schröder-Bernstein_theorem)

If there are injections $X\to Y$ and $Y\to X$, then there is a bijection $X\cong Y$.

## Ordinal

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal)

An ordinal is a transitive set well-ordered by membership and represents the order type of a well-order.

### Finite ordinal

↑ **Parent:** [Ordinal](#ordinal)

A finite [ordinal](#ordinal) is the order type of a finite [well-order](set.md#well-order); in the von Neumann representation it is one of $0,1,2,\ldots$. They are exactly the [ordinals](#ordinal) $x$ such that $x$ and each member of $x$ are either zero or [successor ordinals](#successor-ordinal). If an [ordinal](#ordinal) is infinite, it either is the nonzero limit $\omega$ or contains $\omega$ as a member, so it fails this test. Thus the [finite ordinals](#finite-ordinal) give the usual representation of the [natural numbers](arithmetic.md#natural-number).

### Bounded successor characterization of finite ordinals

↑ **Parent:** [Ordinal](#ordinal)

A [Von Neumann ordinal](#ordinal) $x$ is finite exactly when $x$ and every member of $x$ are either zero or [successor ordinals](#successor-ordinal). Every [finite ordinal](#finite-ordinal) has that property. Conversely, an infinite [ordinal](#ordinal) is either $\omega$, which is a nonzero limit, or is greater than $\omega$ and contains that nonzero [limit ordinal](#limit-ordinal). The test can be expressed by a bounded [first-order formula](mathematical-logic.md#first-order-formula): ordinality uses transitivity and membership comparability, and a nonempty [ordinal](#ordinal) is a successor exactly when it has a greatest member. This defines the class of [natural numbers](arithmetic.md#natural-number) without quantifying over arbitrary infinite [inductive sets](#inductive-set).

### Club set

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Club_set)

For a [limit ordinal](#limit-ordinal) $\kappa$, a [subset](set.md#subset) $C\subseteq\kappa$ is club if it is unbounded and contains each limit below $\kappa$ of an increasing sequence from $C$. At an uncountable [regular cardinal](#regular-cardinal) $\kappa$, intersections of fewer than $\kappa$ club [sets](set.md) are club: above a starting point cycle through the sets and take suprema, using regularity to stay below $\kappa$; closure puts the resulting limit in all of them. Club [sets](set.md) provide the reflecting ranks in [worldly cardinals below an inaccessible cardinal](#worldly-cardinals-below-an-inaccessible-cardinal).

#### Club of closure points for countable set-valued functions

↑ **Parent:** [Club set](#club-set)

For a regular uncountable [cardinal](#cardinal-number) $\lambda$ and $B:\lambda\to[\lambda]^\omega$, the [limit ordinals](#limit-ordinal) closed under all earlier values of $B$ form a [club set](#club-set). Countably iterate bounds for $\bigcup_{\alpha<\gamma}B(\alpha)$ to obtain unboundedly many closure points. Regularity keeps each bound and the countable supremum below $\lambda$. Limits of closure points remain closure points.

#### Diagonal intersection

↑ **Parent:** [Club set](#club-set)

For $\langle C_\alpha:\alpha<\delta\rangle$, its diagonal intersection consists of $\beta<\delta$ belonging to every $C_\alpha$ with $\alpha<\beta$. For club sets on a regular uncountable cardinal, this is a club.

#### Club sequence

↑ **Parent:** [Club set](#club-set)

A sequence $\langle C_\delta\rangle$ in which $C_\delta$ is closed and unbounded in $\delta$. At a successor ordinal its predecessor is a club singleton. Such sequences define [minimal walks along a club sequence](#minimal-walk-along-a-club-sequence).

##### Square principle

↑ **Parent:** [Club sequence](#club-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_principle)

For an infinite [cardinal](#cardinal-number) $\kappa$, the square principle supplies [club sets](#club-set) $C_\zeta\subseteq\zeta$ at limit $\zeta<\kappa^+$, with [order type](#order-type) at most $\kappa$, coherent at limit points: $C_\gamma=C_\zeta\cap\gamma$ whenever $\gamma$ is a limit point of $C_\zeta$. The bound precludes a single [club set](#club-set) threading the entire sequence. For regular uncountable $\kappa$, coherence together with the weaker-looking size clause $\operatorname{cf}(\zeta)<\kappa\Rightarrow|C_\zeta|<\kappa$ implies the order-type bound. At $\kappa=\omega$, that clause alone is vacuous and cannot replace the bound.

##### Minimal walk along a club sequence

↑ **Parent:** [Club sequence](#club-sequence)

To walk from $\beta$ to $\alpha<\beta$, start at $\beta$ and repeatedly move from $\delta$ to $\min(C_\delta\setminus\alpha)$ until reaching $\alpha$. The strict decrease in [ordinals](#ordinal) makes the walk finite. Its trace records the successive $C_\delta\cap\alpha$.

###### Minimal-walk tree

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

The tree of restrictions $\rho_\beta\upharpoonright\alpha$, ordered by extension. For a [club sequence](#club-sequence) on $\omega_2$ with club order types at most $\omega_1$, the [Continuum hypothesis](#continuum-hypothesis) bounds each level by $\aleph_1$. Trace injectivity and [Fodor lemma](#fodor-lemma) exclude a [cofinal branch](set.md#cofinal-branch).

###### Trace coherence lemma for minimal walks

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

If $\rho_\beta(\alpha)=\rho_\gamma(\alpha)$, then the trace functions agree below $\alpha$. Each shorter trace is reconstructed by locating the first recorded club initial segment that meets $[\xi,\alpha)$ and continuing the walk from its least such point.

###### First-divergence lemma for minimal walks

↑ **Parent:** [Minimal walk along a club sequence](#minimal-walk-along-a-club-sequence)

The walks to $\xi<\alpha$ share a unique maximal initial chain of nodes. At the next step the walk to $\xi$ moves into $[\xi,\alpha)$; the walk to $\alpha$ stays at or above $\alpha$ or has just ended.

#### Stationary set

↑ **Parent:** [Club set](#club-set)

A subset of a regular uncountable [cardinal number](#cardinal-number) $\kappa$ is stationary if it meets every [club set](#club-set) in $\kappa$. Intersecting a stationary set with a [club set](#club-set) preserves stationarity. Every member of the [club filter](#club-filter) is stationary. At a regular infinite $\theta<\kappa$, the [stationarity of ordinals of prescribed cofinality](#stationarity-of-ordinals-of-prescribed-cofinality) supplies important examples.

##### Stationary partition at a successor cardinal

↑ **Parent:** [Stationary set](#stationary-set)

Every stationary subset of a successor cardinal $\lambda^+$ can be partitioned into $\lambda^+$ disjoint stationary subsets. For each $\beta\in[\lambda,\lambda^+)$ choose a bijection $e_\beta:\lambda\to\beta$. For each $\xi<\lambda^+$, the function $\beta\mapsto e_\beta^{-1}(\xi)$ is regressive on the stationary tail with $\beta>\xi$. The [Fodor lemma](#fodor-lemma) gives a stationary fiber with one value $i_\xi<\lambda$. Some value occurs for $\lambda^+$ many indices, whose fibers are pairwise disjoint. Assign any leftover part of $S$ to one fiber.

##### Non-reflecting subset

↑ **Parent:** [Stationary set](#stationary-set)

A [subset](set.md#subset) $X\subseteq\lambda$ is non-reflecting in the indicated sense if it is not stationary below any $\delta<\lambda$ of uncountable [cofinality](#cofinality). The [subset](set.md#subset) itself need not be stationary. Nonreflection is inherited by [subsets](set.md#subset). With this definition every [subset](set.md#subset) of $\omega_1$ is non-reflecting, since all smaller [ordinals](#ordinal) have countable [cofinality](#cofinality).

###### Nonreflection of fixed order-type fibers

↑ **Parent:** [Non-reflecting subset](#non-reflecting-subset)

For a coherent [club set](#club-set) sequence, the limit points of $C_\delta$ form a [club set](#club-set) whenever $\operatorname{cf}(\delta)>\omega$. Along these points, $\operatorname{otp}(C_\gamma)=\operatorname{otp}(C_\delta\cap\gamma)$ strictly increases, so a fixed fiber $E_\xi$ meets this a [club set](#club-set) at most once and cannot reflect at $\delta$. Under the [square principle](#square-principle) order-type bound, the fibers with $\xi\le\kappa$ partition all [limit ordinals](#limit-ordinal) below $\kappa^+$ into $\kappa$ non-reflecting pieces.

##### Stationarity in a limit ordinal

↑ **Parent:** [Stationary set](#stationary-set)

For any nonzero [limit ordinal](#limit-ordinal) $\delta$, a [club set](#club-set) is an unbounded [subset](set.md#subset) closed under limit points below $\delta$. A [subset](set.md#subset) is stationary if it meets every such [club set](#club-set). Statements concerning the completeness of the [club filter](#club-filter) or [Fodor lemma](#fodor-lemma) require regular uncountable height; they should not be transferred to arbitrary singular or countable [limit ordinals](#limit-ordinal) without checking their hypotheses.

##### Stationary partition by cofinal-sequence fibers

↑ **Parent:** [Stationary set](#stationary-set)

For an uncountable [regular cardinal](#regular-cardinal) $\kappa$, choose cofinal sequences $c_\alpha:\omega\to\alpha$ for the [stationary set](#stationary-set) of [ordinals](#ordinal) of [cofinality](#cofinality) $\omega$. Above any bound, some fixed coordinate exceeds the bound on a stationary [subset](set.md#subset); [Fodor lemma](#fodor-lemma) makes that coordinate constant on a stationary [subset](set.md#subset). Thus the stationary constant fibers, over all coordinates, have unboundedly many values. Regularity makes one coordinate have $\kappa$ such values. Its fibers are disjoint [stationary sets](#stationary-set); adding all leftover [ordinals](#ordinal) to one piece partitions $\kappa$.

##### Ulam matrix on omega-one

↑ **Parent:** [Stationary set](#stationary-set)

A family $(A_{\alpha,n})_{\alpha<\omega_1,n<\omega}$ whose row at $\alpha$ partitions $(\alpha,\omega_1)$ and whose fixed-column cells are pairwise disjoint. Choose [injections](algebra.md#injective-function) $e_\beta:\beta\to\omega$ and put $A_{\alpha,n}=\{\beta>\alpha:e_\beta(\alpha)=n\}$. This gives a matrix used to split [stationary sets](#stationary-set) into many stationary pieces.

###### Disjoint stationary subsets of omega-one

↑ **Parent:** [Ulam matrix on omega-one](#ulam-matrix-on-omega-one)

There are $\aleph_1$ pairwise disjoint stationary subsets of the nonzero countable limit ordinals. In a [Ulam matrix on omega-one](#ulam-matrix-on-omega-one), each row partitions a stationary tail into countably many cells, so some cell is stationary. One column contains stationary cells in uncountably many rows, and the column cells are disjoint. Unions indexed by different subsets of $\omega_1$ then differ on a stationary set.

##### Diamond principle

↑ **Parent:** [Stationary set](#stationary-set)

A sequence $D_\alpha\subseteq\alpha$ guesses every $X\subseteq\omega_1$ stationarily often: $\{\alpha:D_\alpha=X\cap\alpha\}$ is stationary.

###### CCC forcing cannot create diamond

↑ **Parent:** [Diamond principle](#diamond-principle)

For each index, collect the ground [subsets](set.md#subset) which some condition forces to be the corresponding diamond guess. Distinct forced values have incompatible witnessing conditions, so the [countable chain condition for forcing](forcing.md#countable-chain-condition-for-forcing) makes this a countable family. Every ground [subset](set.md#subset) is guessed by these families on a ground stationary set, by testing each ground [club set](#club-set). The [countable-family diamond equivalence](#countable-family-diamond-equivalence) then yields diamond in the ground model. A generic guess need not itself be a ground [subset](set.md#subset); only values forced equal to one are collected.

###### Stationary diamond principle

↑ **Parent:** [Diamond principle](#diamond-principle)

For a stationary $S\subseteq\omega_1$, a sequence $D_\alpha\subseteq\alpha$ indexed by $S$ guesses every $X\subseteq\omega_1$ on a stationary subset of $S$.

###### Stationary diamond at a regular cardinal

↑ **Parent:** [Stationary diamond principle](#stationary-diamond-principle)

A sequence $D_\alpha\subseteq\alpha$, indexed by a stationary [subset](set.md#subset) $S$ of a regular uncountable [cardinal](#cardinal-number) $\lambda$, guesses every $X\subseteq\lambda$ stationarily often: $\{\alpha\in S:D_\alpha=X\cap\alpha\}$ is stationary. This extends the usual [stationary diamond principle](#stationary-diamond-principle) at $\omega_1$.

###### Countable-family diamond principle

↑ **Parent:** [Stationary diamond at a regular cardinal](#stationary-diamond-at-a-regular-cardinal)

At each $\alpha\in S$, a countable family $E_\alpha\subseteq\mathcal P(\alpha)$ is supplied. Every $X\subseteq\lambda$ has $X\cap\alpha\in E_\alpha$ on a stationary [subset](set.md#subset) of $S$. The [countable-family diamond equivalence](#countable-family-diamond-equivalence) shows that this apparently weaker prediction is equivalent to a single diamond guess at each index.

###### Countable-family diamond equivalence

↑ **Parent:** [Countable-family diamond principle](#countable-family-diamond-principle)

Enumerate each countable guessing family and use a [bijection](function.md#bijection) $\pi:\lambda\times\omega\to\lambda$ with a [club set](#club-set) of prefix-closure points. The $n$th candidate sequence decodes the $n$th component of the $n$th family entry. If all candidates fail, choose counterexample sets $X_n$ and [club sets](#club-set) witnessing failure, then code the $X_n$ together using $\pi$. A correct family guess on the common closure [club set](#club-set) and all failure [club sets](#club-set) decodes to one of the forbidden correct guesses. The singleton-family implication supplies the reverse direction.

###### Antichain sealing by diamond

↑ **Parent:** [Stationary diamond principle](#stationary-diamond-principle)

At a correctly guessing limit stage of a normal tree construction, make every new level node extend a member of the guessed maximal [tree antichain](set.md#tree-antichain). It follows that the antichain has no later member. This produces a [Suslin tree](set.md#suslin-tree) from the [stationary diamond principle](#stationary-diamond-principle).

##### Club principle

↑ **Parent:** [Stationary set](#stationary-set)

There are cofinal sequences $A_\delta\subseteq\delta$ of order type $\omega$ for the countable limit ordinals, such that every uncountable $X\subseteq\omega_1$ contains some $A_\delta$.

###### Stationary-indexed club principle

↑ **Parent:** [Club principle](#club-principle)

For a stationary $S\subseteq\omega_1$, there are cofinal ladders $A_\delta\subset\delta$ of order type $\omega$, indexed by [limit ordinals](#limit-ordinal) in $S$, such that every uncountable $X\subseteq\omega_1$ contains one of these ladders. This predicts a contained ladder, whereas [stationary diamond principle](#stationary-diamond-principle) predicts a whole initial segment.

##### Regressive function

↑ **Parent:** [Stationary set](#stationary-set)

A function on a set of ordinals with $f(\alpha)<\alpha$ at every nonzero point of its domain. On a stationary subset of a regular uncountable cardinal, [Fodor lemma](#fodor-lemma) makes it constant on a stationary subset.

###### Fodor lemma

↑ **Parent:** [Regressive function](#regressive-function)

A [regressive function](#regressive-function) on a stationary subset of a regular uncountable cardinal is constant on a stationary subset.

###### Filtration form of Fodor lemma

↑ **Parent:** [Fodor lemma](#fodor-lemma)

If $S\subseteq\kappa$ is stationary and $f(\alpha)\in A_\alpha$ for a [kappa-filtration](#kappa-filtration), then $f$ is constant on a stationary [subset](set.md#subset). Restrict to limit indices and use continuity to find a smaller stage containing each value. [Fodor lemma](#fodor-lemma) fixes that stage on a stationary [subset](set.md#subset). Its size is less than $\kappa$, so [club filter completeness](#club-filter-completeness) makes one value fiber stationary.

##### Stationarity of ordinals of prescribed cofinality

↑ **Parent:** [Stationary set](#stationary-set)

For a regular infinite $\theta<\kappa$, with $\kappa$ a regular uncountable [cardinal number](#cardinal-number), $S_\theta^\kappa=\{\delta<\kappa:\operatorname{cf}(\delta)=\theta\}$ is stationary. Build a strictly increasing continuous $\theta$-sequence in any [club set](#club-set), and take its supremum. Closure places it in that club and the [cofinality of an increasing ordinal supremum](#cofinality-of-an-increasing-ordinal-supremum) gives [cofinality](#cofinality) $\theta$. In particular the two disjoint sets $S_\omega^{\omega_2}$ and $S_{\omega_1}^{\omega_2}$ show that the [club filter](#club-filter) on $\omega_2$ is not an [ultrafilter](#ultrafilter).

#### Club filter

↑ **Parent:** [Club set](#club-set)

On a regular uncountable [cardinal number](#cardinal-number) $\kappa$, the club filter consists of all subsets containing a [club set](#club-set). It is a [kappa-complete filter](#kappa-complete-filter) by [club filter completeness](#club-filter-completeness). Its members are [stationary sets](#stationary-set), although a [stationary set](#stationary-set) need not be a filter member, and a filter member need not itself be closed.

##### Stationary nonclosed member of the club filter

↑ **Parent:** [Club filter](#club-filter)

For any regular uncountable [cardinal number](#cardinal-number) $\kappa$, the set $\kappa\setminus\{\omega\}$ contains the final-segment [club set](#club-set) $[\omega+1,\kappa)$, so belongs to the [club filter](#club-filter) and is a [stationary set](#stationary-set). It is not closed, since its finite ordinals have supremum $\omega$, which is missing.

##### Club filter completeness

↑ **Parent:** [Club filter](#club-filter)

The [club filter](#club-filter) on a regular uncountable [cardinal number](#cardinal-number) $\kappa$ is $\kappa$-complete. Intersections of fewer than $\kappa$ [club sets](#club-set) are closed. For unboundedness, repeatedly step past a point of each club and take a countable supremum; regularity keeps all suprema below $\kappa$, and closure puts the final supremum in every club.

#### Closed unbounded class of ordinals

↑ **Parent:** [Club set](#club-set)

An unbounded [class in set theory](#class-set-theory) of [ordinals](#ordinal) is closed if every nonempty set-sized increasing sequence of its members has its supremum in the class. This is the proper-class analogue of a [club set](#club-set). The [reflection theorem for definable hierarchies](#reflection-theorem-for-definable-hierarchies) gives such a class for every finite collection of [first-order formulas](mathematical-logic.md#first-order-formula).

### Successor ordinal

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successor_ordinal)

The successor of an ordinal $\alpha$ is $\alpha+1=\alpha\cup\{\alpha\}$.

### Countable ordinal

↑ **Parent:** [Ordinal](#ordinal)

A countable ordinal has a [countable set](#countable-set) as its underlying set.

These are the [ordinals](#ordinal) strictly below the [first uncountable ordinal](#first-uncountable-ordinal).

### Order type

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_type)

The order type of a well-order is the unique ordinal isomorphic to it.

#### Mostowski collapse theorem

↑ **Parent:** [Order type](#order-type)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mostowski_collapse_theorem)

Every well-founded extensional relation is uniquely isomorphic to membership on a transitive set.

##### Mostowski collapse

↑ **Parent:** [Mostowski collapse theorem](#mostowski-collapse-theorem)

The recursively defined [isomorphism](algebra.md#isomorphism) from a [well-founded](#well-founded-relation) extensional set-like relation to membership on a [transitive set](#transitive-set) or class. The [Mostowski collapse theorem](#mostowski-collapse-theorem) asserts its existence and uniqueness; the class form requires each predecessor extension to be a set.

##### Transitive collapse fixes transitive subsets

↑ **Parent:** [Mostowski collapse theorem](#mostowski-collapse-theorem)

If $X$ has a well-founded extensional inherited membership relation and $T\subseteq X$ is a [transitive set](#transitive-set), its [Mostowski collapse theorem](#mostowski-collapse-theorem) map $\pi$ fixes every member of $T$. The recursion $\pi(x)=\{\pi(y):y\in x\cap X\}$ and [well-founded relation](#well-founded-relation) induction give this pointwise. If also $T\in X$, then $\pi(T)=T$.

### Limit ordinal

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limit_ordinal)

A nonzero ordinal is a limit ordinal when it is not a successor ordinal. Equivalently, it is the supremum of all smaller ordinals.

### Normal function on an ordinal

↑ **Parent:** [Ordinal](#ordinal)

A function $f:\lambda\to\lambda$ on an ordinal is normal when it is strictly increasing and continuous at limit ordinals: $f(\delta)=\sup_{\alpha<\delta}f(\alpha)$ for every limit $\delta<\lambda$.

#### Fixed point of a normal ordinal function

↑ **Parent:** [Normal function on an ordinal](#normal-function-on-an-ordinal)

For a strictly increasing ordinal class function continuous at limits, start with $\alpha_0=0$ and iterate $\alpha_{n+1}=f(\alpha_n)$. If the sequence stabilizes, its stable value is a [fixed point](function.md#fixed-point). Otherwise its supremum $\alpha$ is a limit and continuity gives $f(\alpha)=\sup_n f(\alpha_n)=\sup_n\alpha_{n+1}=\alpha$. Starting the iteration above any prescribed ordinal gives arbitrarily large fixed points.

### Transfinite recursion

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfinite_recursion)

Transfinite recursion defines a value at each ordinal from the function of all earlier values.

#### Natural-number recursion theorem

↑ **Parent:** [Transfinite recursion](#transfinite-recursion)

Given an initial value $a$ and a rule $G$, there is a unique function $F$ on $\omega$ satisfying $F(0)=a$ and $F(n+1)=G(F(n))$.

### Transfinite induction

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transfinite_induction)

If a property of an ordinal follows whenever it holds for every smaller ordinal, then it holds for every ordinal.

### Ordinal addition

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_addition)

Ordinal addition is ordered concatenation and is associative but generally not commutative.

#### Associativity of ordinal addition

↑ **Parent:** [Ordinal addition](#ordinal-addition)

For all ordinals $\alpha,\beta,\gamma$,

$$
(\alpha+\beta)+\gamma=\alpha+(\beta+\gamma).
$$

This follows by [transfinite induction](#transfinite-induction) on $\gamma$ from the recursive definition of [ordinal addition](#ordinal-addition).

#### Commuting ordinal addition

↑ **Parent:** [Ordinal addition](#ordinal-addition)

Nonzero ordinals commute under addition precisely when they are positive finite right multiples of a common ordinal. This follows by comparing their [Cantor normal forms](#cantor-normal-form) at the first exponent where they differ.

### Ordinal multiplication

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_multiplication)

Ordinal multiplication is defined recursively by

$$
\alpha0=0,
\qquad
\alpha(\beta+1)=\alpha\beta+\alpha,
\qquad
\alpha\lambda=\sup_{\xi<\lambda}\alpha\xi
$$

for nonzero [limit ordinal](#limit-ordinal) $\lambda$. It is associative and left-distributive over [ordinal addition](#ordinal-addition), but generally neither commutative nor right-distributive.

#### Ordinal division algorithm

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

For [ordinals](#ordinal) $\alpha$ and $\delta>0$, there are unique ordinals $q,r$ with the displayed relation. The function $q\mapsto\delta q$ is strictly increasing, continuous at limit ordinals and unbounded. Its first value above $\alpha$ occurs at a successor, giving the largest $q$ with $\delta q\le\alpha$. The ordered tail of $\alpha$ after that initial segment gives $r$, and maximality gives $r<\delta$.

#### Commuting squares of ordinals

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

Two [ordinals](#ordinal) commute under [ordinal multiplication](#ordinal-multiplication) if and only if their squares commute. One implication follows from [associativity](group.md#associative-property). For the converse, squaring is strictly increasing: $A<B$ implies $A^2\leq BA<B^2$. If $\alpha\beta<\beta\alpha$, monotonicity gives

$$
\alpha^2\beta^2\leq(\alpha\beta)^2<(\beta\alpha)^2\leq\beta^2\alpha^2,
$$

a contradiction to commuting squares. Swap the factors to exclude the reverse inequality; zero factors cause no exception.

#### Distributive law for ordinal multiplication

↑ **Parent:** [Ordinal multiplication](#ordinal-multiplication)

[Ordinal multiplication](#ordinal-multiplication) is distributive in its right argument:

$$
\alpha(\beta+\gamma)=\alpha\beta+\alpha\gamma.
$$

Indeed a sequence of copies of $\alpha$ indexed by the concatenation of $\beta$ and $\gamma$ is the concatenation of the two sequences of copies. The other distributive law fails: $(1+1)\omega=\omega$, while $\omega+\omega>\omega$.

### Ordinal exponentiation

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_exponentiation)

Ordinal exponentiation is defined recursively by

$$
\alpha^0=1,\qquad
\alpha^{\beta+1}=\alpha^\beta\alpha,\qquad
\alpha^\lambda=\sup_{\xi<\lambda}\alpha^\xi
$$

for nonzero limit $\lambda$. Transfinite induction gives

$$
\alpha^{\beta+\gamma}=\alpha^\beta\alpha^\gamma.
$$

#### Epsilon zero

↑ **Parent:** [Ordinal exponentiation](#ordinal-exponentiation)

The [ordinal](#ordinal) $\varepsilon_0$ is the least fixed point of $\alpha\mapsto\omega^\alpha$. It is the supremum of $1,\omega,\omega^\omega,\omega^{\omega^\omega},\ldots$, and is countable.

### Derived-set iteration of a well-order

↑ **Parent:** [Ordinal](#ordinal)

For a well-ordered set $X$, let $X'$ contain the points whose strict initial segments are nonempty and have no greatest element, and iterate this operation transfinitely, taking intersections at limit stages. Every nonempty derivative loses at least its least element. If no derivative became empty, choosing one point from each successive difference would inject the ordinal supplied by [Hartogs theorem](#hartogs-theorem) for $X$ into $X$, a contradiction.

#### Derived sets of an ordinal

↑ **Parent:** [Derived-set iteration of a well-order](#derived-set-iteration-of-a-well-order)

For an ordinal $\xi$,

$$
\xi'=\{\omega\beta<\xi:\beta>0\},
\qquad
\xi''=\{\omega^2\beta<\xi:\beta>0\}.
$$

Thus the derivative index of $\omega$ is one and that of $\omega^2$ is two.

### Ordinal interval

↑ **Parent:** [Ordinal](#ordinal)

For $\alpha<\beta$, the ordinal interval $\beta\setminus\alpha$ is the ordered tail from $\alpha$ inclusive to $\beta$ exclusive.

### First uncountable ordinal

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_uncountable_ordinal)

The first uncountable ordinal $\omega_1$ is the set of all countable ordinals.

#### First uncountable ordinal is regular

↑ **Parent:** [First uncountable ordinal](#first-uncountable-ordinal)

The [first uncountable ordinal](#first-uncountable-ordinal) has [cofinality](#cofinality) $\omega_1$. Indeed, the supremum of any [countable set](#countable-set) of countable ordinals is still a [countable ordinal](#countable-ordinal), so no countable sequence is cofinal in $\omega_1$.

#### Tail of the first uncountable ordinal

↑ **Parent:** [First uncountable ordinal](#first-uncountable-ordinal)

Deleting any countable initial segment from $\omega_1$ leaves a well-order of type $\omega_1$.

### Second uncountable ordinal

↑ **Parent:** [Ordinal](#ordinal)

The second uncountable ordinal $\omega_2$ is the least ordinal whose [cardinal number](#cardinal-number) is strictly larger than that of the [first uncountable ordinal](#first-uncountable-ordinal) $\omega_1$. Equivalently, it is the initial ordinal of the successor cardinal $\aleph_2$.

### Cantor normal form

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cantor_normal_form)

Every nonzero ordinal has a unique finite expression $\omega^{\delta_1}n_1+\cdots+\omega^{\delta_r}n_r$ with decreasing exponents and positive finite coefficients.

#### Generalized Cantor normal form

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

For every [ordinal](#ordinal) base $\rho>1$, a nonzero ordinal has a unique finite [ordinal addition](#ordinal-addition) expansion with strictly decreasing exponents $\beta_i$ and coefficients $0<\xi_i<\rho$. Choose the largest power at most the remaining ordinal and apply the [ordinal division algorithm](#ordinal-division-algorithm). The next remainder has smaller leading exponent, so [well-foundedness](#well-founded-relation) forces termination. Each lower tail is smaller than its preceding power; uniqueness of division consequently fixes the exponent, coefficient and tail successively. For $\rho=\omega$ this is [Cantor normal form](#cantor-normal-form).

#### Commensurable ordinals

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

Two [ordinals](#ordinal) are commensurable when neither is absorbed by adding the other on its left. For positive ordinals, this is equivalent to equality of their leading [Cantor normal form](#cantor-normal-form) exponent. If leading exponents differ, the lower-leading ordinal is absorbed by the higher power of $\omega$. If they agree, either sum adds the two positive leading coefficients and therefore exceeds both original ordinals. Zero is commensurable with no ordinal.

#### Computable Cantor normal form notation

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

Finite canonical terms built from zero, [ordinal](#ordinal) sums and powers of omega describe exactly the [ordinals](#ordinal) below [epsilon zero](#epsilon-zero). Syntactic validity and comparison are decidable by recursion through the exponent subterms. Enumerating valid term codes transfers their order to a [computable well-order](set.md#decidable-well-order) on all [natural numbers](arithmetic.md#natural-number).

##### Slow well-ordering below epsilon zero

↑ **Parent:** [Computable Cantor normal form notation](#computable-cantor-normal-form-notation)

Use the unary [Cantor normal form](#cantor-normal-form) tree norm, counting one root and recursively counting all repeated exponent subterms. There are only finitely many notations of bounded norm. This finite principle bounds all descending sequences whose norms grow at most linearly with the position. [Friedman's finite form of Kruskal's theorem](set.md#friedman-s-finite-form-of-kruskal-s-theorem) implies it through the [natural-sum ordinal rank of a finite rooted tree](combinatorics.md#natural-sum-ordinal-rank-of-a-finite-rooted-tree). The Friedman–Smith miniaturization theorem turns this controlled termination principle for standard epsilon-zero notations into the [formal consistency statement](mathematical-logic.md#formal-consistency-statement) for [Peano arithmetic](mathematical-logic.md#peano-arithmetic); the technical ordinal-analysis result is needed in addition to the tree coding. Section 2.2 of [https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf](https://formal.hknu.ac.kr/Publi/kruskalJKMS.pdf) records the general miniaturization and soundness theorem.

#### Leading term of an ordinal

↑ **Parent:** [Cantor normal form](#cantor-normal-form)

The leading term $\omega^\delta n$ is the highest-exponent term in Cantor normal form; the remaining tail is strictly below $\omega^\delta$.

##### Greatest power of omega below an ordinal

↑ **Parent:** [Leading term of an ordinal](#leading-term-of-an-ordinal)

Every nonzero ordinal $\alpha$ has a greatest exponent $\beta$ such that $\omega^\beta\leq\alpha$. It is the leading exponent in the [Cantor normal form](#cantor-normal-form) of $\alpha$, and

$$
\alpha=\omega^\beta n+\gamma
$$

for a positive finite integer $n$ and $\gamma<\omega^\beta$.

##### Leading exponent of an ordinal product

↑ **Parent:** [Leading term of an ordinal](#leading-term-of-an-ordinal)

Let nonzero ordinals $\xi,\eta$ have leading exponents $\rho,\sigma$. If $\eta$ is finite, then $\xi\eta$ has leading exponent $\rho$. If $\eta$ is infinite, so that $\sigma>0$, then $\xi\eta$ has leading exponent $\rho+\sigma$. This follows by multiplying the leading terms in [Cantor normal form](#cantor-normal-form) and using continuity of [ordinal multiplication](#ordinal-multiplication) at limit ordinals.

### Additively indecomposable ordinal

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additively_indecomposable_ordinal)

The additively indecomposable ordinals are exactly the powers $\omega^\delta$.

#### Additively closed ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

A nonzero ordinal $\delta$ is additively closed when $\beta+\gamma<\delta$ for all $\beta,\gamma<\delta$. These are exactly the ordinals $\omega^\alpha$: sufficiency follows from [Cantor normal form](#cantor-normal-form), while necessity follows by splitting any leading coefficient or nonzero tail below $\delta$ into two smaller summands.

#### Division by an additively indecomposable ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

For every ordinal $\gamma$ and $\lambda=\omega^\alpha$, there are unique ordinals $\beta,\delta$ such that

$$
\gamma=\lambda\beta+\delta,
\qquad \delta<\lambda.
$$

Choose the greatest initial multiple $\lambda\beta\leq\gamma$; if its remainder were at least $\lambda$, the next multiple would still fit. Uniqueness follows because every remainder below $\lambda$ lies before $\lambda(\beta+1)$.

#### Multiplicatively closed ordinal

↑ **Parent:** [Additively indecomposable ordinal](#additively-indecomposable-ordinal)

An ordinal $\delta>2$ is multiplicatively closed when $\beta\gamma<\delta$ for all $\beta,\gamma<\delta$. These are exactly

$$
\delta=\omega^{\omega^\alpha}.
$$

##### Multiplicative closure criterion for a power of omega

↑ **Parent:** [Multiplicatively closed ordinal](#multiplicatively-closed-ordinal)

For nonzero $\lambda$, the ordinal $\omega^\lambda$ is [multiplicatively closed](#multiplicatively-closed-ordinal) exactly when $\lambda$ is [additively closed](#additively-closed-ordinal). One direction follows from

$$
\omega^\rho\omega^\sigma=\omega^{\rho+\sigma}.
$$

For the other, the [leading exponent of an ordinal product](#leading-exponent-of-an-ordinal-product) shows that products of ordinals below $\omega^\lambda$ still have leading exponent below $\lambda$.

### Ordinal arithmetic

↑ **Parent:** [Ordinal](#ordinal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinal_arithmetic)

Ordinal arithmetic defines addition, multiplication and exponentiation of [ordinals](#ordinal) through order types or [transfinite recursion](#transfinite-recursion). The usual operations need not be commutative. Natural sum and natural product instead combine [Cantor normal forms](#cantor-normal-form) and are commutative; the [Hessenberg natural sum](#hessenberg-natural-sum) is the natural addition operation.

#### Fundamental sequence of a limit ordinal

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

For a countable limit [ordinal](#ordinal), a fundamental sequence is an increasing cofinal sequence of smaller ordinals. Effective choices allow a [fast-growing hierarchy](#fast-growing-hierarchy) to turn limit recursion into recursion at a finite input. Below [epsilon zero](#epsilon-zero), write the final term as $\gamma+\omega^\beta$. For successor $\beta=\delta+1$, take $\gamma+\omega^\delta(n+1)$; for nonzero limit $\beta$, take $\gamma+\omega^{\beta[n]}$. Earlier terms in the [Cantor normal form](#cantor-normal-form) remain fixed.

#### Fast-growing hierarchy

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

A fast-growing hierarchy indexes number-theoretic [functions](function.md) by an effective system of [ordinal](#ordinal) notations. Successor stages iterate the preceding function, while limit stages diagonalize along a chosen [fundamental sequence of a limit ordinal](#fundamental-sequence-of-a-limit-ordinal). These choices are part of the definition. With the standard [Cantor normal form](#cantor-normal-form) sequences below [epsilon zero](#epsilon-zero), each fixed $F_\alpha$ for $\alpha<\varepsilon_0$ is provably total in [Peano arithmetic](mathematical-logic.md#peano-arithmetic), but the uniform endpoint $F_{\varepsilon_0}$ is not. Every function provably total in [Peano arithmetic](mathematical-logic.md#peano-arithmetic) is eventually bounded by some lower level. These classification results are proved in [https://epub.ub.uni-muenchen.de/3843/1/3843.pdf](https://epub.ub.uni-muenchen.de/3843/1/3843.pdf) .

##### Eventual dominance in a fast-growing hierarchy

↑ **Parent:** [Fast-growing hierarchy](#fast-growing-hierarchy)

For the standard [fundamental sequences of limit ordinals](#fundamental-sequence-of-a-limit-ordinal) below [epsilon zero](#epsilon-zero), the index order corresponds to eventual, rather than necessarily pointwise, growth. For example, under $\omega[n]=n+1$ and successor iteration $n+1$ times, $F_\omega(1)=F_2(1)=7$ whereas $F_3(1)=2047$. Limit stages are diagonal choices, so a larger index can give a smaller value at small arguments.

#### Hessenberg natural sum

↑ **Parent:** [Ordinal arithmetic](#ordinal-arithmetic)

The Hessenberg natural sum aligns equal exponents in two Cantor normal forms and adds their finite coefficients; unlike ordinal addition it is commutative.

It is the commutative natural addition operation in [ordinal arithmetic](#ordinal-arithmetic).

##### Shuffle bound for ordinal partitions

↑ **Parent:** [Hessenberg natural sum](#hessenberg-natural-sum)

If a well-order is the union of suborders of types $\xi$ and $\eta$, its type is at most $\xi\mathbin\#\eta$.

###### Ordinal partition bound

↑ **Parent:** [Shuffle bound for ordinal partitions](#shuffle-bound-for-ordinal-partitions)

If an ordinal is partitioned into two copies of type $\beta$, its type is below $\beta+\beta+\beta$; two copies do not always give a strict bound.

## Inner model

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_model)

An inner model is a transitive class containing every [ordinal](#ordinal) and satisfying the specified axioms of set theory with the inherited membership relation.

### Constructible-universe obstruction to a uniform inner-model proof of failure of choice

↑ **Parent:** [Inner model](#inner-model)

Every [inner model](#inner-model) $N$ of [ZF](#zermelo-fraenkel-set-theory) contains the ambient [constructible universe](definable-power-set.md#constructible-universe) $L$. By induction, $L_\alpha^N=L_\alpha$: at successor stages, satisfaction in the same [set](set.md) structure and definability with parameters are absolute; at limits both constructions take the same [union](set.md#set-union). Thus, if the ambient universe satisfies $V=L$, its only inner model of [ZF](#zermelo-fraenkel-set-theory) is itself, and it satisfies the [axiom of choice](#axiom-of-choice). A procedure that must produce a choice-failing inner model from every model of [ZF](#zermelo-fraenkel-set-theory) is therefore impossible. This does not assert that arbitrary inner models of arbitrary choice universes satisfy choice; the obstruction concerns a uniform construction.

## Descriptive set theory

↑ **Parent:** [Set theory](set-theory.md)

[This section is present in another page, follow this link to view it.](descriptive-set-theory.md)

## Filter (set theory)

↑ **Parent:** [Set theory](set-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Filter_(set_theory))

A filter $\mathcal F$ on a set $X$ is a nonempty family of subsets that excludes the empty set, is closed under finite intersections, and is upward closed under inclusion.

### Pushforward filter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

For a [function](function.md) $f:X\to Y$, the pushforward of a [filter on a set](#filter-set-theory) $X$ consists of the [subsets](set.md#subset) $B\subseteq Y$ with $f^{-1}(B)\in\mathcal F$. [Preimages](#preimage) preserve inclusions and finite [intersections](set.md#set-intersection), so this is a proper filter. Equivalently it is generated by $f(A)$ for $A\in\mathcal F$. Because preimages preserve complements too, the pushforward of an [ultrafilter](#ultrafilter) is an [ultrafilter](#ultrafilter).

### Convergence of a filter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

A [filter on a set](#filter-set-theory) equipped with a [topology](topology.md) converges to $x$ if it contains every [neighbourhood](topology.md#neighbourhood-mathematics) of $x$. A [Hausdorff space](topology.md#hausdorff-space) gives every convergent filter at most one limit: disjoint neighbourhoods of distinct purported limits would have empty intersection in the filter.

### Addition of filters on the natural numbers

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

For proper filters on positive integers, define $A\in\mathcal F+\mathcal G$ when $\{x:A-x\in\mathcal G\}\in\mathcal F$. This is again a proper filter. The inner truth-set map preserves the whole set, the empty set, inclusions and finite intersections; applying the outer filter gives all filter axioms. The order of the two filter quantifiers is part of the definition and is not silently interchangeable.

### Filter quantifier

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

For a proper [filter on a set](#filter-set-theory), write $\forall_{\mathcal F}x\,p(x)$ when the truth set $\{x:p(x)\}$ belongs to the filter. This quantifier preserves finite conjunctions. For an [ultrafilter](#ultrafilter) it also preserves finite disjunctions and obeys classical negation; a general proper filter need not have those latter properties.

#### Boolean failure of the cofinite-filter quantifier

↑ **Parent:** [Filter quantifier](#filter-quantifier)

The even and odd integers are both absent from the [cofinite filter](#cofinite-filter), but their union is present. Thus its [filter quantifier](#filter-quantifier) need not turn a disjunction into the disjunction of quantified assertions, and failure of a quantified assertion need not imply truth of its quantified negation. An [ultrafilter](#ultrafilter) restores both laws by deciding each set against its complement.

#### Conjunction law for filter quantifiers

↑ **Parent:** [Filter quantifier](#filter-quantifier)

The [filter quantifier](#filter-quantifier) satisfies $\forall_{\mathcal F}(p\wedge q)$ if and only if both $\forall_{\mathcal F}p$ and $\forall_{\mathcal F}q$. Finite-intersection closure gives one direction and upward closure gives the other. Properness ensures contradictory truth sets cannot both be filter members.

### Free filter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

A free [filter on a set](#filter-set-theory) $I$ has empty intersection of all its members. This is equivalent to containing every cofinite subset of $I$: for each $i$ some filter member omits $i$, so upward closure gives $I\setminus\{i\}$, and finite intersections give every cofinite set. A proper free filter on an infinite set contains no finite set.

#### Membership in a free filter is detected by its ultrafilter extensions

↑ **Parent:** [Free filter](#free-filter)

For a [free filter](#free-filter) $F$, a subset $S$ belongs to $F$ if and only if every [ultrafilter](#ultrafilter) extending $F$ contains $S$. If $S\notin F$, every $A\in F$ meets $I\setminus S$ in an infinite set; otherwise a cofinite restriction of $A$ would be contained in $S$. Adjoining $I\setminus S$ therefore generates a proper free filter. The [ultrafilter lemma](#ultrafilter-lemma) extends it to a [nonprincipal ultrafilter](#nonprincipal-ultrafilter) witnessing failure of membership.

### Kappa-complete filter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)

A filter is $\kappa$-complete when the intersection of every family of fewer than $\kappa$ members again belongs to the filter.

#### Cobounded filter on a regular cardinal

↑ **Parent:** [Kappa-complete filter](#kappa-complete-filter)

The cobounded filter on a regular cardinal $\kappa$ consists of sets whose complements have cardinality below $\kappa$. Regularity makes it $\kappa$-complete.

### Cofinite filter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cofinite_filter)

The cofinite filter on an infinite set consists of all subsets whose complements are finite.

#### Cofinite set

↑ **Parent:** [Cofinite filter](#cofinite-filter)

A subset $E$ of a [set](set.md) $X$ is cofinite in $X$ when its complement $X\setminus E$ is a [finite set](set.md#finite-set). For infinite $X$, the cofinite subsets form the [cofinite filter](#cofinite-filter). A [nonprincipal ultrafilter](#nonprincipal-ultrafilter) on $\mathbb N$ contains every cofinite subset: it contains no singleton, hence no [finite set](set.md#finite-set), and decides between each [set](set.md) and its complement.

### Ultrafilter lemma

↑ **Parent:** [Filter (set theory)](#filter-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrafilter_lemma)

Every proper [filter on a set](#filter-set-theory) is contained in an [ultrafilter](#ultrafilter). Order its proper filter extensions by inclusion, use [Zorn lemma](#zorn-s-lemma) to obtain a maximal extension, and observe that maximality forces it to contain exactly one of every set and its complement.

#### Ultrafilter selection from a partition-rich family

↑ **Parent:** [Ultrafilter lemma](#ultrafilter-lemma)

Let $S$ be a nonempty [set](set.md) and $\mathscr P\subseteq\mathcal P(S)$ be upward closed. An [ultrafilter](#ultrafilter) all of whose members lie in $\mathscr P$ exists exactly when every finite [set partition](combinatorics.md#set-partition) of $S$ has a cell in $\mathscr P$. For sufficiency, the complements of sets outside $\mathscr P$ have the [finite intersection property](topology.md#finite-intersection-property): a finite cover by such sets could be disjointified into a partition with no cell in $\mathscr P$. The [ultrafilter lemma](#ultrafilter-lemma) extends the generated proper [filter](#filter-set-theory). Necessity follows because an [ultrafilter](#ultrafilter) selects exactly one cell of every finite partition. This criterion requires partition richness of the whole ground set; it does not assert that the complement family is closed under unions.

### Ultrafilter

↑ **Parent:** [Filter (set theory)](#filter-set-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrafilter)

An ultrafilter on a set $X$ is a proper [filter on a set](#filter-set-theory) that contains exactly one of $A$ and $X\setminus A$ for every $A\subseteq X$.

#### Fine ultrafilter

↑ **Parent:** [Ultrafilter](#ultrafilter)

An [ultrafilter](#ultrafilter) on $P_\kappa(\lambda)$ is fine when it contains the set of small subsets containing $\alpha$, for each $\alpha<\lambda$. Fineness makes every coordinate of $\lambda$ represented in the corresponding [ultrapower](foundations-of-mathematics.md#ultrapower), though no one small subset is required to contain every coordinate.

##### Normal ultrafilter on small subsets

↑ **Parent:** [Fine ultrafilter](#fine-ultrafilter)

An [ultrafilter](#ultrafilter) $U$ on $P_\kappa(\lambda)$ is normal when each [function](function.md) with $f(x)\in x$ on a $U$-large set is constant on a $U$-large subset. This is the small-subset version of normality; together with fineness and [kappa-completeness](#kappa-complete-filter) it gives the measure characterization of a [supercompact cardinal](#supercompact-cardinal).

#### Normal ultrafilter on a cardinal

↑ **Parent:** [Ultrafilter](#ultrafilter)

A uniform [kappa-complete](#kappa-complete-filter) [ultrafilter](#ultrafilter) $U$ on an uncountable cardinal $\kappa$ is normal if every regressive function on a $U$-large set is constant on a $U$-large subset. Equivalently it is closed under diagonal intersections $\Delta_{\alpha<\kappa}X_\alpha=\{\beta<\kappa:(\forall\alpha<\beta)\ \beta\in X_\alpha\}$. Normality supplies homogeneous sets for pair-colourings by combining the chosen large tail at each earlier coordinate.

#### Ultrafilter with arithmetic-progression-rich members

↑ **Parent:** [Ultrafilter](#ultrafilter)

An [ultrafilter](#ultrafilter) on the [positive integers](number-theory.md#positive-integer) with every member containing finite [arithmetic progressions](arithmetic.md#arithmetic-progression) of arbitrarily large length. The [Van der Waerden theorem](ramsey-theory.md#van-der-waerden-theorem) and [ultrafilter selection from a partition-rich family](#ultrafilter-selection-from-a-partition-rich-family) give existence. Such an [ultrafilter](#ultrafilter) must contain the complement of every set with bounded arithmetic-progression length, and it is a [nonprincipal ultrafilter](#nonprincipal-ultrafilter). No corresponding [ultrafilter](#ultrafilter) can have an infinite [arithmetic progression](arithmetic.md#arithmetic-progression) in every member, by the [dyadic block obstruction to infinite arithmetic progressions](arithmetic.md#dyadic-block-obstruction-to-infinite-arithmetic-progressions).

#### Ultrafilter with finite-sums members

↑ **Parent:** [Ultrafilter](#ultrafilter)

An ultrafilter with finite-sums members is an [ultrafilter](#ultrafilter) on the [positive integers](number-theory.md#positive-integer) all of whose members are [IP sets](ramsey-theory.md#ip-set). Such an [ultrafilter](#ultrafilter) exists by extending the [IP-star filter](ramsey-theory.md#ip-star-filter) using the [ultrafilter lemma](#ultrafilter-lemma). If a member were not IP, its complement would be an [IP-star set](ramsey-theory.md#ip-star-set) and hence another member, contradicting properness. Conversely, every such ultrafilter contains the entire IP-star filter, since it cannot contain the non-IP complement of an IP-star set. This characterization does not assert that the ultrafilter is idempotent.

#### Number of ultrafilters on an infinite set

↑ **Parent:** [Ultrafilter](#ultrafilter)

The [finite-trace independent family construction](#fichtenholz-kantorovich-independent-family) gives $2^{|X|}$ independent subsets of an infinite $X$. Each binary assignment generates a proper filter and, in [ZFC](#zermelo-fraenkel-set-theory-with-choice), has an ultrafilter extension. Different assignments force incompatible membership decisions, giving $2^{2^{|X|}}$ distinct ultrafilters. The matching upper bound follows because every ultrafilter is a subset of $\mathcal P(X)$.

#### Pushforward ultrafilter

↑ **Parent:** [Ultrafilter](#ultrafilter)

For an [ultrafilter](#ultrafilter) $U$ on $X$ and a [function](function.md) $g:X\to Y$, define $g_*U=\{B\subseteq Y:g^{-1}[B]\in U\}$. This is an [ultrafilter](#ultrafilter) and inherits countable completeness from a [countably complete ultrafilter](#countably-complete-ultrafilter). It is nonprincipal exactly when no single fibre of $g$ belongs to $U$. Restricting $U$ to a member of $U$ before pushing forward preserves these properties.

#### Fubini product of ultrafilters

↑ **Parent:** [Ultrafilter](#ultrafilter)

For [ultrafilters](#ultrafilter) $\mathcal U$ on $I$ and $\mathcal V$ on $J$, put

$$
A\in\mathcal U\otimes\mathcal V\quad\Longleftrightarrow\quad\{i\in I:\{j\in J:(i,j)\in A\}\in\mathcal V\}\in\mathcal U.
$$

This is an [ultrafilter](#ultrafilter) on $I\times J$: upward closure and finite intersection follow at both levels, and the [ultrafilter](#ultrafilter) dichotomy follows by complementing at both levels. Iterating gives ordered finite products. Projection onto a subsequence of coordinates pushes this product to the product on that subsequence, since omitted coordinates are absent from the tested [first-order formula](mathematical-logic.md#first-order-formula). The order of coordinates matters; these products need not be symmetric.

#### Ultrafilter functor

↑ **Parent:** [Ultrafilter](#ultrafilter)

The ultrafilter functor sends a set $A$ to its set $\mathcal U(A)$ of ultrafilters. A function $f:A\to B$ acts by pushforward,

$$
f_*U=\{C\subseteq B:f^{-1}(C)\in U\}.
$$

It preserves finite coproducts: an ultrafilter on $A\sqcup B$ contains exactly one summand and is uniquely induced by an ultrafilter on that summand.

##### Terminal finite-coproduct-preserving set endofunctor

↑ **Parent:** [Ultrafilter functor](#ultrafilter-functor)

The [ultrafilter functor](#ultrafilter-functor) is terminal among endofunctors of $\mathbf{Set}$ that preserve finite coproducts. For such an endofunctor $F$ and $x\in F(A)$, the unique natural map sends $x$ to

$$
\{B\subseteq A:x\in\operatorname{im}(F(B)\to F(A))\}.
$$

#### Principal ultrafilter

↑ **Parent:** [Ultrafilter](#ultrafilter)

The principal ultrafilter at $x\in X$ is $\{A\subseteq X:x\in A\}$. An ultraproduct by a principal ultrafilter is isomorphic to the factor indexed by $x$.

#### Nonprincipal ultrafilter

↑ **Parent:** [Ultrafilter](#ultrafilter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonprincipal_ultrafilter)

A nonprincipal ultrafilter contains no finite set. On an infinite set it contains the [cofinite filter](#cofinite-filter).

##### Small set is absent from a complete nonprincipal ultrafilter

↑ **Parent:** [Nonprincipal ultrafilter](#nonprincipal-ultrafilter)

If $U$ is a nonprincipal $\kappa$-complete ultrafilter on $X$ and $A\subseteq X$ has cardinality below $\kappa$, then $A\notin U$. Indeed, every $X\setminus\{a\}$ belongs to $U$, so $\kappa$-completeness puts their intersection $X\setminus A$ in $U$.

#### Countably complete ultrafilter

↑ **Parent:** [Ultrafilter](#ultrafilter)

An ultrafilter is countably complete when the intersection of every countable family of its members again belongs to it. Equivalently, whenever the underlying set is partitioned into countably many pieces, exactly one piece belongs to the ultrafilter.

<h4 id="stone-cech-compactification-of-the-natural-numbers">Stone-Čech compactification of the natural numbers</h4>

↑ **Parent:** [Ultrafilter](#ultrafilter)

The Stone-Cech compactification $\beta\mathbb N$ can be identified with the space of ultrafilters on $\mathbb N$. Its basic clopen sets are $\bar A=\{\mathcal U:A\in\mathcal U\}$.

This is the natural-number-space case of [Stone-Čech compactification](physics.md#stone-cech-compactification).

<h5 id="no-nontrivial-convergent-sequences-in-the-stone-cech-compactification">No nontrivial convergent sequences in the Stone-Čech compactification</h5>

↑ **Parent:** [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers)

Every [convergent sequence](real-analysis.md#convergent-sequence) in the [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers) is eventually constant. If distinct [ultrafilters](#ultrafilter) $U_n$ converged, isolate each from the other sequence terms using convergence and finitely many separating [clopen sets](topology.md#clopen-set). Finite disjointification gives disjoint $B_n\in U_n$. The union of the even-indexed $B_n$ then belongs exactly to the even-indexed [ultrafilters](#ultrafilter), contradicting convergence of membership in a [clopen set](topology.md#clopen-set).

##### Compact Hausdorff topology on ultrafilters

↑ **Parent:** [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers)

For $A\subseteq\mathbb N$, the basic set $\widehat A=\{U:A\in U\}$ in the [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers) is a [clopen set](topology.md#clopen-set), since its complement is $\widehat{\mathbb N\setminus A}$. Distinct [ultrafilters](#ultrafilter) are separated by complementary basic sets. A basic cover with no finite subcover would give complements with the [finite intersection property](topology.md#finite-intersection-property), whose generated [filter on a set](#filter-set-theory) extends to an [ultrafilter](#ultrafilter) missing the entire cover. Thus the space is a [compact Hausdorff space](topology.md#compact-hausdorff-space).

<h5 id="addition-on-the-stone-cech-compactification-of-the-natural-numbers">Addition on the Stone-Čech compactification of the natural numbers</h5>

↑ **Parent:** [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers)

For ultrafilters $\mathcal U,\mathcal V\in\beta\mathbb N$, define $\mathcal U+\mathcal V$ by

$$
A\in\mathcal U+\mathcal V
\quad\Longleftrightarrow\quad
\{x:\{y:x+y\in A\}\in\mathcal V\}\in\mathcal U.
$$

This operation is [associative](algebra.md#associative-operation), and each right translation $\mathcal U\mapsto\mathcal U+\mathcal V$ is continuous, so $\beta\mathbb N$ is a compact Hausdorff left-topological [semigroup](algebra.md#semigroup).

###### Idempotent ultrafilter

↑ **Parent:** [Addition on the Stone-Čech compactification of the natural numbers](#addition-on-the-stone-cech-compactification-of-the-natural-numbers)

An additive idempotent [ultrafilter](#ultrafilter) satisfies $\mathcal U+\mathcal U=\mathcal U$. On positive integers it is necessarily nonprincipal, since a principal ultrafilter at $n$ adds to itself to give the principal ultrafilter at $2n$. The [idempotent-ultrafilter star-set lemma](#idempotent-ultrafilter-star-set-lemma) converts this algebraic property into a recursive construction of finite sums. If zero is included, the trivial principal idempotent at zero must be excluded for that increasing-sequence application.

###### Tail finite-sums semigroup

↑ **Parent:** [Idempotent ultrafilter](#idempotent-ultrafilter)

For a sequence of positive integers, the nested closures of its tail [finite-sums sets](ramsey-theory.md#finite-sums-set) have nonempty compact intersection in the [Stone-Čech compactification of the natural numbers](#stone-cech-compactification-of-the-natural-numbers). This intersection is a [subsemigroup](algebra.md#subsemigroup). For a sum $s$ from one tail, all sums supported beyond a chosen finite representation of $s$ lie in that tail translated by $-s$. The [ultrafilter](#ultrafilter) addition formula then establishes closure under addition. The [Ellis–Numakura lemma](algebra.md#ellis-numakura-lemma) supplies an [idempotent ultrafilter](#idempotent-ultrafilter) containing every tail finite-sums set and hence any set containing the full [finite-sums set](ramsey-theory.md#finite-sums-set).

###### Zero-residue constraint for idempotent ultrafilters

↑ **Parent:** [Idempotent ultrafilter](#idempotent-ultrafilter)

An [ultrafilter](#ultrafilter) on the positive integers selects exactly one [residue class](number-theory.md#residue-class) modulo a fixed positive integer $q$. Under [addition on the Stone-Čech compactification of the natural numbers](#addition-on-the-stone-cech-compactification-of-the-natural-numbers), selected residues add. An [idempotent ultrafilter](#idempotent-ultrafilter) must therefore select a residue $r$ with $2r=r$ in the finite cyclic group, hence $r=0$. In particular, the multiples of every fixed positive integer belong to every additive [idempotent ultrafilter](#idempotent-ultrafilter).

###### Idempotent-ultrafilter star-set lemma

↑ **Parent:** [Idempotent ultrafilter](#idempotent-ultrafilter)

For $A\in\mathcal U$ and an [idempotent ultrafilter](#idempotent-ultrafilter), put $A^*=\{n\in A:A-n\in\mathcal U\}$. Then $A^*\in\mathcal U$, and $A^*-n\in\mathcal U$ for every $n\in A^*$. For the second assertion, apply idempotence to $A-n$ and intersect its resulting good-translation set with $A-n$. This allows each new finite-sums generator to be chosen from finitely many translation constraints, proving the [Idempotent-ultrafilter proof of Hindman's theorem](ramsey-theory.md#idempotent-ultrafilter-proof-of-hindman-s-theorem).

###### Idempotent ultrafilter on the natural numbers

↑ **Parent:** [Addition on the Stone-Čech compactification of the natural numbers](#addition-on-the-stone-cech-compactification-of-the-natural-numbers)

An ultrafilter $\mathcal U\in\beta\mathbb N$ is idempotent when $\mathcal U+\mathcal U=\mathcal U$. The [Ellis–Numakura lemma](algebra.md#ellis-numakura-lemma) guarantees such an ultrafilter and supplies the main algebraic input to the [Idempotent-ultrafilter proof of Hindman's theorem](ramsey-theory.md#idempotent-ultrafilter-proof-of-hindman-s-theorem).

#### Ultralimit

↑ **Parent:** [Ultrafilter](#ultrafilter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultralimit)

A point $x$ is the limit of a map $f:I\to X$ along an ultrafilter $\mathcal U$ on $I$ when $f^{-1}(V)\in\mathcal U$ for every [neighbourhood](topology.md#neighbourhood-mathematics) $V$ of $x$. Every ultrafilter on a [compact space](topology.md#compact-space) has a limit, and that limit is unique in a [Hausdorff space](topology.md#hausdorff-space).

##### Ultrafilter characterization of compact Hausdorff spaces

↑ **Parent:** [Ultralimit](#ultralimit)

A [topological space](topology.md#topological-space) is both a [compact space](topology.md#compact-space) and a [Hausdorff space](topology.md#hausdorff-space) exactly when every [ultrafilter](#ultrafilter) on its underlying [set](set.md) converges to exactly one point. Existence of all ultrafilter limits characterizes compactness. If a space is not Hausdorff, two distinct points have neighbourhood systems whose combined finite intersections are nonempty; the [ultrafilter lemma](#ultrafilter-lemma) extends these to an ultrafilter converging to both points. Conversely, disjoint neighbourhoods prevent such a common limit.

## ↑ Ancestors (4)

1. [Foundations of mathematics](foundations-of-mathematics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-25.md#2/solution)
- [Standard model (set theory)](#standard-model-set-theory)
- [Zermelo set theory](#zermelo-set-theory)
