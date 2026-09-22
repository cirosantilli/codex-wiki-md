<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Rankine-Hugoniot conditions for a perfect gas](../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md) express conservation of mass flux, normal momentum flux, and total energy flux through a steady planar [shock wave](../../../../shock-wave.md) in its rest frame. With mass flux $j=\rho_1u_1=\rho_2u_2$, momentum flux is $\rho u^2+p$ and specific transported energy is $u^2/2+e+p/\rho$. The last term is pressure work, so the energy equation contains [specific enthalpy](../../../../specific-enthalpy.md) rather than only [specific internal energy](../../../../specific-internal-energy.md). Neglect gravity across the thin front, magnetic stresses and radiative energy loss for the adiabatic case.

For a calorically perfect [ideal gas](../../../../ideal-gas-split.md), $e=p/[(\gamma-1)\rho]$ and $c_s^2=\gamma p/\rho$. Therefore

$$
\boxed{\frac{u_1^2}{2}+\frac{c_{s,1}^2}{\gamma-1}
=\frac{u_2^2}{2}+\frac{c_{s,2}^2}{\gamma-1}.}
$$

Put $\chi=\rho_2/\rho_1$, so $u_2=u_1/\chi$. Momentum conservation gives

$$
\frac{p_2}{p_1}=1+\gamma\mathcal M_1^2\left(1-\frac1\chi\right),
\qquad \mathcal M_1=\frac{u_1}{c_{s,1}}.
$$

Insert this and $c_{s,2}^2/c_{s,1}^2=(p_2/p_1)/\chi$ into the energy equation. After multiplying out, its two factors are

$$
(\chi-1)\left[\big((\gamma-1)\mathcal M_1^2+2\big)\chi
-(\gamma+1)\mathcal M_1^2\right]=0.
$$

The first root is the unchanged flow. The compressive [shock](../../../../shock-wave.md) branch is

$$
\boxed{\chi=\frac{(\gamma+1)\mathcal M_1^2}{(\gamma-1)\mathcal M_1^2+2}
=\frac{\gamma+1}{\gamma-1+2/\mathcal M_1^2}.}
$$

It has $\chi>1$ for upstream supersonic flow. A strong shock approaches $(\gamma+1)/(\gamma-1)$: **four for a monatomic gas**, or six for a fixed rotationally excited diatomic gas with $\gamma=7/5$. The assumed fixed heat capacity ceases to describe the gas when dissociation or ionization becomes important. Adiabatic here means no net heat lost from the shock-plus-flow energy budget; the irreversible front still increases [entropy](../../../../entropy-split.md).

For an [isothermal shock](../../../../isothermal-shock.md) of unchanged composition, let $a^2=p/\rho=k_BT/\bar m$ be the common [isothermal sound speed](../../../../isothermal-sound-speed.md) squared. Mass and momentum conservation give

$$
u_1^2+a^2=\frac{u_1^2}{\chi}+a^2\chi,
\qquad (\chi-1)(a^2\chi-u_1^2)=0.
$$

The compressive branch is therefore

$$
\boxed{\chi=\mathcal M_{T,1}^2,\qquad \mathcal M_{T,1}=u_1/a.}
$$

Unlike the adiabatic ratio, it has no fixed upper bound as its upstream Mach number grows. Heat removal prevents the pressure increase that would otherwise resist compression. This approximation describes an efficiently cooled jump between equal-temperature far states, not an adiabatic shock with its energy equation left unchanged. For the same upstream physical temperature and velocity, $\mathcal M_{T,1}=\sqrt\gamma\mathcal M_1$; the two sound-speed conventions must not be confused.

<a id="3/image-bounded-adiabatic-compression-and-increasing-isothermal-compression"></a>
![](../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1-shock-compression.png)

**[Figure 2](#3/image-bounded-adiabatic-compression-and-increasing-isothermal-compression). Bounded adiabatic compression and increasing isothermal compression**. Original comparison for fixed composition. The horizontal Mach coordinate uses each model's own upstream sound speed, so equal plotted Mach numbers do not mean identical upstream temperatures and velocities.

Full dissociation changes the equation of state even when the temperature is held constant. With negligible electron and binding-energy mass corrections, upstream molecular [hydrogen](../../../../hydrogen.md) has $a_1^2=k_BT/(2m_H)$ and downstream atomic [hydrogen](../../../../hydrogen.md) has $a_2^2=k_BT/m_H=2a_1^2$. The conserved quantity is mass flux; particle number flux doubles. Thus

$$
\boxed{\chi=\frac{u_1}{u_2},\qquad
u_1^2+a_1^2=u_1u_2+2a_1^2\frac{u_1}{u_2}.}
$$

Equivalently, the [dissociating isothermal shock](../../../../dissociating-isothermal-shock.md) relation between temperature and the two velocities is

$$
\boxed{a_1^2=\frac{u_1u_2(u_1-u_2)}{2u_1-u_2}.}
$$

Writing $\mathcal M_{T,1}=u_1/a_1$ gives

$$
2\chi^2-(\mathcal M_{T,1}^2+1)\chi+\mathcal M_{T,1}^2=0.
$$

The high-compression branch is

$$
\boxed{\chi=\frac{\mathcal M_{T,1}^2+1+
\sqrt{(\mathcal M_{T,1}^2+1)^2-8\mathcal M_{T,1}^2}}4.}
$$

Its strong-shock limit is $\chi\sim\mathcal M_{T,1}^2/2$, rather than $\mathcal M_{T,1}^2$. The pressure per unit mass has doubled, reducing the compression available at a fixed upstream temperature and speed. A real compressive branch in this prescribed fully dissociated, equal-temperature model requires $\mathcal M_{T,1}\ge1+\sqrt2$; the high root has downstream speed no greater than the downstream isothermal sound speed. These mass and momentum conditions do not themselves establish that sufficient energy is available to dissociate every molecule. The chemical energy and any required radiative loss must also be included in a physical energy budget.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
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
