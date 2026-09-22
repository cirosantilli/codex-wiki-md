<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $U=\forall x_i\neg\phi$ and $H=\neg U\to\psi$. All derivations below use the printed replacement axiom, so they do not rely on the false equivalence from part (a).

The identity [logical implication](../../../../../logical-implication.md) $\neg A\to\neg A$ follows by the deduction rule. Substituting $\alpha=\neg A$, $\beta=A$ into the replacement axiom and applying [modus ponens rule](../../../../../implication-elimination-rule.md) therefore gives double-negation elimination:

$$
\vdash\neg\neg A\to A.
$$

Universal instantiation gives $\vdash U\to\neg\phi$. Combine it with $\vdash\neg\neg U\to U$ using [modus ponens rule](../../../../../implication-elimination-rule.md) under a temporary assumption and then the deduction rule, obtaining $\vdash\neg\neg U\to\neg\phi$.

In the replacement axiom now substitute $\alpha=\neg\phi$ and $\beta=\neg U$. Its antecedent is precisely the last theorem, and its consequent is $\neg\neg\phi\to\neg U$. Thus

$$
\vdash\neg\neg\phi\to\neg\forall x_i\neg\phi.
$$

Under the fixed assumption $H$ and temporary assumption $\neg\neg\phi$, [modus ponens rule](../../../../../implication-elimination-rule.md) gives $\neg U$ and then $\psi$. Discharge the temporary assumption to obtain $H\vdash\neg\neg\phi\to\psi$.

Finally apply universal generalization. The variable $x_i$ is not free in $H$, because it is bound in $U$ and is not free in $\psi$ by hypothesis. Hence the side condition is satisfied and

$$
\boxed{\{\neg\forall x_i\neg\phi\to\psi\}\vdash\forall x_i(\neg\neg\phi\to\psi).}
$$

Generalization is applied after the temporary assumption has been discharged; applying it while that assumption remained open would not be justified.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
