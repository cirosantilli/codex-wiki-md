<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [spline interpolation operator](../../../../../spline-interpolation-operator.md) as $P_{\mathbf x}=TA_{\mathbf x}^{-1}R$, where $R$ samples at the interpolation sites and $T$ synthesizes the normalized [B-spline](../../../../../b-spline.md) expansion. Sampling has [operator norm](../../../../../operator-norm.md) at most one, and nonnegative [B-splines](../../../../../b-spline.md) with sum at most one give $\|T\|\le1$. Hence

$$
\|P_{\mathbf x}g\|_\infty\le\|A_{\mathbf x}^{-1}Rg\|_{\ell^\infty}\le\|A_{\mathbf x}^{-1}\|_{\ell^\infty}\|g\|_\infty,
\qquad\boxed{\|P_{\mathbf x}\|\le\|A_{\mathbf x}^{-1}\|_{\ell^\infty}.}
$$

Here the [matrix norm](../../../../../matrix-norm.md) is the maximum absolute row sum. Existence of the [inverse matrix](../../../../../matrix-inverse.md) requires the usual ordered distinct interpolation sites and the [Schoenberg–Whitney theorem](../../../../../schoenberg-whitney-theorem.md) support conditions, with endpoint values interpreted by their one-sided limits. If the displayed diagonal condition is read without the implicit ordering and distinctness, it is insufficient: all three sites equal to $1/2$ in the quadratic example give positive diagonal entries but three identical rows. The estimate applies whenever the interpolating [linear map](../../../../../linear-map.md) in the question is defined uniquely.

For the quadratic [Bernstein basis](../../../../../bernstein-basis.md), $N_1=(1-x)^2$, $N_2=2x(1-x)$ and $N_3=x^2$. Sampling and inverting give

$$
A=\begin{pmatrix}1&0&0\\1/4&1/2&1/4\\0&0&1\end{pmatrix},\qquad
A^{-1}=\begin{pmatrix}1&0&0\\-1/2&2&-1/2\\0&0&1\end{pmatrix},\qquad
\boxed{\|A^{-1}\|_{\ell^\infty}=3.}
$$

The three cardinal [Lagrange interpolation polynomials](../../../../../lagrange-polynomial.md) are

$$
\ell_0(x)=2x^2-3x+1,\qquad\ell_1(x)=4x(1-x),\qquad\ell_2(x)=2x^2-x.
$$

The [Lebesgue constant of interpolation](../../../../../lebesgue-constant-of-interpolation.md) gives the exact [operator norm](../../../../../operator-norm.md): the upper bound follows from $|Pg(x)|\le\|g\|_\infty\sum_i|\ell_i(x)|$. To attain it at a maximizing point, prescribe at the three sites the signs of the corresponding cardinal [polynomials](../../../../../polynomial-split.md) and extend those values by a [continuous](../../../../../continuous-function.md) [piecewise linear function](../../../../../piecewise-linear-function.md) of [norm](../../../../../norm.md) one.

On $0\le x\le1/2$, the first two cardinal [polynomials](../../../../../polynomial-split.md) are nonnegative and the last is nonpositive. Since their sum is one, their absolute sum is $1-2\ell_2(x)=1+2x-4x^2$. Its maximum is $5/4$ at $x=1/4$. Reflection gives the same maximum at $3/4$ on the other half. In particular the data $(1,1,-1)$ produce $1+2x-4x^2$, attaining $5/4$. Thus

$$
\boxed{\|P_{\mathbf x}\|=\frac54<3=\|A^{-1}\|_{\ell^\infty}.}
$$

The coefficient estimate loses cancellation among the [B-splines](../../../../../b-spline.md), which explains why it is not sharp for the resulting [function](../../../../../function-split.md) [norm](../../../../../norm.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
