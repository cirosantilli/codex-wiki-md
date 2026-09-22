<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Full equations and the balanced scaling.** Let $H=h_{00}$, free-surface displacement $\eta$ and layer thickness $h=H+\eta-b$. The inviscid rotating [shallow water equations](../../../../../shallow-water-equations.md) are

$$
\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u+f\widehat z\times\mathbf u=-g\nabla\eta,\qquad
\partial_t h+\nabla\cdot(h\mathbf u)=0.
$$

Here gradients are horizontal and $b$ is a fixed bottom height. For horizontal scales $L$, velocities $V$ and time scale $L/V$, acceleration is $V^2/L$, whereas the Coriolis term is $|f|V$. A small [Rossby number](../../../../../rossby-number.md) $\mathrm{Ro}=V/(|f|L)$ therefore gives leading [geostrophic balance](../../../../../geostrophic-balance.md). Define

$$
\psi=\frac g f\eta,\qquad(u_g,v_g)=(-\psi_y,\psi_x),\qquad
L_R=\frac{\sqrt{gH}}{|f|}.
$$

The last length is the [Rossby deformation radius](../../../../../rossby-deformation-radius.md). Geostrophy gives $\eta\sim |f|VL/g$ and consequently

$$
\frac{\eta}{H}\sim\mathrm{Ro}\frac{L^2}{L_R^2}.
$$

The usual distinguished quasi-geostrophic limit takes the [Burger number](../../../../../burger-number.md) $L_R^2/L^2$ of order one, small surface displacement, and bottom amplitude $b/H=O(\mathrm{Ro})$. The ageostrophic velocity is smaller than the geostrophic velocity by a factor of order $\mathrm{Ro}$, but its small divergence supplies the first nonzero thickness tendency. Motions are slow compared with $|f|^{-1}$, and the shallow-layer approximation also requires depth small compared with horizontal scale. Other deformation-radius limits are possible only if the small-height condition is retained.

Taking the vertical curl and combining it with thickness continuity gives exact [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) conservation,

$$
\frac D{Dt}\left(\frac{f+\zeta}{h}\right)=0,\qquad\zeta=v_x-u_y.
$$

Expand to first order in relative [vorticity](../../../../../vorticity.md), displacement and relief; multiplication by $H$ removes the irrelevant constant depth factor. To quasi-geostrophic accuracy,

$$
Q=f+\nabla^2\psi-\frac{\psi}{L_R^2}+\frac{fb}{H},\qquad
\boxed{\partial_tQ+J(\psi,Q)=0},\qquad J(A,B)=A_xB_y-A_yB_x.
$$

[Potential-vorticity conservation](../../../../../potential-vorticity-conservation.md) transports this scalar with the geostrophic flow. [Potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) solves the elliptic problem

$$
(\nabla^2-L_R^{-2})\psi=Q-f-fb/H
$$

with the required boundary or far-field conditions, then differentiates $\psi$ to recover velocity and surface height. The deformation term suppresses the far-field influence over distances comparable with $L_R$; at scales much shorter than $L_R$ the inversion approaches the two-dimensional Poisson problem.

The full shallow-water system evolves two velocity components and layer thickness independently, with three first-order time equations. The quasi-geostrophic system evolves one scalar; balanced velocity and height are diagnostic consequences of inversion. In particular it filters the two fast inertia–gravity branches, whose resting-layer dispersion is $\omega^2=f^2+gH|\mathbf k|^2$, and does not describe their fast [geostrophic adjustment](../../../../../geostrophic-adjustment.md). Reducing the time order restricts admissible initial data; it does not turn an arbitrary full shallow-water state into a quasi-geostrophic state automatically.

**The intended Gaussian inversion, and its required background qualification.** Set $r^2=x^2+y^2$ and $\psi'=Ae^{-r^2/a^2}$. Direct differentiation gives

$$
(\nabla^2-L_R^{-2})\psi'
=-\frac A{a^2}\left[4\left(1-\frac{r^2}{a^2}\right)+\frac{a^2}{L_R^2}\right]e^{-r^2/a^2}.
$$

Consequently, in an inversion with uniform PV and its background gradient explicitly compensated, the printed relief is balanced by

