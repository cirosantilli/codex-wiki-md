<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $a_n=N^{-1/2}\sum_ke^{ikn}a_k$ with $k=2\pi j/N$, choosing $N$ distinct values modulo $2\pi$ in the [Brillouin zone](../../../../../../brillouin-zone.md). The lattice spacing is one; for spacing $a$ the dimensionless variable here would be $ka$. Orthogonality of the discrete Fourier modes diagonalizes the bilinear Hamiltonian:

$$
H=E_0+\sum_k\varepsilon_k a_k^\dagger a_k,\qquad
\boxed{\varepsilon_k=2JS(1-\cos k)=4JS\sin^2(k/2).}
$$

This is the [nearest-neighbour ferromagnetic magnon dispersion](../../../../../../nearest-neighbour-ferromagnetic-magnon-dispersion.md). The printed expression is missing a factor of four for the stated exchange Hamiltonian. If $\omega_k$ denotes a physical frequency, $\hbar\omega_k=\varepsilon_k$; setting $\hbar=1$ does not remove that factor. The printed coefficient would require an exchange constant $J/4$ in the original Hamiltonian.

An independent check uses one spin lowering at site $n$. The exact one-magnon Hamiltonian relative to $E_0$ has diagonal element $2JS$ and off-diagonal elements $-JS$ at $n\pm1$, giving the same Fourier eigenvalue. At small $k$, **$\varepsilon_k\simeq JS k^2$**, and the $k=0$ state belongs to the degenerate ground multiplet. The quadratic low-energy branch is the ferromagnetic [type-B Goldstone boson](../../../../../../type-b-goldstone-boson.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
