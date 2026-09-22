<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The interface is material. Applying the [kinematic boundary condition](../../../../kinematic-boundary-condition.md) to $y-\eta(x,t)=0$ gives, exactly,

$$
\phi_{-,y}=\eta_t+\phi_{-,x}\eta_x,\qquad
\phi_{+,y}=\eta_t+(U+\phi_{+,x})\eta_x
\quad(y=\eta).
$$

The disturbance [velocities](../../../../velocity.md) and $\eta$ are small. Products of two disturbance quantities are second order, and a [Taylor expansion](../../../../taylor-expansion.md) moves their evaluation to $y=0$ at [linear order](../../../../linear-order.md). Hence

$$
\boxed{\phi_{-,y}=\eta_t,\qquad
\phi_{+,y}=\eta_t+U\eta_x\quad(y=0).}
$$

The extra upper-fluid term is advection of the displaced interface by the base [uniform flow](../../../../uniform-flow.md).

Use the [Unsteady Bernoulli equation](../../../../unsteady-bernoulli-equation.md) separately on each side, with constant [mass density](../../../../density.md) $\rho$. There are no restoring terms specified at this internal interface, and its [pressure](../../../../pressure-split.md) is continuous. Choose the time-dependent potential gauges so that the undisturbed [pressure](../../../../pressure-split.md) is $p_0$ on both sides. Subtracting the base values from [Bernoulli's principle](../../../../bernoulli-s-principle.md) gives, at [linear order](../../../../linear-order.md),

$$
p'_-=-\rho\phi_{-,t},\qquad
p'_+=-\rho(\phi_{+,t}+U\phi_{+,x}).
$$

The quadratic disturbance-[velocity](../../../../velocity.md) terms have been discarded, while the cross term with the base [velocity](../../../../velocity.md) is first order and must remain. Equating the perturbation [pressures](../../../../pressure-split.md) yields the third condition:

$$
\boxed{\phi_{-,t}=\phi_{+,t}+U\phi_{+,x}\quad(y=0).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
