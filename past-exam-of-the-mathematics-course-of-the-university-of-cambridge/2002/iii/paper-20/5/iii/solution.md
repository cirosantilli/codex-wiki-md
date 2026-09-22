<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [category of elements](../../../../../../category-of-elements.md) $\int X$ has objects $(W,x)$ for $x\in X(W)$, and [morphisms](../../../../../../morphism.md) $f:(W,x)\to(V,y)$ with $X(f)y=x$. Send $(W,x)$ to the [representable presheaf](../../../../../../representable-functor.md) $H_W$, and a [morphism](../../../../../../morphism.md) $f$ to $H_\bullet(f)$. The element $x$ supplies a [natural transformation](../../../../../../natural-transformation.md) $H_W\to X$ with component $h\mapsto X(h)x$, by the [Yoneda lemma](../../../../../../yoneda-lemma.md). These transformations form a [cocone](../../../../../../cocone-under-a-diagram.md).

Pointwise at $U$, the [colimit](../../../../../../colimit.md) of this [diagram in a category](../../../../../../diagram-category-theory.md) has representatives $(W,x,h:U\to W)$, with relation $(W,X(f)y,h)\sim(V,y,fh)$. These are exactly the relations of the preceding [categorical coend](../../../../../../coend-of-a-functor.md). Its proved [natural isomorphism](../../../../../../natural-isomorphism.md) with $X(U)$ therefore identifies the [cocone](../../../../../../cocone-under-a-diagram.md) with the universal [colimit](../../../../../../colimit.md) [cocone](../../../../../../cocone-under-a-diagram.md). More directly, every representative equals $(U,X(h)x,1_U)$ through the [morphism](../../../../../../morphism.md) $h:(U,X(h)x)\to(W,x)$; two representatives with the same image therefore agree. As $\mathcal C$ is small, $\int X$ is small, so this is an ordinary small [colimit](../../../../../../colimit.md). Consequently

$$
\boxed{X\cong\operatorname{colim}_{(W,x)\in\int X}H_W.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
