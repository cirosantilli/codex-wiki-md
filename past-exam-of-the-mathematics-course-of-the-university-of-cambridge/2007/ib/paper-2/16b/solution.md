<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

The [orbital angular momentum](../../../../../orbital-angular-momentum.md) operators are $\mathbf L=\mathbf x\times\mathbf p$, so

$$
L_1=x_2p_3-x_3p_2,\qquad L_2=x_3p_1-x_1p_3,\qquad L_3=x_1p_2-x_2p_1.
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are $[x_i,x_j]=[p_i,p_j]=0$ and $[x_i,p_j]=i\hbar\delta_{ij}$. On a common domain of smooth wavefunctions, the product [commutator](../../../../../commutator.md) identity gives

$$
[x_ap_b,x_cp_d]=-i\hbar\delta_{bc}x_ap_d+i\hbar\delta_{ad}x_cp_b.
$$

Contract this with $\epsilon_{iab}\epsilon_{jcd}$. The first term contributes $i\hbar(\delta_{ij}\mathbf x\cdot\mathbf p-x_jp_i)$ and the second contributes $i\hbar(x_ip_j-\delta_{ij}\mathbf x\cdot\mathbf p)$. Their sum is

$$
\boxed{[L_i,L_j]=i\hbar(x_ip_j-x_jp_i)=i\hbar\epsilon_{ijk}L_k.}
$$

This verifies the [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) explicitly. Similarly,

$$
[L_i,p_j]=\epsilon_{iab}[x_ap_b,p_j]
=i\hbar\epsilon_{ijb}p_b,
\qquad \boxed{[L_i,p_j]=i\hbar\epsilon_{ijk}p_k.}
$$

In the position representation $\mathbf p=-i\hbar\nabla$. For a radial wavefunction, $\nabla\Psi_0=\Psi_0'(r)\mathbf x/r$, parallel to $\mathbf x$, so

$$
\boxed{\mathbf L\Psi_0=-i\hbar\mathbf x\times\nabla\Psi_0=0.}
$$

Write $\Phi_i=h(r)x_i$ with $h(r)=\Psi_0'(r)/r$. The operator $L_3=-i\hbar(x_1\partial_2-x_2\partial_1)$ annihilates the radial factor. It gives $L_3x_1=i\hbar x_2$, $L_3x_2=-i\hbar x_1$, and $L_3x_3=0$, hence

$$
\boxed{L_3\Phi_3=0,\qquad
L_3(\Phi_1\pm i\Phi_2)=\pm\hbar(\Phi_1\pm i\Phi_2).}
$$

Thus these components, when nonzero, are the specified [eigenfunctions](../../../../../eigenfunction.md) with [eigenvalues](../../../../../eigenvalue.md) $0,+\hbar,-\hbar$. This is an example of [angular momentum of a radial function times a linear polynomial](../../../../../angular-momentum-of-a-radial-function-times-a-linear-polynomial.md).

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
