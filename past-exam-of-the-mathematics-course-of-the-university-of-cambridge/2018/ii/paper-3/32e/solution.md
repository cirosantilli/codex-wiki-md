<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

Write $z=x+y$. When $\mu_1=\mu_2=0$ the system gives $\dot z=y-z^3$ and $\dot y=-z^3$. Choosing

$$
\boxed{V(x,y)=\frac14(x+y)^4+\frac12y^2}
$$

makes $V$ [positive definite](../../../../../positive-definiteness-of-a-lyapunov-function.md) and [radially unbounded](../../../../../coercive-function.md), while its [orbital derivative](../../../../../orbital-derivative.md) is

$$
\dot V=z^3(y-z^3)-yz^3=-z^6\leq0.
$$

The set $\{\dot V=0\}$ is $z=0$. A trajectory remaining there must also have $\dot z=y=0$, so its largest invariant subset is the origin. The [LaSalle invariance principle](../../../../../lasalle-s-invariance-principle.md) therefore proves that the origin is **globally asymptotically stable**. In the [phase plane](../../../../../phase-plane.md), $\dot x=0$ on $y=0$ and $\dot y=0$ on $x+y=0$; every nonstationary trajectory crosses the nested level curves of $V$ inward and tends to the origin.

At an [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), $y=0$ and

$$
x(\mu_1-x^2)=0.
$$

Hence the origin always exists, while $x=\pm\sqrt{\mu_1}$ exist for $\mu_1>0$. At $(x_*,0)$ the [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J_*=
\begin{pmatrix}
0&1\\
\mu_1-3x_*^2&\mu_2-3x_*^2
\end{pmatrix},
\quad
\det J_*=3x_*^2-\mu_1,
\quad
\operatorname{tr}J_*=\mu_2-3x_*^2.
$$

A [stationary bifurcation](../../../../../stationary-bifurcation.md) occurs when a real [eigenvalue](../../../../../eigenvalue.md) passes through zero, hence on

$$
\boxed{\mu_1=0.}
$$

A [Hopf bifurcation](../../../../../hopf-bifurcation.md) requires zero trace and positive determinant. At the origin this gives

$$
\boxed{\mu_2=0,\quad\mu_1<0,}
$$

and on either nonzero branch it gives

$$
\boxed{\mu_2=3\mu_1,\quad\mu_1>0.}
$$

Thus the Hopf locus consists of the negative $\mu_1$-axis and the ray $\mu_2=3\mu_1$ in the first quadrant; the stationary locus is the $\mu_2$-axis.

Now set $\mu_2=-1$, write $\mu=\mu_1$, and append $\dot\mu=0$. At $(x,y,\mu)=(0,0,0)$ the [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md) is tangent to the $(x,\mu)$-plane, so put $y=h(x,\mu)$. Its [centre-manifold invariance equation](../../../../../centre-manifold-invariance-equation.md) is

$$
h_xh=\mu x-h-(x+h)^3.
$$

Under the ordering $\mu=O(x^2)$, solving through cubic order gives

$$
\boxed{y=h(x,\mu)=\mu x-x^3+O(x^5),
\qquad
\dot x=\mu x-x^3+O(x^5).}
$$

This is the [pitchfork bifurcation normal form](../../../../../pitchfork-bifurcation-normal-form.md): $x=0$ is stable for $\mu<0$ and unstable for $\mu>0$, while the two stable branches $x=\pm\sqrt\mu$ emerge for $\mu>0$. The bifurcation is therefore a **supercritical pitchfork bifurcation**.

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
