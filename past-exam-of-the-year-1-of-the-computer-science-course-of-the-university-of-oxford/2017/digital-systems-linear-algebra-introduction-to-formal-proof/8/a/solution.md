<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a finite domain $\{d_1,\ldots,d_m\}$, $\exists x\,\phi(x)$ says that at least one of $\phi(d_1),\ldots,\phi(d_m)$ holds. A derivation from a fresh generic witness shows how to obtain the same conclusion $\kappa$ whichever witness works, just as [disjunction elimination](../../../../../disjunction-elimination-rule.md) handles all cases. If empty domains were allowed, the existential premise would be false there; ordinary first-order semantics normally assumes a nonempty domain.

Writing the other open assumptions as $\Gamma$, the [existential elimination](../../../../../existential-quantifier-elimination-rule.md) rule in sequent form is

$$
\frac{\Gamma,\phi(v)\vdash\kappa}{\Gamma,\exists x\,\phi(x)\vdash\kappa}.
$$

Combining this with a derivation of the existential premise gives the displayed natural-deduction version. The [eigenvariable condition](../../../../../eigenvariable-condition.md) requires $v$ to occur free in neither $\Gamma$ nor $\kappa$, with capture-free substitution in $\phi(v)$. It is a temporary name for an unspecified witness, not information about a chosen object. Without freshness, the invalid inference $\exists x\,P(x)\vdash P(v)$ would identify an arbitrary named object with that witness. The [witness escape](../../../../../witness-escape.md) restriction prevents this error.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
