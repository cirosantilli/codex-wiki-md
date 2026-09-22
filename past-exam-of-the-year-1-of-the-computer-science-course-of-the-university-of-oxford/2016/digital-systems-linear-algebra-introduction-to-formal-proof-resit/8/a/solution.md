<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a finite domain, an [existential quantifier](../../../../../existential-quantification.md) says that at least one candidate satisfies $\phi$. Reason with a fresh name $v$ for such an unspecified witness. If the same conclusion $\kappa$ follows using only $\phi(v)$ and the original premises, without depending on which candidate $v$ names, then $\kappa$ follows from the existential premise itself.

This is exactly [existential elimination](../../../../../existential-quantifier-elimination-rule.md) in boxed form: the sequent $\Gamma,\phi(v)\vdash\kappa$ is the branch inside the box. The [eigenvariable](../../../../../eigenvariable.md) $v$ must not occur free in the original undischarged context or in the exported conclusion $\kappa$. Otherwise the proof could smuggle in information about a specially chosen individual or export a fact about a witness whose name has just left scope. Freshness does not mean that the domain contains an additional object; it means that its temporary name carries no other assumptions.

## ↑ Ancestors (12)

1. [A](../a.md)
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
