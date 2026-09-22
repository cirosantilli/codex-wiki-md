<h1 id="35a/solution">Solution</h1>

↑ **Parent:** [35A](../35a.md)

For a scalar, $\nabla_a\phi=\partial_a\phi$, while its second [covariant derivative](../../../../../covariant-derivative.md) is $\nabla_a\nabla_b\phi=\partial_a\partial_b\phi-\Gamma^c_{ab}\partial_c\phi$. [Partial derivatives](../../../../../partial-derivative.md) commute and the [Levi-Civita connection](../../../../../levi-civita-connection.md) is torsion-free, $\Gamma^c_{ab}=\Gamma^c_{ba}$, proving the asserted symmetry.

Write the [Einstein equation](../../../../../einstein-field-equations.md) without [cosmological constant](../../../../../cosmological-constant.md) as $G_{ab}=\kappa T_{ab}$, $\kappa=8\pi G/c^4$. Tracing the given Ricci equation gives $R=g^{ab}\partial_a\phi\partial_b\phi$. Hence

$$
\boxed{T_{ab}=\kappa^{-1}\left(\partial_a\phi\partial_b\phi-\frac12g_{ab}\partial_c\phi\partial^c\phi\right).}
$$

In units $\kappa=1$ the prefactor is absent. [Metric compatibility](../../../../../metric-compatibility.md), the product rule and the just-proved [symmetric Hessian of a scalar field](../../../../../symmetric-hessian-of-a-scalar-field.md) give

$$
\kappa\nabla^aT_{ab}=(\nabla^a\nabla_a\phi)\partial_b\phi+\partial^a\phi\nabla_a\partial_b\phi-\partial^a\phi\nabla_b\partial_a\phi=(\nabla^a\nabla_a\phi)\partial_b\phi.
$$

The contracted [Bianchi identity](../../../../../bianchi-identity.md) makes the left side zero. Wherever the gradient covector is nonzero, at least one component is nonzero, forcing **$\nabla_a\nabla^a\phi=0$**, even when that gradient is null.

Finally $\Gamma^a_{ab}=\partial_b\log\sqrt{-g}$, obtained by differentiating the metric [determinant](../../../../../determinant.md). Thus for any vector $V$, $\nabla_aV^a=(\sqrt{-g})^{-1}\partial_a(\sqrt{-g}V^a)$. Applying it to $V^a=g^{ab}\partial_b\phi$ proves

$$
\boxed{\partial_a(\sqrt{-g}\,g^{ab}\partial_b\phi)=0.}
$$

## ↑ Ancestors (10)

1. [35A](../35a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
