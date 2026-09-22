<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

An [abstract smooth surface](../../../../../abstract-smooth-surface.md) is a Hausdorff second-countable topological space with an atlas of [charts](../../../../../manifold-chart.md) to open subsets of $\mathbb R^2$ whose transition maps are smooth. It is [orientable](../../../../../orientable-smooth-manifold.md) when it has such an atlas for which every transition map has positive [Jacobian determinant](../../../../../jacobian-determinant.md). A map $f:S_1\to S_2$ is a [smooth map](../../../../../smooth-map-between-manifolds.md) when every coordinate representation

$$
\psi\circ f\circ\phi^{-1}
$$

is smooth wherever it is defined.

The map $a:C\to C$ is a smooth involution with no fixed point: the equation

$$
(x,y,z)=(-x,-y,-z)
$$

would force $x=y=0$, which is impossible on $x^2+y^2=1$. For each $p\in C$, choose a sufficiently small coordinate neighbourhood $U_p$ such that

$$
U_p\cap a(U_p)=\varnothing.
$$

Then the quotient projection restricts to a homeomorphism

$$
\pi|_{U_p}:U_p\longrightarrow \pi(U_p).
$$

Transporting a smooth chart $\phi_p:U_p\to\mathbb R^2$ across this homeomorphism gives the quotient chart

$$
\widetilde\phi_p
=\phi_p\circ(\pi|_{U_p})^{-1}.
$$

On an overlap, a lift lies either in another chosen neighbourhood or in its image under $a$. The corresponding transition map is therefore a transition map on $C$, possibly composed with the diffeomorphism $a$, and is smooth. Since this is a free action of the finite group $\{1,a\}$, the quotient is Hausdorff and second countable. This constructs the [smooth quotient by a free finite group action](../../../../../smooth-quotient-by-a-free-finite-group-action.md), and in these charts $\pi$ is locally the identity. Hence $\pi$ is a [local diffeomorphism](../../../../../local-diffeomorphism.md), in particular smooth.

To test orientability, parametrize the cylinder by

$$
F(\theta,z)=(\cos\theta,\sin\theta,z).
$$

The involution acts in these coordinates as

$$
(\theta,z)\longmapsto(\theta+\pi,-z),
$$

whose derivative has determinant $-1$. Thus $a$ is an [orientation-reversing diffeomorphism](../../../../../orientation-reversing-diffeomorphism.md) of the cylinder.

If the quotient surface $S$ were orientable, its orientation would pull back through the local diffeomorphism $\pi$ to an orientation of $C$. The identity $\pi\circ a=\pi$ would then force $a$ to preserve that pulled-back orientation, contradicting the negative determinant above. Therefore

$$
\boxed{S\text{ is not orientable}}.
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
