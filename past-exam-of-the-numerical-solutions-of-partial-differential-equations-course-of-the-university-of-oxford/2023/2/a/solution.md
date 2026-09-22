<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $u^{(m,n)}(x,y)=\sin(m\pi x)\sin(n\pi y)$, direct differentiation yields

$$
\partial_{xx}u^{(m,n)}=-(m\pi)^2u^{(m,n)},\qquad
\partial_{yy}u^{(m,n)}=-(n\pi)^2u^{(m,n)}.
$$

Since the planar [Laplacian](../../../../laplacian.md) is $\Delta=\partial_{xx}+\partial_{yy}$, the required [eigenvalue](../../../../eigenvalue.md) of $-\Delta+I$ is

$$
\boxed{\lambda_{m,n}=1+\pi^2(m^2+n^2)>0.}
$$

On the sides $x=0,1$ the first [sine](../../../../sine.md) factor vanishes, and on $y=0,1$ the second [sine](../../../../sine.md) factor vanishes. Thus the homogeneous [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md) holds on the whole boundary. The [eigenfunction](../../../../eigenfunction.md) is nonzero, for instance at $(x,y)=(1/(2m),1/(2n))$, where its value is one.

## ↑ Ancestors (12)

1. [A](../a.md)
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
