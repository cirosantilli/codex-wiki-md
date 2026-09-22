<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [negation introduction rule](../../../../../../negation-introduction-rule.md) to an assumed existential statement and the [existential quantifier elimination rule](../../../../../../existential-quantifier-elimination-rule.md) with a fresh witness $u$:

$$
\begin{array}{rll}
1&\forall x\,\neg P(x)&\text{premise}\\
2&[\exists x\,P(x)]^a&\text{assumption}\\
3&\quad[P(u)]^b&\text{fresh witness assumption}\\
4&\qquad\neg P(u)&\forall E\ 1\\
5&\qquad\bot&\neg E\ 3,4\\
6&\quad\bot&\exists E\ 2,(3\text{--}5)\\
7&\neg\exists x\,P(x)&\neg I\ (2\text{--}6).
\end{array}
$$

The [eigenvariable condition](../../../../../../eigenvariable-condition.md) holds: $u$ is absent from the surrounding premise, the existential assumption and the exported conclusion $\bot$. Its local assumption is discharged before the final [negation introduction rule](../../../../../../negation-introduction-rule.md).

$$
\boxed{\forall x\,\neg P(x)\vdash\neg\exists x\,P(x).}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
