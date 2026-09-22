<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [five-point Laplacian](../../../../five-point-laplacian.md) on the square grid is

$$
\boxed{\Delta_hW_{i,j}=\frac{W_{i+1,j}+W_{i-1,j}+W_{i,j+1}+W_{i,j-1}-4W_{i,j}}{h^2},\qquad1\leq i,j\leq N-1.}
$$

It adds the [second-order central differences](../../../../second-order-central-difference.md) in the two coordinate directions and uses the given zero [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) when a neighbouring node lies on the boundary.

The [sine addition formula](../../../../sine-addition-formula.md) implies

$$
\sin((i+1)\alpha)+\sin((i-1)\alpha)-2\sin(i\alpha)
=2(\cos\alpha-1)\sin(i\alpha)
=-4\sin^2(\alpha/2)\sin(i\alpha).
$$

Apply this identity with $\alpha=m\pi h$ in the $x$ direction and with $\alpha=n\pi h$ in the $y$ direction. For $U_{i,j}^{(m,n)}=\sin(m\pi ih)\sin(n\pi jh)$, it gives

$$
-\Delta_hU_{i,j}^{(m,n)}+U_{i,j}^{(m,n)}
=\left[1+\frac4{h^2}\left(\sin^2\frac{m\pi h}2+\sin^2\frac{n\pi h}2\right)\right]U_{i,j}^{(m,n)}.
$$

Hence the discrete [eigenvalues](../../../../eigenvalue.md) are

$$
\boxed{\Lambda_{m,n}=1+\frac4{h^2}\left(\sin^2\frac{m\pi h}2+\sin^2\frac{n\pi h}2\right)>0,\qquad1\leq m,n\leq N-1.}
$$

Both [sine](../../../../sine.md) factors vanish on their respective boundary sides. Also $U_{1,1}^{(m,n)}>0$, since $m\pi/N$ and $n\pi/N$ lie strictly between zero and $\pi$. Thus each array is a nonzero discrete [eigenvector](../../../../eigenvector.md), rather than merely the zero solution of the homogeneous system. The separated structure is also described by the [five-point Dirichlet Laplacian as a Kronecker sum](../../../../five-point-dirichlet-laplacian-as-a-kronecker-sum.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
