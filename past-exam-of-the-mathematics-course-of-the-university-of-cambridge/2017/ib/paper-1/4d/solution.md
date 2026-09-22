<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

Take a smooth [variation](../../../../../variation.md) $u_\varepsilon=u+\varepsilon\phi$ with $\phi=0$ on the boundary. Assume enough differentiability for the following operations, for example a smooth bounded [open set](../../../../../open-set.md), $u\in C^2$, and a twice continuously differentiable integrand. Differentiation under the [integral](../../../../../integral.md) gives

$$
\left.\frac{dI[u_\varepsilon]}{d\varepsilon}\right|_{0}=\int_{\mathcal D}(L_u\phi+L_{u_x}\phi_x+L_{u_y}\phi_y)\,dx\,dy.
$$

By [integration by parts](../../../../../integration-by-parts.md), the boundary term vanishes and the [first variation](../../../../../first-variation.md) is

$$
\int_{\mathcal D}\left(L_u-\partial_xL_{u_x}-\partial_yL_{u_y}\right)\phi\,dx\,dy.
$$

Stationarity for every such [variation](../../../../../variation.md), including every compactly supported smooth one, and the [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) give the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{L_u-\partial_xL_{u_x}-\partial_yL_{u_y}=0}.
$$

For the quadratic integrand, $L_u=2k^2u$, $L_{u_x}=2u_x$, and $L_{u_y}=2u_y$. Thus

$$
\boxed{u_{xx}+u_{yy}=k^2u}
$$

with the prescribed [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md). For real $k$, a stationary function is also the unique minimizer, if it exists: for any nonzero admissible $\phi$, the linear term vanishes and $I[u+\phi]-I[u]=\int_{\mathcal D}(|\nabla\phi|^2+k^2\phi^2)>0$. This last positivity uses the zero boundary values; it also holds at $k=0$.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
