<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [pointed category](../../../../../../pointed-category.md), a [zero object](../../../../../../zero-object.md) defines zero morphisms between all objects. A [categorical cokernel](../../../../../../cokernel-in-a-category.md) of $f:A\to B$ is a map $g:B\to C$ with $gf=0$ such that every $u:B\to X$ with $uf=0$ factors uniquely as $u=\bar u g$. Equivalently it is the [coequalizer](../../../../../../coequalizer.md) of $f$ and the zero map, so $g$ is an [epimorphism](../../../../../../epimorphism.md).

Write $a:A\to A'$, $b:B\to B'$, and $c:C\to C'$ for the vertical arrows, with $g'=\operatorname{coker}f'$ and $cg=g'b$. The left [pushout in a category](../../../../../../pushout-in-a-category.md) applied to the compatible pair $g:B\to C$ and $0:A'\to C$ gives $h:B'\to C$ satisfying $hb=g$ and $hf'=0$. The [categorical cokernel](../../../../../../cokernel-in-a-category.md) property of $g'$ then gives $d:C'\to C$ with $dg'=h$.

Now $dcg=dg'b=hb=g$. Cancel the [epimorphism](../../../../../../epimorphism.md) $g$ to obtain $dc=1_C$. To prove the other identity, the two arrows $cdg',g':B'\to C'$ agree after $b$, because $cdg'b=cg=g'b$, and after $f'$, because both composites are zero. The [pushout in a category](../../../../../../pushout-in-a-category.md) uniqueness clause gives $cdg'=g'$. Cancelling the [epimorphism](../../../../../../epimorphism.md) $g'$ gives $cd=1_{C'}$.

Thus **$c$ is an isomorphism**: [cokernel invariance under pushout](../../../../../../cokernel-invariance-under-pushout.md) holds already in pointed categories with the indicated cokernels.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
