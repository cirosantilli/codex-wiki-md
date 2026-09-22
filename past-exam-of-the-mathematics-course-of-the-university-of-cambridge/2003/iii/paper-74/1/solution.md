<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Fluid-loaded plate.** Use complex [amplitudes](../../../../../wave-amplitude.md) with time dependence $e^{-i\omega t}$ and take the [velocity potential](../../../../../velocity-potential.md) in the fluid above the [elastic plate](../../../../../elastic-plate.md) to be $\Phi$. Let $\rho_0$ and $c_0$ be the undisturbed [mass density](../../../../../density.md) and [speed of sound](../../../../../speed-of-sound.md). The linearized [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) give $p=i\rho_0\omega\Phi$; the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) is $\Phi_y(x,0)=-i\omega\eta(x)$. We model loading from one fluid half-space, with no fluid loading on the other face. Loading by identical fluids on both faces instead doubles the fluid term below.

Define the [Fourier transform](../../../../../fourier-transform.md) and its inverse by

$$
\widehat f(k)=\int_{\mathbb R}f(x)e^{-ikx}\,dx,\qquad f(x)=\frac1{2\pi}\int_C\widehat f(k)e^{ikx}\,dk.
$$

The [Sommerfeld radiation condition](../../../../../sommerfeld-radiation-condition.md) selects $\widehat\Phi(k,y)=\widehat\Phi(k,0)e^{-\gamma y}$, with $\gamma^2=k^2-k_0^2$ and $k_0=\omega/c_0$. Here and in the diffraction calculation below, the outgoing [square root](../../../../../square-root.md) is specified by first taking $\operatorname{Im}\omega>0$. Draw a vertical cut upwards from $+k_0$ and another downwards from $-k_0$, and put

$$
\gamma=\gamma_u\gamma_l,\qquad \gamma_u=\sqrt{k+k_0},\quad -\frac\pi2<\arg(k+k_0)<\frac{3\pi}2,\qquad
\gamma_l=\sqrt{k-k_0},\quad -\frac{3\pi}2<\arg(k-k_0)<\frac\pi2.
$$

Thus $\gamma_u$ is analytic in the upper half-plane and $\gamma_l$ in the lower half-plane. In the real-frequency limit,

$$
\gamma=\sqrt{k^2-k_0^2}>0\quad (|k|>k_0),\qquad
\gamma=-i\sqrt{k_0^2-k^2}\quad (|k|<k_0).
$$

The [Fourier transform](../../../../../fourier-transform.md) contour $C$ follows the real axis with the limiting-absorption pole prescriptions. In particular, an outgoing propagating component has positive vertical [wavenumber](../../../../../wavenumber.md).

The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) gives $\widehat\Phi(0)=i\omega\widehat\eta/\gamma$, so $\widehat p(0)=-\rho_0\omega^2\widehat\eta/\gamma$. Eliminating the fluid [pressure](../../../../../pressure.md) from the bending balance gives the [line-forced fluid-loaded bending plate](../../../../../line-forced-fluid-loaded-bending-plate.md) kernel

$$
K(k)=\beta k^4-m\omega^2-\frac{\rho_0\omega^2}{\gamma},\qquad D(k)=\gamma K(k).
$$

For harmonic line [force](../../../../../force.md) [amplitude](../../../../../wave-amplitude.md) $F_0$ at the origin, the plate displacement and fluid [velocity potential](../../../../../velocity-potential.md) are therefore

$$
\boxed{\eta(x)=\frac{F_0}{2\pi}\int_C\frac{\gamma(k)e^{ikx}}{D(k)}\,dk},\qquad
\boxed{\Phi(x,y)=\frac{i\omega F_0}{2\pi}\int_C\frac{e^{ikx-\gamma y}}{D(k)}\,dk}.
$$

An arbitrary localized loading replaces $F_0$ by its [Fourier transform](../../../../../fourier-transform.md). This representation both calculates the response and identifies its different [wave](../../../../../wave.md) components through [poles](../../../../../pole.md) and [branch points](../../../../../branch-point.md).

