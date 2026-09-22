<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let $S=\{F_i:i\ge1\}$. Every finite [subset](../../../../../subset.md) of $S$ is satisfiable: if $F_N$ has the largest index occurring, the successive [semantic entailments](../../../../../semantic-entailment.md) imply $F_N\models F_i$ for every earlier index, so any [Boolean valuation](../../../../../boolean-valuation.md) satisfying $F_N$ satisfies that finite [subset](../../../../../subset.md). The [propositional compactness theorem](../../../../../propositional-compactness-theorem.md) therefore also shows that $S$ itself is satisfiable.

Suppose that $G$ had exactly the common models of $S$. Then $S\models G$, and hence $S\cup\{\neg G\}$ is unsatisfiable. By the [propositional compactness theorem](../../../../../propositional-compactness-theorem.md), finitely many $F_i$ together with $\neg G$ are already unsatisfiable. Enlarge the finite list if necessary so it is nonempty, and let $N$ be its greatest index. We obtain

$$
F_N\models G.
$$

On the other hand, the asserted equality of model classes gives $G\models F_{N+1}$. Transitivity of [semantic entailment](../../../../../semantic-entailment.md) would yield

$$
F_N\models F_{N+1},
$$

contradicting the strictness assumption at index $N$. Thus

$$
\boxed{\text{No single propositional formula defines the common models of all }F_i.}
$$

The obstruction is the finite character of [propositional formulas](../../../../../propositional-formula.md): a single consequence of an infinite set already follows from finitely many premises, whereas this chain continues to impose strictly stronger requirements forever.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
