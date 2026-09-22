<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X$ be any [fixed point](../../../../../fixed-point.md) of $H$. Then

$$
X=H(X)=A\cap\{s:\operatorname{Post}(s)\subseteq X\},
$$

so $X\subseteq A$ and every successor of every member of $X$ belongs to $X$. Take $s_0\in X$ and an arbitrary infinite [path in a transition system](../../../../../path-in-a-transition-system.md) $s_0s_1s_2\cdots$ from $s_0$. By [mathematical induction](../../../../../mathematical-induction.md), every $s_i$ belongs to $X$: the base case is the choice of $s_0$, and $s_i\in X$ implies $s_{i+1}\in\operatorname{Post}(s_i)\subseteq X$.

Since $X\subseteq A$, the whole [path in a transition system](../../../../../path-in-a-transition-system.md) stays in $A$. The [path in a transition system](../../../../../path-in-a-transition-system.md) was arbitrary, so $s_0\models\forall\square\Phi$. Thus $s_0\in G_\Phi$, and since $s_0$ was arbitrary in $X$,

$$
X\subseteq G_\Phi.
$$

Part (b) proves that $G_\Phi$ itself is a [fixed point](../../../../../fixed-point.md). Therefore

$$
\boxed{\operatorname{Sat}(\forall\square\Phi)=\nu X.\,H(X),}
$$

the [greatest fixed point](../../../../../greatest-fixed-point.md) with respect to [set inclusion](../../../../../set-inclusion.md). In fact the same induction works for every $X\subseteq H(X)$, showing why a successor-closed [set](../../../../../set-split.md) of good [states](../../../../../state-computer-science.md) certifies this universal property.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
