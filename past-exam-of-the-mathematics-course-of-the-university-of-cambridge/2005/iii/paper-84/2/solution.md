<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\rho_r$ be a constant reference density close to the ambient density, and let $\rho_p$ denote the mean plume density. The [Boussinesq approximation](../../../../../boussinesq-approximation.md) permits full-cross-section kinematic fluxes

$$
\boxed{Q=\int_Aw\,dA,\qquad M=\int_Aw^2dA,\qquad
F=\int_A b w\,dA,\quad b=g\frac{\rho_a(z)-\rho_p}{\rho_r}.}
$$

Thus $Q$ is the specific [mass flux](../../../../../mass-flux.md), equal to [volume flux](../../../../../volumetric-flow-rate.md) at this order; $M$ is the specific vertical [momentum flux](../../../../../momentum-flux.md); and $F$ is the [buoyancy flux](../../../../../buoyancy-flux.md). Physical mass and momentum fluxes are $\rho_rQ$ and $\rho_rM$. These definitions include the full circular area. If factors of $\pi$ are removed in a course's flux convention, divide $Q,M,F$ by $\pi$ throughout rather than mixing normalizations. The PDF's source density is $\rho_0$, distinct from ambient $\rho_a(z)$; the TeX changes the source symbol incorrectly.

For the [top-hat plume model](../../../../../top-hat-plume-model.md), let the plume radius be $r(z)$ and let $w,b$ be uniform inside it. Then

$$
Q=\pi r^2w,\qquad M=\pi r^2w^2,\qquad F=\pi r^2wb,
\qquad w=\frac MQ,\quad r=\frac Q{\sqrt{\pi M}}.
$$

The [Batchelor entrainment hypothesis](../../../../../batchelor-entrainment-hypothesis.md) supplies the necessary closure: the inward edge velocity is $v_e=\alpha_e w$, with constant [entrainment coefficient](../../../../../entrainment-coefficient.md) $\alpha_e>0$. Entrainment across a cylindrical slice gives $Q'=2\pi r\alpha_ew=2\alpha_e\sqrt\pi\sqrt M$. The entrained ambient has negligible upward momentum. The vertical buoyancy force on the slice is $\pi r^2b=F/w$, hence $M'=FQ/M$.

For the buoyancy balance, let $R=\int_A\rho_pw\,dA$ be the transported density scalar. Entrainment gives $R'=\rho_aQ'$. Differentiate $F=g(\rho_aQ-R)/\rho_r$ to get $F'=g\rho_a'Q/\rho_r$. Therefore the **closed flux equations** are

$$
\boxed{Q'=c\sqrt M,\qquad M'=\frac{FQ}{M},\qquad F'=-N^2Q,
\quad c=2\alpha_e\sqrt\pi,\quad N^2=-\frac g{\rho_r}\rho_a'.}
$$

Here $N$ is the [buoyancy frequency](../../../../../buoyancy-frequency.md) when the ambient is stably stratified. These are the [Boussinesq top-hat plume in a stratified ambient](../../../../../boussinesq-top-hat-plume-in-a-stratified-ambient.md) equations in the explicitly stated full-area convention. Stable stratification consumes positive buoyancy flux as the plume rises. The top-hat assumption alone would not determine $Q'$ without an [entrainment](../../../../../fluid-entrainment.md) law.

For uniform ambient density, $F=F_0$ is constant. The source volume $Q_0$ becomes negligible when accumulated entrainment $\int_0^zc\sqrt{M(s)}ds$ is much greater than $Q_0$. In a jet-like region, $M\simeq M_0$, so the criterion is $z\gg Q_0/(c\sqrt{M_0})$. In a buoyancy-dominated far field with $Q\simeq C_Qz^{5/3}$, it is $z\gg(Q_0/C_Q)^{3/5}$, with $C_Q$ determined below. These are the two [source-volume lengths of a turbulent plume](../../../../../source-volume-length-of-a-turbulent-plume.md). They are not the [jet length](../../../../../jet-length.md), which measures the persistence of imposed source momentum. A nonzero source volume can also appear as a [plume virtual origin](../../../../../plume-virtual-origin.md); it is not valid to discard it at every distance simply because the source is geometrically small.

For $Q_0=M_0=0$, $F_0>0$, seek $Q=C_Qz^{5/3}$, $M=C_Mz^{4/3}$. The two flux equations give $C_Q=(3c/5)\sqrt{C_M}$ and $C_M^{3/2}=9cF_0/20$. Thus the **pure-plume solution** is

$$
\boxed{F=F_0,\qquad
M=\left(\frac{9cF_0}{20}\right)^{2/3}z^{4/3},\qquad
Q=\frac{3c}{5}\left(\frac{9cF_0}{20}\right)^{1/3}z^{5/3}.}
$$

For completeness its directly measurable top-hat fields are

$$
r=\frac{6\alpha_e}{5}z,\qquad
w=K_pz^{-1/3},\qquad b=\frac43K_p^2z^{-5/3},\qquad
K_p^3=\frac{25F_0}{48\pi\alpha_e^2}.
$$

This is an [axisymmetric pure plume](../../../../../axisymmetric-pure-plume.md). In this regime the explicit source-volume criterion is

$$
z\gg L_Q^{\mathrm{plume}}=
\left(\frac{2500Q_0^3}{243c^4F_0}\right)^{1/5}.
$$

For $Q_0=F_0=0$, $M_0>0$, the buoyancy vanishes and momentum is constant. The **pure-jet solution** is

$$
\boxed{F=0,\quad M=M_0,\quad Q=c\sqrt{M_0}\,z,\quad
w=\frac{\sqrt{M_0}}{cz},\quad r=2\alpha_ez.}
$$

This is the [jet limit of the top-hat plume model](../../../../../jet-limit-of-the-top-hat-plume-model.md). Both ideal zero-volume sources have singular speeds at $z=0$; they model regions outside a finite source where entrainment has already made the source-volume correction small.

When $M_0$ and $F_0$ are both positive, use the jet solution near the source and the pure-plume solution far above it, with an appropriate virtual-origin correction. To quantify this transition, eliminate $z$:

$$
\frac{dM}{dQ}=\frac{F_0Q}{cM^{3/2}},\qquad
\boxed{M^{5/2}-\frac{5F_0}{4c}Q^2
=M_0^{5/2}-\frac{5F_0}{4c}Q_0^2.}
$$

The conserved quantity is the [plume flux-balance invariant](../../../../../plume-flux-balance-invariant.md). With negligible $Q_0$, comparison of its two terms and $Q\simeq c\sqrt{M_0}z$ gives a transition height of order $M_0^{3/4}/(\sqrt c\sqrt{F_0})$. The exact connection, including finite $Q_0$, is the [finite-source forced-plume quadrature](../../../../../finite-source-forced-plume-quadrature.md)

$$
\boxed{z=\frac1c\int_{Q_0}^{Q(z)}
\left[M_0^{5/2}+\frac{5F_0}{4c}(q^2-Q_0^2)\right]^{-1/5}dq,}
$$

with $M$ then recovered from the invariant. A positive integrand gives the physical increasing-volume branch. As $Q$ grows, the source constant is negligible relative to $Q^2$, proving [attraction to pure plume similarity](../../../../../attraction-to-pure-plume-similarity.md). One matches the two asymptotic regimes or uses this quadrature; **the jet and plume solutions cannot be linearly superposed** because their governing flux equations are nonlinear.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 84](../../paper-84-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
