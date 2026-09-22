<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First negate the implication, then move the [negation](../../../../../negation.md) through the existential quantifier and the [logical conjunction](../../../../../logical-conjunction.md):

$$
\begin{aligned}
\neg\varphi
&\equiv(\forall x\,P(x))\land\neg\exists y\,(Q(y)\land z<y)\\
&\equiv\boxed{(\forall x\,P(x))\land\forall y\,(\neg Q(y)\lor\neg(z<y)).}
\end{aligned}
$$

This is [negation normal form](../../../../../negation-normal-form.md), because each [negation](../../../../../negation.md) is immediately in front of an atomic predicate. The occurrence of $z$ remains free. Keeping $\neg(z<y)$ also avoids assuming any additional order axioms for the relation symbol $<$; if it has its usual linear-order interpretation, that atom can instead be expressed as $z\geq y$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
