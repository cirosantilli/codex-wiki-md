<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the usual homogeneous, local, analytic [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md); [rotational symmetry](../../../../../rotational-symmetry.md) and [Z2 symmetry](../../../../../z2-symmetry.md) alone do not specify locality, analyticity, or the signs of the coefficients. The [local derivative expansion](../../../../../local-derivative-expansion.md) contains every rotational scalar with an even total number of fields:

$$
\begin{aligned}
F[\phi]&=\int d^dx\left[V(\phi)+\frac12 K(\phi)(\nabla\phi)^2+c_1(\nabla^2\phi)^2+c_2\big((\nabla\phi)^2\big)^2+\cdots\right],\\
V(\phi)&=f_0+\frac r2\phi^2+\frac u4\phi^4+\frac v6\phi^6+\cdots,\qquad K(\phi)=\gamma+\gamma_2\phi^2+\cdots.
\end{aligned}
$$

The omitted terms include all allowed higher field powers and contracted spatial derivatives. Terms differing by a total derivative are equivalent for bulk behavior with suitable boundary conditions. The displayed [gradient energy](../../../../../gradient-energy.md) assumes spatial homogeneity. If only rotations about an origin are imposed, rotationally invariant position-dependent coefficients are also possible.

In the [mean-field approximation](../../../../../mean-field-approximation.md), take a spatially uniform [order parameter](../../../../../order-parameter.md) and minimize its [Landau free energy](../../../../../landau-free-energy.md). For $\gamma>0$, $u>0$ and $r=a(T-T_c)$ with $a>0$, keeping the quadratic and quartic terms gives

$$
\phi_0=0\quad(r\geq0),\qquad \phi_0=\pm\sqrt{-r/u}\quad(r<0).
$$

The single minimum splits into two minima as the [temperature](../../../../../temperature.md) passes below the [critical temperature](../../../../../critical-temperature.md). Choosing one minimum gives [spontaneous symmetry breaking](../../../../../spontaneous-symmetry-breaking.md) of the [Z2 symmetry](../../../../../z2-symmetry.md) and a [continuous phase transition](../../../../../continuous-phase-transition.md). The [order parameter](../../../../../order-parameter.md) is the expectation in a selected ordered state; averaging equally over both states gives zero. A [Z2 symmetry](../../../../../z2-symmetry.md) does not guarantee a [continuous phase transition](../../../../../continuous-phase-transition.md): a negative quartic coefficient stabilized by a positive sextic coefficient can instead give a [first-order phase transition](../../../../../first-order-phase-transition.md).

Relaxing the [Z2 symmetry](../../../../../z2-symmetry.md) permits odd terms. A nonzero linear source generally rounds this ordinary [continuous phase transition](../../../../../continuous-phase-transition.md). A cubic term can instead give a [first-order phase transition](../../../../../first-order-phase-transition.md): for $V(\phi)=r\phi^2/2+w\phi^3/3+u\phi^4/4$, $u>0$ and $w\ne0$, equal minima occur at

$$
\phi_*= -\frac{2w}{3u},\qquad r_* =\frac{2w^2}{9u}>0.
$$

The [order parameter](../../../../../order-parameter.md) jumps from zero to $\phi_*$. A [continuous phase transition](../../../../../continuous-phase-transition.md) without an exact [Z2 symmetry](../../../../../z2-symmetry.md) is still possible with additional tuning; odd terms do not logically exclude it.

For the [multicritical even Landau potential](../../../../../multicritical-even-landau-potential.md), set $r=\mu^2=a(T-T_c)$ and assume an integer $n\geq2$, $\lambda_n>0$ and $\gamma>0$. For $n>2$, all lower even interactions must be absent or tuned to zero to obtain these [mean-field critical exponents](../../../../../mean-field-critical-exponent.md). The stationary equation is

$$
0=r\phi_0+2n\lambda_n\phi_0^{2n-1},\qquad |\phi_0|^{2n-2}=\frac{-r}{2n\lambda_n}\quad(r<0).
$$

Its nonzero solutions are minima because $V''(\phi_0)=-(2n-2)r>0$. Thus the [order-parameter critical exponent](../../../../../order-parameter-critical-exponent.md) is

$$
\boxed{\beta_{\mathrm{MF}}=\frac{1}{2(n-1)}}.
$$

Substituting into the minimum [free energy](../../../../../thermodynamic-free-energy.md) density gives

$$
f_{\min}=-\frac{n-1}{2n}(2n\lambda_n)^{-1/(n-1)}(-r)^{n/(n-1)}.
$$

The singular [heat capacity](../../../../../heat-capacity.md) per unit volume is $c_s=-T\,\partial_T^2 f_{\min}$. Smooth variation of the other coefficients does not change the leading power. Consequently

$$
c_s\propto (T_c-T)^{n/(n-1)-2},\qquad \boxed{\alpha_{\mathrm{MF}}=\frac{n-2}{n-1}}.
$$

For $n=2$, this means a finite [heat capacity](../../../../../heat-capacity.md) jump, with $\alpha_{\mathrm{MF}}=0$; for $n=3$, the [tricritical point](../../../../../tricritical-point.md) has $\beta_{\mathrm{MF}}=1/4$ and $\alpha_{\mathrm{MF}}=1/2$. The case $n=1$ would contain only a quadratic potential and would not stabilize an ordered phase.

The [Gaussian fluctuation correction near a critical point](../../../../../gaussian-fluctuation-correction-near-a-critical-point.md) is more singular than the [mean-field approximation](../../../../../mean-field-approximation.md) contribution when

$$
2-\frac d2>\frac{n-2}{n-1}\quad\Longleftrightarrow\quad \boxed{d<d_c=\frac{2n}{n-1}}.
$$

This is the [upper critical dimension of an even scalar interaction](../../../../../upper-critical-dimension-of-an-even-scalar-interaction.md). Equivalently, its coupling has [engineering dimension](../../../../../engineering-dimension.md) $2n-(n-1)d$, positive below $d_c$. Dominant fluctuations signal breakdown of the [mean-field approximation](../../../../../mean-field-approximation.md); the Gaussian expression is not then a calculation of the exact interacting [heat-capacity critical exponent](../../../../../heat-capacity-critical-exponent.md). At $d=d_c$, equality of the powers allows logarithmic corrections.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 303](../../paper-303-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
