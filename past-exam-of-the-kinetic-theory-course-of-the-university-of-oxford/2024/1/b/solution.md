<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the zeroth [velocity moment](../../../../velocity-moment.md) of [a](../a.md). The right side is a [velocity space](../../../../velocity-space.md) divergence with vanishing boundary contribution, giving the [continuity equation](../../../../continuity-equation.md)

$$
\boxed{\partial_t\rho+\nabla\cdot(\rho\mathbf u)=0,\qquad \rho=\int f\,d^3v,\qquad \rho\mathbf u=\int\mathbf v f\,d^3v.}
$$

For the first [velocity moment](../../../../velocity-moment.md), use [integration by parts](../../../../integration-by-parts.md) componentwise:

$$
\int d^3v\,v_i\partial_{v_j}f_2=-\delta_{ij}\int d^3v\,f_2.
$$

Write $\mathbf c=\mathbf v-\mathbf u$; then $\int\mathbf c f\,d^3v=0$, and the [momentum flux](../../../../momentum-flux.md) splits into bulk transport and the [pressure tensor](../../../../pressure-tensor.md):

$$
\int v_iv_jf\,d^3v=\rho u_iu_j+P_{ij},\qquad \boxed{P_{ij}=\int (v_i-u_i)(v_j-u_j)f\,d^3v.}
$$

Therefore

$$
\boxed{\partial_t(\rho u_i)+\partial_{x_j}(\rho u_iu_j+P_{ij})=-\int d^3x_\star\,n_2(\mathbf x,\mathbf x_\star,t)\partial_{x_i}\phi(|\mathbf x-\mathbf x_\star|),}
$$

where repeated Cartesian indices are summed and $n_2=\int f_2\,d^3v\,d^3v_\star$. The negative sign is the attractive or repulsive [force](../../../../force-split.md) $-\nabla\phi$, rather than an additional sign convention for the [pressure tensor](../../../../pressure-tensor.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
