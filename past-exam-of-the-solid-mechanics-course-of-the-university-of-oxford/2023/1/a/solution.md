<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [first strain invariant](../../../../first-strain-invariant.md) in components of the [deformation gradient](../../../../deformation-gradient.md):

$$
I_1=\operatorname{tr}(\mathbf F\mathbf F^T)
=\sum_{i,I}F_{iI}^2.
$$

Here lower-case and upper-case indices refer to the [current configuration](../../../../current-configuration.md) and [reference configuration](../../../../reference-configuration.md), respectively. Differentiating gives $\partial I_1/\partial F_{iI}=2F_{iI}$. The [chain rule](../../../../chain-rule.md) therefore gives

$$
\frac{\partial W}{\partial F_{iI}}=2w'(I_1)F_{iI},
\qquad
\partial_{\mathbf F}W=2w'(I_1)\mathbf F.
$$

Substitution into the given [hyperelastic material](../../../../hyperelastic-material.md) law, with its indicated [matrix transpose](../../../../transpose.md), yields

$$
\boxed{\mathbf T
=\mathbf F(\partial_{\mathbf F}W)^T-p\mathbf1
=2w'(I_1)\mathbf F\mathbf F^T-p\mathbf1
=2\frac{\partial w}{\partial I_1}\mathbf B-p\mathbf1.}
$$

The [left Cauchy-Green deformation tensor](../../../../left-cauchy-green-deformation-tensor.md) is $\mathbf B=\mathbf F\mathbf F^T$. The scalar $p$ is the [Lagrange multiplier](../../../../lagrange-multiplier.md) enforcing [incompressibility](../../../../incompressible-flow.md), rather than a function fixed by the [strain energy density](../../../../strain-energy-density.md) alone. The [identity matrix](../../../../identity-matrix.md) $\mathbf1$ makes this an isotropic [constraint reaction in hyperelastic stress](../../../../constraint-reaction-in-hyperelastic-stress.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
