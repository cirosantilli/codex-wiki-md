<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the supplied [velocity](../../../../velocity.md) in the radial form

$$
\mathbf u=f(r)\mathbf U+g(r)(\mathbf U\cdot\mathbf x)\mathbf x,\qquad
f=\frac{3a}{4r}+\frac{a^3}{4r^3},\quad
g=\frac{3a}{4r^3}-\frac{3a^3}{4r^5}.
$$

At $r=a$, $f=1$ and $g=0$, giving the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) $\mathbf u=\mathbf U$. At infinity $\mathbf u\to0$ and the supplied gauge-fixed [pressure](../../../../pressure-split.md) tends to zero. These are the laboratory-frame conditions for a sphere translating through otherwise quiescent fluid.

The exterior [Stokes equations](../../../../stokes-equation.md) can also be checked directly:

$$
\nabla\cdot\mathbf u=(\mathbf U\cdot\mathbf x)\left(\frac{f'}r+rg'+4g\right)=0,
$$

and

$$
\begin{aligned}
\nabla^2\mathbf u
&=\left(f''+\frac{2f'}r+2g\right)\mathbf U
+\left(g''+\frac{6g'}r\right)(\mathbf U\cdot\mathbf x)\mathbf x\\
&=\frac{3a}{2}\left[\frac{\mathbf U}{r^3}
-\frac{3(\mathbf U\cdot\mathbf x)\mathbf x}{r^5}\right]
=\frac1\mu\nabla p.
\end{aligned}
$$

To compute [surface traction in translating-sphere Stokes flow](../../../../surface-traction-in-translating-sphere-stokes-flow.md), let $\mathbf n=\mathbf x/a$ point from the sphere into the fluid. At the surface, $f'(a)=-3/(2a)$, $g'(a)=3/(2a^3)$ and $g(a)=0$. Hence

$$
\left.\partial_j u_i\right|_{a}
=\frac{3}{2a}\left[-U_i n_j+(\mathbf U\cdot\mathbf n)n_i n_j\right],\qquad
p(a)=\frac{3\mu}{2a}(\mathbf U\cdot\mathbf n).
$$

Substitute into the [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md). Its viscous contribution to the surface [traction](../../../../traction.md) is $3\mu[-\mathbf U+(\mathbf U\cdot\mathbf n)\mathbf n]/(2a)$, so the normal part cancels the [pressure](../../../../pressure-split.md) contribution:

$$
\boxed{\boldsymbol\sigma\mathbf n=-\frac{3\mu}{2a}\mathbf U.}
$$

The vector is constant over the entire sphere in the stated pressure gauge. Integrating it gives the fluid's [drag force](../../../../drag-physics.md) on the sphere,

$$
\boxed{\mathbf F_H=\int_{r=a}\boldsymbol\sigma\mathbf n\,dS
=-\frac{3\mu}{2a}(4\pi a^2)\mathbf U=-6\pi\mu a\mathbf U.}
$$

This is [Stokes's law](../../../../stokes-s-law.md). On an exterior fluid domain the outward domain normal at its inner boundary is $-\mathbf n$; that distinction will matter in the reciprocal calculation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
