<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use geometric units $G=c=1$, [metric signature](../../../../../../metric-signature.md) $(-+++)$, and a [four-velocity](../../../../../../four-velocity.md) normalized by the physical metric. Write $\phi=1+\Phi$, where $|\Phi|\ll1$. For a pressureless [perfect fluid](../../../../../../perfect-fluid.md), the [dust stress-energy tensor](../../../../../../dust-stress-energy-tensor.md) is $T_{ij}=\rho U_iU_j$ and $g^{ij}U_iU_j=-1$. Since $\eta^{ij}=\phi^2g^{ij}$, its background trace is

$$
\eta^{ij}T_{ij}=-\rho\phi^2.
$$

Consequently the field equation is $(-\partial_t^2+\Delta)\phi=4\pi\rho\phi^3$. Neglecting time derivatives and higher weak-field orders gives the [Newtonian limit of Nordstrom gravity](../../../../../../newtonian-limit-of-nordstrom-gravity.md):

$$
\boxed{\Delta\Phi=4\pi\rho,\qquad\Phi=\phi-1.}
$$

The constant shift between $\phi$ and $\Phi$ does not affect the [Poisson equation](../../../../../../poisson-equation.md) or the force. Here $\rho$ is the physical rest density; if fluid indices are instead defined using the background metric, the intermediate powers of $\phi$ change but the same leading-order equation results.

For the motion, the [Levi-Civita connection](../../../../../../levi-civita-connection.md) of the [conformally flat metric](../../../../../../conformally-flat-metric.md) is

$$
\Gamma^i{}_{jk}=\delta^i_j\partial_k\log\phi+\delta^i_k\partial_j\log\phi-\eta_{jk}\eta^{i\ell}\partial_\ell\log\phi.
$$

In particular $\Gamma^\alpha{}_{00}=\partial_\alpha\log\phi$. Replacing the [affine parameter](../../../../../../affine-parameter.md) in the [geodesic equation](../../../../../../geodesic-equation.md) by coordinate time gives, with $w^i=(1,\boldsymbol v)$ and $\boldsymbol v=d\boldsymbol x/dt$,

$$
\frac{d^2x^\alpha}{dt^2}=-\Gamma^\alpha{}_{ij}w^iw^j+\Gamma^0{}_{ij}w^iw^jv^\alpha
=-(1-|\boldsymbol v|^2)\left(\partial_\alpha\log\phi+v^\alpha\partial_t\log\phi\right).
$$

At small speeds and for a nearly static field, this becomes

$$
\boxed{\frac{d^2\boldsymbol x}{dt^2}=-\boldsymbol\nabla\Phi.}
$$

Thus the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) and freely falling trajectories agree to the stated weak-field, slow-motion order. The comparison is an approximation, not an exact equivalence of relativistic trajectories.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
