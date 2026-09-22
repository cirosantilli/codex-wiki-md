<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Introduce the three [logical implications](../../../../../../logical-implication.md) from the outside in. Under assumptions $P\to Q$, $Q\to R$, and $P$, apply the [implication elimination rule](../../../../../../implication-elimination-rule.md) twice, then use [assumption discharge](../../../../../../assumption-discharge.md) in reverse order:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $P\to Q$ | Temporary assumption |
| 2 | $\{1,2\}$ | $Q\to R$ | Temporary assumption |
| 3 | $\{1,2,3\}$ | $P$ | Temporary assumption |
| 4 | $\{1,2,3\}$ | $Q$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 1, 3 |
| 5 | $\{1,2,3\}$ | $R$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 2, 4 |
| 6 | $\{1,2\}$ | $P\to R$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 5; discharge 3 |
| 7 | $\{1\}$ | $(Q\to R)\to(P\to R)$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 6; discharge 2 |
| 8 | $\varnothing$ | $(P\to Q)\to((Q\to R)\to(P\to R))$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 7; discharge 1 |

Thus

$$
\boxed{\vdash(P\to Q)\to((Q\to R)\to(P\to R)).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
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
