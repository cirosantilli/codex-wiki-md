<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work in the body frame and approximate the narrow annulus locally by a planar gap. Let $y=0$ be the cylindrical wall, moving at $-U$ in this frame, and $y=h(x)$ the stationary cell surface. The [red blood cell](../../../../../red-blood-cell.md) is represented by the given compliant body; the surrounding fluid is modeled as incompressible and Newtonian. Assume $h\ll a$, small local gap slope, and negligible inertia. The [lubrication](../../../../../lubrication-theory.md) equations are $p_y=0$ and $\mu w_{yy}=p_x$, with no-slip conditions $w(0)=-U$, $w(h)=0$. Integration gives

$$
w(y)=-U\left(1-\frac yh\right)+\frac{p_x}{2\mu}y(y-h).
$$

[Mass conservation](../../../../../mass-conservation.md) makes the body-frame flux constant. With the sign convention of the problem,

$$
\int_0^h w\,dy=-\frac{Uh}{2}-\frac{p_xh^3}{12\mu}=-Q,
$$

so the [lubrication model of a compliant translating plug](../../../../../lubrication-model-of-a-compliant-translating-plug.md) gives

$$
\boxed{p_x=-\frac{6\mu U}{h^2}+\frac{12\mu Q}{h^3}}.
$$

The circumferential multiplier is $2\pi a$ to leading order, giving the relative [volume flux](../../../../../volumetric-flow-rate.md) $-2\pi aQ$.

Let $p_d$ be the [pressure](../../../../../pressure.md) in front of the cell. Match the film to the reservoirs by $p(L)=p_d$ and $p(-L)=p_d+\Delta p$. Use $h=a-r$ and symmetric end matching for the parabolic-gap reduction. The elastic law gives

$$
\begin{aligned}
h(L)&=a-r_0(L)+(p_d-p_0)/\alpha,\\
h(-L)&=a-r_0(-L)+(p_d+\Delta p-p_0)/\alpha,
\end{aligned}
$$

For $r_0(-L)=r_0(L)$ this gives $h(-L)-h(L)=\Delta p/\alpha$. If the outer unstressed shape is not symmetric at the matching ends, the general relation instead includes $h(-L)-h(L)=\Delta p/\alpha-[r_0(-L)-r_0(L)]$. The proposed reduced end equation assumes the symmetric matching used here. The gap must remain positive. To determine the unknown flux and translating speed one also needs zero net axial [force](../../../../../force.md) on the freely moving body, and a specified absolute downstream [pressure](../../../../../pressure.md) relative to $p_0$, not merely a [pressure](../../../../../pressure.md) difference. If an external [force](../../../../../force.md) pulls the body, it must replace the force-free condition. The stated elasticity law fixes $p_0$; treating it as an unknown internal [pressure](../../../../../pressure.md) would require a further cell-volume constraint.

The force-free condition is most easily obtained from a [control volume](../../../../../control-volume.md) containing both body and surrounding film. The [pressure](../../../../../pressure.md) [force](../../../../../force.md) is $\pi a^2\Delta p$, and the resisting wall traction is $2\pi a\mu\int_{-L}^Lw_y(0)\,dx$. The local [velocity](../../../../../velocity.md) solution gives $w_y(0)=4U/h-6Q/h^2$, so

$$
\boxed{\Delta p=\frac{2\mu}{a}\int_{-L}^L\left(\frac{4U}{h}-\frac{6Q}{h^2}\right)dx}.
$$

This is the [force-free pressure drop of an annular lubrication plug](../../../../../force-free-pressure-drop-of-an-annular-lubrication-plug.md). It includes the film [pressure](../../../../../pressure.md) and shear contributions without separately approximating the deformed body's surface normal.

Put $s=2Q/U>0$, $\ell=\sqrt{s/\kappa}$, $h=sH$ and $x=\ell X$. The local parabolic elastic law is $p=p_0+\alpha[r_{00}-a-\kappa x^2/2+h]$, whence $p_x=\alpha\sqrt{\kappa s}(H_X-X)$. Substitution into the local lubrication equation gives

$$
\boxed{H_X+\lambda(H^{-2}-H^{-3})=X},\qquad\lambda=\frac{6\mu U}{\alpha\sqrt\kappa\,s^{5/2}}.
$$

The derivative is with respect to the scaled coordinate $X$; a derivative with respect to dimensional $x$ would be inconsistent with this nondimensional equation.

Let $C=s/a$ and $\widetilde L=L/\ell$. The elastic end condition gives $\Delta p=\alpha s[H(-\widetilde L)-H(\widetilde L)]$. Scaling the [force](../../../../../force.md) integral and eliminating $\Delta p$ then gives

$$
\boxed{H(-\widetilde L)-H(\widetilde L)=C\lambda\int_{-\widetilde L}^{\widetilde L}\left(\frac4{3H}-\frac1{H^2}\right)dX}.
$$

This completes the requested formulation and both dimensionless equations. The local parabolic approximation is used in the region contributing most strongly to the lubrication integrals; matching to the outer shape and reservoirs supplies the stated end conditions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
