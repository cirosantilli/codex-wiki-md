<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The hydrostatic [buoyancy](../../../../../buoyancy.md) anomaly is $b'=f_0\psi_z$, and its leading adiabatic evolution is $D_gb'/Dt+N_0^2w=0$. The small vertical [velocity](../../../../../velocity.md) advects the background stratification; vertical advection of the perturbation [buoyancy](../../../../../buoyancy.md) is higher order. Consequently

$$
\boxed{w=-\frac{D_g}{Dt}\left(\frac{f_0}{N_0^2}\psi_z\right).}
$$

The [impermeability condition](../../../../../no-penetration-boundary-condition.md) at a stationary lower boundary $z=\alpha y$ is $w=\alpha v$. Using $v_g=\psi_x$ gives the [topographic buoyancy boundary condition for quasi-geostrophic flow](../../../../../topographic-buoyancy-boundary-condition-for-quasi-geostrophic-flow.md)

$$
\frac{D_g}{Dt}\left(\frac{f_0}{N_0^2}\psi_z\right)+\alpha\psi_x=0.
$$

For application at the reference plane, the actual small-height condition is $|\alpha|L/D\ll1$. Slopes scaled by $D/L$ are of Rossby-number order, so this topographic contribution is retained alongside the small ageostrophic vertical [velocity](../../../../../velocity.md). The dimensional slope should not be compared to the [Rossby number](../../../../../rossby-number.md) without also specifying the aspect ratio.

The basic [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) is $\overline\psi=-\Lambda zy$. It gives $U=\Lambda z$, basic [buoyancy](../../../../../buoyancy.md) gradient $\overline b_y=-f_0\Lambda$, and spatially constant interior [quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md). Linearizing its conservation law therefore gives

$$
\boxed{(\partial_t+\Lambda z\partial_x)q'=0,\qquad
q'=\psi'_{xx}+\psi'_{yy}+s\psi'_{zz},\quad s=f_0^2/N_0^2.}
$$

The printed equation omits the shear-advection term. This cannot be omitted for general disturbances: an interior anomaly proportional to $\cos[k(x-\Lambda zt)]$ is materially conserved but not independent of time at a fixed location. The intended zero-interior-PV [Eady model](../../../../../eady-model.md) modes do have $q'=0$ and satisfy both expressions; the ensuing mode calculation is valid in that subspace.

At either boundary, linearizing the geostrophic [material derivative](../../../../../material-derivative.md) includes $v'\overline\psi_{zy}=-\Lambda\psi'_x$. Let

$$
A_0=\Lambda-\frac{N_0^2\alpha}{f_0},\qquad
A_D=\Lambda-\frac{N_0^2\gamma}{f_0},\qquad
b_0=\psi'_z(0),\quad b_D=\psi'_z(D).
$$

The two boundary equations are

