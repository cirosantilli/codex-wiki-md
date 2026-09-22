<h1 id="32c/solution">Solution</h1>

↑ **Parent:** [32C](../32c.md)

Define interaction-picture states by $|\psi_I(t)\rangle=e^{iH_0t/\hbar}|\psi_S(t)\rangle$ and $V_I(t)=e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}$. Differentiation cancels the free [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) and yields

$$
\boxed{i\hbar\frac d{dt}|\psi_I(t)\rangle=\lambda V_I(t)|\psi_I(t)\rangle.}
$$

Assume the interaction is switched off sufficiently fast in the remote past for the following integral to converge. Starting in $|n\rangle$, the first iteration of the [integral equation](../../../../../integral-equation.md) gives

$$
\langle m|\psi_I(t)\rangle=-\frac{i\lambda}{\hbar}\int_{-\infty}^t\langle m|V(t')|n\rangle e^{i(E_m-E_n)t'/\hbar}\,dt'+O(\lambda^2)
$$

for $m\ne n$. The picture change only multiplies the measured amplitude by a phase. Squaring therefore gives

$$
\boxed{P_{n\to m}(t)=\frac{\lambda^2}{\hbar^2}\left|\int_{-\infty}^t\langle m|V(t')|n\rangle e^{i(E_m-E_n)t'/\hbar}\,dt'\right|^2+O(\lambda^3).}
$$

For the [harmonic oscillator](../../../../../simple-harmonic-motion.md), $|1\rangle=a^\dagger|0\rangle$ is normalized and $\langle1|(a+a^\dagger)|0\rangle=1$. The energy difference is $\hbar\omega$, and

$$
\int_{-\infty}^{\infty}e^{-p|t|}e^{i\omega t}\,dt=\frac1{p+i\omega}+\frac1{p-i\omega}=\frac{2p}{p^2+\omega^2}.
$$

Hence the lowest nonzero [transition probability](../../../../../transition-probability.md) is

$$
\boxed{P_{0\to1}(\infty)=\frac{4\lambda^2p^2}{\hbar^2(p^2+\omega^2)^2}+O(\lambda^4).}
$$

The stronger remainder here follows from [parity](../../../../../parity.md): every insertion of $a+a^\dagger$ reverses oscillator [parity](../../../../../parity.md), so the amplitude between $|0\rangle$ and $|1\rangle$ has only odd powers of $\lambda$. The general displayed $O(\lambda^3)$ estimate remains valid.

## ↑ Ancestors (10)

1. [32C](../32c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
