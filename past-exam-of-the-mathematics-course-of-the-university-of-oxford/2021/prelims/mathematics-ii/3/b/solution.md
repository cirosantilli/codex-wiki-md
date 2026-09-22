<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume first that the original nonnegative [series](../../../../../../series-mathematics.md) converges to $S$. Its [partial sums](../../../../../../partial-sum.md) $s_m$ increase to $S$. Write $t_N=\sum_{n=1}^{N}a_{g(n)}$ for the [partial sums](../../../../../../partial-sum.md) of the [rearrangement of a series](../../../../../../rearrangement-of-a-series.md). Since $g$ is an [injection](../../../../../../injective-function.md), the indices $g(1),\ldots,g(N)$ are distinct, so

$$
0\leq t_N\leq s_{\max\{g(1),\ldots,g(N)\}}\leq S.
$$

Thus $(t_N)$ is an increasing [bounded sequence](../../../../../../bounded-sequence.md), and the [bounded monotone sequence theorem](../../../../../../bounded-monotone-sequence-theorem.md) gives $t_N\to T\leq S$.

For any fixed $m$, [surjectivity](../../../../../../surjective-function.md) of $g$ gives

$$
N_m=\max\{g^{-1}(1),\ldots,g^{-1}(m)\}.
$$

For $N\geq N_m$, nonnegativity implies $t_N\geq s_m$. Taking [limits of sequences](../../../../../../limit-of-a-sequence.md) first in $N$ and then in $m$ gives $T\geq S$. Hence $T=S$.

Conversely, $g^{-1}$ is a [bijection](../../../../../../bijection.md), and the original [series](../../../../../../series-mathematics.md) is the [rearrangement of a series](../../../../../../rearrangement-of-a-series.md) of $\sum b_n$ defined by $g^{-1}$. The same argument proves its [convergence](../../../../../../convergence.md) whenever $\sum b_n$ converges. **Both [series](../../../../../../series-mathematics.md) converge together, and their sums are equal.**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
