# Dynamic viscosity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [dynamic viscosity](dynamic-viscosity.md) $\mu$ is the coefficient relating [shear stress](viscous-fluid-flow.md#shear-stress) to [shear rate](viscous-fluid-flow.md#shear-rate) in a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid). For a [simple shear flow](viscous-fluid-flow.md#simple-shear-flow) $\mathbf u=(u(y),0,0)$,

$$
\tau_{xy}=\mu\frac{du}{dy}=\mu\dot\gamma,\qquad
[\mu]=\mathrm{Pa\,s}=\mathrm{kg\,m^{-1}\,s^{-1}}.
$$

Here $\tau_{xy}$ is the $x$ component of viscous [traction](continuum-mechanics.md#traction) on a plane with [normal vector](differential-geometry.md#normal-vector) $+\mathbf e_y$. The [shear rate](viscous-fluid-flow.md#shear-rate) $\dot\gamma=du/dy$ has units $\mathrm{s^{-1}}$. Thus [dynamic viscosity](dynamic-viscosity.md) measures the [stress](continuum-mechanics.md#stress) required to sustain a given rate of deformation. It is the shear coefficient; the separate coefficient for [volume](geometry-and-topology.md#volume) change is [volume viscosity](fluid-mechanics.md#volume-viscosity). [UCL, Fluid Mechanics II, Forces in Fluids, slides 4–5](https://www.homepages.ucl.ac.uk/~uceseug/Fluids2/Slides_1.pdf)

For a worked [Couette flow](viscous-fluid-flow.md#couette-flow) example, place a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) of constant [dynamic viscosity](dynamic-viscosity.md) $\mu=0.10\,\mathrm{Pa\,s}$ between parallel plates separated by $h=0.0010\,\mathrm m$. Hold the lower plate fixed and move the upper plate at $U=0.020\,\mathrm{m\,s^{-1}}$. Assume [steady flow](fluid-mechanics.md#steady-flow), no streamwise [pressure gradient](fluid-mechanics.md#pressure-gradient), and the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition). Then

$$
u(y)=\frac{Uy}{h},\qquad
\dot\gamma=\frac Uh=20\,\mathrm{s^{-1}},\qquad
\tau_{xy}=\frac{\mu U}{h}=2.0\,\mathrm{Pa}.
$$

The fluid pulls backward on the moving plate with [force](force.md) magnitude $F=\tau_{xy}A$, where $A$ is its wetted [area](differential-geometry.md#surface-area). For $A=0.010\,\mathrm{m^2}$ this is $0.020\,\mathrm N$. Measuring that [force](force.md), the gap and the plate [velocity](classical-mechanics.md#velocity) determines $\mu=Fh/(AU)$: a direct way to measure [dynamic viscosity](dynamic-viscosity.md). The linear profile and opposing wall [tractions](continuum-mechanics.md#traction) are the standard plane [Couette flow](viscous-fluid-flow.md#couette-flow) solution. [MIT, Couette and Poiseuille Flows, p. 1](https://ocw.mit.edu/courses/2-25-advanced-fluid-mechanics-fall-2013/1a114d602956fa0dd328155f9b45f93d_MIT2_25F13_Couet_and_Pois.pdf)

<a id="image-couette-flow-a-constant-velocity-gradient-produces-a-constant-shear-stress"></a>
![](viscosity-couette-shear.png)

**[Figure 1](#image-couette-flow-a-constant-velocity-gradient-produces-a-constant-shear-stress). Couette flow: a constant velocity gradient produces a constant shear stress**. Blue arrows show the linear velocity profile between the plates. Orange arrows show viscous traction on the upper and lower faces of a fluid slice; reversing the surface normal reverses the traction. The slice has zero net viscous force although each face carries stress.

The [velocity gradient](continuum-mechanics.md#velocity-gradient) matters, rather than the [velocity](classical-mechanics.md#velocity) itself. Adding the same constant [velocity](classical-mechanics.md#velocity) to both plates and the fluid leaves $du/dy$, and hence [shear stress](viscous-fluid-flow.md#shear-stress), unchanged. In [uniform flow](fluid-mechanics.md#uniform-flow), every layer translates together and $du/dy=0$. More generally, even a nonzero [velocity gradient](continuum-mechanics.md#velocity-gradient) need not generate [viscous stress](#viscous-stress-tensor): [solid-body rotation](rigid-body-dynamics.md#solid-body-rotation) has zero [strain-rate tensor](viscous-fluid-flow.md#strain-rate-tensor), as the [viscous stress tensor](#viscous-stress-tensor) example shows. Thin gaps amplify [shear stress](viscous-fluid-flow.md#shear-stress) for a fixed plate-speed difference, making [dynamic viscosity](dynamic-viscosity.md) useful for predicting the [force](force.md) needed to move lubricated surfaces.

**Table of contents**

- [Zero-shear viscosity](#zero-shear-viscosity)
- [Kinematic viscosity](#kinematic-viscosity)
  - [Momentum diffusion](#momentum-diffusion)
  - [Density-weighted mean kinematic viscosity](#density-weighted-mean-kinematic-viscosity)
  - [Density-weighted viscosity of a disk](#density-weighted-viscosity-of-a-disk)
- [Viscous stress tensor](#viscous-stress-tensor)
  - [Viscous force](#viscous-force)
- [Reynolds number](#reynolds-number)

## Zero-shear viscosity

↑ **Parent:** [Dynamic viscosity](dynamic-viscosity.md)

For an integrable [relaxation modulus](rheology.md#relaxation-modulus), a small constant shear rate sustained from the remote past gives stress equal to that rate times the displayed integral, including any instantaneous solvent mass. For the linear [Oldroyd-B model](rheology.md#oldroyd-b-model) it is $\mu_0+G_0\tau$. A nondecaying elastic modulus would make this integral infinite rather than describe a fluid with finite steady viscosity.

## Kinematic viscosity

↑ **Parent:** [Dynamic viscosity](dynamic-viscosity.md)

The [kinematic viscosity](#kinematic-viscosity) is [dynamic viscosity](dynamic-viscosity.md) divided by [mass density](fluid-mechanics.md#density):

$$
\nu=\frac\mu\rho,\qquad [\nu]=\mathrm{m^2\,s^{-1}}.
$$

It measures the rate at which viscous transport smooths differences in [velocity](classical-mechanics.md#velocity). For constant $\mu$ and $\rho$ in [incompressible flow](fluid-mechanics.md#incompressible-flow), dividing the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) by [mass density](fluid-mechanics.md#density) makes the viscous acceleration $\nu\nabla^2\mathbf u$, where $\nabla^2$ is the [Laplacian](multivariable-calculus.md#laplacian). [David Tong, Fluid Mechanics, section 3.1.1, p. 61](https://www.damtp.cam.ac.uk/user/tong/fluids/fluids.pdf)

For example, stipulate two [Newtonian fluids](viscous-fluid-flow.md#newtonian-fluid) with the same [dynamic viscosity](dynamic-viscosity.md) $0.10\,\mathrm{Pa\,s}$ but different [mass densities](fluid-mechanics.md#density). In the same steady [Couette flow](viscous-fluid-flow.md#couette-flow) as above, both have [shear stress](viscous-fluid-flow.md#shear-stress) $2.0\,\mathrm{Pa}$, but

$$
\begin{aligned}
\rho_1&=1000\,\mathrm{kg\,m^{-3}},&\nu_1&=1.0\times10^{-4}\,\mathrm{m^2\,s^{-1}},\\
\rho_2&=500\,\mathrm{kg\,m^{-3}},&\nu_2&=2.0\times10^{-4}\,\mathrm{m^2\,s^{-1}}.
\end{aligned}
$$

The same [viscous stress](#viscous-stress-tensor) transports [momentum](momentum.md) through less [mass](classical-mechanics.md#mass) in the second fluid, so its [velocity](classical-mechanics.md#velocity) responds faster to a given nonuniform viscous [force](force.md).

To see the [diffusion equation](diffusion-equation.md) directly, consider an unsteady parallel [velocity field](fluid-mechanics.md#velocity-field) $\mathbf u=(u(y,t),0,0)$ with constant material coefficients and no streamwise [pressure gradient](fluid-mechanics.md#pressure-gradient) or body [force](force.md). Its [convective acceleration](continuum-mechanics.md#convective-acceleration) vanishes, and the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) reduces to

$$
\partial_tu=\nu\partial_y^2u.
$$

Balancing $u/t$ against $\nu u/h^2$ gives the [viscous diffusion time](viscous-fluid-flow.md#viscous-diffusion-time) $t_\nu\sim h^2/\nu$. For the $1.0\,\mathrm{mm}$ gap, the two fluids have scales $0.010\,\mathrm s$ and $0.0050\,\mathrm s$. This is a characteristic scale, not an exact settling time. For example, a perturbation of the [Couette flow](viscous-fluid-flow.md#couette-flow) profile satisfying zero perturbation [velocity](classical-mechanics.md#velocity) at both plates is

$$
\delta u(y,t)=V\sin\left(\frac{\pi y}{h}\right)
\exp\left(-\frac{\pi^2\nu t}{h^2}\right).
$$

Substituting verifies the [diffusion equation](diffusion-equation.md); its amplitude falls by a factor $e$ in $h^2/(\pi^2\nu)$. [Kinematic viscosity](#kinematic-viscosity) is therefore useful for predicting how quickly a moving wall influences the interior, while [dynamic viscosity](dynamic-viscosity.md) gives the [shear stress](viscous-fluid-flow.md#shear-stress) at a prescribed [shear rate](viscous-fluid-flow.md#shear-rate).

### Momentum diffusion

↑ **Parent:** [Kinematic viscosity](#kinematic-viscosity)

Viscous transfer of tangential [momentum](momentum.md) smooths gradients of [velocity](classical-mechanics.md#velocity). For unidirectional incompressible flow without a [pressure gradient](fluid-mechanics.md#pressure-gradient), the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) reduces to the displayed [diffusion equation](diffusion-equation.md), whose diffusion coefficient is the [kinematic viscosity](#kinematic-viscosity) $\nu=\eta/\rho$.

### Density-weighted mean kinematic viscosity

↑ **Parent:** [Kinematic viscosity](#kinematic-viscosity)

For a vertically stratified [accretion disk](astrophysical-disk.md#accretion-disk) with [surface density](astrophysical-disk.md#surface-density-of-a-disk) $\Sigma=\int\rho\,dz$, the density-weighted mean [kinematic viscosity](#kinematic-viscosity) is $\bar\nu=\Sigma^{-1}\int\rho\nu\,dz$. In an [alpha disk](astrophysical-disk.md#alpha-disk) with $\nu=\alpha p/(\rho\Omega)$, this becomes $\bar\nu=\alpha(\Sigma\Omega)^{-1}\int p\,dz$.

// Target: astrophysics.bigb

### Density-weighted viscosity of a disk

↑ **Parent:** [Kinematic viscosity](#kinematic-viscosity)

If angular [velocity](classical-mechanics.md#velocity) is independent of height, integrating the viscous stress $\rho\nu r\Omega'$ gives $\Sigma\bar\nu r\Omega'$. Thus the [surface density](astrophysical-disk.md#surface-density-of-a-disk) weighted average, rather than an unweighted height average, enters [vertically averaged viscous disk equations](astrophysical-disk.md#vertically-averaged-viscous-disk-equations).

## Viscous stress tensor

↑ **Parent:** [Dynamic viscosity](dynamic-viscosity.md)

The [viscous stress tensor](#viscous-stress-tensor) is the part of the [Cauchy stress tensor](continuum-mechanics.md#cauchy-stress-tensor) associated with deformation rates. For an isotropic [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) in [incompressible flow](fluid-mechanics.md#incompressible-flow),

$$
\boldsymbol\sigma=-pI+\boldsymbol\sigma_{\mathrm{visc}},\qquad
\boldsymbol\sigma_{\mathrm{visc}}=2\mu D,\qquad
D=\frac12\left[\nabla\mathbf u+(\nabla\mathbf u)^T\right],\qquad
\operatorname{tr}D=\nabla\cdot\mathbf u=0.
$$

Here $p$ is [pressure](pressure.md), $I$ is the [identity matrix](vector-space.md#identity-matrix), $\mu$ is [dynamic viscosity](dynamic-viscosity.md), and $D$ is the [strain-rate tensor](viscous-fluid-flow.md#strain-rate-tensor). The convention is $(\nabla\mathbf u)_{ij}=\partial_j u_i$; $T$ denotes [transpose](vector-space.md#transpose) and $\operatorname{tr}$ denotes [trace](linear-algebra.md#matrix-trace). Across a plane with unit [normal vector](differential-geometry.md#normal-vector) $\mathbf n$, the viscous [traction](continuum-mechanics.md#traction) is $\boldsymbol\sigma_{\mathrm{visc}}\mathbf n$. The [tensor](multilinear-algebra.md#tensor) makes this rule work for any plane orientation. [David Tong, Fluid Mechanics, section 3.1.1, equations (3.5)–(3.6)](https://www.damtp.cam.ac.uk/user/tong/fluids/fluids.pdf)

In the worked [Couette flow](viscous-fluid-flow.md#couette-flow), $\mathbf u=(Uy/h,0,0)$, so

$$
D=\frac{U}{2h}\begin{pmatrix}0&1&0\\1&0&0\\0&0&0\end{pmatrix},\qquad
\boldsymbol\sigma_{\mathrm{visc}}
=\begin{pmatrix}0&2&0\\2&0&0\\0&0&0\end{pmatrix}\,\mathrm{Pa}.
$$

In particular, $D_{xy}=10\,\mathrm{s^{-1}}$ while the [shear rate](viscous-fluid-flow.md#shear-rate) is $20\,\mathrm{s^{-1}}$; the factor $2$ in $2\mu D$ recovers $\tau_{xy}=2\,\mathrm{Pa}$. On the upper face of a fluid slice, $\mathbf n=\mathbf e_y$ gives viscous [traction](continuum-mechanics.md#traction) $+2\mathbf e_x\,\mathrm{Pa}$; on the lower face it is $-2\mathbf e_x\,\mathrm{Pa}$. Constant [stress](continuum-mechanics.md#stress) can therefore transmit a [force](force.md) between the plates even though its [divergence](multivariable-calculus.md#divergence), and the net viscous [force](force.md) on each slice, vanish.

Compare planar extension $\mathbf u=(ax,-ay,0)$ with [solid-body rotation](rigid-body-dynamics.md#solid-body-rotation) $\mathbf u=(-\Omega y,\Omega x,0)$:

$$
D_{\mathrm{extension}}=\begin{pmatrix}a&0&0\\0&-a&0\\0&0&0\end{pmatrix},\qquad
\nabla\mathbf u_{\mathrm{rotation}}=\begin{pmatrix}0&-\Omega&0\\\Omega&0&0\\0&0&0\end{pmatrix},\qquad
D_{\mathrm{rotation}}=0.
$$

Extension changes lengths and produces viscous [normal stresses](continuum-mechanics.md#normal-stress) $\pm2\mu a$. Rotation preserves distances and gives zero [viscous stress](#viscous-stress-tensor), despite its nonzero [velocity gradient](continuum-mechanics.md#velocity-gradient) and [vorticity](vorticity.md) $2\Omega\mathbf e_z$. For $a=\Omega=1\,\mathrm{s^{-1}}$ and $\mu=0.10\,\mathrm{Pa\,s}$, extension gives $\sigma_{\mathrm{visc},xx}=0.20\,\mathrm{Pa}$ and $\sigma_{\mathrm{visc},yy}=-0.20\,\mathrm{Pa}$; rotation gives zero. A rotating fluid may still have a [pressure gradient](fluid-mechanics.md#pressure-gradient) supplying its centripetal [acceleration](classical-mechanics.md#acceleration).

<a id="image-deformation-produces-newtonian-viscous-stress-rigid-rotation-does-not"></a>
![](viscosity-strain-versus-rotation.png)

**[Figure 2](#image-deformation-produces-newtonian-viscous-stress-rigid-rotation-does-not). Deformation produces Newtonian viscous stress; rigid rotation does not**. Blue arrows show instantaneous velocity. The dashed square is a material patch at $t=0$; its orange outline at $t=0.65\,\mathrm s$ is obtained from the exact trajectories of planar extension and solid-body rotation, with $a=\Omega=1\,\mathrm{s^{-1}}$. The marked corner makes rotation visible. Both motions preserve area, but only extension changes the patch's shape.

For an isotropic [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) in three-dimensional [compressible flow](compressible-flow.md), separate shape change from [volume](geometry-and-topology.md#volume) change:

$$
\boldsymbol\sigma_{\mathrm{visc}}
=2\mu\left(D-\frac{\nabla\cdot\mathbf u}{3}I\right)
+\zeta(\nabla\cdot\mathbf u)I.
$$

The first term is [deviatoric stress](continuum-mechanics.md#deviatoric-stress), with zero [trace](linear-algebra.md#matrix-trace); $\zeta$ is [volume viscosity](fluid-mechanics.md#volume-viscosity), also called [bulk viscosity](fluid-mechanics.md#volume-viscosity). For uniform expansion $\mathbf u=b\mathbf x$, $D=bI$ and $\nabla\cdot\mathbf u=3b$, so the shear contribution vanishes and the viscous [stress](continuum-mechanics.md#stress) is $3\zeta bI$. Thus [dynamic viscosity](dynamic-viscosity.md) and [volume viscosity](fluid-mechanics.md#volume-viscosity) describe distinct responses, and [incompressible flow](fluid-mechanics.md#incompressible-flow) removes only the volume-change term. [Shreyas Mandre, Fluid Dynamics Lecture Notes, section 2.11.3, equation (2.49)](https://notes.shreyasmandre.com/fluid-dynamics-notes/Ch2.html)

### Viscous force

↑ **Parent:** [Viscous stress tensor](#viscous-stress-tensor)

The viscous force on a fluid region is the resultant of the [traction](continuum-mechanics.md#traction) supplied by the [viscous stress tensor](#viscous-stress-tensor) $\boldsymbol\tau$. With $\mathbf n$ the outward [unit normal](differential-geometry.md#unit-normal) of the region, its surface contribution is the displayed [surface integral](multivariable-calculus.md#surface-integral). For an incompressible [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid), $\boldsymbol\tau=\eta[\nabla\mathbf u+(\nabla\mathbf u)^T]$, where $\eta$ is [dynamic viscosity](dynamic-viscosity.md) and $\mathbf u$ is [velocity](classical-mechanics.md#velocity). A force scale is $\eta UL$ for a body of size $L$ moving at speed $U$, while the inertial force scale is $\rho U^2L^2$; their ratio is the [Reynolds number](#reynolds-number). Total hydrodynamic [drag](fluid-mechanics.md#drag-physics) on a body includes both viscous traction and the pressure traction induced by the flow. For example, the full [Stokes drag law](stokes-flow.md#stokes-s-law) gives $6\pi\eta RU$ for a no-slip sphere, rather than just the viscous-traction part alone.

## Reynolds number

↑ **Parent:** [Dynamic viscosity](dynamic-viscosity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reynolds_number)

The [Reynolds number](#reynolds-number) $\operatorname{Re}=UL/\nu$ compares inertial and viscous effects. Here $U$ is a characteristic [velocity](classical-mechanics.md#velocity), $L$ a characteristic [length](physics.md#length), $\mu$ the [dynamic viscosity](dynamic-viscosity.md), $\rho$ the [mass density](fluid-mechanics.md#density), and $\nu=\mu/\rho$ the [kinematic viscosity](#kinematic-viscosity). It is a [dimensionless quantity](physics.md#dimensionless-quantity), not a property of the [fluid](fluid-mechanics.md#fluid) alone: the same material has different [Reynolds numbers](#reynolds-number) at different speeds and sizes. Specify the chosen scales when reporting it.

The comparison comes from the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation). For [velocity](classical-mechanics.md#velocity) variations on scale $L$, [convective acceleration](continuum-mechanics.md#convective-acceleration) is of order $U^2/L$, while the viscous term is of order $\nu U/L^2$. Their ratio is $UL/\nu$. Small [Reynolds number](#reynolds-number) favours [Stokes flow](stokes-flow.md); large [Reynolds number](#reynolds-number) permits an [inviscid core](viscous-fluid-flow.md#inviscid-core), although [viscous boundary layers](viscous-fluid-flow.md#viscous-boundary-layer) can remain important. Matching [Reynolds numbers](#reynolds-number) is useful when comparing geometrically similar flows, provided other relevant [dimensionless quantities](physics.md#dimensionless-quantity) and boundary conditions also match. [UCL, Scaling arguments, section 34.1.1](https://uclnatsci.github.io/2021/Electromagnetism-Fluids-and-Waves/fluids/scaling.html)

In the constriction example under [incompressible flow](fluid-mechanics.md#incompressible-flow), use the mean axial [velocity](classical-mechanics.md#velocity) and pipe diameter, $L=D=2R$. Taking $\rho=1000\,\mathrm{kg\,m^{-3}}$ and a stipulated [dynamic viscosity](dynamic-viscosity.md) $\mu=0.001\,\mathrm{Pa\,s}$ gives

$$
\mathrm{Re}_1=\frac{1000(0.20)(0.020)}{0.001}=4000,\qquad
\mathrm{Re}_2=\frac{1000(0.80)(0.010)}{0.001}=8000.
$$

Halving the radius at fixed [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate) doubles this diameter-based [Reynolds number](#reynolds-number), because mean [velocity](classical-mechanics.md#velocity) increases fourfold. These values alone neither establish [laminar flow](fluid-mechanics.md#laminar-flow) nor prove that [viscosity](dynamic-viscosity.md) can be omitted from the [pressure](pressure.md) calculation. Increasing $\mu$ to $0.10\,\mathrm{Pa\,s}$ with the same imposed flow gives $40$ and $80$, but strengthens viscous effects; small [Reynolds number](#reynolds-number) does not justify [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle).

The name recalls Osborne Reynolds's 1883 experimental investigation of water motion and resistance in pipes. His dye experiments distinguished smooth [laminar flow](fluid-mechanics.md#laminar-flow) from mixed, irregular [turbulence](turbulence.md). [Reynolds, 1883, original paper abstract and bibliographic record](https://cir.nii.ac.jp/crid/1362544419765899904) [UCL, Scaling arguments, section 34.1.4](https://uclnatsci.github.io/2021/Electromagnetism-Fluids-and-Waves/fluids/scaling.html) There is no universal transition value applicable to every geometry and disturbance environment. [H. K. Moffatt, transition discussion, p. 208](https://www.damtp.cam.ac.uk/user/hkm2/PDFs/Moffatt_1977_GordonandBreach_Slogfdatohdt_149.pdf)

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (129)

- [Avogadro constant from sedimentation and diffusion](brownian-motion.md#avogadro-constant-from-sedimentation-and-diffusion)
- [Blasius boundary layer](continuum-mechanics.md#blasius-boundary-layer)
- [Boundary layer](continuum-mechanics.md#boundary-layer)
- [Buoyancy-modified Darcy fingering dispersion relation](porous-media-flow.md#buoyancy-modified-darcy-fingering-dispersion-relation)
- [Charge lattice inference from oil drops](electric-charge.md#charge-lattice-inference-from-oil-drops)
- [Clean-bubble Stokes drag](stokes-flow.md#clean-bubble-stokes-drag)
- [Constant gas-radiation ratio vertical disc structure](astrophysical-disk.md#constant-gas-radiation-ratio-vertical-disc-structure)
- [Constant-pressure-ratio vertical disk model](astrophysical-disk.md#constant-pressure-ratio-vertical-disk-model)
- [Constant viscosity in radiation-supported vertical balance](astrophysical-disk.md#constant-viscosity-in-radiation-supported-vertical-balance)
- [Couette flow with a slipping lower wall](fluid-mechanics.md#couette-flow-with-a-slipping-lower-wall)
- [Darcy flow through a homogeneous slab](porous-media-flow.md#darcy-flow-through-a-homogeneous-slab)
- [Darcy law](porous-media-flow.md#darcy-law)
- [Delayed polymer diversion in parallel porous layers](porous-media-flow.md#delayed-polymer-diversion-in-parallel-porous-layers)
- [Drag coefficient](fluid-mechanics.md#drag-coefficient)
- [Dynamic viscosity](dynamic-viscosity.md)
- [Effective permeability](porous-media-flow.md#effective-permeability)
- [Einstein viscosity formula for a dilute suspension](stokes-flow.md#einstein-viscosity-formula-for-a-dilute-suspension)
- [Elementary charge](electric-charge.md#elementary-charge)
- [Energy dissipation identity for Model H](critical-phenomenon.md#energy-dissipation-identity-for-model-h)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Fluid](fluid-mechanics.md#fluid)
- [Friction-dominated grounding-line evolution law](geophysics.md#friction-dominated-grounding-line-evolution-law)
- [Gas-pressure viscosity closure with mixed pressure support](astrophysical-disk.md#gas-pressure-viscosity-closure-with-mixed-pressure-support)
- [Hydraulic conductivity](porous-media-flow.md#hydraulic-conductivity)
- [Hydrodynamic coarsening crossover scales](critical-phenomenon.md#hydrodynamic-coarsening-crossover-scales)
- [Hydrodynamic radius](mixture.md#hydrodynamic-radius)
- [Kinematic viscosity](#kinematic-viscosity)
- [Kinetic estimates of gas transport coefficients](kinetic-theory.md#kinetic-estimates-of-gas-transport-coefficients)
- [Laminar flow](fluid-mechanics.md#laminar-flow)
- [Laminar skin-friction scaling along a slender swimmer](continuum-mechanics.md#laminar-skin-friction-scaling-along-a-slender-swimmer)
- [Layered porous permeability](porous-media-flow.md#layered-porous-permeability)
- [Magma](geophysics.md#magma)
- [Newtonian fluid stress tensor](viscous-fluid-flow.md#newtonian-fluid-stress-tensor)
- [Newtonian till lubrication](geophysics.md#newtonian-till-lubrication)
- [Oil drop charge readout and calibration](electric-charge.md#oil-drop-charge-readout-and-calibration)
- [Optical trap Langevin calibration](optics.md#optical-trap-langevin-calibration)
- [Optical trap relaxation time](optics.md#optical-trap-relaxation-time)
- [Parallel-disc viscometer](viscous-fluid-flow.md#parallel-disc-viscometer)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022.md#section-b/5/a/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-45.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-71.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-73.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-74.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-77.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-77.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-77.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-84.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-75.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-78.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-81.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-86.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-73.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-61.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-61.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-61.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-71.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-78.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-78.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#36e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-80.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-332.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-334.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344.md#2/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#38c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-321.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-334.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-352.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#39c/a/solution)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2021/paper-2.md#section-b/22/ii/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-b/b8/d/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1.md#section-a/a3/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1.md#section-c/13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b8/c/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b9/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-a/a2/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2015/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2016/paper-1.md#2/a/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2018.md#section-a/1/a/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-a/1/solution)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2019.md#section-b/b4/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Permeability of a porous medium](porous-media-flow.md#permeability-of-a-porous-medium)
- [Phase mobility](porous-media-flow.md#phase-mobility)
- [Planar Poiseuille flow with equal wall slip](fluid-mechanics.md#planar-poiseuille-flow-with-equal-wall-slip)
- [Planar viscous-fingering dispersion relation](porous-media-flow.md#planar-viscous-fingering-dispersion-relation)
- [Pointwise alpha-prescription obstruction in a radiation-supported layer](astrophysical-disk.md#pointwise-alpha-prescription-obstruction-in-a-radiation-supported-layer)
- [Porous gravity current with background flow](porous-media-flow.md#porous-gravity-current-with-background-flow)
- [Premelted-film lifting of a disk](geophysics.md#premelted-film-lifting-of-a-disk)
- [Relaxation of a symmetric viscous layer](stokes-flow.md#relaxation-of-a-symmetric-viscous-layer)
- [Reynolds number](#reynolds-number)
- [Rotational diffusion of a sphere](thermodynamics.md#rotational-diffusion-of-a-sphere)
- [Sedimentation scale height](brownian-motion.md#sedimentation-scale-height)
- [Stokes equation](stokes-flow.md#stokes-equation)
- [Stokes flow](stokes-flow.md)
- [Stokes's law](stokes-flow.md#stokes-s-law)
- [Stokes settling velocity](suspension-chemistry.md#stokes-settling-velocity)
- [Strong Boussinesq approximation](geophysical-fluid-dynamics.md#strong-boussinesq-approximation)
- [Thermocapillary migration of an insulating bubble](surface-tension.md#thermocapillary-migration-of-an-insulating-bubble)
- [Two-layer Couette flow](viscous-fluid-flow.md#two-layer-couette-flow)
- [Vertically averaged alpha closure for a mixed-pressure layer](astrophysical-disk.md#vertically-averaged-alpha-closure-for-a-mixed-pressure-layer)
- [Viscous force](#viscous-force)
- [Viscous mountain spreading over an underthrust plate](viscous-fluid-flow.md#viscous-mountain-spreading-over-an-underthrust-plate)
- [Viscous stress tensor](#viscous-stress-tensor)
- [Wall friction in the Navier slip boundary condition](fluid-mechanics.md#wall-friction-in-the-navier-slip-boundary-condition)
