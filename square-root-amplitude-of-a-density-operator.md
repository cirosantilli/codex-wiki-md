# Square-root amplitude of a density operator

↑ **Parent:** [Purification of a density operator](purification-of-a-density-operator.md)

The unique positive square root of a [density operator](density-matrix-split.md) is a Hilbert-Schmidt operator $W$ with $\|W\|_{\mathrm{HS}}^2=\operatorname{tr}\rho=1$. It reproduces expectations by $\operatorname{tr}(A\rho)=\operatorname{tr}(W^*AW)$. In chosen orthonormal bases, vectorizing its entries gives a normalized bipartite vector $|W\rangle\!\rangle=\sum_{r,s}W_{rs}|r\rangle|s\rangle$ whose reduced [density operator](density-matrix-split.md) is $WW^*=\rho$. Thus the positive operator amplitude and the vector [purification](purification-of-a-density-operator.md) are related but distinct objects.

More generally a coefficient matrix $C$ purifies $\rho$ when $CC^*=\rho$. For square nonsingular $C$, the matrix $U=C^{-1}\sqrt\rho$ obeys $UU^*=I$ and is unitary, so $\sqrt\rho=CU$. In an eigenbasis of $\rho$, $C=\operatorname{diag}(\sqrt{p_r})U^*$; its conjugated unitary columns give the second-factor [Schmidt decomposition](schmidt-decomposition.md) vectors. This is the matrix form of [unitary freedom of purification](unitary-freedom-of-purification.md).

## ↑ Ancestors (6)

1. [Purification of a density operator](purification-of-a-density-operator.md)
2. [Density matrix](density-matrix-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
