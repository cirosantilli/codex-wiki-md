<h1 id="a/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose a fresh variable $x_3$. In A7 take the equality antecedent $x_3=x_1$, the atomic formula $\phi=(x_3=x_2)$, and replace its occurrence of $x_3$ by $x_1$. This gives directly the theorem

$$
\vdash x_3=x_1\to(x_3=x_2\to x_1=x_2).
$$

Generalize on $x_3$, with no open assumptions. A4 then instantiates that [quantifier](../../../../../quantifier.md) with the term $f(x_0)$. The substitution is free for $x_3$, since the matrix contains no [quantifiers](../../../../../quantifier.md). One modus-ponens step yields

$$
\vdash f(x_0)=x_1\to(f(x_0)=x_2\to x_1=x_2).
$$

Finally generalize, in order, on $x_2$, $x_1$, and $x_0$. The result is

$$
\boxed{\vdash\forall x_0\forall x_1\forall x_2\,[f(x_0)=x_1\to(f(x_0)=x_2\to x_1=x_2)].}
$$

Every step is A7, [generalization](../../../../../universal-generalization-rule.md), A4, or [modus ponens](../../../../../implication-elimination-rule.md). Neither completeness, adequacy, nor an unproved appeal to all propositional [tautologies](../../../../../tautology.md) is needed. In particular the proof does not silently upgrade the variable-only equality axiom to an arbitrary-term axiom: quantification and instantiation perform that upgrade explicitly.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
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
