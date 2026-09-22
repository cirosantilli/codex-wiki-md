# Gaussian covariance in a harmonic potential

↑ **Parent:** [Gaussian wave packet](gaussian-wave-packet.md)

Under a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) Hamiltonian, the [Heisenberg equations of motion](heisenberg-equation-of-motion.md) give

$$
x(t)=x(0)\cos\omega t+\frac{p(0)}{m\omega}\sin\omega t,\qquad p(t)=p(0)\cos\omega t-m\omega x(0)\sin\omega t.
$$

Subtract the [expectation values](expectation-value.md), square the first equation, and use the symmetrized [covariance](covariance.md) $C_0=\langle\{x-\langle x\rangle,p-\langle p\rangle\}\rangle/2$. This yields

$$
\sigma_x(t)^2=\sigma_x(0)^2\cos^2\omega t+\frac{\sigma_p(0)^2}{m^2\omega^2}\sin^2\omega t+\frac{2C_0}{m\omega}\sin\omega t\cos\omega t.
$$

These moment equations hold for any state with finite second moments; a quadratic Hamiltonian additionally preserves [Gaussian wave packets](gaussian-wave-packet.md). A [coherent state](coherent-state.md) has $\sigma_x(0)^2=\hbar/(2m\omega)$, $\sigma_p(0)^2=m\hbar\omega/2$, and $C_0=0$, so its width stays fixed while its center follows the classical orbit. A [squeezed coherent state](squeezed-coherent-state.md) generally has a width that oscillates at $2\omega$.

## ↑ Ancestors (6)

1. [Gaussian wave packet](gaussian-wave-packet.md)
2. [Wave function](wave-function-split.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
