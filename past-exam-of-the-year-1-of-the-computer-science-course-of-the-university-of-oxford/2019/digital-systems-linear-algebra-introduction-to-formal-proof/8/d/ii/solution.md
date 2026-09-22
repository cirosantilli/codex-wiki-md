<h1 id="8/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $H$ abbreviate the universal premise, and put $K=Q(c_1)\lor Q(c_2)$. The constants need not denote distinct elements. Use a fresh witness $u$ for the existential, then the justified [three-case disjunction elimination](../../../../../../three-case-disjunction-elimination.md) from (i):

```
1  ∀x (x=c0 ∨ x=c1 ∨ x=c2)              premise H
2  | ¬Q(c0)                            assume
3  | | ∃x Q(x)                         assume
4  | | | Q(u)                          fresh witness for 3
5  | | | u=c0 ∨ u=c1 ∨ u=c2            ∀-elim, 1
6  | | | | u=c0                        first case
7  | | | | Q(c0)                       =-elim, 6 and 4
8  | | | | ⊥                           ¬-elim, 7 and 2
9  | | | | K                           ⊥-elim, 8
10 | | | | u=c1                        second case
11 | | | | Q(c1)                       =-elim, 10 and 4
12 | | | | K                           ∨-intro-L, 11
13 | | | | u=c2                        third case
14 | | | | Q(c2)                       =-elim, 13 and 4
15 | | | | K                           ∨-intro-R, 14
16 | | | K                             3-cases, 5, subproofs 6–9, 10–12, 13–15
17 | | K                               ∃-elim, 3, subproof 4–16
18 | (∃x Q(x)) → K                     →-intro, discharge 3–17
19 ¬Q(c0) → ((∃x Q(x)) → K)             →-intro, discharge 2–18
```

[Equality elimination rule](../../../../../../equality-elimination-rule.md) has exactly the forward orientation displayed in Figure 4: substitute the equal constant for $u$ in $Q(u)$. At line 17 the fresh witness is absent from $K$, $H$ and the remaining assumption. This proves the required [sequent](../../../../../../sequent.md) without assuming that the universe has exactly three distinct objects.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [8](../../../8.md)
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
