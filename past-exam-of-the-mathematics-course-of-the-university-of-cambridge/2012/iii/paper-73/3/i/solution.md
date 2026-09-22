<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Consider an unforced [incompressible flow](../../../../../../incompressible-flow.md) with localized [vorticity](../../../../../../vorticity.md) and sufficient smoothness for [integration by parts](../../../../../../integration-by-parts.md). Define the [hydrodynamic impulse](../../../../../../hydrodynamic-impulse.md) per unit density by $\mathbf I=\tfrac12\int\mathbf x\times\boldsymbol\omega\,dV$, denoting the vector [impulse](../../../../../../impulse.md) by $\mathbf I$ to distinguish it from the later scalar $L$. The [vorticity equation](../../../../../../vorticity-equation.md) can be written

$$
\partial_t\boldsymbol\omega=\nabla\times\mathbf F,\qquad
\mathbf F=\mathbf u\times\boldsymbol\omega-\nu\nabla\times\boldsymbol\omega.
$$

The supplied identity, integrated over all space, gives $\tfrac12\int\mathbf x\times\nabla\times\mathbf F\,dV=\int\mathbf F\,dV$, because $\mathbf F$ is localized and its surface terms vanish. Therefore

$$
\frac{d\mathbf I}{dt}=\int\mathbf u\times\boldsymbol\omega\,dV-
\nu\int\nabla\times\boldsymbol\omega\,dV.
$$

The second integral is a vanishing surface integral. The vector identity $\mathbf u\times\boldsymbol\omega=\nabla(|\mathbf u|^2/2)-(\mathbf u\cdot\nabla)\mathbf u$ and incompressibility reduce the first to surface terms proportional to the quadratic velocity. Those vanish for $\mathbf u=O(R^{-3})$. Thus

$$
\boxed{d\mathbf I/dt=0}.
$$

For a large spherical control volume define $\mathbf P_R=\int_{V_R}\mathbf u\,dV$. The [impulse](../../../../../../impulse.md) relation is $\mathbf I=(3/2)\lim_{R\to\infty}\mathbf P_R$ for this localized field. The factor is important: [impulse](../../../../../../impulse.md) is not simply the integral of velocity, since an $R^{-3}$ velocity tail has a nonvanishing contribution in the [impulse](../../../../../../impulse.md) [integration by parts](../../../../../../integration-by-parts.md) involving a factor of $R$.

Using [pressure](../../../../../../pressure.md) per unit density $\Pi$ and the Navier-Stokes equation gives

$$
\frac{d\mathbf P_R}{dt}=-\int_{\partial V_R}[\mathbf u(\mathbf u\cdot\mathbf n)+\Pi\mathbf n-\nu\partial_n\mathbf u],dA.
$$

The advective flux is $O(R^{-4})$, the [pressure](../../../../../../pressure.md) force is $O(R^{-1})$, and the viscous term is $O(\nu R^{-2})$ under the regular far-field derivative decay. All vanish as $R\to\infty$. **The localized eddy cannot change its total [impulse](../../../../../../impulse.md) without a net external [momentum](../../../../../../momentum.md) input.** [Pressure](../../../../../../pressure.md) redistributes [momentum](../../../../../../momentum.md) internally but its resultant force on an increasingly distant control surface tends to zero. At finite $R$, boundary forces need not vanish exactly; the all-space limit is the invariant statement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
