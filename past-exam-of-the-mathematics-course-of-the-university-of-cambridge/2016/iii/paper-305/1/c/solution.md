<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the color matrix intact: $\mathcal A_\mu=A^a_\mu T^a$. Under [parity](../../../../../../parity.md), invariance of its contraction with the [vector current](../../../../../../vector-current.md) requires

$$
\boxed{\mathcal A_\mu(x)\stackrel P\longmapsto\Lambda_\mu{}^\nu\mathcal A_\nu(x_P).}
$$

Under [charge conjugation](../../../../../../charge-conjugation.md), the fermionic reordering in part (b) transposes the color matrix as well as the spinor matrix. For a fixed color matrix $M$, $\bar\psi M\gamma^\mu\psi$ becomes $-\bar\psi M^T\gamma^\mu\psi$. Hence invariance of the interaction requires

$$
\boxed{\mathcal A_\mu(x)\stackrel C\longmapsto-\mathcal A_\mu(x)^T.}
$$

This is not a rule that changes the sign of every individual color component: transposition also acts on the generators of the [fundamental representation](../../../../../../fundamental-representation.md).

Write the [gauge field strength](../../../../../../gauge-field-strength.md) as $\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu+ig[\mathcal A_\mu,\mathcal A_\nu]$. Since $[A^T,B^T]=-[A,B]^T$, the [charge conjugation](../../../../../../charge-conjugation.md) rule gives $\mathcal F_{\mu\nu}\mapsto-\mathcal F_{\mu\nu}^T$. Including the coordinate reflection in [CP symmetry](../../../../../../cp-symmetry.md),

$$
\boxed{\mathcal F_{\mu\nu}(x)\stackrel{CP}\longmapsto
-\Lambda_\mu{}^\alpha\Lambda_\nu{}^\beta\mathcal F_{\alpha\beta}(x_P)^T.}
$$

For generators normalized by $\operatorname{Tr}(T^aT^b)=\kappa\delta^{ab}$, the color contraction equals $\kappa^{-1}\operatorname{Tr}(\mathcal F_{\mu\nu}\mathcal F_{\rho\sigma})$. The two charge-conjugation minus signs cancel, and transposition reverses the order inside the trace without changing it. The [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) acquires $\det\Lambda=-1$ under the remaining reflection. Thus

$$
\boxed{\mathcal L_\theta(x)\stackrel{CP}\longmapsto-\mathcal L_\theta(x_P).}
$$

**The [Yang-Mills theta term](../../../../../../yang-mills-theta-term.md) is CP-odd; a generic fixed nonzero $\theta$ produces [CP violation](../../../../../../cp-violation.md).** Setting $\theta=0$ removes this source. Although the density is a total derivative, it can affect the quantum theory through nontrivial topological sectors; the local transformation test is not rendered irrelevant by that fact.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
