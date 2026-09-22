<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [right-adjoint criterion using comma-category colimits](../../../../../../right-adjoint-criterion-using-comma-category-colimits.md) is as follows. Under the given colimit-preservation hypothesis, with preservation including the possibly large colimits below, $F:\mathcal X\to\mathcal A$ has a [right adjoint](../../../../../../adjoint-functors.md) exactly when, for every $A$, the projection

$$
U_A:(F\downarrow A)\to\mathcal X,\qquad (X,f:FX\to A)\longmapsto X
$$

has a [colimit](../../../../../../colimit.md) in $\mathcal X$. **The right adjoint is obtained from these comma-category colimits.** Thus the objects to construct are

$$
\boxed{GA=\operatorname{colim}_{(X,f)\in(F\downarrow A)}X.}
$$

For necessity, if $F\dashv G$ with [adjunction counit](../../../../../../counit-of-an-adjunction.md) $\varepsilon$, $(GA,\varepsilon_A)$ is a [terminal object](../../../../../../terminal-object.md) of the [comma category](../../../../../../comma-category.md) $(F\downarrow A)$. Its unique incoming [morphisms](../../../../../../morphism.md) give a [colimit](../../../../../../colimit.md) cocone for $U_A$, exactly as for the elements projection in the preceding part.

For sufficiency, choose such a [colimit](../../../../../../colimit.md) $L$ with legs $u_{X,f}:X\to L$. The [morphisms](../../../../../../morphism.md) $f:FX\to A$ are a [cocone](../../../../../../cocone-under-a-diagram.md) on $FU_A$. Since $F$ preserves this [colimit](../../../../../../colimit.md), there is a unique $\varepsilon_A:FL\to A$ satisfying

$$
\varepsilon_A F(u_{X,f})=f.
$$

Each $u_{X,f}$ is thus a [morphism](../../../../../../morphism.md) $(X,f)\to(L,\varepsilon_A)$ in the [comma category](../../../../../../comma-category.md). The original [colimit](../../../../../../colimit.md) cocone gives $u_{L,\varepsilon_A}u_{X,f}=u_{X,f}$ for every object, hence $u_{L,\varepsilon_A}=1_L$ by the [universal property](../../../../../../universal-property.md). For any other [morphism](../../../../../../morphism.md) $h:(X,f)\to(L,\varepsilon_A)$, cocone compatibility gives

$$
u_{X,f}=u_{L,\varepsilon_A}h=h.
$$

So $(L,\varepsilon_A)$ is a [terminal object](../../../../../../terminal-object.md). Equivalently, $L$ represents the [categorical presheaf](../../../../../../presheaf-category-theory.md) $\mathcal A(F-,A)$, via $h\mapsto\varepsilon_A Fh$. The [functoriality of chosen representations](../../../../../../functoriality-of-chosen-representations.md) makes these $L$ into $G:\mathcal A\to\mathcal X$, yielding a [natural bijection](../../../../../../natural-bijection.md)

$$
\boxed{\mathcal X(X,GA)\cong\mathcal A(FX,A),\qquad F\dashv G.}
$$

The preservation of these possibly large [colimits](../../../../../../colimit.md) is essential to the construction of $\varepsilon_A$. Under a small-only interpretation, the preceding [ordinal](../../../../../../ordinal.md) counterexample also disproves the unqualified converse here. Take $F=X^{\mathrm{op}}:\mathcal C\to\mathbf{Set}^{\mathrm{op}}$. It preserves all small [colimits](../../../../../../colimit.md). For a nonempty [set](../../../../../../set-split.md) $A$, the [comma category](../../../../../../comma-category.md) $(F\downarrow A)$ has one object over each [ordinal](../../../../../../ordinal.md) and none over $\infty$, so its projection has [colimit](../../../../../../colimit.md) $\infty$. For $A=\varnothing$, the projection is the identity of $\mathcal C$, again with [colimit](../../../../../../colimit.md) $\infty$. Thus all these projection colimits exist, but $F$ has no [right adjoint](../../../../../../adjoint-functors.md): the [categorical presheaf](../../../../../../presheaf-category-theory.md) $\mathbf{Set}^{\mathrm{op}}(F-,\{*\})=X$ is not [representable](../../../../../../representable-functor.md). This makes the large-preservation qualification substantive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
