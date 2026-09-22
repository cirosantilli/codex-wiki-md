<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Capture-safe equality replacement](../../../../../capture-safe-equality-replacement.md) gives the corrected scheme:

$$
\boxed{\vdash x_i=x_j\to(\phi\to\phi'),}
$$

where $\phi'$ replaces selected free occurrences of $x_i$ by $x_j$, without capture. One may equivalently use full capture-avoiding substitution, after renaming conflicting binders. Replacing bound occurrences as though they were free is not permitted.

Here is a syntactic proof. Write $e$ for $x_i=x_j$. First derive symmetry under $e$: A6 and A4 give $x_i=x_i$, and A7 applied to the first position in that atomic equality gives $e\to(x_i=x_i\to x_j=x_i)$. [Modus ponens](../../../../../implication-elimination-rule.md) and the deduction theorem give $\vdash e\to x_j=x_i$. Atomic replacement in the forward direction is A7 itself; in the reverse direction apply A7 with $i,j$ exchanged and use this symmetry. Thus under $e$, an atomic formula and its designated replacement imply each other.

Induct on the formation of $\phi$, proving both directions simultaneously. For [negation](../../../../../negation.md), the reverse implication for the immediate subformula gives the forward implication of its negations by contraposition, and vice versa. For $\theta\to\eta$, the two induction equivalences combine propositionally to $(\theta\to\eta)\leftrightarrow(\theta'\to\eta')$. This uses only the propositional [tautologies](../../../../../tautology.md) allowed in this part.

For $\phi=\forall z\theta$, first take $z$ distinct from $x_i,x_j$. From assumptions $e$ and $\forall z\theta$, A4 gives $\theta$, the induction hypothesis gives $\theta'$, and [generalization](../../../../../universal-generalization-rule.md) gives $\forall z\theta'$: $z$ is free in neither open assumption. Discharge the two assumptions to obtain $e\to(\forall z\theta\to\forall z\theta')$. The reverse direction is identical. If the binder is $x_i$, no free occurrence of that variable lies beneath it and the replacement there is empty. If it is $x_j$, capture avoidance likewise forbids a changed free $x_i$ below that binder unless the binder is first renamed to a fresh variable. Bound-variable renaming is derived from A4 followed by admissible [generalization](../../../../../universal-generalization-rule.md) and A5, with the same freshness restriction. This completes the [structural induction](../../../../../structural-induction.md) and proves the scheme for arbitrary formulas.

## ↑ Ancestors (13)

1. [D](../d.md)
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
