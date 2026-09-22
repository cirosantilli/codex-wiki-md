<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $h_A=\mathcal C(A,-)$. The covariant [Yoneda lemma](../../../../../../yoneda-lemma.md) gives the natural bijection

$$
\operatorname{Nat}(h_A,F)\cong F(A),\qquad\alpha\longmapsto\alpha_A(1_A),
$$

whose inverse sends $x\in F(A)$ to the [natural transformation](../../../../../../natural-transformation.md) with component $u:A\to B\mapsto F(u)(x)$. This also identifies the two variables' naturality.

To prove that $h_A$ is a [projective object in a category](../../../../../../projective-object.md), let $p:G\twoheadrightarrow F$ be an [epimorphism](../../../../../../epimorphism.md) in the [functor category](../../../../../../functor-category.md) and $\alpha:h_A\to F$. By [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md), lift $\alpha_A(1_A)$ through the [surjective function](../../../../../../surjective-function.md) $p_A$. The [Yoneda lemma](../../../../../../yoneda-lemma.md) turns this lift into $\beta:h_A\to G$ with $p\beta=\alpha$.

For a [small category](../../../../../../small-category.md), the set of pairs $(A,x)$ with $x\in F(A)$ indexes the canonical map

$$
p:\coprod_{(A,x)}h_A\longrightarrow F,\qquad
p_B(A,x,u)=F(u)(x).
$$

It is natural, and every $y\in F(B)$ is the image of $(B,y,1_B)$. Thus it is an [epimorphism](../../../../../../epimorphism.md), establishing the [projective cover of a set-valued functor by representables](../../../../../../projective-cover-of-a-set-valued-functor-by-representables.md) construction. Here cover means a projective presentation; no minimality is asserted.

For the equivalence's first step, if $f:B\to D$ is a [monomorphism](../../../../../../monomorphism.md), then $h_A(f)$, the map $u\mapsto fu$, is injective for every $A$. Hence every [representable functor](../../../../../../representable-functor.md) is a [monofunctor](../../../../../../monofunctor.md). Conversely, injectivity of every $h_A(f)$ is exactly left cancellation against every $u,v:A\to B$, so it implies that $f$ is a [monomorphism](../../../../../../monomorphism.md). Therefore

$$
\boxed{\text{(a)}\Longleftrightarrow\text{(b)},\qquad
\coprod_{(A,x)}h_A\twoheadrightarrow F.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
