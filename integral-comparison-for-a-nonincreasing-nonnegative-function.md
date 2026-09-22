# Integral comparison for a nonincreasing nonnegative function

↑ **Parent:** [Integral test for convergence](integral-test-for-convergence.md)

For a nonnegative [nonincreasing function](nonincreasing-function.md) $f:[1,\infty)\to[0,\infty)$, comparison with unit-width rectangles gives

$$
\int_1^{N+1}f(x)\,dx
\leq\sum_{n=1}^{N}f(n)
\leq f(1)+\int_1^Nf(x)\,dx.
$$

On $[n,n+1]$, the [function](function-split.md) is at most $f(n)$; on $[n-1,n]$, it is at least $f(n)$. Summing these inequalities gives the bounds. Applying them to $f(x)=1/x$ gives $\log(N+1)\leq H_N\leq1+\log N$ for the [harmonic numbers](harmonic-number.md). Unlike a convergence verdict alone, the finite bounds estimate the size of a [partial sum](partial-sum.md).

## ↑ Ancestors (9)

1. [Integral test for convergence](integral-test-for-convergence.md)
2. [Comparison test for series](comparison-test-for-series.md)
3. [Convergent series](convergent-series.md)
4. [Sequence and series](sequence-and-series-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2/10/a/solution.md)
