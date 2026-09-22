<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We prove exhaustiveness, including existence of the positive density when neither form of [arbitrage](../../../../../../arbitrage.md) occurs. Use the subspace $L$ from part (a)(ii), and consider

$$
\mathcal K=\{\mathbb E[\nu A_1]:\nu>0\text{ almost surely},\ \mathbb E[\nu\|A_1\|]<\infty\}\subseteq L.
$$

This is a nonempty [convex cone](../../../../../../convex-cone.md) closed under positive scaling: $\nu_0=(1+\|A_1\|)^{-1}$ supplies one element and guarantees weighted [integrability](../../../../../../integrability.md) even when $A_1$ itself has no first moment. Crucially, $\mathcal K$ is relatively open in $L$; it need not be closed.

To prove openness at a point $z=\mathbb E[\nu A_1]$, put $Z=\nu A_1$. The vectors $\mathbb E[hZ]$, for bounded real [measurable](../../../../../../measurability.md) $h$, span $L$. Indeed, a vector orthogonal to all of them would satisfy $\mathbb E[h\,u^\top Z]=0$ for every such $h$, forcing $u^\top Z=0$ [almost surely](../../../../../../almost-sure-convergence.md). Since $\nu>0$, this says $u\in L^\perp$. Choose finitely many bounded $h_j$ for which $\mathbb E[h_jZ]$ form a basis of $L$. For coefficients $t_j$ sufficiently small,

$$
\nu\left(1+\sum_jt_jh_j\right)>0,\qquad z+\sum_jt_j\mathbb E[h_jZ]\in\mathcal K.
$$

This gives a relative neighbourhood of $z$. It also proves the openness step behind the [strictly positive barycentre cone lemma](../../../../../../strictly-positive-barycentre-cone-lemma.md) without assuming a closed moment cone.

If $A_0\notin L$, the second [arbitrage](../../../../../../arbitrage.md) form was already constructed. If $A_0\in L\setminus\mathcal K$, the [separation of a point and an open convex set](../../../../../../separation-of-a-point-and-an-open-convex-set.md), applied inside the finite-dimensional space $L$, gives a nonzero $x\in L$ with $x^\top A_0\leq\inf_{z\in\mathcal K}x^\top z$. Positive scaling in the cone forces

$$
x^\top A_0\leq0,\qquad x^\top z\geq0\quad(z\in\mathcal K).
$$

We claim $x^\top A_1\geq0$ [almost surely](../../../../../../almost-sure-convergence.md). Otherwise $E=\{x^\top A_1<0\}$ has positive [probability](../../../../../../probability.md), and the admissible positive weights $\nu_m=\nu_0(1+m\mathbf1_E)$ give

$$
x^\top\mathbb E[\nu_m A_1]=\mathbb E[\nu_0x^\top A_1]+m\mathbb E[\nu_0x^\top A_1\mathbf1_E]\longrightarrow-\infty,
$$

contradicting the separation inequality. Since $x\in L$ is nonzero, $x^\top A_1$ cannot vanish [almost surely](../../../../../../almost-sure-convergence.md); thus it is strictly positive on an [event](../../../../../../event.md) of positive [probability](../../../../../../probability.md). This is the first [arbitrage](../../../../../../arbitrage.md) form.

Consequently absence of both forms forces $A_0\in\mathcal K$, which supplies the required $\nu$. Conversely either form excludes every such density by part (a). We have proved **exactly one of arbitrage or a strictly positive pricing density holds**. If $L=\{0\}$, the same argument reduces to the elementary cases $A_0=0$ and $A_0\ne0$, so no nondegeneracy assumption has been hidden.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
