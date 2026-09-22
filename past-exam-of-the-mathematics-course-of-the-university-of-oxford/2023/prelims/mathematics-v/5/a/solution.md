<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a bar of constant cross-sectional [area](../../../../../../surface-area.md) $A$, thermally insulated along its sides, with no internal heat production. [Fourier's law](../../../../../../fourier-s-law.md) says that the [heat flux](../../../../../../heat-flux-density.md) in the positive $x$ direction is

$$
q(x,t)=-k(x)T_x(x,t).
$$

The [thermal conductivity](../../../../../../thermal-conductivity.md) $k(x)$ is positive. On a small slice $[x,x+\Delta x]$, [conservation of energy](../../../../../../conservation-of-energy.md) gives

$$
A\int_x^{x+\Delta x}\rho c_pT_t(s,t)\,ds
=A\bigl[q(x,t)-q(x+\Delta x,t)\bigr].
$$

Here $\rho c_p$ is the volumetric [heat capacity](../../../../../../heat-capacity.md), the product of [mass density](../../../../../../density.md) and [specific heat capacity](../../../../../../specific-heat-capacity.md). Divide by $A\Delta x$, take $\Delta x\to0$, and use $\rho c_p=1$. The resulting [heat equation](../../../../../../heat-equation.md) is

$$
\boxed{T_t=-q_x=\frac{\partial}{\partial x}\bigl(k(x)T_x\bigr).}
$$

For differentiable $k$, this is $T_t=kT_{xx}+k'T_x$; retaining the divergence form also expresses [conservation of energy](../../../../../../conservation-of-energy.md) correctly across an interface where $k$ jumps.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
