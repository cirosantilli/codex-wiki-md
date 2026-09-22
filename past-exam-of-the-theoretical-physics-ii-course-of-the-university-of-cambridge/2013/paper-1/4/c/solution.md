<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [three-point density correlation of an ideal quantum gas](../../../../../three-point-density-correlation-of-an-ideal-quantum-gas.md) follows first for a [number-conserving Gaussian quantum state](../../../../../number-conserving-gaussian-quantum-state.md). There are six pairings, one for each [permutation](../../../../../permutation.md) of three annihilation operators. The identity gives the product of densities; each [transposition](../../../../../transposition-permutation.md) has sign $\epsilon$; both three-cycles have positive sign. Thus

$$
\boxed{\begin{aligned}
C^{(3)}_{123}={}&n_1n_2n_3
+\epsilon\left[n_1|g_{23}|^2+n_2|g_{13}|^2+n_3|g_{12}|^2\right]\\
&+g_{12}g_{23}g_{31}+g_{13}g_{32}g_{21}.
\end{aligned}}
$$

The last two terms are [complex conjugates](../../../../../complex-conjugate.md). They equal $2\operatorname{Re}(g_{12}g_{23}g_{31})$, not an additional signed pair term. This is the [permanent of a matrix](../../../../../permanent-mathematics.md) $(g_{ij})$ for [bosons](../../../../../boson.md) and its [determinant](../../../../../determinant.md) for [fermions](../../../../../fermion.md). [Wick's theorem](../../../../../wick-s-theorem.md) supplies the six terms only with the state assumption stated in part (a).

For completeness an exact bosonic Fock-state alternative can be given without that assumption. Let $\boldsymbol\ell$ be a mode-occupation decrement with $\sum_\alpha\ell_\alpha=3$. Define $A_{\boldsymbol\ell}(1,2,3)$ as the sum of $\prod_{j=1}^3\varphi_{\alpha_j}(\mathbf r_j)$ over all distinct ordered triples having these mode multiplicities. Acting three annihilation fields on the [number state](../../../../../number-state.md) leaves mutually orthogonal states for different $\boldsymbol\ell$. Therefore

$$
\boxed{C^{(3),\rm Fock}_{123}=\sum_{\boldsymbol\ell:\,\sum\ell_\alpha=3}
\left[\prod_\alpha N_\alpha^{\underline{\ell_\alpha}}\right]
|A_{\boldsymbol\ell}(1,2,3)|^2}.
$$

Here $N^{\underline\ell}=N!/(N-\ell)!$, with zero when $\ell>N$. This expression includes repeated-mode occupation corrections absent from the Gaussian permanent; for a single mode it reduces to $N(N-1)(N-2)\prod_j|\varphi(\mathbf r_j)|^2$.

## ↑ Ancestors (15)

1. [C](../c.md)
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
