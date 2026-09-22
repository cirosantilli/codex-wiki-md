<h1 id="27j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Z_t=\int_0^tX(s)\,ds$ and set $a=q+\lambda$. Starting from $-1$, the first holding time has [exponential distribution](../../../../../../exponential-distribution.md) of rate $a$. Its joint density with a jump to $+1$ is $qe^{-au}\,du$. Before such a jump $Z$ decreases to $-u$, so the remaining rise needed to exceed $c$ is $c+u$. If instead the jump is to the absorbing state zero, the level stays nonpositive and never exceeds $c>0$.

Conditioning on this first jump and using the [Strong Markov property](../../../../../../strong-markov-property.md) gives

$$
\boxed{\psi_-(c)=\int_0^\infty qe^{-(q+\lambda)u}\psi_+(c+u)\,du.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [27J](../../27j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
