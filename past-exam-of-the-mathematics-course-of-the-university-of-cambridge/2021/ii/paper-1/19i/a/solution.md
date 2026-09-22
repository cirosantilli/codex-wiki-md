<h1 id="19i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A representation is completely reducible, or [semisimple](../../../../../../semisimple-representation.md), when it is a [direct sum](../../../../../../direct-sum.md) of [irreducible representation](../../../../../../irreducible-representation.md). Equivalently, every invariant subspace has an invariant complement.

[Maschke's theorem](../../../../../../maschke-s-theorem.md) says that every finite-dimensional representation of a finite group $G$ over a field of characteristic zero is completely reducible. More generally, it is enough that the field characteristic does not divide $|G|$.

[Schur lemma](../../../../../../schur-s-lemma.md) states the following.

- If $V$ and $W$ are irreducible $G$-representations, every [intertwining operator](../../../../../../intertwining-operator.md) $T:V\to W$ is either zero or an isomorphism.
- If $V$ is finite-dimensional over an algebraically closed field, every $G$-endomorphism of $V$ is a scalar multiple of the identity.

Indeed, $\ker T\subseteq V$ and $\operatorname{im}T\subseteq W$ are invariant subspaces. If $T\ne0$, irreducibility forces

$$
\ker T=0,
\qquad
\operatorname{im}T=W,
$$

so $T$ is an isomorphism. For an endomorphism of a finite-dimensional complex representation, choose an [eigenvalue](../../../../../../eigenvalue.md) $\lambda$ of $T$. The intertwiner $T-\lambda I$ has nonzero kernel, so the first part forces

$$
T-\lambda I=0.
$$

This proves the [Proof of Schur lemma](../../../../../../proof-of-schur-lemma.md).

Now let $\rho:G\to\operatorname{GL}(V)$ be faithful and irreducible over $\mathbb C$. For every $z\in Z(G)$, the operator $\rho(z)$ commutes with every $\rho(g)$. Schur's lemma therefore gives

$$
\rho(z)=\lambda_zI
$$

for some $\lambda_z\in\mathbb C^\times$. Faithfulness makes $z\mapsto\lambda_z$ an embedding

$$
Z(G)\hookrightarrow\mathbb C^\times.
$$

Since every [finite subgroup of the multiplicative complex numbers](../../../../../../finite-subgroup-of-the-multiplicative-complex-numbers.md) is cyclic,

$$
\boxed{Z(G)\text{ is cyclic}}.
$$

This is the [cyclic-center obstruction to a faithful irreducible representation](../../../../../../cyclic-center-obstruction-to-a-faithful-irreducible-representation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19I](../../19i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
