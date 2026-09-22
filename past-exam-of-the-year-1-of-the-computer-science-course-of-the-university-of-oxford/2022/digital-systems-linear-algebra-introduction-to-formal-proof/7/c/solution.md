<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [structural induction](../../../../../structural-induction.md) on the [propositional formula](../../../../../propositional-formula.md). The induction claim is that its [truth value](../../../../../truth-value.md) under the all-one [Boolean valuation](../../../../../boolean-valuation.md) is one. A variable has this [truth value](../../../../../truth-value.md) by definition. For the induction step, suppose the immediate subformulas $\alpha,\beta$ each have [truth value](../../../../../truth-value.md) one. Then

$$
\llbracket\alpha\lor\beta\rrbracket=1\lor1=1,\qquad
\llbracket\alpha\land\beta\rrbracket=1\land1=1,\qquad
\llbracket\alpha\to\beta\rrbracket=1\to1=1.
$$

These are all permitted construction cases. Thus every such [propositional formula](../../../../../propositional-formula.md) evaluates to one. Equivalently, the three [logical connectives](../../../../../logical-connective.md) define [one-preserving Boolean functions](../../../../../one-preserving-boolean-function.md), and composition preserves this property. The variable-only base grammar matters: admitting a constant false formula would invalidate the claim.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
