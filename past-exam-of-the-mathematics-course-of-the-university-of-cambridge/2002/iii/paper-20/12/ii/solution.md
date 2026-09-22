<h1 id="12/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Category of sets](../../../../../../category-of-sets.md), take the [monoidal tensor product](../../../../../../monoidal-tensor-product.md) to be the [Cartesian product](../../../../../../cartesian-product.md), $A\otimes B=A\times B$, with unit a singleton $1$. On [morphisms](../../../../../../morphism.md) use $(f\times g)(a,b)=(f(a),g(b))$. Define the [associator](../../../../../../associator.md) by $((a,b),c)\mapsto(a,(b,c))$ and the [unitors](../../../../../../unitor.md) by $(*,a)\mapsto a$ and $(a,*)\mapsto a$. These are [natural isomorphisms](../../../../../../natural-isomorphism.md), with inverses obtained by rebracketing or adjoining $*$. Both paths in the pentagon send $(((a,b),c),d)$ to $(a,(b,(c,d)))$, and both paths in the triangle send $((a,*),b)$ to $(a,b)$. This proves the axioms elementwise.

There is a second structure: use [disjoint union](../../../../../../disjoint-union.md) $A\amalg B$ and unit $\varnothing$. Define the [associator](../../../../../../associator.md) by preserving each element and its summand while changing the nested tags, and define the [unitors](../../../../../../unitor.md) by removing the empty summand. These are natural and invertible. In the pentagon, either path takes an element in any of the four summands to that same element in the same summand of $A\amalg(B\amalg(C\amalg D))$; the triangle removes an empty intermediate summand on either path. Thus both axioms hold.

These [product and coproduct monoidal structures on sets](../../../../../../product-and-coproduct-monoidal-structures-on-sets.md) have different units, $1$ and $\varnothing$, which are not isomorphic. They are even inequivalent as [monoidal categories](../../../../../../monoidal-category.md): an equivalence of the underlying [Category of sets](../../../../../../category-of-sets.md) preserves [terminal objects](../../../../../../terminal-object.md), so it cannot take the singleton unit of the product structure to the empty unit of the coproduct structure. Hence **the monoidal structure on [sets](../../../../../../set-split.md) is not unique**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12](../../12.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
