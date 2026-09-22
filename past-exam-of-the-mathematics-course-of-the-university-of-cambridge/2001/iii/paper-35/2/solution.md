<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The energy-conserving [self-similar blast wave](../../../../../self-similar-blast-wave.md) requires a stage in which the original stellar radius, ejecta mass, ambient [pressure](../../../../../pressure.md) and cooling have ceased to supply important scales. In particular, the swept-up [mass](../../../../../mass.md) must greatly exceed the ejecta mass; $R\gg R_*$ alone need not ensure this in a very dilute [interstellar medium](../../../../../interstellar-medium.md). For fixed explosion [energy](../../../../../energy.md) $E$, uniform ambient [mass density](../../../../../density.md) $\rho_0$ and elapsed time $t$, [dimensional analysis](../../../../../dimensional-analysis.md) gives $R=C E^a\rho_0^b t^d$. Matching mass, length and time gives $a=1/5$, $b=-1/5$, $d=2/5$. Equivalently, a self-similar strong [shock wave](../../../../../shock-wave.md) has $E\sim\rho_0R^3\dot R^2$, whose constant-energy solution has the same exponents:

$$
\boxed{R=\xi_0(E/\rho_0)^{1/5}t^{2/5}.}
$$

The dimensionless coefficient depends on $\gamma$ and the post-shock profiles; dimensional reasoning cannot fix it.

For completeness, obtain the [Strong-shock Rankine-Hugoniot conditions](../../../../../strong-shock-rankine-hugoniot-conditions.md) in the [shock frame](../../../../../shock-frame.md). Let $v_1=V-u$ denote downstream speed relative to the outward-moving front. With negligible upstream [pressure](../../../../../pressure.md) and [enthalpy](../../../../../enthalpy.md), conservation of [mass](../../../../../mass.md), [momentum](../../../../../momentum.md) and [energy](../../../../../energy.md) gives

$$
\rho_0V=\rho_1v_1,\qquad
\rho_0V^2=p_1+\rho_1v_1^2,\qquad
\frac{V^2}{2}=\frac{v_1^2}{2}+\frac{\gamma p_1}{(\gamma-1)\rho_1}.
$$

Put $q=\rho_1/\rho_0$. Substituting $v_1=V/q$ into the last two equations and selecting the compressive, nontrivial branch yields $q=(\gamma+1)/(\gamma-1)$. Hence

$$
\boxed{\rho_1=\frac{\gamma+1}{\gamma-1}\rho_0,\quad
p_1=\frac{2}{\gamma+1}\rho_0V^2,\quad
u=\frac{2}{\gamma+1}V.}
$$

Here the symbol $u$, written as $u=2V/(\gamma+1)$ in what follows, is the laboratory-frame radial [velocity](../../../../../velocity.md); it is not the relative speed $v_1$.

Use the [thin-shell approximation for a spherical blast wave](../../../../../thin-shell-approximation-for-a-spherical-blast-wave.md). Set $W=4\pi R^3/3$ and $M_s=\rho_0W$. Equating the swept-up [mass](../../../../../mass.md) to $4\pi R^2d\rho_1$ gives $d/R=(\gamma-1)/[3(\gamma+1)]$. The growing shell's [momentum](../../../../../momentum.md) is $M_su$. Since newly swept gas has zero laboratory [momentum](../../../../../momentum.md), the net force is the cavity [pressure](../../../../../pressure.md) acting on the inner shell, to thin-shell accuracy:

$$
\frac{d}{dt}(M_su)=4\pi R^2p_c,
\qquad p_c=\alpha p_1.
$$

The pressure at the shock is already accounted for by the jump conditions and mass loading; subtracting $p_1$ as an additional external pressure would count the shock reaction twice. With $u=2V/(\gamma+1)$, the last equation becomes

$$
R\dot V+3V^2=3\alpha V^2,\qquad
\frac{d\ln V}{d\ln R}=3(\alpha-1).
$$

Therefore, for constant $\alpha$,

$$
\boxed{\dot R=K R^{3(\alpha-1)}.}
$$

