<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\pi:T^*M\to M$ be the [cotangent bundle](../../../../../cotangent-bundle.md) projection. Its [canonical one-form on a cotangent bundle](../../../../../canonical-one-form-on-a-cotangent-bundle.md) is defined intrinsically by $\lambda_{(x,p)}(V)=p(d\pi(V))$, so locally $\lambda=p_i\,dx^i$. Choose the position-first [symplectic form](../../../../../symplectic-form.md)

$$
\omega=-d\lambda=dx^i\wedge dp_i.
$$

It is closed by $d^2=0$ and nondegenerate, since contraction with $a^i\partial_{x^i}+b_i\partial_{p_i}$ is $a^i dp_i-b_i dx^i$, which vanishes only when both coefficient sets vanish. The intrinsic definition of $\lambda$ makes this [symplectic form](../../../../../symplectic-form.md) independent of coordinates.

Use the convention $\iota_{X_H}\omega=dH$. Then the [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) and the [Poisson bracket](../../../../../poisson-bracket.md) are

$$
X_H=\frac{\partial H}{\partial p_i}\partial_{x^i}
-\frac{\partial H}{\partial x^i}\partial_{p_i},
\qquad
\{F,G\}=\frac{\partial F}{\partial x^i}\frac{\partial G}{\partial p_i}
-\frac{\partial F}{\partial p_i}\frac{\partial G}{\partial x^i},
$$

so $X_H(F)=\{F,H\}$. Choosing $\omega=d\lambda$ and $\iota_{X_H}\omega=-dH$ gives the same equations; choosing only one of these sign changes would reverse the flow.

