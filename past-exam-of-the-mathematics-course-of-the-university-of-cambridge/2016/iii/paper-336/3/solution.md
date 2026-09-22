<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [geometrical optics](../../../../../geometrical-optics.md) convention

$$
\boxed{\omega=-\theta_T,\qquad k=\theta_X,\qquad\ell=\theta_Y.}
$$

Because $\partial_t=\varepsilon\partial_T$ and $\partial_x=\varepsilon\partial_X$, differentiating $e^{i\theta/\varepsilon}$ gives an order-one physical [angular frequency](../../../../../angular-frequency.md) and order-one physical [wavenumbers](../../../../../wavenumber.md). Absorb a constant leading [amplitude](../../../../../wave-amplitude.md) phase into $\theta$ and take $A_0$ real; for a complex [amplitude](../../../../../wave-amplitude.md) the corresponding quadratic density is $|A_0|^2$.

Substitution into the [wave equation](../../../../../wave-equation-split.md) gives the [eikonal equation for a variable-speed wave](../../../../../eikonal-equation-for-a-variable-speed-wave.md) at leading order:

$$
\boxed{\omega^2=c^2(k^2+\ell^2).}
$$

Choose the positive-frequency branch $\omega=\Omega=cK$, $K=\sqrt{k^2+\ell^2}$; the negative branch can be treated in exactly the same way. The imaginary first-order terms give

$$
2\omega A_{0,T}+\omega_TA_0+2c^2(kA_{0,X}+\ell A_{0,Y})+\big[(c^2k)_X+(c^2\ell)_Y\big]A_0=0.
$$

Multiplying by $A_0$ puts this [wave-action transport for a variable-speed wave](../../../../../wave-action-transport-for-a-variable-speed-wave.md) in conservation form:

$$
\boxed{(\omega A_0^2)_T+(c^2kA_0^2)_X+(c^2\ell A_0^2)_Y=0.}
$$

Its density is $\omega A_0^2$ and its flux is that density times the [group velocity](../../../../../group-velocity.md). Independently, equality of mixed [wave phase](../../../../../phase-waves.md) [derivatives](../../../../../derivative.md) gives

$$
\boxed{k_Y=\ell_X},\qquad k_T=-\omega_X,\qquad\ell_T=-\omega_Y.
$$

This [phase compatibility in geometrical optics](../../../../../phase-compatibility-in-geometrical-optics.md) is essential when converting the differentiated dispersion relation into equations along rays.

For completeness let $\omega=\Omega(\mathbf k;\mathbf X,T)$ be a general local [dispersion relation](../../../../../dispersion-relation.md). Define [ray tracing](../../../../../ray-tracing.md) by $d\mathbf X/dT=\mathbf c_g=\nabla_{\mathbf k}\Omega$. Using the [chain rule](../../../../../chain-rule.md) in $\nabla_{\mathbf X}\omega$ and the symmetry $\partial_{X_i}k_j=\partial_{X_j}k_i$ gives

$$
\mathbf k_T+(\mathbf c_g\cdot\nabla_{\mathbf X})\mathbf k=-\nabla_{\mathbf X}\Omega\big|_{\mathbf k}.
$$

Likewise $\omega_T=\Omega_T+\mathbf c_g\cdot\mathbf k_T$ cancels its advective term because $\mathbf k_T=-\nabla\omega$. Hence the [Hamiltonian ray equations for a local dispersion relation](../../../../../hamiltonian-ray-equations-for-a-local-dispersion-relation.md) are

$$
\boxed{\frac{d\mathbf X}{dT}=\nabla_{\mathbf k}\Omega,\qquad\frac{d\mathbf k}{dT}=-\nabla_{\mathbf X}\Omega\big|_{\mathbf k},\qquad\frac{d\omega}{dT}=\Omega_T\big|_{\mathbf k}.}
$$

The derivatives on the right hold the [wavevector](../../../../../wavevector.md) fixed. For this [wave equation](../../../../../wave-equation-split.md) they reduce to

$$
\frac{d\mathbf X}{dT}=c\frac{\mathbf k}{K}=\frac{c^2\mathbf k}{\omega},\qquad\frac{d\mathbf k}{dT}=-K\nabla c,\qquad\frac{d\omega}{dT}=Kc_T.
$$

When $c=c(Y)$, the ray invariants are $k$ and $\omega$, while $d\ell/dT=-Kc_Y<0$. For a monochromatic component with these fixed invariants write $\theta=kX-\omega T+S(Y)$, so

$$
\ell=S'(Y)=\sqrt{\frac{\omega^2}{c(Y)^2}-k^2}>0.
$$

