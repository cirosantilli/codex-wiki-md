<h1 id="k/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a material fluid volume, [mass conservation](../../../../mass-conservation.md) yields $\rho_t+\nabla\cdot(\rho\mathbf u)=0$. Constant [mass density](../../../../density.md) reduces this to $\nabla\cdot\mathbf u=0$. For [inviscid flow](../../../../inviscid-flow.md), the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md) is $-pI$; its net surface [force](../../../../force-split.md) is the volume integral of $-\nabla p$ by the [divergence theorem](../../../../divergence-theorem.md). [Newton's second law](../../../../newton-s-second-law.md) for each material volume therefore gives $\rho D\mathbf u/Dt=-\nabla p$. Since $D/Dt=\partial_t+\mathbf u\cdot\nabla$, these are exactly the two stated equations.

In two dimensions they read

$$
u_t+uu_x+vu_y=-p_x/\rho,\qquad v_t+uv_x+vv_y=-p_y/\rho,\qquad u_x+v_y=0.
$$

Differentiate the second momentum equation in $x$ and subtract the $y$ derivative of the first. The [pressure](../../../../pressure-split.md) terms cancel. For $\omega=v_x-u_y$, collecting terms gives

$$
\omega_t+u\omega_x+v\omega_y+(u_x+v_y)\omega=0.
$$

[Incompressibility](../../../../incompressible-flow.md) removes the last term, giving

$$
\boxed{\frac{D\omega}{Dt}=0.}
$$

Thus **each fluid parcel retains its scalar [vorticity](../../../../vorticity-split.md)** as it moves. In particular an initially [irrotational flow](../../../../irrotational-flow.md) remains irrotational in this smooth two-dimensional inviscid evolution. There is no [vortex stretching](../../../../vortex-stretching.md) in this two-dimensional setting.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [K](../../k.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
