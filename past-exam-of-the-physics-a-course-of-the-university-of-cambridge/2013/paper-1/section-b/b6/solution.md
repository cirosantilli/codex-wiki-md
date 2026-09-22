<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Apply the [radial momentum operator](../../../../../radial-momentum-operator.md) to a smooth radial test function. More generally $[f(r),p_r]=i\hbar f'(r)$, giving the first two labelled identities. Expanding the square gives the third:

$$
\text{(i)}\ [r,p_r]=i\hbar,\qquad
\text{(ii)}\ [r^{-1},p_r]=-i\hbar r^{-2},\qquad
\text{(iii)}\ p_r^2=-\hbar^2\left(\partial_r^2+\frac2r\partial_r\right).
$$

The kinetic-energy decomposition is $p^2=p_r^2+L^2/r^2$. A [central potential](../../../../../central-potential.md) commutes with $L^2$ and $L_z$, so choose simultaneous angular [eigenfunctions](../../../../../eigenfunction.md) $Y_{lm}$, with $L^2=l(l+1)\hbar^2$ and $l=0,1,\ldots$. The radial [Hamiltonian](../../../../../hamiltonian.md) consequently has the stated centrifugal term. The radial inner product uses measure $r^2dr$; adjoints below are taken on compatible regular bound-state domains. The formal radial [momentum](../../../../../momentum-split.md) is not thereby asserted to be a self-adjoint observable on a half-line.

Set $q=l+1$, $W=-q/r+1/(qa)$ and $D=i p_r/\hbar$. Since $D^\dagger=-D$ formally and $[D,W]=W'=q/r^2$,

$$
A_l^\dagger A_l=\frac{a^2}{2}\left[\frac{p_r^2}{\hbar^2}+\frac{l(l+1)}{r^2}-\frac2{ar}+\frac1{q^2a^2}\right].
$$

The [hydrogen radial Hamiltonian factorization](../../../../../hydrogen-radial-hamiltonian-factorization.md) follows by matching the Coulomb coefficient, which fixes the [Bohr radius](../../../../../bohr-radius.md)

$$
\boxed{a=\frac{4\pi\epsilon_0\hbar^2}{me^2}},\qquad
H_l=\frac{\hbar^2}{ma^2}\left(A_l^\dagger A_l-\frac1{2(l+1)^2}\right).
$$

For the second pair of labelled relations, the opposite product changes the sign of $W'$, hence

$$
\text{(i)}\quad[A_l,A_l^\dagger]=a^2W'=\frac{a^2(l+1)}{r^2}
=\frac{ma^2}{\hbar^2}(H_{l+1}-H_l).
$$

Using $[A,A^\dagger A]=[A,A^\dagger]A$ in the [factorization](../../../../../factorization.md) then gives

$$
\text{(ii)}\quad[A_l,H_l]=(H_{l+1}-H_l)A_l,
\qquad H_{l+1}A_l=A_lH_l.
$$

This [Coulomb angular-momentum intertwining](../../../../../coulomb-angular-momentum-intertwining.md) means applying $A_l$ to an [energy eigenstate](../../../../../energy-eigenstate.md) either gives zero or an eigenstate of $H_{l+1}$ with the same [energy](../../../../../energy-split.md). For a normalized negative-energy state,

$$
\|A_l\psi\|^2=\frac{ma^2E}{\hbar^2}+\frac1{2(l+1)^2}\ge0.
$$

At fixed $E<0$ this would become negative if raising $l$ continued indefinitely. The [bound-state ladder termination by norm positivity](../../../../../bound-state-ladder-termination-by-norm-positivity.md) occurs at some $L$ with $A_L\psi=0$, giving

$$
\boxed{E_n=-\frac{\hbar^2}{2ma^2n^2}=-\frac{me^4}{2(4\pi\epsilon_0)^2\hbar^2n^2},\quad n=L+1=1,2,\ldots}.
$$

The terminating radial function is proportional to $r^L e^{-r/[(L+1)a]}$, regular and normalizable; adjoint intertwiners generate lower $l$ values at fixed $n$. Positive-energy [scattering states](../../../../../scattering-state.md) are not subject to this terminating negative-energy argument. Here $m$ is the [mass](../../../../../mass.md) in the supplied [Hamiltonian](../../../../../hamiltonian.md); including nuclear motion replaces it by the [reduced mass](../../../../../reduced-mass.md).

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
