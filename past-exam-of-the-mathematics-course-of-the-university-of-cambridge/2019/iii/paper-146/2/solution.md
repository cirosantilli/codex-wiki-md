<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [symplectic neighborhood theorem](../../../../../symplectic-neighborhood-theorem.md) says that a symplectomorphism between closed symplectic submanifolds which lifts to an isomorphism of their [symplectic normal bundles](../../../../../symplectic-normal-bundle.md) extends to a symplectomorphism of neighborhoods.

Let $C_X\subset X$ and $C_Y\subset Y$ be the given copies of $C$. Their self-intersection numbers are the [Euler classes](../../../../../euler-class-of-a-vector-bundle.md) of their oriented normal bundles, so square zero makes both normal bundles trivial. The neighborhood theorem identifies neighborhoods with $C\times D^2$. Remove their interiors and identify the boundary circle bundles by a map covering the chosen identification $C_X\cong C_Y$ and reversing the normal-circle orientation. On collars, the two forms have the model

$$
\omega_C+d(r^2d\theta),
$$

and the radial coordinate can be reversed while the circle coordinate is reversed so that the forms glue. A collar application of [Moser's trick](../../../../../moser-s-trick.md) removes any discrepancy. This proves that the [symplectic fiber sum along a square-zero surface](../../../../../symplectic-fiber-sum-along-a-square-zero-surface.md) $X\#_CY$ has a natural symplectic form.

The displayed relation is an ordinary product relation, so

$$
\Gamma=\langle a,b,c\mid ba=ac\rangle
\cong\langle a,c\rangle=F_2,
$$

where the relation eliminates $b=aca^{-1}$. The [Gompf realization theorem](../../../../../gompf-realization-theorem.md) constructs a closed symplectic four-manifold $M_\Gamma$ with this fundamental group. Concretely, its construction starts from a product of a sufficiently high-genus surface and a torus, represents the two surviving generators and the relations by loops, and crosses the relevant loops with circle factors to obtain square-zero tori. Symplectic sums with copies of the [rational elliptic surface](../../../../../rational-elliptic-surface.md) kill the unwanted generators and impose the relations: the complement of a regular elliptic fiber is simply connected, so the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) gives exactly $\pi_1(M_\Gamma)=\Gamma\cong F_2$.

Finally, $\mathbb{CP}^{48}$ is simply connected and has real dimension $96$. With the product symplectic form,

$$
\boxed{M_\Gamma\times\mathbb{CP}^{48}}
$$

is a closed symplectic manifold of real dimension $100$ and has fundamental group $\Gamma$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 146](../../paper-146-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
