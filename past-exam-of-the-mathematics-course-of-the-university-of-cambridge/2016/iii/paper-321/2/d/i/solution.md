<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [polytropic equation of state](../../../../../../../polytropic-equation-of-state.md) $p=K\rho^{1+1/n}$, take $K>0$ and $n>0$ for the physical model. The [specific enthalpy](../../../../../../../specific-enthalpy.md) relative to vacuum is

$$
Q=\int_0^\rho\frac{dp(\tilde\rho)}{\tilde\rho}=(n+1)K\rho^{1/n}=\frac{(n+1)p}{\rho}.
$$

Its gradient obeys $\nabla Q=\rho^{-1}\nabla p$, so the [Euler equations](../../../../../../../euler-equations-for-an-inviscid-fluid.md) become

$$
\boxed{\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u=-\nabla Q-2\Omega\mathbf e_z\times\mathbf u-\nabla\Phi_t.}
$$

For the material derivative $D_t=\partial_t+\mathbf u\cdot\nabla$, $D_tQ=(Q/n\rho)D_t\rho$. The [continuity equation](../../../../../../../continuity-equation.md) thus becomes

$$
\boxed{nD_tQ=-Q\nabla\cdot\mathbf u.}
$$

The choice $Q=0$ at zero [mass density](../../../../../../../density.md) fixes the additive convention in this equation. Although the momentum equation alone is unchanged by adding a constant to $Q$, the polytropic relation and enthalpy evolution must use the same vacuum reference.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
