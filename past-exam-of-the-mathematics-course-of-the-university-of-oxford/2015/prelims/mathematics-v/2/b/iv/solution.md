<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** Two applications of [Green's identities](../../../../../../../green-s-identities.md), or two [integrations by parts](../../../../../../../integration-by-parts.md), give

$$
\iiint_Vu\Delta^2u\,dV
=\iiint_V(\Delta u)^2\,dV
+\iint_{\partial V}\bigl(u\partial_n\Delta u-\Delta u\partial_nu\bigr)\,dS.
$$

The [biharmonic equation](../../../../../../../biharmonic-equation.md) makes the left side zero, while the two [clamped boundary conditions](../../../../../../../clamped-boundary-condition.md) $u=\partial_nu=0$ annihilate the [boundary integral](../../../../../../../boundary-integral.md). Consequently

$$
\iiint_V(\Delta u)^2\,dV=0,
$$

so $\Delta u=0$. Apply the first of [Green's identities](../../../../../../../green-s-identities.md) once more with $\phi=\psi=u$: because $u=0$ on the [boundary](../../../../../../../boundary-of-a-set.md), it gives $\int_V|\nabla u|^2=0$. By [path connectedness](../../../../../../../path-connected-space.md), $u$ is constant, and the zero [boundary value](../../../../../../../boundary-value.md) implies $\boxed{u=0}$. This argument assumes the classical differentiability needed for the displayed [integrations by parts](../../../../../../../integration-by-parts.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
