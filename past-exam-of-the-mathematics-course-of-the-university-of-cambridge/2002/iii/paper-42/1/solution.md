<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [stellar polytrope](../../../../../stellar-polytrope.md) has a spatially constant coefficient $K$ in the relation $P=K\rho^{1+1/n}$; $n$ is its [polytropic index](../../../../../polytropic-index.md). This relates [pressure](../../../../../pressure.md) to [mass density](../../../../../density.md) and need not describe an adiabatic gas. Combining [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) with [mass conservation](../../../../../mass-conservation.md) eliminates the enclosed [mass](../../../../../mass.md):

$$
\frac{1}{r^2}\frac{d}{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

For $\rho=\rho_c\theta^n$, the [polytropic equation of state](../../../../../polytropic-equation-of-state.md) gives $(1/\rho)dP/dr=(n+1)K\rho_c^{1/n}d\theta/dr$. Choose the [Lane-Emden variables for a stellar polytrope](../../../../../lane-emden-variables-for-a-stellar-polytrope.md) with

$$
\alpha^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1},\qquad r=\alpha\xi.
$$

Substitution then gives the dimensionless [Lane-Emden equation](../../../../../lane-emden-equation.md):

$$
\boxed{\frac{1}{\xi^2}(\xi^2\theta')'=-\theta^n.}
$$

A regular stellar centre has $\theta(0)=1$, $\theta'(0)=0$ and $m(0)=0$. In particular the regular central expansion is $\theta=1-\xi^2/6+O(\xi^4)$. For an isolated finite-radius [stellar polytrope](../../../../../stellar-polytrope.md) with negligible external [pressure](../../../../../pressure.md), the surface is the first zero $\xi_1$ of $\theta$, and $R=\alpha\xi_1$. A core embedded in an envelope can instead end at a positive matching [pressure](../../../../../pressure.md), before this zero.

The integrated [Lane-Emden equation](../../../../../lane-emden-equation.md) is $\xi^2\theta'=-\int_0^\xi s^2\theta(s)^n ds$. Thus [mass conservation](../../../../../mass-conservation.md) gives the [Lane-Emden mass formula](../../../../../lane-emden-mass-formula.md) directly:

$$
\boxed{m(\xi)=-4\pi\rho_c\alpha^3\xi^2\theta'(\xi).}
$$

For the proposed functional form, differentiation gives

$$
\theta''+\frac{2}{\xi}\theta'=2\beta\gamma(1+\beta\xi^2)^{\gamma-2}\bigl[3+(2\gamma+1)\beta\xi^2\bigr].
$$

Choosing $\gamma=-1/2$ removes the extra polynomial factor; equality to $-\theta^5$ then requires $3\beta=1$. The regular [polytrope of index five](../../../../../polytrope-of-index-five.md) is therefore

$$
\boxed{\beta=\frac13,\quad\gamma=-\frac12,\quad\theta=(1+\xi^2/3)^{-1/2}.}
$$

Its enclosed [mass](../../../../../mass.md) and enclosed mean [mass density](../../../../../density.md) are

$$
m(\xi)=\frac{4\pi\rho_c\alpha^3\xi^3}{3(1+\xi^2/3)^{3/2}},\qquad
\overline\rho(\xi)=\frac{3m}{4\pi r^3}=\rho_c(1+\xi^2/3)^{-3/2}.
$$

There is no finite zero: its isolated radius is infinite. Nevertheless its total [mass](../../../../../mass.md) converges, since the outer [mass density](../../../../../density.md) falls as $r^{-5}$:

$$
\boxed{M=4\pi\sqrt3\rho_c\alpha^3,\qquad R=\infty,\qquad\lim_{r\to\infty}\overline\rho(r)=0.}
$$

The zero mean [mass density](../../../../../density.md) is a limiting volume average, not a statement that the material has zero [mass density](../../../../../density.md) at finite radius.

To turn this density model into a [CNO cycle](../../../../../cno-cycle.md) burning model, use gas-dominated [pressure](../../../../../pressure.md) and uniform [mean molecular weight](../../../../../mean-molecular-weight.md). The [ideal gas law](../../../../../ideal-gas-law.md) and the [polytropic equation of state](../../../../../polytropic-equation-of-state.md) then imply $T/T_c=\theta$. Without this thermal assumption a [polytropic equation of state](../../../../../polytropic-equation-of-state.md) for total [pressure](../../../../../pressure.md) does not alone fix the [temperature](../../../../../temperature.md) profile. Since the [stellar energy-generation rate](../../../../../stellar-energy-generation-rate.md) is power per unit [mass](../../../../../mass.md), its contribution to [luminosity](../../../../../luminosity.md) is $\epsilon\,dm$, giving the [luminosity integral of an index-five polytrope](../../../../../luminosity-integral-of-an-index-five-polytrope.md):

$$
L=4\pi\epsilon_0\alpha^3\rho_c^2T_c^{11}\int_0^\infty\xi^2(1+\xi^2/3)^{-21/2}\,d\xi.
$$

Put $u=\xi/\sqrt{3+\xi^2}$. Then $\xi=\sqrt3u/\sqrt{1-u^2}$ and the dimensionless integral becomes $3\sqrt3\int_0^1u^2(1-u^2)^8du$. Evaluation gives

$$
A=12\pi\sqrt3\frac{8!\,9!\,2^{17}}{19!}=1.029415\ldots,\qquad
\boxed{L=A\epsilon_0\alpha^3\rho_c^2T_c^{11},\quad A\sim1.}
$$

The PDF's power of $\alpha$ in the proposed [luminosity](../../../../../luminosity.md) scaling is a genuine dimensional error: it must be three, rather than two. The volume element supplies $\alpha^3$; replacing it by $\alpha^2$ would give power divided by length, and could not be repaired by a dimensionless numerical constant.

The [polytrope of index five](../../../../../polytrope-of-index-five.md) is unlikely to model a real burning [stellar core](../../../../../stellar-core.md) well. An embedded core has a finite boundary, and a complete isolated star cannot have this infinite radius. More importantly, strongly [temperature](../../../../../temperature.md)-sensitive [CNO cycle](../../../../../cno-cycle.md) heating concentrates the [luminosity](../../../../../luminosity.md) centrally and tends to produce a [convection zone](../../../../../convection-zone.md) there. A well-mixed gas-pressure-dominated convective core is closer to an [adiabatic stellar polytrope](../../../../../adiabatic-stellar-polytrope.md) of index $3/2$ than to index five. A finite truncation would also change the integral defining $A$; its value above pertains to the full mathematical model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
