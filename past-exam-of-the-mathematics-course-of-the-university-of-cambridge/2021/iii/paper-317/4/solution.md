<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let

$$
a_i^2=\frac{P_g}{\rho}=\frac{\mathcal R T}{\mu}
$$

be the local [isothermal sound speed](../../../../../isothermal-sound-speed.md) squared. Steady spherical [mass conservation](../../../../../mass-conservation.md) gives

$$
4\pi r^2\rho v=\dot M,
\qquad
\frac{d\log\rho}{dr}=-\frac2r-\frac1v\frac{dv}{dr}.
$$

The momentum equation, with radiative acceleration represented by the radiation-pressure gradient, is

$$
v\frac{dv}{dr}
=-\frac1\rho\frac{dP_g}{dr}
-\frac{Gm_r}{r^2}
+\frac{\kappa L}{4\pi cr^2}.
$$

[Radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md) gives

$$
\frac{dP_{\rm rad}}{dr}
=-\frac{\kappa\rho L}{4\pi cr^2}.
$$

Using $P_{\rm rad}/P_g=(1-\beta)/\beta$ and

$$
\Gamma\equiv\frac{L}{L_{\rm crit}},
\qquad
L_{\rm crit}=\frac{4\pi cGm_r}{\kappa},
$$

this becomes

$$
\frac{d\log T}{dr}
=-\frac{\beta}{4(1-\beta)}
\frac{Gm_r}{r^2a_i^2}\Gamma.
$$

Substitution of $dP_g/dr=a_i^2d\rho/dr+\rho a_i^2d\log T/dr$ and the continuity equation yields the wind equation

$$
\boxed{\left(v-\frac{a_i^2}{v}\right)\frac{dv}{dr}
=\frac{2a_i^2}{r}
-\frac{Gm_r}{r^2}
\left[1-\Gamma\frac{4-3\beta}{4(1-\beta)}\right]}.
$$

Its topology is that of the [Parker wind equation](../../../../../parker-wind-equation.md). The coefficient of $dv/dr$ vanishes at the sonic line $v=a_i$. A smooth transonic solution must pass through a critical point where the right-hand side also vanishes; generic subsonic solutions are breezes or turn back, while generic supersonic branches cannot be joined smoothly to a quasi-static stellar atmosphere.

At the critical point,

$$
\Gamma_c=
\frac{4(1-\beta_c)}{4-3\beta_c}
\left(1-\frac{2a_{i,c}^2r_c}{Gm_c}\right).
$$

The assumed inequality $a_i^2\ll Gm_r/r$ makes the second factor positive and close to one. Since $0<\beta<1$,

$$
\frac{4(1-\beta)}{4-3\beta}<1.
$$

Thus acceleration through a regular sonic point requires radiation to cancel most, but not all, of the effective gravity and in particular

$$
\boxed{\frac{L}{L_{\rm crit}}<1}.
$$

If the local luminosity reached or exceeded $L_{\rm crit}$ in this diffusion model, the numerator would have the wrong sign for the subsonic branch to cross the sonic line smoothly under the cold-wind assumption.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 317](../../paper-317-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
