<h1 id="10f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $q=1-p$ and track the difference $S_n$ between the numbers of wins. It is a [biased random walk](../../../../../../biased-random-walk.md) with increments $+1$ and $-1$, stopped on first reaching $3$ or $-3$.

To finish at $+3$ on game five, there must be four wins for $A$ and one for $B$, with the final game won by $A$. The unique loss for $A$ can be in position one, two or three. If it were in position four or five, the first three games would already have stopped the contest. Each of the three allowed paths remains strictly inside the barriers until the last step and has [probability](../../../../../../probability.md) $p^4q$. By interchanging players, there are also three paths ending at $-3$, each with [probability](../../../../../../probability.md) $pq^4$. Therefore

$$
\boxed{\mathbb P(N=5)=3p^4q+3pq^4=3pq(p^3+q^3).}
$$

For a fair game this is $3/16$. Counting all five-game sequences with final win difference three would overcount paths on which the contest ended earlier.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
