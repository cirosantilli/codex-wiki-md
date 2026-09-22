<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use letters $x_i$ and their formal inverses. An elementary contraction deletes an adjacent pair $x_ix_i^{-1}$ or $x_i^{-1}x_i$. A [reduced word](../../../../reduced-word-in-a-free-group.md) has no such pair. Repeated contraction terminates because each step reduces length by two, so every word has a reduced descendant.

For uniqueness, two possible first contractions either occur on disjoint pairs, when performing both yields a common descendant, or overlap in three letters $aa^{-1}a$, when either contraction produces the same remaining letter. Induct on word length: the shorter descendants of both first contractions therefore have the same eventual [reduced word](../../../../reduced-word-in-a-free-group.md). This proves every contraction sequence from a given word ends at the same [reduced word](../../../../reduced-word-in-a-free-group.md). An insertion or deletion of an inverse pair preserves that reduced result. Since the word model of the [free group](../../../../free-group.md) identifies words exactly under finite sequences of these moves, every [group](../../../../group-split.md) element has **a unique reduced representative**.

To define the requested [homomorphism](../../../../homomorphism.md), substitute $w_i$ for $x_i$ and $w_i^{-1}$ for $x_i^{-1}$ in any word. Inverse-pair insertions or deletions map to inverse words that cancel, so substitution is well defined on [group](../../../../group-split.md) elements and respects concatenation. This proves the universal property of the [free group](../../../../free-group.md) in this case.

For an [automorphism](../../../../automorphism.md) of order four, take $\phi(x_1)=x_2$ and $\phi(x_2)=x_1^{-1}$. Its iterates on $x_1$ are $x_2,x_1^{-1},x_2^{-1},x_1$; its fourth iterate also fixes $x_2$. Unique reduced representatives show the first three iterates on $x_1$ differ from $x_1$. Hence **its order is exactly four**.

For the final map, every iterate of $x_2$ is a positive word and contains an $x_2$. Substituting once replaces each occurrence of $x_2$ by $x_2w$ and leaves each $x_1$ unchanged. If $\ell=|w|\ge1$, its length consequently increases by at least $\ell$ on every iteration. No cancellation occurs in a positive word, so $|\phi^n(x_2)|\ge1+n\ell>1$. It cannot equal $x_2$, proving **no positive iterate of this [endomorphism](../../../../endomorphism.md) is the identity**. Surjectivity of this last [endomorphism](../../../../endomorphism.md) is not assumed.

This uses [positive-word growth under a free-group endomorphism](../../../../positive-word-growth-under-a-free-group-endomorphism.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../split.md)
5. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
