<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the preceding sign convention, [Green's second identity](../../../../../green-second-identity.md) gives the harmonic representation

$$
u(P)=-\int_{\partial D}u(Q)\,\partial_{n_Q}G(P;Q)\,dS_Q,
$$

provided the far-boundary term vanishes or the bounded-solution representation applies. The face $x=0$ contributes nothing because $g_1=0$. On $\zeta=0$, the outward normal is $-e_\zeta$, so the remaining kernel is $-\partial_{n_Q}G=\partial_\zeta G$. Differentiating the image sum gives

$$
\boxed{u(x,y,z)=\frac z{2\pi}\int_{-\infty}^{\infty}\int_0^\infty\left\{\frac1{[(x-\xi)^2+(y-\eta)^2+z^2]^{3/2}}-\frac1{[(x+\xi)^2+(y-\eta)^2+z^2]^{3/2}}\right\}g(\xi,\eta)\,d\xi\,d\eta}.
$$

Thus the requested constants are

$$
\boxed{h(z)=\frac z{2\pi},\qquad\alpha=\frac32,\qquad\alpha_0=1,\quad\alpha_1=-1}.
$$

The [Poisson kernel of a three-dimensional quarter-space](../../../../../poisson-kernel-of-a-three-dimensional-quarter-space.md) is the difference of the upper-half-space kernel and its reflection in $x=0$. For bounded, suitably continuous data it produces the bounded harmonic solution, taking the prescribed traces away from the edge. Continuous data at the common edge must be compatible. Without any growth restriction at infinity, boundary values alone do not give uniqueness: a multiple of the harmonic function $xz$ can be added while leaving both face values zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the applied partial differential equations course of the University of Oxford](../../../../split.md)
6. [Applied partial differential equations course of the University of Oxford](../../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
