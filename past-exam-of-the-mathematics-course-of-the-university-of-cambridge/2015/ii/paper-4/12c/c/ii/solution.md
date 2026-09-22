<h1 id="12c/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here $(I_1,I_2,I_3)=(20,17,5)Ma^2/12$, so $I_1>I_2>I_3$ and $e_2$ is the intermediate axis. Eliminating the other components from $L^2=2I_2E$ and the [conservation of energy](../../../../../../../conservation-of-energy.md) relation gives, with $J=2E-I_2\omega_2^2$,

$$
\omega_1^2=\frac{I_2-I_3}{I_1(I_1-I_3)}J,\qquad
\omega_3^2=\frac{I_1-I_2}{I_3(I_1-I_3)}J.
$$

Thus the second [Euler equations for a torque-free rigid body](../../../../../../../euler-equations-for-a-torque-free-rigid-body.md) reduces to

$$
\boxed{\dot\omega_2=\pm\frac35\left(\frac{24E}{17Ma^2}-\omega_2^2\right).}
$$

The sign is minus the sign of $\omega_1\omega_3$; it is constant along a nontrivial branch. Let $\Omega=\sqrt{24E/(17Ma^2)}$. Since $\omega_2(0)=0$, integration yields $\omega_2(t)=\pm\Omega\tanh(3\Omega t/5)$, with the same sign as in the scalar equation. The remaining components are

$$
\omega_1(t)=\omega_1(0)\operatorname{sech}(3\Omega t/5),\qquad
\omega_3(t)=\omega_3(0)\operatorname{sech}(3\Omega t/5).
$$

Their initial squares are fixed by the preceding algebraic formulas with $J=2E$; their initial signs determine the branch. Hence $\boxed{\omega(t)\longrightarrow\pm\Omega e_2}$ as $t\to\infty$. This trajectory is an [intermediate-axis separatrix](../../../../../../../intermediate-axis-separatrix.md): approaching intermediate-axis rotation on this special conserved-energy level does not make that rotation stable to generic perturbations. If $E=0$, all components vanish identically.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [12C](../../../12c.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
