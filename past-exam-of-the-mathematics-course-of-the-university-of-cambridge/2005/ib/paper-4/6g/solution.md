<h1 id="6g/solution">Solution</h1>

↑ **Parent:** [6G](../6g.md)

The [operator commutator](../../../../../operator-commutator.md) is $[A,B]=AB-BA$, acting on a common domain where both products are defined. Use the [canonical commutation relation](../../../../../canonical-commutation-relation.md) $[x_i,p_j]=i\hbar\delta_{ij}$, with positions mutually commuting and momenta mutually commuting. On smooth test functions the only nonzero terms in the expansion are

$$
[yp_z,zp_x]=-i\hbar yp_x,\qquad [zp_y,xp_z]=i\hbar xp_y.
$$

Thus the [orbital angular momentum commutation relations](../../../../../orbital-angular-momentum-commutation-relations.md) give

$$
\boxed{[L_x,L_y]=i\hbar(xp_y-yp_x)=i\hbar L_z,\qquad [L_i,L_j]=i\hbar\epsilon_{ijk}L_k.}
$$

The product rule for a [operator commutator](../../../../../operator-commutator.md) gives

$$
[L^2,L_w]=\sum_i\big(L_i[L_i,L_w]+[L_i,L_w]L_i\big)
=i\hbar\sum_{i,k}\epsilon_{iwk}(L_iL_k+L_kL_i)=0,
$$

because the last operator expression is symmetric in $i,k$, whereas $\epsilon_{iwk}$ is antisymmetric. Hence $\boxed{[L^2,L_w]=0}$ for every component.

Write $r=\sqrt{x^2+y^2+z^2}$ and $P=x+y+z$. The differential [angular momentum operator](../../../../../angular-momentum-operator.md) $L=-i\hbar\,x\times\nabla$ annihilates every radial function, so $L_i(Pe^{-r})=e^{-r}L_iP$ and the same holds for its square. For example $L_xx=0$, $L_y^2x=\hbar^2x$ and $L_z^2x=\hbar^2x$. Cyclic symmetry gives $L^2y=2\hbar^2y$ and $L^2z=2\hbar^2z$ as well. Therefore

$$
\boxed{L^2\psi=e^{-r}L^2P=2\hbar^2\psi.}
$$

The wavefunction is an $l=1$ [orbital angular momentum](../../../../../orbital-angular-momentum.md) state; its nontrivial radial factor does not change its angular [eigenvalue](../../../../../eigenvalue.md). The calculation holds away from the origin and defines the same angular-operator identity in the square-integrable state space.

## ↑ Ancestors (10)

1. [6G](../6g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
