<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Retain $\Delta=\operatorname{div}\nabla$ and define the [heat operator](../../../../../heat-operator.md) by $L=\partial_t-\Delta_q$. A [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) $H(p,q,t)$ satisfies $L_qH=0$ for $t>0$ and has the delta initial limit

$$
\lim_{t\downarrow0}\int_M H(p,q,t)f(q)\,dV_q=f(p).
$$

On standard [Euclidean space](../../../../../euclidean-norm.md) the kernel is

$$
\boxed{g(p,q,t)=(4\pi t)^{-d/2}\exp\left(-\frac{|p-q|^2}{4t}\right).}
$$

On the [Riemannian manifold](../../../../../riemannian-manifold.md), the [Gaussian function](../../../../../gaussian-function.md) factor in the local construction uses $r(p,q)=\operatorname{dist}(p,q)$ in place of $|p-q|$.

Choose an open neighbourhood $\mathcal U$ of the diagonal such that every pair $(p,q)\in\mathcal U$ is joined by a unique short minimizing [geodesic](../../../../../geodesic.md) and $q=\exp_p x$ with the inverse [exponential map](../../../../../exponential-map-riemannian-geometry.md) smooth in both variables. It can be obtained from [normal coordinates](../../../../../normal-coordinates.md) tubes of radius smaller than the local [injectivity radius](../../../../../injectivity-radius.md), or from normal neighbourhoods with [geodesic convexity](../../../../../geodesic-convexity.md). Then $r^2$ is smooth on $\mathcal U$. Write the [Riemannian volume form](../../../../../riemannian-volume-form.md) in [normal coordinates](../../../../../normal-coordinates.md) as $dV_q=J(p,x)\,dx$, where $J>0$ is smooth and $J(p,0)=1$.

For fixed $p$, radial divergence in [normal coordinates](../../../../../normal-coordinates.md) gives

$$
\Delta_qr=\frac{d-1}{r}+\partial_r\log J,
\qquad
\Delta_qr^2=2d+2r\partial_r\log J.
$$

For $g=(4\pi t)^{-d/2}e^{-r^2/(4t)}$, use $|\nabla r|=1$ away from the diagonal and the [product rule](../../../../../product-rule.md) to obtain

$$
L(g t^i w)=g\left[t^{i-1}\left(r\partial_r+i+\frac r2\partial_r\log J\right)w-t^i\Delta_qw\right].
$$

The identities extend smoothly in the expressions involving $r\partial_r$, even though $r$ itself is not smooth on the diagonal. The singular powers cancel if

$$
\left(r\partial_r+\frac r2\partial_r\log J\right)w_0=0,
\qquad
\left(r\partial_r+i+\frac r2\partial_r\log J\right)w_i=\Delta_qw_{i-1}\quad(i\geq1).
$$

The correct initial normalization is $w_0(p,p)=1$. These [heat-kernel transport equations](../../../../../heat-kernel-transport-equations.md) have the explicit solutions

$$
\boxed{w_0(p,\exp_p x)=J(p,x)^{-1/2},}
$$

and, recursively,

$$
\boxed{w_i(p,\exp_p x)
=J(p,x)^{-1/2}\int_0^1 s^{i-1}J(p,sx)^{1/2}
(\Delta_qw_{i-1})(p,\exp_p(sx))\,ds.}
$$

To derive the integral, multiply the radial equation by $r^{i-1}J^{1/2}$ and integrate the derivative of $r^iJ^{1/2}w_i$ from zero to $r$. The zero integration constant is forced by smoothness when $i\geq1$. Changing variables from radial distance to $s\in[0,1]$ gives the displayed nonsingular expression. Its integrand is smooth in $(p,x,s)$, so differentiation under the integral proves inductively that every $w_i$ is smooth across the diagonal. In particular $w_i(p,p)=(\Delta_qw_{i-1})(p,p)/i$.

Summing the product-rule identity makes adjacent terms telescope. For $S_k=g\sum_{i=0}^kt^iw_i$, the only term remaining is

$$
\boxed{LS_k=-g t^k\Delta_qw_k.}
$$