$$
\boxed{\partial_tb_0=A_0\psi'_x(0),\qquad
(\partial_t+\Lambda D\partial_x)b_D=A_D\psi'_x(D).}
$$

These are exactly the respective bottom and top slope corrections to the [rigid-boundary buoyancy condition for quasi-geostrophic waves](../../../../../rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves.md).

Assume periodicity horizontally and first consider $q'=0$. Multiply its defining equation by $\psi'_x$ and integrate over the layer. The two horizontal Laplacian terms vanish by [integration by parts](../../../../../integration-by-parts.md); the remaining volume term after one vertical integration is an $x$-derivative. Therefore

$$
0=\int\psi'_xq'\,dV
=s\int dx\,dy\,[\psi'_x\psi'_z]_{0}^{D}.
$$

For nonzero $A_0,A_D$, the boundary equations give

$$
\frac{d}{dt}\int\frac{b_0^2}{2f_0A_0}\,dx\,dy=\frac1{f_0}\int b_0\psi'_x(0)\,dx\,dy,
\qquad
\frac{d}{dt}\int\frac{b_D^2}{2f_0A_D}\,dx\,dy=\frac1{f_0}\int b_D\psi'_x(D)\,dx\,dy.
$$

The top advection term integrates to zero. Subtracting proves conservation of the [boundary pseudomomentum of a sloping Eady layer](../../../../../boundary-pseudomomentum-of-a-sloping-eady-layer.md):

$$
\boxed{\frac{d}{dt}\int dx\,dy\left[\frac{\psi_z'^2(D)}{2(\Lambda f_0-N_0^2\gamma)}-\frac{\psi_z'^2(0)}{2(\Lambda f_0-N_0^2\alpha)}\right]=0.}
$$

The original PDF uses squared vertical derivatives and the upper slope $\gamma$ in the first denominator; these details are corrupted in the converted TeX. For arbitrary nonzero interior PV the same calculation instead gives $d\mathcal P/dt=(f_0s)^{-1}\int\psi'_xq'\,dV$, which need not vanish. For example, at an instant take $\psi'=\cos kx+(z/D)^2\sin kx$, independent of $y$; the zonal average of $\psi'_xq'$ is $-ks/D^2$. Thus the boundary-only conservation statement also needs the zero-interior-PV qualification.

For an exponentially growing smooth [normal mode](../../../../../normal-mode.md), this qualification is automatic: the interior equation is $ik(\Lambda z-c)\widehat q=0$, and a [phase speed](../../../../../phase-speed.md) with nonzero [imaginary part](../../../../../imaginary-part.md) cannot equal the real basic [velocity](../../../../../velocity.md). Therefore $\widehat q=0$. If $A_0A_D<0$, the conserved boundary [quadratic form](../../../../../quadratic-form.md) is definite, so a nonzero exponentially growing boundary amplitude is impossible. Instability consequently requires

$$
\boxed{\left(1-\frac{N_0^2\gamma}{f_0\Lambda}\right)\left(1-\frac{N_0^2\alpha}{f_0\Lambda}\right)>0,}
$$

for $\Lambda\ne0$. When one $A$ vanishes, the corresponding boundary derivative is simply advected and must vanish for a growing mode. The other boundary then yields a real single-edge-wave speed; if both vanish, the zero-interior-PV Neumann problem has no nonzero growing mode. These degenerate cases are neutral and should not be handled by dividing by zero.

For equal slopes, put $\zeta=z/D$, $C=c/(\Lambda D)$, $M=N_0|k|D/|f_0|$, and $a=N_0^2\alpha/(f_0\Lambda)-1$. The normal-mode interior equation is $\Phi_{\zeta\zeta}-M^2\Phi=0$ for the zero-interior-PV modes. Thus

$$
\Phi=P\cosh(M\zeta)+Q\sinh(M\zeta),\qquad
(\zeta-C)\Phi_\zeta+a\Phi=0\quad\text{at }\zeta=0,1.
$$

The coefficient equations are

$$
aP-CMQ=0,
$$



$$
[(1-C)M\sinh M+a\cosh M]P+[(1-C)M\cosh M+a\sinh M]Q=0.
$$

Setting their determinant to zero, without dividing by $C$ or $a$, gives

$$
C(1-C)M\sinh M+a\cosh M+\frac{a^2}{M}\sinh M=0,
$$

so the [Eady model with parallel sloping boundaries](../../../../../eady-model-with-parallel-sloping-boundaries.md) has

$$
\boxed{C=\frac12\pm\sqrt{\frac14+a\frac{\coth M}{M}+\frac{a^2}{M^2}}.}
$$

For positive $k,f_0$, $M$ is the printed $\mu$, and $a$ is the printed $\widetilde\alpha$. The expression is even in the sign of that vertical scale. For $a\ge0$ the radicand is at least $1/4$, so both speeds are real and **these modes have no exponential growth**. For equal slopes the earlier necessary condition is merely $a^2>0$, which is satisfied in many stable cases and is not sufficient. At $a=0$ the speeds are $0$ and $\Lambda D$; the invariant with nonzero denominators cannot be used, but the determinant still correctly gives neutral modes. No claim excluding transient amplification is needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
