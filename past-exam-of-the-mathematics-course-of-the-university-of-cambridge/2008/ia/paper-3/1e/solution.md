<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

For a [permutation](../../../../../permutation.md) $\sigma\in S_n$, let $P_\sigma$ be its [permutation matrix](../../../../../permutation-matrix.md), defined by $P_\sigma e_j=e_{\sigma(j)}$. Define the [signature of a permutation](../../../../../sign-of-a-permutation.md) by $\epsilon(\sigma)=\det P_\sigma$. A [permutation matrix](../../../../../permutation-matrix.md) is orthogonal, so $(\det P_\sigma)^2=1$ and its [permutation sign](../../../../../sign-of-a-permutation.md) lies in $\{1,-1\}$. A [transposition](../../../../../transposition-permutation.md) exchanges two columns of the identity and therefore has [determinant](../../../../../determinant.md) $-1$. Every [permutation](../../../../../permutation.md) is a product of [transpositions](../../../../../transposition-permutation.md), by decomposing each [permutation cycle](../../../../../permutation-cycle.md) as

$$
(a_1\,a_2\,\ldots,a_r)=(a_1\,a_r)(a_1\,a_{r-1})\cdots(a_1\,a_2).
$$

Hence $\epsilon(\sigma)=(-1)^m$ for any expression as $m$ [transpositions](../../../../../transposition-permutation.md); the [determinant](../../../../../determinant.md) definition proves that this [parity of a permutation](../../../../../parity-of-a-permutation.md) is independent of the expression. Equivalently the [permutation sign](../../../../../sign-of-a-permutation.md) is positive for an [even permutation](../../../../../even-permutation.md) and negative for an [odd permutation](../../../../../odd-permutation.md).

Composition is taken rightmost first. Since $P_{\sigma\tau}e_j=e_{\sigma(\tau(j))}=P_\sigma P_\tau e_j$, we have $P_{\sigma\tau}=P_\sigma P_\tau$. Multiplicativity of the [determinant](../../../../../determinant.md) therefore proves the [sign homomorphism](../../../../../sign-homomorphism.md) identity

$$
\boxed{\epsilon(\sigma\tau)=\epsilon(\sigma)\epsilon(\tau).}
$$

The [alternating group](../../../../../alternating-group.md) consists of the [even permutations](../../../../../even-permutation.md):

$$
\boxed{A_n=\{\sigma\in S_n:\epsilon(\sigma)=1\}=\ker\epsilon.}
$$

It contains the identity. If $\sigma,\tau\in A_n$, their product has [permutation sign](../../../../../sign-of-a-permutation.md) $1$, and $\epsilon(\sigma^{-1})=\epsilon(\sigma)^{-1}=1$, so their inverses also belong to $A_n$. This proves it is a [subgroup](../../../../../subgroup.md). Finally, for every $g\in S_n$ and $a\in A_n$,

$$
\epsilon(gag^{-1})=\epsilon(g)\epsilon(a)\epsilon(g)^{-1}=1.
$$

Thus **$A_n$ is a [normal subgroup](../../../../../normal-subgroup.md) of $S_n$**. This also exhibits directly why a [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is normal.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
