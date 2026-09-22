<h1 id="7/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Split on the [law of excluded middle](../../../../../../law-of-excluded-middle.md) for $A$, then use [disjunction elimination](../../../../../../disjunction-elimination-rule.md):
```
 1  D ∧ E          premise
 2  (A ∧ D) → B    premise
 3  (¬A ∧ E) → B   premise
 4  D              ∧-elim-L 1
 5  E              ∧-elim-R 1
 6  A ∨ ¬A         excluded middle
 7  | A            assumption
 8  | A ∧ D        ∧-intro 7,4
 9  | B            →-elim 2,8
10  | ¬A           assumption
11  | ¬A ∧ E       ∧-intro 10,5
12  | B            →-elim 3,11
13  B              ∨-elim 6,7–9,10–12
```
The two occurrences of $B$ have identical type and depend only on the corresponding temporary branch assumption and the original premises.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
