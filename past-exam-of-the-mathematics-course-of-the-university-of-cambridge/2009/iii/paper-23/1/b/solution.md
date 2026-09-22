<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $1$ be a [terminal object](../../../../../../terminal-object.md). The [pullback](../../../../../../pullback-category-theory.md) of the unique arrows $A\to1\leftarrow B$ is a binary [categorical product](../../../../../../product-category-theory.md): maps $X\to A$ and $X\to B$ automatically have equal composites into $1$, so the [pullback](../../../../../../pullback-category-theory.md) [universal property](../../../../../../universal-property.md) is exactly the [categorical product](../../../../../../product-category-theory.md) [universal property](../../../../../../universal-property.md).

For parallel arrows $f,g:A\rightrightarrows B$, form $B\times B$ and take the [pullback](../../../../../../pullback-category-theory.md) of $\langle f,g\rangle:A\to B\times B$ along the diagonal $\delta:B\to B\times B$. Write the resulting projections as $e:E\to A$ and $b:E\to B$. The [pullback](../../../../../../pullback-category-theory.md) equation gives

$$
fe=b=ge.
$$

If $u:X\to A$ satisfies $fu=gu$, the pair $(u,fu)$ is a [pullback](../../../../../../pullback-category-theory.md) cone, producing a unique $v:X\to E$ with $ev=u$ and $bv=fu$. The second condition is forced by the first, since $b=fe$. Thus $e$ is the [equaliser](../../../../../../equaliser.md) of $f,g$.

The [terminal object](../../../../../../terminal-object.md) and iterated binary [categorical products](../../../../../../product-category-theory.md) give all finite [categorical products](../../../../../../product-category-theory.md), including the nullary one. Part (a) therefore proves **[pullbacks](../../../../../../pullback-category-theory.md) and a [terminal object](../../../../../../terminal-object.md) give all finite [categorical limits](../../../../../../categorical-limit.md)**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
