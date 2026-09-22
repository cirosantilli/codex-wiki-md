<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A [binary block code](../../../../../binary-block-code.md) is a subset $C\subseteq\{0,1\}^n$; its length is the common word length $n$, its size is $m=|C|$, and its [minimum distance](../../../../../minimum-distance-of-a-code.md) is the least [Hamming distance](../../../../../hamming-distance.md) between distinct words. There are $V(n,r)=\sum_{j=0}^r\binom nj$ words in a radius-$r$ [Hamming ball](../../../../../hamming-ball.md), since one chooses the positions to change.

Put $t=\lfloor(d-1)/2\rfloor$. Two radius-$t$ [Hamming balls](../../../../../hamming-ball.md) about different codewords cannot meet: otherwise the [triangle inequality](../../../../../triangle-inequality.md) would make their centres at distance at most $2t<d$. Comparing their combined size with $2^n$ gives the [Hamming bound](../../../../../hamming-bound.md)

$$
A(n,d)V(n,t)\le2^n.
$$

For the other direction, start with one word and repeatedly add any word at distance at least $d$ from every word already selected. Finiteness ensures that this process stops. At that point the radius-$(d-1)$ [Hamming balls](../../../../../hamming-ball.md) cover the entire cube; an uncovered word could otherwise be added. These balls may overlap, but their total size is at least $2^n$. This gives the [Gilbert–Varshamov bound](../../../../../gilbert-varshamov-bound.md)

$$
\boxed{\frac{2^n}{V(n,d-1)}\le A(n,d)\le\frac{2^n}{V(n,\lfloor(d-1)/2\rfloor)}.}
$$

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
