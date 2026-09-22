<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Represent spin by $J_i=(\hbar/2)\sigma_i$ in the basis $|\uparrow\rangle,|\downarrow\rangle$. The [Pauli matrices](../../../../../pauli-matrices.md) are Hermitian and satisfy $[\sigma_i,\sigma_j]=2i\epsilon_{ijk}\sigma_k$, giving the general [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) $[J_i,J_j]=i\hbar\epsilon_{ijk}J_k$. The particular representation has $J^2=3\hbar^2I/4$ and $J_3$ eigenvalues $\pm\hbar/2$, the features specific to [spin one-half](../../../../../spin-one-half.md).

In the stated order of two-particle basis vectors, the operator is

$$
\boxed{\sigma^{(A)}\cdot\sigma^{(B)}=\begin{pmatrix}1&0&0&0\\0&-1&2&0\\0&2&-1&0\\0&0&0&1\end{pmatrix}.}
$$

Its eigenvalue-one vectors are $|\uparrow\uparrow\rangle$, $|\downarrow\downarrow\rangle$ and $(|\downarrow\uparrow\rangle+|\uparrow\downarrow\rangle)/\sqrt2$, all symmetric under interchange. The eigenvalue-minus-three vector is $(|\downarrow\uparrow\rangle-|\uparrow\downarrow\rangle)/\sqrt2$, antisymmetric under interchange. These are the [triplet state](../../../../../spin-one-half-triplet-state.md) and [singlet state](../../../../../singlet-state.md), respectively.

Identical spin-half particles are [fermions](../../../../../fermion.md). With no other degrees of freedom to carry antisymmetry, **only the singlet is allowed**. Indeed, for total angular momentum $J=(\hbar/2)(\sigma^{(A)}+\sigma^{(B)})$,

$$
J^2=\frac{\hbar^2}4\left(6I+2\sigma^{(A)}\cdot\sigma^{(B)}\right).
$$

This gives $2\hbar^2$ on the triplet and zero on the singlet, corresponding to total spin one and zero, as required by [addition of angular momentum](../../../../../addition-of-angular-momentum.md).

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
