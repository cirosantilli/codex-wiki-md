<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the complete [logical derivation](../../../../../logical-derivation.md) of the [law of excluded middle](../../../../../law-of-excluded-middle.md) in (a) to $Q$, obtaining $Q\lor\neg Q$. Then use the [disjunction elimination rule](../../../../../disjunction-elimination-rule.md), constructing each [logical implication](../../../../../logical-implication.md) by an explicit hypothetical subproof:

```
1  Q ∨ ¬Q                              result of (a), φ := Q
2  | Q                                 first case
3  | | P                               assume
4  | | Q                               available from 2
5  | P → Q                             →-intro, discharge 3–4
6  | (P → Q) ∨ (P → ¬Q)                ∨-intro-L, 5
7  | ¬Q                                second case
8  | | P                               assume
9  | | ¬Q                              available from 7
10 | P → ¬Q                            →-intro, discharge 8–9
11 | (P → Q) ∨ (P → ¬Q)                ∨-intro-R, 10
12 (P → Q) ∨ (P → ¬Q)                  ∨-elim, 1, cases 2–6 and 7–11
```

Both case assumptions and both hypothetical $P$ assumptions have been discharged. Thus the conclusion is a theorem, not a [logical implication](../../../../../logical-implication.md) that depends on assuming $P$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
