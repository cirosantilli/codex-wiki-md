<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

It is essential to distinguish a finite-dimensional spinor matrix from its action on a family of operator components. Take the [Pauli matrices](../../../../../../pauli-matrices.md) and $\bar\sigma^{\mu\nu}$ in the supplied convention, with $\eta=\operatorname{diag}(1,-1,-1,-1)$. They give

$$
\bar\sigma^{ij}=\frac12\epsilon_{ijk}\sigma_k,
\qquad\bar\sigma^{0i}=\frac i2\sigma_i.
$$

If both displayed transformations are read literally as left multiplication on the column $\bar Q^{\dot\alpha}$, expanding the operator conjugation and comparing its linear term gives the formal answer $[M^{\mu\nu},\bar Q]=+\bar\sigma^{\mu\nu}\bar Q$.

There is a sign inconsistency in that literal reading. With the usual [angular momentum commutation relations](../../../../../../angular-momentum-commutation-relations.md), coefficient matrices $R_i$ in $[J_i,q_a]=(R_i)_{ab}q_b$ must satisfy

$$
[R_i,R_j]=-i\epsilon_{ijk}R_k.
$$

Indeed, the [Jacobi identity](../../../../../../jacobi-identity.md) gives $[J_i,[J_j,q]]-[J_j,[J_i,q]]=(R_jR_i-R_iR_j)q$, whereas $[[J_i,J_j],q]=i\epsilon_{ijk}R_kq$. The formal $R_i=+\sigma_i/2$ violates this identity. For example it would give $[J_3,q_1]=q_1/2$, $[J_+,q_1]=q_2$ and $[J_3,q_2]=-q_2/2$; the two sides of the [Jacobi identity](../../../../../../jacobi-identity.md) for $J_3,J_+,q_1$ are then $-q_2/2$ and $3q_2/2$.

A consistent canonical column-operator convention uses the inverse adjoint action for the displayed spinor transformation, equivalently the contragredient operator-component prescription. It gives

$$
\boxed{[M^{\mu\nu},\bar Q^{\dot\alpha}]
=-(\bar\sigma^{\mu\nu})^{\dot\alpha}{}_{\dot\beta}\bar Q^{\dot\beta}.}
$$

This is the convention used for the physical states below. Reversing the adjoint action is the minimum needed sign correction in the literal column reading; a dual row notation can encode the same correction by its index contractions. The formal printed-sign coefficients are also recorded below, so the distinction is explicit rather than silently changing a convention. The representation matrices themselves remain $J_i=\sigma_i/2$ and $K_i=i\sigma_i/2$ in Question 3: the minus sign here concerns [commutators](../../../../../../commutator.md) of operator components.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
