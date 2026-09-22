# Spectroscopic nuclear quadrupole moment

↑ **Parent:** [Nuclear deformation](nuclear-deformation.md)

The laboratory [expectation value](expectation-value.md) of the axial [electric quadrupole moment](electric-quadrupole-moment.md) in the stretched nuclear [quantum state](quantum-state.md) $|I,M=I\rangle$; $M\hbar$ is the laboratory $z$ component of total [angular momentum](angular-momentum.md). It differs from the [intrinsic nuclear quadrupole moment](intrinsic-nuclear-quadrupole-moment.md) $Q_0$. In an axial [nuclear rotational band](nuclear-rotational-band.md) with $K=0$, projection onto definite [angular momentum](angular-momentum.md) gives

$$
Q_s(I)=-\frac{I}{2I+3}Q_0,\qquad Q_s(0)=0,\qquad Q_s(2)=-\frac27Q_0.
$$

Here $K\hbar$ denotes the component of total [angular momentum](angular-momentum.md) along the intrinsic symmetry axis. Consequently a positive $Q_0$ for a [prolate spheroid](prolate-spheroid.md) corresponds to a negative $Q_s(2)$ in this model. The sign of the laboratory moment alone must be interpreted together with the band assignment.

The $I=0$ result has a short [symmetry](symmetry-physics.md) explanation. A spin-zero state has no preferred spatial direction. Its second charge moments satisfy $\langle x^2\rangle=\langle y^2\rangle=\langle z^2\rangle$, so $\langle2z^2-x^2-y^2\rangle=0$. Equivalently, averaging an intrinsic axis uniformly over directions gives $\langle P_2(\cos\theta)\rangle=0$, where $P_2(u)=(3u^2-1)/2$ is a [Legendre polynomial](legendre-polynomial.md). This is a statement about a quantum [expectation value](expectation-value.md), not a classical picture of a spinning object sweeping through orientations.

For an independent check of the $I=2$ sign, the $K=0$, $M=2$ rotor orientation probability is proportional to $|Y_2^2|^2\propto\sin^4\theta$, using a [spherical harmonic](spherical-harmonic.md). With $u=\cos\theta$,

$$
\frac{Q_s(2)}{Q_0}
=\frac{\int_{-1}^{1}P_2(u)(1-u^2)^2\,du}{\int_{-1}^{1}(1-u^2)^2\,du}
=\frac{-32/105}{16/15}=-\frac27.
$$

A zero static laboratory moment does not make every quadrupole observable zero. With electric multipole operator $\mathcal M_{2\mu}=\int\rho_{\mathrm{ch}}r^2Y_2^\mu\,d^3r$, define the reduced transition strength using a [reduced matrix element](reduced-matrix-element.md):

$$
B(E2;I_i\to I_f)=\frac{|\langle I_f\Vert\mathcal M_2\Vert I_i\rangle|^2}{2I_i+1}.
$$

In the axial $K=0$ rotor, angular projection gives $B(E2;0^+\to2^+)=5Q_0^2/(16\pi)$ and $B(E2;2^+\to0^+)=Q_0^2/(16\pi)$. The factor of five is the ratio of the numbers of magnetic substates. Thus an [electric quadrupole transition](electric-quadrupole-transition.md) can reveal collective deformation even when $Q_s(0)=0$. These strengths determine $|Q_0|$ within the model; their squares alone cannot distinguish its sign.

## ↑ Ancestors (5)

1. [Nuclear deformation](nuclear-deformation.md)
2. [Atomic nucleus](atomic-nucleus-split.md)
3. [Nuclear physics](nuclear-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-particle-and-nuclear-physics-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
