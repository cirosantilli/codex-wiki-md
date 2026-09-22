<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $N$ abbreviate the given negated existential statement, and choose a fresh variable $u$ that is not free in the undischarged premise. Work from an assumed $P(u)$ to $Q(u)$:

```
1  ¬∃x (Q(x) → P(x))                  premise N
2  | P(u)                             assume
3  | | Q(u)                           assume
4  | | P(u)                           available from 2
5  | Q(u) → P(u)                      →-intro, discharge 3–4
6  | ∃x (Q(x) → P(x))                 ∃-intro, witness u in 5
7  | ⊥                                ¬-elim, 6 and 1
8  | Q(u)                             ⊥-elim, 7
9  P(u) → Q(u)                        →-intro, discharge 2–8
10 ∀x (P(x) → Q(x))                   ∀-intro, 9, u fresh
```

The occurrence of $u$ in the [temporary assumption](../../../../../temporary-assumption.md) at line 2 is harmless because that assumption is discharged before [universal quantifier introduction rule](../../../../../universal-quantifier-introduction-rule.md). No unproved implication-creation rule or quantifier-negation equivalence is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
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
