<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G_\Phi=\operatorname{Sat}(\forall\square\Phi)$. By [computation tree logic](../../../../../computation-tree-logic.md) semantics, a [state](../../../../../state-computer-science.md) belongs to $G_\Phi$ exactly when every infinite [path in a transition system](../../../../../path-in-a-transition-system.md) starting there stays in $A=\operatorname{Sat}(\Phi)$ at every position, including position zero. There are no [terminal states](../../../../../terminal-state.md), so every [state](../../../../../state-computer-science.md) lies at the start of an infinite [path in a transition system](../../../../../path-in-a-transition-system.md).

If $s\in G_\Phi$, then $s\in A$. For any successor $t$ of $s$, every infinite [path in a transition system](../../../../../path-in-a-transition-system.md) from $t$ can be prefixed with $s$. Hence every such continuation stays in $A$, so $t\in G_\Phi$. Thus $\operatorname{Post}(s)\subseteq G_\Phi$ and $s\in H(G_\Phi)$.

Conversely, if $s\in H(G_\Phi)$, then $s\in A$ and every successor belongs to $G_\Phi$. Every infinite [path in a transition system](../../../../../path-in-a-transition-system.md) from $s$ therefore has its first [state](../../../../../state-computer-science.md) in $A$ and its entire remaining tail in $A$. Consequently $s\in G_\Phi$. Both inclusions give

$$
\boxed{H(G_\Phi)=G_\Phi,}
$$

so the desired [satisfaction set](../../../../../satisfaction-set.md) is a [fixed point](../../../../../fixed-point.md) of $H$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
