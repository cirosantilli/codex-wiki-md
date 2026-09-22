<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Vary the [geodesic Lagrangian](../../../../../../geodesic-lagrangian.md) before imposing the normalization of [proper time](../../../../../../proper-time.md). With $u^\mu=dx^\mu/d\tau$,

$$
\frac{\partial L}{\partial u^\alpha}=-2g_{\alpha\nu}u^\nu,\qquad
\frac{\partial L}{\partial x^\alpha}=-\partial_\alpha g_{\mu\nu}u^\mu u^\nu.
$$

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is

$$
g_{\alpha\nu}\frac{du^\nu}{d\tau}
+\partial_\rho g_{\alpha\nu}u^\rho u^\nu
-\frac12\partial_\alpha g_{\mu\nu}u^\mu u^\nu=0,
$$

equivalently the affinely parametrized [geodesic equation](../../../../../../geodesic-equation.md). For the static weak metric, its leading spatial connection coefficient is

$$
\Gamma^i{}_{00}=-\frac12g^{ij}\partial_jg_{00}
=\frac{\partial_i\Phi}{1-2\Phi}\simeq\partial_i\Phi.
$$

All terms with two spatial velocities are suppressed by $v^2$. Therefore $d^2x^i/d\tau^2\simeq-\partial_i\Phi\,(dt/d\tau)^2$.

Because $t$ is cyclic, the same [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) gives $(1+2\Phi)\,dt/d\tau=\text{constant}$. On converting to coordinate time, the additional term $(d^2t/d\tau^2)(dx^i/dt)$ is of order $v^2\nabla\Phi$ and can be dropped. Hence

$$
\boxed{\frac{d^2\mathbf x}{dt^2}=-\nabla\Phi}
$$

to leading order, the [Newtonian limit of general relativity](../../../../../../newtonian-limit.md). Restoring SI units gives $\Phi=\Phi_{\rm SI}/c^2$, so the acceleration is $-\nabla(c^2\Phi)$. **Substituting $L=1$ from proper-time normalization before varying would incorrectly erase the dynamics**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
