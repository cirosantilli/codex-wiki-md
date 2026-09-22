<h1 id="5/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [dual Thurston polytope](../../../../../../dual-thurston-polytope.md) is the polar of the [Thurston norm](../../../../../../thurston-norm.md) unit ball. More intrinsically, in the real dual of $H_2(Y,\partial Y)$ it is

$$
B_T(Y)=\{\alpha:|\alpha(u)|\leq\|u\|_T\text{ for every }u\}.
$$

The pairing can be regarded as evaluation of $H^2(Y,\partial Y;\mathbb R)$ on [relative homology](../../../../../../relative-homology.md). Its definition remains valid when the [Thurston norm](../../../../../../thurston-norm.md) has a kernel: the polytope then lies in the annihilator of that kernel.

Identify $Y$ with the [pair of pants](../../../../../../pair-of-pants-mathematics.md) product $P\times S^1$. A regular [Seifert fiber](../../../../../../seifert-fiber.md) has homology class $h=\mu_1+\mu_2+\mu_3$. Let $e_i$ be the relative [homology class](../../../../../../homology-class.md) corresponding by [Poincare-Lefschetz duality](../../../../../../lefschetz-duality.md) to the homomorphism taking the $i$th meridian to one and the other two to zero. A spanning disk for $L_1$ punctured once by each of $L_2,L_3$ is an embedded [pair of pants](../../../../../../pair-of-pants-mathematics.md) $F$ representing $e_1$, with $c(F)=1$.

Take two arcs in $P$, one joining boundary one to boundary two, the other joining boundary one to boundary three. Their products with $S^1$ are embedded [vertical surfaces in a Seifert fibered space](../../../../../../vertical-surface-in-a-seifert-fibered-space.md), namely [annuli](../../../../../../annulus-mathematics.md) $A_{12},A_{13}$. Orient them so that their relative classes are $e_1-e_2$ and $e_1-e_3$. They cost zero. Thus the three required inequalities, with $\alpha_i=\alpha(e_i)$, are

$$
|\alpha_1|\leq1,\qquad |\alpha_1-\alpha_2|\leq0,\qquad |\alpha_1-\alpha_3|\leq0.
$$

For completeness they give the whole polytope. Oriented cut-and-paste of copies of $F,A_{12},A_{13}$ gives the upper bound $\|a e_1+b e_2+c e_3\|_T\leq|a+b+c|$. For the reverse bound, compress a minimizing surface and use the [classification of incompressible surfaces in Seifert fibered spaces](../../../../../../classification-of-incompressible-surfaces-in-seifert-fibered-spaces.md). Its horizontal components cover $P$ and have negative [Euler characteristic](../../../../../../euler-characteristic.md) equal to their unsigned covering degree; its vertical components have zero cost and zero intersection with a regular [Seifert fiber](../../../../../../seifert-fiber.md). The total signed horizontal degree is $a+b+c$, so its cost is at least $|a+b+c|$. Hence

$$
\boxed{\|a e_1+b e_2+c e_3\|_T=|a+b+c|,\qquad B_T(Y)=\{(s,s,s):-1\leq s\leq1\}.}
$$

It is a line segment, because this [Thurston norm](../../../../../../thurston-norm.md) has a two-dimensional kernel.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
