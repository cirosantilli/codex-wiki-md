<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [transfinite induction](../../../../../transfinite-induction.md). The assertion is immediate at stage zero, and at a limit stage it follows by taking the increasing [union](../../../../../set-union.md) of the earlier stages.

Assume $L_\alpha\cap\mathrm{On}=\alpha$. Any [ordinal](../../../../../ordinal-split.md) $\gamma\in L_{\alpha+1}$ is a subset of $L_\alpha$, since members of the [definable power set](../../../../../definable-power-set-split.md) are such subsets. Every element of $\gamma$ is an [ordinal](../../../../../ordinal-split.md), so

$$
\gamma\subseteq L_\alpha\cap\mathrm{On}=\alpha,
$$

which implies $\gamma\leq\alpha$. This gives the upper bound on the [ordinals](../../../../../ordinal-split.md) appearing at the successor stage.

For the reverse inclusion, the smaller [ordinals](../../../../../ordinal-split.md) are already in $L_\alpha$ and hence in $L_{\alpha+1}$. The remaining [ordinal](../../../../../ordinal-split.md) $\alpha$ itself is the definable subset $L_\alpha\cap\mathrm{On}$. The fact used here is **absoluteness of ordinalhood between a [transitive set](../../../../../transitive-set.md) and the universe**: ordinalhood has a bounded definition, and bounded formulas are absolute for [transitive sets](../../../../../transitive-set.md). Thus the formula asserting that a member is an [ordinal](../../../../../ordinal-split.md), interpreted over $L_\alpha$, defines exactly $\alpha$. Therefore $\alpha\in\operatorname{Def}(L_\alpha)=L_{\alpha+1}$.

This proves

$$
\boxed{L_\alpha\cap\mathrm{On}=\alpha\quad\text{for every ordinal }\alpha.}
$$

In particular each [ordinal](../../../../../ordinal-split.md) $\alpha$ is a member of $L_{\alpha+1}$, so $\boxed{\mathrm{On}\subseteq L}$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
