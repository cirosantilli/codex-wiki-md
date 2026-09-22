<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**Hamiltonian and [commutators](../../../../../commutator.md).** Use the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[\widehat x,\widehat p]=i\hbar I$ and define $c_0=\sqrt{m\omega/(2\hbar)}$. Expanding the product of the given [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md),

$$
\widehat a^\dagger\widehat a
=c_0^2\left(\widehat x^2+\frac{\widehat p^2}{m^2\omega^2}
+\frac{i}{m\omega}[\widehat x,\widehat p]\right)
=\frac{m\omega}{2\hbar}\widehat x^2
+\frac{\widehat p^2}{2m\hbar\omega}-\frac12I.
$$

Therefore the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is

$$
\boxed{\widehat H=\frac{\widehat p^2}{2m}+\frac12m\omega^2\widehat x^2
=\hbar\omega\left(\widehat a^\dagger\widehat a+\frac12I\right).}
$$

Similarly,

$$
[\widehat a,\widehat a^\dagger]
=c_0^2\left(-\frac{i}{m\omega}[\widehat x,\widehat p]
+\frac{i}{m\omega}[\widehat p,\widehat x]\right)=I.
$$

Using $[AB,C]=A[B,C]+[A,C]B$ gives

$$
\boxed{[\widehat a,\widehat a^\dagger]=I,\qquad
[\widehat H,\widehat a]=\hbar\omega[\widehat a^\dagger\widehat a,\widehat a]
=-\hbar\omega\widehat a.}
$$

**Lowering a normalized [energy](../../../../../energy-split.md) [eigenstate](../../../../../eigenstate.md).** The [commutator](../../../../../commutator.md) implies

$$
\widehat H\widehat a|\phi_n\rangle
=(E_n-\hbar\omega)\widehat a|\phi_n\rangle
=E_{n-1}\widehat a|\phi_n\rangle.
$$

For $n>0$, nondegeneracy of this one-dimensional [energy](../../../../../energy-split.md) level means $\widehat a|\phi_n\rangle=c_n|\phi_{n-1}\rangle$. Its norm is fixed by the [number operator](../../../../../number-operator.md):

$$
|c_n|^2=\langle\phi_n|\widehat a^\dagger\widehat a|\phi_n\rangle
=\frac{E_n}{\hbar\omega}-\frac12=n.
$$

Choosing successive [eigenstate](../../../../../eigenstate.md) phases in the conventional way makes $c_n=\sqrt n$, so

$$
\boxed{\widehat a|\phi_n\rangle=\sqrt n\,|\phi_{n-1}\rangle.}
$$

For $n=0$, the same norm is zero, hence $\widehat a|\phi_0\rangle=0$. A nonzero lowered [ground state](../../../../../ground-state.md) would have [energy](../../../../../energy-split.md) below the lowest allowed level, and positivity of $\widehat a^\dagger\widehat a$ forbids that possibility.

**Coherent-state [eigenvalue](../../../../../eigenvalue.md).** Applying the [annihilation operator](../../../../../annihilation-operator.md) term by term, with the $n=0$ contribution zero, gives

$$
\begin{aligned}
\widehat a|\chi_\alpha\rangle
&=e^{-|\alpha|^2/2}\sum_{n=1}^\infty
\frac{\alpha^n\sqrt n}{\sqrt{n!}}|\phi_{n-1}\rangle\\
&=\alpha e^{-|\alpha|^2/2}\sum_{r=0}^\infty
\frac{\alpha^r}{\sqrt{r!}}|\phi_r\rangle
=\alpha|\chi_\alpha\rangle.
\end{aligned}
$$

Thus

$$
\boxed{\widehat a|\chi_\alpha\rangle=\alpha|\chi_\alpha\rangle.}
$$

The [coherent state](../../../../../coherent-state.md) is normalized because $e^{-|\alpha|^2}\sum_n|\alpha|^{2n}/n!=1$. Its [annihilation operator](../../../../../annihilation-operator.md) is not Hermitian, so the [eigenvalue](../../../../../eigenvalue.md) $\alpha$ may be complex.

**Time evolution.** Under the time-independent [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), each [energy](../../../../../energy-split.md) component acquires its own phase:

$$
\begin{aligned}
|\chi_\alpha;t\rangle
&=e^{-|\alpha|^2/2}\sum_{n=0}^\infty
\frac{\alpha^n}{\sqrt{n!}}e^{-i(n+1/2)\omega t}|\phi_n\rangle\\
&=e^{-i\omega t/2}e^{-|\alpha|^2/2}\sum_{n=0}^\infty
\frac{(\alpha e^{-i\omega t})^n}{\sqrt{n!}}|\phi_n\rangle.
\end{aligned}
$$

Since $|\alpha e^{-i\omega t}|=|\alpha|$, the normalization prefactor is unchanged. Hence

$$
\boxed{|\chi_\alpha;t\rangle=e^{-i\omega t/2}|\chi_\beta\rangle,
\qquad\beta=\alpha e^{-i\omega t}.}
$$

The state remains a [coherent state](../../../../../coherent-state.md), with its complex parameter rotating at the oscillator's [angular frequency](../../../../../angular-frequency.md); the displayed extra factor is a global phase from the zero-point [energy](../../../../../energy-split.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
