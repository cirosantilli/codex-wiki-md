<h1 id="17f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Colour every vertex independently red or blue with probability $1/2$. Fix a vertex $v$ and enumerate infinitely many distinct neighbours $w_1,w_2,\ldots$. The probability that all neighbours after $w_n$ are red is

$$
\lim_{m\to\infty}2^{-(m-n)}=0.
$$

Taking the countable union over $n$, the probability that $v$ has only finitely many blue neighbours is zero. The same argument with the colours exchanged shows that the probability of only finitely many red neighbours is zero.

The vertex set is countable, so the union of these two null events over all vertices still has probability zero. Thus with probability one every vertex has infinitely many neighbours of each colour. Taking $A$ and $B$ to be the two colour classes gives an unfriendly partition. This is the [random unfriendly partition of a countable infinite-degree graph](../../../../../../random-unfriendly-partition-of-a-countable-infinite-degree-graph.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17F](../../17f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
