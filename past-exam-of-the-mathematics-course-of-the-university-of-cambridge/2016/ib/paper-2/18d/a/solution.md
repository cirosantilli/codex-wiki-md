<h1 id="18d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use SI units and the [Minkowski metric](../../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(1,-1,-1,-1)$. Write $x^\mu=(ct,x,y,z)$, $\partial_\mu=(c^{-1}\partial_t,\nabla)$ and the [four-current](../../../../../../four-current.md) $J^\mu=(c\rho,\boldsymbol J)$, with Greek indices from $0$ to $3$. The [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) is the antisymmetric tensor whose components are

$$
F^{0i}=-E_i/c,\qquad F^{i0}=E_i/c,\qquad F^{ij}=-\epsilon_{ijk}B_k.
$$

Indices are raised and lowered with $\eta$. Define the [dual electromagnetic field tensor](../../../../../../dual-electromagnetic-field-tensor.md) by $\widetilde F^{\mu\nu}=\tfrac12\epsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}$, with $\epsilon^{0123}=+1$. Then **the covariant [Maxwell equations](../../../../../../maxwell-equations.md) are**

$$
\boxed{\partial_\mu F^{\mu\nu}=\mu_0J^\nu,\qquad
\partial_\mu\widetilde F^{\mu\nu}=0.}
$$

Here $\rho$ and $\boldsymbol J$ are charge and current density, $\mu_0$ is the vacuum [magnetic permeability](../../../../../../permeability-electromagnetism.md), and $\epsilon_0\mu_0c^2=1$. For example the $\nu=0$ equation gives $\nabla\cdot\boldsymbol E=\rho/\epsilon_0$, and the spatial equations give $\nabla\times\boldsymbol B-c^{-2}\partial_t\boldsymbol E=\mu_0\boldsymbol J$. With the stated dual convention, $\widetilde F^{0i}=-B_i$ and $\widetilde F^{ij}=\epsilon_{ijk}E_k/c$; the second tensor equation gives the two homogeneous [Maxwell equations](../../../../../../maxwell-equations.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
