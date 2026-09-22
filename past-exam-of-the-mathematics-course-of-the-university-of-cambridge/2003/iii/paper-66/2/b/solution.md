<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Adding and subtracting the canonical [scalar field](../../../../../../scalar-field.md) density and pressure gives

$$
\dot\phi^2=(1+w)\rho_\phi,\qquad V=\frac{1-w}{2}\rho_\phi.
$$

A real scalar with positive kinetic energy consequently needs $w\geq-1$. On the expanding scalar-dominated branch, divide $\dot\phi$ by $H$ and use the [Friedmann equation](../../../../../../friedmann-equations.md):

$$
\frac{d\phi}{d\log a}=\frac{\dot\phi}{H}
=\pm\sqrt{\frac{3(1+w)}{8\pi G}}.
$$

Choose the positive rolling sign. Integration and elimination of $a$ using $\rho_\phi=\rho^0_\phi(a/a_0)^{-3(1+w)}$ give the [scalar-field reconstruction for a constant equation of state](../../../../../../scalar-field-reconstruction-for-a-constant-equation-of-state.md):

$$
\boxed{\phi(a)=\phi_0+\sqrt{\frac{3(1+w)}{8\pi G}}\log\frac a{a_0},}
$$



$$
\boxed{V(\phi)=\frac{1-w}{2}\rho^0_\phi
\exp\left[-\sqrt{24\pi G(1+w)}(\phi-\phi_0)\right].}
$$

Changing the rolling sign reverses the exponential slope. At $w=-1$, $\phi$ is constant and $V=\rho^0_\phi$; elimination by an invertible $\phi(a)$ then degenerates. The [cosmological continuity equation](../../../../../../cosmological-continuity-equation.md) gives $\ddot\phi+3H\dot\phi+V_{,\phi}=0$ whenever $\dot\phi\ne0$, so the reconstruction satisfies the field equation as well as the Friedmann equation.

Compare the reconstructed exponent with $V_0e^{-\lambda\sqrt{8\pi G}\phi}$. In this constant-$w$, scalar-dominated scaling solution,

$$
\lambda^2=3(1+w),\qquad w=-1+\frac{\lambda^2}{3},\qquad a\propto t^{2/\lambda^2}.
$$

Strict $\rho_\phi+P_\phi>0$ requires $w>-1$, and acceleration requires $w<-1/3$. Hence

$$
\boxed{0<\lambda<\sqrt2.}
$$

The accelerating branch has $V_0>0$. The zero-slope limit is a constant potential with $\rho+P=0$, so it does not meet the strict inequality. This result characterizes the [exponential-potential power-law inflation](../../../../../../exponential-potential-power-law-inflation.md) solution; an arbitrary trajectory with the same potential need not have constant $w$ throughout its evolution.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