This also fixes the sign convention: with the nonnegative [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) $P=-\Delta$, the right-hand side would instead be $+g t^kP_qw_k$.

A [heat parametrix](../../../../../heat-parametrix.md) is an approximate kernel with the same delta initial limit and an error under $L$ that is sufficiently regular, or flat, at $t=0$ to be corrected by time convolution. On a closed [compact manifold](../../../../../compact-manifold.md) choose a smooth cutoff $\chi(p,q)$ equal to one near the diagonal and supported in $\mathcal U$. A finite-order explicit parametrix is

$$
P_N(p,q,t)=\chi(p,q)(4\pi t)^{-d/2}e^{-r^2/(4t)}\sum_{i=0}^N t^i w_i(p,q).
$$

Near the diagonal its error is $-\chi g t^N\Delta_qw_N$. Derivatives of $\chi$ produce errors supported a positive distance from the diagonal, where $e^{-r^2/(4t)}$ decays faster than every power of $t$. Taking $N$ large makes the whole error as regular at time zero as any specified finite number of derivatives requires. Its initial delta limit follows from $J(p,0)=w_0(p,p)=1$ and the Euclidean [Gaussian function](../../../../../gaussian-function.md) change of variables $x=\sqrt t\,y$.

One may obtain a smooth error flat at zero by summing all coefficients with time cutoffs. Let $\rho\in C^\infty([0,\infty))$ equal one near zero and zero for arguments at least one, and choose $\epsilon_i\downarrow0$ sufficiently fast. Set

$$
P(p,q,t)=\chi(p,q)g(p,q,t)\sum_{i=0}^{\infty}\rho(t/\epsilon_i)t^i w_i(p,q).
$$

For each $t>0$ the sum is locally finite. Choosing $\epsilon_i$ successively so that the $i$th term and its derivatives through order $\lfloor i/2\rfloor$ have bounds $2^{-i}$ on their cutoff transition regions gives the usual smooth asymptotic sum. For any fixed derivative order, its tail is then smaller than an arbitrarily high power of $t$; the transport identities cancel all earlier orders. Consequently $R=L_qP$ extends smoothly and flatly to $t=0$.

Here is the [Volterra parametrix correction](../../../../../volterra-parametrix-correction.md), with the order of the [Volterra convolution of kernels](../../../../../volterra-convolution-of-kernels.md) factors specified. Define

$$
(A*B)(p,q,t)=\int_0^t\!\int_M A(p,z,s)B(z,q,t-s)\,dV_z\,ds.
$$

Since $L$ acts in the second spatial variable and $P$ has the delta initial limit, $L_q(Q*P)=Q+Q*R$. Thus

$$
\boxed{Q=\sum_{j=1}^{\infty}(-1)^jR^{*j},\qquad H=P+Q*P.}
$$

Indeed, $Q+R+Q*R=0$ by the geometric-series cancellation, whence $L_qH=0$. If $|R|\leq C$ on a bounded time interval and $v=\operatorname{vol}(M)$, then

$$
|R^{*j}|\leq C^jv^{j-1}\frac{t^{j-1}}{(j-1)!}.
$$

This proves convergence; the smooth flat error permits the corresponding derivative estimates. The correction has zero initial limit, so $H$ retains the delta initial condition. Uniqueness of the [heat equation](../../../../../heat-equation.md) on a closed [compact manifold](../../../../../compact-manifold.md) identifies this kernel with the global [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md).

The local coefficient construction requires no [compactness](../../../../../compact-space.md). The global uniformly bounded convolution argument just given uses a closed [compact manifold](../../../../../compact-manifold.md), the usual spectral-geometry setting. For noncompact or incomplete [Riemannian manifolds](../../../../../riemannian-manifold.md) one must specify the heat realization and justify global convergence separately; a canonical choice is the minimal kernel obtained as the increasing limit of Dirichlet kernels on a smooth relatively compact exhaustion. This gives the minimal heat semigroup rather than asserting an unqualified uniqueness statement at infinity or at a missing boundary.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
