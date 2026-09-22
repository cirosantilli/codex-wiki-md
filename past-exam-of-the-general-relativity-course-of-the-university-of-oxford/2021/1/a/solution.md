<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The apple's [proper time](../../../../proper-time.md) $\tau$ is the time read by a clock carried with it, with $d\tau^2=-ds^2/c^2$ for [metric signature](../../../../metric-signature.md) $-+++$. At any event choose a [local inertial frame](../../../../local-inertial-frame.md) with coordinates $\xi^\alpha$, in which free motion satisfies $d^2\xi^\alpha/d\tau^2=0$ at that event. The [chain rule](../../../../chain-rule.md) gives

$$
0=\frac{\partial\xi^\alpha}{\partial x^\mu}\frac{d^2x^\mu}{d\tau^2}
+\frac{\partial^2\xi^\alpha}{\partial x^\nu\partial x^\lambda}
\frac{dx^\nu}{d\tau}\frac{dx^\lambda}{d\tau}.
$$

Multiplying by the inverse coordinate [Jacobian matrix](../../../../jacobian-matrix.md) yields the exact [geodesic equation](../../../../geodesic-equation.md)

$$
\boxed{\frac{d^2x^\mu}{d\tau^2}+\Gamma^\mu_{\nu\lambda}u^\nu u^\lambda=0,\qquad
u^\mu=\frac{dx^\mu}{d\tau},\qquad
\Gamma^\mu_{\nu\lambda}=\frac{\partial x^\mu}{\partial\xi^\alpha}
\frac{\partial^2\xi^\alpha}{\partial x^\nu\partial x^\lambda}.}
$$

Here $x^\mu$ are the observer's coordinates, $u^\mu$ is the apple's [four-velocity](../../../../four-velocity.md), and the [Christoffel symbols](../../../../christoffel-symbol.md) describe the [Levi-Civita connection](../../../../levi-civita-connection.md). The last expression applies when the $\xi$ coordinates are locally inertial at the event considered; one such chart need not remain inertial throughout a finite region.

Choose $x^0=ct$, so $u^0=c\,dt/d\tau$. In the [weak-field approximation](../../../../weak-field-approximation.md) and at small spatial [speed](../../../../speed.md) compared with $c$, the leading spatial [geodesic equation](../../../../geodesic-equation.md) is

$$
\boxed{\frac{d^2x^i}{d\tau^2}+c^2\Gamma^i_{00}\left(\frac{dt}{d\tau}\right)^2\simeq0.}
$$

It is exact at the release event when all spatial $u^i$ vanish, and is the intended approximation to the displayed expression in the source. Terms $2\Gamma^\mu_{0j}u^0u^j$ and $\Gamma^\mu_{ij}u^iu^j$ cannot generally be dropped; the time component must also be retained to find changing $dt/d\tau$. For a concrete counterexample to the unrestricted expression, a straight free trajectory $x=v\gamma\tau$, $y=b$ in flat [spacetime](../../../../spacetime.md) has polar radius $r=\sqrt{b^2+v^2\gamma^2\tau^2}$ and $d^2r/d\tau^2=v^2\gamma^2b^2/r^3\ne0$, although $\Gamma^r_{00}=0$. The missing angular term $\Gamma^r_{\phi\phi}(d\phi/d\tau)^2$ supplies that radial coordinate [acceleration](../../../../acceleration.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
