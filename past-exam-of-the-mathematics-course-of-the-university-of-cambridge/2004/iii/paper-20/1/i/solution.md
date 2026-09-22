<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $X\in\mathfrak g=T_eG$, let $X^L$ be the [left-invariant vector field](../../../../../../left-invariant-vector-field.md) with value $X$ at the identity. Its integral curve through the identity is the unique [one-parameter subgroup](../../../../../../one-parameter-subgroup.md) $\gamma_X$ with $\gamma_X'(0)=X$. It exists for all real time: local existence followed by translation and the identity $\gamma_X(t+s)=\gamma_X(t)\gamma_X(s)$ extends it indefinitely. The [Exponential map of a Lie group](../../../../../../exponential-map-of-a-lie-group.md) is

$$
\boxed{\exp X=\gamma_X(1),\qquad \exp(tX)=\gamma_X(t).}
$$

It is smooth and $d_0\exp=\operatorname{id}_{\mathfrak g}$, because differentiating $t\mapsto\exp(tX)$ at zero gives $X$. The [inverse function theorem](../../../../../../inverse-function-theorem.md) therefore makes it a local [diffeomorphism](../../../../../../diffeomorphism.md) at zero.

If $G$ is abelian, the product $t\mapsto\exp(tX)\exp(tY)$ is a [one-parameter subgroup](../../../../../../one-parameter-subgroup.md) with initial tangent $X+Y$. Uniqueness gives $\exp(t(X+Y))=\exp(tX)\exp(tY)$, hence

$$
\boxed{\exp(X+Y)=\exp X\exp Y.}
$$

Conversely, if this additive [homomorphism](../../../../../../homomorphism.md) identity holds, all $\exp(tX)$ and $\exp(sY)$ commute. Differentiating their adjoint action shows $[X,Y]=0$. Alternatively, their commuting images contain an identity neighbourhood; that neighbourhood generates the [identity component of a Lie group](../../../../../../identity-component-of-a-lie-group.md), so the [identity component](../../../../../../identity-component.md) is abelian. Conversely, if the [Lie algebra](../../../../../../lie-algebra-split.md) is abelian, its [left-invariant vector fields](../../../../../../left-invariant-vector-field.md) commute, so their flows commute. Hence all [one-parameter subgroups](../../../../../../one-parameter-subgroup.md) commute; their product with initial tangent $X+Y$ is the [one-parameter subgroup](../../../../../../one-parameter-subgroup.md) for $X+Y$. The [Lie exponential map](../../../../../../exponential-map-of-a-lie-group.md) is therefore additive, and its image generates an abelian identity component. Thus **the stated equivalence holds for connected $G$**. Without connectedness the exact assertion is that the [Lie exponential map](../../../../../../exponential-map-of-a-lie-group.md) is a [homomorphism](../../../../../../homomorphism.md) precisely when $G^\circ$ is abelian. The converse implication to all of $G$ is false: in $O(2)$ the [Lie algebra](../../../../../../lie-algebra-split.md) consists of $tJ$, where

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
\exp(tJ)=R_t.
$$

Rotations satisfy $R_{t+s}=R_tR_s$, but a reflection $S$ satisfies $SR_tS^{-1}=R_{-t}$, so the full [orthogonal group](../../../../../../orthogonal-group.md) is not abelian.

Now take a connected [abelian Lie group](../../../../../../abelian-lie-group.md) of dimension $n$. Its [Lie exponential map](../../../../../../exponential-map-of-a-lie-group.md) is a [homomorphism](../../../../../../homomorphism.md) whose image contains an identity neighbourhood, hence an open [subgroup](../../../../../../subgroup.md). A connected [group](../../../../../../group-split.md) has no proper open [subgroup](../../../../../../subgroup.md), so this map is onto. Its kernel $\Lambda$ is discrete, since it is injective on a neighbourhood of zero. The induced map is a bijective [local diffeomorphism](../../../../../../local-diffeomorphism.md) and therefore a [Lie group isomorphism](../../../../../../lie-group-isomorphism.md)

$$
G\cong\mathbb R^n/\Lambda.
$$

Here is the needed classification of $\Lambda$. Let $r$ be the dimension of its real span. Choose $\lambda_1,\ldots,\lambda_r\in\Lambda$ that form a real basis of that span. Their [integer](../../../../../../integer.md) span $\Lambda_0$ has finite index in $\Lambda$: subtract [integer](../../../../../../integer.md) multiples of the $\lambda_i$ to put each [coset](../../../../../../coset.md) representative in a compact parallelepiped. Only finitely many points of $\Lambda$ lie there, since discreteness at zero gives a uniform positive separation between distinct points. Thus $\Lambda$ is finitely generated and torsion-free, and the [structure theorem for finitely generated abelian groups](../../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md) makes it free abelian of rank $r$. Its [integer](../../../../../../integer.md) basis is a real basis of the span. A linear change of coordinates consequently sends $\Lambda$ to $\mathbb Z^r\times\{0\}$ in $\mathbb R^n$.

This proves the [classification of connected abelian Lie groups](../../../../../../classification-of-connected-abelian-lie-groups.md):

$$
\boxed{G\cong(\mathbb R/\mathbb Z)^r\times\mathbb R^{n-r}
=\mathbb T^r\times\mathbb R^s,\qquad r+s=n.}
$$

The isomorphism depends on the choice of lattice basis and complementary [vector space](../../../../../../vector-space-split.md). Compactness is equivalent to $s=0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
