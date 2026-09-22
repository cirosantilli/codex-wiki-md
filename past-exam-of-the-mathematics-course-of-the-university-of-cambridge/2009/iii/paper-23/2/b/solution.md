<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write an object of the [slice category](../../../../../../slice-category.md) $\mathcal D/X$ as $a:A\to X$. Its [morphisms](../../../../../../morphism.md) are arrows in $\mathcal D$ commuting with these structure maps, and the [forgetful functor](../../../../../../forgetful-functor.md) $U_X$ removes the structure map.

Suppose a square in the slice becomes a [pullback](../../../../../../pullback-category-theory.md) square in $\mathcal D$, with vertex $p:P\to X$. Given a compatible pair of slice arrows $u:Z\to A$ and $v:Z\to B$, the underlying [pullback](../../../../../../pullback-category-theory.md) gives a unique $h:Z\to P$ with the required projection equations. If $r:P\to A$ is one projection, then

$$
ph=arh=au=z,
$$

where $z:Z\to X$ is the structure map. Thus $h$ is automatically a slice [morphism](../../../../../../morphism.md), and underlying uniqueness gives uniqueness in the slice. Hence **$U_X$ reflects [pullbacks](../../../../../../pullback-category-theory.md)**.

Now let $e:(E,c)\to(A,a)$ be an [equaliser](../../../../../../equaliser.md) of slice arrows $f,g:(A,a)\rightrightarrows(B,b)$. Consider any underlying arrow $u:Z\to A$ with $fu=gu$. Give $Z$ the structure map $au:Z\to X$. Then $u$ is a slice arrow into $(A,a)$, and the slice [equaliser](../../../../../../equaliser.md) gives a unique $h:Z\to E$ with $eh=u$. Conversely any underlying $h$ with that equation automatically obeys $ch=aeh=au$, so there are no additional factorization possibilities outside the slice. Therefore $U_Xe$ has the ordinary [equaliser](../../../../../../equaliser.md) [universal property](../../../../../../universal-property.md) in $\mathcal D$. This proves **$U_X$ preserves [equalisers](../../../../../../equaliser.md)**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
