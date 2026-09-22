<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose real constants $a_0<a_1<\cdots<a_m$ and define the smooth homogeneous quotient

$$
\boxed{f([x_0:\cdots:x_m])=\frac{\sum_{j=0}^ma_jx_j^2}{\sum_{j=0}^mx_j^2}.}
$$

It is unchanged by nonzero rescaling, so it is well defined on [Real projective space](../../../../../real-projective-space.md). On the unit [sphere](../../../../../sphere.md) its differential vanishes on the [tangent space](../../../../../tangent-space.md) precisely when $Ax$ is proportional to $x$, where $A=\operatorname{diag}(a_0,\ldots,a_m)$. The entries are distinct, so the only critical projective lines are $p_i=[e_i]$. In the affine chart $x_i=1$, write $u_j=x_j/x_i$ for $j\ne i$. Then

$$
f=a_i+\frac{\sum_{j\ne i}(a_j-a_i)u_j^2}{1+\sum_{j\ne i}u_j^2}.
$$

Its [Hessian](../../../../../hessian-matrix.md) at zero is diagonal with entries $2(a_j-a_i)$. Exactly $i$ are negative, and none vanish. Thus this is a [Morse function](../../../../../morse-function.md) with **one [critical point](../../../../../critical-point.md) $p_i$ of index $i$ for every $0\le i\le m$**.

Choose the quotient of the round metric on the unit [sphere](../../../../../sphere.md). The downward [gradient flow](../../../../../gradient-flow.md) has [sphere](../../../../../sphere.md) equation $\dot x_j=-2(a_j-f(x))x_j$ and projective solution

$$
[x_0(t):\cdots:x_m(t)]=[e^{-2a_0t}x_0(0):\cdots:e^{-2a_mt}x_m(0)].
$$

Normalization to the unit [sphere](../../../../../sphere.md) supplies the common positive factor. As $t\to+\infty$, the smallest index with nonzero coordinate dominates; as $t\to-\infty$, the largest dominates. Consequently

$$
W^u(p_i)=\{x_i\ne0,\ x_j=0\ (j>i)\}\cong\mathbb R^i,\qquad W^s(p_i)=\{x_i\ne0,\ x_j=0\ (j<i)\}\cong\mathbb R^{m-i}.
$$

These are its [unstable manifolds](../../../../../unstable-manifold.md) and [stable manifolds](../../../../../stable-manifold.md). If $j\ge k$, the tangent directions in $W^u(p_j)$ allow coordinates $0,\ldots,j$, and those in $W^s(p_k)$ allow $k,\ldots,m$, modulo the common projective line. Together they span the full [tangent space](../../../../../tangent-space.md) at every intersection. If $j<k$ the intersection is empty. Thus the flow is a [Morse-Smale gradient flow](../../../../../morse-smale-gradient-flow.md), with no generic perturbation needed.

Orient each unstable [manifold](../../../../../topological-manifold.md) using its affine coordinates. The [Morse-Smale complex](../../../../../morse-smale-complex.md) has $C_i=\mathbb Z p_i$; its differential counts oriented unparametrized connecting trajectories of index difference one. A trajectory from $p_i$ to $p_{i-1}$ has only coordinates $x_{i-1},x_i$ nonzero, and there are exactly two, distinguished by the sign of $x_{i-1}/x_i$. Each sign branch is a single orbit modulo time translation.

To calculate their signs rather than merely count two, use the characteristic [closed disk](../../../../../closed-disc.md) of the unstable cell: the closed upper hemisphere of $S^i$ with $x_i\ge0$, followed by projection onto $\mathbb{RP}^i$. Its interior is $W^u(p_i)$, and its boundary map is the antipodal double cover $S^{i-1}\to\mathbb{RP}^{i-1}$. After collapsing $\mathbb{RP}^{i-2}$, its degree on the $(i-1)$-cell is the sum of the degrees of the two sheets. Comparing the sheets by the [antipodal map](../../../../../antipodal-map.md) on $S^{i-1}$ gives relative orientation $(-1)^i$: it is induced by $-I$ on $\mathbb R^i$, whose determinant is $(-1)^i$. Thus the two trajectory signs add to $1+(-1)^i$, up to the choice of generator orientations. The [projective quadratic Morse complex](../../../../../projective-quadratic-morse-complex.md) is therefore

$$
\boxed{C_i=\mathbb Z\ (0\le i\le m),\qquad\partial_i=\begin{cases}2,&i\text{ even},\\0,&i\text{ odd}.\end{cases}}
$$

In particular $\partial_1=0$, as required for the connected one-dimensional skeleton. The signed trajectory count agrees with this attaching-map incidence calculation, so it computes integral rather than only mod-two [homology](../../../../../homology-split.md).

For $m\ge1$, taking kernels modulo images gives

$$
\boxed{H_k(\mathbb{RP}^m;\mathbb Z)=\begin{cases}\mathbb Z,&k=0,\\\mathbb Z/2,&0<k<m\text{ and }k\text{ odd},\\\mathbb Z,&k=m\text{ and }m\text{ odd},\\0,&\text{otherwise}.\end{cases}}
$$

For example, an odd interior-degree generator has zero outgoing differential but twice itself is the image from the next degree; an even positive-degree differential is injective. At the top there is no incoming differential, leaving a copy of $\mathbb Z$ exactly when $m$ is odd. For $m=0$ the space is one point and only $H_0=\mathbb Z$ remains. This recovers the [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) by explicitly constructing its [Morse-Smale complex](../../../../../morse-smale-complex.md) and signs.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
