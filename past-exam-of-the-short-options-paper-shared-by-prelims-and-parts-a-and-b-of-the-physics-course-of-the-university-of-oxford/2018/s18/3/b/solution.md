<h1 id="s18/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In two spatial dimensions there are only two kinetic matrices and one [mass](../../../../../mass.md) matrix. The three [Pauli matrices](../../../../../pauli-matrices.md) square to identity and anticommute pairwise, so

$$
\boxed{H_{2+1}=c\sigma_xp_x+c\sigma_yp_y+mc^2\sigma_z}
$$

is a two-component Dirac [Hamiltonian](../../../../../hamiltonian.md) with $H_{2+1}^2=c^2(p_x^2+p_y^2)+m^2c^4$. It therefore reproduces the stated first-order equation and its Klein-Gordon square. Requiring a fourth anticommuting matrix in three spatial dimensions is precisely what prevented this two-component construction above.

**Printed angular-momentum qualification.** Define the dimensionless [spin](../../../../../spin.md) $s_i=-i\varepsilon_{ijk}\alpha_j\alpha_k/4$ and the physical orbital [angular momentum](../../../../../angular-momentum.md) $\ell_i=\varepsilon_{ijk}x_jp_k$, with $[x_i,p_j]=i\hbar\delta_{ij}$. Then

$$
[s_i,s_j]=i\varepsilon_{ijk}s_k,\qquad
[\ell_i,\ell_j]=i\hbar\varepsilon_{ijk}\ell_k,\qquad [\ell_i,s_j]=0.
$$

The source prints $L_i=i\ell_i$ instead. Taken literally, it is anti-Hermitian, has incompatible units with the dimensionless [spin](../../../../../spin.md) when they are added, and gives

$$
\boxed{[L_i,L_j]=-\hbar\varepsilon_{ijk}L_k,\qquad
[J_i,J_j]=\varepsilon_{ijk}(-\hbar L_k+i s_k).}
$$

It cannot yield the requested usual angular-momentum algebra or conservation law. For a concrete counterexample set $\hbar=1$ and take a wave with [momentum](../../../../../momentum-split.md) along $z$. Since

$$
[H_D,\ell_i]=-ic(\boldsymbol\alpha\times\mathbf p)_i,
\qquad [H_D,s_i]=ic(\boldsymbol\alpha\times\mathbf p)_i,
$$

the printed $J_i=i\ell_i+s_i$ obeys $[H_D,J_x]=(1+i)c\alpha_y p_z\ne0$.

The physically consistent operator is $\mathbf J_{\rm phys}=\boldsymbol\ell+\hbar\mathbf s$. It satisfies

$$
\boxed{[J_{{\rm phys},i},J_{{\rm phys},j}]=i\hbar\varepsilon_{ijk}J_{{\rm phys},k},\qquad
[H_D,J_{{\rm phys},i}]=0.}
$$

The cancellation follows directly from the two mixed [commutators](../../../../../commutator.md) above. In a spherical basis the free spinor can be labelled by [energy](../../../../../energy-split.md), $j=1/2,3/2,\ldots$, and $m_j=-j,\ldots,j$, together with a [parity](../../../../../parity.md) or equivalent Dirac angular label distinguishing the two orbital couplings $\ell=j\pm1/2$. Alternatively one can choose a [momentum](../../../../../momentum-split.md) and [helicity](../../../../../helicity.md) basis. One cannot simultaneously assign all components of [momentum](../../../../../momentum-split.md) and all angular labels as independent commuting observables.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
