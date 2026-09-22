<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) with no magnetic or gravitational force. Let $w$ denote [specific enthalpy](../../../../../../specific-enthalpy.md). For a [homentropic flow](../../../../../../homentropic-flow.md), $dw=dp/\rho$, so the pressure acceleration is $-\nabla w$. The velocity identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla\frac{u^2}{2}-\mathbf u\times\boldsymbol\omega,\qquad\boldsymbol\omega=\nabla\times\mathbf u,
$$

therefore gives

$$
\partial_t\mathbf u=\mathbf u\times\boldsymbol\omega-\nabla\mathcal B,\qquad\mathcal B=w+\frac{u^2}{2}.
$$

Taking the [curl](../../../../../../curl.md), using that the curl of a [gradient](../../../../../../gradient.md) is zero and that differentiation commutes for smooth fields, proves [barotropic vorticity transport](../../../../../../barotropic-vorticity-transport.md):

$$
\boxed{\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega).}
$$

More generally the same proof works for any [barotropic fluid](../../../../../../barotropic-fluid.md), replacing $w$ by a pressure potential $\int^\rho p'(s)\,ds/s$. Here “isentropic” must supply this barotropic closure, for example through one common [specific entropy](../../../../../../specific-entropy.md) throughout the fluid. Merely imposing [entropy advection equation](../../../../../../entropy-advection-equation.md) $Ds/Dt=0$ allows spatial [specific entropy](../../../../../../specific-entropy.md) gradients; in that case the [vorticity equation](../../../../../../vorticity-equation.md) contains the additional [baroclinic vorticity generation](../../../../../../baroclinic-vorticity-generation.md) term $\rho^{-2}\nabla\rho\times\nabla p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
