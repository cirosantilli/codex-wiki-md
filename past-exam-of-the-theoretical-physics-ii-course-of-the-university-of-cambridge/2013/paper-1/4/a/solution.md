<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There is a state-assumption issue. For a [number-conserving Gaussian quantum state](../../../../../number-conserving-gaussian-quantum-state.md) with no anomalous contractions, put $\psi_i=\psi(\mathbf r_i)$, $n_i=\langle\psi_i^\dagger\psi_i\rangle$ and the [one-body density matrix](../../../../../one-body-density-matrix.md) $g_{ij}=\langle\psi_i^\dagger\psi_j\rangle$. [Wick's theorem](../../../../../wick-s-theorem.md) pairs each creation operator with an annihilation operator. The direct pairing gives $n_1n_2$; the exchanged pairing gives $\epsilon g_{12}g_{21}$, with $\epsilon=+1$ for [bosons](../../../../../boson.md) and $-1$ for [fermions](../../../../../fermion.md). Hence

$$
\boxed{C_{12}=n_1n_2+\epsilon|g_{12}|^2}.
$$

[normal ordering](../../../../../normal-ordering.md) removes the equal-position delta-function self-counting term. Fermionic occupation-number product states are [Slater determinants](../../../../../slater-determinant.md) and obey this [Wick theorem](../../../../../wick-s-theorem.md). Independent thermal bosonic modes also obey it, with $N_\alpha$ understood as mean occupations.

**A bosonic Fock product state does not generally obey the asserted identity.** The [bosonic number-state corrections to Gaussian density correlations](../../../../../bosonic-number-state-corrections-to-gaussian-density-correlations.md) follow from $\langle a_\alpha^{\dagger2}a_\alpha^2\rangle=N_\alpha(N_\alpha-1)$ and give

$$
\boxed{C_{12}^{\rm Fock}=n_1n_2+|g_{12}|^2
-\sum_\alpha N_\alpha(N_\alpha+1)|\varphi_\alpha(\mathbf r_1)|^2
|\varphi_\alpha(\mathbf r_2)|^2}.
$$

For one occupied mode this is $N(N-1)|\varphi_1|^2|\varphi_2|^2$, whereas the uncorrected Gaussian expression gives $2N^2|\varphi_1|^2|\varphi_2|^2$. **This counterexample disproves the asserted identity for arbitrary bosonic number-product states.** The formulas below give both the Gaussian result, with its additional state assumption, and the exact bosonic number-state alternative. The ensemble distinction is also explicit in a later primary treatment of ideal-gas correlations.[Abstract: canonical reduced density matrices versus grand-canonical Wick factorization; 2016](../../../../../quantum-correlations-of-ideal-bose-and-fermi-gases-in-the-canonical-ensemble-by-kazumasa-tsutsui-and-takafumi-kita.md)

## ↑ Ancestors (15)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
