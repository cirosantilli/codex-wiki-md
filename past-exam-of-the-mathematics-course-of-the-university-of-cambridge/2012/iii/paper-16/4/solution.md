<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A closed connected [three-manifold](../../../../../3-manifold.md) has a [handle decomposition](../../../../../handle-decomposition.md) with one zero-handle and one three-handle. To arrange this, cancel the zero-handles along a spanning tree of connecting one-handles; perform the corresponding construction in the dual [handle decomposition](../../../../../handle-decomposition.md) to consolidate the three-handles. This does not require the [three-manifold](../../../../../3-manifold.md) to be orientable.

If there are $r$ one-handles and $s$ two-handles, the [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\chi(Y)=1-r+s-1=s-r.
$$

[Mod-two Poincare duality](../../../../../mod-two-poincare-duality.md) pairs the [Betti numbers](../../../../../betti-number.md) of a closed odd-dimensional [manifold](../../../../../topological-manifold.md), giving $\chi(Y)=0$. Thus $r=s$. The one-handles give $r$ [generators of a group](../../../../../generator-of-a-group.md) of the [fundamental group](../../../../../fundamental-group.md), the attaching circles of the two-handles give $r$ [relators](../../../../../relator.md), and the three-handle does not change the [fundamental group](../../../../../fundamental-group.md). Therefore **$\pi_1(Y)$ admits a balanced presentation**.

Now let

$$
G=\langle x_1,\ldots,x_r\mid R_1,\ldots,R_s\rangle
$$

be any finite [group presentation](../../../../../group-presentation.md). Start with a four-dimensional zero-handle and $r$ one-handles. Its [fundamental group](../../../../../fundamental-group.md) is the [free group](../../../../../free-group.md) on the $x_i$. Represent the finitely many [relators](../../../../../relator.md) by disjoint embedded circles in its three-dimensional boundary; a small perturbation makes the circles disjoint. Choose [framings of an embedded sphere](../../../../../framing-of-an-embedded-sphere.md) and attach $s$ two-handles. The resulting compact connected oriented four-manifold $W$ has $\pi_1(W)\cong G$ by the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md).

The map $\pi_1(\partial W)\to\pi_1(W)$ is surjective. One way to see this is to turn the [handle decomposition](../../../../../handle-decomposition.md) upside down: the relative handles based on $\partial W$ have indices $2,3,4$, and so add no [fundamental group](../../../../../fundamental-group.md) generators. Also $\partial W$ is connected, since surgery on embedded circles in a connected three-manifold preserves connectedness.

Take the [double of a manifold](../../../../../double-of-a-manifold.md)

$$
M=W\cup_{\partial W}(-W).
$$

It is a closed connected smooth oriented four-manifold. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives

$$
\pi_1(M)\cong G*_{\pi_1(\partial W)}G.
$$

Both maps from $\pi_1(\partial W)$ are the same surjection, under the natural identification of the two copies. The pushout identifies the two copies of every element of $G$ and imposes no new relations: the fold homomorphism is inverse to either inclusion. Thus

$$
\boxed{\pi_1(M)\cong G.}
$$

This is [four-manifold realization of finitely presented groups](../../../../../four-manifold-realization-of-finitely-presented-groups.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
