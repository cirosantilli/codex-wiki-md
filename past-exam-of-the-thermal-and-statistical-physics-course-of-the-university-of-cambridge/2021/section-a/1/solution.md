<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The fixed common [temperature](../../../../temperature-split.md), rigid external container and fixed [particle](../../../../particle-physics.md) numbers on either side make the total [Helmholtz free energy](../../../../helmholtz-free-energy.md) the appropriate [thermodynamic potential](../../../../thermodynamic-potential-split.md). Let the barrier have cross-sectional area $A$, and let increasing $x$ expand the left compartment. Then $dV_1=A\,dx$ and $dV_2=-A\,dx$. At fixed [temperature](../../../../temperature-split.md) and [particle](../../../../particle-physics.md) number, $dF_j=-p_j\,dV_j$, so

$$
F(x)=F_1(T,V_1(x),N_1)+F_2(T,V_2(x),N_2),\qquad
\frac{dF}{dx}=A(p_2-p_1).
$$

Thus [mechanical equilibrium](../../../../mechanical-equilibrium.md), $p_1=p_2$, makes $F$ stationary. The physical [force](../../../../force-split.md) on the barrier towards increasing $x$ is $f=A(p_1-p_2)=-F'(x)$. If the barrier is displaced slightly from $x_*$, strict [mechanical stability](../../../../mechanical-stability.md) requires a restoring [force](../../../../force-split.md):

$$
f(x_*+\delta x)=A\left(\frac{\partial p_1}{\partial x}-\frac{\partial p_2}{\partial x}\right)_{x_*}\delta x+O(\delta x^2),
\qquad f'(x_*)<0.
$$

Consequently

$$
\boxed{F''(x_*)=A\left(\frac{\partial p_2}{\partial x}-\frac{\partial p_1}{\partial x}\right)_{x_*}>0.}
$$

The [Taylor expansion](../../../../taylor-expansion.md) $F(x_*+\delta x)=F(x_*)+\tfrac12F''(x_*)\delta x^2+O(\delta x^3)$ proves that [thermodynamic equilibrium](../../../../thermodynamic-equilibrium.md) is a strict local minimum of the [Helmholtz free energy](../../../../helmholtz-free-energy.md), rather than merely a [stationary point](../../../../stationary-point.md).

For individually stable gases, the positive [isothermal compressibilities](../../../../isothermal-compressibility.md) $\kappa_{T,j}=-(1/V_j)(\partial V_j/\partial p_j)_{T,N_j}$ make the sign especially transparent:

$$
\frac{\partial p_1}{\partial x}=-\frac{A}{V_1\kappa_{T,1}},\qquad
\frac{\partial p_2}{\partial x}=\frac{A}{V_2\kappa_{T,2}},\qquad
F''=A^2\left(\frac1{V_1\kappa_{T,1}}+\frac1{V_2\kappa_{T,2}}\right)>0.
$$

If these inequalities hold throughout the accessible interval, $F$ is a [strictly convex function](../../../../strictly-convex-function.md) and an interior [stationary point](../../../../stationary-point.md) is the unique global minimum of the [Helmholtz free energy](../../../../helmholtz-free-energy.md). Stability at one point alone proves only the local statement. A vanishing restoring [derivative](../../../../derivative.md) describes marginal stability and requires examining higher-order terms.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
