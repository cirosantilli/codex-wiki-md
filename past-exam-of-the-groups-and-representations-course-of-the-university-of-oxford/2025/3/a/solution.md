<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Adopt the [Minkowski metric](../../../../minkowski-metric.md) $\eta=\operatorname{diag}(-1,+1)$ and the [Clifford algebra](../../../../clifford-algebra.md) convention $\{\gamma_\mu,\gamma_\nu\}=2\eta_{\mu\nu}I$. The source's [Pauli matrices](../../../../pauli-matrices.md) give

$$
\gamma_0=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\gamma_1=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

They satisfy $\gamma_0^2=-I$, $\gamma_1^2=I$ and $\gamma_0\gamma_1=-\gamma_1\gamma_0=-\sigma_3$, which verifies the required [Clifford algebra](../../../../clifford-algebra.md). Raising the indices gives $\gamma^0=-\gamma_0$ and $\gamma^1=\gamma_1$.

Fix the sign of the [rapidity](../../../../rapidity.md) $\theta$ by taking the [Lorentz boost](../../../../lorentz-boost.md)

$$
\begin{pmatrix}t'\\x'\end{pmatrix}
=\Lambda(\theta)\begin{pmatrix}t\\x\end{pmatrix},\qquad
\Lambda(\theta)=\begin{pmatrix}\cosh\theta&-\sinh\theta\\-\sinh\theta&\cosh\theta\end{pmatrix}.
$$

The corresponding [Spinor representation of the Lorentz group](../../../../spinor-representation-of-the-lorentz-group.md) is

$$
S(\theta)=\exp\left(\frac\theta2\gamma^0\gamma^1\right)
=\exp\left(\frac\theta2\sigma_3\right)
=\operatorname{diag}(e^{\theta/2},e^{-\theta/2}).
$$

For example $S^{-1}\gamma^0S=\gamma^0\cosh\theta-\gamma^1\sinh\theta$ and $S^{-1}\gamma^1S=\gamma^1\cosh\theta-\gamma^0\sinh\theta$, establishing [Lorentz covariance](../../../../lorentz-covariance.md) by $S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu$.

Thus the [Dirac spinor](../../../../dirac-spinor.md) transforms as $\psi'(x')=S(\theta)\psi(x)$, with infinitesimal law

$$
\boxed{\delta\psi=\frac\theta2\sigma_3\psi,\qquad
\delta\psi_+=\frac\theta2\psi_+,\qquad
\delta\psi_-=-\frac\theta2\psi_-.}
$$

These variations compare the fields at corresponding spacetime points. At a fixed coordinate one adds the usual orbital term $-\delta x^\mu\partial_\mu\psi$. Reversing the [rapidity](../../../../rapidity.md) convention reverses both boost signs consistently. Infinitesimal transformations describe the [proper orthochronous Lorentz group](../../../../proper-orthochronous-lorentz-group.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
