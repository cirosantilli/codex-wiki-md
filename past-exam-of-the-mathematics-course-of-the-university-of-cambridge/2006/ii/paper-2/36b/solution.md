<h1 id="36b/solution">Solution</h1>

↑ **Parent:** [36B](../36b.md)

In the lubrication regime the thin region has longitudinal scale $\ell\sim\sqrt{ab}$, since the height increase $x^2/(2a)$ becomes comparable with $b$ there. The characteristic shear is $\mu V/b$, so force per axial length scales as $\mu V\ell/b\sim\mu V\sqrt{a/b}$. Negligible inertia, no slip, no cylinder rotation, and full wetting are understood.

Use a frame translating with the cylinder. The wall moves with [velocity](../../../../../velocity.md) $-V$, the cylinder is stationary, and the gap is $h(x)=b+x^2/(2a)$. Lubrication momentum gives $\mu u_{yy}=p_x$, $p_y=0$, so

$$
u_{\rm frame}=-V(1-y/h)+\frac{p_x}{2\mu}y(y-h),\qquad q=-\frac{Vh}{2}-\frac{h^3p_x}{12\mu}.
$$

Continuity makes $q$ constant. Equal ambient [pressures](../../../../../pressure.md) at both infinities give $\int p_xdx=0$, hence $q=-(V/2)(\int h^{-2}dx)/(\int h^{-3}dx)=-2Vb/3$. Therefore

$$
\boxed{p_x=\frac{2\mu V(4b-3h)}{h^3},\qquad p=\frac{2\mu Vx}{h^2},\qquad u_{\rm lab}=\frac{Vy}{h}+\frac{p_x}{2\mu}y(y-h).}
$$

The [vertical velocity](../../../../../vertical-velocity.md), with the wall condition $w(0)=0$, follows explicitly from incompressibility:

$$
w=\frac{Vh'y^2}{2h^2}-\frac{p_{xx}}{2\mu}\left(\frac{y^3}{3}-\frac{hy^2}{2}\right)+\frac{p_xh'y^2}{4\mu}.
$$

It gives $w(h)=0$, consistently with a horizontally translating cylinder in the lab frame.

The wall shear is $\mu u_y(0)=4\mu V(1/h-b/h^2)$. With $x=\sqrt{2ab}\,s$, its integral is

$$
F=4\mu V\sqrt{2ab}\left(\frac\pi b-\frac\pi{2b}\right),\qquad\boxed{F\sim2\pi\mu V\sqrt{\frac{2a}{b}}\quad(b/a\to0).}
$$

[Force balance](../../../../../force-balance.md) equates this wall force to the required cylinder force at leading order; the [pressure](../../../../../pressure.md) and [viscous stresses](../../../../../viscous-stress-tensor.md) on remote boundaries make no leading contribution. This is the [cylinder translating parallel to a wall in a thin gap](../../../../../cylinder-translating-parallel-to-a-wall-in-a-thin-gap.md) result. The asymptotic sign denotes the approximation implicit in the parabolic gap, rather than an exact finite-gap cylinder formula.

## ↑ Ancestors (10)

1. [36B](../36b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
