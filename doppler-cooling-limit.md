# Doppler cooling limit

↑ **Parent:** [Doppler cooling](doppler-cooling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doppler_cooling_limit)

[Damping](damping.md) removes random [kinetic energy](kinetic-energy.md), but the discrete [photon](photon.md) kicks cause [diffusion](diffusion.md) in [momentum](momentum-split.md). Their balance gives a nonzero [temperature](temperature-split.md). Define the momentum diffusion coefficient $D_p$ by the noise contribution $d\langle p_x^2\rangle/dt=2D_p$. With atom [mass](mass.md) $m$ and linear [damping](damping.md) coefficient $\alpha$,

$$
\frac{d\langle p_x^2\rangle}{dt}=-\frac{2\alpha}{m}\langle p_x^2\rangle+2D_p,\qquad
k_BT=\frac{\langle p_x^2\rangle}{m}=\frac{D_p}{\alpha}
$$

at stationary balance, where $k_B$ is the [Boltzmann constant](boltzmann-constant.md) and mean [momentum](momentum-split.md) is zero.

For ideal three-dimensional [optical molasses](optical-molasses.md) with three identical independent beam pairs and isotropic [spontaneous emission](spontaneous-emission.md), the $x$-pair absorption rate at rest is $R_x=\Gamma s/(1+4d^2)$. Absorption from that pair contributes $(\hbar k)^2R_x$ to the noise growth of $\langle p_x^2\rangle$. Emission from all three pairs contributes the same amount: its total rate is $3R_x$ and each emitted [photon](photon.md) has mean squared $x$-[momentum](momentum-split.md) $(\hbar k)^2/3$. Hence $D_p=(\hbar k)^2R_x$. Using the [Doppler cooling force](doppler-cooling-force.md) coefficient gives

$$
T(d)=\frac{\hbar\Gamma}{8k_B}\frac{1+4d^2}{-d},\qquad d<0.
$$

Put $a=-d>0$. Then $(1+4d^2)/(-d)=a^{-1}+4a\ge4$, with equality at $a=1/2$. The ideal weak-field [Doppler cooling limit](doppler-cooling-limit.md) is therefore $T_D=\hbar\Gamma/(2k_B)$ at $\delta=-\Gamma/2$. It is the minimum of this specified diffusion-and-[damping](damping.md) model, rather than a universal lower bound for [laser cooling](laser-cooling.md). The diffusion approximation also assumes [recoil energy](recoil-energy.md) much smaller than $\hbar\Gamma$. In a one-pair geometry, emission patterns and transverse recoil change the diffusion bookkeeping. [William D. Phillips, Nobel Lecture: Laser cooling and trapping of neutral atoms, 1998, pp. 729–730, Eqs. (1)–(2): recoil heating, linewidth convention and ideal three-dimensional temperature limit](nobel-lecture-laser-cooling-and-trapping-of-neutral-atoms-by-william-d-phillips.md).

## ↑ Ancestors (6)

1. [Doppler cooling](doppler-cooling.md)
2. [Laser cooling](laser-cooling.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Doppler cooling limit](doppler-cooling-limit.md)
- [Optical molasses experiment of 1985](optical-molasses-experiment-of-1985.md)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1/3/a/solution.md)
- [Sub-Doppler cooling](sub-doppler-cooling.md)
- [Sub-Doppler cooling discovery thermometry](sub-doppler-cooling-discovery-thermometry.md)
