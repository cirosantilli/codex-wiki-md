<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the [Curry-Howard correspondence](../../../../../../curry-howard-correspondence.md), [Intuitionistic propositional logic](../../../../../../intuitionistic-propositional-logic.md) propositions are types and proofs are typed terms. Assumptions correspond to typed variables. The [logical implication](../../../../../../logical-implication.md) $A\to B$ corresponds to the function type, [logical conjunction](../../../../../../logical-conjunction.md) $A\wedge B$ to the product type, [logical disjunction](../../../../../../logical-disjunction.md) $A\vee B$ to the sum type, [logical truth](../../../../../../logical-truth.md) to the unit type, and [logical falsity](../../../../../../logical-falsity.md) to the empty type.

The rules of [natural deduction](../../../../../../natural-deduction.md) become term constructors. Implication introduction sends a derivation of $B$ from a variable $x:A$ to the abstraction $\lambda x.M:A\to B$, while implication elimination becomes application $MN$. Pairing and projection implement conjunction, and injections with case analysis implement disjunction. Under this correspondence, normalization of proofs is computation by [beta reduction](../../../../../../beta-reduction.md) in the [simply typed lambda calculus](../../../../../../simply-typed-lambda-calculus.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
