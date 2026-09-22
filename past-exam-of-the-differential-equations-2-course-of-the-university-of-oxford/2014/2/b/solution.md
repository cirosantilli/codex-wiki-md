<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X=(x,y)$ be the integration variable and $P=(\xi,\eta)$ the interior source point. [Green's second identity](../../../../green-second-identity.md), obtained from [Green's theorem](../../../../green-theorem.md) by applying the [divergence theorem](../../../../divergence-theorem.md) to $u\nabla G-G\nabla u$, is

$$
\int_D(u\Delta G-G\Delta u)\,dA
=\int_{\partial D}\left(u\frac{\partial G}{\partial n}-G\frac{\partial u}{\partial n}\right)ds.
$$

The outward normal is used throughout. To obtain the prescribed representation with its positive volume term, choose

$$
\boxed{\Delta_XG(X,P)=\delta(X-P),\qquad
G=0\text{ on }\partial D_1,\qquad
\partial_nG=0\text{ on }\partial D_2.}
$$

Indeed, substituting $\Delta u=f$ makes the left side $u(P)-\int_DGf$. On the Dirichlet portion, $u=g$ and $G=0$ leave only $g\partial_nG$. On the Neumann portion, both normal derivatives vanish. Rearranging gives exactly the desired boundary-plus-volume representation. The distributional identity can equivalently be justified by excluding a small circle around $P$ and using the logarithmic singularity there.

For the quarter-plane, the [fundamental solution of the Laplace equation](../../../../fundamental-solution-of-the-laplace-equation.md) with this sign convention is $\Phi(X,P)=(2\pi)^{-1}\log|X-P|$, since $\Delta\Phi=\delta_P$. The [method of images](../../../../method-of-images.md) uses an equal-sign reflection across the Neumann boundary $x=0$ and an opposite-sign reflection across the Dirichlet boundary $y=0$. Hence

$$
G(X,P)=\frac1{2\pi}\bigl[\log|X-(\xi,\eta)|+\log|X-(-\xi,\eta)|
-\log|X-(\xi,-\eta)|-\log|X-(-\xi,-\eta)|\bigr].
$$

Equivalently,

$$
\boxed{G(x,y,\xi,\eta)=\frac1{4\pi}\log
\frac{\bigl((x-\xi)^2+(y-\eta)^2\bigr)\bigl((x+\xi)^2+(y-\eta)^2\bigr)}
{\bigl((x-\xi)^2+(y+\eta)^2\bigr)\bigl((x+\xi)^2+(y+\eta)^2\bigr)}.}
$$

Only $(\xi,\eta)$ lies inside the domain, so the interior [Laplacian](../../../../laplacian.md) has exactly the required unit point source. At $y=0$ numerator and denominator agree, giving $G=0$. The formula is even in $x$, giving $\partial_xG=0$ at $x=0$, and therefore zero outward normal derivative there.

On the Dirichlet boundary $y=0$, the outward normal is $-\partial_y$, and differentiation gives the useful check

$$
\frac{\partial G}{\partial n}(x,0,\xi,\eta)
=\frac\eta\pi\left[\frac1{(x-\xi)^2+\eta^2}+\frac1{(x+\xi)^2+\eta^2}\right]>0.
$$

This is the [mixed Dirichlet-Neumann Green function in a quadrant](../../../../mixed-dirichlet-neumann-green-function-in-a-quadrant.md). The image solution tends to zero at spatial infinity; on the unbounded domain the representation uses data and solutions for which the [boundary term at infinity in Green's second identity](../../../../boundary-term-at-infinity-in-green-s-second-identity.md) vanishes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
