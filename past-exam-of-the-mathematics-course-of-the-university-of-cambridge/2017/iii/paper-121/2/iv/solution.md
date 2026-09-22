<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A suitable [relative condensation lemma](../../../../../../relative-condensation-lemma.md) fixes the base pointwise. Let $\alpha$ be a nonzero [limit ordinal](../../../../../../limit-ordinal.md), and let $Y\prec(L_\alpha(X),\in)$ be an [elementary substructure](../../../../../../elementary-substructure.md) with

$$
X\cup\{X\}\subseteq Y.
$$

Then the [Mostowski collapse theorem](../../../../../../mostowski-collapse-theorem.md) gives an isomorphism $\pi:Y\to T$ onto a [transitive set](../../../../../../transitive-set.md), and

$$
\boxed{T=L_\beta(X)\quad\text{for a nonzero limit ordinal }\beta\leq\alpha,\qquad\pi\!\upharpoonright X=\operatorname{id}_X.}
$$

For the collapse to apply, the restricted membership relation is well-founded because it is actual membership. It is extensional: if two members of $Y$ differ, an element distinguishing them in $L_\alpha(X)$ can be chosen in $Y$ by [elementary substructure](../../../../../../elementary-substructure.md) structure. Since $X$ is transitive and all its members are in $Y$, [transfinite induction](../../../../../../transfinite-induction.md) on their [rank of a set](../../../../../../rank-of-a-set.md) shows that $\pi$ fixes every member of $X$, and then $\pi(X)=X$.

By the preceding [relative constructible level recognition](../../../../../../relative-constructible-level-recognition.md), $L_\alpha(X)\models\Phi(X)$. [Elementary substructure](../../../../../../elementary-substructure.md) agreement transfers this to $Y$, and the collapse isomorphism transfers it to $T$. Thus $T\models\Phi(X)$ and $T=L_\beta(X)$ for a nonzero [limit ordinal](../../../../../../limit-ordinal.md) $\beta$.

For the bound, let $\rho=X\cap\operatorname{Ord}$. The [relative constructible hierarchy](../../../../../../relative-constructible-hierarchy.md) has ordinal height $L_\gamma(X)\cap\operatorname{Ord}=\rho+\gamma$: at a successor the [definable power set](../../../../../../definable-power-set-split.md) adds exactly the previous ordinal height as a new [ordinal](../../../../../../ordinal.md), and at limits take unions. The order type of $Y\cap\operatorname{Ord}$ is at most $\rho+\alpha$, so $\rho+\beta\leq\rho+\alpha$; strict increase of [ordinal addition](../../../../../../ordinal-addition.md) in the right argument gives $\beta\leq\alpha$. The requirement $X\subseteq Y$ is essential to this version: merely having $X\in Y$ need not make the collapse fix the base.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
