<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the [two-component spinor calculus](../../../../../../two-component-spinor-calculus.md) convention $\epsilon_{01}=\epsilon^{01}=1$, with lowering $\xi_A=\xi^B\epsilon_{BA}$ and raising $\xi^A=\epsilon^{AB}\xi_B$. Thus $\epsilon^{AB}\epsilon_{AB}=2$; use the same convention for primed indices. The [spinor covariant derivative](../../../../../../spinor-covariant-derivative.md) preserves these [symplectic forms](../../../../../../symplectic-form.md).

Write $C_{AA'BB'}=[\nabla_{AA'},\nabla_{BB'}]$. It is antisymmetric on exchanging the two spacetime index pairs. The tensor-product decomposition of a [differential two-form](../../../../../../2-form.md) is

$$
\Lambda^2(S\otimes S')=(\operatorname{Sym}^2S\otimes\Lambda^2S')\oplus(\Lambda^2S\otimes\operatorname{Sym}^2S').
$$

This can also be checked directly: symmetrize or antisymmetrize separately in $A,B$ and $A',B'$. Antisymmetry under simultaneous pair exchange leaves precisely the symmetric–antisymmetric and antisymmetric–symmetric terms. An antisymmetric two-index spinor in a two-dimensional space is a multiple of its [symplectic form](../../../../../../symplectic-form.md). Therefore the [chiral spinor curvature operators](../../../../../../chiral-spinor-curvature-operator.md) are

$$
\Delta_{AB}=\frac12\epsilon^{A'B'}C_{AA'BB'},\qquad \Delta_{A'B'}=\frac12\epsilon^{AB}C_{AA'BB'}.
$$

Exchanging $A,B$ in the first expression and relabeling $A',B'$ shows $\Delta_{AB}=\Delta_{BA}$; the other symmetry follows identically. The projections reconstruct the whole six-component commutator, proving

$$
\boxed{[\nabla_{AA'},\nabla_{BB'}]=\epsilon_{A'B'}\Delta_{AB}+\epsilon_{AB}\Delta_{A'B'}.}
$$

Expanding each projected commutator and relabeling the contracted indices gives the requested derivative expressions:

$$
\boxed{\Delta_{AB}=\epsilon^{A'B'}\nabla_{(A|A'|}\nabla_{B)B'},\qquad \Delta_{A'B'}=\epsilon^{AB}\nabla_{A(A'}\nabla_{|B|B')}.}
$$

These formulas act tensorially on the field being differentiated, including the covariant derivative's action on the intermediate derivative index. The stated convention removes any ambiguity about signs from contracting alternating spinor forms in the opposite order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
