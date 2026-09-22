<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Use the [least-upper-bound property](../../../../../least-upper-bound-property.md) as the least upper bound axiom: every nonempty [set](../../../../../set-split.md) of [real numbers](../../../../../real-number.md) bounded above has a least upper bound in $\mathbb R$. It implies convergence of a bounded increasing [sequence](../../../../../sequence.md): if $L$ is the [supremum](../../../../../supremum.md) of its terms, then for every $\varepsilon>0$ some term exceeds $L-\varepsilon$, and all subsequent terms lie between that term and $L$. A bounded decreasing [sequence](../../../../../sequence.md) converges by applying this argument to its negative.

The [alternating series test](../../../../../alternating-series-test.md) states that if $b_n\ge0$, $b_{n+1}\le b_n$, and $b_n\to0$, then $\sum_{n\ge1}(-1)^{n-1}b_n$ converges. To prove it, let $S_N$ denote its [partial sums](../../../../../partial-sum.md). The even [partial sums](../../../../../partial-sum.md) are increasing because $S_{2m+2}-S_{2m}=b_{2m+1}-b_{2m+2}\ge0$. The odd [partial sums](../../../../../partial-sum.md) are decreasing because $S_{2m+3}-S_{2m+1}=-b_{2m+2}+b_{2m+3}\le0$. Moreover,

$$
0\le S_{2m}\le S_{2m+1}\le b_1.
$$

[Completeness of the real numbers](../../../../../completeness-of-the-real-numbers.md) therefore gives a [limit of a sequence](../../../../../limit-of-a-sequence.md) for each subsequence, denoted $L_e,L_o$ respectively for the even and odd [subsequences](../../../../../subsequence.md). Their difference is $S_{2m+1}-S_{2m}=b_{2m+1}\to0$, so $L_e=L_o$. Every sufficiently late [partial sum](../../../../../partial-sum.md) belongs to one of these two [subsequences](../../../../../subsequence.md), proving convergence of the full [sequence](../../../../../sequence.md) of [partial sums](../../../../../partial-sum.md). Multiplying the terms by $-1$ leaves convergence unchanged.

## ↑ Ancestors (11)

1. [9C](../9c.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ia](../../split.md)
5. [2002](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
