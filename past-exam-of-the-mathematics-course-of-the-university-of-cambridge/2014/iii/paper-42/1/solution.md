<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [scaling hypothesis for critical phenomena](../../../../../scaling-hypothesis-for-critical-phenomena.md) says that the singular part of the equilibrium [free energy](../../../../../thermodynamic-free-energy.md) is a generalized homogeneous function of its thermal and field-like controls. Smooth backgrounds must first be removed; the hypothesis does not claim that the entire [free energy](../../../../../thermodynamic-free-energy.md), including arbitrary regular terms, has a pure scaling form.

For the ordinary scalar quartic [LG theory](../../../../../landau-ginzburg-theory.md), set $r=r_t t$ with $r_t>0$ and $u>0$, and rescale the uniform [order parameter](../../../../../order-parameter.md) as

$$
m=\sqrt{\frac{r_t}{u}}\,|t|^{1/2}\psi.
$$

The order-parameter-dependent [free-energy density](../../../../../free-energy-density.md) becomes

$$
V(m)=\frac{r_t^2}{u}|t|^2\left\{\frac{\operatorname{sgn}(t)}2\psi^2+\frac14\psi^4-H\psi\right\},
\qquad H=\frac{\sqrt u}{r_t^{3/2}}\frac h{|t|^{3/2}}.
$$

Define $f_\pm(H)$ as the minimum of the braces, with the sign of the quadratic term respectively positive or negative. Consequently

$$
\boxed{A_s=a|t|^2f_\pm\left(b\frac h{|t|^{3/2}}\right),\quad a=\frac{r_t^2}{u}>0,\quad b=\frac{\sqrt u}{r_t^{3/2}}>0.}
$$

For an extensive $A_s$, $a$ additionally contains the system volume. The printed double-inequality subscript labels the two temperature branches: the upper-temperature function is $f_+$ and the lower-temperature function is $f_-$. It does not classify positive and negative magnetic fields. In particular $f_+(0)=0$ and $f_-(0)=-1/4$; below the transition the field dependence has a cusp at zero, so derivatives are taken on a selected branch.

For the following derivatives, take $A_s$ to be a density, so $m$ is the [magnetization](../../../../../magnetization.md) density; for total [free energy](../../../../../thermodynamic-free-energy.md) the derivative gives total [magnetization](../../../../../magnetization.md) instead. Differentiate this [mean-field scalar free-energy scaling](../../../../../mean-field-scalar-free-energy-scaling.md) form. The [magnetization](../../../../../magnetization.md) is $m=-\partial A_s/\partial h=-ab|t|^{1/2}f_\pm'(H)$, giving $m_0\propto(-t)^{1/2}$ and **$\beta=1/2$**. The [magnetic susceptibility](../../../../../magnetic-susceptibility.md) is $\chi=-\partial_h^2A_s=-ab^2|t|^{-1}f_\pm''(H)$, giving **$\gamma=1$**. At zero field the nonzero curvature amplitudes are $-f_+''(0)=1$ and $-f_-''(0^+)=1/2$.

To allow nonclassical [critical exponents](../../../../../critical-exponent.md), replace the fixed powers by

$$
\boxed{A_s=a|t|^{2-\alpha}f_\pm\left(b\frac h{|t|^{\Delta}}\right).}
$$

The [heat-capacity critical exponent](../../../../../heat-capacity-critical-exponent.md) is defined by $C_{V,s}\sim|t|^{-\alpha}$; temperature differentiation gives the thermal exponent $2-\alpha$ in $A_s$. The [order-parameter critical exponent](../../../../../order-parameter-critical-exponent.md) has $m_0\sim(-t)^\beta$, and the [magnetic-susceptibility critical exponent](../../../../../magnetic-susceptibility-critical-exponent.md) has $\chi\sim|t|^{-\gamma}$. Differentiating the scaling form gives

$$
\beta=2-\alpha-\Delta,\qquad\gamma=2\Delta-(2-\alpha).
$$

Eliminating $\Delta$ proves the [Rushbrooke scaling relation](../../../../../rushbrooke-scaling-relation.md)

$$
\boxed{\alpha+2\beta+\gamma=2.}
$$

The [critical-isotherm exponent](../../../../../critical-isotherm-exponent.md) is defined by $m(0,h)\sim\operatorname{sgn}(h)|h|^{1/\delta}$. At fixed small $h$, the $t\to0$ limit requires $f_\pm(H)\sim c|H|^{(2-\alpha)/\Delta}$, so that the temperature factors cancel. Therefore $1/\delta=(2-\alpha-\Delta)/\Delta=\beta/\Delta$, yielding $\Delta=\beta\delta$. But the two differentiated identities also give $\Delta=\beta+\gamma$, and hence the [Widom scaling relation](../../../../../widom-scaling-relation.md)

$$
\boxed{\beta\delta=\beta+\gamma.}
$$

These are relations among the leading power indices. At marginal dimensions, multiplicative logarithms can accompany them, and an additive analytic background must not be mistaken for the singular scaling contribution.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
