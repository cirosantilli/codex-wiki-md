<h1 id="5d/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

**No such [finite group](../../../../../../finite-group.md) exists.** [Cayley theorem](../../../../../../cayley-s-theorem.md) embeds every [finite group](../../../../../../finite-group.md) $G$ of order $n$ into $S_n$: the left-regular [group action](../../../../../../group-action.md) sends $g$ to the [permutation](../../../../../../permutation.md) $x\mapsto gx$, and this is faithful because the image of the identity element is $g$.

To make every image permutation even, let $t=(n+1\ n+2)$, with support disjoint from the first $n$ letters. For $\sigma\in S_n$, let $e(\sigma)=0$ for an [even permutation](../../../../../../even-permutation.md) and $e(\sigma)=1$ for an [odd permutation](../../../../../../odd-permutation.md), and set

$$
\iota(\sigma)=\sigma t^{e(\sigma)}.
$$

The [sign homomorphism](../../../../../../sign-homomorphism.md) gives $e(\sigma\tau)\equiv e(\sigma)+e(\tau)\pmod2$, and $t$ commutes with all permutations of the first $n$ letters. Thus $\iota$ is a [group homomorphism](../../../../../../group-homomorphism.md). It is injective by restriction to those letters, and its sign is $(-1)^{e(\sigma)}(-1)^{e(\sigma)}=1$. Consequently

$$
\boxed{G\hookrightarrow S_n\hookrightarrow A_{n+2}.}
$$

This is the [alternating-group embedding of a finite group](../../../../../../alternating-group-embedding-of-a-finite-group.md).

## ↑ Ancestors (11)

1. [V](../v.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
