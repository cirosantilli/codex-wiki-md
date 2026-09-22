# Barnett equivalent magnetic field

↑ **Parent:** [Barnett effect](barnett-effect.md)

Let the specimen rotate uniformly with [angular velocity](angular-velocity.md) $\boldsymbol\Omega=\Omega\widehat{\mathbf z}$. In its [rotating reference frame](rotating-reference-frame.md), the internal [Hamiltonian](hamiltonian.md) contains

$$
\mathcal H_{\rm rot}=\mathcal H_0-\Omega J_z.
$$

Here $J_z$ is the internal [angular momentum operator](angular-momentum-operator-split.md) about the rotation axis, and $\mathcal H_0$ contains the internal interactions and any imposed [magnetic field](magnetic-field-split.md) expressed in that frame. It does not include the separately treated rigid body's [rotational kinetic energy](rotational-kinetic-energy.md). For a sector with [magnetic moment](magnetic-dipole-moment.md) $m_z=\gamma J_z$, the rotational term has exactly the form of a [magnetic dipole potential energy](magnetic-dipole-potential-energy.md):

$$
-\Omega J_z=-m_zB_\Omega,\qquad
B_\Omega=\frac{\Omega}{\gamma}.
$$

This [Barnett equivalent magnetic field](barnett-equivalent-magnetic-field.md) has [tesla](tesla-unit.md) units, with the angular convention for the signed [gyromagnetic ratio](gyromagnetic-ratio.md): $\Omega$ is in radians per second, not revolutions per second. Its sign matters. For an electronic contribution with $\gamma<0$, positive $\Omega$ favors positive $J_z$ and negative $m_z$. A sector with $\gamma>0$ has the opposite magnetic sign. Equal $\Omega$ need not correspond to equal [Barnett fields](barnett-equivalent-magnetic-field.md) for sectors having different [gyromagnetic ratios](gyromagnetic-ratio.md).

A short derivation fixes the sign independently of any material model. Put $U(t)=\exp(-\mathrm i\Omega tJ_z/\hbar)$ and transform a laboratory [quantum state](quantum-state.md) by $|\psi_{\rm rot}\rangle=U^\dagger|\psi_{\rm lab}\rangle$. The [Schrödinger equation](schrodinger-equation.md) gives

$$
\mathcal H_{\rm rot}
=U^\dagger\mathcal H_{\rm lab}U-\mathrm i\hbar U^\dagger\dot U
=\mathcal H_0-\Omega J_z.
$$

The transformed laboratory term is denoted by $\mathcal H_0$; a laboratory perturbation not stationary in the rotating frame can make it time dependent. Establishing a steady thermal response also requires exchange of internal [angular momentum](angular-momentum.md) with the rotating body, for example through [spin-lattice relaxation](spin-lattice-relaxation.md). A mere relabeling of coordinates cannot polarize isolated, unrelaxed [spins](spin.md).

The [Barnett field](barnett-equivalent-magnetic-field.md) is a useful description of [spin-rotation coupling](spin-rotation-coupling.md), not a claim that empty laboratory space acquires a uniform [magnetic flux density](magnetic-field-split.md) $\Omega/\gamma$. In particular, inserting it into the [Lorentz force](lorentz-force.md) on an unrelated test [electric charge](electric-charge-split.md) is unjustified. A nearby [magnetometer](magnetometer.md) detects the specimen's actual stray [magnetic field](magnetic-field-split.md) and backgrounds, rather than directly detecting this internal [Hamiltonian](hamiltonian.md) parameter.

## ↑ Ancestors (7)

1. [Barnett effect](barnett-effect.md)
2. [Magnetic dipole moment](magnetic-dipole-moment.md)
3. [Magnetic vector potential](magnetic-vector-potential.md)
4. [Electromagnetism](electromagnetism-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Barnett equivalent magnetic field](barnett-equivalent-magnetic-field.md)
