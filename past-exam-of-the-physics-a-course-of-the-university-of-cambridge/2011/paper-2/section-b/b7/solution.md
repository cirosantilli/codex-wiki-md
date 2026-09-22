<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

A pure [stationary state](../../../../../stationary-state.md) of a time-independent [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is $\Psi(\mathbf r,t)=\psi(\mathbf r)e^{-iEt/\hbar}$. Its [probability density](../../../../../probability-density.md) and all expectations of time-independent [observables](../../../../../observable.md) are constant. This does not require zero [probability current](../../../../../probability-current.md).

For real scalar [potential energy](../../../../../potential-energy.md) and no [vector potential](../../../../../vector-potential.md), substitute $i\hbar\dot\Psi=-(\hbar^2/2m)\nabla^2\Psi+V\Psi$ and its [complex conjugate](../../../../../complex-conjugate.md) into $\dot\rho=\Psi^*\dot\Psi+\dot\Psi^*\Psi$. The potential terms cancel:

$$
\dot\rho=\frac{i\hbar}{2m}\big(\Psi^*\nabla^2\Psi-\Psi\nabla^2\Psi^*\big)
=-\nabla\cdot\left[\frac{\hbar}{2im}(\Psi^*\nabla\Psi-\Psi\nabla\Psi^*)\right].
$$

Thus the [probability current](../../../../../probability-current.md) is $\mathbf j=(\hbar/m)\operatorname{Im}(\Psi^*\nabla\Psi)$. In a [stationary state](../../../../../stationary-state.md) $\nabla\cdot\mathbf j=0$: flow may circulate without changing the [density](../../../../../density.md).

Here only the azimuthal [phase](../../../../../phase-waves.md) contributes an imaginary logarithmic [derivative](../../../../../derivative.md). Since $\nabla\phi=\hat{\boldsymbol\phi}/(r\sin\theta)$,

$$
\boxed{\mathbf j=\frac{\hbar|\Psi|^2}{mr\sin\theta}\hat{\boldsymbol\phi}
=\frac{\hbar A^2}{m}r e^{-r/a_0}\sin\theta\,\hat{\boldsymbol\phi}}.
$$

There is no radial or polar flow; the azimuthal current is independent of $\phi$, so its [divergence](../../../../../divergence.md) vanishes. The apparent coordinate singularity at $\sin\theta=0$ cancels in the final expression.

The z-component of [orbital angular momentum](../../../../../orbital-angular-momentum.md) follows from the moment of the [mass](../../../../../mass.md) current:

$$
\langle L_z\rangle
=\int mr\sin\theta\,j_\phi\,dV
=\hbar A^2
\left(\int_0^\infty r^4e^{-r/a_0}dr\right)
\left(\int_0^\pi\sin^3\theta\,d\theta\right)
\left(\int_0^{2\pi}d\phi\right)
=\boxed{\hbar}.
$$

Indeed $A^2(24a_0^5)(4/3)(2\pi)=1$. This agrees with $L_z=-i\hbar\partial_\phi$ acting on the [wavefunction](../../../../../wave-function-split.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
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