Using the stated independence of $A_0$ from $X,T$, the [wave-action transport for a variable-speed wave](../../../../../wave-action-transport-for-a-variable-speed-wave.md) becomes $(c^2\ell A_0^2)_Y=0$. Therefore

$$
\boxed{A_0(Y)=\frac\mu{c(Y)\sqrt{\ell(Y)}}.}
$$

This is the [stationary wave amplitude in a stratified wavespeed](../../../../../stationary-wave-amplitude-in-a-stratified-wavespeed.md); $\mu$ is the constant for that component or ray family.

At the proposed [simple turning point of a variable-speed wave](../../../../../simple-turning-point-of-a-variable-speed-wave.md), take $c_s=c(Y_s)=\omega/k$ and $c_s'=c_Y(Y_s)>0$. On the chosen positive branch this entails $k>0$. Define

$$
Q(Y)=\frac{\omega^2}{c^2}-k^2,\qquad q=-Q'(Y_s)=\frac{2k^2c_s'}{c_s}>0.
$$

As the ray approaches from below, $\ell\sim[q(Y_s-Y)]^{1/2}$ and

$$
A_0\sim\frac\mu{c_s q^{1/4}(Y_s-Y)^{1/4}}.
$$

The amplitude diverges and the vertical [group velocity](../../../../../group-velocity.md) $c^2\ell/\omega$ vanishes. The [WKB approximation](../../../../../wkb-approximation.md) also fails its slow-variation condition $\varepsilon|\ell_Y|/\ell^2\ll1$ when $Y_s-Y=O(\varepsilon^{2/3})$. The [turning-point enhancement of wave amplitude](../../../../../turning-point-enhancement-of-wave-amplitude.md) shows that this divergence is a failure of the outer ray approximation, rather than an actual infinite solution.

To derive the inner wavefield directly, separate the conserved horizontal [wave phase](../../../../../phase-waves.md) and frequency in the original [differential equation](../../../../../differential-equation-split.md):

$$
\varphi=\Psi(Y)e^{i(kX-\omega T)/\varepsilon}+\text{c.c.},\qquad\varepsilon^2(c^2\Psi_Y)_Y+(\omega^2-c^2k^2)\Psi=0.
$$

Dividing by $c^2$ gives $\varepsilon^2\Psi_{YY}+2\varepsilon^2(c_Y/c)\Psi_Y+Q(Y)\Psi=0$. Set $Y-Y_s=\delta\eta$. The second derivative is of size $\varepsilon^2/\delta^2$, whereas $Q\sim-q\delta\eta$, so the [Airy scaling at a variable-speed wave turning point](../../../../../airy-scaling-at-a-variable-speed-wave-turning-point.md) is

$$
\boxed{\delta=\left(\frac{\varepsilon^2}{q}\right)^{1/3},\qquad\Psi_{\eta\eta}-\eta\Psi=0\text{ at leading order}.}
$$

The first-derivative term is smaller by $O(\delta)$, and higher coefficients in the expansion of $Q$ give the same relative order. Thus the general leading inner profile is a [linear combination](../../../../../linear-combination.md) of the two [Airy functions](../../../../../airy-function.md) $\operatorname{Ai}(\eta)$ and $\operatorname{Bi}(\eta)$. For [decaying Airy continuation and ray reflection](../../../../../decaying-airy-continuation-and-ray-reflection.md), if the physical continuation is bounded and decays into $Y>Y_s$, its growing $\operatorname{Bi}$ coefficient is zero. In that usual evanescent continuation the wavefield has the form

$$
\boxed{\varphi\sim\varepsilon^{-1/6}B\operatorname{Ai}\!\left(q^{1/3}\frac{Y-Y_s}{\varepsilon^{2/3}}\right)e^{i(kX-\omega T+\theta_s)/\varepsilon}+\text{c.c.},\qquad B=O(1).}
$$

Without a condition in the evanescent region the corresponding $\operatorname{Bi}$ term remains admissible locally; the given existence of a wavefield below the turning point alone does not select its coefficient.

Finally, the outer [amplitude](../../../../../wave-amplitude.md) at distance $\delta$ is $O(\delta^{-1/4})=O(\varepsilon^{-1/6})$ for $\mu=O(1)$ and fixed nonzero $q$. The oscillatory [Airy turning-point connection formula](../../../../../airy-turning-point-connection-formula.md) has exactly the same $(-\eta)^{-1/4}$ envelope on the allowed side. Therefore **the inner wavefield has magnitude $O(\varepsilon^{-1/6})$**. The decaying Airy continuation matches an incident and reflected pair of rays, so a single upward $\ell>0$ branch must be supplemented by its reflected branch near the turning point; no formal coefficient matching is needed to identify this magnitude.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 336](../../paper-336-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
