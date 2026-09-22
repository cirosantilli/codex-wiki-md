<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For real $\Delta_k$ and $\xi_{-k}=\xi_k$, introduce the particle-hole column $\Psi_k=(c_{k\uparrow},c_{-k\downarrow}^\dagger)^T$. Its quadratic block is the [Bogoliubov--de Gennes Hamiltonian](../../../../../../bogoliubov-de-gennes-hamiltonian.md)

$$
K_k=\Psi_k^\dagger\begin{pmatrix}\xi_k&-\Delta_k\\-\Delta_k&-\xi_k\end{pmatrix}\Psi_k+\xi_k.
$$

The [BCS coherence factors](../../../../../../bcs-coherence-factors.md) can be chosen to obey

$$
u_k^2=\frac12\left(1+\frac{\xi_k}{E_k}\right),\quad v_k^2=\frac12\left(1-\frac{\xi_k}{E_k}\right),\quad 2u_kv_k=\frac{\Delta_k}{E_k},\qquad E_k=\sqrt{\xi_k^2+\Delta_k^2}.
$$

With $u_k\ge0$, choose the sign of $v_k$ to match $\Delta_k$. The rotation diagonalizes the matrix to $\operatorname{diag}(E_k,-E_k)$. Reordering $\gamma_{-k\downarrow}\gamma_{-k\downarrow}^\dagger=1-\gamma_{-k\downarrow}^\dagger\gamma_{-k\downarrow}$ and restoring the mean-field constant gives

$$
\boxed{K=\sum_{k,\sigma}E_k\gamma_{k\sigma}^\dagger\gamma_{k\sigma}+\sum_k\left(\xi_k-E_k+\Delta_k\langle b_k^\dagger\rangle\right)}.
$$

The inverse transformation is $\gamma_{k\uparrow}=u_kc_{k\uparrow}-v_kc_{-k\downarrow}^\dagger$ and $\gamma_{-k\downarrow}=v_kc_{k\uparrow}^\dagger+u_kc_{-k\downarrow}$. Both annihilate $(u_k+v_kb_k^\dagger)|0\rangle$. Since every positive-energy [quasiparticle](../../../../../../quasiparticle.md) mode is empty, the normalized [BCS ground state](../../../../../../bcs-ground-state.md) is

$$
\boxed{|\mathrm{g.s.}\rangle=\prod_k\left(\cos\theta_k+\sin\theta_kc_{k\uparrow}^\dagger c_{-k\downarrow}^\dagger\right)|0\rangle}.
$$

Each momentum label refers to the pair $(k\uparrow,-k\downarrow)$ once; distinct labels use disjoint single-particle spin states.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
