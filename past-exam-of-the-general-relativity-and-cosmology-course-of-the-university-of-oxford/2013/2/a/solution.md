<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Although $\nabla_\beta f=\partial_\beta f$ for a [scalar field](../../../../scalar-field.md), its first derivative is a [covector field](../../../../one-form.md). Therefore

$$
\nabla_\alpha\nabla_\beta f=\partial_\alpha\partial_\beta f-\Gamma^\gamma{}_{\alpha\beta}\partial_\gamma f.
$$

Commuting [partial derivatives](../../../../partial-derivative.md) and using the [torsion-free connection](../../../../torsion-free-connection.md) gives $\boxed{[\nabla_\alpha,\nabla_\beta]f=0}$. For a [vector field](../../../../vector-field.md), differentiate the $(1,1)$ [tensor](../../../../tensor.md) $\nabla_\beta V^\mu$ with both its indices included:

$$
\nabla_\alpha\nabla_\beta V^\mu
=\partial_\alpha(\nabla_\beta V^\mu)+\Gamma^\mu{}_{\alpha\epsilon}\nabla_\beta V^\epsilon
-\Gamma^\epsilon{}_{\alpha\beta}\nabla_\epsilon V^\mu.
$$

Subtract the expression with $\alpha,\beta$ exchanged. Second derivatives of $V$ cancel; the terms multiplying first derivatives cancel pairwise, and the final lower-index connection terms cancel by symmetry. The remaining coefficient of $V^\nu$ is

$$
\boxed{[\nabla_\alpha,\nabla_\beta]V^\mu=
\left(\partial_\alpha\Gamma^\mu{}_{\beta\nu}-\partial_\beta\Gamma^\mu{}_{\alpha\nu}
+\Gamma^\mu{}_{\alpha\epsilon}\Gamma^\epsilon{}_{\beta\nu}-\Gamma^\mu{}_{\beta\epsilon}\Gamma^\epsilon{}_{\alpha\nu}\right)V^\nu
=R^\mu{}_{\nu\alpha\beta}V^\nu.}
$$

This is the [curvature commutator](../../../../commutator-of-covariant-derivatives.md). On a covariant index the sign reverses, giving the [curvature commutator on a covariant tensor](../../../../curvature-commutator-on-a-covariant-tensor.md) used in the next part.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
