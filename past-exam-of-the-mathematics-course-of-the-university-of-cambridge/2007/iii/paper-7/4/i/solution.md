<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First determine when a [group automorphism](../../../../../../group-automorphism.md) can carry a [transposition](../../../../../../transposition-permutation.md) to another type of [involution](../../../../../../involution.md). An [involution](../../../../../../involution.md) in $S_n$ is a product of $k$ disjoint [transpositions](../../../../../../transposition-permutation.md), and its [conjugacy class](../../../../../../conjugacy-class.md) has size

$$
\frac{n!}{2^k k!(n-2k)!}.
$$

An automorphism preserves element orders and conjugacy-class sizes. Equality with the transposition-class size $n(n-1)/2$ requires

$$
\frac{(n-2)!}{(n-2k)!}=2^{k-1}k!.
$$

For $k=2$ this says $(n-2)(n-3)=4$, which has no integral solution $n\ge4$. For $k=3$, the minimum value of the left side, at $n=6$, is $4!=24=2^2\cdot3!$; it increases strictly for larger $n$. For $k\ge4$, even its minimum $(2k-2)!$ exceeds $2^{k-1}k!$: at $k=4$ this is $720>192$, and the ratio of these two quantities increases at the next step by $(2k)(2k-1)/(2(k+1))>1$. Thus only in degree six can the [transposition](../../../../../../transposition-permutation.md) class be exchanged with a different [involution](../../../../../../involution.md) class, namely the triple [transpositions](../../../../../../transposition-permutation.md).

We next prove that any automorphism preserving [transpositions](../../../../../../transposition-permutation.md) is an [inner automorphism](../../../../../../inner-automorphism.md). Regard a [transposition](../../../../../../transposition-permutation.md) as an edge of the [complete graph](../../../../../../complete-graph.md) on the $n$ letters. Two distinct [transpositions](../../../../../../transposition-permutation.md) fail to commute exactly when their edges meet. Any family of pairwise intersecting edges is contained in a vertex star or a triangle: after choosing $\{a,b\}$ and $\{a,c\}$, an edge not containing $a$ must be $\{b,c\}$, which precludes any fourth edge. For $n\ge5$, the stars are therefore distinguished as the maximal such families of size $n-1\ge4$. An automorphism permutes stars, inducing a permutation $\pi$ of the letters; their pairwise intersections show that $(i\ j)$ is sent to $(\pi(i)\ \pi(j))$. Since [transpositions](../../../../../../transposition-permutation.md) generate $S_n$, this is conjugation by a permutation.

For $n=4$, stars and triangles both have three edges, but a star generates $S_4$ while a triangle generates a subgroup $S_3$. An automorphism preserves the order of the generated subgroup and hence still distinguishes stars. For $n=3$, every permutation of the three [transpositions](../../../../../../transposition-permutation.md) is induced by conjugation in $S_3$, since its conjugation action on them is faithful and has order six. The groups $S_1,S_2$ have trivial automorphism groups. This completes the small cases.

It follows that all automorphisms for $n\ne6$ are inner. In degree six, an automorphism permutes the two [involution](../../../../../../involution.md) classes of size 15; the kernel of this action consists precisely of the inner automorphisms. Therefore the [automorphisms of the symmetric group](../../../../../../automorphisms-of-the-symmetric-group.md) satisfy

$$
\boxed{\operatorname{Out}(S_n)=1\ (n\ne6),\qquad |\operatorname{Out}(S_6)|\le2.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
