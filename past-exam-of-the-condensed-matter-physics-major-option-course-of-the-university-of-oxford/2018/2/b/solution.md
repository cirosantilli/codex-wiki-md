<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [linear combination of atomic orbitals](../../../../linear-combination-of-atomic-orbitals.md) expands a [crystal](../../../../crystal.md) wavefunction in localized orbitals on all sites,

$$
\Psi_{\mathbf k}(\mathbf r)=\sum_{\mathbf R,\alpha,\eta}c_{\alpha\eta}(\mathbf k)
 e^{i\mathbf k\cdot(\mathbf R+\mathbf d_\alpha)}
 \varphi_{\alpha\eta}(\mathbf r-\mathbf R-\mathbf d_\alpha).
$$

Here $\alpha$ labels the [basis](../../../../crystal-motif.md) site, $\eta$ the retained [atomic orbitals](../../../../atomic-orbital.md) and $\mathbf R=m\mathbf a_1+n\mathbf a_2$. For the two-band model retain one relevant orbital on each B or N atom, usually the out-of-plane $p_z$ orbital, and neglect other orbital manifolds. Define normalized Bloch sums for $N_c$ cells,

$$
\Phi_\alpha(\mathbf k,\mathbf r)=\frac1{\sqrt{N_c}}\sum_{m,n}
 e^{i\mathbf k\cdot(m\mathbf a_1+n\mathbf a_2+\mathbf d_\alpha)}
 \varphi_\alpha(\mathbf r-m\mathbf a_1-n\mathbf a_2-\mathbf d_\alpha),
 \quad\alpha=B,N.
$$

Then $\Psi=\alpha_B\Phi_B+\alpha_N\Phi_N$. Bloch periodicity puts the same two coefficients in every cell. We adopt the stated [orthonormality](../../../../orthonormal-set.md), neglect longer-range hopping, and approximate the diagonal [matrix](../../../../matrix.md) elements by the supplied atomic energies $\epsilon_B,\epsilon_N$. More generally the [crystal](../../../../crystal.md) environment shifts these on-site energies, so equality with isolated-atom expectation values is an additional [tight-binding approximation](../../../../tight-binding.md).

For equal real nearest-neighbour transfer [integral](../../../../integral-split.md) $t_{\rm nn}$, this phase convention gives

$$
\gamma(\mathbf k)=\sum_{j=1}^3e^{i\mathbf k\cdot\mathbf n_j},\qquad
H(\mathbf k)=\begin{pmatrix}\epsilon_B&t_{\rm nn}\gamma\\t_{\rm nn}\gamma^*&\epsilon_N\end{pmatrix}.
$$

The secular determinant is $(\epsilon_B-E)(\epsilon_N-E)-t_{\rm nn}^2|\gamma|^2=0$. Thus

$$
\boxed{E_\pm(\mathbf k)=\frac{\epsilon_B+\epsilon_N}{2}
\pm\sqrt{\frac{(\epsilon_B-\epsilon_N)^2}{4}+t_{\rm nn}^2|\gamma|^2}.}
$$

Since $(\epsilon_B-\epsilon_N)^2/4=(\epsilon_B+\epsilon_N)^2/4-\epsilon_B\epsilon_N$, this is the requested algebraic form. A hopping-sign convention or rephasing of the Bloch sums changes off-diagonal phases but not these [eigenvalues](../../../../eigenvalue.md). Explicitly,

$$
\gamma=e^{ik_xa/\sqrt3}+2e^{-ik_xa/(2\sqrt3)}\cos(k_ya/2),\quad
|\gamma|^2=1+4\cos^2(k_ya/2)+4\cos(k_ya/2)\cos(\sqrt3ak_x/2).
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
