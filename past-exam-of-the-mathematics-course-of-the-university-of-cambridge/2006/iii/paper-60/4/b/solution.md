<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At an unconstrained differentiable extremum the first variation vanishes independently with respect to the state, [costate](../../../../../../costate.md) and real controls, with initial state fixed. For the real functional, take the real Hilbert-Schmidt pairing when necessary. The [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) are most clearly written using the forward generator $K$:

$$
\boxed{\dot\rho_v=K[f]\rho_v,\qquad \rho_v(t_0)=\rho_{v,0},}
$$



$$
\boxed{\dot A_v=-K[f]^\dagger A_v,\qquad A_v(t_F)=\widehat A_v.}
$$

Here the dagger is the adjoint for the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md), and $\widehat A_v$ is the vectorized terminal observable. Equivalently,

$$
i\hbar\dot\rho_v=\mathcal L_{\rm tot}\rho_v,\qquad
\boxed{i\hbar\dot A_v=\mathcal L_{\rm tot}^\dagger A_v.}
$$

The adjoint is essential if $\mathcal L_D$ is not self-adjoint: dissipative [costate](../../../../../../costate.md) evolution must not be replaced by the forward dissipator.

For each unconstrained real field, stationarity gives

$$
\boxed{\frac{p_0\lambda_m}{\hbar}f_m(t)=\operatorname{Re}\langle\!\langle A_v(t)|\partial_{f_m}K|\rho_v(t)\rangle\!\rangle
=\frac1\hbar\operatorname{Im}\langle\!\langle A_v(t)|\mathcal L_m|\rho_v(t)\rangle\!\rangle.}
$$

Thus $f_m=\operatorname{Im}\langle\!\langle A_v|\mathcal L_m|\rho_v\rangle\!\rangle/(p_0\lambda_m)$. For Hermitian state and [costate](../../../../../../costate.md) with [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) couplings, the contraction before taking its imaginary part is purely imaginary, and this is a real field. These are the [Liouville-space costate equations for quantum optimal control](../../../../../../liouville-space-costate-equations-for-quantum-optimal-control.md).

Forward state propagation, backward [costate](../../../../../../costate.md) propagation, and the control stationarity equations must be solved together. They give necessary conditions, not a certificate of global optimality. For a local maximum the second variation on admissible perturbations is nonpositive. If amplitude or bandwidth constraints are imposed, the unrestricted pointwise field equation must be replaced by the corresponding constrained stationarity condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
