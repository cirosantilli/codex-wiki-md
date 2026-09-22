<h1 id="a/2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For this calculus the [deduction theorem for propositional logic](../../../../../deduction-theorem-for-propositional-logic.md) is

$$
\boxed{\Gamma\cup\{\alpha\}\vdash\beta
\quad\Longleftrightarrow\quad\Gamma\vdash\alpha\to\beta.}
$$

For the reverse [logical implication](../../../../../logical-implication.md), retain the [logical derivation](../../../../../logical-derivation.md) from $\Gamma$, add the assumption $\alpha$, and use [modus ponens rule](../../../../../implication-elimination-rule.md).

For the forward [logical implication](../../../../../logical-implication.md), induct on a [logical derivation](../../../../../logical-derivation.md) from $\Gamma\cup\{\alpha\}$. For each line $\delta$ we construct a [logical derivation](../../../../../logical-derivation.md) of $\alpha\to\delta$ from $\Gamma$. If $\delta=\alpha$, use (ii). If $\delta$ is an axiom instance or belongs to $\Gamma$, it is already derivable from $\Gamma$; L1 gives $\delta\to(\alpha\to\delta)$, and [modus ponens rule](../../../../../implication-elimination-rule.md) finishes that case.

If $\delta$ comes from $\eta$ and $\eta\to\delta$ by [modus ponens rule](../../../../../implication-elimination-rule.md), the [induction hypothesis](../../../../../induction-hypothesis.md) supplies

$$
\Gamma\vdash\alpha\to\eta,\qquad
\Gamma\vdash\alpha\to(\eta\to\delta).
$$

Part (iii) supplies $\Gamma\vdash\alpha\to\delta$.

If $\delta$ comes by the elimination rule E from $\eta\to\delta$ and $\neg\eta\to\delta$, the [induction hypothesis](../../../../../induction-hypothesis.md) supplies

$$
\Gamma\vdash\alpha\to(\eta\to\delta),\qquad
\Gamma\vdash\alpha\to(\neg\eta\to\delta).
$$

The L2 instance with $(\alpha,\beta,\gamma)=(\alpha,\eta,\delta)$ combines these by two applications of [modus ponens rule](../../../../../implication-elimination-rule.md). Thus the rule E also survives the discharge construction. These are all possible lines, proving the theorem for the final line $\beta$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
