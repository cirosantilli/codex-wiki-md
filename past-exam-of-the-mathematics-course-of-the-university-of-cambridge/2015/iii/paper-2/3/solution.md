<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work over $\mathbb C$. Decompose $V$ as the [direct sum](../../../../../direct-sum.md) of the [generalized eigenspaces](../../../../../generalized-eigenspace.md) $V_\lambda$ of $X$. Define $X_s$ to be $\lambda I$ on $V_\lambda$ and set $X_n=X-X_s$. Then $X_s$ is a [diagonalisable endomorphism](../../../../../diagonalizable-matrix.md), $X_n$ is a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md), and they commute. For uniqueness, any commuting decomposition $X=S+N$ has $S$ and $N$ commuting with $X$, hence preserving each $V_\lambda$. Decompose $V_\lambda$ further into [eigenspaces](../../../../../eigenspace.md) of $S$. On a nonzero such space with [eigenvalue](../../../../../eigenvalue.md) $\sigma$, the operator $X=\sigma I+N$ has only the [eigenvalue](../../../../../eigenvalue.md) $\sigma$, so $\sigma=\lambda$. Since $S$ is diagonalizable, $S=\lambda I$ throughout $V_\lambda$. Thus $S=X_s$ and $N=X_n$. This is the [Additive Jordan decomposition](../../../../../jordan-chevalley-decomposition.md).

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) for the pairwise coprime polynomials $(t-\lambda)^{r_\lambda}$ also gives a polynomial $p$ with $p(t)\equiv\lambda\pmod{(t-\lambda)^{r_\lambda}}$, where $r_\lambda$ is the largest [Jordan block](../../../../../jordan-block.md) size. Consequently $X_s=p(X)$ and $X_n=X-p(X)$. This polynomial description shows that both parts preserve every $X$-invariant subspace.

On $\operatorname{Hom}(V_\lambda,V_\mu)$ the operator $\operatorname{ad}X_s$ is the scalar $\mu-\lambda$, so it is diagonalizable. The [nilpotence of commutation by a nilpotent endomorphism](../../../../../nilpotence-of-commutation-by-a-nilpotent-endomorphism.md) makes $\operatorname{ad}X_n$ nilpotent. They commute, since $[\operatorname{ad}X_s,\operatorname{ad}X_n]=\operatorname{ad}[X_s,X_n]=0$. Uniqueness of the [Additive Jordan decomposition](../../../../../jordan-chevalley-decomposition.md) therefore gives the [adjoint compatibility of additive Jordan decomposition](../../../../../adjoint-compatibility-of-additive-jordan-decomposition.md):

$$
\boxed{(\operatorname{ad}X)_s=\operatorname{ad}X_s,\qquad(\operatorname{ad}X)_n=\operatorname{ad}X_n.}
$$

Now let $\mathfrak g\subseteq\mathfrak{gl}(V)$ be a complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) and $X\in\mathfrak g$. Since the semisimple part of $\operatorname{ad}X$ is a polynomial in $\operatorname{ad}X$, it preserves $\mathfrak g$. Thus $[X_s,\mathfrak g]\subseteq\mathfrak g$. By the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md), the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) of $\mathfrak g$ on $\operatorname{End}(V)$ has a decomposition $\operatorname{End}(V)=\mathfrak g\oplus M$ into invariant subspaces. Write $X_s=y+z$ with $y\in\mathfrak g$ and $z\in M$. For $a\in\mathfrak g$, the vector $[z,a]=[X_s,a]-[y,a]$ lies in $\mathfrak g$, and invariance of $M$ puts it in $M$ as well. Hence $[z,a]=0$.

Decompose $V=\bigoplus_j U_j$ into [Irreducible Lie algebra representations](../../../../../irreducible-lie-algebra-representation.md). Each $U_j$ is preserved by $X_s=p(X)$ and by $y$, hence by $z$. The [Schur lemma](../../../../../schur-s-lemma.md) makes $z|_{U_j}=c_jI$. A [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is a [perfect Lie algebra](../../../../../perfect-lie-algebra.md), so every representing element of $\mathfrak g$ has zero [trace](../../../../../matrix-trace.md) on every $U_j$. Also $\operatorname{tr}(X_s|_{U_j})=\operatorname{tr}(X|_{U_j})$, because $X_n$ is nilpotent there. It follows that $c_j\dim U_j=\operatorname{tr}(z|_{U_j})=0$. In [characteristic zero](../../../../../characteristic-zero.md), $c_j=0$, so $z=0$. Therefore $X_s\in\mathfrak g$ and $X_n=X-X_s\in\mathfrak g$. This proves that [semisimple matrix Lie algebras are closed under additive Jordan decomposition](../../../../../semisimple-matrix-lie-algebras-are-closed-under-additive-jordan-decomposition.md), including representations with repeated isomorphic irreducible summands.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
