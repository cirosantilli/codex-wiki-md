<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

For $u\in U$, define $\phi(u)\in U^*$ by $\phi(u)(u')=\langle u,u'\rangle$. If $\phi(u)=0$, then in particular

$$
0=\phi(u)(u)=\langle u,u\rangle=\lVert u\rVert^2,
$$

so $u=0$. Thus $\phi$ is [injective](../../../../../injective-function.md). Since a finite-dimensional vector space and its [dual space](../../../../../dual-space.md) have the same [dimension](../../../../../dimension-vector-space.md), $\phi$ is also [surjective](../../../../../surjective-function.md) and hence an [isomorphism](../../../../../isomorphism.md). This is the finite-dimensional real case of the [Riesz representation theorem](../../../../../riesz-representation-theorem.md).

The [adjoint operator](../../../../../adjoint-operator.md) of $\alpha:V\to W$ is the unique linear map $\alpha^*:W\to V$ satisfying

$$
\langle\alpha v,w\rangle_W=\langle v,\alpha^*w\rangle_V
$$

for every $v\in V$ and $w\in W$. In the stated [orthonormal bases](../../../../../orthonormal-basis.md), if $v$ and $w$ denote coordinate columns, then

$$
\langle Av,w\rangle=(Av)^Tw=v^TA^Tw.
$$

Therefore the matrix of $\alpha^*$ is the [matrix transpose](../../../../../transpose.md) $A^T$.

For $w\in W$,

$$
w\in\ker\alpha^*
\iff \langle v,\alpha^*w\rangle=0\text{ for every }v
\iff \langle\alpha v,w\rangle=0\text{ for every }v
\iff w\in(\operatorname{im}\alpha)^\perp.
$$

Hence $\ker\alpha^*=(\operatorname{im}\alpha)^\perp$. Taking orthogonal complements in the finite-dimensional space $W$ proves the [image-kernel orthogonality for an adjoint](../../../../../image-kernel-orthogonality-for-an-adjoint.md)

$$
\boxed{\operatorname{im}\alpha=(\ker\alpha^*)^\perp}.
$$

Put $r=\alpha(v_0)-w_0$. For any $h\in V$,

$$
\lVert\alpha(v_0+h)-w_0\rVert^2
=\lVert r\rVert^2+2\langle r,\alpha h\rangle+\lVert\alpha h\rVert^2.
$$

This is minimized at $h=0$ exactly when $r\perp\operatorname{im}\alpha$, equivalently when $\alpha^*r=0$. Thus the [normal equation for a linear inverse problem](../../../../../normal-equation-for-a-linear-inverse-problem.md) is

$$
\boxed{\alpha^*\alpha(v_0)=\alpha^*(w_0)}.
$$

For the given [linear least-squares problem](../../../../../linear-least-squares-problem.md),

$$
A^TA=\begin{pmatrix}2&1\\1&2\end{pmatrix},
\qquad
A^Tb=\begin{pmatrix}3\\5\end{pmatrix}.
$$

The normal equations $2x+y=3$ and $x+2y=5$ have the unique solution

$$
\boxed{x=\frac13,\qquad y=\frac73}.
$$

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
