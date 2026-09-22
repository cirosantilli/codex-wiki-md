<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $G=g'$ for the positive [reduced gravity](../../../../../reduced-gravity-split.md) of dense fluid. With $z$ upwards, $G_z>0$ places denser fluid above lighter fluid and permits convective [turbulence](../../../../../turbulence-split.md). A displacement over the radius scale $d$ samples a buoyancy difference of order $dG_z$; balancing kinetic energy per mass with buoyant work over $d$ gives

$$
\boxed{u\sim d\sqrt{G_z}}.
$$

The [buoyancy-gradient mixing-length closure](../../../../../buoyancy-gradient-mixing-length-closure.md) then gives an [eddy diffusivity](../../../../../eddy-diffusivity.md) $K\sim ud=d^2\sqrt{G_z}$. We use the paper's unit-prefactor convention for this dimensional closure and its effective cross-sectional area $d^2$; order-one mixing constants and the cylinder's geometric factor $\pi$ are suppressed in its displayed evolution equation.

The downward reduced-gravity transport magnitude and its convergence are different quantities:

$$
\boxed{\mathcal F=d^2KG_z=d^4(G_z)^{3/2},\qquad
F_{\rm conv}=\frac{d\mathcal F}{dz}
=d^2\frac d{dz}\left[d^2(G_z)^{3/2}\right]}.
$$

The printed expression labelled a flux is actually the second quantity, a flux convergence per unit height. The dimensions distinguish them: $\mathcal F$ has units $L^4T^{-3}$, whereas $F_{\rm conv}$ has units $L^3T^{-3}$. A constant positive gradient has nonzero transport but zero convergence, providing a direct counterexample to identifying the derivative with the transport itself.

The upward total [buoyancy flux](../../../../../buoyancy-flux.md) is $QG-\mathcal F$. Conservation therefore yields

$$
\boxed{d^2G_t+QG_z=d^4\partial_z[(G_z)^{3/2}]}.
$$

This [flux convergence in turbulent buoyancy mixing](../../../../../flux-convergence-in-turbulent-buoyancy-mixing.md) obtains the displayed evolution equation with the correct transport interpretation.

For the [arrested cubic buoyancy profile](../../../../../arrested-cubic-buoyancy-profile.md), an undisturbed region below $-H$ has $G=0$ and no turbulent [buoyancy flux](../../../../../buoyancy-flux.md). The joining condition is $G(-H)=0$ and

$$
\boxed{G_z(-H)=0}.
$$

In a steady state, integrating the conservation equation from that front gives $QG=d^4(G_z)^{3/2}$. For a nonzero mixed region,

$$
\frac{d}{dz}G^{1/3}=\frac13\left(\frac Q{d^4}\right)^{2/3},
$$

and hence

$$
\boxed{G(z)=\frac{Q^2}{27d^8}(z+H)^3\quad(-H<z<0),\qquad G=0\quad(z\leq-H)}.
$$

The associated gradient is $Q^2(z+H)^2/(9d^8)$, so it matches the required zero-gradient state continuously. We take the mixed interval to start immediately above $-H$; adding a further zero interval would merely relocate the arrest front.

The source [buoyancy flux](../../../../../buoyancy-flux.md) is $B_s=Q_sg_s'$, with $g_s'=g\Delta\rho/\rho$ in the [Boussinesq approximation](../../../../../boussinesq-approximation.md). The stated top-source convention means that this entire flux enters the downward turbulent transport there: $\mathcal F(0)=B_s$. Since steady transport also satisfies $\mathcal F(0)=QG(0)$,

$$
\boxed{H=\frac{3d^{8/3}(Q_sg_s')^{1/3}}Q,\qquad G(0)=\frac{Q_sg_s'}Q}.
$$

This is the extent in the paper's dimensional-closure normalization. It presupposes positive $Q$; with no upflow there is no finite steady arrest depth. For a mixture of the two original fluids, $G(0)\leq g_s'$ is necessary, so an extrapolation to $Q_s/Q>1$ cannot represent a physical [concentration](../../../../../concentration.md) profile under this top-flux boundary model. A dilute-source regime avoids appreciable source-volume corrections.

Assuming the same scalar-mixing coefficient for a passive tracer, its [eddy diffusivity](../../../../../eddy-diffusivity.md) in the mixed region is

$$
\boxed{K(z)=d^2\sqrt{G_z}=\frac{Q(z+H)}{3d^2}}.
$$

It vanishes at the arrest front and increases linearly towards the source. A different turbulent scalar diffusivity ratio would multiply this result by its corresponding constant.

The geometric normalization can be restored without changing the reasoning. With actual area $S=\pi d^2$ and $K=C_m d^2\sqrt{G_z}$, put $R=SC_md^2$. Then $G=Q^2(z+H)^3/(27R^2)$, $H=3R^{2/3}B_s^{1/3}/Q$, and $K=Q(z+H)/(3S)$. These formulas show which numerical prefactors are convention-dependent.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
