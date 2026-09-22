<h1 id="a/3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $E(x,y)$ for the displayed equality predicate. A6 and A4 give $\vdash E(x,x)$, establishing a [reflexive relation](../../../../../../reflexive-relation.md).

An instance of A7, replacing just the first occurrence of $x$ in $E(x,x)$, is

$$
E(x,y)\to(E(x,x)\to E(y,x)).
$$

Assume $E(x,y)$, apply the [modus ponens rule](../../../../../../implication-elimination-rule.md) twice using reflexivity, and obtain $E(y,x)$. The [deduction theorem for propositional logic](../../../../../../deduction-theorem-for-propositional-logic.md) discharges the assumption. This proves symmetry.

For transitivity, A7 supplies

$$
E(y,z)\to(E(x,y)\to E(x,z)),
$$

by replacing $y$ in the atomic formula $E(x,y)$. From assumptions $E(x,y)$ and $E(y,z)$, two applications of the [modus ponens rule](../../../../../../implication-elimination-rule.md) give $E(x,z)$. Discharging assumptions and universally generalizing gives

$$
\boxed{\vdash\forall x\,E(x,x),\quad\vdash\forall x\forall y(E(x,y)\to E(y,x)),\quad\vdash\forall x\forall y\forall z((E(x,y)\land E(y,z))\to E(x,z)).}
$$

Thus the predicate defines an [equivalence relation](../../../../../../equivalence-relation.md) within the calculus.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
