# Ionospheric virtual height

↑ **Parent:** [Cold-plasma radio dispersion](cold-plasma-radio-dispersion.md)

For a vertical outgoing and returning [radio wave](radio-wave.md), define the virtual height $h'=c\tau_g/2$ from its round-trip [group delay](group-delay.md) $\tau_g$, after removing instrument delays. It is the height a fictitious reflector would have if both legs traveled at $c$. It differs from both the real turning height $z_t$ and a height fitted to an oblique constant-path [interference fringe](interference-fringe.md) model.

An original solvable profile makes the difference explicit. Approximate the region below $z_0$ by $n=1$, and prescribe a linear rise of squared [plasma frequency](plasma-frequency.md) above it:

$$
\omega_p^2(z)=a(z-z_0),\qquad a>0,\qquad
u_t=\frac{\omega^2}{a},\qquad z_t=z_0+u_t.
$$

Here the symbol $u_t$ denotes the penetration depth, and $a$ has units $\mathrm{s^{-2}\,m^{-1}}$. In the propagating part of the ramp, $n=\sqrt{1-(z-z_0)/u_t}$. In the leading geometrical-ray delay model, with a frequency-independent turning connection [wave phase](phase-waves.md), the round-trip [group delay](group-delay.md) is

$$
\tau_g=\frac2c\left[z_0+\int_0^{u_t}\frac{du}{\sqrt{1-u/u_t}}\right]
=\frac2c(z_0+2u_t),\qquad
h'=z_0+2u_t=2z_t-z_0>z_t.
$$

The endpoint singularity is integrable: substitute $s=\sqrt{1-u/u_t}$ to obtain $2u_t$. This approximation does not resolve the finite-wavelength structure at the turning region. It illustrates the effect of slow [group velocity](group-velocity.md) before the return, rather than adding extra geometric altitude.

As an independent phase-based derivation, the propagation contribution to the round-trip [wave phase](phase-waves.md) is

$$
\Psi(\omega)=\frac{2\omega}{c}\left[z_0+\int_0^{u_t}\sqrt{1-u/u_t}\,du\right]
=\frac{2\omega}{c}\left(z_0+\frac23\frac{\omega^2}{a}\right).
$$

Its [derivative](derivative.md) $d\Psi/d\omega=2(z_0+2\omega^2/a)/c$ agrees with the delay [integral](integral-split.md). Using the phase integral itself as a distance at speed $c$ would give $z_0+2u_t/3$ instead of $h'$: [wave phase](phase-waves.md), [group delay](group-delay.md) and real turning height are three different quantities.

Choose $z_0=70\,\mathrm{km}$ and stipulate $f_p(z)=3\,\mathrm{MHz}\sqrt{(z-z_0)/(30\,\mathrm{km})}$, where $f_p=\omega_p/(2\pi)$. Then

$$
z_t=70\,\mathrm{km}+30\,\mathrm{km}\left(\frac{f}{3\,\mathrm{MHz}}\right)^2,\qquad
h'=70\,\mathrm{km}+60\,\mathrm{km}\left(\frac{f}{3\,\mathrm{MHz}}\right)^2.
$$

At $f=3\,\mathrm{MHz}$, the real turning height is $100\,\mathrm{km}$ but the virtual height is $130\,\mathrm{km}$, corresponding to $\tau_g\simeq0.867\,\mathrm{ms}$ with $c\simeq3.00\times10^8\,\mathrm{m\,s^{-1}}$. These stipulated parameters describe neither a measured profile nor a separate physical reflector at $130\,\mathrm{km}$. Because the ramp has no density maximum, it also has no finite upper penetration threshold; a real bounded [E layer](e-layer.md) or [F layer](f-layer.md) requires a richer profile.

<a id="image-cold-plasma-radio-dispersion-separates-real-turning-height-from-ionospheric-virtual-height"></a>
![](ionosphere-dispersive-virtual-height.png)

**[Figure 6](#image-cold-plasma-radio-dispersion-separates-real-turning-height-from-ionospheric-virtual-height). Cold-plasma radio dispersion separates real turning height from ionospheric virtual height**. Original linear-density-ramp model: the refractive index falls to zero at the 3 MHz turning point, while the group refractive index rises. The right panel shows the real turning height and the larger delay-derived virtual height as frequency changes. The 100 km and 130 km values are illustrative model outputs.

## ↑ Ancestors (7)

1. [Cold-plasma radio dispersion](cold-plasma-radio-dispersion.md)
2. [Ionosphere](ionosphere.md)
3. [Upper atmosphere](upper-atmosphere.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ionosphere](ionosphere.md)
- [Ionospheric virtual height](ionospheric-virtual-height.md)
