<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Gödel's completeness theorem](../../../../../godel-s-completeness-theorem.md) for [first-order sentences](../../../../../first-order-sentence.md) says that, in a standard sound first-order [Hilbert calculus](../../../../../hilbert-proof-system.md),

$$
\boxed{T\models\sigma\quad\Longrightarrow\quad T\vdash\sigma.}
$$

Equivalently every [first-order consistent](../../../../../first-order-consistency.md) [set](../../../../../set-split.md) of [first-order sentences](../../../../../first-order-sentence.md) has a [first-order model](../../../../../model-of-a-first-order-theory.md): apply this existence statement to $T\cup\{\neg\sigma\}$ for the consequence formulation.

For the [first-order model](../../../../../model-of-a-first-order-theory.md) existence [formal proof](../../../../../formal-proof.md) use a [Henkin construction](../../../../../henkin-construction.md). Enlarge the language by fresh [constant symbols](../../../../../constant-symbol.md) and adjoin [Henkin witness axioms](../../../../../henkin-witness-axiom.md)

$$
\exists x\theta(x)\to\theta(c_\theta).
$$

Freshness of $c_\theta$ preserves [first-order consistency](../../../../../first-order-consistency.md). In detail, if a contradiction followed after adjoining one witness [axiom](../../../../../axiom.md), the [deduction theorem for first-order logic](../../../../../deduction-theorem-for-first-order-logic.md) would yield its [negation](../../../../../negation.md), from which one obtains both $\exists x\theta(x)$ and $\neg\theta(c_\theta)$ over the old theory. Since the new [constant symbol](../../../../../constant-symbol.md) does not occur in that theory or in $\theta$, replace it by a fresh [logical variable](../../../../../logical-variable.md) and generalize to derive $\forall x\neg\theta(x)$, a contradiction. Finitely many witness additions preserve [first-order consistency](../../../../../first-order-consistency.md) successively, and [unions](../../../../../set-union.md) preserve [first-order consistency](../../../../../first-order-consistency.md) because [formal proofs](../../../../../formal-proof.md) are finite. Iterate the enlargement so that [logical formulas](../../../../../logical-formula.md) involving newly introduced [constant symbols](../../../../../constant-symbol.md) also receive witnesses. Include at least one [constant symbol](../../../../../constant-symbol.md) to guarantee [closed terms](../../../../../closed-term.md).

Extend the resulting [first-order consistent](../../../../../first-order-consistency.md) [witnessed first-order theory](../../../../../henkin-theory.md) to a [maximal consistent set of first-order sentences](../../../../../maximal-consistent-set-of-first-order-sentences.md) $H$. In the equality-free case make the domain the [set](../../../../../set-split.md) of [closed terms](../../../../../closed-term.md). Interpret [constant symbols](../../../../../constant-symbol.md) and [function symbols](../../../../../function-symbol.md) by their formal [first-order term](../../../../../first-order-term.md) constructions; interpret an [atomic formula](../../../../../atomic-formula.md) by

$$
R(t_1,\ldots,t_n)\text{ holds in the term model}\quad\Longleftrightarrow\quad R(t_1,\ldots,t_n)\in H.
$$

The [truth lemma for a Henkin term model](../../../../../truth-lemma-for-a-henkin-term-model.md) follows by induction on [logical formulas](../../../../../logical-formula.md) with [closed terms](../../../../../closed-term.md) substituted for their [free variables](../../../../../free-variable.md). The [logical connective](../../../../../logical-connective.md) steps use [maximal consistency of a first-order theory](../../../../../maximal-consistency-of-a-first-order-theory.md). In the existential step, membership of $\exists x\theta$ supplies a [witness constant](../../../../../witness-constant.md) and hence a [first-order term](../../../../../first-order-term.md) satisfying $\theta$; conversely a satisfying [closed term](../../../../../closed-term.md) gives the [existential sentence](../../../../../existential-sentence.md) by an inference of the calculus. The [term model](../../../../../term-model.md) consequently satisfies $H$ and the original theory. [Equality](../../../../../equality-mathematics.md) is absent here, so distinct [closed terms](../../../../../closed-term.md) may remain distinct domain elements without further identifications.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
