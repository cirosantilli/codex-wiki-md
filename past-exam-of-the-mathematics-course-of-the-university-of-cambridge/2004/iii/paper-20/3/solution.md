<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Lie group–Lie algebra correspondence](../../../../../lie-group-lie-algebra-correspondence.md) separates local differential structure from global topology. For a [Lie group](../../../../../lie-group.md) $G$, define $LG=T_eG$ as a [real vector space](../../../../../real-vector-space.md). Extend each $X\in T_eG$ to the [left-invariant vector field](../../../../../left-invariant-vector-field.md)

$$
X^L(g)=d_eL_g(X).
$$

The [commutator](../../../../../commutator.md) of two such [vector fields](../../../../../vector-field.md) is again left-invariant. Set

$$
\boxed{[X,Y]=[X^L,Y^L](e).}
$$

The vector-field [commutator](../../../../../commutator.md) is bilinear, antisymmetric and satisfies the [Jacobi identity](../../../../../jacobi-identity.md), so this makes $T_eG$ a [Lie algebra](../../../../../lie-algebra-split.md). For a matrix [group](../../../../../group-split.md) this bracket is $XY-YX$.

For a smooth [Lie group homomorphism](../../../../../lie-group-homomorphism.md) $\phi:G_1\to G_2$, its differential at the identity is the [linear map](../../../../../linear-map.md)

$$
L\phi=d_{e_1}\phi:\mathfrak g_1\longrightarrow\mathfrak g_2.
$$

The identity $\phi\circ L_g=L_{\phi(g)}\circ\phi$ shows that the corresponding left-invariant fields are $\phi$-related. Brackets of related [vector fields](../../../../../vector-field.md) are related, hence

$$
\boxed{L\phi([X,Y])=[L\phi(X),L\phi(Y)].}
$$

The chain rule also gives $L(\psi\circ\phi)=L\psi\circ L\phi$ and $L(\operatorname{id})=\operatorname{id}$. Thus differentiation is a functor from [Lie groups](../../../../../lie-group.md) and smooth [homomorphisms](../../../../../homomorphism.md) to real [Lie algebras](../../../../../lie-algebra-split.md) and bracket-preserving [linear maps](../../../../../linear-map.md).

To see what information the differential retains, apply $\phi$ to a [one-parameter subgroup](../../../../../one-parameter-subgroup.md). Its initial tangent is $L\phi(X)$, so uniqueness yields

$$
\boxed{\phi(\exp X)=\exp(L\phi(X)).}
$$

If $G_1$ is connected, a small exponential neighbourhood generates it. Every $g\in G_1$ is a finite product $\exp X_1\cdots\exp X_k$, and therefore

$$
\phi(g)=\exp(L\phi(X_1))\cdots\exp(L\phi(X_k)).
$$

For an already existing [homomorphism](../../../../../homomorphism.md) this expression is independent of the chosen product because it equals $\phi(g)$. Two [homomorphisms](../../../../../homomorphism.md) with the same differential agree on that neighbourhood and hence everywhere. This proves that a [Lie group homomorphism determined by its differential](../../../../../lie-group-homomorphism-determined-by-its-differential.md) requires a connected source.

On a disconnected source only the restriction to $G_1^\circ$ is determined. For instance a nontrivial finite discrete [group](../../../../../group-split.md) has zero [Lie algebra](../../../../../lie-algebra-split.md), so its identity and trivial [endomorphisms](../../../../../endomorphism.md) have the same zero differential but are different maps. The discussion of all components must therefore include additional global data. The remaining parts explain the corresponding existence and topology conditions.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
