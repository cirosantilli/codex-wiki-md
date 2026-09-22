<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret $v$ as the normal upstream speed in the shock rest frame and $\rho$ as its upstream [mass density](../../../../density.md). If the quoted jet speed is in another frame, the shock speed must first be supplied to obtain this relative [velocity](../../../../velocity.md). Use a calorically perfect gas of mean particle [mass](../../../../mass.md) $\bar m=\mu m_u$.

In the strong-shock limit, $\mathcal M_1\gg1$. The [Strong-shock Rankine-Hugoniot conditions](../../../../strong-shock-rankine-hugoniot-conditions.md) give

$$
\rho_2=\frac{\gamma+1}{\gamma-1}\rho,\qquad
u_2=\frac{\gamma-1}{\gamma+1}v,\qquad
p_2\simeq\frac{2}{\gamma+1}\rho v^2.
$$

The [pressure](../../../../pressure-split.md) expression also follows from the supplied ratio by inserting $\mathcal M_1^2=\rho v^2/(\gamma p_1)$. The [ideal gas law](../../../../ideal-gas-law.md) then gives the immediate postshock [temperature](../../../../temperature-split.md)

$$
\boxed{T_2\simeq\frac{2(\gamma-1)}{(\gamma+1)^2}\frac{\mu m_u}{k_B}v^2.}
$$

The upstream thermal contribution is negligible at this order. This is a [temperature](../../../../temperature-split.md) in kelvin, rather than a [temperature](../../../../temperature-split.md) change per unit time.

To turn the postshock thermal energy into a rate, the processed mass per unit time is $\dot m=\rho vS$. Its downstream [specific internal energy](../../../../specific-internal-energy.md) is

$$
\epsilon_2=\frac{k_BT_2}{(\gamma-1)\mu m_u}
=\frac{2v^2}{(\gamma+1)^2}.
$$

Thus the **thermal internal energy carried into the shocked gas per unit time** is

$$
\boxed{\dot E_{\rm int}=\dot m\epsilon_2
=\frac{2}{(\gamma+1)^2}\rho Sv^3.}
$$

Per unit area, divide this expression by $S$. Its dimensions are watts; the [mean molecular weight](../../../../mean-molecular-weight.md) cancels because the heat capacity per unit mass is inversely proportional to it, while $T_2$ is proportional to it.

There is a second common convention for shock heating power: the loss of directed bulk [kinetic energy](../../../../kinetic-energy.md) flux. The [energy fluxes of a strong adiabatic shock](../../../../energy-fluxes-of-a-strong-adiabatic-shock.md) give

$$
\boxed{\dot E_{\rm kin,loss}=\frac{\dot m}{2}(v^2-u_2^2)
=\frac{2\gamma}{(\gamma+1)^2}\rho Sv^3
=\dot m h_2.}
$$

This equals the downstream [enthalpy](../../../../enthalpy-split.md) flux, and includes [pressure](../../../../pressure-split.md) work as well as the advected internal energy. For $\gamma=5/3$, the compression ratio is $4$, $T_2=3\mu m_uv^2/(16k_B)$, $\dot E_{\rm int}=9\rho Sv^3/32$, and $\dot E_{\rm kin,loss}=15\rho Sv^3/32$. Specifying the energy convention avoids conflating these rates. A rate $dT/dt$ for a fixed slab cannot be inferred without its participating mass and thermal evolution; the supplied data fix the postshock [temperature](../../../../temperature-split.md) and the processed energy fluxes.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
