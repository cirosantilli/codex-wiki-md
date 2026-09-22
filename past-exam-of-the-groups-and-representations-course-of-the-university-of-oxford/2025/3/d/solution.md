<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because the present $\gamma_0$ is anti-Hermitian, choose the [Dirac adjoint](../../../../dirac-adjoint.md) with Hermitian intertwining matrix $A=i\gamma_0$:

$$
\bar\psi=\psi^\dagger A,\qquad A=i\gamma_0=\begin{pmatrix}0&-i\\i&0\end{pmatrix}.
$$

This convention makes the [Dirac scalar bilinear](../../../../dirac-scalar-bilinear.md) $\bar\psi\psi$ Hermitian. For real $m$, a [Lorentz invariant](../../../../lorentz-invariance.md) [mass term](../../../../mass-term.md) is

$$
\boxed{\mathcal L_m=-m\bar\psi\psi
=im\left(\psi_+^*\psi_- -\psi_-^*\psi_+\right).}
$$

To check infinitesimal [Lorentz invariance](../../../../lorentz-invariance.md), put $K=\sigma_3/2$. Then $K^\dagger=K$ and $K^\dagger A+AK=\{K,A\}=0$. Using [a](../a.md),

$$
\delta\mathcal L_m=-m\theta\psi^\dagger(K^\dagger A+AK)\psi=0.
$$

Equivalently, $\delta(\psi_+^*\psi_-)=\theta\psi_+^*\psi_-/2-\theta\psi_+^*\psi_-/2=0$, and similarly for its [complex conjugate](../../../../complex-conjugate.md). Exponentiation gives $S^\dagger AS=A$ and therefore $\bar\psi'(x')=\bar\psi(x)S^{-1}$.

At fixed coordinates $\mathcal L_m$ has only the orbital variation of a [Lorentz scalar](../../../../lorentz-scalar.md); the spacetime measure is invariant under the connected [Lorentz group](../../../../lorentz-group.md), so the integrated [action](../../../../action.md) is invariant. The [mass term](../../../../mass-term.md) pairs the two opposite [chiralities](../../../../chirality-physics.md); retaining only one [Weyl spinor](../../../../weyl-spinor.md) removes this Dirac mass. An equivalent spinor phase convention gives a real multiple of $\psi_+^*\psi_-+\psi_-^*\psi_+$ instead.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
