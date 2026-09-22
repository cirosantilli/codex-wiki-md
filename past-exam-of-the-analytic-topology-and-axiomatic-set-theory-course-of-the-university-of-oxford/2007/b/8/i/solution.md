<h1 id="b/8/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a set $A$, its [definable power set](../../../../../definable-power-set-split.md) is

$$
\operatorname{Def}(A)=\{\{x\in A:\langle A,\in\rangle\models\varphi(x,p_1,\ldots,p_n)\}:\varphi\text{ a formula},\ p_1,\ldots,p_n\in A\}.
$$

Only finitely many parameters occur in each definition. Satisfaction for the set structure is definable, so this specifies a uniformly definable class function assigning a set to every set $A$, with $\operatorname{Def}(A)\subseteq\mathcal P(A)$. Every subset definable over the structure with its parameters occurs. The full set $A$ itself occurs by the formula $x=x$. If $A$ is transitive, then $A\subseteq\operatorname{Def}(A)$, since any $p\in A$ is defined as a subset of $A$ by $x\in p$. In that case $\operatorname{Def}(A)$ is transitive as well: a member of one of its elements lies in $A$, hence in $\operatorname{Def}(A)$.

The [constructible hierarchy](../../../../../constructible-hierarchy.md) and universe are

$$
\boxed{L_0=\varnothing,\quad L_{\alpha+1}=\operatorname{Def}(L_\alpha),\quad L_\lambda=\bigcup_{\beta<\lambda}L_\beta,\quad L=\bigcup_{\alpha\in\operatorname{Ord}}L_\alpha.}
$$

The displayed properties prove by induction that levels are transitive and increasing, so $L$ is transitive. It contains every [ordinal](../../../../../ordinal-split.md): inductively $L_\alpha\cap\operatorname{Ord}=\alpha$, and the subset of $L_\alpha$ consisting of [ordinals](../../../../../ordinal-split.md) is definable there, giving $\alpha\in L_{\alpha+1}$. Ordinalhood is absolute here because the levels are transitive. Both the level function and membership in $L$ are definable in $ZF$. This is Gödel's [constructible universe](../../../../../constructible-universe.md), which can contain fewer subsets than the full universe.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
