<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the existential statement and eliminate it using a fresh witness $u$. Let $A$ abbreviate $R(u,u)$. Instantiating its [universal quantification](../../../../../universal-quantification.md) at the witness itself gives two incompatible conditional requirements.

```
1  | ∃x ∀y ((R(x,y) → ¬R(y,y)) ∧ (¬R(y,y) → R(y,y)))     assume
2  | | ∀y ((R(u,y) → ¬R(y,y)) ∧ (¬R(y,y) → R(y,y)))        fresh witness
3  | | (A → ¬A) ∧ (¬A → A)                                 ∀-elim, 2, y := u
4  | | A → ¬A                                               ∧-elim-L, 3
5  | | ¬A → A                                               ∧-elim-R, 3
6  | | | A                                                  assume
7  | | | ¬A                                                 →-elim, 6 and 4
8  | | | ⊥                                                  ¬-elim, 6 and 7
9  | | ¬A                                                   ¬-intro, discharge 6–8
10 | | A                                                    →-elim, 9 and 5
11 | | ⊥                                                    ¬-elim, 10 and 9
12 | ⊥                                                      ∃-elim, 1, subproof 2–11
13 ¬∃x ∀y ((R(x,y) → ¬R(y,y)) ∧ (¬R(y,y) → R(y,y)))        ¬-intro, discharge 1–12
```

The [contradiction](../../../../../contradiction.md) at line 12 contains no free witness variable, so the [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) meets its [eigenvariable condition](../../../../../eigenvariable-condition.md). This argument is already valid without [classical first-order logic](../../../../../classical-first-order-logic.md) [double-negation elimination](../../../../../double-negation-elimination.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
