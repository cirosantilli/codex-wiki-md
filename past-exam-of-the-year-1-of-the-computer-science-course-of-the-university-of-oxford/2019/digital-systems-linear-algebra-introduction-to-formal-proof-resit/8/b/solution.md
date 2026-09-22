<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The displayed derivation is invalid, although its final conjecture is valid.** Its existential-elimination step exports $T(x_0)$ with the local witness name still free, violating the [eigenvariable condition](../../../../../eigenvariable-condition.md). Introducing an existential quantifier afterwards does not repair that earlier invalid rule application.

Move the [existential quantifier introduction rule](../../../../../existential-quantifier-introduction-rule.md) inside the witness scope:

| Line | Formula | Justification |
| --- | --- | --- |
| 1 | $\forall x\,(S(x)\to T(x))$ | Premise |
| 2 | $\exists x\,S(x)$ | Premise |
| 3 | $S(u)$ | Assume with fresh $u$ |
| 4 | $S(u)\to T(u)$ | [Universal quantifier elimination rule](../../../../../universal-quantifier-elimination-rule.md), 1 |
| 5 | $T(u)$ | [Implication elimination rule](../../../../../implication-elimination-rule.md), 3 and 4 |
| 6 | $\exists x\,T(x)$ | [Existential quantifier introduction rule](../../../../../existential-quantifier-introduction-rule.md), 5 |
| 7 | $\exists x\,T(x)$ | [Existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md), 2 and 3–6 |

The exported formula contains no free $u$, and neither original premise contains that name. The witness assumption is now discharged legally.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
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
