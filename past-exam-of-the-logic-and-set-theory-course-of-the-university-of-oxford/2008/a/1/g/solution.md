<h1 id="a/1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Fix any [Boolean valuation](../../../../../boolean-valuation.md) $v$. [Logical equivalence](../../../../../logical-equivalence.md) of $\alpha$ and $\beta$ means $v(\alpha)=v(\beta)$ for this [Boolean valuation](../../../../../boolean-valuation.md) and every other one. Follow the unique path from the replaced node to the root of the [formula syntax tree](../../../../../syntax-tree-of-a-formula.md). At a [negation](../../../../../negation.md) node, equal input [truth values](../../../../../truth-value.md) have equal [negations](../../../../../negation.md). At a [logical implication](../../../../../logical-implication.md) node, the unaffected child has the same [truth value](../../../../../truth-value.md) before and after [subformula replacement](../../../../../subformula-replacement.md), while the affected child has the same [truth value](../../../../../truth-value.md) by induction; the resulting [logical implications](../../../../../logical-implication.md) therefore agree as well.

Induction along that finite path yields $v(\phi)=v(\phi')$. Since $v$ was arbitrary,

$$
\boxed{\phi\equiv\phi'.}
$$

This is the [replacement theorem for logical equivalence](../../../../../replacement-theorem-for-logical-equivalence.md): the semantics of each [logical connective](../../../../../logical-connective.md) depends only on the [truth values](../../../../../truth-value.md) of its immediate inputs.

## ↑ Ancestors (13)

1. [G](../g.md)
2. [1](../../1.md)
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
