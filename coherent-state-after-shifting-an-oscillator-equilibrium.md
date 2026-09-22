# Coherent state after shifting an oscillator equilibrium

↑ **Parent:** [Coherent state](coherent-state.md)

Suddenly shifting a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) equilibrium from zero to a signed position $x_0$ leaves the old [ground state](ground-state.md) unchanged at the instant of the [quantum quench](quantum-quench.md). The new [annihilation operator](annihilation-operator.md) is $a'=a-\lambda$, with $\lambda=\sqrt{m\omega/(2\hbar)}x_0$, so $a'|0\rangle=-\lambda|0\rangle$. In the translated [energy eigenstates](energy-eigenstate.md) $|n'\rangle=e^{-ipx_0/\hbar}|n\rangle$, the expansion is

$$
|0\rangle=e^{-\lambda^2/2}\sum_{n=0}^\infty\frac{(-\lambda)^n}{\sqrt{n!}}|n'\rangle.
$$

The sign follows by translating the old vacuum by $-x_0$ before expanding it in the old [Fock states](fock-state.md). A [Baker--Campbell--Hausdorff formula](baker-campbell-hausdorff-formula.md) with central [commutator](commutator.md) separates the resulting exponential into creation and annihilation parts. Evolution with the shifted [Hamiltonian](hamiltonian.md) preserves this [coherent state](coherent-state.md), with $\alpha(t)=\alpha_0e^{-i\omega t}$. Its mean occupation is $|\alpha_0|^2$ and its mean energy above the new potential minimum is $\hbar\omega(|\alpha_0|^2+1/2)$. Omitting $(-\lambda)^n$ in favour of $|\lambda|^n$ changes the state when $x_0>0$.

## ↑ Ancestors (5)

1. [Coherent state](coherent-state.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2017/2/c/solution.md)
- [Solution](past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2018/4/c/solution.md)
