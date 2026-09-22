<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [duad](../../../../../../duad.md) is an unordered pair of letters, a [syntheme](../../../../../../syntheme.md) is a partition of the six letters into three [duads](../../../../../../duad.md), and a [total of synthemes](../../../../../../total-of-synthemes.md) is a set of five [synthemes](../../../../../../syntheme.md) partitioning the 15 [duads](../../../../../../duad.md). There are $6!/(2^3\cdot3!)=15$ [synthemes](../../../../../../syntheme.md). Fix one, $M$. Each of its three [duads](../../../../../../duad.md) lies in three [synthemes](../../../../../../syntheme.md), and two distinct [duads](../../../../../../duad.md) of $M$ can occur together only in $M$ itself. Thus precisely $1+3\cdot2=7$ [synthemes](../../../../../../syntheme.md) meet $M$ in a [duad](../../../../../../duad.md), leaving eight disjoint from it.

For any [syntheme](../../../../../../syntheme.md) $M'$ disjoint from $M$, their union as edges in $K_6$ is a six-cycle: the two [perfect matchings](../../../../../../perfect-matching.md) alternate, and no two-cycle is possible in a simple graph. Its complement is a triangular prism, namely two triangles joined by three corresponding edges. The prism has four [perfect matchings](../../../../../../perfect-matching.md). One consists of all three joining edges; each of the other three consists of one joining edge and the remaining edge in each triangle. To partition the prism into three [perfect matchings](../../../../../../perfect-matching.md), one cannot use the all-joining matching, since what remains is two odd triangles. The other three do partition it. Hence **two disjoint [synthemes](../../../../../../syntheme.md) extend to a unique [synthematic total](../../../../../../total-of-synthemes.md)**.

There are eight choices for $M'$ and four choices of $M'$ within each [synthematic total](../../../../../../total-of-synthemes.md) containing $M$. Thus $M$ lies in exactly two [synthematic totals](../../../../../../total-of-synthemes.md). Counting incidences of [synthemes](../../../../../../syntheme.md) and [synthematic totals](../../../../../../total-of-synthemes.md) now gives the [counting synthematic totals](../../../../../../counting-synthematic-totals.md) formula

$$
\boxed{\#\{\text{totals}\}=\frac{15\cdot2}{5}=6.}
$$

Two distinct [synthematic totals](../../../../../../total-of-synthemes.md) share at most one [syntheme](../../../../../../syntheme.md), since sharing two would force them to be the unique [synthematic total](../../../../../../total-of-synthemes.md) extending that pair. Each [syntheme](../../../../../../syntheme.md) gives a pair of [synthematic totals](../../../../../../total-of-synthemes.md) containing it, and the 15 [synthemes](../../../../../../syntheme.md) account for all $\binom62=15$ pairs. Therefore every pair of [synthematic totals](../../../../../../total-of-synthemes.md) shares exactly one [syntheme](../../../../../../syntheme.md).

This also explains why the action on the six [synthematic totals](../../../../../../total-of-synthemes.md) defines an automorphism of $S_6$. A permutation fixing all [synthematic totals](../../../../../../total-of-synthemes.md) fixes their pairwise intersections, hence every [syntheme](../../../../../../syntheme.md). Each [duad](../../../../../../duad.md) is the intersection of two distinct [synthemes](../../../../../../syntheme.md) containing it, so every [duad](../../../../../../duad.md) is then fixed. Intersecting two [duads](../../../../../../duad.md) through a point shows that every point is fixed. The action is faithful and, by equality of orders, maps $S_6$ onto the full symmetric group of the [synthematic totals](../../../../../../total-of-synthemes.md). Part iii shows that a [transposition](../../../../../../transposition-permutation.md) acts as a triple [transposition](../../../../../../transposition-permutation.md), establishing that this is an [outer automorphism](../../../../../../outer-automorphism-of-a-group.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
