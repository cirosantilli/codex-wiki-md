<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use a [first-order signature](../../../../../first-order-signature.md) with a constant $a$ and unary predicates $P,Q$, and set

$$
F=\forall x\,[P(x)\lor Q(x)],
\qquad G=\exists x\,[P(x)\lor Q(x)].
$$

The displayed [first-order clause](../../../../../first-order-clause.md) has two positive atoms, so it is not a [Horn clause](../../../../../horn-clause.md). There is a [Herbrand model](../../../../../herbrand-model.md) with $P(a)$ true and $Q(a)$ false, and another with the opposite values. Thus neither atom holds in all [Herbrand models](../../../../../herbrand-model.md); the intersection construction makes both false.

Every [first-order model](../../../../../model-of-a-first-order-theory.md) of $F$ has a nonempty domain, and any element witnesses $G$, so $F\models G$. Nevertheless $\mathcal H_F\not\models G$. Therefore

$$
\boxed{F\models G\quad\text{but}\quad\mathcal H_F\not\models G.}
$$

This example uses a positive [existential sentence](../../../../../existential-sentence.md), so it also shows the necessity of the [Horn clause](../../../../../horn-clause.md) restriction in the repaired result from part (d). Without that restriction, the intersection of [Herbrand models](../../../../../herbrand-model.md) need not itself be a [first-order model](../../../../../model-of-a-first-order-theory.md) of $F$: here it fails the very disjunction that all the original [Herbrand models](../../../../../herbrand-model.md) satisfy.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
