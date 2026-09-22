<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the resonant [interaction picture](../../../../interaction-picture.md) and define $g>0$ by the one-atom [Jaynes-Cummings model](../../../../jaynes-cummings-model.md) in part (a). Equal coupling to both atoms gives the [Tavis-Cummings model](../../../../tavis-cummings-model.md)

$$
H_I=\hbar g\left[a(\sigma_+^{(1)}+\sigma_+^{(2)})
+a^\dagger(\sigma_-^{(1)}+\sigma_-^{(2)})\right].
$$

The initial state has two excitations and is symmetric under atom exchange. Excitation conservation and this symmetry confine the evolution to

$$
|A\rangle=|ee;0\rangle,\quad
|B\rangle=\frac{|eg\rangle+|ge\rangle}{\sqrt2}\otimes|1\rangle,\quad
|C\rangle=|gg;2\rangle.
$$

The antisymmetric atomic [spin singlet state](../../../../spin-singlet-state.md) is uncoupled and unpopulated. Applying the [annihilation operator](../../../../annihilation-operator.md) and [creation operator](../../../../creation-operator.md) gives

$$
\frac{H_I}{\hbar}=g
\begin{pmatrix}0&\sqrt2&0\\\sqrt2&0&2\\0&2&0\end{pmatrix}.
$$

The first off-diagonal entry combines two indistinguishable atomic emission paths; the second also includes the $\sqrt2$ enhancement for creating the second [photon](../../../../photon.md). Its [eigenvalues](../../../../eigenvalue.md) are $0,\pm\sqrt6g$. Put $\Omega=\sqrt6g$ and $K=H_I/\hbar$, so $K^3=\Omega^2K$. Its exponential is

$$
e^{-iKt}=I-\frac{i\sin\Omega t}{\Omega}K
+\frac{\cos\Omega t-1}{\Omega^2}K^2.
$$

Applying this to $|A\rangle$ yields

$$
\boxed{\begin{aligned}
|\psi(t)\rangle={}&\frac{2+\cos\Omega t}{3}|ee;0\rangle\\
&-\frac{i}{\sqrt3}\sin\Omega t\,
\frac{|eg\rangle+|ge\rangle}{\sqrt2}\otimes|1\rangle\\
&+\frac{\sqrt2}{3}(\cos\Omega t-1)|gg;2\rangle.
\end{aligned}}
$$

All three states have the same bare [energy](../../../../energy-split.md) on [resonance](../../../../resonance.md), so restoring the free Schrödinger-picture evolution adds only a common [global phase](../../../../global-phase.md). The expression starts at $|ee;0\rangle$, has initial derivative $-i\sqrt2g|B\rangle$, and its three squared [probability amplitudes](../../../../probability-amplitude.md) sum to one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
