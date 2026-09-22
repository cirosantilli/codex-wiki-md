<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

At an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), the second equation gives $x=y=:s$. The first equation then gives

$$
(a^2-s)(a-s^2)=0.
$$

Hence the fixed-point branches in the $(a,x)$ plane are

$$
\boxed{x=y=a^2\quad(a\in\mathbb R)}
$$

and

$$
\boxed{x=y=\pm\sqrt a\quad(a\geq0).}
$$

The three branches meet at $a=0$. The branch $x=a^2$ meets the positive square-root branch again when $a^2=\sqrt a$, so the second bifurcation value is

$$
\boxed{a^*=1.}
$$

The [Jacobian matrix](../../../../../jacobian-matrix.md) at a general point is

$$
J(x,y;a)=
\begin{pmatrix}
y^2-a&-2y(a^2-x)\\
1&-1
\end{pmatrix}.
$$

On the branch $P_0=(a^2,a^2)$ it is triangular, with [eigenvalues](../../../../../eigenvalue.md)

$$
\lambda_1=a^4-a,
\qquad \lambda_2=-1.
$$

Thus $P_0$ is [unstable](../../../../../unstable-equilibrium.md) for $a<0$, [asymptotically stable](../../../../../asymptotic-stability.md) for $0<a<1$, and unstable for $a>1$.

On a square-root branch write $s=\pm\sqrt a$. Then

$$
J(P_s)=
\begin{pmatrix}
0&2s^2(1-s^3)\\
1&-1
\end{pmatrix},
$$

whose trace is $-1$ and determinant is $2s^2(s^3-1)$. The negative branch $s=-\sqrt a$ is therefore a [saddle equilibrium](../../../../../saddle-equilibrium.md) for every $a>0$. The positive branch is a [saddle](../../../../../saddle-equilibrium.md) for $0<a<1$ and [asymptotically stable](../../../../../asymptotic-stability.md) for $a>1$; close to $a=1$ it is a [stable node](../../../../../stable-node.md).

To resolve the nonhyperbolic point at $a=0$, make the prescribed substitution

$$
X=x-a^2,
\qquad Y=y-a^2
$$

and append $\dot a=0$. The equations become

$$
\dot X=-aX+X(Y+a^2)^2,
\qquad
\dot Y=X-Y,
\qquad
\dot a=0.
$$

The centre subspace is $Y=X$. Seek the [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md) as

$$
Y=h(X,a)
=X+AX^2+BXa+Ca^2+O(3).
$$

The [centre-manifold invariance equation](../../../../../centre-manifold-invariance-equation.md) is

$$
h_X\dot X=X-h.
$$

To second order, $\dot X=-aX+O(3)$, so comparison of coefficients gives

$$
-aX=-AX^2-BXa-Ca^2,
$$

and hence $A=C=0$, $B=1$. Therefore

$$
\boxed{Y=X+aX+O(3).}
$$

Substitution into the $X$ equation gives the reduced flow

$$
\boxed{\dot X=-aX+X^3+O(4).}
$$

Its central branch $X=0$ is [unstable](../../../../../unstable-equilibrium.md) for $a<0$ and [stable](../../../../../asymptotic-stability.md) for $a>0$, while the two nonzero branches $X\sim\pm\sqrt a$ for $a>0$ are [unstable](../../../../../unstable-equilibrium.md). Thus the bifurcation at zero is a [subcritical pitchfork bifurcation](../../../../../subcritical-pitchfork-bifurcation.md) with reversed normal-form parameter $\mu=-a$, exactly as recorded by the [extended centre manifold of the 2023 Cambridge quadratic-product system](../../../../../extended-centre-manifold-of-the-2023-cambridge-quadratic-product-system.md).

The complete [bifurcation diagram](../../../../../bifurcation-diagram.md) is therefore as follows. For $a<0$, only $P_0$ exists and is [unstable](../../../../../unstable-equilibrium.md). For $0<a<1$, $P_0$ is [stable](../../../../../asymptotic-stability.md) while both $P_+$ and $P_-$ are saddles. For $a>1$, $P_+$ is [stable](../../../../../asymptotic-stability.md) while $P_0$ and $P_-$ are saddles. At $a=1$, $P_0$ and $P_+$ cross and exchange stability, so the bifurcation is [transcritical](../../../../../transcritical-bifurcation.md). This gives the [bifurcation diagram of the 2023 Cambridge quadratic-product system](../../../../../bifurcation-diagram-of-the-2023-cambridge-quadratic-product-system.md).

Finally consider the phase plane near $(x,y)=(1,1)$ with $|a-1|\ll1$. If $a<1$, the lower equilibrium $(a^2,a^2)$ is a stable node and the upper equilibrium $(\sqrt a,\sqrt a)$ is a saddle. If $a>1$, the lower equilibrium $(\sqrt a,\sqrt a)$ is the stable node and the upper equilibrium $(a^2,a^2)$ is the saddle. In each case the saddle has one-dimensional [stable and unstable manifolds](../../../../../stable-manifold.md); one unstable separatrix runs toward the nearby stable node, while the other runs out of the local neighbourhood. The two equilibrium branches and their local invariant manifolds exchange roles as $a$ passes through one, which is the standard local phase portrait of a transcritical bifurcation.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
