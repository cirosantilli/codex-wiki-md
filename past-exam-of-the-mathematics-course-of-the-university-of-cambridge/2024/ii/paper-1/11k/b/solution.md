<h1 id="11k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose $\delta$ with

$$
p<\delta<\frac14.
$$

A greedy packing construction gives binary length-$n$ codes of minimum distance greater than $2\delta n$ and size at least

$$
\frac{2^n}{\sum_{j\leq2\delta n}\binom nj}.
$$

Their asymptotic rate is at least

$$
1-h_2(2\delta)>0,
$$

where $h_2$ is binary [Binary entropy](../../../../../../binary-entropy.md). Minimum-distance decoding corrects every error pattern of weight at most $\delta n$. Since a channel error count is $\operatorname{Bin}(n,p)$, the law of large numbers gives

$$
\mathbb P\{\operatorname{Bin}(n,p)>\delta n\}\longrightarrow0.
$$

**Thus a fixed positive rate is achievable with error tending to zero, proving that the operational capacity is nonzero. This is the [positive-rate coding bound below one-quarter crossover](../../../../../../positive-rate-coding-bound-below-one-quarter-crossover.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11K](../../11k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
