<h1 id="37a/solution">Solution</h1>

↑ **Parent:** [37A](../37a.md)

The [lubrication approximation](../../../../../lubrication-theory.md) applies in a gap thin compared with its horizontal scale, with small slopes, no slip at the walls, negligible inertia, and approximately constant pressure across the gap. Continuity makes the horizontal velocity much larger than the normal velocity. At $t=0$, write $h(x)=h_0+\delta x/L$, where $\delta=\Delta h$ and $|\delta|<h_0$ keeps the gap open.

The horizontal [Stokes equation](../../../../../stokes-equation.md) becomes $\mu u_{yy}=p_x$. Both plates have zero horizontal velocity, so

$$
u=\frac{p_x}{2\mu}y(y-h),\qquad
\boxed{Q(x)=\int_0^hu\,dy=-\frac{h^3}{12\mu}p_x}.
$$

Integrated incompressibility with the moving upper wall gives $h_t+Q_x=0$. Since $h_t=-V$, $Q_x=V$, and $Q(x)=Vx+C$, giving $Q(L)-Q(-L)=2VL$.

Equal end pressures impose $\int_{-L}^L(Vx+C)/h^3\,dx=0$. The two elementary integrals are

$$
\int_{-L}^L\frac{dx}{h^3}=\frac{2Lh_0}{(h_0^2-\delta^2)^2},\qquad
\int_{-L}^L\frac{x\,dx}{h^3}=-\frac{2L^2\delta}{(h_0^2-\delta^2)^2}.
$$

Hence $C=VL\delta/h_0$. In endpoint form this pressure condition is $(h_0-\delta)Q(L)+(h_0+\delta)Q(-L)=0$. Combining it with the flux difference gives

$$
\boxed{Q(\pm L)=VL(\delta/h_0\pm1)}.
$$

The limits $\delta=0$ recover equal outward fluxes.

The horizontal velocity scale is $U\sim VL/h_0$. The ratio of convective inertia $\rho U^2/L$ to viscous force $\mu U/h_0^2$ is $\rho Vh_0/\mu$; the unsteady term on time scale $h_0/V$ has the same ratio. Therefore, alongside $h_0/L\ll1$, the required condition is **$\boxed{V\ll\mu/(\rho h_0)}$.**

## ↑ Ancestors (10)

1. [37A](../37a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
