<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Temporarily deny the desired [logical disjunction](../../../../../../logical-disjunction.md). If $\neg P$ held, it would introduce that very [logical disjunction](../../../../../../logical-disjunction.md), producing [logical falsity](../../../../../../logical-falsity.md); [double-negation elimination](../../../../../../double-negation-elimination.md) therefore gives $P$. The same argument gives $Q$, contradicting the premise. The complete [natural deduction](../../../../../../natural-deduction.md) derivation is:

<a id="7/d/ii/table-classical-derivation-of-the-disjunction-of-negations"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\neg (P\land Q)$ | Premise |
| 2 | 1, 2 | $\neg (\neg P\lor\neg Q)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 3 | 1, 2, 3 | $\neg P$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 4 | 1, 2, 3 | $\neg P\lor\neg Q$ | [disjunction introduction](../../../../../../disjunction-introduction-rule.md) L 3 |
| 5 | 1, 2, 3 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 4, 2 |
| 6 | 1, 2 | $\neg \neg P$ | [negation introduction](../../../../../../negation-introduction-rule.md) 3, 5 |
| 7 | 1, 2 | $P$ | [double-negation elimination](../../../../../../double-negation-elimination.md) 6 |
| 8 | 1, 2, 8 | $\neg Q$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 9 | 1, 2, 8 | $\neg P\lor\neg Q$ | [disjunction introduction](../../../../../../disjunction-introduction-rule.md) R 8 |
| 10 | 1, 2, 8 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 9, 2 |
| 11 | 1, 2 | $\neg \neg Q$ | [negation introduction](../../../../../../negation-introduction-rule.md) 8, 10 |
| 12 | 1, 2 | $Q$ | [double-negation elimination](../../../../../../double-negation-elimination.md) 11 |
| 13 | 1, 2 | $P\land Q$ | [conjunction introduction](../../../../../../conjunction-introduction-rule.md) 7, 12 |
| 14 | 1, 2 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 13, 1 |
| 15 | 1 | $\neg \neg (\neg P\lor\neg Q)$ | [negation introduction](../../../../../../negation-introduction-rule.md) 2, 14 |
| 16 | 1 | $\neg P\lor\neg Q$ | [double-negation elimination](../../../../../../double-negation-elimination.md) 15 |

Consequently

$$
\boxed{\neg P\lor\neg Q.}
$$

The uses of [double-negation elimination](../../../../../../double-negation-elimination.md) are justified by the supplied rules. This distinguishes the proof from the preceding constructive direction of [De Morgan's laws](../../../../../../de-morgan-s-laws.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
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
