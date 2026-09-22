# Definable power set

↑ **Parent:** [Set theory](set-theory.md)

The definable power set $\mathcal D(X)=\operatorname{Def}(X)$ consists of the [subsets](set.md#subset) of $X$ definable over the [first-order structure](mathematical-logic.md#first-order-structure) $(X,\in)$ by a [first-order formula](mathematical-logic.md#first-order-formula) with parameters from $X$. [Satisfaction for a set structure](mathematical-logic.md#satisfaction-for-a-set-structure) makes this a definable operation in [ZF](set-theory.md#zermelo-fraenkel-set-theory). Iterating it produces the [constructible hierarchy](#constructible-hierarchy) and the [relative constructible hierarchy](#relative-constructible-hierarchy); their unions are the [constructible universe](#constructible-universe) and the [relative constructible universe](#relative-constructible-universe).

**Table of contents**

- [Finite relation closure for set-theoretic coding](#finite-relation-closure-for-set-theoretic-coding)
- [Constructible hierarchy](#constructible-hierarchy)
  - [Constructible sets of low rank can appear at later stages](#constructible-sets-of-low-rank-can-appear-at-later-stages)
  - [Absoluteness of constructible levels](#absoluteness-of-constructible-levels)
    - [Constructible-level absoluteness over ZF](#constructible-level-absoluteness-over-zf)
  - [Constructible universe](#constructible-universe)
    - [Shepherdson's wall](#shepherdson-s-wall)
    - [Axiom of constructibility](#axiom-of-constructibility)
    - [Separation proof in the constructible universe](#separation-proof-in-the-constructible-universe)
    - [Constructible universe theorem](#constructible-universe-theorem)
    - [Diamond theorem in the constructible universe](#diamond-theorem-in-the-constructible-universe)
    - [Countability of constructible omega-one](#countability-of-constructible-omega-one)
    - [Hereditarily countable constructible sets appear below omega-one](#hereditarily-countable-constructible-sets-appear-below-omega-one)
    - [Constructible power set](#constructible-power-set)
    - [Relative constructible universe](#relative-constructible-universe)
      - [Inner models with all reals preserve omega-one](#inner-models-with-all-reals-preserve-omega-one)
      - [Relative constructible hierarchy](#relative-constructible-hierarchy)
        - [Relative condensation lemma](#relative-condensation-lemma)
        - [Relative constructible level recognition](#relative-constructible-level-recognition)
        - [Coded relative constructible stage](#coded-relative-constructible-stage)
          - [Stage histories appear below every limit constructible level](#stage-histories-appear-below-every-limit-constructible-level)
      - [Relative constructible universe can violate the continuum hypothesis](#relative-constructible-universe-can-violate-the-continuum-hypothesis)
  - [Condensation sentence for the constructible hierarchy](#condensation-sentence-for-the-constructible-hierarchy)
  - [Well-order code](#well-order-code)
  - [Coding level of the constructible hierarchy](#coding-level-of-the-constructible-hierarchy)
  - [Condensation lemma for the constructible universe](#condensation-lemma-for-the-constructible-universe)

## Finite relation closure for set-theoretic coding

↑ **Parent:** [Definable power set](definable-power-set.md)

A useful finite conjunction of closure assertions requires empty set, pairing, [set union](set.md#set-union), [set difference](set.md#set-difference), [Cartesian products](set-theory.md#cartesian-product), all finite tuple domains $A^n$, and the following operations on their relations: relative complements, intersections, coordinate projections and pullbacks along finite coordinate maps, together with equality and membership restricted to $A^2$. The arities and maps are quantified objects, so these requirements form finitely many [first-order formulas](mathematical-logic.md#first-order-formula), not an infinite schema. In a [transitive set](set-theory.md#transitive-set), individual finite tuples exist by pairing and union, making the tuple-domain assertions correct externally. Atomic truth relations, Boolean operations and projection then compute the truth table of each coded [first-order formula](mathematical-logic.md#first-order-formula) correctly by finite induction. Thus [satisfaction for a set structure](mathematical-logic.md#satisfaction-for-a-set-structure) and the relation $B=\operatorname{Def}(A)$ are absolute for shared arguments. Every nonzero limit level of the [relative constructible hierarchy](#relative-constructible-hierarchy) is closed under these operations, since each result can be defined at finitely many subsequent stages.

## Constructible hierarchy

↑ **Parent:** [Definable power set](definable-power-set.md)

The constructible hierarchy is defined by

$$
L_0=\varnothing,
\qquad L_{\alpha+1}=\mathcal D(L_\alpha),
\qquad L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha
$$

for limit ordinals $\lambda$. Its union is the constructible universe $L$.

### Constructible sets of low rank can appear at later stages

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

The equality $L\cap V_\alpha=L_\alpha$ can fail even at $\alpha=\omega+1$. Inside the [constructible universe](#constructible-universe), $L_\omega=V_\omega$ is countable, so its [definable power set](definable-power-set.md) $L_{\omega+1}$ is countable. The [constructible power set](#constructible-power-set) of $\omega$ is uncountable there by the [Cantor theorem](set.md#cantor-s-theorem). A real outside $L_{\omega+1}$ remains a constructible subset of $\omega$, hence belongs to $V_{\omega+1}$. The cardinal comparison must be made inside $L$, since its reals can be externally countable.

### Absoluteness of constructible levels

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

For a [transitive model](set-theory.md#transitive-model) $M$ of [ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice) and $\alpha\in M\cap\operatorname{Ord}$, the internally computed [constructible hierarchy](#constructible-hierarchy) agrees with the ambient level: $L_\alpha^M=L_\alpha$. Satisfaction for a fixed set structure is computed from the same finite formulas and the same domain in both universes. [Transfinite recursion](set-theory.md#transfinite-recursion) then proves agreement at successors and limits. If $\theta=M\cap\operatorname{Ord}$, it follows that $L_\theta\subseteq M$.

#### Constructible-level absoluteness over ZF

↑ **Parent:** [Absoluteness of constructible levels](#absoluteness-of-constructible-levels)

If $M$ is a [transitive model](set-theory.md#transitive-model) of [ZF](set-theory.md#zermelo-fraenkel-set-theory), its internally computed $L_\alpha$ is the actual $L_\alpha$ for each [ordinal](set-theory.md#ordinal) $\alpha\in M$. At a successor stage use absoluteness of satisfaction for the same [set](set.md) structure, formula codes and parameters; at a limit stage take the union of the already identical earlier stages. Choice is not required.

### Constructible universe

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constructible_universe)

The constructible universe is the [inner model](set-theory.md#inner-model) $L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha$ obtained by iterating the [definable power set](definable-power-set.md). It satisfies [ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice) and the [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis).

<h4 id="shepherdson-s-wall">Shepherdson's wall</h4>

↑ **Parent:** [Constructible universe](#constructible-universe)

The obstruction to proving the consistency of nonconstructibility by a uniform [inner model](set-theory.md#inner-model) construction is that, inside a universe satisfying $V=L$, every transitive inner model containing all ordinals has $L$ as its own constructible universe and therefore is the entire ambient universe. The [absoluteness of constructible levels](#absoluteness-of-constructible-levels) proves this by induction over successor definability and limit unions. Thus a construction valid in every model of [ZF](set-theory.md#zermelo-fraenkel-set-theory) cannot always produce such an inner model satisfying $V\ne L$, and in particular cannot always produce one violating [axiom of choice](set-theory.md#axiom-of-choice).

#### Axiom of constructibility

↑ **Parent:** [Constructible universe](#constructible-universe)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axiom_of_constructibility)

Every [set](set.md) belongs to some level of the [constructible hierarchy](#constructible-hierarchy). The assertion is $\forall x\,\exists\alpha\,(x\in L_\alpha)$, not that each set is definable without parameters. The [constructible universe theorem](#constructible-universe-theorem) supplies a relative-consistency model of this assertion from [ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice).

#### Separation proof in the constructible universe

↑ **Parent:** [Constructible universe](#constructible-universe)

To separate a [subset](set.md#subset) of a constructible [set](set.md) by a formula interpreted in the [constructible universe](#constructible-universe), apply the [reflection theorem for definable hierarchies](set-theory.md#reflection-theorem-for-definable-hierarchies) to the formula and its subformulas. At a sufficiently large reflecting level containing the parameters, the desired [subset](set.md#subset) is definable and belongs to the next [constructible hierarchy](#constructible-hierarchy) level. The reflection proof uses least witness stages and ambient [Axiom schema of replacement](set-theory.md#axiom-schema-of-replacement), so does not presuppose [Axiom schema of separation](set-theory.md#axiom-schema-of-specification) within the [constructible universe](#constructible-universe).

#### Constructible universe theorem

↑ **Parent:** [Constructible universe](#constructible-universe)

[ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice) proves that the [constructible universe](#constructible-universe) is an [inner model](set-theory.md#inner-model) of [ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice) and satisfies the [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis). Relativizing to $L$ yields the corresponding relative-consistency implication.

#### Diamond theorem in the constructible universe

↑ **Parent:** [Constructible universe](#constructible-universe)

The [constructible universe](#constructible-universe) satisfies the [diamond principle](set-theory.md#diamond-principle). Together with [antichain sealing by diamond](set-theory.md#antichain-sealing-by-diamond), this supplies a [Suslin tree](set.md#suslin-tree) in $L$.

#### Countability of constructible omega-one

↑ **Parent:** [Constructible universe](#constructible-universe)

This statement says that the [first uncountable ordinal of an inner model](descriptive-set-theory.md#first-uncountable-ordinal-of-an-inner-model) $L$ is a [countable ordinal](set-theory.md#countable-ordinal) in the ambient universe. It can hold together with the [Generalized continuum hypothesis](set-theory.md#generalized-continuum-hypothesis): start with constructibility and use a [finite-function collapse to countable size](forcing.md#finite-function-collapse-to-countable-size) on $\omega_1^L$. The [GCH preservation by a finite-function collapse](forcing.md#gch-preservation-by-a-finite-function-collapse) calculation gives the relative consistency result already from the consistency of [ZFC](set-theory.md#zermelo-fraenkel-set-theory-with-choice).

#### Hereditarily countable constructible sets appear below omega-one

↑ **Parent:** [Constructible universe](#constructible-universe)

Inside the [constructible universe](#constructible-universe), every [hereditarily countable set](set-theory.md#hereditarily-countable-set) appears in a countable level of the [constructible hierarchy](#constructible-hierarchy). Take a countable [elementary substructure](mathematical-logic.md#elementary-substructure) of a sufficiently large $L_\eta$ containing its [transitive closure](set-theory.md#transitive-closure) pointwise. The [condensation lemma for the constructible universe](#condensation-lemma-for-the-constructible-universe) identifies the collapse with $L_\beta$ for countable $\beta$, and the collapse fixes the original set. Conversely, a countable-indexed level is countable inside the [constructible universe](#constructible-universe).

#### Constructible power set

↑ **Parent:** [Constructible universe](#constructible-universe)

For $A\in L$, its constructible power set is

$$
\mathcal P^L(A)=\{X\in L:X\subseteq A\}=\mathcal P(A)\cap L.
$$

Unlike the single-stage [definable power set](definable-power-set.md) $\mathcal D(A)$, it includes subsets of $A$ appearing arbitrarily late in the [constructible hierarchy](#constructible-hierarchy).

#### Relative constructible universe

↑ **Parent:** [Constructible universe](#constructible-universe)

For a [transitive set](set-theory.md#transitive-set) $X$, the relative constructible universe $L(X)$ is the union of the [relative constructible hierarchy](#relative-constructible-hierarchy), starting at $L_0(X)=X$, applying the [definable power set](definable-power-set.md) at successors and taking unions at [limit ordinals](set-theory.md#limit-ordinal). It is the smallest [inner model](set-theory.md#inner-model) of [ZF](set-theory.md#zermelo-fraenkel-set-theory) containing $X$ and all its members. For an arbitrary [set](set.md) $A$, take the base $X$ to be the [transitive closure](set-theory.md#transitive-closure) of $\{A\}$, so that $A\in X$. [Axiom of choice](set-theory.md#axiom-of-choice) need not hold for an arbitrary base; the construction uses initial parameters rather than a predicate relativization.

##### Inner models with all reals preserve omega-one

↑ **Parent:** [Relative constructible universe](#relative-constructible-universe)

An [inner model](set-theory.md#inner-model) $W$ of [ZF](set-theory.md#zermelo-fraenkel-set-theory) containing all ambient [subsets](set.md#subset) of $\omega$ computes the same [countable ordinals](set-theory.md#countable-ordinal) as the ambient universe. Every ambient countably infinite [ordinal](set-theory.md#ordinal) has a [well-order code](#well-order-code) coded by a [subset](set.md#subset) of $\omega$, hence that code belongs to $W$; finite [ordinals](set-theory.md#ordinal) are already shared. The [Mostowski collapse theorem](set-theory.md#mostowski-collapse-theorem) inside $W$ recovers the actual [ordinal](set-theory.md#ordinal) and its countability witness. Conversely any countability witness in $W$ remains one outside. If $W$ also contains the full [power set](set.md#power-set) of $\omega$ as a [set](set.md), its [Continuum hypothesis](set-theory.md#continuum-hypothesis) would give an ambient [bijection](function.md#bijection) from $\omega_1$ onto that same [power set](set.md#power-set). Thus an ambient failure of this well-orderable formulation of the [Continuum hypothesis](set-theory.md#continuum-hypothesis) is preserved in such an inner model. No internal [axiom of choice](set-theory.md#axiom-of-choice) is required for this argument.

##### Relative constructible hierarchy

↑ **Parent:** [Relative constructible universe](#relative-constructible-universe)

For a [transitive set](set-theory.md#transitive-set) $X$, use $L_0(X)=X$, $L_{\alpha+1}(X)=\operatorname{Def}(L_\alpha(X))$ and unions at nonzero [limit ordinals](set-theory.md#limit-ordinal). The successor operation is the [definable power set](definable-power-set.md). Each level is transitive and the levels increase; moreover $X\in L_1(X)$. Their union is $L(X)$, an [inner model](set-theory.md#inner-model) of [ZF](set-theory.md#zermelo-fraenkel-set-theory). The initial-set convention differs from a hierarchy using a predicate, or one starting at $X\cup\{X\}$. [Axiom of choice](set-theory.md#axiom-of-choice) need not hold for an arbitrary base without an internally available [well-order](set.md#well-order).

###### Relative condensation lemma

↑ **Parent:** [Relative constructible hierarchy](#relative-constructible-hierarchy)

If $\alpha$ is a nonzero [limit ordinal](set-theory.md#limit-ordinal) and $Y\prec L_\alpha(X)$ with $X\cup\{X\}\subseteq Y$, the [Mostowski collapse theorem](set-theory.md#mostowski-collapse-theorem) sends $Y$ to $L_\beta(X)$ for some nonzero limit $\beta\leq\alpha$ and fixes $X$ pointwise. The base is fixed by transitivity and inclusion of all its members. Transfer the [relative constructible level recognition](#relative-constructible-level-recognition) formula first by elementarity and then through the collapse isomorphism to identify its image. If $\rho=X\cap\operatorname{Ord}$, ordinal heights are $\rho+\alpha$ and $\rho+\beta$, giving the bound. Having only $X\in Y$ does not guarantee this base-fixing version.

###### Relative constructible level recognition

↑ **Parent:** [Relative constructible hierarchy](#relative-constructible-hierarchy)

For [transitive sets](set-theory.md#transitive-set) $M,X$ with $X\in M$, a single [first-order formula](mathematical-logic.md#first-order-formula) $\Phi(X)$ recognises the nonzero limit levels $L_\alpha(X)$. Require [finite relation closure for set-theoretic coding](#finite-relation-closure-for-set-theoretic-coding), transitivity of $X$, that every element belongs to a [coded relative constructible stage](#coded-relative-constructible-stage), and that every represented stage index has a larger represented index. Correct history codes have downward-closed indices with no maximum, hence form a nonzero [limit ordinal](set-theory.md#limit-ordinal) $\alpha$. The exhaustion assertion and transitivity then give $M=\bigcup_{\xi<\alpha}L_\xi(X)$. Conversely every limit level has the required closure, correct histories cofinal in its index, and exhaustion. This formulation does not assume [ZF](set-theory.md#zermelo-fraenkel-set-theory) for an arbitrary input $M$ and does not replace finite coding closure with an unjustified internal constructibility assertion.

###### Coded relative constructible stage

↑ **Parent:** [Relative constructible hierarchy](#relative-constructible-hierarchy)

This [first-order formula](mathematical-logic.md#first-order-formula) asserts the existence of a history function on $\xi+1$ starting at $X$, applying [definable power set](definable-power-set.md) at successors and unions at nonzero [limit ordinals](set-theory.md#limit-ordinal), and ending at $B$. In a [transitive set](set-theory.md#transitive-set) satisfying [finite relation closure for set-theoretic coding](#finite-relation-closure-for-set-theoretic-coding), each history is correct by [transfinite induction](set-theory.md#transfinite-induction), so $B=L_\xi(X)$. Relation operations produce restrictions to shorter histories. Since [stage histories appear below every limit constructible level](#stage-histories-appear-below-every-limit-constructible-level), every history of length $\xi+1$ for $\xi<\alpha$ belongs to $L_\alpha(X)$ when $\alpha$ is a nonzero [limit ordinal](set-theory.md#limit-ordinal). This is the coding step behind [relative constructible level recognition](#relative-constructible-level-recognition).

###### Stage histories appear below every limit constructible level

↑ **Parent:** [Coded relative constructible stage](#coded-relative-constructible-stage)

For a [transitive set](set-theory.md#transitive-set) $X$, let $f_\xi$ be the history function $\eta\mapsto L_\eta(X)$ on $\xi+1$ in the [relative constructible hierarchy](#relative-constructible-hierarchy). By [transfinite induction](set-theory.md#transfinite-induction), $f_\xi\in L_{\xi+k}(X)$ for some finite $k$, possibly depending on $\xi$. The base and successor steps follow by forming finite [ordered pairs](set.md#ordered-pair) and adjoining the next entry, using $L_{\xi+1}(X)\in L_{\xi+2}(X)$. These operations require finitely many subsequent [definable power sets](definable-power-set.md).

At a nonzero [limit ordinal](set-theory.md#limit-ordinal) $\lambda$, the inductive bounds put every earlier $f_\eta$ in $L_\lambda(X)$, since $\eta+k<\lambda$. This level satisfies [finite relation closure for set-theoretic coding](#finite-relation-closure-for-set-theoretic-coding), independently of the availability of history functions. Consequently its [coded relative constructible stage](#coded-relative-constructible-stage) predicate computes the endpoints correctly. Finite pairing closure and the earlier histories show that

$$
h=\{\langle\eta,B\rangle\in L_\lambda(X):(L_\lambda(X),\in)\models S_X(\eta,B)\}
$$

contains exactly the pairs $\langle\eta,L_\eta(X)\rangle$ for $\eta<\lambda$. There are no extra indices: if $\eta\geq\lambda$ and $B=L_\eta(X)\in L_\lambda(X)$, increasing levels would give $B\in B$, contradicting [Axiom of foundation](set-theory.md#axiom-of-regularity). Thus $h=f_\lambda\!\upharpoonright\lambda$ is a definable [subset](set.md#subset) of $L_\lambda(X)$ and belongs to $L_{\lambda+1}(X)$. Extracting its domain $\lambda$ and adjoining $\langle\lambda,L_\lambda(X)\rangle$ uses finitely many further operations, proving the induction step. Every nonzero limit $\alpha$ therefore contains all $f_\xi$ with $\xi<\alpha$, as required by [relative constructible level recognition](#relative-constructible-level-recognition).

##### Relative constructible universe can violate the continuum hypothesis

↑ **Parent:** [Relative constructible universe](#relative-constructible-universe)

Assume a [transitive model](set-theory.md#transitive-model) $M$ satisfies $2^{\aleph_0}=\aleph_2$. In $M$, encode a bijection $e:\omega_2\to\mathcal P(\omega)$ by one set $A\subseteq\omega_2$, using a fixed pairing of $\omega_2\times\omega$ with $\omega_2$. Then $L(A)$ decodes $e$ and contains every real of $M$. The two models consequently have the same $\omega_1$, and any bijection between $\omega_1$ and the real numbers in $L(A)$ would also be one in $M$. Thus $L(A)\models\neg\mathsf{CH}$.

### Condensation sentence for the constructible hierarchy

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

A condensation sentence is a fixed first-order sentence $\sigma$ such that every transitive set satisfying $\sigma$ is $L_\lambda$ for a limit ordinal $\lambda$. It combines a sufficiently strong finite fragment of set theory, the assertion that every set is constructible, and the absence of a largest ordinal.

### Well-order code

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

A well-order code is a [binary relation](set-theory.md#binary-relation) $R\subseteq\omega\times\omega$ for which $(\omega,R)$ is a [well-order](set.md#well-order). Its representation is the unique [countable ordinal](set-theory.md#countable-ordinal) isomorphic to $(\omega,R)$.

### Coding level of the constructible hierarchy

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

A level $L_\lambda$ is a coding level when $\lambda$ is a [limit ordinal](set-theory.md#limit-ordinal), the representation of every [well-order code](#well-order-code) in $L_\lambda$ is below $\lambda$, and every [ordinal](set-theory.md#ordinal) below $\lambda$ has a well-order code in $L_\lambda$.

### Condensation lemma for the constructible universe

↑ **Parent:** [Constructible hierarchy](#constructible-hierarchy)

If $X$ is an elementary substructure of a sufficiently large level $L_\theta$, then the transitive collapse of $X$ is a level $L_\beta$. In particular, a countable $X$ collapses to a level indexed by a countable ordinal.

## ↑ Ancestors (5)

1. [Set theory](set-theory.md)
2. [Foundations of mathematics](foundations-of-mathematics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (17)

- [Coded relative constructible stage](#coded-relative-constructible-stage)
- [Constructible power set](#constructible-power-set)
- [Constructible sets of low rank can appear at later stages](#constructible-sets-of-low-rank-can-appear-at-later-stages)
- [Constructible universe](#constructible-universe)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-19.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-121.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-121.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-121.md#2/ii/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-121.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-128.md#1/a/i/solution)
- [Relative constructible hierarchy](#relative-constructible-hierarchy)
- [Relative constructible universe](#relative-constructible-universe)
- [Stage histories appear below every limit constructible level](#stage-histories-appear-below-every-limit-constructible-level)
