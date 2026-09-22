<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are $[x,p_x]=[y,p_y]=i\hbar$, with $[x,y]=[p_x,p_y]=[x,p_y]=[y,p_x]=0$. Operators from different Cartesian modes commute, so $(p_xp_y)^\dagger=p_yp_x=p_xp_y$ and $(xy)^\dagger=yx=xy$. Thus $J_1$ is Hermitian and represents an [observable](../../../../../observable.md) on the usual oscillator domain.

Introduce [annihilation operators](../../../../../annihilation-operator.md) $a_x=\sqrt{m\omega/(2\hbar)}x+ip_x/\sqrt{2m\hbar\omega}$ and similarly $a_y$. Set $N_x=a_x^\dagger a_x$, $N_y=a_y^\dagger a_y$ and $N=N_x+N_y$. The [Schwinger boson representation](../../../../../schwinger-boson-representation.md) gives

$$
H=\hbar\omega(N+1),\quad
J_1=\frac\hbar2(a_x^\dagger a_y+a_y^\dagger a_x),\quad
J_2=\frac\hbar2(N_y-N_x),\quad
J_3=\frac\hbar{2i}(a_x^\dagger a_y-a_y^\dagger a_x).
$$

For $A=a_x^\dagger a_y$ and $B=a_y^\dagger a_x$, $AB=N_x(N_y+1)$ and $BA=N_y(N_x+1)$. Therefore

$$
J_1^2+J_3^2=\frac{\hbar^2}{2}(AB+BA),\qquad
J^2=\frac{\hbar^2}{4}(N^2+2N).
$$

The [two-mode oscillator Casimir identity](../../../../../two-mode-oscillator-casimir-identity.md) is

$$
\boxed{H^2=4\omega^2J^2+\hbar^2\omega^2},\qquad
\boxed{\alpha=4\omega^2,\quad\beta=\hbar^2\omega^2}.
$$

Since $[N,A]=[N,B]=0$, $[H,J_1]=0$, and $J_1$ is conserved. However, $[J_1,J_2]=i\hbar J_3$ is not the zero operator, so there is no general joint eigenbasis. The exception is important: a [common eigenstate of two angular-momentum components](../../../../../common-eigenstate-of-two-angular-momentum-components.md) must satisfy $J_3\psi=0$, then the other [commutators](../../../../../commutator.md) force $J_1\psi=J_2\psi=0$. Thus only the $j=0$ sector admits a common state; here that is the oscillator [ground state](../../../../../ground-state.md).

Using $J^2=\hbar^2j(j+1)$, with $j=0,1/2,1,\ldots$, and selecting the positive [energy](../../../../../energy-split.md) branch gives

$$
\boxed{E_j=\hbar\omega(2j+1),\qquad g_j=2j+1}.
$$

Equivalently $N=2j=0,1,\ldots$, so $E_N=\hbar\omega(N+1)$ and the degeneracy is $N+1$, corresponding to $N_x=0,\ldots,N$.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
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
