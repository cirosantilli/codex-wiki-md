# Upper and lower peak convergence criterion

↑ **Parent:** [Peak of a sequence](peak-of-a-sequence.md)

Suppose $k_1<k_2<\cdots$ are [peaks of a sequence](peak-of-a-sequence.md) $(a_n)$ and $m_1<m_2<\cdots$ are [peaks of a sequence](peak-of-a-sequence.md) $(-a_n)$. Then $(a_n)$ converges precisely when these two [subsequences](subsequence.md) have a common finite [limit of a sequence](limit-of-a-sequence.md) $L$.

Necessity follows because every [subsequence](subsequence.md) inherits the [limit of a sequence](limit-of-a-sequence.md) of a [convergent sequence](convergent-sequence.md). For sufficiency, choose one selected value from each [subsequence](subsequence.md) within $\varepsilon$ of $L$. Every term after both selected indices lies between the two selected values:

$$
L-\varepsilon<a_{m_r}\leq a_n\leq a_{k_r}<L+\varepsilon\qquad(n>\max\{k_r,m_r\}).
$$

This is exactly $a_n\to L$.

## ↑ Ancestors (10)

1. [Peak of a sequence](peak-of-a-sequence.md)
2. [Monotone subsequence theorem](monotone-subsequence-theorem.md)
3. [Subsequence](subsequence.md)
4. [Sequence](sequence.md)
5. [Sequence and series](sequence-and-series-split.md)
6. [Real analysis](real-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
