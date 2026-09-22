<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take an admissible variation $u+\epsilon\eta$ with $\eta=0$ on the boundary. Differentiating the functional at an extremum gives

$$
0=\int_V(F_u\eta+F_{u_x}\eta_x+F_{u_y}\eta_y+F_{u_z}\eta_z)dV.
$$

Integration by parts removes the derivatives from $\eta$; the boundary term vanishes. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields

$$
\boxed{\partial_xF_{u_x}+\partial_yF_{u_y}+\partial_zF_{u_z}-F_u=0.}
$$

For the specified squared-[gradient](../../../../gradient.md) energy this is $2\Delta u=0$, so $u$ is harmonic. The affine function $\ell=ax+by+cz$ is harmonic and satisfies the boundary data.

To verify a global minimum, write $u=\ell+v$ with zero boundary trace. Then

$$
I[u]=I[\ell]+2\int_V\nabla\ell\cdot\nabla v\,dV+\int_V|\nabla v|^2dV.
$$

The middle term vanishes by integration by parts, since $\Delta\ell=0$ and $v=0$ at the boundary. Hence $I[u]\geq I[\ell]$, and

$$
\boxed{\min I=(a^2+b^2+c^2)\operatorname{vol}V.}
$$

This proves minimality directly, rather than relying only on a necessary Euler-Lagrange equation.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
