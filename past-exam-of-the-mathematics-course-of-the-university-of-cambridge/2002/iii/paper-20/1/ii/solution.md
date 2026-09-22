<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the [Yoneda embedding](../../../../../../yoneda-embedding.md) $H_\bullet:\mathcal C\to[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ by $H_A(U)=\mathcal C(U,A)$ and $H_A(k)(h)=hk$. For $f:A\to B$, define $H_\bullet(f)_U(h)=fh$. Associativity proves [naturality](../../../../../../naturality.md) in $U$, and preservation of [identity morphisms](../../../../../../identity-morphism.md) and [composition in a category](../../../../../../composition-in-a-category.md) proves that $H_\bullet$ is a [functor](../../../../../../functor.md).

Apply the [Yoneda lemma](../../../../../../yoneda-lemma.md) to $X=H_B$. It gives

$$
\boxed{\operatorname{Nat}(H_A,H_B)\cong\mathcal C(A,B).}
$$

The [natural transformation](../../../../../../natural-transformation.md) corresponding to $f$ has component $h\mapsto fh$, exactly $H_\bullet(f)$. Therefore the induced map on every [hom-set](../../../../../../hom-set.md) is a [bijection](../../../../../../bijection.md): **the Yoneda embedding is [full and faithful](../../../../../../full-and-faithful-functor.md)**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
