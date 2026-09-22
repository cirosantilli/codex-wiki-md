<h1 id="5d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [alternating group](../../../../../../alternating-group.md) is the [subgroup](../../../../../../subgroup.md) of the [symmetric group](../../../../../../symmetric-group.md) consisting of [even permutations](../../../../../../even-permutation.md):

$$
A_n=\ker(\operatorname{sgn}:S_n\to\{1,-1\}).
$$

For a [permutation cycle](../../../../../../permutation-cycle.md) of length $l$,

$$
(a_1\ a_2\ \cdots\ a_l)=(a_1\ a_l)(a_1\ a_{l-1})\cdots(a_1\ a_2),
$$

using rightmost-first composition. Its [sign of a permutation](../../../../../../sign-of-a-permutation.md) is therefore $(-1)^{l-1}$. Multiplicativity of the [sign homomorphism](../../../../../../sign-homomorphism.md) gives

$$
\operatorname{sgn}(g)=(-1)^{\sum_j(l_j-1)}.
$$

Thus

$$
\boxed{g\in A_n\iff\text{the number of even-length cycles is even}.}
$$

Equivalently, $n-t$ is even when $t$ counts all cycles, including fixed points. Odd-length cycles contribute positive sign and impose no further restriction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
