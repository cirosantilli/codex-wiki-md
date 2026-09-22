<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $X\cong\mathcal C(-,R)$. As a [functor](../../../../../../../functor.md) on the [opposite category](../../../../../../../opposite-category.md), a [representable presheaf](../../../../../../../representable-functor.md) preserves every existing [categorical limit](../../../../../../../categorical-limit.md): a [colimit](../../../../../../../colimit.md) in $\mathcal C$ is defined by the [bijection](../../../../../../../bijection.md) between [morphisms](../../../../../../../morphism.md) from its vertex into $R$ and compatible families of [morphisms](../../../../../../../morphism.md) from its diagram objects into $R$. This remains valid for a possibly large [diagram in a category](../../../../../../../diagram-category-theory.md) whenever that [colimit](../../../../../../../colimit.md) exists and the compatible-family collection is the corresponding [set](../../../../../../../set-split.md).

The [category of elements](../../../../../../../category-of-elements.md) has a [terminal object](../../../../../../../terminal-object.md) $(R,r)$, where $r$ is the image of $1_R$ under the representation. For each $(C,x)$ let $u_{C,x}:C\to R$ be its unique [morphism](../../../../../../../morphism.md) to $(R,r)$. These form a [cocone](../../../../../../../cocone-under-a-diagram.md) for the [forgetful functor](../../../../../../../forgetful-functor.md) $G$. Any competing [cocone](../../../../../../../cocone-under-a-diagram.md) $v_{C,x}:C\to A$ satisfies

$$
v_{C,x}=v_{R,r}\,u_{C,x}.
$$

The component at $(R,r)$ uniquely determines the mediating [morphism](../../../../../../../morphism.md). Thus **the representing object is the colimit of the elements projection**:

$$
\boxed{\operatorname{colim}_{(C,x)\in\operatorname{Elts}(X)}C\cong R.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
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
