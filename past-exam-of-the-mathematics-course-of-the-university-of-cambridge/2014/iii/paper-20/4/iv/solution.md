<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The canonical [geometric morphism](../../../../../../geometric-morphism.md) $\widehat{\mathcal C}\to\mathbf{Set}$ has inverse image the constant-presheaf functor $\Delta$ and direct image the [global sections functor](../../../../../../global-sections-functor.md)

$$
\Gamma(P)=\operatorname{Hom}(1,P),\qquad\Delta\dashv\Gamma.
$$

If the [presheaf topos](../../../../../../presheaf-topos.md) is a [local topos](../../../../../../local-topos.md), $\Gamma$ is also the inverse image of a [geometric morphism](../../../../../../geometric-morphism.md) $g:\mathbf{Set}\to\widehat{\mathcal C}$. This morphism has an extra [left adjoint](../../../../../../adjoint-functors.md) $\Delta$. Apply part (iii) with source category $1$ and target category $\mathcal C$, using its idempotent-splitting hypothesis. Then $g$ is induced by a functor $1\to\mathcal C$, choosing an object $C_0$, and $\Gamma$ is naturally evaluation at $C_0$.

Since evaluation at $C_0$ is $\operatorname{Hom}(yC_0,-)$, this says $\operatorname{Hom}(1,-)\cong\operatorname{Hom}(yC_0,-)$. Uniqueness of representing objects gives $yC_0\cong1$. Thus $\mathcal C(C,C_0)$ is a singleton for every $C$: $C_0$ is terminal.

Conversely, if $C_0$ is terminal, $yC_0=1$ and $\Gamma(P)=P(C_0)$. Evaluation at that object preserves [finite limits](../../../../../../finite-limit.md) and has a right Kan extension as [right adjoint](../../../../../../adjoint-functors.md), so is an inverse image functor. Therefore, under the permitted idempotent-completeness assumption,

$$
\boxed{\widehat{\mathcal C}\text{ is local if and only if }\mathcal C\text{ has a terminal object}.}
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Section B](../../section-b.md)
4. [Paper 20](../../../paper-20-split.md)
5. [Iii](../../../split.md)
6. [2014](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
