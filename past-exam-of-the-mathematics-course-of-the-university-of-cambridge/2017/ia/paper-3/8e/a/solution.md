<h1 id="8e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With rightmost-first composition, a [permutation cycle](../../../../../../permutation-cycle.md) satisfies

$$
(a_1\ a_2\ \cdots\ a_m)
=(a_1\ a_m)(a_1\ a_{m-1})\cdots(a_1\ a_2).
$$

Tracing each $a_j$ verifies the equality, and every other letter is fixed. Thus every cycle is a product of [transpositions](../../../../../../transposition-permutation.md); decomposing a [permutation](../../../../../../permutation.md) into [disjoint permutation cycles](../../../../../../disjoint-permutation-cycles.md) proves that every element of $S_n$ is such a product. The identity is the empty product.

To establish that parity is well defined, use the [permutation matrix](../../../../../../permutation-matrix.md) $P_\sigma$ defined by $P_\sigma e_i=e_{\sigma(i)}$. Its [determinant](../../../../../../determinant.md) is $\pm1$, and $P_{\sigma\tau}=P_\sigma P_\tau$. A [transposition](../../../../../../transposition-permutation.md) swaps two columns of the [identity matrix](../../../../../../identity-matrix.md) and has [determinant](../../../../../../determinant.md) $-1$. Therefore if $\sigma$ is expressed as a product of $r$ [transpositions](../../../../../../transposition-permutation.md),

$$
\det P_\sigma=(-1)^r.
$$

The left side depends only on $\sigma$, so any two decompositions have the same parity. Define

$$
\boxed{\operatorname{sgn}(\sigma)=\det P_\sigma=(-1)^r.}
$$

Multiplicativity of the [determinant](../../../../../../determinant.md) makes this the [sign homomorphism](../../../../../../sign-homomorphism.md). Its [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is the [alternating group](../../../../../../alternating-group.md)

$$
\boxed{A_n=\{\sigma\in S_n:\operatorname{sgn}(\sigma)=1\}.}
$$

It is a [normal subgroup](../../../../../../normal-subgroup.md) consisting of the [even permutations](../../../../../../even-permutation.md). For $n\geq2$ the sign map is surjective because a [transposition](../../../../../../transposition-permutation.md) has sign $-1$, so $[S_n:A_n]=2$. For $n=1$ both [groups](../../../../../../group-split.md) are trivial.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8E](../../8e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
