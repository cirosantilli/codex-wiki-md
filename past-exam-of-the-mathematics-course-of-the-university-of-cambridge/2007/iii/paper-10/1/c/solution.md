<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A strongly continuous [unitary representation](../../../../../../unitary-representation.md) of the [circle group](../../../../../../circle-group.md) decomposes as $H=\widehat\bigoplus_{m\in\mathbb Z}H_m$, with $U_z\xi=z^m\xi$ on $H_m$. Its [positive energy unitary representation of the circle](../../../../../../positive-energy-unitary-representation-of-the-circle.md) condition is that the occurring integers are bounded below. Equivalently $U_{e^{it}}=e^{itL}$ with a [self-adjoint](../../../../../../self-adjoint-operator.md) generator bounded below. An integer character can shift the lowest weight to zero.

Let $M=S''$. Because $S=S^*$, this is a [Von Neumann algebra](../../../../../../von-neumann-algebra.md), and rotation invariance makes $U_zM'U_z^*=M'$. Joint irreducibility implies $M'\cap\{U_z\}'=\mathbb CI$: a nonscalar [self-adjoint](../../../../../../self-adjoint-operator.md) element of that joint [commutant](../../../../../../centralizer.md) would have a nontrivial invariant [spectral projection gives a reducing subspace](../../../../../../spectral-projection-gives-a-reducing-subspace.md).

For $T\in M'$, take its strong [Fourier coefficients](../../../../../../fourier-coefficient.md) $T_k=\int_{\mathbb T}z^{-k}U_zTU_z^*\,dz$. They lie in $M'$ and satisfy $U_zT_kU_z^*=z^kT_k$. Both $T_k^*T_k$ and $T_kT_k^*$ are rotation-invariant elements of $M'$, hence scalar. If $T_k\ne0$, both scalars equal $\|T_k\|^2$, so $T_k/\|T_k\|$ is a unitary. It shifts energy by $k$. For $k\ne0$, applying it or its adjoint to a nonzero lowest-energy [vector](../../../../../../vector.md) produces a [vector](../../../../../../vector.md) below the lowest energy, a contradiction. Thus $T_k=0$ for every $k\ne0$, while $T_0$ is scalar.

[Fejér sum](../../../../../../fejer-sum.md) averaging of the strongly continuous orbit $U_zTU_z^*$ converges strongly to $T$. Its [Fourier coefficients](../../../../../../fourier-coefficient.md) have just shown every such average is $T_0$, so $T=T_0$ is scalar. In particular **every [bounded operator](../../../../../../continuous-linear-operator.md) commuting with $S$ commutes with every $U_z$**. In fact the hypotheses force the stronger conclusion $S'=\mathbb CI$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
