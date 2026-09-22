<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Stellar rotation](../../../../../stellar-rotation.md) is a problem of coupled force balance, heat transport and [angular momentum transport](../../../../../angular-momentum-transport.md). A [star](../../../../../star.md) need not rotate as a rigid body: in the [Sun](../../../../../sun.md), the convective envelope rotates faster near the equator than near the poles, while much of the radiative interior rotates more nearly uniformly. The [tachocline](../../../../../tachocline.md) is the thin transition near the base of the convection zone. Surface tracking and [Doppler effect](../../../../../doppler-effect.md) measurements constrain the exterior flow; [solar rotational mode splitting](../../../../../solar-rotational-mode-splitting.md) in [helioseismology](../../../../../helioseismology.md) constrains interior [stellar rotation](../../../../../stellar-rotation.md) through integrals of the form $\delta\omega_{n\ell m}\simeq m\int K_{n\ell m}\Omega\,dV$. Multiple kernels are needed, so surface rotation is not a measurement of every depth.

A useful mean [velocity](../../../../../velocity.md) decomposition is $\mathbf U=\varpi\Omega\mathbf e_\phi+\mathbf v_m$, where $\varpi=r\sin\theta$ is distance from the axis and $\mathbf v_m$ is [stellar meridional circulation](../../../../../meridional-circulation-in-a-star.md). In a frame of constant angular velocity $\boldsymbol\Omega_0$, use the relative [velocity](../../../../../velocity.md) $\mathbf V=\mathbf U-\boldsymbol\Omega_0\times\mathbf r$. Its momentum equation includes

$$
\frac{D\mathbf V}{Dt}+2\boldsymbol\Omega_0\times\mathbf V
=-\frac{\nabla p}{\rho}-\nabla\left(\Phi-\frac12\Omega_0^2\varpi^2\right)
+\frac{(\nabla\times\mathbf B)\times\mathbf B}{\mu_0\rho}
+\frac{1}{\rho}\nabla\cdot\boldsymbol\tau.
$$

The [Coriolis force](../../../../../coriolis-force.md) changes the direction of a parcel's motion but does no work. Thermal driving, release of differential rotational [kinetic energy](../../../../../kinetic-energy.md), contraction, or external torques supply the energy of the flows. Solid-body [stellar rotation](../../../../../stellar-rotation.md) in a suitable [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) does not by itself require a meridional flow.

For slowly circulating, approximately axisymmetric material, the leading mechanical balance in an inertial frame is $\nabla p/\rho=-\nabla\Phi+\varpi\Omega^2\mathbf e_\varpi$. Taking its [curl](../../../../../curl.md) gives the [stellar thermal-wind balance](../../../../../stellar-thermal-wind-balance.md)

$$
\varpi\partial_z\Omega^2=\frac{(\nabla p\times\nabla\rho)_\phi}{\rho^2}
\simeq\frac{g}{rc_p}\partial_\theta S.
$$

Here $z$ is the axial coordinate, $S$ is specific [entropy](../../../../../entropy.md) and $c_p$ is the specific heat at fixed [pressure](../../../../../pressure.md). The last form uses approximately radial [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) and uniform composition. If the material is [barotropic](../../../../../barotropic-fluid.md), the right-hand side vanishes and angular velocity is constant on cylinders. Small latitudinal [entropy](../../../../../entropy.md) differences can instead support the observed noncylindrical [differential rotation](../../../../../differential-rotation.md). Stresses and inertial terms modify this leading balance. The equation relates shear to [baroclinicity](../../../../../baroclinity.md); it does not give the circulation speed or explain how the shear is maintained.

That second question requires an angular-momentum budget. With $j=\varpi^2\Omega$ and density-weighted mean quantities, [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) can be written schematically as

$$
\partial_t(\rho j)+\nabla\cdot(\rho\mathbf v_m j+\mathbf F_J)=0,
$$



