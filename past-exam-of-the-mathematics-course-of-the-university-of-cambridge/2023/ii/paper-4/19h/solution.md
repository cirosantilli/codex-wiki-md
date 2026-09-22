<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

[Schur lemma](../../../../../schur-s-lemma.md) says that an intertwining linear map between irreducible finite-dimensional complex representations is either zero or an isomorphism. In particular, every endomorphism of an irreducible complex representation is a scalar multiple of the identity.

A [continuous representation of a topological group](../../../../../continuous-representation-of-a-topological-group.md) is a continuous homomorphism

$$
\rho:G\longrightarrow\operatorname{GL}(V)
$$

for a finite-dimensional complex [vector space](../../../../../vector-space-split.md) $V$. It is a [unitary representation](../../../../../unitary-representation.md) if $V$ has a positive-definite Hermitian [inner product](../../../../../inner-product.md) for which

$$
\langle\rho(g)v,\rho(g)w\rangle
=\langle v,w\rangle
$$

for every $g\in G$ and $v,w\in V$.

For $G=S^1$, start with any positive-definite Hermitian form and average it using normalized [Haar measure](../../../../../haar-measure.md):

$$
\langle v,w\rangle_{S^1}
=\int_{S^1}
 \langle\rho(z)v,\rho(z)w\rangle\,dz.
$$

Translation invariance makes this form $S^1$-invariant, and positivity is preserved, proving [unitarity](../../../../../unitarization-of-a-compact-group-representation.md). Since $S^1$ is abelian, the operators $\rho(z)$ commute; since they are unitary, they are [normal](../../../../../normal-matrix.md). [Simultaneous diagonalization](../../../../../simultaneous-diagonalization.md) therefore decomposes $V$ into common one-dimensional eigenspaces. Thus every [representation of the circle group](../../../../../representation-of-the-circle-group.md) is a direct sum of one-dimensional representations.

Write

$$
g(x,y,z)=
\begin{pmatrix}
1&x&z\\0&1&y\\0&0&1
\end{pmatrix}.
$$

The group law and inverse are

$$
\begin{aligned}
g(x,y,z)g(x',y',z')
 &=g(x+x',y+y',z+z'+xy'),\\
g(x,y,z)^{-1}
 &=g(-x,-y,-z+xy).
\end{aligned}
$$

A calculation gives

$$
g(x,y,z)^{-1}g(x',y',z')^{-1}g(x,y,z)g(x',y',z')
=g(0,0,xy'-x'y).
$$

Every element of the [centre](../../../../../center-of-a-group.md) $Z$ occurs by taking, for example, $x'=y=0$ and $y'=1$. Hence the [commutator subgroup](../../../../../commutator-subgroup.md) is exactly $Z$. The image of a one-dimensional representation is abelian, so the [one-dimensional representation kills the commutator subgroup](../../../../../one-dimensional-representation-kills-the-commutator-subgroup.md) and its kernel contains $Z$.

Now let $(\rho,V)$ be a complex representation of $G/Z_0$. Its restriction to the central subgroup

$$
Z/Z_0\cong\mathbb R/\mathbb Z\cong S^1
$$

is a representation of the circle group. Decompose it into its distinct weight spaces:

$$
V=V_1\oplus\cdots\oplus V_d,
\qquad
\rho(z)|_{V_i}=\theta_i(z)\operatorname{id}_{V_i}.
$$

Because $Z/Z_0$ is central, every $\rho(g)$ commutes with its action and preserves every common eigenspace. Thus the $V_i$ are $G/Z_0$-subrepresentations, as asserted by the [central circle weight-space decomposition](../../../../../central-circle-weight-space-decomposition.md).

Let $n_i=\dim V_i$. The map

$$
g\longmapsto\det(\rho(g)|_{V_i})
$$

is a one-dimensional representation of $G/Z_0$; after composition with $G\to G/Z_0$, its kernel contains $Z$. On $z\in Z/Z_0$ its value is

$$
\det(\theta_i(z)I_{n_i})=\theta_i(z)^{n_i},
$$

so $\theta_i^{n_i}=1$. A continuous character of $S^1$ has the form $z\mapsto z^m$; the displayed identity forces $m=0$. Therefore every $\theta_i$ is trivial. Since the $\theta_i$ were distinct, $d=1$ and $\theta_1=1$.

It follows that every finite-dimensional complex representation of $G/Z_0$ kills the entire nontrivial central circle $Z/Z_0$. Its kernel is therefore nontrivial, so no such representation is [faithful](../../../../../faithful-representation.md). This is the [real Heisenberg quotient has no faithful finite-dimensional representation](../../../../../real-heisenberg-quotient-has-no-faithful-finite-dimensional-representation.md).

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
