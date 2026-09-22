<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

For a continuously differentiable [vector field](../../../../../vector-field.md) on a volume and its boundary, the [divergence theorem](../../../../../divergence-theorem.md) equates $\int_V\nabla\cdot F\,dV$ to the outward flux $\int_{\partial V}F\cdot n\,dS$. For the given field, $\nabla\cdot F=5(x^2+y^2+z^2)=5r^2$, so

$$
\int_V\nabla\cdot F\,dV=4\pi\int_0^R5r^4\,dr=4\pi R^5.
$$

On the sphere, $n=(x,y,z)/R$, and

$$
F\cdot n=\frac{x^4+y^4+z^4+2x^2y^2+2y^2z^2+2z^2x^2}{R}=\frac{r^4}{R}=R^3.
$$

Thus the surface flux is also **$4\pi R^5$**, verifying the theorem by explicit calculation.

Apply the [product rule](../../../../../product-rule.md) to $\nabla\cdot(\phi\nabla\psi)=\phi\Delta\psi+\nabla\phi\cdot\nabla\psi$, then apply the [divergence theorem](../../../../../divergence-theorem.md). This proves [Green's first identity](../../../../../green-s-first-identity.md):

$$
\int_V(\phi\Delta\psi+\nabla\phi\cdot\nabla\psi)\,dV=\int_S\phi\,\partial_n\psi\,dS.
$$

Swap $\phi$ and $\psi$ and subtract. The gradient products cancel, giving [Green's second identity](../../../../../green-second-identity.md):

$$
\int_V(\phi\Delta\psi-\psi\Delta\phi)\,dV=\int_S(\phi\,\partial_n\psi-\psi\,\partial_n\phi)\,dS.
$$

For uniqueness, set $w=\phi_1-\phi_2$. It is a [harmonic function](../../../../../harmonic-function.md) with zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md). Under the stated smoothness assumptions, [Green's first identity](../../../../../green-s-first-identity.md) with $\phi=\psi=w$ gives $\int_V|\nabla w|^2dV=0$. Thus $w$ is constant on each connected component, and its boundary value makes every constant zero. **The two solutions agree throughout $V$.** This is [Dirichlet uniqueness for the Poisson equation](../../../../../dirichlet-uniqueness-for-the-poisson-equation.md). For classical solutions merely continuous up to the boundary and twice continuously differentiable in the interior, the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) gives the same conclusion without requiring boundary derivatives.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