$$
\mathbf F_J=\rho\varpi\langle u'_\phi\mathbf u'_m\rangle
-\frac{\varpi}{\mu_0}\langle B_\phi\mathbf B_m\rangle
-\rho\nu\varpi^2\nabla\Omega.
$$

The three contributions are [Reynolds stress](../../../../../reynolds-stress.md), magnetic [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) and [viscosity](../../../../../dynamic-viscosity.md) transport. Appropriate density weighting replaces the simple correlations in a strongly compressible average. Since $\nabla\cdot(\rho\mathbf v_m)=0$ in a steady star, the stationary equation gives [gyroscopic pumping in a star](../../../../../gyroscopic-pumping-in-a-star.md):

$$
\boxed{\rho\mathbf v_m\cdot\nabla j=-\nabla\cdot\mathbf F_J.}
$$

A torque that maintains [differential rotation](../../../../../differential-rotation.md) therefore drives a meridional response unless another stress cancels it. Conversely the circulation transports [angular momentum](../../../../../angular-momentum.md) and feeds back on the rotation. An assumed meridional pattern without its driving torque is not a closed dynamical model.

In the convection zone, outward heat transport drives [convection](../../../../../convection.md). Rotation deflects the rising and falling parcels and makes their correlations anisotropic. [Nondiffusive convective angular momentum transport](../../../../../nondiffusive-convective-angular-momentum-transport.md) can drive shear even from an initially uniform rotation rate; treating every [Reynolds stress](../../../../../reynolds-stress.md) as a positive eddy [viscosity](../../../../../dynamic-viscosity.md) would only smooth shear and miss its source. A limiting parcel that conserves $j$ when it moves outwards slows relative to uniform rotation, whereas rapid rotational constraint and correlated horizontal motions change the sign and direction of the net transport. Thus the solar equator-fast pattern requires the actual convective correlations, not a universal parcel argument. The [Rossby number](../../../../../rossby-number.md) $u_c/(2\Omega\ell_c)$ compares convective inertia with rotational deflection: deep, slower, larger-scale [convection](../../../../../convection.md) is more rotationally constrained than the fastest photospheric motions. Turnover times $\ell_c/u_c$ range from minutes near the visible surface to weeks or longer at greater depth. On these times the [Reynolds stresses](../../../../../reynolds-stress.md) can redistribute angular momentum and drive circulation, while the star's total spin changes much more slowly.

In a radiative region, rotation distorts [equipotential surfaces](../../../../../equipotential-surface.md). Under uniform rotation and uniform composition, leading [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) makes pressure, density and temperature constant on each such surface, but effective gravity varies along it. [Radiative diffusion](../../../../../radiative-diffusion.md) then produces a flux $\mathbf F=f(\Phi_{\rm eff})\nabla\Phi_{\rm eff}$. Its divergence contains $f'|\nabla\Phi_{\rm eff}|^2$, which varies over a surface and generally cannot match a nuclear source constant there. This is the [radiative-equilibrium obstruction in a rotating barotropic star](../../../../../radiative-equilibrium-obstruction-in-a-rotating-barotropic-star.md). Thermal imbalance drives [Eddington-Sweet circulation](../../../../../eddington-sweet-circulation.md), with heat advection entering

$$
\rho T\left(\partial_t S+\mathbf v_m\cdot\nabla S\right)
=\rho\epsilon_{\rm nuc}-\nabla\cdot\mathbf F+\text{dissipative heating}.
$$

Its global thermal estimate is

$$
\epsilon_\Omega\sim\frac{\Omega^2R^3}{GM},\qquad
\boxed{t_{\rm ES}\sim\frac{t_{\rm KH}}{\epsilon_\Omega},\quad t_{\rm KH}\sim\frac{GM^2}{RL}.}
$$

