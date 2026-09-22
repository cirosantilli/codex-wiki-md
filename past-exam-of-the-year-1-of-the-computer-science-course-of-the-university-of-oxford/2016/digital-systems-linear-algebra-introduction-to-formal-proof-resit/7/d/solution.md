<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A derivation of the [law of excluded middle](../../../../../law-of-excluded-middle.md) using only the supplied primitive rules is
```
1  | ¬(A ∨ ¬A)    assumption
2  | | A          assumption
3  | | A ∨ ¬A     ∨-intro-L 2
4  | | ⊥          ¬-elim 3,1
5  | ¬A           ¬-intro 2–4
6  | A ∨ ¬A       ∨-intro-R 5
7  | ⊥            ¬-elim 6,1
8  ¬¬(A ∨ ¬A)     ¬-intro 1–7
9  A ∨ ¬A         ¬¬-elim 8
```
Both boxes have been discharged, so the final formula has no undischarged assumptions.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
