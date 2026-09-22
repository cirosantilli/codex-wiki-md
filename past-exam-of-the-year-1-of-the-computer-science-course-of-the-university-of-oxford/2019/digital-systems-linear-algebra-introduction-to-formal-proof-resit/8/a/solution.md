<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a finite domain $\{d_1,\ldots,d_n\}$, a true existential premise says that at least one $d_j$ satisfies $\phi$. The [subproof](../../../../../subproof.md) treats its witness as an unknown object named $v$, derives $\kappa$ without relying on which object was chosen, and can therefore be applied to the actual witness. Thus $\kappa$ follows whenever the existential premise is true. This argument does not require knowing the domain's size or selecting a particular named element in advance.

The [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) in sequent form records the same [assumption discharge](../../../../../assumption-discharge.md): a derivation of $\Gamma,\phi(v)\vdash\kappa$ yields $\Gamma,\exists x\,\phi(x)\vdash\kappa$. The natural-deduction box represents the temporary witness assumption that the sequent rule replaces by the existential premise.

The [eigenvariable condition](../../../../../eigenvariable-condition.md) requires that $v$ have no free occurrence in the other undischarged assumptions, the existential premise or the exported conclusion $\kappa$. Bound occurrences can be renamed harmlessly. This freshness condition keeps $v$ from denoting a previously special object and prevents [witness escape](../../../../../witness-escape.md). Without it, one could export $S(v)$ from $\exists x\,S(x)$, falsely asserting that an arbitrarily named object has the witness property. A two-element domain with only one element satisfying $S$ supplies an immediate counterexample.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
