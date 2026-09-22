# Composition coefficients of power series

↑ **Parent:** [Power series](power-series.md)

For [power series](power-series.md) $f(z)=\sum_{m\geq0}f_mz^m$ and $g(x)=\sum_{j\geq1}g_jx^j$, their [function composition](function-composition.md) is well defined as a [formal power series](formal-power-series.md): the coefficient of $x^n$ receives contributions only from $m\leq n$, since $g$ has zero [constant term](constant-term.md). For $m\geq1$, expand the coefficient as

$$
[x^n]g(x)^m=\sum_{\substack{j_1+\cdots+j_m=n\\j_1,\ldots,j_m\geq1}}g_{j_1}\cdots g_{j_m}.
$$

The $m=0$ term is one for $n=0$ and zero otherwise. The first four coefficients of the [function composition](function-composition.md) are therefore $f_0$, $f_1g_1$, $f_1g_2+f_2g_1^2$, and $f_1g_3+2f_2g_1g_2+f_3g_1^3$. For convergent [power series](power-series.md), the same calculation holds wherever $g(x)$ lies inside the [radius of convergence](radius-of-convergence.md) of $f$.

## ↑ Ancestors (7)

1. [Power series](power-series.md)
2. [Sequence and series](sequence-and-series-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/section-b/3/b/solution.md)
