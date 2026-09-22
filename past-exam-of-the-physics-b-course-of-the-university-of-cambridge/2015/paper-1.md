# Paper 1

↑ **Parent:** [2015](../2015.md)

[Original public PDF, physical pages 170–179; examination dated 30 May 2015](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=170)

**Table of contents**

- [Section A](#section-a)
  - [A1](#section-a/a1)
    - [Solution](#section-a/a1/solution)
  - [A2](#section-a/a2)
    - [Solution](#section-a/a2/solution)
  - [A3](#section-a/a3)
    - [Solution](#section-a/a3/solution)
  - [A4](#section-a/a4)
    - [Solution](#section-a/a4/solution)
  - [A5](#section-a/a5)
    - [Solution](#section-a/a5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [Solution](#section-b/b6/solution)
  - [B7](#section-b/b7)
    - [Solution](#section-b/b7/solution)
  - [B8](#section-b/b8)
    - [Solution](#section-b/b8/solution)
  - [B9](#section-b/b9)
    - [Solution](#section-b/b9/solution)
- [Section C](#section-c)
  - [C10](#section-c/c10)
    - [Solution](#section-c/c10/solution)
  - [C11](#section-c/c11)
    - [Solution](#section-c/c11/solution)
  - [12](#section-c/12)
    - [Solution](#section-c/12/solution)
  - [13](#section-c/13)
    - [Solution](#section-c/13/solution)

## Section A

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-a/a1">A1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a1/solution">Solution</h4>

↑ **Parent:** [A1](#section-a/a1)

For a smooth isolated [conducting sphere](../../electrostatics.md#conducting-sphere), [Gauss's law](../../maxwell-equations.md#gauss-s-law) gives the surface [electric field](../../electric-field.md) $E_s=Q/(4\pi\epsilon_0a^2)$ and [electric potential](../../electric-field.md#electric-potential) $V=Q/(4\pi\epsilon_0a)=aE_s$. At the specified [dielectric strength](../../permittivity.md#dielectric-strength), $V_{\max}=3.0\times10^3\ \mathrm V$. The [capacitance of an isolated conducting sphere](../../electromagnetism.md#capacitance-of-an-isolated-conducting-sphere) is $C=4\pi\epsilon_0a$, so its [capacitor energy](../../electromagnetism.md#capacitor-energy) is

$$
U_{\max}=\frac12 C V_{\max}^2=2\pi\epsilon_0a^3E_s^2
=\boxed{5.0\times10^{-7}\ \mathrm J\simeq0.50\ \mu\mathrm J.}
$$

This is the ideal [breakdown-limited energy of a conducting sphere](../../electromagnetism.md#breakdown-limited-energy-of-a-conducting-sphere), taking air's [permittivity](../../permittivity.md) approximately equal to [vacuum permittivity](../../permittivity.md#vacuum-permittivity) and neglecting nearby objects and surface irregularities. The [vacuum permittivity](../../permittivity.md#vacuum-permittivity) used numerically is $8.8542\times10^{-12}\ \mathrm{F\,m^{-1}}$.[2022 CODATA adjustment, vacuum electric permittivity entry](../../chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others)

<h3 id="section-a/a2">A2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a2/solution">Solution</h4>

↑ **Parent:** [A2](#section-a/a2)

Take the initial thrower and receiver positions to be $(-a,0)$ and $(a,0)$, with counterclockwise [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\omega$. Interpret $v$ as the launch [speed](../../classical-mechanics.md#speed) relative to the thrower. The ball inherits the thrower's tangential [velocity](../../classical-mechanics.md#velocity), so in an [inertial frame](../../mathematical-physics.md#inertial-frame) its initial horizontal [velocity](../../classical-mechanics.md#velocity) is $(v,-a\omega)$. The flight time across the diameter is $t_f\simeq2a/v$. During that time the receiver moves approximately $+a\omega t_f$ sideways while the ball moves $-a\omega t_f$. Thus the [transverse miss on a rotating platform](../../mathematical-physics.md#transverse-miss-on-a-rotating-platform) is

$$
\boxed{d\simeq2a\omega t_f=\frac{4a^2\omega}{v}.}
$$

The ball passes behind the receiver in the sense of rotation. Equivalently, in the rotating frame its transverse [Coriolis acceleration](../../mathematical-physics.md#coriolis-acceleration) has magnitude $2\omega v$ to leading order; integrating over $t_f$ gives $d=\tfrac12(2\omega v)t_f^2$. Terms neglected here are higher order in $a\omega/v$. Specifying an initially radial launch [velocity](../../classical-mechanics.md#velocity) in the inertial frame instead would define a different throw and would lose the inherited tangential [velocity](../../classical-mechanics.md#velocity).

<h3 id="section-a/a3">A3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a3/solution">Solution</h4>

↑ **Parent:** [A3](#section-a/a3)

The [dynamic viscosity](../../dynamic-viscosity.md) measures the transport of tangential [momentum](../../momentum.md) between adjacent layers. The [kinetic estimates of gas transport coefficients](../../kinetic-theory.md#kinetic-estimates-of-gas-transport-coefficients) give

$$
\eta\sim\frac13nm\overline v\lambda,\qquad
\lambda\sim\frac1{\sqrt2n\sigma_c},\qquad
\overline v\propto\sqrt{\frac{k_BT}{m}},
$$

where $n$ is number density, $m$ the molecular [mass](../../classical-mechanics.md#mass), $\lambda$ the [mean free path](../../ideal-gas.md#mean-free-path), and $\sigma_c$ a collision [cross section](../../physics.md#cross-section-physics). At fixed [temperature](../../temperature.md), raising the [pressure](../../pressure.md) increases the number of momentum carriers but shortens their [mean free path](../../ideal-gas.md#mean-free-path) by the same factor. Consequently **the [dynamic viscosity](../../dynamic-viscosity.md) of a dilute gas is approximately independent of [pressure](../../pressure.md)**.

For a temperature-independent collision [cross section](../../physics.md#cross-section-physics), the same estimate gives $\eta\propto\sqrt{mk_BT}/\sigma_c$, so **$\eta\propto T^{1/2}$ in the hard-sphere model**. Faster molecules carry [momentum](../../momentum.md) across layers more rapidly. Real intermolecular interactions make the effective collision [cross section](../../physics.md#cross-section-physics) temperature-dependent, changing this simple exponent. The pressure-independence also fails when wall collisions, rather than molecule–molecule collisions, set the transport distance; the continuum estimate assumes a small [Knudsen number](../../kinetic-theory.md#knudsen-number).

<h3 id="section-a/a4">A4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a4/solution">Solution</h4>

↑ **Parent:** [A4](#section-a/a4)

The varying [magnetic flux](../../magnetic-field.md#magnetic-flux) through the ring induces an [electromotive force](../../electric-charge.md#electromotive-force) by [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction). Its direction follows [Lenz's law](../../maxwell-equations.md#lenz-s-law). With solenoid current $I_s$, ring current $I_r$, ring [self-inductance](../../electromagnetism.md#self-inductance) $L_r$, [electrical resistance](../../electric-charge.md#electrical-resistance) $R$, and [mutual inductance](../../electromagnetism.md#mutual-inductance) $M(z)$,

$$
L_r\dot I_r+RI_r=-M\dot I_s,\qquad F_z=I_sI_r\frac{dM}{dz}.
$$

The ring sits in a nonuniform [magnetic field](../../magnetic-field.md): coupling decreases above the solenoid, so $M>0$ and $M'<0$ with a common orientation for the two windings. For $I_s=I_0\cos\omega t$, the in-phase part of the induced ring current is negative:

$$
\langle I_sI_r\rangle=-\frac{I_0^2\omega^2ML_r}{2(R^2+\omega^2L_r^2)},\qquad
\boxed{\langle F_z\rangle=-\frac{I_0^2\omega^2ML_rM'}{2(R^2+\omega^2L_r^2)}>0.}
$$

Thus [alternating-current induction levitation](../../electromagnetism.md#alternating-current-induction-levitation) can balance the ring's weight when $\langle F_z\rangle=mg$. A falling mean lifting [force](../../force.md) with height supplies vertical [stability](../../numerical-analysis.md#stability-of-a-numerical-method). In the strongly inductive limit the two currents are almost opposite: the ring repels the solenoid during both half cycles. Finite [self-inductance](../../electromagnetism.md#self-inductance) matters; an ideal purely resistive loop would carry a current exactly in quadrature with $I_s$ and give zero average [force](../../force.md) in this model. The source supplies the [Joule heating](../../electric-charge.md#joule-heating) in the real ring, and any mechanical work while it rises.

<h3 id="section-a/a5">A5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a5/solution">Solution</h4>

↑ **Parent:** [A5](#section-a/a5)

After the [photon](../../quantum-mechanics.md#photon) has thermalized, its [energy](../../energy.md) $E_\gamma=hc/\lambda$ belongs to the macroscopic body's internal [energy](../../energy.md). The body's [heat capacity](../../heat.md#heat-capacity) makes the resulting [temperature](../../temperature.md) change negligible. Its equilibrium [entropy](../../entropy.md) therefore increases by

$$
\boxed{\Delta S\simeq\frac{hc}{\lambda T}.}
$$

The [Boltzmann entropy](../../entropy.md#boltzmann-s-entropy-formula) $S=k_B\ln\Omega$ then gives the [microstate multiplier from photon absorption](../../entropy.md#microstate-multiplier-from-photon-absorption):

$$
\boxed{\frac{\Omega_f}{\Omega_i}=\exp(\Delta S/k_B)\simeq
\exp\!\left(\frac{hc}{\lambda k_BT}\right).}
$$

For scale, explicitly choosing a representative visible [wavelength](../../wave-equation.md#wavelength) $\lambda=500\ \mathrm{nm}$ and room [temperature](../../temperature.md) $T=300\ \mathrm K$ gives $\Delta S=1.32\times10^{-21}\ \mathrm{J\,K^{-1}}$, or $\Delta S/k_B=95.9$, and **a multiplier approximately $4.5\times10^{41}$**. These are illustrative choices, not additional supplied data: the exact multiplier depends exponentially on the particular visible [wavelength](../../wave-equation.md#wavelength) and [temperature](../../temperature.md). The exact [Planck constant](../../quantum-mechanics.md#planck-constant), [speed of light](../../special-relativity.md#speed-of-light), and [Boltzmann constant](../../thermodynamics.md#boltzmann-constant) fix the conversion.[2022 CODATA adjustment, Planck constant, speed of light in vacuum, and Boltzmann constant entries](../../chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others)

## Section B

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/solution">Solution</h4>

↑ **Parent:** [B6](#section-b/b6)

In [electrostatics](../../electrostatics.md), the [Maxwell equations in matter](../../maxwell-equations.md#maxwell-equations-in-matter) are

$$
\nabla\cdot\mathbf D=\rho_f,\qquad \nabla\times\mathbf E=\mathbf0,
\qquad \mathbf D=\epsilon_0\mathbf E+\mathbf P.
$$

Here $\rho_f$ is free [charge density](../../electric-charge.md#charge-density) and $\mathbf P$ is [polarization density](../../electromagnetism.md#polarization-density). For a homogeneous isotropic linear [dielectric](../../permittivity.md#dielectric), the [constitutive equation](../../continuum-mechanics.md#constitutive-equation) is $\mathbf D=\epsilon_0\epsilon_r\mathbf E$. Integrating the first equation over a thin pillbox straddling an interface, with unit normal $\mathbf n$ from medium 1 to medium 2, gives $\mathbf n\cdot(\mathbf D_2-\mathbf D_1)=\sigma_f$. Integrating the second around a vanishingly narrow rectangular loop gives $\mathbf n\times(\mathbf E_2-\mathbf E_1)=\mathbf0$. These are the [electrostatic interface boundary conditions](../../electrostatics.md#electrostatic-interface-boundary-conditions). When there is no free surface [electric charge](../../electric-charge.md), the normal [electric displacement field](../../electromagnetism.md#electric-displacement-field) and tangential [electric field](../../electric-field.md) are continuous; the normal [electric field](../../electric-field.md) generally is not.

Neglect end [fringing field of a capacitor](../../electromagnetism.md#fringing-field-of-a-capacitor). In either axial segment of the [coaxial cylindrical capacitor](../../electrostatics.md#coaxial-cylindrical-capacitor), a cylindrical [Gaussian surface](../../maxwell-equations.md#gaussian-surface) gives $D_r=\lambda_f/(2\pi r)$, where $\lambda_f$ is free [electric charge](../../electric-charge.md) per length. Integrating the radial [electric field](../../electric-field.md) between the conductors gives

$$
V=\frac{\lambda_f}{2\pi\epsilon_0\epsilon_r}\ln\frac ba,
\qquad C'=\frac{\lambda_f}{V}=\frac{2\pi\epsilon_0\epsilon_r}{\ln(b/a)}.
$$

The liquid and air segments share the same conductor [electric potential difference](../../electric-field.md#electric-potential-difference), so their capacitances add in parallel. Thus the [partially filled coaxial capacitor](../../electrostatics.md#partially-filled-coaxial-capacitor) has

$$
\boxed{C(h)=\frac{2\pi\epsilon_0}{\ln(b/a)}[L-h+\epsilon h].}
$$

Here the question's $\epsilon$ is relative [permittivity](../../permittivity.md), and air's relative [permittivity](../../permittivity.md) is approximated by one.

Write $x$ for the rise above the external level. The wide reservoir keeps that level approximately fixed. At constant applied [voltage](../../random-walk.md#voltage), one must include work done by the source: the appropriate electrical contribution to the mechanical potential is $-C V^2/2$. The upward [dielectric insertion force at fixed voltage](../../electromagnetism.md#dielectric-insertion-force-at-fixed-voltage) is consequently

$$
F_e=\frac12V^2\frac{dC}{dx}
=\frac{\pi\epsilon_0(\epsilon-1)V^2}{\ln(b/a)}.
$$

The excess [hydrostatic pressure](../../fluid-mechanics.md#hydrostatic-pressure) $\rho gx$ acts over the annular area $A=\pi(b^2-a^2)$. Alternatively its gravitational [potential energy](../../energy.md#potential-energy) is $\rho gAx^2/2$, since liquid initially at the reservoir level must be raised through all heights from zero to $x$. Balancing the derivatives gives

$$
\boxed{x=\Delta h=\frac{\epsilon_0(\epsilon-1)V^2}{\rho g(b^2-a^2)\ln(b/a)}.}
$$

This assumes $h+x<L$, a communicating liquid reservoir, negligible capillarity, and a sufficiently long [capacitor](../../electromagnetism.md#capacitor) that end effects are small. Differentiating gives the [dielectric-rise voltmeter](../../electrostatics.md#dielectric-rise-voltmeter)'s sensitivity at a bias $V$:

$$
\boxed{\frac{dx}{dV}=\frac{2\epsilon_0(\epsilon-1)V}{\rho g(b^2-a^2)\ln(b/a)}.}
$$

To obtain its numerical value in $\mu\mathrm m\,\mathrm V^{-1}$, multiply the right-hand side in SI units by $10^6$. A convenient parametric scale, with $\beta=b/a$, is

$$
\frac{dx}{dV}=1.805\times10^{-3}\,
\frac{\epsilon-1}{(\beta^2-1)\ln\beta}
\left(\frac V{1\ \mathrm V}\right)
\left(\frac{10^3\ \mathrm{kg\,m^{-3}}}{\rho}\right)
\left(\frac{1\ \mathrm{mm}}a\right)^2
\left(\frac{9.81\ \mathrm{m\,s^{-2}}}g\right)
\ \mu\mathrm m\,\mathrm V^{-1}.
$$

For a concrete estimate, choose $a=1\,\mathrm{mm}$, $b=2\,\mathrm{mm}$, [mass density](../../fluid-mechanics.md#density) $\rho=10^3\,\mathrm{kg\,m^{-3}}$, [relative permittivity](../../quantum-mechanics.md#relative-permittivity) $\epsilon=2$ and operating [voltage](../../random-walk.md#voltage) $V=100\,\mathrm V$. These are illustrative choices, not supplied apparatus data. They give

$$
\boxed{\frac{dx}{dV}\simeq0.087\,\mu\mathrm m\,\mathrm V^{-1},\qquad x\simeq4.3\,\mu\mathrm m.}
$$

Thus this millimetre-scale example requires fine optical [displacement](../../classical-mechanics.md#displacement) measurement for volt-level changes. The parametric formula states exactly how the estimate changes with the chosen geometry, liquid and bias.

The displacement is quadratic in [voltage](../../random-walk.md#voltage), cannot distinguish its sign, and has zero first-order sensitivity at zero bias. Smaller gaps and larger [relative permittivity](../../quantum-mechanics.md#relative-permittivity) increase sensitivity, but capillarity, leakage, [dielectric breakdown](../../permittivity.md#dielectric-breakdown), temperature-dependent liquid properties, and finite available rise then limit performance. A nonconducting liquid avoids a sustained conduction load, although charging still draws [electric charge](../../electric-charge.md) and leakage is possible. A high [voltage](../../random-walk.md#voltage) can give a readable displacement; a low-voltage instrument would require fine displacement measurement and careful calibration.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

The differential form of [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction) is

$$
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t}.
$$

By [Stokes theorem](../../multivariable-calculus.md#stokes-theorem), for a stationary oriented circuit it becomes $\mathcal E=\oint\mathbf E\cdot d\boldsymbol\ell=-d\Phi_B/dt$, where $\Phi_B=\int\mathbf B\cdot d\mathbf S$ is [magnetic flux](../../magnetic-field.md#magnetic-flux) and $\mathcal E$ is [electromotive force](../../electric-charge.md#electromotive-force). Circuit orientation and surface normal obey the [right-hand rule](../../electromagnetism.md#right-hand-rule). [Lenz's law](../../maxwell-equations.md#lenz-s-law) is the physical meaning of the minus sign: the induced current's [magnetic field](../../magnetic-field.md) opposes the change in linked [magnetic flux](../../magnetic-field.md#magnetic-flux). For a moving circuit, the force per unit [electric charge](../../electric-charge.md) is $\mathbf E+\mathbf v\times\mathbf B$, and its line integral is the corresponding [electromotive force](../../electric-charge.md#electromotive-force). Motion through a static [magnetic field](../../magnetic-field.md) can therefore induce a [voltage](../../random-walk.md#voltage) even when $\partial_t\mathbf B=0$.

Let $\theta$ be the wire's angle from the downward vertical, $r=L\sin\theta$, and choose $\boldsymbol\omega$ and $\mathbf B$ upward, as in the figure. The motional term along the wire has radial component $B\omega s$ at cylindrical radius $s$. In steady electrical [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), integrating from the grounded axis to the bob gives

$$
V_b=\int_0^rB\omega s\,ds=\frac12B\omega r^2,
\qquad Q=CV_b=\frac12BC\omega r^2.
$$

The [Lorentz force](../../relativistic-electromagnetism.md#lorentz-force) on this positive [electric charge](../../electric-charge.md) is radially outward. Its ratio to the required centripetal term is $QB/(m\omega)\lesssim CB^2L^2/(2m)$, so the stated heavy-bob condition makes its effect on the zero-field [conical pendulum](../../simple-pendulum.md#conical-pendulum) geometry negligible. With wire tension $T_w$, $T_w\cos\theta=mg$ and $T_w\sin\theta=m\omega^2r$, giving $\cos\theta=g/(\omega^2L)$. Hence the [magnetically charged conical pendulum](../../simple-pendulum.md#magnetically-charged-conical-pendulum) has

$$
\boxed{Q_0=\frac12BC\left(\omega L^2-\frac{g^2}{\omega^3}\right).}
$$

A nonzero-radius orbit requires $\omega^2L>g$. Reversing the sense of rotation or the [magnetic field](../../magnetic-field.md) reverses the sign of $Q_0$.

The response to the added [electric field](../../electric-field.md) requires an electrical convention. In the usual mechanical approximation, treat the pre-existing [electric charge](../../electric-charge.md) as $Q_0$, include its upward [electric force](../../electric-field.md#electric-force) $Q_0E$, and neglect all magnetic-force feedback. Then

$$
\cos\theta(E)=\frac{mg-Q_0E}{m\omega^2L},\qquad
\frac{\delta r}{r}=-\frac{\cos\theta\,\delta(\cos\theta)}{\sin^2\theta}
=\frac{Q_0E g}{m\omega^4r^2}
=\boxed{\frac{CBgE}{2m\omega^3}.}
$$

This predicts an increased radius for $Q_0E>0$. It is the result when the newly applied field is used only as a probe force on the original [electric charge](../../electric-charge.md).

There is a first-order qualification if the bob remains electrically connected to the grounded pivot and the uniform added field's potential is included consistently. Put $s=\cos\theta$ and set the external [electric potential](../../electric-field.md#electric-potential) to zero at the pivot. The external potential at the bob is then $ELs$, so the charging relation and full force balance become

$$
Q=C\!\left[\frac12B\omega L^2(1-s^2)-ELs\right],\qquad
\omega^2Ls+\frac Qm(B\omega Ls+E)=g.
$$

The second equation follows by eliminating the wire tension between vertical balance and radial balance, including the outward magnetic [Lorentz force](../../relativistic-electromagnetism.md#lorentz-force). Expanding both equations to first order in $E$, and to leading order in $CB^2L^2/m$, with $s_0=g/(\omega^2L)$, gives

$$
\delta s=-\frac{CBLE}{2m\omega}(1-3s_0^2),\qquad
\boxed{\frac{\delta r}{r}=\frac{CBgE}{2m\omega^3}\,
\frac{1-3s_0^2}{1-s_0^2}.}
$$

The extra factor arises from the added field changing $Q$ by $-CELs_0$ and therefore changing the radial magnetic [force](../../force.md). That term is linear in $E$ too; the heavy-bob assumption alone does not justify retaining $Q_0E$ while dropping it. The two expressions refer to the two electrical approximations just specified. The expansion requires a small change relative to the initial radius and is nonuniform as that radius tends to zero.

For an electrical measurement, route the grounded connection through a sensitive [electrometer](../../electric-charge.md#electrometer) operated near zero input [voltage](../../random-walk.md#voltage), and integrate the charging [electric current](../../electric-charge.md#electric-current) when $B$ or $\omega$ is changed. Starting with the field off, the transferred [electric charge](../../electric-charge.md) is $Q_0$ in this ideal capacitance model. Reversing $B$ separates the induced signal from offsets. Alternatively, isolate the charged bob briefly and measure its [electric potential](../../electric-field.md#electric-potential) with a high-input-impedance [electrometer](../../electric-charge.md#electrometer), accounting for the instrument's extra [capacitance](../../electromagnetism.md#capacitance) and for the fact that isolation changes the electrical boundary condition.

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/solution">Solution</h4>

↑ **Parent:** [B8](#section-b/b8)

The [characteristic impedance](../../electrical-engineering.md#characteristic-impedance) of a lossless [transmission line](../../electrical-engineering.md#transmission-line) is the ratio of the [voltage](../../random-walk.md#voltage) to the current amplitude of a single forward-travelling wave. If $\mathcal L$ and $\mathcal C$ denote [inductance](../../electromagnetism.md#inductance) and [capacitance per unit length](../../electromagnetism.md#capacitance-per-unit-length), the lossless telegrapher equations give

$$
\partial_z V=-\mathcal L\partial_t I,\qquad
\partial_z I=-\mathcal C\partial_t V,
\qquad \boxed{Z=\sqrt{\mathcal L/\mathcal C}},\qquad
v_p=(\mathcal L\mathcal C)^{-1/2}.
$$

A backward wave has $I_-=-V_-/Z$ when current is positive along $+z$. Thus [characteristic impedance](../../electrical-engineering.md#characteristic-impedance) is not a resistor's [electrical resistance](../../electric-charge.md#electrical-resistance): it describes travelling-wave amplitudes and determines [impedance matching](../../electrical-circuit.md#impedance-matching), power transfer and reflections. A semi-infinite line, or a line terminated by a matching load, presents that impedance at its input.

At a junction with no lumped branch, [voltage](../../random-walk.md#voltage) and [electric current](../../electric-charge.md#electric-current) are continuous:

$$
V_i+V_r=V_t,\qquad \frac{V_i-V_r}{Z_1}=\frac{V_t}{Z_2}.
$$

Eliminating $V_t$ gives the voltage [reflection coefficient](../../partial-differential-equation.md#reflection-coefficient)

$$
\boxed{r=\frac{V_r}{V_i}=\frac{Z_2-Z_1}{Z_2+Z_1}.}
$$

For real positive $Z_1$, incident and reflected waves occupy the same line, so their power ratio is $|r|^2$.

For the slightly mismatched [coaxial cables](../../electrical-engineering.md#coaxial-cable), the change in [characteristic impedance](../../electrical-engineering.md#characteristic-impedance) is

$$
\Delta Z=\frac{Z_{\rm vac}}{2\pi n}\ln\!\left(1+\frac{\Delta b}b\right)
\simeq\frac{Z_{\rm vac}}{2\pi n}\frac{\Delta b}b.
$$

Consequently

$$
r\simeq\frac{\Delta Z}{2Z}=\frac1{2\ln(b/a)}\frac{\Delta b}b,\qquad
\boxed{\mathcal R\simeq\frac{1}{4\ln^2(b/a)}\left(\frac{\Delta b}b\right)^2.}
$$

The requested power limit $0.01\%=10^{-4}$ implies $|\Delta b|/b<0.02\ln(b/a)$. Since $\ln(b/a)=2\pi nZ/Z_{\rm vac}=1.918$ for the stated line, **the adjacent cables' outer radii must match within approximately $3.84\%$**. If a tolerance is quoted separately as a symmetric manufacturing range $\pm\delta b$ and arbitrary worst-case pairs can differ by $2\delta b$, the corresponding individual tolerance is approximately **$\pm1.92\%$**. The leading calculation is for small mismatches; the exact logarithmic expression gives slightly asymmetric positive and negative limits. The vacuum [wave impedance](../../electromagnetic-wave.md#wave-impedance) used here is approximately $376.73\ \Omega$.[2022 CODATA adjustment, characteristic impedance of vacuum entry](../../chemistry-bibliography.md#fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others)

A needle is a shunt [electrical resistance](../../electric-charge.md#electrical-resistance) $R_n$, so the load seen at its location is the continuation of the line in parallel with $R_n$: $Z_L=ZR_n/(Z+R_n)$. The local voltage [reflection coefficient](../../partial-differential-equation.md#reflection-coefficient) and transmission amplitude are

$$
\boxed{r=-\frac{Z}{2R_n+Z}\simeq-\frac{Z}{2R_n}},\qquad t=1+r.
$$

For [periodic resistive loading of a transmission line](../../electrical-engineering.md#periodic-resistive-loading-of-a-transmission-line), the reflection from the next needle travels an additional round trip $2L$ and crosses each previous needle twice. Taking the first needle as phase reference, the [single-return approximation for periodic line reflections](../../electrical-engineering.md#single-return-approximation-for-periodic-line-reflections) therefore sums to

$$
R_{\rm first}=r\sum_{j=0}^\infty[t^2e^{i\phi}]^j
=\frac r{1-(1+r)^2e^{i\phi}},\qquad
\phi=2kL=\frac{4\pi\nu L}{v_p}.
$$

Here $v_p$ is the propagation [phase velocity](../../dispersion-relation.md#phase-velocity) in the cable, $c/n$ for the stated nondispersive nonmagnetic filling. Squaring the amplitude gives the requested expression

$$
\boxed{\mathcal R_{\rm first}(\nu)=\left|\frac r{1-(1+r)^2e^{i\phi(\nu)}}\right|^2.}
$$

For a finite number $N$ of needles the amplitude has the additional numerator $1-[t^2e^{i\phi}]^N$. The displayed semi-infinite result assumes sufficiently many needles, no terminal reflection, and neglects intrinsic propagation loss.

For real $r<0$, write $q=t^2$. The denominator of the power coefficient is $1+q^2-2q\cos\phi$. It has constructive peaks at $\phi=2\pi j$ and minima at $\phi=(2j+1)\pi$, repeating with **frequency spacing $\Delta\nu=v_p/(2L)$**. Within this approximation,

$$
\mathcal R_{\max}=\frac1{(2+r)^2}\simeq\frac14,\qquad
\mathcal R_{\min}=\frac{r^2}{[1+(1+r)^2]^2}\simeq\frac{r^2}{4}.
$$

Weak individual shunts thus give narrow interference peaks, with phase width of order $|r|$.

The requested sum excludes paths that reflect repeatedly between different needles. It should not be read as an exact multiple-scattering result, particularly at the coherent peaks. For example the exact semi-infinite amplitude satisfies

$$
R=r+\frac{t^2e^{i\phi}R}{1-r e^{i\phi}R}.
$$

At $\phi=2\pi j$ this equation reduces to $(R+1)^2=0$: the exact ideal infinite array has unit power reflection there, rather than the first-return approximation's value near $1/4$. This does not change the requested geometric-series derivation, but identifies its physical limitation.

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

Choose the guide axis as $z$, with $0<x<a$ and $0<y<b$. The [electric field](../../electric-field.md) is along $y$, parallel to the walls' $b$ dimension. Take a homogeneous lossless nonmagnetic [dielectric](../../permittivity.md#dielectric) with [relative permittivity](../../quantum-mechanics.md#relative-permittivity) $\epsilon$, ideal conducting walls, and time dependence $e^{-i\omega t}$. The lowest [transverse electric mode of a rectangular waveguide](../../electromagnetic-wave.md#transverse-electric-mode-of-a-rectangular-waveguide) is

$$
\widetilde{\mathbf E}=\widehat{\mathbf y}E_0\sin\!\left(\frac{\pi x}a\right)e^{i\beta z},\qquad
\beta^2=\frac{\epsilon\omega^2}{c^2}-\frac{\pi^2}{a^2},\qquad \omega=2\pi f.
$$

At $x=0,a$, this tangential [electric field](../../electric-field.md) vanishes. At $y=0,b$ the [electric field](../../electric-field.md) is normal to the wall; a nonzero value is supported by surface [electric charge](../../electric-charge.md) and violates no conducting boundary condition. The field has zero [divergence](../../multivariable-calculus.md#divergence). The associated normal [magnetic field](../../magnetic-field.md) also vanishes at each wall, as verified below. The fundamental sine across the wider dimension minimizes the nonzero transverse wave number; $\mathrm{TE}_{00}$ is not a physical propagating mode of a hollow simply connected guide.

Below the [waveguide cutoff frequency](../../electromagnetic-wave.md#waveguide-cutoff-frequency) $f_c=c/(2a\sqrt\epsilon)$, put $\beta=i\kappa$ with $\kappa>0$ to select decay for $z>0$. The [evanescent transverse electric mode in a rectangular waveguide](../../electromagnetic-wave.md#evanescent-transverse-electric-mode-in-a-rectangular-waveguide) then has

$$
\widetilde E_y=E_0\sin(\pi x/a)e^{-\kappa z},\qquad
\boxed{\ell^{-2}=\kappa^2=\pi^2\!\left(\frac1{a^2}-\frac{4\epsilon f^2}{c^2}\right).}
$$

For the fixed [frequency](../../wave.md#frequency) in the question,

$$
\boxed{\frac\ell a=\frac1{\pi\sqrt{1-\epsilon/4}}\quad(0<\epsilon<4).}
$$

The decay length increases monotonically and diverges as $\epsilon\to4^-$; its formal limit at $\epsilon\to0^+$ is $a/\pi$. At $\epsilon=4$ the mode is at cutoff, with zero axial wave number. For $\epsilon>4$, $\beta=(\pi/a)\sqrt{\epsilon/4-1}$ is real and the mode propagates without axial attenuation in this ideal lossless model. There is no real finite evanescent decay length to continue beyond cutoff. The paper's graph notation $l$ denotes the same $\ell$ as its preceding formula.

<a id="section-b/b9/image-evanescent-decay-length-and-propagating-axial-wave-number-on-opposite-sides-of-cutoff"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1-waveguide-cutoff.png)

**[Figure 1](#section-b/b9/image-evanescent-decay-length-and-propagating-axial-wave-number-on-opposite-sides-of-cutoff). Evanescent decay length and propagating axial wave number on opposite sides of cutoff**.

From [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction), $\nabla\times\widetilde{\mathbf E}=i\omega\widetilde{\mathbf B}$. Writing $q=\pi/a$ gives

$$
\boxed{\widetilde B_x=-\frac{i\kappa}{\omega}E_0\sin(qx)e^{-\kappa z},\quad
\widetilde B_y=0,\quad
\widetilde B_z=-\frac{iq}{\omega}E_0\cos(qx)e^{-\kappa z}.}
$$

Thus $B_x$ vanishes on the $x$ walls and $B_y$ vanishes on the $y$ walls, meeting the normal magnetic boundary conditions. The fields also satisfy $\nabla\cdot\mathbf B=0$. For real $E_0$ the physical fields are $E_y=E_0\sin(qx)e^{-\kappa z}\cos\omega t$, $B_x=-(\kappa/\omega)E_0\sin(qx)e^{-\kappa z}\sin\omega t$, and $B_z=-(q/\omega)E_0\cos(qx)e^{-\kappa z}\sin\omega t$.

The time-averaged [Poynting vector](../../electromagnetic-wave.md#poynting-vector) is

$$
\langle\mathbf S\rangle=\frac1{2\mu_0}\operatorname{Re}
(\widetilde{\mathbf E}\times\widetilde{\mathbf B}^{\,*})=\mathbf0,
\qquad \boxed{\langle P_z\rangle=0.}
$$

All products are imaginary because the [electric field](../../electric-field.md) and [magnetic field](../../magnetic-field.md) are in quadrature. A single decaying [evanescent wave](../../elasticity-physics.md#evanescent-wave) stores reactive [energy](../../energy.md) without transmitting average power into a semi-infinite lossless guide. A finite below-cutoff section can transmit power when both independent evanescent solutions are present; that is a different boundary-value problem.

The [skin effect](../../electric-charge.md#skin-effect) also gives exponential field decay, but in a good metal $k$ has both real and imaginary parts and there is a real inward mean [Poynting vector](../../electromagnetic-wave.md#poynting-vector). That flux supplies [Joule heating](../../electric-charge.md#joule-heating) $\sigma|\widetilde E|^2/2$. Here attenuation comes from geometric cutoff in a lossless region, with no conductivity and no dissipative power sink; exponential decay alone does not establish absorption.

## Section C

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

For the attractive [inverse-square force](../../classical-mechanics.md#inverse-square-force), choose zero [potential energy](../../energy.md#potential-energy) at infinity, so $U=-A/r$. At either radial turning point $r_p,r_a$, the [kinetic energy](../../energy.md#kinetic-energy) is purely tangential, with conserved [angular momentum](../../momentum.md#angular-momentum) $J$. Thus

$$
E=\frac{J^2}{2mr^2}-\frac Ar,\qquad
Er^2+Ar-\frac{J^2}{2m}=0.
$$

Its two roots are the periapsis and apoapsis distances. Their sum is $r_p+r_a=-A/E$, whereas the [ellipse](../../euclidean-geometry.md#ellipse) has $r_p+r_a=2a$. Therefore **$a=-A/(2E)$**, with $E<0$ for a nondegenerate bound [ellipse](../../euclidean-geometry.md#ellipse). The circular case follows by the double-root limit.

For the [two-body problem](../../celestial-mechanics.md#two-body-problem), define $\mathbf r=\mathbf r_B-\mathbf r_A$, total [mass](../../classical-mechanics.md#mass) $M=m_A+m_B$, [reduced mass](../../classical-mechanics.md#reduced-mass) $\mu=m_Am_B/M$, and [center of mass](../../classical-mechanics.md#center-of-mass) $\mathbf R$. The relative equation is $\mu\ddot{\mathbf r}=\mathbf F$, while the isolated [center of mass](../../classical-mechanics.md#center-of-mass) has $\ddot{\mathbf R}=0$. Once the relative [orbit](../../dynamical-systems.md#orbit-dynamical-system) is known,

$$
\mathbf r_A=\mathbf R-\frac{m_B}{M}\mathbf r,\qquad
\mathbf r_B=\mathbf R+\frac{m_A}{M}\mathbf r.
$$

The relative [energy](../../energy.md) uses $\mu$ in its [kinetic energy](../../energy.md#kinetic-energy) and $A=Gm_Am_B$ in the gravitational [potential energy](../../energy.md#potential-energy).

In the equal-mass case the initial relative [speed](../../classical-mechanics.md#speed) is $u$, $\mu=m/2$, and the center-of-mass [velocity](../../classical-mechanics.md#velocity) is half B's initial [velocity](../../classical-mechanics.md#velocity). Thus

$$
E_{\rm rel}=\frac14mu^2-\frac{Gm^2}{a_1}.
$$

Negative relative [energy](../../energy.md) requires $u^2<4Gm/a_1$. The **escape threshold is $u_E=2\sqrt{Gm/a_1}$**; equality is marginal parabolic escape, so a strictly bound pair has $u<u_E$.

For $u=u_E/2=\sqrt{Gm/a_1}$, $E_{\rm rel}=-3Gm^2/(4a_1)$ and the relative semimajor axis is $a=2a_1/3$. The initial transverse [speed](../../classical-mechanics.md#speed) is below the relative circular value $\sqrt{2Gm/a_1}$, so the initial turning point is apoapsis. Hence

$$
\boxed{r_p=2a-a_1=\frac{a_1}{3},\qquad e=\frac12.}
$$

Choose the initial separation along $+x$ from A to B, with B's initial [velocity](../../classical-mechanics.md#velocity) $+u\widehat{\mathbf y}$. [Conservation of angular momentum](../../momentum.md#conservation-of-angular-momentum) gives relative periapsis [speed](../../classical-mechanics.md#speed) $3u$. At the opposite end of the [ellipse](../../euclidean-geometry.md#ellipse) the direction is $-\widehat{\mathbf y}$, so

$$
\mathbf V_{\rm CM}=\frac u2\widehat{\mathbf y},\qquad
\mathbf v_{B,p}=\mathbf V_{\rm CM}+\frac12\mathbf v_{{\rm rel},p}
=\boxed{-u\widehat{\mathbf y}}.
$$

Thus B has the same [speed](../../classical-mechanics.md#speed) as initially but the opposite [velocity](../../classical-mechanics.md#velocity). A has $2u\widehat{\mathbf y}$ at that instant. A value $3u/2$ for B would be its center-of-mass-frame [speed](../../classical-mechanics.md#speed), not the requested initial laboratory frame result.

The relative [orbital period](../../celestial-mechanics.md#orbital-period) follows from [Kepler's third law](../../mathematical-physics.md#kepler-s-third-law) with total gravitating [mass](../../classical-mechanics.md#mass) $2m$:

$$
\boxed{T=2\pi\sqrt{\frac{(2a_1/3)^3}{2Gm}}
=\frac{4\pi}{3\sqrt3}\sqrt{\frac{a_1^3}{Gm}}
=\frac{4\pi a_1}{3\sqrt3\,u}.}
$$

In the center-of-mass frame each star follows an [ellipse](../../euclidean-geometry.md#ellipse) of semimajor axis $a_1/3$ and [eccentricity](../../euclidean-geometry.md#eccentricity-of-a-conic) $1/2$, with the [center of mass](../../classical-mechanics.md#center-of-mass) at a focus; they remain opposite on their simultaneous position vectors. In the laboratory frame add the uniform drift $ut/2$ along $y$. The [laboratory paths of an equal-mass binary](../../celestial-mechanics.md#laboratory-paths-of-an-equal-mass-binary) are therefore not closed [ellipses](../../euclidean-geometry.md#ellipse), even though their relative motion repeats.

<a id="section-c/c10/image-equal-mass-binary-trajectories-in-the-center-of-mass-frame-and-the-original-laboratory-frame"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1-binary-orbits.png)

**[Figure 2](#section-c/c10/image-equal-mass-binary-trajectories-in-the-center-of-mass-frame-and-the-original-laboratory-frame). Equal-mass binary trajectories in the center-of-mass frame and the original laboratory frame**.

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/solution">Solution</h4>

↑ **Parent:** [C11](#section-c/c11)

In [Lagrangian mechanics](../../lagrangian-mechanics.md), choose independent [generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate) $q_i$ compatible with the mechanical [constraints](../../classical-mechanics.md#constraint-mechanics), write $L=T-U$, and apply the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation)

$$
\frac d{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.
$$

Equivalently, the physical path makes the [action](../../lagrangian-mechanics.md#action) stationary under variations with fixed endpoints. For ideal holonomic [constraints](../../classical-mechanics.md#constraint-mechanics), their unknown reaction forces need not appear in the reduced equations. Direct use of [Newton's laws of motion](../../force.md#newton-s-laws-of-motion) instead resolves vector [forces](../../force.md) and reactions and enforces the [constraints](../../classical-mechanics.md#constraint-mechanics) separately. Both approaches describe the same mechanics; the scalar [Lagrangian](../../calculus-of-variations.md#lagrangian) is often shorter in curvilinear coordinates. Nonconservative generalized forces must be added separately. Here a drive maintains the prescribed azimuthal [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\Omega$.

The mass has polar [speed](../../classical-mechanics.md#speed) $a\dot\theta$ and azimuthal [speed](../../classical-mechanics.md#speed) $a\Omega\sin\theta$, so its [kinetic energy](../../energy.md#kinetic-energy) is $ma^2(\dot\theta^2+\Omega^2\sin^2\theta)/2$. The elastic [potential energy](../../energy.md#potential-energy) is $\mu\theta^2/2$, and the height is $a\cos\theta$, giving gravitational [potential energy](../../energy.md#potential-energy) $mga\cos\theta$. Therefore

$$
L=\frac12ma^2\dot\theta^2+\frac12ma^2\Omega^2\sin^2\theta
-\frac12\mu\theta^2-mga\cos\theta,
$$

and the [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) gives

$$
\boxed{\ddot\theta=\Omega^2\sin\theta\cos\theta
-\frac\mu{ma^2}\theta+\frac ga\sin\theta.}
$$

For $\mu=2mga$, define $q=\Omega^2a/g$ and $F(\theta)=q\sin\theta\cos\theta-2\theta+\sin\theta$, so $\ddot\theta=(g/a)F(\theta)$. Near zero,

$$
F(\theta)=(q-1)\theta-\left(\frac{2q}{3}+\frac16\right)\theta^3+O(\theta^5).
$$

When $q<1$ the upright [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is linearly stable and the [small oscillations](../../lagrangian-mechanics.md#small-oscillation) have **$\omega_1^2=g/a-\Omega^2$**.

For $q>1$, the graph of $F$ initially rises, whereas $F(\pi/2)=1-\pi<0$. There must therefore be a zero inside the interval. More strongly, for $0<\theta<\pi/2$,

$$
\frac{F(\theta)}{\sin\theta}=q\cos\theta+1-\frac{2\theta}{\sin\theta}
$$

is strictly decreasing: $\cos\theta$ decreases and $\theta/\sin\theta$ increases because $\sin\theta-\theta\cos\theta>0$. The ratio goes from $q-1>0$ to $1-\pi<0$, giving exactly one zero $\theta_0$ in that interval. At the zero, $F'(\theta_0)<0$, so it is a stable [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). The [rotating torsion-stabilized inverted pendulum](../../classical-mechanics.md#rotating-torsion-stabilized-inverted-pendulum) also has a symmetric stable angle $-\theta_0$ if both signs of tilt are permitted.

<a id="section-c/c11/image-acceleration-curves-after-the-upright-instability-and-the-quartic-potential-at-the-threshold"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1-rotating-pendulum.png)

**[Figure 3](#section-c/c11/image-acceleration-curves-after-the-upright-instability-and-the-quartic-potential-at-the-threshold). Acceleration curves after the upright instability and the quartic potential at the threshold**.

At $\theta_0=\pi/4$, setting $F(\theta_0)=0$ gives $q/2-\pi/2+1/\sqrt2=0$, so

$$
\boxed{\Omega=\sqrt{\frac ga(\pi-\sqrt2)}.}
$$

For $\theta=\theta_0+\xi$, the linearized equation is $\ddot\xi=(g/a)F'(\theta_0)\xi$. Since $F'=q\cos2\theta-2+\cos\theta$,

$$
\boxed{\omega_2^2=\frac ga\left(2-\frac1{\sqrt2}\right).}
$$

At the threshold $q=1$ the linear restoring term vanishes, but the cubic term remains:

$$
\ddot\theta=-\frac{5g}{6a}\theta^3+O(\theta^5),\qquad
U_{\rm eff}(\theta)-U_{\rm eff}(0)=\frac{5mga}{24}\theta^4+O(\theta^6).
$$

**The upright state remains nonlinearly stable, with no nonzero infinitesimal harmonic frequency.** Small finite disturbances produce [quartic oscillator](../../classical-mechanics.md#quartic-oscillator) motion whose [frequency](../../wave.md#frequency) is proportional to its small angular [amplitude](../../wave.md#wave-amplitude); its [period](../../mathematics.md#period-of-a-function) tends to infinity as that amplitude tends to zero. Zero linear stiffness is not the same as an absent restoring [torque](../../momentum.md#torque).

<h3 id="section-c/12">12</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/12/solution">Solution</h4>

↑ **Parent:** [12](#section-c/12)

Use positive [normal stress](../../continuum-mechanics.md#normal-stress) for tension. On a small rectangular material element, $\tau_i$ is the normal force per unit area on the face perpendicular to axis $i$, and $e_i=\Delta\ell_i/\ell_i$ is the corresponding [normal strain](../../continuum-mechanics.md#normal-strain). [Young's modulus](../../elasticity-physics.md#young-s-modulus) $E$ is the ratio of axial [normal stress](../../continuum-mechanics.md#normal-stress) to axial [strain](../../continuum-mechanics.md#strain) in uniaxial stress; [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio) $\sigma$ is minus the transverse-to-axial strain ratio in the same test. Thus isotropic [linear elasticity](../../elasticity-physics.md#linear-elasticity) gives $Ee_1=\tau_1-\sigma\tau_2-\sigma\tau_3$ and cyclic permutations. The stress symbols here follow the question; $\sigma$ denotes [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio), not a stress component.

<a id="section-c/12/image-normal-stresses-on-a-material-element-and-the-distinct-deformation-fields-in-twist-and-tilt"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1-elastic-layer.png)

**[Figure 4](#section-c/12/image-normal-stresses-on-a-material-element-and-the-distinct-deformation-fields-in-twist-and-tilt). Normal stresses on a material element and the distinct deformation fields in twist and tilt**.

For $e_2=e_3=0$, the two transverse compliance equations imply $\tau_2=\tau_3=\sigma\tau_1/(1-\sigma)$. Substitution into the first gives

$$
Ee_1=\frac{(1+\sigma)(1-2\sigma)}{1-\sigma}\tau_1,\qquad
\boxed{M=\frac{E(1-\sigma)}{(1+\sigma)(1-2\sigma)}.}
$$

This [uniaxial strain modulus](../../elasticity-physics.md#uniaxial-strain-modulus) is greater than the uniaxial-stress [Young's modulus](../../elasticity-physics.md#young-s-modulus) for the positive [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio) of interest, because the lateral [constraints](../../classical-mechanics.md#constraint-mechanics) prevent free Poisson contraction.

For a small twist $\phi$, the bonded faces' relative tangential displacement at radius $r$ is $r\phi$. The layer's [shear strain](../../continuum-mechanics.md#shear-strain) is $r\phi/h$, so the [shear stress](../../viscous-fluid-flow.md#shear-stress) is $Gr\phi/h$. Integrating the [torque](../../momentum.md#torque) gives

$$
T_V=-\frac{G\phi}h\int_A r^2\,dA
=-\frac{G\phi}h\int_0^a2\pi r^3dr
=\boxed{-\frac\pi2\frac{Ga^4}h\phi.}
$$

The minus sign denotes a restoring [torque](../../momentum.md#torque); the question quotes its magnitude. This uses the disk's [polar second moment of area](../../elasticity-physics.md#polar-second-moment-of-area).

For tilt about H, choose $y$ in the plate perpendicular to H. The vertical displacement of the bonded top face is $y\theta$ to first order, giving [normal strain](../../continuum-mechanics.md#normal-strain) $y\theta/h$. The thin layer is constrained laterally by bonding, so its leading normal traction is $My\theta/h$, not $Ey\theta/h$. Integrating its moment about H gives

$$
T_H=-\frac{M\theta}h\int_Ay^2dA
=\boxed{-\frac\pi4\frac{Ma^4}h\theta,}
$$

since the diametric [second moment of area](../../elasticity-physics.md#second-moment-of-area) is $\pi a^4/4$. This is the specified thin-layer approximation to the [torsion and tilt stiffness of a bonded elastic disk](../../elasticity-physics.md#torsion-and-tilt-stiffness-of-a-bonded-elastic-disk). Relaxation near the free cylindrical edge is neglected; for a nearly incompressible layer it can limit quantitative accuracy unless the thinness is sufficient.

The thin square plate's [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) about V is $I_V=2mb^2/3$. Its two perpendicular in-plane central moments are equal and sum to $I_V$, so the diagonal H has $I_H=mb^2/3$. Dividing the two angular stiffnesses by the appropriate [moments of inertia](../../rigid-body-dynamics.md#moment-of-inertia) gives

$$
\boxed{\omega_V=\sqrt{\frac{3\pi Ga^4}{4hmb^2}},\qquad
\omega_H=\sqrt{\frac{3\pi Ma^4}{4hmb^2}}.}
$$

The geometry factors cancel in their ratio. Using the supplied relation between [shear modulus](../../elasticity-physics.md#shear-modulus) and [Young's modulus](../../elasticity-physics.md#young-s-modulus),

$$
R^2=\left(\frac{\omega_H}{\omega_V}\right)^2=\frac MG
=\frac{2(1-\sigma)}{1-2\sigma},\qquad
\boxed{\sigma=\frac{R^2-2}{2(R^2-1)}=0.4919\quad(R=7.9).}
$$

The result lies just below the incompressible isotropic limit $1/2$, as expected for a rubber with a large compression stiffness compared with its [shear modulus](../../elasticity-physics.md#shear-modulus). It is an inference within the bonded-layer model, rather than an independently measured material constant.

<h3 id="section-c/13">13</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/13/solution">Solution</h4>

↑ **Parent:** [13](#section-c/13)

For a [Newtonian fluid](../../viscous-fluid-flow.md#newtonian-fluid) with [velocity](../../classical-mechanics.md#velocity) $u(z)\widehat{\mathbf x}$, $\tau=\eta\,\partial_z u$ is the $x$ component of traction on a plane whose normal points along $+z$. The opposite face has the opposite traction. The coefficient $\eta$ is [dynamic viscosity](../../dynamic-viscosity.md), with units $\mathrm{Pa\,s}$. Faster layers transfer positive $x$ [momentum](../../momentum.md) toward slower neighbours; the internal [shear stress](../../viscous-fluid-flow.md#shear-stress) resists relative sliding.

<a id="section-c/13/image-shear-traction-convention-couette-poiseuille-profiles-and-oscillatory-viscous-penetration"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2015/paper-1-viscous-flow.png)

**[Figure 5](#section-c/13/image-shear-traction-convention-couette-poiseuille-profiles-and-oscillatory-viscous-penetration). Shear-traction convention, Couette-Poiseuille profiles, and oscillatory viscous penetration**.

Take a thin fluid element with horizontal area $A$ and thickness $dz$. The difference between its upper and lower viscous tractions is $A\eta u_{zz}dz$. The [pressure gradient](../../fluid-mechanics.md#pressure-gradient) supplies $-A p_xdz$. Incompressibility is satisfied because $u$ has no $x$ dependence, and the convective [acceleration](../../classical-mechanics.md#acceleration) vanishes: $(\mathbf u\cdot\nabla)\mathbf u=u\partial_x\mathbf u=0$. Equating net force to [mass](../../classical-mechanics.md#mass) times [acceleration](../../classical-mechanics.md#acceleration) therefore gives the relevant component of the [Navier-Stokes equation](../../viscous-fluid-flow.md#navier-stokes-equation):

$$
\boxed{\rho\frac{\partial u}{\partial t}=-\frac{\partial p}{\partial x}
+\eta\frac{\partial^2u}{\partial z^2}.}
$$

For steady flow, integrate $\eta u''=p'$ twice and impose the [no-slip boundary condition](../../viscous-fluid-flow.md#no-slip-boundary-condition) at each plate, $u(0)=0$ and $u(a)=u_0$. The [Couette-Poiseuille flow](../../viscous-fluid-flow.md#couette-poiseuille-flow) profile is

$$
\boxed{u(z)=u_0\frac za+\frac{p'}{2\eta}z(z-a).}
$$

The linear term is [Couette flow](../../viscous-fluid-flow.md#couette-flow) and the parabolic term is [plane Poiseuille flow](../../viscous-fluid-flow.md#plane-poiseuille-flow). A negative $p'$ drives flow in $+x$. Integrating the profile across the gap gives the volumetric flow per unit width,

$$
\boxed{q=\int_0^au(z)\,dz=\frac{u_0a}{2}-\frac{p'a^3}{12\eta}.}
$$

It has units $\mathrm{m^2\,s^{-1}}$; multiplying by the plate width gives the actual volume per time.

With zero [pressure gradient](../../fluid-mechanics.md#pressure-gradient), substituting $u=\operatorname{Re}[A e^{i(kz-\omega t)}]$ gives $-i\rho\omega=-\eta k^2$. Select the root that decays into fluid occupying $z>0$:

$$
\boxed{k=(1+i)\sqrt{\frac{\rho\omega}{2\eta}}=\frac{1+i}{\delta},\qquad
\delta=\sqrt{\frac{2\eta}{\rho\omega}}.}
$$

The other sign applies to decay in the opposite half-space. With a real wall velocity amplitude $U_0$, the established periodic solution of [Stokes' second problem](../../viscous-fluid-flow.md#stokes-second-problem) is

$$
u(z,t)=U_0e^{-z/\delta}\cos(z/\delta-\omega t).
$$

The oscillation's [amplitude](../../wave.md#wave-amplitude) decays exponentially and its phase lags with distance from the plate. This is diffusion of tangential [momentum](../../momentum.md), not a freely propagating undamped elastic wave. Initial transients must have decayed before this purely periodic expression applies.

The fluid-displacement amplitude and the wall-displacement amplitude have the same ratio as their velocity amplitudes, since both are divided by the common $\omega$. Thus for the specified amplitudes,

$$
\frac{0.002}{0.10}=e^{-z/\delta},\qquad
\boxed{z=\sqrt{\frac{2\eta}{\rho(2\pi f)}}\ln50.}
$$

Using the standard approximate water [density](../../fluid-mechanics.md#density) $\rho\simeq10^3\ \mathrm{kg\,m^{-3}}$, explicitly an approximation rather than another value printed on the paper, gives $\delta=0.564\ \mathrm{mm}$ and **$z\simeq2.21\ \mathrm{mm}$ from either face of a sufficiently large plate**. The [viscous penetration depth](../../viscous-fluid-flow.md#viscous-penetration-depth) varies as $\rho^{-1/2}$ if a more precise water [density](../../fluid-mechanics.md#density) is used. The ideal parallel-flow solution ignores finite plate edges and tank walls.

## ↑ Ancestors (11)

1. [2015](../2015.md)
2. [Past exam of the physics B course of the University of Cambridge](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge.md)
3. [Physics B course of the University of Cambridge](../../university-of-cambridge.md#physics-b-course-of-the-university-of-cambridge)
4. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
