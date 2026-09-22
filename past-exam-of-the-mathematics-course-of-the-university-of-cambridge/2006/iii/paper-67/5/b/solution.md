<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [B-spline collocation matrix](../../../../../../b-spline-collocation-matrix.md) in the cubic case is the finite [tridiagonal matrix](../../../../../../tridiagonal-matrix.md)

$$
\boxed{A_n=\frac16\begin{pmatrix}
4&1&0&\cdots&0\\
1&4&1&\ddots&\vdots\\
0&1&4&\ddots&0\\
\vdots&\ddots&\ddots&\ddots&1\\
0&\cdots&0&1&4
\end{pmatrix}.}
$$

For $n=1$, this is simply the one-entry [matrix](../../../../../../matrix.md) $(2/3)$.

To evaluate the inverse [norm](../../../../../../norm.md) exactly, let $D=\operatorname{diag}((-1)^1,\ldots,(-1)^n)$. Then $B_n=DA_nD=(4I-C)/6$, where $C$ has ones immediately above and below the diagonal and zeros elsewhere. Since $\|C/4\|_{\ell^\infty}\leq1/2$, the convergent [Neumann series](../../../../../../neumann-series.md)

$$
B_n^{-1}=\frac32\sum_{r=0}^\infty(C/4)^r
$$

has nonnegative entries and proves invertibility. Since $A_n^{-1}=DB_n^{-1}D$, its absolute entries equal those of $B_n^{-1}$. The absolute row sums are therefore the entries of $u=B_n^{-1}\mathbf1$.

The equation $B_nu=\mathbf1$ becomes

$$
4u_i-u_{i-1}-u_{i+1}=6,\qquad u_0=u_{n+1}=0.
$$

Its constant particular solution is $3$; the two characteristic roots of the homogeneous recurrence are $\rho=2-\sqrt3$ and $\rho^{-1}=2+\sqrt3$. Imposing the two boundary values gives

$$
\boxed{u_i=3\left[1-\frac{\rho^i+\rho^{n+1-i}}{1+\rho^{n+1}}\right],\qquad\rho=2-\sqrt3.}
$$

This can also be checked by direct substitution, since $\rho+\rho^{-1}=4$. The numerator is smallest at the central index or central pair of indices: its successive difference is $(1-\rho)(\rho^{n-i}-\rho^i)$. Thus, with $j=\lfloor(n+1)/2\rfloor$, the [exact inverse norm of midpoint cubic spline collocation](../../../../../../exact-inverse-norm-of-midpoint-cubic-spline-collocation.md) is

$$
\boxed{\|A_n^{-1}\|_{\ell^\infty}=u_j
=3\left[1-\frac{\rho^j+\rho^{n+1-j}}{1+\rho^{n+1}}\right]<3.}
$$

Equivalently, if $n=2m-1$ the fraction is $2\rho^m/(1+\rho^{2m})$, and if $n=2m$ it is $(\rho^m+\rho^{m+1})/(1+\rho^{2m+1})$. The finite [norm](../../../../../../norm.md) is not exactly three: it equals $3/2$ for $n=1$, two for $n=2$, and tends to three as $n$ grows. Hence three is the sharp dimension-independent bound for these inverse [matrix](../../../../../../matrix.md) [norms](../../../../../../norm.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