For an observer $x=r\cos\theta$, $y=r\sin\theta$, with $0<\theta<\pi$, the [method of steepest descent](../../../../../method-of-steepest-descent.md) uses the [saddle point](../../../../../saddle-point.md) $k_s=k_0\cos\theta$. At fixed angle away from grazing, the [acoustic far field](../../../../../acoustic-far-field.md) is

$$
\Phi_{\rm rad}\sim\frac{i\omega F_0\sin\theta}{D(k_s)}\sqrt{\frac{k_0}{2\pi r}}e^{ik_0r-i\pi/4},\qquad p_{\rm rad}=i\rho_0\omega\Phi_{\rm rad}.
$$

The $r^{-1/2}$ spreading is that of cylindrical [acoustic waves](../../../../../acoustic-wave.md). The [phase velocity](../../../../../phase-velocity.md) parallel to the plate is $\omega/|k|$: components with $|k|<k_0$ are supersonic in that sense and radiate, whereas those with $|k|>k_0$ are subsonic and exponentially decay normally to the plate. The latter have reactive fluid loading and zero mean normal [acoustic energy flux](../../../../../acoustic-energy-flux.md).

There is also a real guided root $\kappa>k_0$. Indeed, $K(k_0+)=-\infty$, $K(+\infty)=+\infty$, and

$$
K'(k)=4\beta k^3+\frac{\rho_0\omega^2 k}{\gamma^3}>0\quad(k>k_0).
$$

The [residue theorem](../../../../../residue-theorem.md) then gives an outgoing displacement contribution $iF_0e^{i\kappa|x|}/K'(\kappa)$. It transports energy along the plate while its fluid field decays as $e^{-\gamma(\kappa)y}$. Other zeros on continued sheets can describe leaky or resonant [waves](../../../../../wave.md); [branch point](../../../../../branch-point.md) contributions describe near and grazing fields. A fixed-angle [acoustic far field](../../../../../acoustic-far-field.md) expansion is not uniform near the plate, where these components can matter.

For a propagating spectral component, write $\ell=(k_0^2-k^2)^{1/2}$. Its upward normal [velocity](../../../../../velocity.md) is $i\ell\widehat\Phi$ and its [pressure](../../../../../pressure.md) is $i\rho_0\omega\widehat\Phi$. Applying [Parseval's identity](../../../../../parseval-identity.md) to the time-averaged [acoustic energy flux](../../../../../acoustic-energy-flux.md) gives the upward power per unit length of the forcing line:

$$
\boxed{P_y=\frac{\rho_0\omega^3|F_0|^2}{4\pi}\int_{-k_0}^{k_0}\frac{\sqrt{k_0^2-k^2}}{|D(k)|^2}\,dk
=\frac{\rho_0\omega^3k_0^2|F_0|^2}{4\pi}\int_0^\pi\frac{\sin^2\theta}{|D(k_0\cos\theta)|^2}\,d\theta}.
$$

Equivalently, the integrand is $|\widehat\eta|^2/\ell$ with prefactor $\rho_0\omega^3/(4\pi)$. Integrating the radial [acoustic intensity](../../../../../acoustic-energy-flux.md) of the far field over a semicircle gives the same expression. The input power $\omega\operatorname{Im}(F_0^*\eta(0))/2$ also feeds guided [waves](../../../../../wave.md) along the plate, so it must not be identified with $P_y$ alone.

**Rigid half-plane diffraction.** Suppress the time factor and assume $0<\theta_0<\pi$. Write $a=k_0\cos\theta_0$, $b=k_0\sin\theta_0$, and denote the incident spatial field by $I=e^{-iax-iby}$. The [Helmholtz equation](../../../../../helmholtz-equation.md), [Sommerfeld radiation condition](../../../../../sommerfeld-radiation-condition.md), and square-root branches are as above. Across the open positive axis the scattered field and its normal derivative are continuous. Across the rigid negative axis its normal derivative is also continuous, while its potential can jump. Let $J(x)$ be this jump, supported on $x<0$. The transformed scattered field is

$$
\widehat\phi(k,y)=\tfrac12\operatorname{sgn}(y)\widehat J_u(k)e^{-\gamma|y|}.
$$

The jump transform is analytic in the upper half-plane. The absence of an even scattered component follows from derivative continuity and the outgoing condition. Its normal derivative on either face is $-\gamma\widehat J_u/2$.

On the negative axis this derivative must cancel $-ib e^{-iax}$. Since the [Half-range Fourier transform](../../../../../half-range-fourier-transform.md) of $H(-x)e^{-iax}$ is $i/(k+a)$, the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md) has the form

