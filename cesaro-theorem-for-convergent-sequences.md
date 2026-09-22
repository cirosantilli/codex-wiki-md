<h1 id="cesaro-theorem-for-convergent-sequences">Cesàro theorem for convergent sequences</h1>

↑ **Parent:** [Cesàro mean](cesaro-mean.md)

If a real or complex [sequence](sequence.md) converges to $a$, its [Cesàro means](cesaro-mean.md) have the same [limit of a sequence](limit-of-a-sequence.md). This is why [Cesàro summation](cesaro-summation.md) is a [regular summation method](regular-summation-method.md) when applied to the [partial sums](partial-sum.md) of a [series](series-mathematics.md).

**Proof outline.** Given $\varepsilon>0$, choose $K$ so that $|a_k-a|<\varepsilon$ for $k>K$. The [triangle inequality](triangle-inequality.md) gives, for $n>K$,

$$
\left|\frac1n\sum_{k=1}^n a_k-a\right|\leq\frac1n\sum_{k=1}^{K}|a_k-a|+\varepsilon\frac{n-K}{n}.
$$

The finite initial contribution tends to zero, and the remaining contribution is at most $\varepsilon$. The converse fails: the alternating [sequence](sequence.md) $(-1)^n$ has [Cesàro means](cesaro-mean.md) tending to zero while its terms do not converge.

## ↑ Ancestors (8)

1. [Cesàro mean](cesaro-mean.md)
2. [Convergent sequence](convergent-sequence.md)
3. [Sequence and series](sequence-and-series-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Cesàro summation](cesaro-summation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/8d/b/solution.md)
- [Regular summation method](regular-summation-method.md)
- [Ultrafilter construction of a Banach limit](ultrafilter-construction-of-a-banach-limit.md)
