# Exponential variational bound for a capped Coulomb potential

↑ **Parent:** [Quantum variational principle](quantum-variational-principle.md)

For $\kappa>0$ and the radial exponential trial state $e^{-\alpha r}$, $\alpha>0$, put $a=\hbar^2/(m\kappa)$. Direct radial integration gives the [Rayleigh quotient](rayleigh-quotient.md)

$$
E(\alpha)=\kappa\left[\frac{a\alpha^2}{2}
-\frac{1-(1+\alpha R)e^{-2\alpha R}}R\right].
$$

The kinetic expectation is $\hbar^2\alpha^2/(2m)$; the potential expectation follows by splitting its radial integral at $R$. The common prefactor cancels from the stationary condition, giving $a\alpha=(1+2\alpha R)e^{-2\alpha R}$. Its positive solution is unique, since the left side increases and the right side decreases. For $\varepsilon=R/a\to0$, it satisfies $a\alpha=1-2\varepsilon^2+O(\varepsilon^3)$.

The [quantum variational principle](quantum-variational-principle.md) makes $E(\alpha)$ an upper bound for the ground energy. The explicit choice $\alpha=1/a$ gives $E_0(R)\leq(\kappa/a)[1/2-\{1-(1+\varepsilon)e^{-2\varepsilon}\}/\varepsilon]$, whose first correction to $-\kappa/(2a)$ is $2\kappa R^2/(3a^3)$. The true energy is no lower than the point-Coulomb value because capping makes the potential less attractive.

## ↑ Ancestors (7)

1. [Quantum variational principle](quantum-variational-principle.md)
2. [Ground-state energy](ground-state-energy.md)
3. [Ground state](ground-state.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
