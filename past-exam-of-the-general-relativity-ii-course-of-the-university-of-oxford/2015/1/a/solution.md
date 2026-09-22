<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Killing vector field](../../../../killing-vector-field-split.md) $K$ generates local [isometries](../../../../isometry.md): its [flow of a vector field](../../../../flow-of-a-vector-field.md) $\Phi_s$ satisfies $\Phi_s^*g=g$. Equivalently, the [Lie derivative](../../../../lie-derivative-of-a-differential-form.md) of the [metric tensor](../../../../metric-tensor.md) vanishes. For the [Levi-Civita connection](../../../../levi-civita-connection.md), [metric compatibility](../../../../metric-compatibility.md) converts the coordinate expression into the [Killing equation](../../../../killing-equation.md):

$$
\boxed{\mathcal L_Kg=0,\qquad \nabla_\mu K_\nu+\nabla_\nu K_\mu=0.}
$$

**The [Levi-Civita connection](../../../../levi-civita-connection.md) is an implicit extra assumption in this question.** The printed assumption of vanishing [torsion tensor](../../../../torsion-tensor.md) alone does not imply [metric compatibility](../../../../metric-compatibility.md). For example, on [Minkowski spacetime](../../../../minkowski-spacetime.md), take the [affine connection](../../../../affine-connection.md) whose only nonzero [Christoffel symbol](../../../../christoffel-symbol.md) is $\Gamma^0{}_{00}=1$. The [vector field](../../../../vector-field.md) $K=\partial_0$ preserves the [Minkowski metric](../../../../minkowski-metric.md), but $K_0=-1$ gives $\nabla_0K_0=1$, contradicting the [Killing equation](../../../../killing-equation.md). The following calculation, and the covariant formulas in part (b), use the [Levi-Civita connection](../../../../levi-civita-connection.md); this is the role of [metric compatibility in Killing identities](../../../../metric-compatibility-in-killing-identities.md).

For the stated [curvature sign convention](../../../../curvature-sign-convention.md), the [Ricci identity](../../../../curvature-commutator-on-a-covariant-tensor.md) on a [covector](../../../../covector.md) has a minus sign:

$$
[\nabla_\mu,\nabla_\nu]K_\rho=-R^\sigma{}_{\rho\mu\nu}K_\sigma.
$$

Write $A_{\mu\nu\rho}=\nabla_\mu\nabla_\nu K_\rho$. Differentiating the [Killing equation](../../../../killing-equation.md) gives $A_{\mu\nu\rho}=-A_{\mu\rho\nu}$. Alternately using this relation and the [Ricci identity](../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
\begin{aligned}
A_{\mu\nu\rho}
&=-A_{\mu\rho\nu}
=-A_{\rho\mu\nu}+R^\sigma{}_{\nu\mu\rho}K_\sigma\\
&=A_{\rho\nu\mu}+R^\sigma{}_{\nu\mu\rho}K_\sigma\\
&=A_{\nu\rho\mu}-R^\sigma{}_{\mu\rho\nu}K_\sigma+R^\sigma{}_{\nu\mu\rho}K_\sigma\\
&=-A_{\mu\nu\rho}-R^\sigma{}_{\rho\mu\nu}K_\sigma-R^\sigma{}_{\mu\rho\nu}K_\sigma+R^\sigma{}_{\nu\mu\rho}K_\sigma.
\end{aligned}
$$

The [first Bianchi identity](../../../../first-bianchi-identity.md) and antisymmetry of the last two indices of the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) reduce the three curvature terms to $2R^\sigma{}_{\mu\nu\rho}K_\sigma$. Consequently the [second covariant derivative of a Killing vector](../../../../second-covariant-derivative-of-a-killing-vector.md) is

$$
\boxed{\nabla_\mu\nabla_\nu K_\rho=R^\sigma{}_{\mu\nu\rho}K_\sigma.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
