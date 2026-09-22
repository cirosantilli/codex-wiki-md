<h1 id="7/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The premise turns an assumed $\neg P$ into a [contradiction](../../../../../../contradiction.md). Use the [negation introduction rule](../../../../../../negation-introduction-rule.md) to obtain $\neg\neg P$, then the supplied classical [double-negation elimination](../../../../../../double-negation-elimination.md) rule:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $\neg P\to\bot$ | Premise |
| 2 | $\{1,2\}$ | $\neg P$ | Temporary assumption |
| 3 | $\{1,2\}$ | $\bot$ | [implication elimination rule](../../../../../../implication-elimination-rule.md) $\to\text{-elim}$ on 1, 2 |
| 4 | $\{1\}$ | $\neg\neg P$ | [negation introduction rule](../../../../../../negation-introduction-rule.md) $\neg\text{-intro}$ on 3; discharge 2 |
| 5 | $\{1\}$ | $P$ | [double-negation elimination](../../../../../../double-negation-elimination.md) $\neg\neg\text{-elim}$ on 4 |

Hence $\boxed{(\neg P\to\bot)\vdash P}$. The final classical rule is essential: deriving $\neg\neg P$ alone is not yet a proof of $P$ in [Intuitionistic propositional logic](../../../../../../intuitionistic-propositional-logic.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
