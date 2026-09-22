<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the displayed square's notation $f:A\to B$, $h:A\to C$, $g:B\to D$, $k:C\to D$, with $gf=kh$ and $g$ epic. Form the [biproduct](../../../../../../biproduct.md) and the morphisms

$$
q=[g,-k]:B\oplus C\to D,\qquad j=\binom f h:A\to B\oplus C.
$$

The map $q$ is an [epimorphism](../../../../../../epimorphism.md), since its restriction to $B$ is $g$: equality after $q$ implies equality after $g$. The [pullback in a category](../../../../../../pullback-category-theory.md) property says exactly that $j$ is a [categorical kernel](../../../../../../kernel-in-a-category.md) of $q$. Indeed $qj=gf-kh=0$, and a map into $B\oplus C$ killed by $q$ is a pair $(x,y)$ with $gx=ky$, which factors uniquely through $(f,h)$.

Use the standard [abelian category](../../../../../../abelian-category.md) property that every [epimorphism](../../../../../../epimorphism.md) is the [categorical cokernel](../../../../../../cokernel-in-a-category.md) of its [categorical kernel](../../../../../../kernel-in-a-category.md). If $u:B\to X$ and $v:C\to X$ satisfy $uf=vh$, then $[u,-v]j=0$. Hence there is a unique $w:D\to X$ with $wq=[u,-v]$. Restriction to the two summands gives $wg=u$ and $wk=v$. This is the [pushout in a category](../../../../../../pushout-in-a-category.md) universal property. Thus **a [pullback of an epimorphism is a pushout in an abelian category](../../../../../../pullback-of-an-epimorphism-is-a-pushout-in-an-abelian-category.md)**.

In this pushout, $g$ is the pushout of $h$ along $f$. The reflection result of part (b) therefore makes $h$ epic. This proves [pullback stability of epimorphisms in an abelian category](../../../../../../pullback-stability-of-epimorphisms-in-an-abelian-category.md).

Finally, let $e:E\to B$ be an [epimorphism](../../../../../../epimorphism.md) and let $p_1,p_2:R\rightrightarrows E$ be its [kernel pair](../../../../../../kernel-pair.md). Their pullback square is a pushout by the result just proved. If $u:E\to X$ satisfies $up_1=up_2$, the two copies of $u$ form a pushout cocone. There is a unique $v:B\to X$ with $ve=u$. Hence **[epimorphisms in an abelian category are coequalizers of their kernel pairs](../../../../../../epimorphisms-in-an-abelian-category-are-coequalizers-of-their-kernel-pairs.md)**, so they are [regular epimorphisms](../../../../../../regular-epimorphism.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
