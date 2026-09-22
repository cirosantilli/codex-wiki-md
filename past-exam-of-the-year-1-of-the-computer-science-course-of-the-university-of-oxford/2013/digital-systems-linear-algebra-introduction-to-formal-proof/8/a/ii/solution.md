<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose an arbitrary fresh [eigenvariable](../../../../../../eigenvariable.md) $v$. If $\neg R(v)$ held, [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) would contradict the premise. Derive $R(v)$ by [double-negation elimination](../../../../../../double-negation-elimination.md), then generalize:

<a id="8/a/ii/table-an-arbitrary-object-satisfies-the-relation"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\neg (\exists x\, \neg R(x))$ | Premise |
| 2 | 1, 2 | $\neg R(v)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 3 | 1, 2 | $\exists x\, \neg R(x)$ | [existential quantifier introduction rule](../../../../../../existential-quantifier-introduction-rule.md) 2; term $v$ |
| 4 | 1, 2 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 3, 1 |
| 5 | 1 | $\neg \neg R(v)$ | [negation introduction](../../../../../../negation-introduction-rule.md) 2, 4 |
| 6 | 1 | $R(v)$ | [double-negation elimination](../../../../../../double-negation-elimination.md) 5 |
| 7 | 1 | $\forall y\, R(y)$ | [universal introduction](../../../../../../universal-quantifier-introduction-rule.md) 6; fresh $v$ |

Hence

$$
\boxed{\forall y\,R(y).}
$$

At the final [universal introduction](../../../../../../universal-quantifier-introduction-rule.md), $v$ is free in no open assumption: the only remaining premise is the closed [first-order formula](../../../../../../first-order-formula.md) $\neg\exists x\,\neg R(x)$. Thus the [eigenvariable condition](../../../../../../eigenvariable-condition.md) is satisfied. The passage from double [negation](../../../../../../negation.md) to the positive relation uses the paper's classical rule.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
