<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

**(1) True.** Over $\mathbb C$, $A$ has an [eigenvalue](../../../../../eigenvalue.md) $\lambda$ with nonzero [eigenspace](../../../../../eigenspace.md) $E$. Commutativity makes $E$ invariant under $B$: $A(Bv)=B(Av)=\lambda Bv$. The [endomorphism](../../../../../endomorphism.md) $B|_E$ has an [eigenvector](../../../../../eigenvector.md) $v\ne0$ because its [characteristic polynomial](../../../../../characteristic-polynomial.md) has a complex root. This $v$ is an [eigenvector](../../../../../eigenvector.md) of both matrices, though their [eigenvalues](../../../../../eigenvalue.md) on it may differ.

**(2) False.** Take $A=I$ and $B=2I$. They commute, but their only [eigenvalues](../../../../../eigenvalue.md) are respectively $1$ and $2$.

**(3) True.** Associativity gives $(BA)^{n+1}=B(AB)^nA=0$, so $T=BA$ is nilpotent. A nilpotent [endomorphism](../../../../../endomorphism.md) of an $n$-dimensional space has index at most $n$: in $V\supseteq TV\supseteq T^2V\supseteq\cdots$, equality at a nonzero image would make $T$ surjective on that finite-dimensional image, hence invertible there, contradicting nilpotence. Thus dimensions strictly decrease until zero, in at most $n$ steps. Therefore $(BA)^n=0$.

**(4) False.** Take $T=0$ on a two-dimensional [vector space](../../../../../vector-space-split.md) and $\lambda=0$. The [eigenspace](../../../../../eigenspace.md) has dimension two, but the [minimal polynomial](../../../../../minimal-polynomial.md) is $t$, in which the root zero has multiplicity one. [Eigenspace](../../../../../eigenspace.md) dimension counts independent [eigenvectors](../../../../../eigenvector.md); the exponent in the [minimal polynomial](../../../../../minimal-polynomial.md) measures the longest corresponding [Jordan chain](../../../../../jordan-chain.md), not that dimension.

**(5) True.** Factor the [minimal polynomial](../../../../../minimal-polynomial.md) as $m_T(t)=(t-\lambda)^c q(t)$, with $q(\lambda)\ne0$, and set $S=T-\lambda I$. If $v\in W_{c+1}$, then $w=S^cv$ satisfies $Sw=0$, so $q(T)w=q(\lambda)w$. But $m_T(T)v=0$ also gives $q(T)w=0$. Thus $w=0$, so $v\in W_c$. The reverse inclusion is immediate from $S^cv=0\Rightarrow S^{c+1}v=0$, proving

$$
\boxed{W_c=W_{c+1}.}
$$

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
