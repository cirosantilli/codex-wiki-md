<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For distinguishable particles, the ordered spatial products are independent states, and neither [singlet states](../../../../../singlet-state.md) nor [triplet states](../../../../../spin-one-half-triplet-state.md) are excluded from any orbital occupation. The unperturbed [energy eigenvalues](../../../../../energy-eigenvalue-split.md) are

$$
E_{rs,0}=(r^2+s^2)\varepsilon+3J/4,\qquad
E_{rs,1}=(r^2+s^2)\varepsilon-J/4.
$$

For $0<J\ll\varepsilon$, the three lowest distinct [energy levels](../../../../../energy-level.md) are

$$
\boxed{\begin{array}{c|c|c}
\text{energy}&\text{multiplicity}&\text{normalized eigenfunctions}\\ \hline
2\varepsilon-J/4&3&u_1(x_1)u_1(x_2)\chi_{1M}\\
2\varepsilon+3J/4&1&u_1(x_1)u_1(x_2)\chi_{00}\\
5\varepsilon-J/4&6&u_1(x_1)u_2(x_2)\chi_{1M},\ u_2(x_1)u_1(x_2)\chi_{1M}
\end{array}}
$$

where $M=-1,0,1$. The first two levels do have zero first-order correction, since their spatial [expectation value](../../../../../expectation-value.md) factorizes as $\langle1|x|1\rangle^2=0$.

The last instruction in the original PDF is false for the third level. Although every diagonal product-state [matrix element](../../../../../matrix-element.md) vanishes, the two orbital states have [degenerate energy levels](../../../../../degenerate-energy-levels.md). [Degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md) requires diagonalizing the perturbation within their span. For each $M$, its matrix in the ordered basis $(u_1u_2,u_2u_1)$ is

$$
W=\alpha\begin{pmatrix}0&D\\D&0\end{pmatrix},\qquad
D=\langle1|x|2\rangle\langle2|x|1\rangle>0.
$$

The [eigenfunctions](../../../../../eigenfunction.md) are $\Phi_{12}^\pm\chi_{1M}$, with

$$
\boxed{\delta E_\pm^{(1)}=\pm\alpha D
=\pm\frac{256\alpha a^2}{81\pi^4},\qquad
\text{multiplicity three for each branch}.}
$$

Thus the sixfold unperturbed level splits into two triplets. Its average shift is zero, and the diagonal expectation in an individual ordered product state is zero, but neither fact makes all its [energy eigenvalue](../../../../../energy-eigenvalue-split.md) corrections zero. This is the [degenerate orbital exchange splitting from a product perturbation](../../../../../degenerate-orbital-exchange-splitting-from-a-product-perturbation.md); distinguishability allows both combinations rather than removing their coupling.

For negative $J$, the lowest two rows exchange order and the third unperturbed level is instead the twofold singlet orbital pair at $5\varepsilon+3J/4$. It splits into $\Phi_{12}^\pm\chi_{00}$ with the same shifts $\pm\alpha D$, each nondegenerate. At $J=0$, the three lowest distinct unperturbed energies are $2\varepsilon,5\varepsilon,8\varepsilon$, with multiplicities $4,8,4$. The first and third have zero first-order shift; the middle splits by $\pm\alpha D$, each fourfold. The printed zero-shift assertion therefore fails also in the zero-exchange limit.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
