<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under $P$, the first assumption yields $Q\to R$, while the second yields $Q$. Apply the [implication elimination rule](../../../../../../implication-elimination-rule.md) once more to obtain $R$, and discharge the three temporary assumptions:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $P\to(Q\to R)$ | Temporary assumption |
| 2 | $\{1,2\}$ | $P\to Q$ | Temporary assumption |
| 3 | $\{1,2,3\}$ | $P$ | Temporary assumption |
| 4 | $\{1,2,3\}$ | $Q\to R$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 1, 3 |
| 5 | $\{1,2,3\}$ | $Q$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 2, 3 |
| 6 | $\{1,2,3\}$ | $R$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 4, 5 |
| 7 | $\{1,2\}$ | $P\to R$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 6; discharge 3 |
| 8 | $\{1\}$ | $(P\to Q)\to(P\to R)$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 7; discharge 2 |
| 9 | $\varnothing$ | $(P\to(Q\to R))\to((P\to Q)\to(P\to R))$ | [implication introduction rule](../../../../../../implication-introduction-rule.md) $\to\text{-intro}$ on 8; discharge 1 |

The two uses of $P$ are permitted in ordinary [natural deduction](../../../../../../natural-deduction.md). Therefore

$$
\boxed{\vdash(P\to(Q\to R))\to((P\to Q)\to(P\to R)).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
