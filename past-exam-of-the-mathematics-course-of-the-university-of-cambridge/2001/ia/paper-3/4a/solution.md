<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Consider the globally smooth potential $\Phi(x,y,z)=xy^2\sin(xz)$. Direct differentiation gives

$$
\Phi_x=y^2\sin(xz)+xy^2z\cos(xz)=u,\qquad
\Phi_y=2xy\sin(xz)=v,\qquad
\Phi_z=x^2y^2\cos(xz)=w.
$$

Thus the [differential one-form](../../../../../one-form.md) is the [exact differential](../../../../../exact-differential.md) $d\Phi$, proving exactness rather than only checking a necessary condition on its partial derivatives. Along any piecewise differentiable path, the [chain rule](../../../../../chain-rule.md) gives $u\,dx+v\,dy+w\,dz=d\Phi$. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) therefore makes the [line integral](../../../../../line-integral.md) depend only on its endpoints:

$$
\boxed{\int_{(0,0,0)}^{(\pi/2,1,1)}(u\,dx+v\,dy+w\,dz)
=\Phi(\pi/2,1,1)-\Phi(0,0,0)=\frac\pi2.}
$$

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
