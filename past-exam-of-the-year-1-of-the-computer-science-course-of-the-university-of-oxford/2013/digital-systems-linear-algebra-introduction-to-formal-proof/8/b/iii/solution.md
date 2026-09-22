<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Introduce a fresh [existential witness](../../../../../../existential-witness.md) $v$ with $R(v)$. The universal premise gives $v=0\lor v=1$. In the first case, [equality elimination rule](../../../../../../equality-elimination-rule.md) gives $R(0)$. In the second, it gives $R(1)$, contradicting $\neg R(1)$; [explosion](../../../../../../logical-falsity-elimination-rule.md) then supplies the common case conclusion $R(0)$. Close both cases and then the witness scope:

<a id="8/b/iii/table-a-witness-must-yield-the-relation-at-zero"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\forall x\, x=0\lor x=1$ | Premise |
| 2 | 1, 2 | $\exists x\, R(x)$ | Premise |
| 3 | 1, 2, 3 | $\neg R(1)$ | Premise |
| 4 | 1, 2, 3, 4 | $R(v)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 5 | 1, 2, 3, 4 | $v=0\lor v=1$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) 1; term $v$ |
| 6 | 1, 2, 3, 4, 6 | $v=0$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 7 | 1, 2, 3, 4, 6 | $R(0)$ | [equality elimination rule](../../../../../../equality-elimination-rule.md) 6, 4 |
| 8 | 1, 2, 3, 4, 8 | $v=1$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 9 | 1, 2, 3, 4, 8 | $R(1)$ | [equality elimination rule](../../../../../../equality-elimination-rule.md) 8, 4 |
| 10 | 1, 2, 3, 4, 8 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 9, 3 |
| 11 | 1, 2, 3, 4, 8 | $R(0)$ | [explosion](../../../../../../logical-falsity-elimination-rule.md) 10 |
| 12 | 1, 2, 3, 4 | $R(0)$ | [disjunction elimination](../../../../../../disjunction-elimination-rule.md) 5, 6, 7, 8, 11 |
| 13 | 1, 2, 3 | $R(0)$ | [existential elimination](../../../../../../existential-quantifier-elimination-rule.md) 2, 4, 12; fresh $v$ |

Hence

$$
\boxed{R(0).}
$$

For both uses of [equality elimination rule](../../../../../../equality-elimination-rule.md), the formula template is $R(z)$. At the final [existential elimination](../../../../../../existential-quantifier-elimination-rule.md), $v$ is fresh in all three original premises and absent from $R(0)$, so the [eigenvariable condition](../../../../../../eigenvariable-condition.md) holds. No additional assumption that the constants $0$ and $1$ denote distinct objects is needed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
