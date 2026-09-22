<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Identify $\operatorname{Pic}^{g-1}(X)$ with the [Jacobian variety](../../../../../jacobian-variety.md) using the base point and the translation of Solution 4. A [line bundle](../../../../../line-bundle.md) $L$ of degree $g-1$ corresponds to the point $z=u(D)-\kappa$ for any [divisor](../../../../../divisor.md) representation $L\simeq\mathcal O_X(D)$. The [Riemann singularity theorem](../../../../../riemann-singularity-theorem.md) is

$$
\boxed{\operatorname{mult}_{z}\Theta=h^0(X,L).}
$$

In particular, the [theta divisor](../../../../../theta-divisor.md) is singular exactly at the degree-$g-1$ [line bundles](../../../../../line-bundle.md) with at least two independent sections. We prove the equality, including the upper bound on multiplicity.

Choose a fixed effective [divisor](../../../../../divisor.md) $A$ of degree $N\ge g$, and a local [holomorphic](../../../../../complex-differentiability-at-a-point.md) family $L_\eta$ representing nearby points of $\operatorname{Pic}^{g-1}(X)$. Such a family can be constructed locally from the [holomorphic exponential sequence](../../../../../holomorphic-exponential-sequence.md), by varying line-bundle transition functions through exponentials of [Čech cohomology](../../../../../cech-cohomology.md) representatives. By [Serre duality](../../../../../serre-duality.md), $H^1(L_\eta(A))$ is dual to $H^0(K_X\otimes L_\eta^{-1}(-A))$, whose degree is $g-1-N<0$, so it vanishes. The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(L_\eta(A))=N$. By [cohomology and base change for line bundles on a curve](../../../../../cohomology-and-base-change-for-line-bundles-on-a-curve.md), these spaces form a [holomorphic vector bundle](../../../../../holomorphic-vector-bundle.md) $E$ of [rank](../../../../../rank-one-quadratic-form.md) $N$. The spaces $H^0(L_\eta(A)|_A)$ form another [holomorphic vector bundle](../../../../../holomorphic-vector-bundle.md) $F$ of [rank](../../../../../rank-one-quadratic-form.md) $N$. Evaluation gives a [holomorphic](../../../../../complex-differentiability-at-a-point.md) square matrix $T(\eta)$ locally, with exact sequence

$$
0\longrightarrow H^0(L_\eta)\longrightarrow E_\eta
\xrightarrow{T(\eta)}F_\eta\longrightarrow H^1(L_\eta)\longrightarrow0.
$$

Consequently $\det T(\eta)=0$ exactly when $L_\eta$ has a nonzero section, namely on the support of the [theta divisor](../../../../../theta-divisor.md).

At the point $L$, put $r=h^0(L)=h^1(L)$, the equality being [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). An invertible minor of size $N-r$ persists near this point. [Holomorphic](../../../../../complex-differentiability-at-a-point.md) row and column operations, or the [Schur complement](../../../../../schur-complement.md), give

$$
\det T(\eta)=a(\eta)\det M(\eta),\qquad a(0)\ne0,
\qquad M(0)=0,
$$

where $M$ is an $r\times r$ [holomorphic](../../../../../complex-differentiability-at-a-point.md) matrix. This is the [Schur complement presentation of a theta singularity](../../../../../schur-complement-presentation-of-a-theta-singularity.md). Its linear term in a tangent direction $\xi\in H^1(\mathcal O_X)$ is the [cup product](../../../../../cup-product.md) map

$$
dM_0(\xi):H^0(L)\longrightarrow H^1(L),\qquad s\longmapsto\xi\smile s.
$$

To see this concretely, vary transition functions $g_{ij}$ of $L$ to $g_{ij}(1+\epsilon\xi_{ij})$. A section $s_i$ lifts to $s_i+\epsilon s'_i$ precisely when its first-order compatibility equation can be solved; the obstruction is the cocycle $\xi_{ij}s_j$. This is $\xi\smile s$. Passing to the [kernel](../../../../../kernel-of-a-linear-map.md) and [cokernel](../../../../../cokernel.md) of $T(0)$ gives exactly the derivative of the reduced matrix $M$, proving the assertion without assuming a multiplicity formula.

