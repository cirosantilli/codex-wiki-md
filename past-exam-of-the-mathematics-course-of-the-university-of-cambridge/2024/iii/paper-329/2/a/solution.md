<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For two body-force-free [Stokes flows](../../../../../../stokes-flow-split.md) $(\mathbf u^{(1)},\boldsymbol\sigma^{(1)})$ and $(\mathbf u^{(2)},\boldsymbol\sigma^{(2)})$ in the same domain, the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) is

$$
\int_{\partial\mathcal D}
\mathbf u^{(1)}\mathbin\cdot\boldsymbol\sigma^{(2)}\mathbf n\,dS
=
\int_{\partial\mathcal D}
\mathbf u^{(2)}\mathbin\cdot\boldsymbol\sigma^{(1)}\mathbf n\,dS.
$$

Indeed, the difference of the two volume integrands is

$$
\nabla\mathbf u^{(1)}:\boldsymbol\sigma^{(2)}
-\nabla\mathbf u^{(2)}:\boldsymbol\sigma^{(1)}=0
$$

because both flows are incompressible and the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) is symmetric. The [divergence theorem](../../../../../../divergence-theorem.md) proves the boundary identity.

On a rigid body, $\mathbf u^{(r)}=\mathbf U^{(r)}+\boldsymbol\Omega^{(r)}\times\mathbf x$. The reciprocal theorem becomes

$$
\mathbf U^{(1)}\mathbin\cdot\mathbf F^{(2)}
+\boldsymbol\Omega^{(1)}\mathbin\cdot\mathbf G^{(2)}
=
\mathbf U^{(2)}\mathbin\cdot\mathbf F^{(1)}
+\boldsymbol\Omega^{(2)}\mathbin\cdot\mathbf G^{(1)}.
$$

Writing $(\mathbf F,\mathbf G)^T=\mathsf R(\mathbf U,\boldsymbol\Omega)^T$ and choosing arbitrary pairs of rigid velocities shows that

$$
\boxed{\mathsf R=\mathsf R^T}.
$$

**Thus the [hydrodynamic resistance matrix](../../../../../../hydrodynamic-resistance-matrix.md) is symmetric.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
