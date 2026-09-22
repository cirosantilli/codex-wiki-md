<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The supplied [double-negation elimination](../../../../../double-negation-elimination.md) rule provides the classical step needed to recover each positive component:

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\neg(\neg\phi\lor\neg\psi)$ | Premise |
| 2 | $\neg\phi$ | Assume locally |
| 3 | $\neg\phi\lor\neg\psi$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), left, 2 |
| 4 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 1 and 3 |
| 5 | $\neg\neg\phi$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 2–4 |
| 6 | $\phi$ | [Double-negation elimination](../../../../../double-negation-elimination.md), 5 |
| 7 | $\neg\psi$ | Assume locally |
| 8 | $\neg\phi\lor\neg\psi$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), right, 7 |
| 9 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 1 and 8 |
| 10 | $\neg\neg\psi$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 7–9 |
| 11 | $\psi$ | [Double-negation elimination](../../../../../double-negation-elimination.md), 10 |
| 12 | $\phi\land\psi$ | [Conjunction introduction rule](../../../../../conjunction-introduction-rule.md), 6 and 11 |

Both local negated assumptions have been discharged. The [proof](../../../../../mathematical-proof.md) establishes the positive conjunction without assuming an unproved derived version of [De Morgan's laws](../../../../../de-morgan-s-laws.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
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
