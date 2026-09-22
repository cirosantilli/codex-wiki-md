<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $x$ tailward, so forward swimming has laboratory [velocity](../../../../../velocity.md) $-U\mathbf i$. For an inextensible travelling waveform, material motion in the swimmer frame is $V\mathbf i-c\mathbf t$: a material point passes through the wave along its tangent while the wave pattern translates at $V$. Thus the relative [velocity](../../../../../velocity.md) of otherwise stationary fluid is

$$
\mathbf w=c\mathbf t-(V-U)\mathbf i.
$$

Put $q=V-U$ and choose $\mathbf t=(X_s,Y_s)$, $\mathbf n=(-Y_s,X_s)$, with $X_s^2+Y_s^2=1$. Then

$$
w_t=c-qX_s,\qquad w_n=qY_s.
$$

On the forward-swimming branch $0<U<V<c$ and $X_s>0$, the tangential slip is positive. A law for reversed tangential slip would also need its sign, not just its absolute magnitude.

The quadratic normal law represents inertial cross-flow [drag](../../../../../drag-physics.md): dynamic [pressure](../../../../../pressure.md) scales as fluid density times $w_n^2$, while $|w_n|w_n$ chooses the [force](../../../../../force.md) direction. Its coefficient contains the cross-sectional size and an empirical [drag](../../../../../drag-physics.md) coefficient. The $|w_t|^{3/2}$ exponent is characteristic of an attached laminar [boundary layer](../../../../../boundary-layer.md): its thickness scales as $\delta\sim(\nu s/|w_t|)^{1/2}$ and its shear as $\mu|w_t|/\delta$. However, this gives local shear proportional to $|w_t|^{3/2}s^{-1/2}$, not $s^{1/2}$. The positive power of $s$ is genuinely printed in this paper and repeated in its target formulas. Below it is treated as the prescribed phenomenological weight, rather than misidentified as standard local [laminar skin-friction scaling along a slender swimmer](../../../../../laminar-skin-friction-scaling-along-a-slender-swimmer.md).

The normal axial [force](../../../../../force.md) on an element is

$$
dF_{N,x}=K_N|qY_s|qY_s(-Y_s)ds=-K_Nq^2|Y_s|^3ds.
$$

The prescribed tangential [force](../../../../../force.md) gives $dF_{T,x}=K_T(c-qX_s)^{3/2}X_s s^{1/2}ds$. Zero mean axial [force](../../../../../force.md) therefore gives the [nonlinear resistive-force balance for a travelling filament](../../../../../nonlinear-resistive-force-balance-for-a-travelling-filament.md)

$$
\boxed{K_N(V-U)^2\int_0^L|\widehat Y_s|^3ds
=K_T\int_0^L|c-(V-U)X_s|^{3/2}X_s s^{1/2}ds.}
$$

The absolute values are present in the original PDF. In a periodically beating, constant-mean-speed model, phase-average the integrals where necessary; the leading approximation below is phase independent. Local [force](../../../../../force.md) laws neglect nonlocal hydrodynamic interactions and assume nearly steady local response.

For the sinusoidal displacement, let $\varepsilon=\beta k\ll1$. Then $Y_s=\varepsilon\cos ks$ and $X_s=(1-Y_s^2)^{1/2}=1+O(\varepsilon^2)$. Over one wavelength,

$$
\int_0^L|Y_s|^3ds=\frac{\beta^3k^3}{k}\int_0^{2\pi}|\cos z|^3dz=\frac83\beta^3k^2,
\qquad \int_0^Ls^{1/2}ds=\frac23L^{3/2}.
$$

Replace $X_s$ by one in the leading tangential term and balance the [forces](../../../../../force.md). After multiplication by $3/2$,

$$
\boxed{4\beta^3k^2K_N(V-U)^2\simeq K_TL^{3/2}(c-V+U)^{3/2}.}
$$

This replacement also requires $c\varepsilon^2\ll c-V+U$ for a uniformly small relative error inside the fractional power. If the tangential slip is itself $O(c\varepsilon^2)$, its variation along the body must be retained. Periodicity gives $V/c=\langle X_s\rangle=1-\varepsilon^2/4+O(\varepsilon^4)$, so small geometric slope alone does not guarantee that additional slip condition.

For [Lighthill elongated-body theory](../../../../../lighthill-elongated-body-theory.md), put $h(x,t)\simeq\beta\sin[k(x-Vt)]$ and $w_\perp=h_t+Uh_x$. The transverse fluid [kinetic energy](../../../../../kinetic-energy.md) per unit length is $M_Aw_\perp^2/2$. In the usual tail-flux approximation, with negligible leading-end contribution, the lateral work flux is $M_AU\langle h_tw_\perp\rangle$, whereas [kinetic energy](../../../../../kinetic-energy.md) carried into the wake is $M_AU\langle w_\perp^2\rangle/2$. Their difference is the useful propulsive power $TU$. Consequently

$$
T=M_A\left\langle h_tw_\perp-\frac12w_\perp^2\right\rangle
=\frac{M_A}{2}\langle h_t^2-U^2h_x^2\rangle
=\frac{M_A}{4}\beta^2k^2(V^2-U^2).
$$

Balancing this against the [drag](../../../../../drag-physics.md) of the printed tangential model, $D=(2/3)K_TL^{3/2}(c-V+U)^{3/2}$, gives

$$
\boxed{\frac38M_A\beta^2k^2(V^2-U^2)=K_TL^{3/2}(c-V+U)^{3/2}.}
$$

For a genuine local laminar skin-friction estimate, write $dD=C_Tu_t^{3/2}s^{-1/2}ds$, where $C_T$ has the appropriate different dimensions. Its integrated [drag](../../../../../drag-physics.md) is $2C_Tu_t^{3/2}\sqrt L$, and the corresponding elongated-body balance is instead $M_A\beta^2k^2(V^2-U^2)/8=C_T\sqrt L\,(c-V+U)^{3/2}$. The printed $L^{3/2}$ expression is therefore a result of its stated [force](../../../../../force.md) model, not of that standard boundary-layer law.

The two thrust models describe different mechanisms: cross-flow [resistive-force theory](../../../../../resistive-force-theory.md) uses dissipative local [drag](../../../../../drag-physics.md), while [elongated-body theory](../../../../../lighthill-elongated-body-theory.md) uses reactive acceleration of [added mass](../../../../../added-mass.md). Both suppress details of the wake, body-body interactions, finite slenderness, skin-friction unsteadiness, separation and possible turbulent transition. The tail-only reactive result also requires a negligible leading-end flux, usually supplied by a nose taper or small leading-end motion; a blunt constant-cross-section body waving equally at both ends cannot automatically omit its leading-end contribution. Speed fluctuations and recoil may matter, and a planar constant-amplitude waveform is an idealization of a real sea snake.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
