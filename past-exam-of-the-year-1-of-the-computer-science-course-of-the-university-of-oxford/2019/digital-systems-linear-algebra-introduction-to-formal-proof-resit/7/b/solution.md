<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Derive each negated component in its own [subproof](../../../../../subproof.md), then combine them. Assumption lines below begin local scopes; the listed discharge ranges close those scopes.

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\neg(\phi\lor\psi)$ | Premise |
| 2 | $\phi$ | Assume locally |
| 3 | $\phi\lor\psi$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), left, 2 |
| 4 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 1 and 3 |
| 5 | $\neg\phi$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 2–4 |
| 6 | $\psi$ | Assume locally |
| 7 | $\phi\lor\psi$ | [Disjunction introduction rule](../../../../../disjunction-introduction-rule.md), right, 6 |
| 8 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 1 and 7 |
| 9 | $\neg\psi$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 6–8 |
| 10 | $\neg\phi\land\neg\psi$ | [Conjunction introduction rule](../../../../../conjunction-introduction-rule.md), 5 and 9 |

Only the original premise remains open. No classical principle is needed for this direction of [De Morgan's laws](../../../../../de-morgan-s-laws.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
