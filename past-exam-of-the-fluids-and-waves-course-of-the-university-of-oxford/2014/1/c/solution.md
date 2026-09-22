<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [product rule](../../../../product-rule.md), the [Laplace equation](../../../../laplace-equation.md) and $\mathbf u=\nabla\phi$ give

$$
\boxed{\nabla\cdot(\phi\nabla\phi)=|\nabla\phi|^2+\phi\nabla^2\phi=|\mathbf u|^2.}
$$

First truncate the exterior fluid domain by a large [circle](../../../../circle.md) $C_R$. Let $\mathbf n_B$ point outward from the body into the fluid. The outward normal of the exterior fluid domain at the body is $-\mathbf n_B$. The planar [divergence theorem](../../../../divergence-theorem.md), equivalently [Green's theorem](../../../../green-theorem.md), therefore gives

$$
\int_{D_R}|\mathbf u|^2\,dA
=\oint_{C_R}\phi\phi_r\,ds-\oint_{\partial B}\phi\,\partial_{n_B}\phi\,ds.
$$

Orient $\partial B$ counterclockwise around the body. Then $\mathbf n_B\,ds=(dy,-dx)$ and

$$
\partial_{n_B}\phi\,ds=\phi_x\,dy-\phi_y\,dx
=\psi_y\,dy+\psi_x\,dx=d\psi.
$$

For the finite-energy exterior rigid-body flow intended here, the outer boundary term vanishes as $R\to\infty$. In particular, zero net [volume flux](../../../../volumetric-flow-rate.md) and zero [circulation](../../../../circulation-physics.md) eliminate the $1/z$ term in the exterior [Laurent series](../../../../laurent-series.md) of the [complex velocity](../../../../complex-velocity.md). Thus $\mathbf u=O(R^{-2})$ and, after choosing the additive potential constant, $\phi=O(R^{-1})$. The outer integral is then $O(R^{-2})$.

Multiplying by half the constant [mass density](../../../../density.md) gives the [boundary integral for kinetic energy of planar potential flow](../../../../boundary-integral-for-kinetic-energy-of-planar-potential-flow.md):

$$
\boxed{T=\frac\rho2\int_{\mathbb R^2\setminus B}|\mathbf u|^2\,dA
=-\frac\rho2\oint_{\partial B}\phi\,d\psi.}
$$

The minus sign comes from the fluid's inner-boundary orientation, rather than a negative physical [kinetic energy](../../../../kinetic-energy.md).

There is a necessary qualification to the printed hypotheses. Decaying [velocity](../../../../velocity.md) and zero [circulation](../../../../circulation-physics.md) alone do not ensure a finite [kinetic energy](../../../../kinetic-energy.md): $\phi=A\log r$ gives $\mathbf u=A\mathbf e_r/r$, zero [circulation](../../../../circulation-physics.md), and logarithmically divergent exterior [kinetic energy](../../../../kinetic-energy.md). It carries a nonzero [volume flux](../../../../volumetric-flow-rate.md) from the body and is not the flow of an impermeable rigid body. The [finite-energy condition for planar exterior potential flow](../../../../finite-energy-condition-for-planar-exterior-potential-flow.md) makes explicit the source-free assumption needed to discard the outer boundary term.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
