<h1 id="8/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose distinct fresh parameters $a,b$. Within the assumption $a=b$, [equality elimination rule](../../../../../../equality-elimination-rule.md) gives the forward implication directly. Derive the reverse equality explicitly before using it for the reverse implication:
```
1  | a = b                                           assumption
 2  | | P(a)                                         assumption
 3  | | P(b)                                         =-elim 1,2
 4  | P(a) → P(b)                                    →-intro 2–3
 5  | a = a                                          =-intro
 6  | b = a                                          =-elim 1,5; φ(u) := (u = a)
 7  | | P(b)                                         assumption
 8  | | P(a)                                         =-elim 6,7
 9  | P(b) → P(a)                                    →-intro 7–8
10  | (P(a) → P(b)) ∧ (P(b) → P(a))                  ∧-intro 4,9
11  a = b → ((P(a) → P(b)) ∧ (P(b) → P(a)))          →-intro 1–10
12  ∀y. a = y → ((P(a) → P(y)) ∧ (P(y) → P(a)))      ∀-intro 11, b fresh
13  ∀x. ∀y. x = y → ((P(x) → P(y)) ∧ (P(y) → P(x)))  ∀-intro 12, a fresh
```
The equality assumption is discharged before either [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md). There are then no undischarged assumptions, so both [eigenvariable condition](../../../../../../eigenvariable-condition.md) requirements hold. The final **universal theorem** expresses that equal arguments are interchangeable in the [predicate](../../../../../../predicate.md) $P$ in both directions.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
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
