<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [category of elements](../../../../../../category-of-elements.md) of $X$ has objects $(W,x)$ with $x\in X(W)$ and morphisms $f:(W,x)\to(V,y)$ satisfying $X(f)y=x$. Send $(W,x)$ to the [representable presheaf](../../../../../../representable-functor.md) $H_W$ and a morphism to $H_f$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a canonical cocone to $X$, whose leg at $(W,x)$ corresponds to $x$.

For any target presheaf $Z$, a cocone from this diagram to $Z$ is a family of maps $H_W\to Z$, or equivalently elements $z_{W,x}\in Z(W)$, with $z_{W,x}=Z(f)z_{V,y}$ whenever $X(f)y=x$. Such a family is exactly a [natural transformation](../../../../../../natural-transformation.md) $X\to Z$, via $x\mapsto z_{W,x}$. This bijection respects the canonical cocone, so it proves its [colimit](../../../../../../colimit.md) universal property. Consequently the [canonical colimit presentation of a presheaf](../../../../../../canonical-colimit-presentation-of-a-presheaf.md) is

$$
\boxed{X\cong\operatorname*{colim}_{(W,x)\in\int X}H_W.}
$$

Equivalently, the density coend identifies the disjoint copies of the representables by exactly these element-category arrows. Smallness of $\mathcal C$ and the set-valued fibers make the indexing category small.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
