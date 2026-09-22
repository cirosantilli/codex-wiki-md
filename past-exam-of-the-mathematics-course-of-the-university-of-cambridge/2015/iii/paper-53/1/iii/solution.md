<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Normalize the present [scale factor](../../../../../../scale-factor-cosmology.md) to one. For $0<\Omega<1$, the parametric solution gives

$$
u_0:=\alpha\tau_0=2\operatorname{arsinh}\sqrt{\frac b\Omega},\qquad \sinh u_0=\frac{2\sqrt b}{\Omega}.
$$

Thus the [age of a flat matter-coasting-fluid universe](../../../../../../age-of-a-flat-matter-coasting-fluid-universe.md) is

$$
\boxed{t_0=H_0^{-1}\left[\frac1b-\frac{\Omega}{b^{3/2}}\operatorname{arsinh}\sqrt{\frac b\Omega}\right],\qquad b=1-\Omega.}
$$

A direct age integral proves the bound more transparently than manipulating inverse hyperbolic functions. Since $\dot a=H_0\sqrt{\Omega/a+b}$,

$$
H_0t_0=\int_0^1\frac{\sqrt a\,da}{\sqrt{\Omega+ba}}.
$$

For $0\leq a\leq1$ and $0\leq\Omega\leq1$, one has $a\leq\Omega+ba\leq1$, hence

$$
\sqrt a\leq\frac{\sqrt a}{\sqrt{\Omega+ba}}\leq1.
$$

Integrating gives

$$
\boxed{\frac{2}{3}H_0^{-1}\leq t_0\leq H_0^{-1}.}
$$

Equality on the left is the pure [pressureless matter](../../../../../../pressureless-matter.md) universe, $\Omega=1$; equality on the right is the pure [coasting fluid](../../../../../../coasting-fluid.md), $\Omega=0$. These are all physically allowed density fractions for the nonnegative two-fluid model. The integrand decreases with $\Omega$, so the [coasting-fluid age bound](../../../../../../coasting-fluid-age-bound.md) is approached continuously between those endpoints. In the closed expression the apparent $b=0$ singularities cancel using $\operatorname{arsinh}x=x-x^3/6+\cdots$; as $\Omega\to0$, the term $\Omega\log(1/\Omega)$ vanishes. The limits are respectively $H_0t_0=2/3$ and $1$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
