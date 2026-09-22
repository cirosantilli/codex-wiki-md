<h1 id="a/1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [thinning rule](../../../../../context-sensitive-hilbert-weakening.md), or [weakening](../../../../../weakening.md), is

$$
\boxed{\frac{\Gamma\vdash\alpha\qquad\Gamma\subseteq\Delta}{\Delta\vdash\alpha}.}
$$

It expresses that extra unused assumptions do not destroy a proof. In the context-sensitive predicate-calculus presentation it also allows a theorem first proved with a fresh [generalization](../../../../../universal-generalization-rule.md) variable to be used later in a context containing that variable free. Simply replaying the same [generalization](../../../../../universal-generalization-rule.md) under the larger context could violate its side condition. For instance a proof of $\forall x(x=x)$ from the empty context may generalize on $x$; it should remain available when an unused assumption $P(x)$ is added, even though that last [generalization](../../../../../universal-generalization-rule.md) could not be replayed with $P(x)$ open.

In propositional calculus the axiom schemes and [modus ponens](../../../../../implication-elimination-rule.md) have no analogous free-variable restriction. An induction on the original proof simply reuses each axiom, assumption and modus-ponens step under the enlarged assumptions, so [weakening](../../../../../weakening.md) is admissible and need not be postulated separately. [Context-sensitive Hilbert weakening](../../../../../context-sensitive-hilbert-weakening.md) concerns this proof presentation: systems already tracking only the assumptions on which each line depends can build admissible [weakening](../../../../../weakening.md) into their treatment of predicate-calculus [generalization](../../../../../universal-generalization-rule.md) as well.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
