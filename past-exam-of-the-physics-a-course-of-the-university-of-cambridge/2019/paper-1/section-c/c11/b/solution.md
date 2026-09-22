<h1 id="section-c/c11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Schrödinger picture](../../../../../../schrodinger-picture.md), a time-independent [Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) gives $|\psi_S(t)\rangle=U(t)|\psi(0)\rangle$, where $U=e^{-iHt/\hbar}$. The [Heisenberg picture](../../../../../../heisenberg-picture.md) transfers this evolution to each [observable](../../../../../../observable.md):

$$
A_H(t)=U^\dagger(t)A_S(t)U(t),\qquad |\psi_H\rangle=|\psi(0)\rangle.
$$

Both pictures give the same [probabilities](../../../../../../probability.md) and [expectation values](../../../../../../expectation-value.md). Differentiating yields the [Heisenberg equation of motion](../../../../../../heisenberg-equation-of-motion.md)

$$
\boxed{\frac{dA_H}{dt}=\frac{i}{\hbar}[H_H,A_H]+U^\dagger\frac{\partial A_S}{\partial t}U.}
$$

The last term is an explicit change of the measured operator. If it is absent and $[H,A]=0$, the [observable](../../../../../../observable.md) is conserved.

The corresponding classical equation is $dA/dt=\{A,H\}_{\mathrm{PB}}+\partial A/\partial t$. The [correspondence principle](../../../../../../correspondence-principle.md) relates the [Poisson bracket](../../../../../../poisson-bracket.md) to $[A,H]/(i\hbar)$, with suitable operator ordering and a [classical limit](../../../../../../classical-limit.md). For $H=p^2/(2m)+V(x)$, the [canonical commutation relation](../../../../../../canonical-commutation-relation.md) gives

$$
\dot x_H=\frac{p_H}{m},\qquad \dot p_H=-V'(x_H).
$$

Taking means gives [Ehrenfest theorem](../../../../../../ehrenfest-theorem.md). Its second equation contains $-\langle V'(x)\rangle$, which need not equal $-V'(\langle x\rangle)$. A narrow [wave packet](../../../../../../wave-packet.md) in a slowly varying force field can follow the classical equations approximately; a quadratic potential makes the equality exact for the means.

For a [quantum harmonic oscillator](../../../../../../quantum-harmonic-oscillator-split.md), direct solution gives $x_H(t)=x_H(0)\cos\omega t+p_H(0)\sin\omega t/(m\omega)$ and $p_H(t)=p_H(0)\cos\omega t-m\omega x_H(0)\sin\omega t$. These have the classical form as operator identities. A [coherent state](../../../../../../coherent-state.md) supplies a localized center moving on the classical orbit, whereas an [energy eigenstate](../../../../../../energy-eigenstate.md) has stationary density and $\langle x\rangle=0$, even at large excitation. Thus large quantum numbers alone do not create a localized classical trajectory. Classical behavior also concerns state preparation, relative fluctuations and the resolution of the measurements.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