A rotational thermal imbalance of order $\epsilon_\Omega L$ processes the thermal reservoir on this longer time. For the slowly rotating [Sun](../../../../../sun.md), $t_{\rm KH}$ is of order $3\times10^7$ years and $\epsilon_\Omega$ of order $2\times10^{-5}$, giving $t_{\rm ES}\sim10^{12}$ years, much longer than the solar age. Stable composition gradients impede the flow further. Thus classical radiative [Eddington-Sweet circulation](../../../../../eddington-sweet-circulation.md) cannot by itself establish the Sun's interior rotation rapidly. In a rapidly rotating star the same estimate is shorter and rotational mixing can compete with its evolutionary lifetime. Torque-driven convection-zone circulation and radiative thermal circulation have different controlling balances.

[Magnetic fields](../../../../../magnetic-field.md) introduce a further coupling. A [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) linking different layers is wound by differential rotation into a [toroidal magnetic field](../../../../../toroidal-magnetic-field.md), roughly $\partial_tB_\phi\simeq\varpi\mathbf B_p\cdot\nabla\Omega$. The resulting [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) transport angular momentum. Communication along a field occurs on an [Alfvén speed](../../../../../alfven-speed.md) crossing time $t_A\sim\ell\sqrt{\mu_0\rho}/B$, which can be far shorter than molecular diffusion if a coherent connecting field exists. In steady ideal axisymmetric induction, absence of continuing winding requires $\mathbf B_p\cdot\nabla\Omega=0$; this is constancy along the field, not automatically solid-body rotation throughout the star. The topology and strength of an interior field matter. [Solar dynamo](../../../../../solar-dynamo.md) action, especially the interaction of shear with poloidal-field regeneration, couples [stellar rotation](../../../../../stellar-rotation.md) to the magnetic cycle. Magnetic feedback can change shear and circulation on dynamical or cycle times; an approximately eleven-year activity cycle and twenty-two-year magnetic polarity cycle are distinct from secular spin-down.

A magnetized [stellar wind](../../../../../stellar-wind.md) also supplies an external torque. It enforces approximate corotation out to an effective [Alfvén radius](../../../../../alfven-radius.md) $R_A$, giving [wind-driven magnetic braking of a solar-type star](../../../../../wind-driven-magnetic-braking-of-a-solar-type-star.md) $\dot J\sim-\dot M_w\Omega R_A^2$. Its spin-down time is $t_J\sim I/(\dot M_wR_A^2)$, much longer than a convective turnover time. For slowly changing moment of inertia and an unsaturated field scaling that gives $\dot J=-K\Omega^3$, integration gives $\Omega^{-2}=\Omega_0^{-2}+2Kt/I$, the [Skumanich rotation law](../../../../../skumanich-rotation-law.md). A growing or contracting star also changes $I$ and can spin up or down even without torque. Differential spin-down can create shear between layers unless internal transport couples them.

Finally, shear can excite [Kelvin-Helmholtz instability](../../../../../kelvin-helmholtz-instability.md), and convection can launch [internal gravity waves](../../../../../internal-wave.md) into the stable radiative interior. Wave damping deposits angular momentum; the net transport depends on excitation and selective absorption and is not fixed by a wave-crossing time alone. Such stresses, magnetic coupling and circulation are candidate agents for the nearly uniform radiative rotation and the narrow [tachocline](../../../../../tachocline.md). Molecular [kinematic viscosity](../../../../../kinematic-viscosity.md) has a diffusion time $\ell^2/\nu$ generally too long to couple the entire solar interior over its age, whereas a turbulent effective [kinematic viscosity](../../../../../kinematic-viscosity.md) can act much faster but is not appropriate to every stable layer. A circulation has an advection time $\ell/U_m$, thermal diffusion has time $\ell^2/\chi$, and magnetic diffusion has time $\ell^2/\eta_m$; these must be compared with the local [stellar rotation](../../../../../stellar-rotation.md) and evolutionary times rather than conflated with them. The solar dynamical time $\sqrt{R^3/(GM)}$ is about half an hour, its rotation period is of order a month, and secular magnetic braking takes an evolutionary time. **Rapid force adjustment, convective maintenance of shear, cyclic magnetic feedback and slow global spin evolution are separate processes.** Their coupled conservation equations and timescale hierarchy are the basis of a consistent account of solar rotation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
