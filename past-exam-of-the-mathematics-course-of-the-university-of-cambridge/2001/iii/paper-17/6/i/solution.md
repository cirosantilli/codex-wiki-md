<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$, let $\int X$ be its [category of elements](../../../../../../category-of-elements.md). Its objects are $(A,a)$ with $a\in X(A)$; an arrow $(A,a)\to(B,b)$ is a [morphism](../../../../../../morphism.md) $f:A\to B$ satisfying $X(f)b=a$. This is a [small category](../../../../../../small-category.md), because $\mathcal C$ is small and all values of $X$ are [sets](../../../../../../set-split.md).

Send $(A,a)$ to the [representable presheaf](../../../../../../representable-functor.md) $h_A$, and send an arrow $f$ to postcomposition $h_f$. There is a [cocone](../../../../../../cocone-under-a-diagram.md) to $X$ whose map at $(A,a)$ is

$$
\iota_{A,a}:h_A\to X,\qquad
(\iota_{A,a})_C(g)=X(g)a.
$$

The [functor](../../../../../../functor.md) laws give its [naturality](../../../../../../naturality.md) and the required [cocone](../../../../../../cocone-under-a-diagram.md) compatibility.

Compute the [colimit](../../../../../../colimit.md) pointwise as a disjoint union modulo its diagram identifications. At $C$ a representative is a triple $(A,a,g:C\to A)$, and it maps to $X(g)a\in X(C)$. Every $x\in X(C)$ is the image of $(C,x,1_C)$. Moreover $g$ is an arrow $(C,X(g)a)\to(A,a)$ in $\int X$, so its diagram relation identifies

$$
(A,a,g)\sim(C,X(g)a,1_C).
$$

Thus every representative is identified with the canonical representative of its image. Two representatives have equal images exactly when their canonical representatives agree. This proves a componentwise [bijection](../../../../../../bijection.md); restriction maps respect it. The resulting [natural isomorphism](../../../../../../natural-isomorphism.md) is the [canonical colimit presentation of a presheaf](../../../../../../canonical-colimit-presentation-of-a-presheaf.md):

$$
\boxed{X\cong\operatorname{colim}_{(A,a)\in\int X}h_A.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
