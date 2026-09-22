<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

The [completeness theorem for propositional logic](../../../../../completeness-theorem-for-propositional-logic.md), together with soundness, states $S\vdash\varphi$ if and only if $S\models\varphi$. In particular, an inconsistent [set](../../../../../set-split.md) of formulae has a finite formal proof of contradiction. Such a proof uses only finitely many assumptions, yielding the [propositional compactness theorem](../../../../../propositional-compactness-theorem.md): if every finite subset of $S$ is satisfiable, then $S$ is satisfiable.

The [decidability theorem for propositional logic](../../../../../decidability-theorem-for-propositional-logic.md) concerns theoremhood of a formula, or entailment from a finite list of premises. Formulae involve finitely many variables, so their valuations can be tested by a finite truth table; completeness identifies semantic validity with provability. Equivalently, dovetail effective proof enumeration with the finite search for a countervaluation: completeness ensures that one succeeds. This is not a decidability claim for consequences of an arbitrary noncomputable infinite theory.

An infinite collection of distinct tautologies is a [finitary set of formulae](../../../../../finitary-set-of-formulae.md), since its deductive closure equals that of the empty [set](../../../../../set-split.md). By contrast, the [set](../../../../../set-split.md) of independent variables $\{p_i:i\ge1\}$ is not finitary. If a finite [set](../../../../../set-split.md) $T$ had the same closure, it would mention only finitely many variables. It is satisfiable because it is a consequence of the all-true model of the $p_i$; changing an unmentioned $p_j$ to false preserves $T$ and contradicts $T\models p_j$.

Under the final hypothesis, $A\cup B$ has no model. The [propositional compactness theorem](../../../../../propositional-compactness-theorem.md) gives finite $A'\subset A$, $B'\subset B$ with $A'\cup B'$ inconsistent. Any valuation satisfying $A'$ cannot satisfy $B$, because it would then satisfy $B'$; by the exactly-one hypothesis it must satisfy $A$. The reverse implication holds by inclusion. Thus $A$ and $A'$ have identical models, and similarly $B$ and $B'$. Completeness gives identical deductive closures, proving

$$
\boxed{A\text{ and }B\text{ are finitary}}.
$$

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
