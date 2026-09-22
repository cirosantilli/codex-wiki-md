# Momentum matrix-element expansion of band energy

↑ **Parent:** [Bloch Hamiltonian](bloch-hamiltonian.md)

For a real scalar lattice-periodic potential, let $|n\rangle$ be a nondegenerate zone-centre periodic eigenstate with energy $E_n$. Conjugation by $e^{i\mathbf k\cdot\mathbf r}$ gives $H(\mathbf k)=H(0)+\hbar\mathbf k\cdot\mathbf p/m+\hbar^2k^2/(2m)$. The zone-centre state can be chosen real, so $\langle n|\mathbf p|n\rangle=0$. [Second-order nondegenerate perturbation theory](second-order-nondegenerate-perturbation-theory.md) then gives

$$
E_n(\mathbf k)=E_n+\frac{\hbar^2k^2}{2m}+\frac{\hbar^2}{m^2}\sum_{l\ne n}\frac{|\langle n|\mathbf k\cdot\mathbf p|l\rangle|^2}{E_n-E_l}+O(|\mathbf k|^4).
$$

Time-reversal symmetry makes this isolated spinless band even in $\mathbf k$. In a direction $\mathbf e$, the curvature gives

$$
\frac{m}{m^*_{\mathbf e}}=1+\frac2m\sum_{l\ne n}\frac{|\langle n|\mathbf e\cdot\mathbf p|l\rangle|^2}{E_n-E_l}.
$$

A degeneracy requires a matrix treatment before extracting curvatures; a nonlocal potential or spin-orbit terms can also alter the simple momentum vertex.

## ↑ Ancestors (6)

1. [Bloch Hamiltonian](bloch-hamiltonian.md)
2. [Bloch's theorem](bloch-s-theorem-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2016/3/solution.md)
