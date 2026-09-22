# Latitude law of Foucault precession

↑ **Parent:** [Foucault pendulum](foucault-pendulum.md)

Use local east, north, and up [unit vectors](unit-vector.md), with $x$ eastward, $y$ northward, and positive orientation $\psi$ anticlockwise as viewed from above. Let $\varphi$ be signed [geographical latitude](geographical-latitude.md), positive north, and $\Omega>0$ the magnitude of [Earth](earth.md)'s [angular velocity](angular-velocity.md). In the spherical-[Earth](earth.md) approximation,

$$
\boldsymbol\Omega=\Omega\cos\varphi\,\mathbf e_N+\Omega\sin\varphi\,\mathbf e_U,\qquad
\alpha=\Omega\sin\varphi,\qquad \omega_0^2=\frac g\ell.
$$

Here $g$ is the local [effective gravity in a rotating frame](effective-gravity-in-a-rotating-frame.md), including the steady terrestrial [centrifugal acceleration](centrifugal-acceleration.md). For small horizontal displacements compared with $\ell$, the horizontal restoring [acceleration](acceleration.md) from [tension](tension.md) is $-\omega_0^2(x,y)$. Vertical displacement is second order in the swing [amplitude](wave-amplitude.md), so vertical [velocity](velocity.md) can be omitted at this order. The horizontal [Coriolis acceleration in local Earth coordinates](coriolis-acceleration-in-local-earth-coordinates.md) then gives the coupled [linear differential equations](linear-differential-equation.md)

$$
\ddot x+\omega_0^2x=2\alpha\dot y,\qquad
\ddot y+\omega_0^2y=-2\alpha\dot x.
$$

These equations neglect [damping](damping.md), finite-amplitude corrections, support [anisotropy](anisotropy.md), and spatial changes of the [centrifugal force](centrifugal-force.md) of order $\Omega^2$; they retain the leading terrestrial [Coriolis force](coriolis-force.md). A related derivation uses south/east axes instead.[Foucault's pendulum - the physics (and maths) explained, equations (9.1\*)–(11): horizontal small-oscillation equations](foucault-s-pendulum-the-physics-and-maths-explained-by-joe-wolfe.md)

Introduce the [complex number](complex-number.md) $z=x+iy$. Multiplying the second equation by $i$ and adding gives

$$
\ddot z+2i\alpha\dot z+\omega_0^2z=0.
$$

Set $z=e^{-i\alpha t}u$. Direct [differentiation](differentiation.md) cancels the first [derivative](derivative.md) of $u$ and yields

$$
\ddot u+(\omega_0^2+\alpha^2)u=0,\qquad
\beta=\sqrt{\omega_0^2+\alpha^2},\qquad
z=e^{-i\alpha t}(C\cos\beta t+D\sin\beta t).
$$

The $\alpha^2$ in $\beta$ comes from solving these reduced equations exactly; it is not a complete prediction of terrestrial corrections of order $\Omega^2$. Thus the horizontal [trajectory](trajectory.md) is an [ellipse](ellipse.md) in coordinates rotating at [angular velocity](angular-velocity.md) $-\alpha$ relative to the building. When $|\alpha|\ll\omega_0$, each rapid swing samples an almost fixed long axis; its slow [precession](precession.md) is

$$
\dot\psi=-\Omega\sin\varphi,\qquad
T_{\mathrm p}=\frac{2\pi}{\Omega|\sin\varphi|}=\frac{T_{\mathrm{sid}}}{|\sin\varphi|}.
$$

The [sidereal day](sidereal-day.md) $T_{\mathrm{sid}}=2\pi/\Omega$ is a rotation relative to distant directions. $T_{\mathrm p}$ denotes a full $2\pi$ turn of a continuously followed orientation; an unlabelled swing line repeats after $T_{\mathrm p}/2$. At the equator there is no finite [precession period](precession-period.md) in this model. The [Coriolis parameter](coriolis-parameter.md) is $f=2\alpha$, so the plane's rate is $-f/2$, not $-f$.

The limiting cases check the sign and scale. At the north pole $\alpha=\Omega$: the swing direction turns clockwise once per [sidereal day](sidereal-day.md). At the equator $\alpha=0$: both horizontal equations reduce to independent [simple harmonic motions](simple-harmonic-motion.md) and a line launch stays on its original line. At the south pole $\alpha=-\Omega$: the direction turns anticlockwise once per [sidereal day](sidereal-day.md). Vanishing horizontal [precession](precession.md) at the equator does not mean that every component of [Coriolis acceleration](coriolis-acceleration.md) vanishes there.

For a stipulated $\Omega=7.292115\times10^{-5}\,\mathrm{s^{-1}}$, the [sidereal day](sidereal-day.md) is approximately $23.9345\,\mathrm h$. At $45^\circ$ north the predicted rate is $-10.6356^\circ/\mathrm h$ and $T_{\mathrm p}\simeq33.8485\,\mathrm h$; at $45^\circ$ south the rate changes sign. At the illustrative [geographical latitude](geographical-latitude.md) $34^\circ$ south, the prediction is $+8.4109^\circ/\mathrm h$. These calculations are model predictions, not new observations of the UNSW apparatus.

A swing [plane](plane.md) fixed among the stars is generally only a polar picture. A north–south swing at the equator turns with [Earth](earth.md) in an [inertial frame](inertial-frame.md), while having no [precession](precession.md) against the building.[The Foucault pendulum, The 'plane' of the pendulum's swing is not fixed in space: equatorial counterexample](the-foucault-pendulum-by-joe-wolfe.md)

## ↑ Ancestors (6)

1. [Foucault pendulum](foucault-pendulum.md)
2. [Simple pendulum](simple-pendulum-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Earth's rotation](earth-s-rotation.md)
- [UNSW Foucault pendulum observation](unsw-foucault-pendulum-observation.md)
