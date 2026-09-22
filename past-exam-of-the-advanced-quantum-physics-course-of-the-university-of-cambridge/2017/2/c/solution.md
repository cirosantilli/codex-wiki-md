<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [coherent state](../../../../coherent-state.md) is a normalized [eigenstate](../../../../eigenstate.md) of the [annihilation operator](../../../../annihilation-operator.md), $a|\alpha\rangle=\alpha|\alpha\rangle$. Expanding in the [Fock state](../../../../fock-state.md) [eigenbasis](../../../../eigenbasis.md) gives a recurrence $c_{n+1}=\alpha c_n/\sqrt{n+1}$, and [wavefunction normalization](../../../../wavefunction-normalization.md) fixes

$$
|\alpha\rangle=e^{-|\alpha|^2/2}\sum_{n=0}^\infty\frac{\alpha^n}{\sqrt{n!}}|n\rangle
=D(\alpha)|0\rangle,\qquad
D(\alpha)=e^{\alpha a^\dagger-\alpha^*a}.
$$

The [displacement operator](../../../../displacement-operator.md) therefore shifts the oscillator [ground state](../../../../ground-state.md) in [phase space](../../../../phase-space.md). Distinct [coherent states](../../../../coherent-state.md) are not orthogonal:

$$
\langle\alpha|\beta\rangle=
\exp\left[-\frac{|\alpha|^2+|\beta|^2}{2}+\alpha^*\beta\right].
$$

The occupation probabilities form a [Poisson distribution](../../../../poisson-distribution.md),

$$
P_n=e^{-N}\frac{N^n}{n!},\qquad N=|\alpha|^2,
\qquad \langle n\rangle=N,\quad (\Delta n)^2=N.
$$

For the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md), the [expectation values](../../../../expectation-value.md) of position and momentum are

$$
\langle x\rangle=\sqrt{\frac{2\hbar}{m\omega}}\operatorname{Re}\alpha,\qquad
\langle p\rangle=\sqrt{2m\hbar\omega}\operatorname{Im}\alpha.
$$

The fluctuations equal those of the [ground state](../../../../ground-state.md),

$$
(\Delta x)^2=\frac{\hbar}{2m\omega},\qquad
(\Delta p)^2=\frac{m\hbar\omega}{2},\qquad
\boxed{\Delta x\,\Delta p=\frac{\hbar}{2}}.
$$

Thus the position [wavefunction](../../../../wave-function-split.md) is a displaced [Gaussian wave packet](../../../../gaussian-wave-packet.md) that saturates the [Heisenberg uncertainty principle](../../../../heisenberg-uncertainty-relation.md).

Time evolution under $H=\hbar\omega(a^\dagger a+1/2)$ preserves this form:

$$
\boxed{e^{-iHt/\hbar}|\alpha\rangle=e^{-i\omega t/2}|\alpha e^{-i\omega t}\rangle}.
$$

The center follows the classical oscillator trajectory while the packet width stays constant. Its mean [energy](../../../../energy-split.md) is $\hbar\omega(N+1/2)$; it is generally a superposition of [energy eigenstates](../../../../energy-eigenstate.md), rather than a state of definite [energy](../../../../energy-split.md). For $N\gg1$, the relative occupation fluctuation is $1/\sqrt N$, explaining the classical appearance of a highly excited [coherent state](../../../../coherent-state.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
