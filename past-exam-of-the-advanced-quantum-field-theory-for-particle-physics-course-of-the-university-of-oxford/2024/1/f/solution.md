<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

In the [Weyl representation of the gamma matrices](../../../../weyl-representation-of-the-gamma-matrices.md), write each [Dirac field](../../../../dirac-field.md) as $\psi_i=(\ell_{i\alpha},r_i^{\dot\alpha})^T$, where $\ell_i$ and $r_i$ have opposite [chirality](../../../../chirality-physics.md). With the [Weyl sigma matrices](../../../../weyl-sigma-matrices.md) $\sigma^\mu=(\mathbf1,\boldsymbol\sigma)$ and $\bar\sigma^\mu=(\mathbf1,-\boldsymbol\sigma)$,

$$
\boxed{\mathcal L=\sum_{i=1}^2\left[
i\ell_i^\dagger\bar\sigma^\mu\partial_\mu\ell_i
+ir_i^\dagger\sigma^\mu\partial_\mu r_i
-m(\ell_i^\dagger r_i+r_i^\dagger\ell_i)\right].}
$$

The [Dirac mass term](../../../../dirac-mass-term.md) couples the two [Weyl fields](../../../../weyl-field.md). Under $\ell\mapsto U_L\ell$, $r\mapsto U_Rr$, its first term acquires $U_L^\dagger U_R$, so a common nonzero [mass](../../../../mass.md) requires $U_L=U_R$. At zero [mass](../../../../mass.md) there is no such constraint:

$$
\boxed{G_{\rm number\ preserving}=U(2)_L\times U(2)_R.}
$$

This is the [chiral flavour symmetry of massless Dirac fields](../../../../chiral-flavour-symmetry-of-massless-dirac-fields.md). Its eight [Noether currents](../../../../noether-current.md) are $j_{L,A}^\mu=\ell^\dagger\bar\sigma^\mu T^A\ell$ and $j_{R,A}^\mu=r^\dagger\sigma^\mu T^Ar$. The sum $j_R+j_L$ is the [vector current](../../../../vector-current.md), and $j_R-j_L$ is the [axial current](../../../../axial-current.md), for each flavour generator. This statement concerns the free theory in flat spacetime; an interacting theory can have a [chiral anomaly](../../../../chiral-anomaly.md).

For completeness, allowing the extra transformations described in part [e](../e.md) gives four left-handed [Weyl fields](../../../../weyl-field.md), $q=(\ell_1,\ell_2,r_1^c,r_2^c)^T$, where $r_i^c$ is the left-handed [charge-conjugate field](../../../../charge-conjugate-field.md) of $r_i$. After [integration by parts](../../../../integration-by-parts.md) their kinetic term is $iq^\dagger\bar\sigma^\mu\partial_\mu q$, whose maximal linear [unitary group](../../../../unitary-group.md) is $U(4)$. The symmetric [mass matrix](../../../../mass-matrix.md) for equal [Dirac masses](../../../../dirac-mass-term.md) is

$$
M=m\begin{pmatrix}0&\mathbf1_2\\\mathbf1_2&0\end{pmatrix},\qquad
\mathcal L_m=-\frac12(q^TMq+\text{Hermitian conjugate}),
$$

with the antisymmetric spinor contraction implicit. A unitary change of basis makes $M=m\mathbf1_4$; preserving both the kinetic term and $M$ requires $V^\dagger V=V^TV=\mathbf1_4$, hence real $V\in O(4)$. Thus the unrestricted free-theory enhancement is $U(4)$ at zero [mass](../../../../mass.md) and $O(4)$ at equal nonzero [mass](../../../../mass.md); the familiar $U(2)_L\times U(2)_R$ and diagonal $U(2)$ are their common-[fermion number](../../../../fermion-number.md)-preserving subgroups.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
