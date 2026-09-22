<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under the premise, assuming either disjunct would introduce the forbidden [logical disjunction](../../../../../../logical-disjunction.md). Discharging those two assumptions gives the two separate [negations](../../../../../../negation.md), which can then be conjoined.

<a id="7/d/i/table-derivation-of-the-two-negated-disjuncts"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\neg (P\lor Q)$ | Premise |
| 2 | 1, 2 | $P$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 3 | 1, 2 | $P\lor Q$ | [disjunction introduction](../../../../../../disjunction-introduction-rule.md) L 2 |
| 4 | 1, 2 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 3, 1 |
| 5 | 1 | $\neg P$ | [negation introduction](../../../../../../negation-introduction-rule.md) 2, 4 |
| 6 | 1, 6 | $Q$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 7 | 1, 6 | $P\lor Q$ | [disjunction introduction](../../../../../../disjunction-introduction-rule.md) R 6 |
| 8 | 1, 6 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 7, 1 |
| 9 | 1 | $\neg Q$ | [negation introduction](../../../../../../negation-introduction-rule.md) 6, 8 |
| 10 | 1 | $\neg P\land\neg Q$ | [conjunction introduction](../../../../../../conjunction-introduction-rule.md) 5, 9 |

Thus

$$
\boxed{\neg P\land\neg Q.}
$$

The redundant closing parenthesis printed after the conclusion on p. 8 does not alter the readable [propositional formula](../../../../../../propositional-formula.md).[Printed p. 8, Question 7(d)(i)](../../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2013.md)

## ↑ Ancestors (13)

1. [I](../i.md)
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
