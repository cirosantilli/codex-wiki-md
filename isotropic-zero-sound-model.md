# Isotropic zero-sound model

↑ **Parent:** [Zero sound](zero-sound.md)

Consider a neutral, isotropic, unpolarized three-dimensional spin-one-half [Fermi liquid](fermi-liquid-split.md), with only $F_0^s>0$ nonzero. A longitudinal density wave with [angular frequency](angular-frequency.md) $\omega$ and [wavevector](wavevector.md) magnitude $q$ has $s=\omega/(qv_F)=c_0/v_F$. The collisionless angular equation for the energy displacement $\nu(u)$ of the [Fermi surface](fermi-surface.md) is

$$
(s-u)\nu(u)=uF_0^s\langle\nu\rangle,\qquad \langle\nu\rangle=\frac12\int_{-1}^1\nu(u)\,du,\qquad u=\cos\theta.
$$

Averaging gives

$$
1=\frac{F_0^s}{2}\int_{-1}^{1}\frac{u}{s-u}\,du=F_0^s\left[\frac{s}{2}\log\frac{s+1}{s-1}-1\right].
$$

The bracket decreases from infinity to zero on $1<s<\infty$: each $F_0^s>0$ gives one undamped root above the small-$q$ [particle-hole continuum](particle-hole-continuum.md).[Section 1, equations (11)–(15), pp.103–104](oscillations-in-a-fermi-liquid-by-lev-davidovich-landau.md)

For an original example, $F_0^s=2$ gives $s=1.16474145$. Since $F_1^s=0$ here, the [Principle of Galilean relativity](principle-of-galilean-relativity.md) gives $m^*=m$ and taking the hydrodynamic limit before $T\to0$ gives $c_1/v_F=\sqrt{(1+F_0^s)/3}=1$. Stipulating $v_F=50\ \mathrm{m\,s^{-1}}$ gives $c_0\simeq58.24\ \mathrm{m\,s^{-1}}$ and $c_1=50\ \mathrm{m\,s^{-1}}$. These are model choices, not [helium-3](helium-3.md) measurements. At large $F_0^s$, expanding the logarithm gives $s\sim\sqrt{F_0^s/3}$; for small positive $F_0^s$, the root approaches $1$ exponentially closely, so numerical resolution matters. A charged [electron](electron.md) liquid needs its long-range interaction included; this neutral model is not its long-wavelength density mode.

<a id="image-collisionless-zero-sound-root-and-the-first-sound-collision-condition"></a>
![](fermi-liquid-zero-sound-root-and-collision-regimes.png)

**[Figure 4](#image-collisionless-zero-sound-root-and-the-first-sound-collision-condition). Collisionless zero-sound root and the first-sound collision condition**. Original three-dimensional $F_0^s$-only model. [Zero sound](zero-sound.md) and [first sound](first-sound.md) speeds refer to their respective limits, rather than two simultaneous solutions at a fixed collision rate. The lower panel stipulates $\omega\tau=(T/T_\times)^{-2}$ at fixed [angular frequency](angular-frequency.md); its crossover is not measured [helium-3](helium-3.md) data.

## ↑ Ancestors (6)

1. [Zero sound](zero-sound.md)
2. [Fermi liquid](fermi-liquid-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
