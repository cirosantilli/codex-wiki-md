<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) convention $R(X,Y)Z=\nabla_X\nabla_YZ-\nabla_Y\nabla_XZ-\nabla_{[X,Y]}Z$. A [Jacobi field](../../../../../jacobi-field.md) is a smooth [vector field](../../../../../vector-field.md) $J$ along $\gamma$ satisfying

$$
\boxed{D_t^2J+R(J,\dot\gamma)\dot\gamma=0,}
$$

where $D_t$ is the [covariant derivative along a curve](../../../../../covariant-derivative-along-a-curve.md) for the [Levi-Civita connection](../../../../../levi-civita-connection.md). Differentiating a [geodesic variation](../../../../../geodesic-variation.md) gives this equation, and conversely every [Jacobi field](../../../../../jacobi-field.md) arises from a [geodesic variation](../../../../../geodesic-variation.md) by varying its initial point and velocity.

Choose a [parallel frame](../../../../../parallel-frame-along-a-curve.md) $E_1(t),\ldots,E_n(t)$ along $\gamma$ and write $J=\sum_a y_aE_a$. The [Jacobi equation](../../../../../jacobi-equation.md) becomes the linear system

$$
y''(t)+K(t)y(t)=0,\qquad K_{ab}(t)=\langle R(E_b,\dot\gamma)\dot\gamma,E_a\rangle.
$$

The existence and uniqueness theorem for linear [ordinary differential equations](../../../../../ordinary-differential-equation.md) says that each pair $(y(0),y'(0))\in\mathbb R^n\oplus\mathbb R^n$ determines exactly one solution on $[0,1]$. Addition and scalar multiplication preserve the equation. Thus evaluation of initial position and covariant velocity is a linear isomorphism

$$
\mathcal J_\gamma\longrightarrow T_{\gamma(0)}M\oplus T_{\gamma(0)}M,
\qquad J\longmapsto(J(0),D_tJ(0)),
$$

and **the dimension is**

$$
\boxed{\dim\mathcal J_\gamma=2n.}
$$

For the convexity assertion, use the convex-normal meaning of a geodesically convex open set: its points are joined by a unique geodesic within the set, and the joining geodesic depends smoothly on its endpoints. Equivalently, the appropriate star-shaped restriction of $\exp_p$ is a [diffeomorphism](../../../../../diffeomorphism.md) onto the set. The convex-normal-neighbourhood theorem supplies such sets around every point. Mere existence of some minimizing geodesic, without this uniqueness and normality, would not imply the assertion.

Let $p=\gamma(0)$ and $v=\dot\gamma(0)$. For a [Jacobi field](../../../../../jacobi-field.md) with $J(0)=0$ and $D_tJ(0)=w$, differentiating $\exp_p(t(v+sw))$ gives the standard differential-of-the-[exponential map](../../../../../exponential-map-riemannian-geometry.md) identity

$$
J(1)=(d\exp_p)_v(w).
$$

In a [convex normal neighbourhood](../../../../../convex-normal-neighbourhood.md), $(d\exp_p)_v$ is invertible. Therefore a [Jacobi field](../../../../../jacobi-field.md) vanishing at both endpoints has $w=0$ and hence is identically zero. The difference of two fields with the same endpoint values consequently vanishes. More precisely, the map

$$
\boxed{\mathcal J_\gamma\longrightarrow T_pM\oplus T_{\gamma(1)}M,\qquad J\longmapsto(J(0),J(1))}
$$

is an isomorphism: it is injective and both spaces have dimension $2n$. The constant-geodesic case follows directly from $D_t^2J=0$. This uses the convex-normal-neighbourhood theorem, the differential-of-the-[exponential map](../../../../../exponential-map-riemannian-geometry.md) identity, and linear [ordinary differential equation](../../../../../ordinary-differential-equation.md) uniqueness.

For the [special unitary group](../../../../../special-unitary-group.md) example, use [Jacobi fields from conjugation at a central endpoint](../../../../../jacobi-fields-from-conjugation-at-a-central-endpoint.md). Write

$$
A=\operatorname{diag}(2\pi i/3,2\pi i/3,-4\pi i/3),\qquad z=e^{2\pi i/3}.
$$

The endpoints of $\gamma(t)=\exp(tA)$ are $I$ and $zI$. The latter is central. For every $X\in\mathfrak{su}(3)$ consider

$$
F_X(s,t)=e^{sX}e^{tA}e^{-sX}.
$$

Conjugation is an [isometry](../../../../../isometry.md) for a [bi-invariant Riemannian metric](../../../../../bi-invariant-riemannian-metric.md), and [geodesics of a bi-invariant metric are one-parameter subgroups](../../../../../geodesics-of-a-bi-invariant-metric-are-one-parameter-subgroups.md). Thus $F_X$ is a [geodesic variation](../../../../../geodesic-variation.md). Its [Jacobi field](../../../../../jacobi-field.md) is

$$
J_X(t)=Xe^{tA}-e^{tA}X,
$$

which vanishes at $t=0$ and $t=1$ because both endpoints are central. Its initial covariant derivative is $[X,A]$.

The linear map $X\mapsto J_X$ has kernel equal to the [centralizer of an element of a Lie algebra](../../../../../centralizer-of-an-element-of-a-lie-algebra.md) of $A$. Indeed, $J_X\equiv0$ implies $[X,A]=0$ on differentiating at $t=0$, and that commutation conversely implies $J_X\equiv0$. The repeated first two eigenvalues give

$$
\mathfrak z(A)=\left\{\begin{pmatrix}B&0\\0&c\end{pmatrix}:B\in\mathfrak u(2),\ c\in i\mathbb R,\ \operatorname{tr}B+c=0\right\},\qquad\dim_\mathbb R\mathfrak z(A)=4.
$$

As $\dim_\mathbb R\mathfrak{su}(3)=8$, [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives

$$
\boxed{\dim\{J:J(0)=J(1)=0\}\geq8-4=4.}
$$

Explicit independent generators are the fields belonging to $E_{13}-E_{31}$, $i(E_{13}+E_{31})$, $E_{23}-E_{32}$ and $i(E_{23}+E_{32})$. Their initial derivatives $[X,A]$ are independent because the eigenvalue differences in the $13$ and $23$ entries are $2\pi i$. This also demonstrates directly why the endpoint-value conclusion fails along this geodesic.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 116](../../paper-116-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
