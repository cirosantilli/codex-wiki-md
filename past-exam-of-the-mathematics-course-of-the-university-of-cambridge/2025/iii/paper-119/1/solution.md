<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Yoneda lemma](../../../../../yoneda-lemma.md) states that for $A\in\mathcal C$ and $P:\mathcal C\to\mathbf{Set}$ there is a natural bijection

$$
\operatorname{Nat}(\mathcal C(A,-),P)\cong P(A),
\qquad \alpha\longmapsto\alpha_A(1_A).
$$

If $P\twoheadrightarrow Q$ is an epimorphism in the [functor category](../../../../../functor-category.md), it is pointwise surjective, so $P(A)\to Q(A)$ is surjective. Yoneda identifies this map with

$$
[\mathcal C,\mathbf{Set}](\mathcal C(A,-),P)
\longrightarrow
[\mathcal C,\mathbf{Set}](\mathcal C(A,-),Q).
$$

Thus every [representable functor](../../../../../representable-functor.md) is a [projective object in a category](../../../../../projective-object.md).

The colimit form of the [Special adjoint functor theorem](../../../../../special-adjoint-functor-theorem.md) says that a colimit-preserving functor from a locally small, cocomplete, well-copowered category with a small generating family into a locally small category has a right [adjoint functor](../../../../../adjoint-functors.md). For small $\mathcal C$, the category $[\mathcal C,\mathbf{Set}]$ is locally small and has colimits pointwise. Quotients of $P$ are represented by compatible equivalence relations on the sets $P(C)$, so they form a set; hence the category is well-copowered. The set of representables $\{\mathcal C(C,-):C\in\mathcal C\}$ generates it by the [Yoneda lemma](../../../../../yoneda-lemma.md). The theorem therefore gives a right adjoint to every small-colimit-preserving functor

$$
[\mathcal C,\mathbf{Set}]\longrightarrow[\mathcal D,\mathbf{Set}].
$$

In particular, product with a fixed functor $P$ is computed pointwise, and $-\times P(C)$ preserves colimits in the [Category of sets](../../../../../category-of-sets.md). Hence $-\times P$ preserves all small colimits and has a right adjoint $(-)^P$. Thus $[\mathcal C,\mathbf{Set}]$ is a [Cartesian closed category](../../../../../cartesian-closed-category.md).

Now work in $[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ and write $yA=\mathcal C(-,A)$. If $\mathcal C$ has binary products, then

$$
(P^{yA})(C)
\cong\operatorname{Nat}(yC\times yA,P)
\cong\operatorname{Nat}(y(C\times A),P)
\cong P(C\times A).
$$

Thus exponentiation by $yA$ is precomposition with $-\times A$. Precomposition between functor categories has a right adjoint given by [Right Kan extension](../../../../../right-kan-extension.md), so $yA$ is a [tiny object](../../../../../tiny-object.md).

Conversely, suppose $\mathcal C$ has a [terminal object](../../../../../terminal-object.md) $1$ and $F$ is tiny. The representable $y1$ is the terminal presheaf, and the exponential adjunction plus Yoneda gives

$$
[\mathcal C^{\mathrm{op}},\mathbf{Set}](F,P)
\cong(P^F)(1).
$$

Since $F$ is tiny, $(-)^F$ is a left adjoint and preserves all colimits; evaluation at $1$ also preserves pointwise colimits. Therefore the hom functor $[\mathcal C^{\mathrm{op}},\mathbf{Set}](F,-)$ preserves coproducts and epimorphisms. Preservation of epimorphisms makes $F$ projective, while preservation of coproducts makes it indecomposable.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
