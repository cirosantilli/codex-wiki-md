<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A semicolon denotes the [covariant derivative](../../../../covariant-derivative.md) for the [Levi-Civita connection](../../../../levi-civita-connection.md). For example, the four lower indices of the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) contribute four connection terms:

$$
\begin{aligned}
R_{\lambda\mu\nu\kappa;\eta}
={}&\partial_\eta R_{\lambda\mu\nu\kappa}
-\Gamma^a_{\lambda\eta}R_{a\mu\nu\kappa}
-\Gamma^a_{\mu\eta}R_{\lambda a\nu\kappa}\\
&-\Gamma^a_{\nu\eta}R_{\lambda\mu a\kappa}
-\Gamma^a_{\kappa\eta}R_{\lambda\mu\nu a}.
\end{aligned}
$$

Here $\partial_\eta=\partial/\partial x^\eta$ is a [partial derivative](../../../../partial-derivative.md), $\Gamma^a_{b\eta}$ are [Christoffel symbols](../../../../christoffel-symbol.md), and repeated indices are summed from $0$ to $3$. Write $g_{\mu\nu}$ for the [metric tensor](../../../../metric-tensor.md), $g^{\mu\nu}$ for its [inverse metric](../../../../inverse-metric.md), $R_{\mu\nu}=g^{\lambda\nu'}R_{\lambda\mu\nu'\nu}$ for the [Ricci tensor](../../../../ricci-tensor.md), and $R=g^{\mu\nu}R_{\mu\nu}$ for the [Ricci scalar](../../../../ricci-scalar.md). This [tensor contraction](../../../../tensor-contraction.md) agrees with the paper's $R_{\mu\nu}=-R^a{}_{\mu\nu a}$.

By [metric compatibility](../../../../metric-compatibility.md), the [inverse metric](../../../../inverse-metric.md) may pass through each [covariant derivative](../../../../covariant-derivative.md). Contracting the [second Bianchi identity](../../../../second-bianchi-identity.md) with $g^{\lambda\nu}$ gives

$$
\nabla_\eta R_{\mu\kappa}-\nabla_\kappa R_{\mu\eta}
+\nabla^\lambda R_{\lambda\mu\kappa\eta}=0,
$$

where $\nabla_\eta$ is the same [covariant derivative](../../../../covariant-derivative.md) as the semicolon. Next contract with $g^{\mu\kappa}$. Antisymmetry of the first pair gives $g^{\mu\kappa}R_{\lambda\mu\kappa\eta}=-R_{\lambda\eta}$, so

$$
\partial_\eta R-\nabla^\mu R_{\mu\eta}-\nabla^\lambda R_{\lambda\eta}=0.
$$

Thus the [contracted Bianchi identity](../../../../contracted-bianchi-identity.md) is $\nabla^\mu R_{\mu\eta}=\tfrac12\partial_\eta R$. Raising the remaining index and using [metric compatibility](../../../../metric-compatibility.md) proves

$$
\boxed{\nabla_\mu G^{\mu\nu}=0,\qquad
G^{\mu\nu}=R^{\mu\nu}-\tfrac12g^{\mu\nu}R.}
$$

The [Einstein tensor](../../../../einstein-tensor.md) $G^{\mu\nu}$ therefore has identically zero [covariant divergence](../../../../covariant-divergence.md), without imposing any field equation. This makes the [Einstein field equations](../../../../einstein-field-equations-split.md) compatible with [stress-energy conservation](../../../../stress-energy-conservation.md), $\nabla_\mu T^{\mu\nu}=0$, where $T^{\mu\nu}$ is the [stress-energy tensor](../../../../stress-energy-tensor-split.md). The connection terms describe how [energy](../../../../energy-split.md) and [momentum](../../../../momentum-split.md) are compared at neighboring points; ordinary componentwise [partial derivatives](../../../../partial-derivative.md) would not give a coordinate-independent conservation law in curved [spacetime](../../../../spacetime.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
