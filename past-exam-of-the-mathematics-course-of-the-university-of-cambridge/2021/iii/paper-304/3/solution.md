<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Renormalization introduces an arbitrary [renormalization scale](../../../../../renormalization-scale.md) $\mu$ even though the classical massless theory has no dimensionful parameter. Independence of the bare correlation function from that auxiliary scale gives the [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md)

$$
\left(\mu\frac{\partial}{\partial\mu}+\beta(g)\frac{\partial}{\partial g}+n\gamma(g)\right)G^{(n)}=0.
$$

Here

$$
\beta(g)=\mu\frac{dg}{d\mu}\bigg|_{g_0}
$$

is the [beta function](../../../../../beta-function-physics.md) and $\gamma(g)$ is the field [anomalous dimension](../../../../../anomalous-dimension.md), with its sign fixed by the displayed equation. The beta function determines the [running coupling](../../../../../running-coupling.md). Its zeros are [renormalization-group fixed points](../../../../../renormalization-group-fixed-point.md), where the theory can become scale invariant. A positive beta function makes a positive coupling increase toward larger $\mu$, while a negative one makes it decrease.

For the propagator coefficient $C$, follow a characteristic with $t=\log(\mu/\mu_0)$ and $dg/dt=\beta(g)$. The $n=2$ equation becomes

$$
\frac{d\log C}{dt}=-2\gamma(g(t)).
$$

Integration gives

$$
\boxed{C\left(\frac{p^2}{\mu^2},g(\mu)\right)
=f(\mu)C\left(\frac{p^2}{\mu_0^2},g(\mu_0)\right)},
$$

with

$$
\boxed{f(\mu)=e^{h(\mu)},
\qquad h(\mu)=-2\int_{g(\mu_0)}^{g(\mu)}\frac{\gamma(g)}{\beta(g)}\,dg}.
$$

For $\beta(g)=-bg^3$ with $b>0$, the only real fixed point is $g^*=0$. It is ultraviolet-attractive: the theory is [asymptotically free](../../../../../asymptotic-freedom.md). Integrating the running equation gives

$$
\frac1{g^2(\mu)}=\frac1{g^2(\mu_0)}+2b\log\frac\mu{\mu_0},
$$

or

$$
\boxed{g(\mu)=\frac{g(\mu_0)}
{\sqrt{1+2bg^2(\mu_0)\log(\mu/\mu_0)}}}
$$

for the branch with the same sign as $g(\mu_0)$. The perturbative expression has an infrared [Landau pole](../../../../../landau-pole.md) at

$$
\Lambda=\mu_0\exp\left[-\frac1{2bg^2(\mu_0)}\right],
$$

and therefore

$$
\boxed{g^2(\mu)=\frac1{2b\log(\mu/\Lambda)}}.
$$

Finally set $\mu_0=p$ and use $\gamma(g)=cg^2$. The characteristic factor becomes

$$
\frac{C(p^2/\mu^2,g(\mu))}{C(1,g(p))}
=\exp\left[-2\int_{g(p)}^{g(\mu)}\frac{cg^2}{-bg^3}\,dg\right]
=\left(\frac{g(\mu)}{g(p)}\right)^{2c/b}.
$$

In terms of the dynamically generated scale,

$$
\boxed{\frac{C(p^2/\mu^2,g(\mu))}{C(1,g(p))}
=\left[\frac{\log(p/\Lambda)}{\log(\mu/\Lambda)}\right]^{c/b}}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
