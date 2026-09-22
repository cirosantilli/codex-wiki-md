<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [group automorphism](../../../../../../group-automorphism.md) preserves element orders and sizes of [conjugacy classes](../../../../../../conjugacy-class.md). A nonidentity involution in $S_n$ has [cycle type](../../../../../../cycle-type.md) $2^k1^{n-2k}$ and class size

$$
\frac{n!}{2^kk!(n-2k)!},\qquad 1\leq k\leq\lfloor n/2\rfloor.
$$

For its class to have the same size as the [transposition](../../../../../../transposition-permutation.md) class, it must satisfy

$$
\frac{(n-2)!}{(n-2k)!}=2^{k-1}k!.
$$

For fixed $k\geq2$ the left side grows strictly with $n$. When $k=2$, it is $(n-2)(n-3)$, which is two at $n=4$ and at least six at $n=5$, never the required four. For $k=3$ equality first occurs at $n=6$, since $4!=2^2\cdot3!$, and thereafter the left side is larger. For $k\geq4$ it is already larger at $n=2k$: the ratio $(2k-2)!/[2^{k-1}k!]$ is $15/4$ at $k=4$, and increases with $k$, its successive ratio being $k(2k-1)/(k+1)>1$. This proves the [symmetric-group involution class-size collision](../../../../../../symmetric-group-involution-class-size-collision.md) result. Therefore, for $n\ne6$, every [group automorphism](../../../../../../group-automorphism.md) maps [transpositions](../../../../../../transposition-permutation.md) to [transpositions](../../../../../../transposition-permutation.md).

Now recover the underlying points from [transpositions](../../../../../../transposition-permutation.md). Two distinct [transpositions](../../../../../../transposition-permutation.md) fail to commute exactly when their two-element supports meet. A maximal family of pairwise intersecting edges of a [complete graph](../../../../../../complete-graph.md) is either a vertex star or a triangle. Indeed, after selecting edges $\{1,2\}$ and $\{1,3\}$, every edge either contains 1 or is $\{2,3\}$; if the latter occurs, all edges lie in that triangle. For $n\geq5$, the stars have size $n-1\geq4$ and triangles size three, so stars are recognized purely by the multiplication structure of $S_n$.

An [group automorphism](../../../../../../group-automorphism.md) must thus permute the stars, giving a [permutation](../../../../../../permutation.md) $\tau$ of the points. The unique [transposition](../../../../../../transposition-permutation.md) shared by stars $i,j$ is $(i\ j)$, so its image is $(\tau(i)\ \tau(j))$. Since [transpositions](../../../../../../transposition-permutation.md) generate $S_n$, the whole [group automorphism](../../../../../../group-automorphism.md) is conjugation by $\tau$.

At $n=4$, stars and triangles both have three elements, but their generated [subgroups](../../../../../../subgroup.md) distinguish them: the [transpositions](../../../../../../transposition-permutation.md) in a star generate all of $S_4$ (since $(i\ j)=(a\ i)(a\ j)(a\ i)$ for its center $a$), while a triangle generates the $S_3$ fixing the fourth point. The same reconstruction follows. At $n=3$, conjugation by $S_3$ induces every [permutation](../../../../../../permutation.md) of its three [transpositions](../../../../../../transposition-permutation.md) (a [transposition](../../../../../../transposition-permutation.md) swaps the other two, and a three-cycle rotates all three), so a transposition-preserving [group automorphism](../../../../../../group-automorphism.md) is again inner. At $n=2$ the only [group automorphism](../../../../../../group-automorphism.md) of $C_2$ is the identity, and $n=0,1$ are trivial (if the empty-set degree is included). Thus

$$
\boxed{\operatorname{Out}(S_n)=1\quad\text{for }n\ne6.}
$$

The small-degree adjustments are necessary: a cardinality-only star argument would not cover $n=4$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
