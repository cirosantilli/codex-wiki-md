<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [endomorphisms](../../../../../endomorphism.md) of the [finite-dimensional vector space](../../../../../finite-dimensional-vector-space.md) $V$ over the [complex numbers](../../../../../complex-number.md) form the [general linear Lie algebra](../../../../../general-linear-lie-algebra.md) $L=\operatorname{End}_{\mathbb C}(V)$ with the usual addition and scalar multiplication and [Lie bracket](../../../../../lie-bracket.md) $[x,y]=xy-yx$. This [commutator](../../../../../commutator.md) is bilinear and antisymmetric, and expanding the six products verifies the [Jacobi identity](../../../../../jacobi-identity.md).

For a [Lie subalgebra](../../../../../lie-subalgebra.md) $\mathfrak g=L_1$, being an [abelian Lie algebra](../../../../../abelian-lie-algebra.md) means $[\mathfrak g,\mathfrak g]=0$. A [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) has $\gamma_1=\mathfrak g$, $\gamma_{j+1}=[\mathfrak g,\gamma_j]$ eventually zero; a [solvable Lie algebra](../../../../../solvable-lie-algebra.md) has $\mathfrak g^{(0)}=\mathfrak g$, $\mathfrak g^{(j+1)}=[\mathfrak g^{(j)},\mathfrak g^{(j)}]$ eventually zero. These are the [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) and [derived series of a Lie algebra](../../../../../derived-series-of-a-lie-algebra.md), respectively. Nilpotence is a condition on the [Lie bracket](../../../../../lie-bracket.md), and does not require every member to be a [nilpotent endomorphism](../../../../../nilpotent-linear-map.md): a nonzero scalar multiple of the identity spans an [abelian Lie algebra](../../../../../abelian-lie-algebra.md).

A [flag of a vector space](../../../../../flag-linear-algebra.md) is an increasing chain of [vector subspaces](../../../../../vector-subspace.md). The flag we construct is a [complete flag](../../../../../complete-flag.md), $0=V_0\subset V_1\subset\cdots\subset V_d=V$, where $\dim V_i=i$, and each $V_i$ is an [invariant subspace](../../../../../invariant-subspace.md) for $\mathfrak g$. We first prove the common-[eigenvector](../../../../../eigenvector.md) assertion in the [Lie theorem](../../../../../lie-s-theorem.md), by induction on $\dim\mathfrak g$; the zero algebra is immediate. For nonzero solvable $\mathfrak g$, its [derived algebra](../../../../../derived-algebra.md) is proper, so there is a codimension-one [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md) $\mathfrak k$ containing $[\mathfrak g,\mathfrak g]$. Write $\mathfrak g=\mathfrak k\oplus\mathbb Cx$. By induction there are $v\ne0$ and a [linear functional](../../../../../linear-functional.md) $\lambda$ on $\mathfrak k$ such that $kv=\lambda(k)v$ for every $k\in\mathfrak k$.

Let $W$ be the [cyclic subspace](../../../../../cyclic-subspace.md) spanned by $v,xv,x^2v,\ldots$. The [commutator derivation identity](../../../../../commutator-derivation-identity.md) and $[\mathfrak k,x]\subseteq\mathfrak k$ show inductively that

$$
kx^jv\equiv\lambda(k)x^jv\pmod{\operatorname{span}\{v,xv,\ldots,x^{j-1}v\}}.
$$

Thus $W$ and all its initial cyclic spans are $\mathfrak k$-invariant. If $m=\dim W$, the first $m$ cyclic vectors form a [basis](../../../../../basis.md), $W$ is also $x$-invariant, and $\operatorname{tr}_W k=m\lambda(k)$. For $k\in\mathfrak k$, the [trace of a matrix commutator](../../../../../trace-of-a-matrix-commutator.md) gives

$$
0=\operatorname{tr}_W[k,x]=m\lambda([k,x]).
$$

Hence $\lambda([k,x])=0$, since the field has [characteristic zero](../../../../../characteristic-zero.md). The nonzero common [weight space](../../../../../weight-space.md)

$$
V_\lambda=\{w\in V:kw=\lambda(k)w\text{ for all }k\in\mathfrak k\}
$$

is $x$-invariant: $k(xw)=x(kw)+[k,x]w=\lambda(k)xw$. The restriction of $x$ to $V_\lambda$ has an [eigenvector](../../../../../eigenvector.md), because $\mathbb C$ is an [algebraically closed field](../../../../../algebraically-closed-field.md). This is a common [eigenvector](../../../../../eigenvector.md) for $\mathfrak g$. Its line is invariant, and repeating the argument on the [quotient vector space](../../../../../quotient-vector-space.md) gives the complete invariant flag. Equivalently, this proves [simultaneous triangularization of a Lie algebra representation](../../../../../simultaneous-triangularization-of-a-lie-algebra-representation.md).

In a [basis](../../../../../basis.md) adapted to this [complete flag](../../../../../complete-flag.md), every member of $\mathfrak g$ is upper triangular, so every member of its [derived algebra](../../../../../derived-algebra.md) is strictly upper triangular. Products of $d$ [strictly upper triangular matrices](../../../../../strictly-upper-triangular-matrix.md) vanish, and each iterated [Lie bracket](../../../../../lie-bracket.md) of $d$ such matrices is a sum of these products. Consequently the [derived algebra](../../../../../derived-algebra.md) is a [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md). We may therefore take **$L_2=[L_1,L_1]$**: it is an ideal, and the [quotient Lie algebra](../../../../../quotient-lie-algebra.md) $L_1/L_2$ is abelian. This also covers $\dim V=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
