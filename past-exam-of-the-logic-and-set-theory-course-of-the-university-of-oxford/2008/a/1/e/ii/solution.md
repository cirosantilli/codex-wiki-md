<h1 id="a/1/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A useful consequence of the [formation rules](../../../../../../formation-rule.md) is that [logical formulas](../../../../../../logical-formula.md) form a prefix-free [set](../../../../../../set-split.md) of strings. To see this, describe a deterministic [parser](../../../../../../parser.md) that reads one [logical formula](../../../../../../logical-formula.md) from its starting position. On a [logical variable](../../../../../../logical-variable.md) it consumes that one symbol. On a [negation](../../../../../../negation.md) symbol it recursively reads one following [logical formula](../../../../../../logical-formula.md). On an opening parenthesis it recursively reads a left [logical formula](../../../../../../logical-formula.md), requires a [logical implication](../../../../../../logical-implication.md) symbol, recursively reads a right [logical formula](../../../../../../logical-formula.md), and requires the closing parenthesis. Induction on formation proves that, if a valid [logical formula](../../../../../../logical-formula.md) begins at the current position, this procedure consumes exactly that [logical formula](../../../../../../logical-formula.md) and stops at its end.

Suppose now that both $\alpha$ and $\phi$ are [logical formulas](../../../../../../logical-formula.md) and $\phi=\alpha\epsilon$. The same [parser](../../../../../../parser.md), started at their common first symbol, must stop both at the end of $\alpha$ and at the end of $\phi$. Its deterministic stopping position cannot differ, so $\epsilon$ is empty. Hence

$$
\boxed{\alpha=\phi.}
$$

This argument applies to symbol strings; it does not use [truth values](../../../../../../truth-value.md) or [logical equivalence](../../../../../../logical-equivalence.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
