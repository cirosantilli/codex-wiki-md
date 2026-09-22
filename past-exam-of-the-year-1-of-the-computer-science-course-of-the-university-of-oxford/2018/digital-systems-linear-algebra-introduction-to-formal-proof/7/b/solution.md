<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [disjunction introduction](../../../../../disjunction-introduction-rule.md), [negation introduction](../../../../../negation-introduction-rule.md) and [conjunction introduction](../../../../../conjunction-introduction-rule.md) in the following [natural deduction](../../../../../natural-deduction.md) proof. Indentation marks the assumptions discharged at their closing lines.
```
1. ¬(φ ∨ ψ)             premise
2.   φ                  assumption [i]
3.   φ ∨ ψ              ∨I-left, 2
4.   ⊥                  ¬E, 1, 3
5. ¬φ                   ¬I, 2–4, discharging [i]
6.   ψ                  assumption [j]
7.   φ ∨ ψ              ∨I-right, 6
8.   ⊥                  ¬E, 1, 7
9. ¬ψ                   ¬I, 6–8, discharging [j]
10. ¬φ ∧ ¬ψ             ∧I, 5, 9
```
The two separate temporary assumptions establish the two required negations; neither is retained in the conclusion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
