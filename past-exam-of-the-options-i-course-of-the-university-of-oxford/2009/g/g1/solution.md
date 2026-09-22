<h1 id="g/g1/solution">Solution</h1>

↑ **Parent:** [G1](../g1.md)

Take a smooth [variation](../../../../variation.md) $u+\varepsilon\eta$ with $\eta$ vanishing on the boundary; compactly supported test functions suffice for the interior equation. At an extremum, the [first variation](../../../../first-variation.md) is zero:

$$
0=\left.\frac{d}{d\varepsilon}I[u+\varepsilon\eta]\right|_{\varepsilon=0}
=\int_V\left(F_u\eta+F_{u_x}\eta_x+F_{u_y}\eta_y+F_{u_z}\eta_z\right)\,dV.
$$

[Integration by parts](../../../../integration-by-parts.md) removes the derivatives from $\eta$. The boundary terms vanish, giving

$$
\int_V\left(F_u-\partial_xF_{u_x}-\partial_yF_{u_y}-\partial_zF_{u_z}\right)\eta\,dV=0.
$$

The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md)

$$
\boxed{\partial_xF_{u_x}+\partial_yF_{u_y}+\partial_zF_{u_z}-F_u=0}.
$$

This is the classical equation for sufficiently smooth admissible extrema; for weaker regularity the first-[variation](../../../../variation.md) identity supplies its weak form.

For the squared-[gradient](../../../../gradient.md) integrand, the equation is $2(u_{xx}+u_{yy}+u_{zz})=0$, namely the [Laplace equation](../../../../laplace-equation.md). Put $u_0=ax+by+cz$ and write any admissible [function](../../../../function-split.md) as $u=u_0+v$, with $v=0$ on the boundary. The [energy](../../../../energy-split.md) identity is

$$
I[u]=(a^2+b^2+c^2)\operatorname{vol}V
+2\int_V(a,b,c)\cdot\nabla v\,dV+\int_V|\nabla v|^2\,dV.
$$

By the [divergence theorem](../../../../divergence-theorem.md), the middle integral is $\int_{\partial V}v(a,b,c)\cdot n\,dS=0$; equivalently it vanishes by weak [integration by parts](../../../../integration-by-parts.md) for zero-trace functions. The final term is nonnegative and vanishes at $v=0$. Thus this is a global minimum, not merely a stationary value:

$$
\boxed{\min I=(a^2+b^2+c^2)\operatorname{vol}V}.
$$

## ↑ Ancestors (12)

1. [G1](../g1.md)
2. [G](../../g.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
