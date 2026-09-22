<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $K$ abbreviate $Q(c_1)\lor Q(c_2)$, and group the three equality alternatives on the left. The [proof](../../../../../mathematical-proof.md) uses the binary [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) twice, so no unproved three-way derived rule is needed.

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\forall x\,((x=c_0\lor x=c_1)\lor x=c_2)$ | Premise |
| 2 | $\neg Q(c_0)$ | Assume for the first implication |
| 3 | $\exists x\,Q(x)$ | Assume for the second implication |
| 4 | $Q(u)$ | Assume with fresh witness name $u$ |
| 5 | $(u=c_0\lor u=c_1)\lor u=c_2$ | [Universal quantifier elimination rule](../../../../../universal-quantifier-elimination-rule.md), 1 |
| 6 | $u=c_0\lor u=c_1$ | Assume the first outer case |
| 7 | $u=c_0$ | Assume the first inner case |
| 8 | $Q(c_0)$ | [Equality elimination rule](../../../../../equality-elimination-rule.md), 7 and 4 |
| 9 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 2 and 8 |
| 10 | $K$ | [Logical falsity elimination rule](../../../../../logical-falsity-elimination-rule.md), 9 |
| 11 | $u=c_1$ | Assume the second inner case |
| 12 | $Q(c_1)$ | [Equality elimination rule](../../../../../equality-elimination-rule.md), 11 and 4 |
| 13 | $K$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), left, 12 |
| 14 | $K$ | [Disjunction elimination rule](../../../../../disjunction-elimination-rule.md), 6, 7–10 and 11–13 |
| 15 | $u=c_2$ | Assume the second outer case |
| 16 | $Q(c_2)$ | [Equality elimination rule](../../../../../equality-elimination-rule.md), 15 and 4 |
| 17 | $K$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), right, 16 |
| 18 | $K$ | [Disjunction elimination rule](../../../../../disjunction-elimination-rule.md), 5, 6–14 and 15–17 |
| 19 | $K$ | [Existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md), 3 and 4–18 |
| 20 | $(\exists x\,Q(x))\to K$ | [Implication introduction rule](../../../../../implication-introduction-rule.md), discharging 3–19 |
| 21 | $\neg Q(c_0)\to(\exists x\,Q(x))\to K$ | [Implication introduction rule](../../../../../implication-introduction-rule.md), discharging 2–20 |

The witness name is absent from $K$ and from every assumption remaining after line 19, so the existential elimination is legal. Each equality is used in the forward direction supplied by the printed equality rule. The three named constants need not denote distinct objects: the case [proof](../../../../../mathematical-proof.md) requires only that they exhaust the domain. This is [existential quantification over a finitely named domain](../../../../../existential-quantification-over-a-finitely-named-domain.md) followed by exclusion of the first case.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
