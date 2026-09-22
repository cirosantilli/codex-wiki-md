<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use units $\hbar=1$. A Hermitian quadrature coupling of a cavity mode to a continuum of external modes can be written

$$
H_{\mathrm{couple}}=i\int d\omega\,\kappa(\omega)(a+a^\dagger)\otimes(b_\omega^\dagger-b_\omega),
$$

with real coupling amplitude $\kappa$. The free [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) is $H_0=\omega_ca^\dagger a+\int\omega b_\omega^\dagger b_\omega\,d\omega$. In the [interaction picture](../../../../../../interaction-picture.md), the two photon-exchange products $ab_\omega^\dagger$ and $a^\dagger b_\omega$ acquire phases with frequency $\omega-\omega_c$, whereas $a^\dagger b_\omega^\dagger$ and $ab_\omega$ oscillate at $\omega+\omega_c$.

For weak coupling near resonance, the [rotating-wave approximation](../../../../../../rotating-wave-approximation.md) drops those rapidly oscillating pair-creation and pair-annihilation terms and retains

$$
H_I(t)=i\int d\omega\,\kappa(\omega)\{a\otimes b_\omega^\dagger e^{i(\omega-\omega_c)t}-a^\dagger\otimes b_\omega e^{-i(\omega-\omega_c)t}\}.
$$

For a broadband flat coupling $\kappa=\sqrt{\gamma/(2\pi)}$, define the envelope [annihilation operator](../../../../../../annihilation-operator.md) $b(t)=(2\pi)^{-1/2}\int b_\omega e^{-i(\omega-\omega_c)t}d\omega$. The [Markov approximation](../../../../../../markov-approximation-for-a-random-medium.md) extends the detuning integral over the full real line and gives $[b(t),b^\dagger(s)]=\delta(t-s)$. Then the [cavity-reservoir interaction](../../../../../../cavity-reservoir-interaction.md) is

$$
\boxed{H_I(t)=i\sqrt\gamma\{a(t)\otimes b^\dagger(t)-a^\dagger(t)\otimes b(t)\}.}
$$

The phases and normalization of the external field fix the sign convention. The [creation operators](../../../../../../creation-operator.md) and [annihilation operators](../../../../../../annihilation-operator.md) exchange one excitation between cavity and field, rather than creating or destroying a pair.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
