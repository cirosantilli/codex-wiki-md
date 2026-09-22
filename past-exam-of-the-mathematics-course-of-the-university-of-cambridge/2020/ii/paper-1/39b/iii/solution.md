<h1 id="39b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $B=0$, the stated [biharmonic stream function for planar Stokes flow](../../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) is

$$
\psi=A\sin^2\theta+Cr\sin\theta+\frac{D\sin^3\theta}{r}.
$$

Requiring it to vanish at $r=2a\sin\theta$ and $r=4a\sin\theta$ gives

$$
A+2aC+\frac{D}{2a}=0,
\qquad A+4aC+\frac{D}{4a}=0.
$$

Thus $A=-6aC$ and $D=8a^2C$. Writing $C=\alpha$ yields

$$
\boxed{\psi=\alpha\left(r\sin\theta-6a\sin^2\theta
+\frac{8a^2\sin^3\theta}{r}\right)
=\frac{\alpha\sin\theta}{r}
(r-2a\sin\theta)(r-4a\sin\theta).}
$$

Using $u_r=\psi_\theta/r$ and $u_\theta=-\psi_r$, differentiation shows that $u_r\cos\theta+u_\theta\sin\theta$ equals $\alpha$ on the inner boundary and $-\alpha/2$ on the outer boundary. Both wall conditions hold precisely when

$$
\boxed{\alpha=a\Omega.}
$$

This is the [Stokes flow between touching counter-rotating cylinders](../../../../../../stokes-flow-between-touching-counter-rotating-cylinders.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [39B](../../39b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
