<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

For $n\ge2$ with $n\ne6$, bijectivity of $\phi$ and the previous part imply

$$
\frac{n!}{2^k k!(n-2k)!}=|T_k|=|T_1|=\frac{n(n-1)}2.
$$

The supplied numerical fact forces $k=1$. Thus $\phi$ permutes the [transpositions](../../../../../../../transposition-permutation.md).

Suppose $n\ge3$, and write $s_r=\phi((1r))$ for $r=2,\ldots,n$. These are distinct [transpositions](../../../../../../../transposition-permutation.md). For $r\ne t$, the product $(1r)(1t)$ has [order of a group element](../../../../../../../order-of-a-group-element.md) three, so $s_rs_t$ also has order three. Two distinct [transpositions](../../../../../../../transposition-permutation.md) have this property precisely when their two-element sets of moved points meet in one point: disjoint ones have a product of order two, whereas ones sharing one point have a three-cycle as product. The two-element [support of a permutation](../../../../../../../support-of-a-permutation.md) associated with each $s_r$ therefore meets that of every other $s_t$.

We now show that they have a common point. Choose two; the [support of a permutation](../../../../../../../support-of-a-permutation.md) is $\{a,b\}$ for one and $\{a,c\}$ for the other, where $a,b,c$ are distinct. Any further two-element set meeting both either contains $a$ or is $\{b,c\}$. If $\{b,c\}$ occurs, any two-element set meeting all three must itself be one of $\{a,b\},\{a,c\},\{b,c\}$: a set containing $a$ must also contain $b$ or $c$, and a set omitting $a$ must contain both $b,c$. Hence a pairwise-intersecting family with no common point consists of exactly those three edges of a triangle.

For $n\ge5$, there are $n-1\ge4$ distinct $s_r$, ruling out that triangle. For $n=3$, the two sets already have a common point. For $n=4$, the triangle alternative would make all three $s_r$ fix the fourth point. They would then generate a proper [subgroup](../../../../../../../subgroup.md) of $S_4$, contrary to surjectivity of $\phi$ and part (a)(iv), which imply that the $s_r$ generate $S_4$. Thus in every case $n\ge3$ there is a common point $a$, and we may write

$$
s_r=(a\ b_r)\qquad(2\le r\le n).
$$

The $b_r$ are distinct and different from $a$, so they exhaust the remaining $n-1$ points. Define a [permutation](../../../../../../../permutation.md) $\sigma$ by

$$
\sigma(a)=1,\qquad \sigma(b_r)=r.
$$

Then

$$
\sigma^{-1}(1r)\sigma
=(\sigma^{-1}(1)\ \sigma^{-1}(r))
=(a\ b_r)=\phi((1r)).
$$

The two [group homomorphisms](../../../../../../../group-homomorphism.md) $\tau\mapsto\phi(\tau)$ and $\tau\mapsto\sigma^{-1}\tau\sigma$ agree on a [generating set of a group](../../../../../../../generating-set-of-a-group.md), so agree on every product of its elements, hence throughout $S_n$:

$$
\boxed{\phi(\tau)=\sigma^{-1}\tau\sigma\qquad(\tau\in S_n).}
$$

Finally, $S_1$ is trivial and $S_2$ has a unique nonidentity element, so every [automorphism](../../../../../../../automorphism.md) of either is the identity and we can take $\sigma=e$. This completes all degrees $n\ne6$ and proves that every such [automorphism](../../../../../../../automorphism.md) is an [inner automorphism](../../../../../../../inner-automorphism.md).

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [b](../../b.md)
3. [7](../../../7.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
