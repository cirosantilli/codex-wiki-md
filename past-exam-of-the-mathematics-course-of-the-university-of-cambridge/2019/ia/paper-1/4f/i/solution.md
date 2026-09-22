<h1 id="4f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
S=\left\{r\geq0:\sum_{n=1}^\infty |a_n|r^n<\infty\right\}.
$$

The set $S$ contains zero. If $r\in S$ and $0\leq s<r$, then $s\in S$ by comparison. Moreover, if the original [power series](../../../../../../power-series.md) diverges at $x_0$, no $r>|x_0|$ can lie in $S$, because absolute convergence at $r$ would imply absolute convergence at $x_0$. Thus $R=\sup S$ is finite and nonnegative.

If $|x|<R$, choose $r\in S$ with $|x|<r$; comparison gives absolute convergence at $x$. If $|x|>R$ and the series converged at $x$, then its terms $a_nx^n$ would be bounded. For any $y$ with $R<|y|<|x|$,

$$
|a_ny^n|\leq M\left|\frac yx\right|^n,
$$

so the [geometric series](../../../../../../geometric-series.md) comparison would put $|y|$ in $S$, contradicting the definition of $R$. This proves the [radius of convergence](../../../../../../radius-of-convergence.md) property.

For $\sum_{n\geq1}x^n/3^n$, the ratio is $x/3$, so the [geometric series](../../../../../../geometric-series.md) criterion gives

$$
\boxed{R=3}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4F](../../4f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
