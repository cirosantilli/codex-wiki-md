<h1 id="a/2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Suppose both extensions were inconsistent. By the [explosion](../../../../../logical-falsity-elimination-rule.md) argument in (i), the extension by $\phi$ proves $\neg\phi$, and the extension by $\neg\phi$ proves $\phi$. The [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) therefore yields

$$
\Gamma\vdash\phi\to\neg\phi,\qquad
\Gamma\vdash\neg\phi\to\phi.
$$

The identity theorem gives $\vdash\neg\phi\to\neg\phi$ and $\vdash\phi\to\phi$. Apply E to the first displayed [logical implication](../../../../../logical-implication.md) and the identity [logical implication](../../../../../logical-implication.md) with antecedent $\neg\phi$ to obtain $\Gamma\vdash\neg\phi$. Apply E to the identity [logical implication](../../../../../logical-implication.md) with antecedent $\phi$ and the second displayed [logical implication](../../../../../logical-implication.md) to obtain $\Gamma\vdash\phi$. This contradicts [propositional consistency](../../../../../propositional-consistency.md) of $\Gamma$.

Consequently **at least one of the two one-formula extensions is [propositionally consistent](../../../../../propositional-consistency.md)**. The [formal proof](../../../../../formal-proof.md) uses the source's own calculus, including its rule E, rather than assuming an unproved completeness theorem for this presentation.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
