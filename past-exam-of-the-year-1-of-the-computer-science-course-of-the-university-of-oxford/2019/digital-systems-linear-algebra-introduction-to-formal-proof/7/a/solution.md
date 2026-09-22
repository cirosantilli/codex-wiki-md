<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use only the displayed [natural deduction](../../../../../natural-deduction.md) rules. Let $A$ abbreviate $\phi\lor\neg\phi$. Indentation below marks [temporary assumptions](../../../../../temporary-assumption.md); the closing rule names the assumption discharged.

```
1  | ¬A                         assume
2  | | φ                        assume
3  | | A                        ∨-intro-L, 2
4  | | ⊥                        ¬-elim, 3 and 1
5  | ¬φ                         ¬-intro, discharge 2–4
6  | A                          ∨-intro-R, 5
7  | ⊥                          ¬-elim, 6 and 1
8  ¬¬A                          ¬-intro, discharge 1–7
9  A                            ¬¬-elim, 8
```

There are no undischarged assumptions at line 9, so this proves the [law of excluded middle](../../../../../law-of-excluded-middle.md). The use of [double-negation elimination](../../../../../double-negation-elimination.md) is explicit; an unproved appeal to the derived RAA rule is unnecessary.

## ↑ Ancestors (12)

1. [A](../a.md)
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
