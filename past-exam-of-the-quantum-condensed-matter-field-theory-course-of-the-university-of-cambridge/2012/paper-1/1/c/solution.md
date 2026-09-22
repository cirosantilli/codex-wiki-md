<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the specified [Fourier transform](../../../../../fourier-transform-split.md) convention, [normal ordering](../../../../../normal-ordering.md) gives

$$
\sum_n(c_n^\dagger c_{n+1}-c_nc_{n+1}^\dagger)=2\sum_k\cos k\,c_k^\dagger c_k,
$$

where the possible constant $\sum_ke^{ik}$ vanishes on the complete lattice momentum grid. Antisymmetry of opposite-momentum pairs similarly gives

$$
\sum_nc_n^\dagger c_{n+1}^\dagger=-i\sum_k\sin k\,c_k^\dagger c_{-k}^\dagger,\qquad
\sum_nc_nc_{n+1}=i\sum_k\sin k\,c_kc_{-k}.
$$

Hence

$$
H=-JgN+2J\sum_k(g-\cos k)c_k^\dagger c_k
+iJ\sum_k\sin k\,(c_k^\dagger c_{-k}^\dagger+c_kc_{-k}).
$$

Use the [Ising-chain Nambu spinor](../../../../../ising-chain-nambu-spinor.md) $\Psi_k=(c_k,-ic_{-k}^\dagger)^T$. Expanding its two diagonal terms uses $c_{-k}c_{-k}^\dagger=1-c_{-k}^\dagger c_{-k}$, retaining the constant. The result is

$$
\boxed{H=J\sum_k\Psi_k^\dagger\left[(g-\cos k)\sigma_z-\sin k\,\sigma_x\right]\Psi_k.}
$$

This is a full-zone sum. Its opposite-momentum components are redundant; treating each matrix eigenvalue as an independent physical excitation would miss the factor of two in the quasiparticle energy. Self-paired momenta have zero anomalous term and are ordinary number levels.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
