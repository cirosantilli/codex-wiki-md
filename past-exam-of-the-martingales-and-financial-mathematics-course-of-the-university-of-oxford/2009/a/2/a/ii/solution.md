<h1 id="a/2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\Delta_0=X_0$ and $\Delta_j=X_j-X_{j-1}$ for $j\geq1$. If $i<j$, then $\Delta_i$ is $\mathcal F_{j-1}$-measurable. The [martingale](../../../../../../martingale-split.md) property and linearity of [conditional expectation](../../../../../../conditional-expectation.md) give

$$
\mathbb E(\Delta_j\mid\mathcal F_{j-1})=0.
$$

The product $\Delta_i\Delta_j$ is integrable by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The pull-out property of [conditional expectation](../../../../../../conditional-expectation.md), followed by its [tower property](../../../../../../law-of-total-expectation.md), therefore gives

$$
\mathbb E(\Delta_i\Delta_j)
=\mathbb E\{\Delta_i\mathbb E(\Delta_j\mid\mathcal F_{j-1})\}=0.
$$

For unbounded $\Delta_i$, the pull-out identity follows by truncation and [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). This proves [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md), including orthogonality to the initial value.

Expand $X_n=\sum_{j=0}^n\Delta_j$ in the Hilbert space $L^2$. Orthogonality gives the exact identity

$$
\boxed{\mathbb E X_n^2=\mathbb E X_0^2+\sum_{j=0}^{n-1}\mathbb E(X_{j+1}-X_j)^2.}
$$

The terms are nonnegative and $\mathbb E X_0^2<\infty$, so boundedness of the left side over $n$ is equivalent to convergence of the series on the right.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
