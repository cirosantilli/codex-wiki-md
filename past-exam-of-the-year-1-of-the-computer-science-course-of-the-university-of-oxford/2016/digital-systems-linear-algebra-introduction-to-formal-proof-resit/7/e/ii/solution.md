<h1 id="7/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Now derive the needed $D$ or $E$ inside its respective [subproof](../../../../../../subproof.md):
```
 1  A → D          premise
 2  ¬A → E         premise
 3  (A ∧ D) → B    premise
 4  (¬A ∧ E) → B   premise
 5  A ∨ ¬A         excluded middle
 6  | A            assumption
 7  | D            →-elim 1,6
 8  | A ∧ D        ∧-intro 6,7
 9  | B            →-elim 3,8
10  | ¬A           assumption
11  | E            →-elim 2,10
12  | ¬A ∧ E       ∧-intro 10,11
13  | B            →-elim 4,12
14  B              ∨-elim 5,6–9,10–13
```
[Implication elimination](../../../../../../implication-elimination-rule.md) supplies the branch-specific premise before [conjunction introduction](../../../../../../conjunction-introduction-rule.md) packages it for the final implication.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
