<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The stated coordinate substitution splits the polynomial [basis](../../../../basis.md) into two three-cycles:

$$
x^2\longmapsto y^2\longmapsto z^2\longmapsto x^2,\qquad
xy\longmapsto yz\longmapsto xz\longmapsto xy.
$$

The identity fixes all six [basis vectors](../../../../basis-vector.md); neither nonidentity element fixes any. A [permutation representation](../../../../permutation-representation.md) has [character](../../../../character-of-a-representation.md) equal to the number of fixed [basis vectors](../../../../basis-vector.md), hence

$$
\boxed{\chi_{\widetilde R}(0)=6,\qquad
\chi_{\widetilde R}(1)=\chi_{\widetilde R}(2)=0.}
$$

The [representation multiplicity](../../../../multiplicity-of-an-irreducible-representation.md) of each [irreducible character](../../../../irreducible-character.md) is therefore

$$
m_k=\langle\chi_k,\chi_{\widetilde R}\rangle=\frac13\cdot6=2,
\qquad
\boxed{\widetilde R\cong2\rho_0\oplus2\rho_1\oplus2\rho_2.}
$$

An explicit [eigenbasis](../../../../eigenbasis.md) confirms the result. For $k=0,1,2$, put

$$
f_k=x^2+\alpha^{-k}y^2+\alpha^{-2k}z^2,\qquad
h_k=xy+\alpha^{-k}yz+\alpha^{-2k}xz.
$$

Then $\widetilde R(1)f_k=\alpha^kf_k$ and $\widetilde R(1)h_k=\alpha^kh_k$. Thus each three-cycle carries one copy of every [irreducible representation](../../../../irreducible-representation.md). These signs use precisely the source's substitution action; taking an inverse substitution would interchange $\rho_1$ and $\rho_2$, leaving the total decomposition unchanged.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
