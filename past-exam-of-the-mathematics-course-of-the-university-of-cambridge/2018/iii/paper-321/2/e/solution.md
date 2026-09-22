<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

At fixed [cylindrical radius](../../../../../../cylindrical-radius.md), let $w=u_z$ and use the [continuity equation](../../../../../../continuity-equation.md) $\partial_t\rho+\partial_z(\rho w)=0$. For the [similarity solution](../../../../../../similarity-solution.md) $z=\xi\eta(t)$ and $\rho=\widetilde\rho(\xi)/\eta$, the [continuity equation](../../../../../../continuity-equation.md) reduces to

$$
\partial_\xi\left[\widetilde\rho(w-\dot\eta\xi)\right]=0.
$$

Here $\eta$ is dimensionless and $\xi$ labels the initial height. Midplane symmetry sets the integration constant to zero, so the flow is a [homologous vertical motion of an astrophysical disk](../../../../../../homologous-vertical-motion-of-an-astrophysical-disk.md):

$$
w=\dot\eta\xi=\frac{\dot\eta}{\eta}z,\qquad
\partial_z=\eta^{-1}\partial_\xi,\qquad
\left.\partial_t\right|_z=\left.\partial_t\right|_\xi-\frac{\dot\eta}{\eta}\xi\partial_\xi,\qquad
D_t=\left.\partial_t\right|_\xi.
$$

The [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) and [ideal gas](../../../../../../ideal-gas.md) law become

$$
\frac{d\widetilde P}{d\xi}=-\Omega^2\xi\widetilde\rho,\qquad
\widetilde P=\mathcal R\widetilde\rho\widetilde T.
$$

The [material derivatives](../../../../../../material-derivative.md) are $D_tP=\widetilde P\dot\eta$ and $D_t\rho=-\widetilde\rho\dot\eta/\eta^2$, so the energy equation gives

$$
\frac{\gamma+1}{\gamma-1}\widetilde P\dot\eta=-A\widetilde T^{1+\beta}\eta^{2+2\beta}.
$$

[Separation of variables](../../../../../../separation-of-variables.md) requires a positive constant $K$ such that

$$
\dot\eta=-K\eta^{2+2\beta},\qquad
\widetilde P=\frac{(\gamma-1)A}{(\gamma+1)K}\widetilde T^{1+\beta}.
$$

Integrating with $\eta(0)=1$ gives the [slow cooling of an astrophysical disk](../../../../../../slow-cooling-of-an-astrophysical-disk.md) similarity factor

$$
\boxed{\eta(t)=(1+Ct)^{-1/(1+2\beta)},\qquad C=(1+2\beta)K>0.}
$$

A closed set of profile equations is therefore

$$
\boxed{\widetilde P'=-\Omega^2\xi\widetilde\rho,\qquad
\widetilde P=\mathcal R\widetilde\rho\widetilde T,\qquad
\widetilde P=\frac{(\gamma-1)(1+2\beta)A}{(\gamma+1)C}\widetilde T^{1+\beta}.}
$$

These have the same [polytropic vertical structure in stellar gravity](../../../../../../polytropic-vertical-structure-in-stellar-gravity.md) as part (b). Writing

$$
H_0^2=\frac{2(1+\beta)\mathcal R T_0}{\Omega^2},\qquad
\widetilde T=T_0\left(1-\frac{\xi^2}{H_0^2}\right),\qquad
\widetilde\rho=\rho_0\left(1-\frac{\xi^2}{H_0^2}\right)^\beta,\qquad
\widetilde P=P_0\left(1-\frac{\xi^2}{H_0^2}\right)^{1+\beta},
$$

with $P_0=\mathcal R\rho_0T_0$, fixes

$$
C=\frac{(\gamma-1)(1+2\beta)A T_0^{1+\beta}}{(\gamma+1)P_0}.
$$

Returning to physical height, the explicit profiles and evolving semi-thickness for $|z|\leq H(t)$ are

$$
\boxed{H(t)=H_0(1+Ct)^{-1/(1+2\beta)},\qquad
T(z,t)=\frac{\Omega^2}{2(1+\beta)\mathcal R}\left[H(t)^2-z^2\right],}
$$

and

$$
\rho(z,t)=\frac{\rho_0}{\eta(t)}\left[1-\frac{z^2}{H(t)^2}\right]^\beta,\qquad
P(z,t)=P_0\eta(t)\left[1-\frac{z^2}{H(t)^2}\right]^{1+\beta}.
$$

Outside this moving surface $\rho=P=0$. The [surface density of a disk](../../../../../../surface-density-of-a-disk.md) is conserved because $\rho\,dz=\widetilde\rho\,d\xi$. The column **cools and contracts without changing its scaled profile**: its midplane [temperature](../../../../../../temperature.md) falls as $\eta^2$, its [mass density](../../../../../../density.md) rises as $\eta^{-1}$ and its [pressure](../../../../../../pressure.md) falls as $\eta$.

The value $T_0$ determines $H_0$, but the [mass density](../../../../../../density.md) normalization also enters $C$. If the initial column is specifically the heated equilibrium of part (b), switching off its heating gives

$$
C=\frac{9\alpha\Omega}{4}\frac{(\gamma-1)(1+2\beta)}{\gamma+1}.
$$

Otherwise $P_0$, or equivalently the conserved column mass, is additional initial data. The contraction timescale grows with $1+Ct$, so sufficiently slow initial evolution remains slow relative to the fixed [vertical dynamical timescale of a disk](../../../../../../vertical-dynamical-timescale-of-a-disk.md). This is an exact solution of the reduced [hydrostatic approximation](../../../../../../hydrostatic-approximation.md), rather than the full momentum equation: its omitted vertical acceleration is $\ddot\eta\xi$, with $\ddot\eta/(\eta\Omega^2)=2(1+\beta)C^2/[(1+2\beta)^2\Omega^2(1+Ct)^2]$, which remains small and decreases if $C\ll\Omega$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