$$
\gamma_u\gamma_l\widehat J_u=\frac{2b}{k+a}+G_l(k),
$$

where $G_l$ is the transform of an unknown function supported on $x>0$ and analytic in the lower half-plane. The incident pole $k=-a$ lies below the Fourier contour. Divide by $\gamma_l$ and perform [pole subtraction in a Wiener-Hopf equation](../../../../../pole-subtraction-in-a-wiener-hopf-equation.md):

$$
\frac{2b}{(k+a)\gamma_l(k)}=
\frac{2b}{(k+a)\gamma_l(-a)}+
\frac{2b}{k+a}\left(\frac1{\gamma_l(k)}-\frac1{\gamma_l(-a)}\right).
$$

The first term is upper analytic and the second lower analytic, since the latter's apparent pole cancels. Equality of the two continued sides gives an entire function. The finite-energy edge condition, with $J(x)=O(\sqrt{-x})$, and the decay of the transforms at infinity force that function to vanish by [Liouville's theorem](../../../../../liouville-theorem.md). Consequently

$$
\widehat J_u(k)=\frac{2b}{\gamma_l(-a)(k+a)\gamma_u(k)},\qquad
\boxed{\phi(x,y)=\frac{\operatorname{sgn}(y)b}{2\pi\gamma_l(-a)}\int_C\frac{e^{ikx-\gamma|y|}}{(k+a)\gamma_u(k)}\,dk}.
$$

This is the [Wiener-Hopf solution of rigid half-plane diffraction](../../../../../wiener-hopf-solution-of-rigid-half-plane-diffraction.md) with the present transform and time conventions.

Deforming to a [steepest descent contour](../../../../../steepest-descent-contour.md) gives a residue from the incident pole precisely when $x+|y|\cot\theta_0<0$. At that pole $\gamma(-a)=-ib$; its residue produces

$$
\phi_{\rm GO}=\operatorname{sgn}(y)e^{-iax+ib|y|}H(-x-|y|\cot\theta_0).
$$

Thus the total [geometrical optics](../../../../../geometrical-optics.md) field is $I$ plus a reflected [wave](../../../../../wave.md) in the upper reflection region; in the lower shadow region the scattered residue cancels $I$, and outside that shadow the direct incident [wave](../../../../../wave.md) remains. This gives both the [amplitude](../../../../../wave-amplitude.md) and the spatial support of the [geometrical optics](../../../../../geometrical-optics.md) fields rather than merely naming a reflected [wave](../../../../../wave.md).

For $x=r\cos\theta$, $y=r\sin\theta$, $-\pi<\theta<\pi$, the saddle contribution uses $\gamma_l(-a)=-i\sqrt{2k_0}\cos(\theta_0/2)$ and $\gamma_u(k_s)=\sqrt{2k_0}\cos(\theta/2)$. The diffracted [wave](../../../../../wave.md) is

$$
\boxed{\phi_d\sim\frac{e^{ik_0r+i\pi/4}}{\sqrt{2\pi k_0r}}\frac{2\sin(\theta/2)\sin(\theta_0/2)}{\cos\theta+\cos\theta_0}
=\frac{e^{ik_0r+i\pi/4}}{2\sqrt{2\pi k_0r}}\left[\sec\frac{\theta+\theta_0}{2}-\sec\frac{\theta-\theta_0}{2}\right]}.
$$

The total field is $I+\phi_{\rm GO}+\phi_d$ to this order. This far-field expression applies away from the shadow/reflection boundaries $|\theta|=\pi-\theta_0$. There the pole and saddle coalesce, and a uniform [Fresnel integral](../../../../../fresnel-integral.md) approximation replaces the divergent separate terms by a smooth transition. The exact contour integral remains well defined.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
