<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [Grothendieck topos](../../../../../../grothendieck-topos.md) define

$$
\Delta S=\coprod_{s\in S}1,\qquad
\Gamma A=\operatorname{Hom}_{\mathcal E}(1,A).
$$

The [coproduct](../../../../../../coproduct.md) universal property gives $\operatorname{Hom}_{\mathcal E}(\Delta S,A)\cong\operatorname{Set}(S,\Gamma A)$, naturally. Thus $\Delta\dashv\Gamma$. On any sheaf presentation, $\Delta$ is the composite of the constant-presheaf [functor](../../../../../../functor.md) with [sheafification](../../../../../../sheafification.md). The former preserves [finite limits](../../../../../../finite-limit.md) pointwise, and the latter is left exact, so $\Delta$ preserves [finite limits](../../../../../../finite-limit.md). Therefore these [functors](../../../../../../functor.md) define a [geometric morphism](../../../../../../geometric-morphism.md) $\gamma:\mathcal E\to\mathbf{Set}$.

For uniqueness, let $v$ be any such [geometric morphism](../../../../../../geometric-morphism.md). Its inverse image is a [left adjoint](../../../../../../adjoint-functors.md) and preserves the [terminal object](../../../../../../terminal-object.md). Every set has the canonical [coproduct](../../../../../../coproduct.md) decomposition $S=\coprod_{s\in S}\{*\}$, so

$$
v^*S\cong\coprod_{s\in S}v^*\{*\}
\cong\coprod_{s\in S}1=\Delta S.
$$

These isomorphisms respect all functions between sets, giving a [natural isomorphism](../../../../../../natural-isomorphism.md) $v^*\cong\Delta$. The [right adjoint](../../../../../../adjoint-functors.md) is then unique up to the corresponding [natural isomorphism](../../../../../../natural-isomorphism.md), so $v_*\cong\Gamma$. **There is a unique [geometric morphism](../../../../../../geometric-morphism.md) to sets, up to isomorphism**, called the [global sections geometric morphism](../../../../../../global-sections-geometric-morphism.md). This also applies to the degenerate topos.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
