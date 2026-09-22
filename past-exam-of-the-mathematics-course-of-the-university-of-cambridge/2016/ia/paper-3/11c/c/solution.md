<h1 id="11c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The identity [divergence of a curl is zero](../../../../../../divergence-of-a-curl-is-zero.md) follows by the symmetry of second [partial derivatives](../../../../../../partial-derivative.md) and antisymmetry of the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md). Therefore

$$
\boxed{\nabla\cdot\mathbf J=\nabla\cdot(\nabla\times\mathbf B)=0.}
$$

If $\mathbf B=\nabla\times\mathbf A$ and $\mathbf A$ is in [Coulomb gauge](../../../../../../coulomb-gauge.md), the [curl of the curl identity](../../../../../../curl-of-the-curl-identity.md) gives $\mathbf J=-\nabla^2\mathbf A$. Apply the supplied scalar [Poisson equation](../../../../../../poisson-equation.md) representation to each component of the decaying [vector potential](../../../../../../vector-potential.md). In the units of this problem the [Coulomb-gauge vector potential of a localized steady current](../../../../../../coulomb-gauge-vector-potential-of-a-localized-steady-current.md) is

$$
\boxed{\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf y)}{4\pi|\mathbf x-\mathbf y|}\,d^3y.}
$$

Here one needs $\mathbf A=O(|\mathbf x|^{-1})$, $\nabla\mathbf A=O(|\mathbf x|^{-2})$ and enough localization of $\mathbf J$ for the stated representation and differentiations. A smooth compactly supported [current density](../../../../../../current-density.md) is a sufficient convenient case. The local differential equations and gauge alone do not impose these conditions: $\mathbf A=(-y,x,0)$, $\mathbf B=(0,0,2)$, $\mathbf J=0$ satisfy them but do not satisfy the displayed integral formula. The formula selects the decaying solution, excluding nondecaying homogeneous [harmonic functions](../../../../../../harmonic-function.md).

With $\mathbf r=\mathbf x-\mathbf y$, the [gradient](../../../../../../gradient.md) of the kernel is $\nabla_x(1/|\mathbf r|)=-\mathbf r/|\mathbf r|^3$. Since $\mathbf J(\mathbf y)$ is independent of $\mathbf x$,

$$
\nabla_x\times\left(\frac{\mathbf J(\mathbf y)}{4\pi|\mathbf r|}\right)=\frac{\mathbf J(\mathbf y)\times\mathbf r}{4\pi|\mathbf r|^3}.
$$

Thus **taking the [curl](../../../../../../curl.md) gives the [Biot-Savart law](../../../../../../biot-savart-law.md) in the problem's normalization**:

$$
\boxed{\mathbf B(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf y)\times(\mathbf x-\mathbf y)}{4\pi|\mathbf x-\mathbf y|^3}\,d^3y.}
$$

Finally, change variables $\mathbf z=\mathbf x-\mathbf y$ in the integral for $\mathbf A$. This keeps the singular kernel independent of the differentiation variable:

$$
\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf x-\mathbf z)}{4\pi|\mathbf z|}\,d^3z,\qquad\nabla\cdot\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{(\nabla\cdot\mathbf J)(\mathbf x-\mathbf z)}{4\pi|\mathbf z|}\,d^3z=0.
$$

For smooth localized $\mathbf J$, [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) is legitimate: $1/|\mathbf z|$ is locally integrable in three dimensions, and on a bounded neighbourhood of $\mathbf x$ the translated sources and their derivatives have common compact support. **The integral indeed satisfies [Coulomb gauge](../../../../../../coulomb-gauge.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
