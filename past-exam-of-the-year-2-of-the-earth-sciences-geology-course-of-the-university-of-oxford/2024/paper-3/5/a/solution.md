<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $h=\Delta x$ and suppose $L=(n+1)h$, so there are $n$ interior grid points $x_j=jh$, $j=1,\ldots,n$. Write $u_j(t)\simeq u(x_j,t)$. The fixed ends impose homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md),

$$
u_0(t)=u_{n+1}(t)=0.
$$

For a sufficiently smooth [displacement](../../../../../displacement.md) field, the two [Taylor series](../../../../../taylor-series.md) at fixed time give

$$
\begin{aligned}
u(x_j+h,t)&=u(x_j,t)+hu_x+\frac{h^2}{2}u_{xx}+\frac{h^3}{6}u_{xxx}+O(h^4),\\
u(x_j-h,t)&=u(x_j,t)-hu_x+\frac{h^2}{2}u_{xx}-\frac{h^3}{6}u_{xxx}+O(h^4),
\end{aligned}
$$

where all displayed [derivatives](../../../../../derivative.md) on the right are evaluated at $(x_j,t)$. Adding cancels the odd terms, leaving the [second-order central difference](../../../../../second-order-central-difference.md)

$$
u_{xx}(x_j,t)=\frac{u(x_j-h,t)-2u(x_j,t)+u(x_j+h,t)}{h^2}+O(h^2).
$$

Substitute this [finite difference](../../../../../finite-difference-split.md) into the [wave equation](../../../../../wave-equation-split.md) and retain continuous time. The resulting [method of lines](../../../../../method-of-lines.md) gives coupled second-order [ordinary differential equations](../../../../../ordinary-differential-equation.md),

$$
\ddot u_j=\frac{c^2}{h^2}(u_{j-1}-2u_j+u_{j+1}),\qquad j=1,\ldots,n.
$$

In particular, the first and last equations are $\ddot u_1=(c^2/h^2)(-2u_1+u_2)$ and $\ddot u_n=(c^2/h^2)(u_{n-1}-2u_n)$ for $n\ge2$. With the interior [displacement](../../../../../displacement.md) [vector](../../../../../vector.md) only,

$$
\boxed{\ddot{\mathbf u}=A\mathbf u,\qquad
\mathbf u=(u_1,\ldots,u_n)^T,\qquad
A=\frac{c^2}{h^2}\begin{pmatrix}
-2&1&0&\cdots&0\\
1&-2&1&\ddots&\vdots\\
0&\ddots&\ddots&\ddots&0\\
\vdots&\ddots&1&-2&1\\
0&\cdots&0&1&-2
\end{pmatrix}.}
$$

Equivalently, $A_{jj}=-2c^2/h^2$, $A_{j,j+1}=A_{j+1,j}=c^2/h^2$, and all other entries vanish. This entrywise definition also covers small $n$, including $A=(-2c^2/h^2)$ when $n=1$. The [matrix](../../../../../matrix.md) is a [symmetric matrix](../../../../../symmetric-matrix.md) and a [tridiagonal matrix](../../../../../tridiagonal-matrix.md). The spatial approximation has error $O(h^2)$ in [Big O notation](../../../../../big-o-notation.md); time has not yet been discretized.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
