# Newtonian binary chirp

↑ **Parent:** [Gravitational wave](gravitational-wave-split.md)

A [Newtonian binary chirp](newtonian-binary-chirp.md) is a leading-order model in which loss of orbital [energy](energy-split.md) to [gravitational radiation](gravitational-wave-split.md) makes an almost circular [binary system](binary-system.md) shrink and its [gravitational-wave frequency](gravitational-wave-frequency.md) rise. Here is a derivation with explicit SI units. Let the constant component [masses](mass.md) $m_1,m_2$ be in kilograms, $M=m_1+m_2$, $\mu=m_1m_2/M$, separation $a$ in metres, and orbital [angular frequency](angular-frequency.md) $\Omega$ in radians per second. [Newtonian gravity](gravitational-acceleration.md), circular motion and the [quadrupole formula](quadrupole-formula.md) give

$$
\Omega^2=\frac{GM}{a^3},\qquad f=\frac{\Omega}{\pi},\qquad
E=-\frac{G\mu M}{2a},\qquad
P=\frac{32G^4\mu^2M^3}{5c^5a^5},\qquad \dot E=-P.
$$

The factor $\pi$ rather than $2\pi$ appears because the dominant [mass quadrupole moment](mass-quadrupole-moment.md) repeats twice per orbit. Since $dE/da>0$, radiative [energy](energy-split.md) loss implies $\dot a<0$, hence

$$
\dot a=-\frac{64G^3\mu M^2}{5c^5a^3},\qquad
\dot f=Kf^{11/3},\qquad
K=\frac{96}{5}\pi^{8/3}\left(\frac{G\mathcal M}{c^3}\right)^{5/3},\qquad
\mathcal M=\mu^{3/5}M^{2/5}.
$$

The quantity $G\mathcal M/c^3$ is a time in seconds. Thus $K$ has units $\mathrm{s}^{5/3}$ and $Kf^{11/3}$ has units $\mathrm{s}^{-2}$, as required for [frequency](frequency.md) change per second. This model assumes weak gravity, slow relative motion, negligible [eccentricity of a conic](eccentricity-of-a-conic.md), no spin corrections and adiabatic evolution over an orbit. It does not describe merger or ringdown.

Separating variables gives a finite formal coalescence time $t_c$ and accumulated [wave phase](phase-waves.md) $\Phi$:

$$
\tau(f)=t_c-t=\frac{3}{8K}f^{-8/3},\qquad
f(t)=\left[\frac{8K}{3}(t_c-t)\right]^{-3/8},\qquad
\Phi(f)-\Phi(f_0)=\frac{6\pi}{5K}\left(f_0^{-5/3}-f^{-5/3}\right).
$$

Indeed $d\Phi/dt=2\pi f$; the formal divergence at $t_c$ signals extrapolation outside the approximation. Over a finite frequency interval, the number of [gravitational wave](gravitational-wave-split.md) cycles is $N=3(f_0^{-5/3}-f_1^{-5/3})/(5K)$. This accumulated phase is why a [chirp mass](chirp-mass.md) can be constrained even when distance and inclination remain entangled.

**Table of contents**

- [Chirp mass](chirp-mass.md)
- [Stipulated chirps and detector projections](stipulated-chirps-and-detector-projections.md)

## ↑ Ancestors (5)

1. [Gravitational wave](gravitational-wave-split.md)
2. [General relativity](general-relativity-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chirp mass](chirp-mass.md)
- [Newtonian binary chirp](newtonian-binary-chirp.md)
- [Stipulated chirps and detector projections](stipulated-chirps-and-detector-projections.md)
