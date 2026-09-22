<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Quantize along the selected field direction by the right-handed relabeling $\tilde S^z=S^x$, $\tilde S^x=S^y$, $\tilde S^y=S^z$. Then the exact [Holstein–Primakoff transformation](../../../../holstein-primakoff-transformation.md) in [c](../c.md) gives $S_j^x=S-n_j$. Keep exchange terms of order $S^2$ and $S$, with $J$ and the printed $B$ held fixed. For a nearest-neighbor bond,

$$
\mathbf S_j\cdot\mathbf S_k
=S^2-S(n_j+n_k)+S(a_j^\dagger a_k+a_k^\dagger a_j)+O(S^0).
$$

On a periodic [cubic lattice](../../../../cubic-lattice.md) with $N$ sites and spacing $a$, there are $3N$ undirected bonds. Consequently,

$$
H_{\rm LSW}=-NS^2(3J+B)
+JS\sum_{\langle j,k\rangle}(n_j+n_k-a_j^\dagger a_k-a_k^\dagger a_j)
+BS\sum_jn_j.
$$

Use the unitary lattice [Fourier transform](../../../../fourier-transform-split.md) $a_j=N^{-1/2}\sum_{\mathbf k}e^{i\mathbf k\cdot\mathbf r_j}a_{\mathbf k}$. Each positive lattice direction contributes $2(1-\cos k_\alpha a)$, so the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is already diagonal in momentum space:

$$
\boxed{H_{\rm LSW}=E_{\rm GS}+\sum_{\mathbf k}\varepsilon_{\mathbf k}a_{\mathbf k}^\dagger a_{\mathbf k},\qquad
\varepsilon_{\mathbf k}=S\left[B+2J\sum_{\alpha=1}^3(1-\cos k_\alpha a)\right],\quad
E_{\rm GS}=-NS^2(3J+B).}
$$

There are no anomalous $aa$ or $a^\dagger a^\dagger$ terms, so no [Bogoliubov transformation](../../../../bogoliubov-transformation.md) or extra zero-point correction is needed. At long wavelengths,

$$
\boxed{\varepsilon_{\mathbf k}=BS+JSa^2|\mathbf k|^2+O(k^4).}
$$

At $B=0$ this is the quadratic ferromagnetic [Goldstone mode](../../../../goldstone-boson.md); for $B>0$ it is gapped by $BS$. Energies are written with $\hbar=1$; an excitation frequency is $\omega_{\mathbf k}=\varepsilon_{\mathbf k}/\hbar$. In this isotropic ferromagnet the fully aligned vacuum and its one-magnon dispersion are also exact; higher-magnon interactions are among the terms discarded from the linear spin-wave [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
