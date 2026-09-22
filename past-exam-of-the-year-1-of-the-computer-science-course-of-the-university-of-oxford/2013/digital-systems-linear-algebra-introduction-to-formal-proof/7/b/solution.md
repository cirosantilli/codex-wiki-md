<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The following [natural deduction](../../../../../natural-deduction.md) tables record the active assumption lines explicitly. A rule may use an earlier line only while all of that line's assumptions remain available; [assumption discharge](../../../../../assumption-discharge.md) closes the indicated case or hypothesis. The first proof makes the case split first, constructs the whole required [logical conjunction](../../../../../logical-conjunction.md) in each case, and then closes the cases.

<a id="7/b/table-first-proof-one-case-split-constructs-both-conjuncts"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $P\lor(Q\land R)$ | Premise |
| 2 | 1, 2 | $P$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 3 | 1, 2 | $P\lor Q$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) L 2 |
| 4 | 1, 2 | $P\lor R$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) L 2 |
| 5 | 1, 2 | $(P\lor Q)\land(P\lor R)$ | [conjunction introduction](../../../../../conjunction-introduction-rule.md) 3, 4 |
| 6 | 1, 6 | $Q\land R$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 7 | 1, 6 | $Q$ | [conjunction elimination](../../../../../conjunction-elimination-rule.md) L 6 |
| 8 | 1, 6 | $R$ | [conjunction elimination](../../../../../conjunction-elimination-rule.md) R 6 |
| 9 | 1, 6 | $P\lor Q$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) R 7 |
| 10 | 1, 6 | $P\lor R$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) R 8 |
| 11 | 1, 6 | $(P\lor Q)\land(P\lor R)$ | [conjunction introduction](../../../../../conjunction-introduction-rule.md) 9, 10 |
| 12 | 1 | $(P\lor Q)\land(P\lor R)$ | [disjunction elimination](../../../../../disjunction-elimination-rule.md) 1, 2, 5, 6, 11 |

The second proof instead splits the goal first. It proves each required [logical disjunction](../../../../../logical-disjunction.md) by a separate use of [disjunction elimination](../../../../../disjunction-elimination-rule.md), then applies [conjunction introduction](../../../../../conjunction-introduction-rule.md) at the end.

<a id="7/b/table-second-proof-separate-case-splits-establish-the-two-conjuncts"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $P\lor(Q\land R)$ | Premise |
| 2 | 1, 2 | $P$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 3 | 1, 2 | $P\lor Q$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) L 2 |
| 4 | 1, 4 | $Q\land R$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 5 | 1, 4 | $Q$ | [conjunction elimination](../../../../../conjunction-elimination-rule.md) L 4 |
| 6 | 1, 4 | $P\lor Q$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) R 5 |
| 7 | 1 | $P\lor Q$ | [disjunction elimination](../../../../../disjunction-elimination-rule.md) 1, 2, 3, 4, 6 |
| 8 | 1, 8 | $P$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 9 | 1, 8 | $P\lor R$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) L 8 |
| 10 | 1, 10 | $Q\land R$ | [Temporary assumption](../../../../../temporary-assumption.md) |
| 11 | 1, 10 | $R$ | [conjunction elimination](../../../../../conjunction-elimination-rule.md) R 10 |
| 12 | 1, 10 | $P\lor R$ | [disjunction introduction](../../../../../disjunction-introduction-rule.md) R 11 |
| 13 | 1 | $P\lor R$ | [disjunction elimination](../../../../../disjunction-elimination-rule.md) 1, 8, 9, 10, 12 |
| 14 | 1 | $(P\lor Q)\land(P\lor R)$ | [conjunction introduction](../../../../../conjunction-introduction-rule.md) 7, 13 |

The essential difference is the order of proof construction: the first shares one case split between both goals, whereas the second duplicates that split and combines the results outside the cases. Both use only the stated [natural deduction](../../../../../natural-deduction.md) rules, and both conclude

$$
\boxed{(P\lor Q)\land(P\lor R).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
