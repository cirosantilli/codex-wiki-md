<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work backwards from the outermost available [logical connective](../../../../../logical-connective.md). One strategy applies the [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) to the premise first, constructs the whole target in each case, and then closes the cases. In the tables, a context such as $\{1,2\}$ means that assumptions on lines 1 and 2 remain open. A range in a discharge rule denotes the entire local subproof.

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $(P\land Q)\lor(P\land R)$ | Premise |
| 2 | $\{1,2\}$ | $P\land Q$ | Temporary assumption |
| 3 | $\{1,2\}$ | $P$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 2 |
| 4 | $\{1,2\}$ | $Q$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 2 |
| 5 | $\{1,2\}$ | $Q\lor R$ | [disjunction introduction rule](../../../../../disjunction-introduction-rule.md) $\lor\text{-intro-L}$ on 4 |
| 6 | $\{1,2\}$ | $P\land(Q\lor R)$ | [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) $\land\text{-intro}$ on 3, 5 |
| 7 | $\{1,7\}$ | $P\land R$ | Temporary assumption |
| 8 | $\{1,7\}$ | $P$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 7 |
| 9 | $\{1,7\}$ | $R$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 7 |
| 10 | $\{1,7\}$ | $Q\lor R$ | [disjunction introduction rule](../../../../../disjunction-introduction-rule.md) $\lor\text{-intro-R}$ on 9 |
| 11 | $\{1,7\}$ | $P\land(Q\lor R)$ | [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) $\land\text{-intro}$ on 8, 10 |
| 12 | $\{1\}$ | $P\land(Q\lor R)$ | [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) $\lor\text{-elim}$ on 1, 6, 11; discharge 2, 7 |

A second strategy applies the [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) backwards to the target first. Prove $P$ and $Q\lor R$ separately, each by the [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) on the premise, and combine them:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $(P\land Q)\lor(P\land R)$ | Premise |
| 2 | $\{1,2\}$ | $P\land Q$ | Temporary assumption |
| 3 | $\{1,2\}$ | $P$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 2 |
| 4 | $\{1,4\}$ | $P\land R$ | Temporary assumption |
| 5 | $\{1,4\}$ | $P$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-L}$ on 4 |
| 6 | $\{1\}$ | $P$ | [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) $\lor\text{-elim}$ on 1, 3, 5; discharge 2, 4 |
| 7 | $\{1,7\}$ | $P\land Q$ | Temporary assumption |
| 8 | $\{1,7\}$ | $Q$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 7 |
| 9 | $\{1,7\}$ | $Q\lor R$ | [disjunction introduction rule](../../../../../disjunction-introduction-rule.md) $\lor\text{-intro-L}$ on 8 |
| 10 | $\{1,10\}$ | $P\land R$ | Temporary assumption |
| 11 | $\{1,10\}$ | $R$ | [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) $\land\text{-elim-R}$ on 10 |
| 12 | $\{1,10\}$ | $Q\lor R$ | [disjunction introduction rule](../../../../../disjunction-introduction-rule.md) $\lor\text{-intro-R}$ on 11 |
| 13 | $\{1\}$ | $Q\lor R$ | [disjunction elimination rule](../../../../../disjunction-elimination-rule.md) $\lor\text{-elim}$ on 1, 9, 12; discharge 7, 10 |
| 14 | $\{1\}$ | $P\land(Q\lor R)$ | [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) $\land\text{-intro}$ on 6, 13 |

Both derivations establish

$$
\boxed{((P\land Q)\lor(P\land R))\vdash P\land(Q\lor R).}
$$

Counting only applications of [inference rules](../../../../../inference-rule.md), each proof has **nine** steps: four [conjunction elimination rule](../../../../../conjunction-elimination-rule.md) applications, two [disjunction introduction rule](../../../../../disjunction-introduction-rule.md) applications, and three remaining applications. The first uses two [conjunction introduction rule](../../../../../conjunction-introduction-rule.md) applications and one [disjunction elimination rule](../../../../../disjunction-elimination-rule.md); the second uses one and two, respectively. The second has two additional temporary-assumption lines, giving 14 displayed lines instead of 12, but assumptions are not additional inference applications. Its duplicated case analysis is exchanged for avoiding construction of the complete [logical conjunction](../../../../../logical-conjunction.md) separately in both cases. In a proof tree it also repeats the use of the original premise.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
