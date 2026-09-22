<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All invariants in this part refer to the selected [magnetic field line](../../../../../../magnetic-field-line.md). Its squared poloidal [Alfvén number](../../../../../../alfven-number.md) is

$$
M_{Ap}^2=\frac{\mu_0\rho u_p^2}{B_p^2}=\frac{\mu_0k^2}{\rho}.
$$

At the [Alfvén surface](../../../../../../alfven-surface.md) crossing it equals unity, so $\rho_a=\mu_0k^2$ and $M_{Ap}^2=1/y$. Subtract the two azimuthal integrals in part (a) to find

$$
R\omega-\frac\ell R=\frac{B_\phi}{\mu_0k}\left(1-\frac{\mu_0k^2}{\rho}\right),\qquad
v_\phi\equiv u_\phi-R\omega=\frac{R\omega-\ell/R}{y-1}.
$$

Finite azimuthal fields and [velocity](../../../../../../velocity.md) at $y=1$ require the [Alfvén-surface regularity condition for an axisymmetric wind](../../../../../../alfven-surface-regularity-condition-for-an-axisymmetric-wind.md) $\ell=\omega R_a^2$. Hence

$$
v_\phi=\omega R_a\frac{x-x^{-1}}{y-1},\qquad
|u_p|=\frac{|k|C}{\rho_aR_a^2x^2y}
=\frac{C}{\sqrt{\mu_0\rho_a}R_a^2x^2y}.
$$

Here $v_\phi$ denotes the azimuthal [velocity](../../../../../../velocity.md) relative to field-line rotation. For gravity of a [point mass](../../../../../../point-mass.md) at $z=0$, $\Phi=-GM/R=-GM/(R_ax)$.

Insert these quantities in the corotating [energy](../../../../../../energy.md) integral with $w=0$, and divide by the gravitational [energy](../../../../../../energy.md) scale $GM/R_a$. This gives the [cold radial magnetohydrodynamic wind integral](../../../../../../cold-radial-magnetohydrodynamic-wind-integral.md),

$$
\boxed{f(x,y)=\frac\alpha2\left[\left(\frac{x-x^{-1}}{y-1}\right)^2-x^2\right]
+\frac\beta{2x^4y^2}-\frac1x=\frac{\varepsilon R_a}{GM}},
$$

with

$$
\boxed{\alpha=\frac{\omega^2R_a^3}{GM},\qquad
\beta=\frac{C^2}{\mu_0\rho_a GM R_a^3}}.
$$

Both are dimensionless. The apparent $0/0$ at $x=y=1$ must be evaluated on the smooth solution branch, not assigned an arbitrary value.

A constant-[energy](../../../../../../energy.md) curve obeys $f_x+f_y\,dy/dx=0$. At a nondegenerate magnetosonic point, the vanishing coefficient of the [mass density](../../../../../../density.md) derivative requires simultaneous vanishing of its numerator:

$$
\boxed{f_y=0,\qquad f_x=0,\qquad f=f_{\rm wind}}.
$$

The curve must admit a real crossing slope. Expanding about such a point gives $f_{yy}m^2+2f_{xy}m+f_{xx}=0$, $m=dy/dx$, so a regular [saddle point of a scalar function](../../../../../../saddle-point-of-a-scalar-function.md) crossing has $f_{xy}^2-f_{xx}f_{yy}>0$. These are the form of the slow and fast regularity conditions in a warm wind, with the [enthalpy](../../../../../../enthalpy.md) contribution retained in $f$.

In the strictly cold approximation used to obtain the displayed $f$, the slow speed is zero. There is a [cold-limit degeneracy of a slow magnetosonic point](../../../../../../cold-limit-degeneracy-of-a-slow-magnetosonic-point.md): a finite-speed interior slow crossing need not survive. Indeed,

$$
f_y=-\frac{\alpha(x-x^{-1})^2}{(y-1)^3}-\frac{\beta}{x^4y^3}<0\qquad(y>1,\ \beta>0),
$$

so this cold equation has no ordinary sub-Alfvénic slow critical point. A small retained [enthalpy](../../../../../../enthalpy.md) is needed to locate that point, which can approach the launching boundary as the [sound speed](../../../../../../speed-of-sound.md) tends to zero. The fast critical point still obeys the simultaneous conditions above wherever the reduced expression is nonsingular.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
