<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [two-mode approximation for a Bose gas](../../../../two-mode-approximation-for-a-bose-gas.md) retains the real localized [orbitals](../../../../single-particle-orbital.md):

$$
\boxed{\hat\psi^\dagger(\mathbf r)\simeq\varphi_L(\mathbf r)\hat a_L^\dagger+\varphi_R(\mathbf r)\hat a_R^\dagger.}
$$

It is valid when the lowest doublet is well separated from higher [energy levels](../../../../energy-level.md), and the [temperature](../../../../temperature-split.md) and interaction-induced changes of the [orbitals](../../../../single-particle-orbital.md) are small on that separation. More explicitly, if $\Delta$ is the [energy gap](../../../../energy-gap.md) to discarded [orbitals](../../../../single-particle-orbital.md), sufficient low-[energy](../../../../energy-split.md) conditions are $k_BT,t,NU_0I\ll\Delta$, where $I=\int d^3r\,|\varphi_L|^4$. A deep [double-well potential](../../../../double-well-potential.md) suppresses interwell interaction overlaps. Large $N$ alone does not justify the truncation: increasing $N$ at fixed coupling can violate the interaction condition.

Let $\epsilon=(E_0+E_1)/2$ and use the even and odd [eigenfunctions](../../../../eigenfunction.md) to evaluate the projected one-particle [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md):

$$
\langle L|h_0|L\rangle=\langle R|h_0|R\rangle=\epsilon,\qquad
\langle L|h_0|R\rangle=\frac{E_0-E_1}{2}=-t.
$$

Thus

$$
\hat H_0=\epsilon(\hat n_L+\hat n_R)-t(\hat a_L^\dagger\hat a_R+\hat a_R^\dagger\hat a_L),\qquad
\boxed{t=\frac{E_1-E_0}{2}>0.}
$$

The same [quantum tunnelling](../../../../quantum-tunnelling.md) matrix element is $t=-\int d^3r\,\varphi_Lh_0\varphi_R$. Reflection symmetry makes $\int|\varphi_L|^4=\int|\varphi_R|^4=I$. Neglecting mixed [contact interaction](../../../../contact-interaction-quantum-mechanics.md) integrals leaves

$$
\hat H_{\rm int}=\frac{U_0I}{2}\sum_{j=L,R}(\hat a_j^\dagger)^2\hat a_j^2
=\frac{U_0I}{2}\sum_{j=L,R}\hat n_j(\hat n_j-1).
$$

The last step is the [normal-ordered boson pair count](../../../../normal-ordered-boson-pair-count.md), following from the [canonical commutation relation](../../../../canonical-commutation-relation.md). Consequently the [two-site Bose-Hubbard model](../../../../two-site-bose-hubbard-model.md) has precisely the requested coefficients

$$
\boxed{w=\frac{U_0}{2}\int d^3r\,|\varphi_L(\mathbf r)|^4,\qquad
\mu=w-\frac{E_0+E_1}{2},}
$$

and

$$
\boxed{\hat H=-t(\hat a_L^\dagger\hat a_R+\hat a_R^\dagger\hat a_L)
+w(\hat n_L^2+\hat n_R^2)-\mu(\hat n_L+\hat n_R).}
$$

Here $\mu$ is the coefficient obtained by rewriting the fixed-[particle number](../../../../particle-number.md) [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md), rather than an independently prescribed thermodynamic [chemical potential](../../../../chemical-potential-split.md). Adding a reservoir term $-\mu_{\rm res}\hat N$ would replace it by $\mu+\mu_{\rm res}$.

The negligible-overlap instruction applies to the mixed [contact interaction](../../../../contact-interaction-quantum-mechanics.md) integrals while the small [quantum tunnelling](../../../../quantum-tunnelling.md) matrix element is retained. Exactly disjoint smooth [orbitals](../../../../single-particle-orbital.md) for a local $h_0$ would also give $t=0$; setting every overlap-related matrix element identically to zero would discard the physical splitting one is trying to describe.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
