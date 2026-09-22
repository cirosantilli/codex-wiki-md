<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the conjunction and obtain a contradiction in each of the two cases supplied by the premise:

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\neg\phi\lor\neg\psi$ | Premise |
| 2 | $\phi\land\psi$ | Assume locally |
| 3 | $\phi$ | [Conjunction elimination rule](../../../../../conjunction-elimination-rule.md), left, 2 |
| 4 | $\psi$ | [Conjunction elimination rule](../../../../../conjunction-elimination-rule.md), right, 2 |
| 5 | $\neg\phi$ | Assume first case |
| 6 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 3 and 5 |
| 7 | $\neg\psi$ | Assume second case |
| 8 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 4 and 7 |
| 9 | $\bot$ | [Disjunction elimination rule](../../../../../disjunction-elimination-rule.md), 1, 5–6 and 7–8 |
| 10 | $\neg(\phi\land\psi)$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 2–9 |

The two case assumptions disappear at line 9, while the conjunction assumption remains available until line 10. The [proof](../../../../../mathematical-proof.md) uses only the primitive rules printed in the paper.

## ↑ Ancestors (12)

1. [C](../c.md)
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
