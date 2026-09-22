<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose field $a$ to be $(\widehat{\mathbf u}^a)^*$ at [frequency](../../../../../../frequency.md) $-\omega_a$, and field $b$ to be $\widehat{\mathbf u}^b$ at $\omega_b$. Zero [body forces](../../../../../../body-force.md) and zero boundary [tractions](../../../../../../traction.md) make all source and surface terms vanish. Therefore

$$
(\omega_b^2-\omega_a^2)\int_{\mathcal D}\rho(\widehat u_i^a)^*\widehat u_i^b\,dV=0.
$$

For distinct squared [frequencies](../../../../../../frequency.md) this proves **weighted [orthogonality](../../../../../../orthogonal-vectors.md)**,

$$
\boxed{\langle\widehat{\mathbf u}^a,\widehat{\mathbf u}^b\rangle_\rho=\int_{\mathcal D}\rho(\widehat u_i^a)^*\widehat u_i^b\,dV=0.}
$$

Assume positive [mass density](../../../../../../density.md) bounded above and below and finite-energy fields in the ordinary bounded domain. The weighted space $H=L^2(\mathcal D,\rho\,dV)^3$ is a [separable Hilbert space](../../../../../../separable-hilbert-space.md). Select one unit [eigenfunction](../../../../../../eigenfunction.md) for each distinct squared [frequency](../../../../../../frequency.md). They form an [orthonormal set](../../../../../../orthonormal-set.md). Let $\{d_j\}$ be a countable dense subset of $H$; assign to each [eigenfunction](../../../../../../eigenfunction.md) a point $d_j$ within distance $1/3$. Two [orthogonal](../../../../../../orthogonal-vectors.md) unit [eigenfunctions](../../../../../../eigenfunction.md) have distance $\sqrt2$, so the same $d_j$ cannot be assigned to both. This gives an injection into a countable set.

Hence there are **at most countably many squared [eigenfrequencies](../../../../../../eigenfrequency.md)**, and at most twice that many signed [frequencies](../../../../../../frequency.md). Multiplicity at one [frequency](../../../../../../frequency.md) does not change the argument. A zero [frequency](../../../../../../frequency.md) associated with rigid translations or rotations is included. This proves the [countability of elastic eigenfrequencies](../../../../../../countability-of-elastic-eigenfrequencies.md) directly; proving discreteness or finite multiplicity would require additional spectral regularity arguments.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
