<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [quantum optimal control](../../../../../../quantum-optimal-control.md) problem specifies a terminal task, admissible fields and resource costs. Pure-state transfer can minimize $1-|\langle\psi_d|\psi(T)\rangle|^2$; mixed-state transfer on an accessible spectral orbit can minimize $\|\rho(T)-\rho_d\|_{\mathrm{HS}}^2/2$; preparing an observable value can minimize $-\operatorname{Tr}(O\rho(T))$. A gate task can minimize $1-|\operatorname{Tr}(U_d^\dagger U(T))|^2/n^2$ for an $n$-dimensional [Hilbert space](../../../../../../hilbert-space-split.md), which is insensitive to an overall phase. These different terminal functions encode different tasks even when the dynamics are the same. Fluence penalties, amplitude bounds, bandwidth limits, or the total duration can be added to express experimental requirements.

For example, minimize

$$
J[f]=\Phi(\rho(T))+\frac12\sum_m\lambda_m\int_0^T f_m(t)^2\,dt,\qquad \lambda_m>0,
$$

subject to $\dot\rho=\mathcal L_f(\rho)$ and a specified $\rho(0)$. For a closed system, $\mathcal L_f(\rho)=-i[H_0+\sum_mf_mH_m,\rho]$; for an open system add the known [Lindblad equation](../../../../../../lindblad-equation.md) dissipator. Introducing a Hermitian [costate](../../../../../../costate.md) $\Lambda$ and taking the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) gives the forward and backward equations and functional gradient

$$
\dot\rho=\mathcal L_f(\rho),\qquad \dot\Lambda=-\mathcal L_f^\dagger(\Lambda),\qquad \Lambda(T)=\nabla_\rho\Phi(\rho(T)),
$$



$$
\boxed{\frac{\delta J}{\delta f_m(t)}=\lambda_mf_m(t)+\operatorname{Tr}\left(\Lambda(t)\frac{\partial\mathcal L_f}{\partial f_m}(\rho(t))\right)}.
$$

For Hamiltonian controls the second term is $\operatorname{Tr}(\Lambda[-iH_m,\rho])$. The adjoint is defined by the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md); in particular, the closed-system costate equation is $\dot\Lambda=-i[H,\Lambda]$, integrated backward from its terminal condition. An unconstrained interior optimum has zero gradient; amplitude constraints replace this by the corresponding constrained first-order conditions.

Numerically, represent the fields by piecewise constant amplitudes $f_{m,j}$ on slices, or by a finite basis $f_m(t)=\sum_j a_{mj}b_j(t)$ such as splines or Fourier modes. For piecewise constant closed-system dynamics, $U_j=e^{-iH_j\Delta t}$ and $U(T)=U_K\cdots U_1$. Forward products and backward costates provide all slice derivatives in one pair of propagations. In [gradient ascent pulse engineering](../../../../../../gradient-ascent-pulse-engineering.md), update these amplitudes to improve the chosen objective, with projection onto amplitude bounds if needed. The exact slice derivative is the [derivative of the matrix exponential](../../../../../../derivative-of-the-matrix-exponential.md)

$$
\frac{\partial U_j}{\partial f_{m,j}}=-i\int_0^{\Delta t}e^{-iH_j(\Delta t-\tau)}H_m e^{-iH_j\tau}\,d\tau.
$$

Replacing it by $-i\Delta t H_mU_j$ is only a short-slice approximation when $H_j$ and $H_m$ do not commute. Other [gradient descent](../../../../../../gradient-descent.md) or [nonlinear optimization](../../../../../../nonlinear-programming.md) methods can optimize the same finite parameter set; [direct-adjoint looping](../../../../../../direct-adjoint-looping.md) avoids a separate dynamical simulation for each control coefficient.

A pulse is accepted after propagation with the actual constrained waveform confirms its terminal error and resource use. Sampling model uncertainties in the objective can favor robust pulses. Nonconvexity means a numerical stationary point need not be a global optimum, so initial guesses, convergence tolerances and a sufficiently resolved time grid matter.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
