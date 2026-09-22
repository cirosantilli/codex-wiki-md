<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [negation introduction](../../../../../negation-introduction-rule.md) separately to the two disjuncts, then [conjunction introduction](../../../../../conjunction-introduction-rule.md):
```
 1  ¬(E ∨ F)      premise
 2  | E           assumption
 3  | E ∨ F       ∨-intro-L 2
 4  | ⊥           ¬-elim 3,1
 5  ¬E            ¬-intro 2–4
 6  | F           assumption
 7  | E ∨ F       ∨-intro-R 6
 8  | ⊥           ¬-elim 7,1
 9  ¬F            ¬-intro 6–8
10  ¬E ∧ ¬F       ∧-intro 5,9
```
No assumption from either branch remains open in the conclusion apart from the original premise.

## ↑ Ancestors (12)

1. [B](../b.md)
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
