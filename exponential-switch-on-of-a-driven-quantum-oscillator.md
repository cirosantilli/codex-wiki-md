# Exponential switch-on of a driven quantum oscillator

↑ **Parent:** [Displaced quantum harmonic oscillator](displaced-quantum-harmonic-oscillator.md)

For $H(t)=\hbar\omega(a^\dagger a+1/2)-Fx e^{t/\tau}$ on $t\leq0$, start in the unforced [ground state](ground-state.md) at $t=-\infty$. Define $x_{01}=\sqrt{\hbar/(2m\omega)}$ and $\eta=Fx_{01}/(\hbar\omega)$. [Time-dependent perturbation theory](time-dependent-perturbation-theory.md) gives

$$
c_1(0)=\frac{iFx_{01}}\hbar\int_{-\infty}^0 e^{(1/\tau+i\omega)t}\,dt=\frac{i\eta\omega\tau}{1+i\omega\tau}.
$$

Thus the first excited-state probability in the original oscillator basis tends to zero for a rapid turn-on and to $\eta^2$ for slow turn-on, within the weak-force approximation $|\eta|\ll1$.

This finite adiabatic limit is not a failure of the [adiabatic theorem](adiabatic-theorem.md): the instantaneous [ground state](ground-state.md) is displaced and has a nonzero projection onto the original excited states. In fact a linear force preserves a [coherent state](coherent-state.md), whose exact original-basis displacement at $t=0$ is $\alpha=i\eta\omega\tau/(1+i\omega\tau)$. It follows either from $\dot\alpha=-i\omega\alpha+iFx_{01}e^{t/\tau}/\hbar$ or from the forced oscillator equations. Consequently the exact original-basis probability is $P_1^{(0)}=|\alpha|^2e^{-|\alpha|^2}$. The instantaneous oscillator basis has displacement $\eta$, so its mean excitation is instead $|\alpha-\eta|^2=\eta^2/[1+(\omega\tau)^2]$, which vanishes adiabatically.

## ↑ Ancestors (6)

1. [Displaced quantum harmonic oscillator](displaced-quantum-harmonic-oscillator.md)
2. [Quantum harmonic oscillator](quantum-harmonic-oscillator-split.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018/section-b/b2/solution.md)