$$
\boxed{A=\frac{f\epsilon a^2}{H},\qquad\psi'=\frac{f\epsilon a^2}{H}e^{-r^2/a^2}.}
$$

This is the [Gaussian topographic response with compensated uniform potential vorticity](../../../../../gaussian-topographic-response-with-compensated-uniform-potential-vorticity.md). In that model the perturbation PV is identically zero, and any steady velocity field advects this uniform PV trivially.

There is a genuine [uniform-current obstruction to constant shallow-water QG potential vorticity](../../../../../uniform-current-obstruction-to-constant-shallow-water-qg-potential-vorticity.md) in the literal constant-$f$, finite-$L_R$ formulation. A geostrophic background current $(U,0)$ has total [streamfunction](../../../../../stream-function.md) $\Psi=-Uy+\psi'$ and a background free-surface slope. Over flat bottom its PV is $\overline Q=f+Uy/L_R^2$, not uniform. For the displayed Gaussian and printed relief, the two disturbance terms cancel in inversion but leave

$$
Q=f+Uy/L_R^2,\qquad J(\Psi,Q)=\frac U{L_R^2}\psi'_x.
$$

For $U\epsilon\ne0$ and finite $L_R$ this residual is nonzero; for example, it is nonzero at $x=a/\sqrt2,y=0$. Thus the claimed Gaussian is not a steady solution of the standard unforced constant-$f$ equations as literally stated. Omitting the mean contribution to the stretching term is not a legitimate gauge choice.

A precise intended repair is to supply a background PV gradient $-Uy/L_R^2$ from an explicitly compensating weak bottom slope or beta-plane background, so the current really does have uniform PV. Another repair is the rigid-lid limit $L_R\to\infty$. In the uncompensated finite-$L_R$ current model, a Gaussian can instead solve steady equations if the $a^2/L_R^2$ term is removed from the relief: then $\nabla^2\psi'+fb/H=0$ and $Q=f-\Psi/L_R^2$, so $J(\Psi,Q)=0$. Its PV is not uniform. These repairs distinguish the intended calculation from the false literal claim.

**Smallness and closed streamlines of the intended response.** Its maximum disturbance speed is

$$
V'_{\max}=\max|\nabla\psi'|=\sqrt{2/e}\frac{|A|}{a}
=\sqrt{2/e}\frac{|f\epsilon|a}{H}.
$$

Its relative [vorticity](../../../../../vorticity.md) is of order $|f\epsilon|/H$, and its surface displacement has maximum $|\eta'|=|\epsilon|a^2/L_R^2$. The relief satisfies $|b|\le |\epsilon|(4+a^2/L_R^2)$. Sufficient conditions for quasi-geostrophic consistency are therefore

$$
\frac{|U|}{|f|a}\ll1,\qquad
\frac{|U|}{|f|a}\frac{a^2}{L_R^2}\ll1,\qquad
\boxed{\frac{|\epsilon|}{H}\left(1+\frac{a^2}{L_R^2}\right)\ll1.}
$$

The second condition limits the background geostrophic height change across the disturbance scale. The last controls disturbance [Rossby number](../../../../../rossby-number.md), surface height and bottom relief, including positive layer depth. For $a$ comparable with $L_R$ it reduces to $|\epsilon|\ll H$. It does not require disturbance velocity to be small relative to $U$.

Take $U>0$ without loss of horizontal orientation. The total [streamfunction](../../../../../stream-function.md) is $\Psi=-Uy+Ae^{-r^2/a^2}$, with

$$
u=U+\frac{2Ay}{a^2}e^{-r^2/a^2},\qquad v=-\frac{2Ax}{a^2}e^{-r^2/a^2}.
$$

If $\sqrt{2/e}|A|/a<U$, then $u>0$ everywhere and no streamline can close. In terms of the relief amplitude,

$$
\boxed{|\epsilon|<\sqrt{e/2}\frac{|U|H}{|f|a}}
$$

is the strict no-closed-cell condition. Above this [closed-streamline threshold for a Gaussian disturbance in uniform flow](../../../../../closed-streamline-threshold-for-a-gaussian-disturbance-in-uniform-flow.md), stagnation points occur at $x=0$ on the side opposing the current. The equation $|y|e^{-y^2/a^2}=|U|a^2/(2|A|)$ has two roots: the inner one is a center because both Hessian eigenvalues of $\Psi$ have the same sign; the outer one is a saddle. Closed contours surround the center and are bounded by a separatrix. Equality gives a degenerate onset, with no finite-area closed cell yet. If $U=0$, every nontrivial Gaussian response instead has circular closed streamlines.

Closed streamlines are compatible with small [Rossby number](../../../../../rossby-number.md): their threshold can be reached with $|\epsilon|/H$ of order the already small background [Rossby number](../../../../../rossby-number.md). They do not alone invalidate quasi-geostrophy. They do, however, disconnect the cell from upstream PV data. If only the upstream PV is specified, the PV in such a cell depends on its formation history and cannot generally be assigned from the upstream value alone. Globally uniform initial PV would remain uniform in the ideal compensated model, but mixing, dissipation and forcing history can select a different physical trapped circulation. These qualifications are separate from the constant-$f$ inconsistency demonstrated above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
