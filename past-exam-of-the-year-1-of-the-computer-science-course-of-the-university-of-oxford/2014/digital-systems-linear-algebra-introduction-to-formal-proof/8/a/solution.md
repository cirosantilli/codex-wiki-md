<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A variable $v$ is fresh for the relevant context when it occurs free in none of its undischarged assumptions. For the [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md), it must also not occur free in the final conclusion $\kappa$ or the existential premise: it is a new [eigenvariable](../../../../../eigenvariable.md), allowed in the temporary witness assumption $\phi(v)$ and formulas inside that witness subproof. Bound variable names can always be renamed to avoid collisions.

The premise $\exists x\,\phi(x)$ guarantees some witness, without saying which object it is. Temporarily call one such witness $v$ and assume $\phi(v)$. If the subproof yields $\kappa$ without depending on any special identity or extra property of $v$, its conclusion holds whichever witness exists. The [existential quantifier elimination rule](../../../../../existential-quantifier-elimination-rule.md) therefore discharges $\phi(v)$ and retains only the original existential premise and other open assumptions.

$$
\boxed{\Gamma,\phi(v)\vdash\kappa\quad\Longrightarrow\quad\Gamma,\exists x\,\phi(x)\vdash\kappa,\qquad v\notin\operatorname{FV}(\Gamma,\kappa,\exists x\,\phi(x)).}
$$

This [eigenvariable condition](../../../../../eigenvariable-condition.md) prevents inferring $\phi(v)$ for a previously chosen object merely from existence. In particular, $\exists x\,Q(x)$ does not license $Q(v)$ outside the discharged witness subproof.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
