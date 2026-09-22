<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $D=R_e-R_i$, $S=R_e+R_i$, $A=R_e^2-R_i^2=DS$, and $\Delta p=p_i-p_e$. [Incompressible flow](../../../../../../incompressible-flow.md) with [axial strain rate](../../../../../../axial-strain-rate.md) $E$ gives

$$
u_r=-\frac E2r+\frac{C(t)}r.
$$

Its radial [Stokes equation](../../../../../../stokes-equation.md) gives $p_r=0$, because $u_{r,rr}+u_{r,r}/r-u_r/r^2=0$. The radial [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) component is $\sigma_{rr}=-p-\mu E-2\mu C/r^2$. The outer and inner [Young–Laplace equation](../../../../../../young-laplace-equation.md) conditions have opposite curvature signs:

$$
\sigma_{rr}(R_e)=-p_e-\frac\gamma{R_e},\qquad
\sigma_{rr}(R_i)=-p_i+\frac\gamma{R_i}.
$$

Subtracting and eliminating $C$ gives

$$
\boxed{C=\frac{R_i^2R_e^2}{2\mu A}\left[\Delta p-\gamma\left(\frac1{R_i}+\frac1{R_e}\right)\right],\qquad
p=p_e-\frac{\Delta p R_i^2}{A}+\frac{\gamma S}{A}-\mu E.}
$$

In particular, the boxed [pressure](../../../../../../pressure.md) is equivalent to the printed identity for $(-p-\mu E)A$. For equal gas [pressures](../../../../../../pressure.md), $C=-\gamma R_iR_e/(2\mu D)$, so [surface tension](../../../../../../surface-tension.md) draws both interfaces inward in addition to the imposed extension.

The [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) is $\dot R_j=-ER_j/2+C/R_j$ at either interface. Taking the difference, and then the difference of squared radii, gives

$$
\boxed{\dot D=-\frac E2D+\frac\gamma{2\mu}-\frac{\Delta p R_iR_e}{2\mu S},\qquad
\dot A=-EA,\quad A(t)=A(0)e^{-Et}.}
$$

The cancellation of $C$ in the area equation is [mass conservation](../../../../../../mass-conservation.md): axial stretching reduces the liquid area while radial redistribution changes the hole size. For $E=0$, equal [pressures](../../../../../../pressure.md), and $R_i(0)=b$, $R_e(0)=2b$, one has $A=3b^2$ and $D=b+\gamma t/(2\mu)$. Since $S=A/D$,

$$
R_i=\frac12\left(\frac A D-D\right),\qquad
R_e=\frac12\left(\frac A D+D\right).
$$

Closure occurs at $D=\sqrt A=\sqrt3b$, so

$$
\boxed{t_*=\frac{2\mu b}{\gamma}(\sqrt3-1).}
$$

This [capillary collapse of an annular viscous cylinder](../../../../../../capillary-collapse-of-an-annular-viscous-cylinder.md) has finite closure time for $\gamma>0$ and $b>0$. For $\gamma=0$ it does not close in this case. The annular formula is used only up to closure; the singular cylindrical inner curvature is not a [boundary condition](../../../../../../boundary-condition.md) on the subsequent solid cylinder.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
