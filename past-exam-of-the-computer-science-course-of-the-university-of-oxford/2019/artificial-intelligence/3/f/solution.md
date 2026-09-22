<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Read the satisfying assignment in increasing time order. In layer $t$, output the unique [ground action](../../../../../ground-action.md) whose occurrence [Boolean variable](../../../../../boolean-variable.md) is true, or output nothing if all are false. Discard idle layers. The result is a [sequence](../../../../../sequence.md) of at most $T$ actions.

For correctness, the layer-zero [planning fluents](../../../../../planning-fluent.md) are exactly the actual initial state. The [action precondition axioms](../../../../../action-precondition-axiom.md) make the selected action applicable, while the [successor-state axioms](../../../../../successor-state-axiom.md) give precisely its add/delete update; the [action exclusion axioms](../../../../../action-exclusion-axiom.md) prevent simultaneous competing actions. By [induction](../../../../../mathematical-induction.md), every following time layer is the real state reached by the decoded prefix. The final goal formula therefore proves that **the extracted [plan](../../../../../plan.md) reaches both required goals**.

Conversely, execute any valid [plan](../../../../../plan.md) of length at most $T$, assign each layer its actual fluent values and pad with idle layers. These values satisfy every component of $\varphi_T$. In this instance, decoding the three-action trajectory in part (d) gives a model at $T=3$ and at every larger horizon after padding; direct state-space and propositional checks find no model for $T<3$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