Before extracting the order of $\det M$, we verify that $\det T$ is a reduced equation of the [theta divisor](../../../../../theta-divisor.md). Generic points of $W_{g-1}$ have $h^0(L)=1$ by Solution 3. At such a point, both $H^0(L)$ and $H^0(K_X\otimes L^{-1})$ are one-dimensional. Their nonzero sections $s,t$ have nonzero product $st\in H^0(K_X)$. Choose $\xi\in H^1(\mathcal O_X)$ with $\langle\xi,st\rangle\ne0$ under [Serre duality](../../../../../serre-duality.md). The scalar $dM_0(\xi)$ is nonzero, so $\det T$ has a simple zero generically on the [irreducible](../../../../../irreducible-representation.md) [theta divisor](../../../../../theta-divisor.md). Since its support is exactly that [irreducible](../../../../../irreducible-representation.md) [hypersurface](../../../../../hypersurface.md), it defines the reduced [divisor](../../../../../divisor.md). Solution 4 independently proved the same reduced structure for the [Riemann theta function](../../../../../riemann-theta-function.md). On the smooth ambient [Jacobian variety](../../../../../jacobian-variety.md), local equations of the same reduced [divisor](../../../../../divisor.md) differ by a nonvanishing [holomorphic](../../../../../complex-differentiability-at-a-point.md) unit. Hence the orders of the local theta equation and $\det M$ agree everywhere.

Every entry of $M$ vanishes at the point, so each term in its [determinant](../../../../../determinant.md) has order at least $r$. This proves $\operatorname{mult}_z\Theta\ge r$. To obtain equality, we exhibit an [invertible cup-product direction for a line bundle on a curve](../../../../../invertible-cup-product-direction-for-a-line-bundle-on-a-curve.md). Set $V=H^0(L)$ and $W=H^0(K_X\otimes L^{-1})$, both of dimension $r$. There are $r$ distinct points $p_1,\ldots,p_r$ at which evaluation is an [isomorphism](../../../../../isomorphism.md) for $V$: choose them inductively, since a surviving nonzero section has only finitely many zeros. The same holds for $W$. The nonvanishing of each evaluation [determinant](../../../../../determinant.md) defines a nonempty open subset of the [irreducible](../../../../../irreducible-representation.md) variety $X^r$. Their intersection, also avoiding the diagonals, is therefore nonempty. Choose points in it and [local coordinates](../../../../../local-coordinate.md) and compatible trivializations of $L$ and $K_X\otimes L^{-1}$ at each point.

Let $\xi$ be the [connecting homomorphism](../../../../../connecting-homomorphism.md) class of the [meromorphic](../../../../../meromorphic-function.md) [principal parts](../../../../../principal-part-of-a-meromorphic-function.md) $\lambda_i/t_i$ at these points, with all $\lambda_i\ne0$. The [residue](../../../../../residue.md) form of [Serre duality](../../../../../serre-duality.md) gives

$$
\langle\xi\smile s,t\rangle=\langle\xi,st\rangle
=\sum_{i=1}^r\lambda_i s(p_i)t(p_i).
$$

If $S$ and $U$ are the two invertible evaluation matrices, the matrix of this pairing is $S^t\operatorname{diag}(\lambda_1,\ldots,\lambda_r)U$, and is invertible. Thus the [cup product](../../../../../cup-product.md) map $\xi\smile-:H^0(L)\to H^1(L)$ is an [isomorphism](../../../../../isomorphism.md). Along the corresponding analytic parameter line,

$$
M(\epsilon\xi)=\epsilon\,dM_0(\xi)+O(\epsilon^2),\qquad
\det M(\epsilon\xi)=\epsilon^r\det(dM_0(\xi))+O(\epsilon^{r+1}),
$$

with nonzero leading coefficient. The order is at most $r$, completing the proof of the [Riemann singularity theorem](../../../../../riemann-singularity-theorem.md).

This argument also identifies the [tangent cone to a theta divisor](../../../../../tangent-cone-to-a-theta-divisor.md): its degree-$r$ equation is $\det(\xi\smile-)$, which is not the zero polynomial. For $r=1$, the tangent hyperplane is $\langle\xi,st\rangle=0$, in agreement with the annihilator description of the [derivative of the Abelian sum map](../../../../../derivative-of-the-abelian-sum-map.md). For $r\ge2$ all first derivatives vanish, proving singularity. In [genus](../../../../../genus-of-a-surface.md) $1$ the [theta divisor](../../../../../theta-divisor.md) is a single smooth point of multiplicity $1$. In [genus](../../../../../genus-of-a-surface.md) $0$ the effective degree-$-1$ locus is empty, so there is no singularity statement at a point of it.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
