<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [Lie derivative of a differential form](../../../../../../lie-derivative-of-a-differential-form.md) by $\mathcal L_X\alpha=(d/dt)_{t=0}\phi_t^*\alpha$, using the [local flow](../../../../../../local-flow.md). The [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) respects the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) and commutes with the [exterior derivative](../../../../../../exterior-derivative.md). Therefore $\mathcal L_X$ is a [derivation of an algebra](../../../../../../derivation-of-an-algebra.md) of degree zero and commutes with $d$.

Let $D_X=\iota_Xd+d\iota_X$, where $\iota_X$ is the [interior product of a differential form](../../../../../../interior-product.md). The graded product rules for $d$ and $\iota_X$ show that their anticommutator $D_X$ is also a degree-zero [derivation of an algebra](../../../../../../derivation-of-an-algebra.md): the two mixed terms cancel. Since $d^2=0$, it commutes with $d$. On a function $f$, $\iota_Xf=0$ and $D_Xf=\iota_Xdf=Xf=\mathcal L_Xf$. Hence $D_X(df)=d(Xf)=\mathcal L_X(df)$.

In a [manifold chart](../../../../../../manifold-chart.md), every [differential form](../../../../../../differential-form-split.md) is a sum of functions times products $dx^{i_1}\wedge\cdots\wedge dx^{i_p}$. The two derivations agree on its generators $f$ and $dx^i$, and therefore agree on every such form. This proves [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md), including the case $p=0$:

$$
\boxed{\mathcal L_X\alpha=\iota_Xd\alpha+d(\iota_X\alpha).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
