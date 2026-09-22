<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the already proved inference in (a) on the negated existential premise. Eliminate the remaining existential with a fresh witness $u$, which must not appear in the final conclusion or the other undischarged assumptions.

```
1  ∃x P(x)                              premise
2  ¬∃x (Q(x) → P(x))                    premise
3  ∀x (P(x) → Q(x))                     derivation in (a), from 2
4  | P(u)                               fresh-witness assumption for 1
5  | P(u) → Q(u)                        ∀-elim, 3
6  | Q(u)                               →-elim, 4 and 5
7  | P(u) ∧ Q(u)                        ∧-intro, 4 and 6
8  | ∃x (P(x) ∧ Q(x))                   ∃-intro, witness u
9  ∃x (P(x) ∧ Q(x))                     ∃-elim, 1, subproof 4–8
```

The result in (a) is a proved dependency, not an additional [axiom](../../../../../axiom.md). The witness introduced at line 4 does not escape its subproof.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
