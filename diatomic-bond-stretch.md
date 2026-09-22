# Diatomic bond stretch

↑ **Parent:** [Molecular vibration](molecular-vibration.md)

Let $r$ be the instantaneous [bond length](bond-length.md), $r_e>0$ its equilibrium value, and $q=r-r_e$ the stretching [displacement](displacement.md). Assume one fixed electronic [quantum state](quantum-state.md), a smooth [potential energy](potential-energy.md) $V(r)$ with a nondegenerate [local minimum](local-minimum.md) at $r_e$, and omit [molecular rotation](molecular-rotation.md) initially. The [Taylor series](taylor-series.md) has no linear term because $V'(r_e)=0$:

$$
V(r_e+q)=V_0+\frac12kq^2+O(q^3),\qquad
V_0=V(r_e),\qquad k=V''(r_e)>0.
$$

Keeping only the quadratic term is the [harmonic approximation near a potential minimum](harmonic-approximation-near-a-potential-minimum.md). The [bond force constant](bond-force-constant.md) $k$ has units $\mathrm{N\,m^{-1}}$. It measures local stiffness; it is not the [bond-dissociation energy](bond-dissociation-energy.md), which concerns the depth and distant shape of the entire well.

The [two-particle relative coordinate](two-particle-relative-coordinate.md) explains the [reduced mass](reduced-mass.md). For stretching along a fixed axis in a stationary [centre of mass](center-of-mass.md) frame, let $u_1,u_2$ be the nuclear [displacements](displacement.md) from equilibrium. Then $u_2-u_1=q$ and $m_1u_1+m_2u_2=0$, so

$$
u_1=-\frac{m_2}{m_1+m_2}q,\qquad
u_2=\frac{m_1}{m_1+m_2}q,\qquad
T=\frac12m_1\dot u_1^2+\frac12m_2\dot u_2^2=\frac12\mu\dot q^2,\qquad
\mu=\frac{m_1m_2}{m_1+m_2}.
$$

Here $T$ is the internal [kinetic energy](kinetic-energy.md), and $m_1,m_2>0$ are the two nuclear [masses](mass.md). The lighter partner moves farther; the [reduced mass](reduced-mass.md) is smaller than either individual [mass](mass.md). The restoring [force](force-split.md) $-dV/dq\simeq-kq$ gives [simple harmonic motion](simple-harmonic-motion.md):

$$
\mu\ddot q=-kq,\qquad
q(t)=A\cos(\omega t+\phi),\qquad
\omega=\sqrt{\frac{k}{\mu}},\qquad
\nu=\frac{\omega}{2\pi},\qquad
\widetilde\nu_{\rm harm}=\frac{\omega}{2\pi c}.
$$

The [angular frequency](angular-frequency.md) is $\omega$, the ordinary [frequency](frequency.md) is $\nu$, and $\widetilde\nu_{\rm harm}$ is the corresponding [spectroscopic wavenumber](spectroscopic-wavenumber.md); $c$ is the [speed of light](speed-of-light.md). Use $c$ in $\mathrm{cm\,s^{-1}}$ to obtain $\widetilde\nu_{\rm harm}$ in $\mathrm{cm^{-1}}$. The symbol $k$ here is a [bond force constant](bond-force-constant.md), not an angular [wavenumber](wavenumber.md).

For an original dimensionless example, choose $m_1=m_2=2$ and $k=4$ in consistent model units. Then $\mu=1$ and $\omega=2$. Releasing at $q(0)=0.1$ with $\dot q(0)=0$ gives $q(t)=0.1\cos(2t)$ and $u_1=-q/2$, $u_2=q/2$. Each [atomic nucleus](atomic-nucleus-split.md) moves only half the stretching [amplitude](wave-amplitude.md), while the conserved internal [mechanical energy](mechanical-energy.md) above $V_0$ is $\frac12k(0.1)^2=0.02$. Fixing one partner instead would give $\omega=\sqrt2$, demonstrating why a one-body calculation changes the model.

**Table of contents**

- [Bond force constant](bond-force-constant.md)
- [Harmonic vibrational energy levels](harmonic-vibrational-energy-levels.md)
- [HCl and DCl harmonic stretch comparison](hcl-and-dcl-harmonic-stretch-comparison.md)

## ↑ Ancestors (4)

1. [Molecular vibration](molecular-vibration.md)
2. [Molecule](molecule-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Bond force constant](bond-force-constant.md)
- [HCl and DCl harmonic stretch comparison](hcl-and-dcl-harmonic-stretch-comparison.md)
- [Molecular vibration](molecular-vibration.md)
- [Vibrational infrared activity](vibrational-infrared-activity.md)
