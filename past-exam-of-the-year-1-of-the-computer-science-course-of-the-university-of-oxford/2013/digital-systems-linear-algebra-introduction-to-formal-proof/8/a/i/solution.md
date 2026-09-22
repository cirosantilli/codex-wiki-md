<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume that every object fails $R$. A fresh [existential witness](../../../../../../existential-witness.md) for the premise then has both $R$ and its [negation](../../../../../../negation.md). Eliminate the witness before closing the assumption about all objects:

<a id="8/a/i/table-eliminate-the-witness-inside-the-negation-subproof"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\exists x\, R(x)$ | Premise |
| 2 | 1, 2 | $\forall y\, \neg R(y)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 3 | 1, 2, 3 | $R(v)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 4 | 1, 2, 3 | $\neg R(v)$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) 2; term $v$ |
| 5 | 1, 2, 3 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 3, 4 |
| 6 | 1, 2 | $\bot$ | [existential elimination](../../../../../../existential-quantifier-elimination-rule.md) 1, 3, 5; fresh $v$ |
| 7 | 1 | $\neg (\forall y\, \neg R(y))$ | [negation introduction](../../../../../../negation-introduction-rule.md) 2, 6 |

The conclusion is

$$
\boxed{\neg\forall y\,\neg R(y).}
$$

The witness $v$ occurs neither in the conclusion of [existential elimination](../../../../../../existential-quantifier-elimination-rule.md) nor in its other open assumptions, so the [eigenvariable condition](../../../../../../eigenvariable-condition.md) holds.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
