<h1 id="a/1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Boolean valuation](../../../../../boolean-valuation.md) is an arbitrary [function](../../../../../function-split.md) $v$ assigning one of the two [truth values](../../../../../truth-value.md) to each [propositional variable](../../../../../propositional-variable.md). It extends uniquely to all [propositional formulas](../../../../../propositional-formula.md) by following the construction of the [propositional formula](../../../../../propositional-formula.md):

$$
\widetilde v(p)=v(p),\quad
\widetilde v(\neg A)=\neg\widetilde v(A),\quad
\widetilde v(A\wedge B)=\widetilde v(A)\wedge\widetilde v(B),\quad
\widetilde v(A\vee B)=\widetilde v(A)\vee\widetilde v(B).
$$

For [logical implication](../../../../../logical-implication.md), $\widetilde v(A\to B)$ is false exactly when $\widetilde v(A)$ is true and $\widetilde v(B)$ is false; otherwise it is true. Here the operations on the right are [Boolean operations](../../../../../boolean-operation.md) on [truth values](../../../../../truth-value.md). [Structural recursion](../../../../../structural-recursion.md) gives existence, and [structural induction](../../../../../structural-induction.md) gives uniqueness: once the immediate subformulas have their values, the outer connective fixes the resulting value.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
