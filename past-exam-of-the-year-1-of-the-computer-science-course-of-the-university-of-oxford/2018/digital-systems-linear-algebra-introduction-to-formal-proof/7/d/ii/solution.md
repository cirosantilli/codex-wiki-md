<h1 id="7/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [exclusive-or natural deduction rules](../../../../../../exclusive-or-natural-deduction-rules.md) defined in part (i). The only extra lemma needed is [double-negation introduction](../../../../../../double-negation-introduction.md), derived from the given rules by assuming $\neg Q$ under $Q$, obtaining contradiction, and discharging that assumption. The full proof incorporates that derivation:
```
1. ¬P ⊕ Q               premise
2.   ¬P                 first ⊕E case assumption [i]
3.   ¬Q                 first ⊕E case assumption [j]
4.   P ⊕ ¬Q             ⊕I₂, 2, 3
5.   ¬¬P                second ⊕E case assumption [k]
6.   Q                  second ⊕E case assumption [l]
7.   P                  ¬¬E, 5
8.     ¬Q               assumption [m]
9.     ⊥                ¬E, 6, 8
10.  ¬¬Q                ¬I, 8–9, discharging [m]
11.  P ⊕ ¬Q             ⊕I₁, 7, 10
12. P ⊕ ¬Q              ⊕E, 1, 2–4, 5–11,
                        discharging [i], [j], [k], [l]
```
In the first case the second introduction rule is instantiated with right operand $\neg Q$. In the second case the first introduction rule requires $\neg(\neg Q)$, which is exactly the derived line 10.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [7](../../../7.md)
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
