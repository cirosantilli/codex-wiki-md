<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [stationary state](../../../../../stationary-state.md) has $\Psi(t,x)=e^{-iEt/\hbar}\psi(x)$. Substitution into the [Schrödinger equation](../../../../../schrodinger-equation.md) gives the [energy eigenvalue](../../../../../energy-eigenvalue-split.md) equation

$$
-\frac{\hbar^2}{2m}\psi''=E\psi.
$$

The trial [wavefunction](../../../../../wave-function-split.md) $Ce^{ikx}$ satisfies it with $E=\hbar^2k^2/(2m)$. The [periodic boundary condition](../../../../../periodic-boundary-conditions.md) requires $e^{2\pi ikR}=1$, hence $k=n/R$, $n\in\mathbb Z$. The [wavefunction normalization](../../../../../wavefunction-normalization.md) is $1=2\pi R|C|^2$, so a convenient common [global phase](../../../../../global-phase.md) gives the [orthonormal basis](../../../../../orthonormal-basis.md)

$$
\boxed{\phi_n(x)=\frac{e^{inx/R}}{\sqrt{2\pi R}},\qquad E_n=\frac{\hbar^2n^2}{2mR^2},\qquad n\in\mathbb Z.}
$$

Indeed, $\int_0^{2\pi R}\phi_n^*\phi_q\,dx=\delta_{nq}$. This is the [free particle spectrum on a circle](../../../../../free-particle-spectrum-on-a-circle.md). The [ground state](../../../../../ground-state.md) $\phi_0$ has [energy](../../../../../energy-split.md) zero and is nondegenerate. Each positive [energy level](../../../../../energy-level.md) $\hbar^2n^2/(2mR^2)$, $n=1,2,\ldots$, has [energy eigenspace](../../../../../energy-eigenspace.md) $\operatorname{span}\{\phi_n,\phi_{-n}\}$ and [quantum degeneracy](../../../../../degenerate-energy-levels.md) two. Real sine and cosine combinations give another basis of the same [energy eigenspace](../../../../../energy-eigenspace.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
