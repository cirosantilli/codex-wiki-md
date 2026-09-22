<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) $\Delta=-\operatorname{div}\nabla$. For the global discrete spectral statements, take $M$ to be a [closed manifold](../../../../../closed-manifold.md) with a smooth [Riemannian metric](../../../../../riemannian-metric.md). The [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) is the integral kernel $H(t,x,y)$ of the [heat semigroup](../../../../../heat-semigroup.md) $e^{-t\Delta}$:

$$
(e^{-t\Delta}f)(x)=\int_MH(t,x,y)f(y)\,dV_y,\qquad
(\partial_t+\Delta_x)H=0,\qquad H(0,x,y)=\delta_y(x).
$$

The initial condition is distributional with respect to the [Riemannian volume form](../../../../../riemannian-volume-form.md). Equivalently, an orthonormal basis of [Laplacian eigenfunctions](../../../../../laplacian-eigenfunction.md) gives the [spectral expansion of the Riemannian heat kernel](../../../../../spectral-expansion-of-the-riemannian-heat-kernel.md)

$$
H(t,x,y)=\sum_j e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.
$$

The usual compact elliptic spectral theorem supplies this basis; polynomial [elliptic regularity](../../../../../elliptic-regularity.md) bounds and exponential decay prove convergence with every space derivative on $t\geq\varepsilon>0$. These analytic results may be used as clearly stated external ingredients. We will also construct the kernel locally and prove its short-time expansion.

On a sufficiently small neighbourhood of the diagonal, let $r=d(x,y)$ and write $x=\exp_y\xi$ in [geodesic normal coordinates](../../../../../geodesic-normal-coordinates.md), with $dV_x=J(y,\xi)\,d\xi$. The [heat kernel expansion](../../../../../heat-kernel-expansion.md) has the form

$$
H(t,x,y)\sim(4\pi t)^{-m/2}e^{-r^2/(4t)}\sum_{j\geq0}t^ju_j(x,y),\qquad m=\dim M.
$$

The [heat invariants](../../../../../heat-invariants.md) are the integrated diagonal coefficients $a_j=\int_Mu_j(x,x)\,dV_x$, so

$$
\operatorname{Tr}(e^{-t\Delta})\sim(4\pi t)^{-m/2}\sum_{j\geq0}a_jt^j.
$$

In particular

$$
a_0=\operatorname{vol}(M),\qquad a_1=\frac16\int_M R\,dV,\qquad
a_2=\frac1{360}\int_M(5R^2-2|\operatorname{Ric}|^2+2|\operatorname{Rm}|^2)\,dV.
$$

Here $R$ is [scalar curvature](../../../../../scalar-curvature.md), $\operatorname{Ric}$ is the [Ricci tensor](../../../../../ricci-tensor.md) and $\operatorname{Rm}$ is the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md). The last expression is the [integrated second scalar heat coefficient](../../../../../integrated-second-scalar-heat-coefficient.md); a local divergence term integrates to zero on a [closed manifold](../../../../../closed-manifold.md). The exponent of the leading heat-trace term determines dimension, and these coefficients determine volume, total [scalar curvature](../../../../../scalar-curvature.md), and the displayed integrated curvature combination. On a surface $R=2K$, where $K$ is [Gaussian curvature](../../../../../gaussian-curvature.md), so $a_1=\frac13\int K\,dA=\frac{2\pi}{3}\chi(M)$ by the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), and $a_2=\frac1{15}\int K^2\,dA$. Thus the [Euler characteristic](../../../../../euler-characteristic.md), and the genus of a connected orientable closed surface, are determined. The first three coefficients also detect constant [Gaussian curvature](../../../../../gaussian-curvature.md), since they determine $\int(K-\overline K)^2\,dA$. These conclusions do not claim that the pointwise curvature function or the metric is determined.

Here is the local construction. Put $g_t=(4\pi t)^{-m/2}e^{-r^2/(4t)}$. The [Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) and the radial expression for the geometric Laplacian give, for a smooth amplitude $u$,

$$
(\partial_t+\Delta_x)(g_t t^ju)
=g_t\left[t^{j-1}\left(r\partial_ru+\frac r2\partial_r\log J\,u+ju\right)+t^j\Delta_xu\right].
$$

The $t^{-2}$ terms cancel because $|\nabla r|=1$. Define $D=r\partial_r+(r/2)\partial_r\log J$. The singular term disappears with $u_0=J^{-1/2}$, normalized by $u_0(y,y)=1$. For $j\geq1$, cancel the remaining powers of $t$ by the [heat-kernel transport equations](../../../../../heat-kernel-transport-equations.md)

$$
(D+j)u_j=-\Delta_xu_{j-1},
$$

which have the explicit solution

$$
u_j(\exp_y\xi,y)=-J(y,\xi)^{-1/2}\int_0^1s^{j-1}J(y,s\xi)^{1/2}(\Delta_xu_{j-1})(\exp_y(s\xi),y)\,ds.
$$

