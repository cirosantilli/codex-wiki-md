<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A comoving material cell contains the same particles in its perturbed and background descriptions, so its mass is $\bar\rho a^3d^3q=\rho d^3r$. The [Jacobian determinant](../../../../../../jacobian-determinant.md) is $a^3\det(I+\nabla_q\psi)$. Expanding the [determinant](../../../../../../determinant.md) gives

$$
\frac\rho{\bar\rho}=\det(I+\nabla_q\psi)^{-1}
=1-\nabla_q\cdot\psi+O(\psi^2),\qquad
\boxed{\delta=-\nabla_q\cdot\psi}.
$$

Split the potential into homogeneous and perturbed parts. There is a sign error in the printed hint: $\nabla^2\Phi_0=4\pi G\bar\rho$ requires **$\nabla\Phi_0=+4\pi G\bar\rho r/3$**, not the printed negative sign. Its acceleration $-\nabla\Phi_0$ agrees with $\ddot a/a=-4\pi G\bar\rho/3$.

For the perturbation, $\nabla_q^2\phi=4\pi G\bar\rho a^2\delta=-4\pi G\bar\rho a^2\nabla_q\cdot\psi$. Under the usual homogeneous boundary convention the curl-free force therefore satisfies

$$
\nabla_q\phi=-4\pi G\bar\rho a^2\psi_L,
$$

where $\psi_L$ is the longitudinal part of the displacement. Expanding the particle acceleration gives $\ddot r=\ddot a(q+\psi)+2\dot a\dot\psi+a\ddot\psi$. The background acceleration cancels the first term, leaving

$$
\ddot\psi+2H\dot\psi-4\pi G\bar\rho\psi_L=0,\qquad H=\dot a/a.
$$

For a longitudinal displacement this proves the displayed [longitudinal displacement in linear dust perturbations](../../../../../../longitudinal-displacement-in-linear-dust-perturbations.md) equation with $\psi_L=\psi$. For unrestricted displacement, a transverse component has no [density contrast](../../../../../../density-contrast.md) and instead obeys $\ddot\psi_T+2H\dot\psi_T=0$; the full-vector equation printed in the question thus needs the longitudinal assumption. Taking the divergence removes this qualification and gives

$$
\boxed{\ddot\delta+2\frac{\dot a}{a}\dot\delta-4\pi G\bar\rho\delta=0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
