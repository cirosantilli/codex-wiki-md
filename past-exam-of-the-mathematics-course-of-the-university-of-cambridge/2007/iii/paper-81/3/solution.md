<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\widehat u(\widehat r)=-W_0(1-\widehat r^2/R^2)+\widehat w(\widehat r)$ and $\mathbf p=\sin\theta\,\mathbf e_r+\cos\theta\,\mathbf k$, with $\cos\theta>0$ for the upward-stable orientation. [Cell conservation in a swimming suspension](../../../../../cell-conservation-in-a-swimming-suspension.md) gives radial flux

$$
\widehat j_r=V_C\widehat n\sin\theta-D\frac{d\widehat n}{d\widehat r},\qquad
\frac1{\widehat r}\frac{d}{d\widehat r}(\widehat r\widehat j_r)=0.
$$

Regularity at the axis and impermeability at the wall imply $\widehat j_r=0$, hence $D\widehat n'=V_C\widehat n\sin\theta$. Axial advection has no divergence in this fully developed, axially uniform state.

The fluid is incompressible. Use dynamic [stresslet](../../../../../force-dipole-flow.md) strength $S_d$ and [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu_d$ first, so the swimming contribution to its stress is $S_d\widehat n(\mathbf p\mathbf p-I/3)$. The isotropic part can be absorbed into the effective [pressure](../../../../../pressure.md). With the ordinary fluid hydrostatic [pressure](../../../../../pressure.md) removed, the axial momentum equation is

$$
0=-\frac{d\widehat P}{d\widehat z}
+\frac{\mu_d}{\widehat r}\frac{d}{d\widehat r}(\widehat r\widehat u')
+\frac{S_d}{\widehat r}\frac{d}{d\widehat r}(\widehat r\widehat n\sin\theta\cos\theta)
-g\Delta\rho\,\nu\widehat n.
$$

The final term is the downward excess weight of the cells. Sedimentation is neglected in their swimming flux, not in this buoyancy [force](../../../../../force.md). Fluid convective inertia vanishes for the specified fully developed [velocity](../../../../../velocity.md) even before a low-Reynolds-number approximation is invoked.

There is a dimensional convention to make explicit. The printed definition of $\gamma$ contains the extra fluid density $\rho$. All the printed coefficients are consistent if this question uses density-normalized [pressure](../../../../../pressure.md), [kinematic viscosity](../../../../../kinematic-viscosity.md) and [stresslet](../../../../../force-dipole-flow.md) strength:

$$
\widehat p=\widehat P/\rho,\qquad \mu=\mu_d/\rho,\qquad S=S_d/\rho.
$$

Then $\widehat p'=4\mu W_0/R^2$ generates the stated background [Poiseuille flow](../../../../../hagen-poiseuille-equation.md). If $\mu$ and $S$ instead mean [dynamic viscosity](../../../../../dynamic-viscosity.md) and a physical force-dipole strength, the correct buoyancy parameter is $g\Delta\rho\nu N_0R^2/(\mu_dW_0)$, without a further density denominator. The following derivation retains the consistent density-normalized interpretation of the printed parameters.

The [bottom-heavy spherical-cell orientation dynamics](../../../../../bottom-heavy-spherical-cell-orientation-dynamics.md) is

$$
\dot{\mathbf p}=\frac1B[\mathbf k-(\mathbf k\cdot\mathbf p)\mathbf p]
+\frac12\boldsymbol\omega\times\mathbf p,
\qquad \boldsymbol\omega=-\widehat u'\mathbf e_\phi.
$$

Its scalar tilt equation is $\dot\theta=-\sin\theta/B-\widehat u'/2$. Steady gravitational-viscous [torque](../../../../../torque.md) balance therefore gives $\sin\theta=-B\widehat u'/2$. This equilibrium is stable on the $\cos\theta>0$ branch and exists only when $|B\widehat u'/2|<1$.

Put $r=\widehat r/R$, $w=\widehat w/W_0$, $n=\widehat n/N_0$. Subtract the background pressure-driven balance and divide by $\mu W_0/R^2$. The governing system is

$$
\boxed{n'=\chi n\sin\theta,\qquad
\frac1r(rw')'+\frac\sigma r(rn\sin2\theta)'=\gamma n,\qquad
\sin\theta=-\lambda(2r+w'),}
$$

where

$$
\chi=\frac{V_CR}{D},\qquad \sigma=\frac{SN_0R}{2\mu W_0},\qquad
\gamma=\frac{g\Delta\rho\nu N_0R^2}{\rho\mu W_0},\qquad
\lambda=\frac{BW_0}{2R}.
$$

The last parameter contains $B$, as in the PDF, not the [diffusivity](../../../../../diffusion-coefficient.md) substituted by the converted TeX. Boundary and normalization conditions are

$$
w(1)=0,\qquad w'(0)=0,\qquad n'(0)=0,\qquad \theta(0)=0,\qquad
2\int_0^1 n(r)r\,dr=1.
$$

The wall cell-flux condition is already incorporated in $n'=\chi n\sin\theta$; there is no prescribed wall concentration or additional fixed-volume-flux condition. The radial divergence of the [stresslet](../../../../../force-dipole-flow.md) stress can be balanced by a radial [pressure](../../../../../pressure.md) depending only on $r$. It neither produces radial flow in this ansatz nor changes the imposed axial [pressure](../../../../../pressure.md) gradient, so it is eliminated from the axial problem, not assumed to vanish.

For $\gamma\ll1$, $\sigma=\gamma\sigma_1$, let $w=\gamma w_1+O(\gamma^2)$, $n=n_0+\gamma n_1+O(\gamma^2)$. The leading tilt has

$$
\sin\theta_0=-2\lambda r,\qquad \cos\theta_0=\sqrt{1-4\lambda^2r^2}.
$$

The supplied $BW_0/R<1$ ensures this leading orientation remains on the stable branch. Put $a=\lambda\chi$. Integrating the concentration equation and imposing the average concentration gives the [gyrotactic focusing in a downward pipe flow](../../../../../gyrotactic-focusing-in-a-downward-pipe-flow.md) profile

$$
\boxed{n_0(r)=Ae^{-ar^2},\qquad A=\frac{a}{1-e^{-a}}.}
$$

At $a=0$ the continuous limit is $n_0=1$.

At first order the axial equation is

$$
(rw_1')'+\sigma_1(rn_0\sin2\theta_0)'=rn_0.
$$

Integrate from the regular axis, where both boundary terms vanish:

$$
rw_1'+\sigma_1rn_0\sin2\theta_0=\int_0^r sn_0(s)\,ds
=\frac{A}{2a}(1-e^{-ar^2}).
$$

Since $\sin2\theta_0=-4\lambda r\sqrt{1-4\lambda^2r^2}$, the [stresslet correction to gyrotactic pipe flow](../../../../../stresslet-correction-to-gyrotactic-pipe-flow.md) is

$$
\boxed{w_1'(r)=\frac{A(1-e^{-ar^2})}{2ar}
+4\sigma_1\lambda r n_0(r)\sqrt{1-4\lambda^2r^2},}
$$

with its regular limiting value at $r=0$, and

$$
\boxed{w_1(r)=-\int_r^1\left[\frac{A(1-e^{-as^2})}{2as}
+4\sigma_1\lambda s n_0(s)\sqrt{1-4\lambda^2s^2}\right]ds.}
$$

The orientation and concentration corrections, if needed to complete the expansion, follow without another differential boundary problem:

$$
\theta_1=-\frac{\lambda w_1'}{\cos\theta_0},\qquad
n_1=a n_0(\langle w_1\rangle_0-w_1),\qquad
\langle w_1\rangle_0=2\int_0^1n_0w_1r\,dr.
$$

These enforce $2\int_0^1n_1r\,dr=0$.

For $\lambda>0$, write the two positive integrand coefficients as $F(s)=A(1-e^{-as^2})/(2as)$ and $H(s)=4\lambda s n_0(s)\sqrt{1-4\lambda^2s^2}$. Then

$$
w_1(r)=-\int_r^1F(s)ds-\sigma_1\int_r^1H(s)ds.
$$

Thus $w_1<0$ throughout the interior for $\sigma_1\geq0$, and at any given radius a positive correction is possible only if

$$
\boxed{\sigma_1<-\frac{\int_r^1F(s)ds}{\int_r^1H(s)ds}.}
$$

A simple sufficient condition for negativity is $\sigma_1\geq-1/(8\lambda)$: indeed

$$
\frac{F(s)}{H(s)}=\frac{e^{as^2}-1}{8a\lambda s^2\sqrt{1-4\lambda^2s^2}}\geq\frac1{8\lambda}.
$$

When $\lambda=0$, the [stresslet](../../../../../force-dipole-flow.md) contribution vanishes and the buoyancy correction is negative regardless of $\sigma_1$.

Physically, downward shear tilts upward swimmers toward the axis, concentrating excess weight there and enhancing the downward flow. Positive $S$ in the specified $+Sn\mathbf p\mathbf p$ stress convention reinforces this effect; sufficiently negative $S$ opposes it. A positive $w$ means reduced downward [velocity](../../../../../velocity.md), not necessarily reversal of the total pipe flow. The deterministic orientation closure fails at excessive shear, and scalar [diffusivity](../../../../../diffusion-coefficient.md) neglects directional and shear-dependent dispersion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
