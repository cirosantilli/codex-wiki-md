<h1 id="7/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Abbreviate $H=(\neg P)\to Q$ and $K=(\neg P)\to\neg Q$. Use the primitive [natural deduction](../../../../../../natural-deduction.md) rules, including [double-negation elimination](../../../../../../double-negation-elimination.md):
```
1  H             premise
 2  | H          assumption
 3  | | K        assumption
 4  | | | ¬P     assumption
 5  | | | Q      →-elim 2,4
 6  | | | ¬Q     →-elim 3,4
 7  | | | ⊥      ¬-elim 5,6
 8  | | ¬¬P      ¬-intro 4–7
 9  | | P        ¬¬-elim 8
10  | K → P      →-intro 3–9
11  H → (K → P)  →-intro 2–10
```
The outer premise is redundant: the proof uses the locally assumed $H$, so the conclusion is already a theorem. Keeping the redundant premise is allowed. The successive discharges give **$((\neg P)\to Q)\to(((\neg P)\to\neg Q)\to P)$** with exactly the requested assumption scopes.

## ↑ Ancestors (13)

1. [I](../i.md)
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
