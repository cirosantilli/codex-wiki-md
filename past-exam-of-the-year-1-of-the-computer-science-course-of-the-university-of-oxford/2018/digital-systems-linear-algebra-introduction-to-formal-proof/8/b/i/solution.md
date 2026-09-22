<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a fresh witness $a$ in the [existential elimination](../../../../../../existential-quantifier-elimination-rule.md) subproof. The [universal elimination](../../../../../../universal-quantifier-elimination-rule.md) step gives the opposite of its assumed negated property.
```
1. ∀x R(x)              premise
2.   ∃y ¬R(y)           assumption [i]
3.     ¬R(a)            fresh witness assumption [j]
4.     R(a)             ∀E, 1
5.     ⊥                ¬E, 3, 4
6.   ⊥                  ∃E, 2, 3–5, discharging [j]
7. ¬∃y ¬R(y)            ¬I, 2–6, discharging [i]
```
The witness $a$ is absent from the premise and from the conclusion of the existential-elimination step, so its freshness condition is met.

## ↑ Ancestors (13)

1. [I](../i.md)
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
