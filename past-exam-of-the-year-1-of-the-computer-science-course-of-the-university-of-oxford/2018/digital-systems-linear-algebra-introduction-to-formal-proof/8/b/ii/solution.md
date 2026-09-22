<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take a fresh arbitrary variable $a$. Assuming $R(a)$ would provide precisely the witness forbidden by the premise; discharge that assumption before [universal introduction](../../../../../../universal-quantifier-introduction-rule.md).
```
1. ¬∃x R(x)             premise
2.   R(a)               assumption [i], a fresh
3.   ∃x R(x)            ∃I, 2
4.   ⊥                  ¬E, 1, 3
5. ¬R(a)                ¬I, 2–4, discharging [i]
6. ∀y ¬R(y)             ∀I, 5
```
At line 6, $a$ is free in no undischarged assumption: line 2 has already been discharged. The change of bound variable name is part of the universal-introduction instance.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
