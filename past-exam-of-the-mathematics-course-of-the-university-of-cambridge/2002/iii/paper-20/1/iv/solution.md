<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We first justify the relevant [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md) criterion. A componentwise [surjective function](../../../../../../surjective-function.md) gives an [epimorphism](../../../../../../epimorphism.md), because equality of two composites can be cancelled at each component. Conversely, for a [natural transformation](../../../../../../natural-transformation.md) $t:X\to Y$, form the pointwise [pushout](../../../../../../pushout.md) $P=Y\amalg_XY$. Restrictions of $Y$ preserve the identifications imposed by $t$, so these pointwise [sets](../../../../../../set-split.md) and restrictions form a [categorical presheaf](../../../../../../presheaf-category-theory.md). The two inclusions $j_1,j_2:Y\to P$ satisfy $j_1t=j_2t$. If $t$ is epic, $j_1=j_2$. At an object $U$, an element outside the image of $t_U$ would retain two distinct copies in $P(U)$, contradicting this equality. Thus every $t_U$ is surjective.

Apply this criterion to $H_\bullet(f)$ at $B$. Surjectivity of $\mathcal C(B,A)\to\mathcal C(B,B)$ supplies $g:B\to A$ with $fg=1_B$. Conversely, if $fg=1_B$, then $H_\bullet(f)H_\bullet(g)=1_{H_B}$, making $H_\bullet(f)$ a [split epimorphism](../../../../../../split-epimorphism.md) and hence an [epimorphism](../../../../../../epimorphism.md). Therefore

$$
\boxed{H_\bullet(f)\text{ epic}\iff f\text{ split epic}.}
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
