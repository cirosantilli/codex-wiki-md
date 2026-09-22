<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All [homology](../../../../../homology-split.md) and [cohomology](../../../../../cohomology-split.md) in this solution use $\mathbb F_2$ coefficients, so no [orientation](../../../../../orientation-of-a-simplex.md) hypothesis is necessary. The [Poincare-Lefschetz duality](../../../../../lefschetz-duality.md) degrees are complementary:

$$
\boxed{H_k(W;\mathbb F_2)\cong H^{n-k}(W,\partial W;\mathbb F_2).}
$$

The starred notation in the question must be understood with this degree reversal.

Turn the [handle decomposition](../../../../../handle-decomposition.md) upside down. An absolute $k$-handle becomes a relative $(n-k)$-handle based on $\partial W$. The absolute cellular boundary coefficient counts intersections of an [attaching sphere](../../../../../attaching-sphere.md) with a [belt sphere](../../../../../belt-sphere.md). In the reversed [handle decomposition](../../../../../handle-decomposition.md), the same intersections are counted in the opposite order. Over $\mathbb F_2$ the two incidence matrices are transposes, with no sign ambiguity. Thus the absolute [chain complex](../../../../../chain-complex.md) is the complementary-degree dual of the relative [chain complex](../../../../../chain-complex.md). Taking [homology](../../../../../homology-split.md) and using the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) over a [field](../../../../../field.md) proves the displayed [isomorphism](../../../../../isomorphism.md). This is [mod-two handle duality](../../../../../mod-two-handle-duality.md).

To obtain a [perfect pairing](../../../../../perfect-pairing.md) from the assumed closed case, form the [double of a manifold](../../../../../double-of-a-manifold.md) $D(W)$ from two copies of $W$. The fold map $D(W)\to W$ is a [retraction](../../../../../retraction.md), so the inclusion of either copy induces an injection on [homology](../../../../../homology-split.md). If $a\ne0$ in $H_k(W)$, its image in $H_k(D(W))$ is nonzero. Closed-manifold [mod-two Poincare duality](../../../../../mod-two-poincare-duality.md) supplies a class $z\in H_{n-k}(D(W))$ with intersection $1$ against that image. Cut a representative of $z$ along the boundary and retain its part in the first copy; it defines $b\in H_{n-k}(W,\partial W)$. Equivalently, apply the quotient map $D(W)\to D(W)/W_-\cong W/\partial W$ and [excision](../../../../../excision-theorem.md). Intersections with a representative of $a$ in the interior are unchanged, so $a\cdot b=1$. This proves nondegeneracy in the first variable. [Mod-two handle duality](../../../../../mod-two-handle-duality.md) gives equal finite dimensions for the two spaces, hence nondegeneracy in the second variable as well.

For the three-dimensional conclusion, set

$$
V=H_1(\partial W),\qquad L=\ker\bigl(H_1(\partial W)\to H_1(W)\bigr).
$$

The [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) says $L=\operatorname{im}\partial$, where $\partial:H_2(W,\partial W)\to V$. The closed-surface [intersection pairing](../../../../../intersection-pairing.md) on $V$ is nondegenerate. A collar calculation gives the adjoint identity

$$
(\partial b)\cdot x=b\cdot i_*x.
$$

Indeed, push $x$ slightly into the collar: intersections with the relative surface representing $b$ correspond to its boundary intersections with $x$. By the absolute-relative [perfect pairing](../../../../../perfect-pairing.md) already proved, $x$ is orthogonal to every $\partial b$ precisely when $i_*x=0$. Therefore $L^\perp=L$.

For any finite-dimensional space with a [perfect pairing](../../../../../perfect-pairing.md), $\dim L+\dim L^\perp=\dim V$. Hence the **half-lives-half-dies theorem** gives

$$
\boxed{\dim\ker i_*=\frac12\dim H_1(\partial W;\mathbb F_2).}
$$

But $H_1(\mathbb{RP}^2;\mathbb F_2)\cong\mathbb F_2$ has dimension one. It cannot be the entire boundary of a compact three-manifold, because the displayed dimension would be $1/2$. This excludes nonorientable three-manifolds as well as orientable ones.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
