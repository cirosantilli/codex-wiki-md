<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First derive $A$ by [double-negation elimination](../../../../../../double-negation-elimination.md), then derive $\neg B$ by [negation introduction](../../../../../../negation-introduction-rule.md). The [logical falsity elimination rule](../../../../../../logical-falsity-elimination-rule.md) is used only inside the attempt to derive $A$.
```
1  ¬(A → B)  premise
 2  | ¬A     assumption
 3  | | A    assumption
 4  | | ⊥    ¬-elim 3,2
 5  | | B    ⊥-elim 4
 6  | A → B  →-intro 3–5
 7  | ⊥      ¬-elim 6,1
 8  ¬¬A      ¬-intro 2–7
 9  A        ¬¬-elim 8
10  | B      assumption
11  | | A    assumption
12  | | B    reiteration 10
13  | A → B  →-intro 11–12
14  | ⊥      ¬-elim 13,1
15  ¬B       ¬-intro 10–14
16  A ∧ ¬B   ∧-intro 9,15
```
Reiteration at line 12 merely uses an assumption that remains in scope. The final **$A\land\neg B$** follows by [conjunction introduction](../../../../../../conjunction-introduction-rule.md). This explicitly supplies the classical step needed to obtain $A$ rather than just $\neg\neg A$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
