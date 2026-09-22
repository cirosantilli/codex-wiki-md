<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [equality introduction rule](../../../../../../equality-introduction-rule.md) to prove $t_1=t_1$. In the [equality elimination rule](../../../../../../equality-elimination-rule.md), choose the [first-order formula](../../../../../../first-order-formula.md) $\phi(z)$ to be $z=t_1$. Substituting $t_2$ for $t_1$ in its first position proves symmetry:

| Line | Context | Formula | Justification |
| --- | --- | --- | --- |
| 1 | $\{1\}$ | $t_1=t_2$ | Premise |
| 2 | $\{1\}$ | $t_1=t_1$ | [equality introduction rule](../../../../../../equality-introduction-rule.md) $=\text{-intro}$ |
| 3 | $\{1\}$ | $t_2=t_1$ | [equality elimination rule](../../../../../../equality-elimination-rule.md) $=\text{-elim}$ on 1, 2 |

Thus $\boxed{t_1=t_2\vdash t_2=t_1}$. This uses only the two supplied equality rules; symmetry has not been assumed as an additional rule.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
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
