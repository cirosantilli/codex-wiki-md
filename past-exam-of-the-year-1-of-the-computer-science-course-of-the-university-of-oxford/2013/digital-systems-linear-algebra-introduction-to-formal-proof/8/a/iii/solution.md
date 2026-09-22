<h1 id="8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The original scan repeats the premise and conclusion of part (i) exactly; it is not a missing or unreadable alternative exercise.[Printed p. 8, Question 8(a)(i) and (iii)](../../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2013.md) Here is a second formal ordering of the same argument. First introduce the fresh [existential witness](../../../../../../existential-witness.md), derive the desired [negation](../../../../../../negation.md) inside its scope, and then eliminate the witness:

<a id="8/a/iii/table-close-the-negation-subproof-before-eliminating-the-witness"></a>
| Line | Open assumptions | Formula | Justification |
| --- | --- | --- | --- |
| 1 | 1 | $\exists x\, R(x)$ | Premise |
| 2 | 1, 2 | $R(v)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 3 | 1, 2, 3 | $\forall y\, \neg R(y)$ | [Temporary assumption](../../../../../../temporary-assumption.md) |
| 4 | 1, 2, 3 | $\neg R(v)$ | [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) 3; term $v$ |
| 5 | 1, 2, 3 | $\bot$ | [negation elimination rule](../../../../../../negation-elimination-rule.md) 2, 4 |
| 6 | 1, 2 | $\neg (\forall y\, \neg R(y))$ | [negation introduction](../../../../../../negation-introduction-rule.md) 3, 5 |
| 7 | 1 | $\neg (\forall y\, \neg R(y))$ | [existential elimination](../../../../../../existential-quantifier-elimination-rule.md) 1, 2, 6; fresh $v$ |

Thus, again,

$$
\boxed{\neg\forall y\,\neg R(y).}
$$

At the last [existential elimination](../../../../../../existential-quantifier-elimination-rule.md), $v$ occurs in neither the exported conclusion nor the remaining premise. The [eigenvariable condition](../../../../../../eigenvariable-condition.md) is therefore satisfied. This proof retains a different nesting of the [subproofs](../../../../../../subproof.md) from part (i).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
