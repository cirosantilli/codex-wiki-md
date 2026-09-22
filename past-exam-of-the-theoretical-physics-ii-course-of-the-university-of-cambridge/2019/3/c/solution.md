<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is a normalization mismatch in the printed definitions: $\sigma^x\pm i\sigma^y$ have nonzero entries of magnitude two, whereas a single fermionic creation or annihilation operator has magnitude one. To obtain the intended [Jordan–Wigner transformation](../../../../jordan-wigner-transformation.md), use normalized spin ladders $s_j^\pm=(\sigma_j^x\pm i\sigma_j^y)/2$. The given fermion expressions represent these $s_j^\pm$. The [two-site Jordan-Wigner normalization and signs](../../../../two-site-jordan-wigner-normalization-and-signs.md) then fix every factor unambiguously.

Put $n_j=f_j^\dagger f_j$ and $P_1=e^{i\pi n_1}=1-2n_1$. The [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) give $P_1^2=I$, $P_1f_1=-f_1P_1$, and $[P_1,f_2]=[P_1,f_2^\dagger]=0$. Hence

$$
[s_1^-,s_1^+]=[f_1,f_1^\dagger]=1-2n_1=-\sigma_1^z,\qquad
[\sigma_1^z,\sigma_2^z]=4[n_1,n_2]=0,
$$



$$
[s_1^-,s_2^-]=f_1P_1f_2-P_1f_2f_1=-P_1\{f_1,f_2\}=0,
$$

and

$$
[s_2^-,s_2^+]=[P_1f_2,f_2^\dagger P_1]=f_2f_2^\dagger-f_2^\dagger f_2=1-2n_2=-\sigma_2^z.
$$

These are the [spin commutation relations](../../../../spin-commutation-relations.md), with distinct sites commuting. If one retains the unscaled symbols $\sigma_j^\pm=2s_j^\pm$, the first and last displayed commutators instead equal $-4\sigma_j^z$; the off-site commutators remain zero. Setting the unscaled $\sigma_j^-$ equal to $f_j$ would contradict the original [Pauli matrices](../../../../pauli-matrices.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
