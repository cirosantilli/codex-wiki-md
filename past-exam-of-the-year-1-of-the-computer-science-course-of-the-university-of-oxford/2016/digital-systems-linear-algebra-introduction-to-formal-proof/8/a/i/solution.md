<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [negation introduction](../../../../../../negation-introduction-rule.md) on the unwanted [existential quantification](../../../../../../existential-quantification.md), and [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) with a fresh witness $a$:
```
1  ∀x. ¬P(x)    premise
2  | ∃x. P(x)   assumption
3  | | P(a)     assumption, a fresh
4  | | ¬P(a)    ∀-elim 1
5  | | ⊥        ¬-elim 3,4
6  | ⊥          ∃-elim 2,3–5
7  ¬(∃x. P(x))  ¬-intro 2–6
```
The witness name occurs neither in the surrounding assumptions nor in the conclusion $\bot$ of its [subproof](../../../../../../subproof.md). This satisfies the [eigenvariable condition](../../../../../../eigenvariable-condition.md); it is not an arbitrarily chosen fixed element assumed to witness the [existential quantification](../../../../../../existential-quantification.md). The result is **$\neg\exists x\,P(x)$**.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
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
