<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If every [monomorphism](../../../../../../monomorphism.md) is strong, let $m:A\to B$ be both a [monomorphism](../../../../../../monomorphism.md) and an [epimorphism](../../../../../../epimorphism.md). Use $m$ as both vertical maps in the lifting square, with horizontal maps $1_A$ and $1_B$. The [strong monomorphism](../../../../../../strong-monomorphism.md) property gives $d:B\to A$ satisfying $dm=1_A$ and $md=1_B$. Thus $m$ is an [isomorphism](../../../../../../isomorphism.md), proving that the [category](../../../../../../category-split.md) is [balanced](../../../../../../balanced-category.md).

For the converse, take $e:X\to Y$ epic, $m:A\to B$ monic, and $mu=ve$. Form the [pullback in a category](../../../../../../pullback-category-theory.md) of $m$ along $v$:

$$
P=Y\times_B A,\qquad p:P\to Y,\quad q:P\to A,\quad mq=vp.
$$

The equality $mu=ve$ gives $t:X\to P$ with $pt=e$ and $qt=u$. By preservation of [monomorphisms](../../../../../../monomorphism.md) under [pullback in a category](../../../../../../pullback-category-theory.md), $p$ is monic. It is also epic: if $hp=kp$, then $he=hpt=kpt=ke$, and cancellation of $e$ gives $h=k$. The [balanced category](../../../../../../balanced-category.md) hypothesis therefore makes $p$ an [isomorphism](../../../../../../isomorphism.md).

Set $d=qp^{-1}$. Then $md=v$ and $de=qt=u$. Any other such lift agrees with $d$ after composing with the [monomorphism](../../../../../../monomorphism.md) $m$, so it is equal to $d$. Consequently **in a [category](../../../../../../category-split.md) with [pullbacks in a category](../../../../../../pullback-category-theory.md), being [balanced](../../../../../../balanced-category.md) is equivalent to every [monomorphism](../../../../../../monomorphism.md) being a [strong monomorphism](../../../../../../strong-monomorphism.md)**. This is the [balanced categories with pullbacks have strong monomorphisms](../../../../../../balanced-categories-with-pullbacks-have-strong-monomorphisms.md) principle; the proof does not assume pullback stability of epimorphisms.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
