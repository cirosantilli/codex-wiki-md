<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Stationarity of the equality-constrained quadratic subproblem gives $B_ks_k+g_k-A_k^Ty_{k+1}=0$. Together with feasibility, this is

$$
\boxed{\begin{pmatrix}B_k&-A_k^T\\A_k&0\end{pmatrix}\begin{pmatrix}s_k\\y_{k+1}\end{pmatrix}=\begin{pmatrix}-g_k\\-c_k\end{pmatrix}.}
$$

Multiplying the bottom block row by $-1$ gives a symmetric indefinite [saddle-point matrix](../../../../../saddle-point-matrix.md), with right side $(-g_k,c_k)^T$.

One solution strategy uses the [Schur complement](../../../../../schur-complement.md). From $s_k=B_k^{-1}(A_k^Ty_{k+1}-g_k)$ obtain

$$
\boxed{(A_kB_k^{-1}A_k^T)y_{k+1}=A_kB_k^{-1}g_k-c_k.}
$$

This is an $m\times m$ positive-definite system when $A_k$ has full row rank; factor $B_k$ and solve with it rather than forming its inverse.

A second strategy uses a [nullspace](../../../../../kernel-of-a-linear-map-split.md) basis $Z$ for $\ker A_k$. Choose one particular $s_p$ with $A_ks_p=-c_k$, write $s_k=s_p+Zz$, and solve the reduced system

$$
\boxed{Z^TB_kZz=-Z^T(g_k+B_ks_p).}
$$

The [reduced Hessian](../../../../../reduced-hessian.md) is positive definite. These range-space and nullspace reductions exploit different relative sizes of $m$ and $n-m$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
