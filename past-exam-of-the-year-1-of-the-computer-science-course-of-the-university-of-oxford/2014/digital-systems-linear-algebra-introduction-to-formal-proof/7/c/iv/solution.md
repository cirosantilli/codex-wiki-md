<h1 id="7/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Assuming $\neg P$ lets the [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) produce the [logical disjunction](../../../../../../logical-disjunction.md) excluded by the premise. This gives a [contradiction](../../../../../../contradiction.md), so conclude by [negation introduction](../../../../../../negation-introduction-rule.md) and [double-negation elimination](../../../../../../double-negation-elimination.md):

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $\neg(\neg P\lor\neg Q)$ | Premise |
| 2 | $\{1,2\}$ | $\neg P$ | Temporary assumption |
| 3 | $\{1,2\}$ | $\neg P\lor\neg Q$ | [disjunction introduction rule](../../../../../../disjunction-introduction-rule.md) $\lor\text{-intro-L}$ on 2 |
| 4 | $\{1,2\}$ | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) $\neg\text{-elim}$ on 3, 1 |
| 5 | $\{1\}$ | $\neg\neg P$ | [negation introduction rule](../../../../../../negation-introduction-rule.md) $\neg\text{-intro}$ on 4; discharge 2 |
| 6 | $\{1\}$ | $P$ | [double-negation elimination](../../../../../../double-negation-elimination.md) $\neg\neg\text{-elim}$ on 5 |

Thus

$$
\boxed{\neg(\neg P\lor\neg Q)\vdash P.}
$$

No separate result about $Q$ or use of a derived De Morgan rule is needed.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
