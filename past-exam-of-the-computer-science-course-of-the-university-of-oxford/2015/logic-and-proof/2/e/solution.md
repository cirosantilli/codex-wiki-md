<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

By part (c), $T$ has a [first-order model](../../../../../model-of-a-first-order-theory.md), so it is consistent. By part (d), every [first-order sentence](../../../../../first-order-sentence.md) is equivalent modulo $T$ to a [quantifier-free sentence](../../../../../quantifier-free-sentence.md). In the [first-order signature](../../../../../first-order-signature.md) consisting only of $E$ and [first-order equality](../../../../../logical-equality.md), there are no constant symbols, no ground [first-order terms](../../../../../first-order-term.md), and no nullary predicates. Thus a closed [quantifier-free formula](../../../../../quantifier-free-formula.md) reduces to true or false, using the logical truth constants. All [first-order models](../../../../../model-of-a-first-order-theory.md) of $T$ therefore agree on every [first-order sentence](../../../../../first-order-sentence.md):

$$
\boxed{T\text{ is complete}.}
$$

The construction in part (d) is effective. Conversion to [disjunctive normal form](../../../../../disjunctive-normal-form.md), enumeration of finite equality partitions and adjacency patterns, and testing the finitely many witness cases are all terminating operations. Apply them recursively to a given [first-order sentence](../../../../../first-order-sentence.md) and evaluate the final truth constant. This decides whether the [first-order sentence](../../../../../first-order-sentence.md) belongs to $T$, giving

$$
\boxed{T\text{ is decidable}.}
$$

No useful bound on the running time is needed for decidability; the potentially large enumeration still always terminates.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
