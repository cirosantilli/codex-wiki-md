<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose arbitrary fresh variables $y,x,z$ and assume $H=((x=y\lor y=z)\land P(y))$ under label $a$. The [conjunction elimination rule](../../../../../../conjunction-elimination-rule.md) gives $x=y\lor y=z$ and $P(y)$. Apply the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md) to the equality disjunction.

In the case $x=y$, the supplied symmetry rule gives $y=x$, and the [equality elimination rule](../../../../../../equality-elimination-rule.md) applied to $P(y)$ gives $P(x)$. [Disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) gives $P(x)\lor P(z)$. In the case $y=z$, [equality elimination rule](../../../../../../equality-elimination-rule.md) applied directly to $P(y)$ gives $P(z)$; the other [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) gives the same conclusion $P(x)\lor P(z)$. Discharge the two equality case assumptions by [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md).

Discharge $a$ with the [implication introduction rule](../../../../../../implication-introduction-rule.md). There are now no undischarged assumptions. Use the [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) successively for $z$, then $x$, then $y$, yielding

$$
\forall y\,\forall x\,\forall z\,\bigl(((x=y\lor y=z)\land P(y))\to(P(x)\lor P(z))\bigr).
$$

Freshness holds at every generalization because the sole temporary assumption has already been discharged; the arbitrary variables are not tied to any premise.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
