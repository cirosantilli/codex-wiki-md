<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Identify the [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak g$ with the tangent space $T_eG$. For $X\in\mathfrak g$, its [left-invariant vector field](../../../../../left-invariant-vector-field.md) is $X^L(g)=(dL_g)_eX$. Let $\gamma_X$ be its integral curve with $\gamma_X(0)=e$. Uniqueness of integral curves and left invariance give $\gamma_X(s+t)=\gamma_X(s)\gamma_X(t)$ wherever initially defined. Repetition of a local curve extends it to all real times. Thus $\gamma_X$ is the unique [one-parameter subgroup](../../../../../one-parameter-subgroup.md) with derivative $X$ at zero, and the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md) is defined by

$$
\boxed{\exp X=\gamma_X(1),\qquad \exp(tX)=\gamma_X(t).}
$$

Smooth dependence of solutions of differential equations on their initial data and parameters makes this map smooth.

The derivative at zero is particularly simple:

$$
(d\exp)_0(X)=\left.\frac d{dt}\right|_{t=0}\exp(tX)=X.
$$

It is the identity linear map from $\mathfrak g$ to $T_eG$. The [inverse function theorem](../../../../../inverse-function-theorem.md) therefore proves that the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md) is a [local diffeomorphism](../../../../../local-diffeomorphism.md) at zero, producing a [local exponential chart](../../../../../local-exponential-chart.md). This proves the requested local assertion.

There is a necessary qualification to the other assertion: the image of every [one-parameter subgroup](../../../../../one-parameter-subgroup.md) lies in the [identity component of a Lie group](../../../../../identity-component-of-a-lie-group.md) $G^\circ$. The correct statement without a connectedness hypothesis is

$$
\boxed{\exp:(\mathfrak g,+)\to G\text{ is a homomorphism}
\quad\Longleftrightarrow\quad G^\circ\text{ is abelian}.}
$$

Indeed, if $\exp$ is a [group homomorphism](../../../../../group-homomorphism.md), its image is an abelian subgroup. It contains an identity neighborhood by the local result. An open subgroup of a connected [group](../../../../../group-split.md) is the entire [group](../../../../../group-split.md): every coset is open, so its complement is also open. Thus $\exp(\mathfrak g)=G^\circ$, proving that this component is abelian.

Conversely, if $G^\circ$ is abelian, then $\exp(tX)\exp(tY)$ is a [one-parameter subgroup](../../../../../one-parameter-subgroup.md): its [group](../../../../../group-split.md) law follows by commuting the factors. Its derivative at zero is $X+Y$. Uniqueness gives $\exp(t(X+Y))=\exp(tX)\exp(tY)$ and, at $t=1$, additivity. This proves the [additivity of the Lie exponential map](../../../../../additivity-of-the-lie-exponential-map.md) criterion. For connected $G$ it is exactly the stated equivalence with an abelian [group](../../../../../group-split.md). For disconnected $G$ the unrestricted claim is false: $S_3\times\mathbb R$ is a nonabelian [Lie group](../../../../../lie-group.md), but its exponential is the homomorphism $x\mapsto(e,x)$. The original PDF does not impose connectedness in that sentence, so that qualification cannot be omitted.

Now suppose $G$ is connected and abelian, of dimension $n$. The exponential is a surjective [group homomorphism](../../../../../group-homomorphism.md), and its kernel $\Lambda$ is discrete by local injectivity at zero. The induced map

$$
\mathbb R^n/\Lambda\longrightarrow G
$$

is a bijective [Lie group homomorphism](../../../../../lie-group-homomorphism.md) and a local diffeomorphism, hence a [Lie group isomorphism](../../../../../lie-group-isomorphism.md). To identify the quotient, take linearly independent elements $\lambda_1,\ldots,\lambda_b\in\Lambda$ spanning the real linear span of $\Lambda$, and let $\Lambda_0=\sum_i\mathbb Z\lambda_i$. Every coset of $\Lambda_0$ in $\Lambda$ has a representative in the bounded fundamental parallelepiped of these vectors. A discrete additive subgroup has finite intersection with a compact set: otherwise differences of arbitrarily close elements would approach zero, contradicting discreteness at zero. Thus $\Lambda/\Lambda_0$ is finite.

It follows that $\Lambda$ is a finitely generated torsion-free abelian [group](../../../../../group-split.md) of rank $b$, hence has a $\mathbb Z$-basis of $b$ elements. These basis elements also span its $b$-dimensional real span and are linearly independent over $\mathbb R$. Extending them to a real basis identifies $\Lambda$ with $\mathbb Z^b\times\{0\}^{n-b}$. Consequently the [classification of connected abelian Lie groups](../../../../../classification-of-connected-abelian-lie-groups.md) is

$$
\boxed{G\cong\mathbb R^{n-b}\times(\mathbb R/\mathbb Z)^b
=\mathbb R^a\times T^b,\qquad a+b=n.}
$$

The compact circle factors record the periods of the [one-parameter subgroups](../../../../../one-parameter-subgroup.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
