<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two opens are $U_1=\mathbb C\times\mathbb C^*$ and $U_2=\mathbb C^*\times\mathbb C$; their intersection is $(\mathbb C^*)^2$. There is just one degree-one term in the [Čech cochain complex](../../../../../../cech-cochain-complex.md), and no degree-two term. The [Čech coboundary](../../../../../../cech-coboundary.md) sends $(g_1,g_2)$ to $g_2-g_1$, so

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)
=\frac{\mathcal O((\mathbb C^*)^2)}{\mathcal O(\mathbb C\times\mathbb C^*)+\mathcal O(\mathbb C^*\times\mathbb C)}.}
$$

The denominator denotes the sum of the restricted function spaces.

To make the quotient explicit, expand a [holomorphic function](../../../../../../holomorphic-function.md) on the intersection in a normally convergent two-variable [Laurent series](../../../../../../laurent-series.md),

$$
h=\sum_{m,n\in\mathbb Z}a_{mn}z_1^mz_2^n.
$$

The terms with $m\geq0$ extend to $U_1$. Of the remaining terms, those with $n\geq0$ extend to $U_2$. Both subseries converge normally on their stated domains, by the coefficient bounds from the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md). The unique remaining representative is the doubly negative part

$$
h_{--}=\sum_{i,j\geq1}a_{-i,-j}z_1^{-i}z_2^{-j}.
$$

No nonzero series of this form lies in the denominator, since a function on $U_1$ has no negative $z_1$ exponents and a function on $U_2$ has no negative $z_2$ exponents.

Writing $w_i=z_i^{-1}$, these representatives are exactly $w_1w_2F(w_1,w_2)$ with $F$ an entire [holomorphic function](../../../../../../holomorphic-function.md) on $\mathbb C^2$. To see that $F$ is entire, integrate for the coefficients on arbitrarily small product circles: $|a_{-i,-j}|\leq M(r_1,r_2)r_1^ir_2^j$. Choosing $r_iR_i<1$ gives absolute convergence for $|w_i|\leq R_i$, for every finite pair $R_i$. Conversely every such entire $F$ supplies a normally convergent representative on the intersection. Therefore **the quotient consists of convergent doubly negative Laurent series**, not merely finite Laurent polynomials:

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)\cong w_1w_2\mathcal O(\mathbb C_w^2).}
$$

This gives the [holomorphic first cohomology of punctured complex two-space](../../../../../../holomorphic-first-cohomology-of-punctured-complex-two-space.md); for instance $1/(z_1z_2)$ represents a nonzero class.

For the comparison with [sheaf cohomology](../../../../../../sheaf-cohomology.md), $U_1,U_2$ and their intersection are [Stein manifolds](../../../../../../stein-manifold.md). They can be realized as closed [complex submanifolds](../../../../../../complex-submanifold.md) of affine complex spaces by adding equations $z_iw_i=1$ for their nonzero coordinates. [Cartan theorem B](../../../../../../cartan-theorem-b.md) makes their higher cohomology with coefficients in the [sheaf of holomorphic functions](../../../../../../structure-sheaf-of-a-complex-manifold.md) vanish. Thus the cover is acyclic for $\mathcal O_X$, and the [acyclic cover theorem](../../../../../../leray-s-theorem.md) gives

$$
\boxed{\check H^1(\mathfrak U,\mathcal O_X)\cong H^1(X,\mathcal O_X).}
$$

The individual cover members are Stein; their union has the nonzero cohomology just computed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