The shell volume is $M_s/\rho_1=W/q$. Its internal [energy](../../../../../energy.md) and [kinetic energy](../../../../../kinetic-energy.md) are

$$
E_{s,\rm int}=\frac{p_1W}{q(\gamma-1)}=\frac{2\rho_0WV^2}{(\gamma+1)^2},\qquad
E_{s,\rm kin}=\frac12M_su^2=\frac{2\rho_0WV^2}{(\gamma+1)^2}.
$$

Treat the cavity volume as $W$ at the same thin-shell level, so its internal [energy](../../../../../energy.md) is $E_{c,\rm int}=\alpha p_1W/(\gamma-1)$. Their sum is proportional to $R^3V^2$ for constant $\alpha$ and $\gamma$. Constant total [energy](../../../../../energy.md) thus requires $3+6(\alpha-1)=0$, giving **$\alpha=1/2$**. Consequently

$$
E=\rho_0WV^2\frac{5\gamma-3}{(\gamma-1)(\gamma+1)^2}.
$$

Using $V=2R/(5t)$, this becomes

$$
\boxed{\xi_0^5=\frac{75}{16\pi}\frac{(\gamma-1)(\gamma+1)^2}{5\gamma-3}.}
$$

For $\gamma=5/3$, $d/R=1/12$ and the approximate [energy](../../../../../energy.md) fractions are $E_{s,\rm kin}/E=1/4$, $E_{s,\rm int}/E=1/4$, $E_{c,\rm int}/E=1/2$.

This is an approximate normalization, not an exact treatment of finite shell thickness. If instead one subtracts the shell volume and uses $W_c=W(1-1/q)$ for the cavity, while retaining the other shell assumptions, the energy coefficient becomes $2(2\gamma-1)/[(\gamma-1)(\gamma+1)^2]$ and $\xi_0^5=75(\gamma-1)(\gamma+1)^2/[32\pi(2\gamma-1)]$. The difference is an order-$d/R$ geometric correction of this crude shell model; a consistent exact coefficient requires the full self-similar profiles.

In the idealized mass budget all swept gas is assigned to the shell, so the cavity inertia is neglected. The hot cavity's residual [mass density](../../../../../density.md) is not specified, so its [kinetic energy](../../../../../kinetic-energy.md) cannot be assigned a unique numerical fraction from the stated data. If its low mass is $M_c$ and its [velocity](../../../../../velocity.md) is of order $u$, then $E_{c,\rm kin}\sim M_cu^2/2$ and

$$
\frac{E_{c,\rm kin}}{E}\sim\frac{M_c}{M_s}\frac{2(\gamma-1)}{5\gamma-3}\ll1
\quad\text{when }M_c\ll M_s.
$$

For an illustrative uniform-density cavity with homologous [velocity](../../../../../velocity.md) $v(r)=ur/R$, direct radial integration gives $E_{c,\rm kin}=3M_cu^2/10$, so the preceding fraction has an extra factor $3/5$. The cavity can carry substantial internal [energy](../../../../../energy.md) despite negligible [kinetic energy](../../../../../kinetic-energy.md) because it is hot. Neglect of its inertia is justified in the swept-mass-dominated stage, not merely by its small initial radius.

The calculation describes the adiabatic expansion stage of a [supernova remnant](../../../../../supernova-remnant.md), giving an estimate of its age or explosion [energy](../../../../../energy.md) from its radius, expansion speed and ambient [mass density](../../../../../density.md). For example $t\simeq2R/(5V)$, and $E\propto\rho_0R^3V^2$. Such blasts inject [energy](../../../../../energy.md) and [momentum](../../../../../momentum.md) into the [interstellar medium](../../../../../interstellar-medium.md) and redistribute stellar ejecta. The early ejecta-dominated stage, radiatively cooled late shell, nonuniform ambient medium, finite ambient [sound speed](../../../../../speed-of-sound.md), [magnetic fields](../../../../../magnetic-field.md), nonspherical geometry and energy transfer to [cosmic rays](../../../../../cosmic-ray.md) violate different assumptions. Even in the adiabatic spherical stage, the real profiles are not a uniform thin shell and a uniform-pressure cavity, so $\xi_0$ here is an estimate.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
