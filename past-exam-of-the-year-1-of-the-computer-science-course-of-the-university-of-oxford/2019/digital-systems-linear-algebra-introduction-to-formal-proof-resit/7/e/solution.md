<h1 id="7/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $H$ for $(\phi\to\psi)\to\phi$. The following derives [Peirce's law](../../../../../peirce-s-law.md) directly from the printed primitive rules, including [double-negation elimination](../../../../../double-negation-elimination.md):

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $H$ | Assume for the final implication |
| 2 | $\neg\phi$ | Assume locally |
| 3 | $\phi$ | Assume inside the scope of 2 |
| 4 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 2 and 3 |
| 5 | $\psi$ | [Logical falsity elimination rule](../../../../../logical-falsity-elimination-rule.md), 4 |
| 6 | $\phi\to\psi$ | [Implication introduction rule](../../../../../implication-introduction-rule.md), discharging 3–5 |
| 7 | $\phi$ | [Implication elimination rule](../../../../../implication-elimination-rule.md), 1 and 6 |
| 8 | $\bot$ | [Negation elimination rule](../../../../../negation-elimination-rule.md), 2 and 7 |
| 9 | $\neg\neg\phi$ | [Negation introduction rule](../../../../../negation-introduction-rule.md), discharging 2–8 |
| 10 | $\phi$ | [Double-negation elimination](../../../../../double-negation-elimination.md), 9 |
| 11 | $((\phi\to\psi)\to\phi)\to\phi$ | [Implication introduction rule](../../../../../implication-introduction-rule.md), discharging 1–10 |

Every assumption is discharged, so the last formula is a theorem. In particular, no unproved appeal to the derived `RAA` rule is hidden in the argument.

## ↑ Ancestors (12)

1. [E](../e.md)
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
