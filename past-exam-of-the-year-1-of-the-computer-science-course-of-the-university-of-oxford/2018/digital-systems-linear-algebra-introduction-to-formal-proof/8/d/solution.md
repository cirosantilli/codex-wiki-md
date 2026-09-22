<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the two [existential elimination](../../../../../existential-quantifier-elimination-rule.md) scopes nested. Let $b$ witness the outer existential and $a$ the inner one, both fresh. Inside them, [negation introduction](../../../../../negation-introduction-rule.md) proves the required counterexample to $P$ without invoking an unproved contraposition lemma.
```
1. ∀x ∀y (P(x,y) → Q(x,y))          premise
2.   ∃y ∃x ¬Q(x,y)                  assumption [i]
3.     ∃x ¬Q(x,b)                   fresh witness assumption [j]
4.       ¬Q(a,b)                    fresh witness assumption [k]
5.       ∀y (P(a,y) → Q(a,y))        ∀E, 1
6.       P(a,b) → Q(a,b)             ∀E, 5
7.         P(a,b)                   assumption [l]
8.         Q(a,b)                   →E, 6, 7
9.         ⊥                        ¬E, 4, 8
10.      ¬P(a,b)                    ¬I, 7–9, discharging [l]
11.      ∃x ¬P(x,b)                 ∃I, 10
12.      ∃y ∃x ¬P(x,y)              ∃I, 11
13.    ∃y ∃x ¬P(x,y)                ∃E, 3, 4–12, discharging [k]
14.  ∃y ∃x ¬P(x,y)                 ∃E, 2, 3–13, discharging [j]
15. (∃y ∃x ¬Q(x,y)) → (∃y ∃x ¬P(x,y))
                                   →I, 2–14, discharging [i]
```
The result at lines 12–14 has no free occurrence of either fresh witness. At the inner discharge, $a$ is absent from the remaining assumptions; at the outer discharge, $b$ is absent from the premise and final conclusion. Hence the [eigenvariable conditions](../../../../../eigenvariable-condition.md) hold at both eliminations.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
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
