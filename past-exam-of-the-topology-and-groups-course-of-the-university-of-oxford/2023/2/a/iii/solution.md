<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [universal property of a pushout of groups](../../../../../universal-property-of-a-pushout-of-groups.md) says: for every [group](../../../../../group-split.md) $H$ and [group homomorphisms](../../../../../group-homomorphism.md) $u_j:G_j\to H$ satisfying $u_1\phi_1=u_2\phi_2$, there is exactly one [group homomorphism](../../../../../group-homomorphism.md) $u:P\to H$ such that

$$
\boxed{uj_1=u_1,\qquad uj_2=u_2.}
$$

To prove existence, the [universal property of a free product](../../../../../universal-property-of-a-free-product.md) supplies a unique [group homomorphism](../../../../../group-homomorphism.md) $v:G_1*G_2\to H$ with $vk_j=u_j$. Every defining [relator](../../../../../relator.md) of $N$ maps to

$$
u_1(\phi_1(h))\,u_2(\phi_2(h))^{-1}=1.
$$

Since $\ker v$ is a [normal subgroup](../../../../../normal-subgroup.md), it contains the entire [normal closure](../../../../../normal-closure.md) $N$. The [universal property of a quotient group](../../../../../universal-property-of-a-quotient-group.md) therefore gives a [group homomorphism](../../../../../group-homomorphism.md) $u:P\to H$ through which $v$ factors. Its restrictions are the required $u_j$.

For uniqueness, $j_1(G_1)$ and $j_2(G_2)$ together generate $P$: their preimages already generate the [free product](../../../../../free-product.md). Consequently a [group homomorphism](../../../../../group-homomorphism.md) out of $P$ is determined by its restrictions to these two [subgroups](../../../../../subgroup.md). Any two candidates for $u$ therefore coincide.

This also proves that the [pushout of groups](../../../../../pushout-of-groups.md) is unique up to a unique compatible [group isomorphism](../../../../../group-isomorphism.md). Given another such object $P'$, apply the [universal property](../../../../../universal-property.md) in both directions. Both composites restrict to the original maps from $G_1,G_2$, so uniqueness makes them the respective [identity maps](../../../../../identity-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
