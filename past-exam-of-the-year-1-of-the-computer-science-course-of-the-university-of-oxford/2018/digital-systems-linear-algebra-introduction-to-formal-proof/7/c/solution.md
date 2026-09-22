<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This instance of [Peirce's law](../../../../../peirce-s-law.md) uses the supplied classical [double-negation elimination](../../../../../double-negation-elimination.md) rule. First derive $P\to Q$ while assuming $\neg P$, using [explosion](../../../../../logical-falsity-elimination-rule.md) inside a further temporary assumption.
```
1. (P → Q) → P          premise
2.   ¬P                 assumption [i]
3.     P                assumption [j]
4.     ⊥                ¬E, 2, 3
5.     Q                ⊥E, 4
6.   P → Q              →I, 3–5, discharging [j]
7.   P                  →E, 1, 6
8.   ⊥                  ¬E, 2, 7
9. ¬¬P                  ¬I, 2–8, discharging [i]
10. P                   ¬¬E, 9
```
This is a formal [natural deduction](../../../../../natural-deduction.md) proof from exactly the given premise; no unproved excluded-middle lemma is needed.

## ↑ Ancestors (12)

1. [C](../c.md)
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
