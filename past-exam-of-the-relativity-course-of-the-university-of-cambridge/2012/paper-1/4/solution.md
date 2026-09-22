<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Put $f=1-2\mu/r$ and let dots now denote an [affine parameter](../../../../affine-parameter.md) [derivative](../../../../derivative.md). The [null geodesic](../../../../null-geodesic.md) [lagrangian](../../../../lagrangian.md) in the [orbital plane](../../../../orbital-plane.md) is $L=(fc^2\dot t^2-\dot r^2/f-r^2\dot\phi^2)/2$. The time and azimuthal [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) integrate once; the null normalization gives

$$
f\dot t=k,\qquad r^2\dot\phi=h,\qquad
fc^2\dot t^2-\dot r^2/f-r^2\dot\phi^2=0.
$$

For completeness, the differential radial [geodesic equation](../../../../geodesic-equation.md) is

$$
\ddot r+\frac{c^2ff'}2\dot t^2-\frac{f'}{2f}\dot r^2
-fr\dot\phi^2=0;
$$

the remaining differential equations are $\ddot t+(f'/f)\dot t\dot r=0$ and $\ddot\phi+2\dot r\dot\phi/r=0$. Spherical symmetry permits the equatorial choice.

Eliminating $\dot t,\dot\phi$ yields $\dot r^2+h^2f/r^2=c^2k^2$. For $h\ne0$, divide by $h^2$:

$$
\boxed{\frac{\dot r^2}{h^2}+V_{\rm eff}(r)=\frac1{b^2},\qquad
V_{\rm eff}=\frac1{r^2}-\frac{2\mu}{r^3},\qquad
b=\frac{|h|}{c|k|}.}
$$

The [impact parameter](../../../../impact-parameter.md) is unchanged by a common rescaling of the [affine parameter](../../../../affine-parameter.md). At infinity it is $c$ times [angular momentum](../../../../angular-momentum.md) divided by [energy](../../../../energy-split.md). Radial [photons](../../../../photon.md) have $h=0$ and obey the undivided equation $\dot r^2=c^2k^2$.

The [effective potential](../../../../effective-potential.md) is zero at $r=2\mu$, positive outside, and tends to zero as $r\to\infty$. Its [derivative](../../../../derivative.md) is $V'_{\rm eff}=2(3\mu-r)/r^4$. Thus

$$
\boxed{r_{\rm circ}=3\mu,\quad
V_{\rm eff}(3\mu)=\frac1{27\mu^2},\quad
b_{\rm crit}=3\sqrt3\,\mu.}
$$

The [circular null geodesic](../../../../circular-null-geodesic.md) lies at a maximum, since $V''_{\rm eff}(3\mu)=-2/(81\mu^4)<0$. It is **unstable**: a small radial displacement away from the maximum permits motion away from the orbit. For incoming [photons](../../../../photon.md) from infinity in the exterior of a [black hole](../../../../black-hole-split.md), an outer [turning point](../../../../turning-point.md) exists when $b>b_{\rm crit}$; for $b<b_{\rm crit}$ the [photon](../../../../photon.md) can cross the [event horizon](../../../../event-horizon.md). For a material central body, the [vacuum](../../../../vacuum.md) circular orbit is relevant only if $3\mu$ lies outside its surface.

<a id="4/image-photon-potential-and-horizon-penetrating-light-cones"></a>
![](../../../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2012/paper-1-photon-potential.png)

**[Figure 3](#4/image-photon-potential-and-horizon-penetrating-light-cones). Photon potential and horizon-penetrating light cones**.

For the new coordinates, set $q=2\mu/r$, so $f=1-q$. The [geodesic Lagrangian](../../../../geodesic-lagrangian.md) is $L'=[fc^2\dot t'^2-2qc\dot t'\dot r-(1+q)\dot r^2-r^2\dot\phi^2]/2$. Cyclic-coordinate conservation and the null condition give the required analogous equations:

$$
\boxed{\begin{aligned}
f\dot t'-\frac q c\dot r&=k,& r^2\dot\phi&=h,\\
fc^2\dot t'^2-2qc\dot t'\dot r
-(1+q)\dot r^2-r^2\dot\phi^2&=0.
\end{aligned}}
$$

Here $k$ denotes the same conserved time-translation quantity as before. The transformation is $t'=t+(2\mu/c)\log|r/(2\mu)-1|$. In particular, the displayed time coordinate belongs to [Ingoing Kerr-Schild coordinates for Schwarzschild spacetime](../../../../ingoing-kerr-schild-coordinates-for-schwarzschild-spacetime.md); the usual advanced null coordinate of [ingoing Eddington-Finkelstein coordinates](../../../../ingoing-eddington-finkelstein-coordinates.md) is $v=t'+r/c$. Using a [metric tensor](../../../../metric-tensor.md) with a vanishing $dr^2$ coefficient while retaining the name $t'$ would therefore solve a different coordinate representation.

An elimination that stays finite at the horizon is especially simple:

$$
\begin{aligned}
c^2k^2-\dot r^2
&=(fc\dot t'-q\dot r)^2-\dot r^2\\
&=f\left[fc^2\dot t'^2-2qc\dot t'\dot r
-(1+q)\dot r^2\right]\\
&=f r^2\dot\phi^2=\frac{fh^2}{r^2}.
\end{aligned}
$$

The middle equality uses $q^2+f(1+q)=1$. Hence **the radial [energy](../../../../energy-split.md) equation and $V_{\rm eff}(r)$ are unchanged**, including the horizon limit. The radial [metric tensor](../../../../metric-tensor.md) block has [determinant](../../../../determinant.md) $-c^2$ and is regular at $r=2\mu$. Its radial null directions are $dr/(c\,dt')=-1$ and $dr/(c\,dt')=f/(1+q)$, as shown in the original schematic.

This [coordinate invariance of the Schwarzschild photon radial potential](../../../../coordinate-invariance-of-the-schwarzschild-photon-radial-potential.md) follows because the transformation changes the time slicing but preserves the [areal radius](../../../../areal-radius.md) and the stationary [Killing vector field](../../../../killing-vector-field-split.md) $\partial_{t'}=\partial_t$. Consequently the conserved [Killing energy](../../../../killing-energy.md), [angular momentum](../../../../angular-momentum.md) and [impact parameter](../../../../impact-parameter.md) are the same. [photon](../../../../photon.md) capture, the circular orbit and the radial [turning points](../../../../turning-point.md) cannot depend on coordinate labels; coordinate velocities can.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
