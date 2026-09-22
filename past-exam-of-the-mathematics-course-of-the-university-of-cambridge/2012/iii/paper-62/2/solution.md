<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $u=u_r<0$ for accretion. The steady spherical [continuity equation](../../../../../continuity-equation.md) and radial [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) give

$$
\frac{d}{dr}(r^2\rho u)=0,\qquad
u\frac{du}{dr}=-\frac1\rho\frac{dp}{dr}-\frac{d\Phi}{dr},\qquad
\dot M=-4\pi r^2\rho u>0.
$$

For a [barotropic fluid](../../../../../barotropic-fluid.md), $dp/dr=c_s^2\,d\rho/dr$. Dividing [continuity equation](../../../../../continuity-equation.md) by $r^2\rho u$ gives $\rho'/\rho=-2/r-u'/u$. Eliminating this derivative yields

$$
\boxed{\frac{u^2-c_s^2}{u}\frac{du}{dr}=\frac{2c_s^2}{r}-\Phi'(r).}
$$

At a smooth transonic critical point, the coefficient of $du/dr$ vanishes. A finite derivative then requires the right side to vanish simultaneously:

$$
\boxed{u_c=-c_{s,c},\qquad \Phi'(r_c)=\frac{2c_{s,c}^2}{r_c}.}
$$

These are the sonic and regularity conditions. Otherwise the derivative is singular and the proposed smooth transonic passage fails. The local slope must also be a real root compatible with the desired branch. For example, defining $C=\rho\,d(c_s^2)/d\rho$ at the point and differentiating both sides gives

$$
\left(2+\frac C{c_s^2}\right)(u_c')^2
+\frac{4C}{r_cu_c}u_c'+\frac{4C+2c_s^2}{r_c^2}+\Phi''(r_c)=0.
$$

This explains why simultaneous vanishing is a necessary regularity condition, rather than an automatic proof that every potential admits a critical crossing.

Define the [barotropic enthalpy function](../../../../../barotropic-enthalpy-function.md) by $dh=dp/\rho$. The momentum equation integrates to the [Bernoulli equation](../../../../../bernoulli-equation.md)

$$
\boxed{\frac12u^2+h(\rho)+\Phi=B.}
$$

Changing the reference [mass density](../../../../../density.md) in $h$ changes only the constant $B$. For an isothermal closure this logarithmic function is a barotropic [barotropic pressure potential](../../../../../barotropic-enthalpy-function.md); it should not be confused with the constant thermodynamic [specific enthalpy](../../../../../specific-enthalpy.md) of an ideal gas held at fixed temperature.

For [isothermal transonic accretion in the Paczyński-Wiita potential](../../../../../isothermal-transonic-accretion-in-the-paczynski-wiita-potential.md), assume $M>0$ and $c_s>0$, and define $r_B=GM/(2c_s^2)$ and $\beta=16c_s^2/c^2$. The critical equation is

$$
(r_c-r_G)^2=r_Br_c,
$$

whose two roots are $r_G+\tfrac12r_B(1\pm\sqrt{1+\beta})$. Only the plus root lies outside $r_G$. Therefore

$$
\boxed{r_c=r_G+\frac{GM}{4c_s^2}(1+\sqrt{1+\beta})
=\frac{GM}{4c_s^2}\bigl(1+\beta/2+\sqrt{1+\beta}\bigr)>r_G.}
$$

For this isothermal case $C=0$, and the slope relation reduces to

$$
(u_c')^2=\frac{GM}{(r_c-r_G)^3}-\frac{c_s^2}{r_c^2}
=\frac{c_s^2(r_c+r_G)}{r_c^2(r_c-r_G)}>0.
$$

The positive slope is the inward-accretion solution connecting a small inward speed at large radius to the supersonic inward branch. Thus the exterior critical point is a genuine nondegenerate transonic point.

Choose the reference [mass density](../../../../../density.md) as $\rho_0$, so $h=c_s^2\log(\rho/\rho_0)$ and $B=0$ from the conditions at infinity. At $u_c=-c_s$,

$$
\rho_c=\rho_0\exp\left[\frac{GM}{c_s^2(r_c-r_G)}-\frac12\right]
=\rho_0\exp\left[\frac4{1+\sqrt{1+\beta}}-\frac12\right].
$$

Substitution into $\dot M=4\pi r_c^2\rho_cc_s$ gives

$$
\boxed{\dot M=\frac{\pi\rho_0(GM)^2}{4c_s^3}
\bigl(1+\beta/2+\sqrt{1+\beta}\bigr)^2
\exp\left[\frac4{1+\sqrt{1+\beta}}-\frac12\right].}
$$

This is the rate selected by the smooth transonic accretion solution. Arbitrary static or subsonic formal solutions are not assigned this rate merely by specifying conditions at infinity. As $r_G/r_B\to0$, the result tends to the [isothermal Bondi accretion rate](../../../../../isothermal-bondi-accretion-rate.md) $\pi e^{3/2}\rho_0(GM)^2/c_s^3$, a useful normalization check.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
