<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The dot after $\forall x$ gives it scope over the following implication: read the premise as $H=\forall x\,(P(x)\to Q(x))$. Choose a fresh arbitrary [eigenvariable](../../../../../../eigenvariable.md) $u$. A [natural deduction](../../../../../../natural-deduction.md) proof is

$$
\begin{array}{rll}
1&H&\text{premise}\\
2&[\forall x\,P(x)]^a&\text{assumption}\\
3&\quad P(u)\to Q(u)&\forall E\ 1\\
4&\quad P(u)&\forall E\ 2\\
5&\quad Q(u)&\to E\ 4,3\\
6&\quad\forall x\,Q(x)&\forall I\ 5\\
7&(\forall x\,P(x))\to(\forall x\,Q(x))&\to I\ (2\text{--}6).
\end{array}
$$

At line 6, $u$ is free in no undischarged assumption, so the [universal quantifier introduction rule](../../../../../../universal-quantifier-introduction-rule.md) is valid.

The proposed variant is not derivable in a sound [first-order logic](../../../../../../first-order-logic.md). For a [countermodel](../../../../../../countermodel.md), use the two-element domain $\{0,1\}$, interpret both [predicates](../../../../../../predicate.md) $P,Q$ as $\{0\}$, and assign the free variable $x$ the value 0. Then $\forall x(P(x)\to Q(x))$ is true, as is $P(x)$ under the assignment, but $\forall x\,Q(x)$ is false at element 1. The premise's bound $x$ and the conclusion's free $x$ have different scopes.

$$
\boxed{H\vdash(\forall x\,P(x))\to(\forall x\,Q(x)),\qquad
H\not\vdash P(x)\to(\forall x\,Q(x)).}
$$

Attempting to generalize from $Q(x)$ in the variant would violate the [eigenvariable condition](../../../../../../eigenvariable-condition.md), because $x$ remains free in the undischarged assumption $P(x)$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
