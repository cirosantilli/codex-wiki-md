<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

[Maschke's theorem](../../../../../maschke-s-theorem.md) says that if $H$ is a [finite group](../../../../../finite-group.md) and the [characteristic of a field](../../../../../characteristic-of-a-field.md) $F$ does not divide $|H|$, then every finite-dimensional $F$-representation of $H$ is [semisimple](../../../../../semisimple-representation.md).

To prove it, let $W$ be an [invariant subspace](../../../../../invariant-subspace.md) of a representation $V$, and choose any linear projection $P:V\to W$. Average its conjugates:

$$
\overline P=\frac1{|H|}\sum_{h\in H}\rho(h)P\rho(h)^{-1}.
$$

The scalar $|H|^{-1}$ exists by the characteristic assumption. Reindexing the sum shows that $\overline P$ commutes with every $\rho(g)$. Since each summand restricts to the identity on $W$, so does $\overline P$; hence $\overline P$ is an equivariant projection onto $W$. Its kernel is an invariant complement, and induction on $\dim V$ decomposes $V$ into [irreducible representations](../../../../../irreducible-representation.md).

The isometry group of $\mathbb Z$ is the [infinite dihedral group](../../../../../infinite-dihedral-group.md)

$$
G=\langle t,s\mid s^2=1,\ sts=t^{-1}\rangle.
$$

Let $\rho$ be a nonfaithful finite-dimensional complex representation. Its nontrivial normal kernel contains $t^m$ for some $m>0$, by the stated hint, so $\rho$ factors through the finite quotient

$$
\langle t,s\mid t^m=s^2=1,\ sts=t^{-1}\rangle.
$$

Maschke's theorem decomposes this quotient representation into irreducibles. To bound their dimensions, choose a $t$-eigenvector $v$ with eigenvalue $\lambda$ in an irreducible constituent. The relation gives

$$
t(sv)=st^{-1}v=\lambda^{-1}sv,
$$

so $\operatorname{span}\{v,sv\}$ is invariant under both generators. Irreducibility makes it the whole constituent, whose dimension is therefore at most two. This proves the result on [nonfaithful representations of the infinite dihedral group](../../../../../nonfaithful-representations-of-the-infinite-dihedral-group.md).

For the requested representation of $(\mathbb Z,+)$, let its generator act on the polynomials of degree at most one by translation:

$$
(Tp)(x)=p(x+1).
$$

In the basis $(1,x)$,

$$
T=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
$$

This is a nontrivial [Jordan block](../../../../../jordan-block.md), so it is not diagonalizable. A direct sum of one-dimensional subrepresentations would make $T$ diagonalizable, proving that this [nonsemisimple translation representation of the infinite cyclic group](../../../../../nonsemisimple-translation-representation-of-the-infinite-cyclic-group.md) has the required property.

Finally, on $V=\mathbb C[x]_{\le2}$ define

$$
(Tp)(x)=p(x+1),
\qquad
(Sp)(x)=p(-x).
$$

Then $S^2=I$ and $STS=T^{-1}$, so these operators define a [quadratic-polynomial representation of the infinite dihedral group](../../../../../quadratic-polynomial-representation-of-the-infinite-dihedral-group.md). In the basis $(1,x,x^2)$ they are

$$
T=
\begin{pmatrix}
1&1&1\\
0&1&2\\
0&0&1
\end{pmatrix},
\qquad
S=
\begin{pmatrix}
1&0&0\\
0&-1&0\\
0&0&1
\end{pmatrix}.
$$

Here $(T-I)^2\ne0$ but $(T-I)^3=0$, so $T$ consists of one size-three [Jordan block](../../../../../jordan-block.md). If $V$ were a direct sum of subrepresentations of dimensions at most two, then $T$ would be block diagonal with Jordan blocks of sizes at most two, a contradiction. Thus this representation has the required failure of decomposition.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
