<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep only first order in the [metric perturbation](../../../../../../linearized-gravity.md) and use the [Minkowski metric](../../../../../../minkowski-metric.md) to raise and lower indices; set $G=c=1$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) has

$$
\Gamma^{\rho(1)}{}_{\mu\nu}=\frac12\eta^{\rho\sigma}(\partial_\mu h_{\sigma\nu}+\partial_\nu h_{\sigma\mu}-\partial_\sigma h_{\mu\nu}).
$$

The quadratic products of [Christoffel symbols](../../../../../../christoffel-symbol.md) in the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) can be dropped at this order. Contracting the remaining derivatives gives

$$
R^{(1)}_{\mu\nu}=\frac12\bigl(\partial_\rho\partial_\mu h^\rho{}_\nu+\partial_\rho\partial_\nu h^\rho{}_\mu-\Box h_{\mu\nu}-\partial_\mu\partial_\nu h\bigr),\qquad R^{(1)}=\partial_\mu\partial_\nu h^{\mu\nu}-\Box h,
$$

where $\Box=\eta^{\rho\sigma}\partial_\rho\partial_\sigma=-\partial_t^2+\nabla^2$ is the [d'Alembert operator](../../../../../../d-alembert-operator.md). In four dimensions the [trace-reversed metric perturbation](../../../../../../trace-reversed-metric-perturbation.md) satisfies $\bar h=-h$ and $h_{\mu\nu}=\bar h_{\mu\nu}-\tfrac12\eta_{\mu\nu}\bar h$. Writing the [Linearized Einstein equations](../../../../../../linearized-einstein-equations.md) in terms of it gives

$$
G^{(1)}_{\mu\nu}=\frac12\bigl(\partial_\rho\partial_\mu\bar h^\rho{}_\nu+\partial_\rho\partial_\nu\bar h^\rho{}_\mu-\Box\bar h_{\mu\nu}-\eta_{\mu\nu}\partial_\rho\partial_\sigma\bar h^{\rho\sigma}\bigr).
$$

In [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md), the first, second and fourth terms vanish. Therefore $G^{(1)}_{\mu\nu}=8\pi T_{\mu\nu}$ becomes

$$
\boxed{\Box\bar h_{\mu\nu}=-16\pi T_{\mu\nu}.}
$$

The divergence of this equation also gives $\partial^\mu T_{\mu\nu}=0$, the leading-order [stress-energy conservation](../../../../../../stress-energy-conservation.md) required by the [contracted Bianchi identity](../../../../../../contracted-bianchi-identity.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
