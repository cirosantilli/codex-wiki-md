<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $H(t)=\forall p\,((S(t,p)\to\neg S(p,p))\land(\neg S(p,p)\to S(t,p)))$. Use [negation introduction](../../../../../negation-introduction-rule.md) on the existential claim. For its fresh witness $b$, instantiate $p=b$; the resulting self-application says both $S(b,b)\to\neg S(b,b)$ and its reverse. The given [law of excluded middle](../../../../../law-of-excluded-middle.md) then provides the two cases.
```
1  ∀x. ∀y. (S(x,y) ∨ ¬S(x,y))                    premise
 2  | ∃b. H(b)                                   assumption
 3  | | H(b)                                     assumption, b fresh
 4  | | (S(b,b) → ¬S(b,b)) ∧ (¬S(b,b) → S(b,b))  ∀-elim 3, p := b
 5  | | S(b,b) → ¬S(b,b)                         ∧-elim-L 4
 6  | | ¬S(b,b) → S(b,b)                         ∧-elim-R 4
 7  | | ∀y. (S(b,y) ∨ ¬S(b,y))                   ∀-elim 1, x := b
 8  | | S(b,b) ∨ ¬S(b,b)                         ∀-elim 7, y := b
 9  | | | S(b,b)                                 assumption
10  | | | ¬S(b,b)                                →-elim 5,9
11  | | | ⊥                                      ¬-elim 9,10
12  | | | ¬S(b,b)                                assumption (new case)
13  | | | S(b,b)                                 →-elim 6,12
14  | | | ⊥                                      ¬-elim 13,12
15  | | ⊥                                        ∨-elim 8,9–11,12–14
16  | ⊥                                          ∃-elim 2,3–15
17  ¬∃b. H(b)                                    ¬-intro 2–16
```
Both case assumptions are discharged at line 15; the witness assumption is discharged at line 16. Since $b$ is absent from the surrounding premise and the exported conclusion $\bot$, [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) is valid. Line 17 is **the required negated existential**. This is the diagonal self-application underlying the [barber paradox](../../../../../barber-paradox.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
