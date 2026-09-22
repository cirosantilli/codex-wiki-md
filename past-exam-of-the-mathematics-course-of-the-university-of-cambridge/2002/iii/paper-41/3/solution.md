<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix the sign convention first: depth $z$ increases downward, while the vertical displacement amplitude $\xi$ is positive upward. Write $\Pi=\delta p$ for the [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md), and $p_1,\rho_1$ for [Eulerian fluid perturbations](../../../../../eulerian-fluid-perturbation.md). [Hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) gives $dp/dz=\rho g$, and the adiabatic relation gives $\delta\rho=\Pi/c^2$. Since the vertical displacement vector has component $-\xi$ along increasing $z$,

$$
p_1=\Pi+\rho g\xi,\qquad\rho_1=\Pi/c^2+(d\rho/dz)\xi.
$$

In the [Cowling approximation](../../../../../cowling-approximation.md), horizontal momentum gives $\boldsymbol\xi_h=i\boldsymbol k p_1/(\rho\omega^2)$. The [mass conservation](../../../../../mass-conservation.md) equation $\delta\rho=-\rho(i\boldsymbol k\cdot\boldsymbol\xi_h-\xi')$ and vertical momentum $\omega^2\rho\xi=-p_1'+g\rho_1$ then eliminate the horizontal displacement. The [plane-parallel Cowling displacement-pressure equations](../../../../../plane-parallel-cowling-displacement-pressure-equations.md) are

$$
\boxed{\begin{aligned}
\xi'&=-\frac{gk^2}{\omega^2}\xi-\left(\frac{k^2}{\omega^2}-\frac1{c^2}\right)\frac\Pi\rho,\\
\Pi'&=-\rho\left(\omega^2-\frac{g^2k^2}{\omega^2}\right)\xi+\frac{gk^2}{\omega^2}\Pi.
\end{aligned}}
$$

For $\omega^2=gk$, the second equation admits $\Pi=0$ and the first reduces to $\xi'=-k\xi$. Thus the [plane-parallel stellar f-mode](../../../../../plane-parallel-stellar-f-mode.md) has

$$
\boxed{\omega^2=gk,\quad\xi=C e^{-k(z-z_0)},\quad\Pi=0,\quad\boldsymbol\xi_h=i\boldsymbol k\xi/k.}
$$

Its Eulerian eigenfunctions are $p_1=\rho g\xi$ and $\rho_1=\rho'\xi$, while $\delta\rho=0$. Hence it has no Lagrangian compression even in a stratified star. It decays inward but grows upward, explaining the failure of a pure small-amplitude continuation to $z\to-\infty$.

For the lower part of the [matched chromospheric interfacial mode](../../../../../matched-chromospheric-interfacial-mode.md), put $\omega^2=gk(1-\varepsilon)$, $\xi=e^{-k(z-z_0+\varepsilon\phi)}$ and $\Pi=\varepsilon f\xi$. The pressure amplitude is of order $\varepsilon$ because the limiting f-mode has identically zero Lagrangian pressure amplitude; the frequency correction perturbs that zero solution. Expand $gk^2/\omega^2=k(1+\varepsilon)+O(\varepsilon^2)$ and $\omega^2-g^2k^2/\omega^2=-2gk\varepsilon+O(\varepsilon^2)$. The leading equations are

$$
\boxed{\phi'=1+\frac f\rho\left(\frac1g-\frac1{kc^2}\right),\qquad f'-2kf=2gk\rho.}
$$

Exclude the lower homogeneous component $f\propto e^{2kz}$, which would make $\Pi$ grow into the star. Integrating the remaining equation with its integrating factor gives

$$
\boxed{f(z)=-2gk e^{2k(z-z_0)}\int_z^\infty e^{-2k(z'-z_0)}\rho(z')\,dz'.}
$$

The accompanying correction is $\phi(z)=\int_{z_0}^z[1+(f/\rho)(1/g-1/(kc^2))]\,ds$, with the integrand evaluated at $s$. This fixes $\phi(z_0)=0$ and determines the lower eigenfunctions to the stated order.

For the upper part, distinguish the rescaled sound speed by writing $\rho=\varepsilon\widehat\rho$ and $c^2=\varepsilon^{-1}\widehat c^2$. Set $\Pi=\varepsilon\psi$, $\psi=Ae^{k(z-z_0+\varepsilon\phi)}$ and $\xi=\mu\psi$. To leading order the first displacement equation becomes $\xi'=-k\xi-k\psi/(g\widehat\rho)$, while the pressure equation gives $\psi'=k\psi+\varepsilon[k\psi+2gk\widehat\rho\xi]+O(\varepsilon^2)$. Consequently

$$
\boxed{\mu'+2k\mu=-\frac{k}{g\widehat\rho},\qquad\phi'=1+2g\widehat\rho\mu.}
$$

The component $\mu\propto e^{-2kz}$ would give $\xi\propto e^{-kz}$, which diverges upward. Remove it by the upper boundary condition. The leading upper solution is

$$
\boxed{\mu(z)=-\frac{k}{g}e^{-2k(z-z_0)}\int_{-\infty}^z\frac{e^{2k(z'-z_0)}}{\widehat\rho(z')}\,dz',\qquad\psi(z)\simeq Ae^{k(z-z_0)}.}
$$

Integrating $\phi'$ with $\phi(z_0)=0$ gives the first correction to the upper exponential. The displayed $\xi=\mu\psi$ satisfies the required decay only for compatible upper density profiles; integral convergence alone is not the full boundary condition.

To match, define the positive weighted integrals

$$
I_b=\int_{z_0}^\infty e^{-2k(z-z_0)}\rho(z)\,dz,\qquad
I_a=\int_{-\infty}^{z_0}\frac{e^{2k(z-z_0)}}{\rho(z)}\,dz.
$$

The lower normalization is $\xi(z_0)=1$ and $f(z_0)=-2gkI_b$. Continuity of [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md) makes the upper $A=f(z_0)$; continuity of [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) then requires $\mu(z_0)A=1$. Since $1/\widehat\rho=\varepsilon/\rho$, the upper integral gives $\mu(z_0)=-(k/g)\varepsilon I_a$. The two matching conditions therefore give

$$
\boxed{\varepsilon^{-1}\simeq2k^2 I_a I_b.}
$$

As a sign and normalization check, two incompressible constant-density layers give $I_a=(2k\rho_a)^{-1}$ and $I_b=\rho_b/(2k)$, so $\varepsilon\simeq2\rho_a/\rho_b$. This agrees with expansion of the exact [interfacial gravity-wave dispersion relation](../../../../../interfacial-gravity-wave-dispersion-relation.md) $\omega^2=gk(\rho_b-\rho_a)/(\rho_b+\rho_a)$.

For validity, require $\varepsilon\ll1$, convergent weighted integrals, a matching level separating the low-density high-sound-speed atmosphere from the denser envelope, and small accumulated corrections $\varepsilon k|\phi|$ over the regions carrying the matching integrals. The upper expansion also needs $g/(kc^2)\ll1$. The resulting upper displacement must tend to zero: for example if $\widehat\rho\propto e^{a(z-z_0)}$ at great height, its leading amplitude is proportional to $e^{(k-a)(z-z_0)}$, requiring $a<k$; the weaker condition $a<2k$ merely makes the upper integral converge. Plane geometry, constant $g$ and the [Cowling approximation](../../../../../cowling-approximation.md) must be appropriate on the wavelength scale. The physical mode amplitude must remain small compared with both its wavelength and local background scale heights, so the [adiabatic fluid perturbation](../../../../../adiabatic-fluid-perturbation.md) remains linear. If these requirements fail, neither the matching formula nor continuation of the leading expansions is controlled.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
