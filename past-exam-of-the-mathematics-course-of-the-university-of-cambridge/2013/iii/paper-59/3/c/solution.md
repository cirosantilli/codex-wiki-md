<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [AND-NOT circuit value problem](../../../../../../and-not-circuit-value-problem.md) belongs to [P](../../../../../../p-complexity.md): validate the [Boolean circuit](../../../../../../boolean-circuit.md) and evaluate its gates in a [topological ordering](../../../../../../topological-ordering.md). Evaluation takes [polynomial time](../../../../../../polynomial-time.md) even if its description is not already in a [topological ordering](../../../../../../topological-ordering.md).

For [P-completeness](../../../../../../p-completeness.md) we use [logspace many-one reductions](../../../../../../logspace-many-one-reduction.md). Start from the supplied [circuit value problem](../../../../../../circuit-value-problem.md) over the usual AND ([logical conjunction](../../../../../../logical-conjunction.md)), OR ([logical disjunction](../../../../../../logical-disjunction.md)) and NOT ([negation](../../../../../../negation.md)) basis. Retain AND and NOT gates, and replace every OR gate by the [De Morgan's laws](../../../../../../de-morgan-s-laws.md) gadget

$$
\boxed{x\vee y=\neg(\neg x\wedge\neg y)}.
$$

This adds only a constant number of gates per old gate, preserves its truth value for all inputs and keeps the [Boolean circuit](../../../../../../boolean-circuit.md) acyclic. If the format includes constant source nodes, replace them by additional input nodes assigned fixed bits zero and one; these are inputs, not disallowed gates. Larger fan-in gates can first be replaced by binary trees of their inputs.

To output the new description, keep the old gate index and a constant-size gadget position, rescan old references when necessary, and assign consistent new indices to each gadget's terminal output. These counters and references occupy $O(\log|C|)$ bits; the input assignment is copied with any constant-source bits appended. Thus the construction is a [logspace many-one reduction](../../../../../../logspace-many-one-reduction.md) preserving acceptance. Since [Boolean circuit](../../../../../../boolean-circuit.md) Value is [P-complete](../../../../../../p-completeness.md) under such reductions,

$$
\boxed{\mathrm{AND\text{-}NOT\ CIRCUIT\ VALUE}\text{ is P-complete}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
