<h1 id="15c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The Hamiltonian is the sum of three commuting one-dimensional [harmonic-oscillator](../../../../../../quantum-harmonic-oscillator.md) Hamiltonians. Its product [eigenstates](../../../../../../eigenstate.md) are

$$
\Psi_{n_xn_yn_z}(x,y,z)
=\psi_{n_x}(x)\psi_{n_y}(y)\psi_{n_z}(z),
$$

with energies

$$
\boxed{
E_{n_xn_yn_z}
=\hbar\omega\left(n_x+n_y+n_z+\frac32\right)
}.
$$

Equivalently, the level with $N=n_x+n_y+n_z$ has energy $E_N=\hbar\omega(N+3/2)$, as in the [three-dimensional isotropic harmonic oscillator](../../../../../../three-dimensional-isotropic-harmonic-oscillator.md).

Up to normalization, the ground-state wavefunction is

$$
\Psi_{000}
=\exp\left[-\frac{M\omega}{2\hbar}(x^2+y^2+z^2)\right].
$$

It is radial, so $\nabla\Psi_{000}$ is parallel to the position vector. Since the [orbital angular momentum](../../../../../../orbital-angular-momentum.md) is $L=-i\hbar\,r\times\nabla$, every component of $L$ annihilates this state. Therefore

$$
L_z\Psi_{000}=0,
\qquad
L^2\Psi_{000}=0,
$$

and the ground state has $\ell=m=0$.

The first excited level has $N=1$ and is spanned by

$$
x\Psi_{000},\qquad y\Psi_{000},\qquad z\Psi_{000}.
$$

The state

$$
\Phi_0=z\Psi_{000}
$$

satisfies $L_z\Phi_0=0$. Applying the ladder operators gives

$$
L_+\Phi_0=-\hbar(x+iy)\Psi_{000},
\qquad
L_-\Phi_0=\hbar(x-iy)\Psi_{000}.
$$

Hence convenient $m=\pm1$ eigenstates are

$$
\boxed{\Phi_{\pm1}=(x\pm iy)\Psi_{000}},
$$

up to normalization and irrelevant overall phases.

Finally, the isotropic Hamiltonian is rotationally invariant. The [rotational invariance of a central-potential Hamiltonian](../../../../../../rotational-invariance-of-a-central-potential-hamiltonian.md) gives

$$
[H,L_z]=[H,L^2]=[L_z,L^2]=0.
$$

These commuting self-adjoint operators can be simultaneously diagonalized within each energy eigenspace, which is why joint eigenstates of $H,L^2,L_z$ must exist.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15C](../../15c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
