<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The proposed proof is invalid:** its existential-elimination step exports $Q(x_0)$ while the witness name $x_0$ still occurs free in that conclusion. Introducing an existential quantifier later does not retrospectively repair that scope error.

Introduce the existential quantifier before discharging the witness box:
```
1  ∀x (P(x) → Q(x))   premise
2  ∃x P(x)            premise
3  | P(a)             assumption, a fresh
4  | P(a) → Q(a)      ∀-elim 1
5  | Q(a)             →-elim 4,3
6  | ∃x Q(x)          ∃-intro 5
7  ∃x Q(x)            ∃-elim 2,3–6
```
The conclusion of [existential elimination](../../../../../existential-quantifier-elimination-rule.md) now has no free occurrence of $a$, and the name occurs in neither original premise, satisfying the [eigenvariable](../../../../../eigenvariable.md) condition.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
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
