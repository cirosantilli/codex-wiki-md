<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $X\subseteq A$, define

$$
\exists_p(X)=p[X],\qquad \forall_p(X)=\{b\in B:p^{-1}\{b\}\subseteq X\}=B\setminus p[A\setminus X].
$$

Both are monotone maps $PA\to PB$. For $Y\subseteq B$,

$$
p[X]\subseteq Y\quad\Longleftrightarrow\quad X\subseteq p^{-1}[Y],
$$

so [direct image](../../../../../../direct-image-sheaf.md) is a [left adjoint](../../../../../../adjoint-functors.md) to inverse image. Also,

$$
p^{-1}[Y]\subseteq X\quad\Longleftrightarrow\quad Y\subseteq\{b:p^{-1}\{b\}\subseteq X\},
$$

so the fiberwise universal condition gives the [right adjoint](../../../../../../adjoint-functors.md). Therefore

$$
\boxed{\exists_p\dashv p^*\dashv\forall_p.}
$$

An empty fiber satisfies the universal condition vacuously, so every point outside $p[A]$ belongs to $\forall_p(X)$, regardless of $X$. This is essential when $p$ is not surjective.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
