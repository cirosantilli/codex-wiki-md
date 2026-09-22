<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $A$, and let $S(B)=B\amalg A$ be the [functor](../../../../../../functor.md) obtained from the chosen binary [coproduct in a category](../../../../../../coproduct.md) construction. Its arrow map is $S(v)=v\amalg1_A$. For $h_A=\mathcal C(A,-)$, the binary coproduct property gives $h_B\times h_A\cong h_{B\amalg A}$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) and part (i) therefore give, naturally in $B,F$,

$$
(F^{h_A})(B)=\operatorname{Nat}(h_B\times h_A,F)
\cong\operatorname{Nat}(h_{B\amalg A},F)
\cong F(B\amalg A).
$$

Thus exponentiation by $h_A$ is precomposition $S^*:F\mapsto F\circ S$.

This precomposition has a [right adjoint](../../../../../../adjoint-functors.md) given by [Right Kan extension](../../../../../../right-kan-extension.md). Explicitly, for $K:\mathcal C\to\mathbf{Set}$ put

$$
(RK)(B)=\lim_{(C,u:B\to SC)\in(B\downarrow S)}K(C).
$$

The [comma category](../../../../../../comma-category.md) is small, so this [categorical limit](../../../../../../categorical-limit.md) exists in the [Category of sets](../../../../../../category-of-sets.md). A map $v:B\to B'$ gives $(RK)(v)$ by taking a compatible family indexed by $u:B\to SC$ and selecting its entries at $u'v$ for the indices $u':B'\to SC$.

A [natural transformation](../../../../../../natural-transformation.md) $\alpha:F\circ S\to K$ determines $F\to RK$ by sending $x\in F(B)$ to the family $\alpha_C(F(u)x)$ indexed by $(C,u)$. Conversely, a map $F\to RK$ determines $F(SC)\to K(C)$ by projecting to the index $(C,1_{SC})$. Naturality and the limit's compatibility relations make these constructions inverse. Hence $S^*\dashv R$, proving the [tiny covariant representable functor on a category with binary coproducts](../../../../../../tiny-covariant-representable-functor-on-a-category-with-binary-coproducts.md) result:

$$
\boxed{\mathcal C(A,-)\text{ is tiny}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
