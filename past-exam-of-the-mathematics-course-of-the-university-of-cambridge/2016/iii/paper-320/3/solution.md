<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [small-angle gravitational encounter](../../../../../small-angle-gravitational-encounter.md) between a test [star](../../../../../star.md) and a field [star](../../../../../star.md) of mass $m$ gives a transverse kick $\Delta v_\perp\simeq2Gm/(bu)$, where $b$ is the impact parameter and $u$ the relative speed. For number density $n$, encounters in $b,b+db$ occur at rate $2\pi b\,db\,nu$. Independent kicks add in mean square, giving the [random-walk derivation of stellar relaxation](../../../../../random-walk-derivation-of-stellar-relaxation.md)

$$
\frac{d\langle\Delta v^2\rangle}{dt}\simeq\frac{8\pi G^2m^2n}{u}\int_{b_{\min}}^{b_{\max}}\frac{db}{b}=\frac{8\pi G^2m^2n}{u}\ln\Lambda.
$$

The [Coulomb logarithm in stellar dynamics](../../../../../coulomb-logarithm-in-stellar-dynamics.md) has $b_{\max}$ of order system size $r_s$, and $b_{\min}$ of order the strong-deflection scale $Gm/u^2$. For a virialized $N$-[star](../../../../../star.md) system, $u^2\sim GNm/r_s$, so $\Lambda$ is of order $N$. The [stellar relaxation time](../../../../../stellar-relaxation-time.md) is the time for accumulated [velocity](../../../../../velocity.md) variance to become comparable with $u^2$:

$$
t_{\mathrm{rel}}\simeq\frac{u^3}{8\pi G^2m^2n\ln\Lambda}.
$$

Using $n\sim3N/(4\pi r_s^3)$ gives $t_{\mathrm{rel}}\sim[N/(6\ln N)]r_s/u$. With a diameter-crossing convention $T_{\mathrm{cross}}\sim2r_s/u$, this is $[N/(12\ln N)]T_{\mathrm{cross}}$, conventionally rounded to

$$
\boxed{T_{\mathrm{relax}}\simeq0.1\frac{N}{\ln N}T_{\mathrm{cross}}.}
$$

The coefficient is approximate: spatial profile, [velocity](../../../../../velocity.md) averages and crossing-time convention change it by factors of order unity. The robust result is $N/\ln N$ crossing times.

For $N\sim10^{10}$ and $T_{\mathrm{cross}}\sim10^8$ years, the estimate is about $4\times10^{15}$ years, enormously longer than a [Hubble time](../../../../../hubble-time.md). Most [galaxies](../../../../../galaxy-split.md) therefore behave as [collisionless stellar systems](../../../../../collisionless-stellar-system.md). Dense nuclei and [star clusters](../../../../../star-cluster.md) can relax more rapidly. Negligible stellar encounters do not mean negligible collective gravitational instabilities.

Define the mass-weighted [galactic distribution function](../../../../../galactic-distribution-function.md) by $dM=F(\mathbf x,\mathbf v,t)d^3x\,d^3v$, so $\rho=\int F\,d^3v$. Hamiltonian gravitational motion preserves [phase space](../../../../../phase-space.md) volume by the [Liouville theorem in Hamiltonian mechanics](../../../../../liouville-s-theorem-hamiltonian.md). In the collisionless regime no encounter term redistributes [stars](../../../../../star.md) between neighbouring [phase space](../../../../../phase-space.md) trajectories, so $dF/dt=0$. With acceleration $\nabla\psi$, the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) is

$$
\partial_tF+\mathbf v\cdot\nabla_{\mathbf x}F+\nabla\psi\cdot\nabla_{\mathbf v}F=0.
$$

For a steadily rotating [galactic bar](../../../../../galactic-bar.md), write the inertial polar angle as $\phi_{\mathrm I}=\phi+\Omega_b t$. The inertial radial and angular equations are $\ddot R-R\dot\phi_{\mathrm I}^2=\psi_R$ and $R\ddot\phi_{\mathrm I}+2\dot R\dot\phi_{\mathrm I}=\psi_\phi/R$. Substitution gives the [equations of motion in a rotating frame](../../../../../equation-of-motion-in-a-rotating-frame.md):

$$
\boxed{\ddot R-R\dot\phi^2=\psi_R+2R\dot\phi\Omega_b+\Omega_b^2R,\qquad R\ddot\phi+2\dot R\dot\phi=\frac{\psi_\phi}{R}-2\dot R\Omega_b.}
$$

Here the [velocities](../../../../../velocity.md) are measured in the bar frame. Set $v_R=\dot R$, $v_\phi=R\dot\phi$ and define the positive-force [rotating-frame relative effective potential](../../../../../rotating-frame-relative-effective-potential.md)

