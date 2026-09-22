<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Both $A$ and $C$ are real symmetric and couple only neighboring sites whose diagonal entries in $J$ have opposite signs. For an entry $x_{mn}$ of $x=iA$ or $iC$, symmetry gives $(x^TJ+Jx)_{mn}=(J_{nn}+J_{mm})x_{mn}$. Every nonzero entry joins signs $+1$ and $-1$, while the diagonal entries vanish. Hence $\boxed{x^TJ+Jx=0\text{ for }x=iA,iC}$.

The condition is preserved by real linear combinations and [commutators](../../../../../../commutator.md), so the entire [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md) satisfies it. For the physical generator $x(t)=-i(A+f(t)C)$, differentiation gives $\frac{d}{dt}(U^TJU)=U^T(x^TJ+Jx)U=0$, and therefore $\boxed{U(t)^TJU(t)=J}$. This is an [orthogonal dynamical symmetry in quantum control](../../../../../../orthogonal-dynamical-symmetry-in-quantum-control.md): a preserved symmetric bilinear form. It need not give eigenspaces of a commuting operator; indeed $J$ does not commute with $A$ or $C$.

Set $D=\operatorname{diag}(1,i,1)$. Then $D^TJD=I$, so the transformed generators $x'=D^\dagger xD$ satisfy $x'^T+x'=0$ as well as $x'^\dagger+x'=0$. They are consequently real antisymmetric, lying in $\mathfrak{so}(3)$. The original generators already supply the independent directions $p=iC=i(E_{12}+E_{21})$ and $q=i(A-C)=i(E_{23}+E_{32})$, and their [commutator](../../../../../../commutator.md) is $[p,q]=E_{31}-E_{13}$. These three independent directions exhaust the three-dimensional algebra. Thus

$$
\boxed{D^\dagger\mathfrak gD=\mathfrak{so}(3),\qquad \dim\mathfrak g=3}.
$$

Here $E_{mn}$ denotes a [matrix unit](../../../../../../matrix-unit.md). The reachable connected group is a unitary conjugate of $SO(3)$, a proper subgroup of $SU(3)$, so there is no [unitary operator controllability](../../../../../../unitary-operator-controllability.md).

Pure-state control also fails. For every reachable state $\psi'=U\psi$, the quantity $\psi'^TJ\psi'=\psi^TJ\psi$ is invariant, and its absolute value is unchanged even by an overall state phase. The normalized states $e_1$ and $(e_1+e_2)/\sqrt2$ have respectively $|\psi^TJ\psi|=1$ and $0$, so no allowed control connects their rays. Therefore $\boxed{\text{neither pure-state nor density operator controllability holds}}$ for this reduced three-level system, despite the absence of a simple excitation-sector obstruction within the sector.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
