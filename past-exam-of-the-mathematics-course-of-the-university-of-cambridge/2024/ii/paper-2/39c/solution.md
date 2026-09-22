<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

The incompressible Stokes equations are

$$
-\nabla p+\mu\nabla^2u=0,\qquad\nabla\cdot u=0.
$$

Taking the curl gives $\nabla^2\omega=0$. For a planar [stream function](../../../../../stream-function.md), $\omega=-\nabla^2\psi$, so the [biharmonic stream function for planar Stokes flow](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) satisfies

$$
\boxed{\nabla^4\psi=0}.
$$

For $\psi=r^2f(\theta)$,

$$
u_r=rf',\qquad u_\theta=-2rf.
$$

The polar rate-of-strain components are

$$
e_{rr}=\partial_ru_r=f',\qquad
e_{\theta\theta}=\frac1r\partial_\theta u_\theta+\frac{u_r}{r}=-f',
$$



$$
e_{r\theta}=\frac12\left(
\frac1r\partial_\theta u_r+\partial_ru_\theta-\frac{u_\theta}{r}
\right)=\frac12f''.
$$

Hence

$$
\boxed{
e=\begin{pmatrix}f'&f''/2\\f''/2&-f'\end{pmatrix},
\qquad
\tau=2\mu e
=\mu\begin{pmatrix}2f'&f''\\f''&-2f'\end{pmatrix}.}
$$

Since

$$
\nabla^2(r^2f)=4f+f'',
$$

biharmonicity gives

$$
f^{(4)}+4f''=0,
\qquad
f=A+B\theta+C\cos2\theta+D\sin2\theta.
$$

No slip at $\theta=-\alpha$, no penetration at $\theta=0$, and the imposed tangential traction give

$$
f(-\alpha)=f'(-\alpha)=f(0)=0,\qquad
\mu f''(0)=S.
$$

Put $\Delta=\sin2\alpha-2\alpha\cos2\alpha$. Solving,

$$
f(\theta)=\frac{S}{4\mu}\left[
1-\cos2\theta+
\frac{2(1-\cos2\alpha)\theta+
(1-\cos2\alpha-2\alpha\sin2\alpha)\sin2\theta}
{\Delta}\right].
$$

The upper-surface [velocity](../../../../../velocity.md) is radial and equals $rf'(0)$. Therefore the [similarity solution for tangentially forced Stokes wedge](../../../../../similarity-solution-for-tangentially-forced-stokes-wedge.md) gives

$$
\boxed{
U(r)=\frac{Sr}{\mu}
\frac{1-\cos2\alpha-\alpha\sin2\alpha}
{\sin2\alpha-2\alpha\cos2\alpha}}.
$$

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
