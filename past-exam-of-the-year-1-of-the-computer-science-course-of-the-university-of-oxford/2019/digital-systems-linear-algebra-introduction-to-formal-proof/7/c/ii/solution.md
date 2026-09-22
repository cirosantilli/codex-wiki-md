<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [logical implication](../../../../../../logical-implication.md) associates to the right. Assume its two antecedents, then use nested applications of the [disjunction elimination rule](../../../../../../disjunction-elimination-rule.md).

```
1  | P ∨ Q                              assume
2  | | P ∨ ¬Q                           assume
3  | | | P                              first case of 1
4  | | | P                              available from 3
5  | | | Q                              second case of 1
6  | | | | P                            first case of 2
7  | | | | P                            available from 6
8  | | | | ¬Q                           second case of 2
9  | | | | ⊥                            ¬-elim, 5 and 8
10 | | | | P                            ⊥-elim, 9
11 | | | P                              ∨-elim, 2, cases 6–7 and 8–10
12 | | P                                ∨-elim, 1, cases 3–4 and 5–11
13 | (P ∨ ¬Q) → P                       →-intro, discharge 2–12
14 (P ∨ Q) → ((P ∨ ¬Q) → P)             →-intro, discharge 1–13
```

This [proof](../../../../../../mathematical-proof.md) uses [logical falsity elimination rule](../../../../../../logical-falsity-elimination-rule.md), but does not need [law of excluded middle](../../../../../../law-of-excluded-middle.md) or [double-negation elimination](../../../../../../double-negation-elimination.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
