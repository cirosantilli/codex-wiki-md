<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $U(t)=e^{-iHt/\hbar}$ and take an observable with no explicit time dependence. In the [Schrödinger picture](../../../schrodinger-picture.md), $\psi_S(t)=U(t)\psi_0$ and $A_S=A$. In the [Heisenberg picture](../../../heisenberg-picture.md), $\psi_H=\psi_0$ and $A_H(t)=U(t)^\dagger A U(t)$. For the [interaction picture](../../../interaction-picture.md) choose a time-independent splitting $H=H_0+V$, put $U_0=e^{-iH_0t/\hbar}$, and define

$$
\psi_I=U_0^\dagger\psi_S,\qquad A_I=U_0^\dagger A U_0,\qquad V_I=U_0^\dagger VU_0.
$$

Then $i\hbar\dot\psi_I=V_I\psi_I$ and $\dot A_I=(i/\hbar)[H_0,A_I]$. Unitarity gives the identical [expectation](../../../expected-value-split.md) in all three descriptions:

$$
\boxed{\langle\psi_S,A\psi_S\rangle=\langle\psi_0,A_H\psi_0\rangle=\langle\psi_I,A_I\psi_I\rangle.}
$$

Different choices of the split interpolate between pictures; $H_0=H$ makes the state constant, while $H_0=0$ gives the Schrödinger description.

Differentiate $U^\dagger AU$ to obtain the [Heisenberg equation of motion](../../../heisenberg-equation-of-motion.md)

$$
\boxed{\dot A_H=\frac{i}{\hbar}[H,A_H].}
$$

For an explicitly time-dependent observable there is additionally $U^\dagger(\partial_tA)U$. Thus $H_H=H$ is constant. In a normalized [energy](../../../energy-split.md) [eigenstate](../../../eigenstate.md), $\langle[H,A_H]\rangle=E\langle A_H\rangle-E\langle A_H\rangle=0$, so the [expectation](../../../expected-value-split.md) of its Heisenberg derivative vanishes whenever the products are defined.

For the [harmonic oscillator](../../../simple-harmonic-motion.md), the canonical [commutator](../../../commutator.md) gives

$$
\boxed{\dot X=P/m,\qquad\dot P=-m\omega^2X,\qquad\frac d{dt}(XP)=P^2/m-m\omega^2X^2.}
$$

The last identity follows from the operator product rule without commuting $X$ and $P$. Although $XP$ is not itself [self-adjoint](../../../self-adjoint-operator.md), the same calculation can be applied to the [self-adjoint](../../../self-adjoint-operator.md) dilation observable $(XP+PX)/2$ and gives the same derivative.

Stationarity of the three [expectations](../../../expected-value-split.md) gives $\langle P\rangle=\langle X\rangle=0$ and $\langle P^2\rangle=m^2\omega^2\langle X^2\rangle$. Substitution into $E=\langle P^2\rangle/(2m)+m\omega^2\langle X^2\rangle/2$ yields the [quantum virial theorem](../../../quantum-virial-theorem.md)

$$
\boxed{\left\langle\frac{P^2}{2m}\right\rangle=\frac E2=\frac12m\omega^2\langle X^2\rangle.}
$$

The vanishing means make the [variances](../../../variance-split.md) equal to the second moments, so

$$
\boxed{(\Delta P)^2=mE,\qquad(\Delta X)^2=\frac E{m\omega^2},\qquad\Delta X\Delta P=\frac E\omega=(n+\tfrac12)\hbar\geq\hbar/2.}
$$

This satisfies the position-momentum [Heisenberg uncertainty relation](../../../heisenberg-uncertainty-relation.md), with equality only for the [ground state](../../../ground-state.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2009](../../2009-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
