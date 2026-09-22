<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [torsion-free connection](../../../../torsion-free-connection.md), the connection terms in the antisymmetrized [covariant derivative](../../../../covariant-derivative.md) cancel: $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu$. Thus the [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) is the [exterior derivative](../../../../exterior-derivative.md) of the [four-potential](../../../../electromagnetic-four-potential.md). It is a [tensor](../../../../tensor.md), is invariant under $A_\mu\mapsto A_\mu+\partial_\mu\chi$, and obeys the homogeneous [Maxwell equations](../../../../maxwell-equations-split.md) $\nabla_{[\alpha}F_{\beta\gamma]}=0$. The covariant divergence equation is the generally covariant form of the local source equation; use its minus sign as specified in the paper.

Expand that equation before imposing the [Lorenz gauge condition](../../../../lorenz-gauge-condition.md):

$$
\nabla^\mu F_{\mu\nu}=\nabla^\mu\nabla_\mu A_\nu-\nabla^\mu\nabla_\nu A_\mu.
$$

The [curvature commutator on a covariant tensor](../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
[\nabla_\rho,\nabla_\nu]A_\mu=-R^\alpha{}_{\mu\rho\nu}A_\alpha,
\qquad
\nabla^\mu\nabla_\nu A_\mu=\nabla_\nu(\nabla^\mu A_\mu)+R^\alpha{}_\nu A_\alpha.
$$

Here the contraction $g^{\mu\rho}R^\alpha{}_{\mu\rho\nu}=-R^\alpha{}_\nu$ accounts for the second sign reversal. Hence in [Lorenz gauge](../../../../lorenz-gauge-condition.md)

$$
\boxed{\nabla^\mu\nabla_\mu A_\nu-R^\alpha{}_\nu A_\alpha=-\mu_0J_\nu.}
$$

This [curved-spacetime electromagnetic potential wave equation](../../../../curved-spacetime-electromagnetic-potential-wave-equation.md) contains a [Ricci tensor](../../../../ricci-tensor.md) term even in a locally inertial coordinate system: a connection can vanish at one point while its derivatives and [curvature](../../../../curvature.md) remain nonzero.

## ↑ Ancestors (12)

1. [B](../b.md)
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
