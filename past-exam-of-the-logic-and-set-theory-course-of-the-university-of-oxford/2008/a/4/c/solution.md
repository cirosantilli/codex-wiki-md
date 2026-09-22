<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the presence of [equality](../../../../../equality-mathematics.md), two syntactically different [closed terms](../../../../../closed-term.md) can be asserted equal by the [Henkin theory](../../../../../henkin-theory.md), so the raw [first-order term](../../../../../first-order-term.md) domain from part (b) must be replaced by a [quotient set](../../../../../quotient-set.md). Define

$$
t\sim u\quad\Longleftrightarrow\quad (t=u)\in H.
$$

The [equality](../../../../../equality-mathematics.md) [axioms](../../../../../axiom.md) give reflexivity, symmetry and transitivity, so this is an [equivalence relation](../../../../../equivalence-relation.md). Their substitution consequences make it a [congruence relation on a first-order structure](../../../../../congruence-relation-on-a-first-order-structure.md): replacing an input by an equivalent [first-order term](../../../../../first-order-term.md) preserves equivalence of [function](../../../../../function-split.md) values and preserves membership of [atomic formulas](../../../../../atomic-formula.md) in $H$.

Take domain $\{[t]:t\text{ is a closed term}\}$. Define a [function symbol](../../../../../function-symbol.md) by $f([t_1],\ldots,[t_n])=[f(t_1,\ldots,t_n)]$, and relations by the same membership test as before using representatives. The [congruence relation on a first-order structure](../../../../../congruence-relation-on-a-first-order-structure.md) makes these definitions independent of representatives. Actual identity of [equivalence classes](../../../../../equivalence-class.md) now agrees with the formal [equality](../../../../../equality-mathematics.md) [first-order sentences](../../../../../first-order-sentence.md) in $H$:

$$
\boxed{[t]=[u]\quad\Longleftrightarrow\quad(t=u)\in H.}
$$

This supplies the [equality](../../../../../equality-mathematics.md) case of the [truth lemma for a Henkin term model](../../../../../truth-lemma-for-a-henkin-term-model.md); the [logical connective](../../../../../logical-connective.md) and [quantifier](../../../../../quantifier.md) cases then proceed exactly as in the [Henkin construction](../../../../../henkin-construction.md). Thus the [term model](../../../../../term-model.md) built from the [quotient set](../../../../../quotient-set.md) is a genuine [first-order model](../../../../../model-of-a-first-order-theory.md) with [equality](../../../../../equality-mathematics.md) interpreted as identity.

## ↑ Ancestors (13)

1. [C](../c.md)
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
