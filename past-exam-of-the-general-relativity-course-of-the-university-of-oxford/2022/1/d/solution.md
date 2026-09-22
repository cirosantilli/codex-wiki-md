<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $x^0=ct$ and [metric signature](../../../../metric-signature.md) $(-,+,+,+)$. With the source's [curvature sign convention](../../../../curvature-sign-convention.md), the [Ricci tensor](../../../../ricci-tensor.md) is

$$
\begin{aligned}
R_{\mu\nu}&=-R^\lambda{}_{\mu\nu\lambda}\\
&=\partial_\nu\Gamma^\lambda_{\mu\lambda}
-\partial_\lambda\Gamma^\lambda_{\mu\nu}
+\Gamma^\sigma_{\mu\lambda}\Gamma^\lambda_{\nu\sigma}
-\Gamma^\sigma_{\mu\nu}\Gamma^\lambda_{\sigma\lambda}.
\end{aligned}
$$

Its time-time component is therefore

$$
R_{00}=\partial_0\Gamma^\lambda_{0\lambda}
-\partial_\lambda\Gamma^\lambda_{00}
+\Gamma^\sigma_{0\lambda}\Gamma^\lambda_{0\sigma}
-\Gamma^\sigma_{00}\Gamma^\lambda_{\sigma\lambda}.
$$

For a slowly moving, pressure-negligible source, the [stress-energy tensor](../../../../stress-energy-tensor-split.md) is approximated by [relativistic dust](../../../../relativistic-dust.md): $T^{\mu\nu}=\rho U^\mu U^\nu$, where $\rho$ is [mass density](../../../../density.md) and $U^\mu$ is the [four-velocity](../../../../four-velocity.md). In its approximate rest [local inertial frame](../../../../local-inertial-frame.md), $U^\mu\simeq(c,0,0,0)$ and $U_0\simeq-c$. Thus

$$
T_{00}\simeq\rho c^2,\qquad T_{ij}\ll T_{00},\qquad
T\simeq-\rho c^2,
$$

and the [trace-reversed stress-energy tensor](../../../../trace-reversed-stress-energy-tensor.md) satisfies

$$
S_{00}=T_{00}-\frac12g_{00}T\simeq\frac12\rho c^2.
\qquad\boxed{R_{00}\simeq\frac12C\rho c^2.}
$$

Independently, introduce the [metric perturbation](../../../../linearized-gravity-split.md) $g_{\mu\nu}=\eta_{\mu\nu}+h_{\mu\nu}$, with $|h_{\mu\nu}|\ll1$ and constant [Minkowski metric](../../../../minkowski-metric.md) $\eta_{\mu\nu}$. The [Christoffel symbols](../../../../christoffel-symbol.md) are first order in $h$, so their products are discarded in the [weak-field approximation](../../../../weak-field-approximation.md). With a comma denoting a [partial derivative](../../../../partial-derivative.md), the linearized [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) is

$$
R_{\lambda\mu\nu\kappa}
=\frac12\left(h_{\lambda\nu,\kappa\mu}
-h_{\mu\nu,\kappa\lambda}
-h_{\lambda\kappa,\nu\mu}
+h_{\mu\kappa,\nu\lambda}\right)+O(h^2).
$$

Taking the [tensor contraction](../../../../tensor-contraction.md) gives, to this order,

$$
R_{00}=\sum_{i=1}^3R_{i0i0}
=\frac12\sum_{i=1}^3\left(\partial_0^2h_{ii}
-2\partial_0\partial_i h_{0i}+\partial_i^2h_{00}\right).
$$

In the static [Newtonian limit](../../../../newtonian-limit.md), all time [partial derivatives](../../../../partial-derivative.md) vanish. The constant $\eta_{00}$ also has zero [partial derivatives](../../../../partial-derivative.md), leaving

$$
\boxed{R_{00}\simeq\frac12\nabla^2h_{00}
=\frac12\nabla^2g_{00}.}
$$

Here $\nabla^2=\sum_i\partial_i^2$ is the spatial [Laplace operator](../../../../laplace-operator.md) in the approximately Cartesian background coordinates. This sign follows the paper's [curvature sign convention](../../../../curvature-sign-convention.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
