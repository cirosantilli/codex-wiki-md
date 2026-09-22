<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [Riemannian metric](../../../../riemannian-metric-split.md) is a smooth positive definite symmetric bilinear form $g_q$ on each [tangent space](../../../../tangent-space.md). The inverse form on the cotangent space defines the kinetic [Hamiltonian](../../../../hamiltonian.md)

$$
H(q,p)=\tfrac12g_q^{-1}(p,p)=\tfrac12g^{ij}(q)p_ip_j.
$$

It is smooth and satisfies $H(q,ap)=a^2H(q,p)$. With the canonical [symplectic form](../../../../symplectic-form.md) $\Omega=\sum_i dq^i\wedge dp_i$, define $\iota_{X_H}\Omega=dH$. This gives Hamilton's equations

$$
\dot q^i=\partial_{p_i}H=g^{ij}p_j,\qquad\dot p_i=-\partial_{q^i}H.
$$

Thus $p_i=g_{ij}\dot q^j$. Differentiating the inverse metric yields $\dot p_i=\tfrac12\partial_i g_{jk}\dot q^j\dot q^k$. Differentiating $p_i=g_{ij}\dot q^j$ and substituting gives

$$
\ddot q^i+\Gamma^i_{jk}\dot q^j\dot q^k=0.
$$

Therefore the projections of the [Hamiltonian](../../../../hamiltonian.md) integral curves are affinely parametrized geodesics, and lifting a [geodesic](../../../../geodesic.md) by its metric covector gives a [Hamiltonian](../../../../hamiltonian.md) integral curve.

For the [Killing vector field](../../../../killing-vector-field-split.md) define the fibrewise linear [function](../../../../function-split.md) $f(q,p)=p(Y_q)=p_iY^i(q)$. Along the lifted [geodesic](../../../../geodesic.md) it equals $g(\dot q,Y)$. Metric compatibility and the [geodesic equation](../../../../geodesic-equation.md) give

$$
\frac d{dt}g(\dot q,Y)=g(\dot q,\nabla_{\dot q}Y)=\tfrac12(\mathcal L_Yg)(\dot q,\dot q)=0.
$$

Thus **$f$ is conserved**. Equivalently the cotangent lift of the [isometry](../../../../isometry.md) flow preserves $H$, and its generator has [Hamiltonian](../../../../hamiltonian.md) $f$, so their [Poisson bracket](../../../../poisson-bracket.md) vanishes.

For the final two metrics write $s=\ell(x)+m(y)$, restricting to an [open set](../../../../open-set.md) where the printed tensors are smooth nondegenerate metrics. Their inverse forms give

$$
H_1=\frac{p_x^2+p_y^2}{2s},\qquad
H_2=\frac{m(y)p_x^2-\ell(x)p_y^2}{2s}=m(y)H_1-\frac12p_y^2.
$$

Along the $H_1$ flow, $H_1$ is constant, while

$$
\dot y=p_y/s,\qquad \dot p_y=\frac{m'(y)}{2s^2}(p_x^2+p_y^2)=\frac{m'(y)H_1}{s}.
$$

Hence

$$
\boxed{\frac{dH_2}{dt}=m'(y)\frac{p_y}{s}H_1-p_y\frac{m'(y)H_1}{s}=0}.
$$

This is the [Liouville metric geodesic integral](../../../../liouville-metric-geodesic-integral.md), a quadratic conserved quantity. It does not require a [Killing vector field](../../../../killing-vector-field-split.md); it arises from the separated metric coefficients. When both printed metrics are Riemannian, their positivity in particular requires $s>0$, $m>0$ and $\ell<0$; the calculation also applies wherever the corresponding inverse tensors are defined.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the lie Groups and Differentiable Manifolds course of the University of Oxford](../../../split.md)
5. [Lie Groups and Differentiable Manifolds course of the University of Oxford](../../../../lie-groups-and-differentiable-manifolds-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
