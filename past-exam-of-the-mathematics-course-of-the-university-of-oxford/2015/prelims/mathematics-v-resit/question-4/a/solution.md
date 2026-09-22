<h1 id="question-4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the rod has constant [cross-sectional area](../../../../../../cross-sectional-area.md) $A$, no internal source of [heat](../../../../../../heat-split.md), no bulk motion, and no lateral [heat flux](../../../../../../heat-flux-density.md). Assume also that each section has a uniform [temperature](../../../../../../temperature-split.md), so that $T$ depends only on $x,t$, and that [Fourier's law](../../../../../../fourier-s-law.md) applies with the stated constant [thermal conductivity](../../../../../../thermal-conductivity.md) $k$. The longitudinal [heat flux density](../../../../../../heat-flux-density.md) is then $q=-kT_x$.

By [conservation of energy](../../../../../../conservation-of-energy.md), the rate of increase of [internal energy](../../../../../../internal-energy-split.md) in a slice $[x,x+\Delta x]$ equals incoming minus outgoing [heat](../../../../../../heat-split.md):

$$
\rho c A\int_x^{x+\Delta x}T_t(s,t)\,ds
=A\bigl(q(x,t)-q(x+\Delta x,t)\bigr).
$$

Divide by $A\Delta x$ and take the [limit](../../../../../../limit-of-a-function.md) $\Delta x\to0$. For a sufficiently differentiable [temperature](../../../../../../temperature-split.md) field this gives $\rho cT_t=-q_x=kT_{xx}$, and hence

$$
\boxed{T_t=\kappa T_{xx},\qquad\kappa=\frac{k}{\rho c},\qquad0<x<L,\quad t>0.}
$$

Here $\rho$ is [mass density](../../../../../../density.md), $c$ is [specific heat capacity](../../../../../../specific-heat-capacity.md), and $\kappa$ is [thermal diffusivity](../../../../../../thermal-diffusivity.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
