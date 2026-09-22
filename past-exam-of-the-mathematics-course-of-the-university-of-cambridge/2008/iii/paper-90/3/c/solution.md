<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the carrier fluid has ambient [mass density](../../../../../../density.md) $\rho_0$, the particles have [mass density](../../../../../../density.md) $\rho_p>\rho_0$, and volumes add. The well-mixed current then has

$$
\boxed{\rho=(1-\phi)\rho_0+\phi\rho_p,\qquad
g'=g\frac{\rho-\rho_0}{\rho_0}=g_0'\phi,\qquad
g_0'=g\frac{\rho_p-\rho_0}{\rho_0}.}
$$

Here $g_0'$ is the particle-fluid reference [reduced gravity](../../../../../../reduced-gravity-split.md) per unit volume fraction, which is the convention needed in the requested expansion. The initial current [reduced gravity](../../../../../../reduced-gravity-split.md) is $g_0'\phi_0$; it should not be confused with $g_0'$ itself. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) requires $\phi(\rho_p-\rho_0)/\rho_0\ll1$.

For particles to remain well mixed, the turbulent vertical mixing time must be short compared with the settling time. In a [turbulent diffusion](../../../../../../eddy-diffusion.md) description with diffusivity $K_z$, require $h^2/K_z\ll h/[V_s(1-\phi)]$, or $K_z\gg hV_s(1-\phi)$. Equivalently, characteristic turbulent vertical speeds should substantially exceed the particle [settling velocity](../../../../../../settling-velocity.md). [Turbulence](../../../../../../turbulence-split.md) can maintain an approximately uniform [concentration](../../../../../../concentration.md) in the body while particles still settle relative to the fluid. At the impermeable bed, fluid has no normal transport into the solid boundary, but particles can reach and be captured by it. Assume no resuspension after capture.

Use a [gravity-current box model](../../../../../../gravity-current-box-model.md) of length $L(t)$, uniform depth $h(t)$ and uniform [concentration](../../../../../../concentration.md) $\phi(t)$. Neglect ambient [entrainment](../../../../../../fluid-entrainment.md) and the small volume change caused by depositing dilute solids, so $Lh=M$ remains constant. Take a constant front [Froude number](../../../../../../froude-number.md) $F>0$ and the [gravity-current front condition](../../../../../../gravity-current-front-condition.md) $\dot L=F\sqrt{g'h}$. With $\phi_{\max}=1$, the deposition flux is $V_s\phi(1-\phi)$ per unit bed area. The particle-volume budget is

$$
\frac{d}{dt}(M\phi)=-LV_s\phi(1-\phi).
$$

Hence the integral model is

$$
\boxed{h=\frac ML,\qquad
\dot L=F\sqrt{\frac{g_0'M\phi}{L}},\qquad
\dot\phi=-\frac{V_sL}{M}\phi(1-\phi),\qquad
L(0)=L_0,\quad\phi(0)=\phi_0.}
$$

The model assumes a fixed rear boundary, one advancing front, a deep stationary ambient, negligible drag during the inertial spreading regime, and a perfectly absorbing bed. The supplied hindered-settling law is retained in the deposition closure.

For $0<\phi<1$, eliminating time gives

$$
\frac{d\phi}{\sqrt\phi(1-\phi)}=-\frac{V_s}{F\sqrt{g_0'}M^{3/2}}L^{3/2}\,dL.
$$

The [concentration](../../../../../../concentration.md) integral is $2\operatorname{artanh}\sqrt\phi$. Therefore

$$
L^{5/2}=L_0^{5/2}+\frac{5FM^{3/2}\sqrt{g_0'}}{V_s}
\left(\operatorname{artanh}\sqrt{\phi_0}-\operatorname{artanh}\sqrt\phi\right).
$$

As the particle [concentration](../../../../../../concentration.md) tends to zero, the current [reduced gravity](../../../../../../reduced-gravity-split.md) and front speed tend to zero. The [hindered-settling runout in a rectangular channel](../../../../../../hindered-settling-runout-in-a-rectangular-channel.md) is

$$
\boxed{L_\infty=\left[L_0^{5/2}+\frac{5FM^{3/2}\sqrt{g_0'}}{V_s}
\operatorname{artanh}\sqrt{\phi_0}\right]^{2/5}.}
$$

It is a finite limiting distance; in this idealized model, the exponential tail of particle loss makes complete stopping asymptotic in time. For $L_\infty\gg L_0$, omit $L_0^{5/2}$. Using $\operatorname{artanh}x=x+x^3/3+O(x^5)$ gives

$$
\boxed{L_\infty^5\approx\frac{25F^2M^3g_0'}{V_s^2}
\left(\phi_0+\frac23\phi_0^2+O(\phi_0^3)\right).}
$$

The original PDF has $V_s^2$ in this expression; the TeX aid's $V_s^3$ is a transcription error. Dimensions independently confirm the square: $M^3g_0'/V_s^2$ has dimensions of length to the fifth power. If one instead names the initial current [reduced gravity](../../../../../../reduced-gravity-split.md) $G_{\mathrm{init}}=g_0'\phi_0$, the same expansion is $25F^2M^3G_{\mathrm{init}}[1+2\phi_0/3+O(\phi_0^2)]/V_s^2$. Late loss of [turbulent mixing](../../../../../../turbulent-mixing.md), viscous resistance or bed resuspension can change the physical runout beyond this specified box model.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
