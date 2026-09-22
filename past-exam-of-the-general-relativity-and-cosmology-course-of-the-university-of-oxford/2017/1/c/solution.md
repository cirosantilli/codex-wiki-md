<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [relativistic dust](../../../../relativistic-dust.md), $T^{\alpha\beta}=\rho u^\alpha u^\beta$, with $u^\alpha u_\alpha=-c^2$. Expanding [stress-energy conservation](../../../../stress-energy-conservation.md) gives

$$
0=\nabla_\alpha(\rho u^\alpha u^\beta)
=u^\beta\nabla_\alpha(\rho u^\alpha)
+\rho u^\alpha\nabla_\alpha u^\beta.
$$

Contract with $u_\beta$. [Metric compatibility](../../../../metric-compatibility.md) and the fixed normalization imply

$$
u_\beta u^\alpha\nabla_\alpha u^\beta
=\frac12u^\alpha\nabla_\alpha(u_\beta u^\beta)=0.
$$

Consequently

$$
-c^2\nabla_\alpha(\rho u^\alpha)=0.
$$

This is the covariant [mass conservation](../../../../mass-conservation.md) equation. Substituting it back, wherever $\rho>0$, gives

$$
\boxed{u^\alpha\nabla_\alpha u^\beta=0.}
$$

Thus the dust's fluid elements follow [timelike geodesics](../../../../timelike-geodesic.md). With $u^\alpha=dx^\alpha/d\tau$, the [proper time](../../../../proper-time.md) $\tau$ is an [affine parameter](../../../../affine-parameter.md), and explicitly

$$
\frac{d^2x^\beta}{d\tau^2}
+\Gamma^\beta{}_{\alpha\gamma}
\frac{dx^\alpha}{d\tau}\frac{dx^\gamma}{d\tau}=0.
$$

The absence of [pressure](../../../../pressure-split.md) removes the force produced by pressure gradients; gravity is encoded by the [Levi-Civita connection](../../../../levi-civita-connection.md). At a point with $\rho=0$ this calculation makes no claim about a fluid velocity.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