For the [geodesic Hamiltonian](../../../../../geodesic-hamiltonian.md), [Hamilton's equations](../../../../../hamilton-s-equations.md) give

$$
\dot x^i=g^{ij}p_j,\qquad
\dot p_i=-\frac12(\partial_i g^{jk})p_jp_k.
$$

Put $v^i=\dot x^i$, so $p_i=g_{ij}v^j$. Differentiating $g^{jk}g_{ka}=\delta^j_a$ gives

$$
(\partial_i g^{jk})p_jp_k=-(\partial_i g_{ab})v^av^b.
$$

Consequently,

$$
g_{ij}\ddot x^j+(\partial_k g_{ij})v^kv^j
=\frac12(\partial_i g_{ab})v^av^b.
$$

Symmetrizing the velocity factors and raising the first index converts this to

$$
\boxed{\ddot x^\ell+\Gamma^\ell{}_{jk}\dot x^j\dot x^k=0},
\qquad
\Gamma^\ell{}_{jk}=\frac12g^{\ell i}
(\partial_jg_{ik}+\partial_kg_{ij}-\partial_ig_{jk}).
$$

These [Christoffel symbols](../../../../../christoffel-symbol.md) are those of the [Levi-Civita connection](../../../../../levi-civita-connection.md). Thus a Hamiltonian [integral curve of a vector field](../../../../../integral-curve-of-a-vector-field.md) projects to an affinely parametrized [geodesic](../../../../../geodesic.md). Conversely, an affinely parametrized [geodesic](../../../../../geodesic.md) lifts by $p_i=g_{ij}\dot x^j$ to an [integral curve of a vector field](../../../../../integral-curve-of-a-vector-field.md) of $X_H$, since reversing the calculation proves both [Hamilton's equations](../../../../../hamilton-s-equations.md). This is the [geodesic flow](../../../../../geodesic-flow.md) on the [cotangent bundle](../../../../../cotangent-bundle.md). The conserved [Hamiltonian](../../../../../hamiltonian.md) is half the squared speed, and the zero-energy case gives the constant [geodesics](../../../../../geodesic.md).

A quadratic [homogeneous polynomial](../../../../../homogeneous-polynomial.md) depends only on the symmetric part of its coefficient matrix. Accordingly take its unique [symmetric coefficients of a quadratic polynomial](../../../../../symmetric-coefficients-of-a-quadratic-polynomial.md), $K^{ij}=K^{ji}$. This is the standard implicit convention in identifying such polynomials with [symmetric tensors](../../../../../symmetric-tensor.md). If an arbitrary nonsymmetric representative were allowed, the literal equivalence would fail: in Euclidean $\mathbb R^2$, $K^{12}=x^1$, $K^{21}=-x^1$ and all other components zero give the zero polynomial, which has zero [Poisson bracket](../../../../../poisson-bracket.md) with every function, whereas the lowered coefficient array is not a [Killing tensor](../../../../../killing-tensor.md) because it is not symmetric.

Lower the indices of the symmetric coefficient tensor using the [Riemannian metric](../../../../../riemannian-metric.md). Since $p_i=g_{ij}v^j$,

$$
K^{ij}p_ip_j=K_{ij}v^iv^j.
$$

Along an affinely parametrized [geodesic](../../../../../geodesic.md), [metric compatibility](../../../../../metric-compatibility.md) and $\nabla_vv=0$ imply

$$
\frac{d}{dt}(K_{ij}v^iv^j)
=(\nabla_aK_{bc})v^av^bv^c
=\nabla_{(a}K_{bc)}\,v^av^bv^c.
$$

Here parentheses mean normalized symmetrization over all indicated indices. The left side is $\{K,H\}$ by the [Hamiltonian vector field](../../../../../hamiltonian-vector-field.md) convention. Therefore a [rank-two Killing tensor](../../../../../rank-two-killing-tensor.md), defined by symmetry and $\nabla_{(a}K_{bc)}=0$, gives a [quadratic geodesic first integral](../../../../../quadratic-geodesic-first-integral.md).

Conversely, if $\{K,H\}=0$ everywhere on $T^*M$, the last cubic expression vanishes for every $v$ at every point, because the [Riemannian metric](../../../../../riemannian-metric.md) identifies tangent and cotangent spaces invertibly. A symmetric trilinear form is determined by its diagonal cubic polynomial: equivalently, compare its coefficients, or polarize the cubic. Hence $\nabla_{(a}K_{bc)}=0$. This proves both directions:

$$
\boxed{\{K,H\}=0\quad\Longleftrightarrow\quad
K_{ij}=K_{ji}\ \text{and}\ \nabla_{(a}K_{bc)}=0}
$$

with symmetry understood on the coefficient representative from the outset. The equivalence is local and does not require [geodesic completeness](../../../../../geodesic-completeness.md).

For the final construction, the antisymmetric [differential two-form](../../../../../2-form.md) $Y$ is a [Killing-Yano two-form](../../../../../killing-yano-two-form.md). Its defining equation says $\nabla_aY_{bc}=-\nabla_bY_{ac}$. Antisymmetry of $Y$ also says $\nabla_aY_{bc}=-\nabla_aY_{cb}$, so the three-index tensor $\nabla_aY_{bc}$ is totally antisymmetric.

The proposed tensor is symmetric, since it is the inner product of the covectors $Y_{i\cdot}$ and $Y_{j\cdot}$:

$$
K_{ij}=g^{k\ell}Y_{ik}Y_{j\ell}=K_{ji}.
$$

There is a useful geometric proof of its [Killing tensor](../../../../../killing-tensor.md) equation. Along any affinely parametrized [geodesic](../../../../../geodesic.md), define $w_k=Y_{ik}v^i$. Then

$$
\nabla_vw_k=v^av^i\nabla_aY_{ik}+Y_{ik}\nabla_vv^i=0.
$$

The first term vanishes by antisymmetry in $a,i$, and the second by the [geodesic](../../../../../geodesic.md) equation. Thus $w$ is carried by [parallel transport](../../../../../parallel-transport.md). By [metric compatibility](../../../../../metric-compatibility.md), its squared norm is constant, and

$$
|w|^2=g^{k\ell}Y_{ik}Y_{j\ell}v^iv^j=K_{ij}v^iv^j.
$$

Every tangent vector is the initial velocity of a local [geodesic](../../../../../geodesic.md), so differentiation at the initial point gives $\nabla_{(a}K_{bc)}v^av^bv^c=0$ for every $v$. The same cubic-coefficient argument proves

$$
\boxed{\nabla_{(a}K_{bc)}=0}.
$$

This proves that the [square of a Killing-Yano two-form](../../../../../square-of-a-killing-yano-two-form.md) is a [rank-two Killing tensor](../../../../../rank-two-killing-tensor.md) and supplies a nonnegative [quadratic geodesic first integral](../../../../../quadratic-geodesic-first-integral.md). The argument also explains the conserved quantity: it is the squared norm of a covector that the [Killing-Yano two-form](../../../../../killing-yano-two-form.md) makes parallel along every [geodesic](../../../../../geodesic.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
