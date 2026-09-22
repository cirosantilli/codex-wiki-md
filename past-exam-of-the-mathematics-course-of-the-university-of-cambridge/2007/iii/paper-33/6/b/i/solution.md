<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At level $n$, the $N_n$ dyadic cells fully contained in $J$ are disjoint. Their occupied indicators are independent by the preceding part, and every cell has length $2^{-n}$, so each has success [probability](../../../../../../../probability.md)

$$
p_n=\mathbb P(M(D_k^n)>0)=1-e^{-2^{-n}}.
$$

Their sum therefore satisfies

$$
\boxed{M_n(J)\sim\operatorname{Binomial}(N_n,1-e^{-2^{-n}}).}
$$

If there are no fully contained cells, $N_n=0$ and this means the deterministic zero count. The binomial law follows directly from [independence](../../../../../../../independent-random-variables.md) of occupation indicators, without assuming that the full counts $M(D_k^n)$ are already Poisson.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
