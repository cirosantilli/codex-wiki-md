<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Truncate the [Chebyshev series](../../../../../chebyshev-series.md) at the full [degree of precision of a quadrature rule](../../../../../degree-of-precision-of-a-quadrature-rule.md):

$$
s_{2n+1}(x)=\sum_{j=0}^{2n+1}c_jT_j(x),\qquad R_n=f-s_{2n+1}.
$$

Since $|T_j(x)|\leq1$ on $[-1,1]$, the [geometric series](../../../../../geometric-series.md) estimate gives

$$
\|R_n\|_\infty\leq\sum_{j=2n+2}^\infty e^{-Kj}
=\frac{e^{-K(2n+2)}}{1-e^{-K}}.
$$

The same bound proves [uniform convergence](../../../../../uniform-convergence.md) of the original [Chebyshev series](../../../../../chebyshev-series.md), so its sum and the tail estimate are justified. [Gauss-Legendre quadrature](../../../../../gauss-legendre-quadrature.md) is exact on $s_{2n+1}$. Its positive [quadrature weights](../../../../../quadrature-weight.md) sum to $2$, hence

$$
\begin{aligned}
|I-\widehat I_n|
&=\left|\int_{-1}^1R_n(x)\,dx-\sum_{i=0}^nw_iR_n(x_i)\right|\\
&\leq2\|R_n\|_\infty+\left(\sum_{i=0}^nw_i\right)\|R_n\|_\infty\\
&\leq\frac{4e^{-2K}}{1-e^{-K}}e^{-2Kn}.
\end{aligned}
$$

Therefore one explicit choice proving [exponential convergence of Gaussian quadrature](../../../../../exponential-convergence-of-gaussian-quadrature.md) is

$$
\boxed{C=\frac{4e^{-2K}}{1-e^{-K}},\qquad L=2K.}
$$

Using exactness through [polynomial degree](../../../../../degree-of-a-polynomial.md) $2n+1$ doubles the exponent compared with truncating at [polynomial degree](../../../../../degree-of-a-polynomial.md) $n$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
