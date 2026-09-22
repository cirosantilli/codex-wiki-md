<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

It is enough to assume that $h_k:\pi_k(X)\otimes\mathbb Q\to H_k(X;\mathbb Q)$ is surjective for every $k\ge2$; an integrally surjective [Hurewicz homomorphism](../../../../../hurewicz-homomorphism.md) certainly has this property. First give the minimal-model argument suggested by the hint. Let $A=(\Lambda V,d)$ be a [simply connected](../../../../../simply-connected-space.md) [Sullivan minimal model](../../../../../sullivan-minimal-model.md), with $V$ in degrees at least two. Put $A^+=\bigoplus_{k>0}A^k$. Its [indecomposable quotient of an augmented algebra](../../../../../indecomposable-quotient-of-an-augmented-algebra.md) is

$$
A^+/(A^+)^2\cong V.
$$

Minimality makes the induced differential on $V$ zero, so projection is a [chain map](../../../../../chain-map.md) $q:A^+\to(V,0)$. The Sullivan model identification says that the induced map

$$
q_*:\widetilde H^*(X;\mathbb Q)\longrightarrow V
$$

is dual to rational [Hurewicz homomorphism](../../../../../hurewicz-homomorphism.md). Under the usual finite-type duality convention, the assumed surjectivity makes $q_*$ injective.

A product of two positive [cohomology classes](../../../../../cohomology-class.md) has a decomposable cocycle representative, so its image under $q_*$ is zero. Injectivity therefore gives

$$
\boxed{\widetilde H^{>0}(X;\mathbb Q)\cdot
\widetilde H^{>0}(X;\mathbb Q)=0.}
$$

This deduction uses the hypothesis; zero [cup products](../../../../../cup-product.md) by themselves would not yet prove [formality of a topological space](../../../../../formal-space.md).

Choose a homogeneous [cohomology](../../../../../cohomology-split.md) [basis](../../../../../basis.md) $h_\lambda$ and cocycle representatives $z_\lambda\in A$. Their indecomposable parts $q(z_\lambda)$ are linearly independent. Extend them to a graded [basis](../../../../../basis.md) of $V$ and replace the corresponding generators by the actual cocycles $z_\lambda$. This is a valid change of free algebra generators: each $z_\lambda$ differs from its indecomposable part by products of generators of strictly smaller degree, so degree induction constructs the inverse substitution. Call these closed generators $C$, and the remaining generators $N$.

Define a map of graded algebras

$$
\phi:A\longrightarrow H^*(X;\mathbb Q),
\qquad z_\lambda\longmapsto h_\lambda,\quad N\longmapsto0.
$$

Its target has zero differential. Every differential in $A$ is decomposable, and all products of positive target classes vanish, so $\phi$ is a [chain map](../../../../../chain-map.md). If $z$ is any positive cocycle, its indecomposable part is in the span of the $q(z_\lambda)$, because these form the image of $q_*$. Write $q(z)=\sum_\lambda c_\lambda q(z_\lambda)$. Then $\phi(z)=\sum_\lambda c_\lambda h_\lambda$, while injectivity of $q_*$ gives $[z]=\sum_\lambda c_\lambda h_\lambda$. Thus $\phi$ induces the identity on [cohomology](../../../../../cohomology-split.md) and is a [quasi-isomorphism](../../../../../quasi-isomorphism.md). This proves that $X$ is a [formal space](../../../../../formal-space.md).

The rational [wedge sum](../../../../../wedge-sum.md) assertion has a direct topological proof, which also avoids finite-dimensional duality restrictions in the preceding model argument. Choose a homogeneous [basis](../../../../../basis.md) $b_\lambda$ of $\widetilde H_*(X;\mathbb Q)$. By surjectivity, each [basis](../../../../../basis.md) class is the image under the [Hurewicz homomorphism](../../../../../hurewicz-homomorphism.md) of an element of $\pi_{n_\lambda}(X)\otimes\mathbb Q$. In $X_{\mathbb Q}$ this element is represented by an actual sphere map $S^{n_\lambda}\to X_{\mathbb Q}$. Simple connectivity and $H_1=0$ ensure $n_\lambda\ge2$. The [wedge sum](../../../../../wedge-sum.md) of these maps gives

$$
F:\bigvee_\lambda S^{n_\lambda}\longrightarrow X_{\mathbb Q}
$$

and induces an isomorphism of [rational homology](../../../../../rational-homology.md) by the choice of [basis](../../../../../basis.md). The [rational Whitehead theorem](../../../../../rational-whitehead-theorem.md) now makes it a [rational homotopy equivalence](../../../../../rational-homotopy-equivalence.md), giving

$$
\boxed{X\simeq_{\mathbb Q}\bigvee_\lambda S^{n_\lambda}.}
$$

A [wedge sum](../../../../../wedge-sum.md) of spheres is a [formal space](../../../../../formal-space.md). For each individual sphere, its augmented [minimal model](../../../../../sullivan-minimal-model.md) maps by a [quasi-isomorphism](../../../../../quasi-isomorphism.md) to its sphere cochain algebra, and also to its [cohomology](../../../../../cohomology-split.md) algebra, by killing the extra odd generator in the even-sphere case. Take based simplicial models of the spheres. Their [wedge sum](../../../../../wedge-sum.md) is a simplicial pushout over the common basepoint, so the algebra of [rational polynomial differential forms](../../../../../rational-polynomial-differential-forms.md) is the corresponding fibre product of augmented sphere algebras. Taking fibre products of these model maps gives a [quasi-isomorphism](../../../../../quasi-isomorphism.md) zigzag to the square-zero [cohomology](../../../../../cohomology-split.md) algebra. This also works for infinitely many sphere summands: the positive parts are products of the individual complexes, and products of vector-space exact sequences over a [field](../../../../../field.md) are exact. In the finite case its minimal resolution is the [minimal model of a wedge of simply connected spheres](../../../../../minimal-model-of-a-wedge-of-simply-connected-spheres.md). Thus the topological proof establishes both conclusions without imposing finite rank on the sphere [basis](../../../../../basis.md). For the zero reduced-homology case the [wedge sum](../../../../../wedge-sum.md) is a point. Both the minimal-model construction and the explicit sphere map explain why the surjectivity hypothesis is decisive.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
