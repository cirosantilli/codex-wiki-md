<h1 id="4/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [centered quadratic spline interpolation](../../../../../../../centered-quadratic-spline-interpolation.md) [matrix](../../../../../../../matrix.md) is the [symmetric tridiagonal Toeplitz matrix](../../../../../../../symmetric-tridiagonal-toeplitz-matrix.md)

$$
\boxed{A_x=\frac18\begin{pmatrix}
6&1&0&\cdots&0\\
1&6&1&\ddots&\vdots\\
0&1&6&\ddots&0\\
\vdots&\ddots&\ddots&\ddots&1\\
0&\cdots&0&1&6
\end{pmatrix}.}
$$

For $n=1$, this means simply $A_x=(3/4)$. To evaluate the inverse [norm](../../../../../../../norm.md) exactly, let $D=\operatorname{diag}((-1)^i)_{i=1}^n$ and $M=8DA_xD=\operatorname{tridiag}(-1,6,-1)$. If $J$ is the nonnegative adjacency [matrix](../../../../../../../matrix.md) of the path, then $M=6I-J$ and $\|J/6\|_\infty\le1/3$. The convergent [Neumann series](../../../../../../../neumann-series.md)

$$
M^{-1}=\frac16\sum_{r=0}^{\infty}(J/6)^r
$$

therefore has nonnegative entries. Since $A_x^{-1}=8DM^{-1}D$, its entrywise absolute values are $8M^{-1}$. Let $r_i=\sum_j|(A_x^{-1})_{ij}|$. Then $r=8M^{-1}\mathbf1$, or

$$
6r_i-r_{i-1}-r_{i+1}=8,\qquad r_0=r_{n+1}=0.
$$

The homogeneous characteristic roots are $3\pm2\sqrt2$. Put $\tau=3-2\sqrt2\in(0,1)$. The particular solution $r_i=2$ and the two boundary conditions give

$$
r_i=2\left(1-\frac{\tau^i+\tau^{n+1-i}}{1+\tau^{n+1}}\right).
$$

These row sums are symmetric and increase toward the centre: the exponential sum in the numerator is minimized at the middle [integer](../../../../../../../integer.md) or pair of [integers](../../../../../../../integer.md). With $m=\lfloor(n+1)/2\rfloor$, the exact finite-size inverse [norm](../../../../../../../norm.md) is thus

$$
\boxed{\|A_x^{-1}\|_{\ell^\infty}
=2\left(1-\frac{\tau^m+\tau^{n+1-m}}{1+\tau^{n+1}}\right)<2.}
$$

For example it equals $4/3$ at $n=1$ and $8/5$ at $n=2$, tending to $2$ as $n\to\infty$. Stating only the bound two would not evaluate the finite [matrix](../../../../../../../matrix.md) [norm](../../../../../../../norm.md) requested here.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 71](../../../../paper-71-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
