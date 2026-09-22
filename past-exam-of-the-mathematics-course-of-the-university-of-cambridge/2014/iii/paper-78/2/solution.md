<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose $U$ and $Q$ as the speed and source strength in the same kinematic velocity convention. With $r=(x^2+y^2)^{1/2}$ and $\vartheta=\arg(x+iy)$, [superposition](../../../../../superposition-principle.md) of uniform [potential flow](../../../../../potential-flow.md) and a two-dimensional [point source](../../../../../point-source.md) gives

$$
\boxed{\Phi=Ux+\frac{Q}{2\pi}\log r,\qquad
\psi=Uy+\frac{Q}{2\pi}\vartheta,}
$$

where $(u,v)=\nabla\Phi=(\psi_y,-\psi_x)$. The angular branch cut records the [volume flux](../../../../../volumetric-flow-rate.md) from the source; the logarithm's arbitrary reference length only changes an additive constant in the [velocity potential](../../../../../velocity-potential.md).

The [stagnation point](../../../../../stagnation-point.md) lies on the negative axis, where $u=U+Q/(2\pi x)=0$. Thus the limiting upstream reach of source fluid is

$$
\boxed{x_s=-\frac{Q}{2\pi U}=-\frac b\pi,\qquad b=\frac{Q}{2U}.}
$$

The stagnation point is approached asymptotically, rather than reached in finite time by a parcel on the upstream axis. The dividing [streamlines](../../../../../streamline.md) through it have $\psi=\pm Q/2$ when the angle is taken in $(-\pi,\pi)$. Far downstream $\vartheta\to0$, so these [streamlines](../../../../../streamline.md) approach $y=\pm Q/(2U)$. Consequently the source fluid occupies the [Rankine half-body](../../../../../rankine-half-body.md) between them, with downstream width $2b=Q/U$. In the upper half-plane its boundary can also be parametrized by $y=b(1-\vartheta/\pi)$, $x=y\cot\vartheta$, $0<\vartheta<\pi$.

For arrival at the downstream axis, the direct streamline $y=0$, $x>0$ has speed $U+Q/(2\pi x)$. Its transit time from the ideal point source is

$$
T_s(x)=\int_0^x\frac{dX}{U+Q/(2\pi X)}
=\frac xU-\frac{Q}{2\pi U^2}\log\left(1+\frac{2\pi Ux}{Q}\right).
$$

The first source fluid at a downstream cross-section lies on this symmetry axis: for positive $x$, the horizontal source contribution $Qx/[2\pi(x^2+y^2)]$ is maximal at $y=0$, and off-axis paths cannot advance through positive $x$ more quickly. A far-away parcel passing the inlet line at the same release time has transit time $x/U$. The time advance is therefore

$$
\boxed{\tau=\frac xU-T_s(x)=\frac b{\pi U}\log\left(1+\frac{\pi x}{b}\right).}
$$

This is an advance, not the source parcel's absolute transit time. If a source parcel is released at time $t_0$ while the distant comparison parcel crosses $x=0$ at time zero, the advance relative to that parcel is $\tau-t_0$; the printed formula uses simultaneous releases. If $U,Q$ instead denote [Darcy velocity](../../../../../darcy-velocity.md) and bulk-area source flux in a medium of uniform [porosity](../../../../../porosity.md) $\phi$, their ratio still gives the same $b$, but both parcel times acquire a factor $\phi$. No [porosity](../../../../../porosity.md) is specified here, so the displayed time formula fixes the kinematic convention.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
