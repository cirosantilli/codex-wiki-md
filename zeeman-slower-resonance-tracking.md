# Zeeman slower resonance tracking

↑ **Parent:** [Zeeman slower](zeeman-slower.md)

A [Zeeman slower](zeeman-slower.md) prepares a slow beam for capture; a narrow longitudinal [velocity](velocity.md) group is not by itself a cold three-dimensional cloud. The historical apparatus measured slowed-beam [velocities](velocity.md) with a separate [fluorescence](fluorescence-split.md) probe scanned in [frequency](frequency.md), just after switching off the slowing beam. This avoided simultaneous-beam complications.[p. 724, Figs. 4–5](nobel-lecture-laser-cooling-and-trapping-of-neutral-atoms-by-william-d-phillips.md)

For an original resonance-tracking calculation, let atoms travel along $+z$ with $v>0$ and the slowing beam along $-z$, so its atom-frame [angular frequency](angular-frequency.md) is $\omega_L+kv$. Approximate the selected cycling transition by $\omega_{eg}(B)=\omega_0+\zeta B$ on one field branch; $\zeta$ is its signed [angular frequency](angular-frequency.md) shift per unit [magnetic field](magnetic-field-split.md). A multilevel atom may require a nonlinear $\omega_{eg}(B)$ outside that branch. Maintaining a chosen effective [laser detuning](laser-detuning.md) $\delta_s$ requires

$$
B(z)=\frac{\omega_L-\omega_0+kv(z)-\delta_s}{\zeta}.
$$

For chosen constant deceleration magnitude $a>0$, $v\,dv/dz=-a$ gives $v(z)=\sqrt{v_i^2-2az}$ and length $L=(v_i^2-v_f^2)/(2a)$. Substitution supplies a square-root [magnetic field](magnetic-field-split.md) profile, plus a constant offset. The signs follow from the specified directions; reversing the selected transition's magnetic slope reverses the required field variation.

As a hypothetical design, take $v_i=300\ \mathrm{m\,s^{-1}}$, $v_f=30\ \mathrm{m\,s^{-1}}$ and $a=5.0\times10^4\ \mathrm{m\,s^{-2}}$. The required length is $0.891\ \mathrm m$ and flight time $(v_i-v_f)/a=5.4\ \mathrm{ms}$. For chosen $\lambda=589\ \mathrm{nm}$ and $m=3.82\times10^{-26}\ \mathrm{kg}$, [photon](photon.md) recoil [velocity](velocity.md) $\hbar k/m\simeq0.0294\ \mathrm{m\,s^{-1}}$ implies roughly $9.17\times10^3$ directed absorption events. The mean required scattering rate is about $1.70\times10^6\ \mathrm{s^{-1}}$. This budget must lie below the available scattering rate, with margin for capture and intensity variation. [Optical pumping](optical-pumping.md) into unwanted [hyperfine structure](hyperfine-structure.md) or [magnetic sublevels](magnetic-sublevel.md) can interrupt the cycle. Longitudinal slowing, transverse recoil heating and final cloud [temperature](temperature-split.md) are separate quantities.

## ↑ Ancestors (6)

1. [Zeeman slower](zeeman-slower.md)
2. [Laser cooling](laser-cooling.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
