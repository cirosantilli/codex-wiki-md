<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On a closed compact [Riemannian manifold](../../../../../riemannian-manifold.md), the [heat kernel](../../../../../heat-kernel.md) for the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) is the smooth kernel $K_M(t,x,y)$ of $e^{-t\Delta_M}$ for $t>0$. It solves $(\partial_t+\Delta_x)K_M=0$ and tends to the delta kernel as $t\downarrow0$, so that

$$
u(t,x)=\int_M K_M(t,x,y)f(y)\,dV_M(y),\qquad u(0,x)=f(x).
$$

For an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) with [eigenvalues](../../../../../eigenvalue.md) repeated according to multiplicity,

$$
K_M(t,x,y)=\sum_{j=0}^\infty e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)},\qquad
Z_M(t)=\operatorname{Tr}(e^{-t\Delta_M})=\int_MK_M(t,x,x)\,dV_M(x).
$$

The exponential factors and [elliptic regularity](../../../../../elliptic-regularity.md) ensure smooth convergence for positive time. If a boundary is present, the same construction uses a specified [boundary condition](../../../../../boundary-condition.md) preserved by the covering; the closed-manifold case is the one needed below.

Let $p:N\to M=N/U$ be the finite normal locally isometric [covering map](../../../../../covering-space.md). The [heat equation](../../../../../heat-equation.md) for $f\circ p$ on $N$ is the lift of the one for $f$ on $M$. Integrate the lifted solution over a [fundamental domain](../../../../../fundamental-domain.md) for the [deck transformation group](../../../../../deck-transformation-group.md) $U$, splitting the integral over $N$ into its translates. This gives

$$
\boxed{K_M(t,px,py)=\sum_{u\in U}K_N(t,x,uy)}.
$$

There is no averaging factor in this kernel formula: each translate accounts for one lift of the integration variable. To verify it directly, the sum solves the lifted [heat equation](../../../../../heat-equation.md) and its integral against $f$ converges to $f(px)$; uniqueness of the heat solution identifies the kernel. Replacing either lift $x$ or $y$ only permutes the sum, since [isometries](../../../../../isometry.md) preserve the [heat kernel](../../../../../heat-kernel.md).

Integrating the diagonal and using the covering degree gives the [heat trace](../../../../../heat-trace.md) formula

$$
\boxed{Z_M(t)=\frac1{|U|}\sum_{u\in U}F_t(u)},\qquad
F_t(u)=\int_NK_N(t,x,ux)\,dV_N(x).
$$

Suppose $U$ is contained in a [finite group](../../../../../finite-group.md) $T$ of [isometries](../../../../../isometry.md) of $N$. For $s\in T$, change variables $x=sy$ and use invariance of both volume and the [heat kernel](../../../../../heat-kernel.md). Then

$$
F_t(sus^{-1})=\int_NK_N(t,sy,suy)\,dV_N(y)=F_t(u).
$$

Thus $F_t$ is a [class function](../../../../../class-function.md) on $T$, and for its [conjugacy classes](../../../../../conjugacy-class.md) $\mathcal C$,

$$
Z_{N/U}(t)=\frac1{|U|}\sum_{\mathcal C\subset T}|U\cap\mathcal C|\,F_t(c_{\mathcal C}).
$$

Consequently, if $U_1,U_2\leq T$ are [Gassmann equivalent](../../../../../gassmann-equivalence.md) and act freely, their orders are equal and the displayed class-by-class sums give $Z_{N/U_1}(t)=Z_{N/U_2}(t)$ for every $t>0$. Equal [heat traces](../../../../../heat-trace.md) determine equal [eigenvalues](../../../../../eigenvalue.md) with multiplicities: the least [eigenvalue](../../../../../eigenvalue.md) at which the multiplicities differed would give a nonzero leading exponential in their [trace](../../../../../matrix-trace.md) difference as $t\to\infty$, a contradiction. Hence **the two smooth quotient manifolds are isospectral**. This proves the [Sunada theorem](../../../../../sunada-theorem.md), with the free-action hypothesis ensuring that the quotients are manifolds rather than [orbifolds](../../../../../orbifold.md). The theorem alone makes no nonisometry claim.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