This formula is obtained by differentiating $r^jJ^{1/2}u_j$ along each radial geodesic. It proves smoothness jointly in $x,y$, including the diagonal, by induction: the integrand is smooth on a fixed compact integration interval. A homogeneous solution of $(D+j)u=0$ has $r^jJ^{1/2}u$ constant along a ray, and smoothness at $r=0$ forces this constant to vanish for $j>0$. Thus the smooth transport coefficients are unique. In particular $u_j(y,y)=-(\Delta_xu_{j-1})(y,y)/j$. Expanding $J=1-\operatorname{Ric}_{ab}(y)\xi^a\xi^b/6+O(|\xi|^3)$ gives $u_1(y,y)=R(y)/6$, checking the sign convention.

Choose a smooth cutoff $\eta(x,y)$ that is one near the diagonal and supported where these [normal coordinates](../../../../../normal-coordinates.md) exist, and form the [heat parametrix](../../../../../heat-parametrix.md)

$$
P_N(t,x,y)=\eta(x,y)g_t(x,y)\sum_{j=0}^Nt^ju_j(x,y).
$$

It tends to the identity kernel as $t\downarrow0$: in [normal coordinates](../../../../../normal-coordinates.md) the Gaussian is an [approximate identity](../../../../../approximate-identity.md), and $u_0J=J^{1/2}\to1$ at the centre. Its residual $R_N=(\partial_t+\Delta_x)P_N$ is $\eta g_tt^N\Delta_xu_N$ plus cutoff-derivative terms supported a positive distance from the diagonal. Those latter terms are smaller than every power of $t$. Hence $R_N=O(t^{N-m/2})$ uniformly. Every prescribed finite number of derivatives has the same kind of estimate after increasing $N$; differentiating a Gaussian costs only finitely many powers of $t$.

For $N$ large enough that the residual is continuous and bounded up to time zero, use the [Volterra parametrix correction](../../../../../volterra-parametrix-correction.md). For kernels define

$$
(F*G)(t,x,y)=\int_0^t\int_MF(t-s,x,z)G(s,z,y)\,dV_z\,ds.
$$

Set $Q=-R_N+R_N*R_N-R_N*R_N*R_N+\cdots$. A bounded residual with bound $C$ gives

$$
|R_N^{*k}(t,x,y)|\leq C^k\operatorname{vol}(M)^{k-1}\frac{t^{k-1}}{(k-1)!},
$$

so this series converges and $Q+R_N+R_N*Q=0$. Because $P_N$ has identity initial kernel, differentiating the convolution gives $(\partial_t+\Delta_x)(P_N*Q)=Q+R_N*Q$. Thus

$$
\boxed{H=P_N+P_N*Q}
$$

is an exact kernel with the correct initial condition. Taking $N$ sufficiently large gives any required finite regularity; uniqueness of the heat equation makes the kernels obtained from different $N$ equal. For uniqueness, the difference applied to smooth initial data has zero initial value, and the energy identity $\frac d{dt}\|v\|_2^2=-2\|\nabla v\|_2^2$ forces $v=0$. Parabolic regularity then gives smoothness for positive time.

The Gaussian part of $P_N$ has uniformly bounded spatial $L^1$ norm, so the correction is $O(t^{N+1-m/2})$. This proves, uniformly near the diagonal,

$$
H(t,x,y)-g_t(x,y)\sum_{j=0}^Nt^ju_j(x,y)=O(t^{N+1-m/2}),
$$

with corresponding derivative estimates on increasing the truncation order. In particular on every parabolic neighbourhood $r\leq B\sqrt t$ it is the stated Gaussian expansion with relative remainder $O(t^{N+1})$, and on the diagonal it yields the complete [heat trace](../../../../../heat-trace.md) expansion. The standard off-diagonal Gaussian version on compact subsets of a sufficiently small convex normal neighbourhood follows from the same convolution estimates with the Gaussian factor retained: the inequality

$$
\frac{d(x,z)^2}{t-s}+\frac{d(z,y)^2}{s}\geq\frac{d(x,y)^2}{t}
$$

localizes the convolution to the unique joining geodesic; its transverse Hessian is positive, and Gaussian integration gives the successive transport orders. The additive estimate above already specifies an appropriate uniform near-diagonal remainder without asserting a relative estimate far from the diagonal on the basis of a crude bound.

If $M$ is noncompact, use the minimal [Friedrichs extension](../../../../../friedrichs-extension.md) heat semigroup; if there is a boundary, specify boundary conditions. The same construction is local in the interior. One may extend a relatively compact coordinate neighbourhood to a closed auxiliary manifold; localization errors are supported a positive distance away and are exponentially small near the smaller diagonal neighbourhood. Thus the local coefficients remain the same. Finite integrated [heat invariants](../../../../../heat-invariants.md) and a discrete [spectrum](../../../../../spectrum-functional-analysis.md) require the global hypotheses used above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