$$
\boxed{\psi_{\mathrm{eff}}=\psi+\frac12\Omega_b^2R^2.}
$$

The centrifugal sign is positive in this relative-potential convention. The characteristics are

$$
\dot R=v_R,\quad\dot\phi=v_\phi/R,\quad\dot v_R=2\Omega_bv_\phi+v_\phi^2/R+\psi_{\mathrm{eff},R},\quad\dot v_\phi=-2\Omega_bv_R-v_Rv_\phi/R+\psi_{\mathrm{eff},\phi}/R.
$$

Consequently the [rotating-frame collisionless Boltzmann equation](../../../../../rotating-frame-collisionless-boltzmann-equation.md) is

$$
\boxed{\begin{aligned}
0={}&F_t+v_RF_R+\frac{v_\phi}{R}F_\phi+\left(2\Omega_bv_\phi+\frac{v_\phi^2}{R}+\psi_{\mathrm{eff},R}\right)F_{v_R}\\
&+\left(-2\Omega_bv_R-\frac{v_Rv_\phi}{R}+\frac{\psi_{\mathrm{eff},\phi}}R\right)F_{v_\phi}.
\end{aligned}}
$$

For these planar equations, integrate over $dv_R\,dv_\phi$ and interpret $\rho$ as the planar or vertically integrated [mass density](../../../../../density.md). Define $\rho\langle A\rangle=\int A F\,dv_R\,dv_\phi$. Boundary terms in [velocity](../../../../../velocity.md) vanish for a sufficiently decaying distribution.

Let the [velocity](../../../../../velocity.md) accelerations above be $A_R,A_\phi$. Their [velocity](../../../../../velocity.md) divergence is $\partial_{v_R}A_R+\partial_{v_\phi}A_\phi=-v_R/R$. Thus [integration by parts](../../../../../integration-by-parts.md) in the zeroth moment contributes $\rho\langle v_R\rangle/R$, producing the [cylindrical continuity equation for a rotating stellar system](../../../../../cylindrical-continuity-equation-for-a-rotating-stellar-system.md)

$$
\boxed{\partial_t\rho+\frac1R\partial_R[R\rho\langle v_R\rangle]+\frac1R\partial_\phi[\rho\langle v_\phi\rangle]=0.}
$$

This is conservation of mass: change of density balances flux through the radial and azimuthal sides of a small cylindrical element. The factor $R$ is geometric; the physical [phase space](../../../../../phase-space.md) measure is $R\,dR\,d\phi\,dv_R\,dv_\phi$.

For the radial first moment, multiply the [rotating-frame collisionless Boltzmann equation](../../../../../rotating-frame-collisionless-boltzmann-equation.md) by $v_R$. Its [velocity](../../../../../velocity.md) integrations are $\int v_RA_RF_{v_R}\,d^2v=-\rho\langle A_R\rangle$ and $\int v_RA_\phi F_{v_\phi}\,d^2v=\rho\langle v_R^2\rangle/R$. Hence the radial [cylindrical Jeans equations in a rotating frame](../../../../../cylindrical-jeans-equations-in-a-rotating-frame.md) are

$$
\boxed{\begin{aligned}
\partial_t(\rho\langle v_R\rangle)&+\partial_R(\rho\langle v_R^2\rangle)+\frac1R\partial_\phi(\rho\langle v_Rv_\phi\rangle)\\
&-2\Omega_b\rho\langle v_\phi\rangle+\frac\rho R(\langle v_R^2\rangle-\langle v_\phi^2\rangle)=\rho\psi_{\mathrm{eff},R}.
\end{aligned}}
$$

For the azimuthal first moment, the $A_R$ [velocity](../../../../../velocity.md) integral vanishes, while $\partial_{v_\phi}(v_\phi A_\phi)=\psi_{\mathrm{eff},\phi}/R-2\Omega_bv_R-2v_Rv_\phi/R$. This gives

$$
\boxed{\begin{aligned}
\partial_t(\rho\langle v_\phi\rangle)&+\partial_R(\rho\langle v_Rv_\phi\rangle)+\frac1R\partial_\phi(\rho\langle v_\phi^2\rangle)\\
&+2\Omega_b\rho\langle v_R\rangle+\frac{2\rho\langle v_Rv_\phi\rangle}{R}=\frac\rho R\psi_{\mathrm{eff},\phi}.
\end{aligned}}
$$

The [Jeans equations](../../../../../jeans-equation.md) are local momentum-balance equations. The second moments include streaming momentum flux and random-[velocity](../../../../../velocity.md) stress, while gravity, centrifugal acceleration and Coriolis acceleration supply the frame-dependent forces. They do not by themselves close the full distribution: a stress prescription or a [galactic distribution function](../../../../../galactic-distribution-function.md) is also needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 320](../../paper-320-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
