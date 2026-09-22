<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

On a common domain where all products are defined, expansion of the [operator commutator](../../../../../operator-commutator.md) gives

$$
A[B,C]+[A,C]B=ABC-ACB+ACB-CAB=\boxed{[AB,C]}.
$$

Use the usual quantum position and momentum operators with $p_j=-i\hbar\partial_j$, the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[x_i,p_j]=i\hbar\delta_{ij}$, and [wavefunctions](../../../../../wave-function.md) with the decay/domain conditions needed for adjoints. The cross-coordinate operators commute, so

$$
L^\dagger=p_yx-p_xy=xp_y-yp_x=L.
$$

For an eigenstate $L\psi=\lambda\psi$, hermiticity gives $\lambda\|\psi\|^2=\overline\lambda\|\psi\|^2$, hence its [eigenvalue](../../../../../eigenvalue.md) is real.

The product identity gives $[L,x]=i\hbar y$, $[L,y]=-i\hbar x$, $[L,p_x]=i\hbar p_y$, $[L,p_y]=-i\hbar p_x$. Thus the commutators with $x^2,y^2$ cancel, as do those with $p_x^2,p_y^2$, proving **$[L,H]=0$**. Each oscillator energy [eigenspace](../../../../../eigenspace.md) is finite-dimensional and preserved by $L$; the Hermitian restriction of $L$ can be diagonalized within it. Therefore an energy eigenbasis can be chosen to diagonalize [angular momentum](../../../../../angular-momentum.md) as well.

For $\phi_0=e^{-(x^2+y^2)/(2\hbar)}$, differentiation gives $\Delta\phi_0=[(x^2+y^2)/\hbar^2-2/\hbar]\phi_0$, so $H\phi_0=\hbar\phi_0$. Also $[H,x]=-i\hbar p_x$ and $p_x\phi_0=ix\phi_0$, giving $H(x\phi_0)=2\hbar x\phi_0$; the same calculation holds for $y\phi_0$. Directly $L=-i\hbar(x\partial_y-y\partial_x)$, hence

$$
L\phi_0=0,\qquad L\phi_x=i\hbar\phi_y,\qquad L\phi_y=-i\hbar\phi_x.
$$

The simultaneous normalized states are

$$
\boxed{\psi_1=\frac{(x+iy)\phi_0}{\sqrt\pi\,\hbar},\qquad
\psi_2=\frac{(x-iy)\phi_0}{\sqrt\pi\,\hbar},\qquad
\lambda_1=\hbar,\quad\lambda_2=-\hbar,\quad E_1=E_2=2\hbar.}
$$

Their squared unnormalized [norm](../../../../../norm.md) is $\int r^2e^{-r^2/\hbar}\,d^2x=\pi\hbar^2$. Their [inner product](../../../../../inner-product.md) vanishes because the integral of $(x-iy)^2e^{-r^2/\hbar}$ is zero: the $xy$ term is odd and the $x^2,y^2$ terms cancel by rotational symmetry.

Put $a=e\mathcal E$. The new Hamiltonian has

$$
\boxed{[L,H']=-a[L,x]=-i\hbar ay.}
$$

For a nonzero applied coupling $a$, a common normalizable eigenstate would be killed by the commutator, so $y\psi=0$. It would have to be supported on the line $y=0$, a set of zero planar measure, and would be the zero vector in $L^2$. Thus there are no nonzero common eigenstates in this case. Merely having a nonzero commutator would not prove that conclusion for arbitrary operators; the multiplication operator here has trivial kernel. If $a=0$, the original simultaneous eigenstates remain.

For the [shifted two-dimensional oscillator in a uniform electric field](../../../../../shifted-two-dimensional-oscillator-in-a-uniform-electric-field.md), complete the square:

$$
H'=\frac12(p_{x'}^2+p_{y'}^2+x'^2+y'^2)-\frac{a^2}2,\qquad x'=x-a,\quad y'=y.
$$

Therefore $\psi_1(x',y')$ and $\psi_2(x',y')$ have the same shifted energy

$$
\boxed{E'_1=E'_2=2\hbar-\frac{(e\mathcal E)^2}2.}
$$

The modified [angular momentum](../../../../../angular-momentum.md) is

$$
\boxed{L'=(x-e\mathcal E)p_y-yp_x=L-e\mathcal E p_y.}
$$

It is [angular momentum](../../../../../angular-momentum.md) about the displaced centre, commutes with $H'$, and has [eigenvalues](../../../../../eigenvalue.md) $\pm\hbar$ on the two translated states.

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
