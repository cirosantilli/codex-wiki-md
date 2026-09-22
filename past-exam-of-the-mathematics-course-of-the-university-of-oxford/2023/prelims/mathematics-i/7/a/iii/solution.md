<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

For $0\le k\le\lfloor n/2\rfloor$, first select an ordered list of $2k$ distinct entries. There are $n!/(n-2k)!$ lists. Pair consecutive entries to obtain

$$
(a_1a_2)(a_3a_4)\cdots(a_{2k-1}a_{2k}).
$$

Each product of $k$ disjoint [transpositions](../../../../../../../transposition-permutation.md) is counted $2^k k!$ times: each pair has two orientations, and the $k$ pairs can be ordered in $k!$ ways. There is no other duplication, by uniqueness of the [disjoint cycle decomposition](../../../../../../../disjoint-cycle-decomposition.md). Therefore

$$
\boxed{|T_k|=\frac{n!}{2^k k!(n-2k)!}.}
$$

If $2k>n$, there are no such [permutations](../../../../../../../permutation.md). For $k=0$, $T_0=\{e\}$.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [a](../../a.md)
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
