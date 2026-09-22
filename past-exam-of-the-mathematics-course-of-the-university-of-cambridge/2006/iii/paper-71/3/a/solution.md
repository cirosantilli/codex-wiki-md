<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A fully ionized [helium](../../../../../../helium.md) nucleus supplies two [Electrons](../../../../../../electron.md) for approximately $4m_p$ of [mass](../../../../../../mass.md), so $n_e=\rho/(2m_p)$. Filling all [Electron](../../../../../../electron.md) [momentum](../../../../../../momentum.md) states up to the [Fermi momentum](../../../../../../fermi-momentum.md) gives

$$
n_e=\int_0^{p_0}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^3}{3h^3},\qquad
p_0=\left(\frac{3h^3\rho}{16\pi m_p}\right)^{1/3}.
$$

For a nonrelativistic [Electron](../../../../../../electron.md), the speed is $p/m_e$. The three mean squared Cartesian components of [momentum](../../../../../../momentum.md) are equal by rotational symmetry and sum to $p^2$, so each is $p^2/3$. This is the [isotropic tensor integral](../../../../../../isotropic-tensor-integral.md). Thus the [momentum flux](../../../../../../momentum-flux.md), or [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md), is

$$
P_e=\frac13\int_0^{p_0}\frac{p^2}{m_e}\frac{8\pi p^2}{h^3}dp
=\frac{8\pi p_0^5}{15m_eh^3}.
$$

Substituting the expression for $p_0$ and simplifying the powers of two gives

$$
\boxed{P_e=K\rho^{5/3},\qquad
K=\left(\frac3{2\pi}\right)^{2/3}\frac{h^2}{40m_em_p^{5/3}}.}
$$

Here $h$ is the [Planck constant](../../../../../../planck-constant.md). This is the pure-helium specialization of [nonrelativistic electron-degeneracy pressure in a hydrogen-helium mixture](../../../../../../nonrelativistic-electron-degeneracy-pressure-in-a-hydrogen-helium-mixture.md).

For a cold [helium white dwarf](../../../../../../helium-white-dwarf.md), neglect ion thermal [pressure](../../../../../../pressure.md) and use this [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) as the support against [Newtonian gravity](../../../../../../gravitational-acceleration.md). Combining [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) with [mass conservation](../../../../../../mass-conservation.md) gives

$$
\frac1{r^2}\frac d{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

Set $\rho=\rho_c\theta^{3/2}$ and $r=\alpha\xi$, where $\alpha^2=5K\rho_c^{-1/3}/(8\pi G)$. Direct substitution gives the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\frac1{\xi^2}\frac d{d\xi}(\xi^2\theta')=-\theta^{3/2},\qquad\theta(0)=1,\quad\theta'(0)=0.
$$

Its [dimensionless](../../../../../../dimensionless-quantity.md) solution is independent of $\rho_c$. Let $\xi_1$ be its first zero and $\omega_1=-\xi_1^2\theta'(\xi_1)=\int_0^{\xi_1}\xi^2\theta^{3/2}d\xi$. Integrating [mass conservation](../../../../../../mass-conservation.md) gives

$$
R=\alpha\xi_1,\qquad M=4\pi\alpha^3\rho_c\omega_1.
$$

Eliminating $\rho_c$ yields the [polytropic mass-radius relation](../../../../../../polytropic-mass-radius-relation.md)

$$
\boxed{R=AM^{-1/3},\qquad
A=\frac{5K}{8\pi G}\,\xi_1(4\pi\omega_1)^{1/3}.}
$$

Thus a more massive [nonrelativistic white dwarf](../../../../../../nonrelativistic-white-dwarf.md) is smaller at fixed [stellar composition](../../../../../../stellar-chemical-abundance.md). The assumptions require $p_0\ll m_ec$ and $k_BT\ll p_0^2/(2m_e)$ in the region providing most support; the law is not extended into the relativistic or thermally supported regimes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
