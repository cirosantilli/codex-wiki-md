<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $u_{C,x}:C\to R$ be a [colimit](../../../../../../../colimit.md) cocone for $G:\operatorname{Elts}(X)\to\mathcal C$. Here the preservation hypothesis must include the [categorical limit](../../../../../../../categorical-limit.md) of $G^{\mathrm{op}}$ in $\mathcal C^{\mathrm{op}}$; this indexing [category](../../../../../../../category-split.md) can be large. For a [morphism](../../../../../../../morphism.md) $f:(C,x)\to(D,y)$ of the [category of elements](../../../../../../../category-of-elements.md), the defining equation $X(f)(y)=x$ says that the family of distinguished elements $(x)_{(C,x)}$ is compatible. Preservation gives a unique $r\in X(R)$ with

$$
X(u_{C,x})(r)=x\quad\text{for every }(C,x).
$$

In particular each $u_{C,x}$ is now a [morphism](../../../../../../../morphism.md) $(C,x)\to(R,r)$ in the [category of elements](../../../../../../../category-of-elements.md). Naturality of the [colimit](../../../../../../../colimit.md) cocone gives

$$
u_{R,r}\,u_{C,x}=u_{C,x}.
$$

The [universal property](../../../../../../../universal-property.md) of the [colimit](../../../../../../../colimit.md) forces $u_{R,r}=1_R$, since it and $1_R$ agree after every cocone leg. If $f:C\to R$ also satisfies $X(f)(r)=x$, it is a [morphism](../../../../../../../morphism.md) $(C,x)\to(R,r)$, and cocone compatibility now yields $u_{C,x}=u_{R,r}f=f$. Thus $(R,r)$ is a [universal element](../../../../../../../universal-element-of-a-set-valued-functor.md). By the preceding representability criterion, **the presheaf is represented by the colimit object**:

$$
\boxed{\mathcal C(-,R)\cong X,\qquad f\longmapsto X(f)(r).}
$$

The size qualification matters. If preservation means only small [categorical limits](../../../../../../../categorical-limit.md), the implication as printed is false for general [locally small categories](../../../../../../../locally-small-category.md). For an explicit counterexample, let $\mathcal C$ be the ordered [category](../../../../../../../category-split.md) of all [ordinals](../../../../../../../ordinal.md) with an extra greatest object $\infty$. Put $X(\alpha)=\{*\}$ for every [ordinal](../../../../../../../ordinal.md) $\alpha$ and $X(\infty)=\varnothing$, with the forced restriction maps. Every small [colimit](../../../../../../../colimit.md) in $\mathcal C$ is the supremum of its object values: it is an [ordinal](../../../../../../../ordinal.md) unless the diagram contains $\infty$. Applying $X$ therefore gives the appropriate small [categorical limit](../../../../../../../categorical-limit.md) of singletons, or the empty [set](../../../../../../../set-split.md) when a value is empty; an empty diagram gives $X(0)=\{*\}$. Hence $X$ preserves all small [categorical limits](../../../../../../../categorical-limit.md).

Its [category of elements](../../../../../../../category-of-elements.md) consists of all [ordinals](../../../../../../../ordinal.md), whose projection has the large [colimit](../../../../../../../colimit.md) $\infty$ in $\mathcal C$. Nevertheless, no [ordinal](../../../../../../../ordinal.md) represents $X$, because its representable vanishes on larger ordinals; $\infty$ does not represent it either, since $\mathcal C(\infty,\infty)$ is nonempty while $X(\infty)$ is empty. The valid proof consequently uses preservation of the displayed possibly large limit, or a smallness hypothesis making that diagram small.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 22](../../../../paper-22-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
