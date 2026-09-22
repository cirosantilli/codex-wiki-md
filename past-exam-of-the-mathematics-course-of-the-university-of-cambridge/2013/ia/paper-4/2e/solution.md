<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

A real [sequence](../../../../../sequence.md) converges to a finite limit $L$ if

$$
\forall\varepsilon>0\ \exists N\ \forall n\geq N:\quad |x_n-L|<\varepsilon.
$$

A [series](../../../../../series-mathematics.md) converges when its [partial sums](../../../../../partial-sum.md) $s_N=\sum_{n=1}^N x_n$ form a [convergent sequence](../../../../../convergent-sequence.md) with a finite limit. These are different conditions: a [series](../../../../../series-mathematics.md) concerns accumulated terms, whereas [sequence](../../../../../sequence.md) convergence concerns the terms themselves.

If $s_N\to S$, then $s_{N-1}\to S$ as well and $x_N=s_N-s_{N-1}\to0$. Explicitly, choose $N$ large enough that both [partial sums](../../../../../partial-sum.md) lie within $\varepsilon/2$ of $S$; the [triangle inequality](../../../../../triangle-inequality.md) gives $|x_N|<\varepsilon$. Hence **convergence of a series forces its terms to tend to zero**.

For the converse, take $x_n=1/n$. This is a [null sequence](../../../../../null-sequence.md), but its [harmonic series](../../../../../harmonic-series.md) diverges. In each block $2^{j-1}<n\leq2^j$, there are $2^{j-1}$ terms each at least $2^{-j}$, so the block contributes at least $1/2$. Thus

$$
s_{2^k}\geq1+\frac k2\longrightarrow\infty.
$$

**A zero limit for the terms is necessary, but not sufficient, for [convergent series](../../../../../convergent-series.md).**

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
