<h1 id="3/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [midpoint quadratic spline collocation](../../../../../../../midpoint-quadratic-spline-collocation.md) matrix is

$$
\boxed{A_x=\frac18
\begin{pmatrix}
6&1&0&\cdots&0\\
1&6&1&\ddots&\vdots\\
0&1&6&\ddots&0\\
\vdots&\ddots&\ddots&\ddots&1\\
0&\cdots&0&1&6
\end{pmatrix}.}
$$

Its [strict diagonal dominance](../../../../../../../strictly-diagonally-dominant-matrix.md) margin is at least $3/4-2/8=1/2$. The [inverse infinity-norm bound from diagonal dominance](../../../../../../../inverse-infinity-norm-bound-from-diagonal-dominance.md) thus already proves $\|A_x^{-1}\|_\infty\le2$: choosing an index where a vector $c$ attains its maximum absolute entry gives $\|A_xc\|_\infty\ge\tfrac12\|c\|_\infty$, which also proves invertibility.

To evaluate the finite-dimensional norm exactly, set $D_{ii}=(-1)^i$ and $B=DA_xD$. If $T$ is the matrix with ones on its two adjacent diagonals and zeros elsewhere, then $B=(3/4)(I-T/6)$. Since $\|T/6\|_\infty\le1/3$, the [Neumann series](../../../../../../../neumann-series.md)

$$
B^{-1}=\frac43\sum_{r=0}^\infty(T/6)^r
$$

has nonnegative entries. Thus $A_x^{-1}=DB^{-1}D$ has absolute entry values equal to those of $B^{-1}$. Its absolute row-sum vector is $v=B^{-1}\mathbf1$, characterized by

$$
6v_i-v_{i-1}-v_{i+1}=8,\qquad v_0=v_{n+1}=0.
$$

The homogeneous roots are $3\pm2\sqrt2$, and the constant particular solution is $v_i=2$. Writing $q=3-2\sqrt2\in(0,1)$ and imposing the two boundary values gives

$$
v_i=2\left[1-\frac{q^i+q^{n+1-i}}{1+q^{n+1}}\right].
$$

This is largest at the middle row or rows. Therefore, with $i_* =\lfloor(n+1)/2\rfloor$, **the exact norm is**

$$
\boxed{\|A_x^{-1}\|_\infty=
2\left[1-\frac{q^{i_*}+q^{n+1-i_*}}{1+q^{n+1}}\right]<2.}
$$

For example, it is $4/3$ for $n=1$ and $8/5$ for $n=2$, and it increases towards two as the system grows. Thus two is a uniform bound, rather than the exact finite-$n$ inverse norm.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 69](../../../../paper-69-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
