<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For any closed surface enclosing a region $V$, [Gauss's law for gravity](../../../../../../gauss-s-law-for-gravity.md) states that the outward [flux](../../../../../../flux.md) of the [gravitational field](../../../../../../gravitational-field.md) is

$$
\boxed{\iint_{\partial V}\mathbf g\cdot\mathbf n\,dA=-4\pi G\iiint_V\rho\,dV=-4\pi GM_V.}
$$

Here $G$ is the [gravitational constant](../../../../../../gravitational-constant.md) and $M_V$ is the enclosed [mass](../../../../../../mass.md); the negative sign expresses attractive [gravity](../../../../../../gravity.md).

Use the [gravitational potential sign conventions](../../../../../../gravitational-potential-sign-conventions.md) specified by this paper: $\mathbf g=\nabla\varphi$. Thus $\varphi$ is the negative of the usual [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) $\Phi$ defined by $\mathbf g=-\nabla\Phi$. For example, setting the value at infinity to zero gives $\varphi=GM/r$ for a [point mass](../../../../../../point-mass.md). The [divergence theorem](../../../../../../divergence-theorem.md) now gives

$$
\iiint_V\nabla^2\varphi\,dV=-4\pi G\iiint_V\rho\,dV.
$$

Since $V$ is arbitrary, continuity of the integrands implies the local [Poisson's equation](../../../../../../poisson-s-equation.md)

$$
\boxed{\nabla^2\varphi=-4\pi G\rho.}
$$

Conversely, integrating this [Poisson's equation](../../../../../../poisson-s-equation.md) over any $V$ and applying the [divergence theorem](../../../../../../divergence-theorem.md) recovers [Gauss's law for gravity](../../../../../../gauss-s-law-for-gravity.md). At a discontinuity of the [mass density](../../../../../../density.md), the local equation is interpreted piecewise, or globally in the sense of [distributions](../../../../../../distribution-mathematical-analysis.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
