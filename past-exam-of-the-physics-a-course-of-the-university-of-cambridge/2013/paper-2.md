# Paper 2

↑ **Parent:** [2013](../2013.md)

[Original public PDF, physical pages 79–85](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1)

**Table of contents**

- [Section A](#section-a)
  - [1](#section-a/1)
    - [Solution](#section-a/1/solution)
  - [2](#section-a/2)
    - [Solution](#section-a/2/solution)
  - [3](#section-a/3)
    - [Solution](#section-a/3/solution)
  - [4](#section-a/4)
    - [Solution](#section-a/4/solution)
  - [5](#section-a/5)
    - [Solution](#section-a/5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [Solution](#section-b/b6/solution)
    - [a](#section-b/b6/a)
      - [Solution](#section-b/b6/a/solution)
    - [b](#section-b/b6/b)
      - [Solution](#section-b/b6/b/solution)
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
- [Section D](#section-d)
  - [D12](#section-d/d12)
    - [Solution](#section-d/d12/solution)
  - [D13](#section-d/d13)
    - [a](#section-d/d13/a)
      - [Solution](#section-d/d13/a/solution)
    - [b](#section-d/d13/b)
      - [Solution](#section-d/d13/b/solution)
    - [c](#section-d/d13/c)
      - [Solution](#section-d/d13/c/solution)

## Section A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-a/1">1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/1/solution">Solution</h4>

↑ **Parent:** [1](#section-a/1)

The [wavelength](../../wave-equation.md#wavelength) is $\lambda=c/f\simeq0.020\ \mathrm m$. The longest [interferometric baseline](../../astrophysics.md#interferometric-baseline) measures the finest angular structure and the [shortest-baseline angular scale](../../astrophysics.md#shortest-baseline-angular-scale) describes the coarsest:

$$
\boxed{\theta_{\rm res}\sim\frac\lambda{B_{\max}}=2.0\times10^{-4}\ \mathrm{rad}\simeq41'',\qquad
\theta_{\rm large}\sim\frac\lambda{B_{\min}}=4.0\times10^{-3}\ \mathrm{rad}\simeq14'}.
$$

These are order-of-magnitude scales, not sharp cutoffs. A commonly used maximum-recoverable-scale convention is $0.6\lambda/B_{\min}$, giving about $8.2'$; reconstruction also depends on baseline coverage and source structure. The individual antenna's [primary beam](../../astrophysics.md#primary-beam) is a separate field-of-view limit.[“Interferometry”, “Field of view”, and “Imaging of extended structures”](../../physics-bibliography.md#alma-basics-by-national-radio-astronomy-observatory)

<h3 id="section-a/2">2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/2/solution">Solution</h4>

↑ **Parent:** [2](#section-a/2)

A thin [antireflection coating](../../physical-optics.md#antireflection-coating) makes [reflections](../../linear-algebra.md#reflection-mathematics) from its two interfaces interfere destructively near a chosen [wavelength](../../wave-equation.md#wavelength), often in the green part of the visible spectrum. For a single lossless layer at [normal incidence](../../optics.md#normal-incidence), $n_fd=\lambda_0/4$ and ideally $n_f=\sqrt{n_0n_s}$ minimize [reflection](../../linear-algebra.md#reflection-mathematics) at $\lambda_0$. [reflection](../../linear-algebra.md#reflection-mathematics) is less completely cancelled in the red and blue, so **the residual reflected light can appear purple**. This is primarily a [reflection](../../linear-algebra.md#reflection-mathematics) colour, not a claim that the transmitted beam is strongly purple. Multilayer coatings can broaden the low-reflectance band.

<h3 id="section-a/3">3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/3/solution">Solution</h4>

↑ **Parent:** [3](#section-a/3)

Sound compressions in air are approximately adiabatic, giving $c_s^2=(\partial p/\partial\rho)_s=\gamma p/\rho$. With $p=\rho RT/M$,

$$
\boxed{T=\frac{Mc_s^2}{\gamma R}\simeq255\ \mathrm K\simeq-18\ ^\circ\mathrm C}.
$$

Here dry air is approximated as a diatomic [ideal gas](../../ideal-gas.md) with $\gamma=7/5$ and [molar mass](../../chemistry.md#molar-mass) $M\simeq0.029\ \mathrm{kg\,mol^{-1}}$. The ideal-gas law alone is insufficient without this adiabatic response and mean molecular [mass](../../classical-mechanics.md#mass); humidity and composition affect a more precise inference.

<h3 id="section-a/4">4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/4/solution">Solution</h4>

↑ **Parent:** [4](#section-a/4)

For conventional cubic cell side $a$, the [face-centered cubic lattice](../../quantum-scattering.md#face-centered-cubic-lattice) has corner and face-centre sites, giving four lattice points per cell; the [body-centered cubic lattice](../../quantum-scattering.md#body-centered-cubic-lattice) has corners and a body centre, giving two. Their [primitive unit cells](../../quantum-scattering.md#primitive-unit-cell) each contain one lattice point. With reciprocal vectors written $\mathbf G=(2\pi/a)(h,k,l)$, [face-centered cubic lattice](../../quantum-scattering.md#face-centered-cubic-lattice) allows $h,k,l$ all even or all odd, while [body-centred cubic](../../quantum-scattering.md#body-centered-cubic-lattice) allows $h+k+l$ even. Hence

$$
\boxed{\text{fcc}\longleftrightarrow\text{bcc in reciprocal space},\qquad a^*=4\pi/a}.
$$

Here $a^*$ is the side of the [reciprocal lattice](../../quantum-scattering.md#reciprocal-lattice)'s conventional cubic cell. The parity conditions describe the reciprocal point sets; reciprocal space contains [wavevectors](../../elasticity-physics.md#wavevector), not a second arrangement of physical atoms.

<h3 id="section-a/5">5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/5/solution">Solution</h4>

↑ **Parent:** [5](#section-a/5)

In the [Hall effect](../../relativistic-electromagnetism.md#hall-effect), the [Lorentz force](../../relativistic-electromagnetism.md#lorentz-force) deflects drifting [charge carriers](../../electric-charge.md#charge-carrier) until a transverse [electric field](../../electric-field.md) balances it: $\mathbf E_H=-\mathbf v_d\times\mathbf B$. Choose current along $x$, field along $z$ and define $R_H=E_y/(j_xB_z)$. Since $j_x=nqv_x$,

$$
\boxed{R_H=\frac1{nq},\qquad n=\frac1{e|R_H|}\quad\text{for electron carriers}}.
$$

The sign is negative for [electrons](../../physics.md#electron) with this convention. If the sample's [mass density](../../fluid-mechanics.md#density) is $\rho_m$ and its [molar mass](../../chemistry.md#molar-mass) is $M$, the atomic [number density](../../statistical-physics.md#number-density) is $n_{\rm at}=\rho_mN_A/M$, so

$$
\boxed{z_{\rm free}=\frac n{n_{\rm at}}=\frac{M}{e|R_H|\rho_mN_A}}.
$$

Measure the transverse voltage, specimen thickness, current and [magnetic field](../../magnetic-field.md); reversing field and current helps remove longitudinal-voltage pickup and offsets. This [free-electron count from a Hall coefficient](../../relativistic-electromagnetism.md#free-electron-count-from-a-hall-coefficient) assumes one approximately free carrier band. Multiple bands, unequal mobilities or a complicated [Fermi surface](../../fermi-liquid.md#fermi-surface) can make a [Hall coefficient](../../relativistic-electromagnetism.md#hall-coefficient) differ from $-1/(ne)$.

## Section B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/solution">Solution</h4>

↑ **Parent:** [B6](#section-b/b6)

**[time average of harmonic power](../../linear-acoustics.md#time-average-of-harmonic-power).** Expand the two [real parts](../../complex-analysis.md#real-part):

$$
\langle\operatorname{Re}F\operatorname{Re}u\rangle
=\frac14\langle Fu+Fu^*+F^*u+F^*u^*\rangle
=\boxed{\frac12\operatorname{Re}(Fu^*)}.
$$

The terms proportional to $e^{\pm2i\omega t}$ average to zero over complete periods, while $Fu^*$ is time-independent. For real peak amplitudes this is $F_0u_0\cos\phi/2$.

**String dynamics.** A short element of length $dx$ experiences transverse [force](../../force.md) $T[\psi_x(x+dx)-\psi_x(x)]$. [Newton's second law](../../force.md#newton-s-second-law) therefore gives $\rho\,dx\,\psi_{tt}=T\,dx\,\psi_{xx}$, or

$$
\boxed{\psi_{xx}=\frac1{v^2}\psi_{tt},\qquad v=\sqrt{T/\rho}}.
$$

The approximation is a flexible, lossless string with small slope and constant [tension](../../force.md#tension); $\rho$ is its [linear mass density](../../fluid-mechanics.md#linear-mass-density).

**[energy](../../energy.md) transport.** Across a cut toward increasing $x$, the transverse [force](../../force.md) is $F_y=-T\psi_x$ and the transverse velocity is $u=\psi_t$. For a rightgoing wave these have [complex amplitudes](../../wave.md#complex-amplitude) $ikTA$ and $i\omega A$. Hence

$$
\boxed{Z=\frac Tv=\rho v=\sqrt{T\rho},\qquad
\langle P\rangle=\frac12Z\omega^2|A_0|^2}.
$$

This real [mechanical impedance](../../classical-mechanics.md#mechanical-impedance) is [force](../../force.md) divided by transverse velocity for a [travelling wave](../../analysis.md#travelling-wave), with units $\mathrm{kg\,s^{-1}}$.

**Matching and [power](../../energy.md#power) ratios.** At an ordinary massless junction without an external transverse [force](../../force.md), displacement is continuous and transverse [tension](../../force.md#tension) is balanced: $\psi_1=\psi_2$, $T_1\psi_{1x}=T_2\psi_{2x}$. For the same [tension](../../force.md#tension), the slope is therefore continuous even if density changes. With real positive impedances,

$$
r_\psi=\frac{Z_1-Z_2}{Z_1+Z_2},\quad t_\psi=\frac{2Z_1}{Z_1+Z_2},
\qquad
\boxed{P_r=\frac{(Z_1-Z_2)^2}{(Z_1+Z_2)^2}P_i,\quad
P_t=\frac{4Z_1Z_2}{(Z_1+Z_2)^2}P_i}.
$$

Their sum equals $P_i$; the transmitted [power](../../energy.md#power) includes the impedance ratio and is not simply $t_\psi^2P_i$.

<h4 id="section-b/b6/a">a</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b6/a)

Substituting $Z_j=\sqrt{T\rho_j}$ into the junction formula gives

$$
\boxed{\frac{P_r}{P_i}=\left(\frac{\sqrt{\rho_1}-\sqrt{\rho_2}}{\sqrt{\rho_1}+\sqrt{\rho_2}}\right)^2,\qquad
\frac{P_t}{P_i}=\frac{4\sqrt{\rho_1\rho_2}}{(\sqrt{\rho_1}+\sqrt{\rho_2})^2}}.
$$

Equal densities give zero [reflection](../../linear-algebra.md#reflection-mathematics); a very large mismatch gives nearly complete [reflection](../../linear-algebra.md#reflection-mathematics). [reflection](../../linear-algebra.md#reflection-mathematics) from the higher-impedance side reverses displacement phase.

<h4 id="section-b/b6/b">b</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b6/b)

At the zero-slope boundary, the rightgoing and leftgoing slopes cancel, so $A_r=A_i$. Consequently

$$
\boxed{r_\psi=+1,\qquad P_r=P_i,\qquad P_t=0}.
$$

This [free-end reflection of a transverse string wave](../../wave-equation.md#free-end-reflection-of-a-transverse-string-wave) uses a [Neumann boundary condition](../../differential-equation.md#neumann-boundary-condition): the displacement has an antinode and is not forced to vanish. The instantaneous flux $-T\psi_x\psi_t$ through the boundary is zero, confirming that it transmits no [power](../../energy.md#power).

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

**Response and [resonance](../../dynamical-systems.md#resonance).** The terms $m\ddot x$, $b\dot x$ and $kx$ describe inertia, linear viscous resistance and the spring's restoring [force](../../force.md); the right side is the applied harmonic [force](../../force.md). Substituting the complex trial motion and taking [real parts](../../complex-analysis.md#real-part) gives

$$
\boxed{A=R(\omega)F_0,\qquad R(\omega)=\frac1{k-m\omega^2+ib\omega}}.
$$

The steady response excludes the decaying homogeneous transient. Its magnitude is $[(k-m\omega^2)^2+b^2\omega^2]^{-1/2}$. Differentiating the denominator gives $2\omega[-2m(k-m\omega^2)+b^2]=0$, so

$$
\boxed{\omega_{\rm res}=\sqrt{k/m-b^2/(2m^2)}}.
$$

A nonzero-frequency amplitude maximum exists only for $b^2<2km$; otherwise the maximum is at zero [frequency](../../wave.md#frequency). Increasing [damping](../../wave-equation.md#damping) lowers and broadens the peak and shifts it downward. Every curve starts at $|R(0)|=1/k$ and tends to $1/(m\omega^2)$ at high [frequency](../../wave.md#frequency).

<a id="section-b/b7/image-original-normalized-oscillator-response-for-several-damping-ratios-distinguishing-amplitude-and-current-resonance"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2-response-resonance.png)

**[Figure 1](#section-b/b7/image-original-normalized-oscillator-response-for-several-damping-ratios-distinguishing-amplitude-and-current-resonance). Original normalized oscillator response for several damping ratios, distinguishing amplitude and current resonance**.

**Series circuit.** The PDF circuit has the [resistor](../../electric-charge.md#resistor), [inductor](../../electromagnetism.md#inductor) and [capacitor](../../electromagnetism.md#capacitor) in one loop. With current $I=\dot q$, [Kirchhoff's voltage law](../../random-walk.md#kirchhoff-cycle-law) gives $V=L\dot I+RI+q/C$, hence

$$
\boxed{L\ddot q+R\dot q+q/C=V}.
$$

Thus $m,b,k$ correspond to $L,R,1/C$. The [resistor](../../electric-charge.md#resistor)'s rms voltage is

$$
V_{R,\rm rms}=\frac{|V_0|}{\sqrt2}\frac{R}{\sqrt{R^2+(\omega L-1/(\omega C))^2}}.
$$

It is maximized exactly at $\omega_{\max}=\omega_0=1/\sqrt{LC}$ for $R>0$. The charge-amplitude [resonance](../../dynamical-systems.md#resonance) is lower. Expanding its square root for $R^2C/L\ll1$ gives

$$
\boxed{\omega_{\max}-\omega_{\rm res}
=\omega_0-\sqrt{\omega_0^2-R^2/(2L^2)}
\simeq\frac{R^2}{4L}\sqrt{\frac CL}}.
$$

The two maxima refer to different observables: [resistor](../../electric-charge.md#resistor) voltage follows current, whereas charge follows displacement.

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/solution">Solution</h4>

↑ **Parent:** [B8](#section-b/b8)

**Packet and group index.** A [wave packet](../../dispersion-relation.md#wave-packet) superposes nearby [wavevectors](../../elasticity-physics.md#wavevector) to form a localized envelope. The [phase velocity](../../dispersion-relation.md#phase-velocity) is $v_p=\omega/k$; for a narrow packet with weak distortion the envelope velocity is $v_g=d\omega/dk$. Since $k=2\pi fn(f)/c$,

$$
\boxed{\frac c{v_g}=n_g=n+f\frac{dn}{df}}.
$$

For the stipulated linear index, $n_g=1.5+\tau(2f-f_0)$, not simply $n(f)$.

**[bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) and speed spread.** A pulse lasting $t_p$ has Fourier [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) of order $1/t_p$, so $\Delta f\sim10^{10}\ \mathrm{Hz}$; an exact width coefficient depends on pulse shape and width convention. At the carrier,

$$
\boxed{n_g(f_0)=1.56,\qquad v_g(f_0)=\frac c{1.56}\simeq1.92\times10^8\ \mathrm{m\,s^{-1}}}.
$$

Across a full [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) $\Delta f$,

$$
\Delta n_g=2\tau\Delta f=6.0\times10^{-6},\qquad
\boxed{\Delta v_g\simeq\frac{2c\tau\Delta f}{1.56^2}\simeq7.4\times10^2\ \mathrm{m\,s^{-1}}}.
$$

Higher-frequency components have the lower [group velocity](../../dispersion-relation.md#group-velocity). For a band symmetric about $f_0$, the endpoint velocities are approximately $v_g(f_0)\pm370\ \mathrm{m\,s^{-1}}$.

**[dispersion-limited digital-fibre link length](../../dispersion-relation.md#dispersion-limited-digital-fibre-link-length).** Differential [group delay](../../physical-optics.md#group-delay) accumulates as

$$
\Delta t_{\rm disp}=L\Delta(1/v_g)=\frac{2\tau L\Delta f}{c}
\simeq(2.0\times10^{-14}\ \mathrm{s\,m^{-1}})L.
$$

The pulse spacing is $t_r=10^{-9}\ \mathrm s$. Pulse overlap and intersymbol interference become serious when the dispersive spread approaches that spacing, giving

$$
\boxed{L_{\max}\sim\frac{ct_r}{2\tau\Delta f}\simeq50\ \mathrm{km}}.
$$

A conservative full-width estimate $t_p+\Delta t_{\rm disp}\lesssim t_r$ gives about **45 km**; this refinement is not a universal sharp boundary because pulse shape, chirp and detection tolerance are unspecified. Attenuation and modal or waveguide dispersion could impose further limits, but are not quantified by the supplied index law.

**[digital optical pulse regeneration](../../dispersion-relation.md#digital-optical-pulse-regeneration).** Each stage must recover and regenerate the data with fresh, short pulses and correct timing, as well as restore signal level. Amplifying the already broadened waveform alone does not remove accumulated dispersion; explicit dispersion compensation is an alternative to full regeneration.

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

**Far-field transform.** For transverse aperture scale $b$ and screen distance $z$, the quadratic phase across the aperture is negligible when $kb^2/(2z)\ll1$, equivalently a small [Fresnel number](../../physical-optics.md#fresnel-number) up to geometrical factors. Expanding the source-to-screen distance at transverse screen coordinate $X$ gives

$$
r\simeq z+\frac{X^2}{2z}-\frac{Xx}{z}+\frac{x^2}{2z}.
$$

Dropping the final aperture-dependent term and treating the prefactor as constant gives

$$
U(X)\propto\frac{e^{ikz+ikX^2/(2z)}}z\int h(x)e^{-i(kX/z)x}dx,
\qquad
\boxed{I(\theta)\propto\left|\int h(x)e^{-ikx\sin\theta}dx\right|^2}.
$$

Thus intensity is the modulus squared of the aperture [Fourier transform](../../fourier-transform.md). A lens [focal plane](../../optical-instrument.md#focal-plane) supplies the same angular transform without a very distant screen. The infinitely extended vertical dimension is treated per unit vertical extent.

**[half-slit phase-reversal diffraction](../../physical-optics.md#half-slit-phase-reversal-diffraction).** Put $h=-1$ on the left half and $h=1$ on the right half. With $q=k\sin\theta$ and $s=qb/4$,

$$
H(q)=\int_0^{b/2}e^{-iqx}dx-\int_{-b/2}^0e^{-iqx}dx
=\frac{4\sin^2(qb/4)}{iq}.
$$

Therefore

$$
\boxed{I(\theta)\propto\frac{\sin^4(kb\sin\theta/4)}{\sin^2\theta}}.
$$

The apparent singularity at zero angle is removable: $H\to0$, so the centre is dark. Normalizing by the uncoated slit's on-axis intensity $I_0$ gives $I/I_0=\sin^4s/s^2$. Noncentral zeros have $s=j\pi$, or $\sin\theta=2j\lambda/b$. The two largest lobes are symmetric, at the first nonzero root of $\tan s=2s$, $s\simeq\pm1.166$, giving $\sin\theta\simeq\pm0.742\lambda/b$ when those directions propagate. Smaller lobes lie farther out under a decaying envelope.

<a id="section-b/b9/image-original-calculated-half-slit-phase-reversal-pattern-and-its-change-when-the-phase-layer-thickness-is-doubled"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2-phase-slit.png)

**[Figure 2](#section-b/b9/image-original-calculated-half-slit-phase-reversal-pattern-and-its-change-when-the-phase-layer-thickness-is-doubled). Original calculated half-slit phase-reversal pattern and its change when the phase-layer thickness is doubled**.

**Doubled thickness.** Neglecting absorption and interface [reflection](../../linear-algebra.md#reflection-mathematics), the phase delay doubles from $\pi$ to $2\pi$. Both halves then transmit with the same phase, recovering the ordinary single-slit pattern

$$
\boxed{I/I_0=\left[\frac{\sin(qb/2)}{qb/2}\right]^2}.
$$

It has a bright centre and first zeros at $\sin\theta=\pm\lambda/b$. The phase layer redistributes transmitted [power](../../energy.md#power) rather than absorbing it in this idealization.

## Section C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

**[spin normalization in two-dimensional free-electron state counting](../../quantum-ideal-gas-statistics.md#spin-normalization-in-two-dimensional-free-electron-state-counting).** Treat the mobile [electrons](../../physics.md#electron) as independent particles in a constant interior potential, with [parabolic dispersion](../../bloch-s-theorem.md#parabolic-band-dispersion) $\epsilon=\hbar^2k^2/(2m)$, and impose confinement or [periodic boundary conditions](../../differential-equation.md#periodic-boundary-conditions). [electron](../../physics.md#electron)–[electron](../../physics.md#electron) interactions and the detailed periodic ionic potential are neglected, while Fermi statistics are retained. Each spatial state occupies area $(2\pi)^2/A$ in two-dimensional [wavevector](../../elasticity-physics.md#wavevector) space. For [spin degeneracy](../../statistical-physics.md#spin-degeneracy) $g_s$,

$$
\mathcal N(k)=g_s\frac{A\pi k^2}{(2\pi)^2},\qquad
\boxed{g(\epsilon)=\frac{d\mathcal N}{d\epsilon}=\frac{g_sAm}{2\pi\hbar^2}}.
$$

The printed coefficient $Am/(2\pi\hbar^2)$ is the **per-spin [density of states](../../quantum-ideal-gas-statistics.md#density-of-states)**. Unpolarized spin-one-half [electrons](../../physics.md#electron) have $g_s=2$, doubling it. Actual [graphene](../../chemical-substance.md#graphene) near its [Dirac points](../../bloch-s-theorem.md#dirac-point) has approximately linear dispersion, so its energy-dependent [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) is not this parabolic-model result; the plane geometry alone does not establish the free-electron dispersion.[Abstract: massless Dirac charge carriers rather than a finite-mass parabolic band](../../physics-bibliography.md#two-dimensional-gas-of-massless-dirac-fermions-in-graphene-by-konstantin-novoselov-and-others)

**Occupied disk and [Fermi energy](../../quantum-ideal-gas-statistics.md#fermi-energy).** At zero [temperature](../../temperature.md) fill the lowest states up to a disk of radius $k_F$. State counting gives

$$
\boxed{k_F=\sqrt{\frac{4\pi N}{g_sA}},\qquad
\epsilon_F=\frac{2\pi\hbar^2N}{g_sAm}}.
$$

Thus the physical spin-degenerate result is $\epsilon_F=\pi\hbar^2N/(Am)$. If $N$ instead counts one spin species, the per-spin convention gives $2\pi\hbar^2N/(Am)$. Each occupied [wavevector](../../elasticity-physics.md#wavevector) can contain one [electron](../../physics.md#electron) of each allowed spin, never two in the same complete [one-particle state](../../quantum-field-theory.md#one-particle-state).

<a id="section-c/c10/image-original-occupied-wavevector-disk-and-fermi-dirac-occupations-for-a-parabolic-two-dimensional-electron-gas"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2-two-dimensional-fermi-gas.png)

**[Figure 3](#section-c/c10/image-original-occupied-wavevector-disk-and-fermi-dirac-occupations-for-a-parabolic-two-dimensional-electron-gas). Original occupied wavevector disk and Fermi-Dirac occupations for a parabolic two-dimensional electron gas**.

**Occupation probability and [chemical potential of a two-dimensional ideal Fermi gas](../../quantum-ideal-gas-statistics.md#chemical-potential-of-a-two-dimensional-ideal-fermi-gas).** A single [fermion](../../tensor-product-of-quantum-systems.md#fermion) state permits occupation zero or one. In a [grand canonical ensemble](../../statistical-physics.md#grand-canonical-ensemble) their relative weights are $1$ and $e^{-\beta(\epsilon-\mu)}$. Normalizing gives

$$
\boxed{p(\epsilon)=\frac{e^{-\beta(\epsilon-\mu)}}{1+e^{-\beta(\epsilon-\mu)}}
=\frac1{e^{\beta(\epsilon-\mu)}+1}}.
$$

The [chemical potential](../../chemical-potential.md) is fixed by the total particle number. Here the total [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) $D=g_sAm/(2\pi\hbar^2)$ is constant above the band bottom. Integrating the occupation gives $N=Dk_BT\ln(1+e^{\mu/(k_BT)})$, and therefore

$$
\boxed{\mu=\epsilon_F+k_BT\ln\left(1-e^{-\epsilon_F/(k_BT)}\right)
\longrightarrow\epsilon_F\quad(T\to0)}.
$$

The approach is exponentially close in this ideal two-dimensional constant-density-of-states model; a three-dimensional $T^2$ correction should not be inserted here. A narrow interval of width of order $k_BT$ around $\mu$ is thermally smeared.

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/solution">Solution</h4>

↑ **Parent:** [C11](#section-c/c11)

**One [mass](../../classical-mechanics.md#mass) per cell.** If $u_j$ is the displacement from equilibrium, the two springs give $m\ddot u_j=\alpha(u_{j+1}+u_{j-1}-2u_j)$. Substituting $u_j=Ue^{i(qja-\omega t)}$ yields

$$
\boxed{\omega(q)=2\sqrt{\alpha/m}\,|\sin(qa/2)|}.
$$

The [first Brillouin zone](../../bloch-s-theorem.md#first-brillouin-zone) is $-\pi/a\leq q\leq\pi/a$; adding $2\pi/a$ leaves the sampled displacements unchanged. The branch is linear near zero, with [sound speed](../../compressible-flow.md#speed-of-sound) $a\sqrt{\alpha/m}$, and reaches $2\sqrt{\alpha/m}$ at either zone edge.

**Two [masses](../../classical-mechanics.md#mass) per cell.** Take a cell of length $2a$, with light displacement $u_j=Ue^{i(2jaq-\omega t)}$ and heavy displacement $v_j=Ve^{i[(2j+1)aq-\omega t]}$. The coupled equations reduce to

$$
\begin{pmatrix}2\alpha-m\omega^2&-2\alpha\cos qa\\
-2\alpha\cos qa&2\alpha-M\omega^2\end{pmatrix}
\begin{pmatrix}U\\V\end{pmatrix}=0.
$$

A nonzero displacement requires determinant zero:

$$
Mm\omega^4-2\alpha(M+m)\omega^2+4\alpha^2\sin^2qa=0.
$$

Solving this quadratic in $\omega^2$ gives

$$
\boxed{\omega_\pm^2=\frac\alpha{Mm}\left[M+m\pm\sqrt{(M+m)^2-4Mm\sin^2qa}\right]}.
$$

Now the first zone is $|q|\leq\pi/(2a)$. The minus branch is acoustic: as $q\to0$, both sublattices move together and $\omega_-\to0$. Its [sound speed](../../compressible-flow.md#speed-of-sound) is $a\sqrt{2\alpha/(M+m)}$. The plus branch is optical: at $q=0$ the atoms move oppositely with $mU+MV=0$, giving finite [frequency](../../wave.md#frequency) $\sqrt{2\alpha(1/m+1/M)}$. This terminology describes relative motion; optical activity itself also requires coupling to the electromagnetic field.

**[diatomic-chain zone-edge polarizations](../../quantum-ideal-gas-statistics.md#diatomic-chain-zone-edge-polarizations) and dimensionality.** At the edge, $\cos qa=0$, so the heavy and light sublattices decouple: the acoustic edge [frequency](../../wave.md#frequency) is $\sqrt{2\alpha/M}$ and the optical edge [frequency](../../wave.md#frequency) is $\sqrt{2\alpha/m}$. Hence

$$
\boxed{\Delta\omega=\sqrt{2\alpha/m}-\sqrt{2\alpha/M}}.
$$

The acoustic edge mode moves only the heavy sublattice; the optical edge mode only the light one. If $M=m$, the gap closes and the two branches are the zone-folded monatomic branch.

<a id="section-c/c11/image-original-monatomic-and-diatomic-chain-dispersions-zone-edge-gap-and-long-wavelength-displacement-patterns"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2-chain-phonons.png)

**[Figure 4](#section-c/c11/image-original-monatomic-and-diatomic-chain-dispersions-zone-edge-gap-and-long-wavelength-displacement-patterns). Original monatomic and diatomic chain dispersions, zone-edge gap and long-wavelength displacement patterns**.

A three-dimensional crystal with two atoms per primitive cell has **six branches: three acoustic and three optical**. For propagation along a suitable symmetry direction these resolve into one longitudinal and two transverse branches of each type. The [wavevector](../../elasticity-physics.md#wavevector) and [Brillouin zone](../../bloch-s-theorem.md#brillouin-zone) are three-dimensional; anisotropic [force](../../force.md) constants determine the dispersions, and polar crystals can have longitudinal–transverse optical splitting. A universal six-branch curve cannot be specified from [masses](../../classical-mechanics.md#mass) alone.

## Section D

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-d/d12">D12</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d12/solution">Solution</h4>

↑ **Parent:** [D12](#section-d/d12)

The [Debye model](../../quantum-ideal-gas-statistics.md#debye-model) replaces the crystal by a harmonic elastic continuum with acoustic dispersion $\omega=v_sk$. It counts three [polarizations](../../wave.md#polarization-waves) and introduces a cutoff so that the total number of vibrational modes is $3N$, where $N$ is the atom count. Periodic-box counting gives

$$
g(\omega)=\frac{V\omega^2}{2\pi^2}\left(\frac1{v_L^3}+\frac2{v_T^3}\right).
$$

For an isotropic average speed, $3/v_D^3=1/v_L^3+2/v_T^3$. With cutoff [frequency](../../wave.md#frequency) $\omega_D$ fixed by the mode count,

$$
\boxed{g(\omega)=\frac{9N\omega^2}{\omega_D^3}\quad(0<\omega<\omega_D),\qquad
\Theta_D=\frac{\hbar\omega_D}{k_B}}.
$$

This [density of states](../../quantum-ideal-gas-statistics.md#density-of-states) is quadratic because a three-dimensional shell has [volume](../../geometry-and-topology.md#volume) proportional to $k^2dk$ and the acoustic dispersion is linear. The cutoff is a mode-counting device; it is not a claim that every actual branch stays linear to the zone boundary.

Each [phonon](../../quantum-ideal-gas-statistics.md#phonon) mode has mean thermal [energy](../../energy.md) $\hbar\omega/(e^{\beta\hbar\omega}-1)$, using [Bose-Einstein statistics](../../quantum-ideal-gas-statistics.md#bose-einstein-statistics) with zero [phonon](../../quantum-ideal-gas-statistics.md#phonon) [chemical potential](../../chemical-potential.md). The fixed harmonic zero-point contribution has zero [temperature](../../temperature.md) [derivative](../../calculus.md#derivative). With $x=\hbar\omega/(k_BT)$,

$$
U_{\rm th}=9Nk_BT\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^3}{e^x-1}dx,
$$

and differentiating at fixed [volume](../../geometry-and-topology.md#volume) gives

$$
\boxed{C_V=9Nk_B\left(\frac{T}{\Theta_D}\right)^3
\int_0^{\Theta_D/T}\frac{x^4e^x}{(e^x-1)^2}dx}.
$$

For $T\ll\Theta_D$, extend the upper limit to infinity. Expanding $1/(e^x-1)=\sum_{j\geq1}e^{-jx}$ gives $\int_0^\infty x^3/(e^x-1)dx=6\sum j^{-4}=\pi^4/15$. [integration](../../integral.md) by parts makes the heat-capacity [integral](../../integral.md) $4\pi^4/15$, so

$$
\boxed{C_V\simeq\frac{12\pi^4}{5}Nk_B\left(\frac T{\Theta_D}\right)^3}.
$$

Only modes with $\hbar\omega\lesssim k_BT$ are appreciably excited; their number scales as $T^3$, explaining the [power](../../energy.md#power) law physically. At high [temperature](../../temperature.md) every mode contributes $k_B$, giving the Dulong-Petit limit $C_V\to3Nk_B$.

The model assumes the [harmonic approximation](../../lagrangian-mechanics.md#harmonic-approximation), a macroscopic three-dimensional solid and acoustic continuum behaviour for the thermally populated modes. Anisotropic [sound speeds](../../compressible-flow.md#speed-of-sound) change the low-temperature coefficient rather than its cubic [power](../../energy.md#power). Real optical branches and nonlinear acoustic dispersion limit the full-temperature approximation; electronic excitations can add a linear term in a metal, and [anharmonicity](../../wave.md#anharmonicity) produces [thermal expansion](../../thermodynamics.md#thermal-expansion) and distinctions between $C_P$ and $C_V$. At [temperatures](../../temperature.md) below the lowest finite-sample mode, the bulk continuum law also fails. Thus **the $T^3$ result is the low-temperature lattice contribution**, not a universal total [heat capacity](../../heat.md#heat-capacity) for every solid.

<h3 id="section-d/d13">D13</h3>

↑ **Parent:** [Section D](#section-d)

<h4 id="section-d/d13/a">a</h4>

↑ **Parent:** [D13](#section-d/d13)

<h5 id="section-d/d13/a/solution">Solution</h5>

↑ **Parent:** [A](#section-d/d13/a)

For a circular structure, cylindrical symmetry reduces the scalar [Fresnel-Kirchhoff diffraction integral](../../physical-optics.md#fresnel-kirchhoff-diffraction-integral) to concentric annuli. With plane-wave illumination, radius $a$ and distance $z$, the relevant [Fresnel number](../../physical-optics.md#fresnel-number) is $N_F=a^2/(\lambda z)$. Successive [Fresnel half-period zones](../../physical-optics.md#fresnel-half-period-zone) have radii $r_j^2\simeq j\lambda z$: their areas are approximately equal while their phases alternate by $\pi$, causing neighbouring-zone cancellation.

For [Fresnel diffraction by a circular aperture](../../physical-optics.md#fresnel-diffraction-by-a-circular-aperture), the on-axis field follows directly from the radial [integral](../../integral.md),

$$
\frac{U_{\rm ap}}{U_{\rm free}}
=\frac1{i\lambda z}\int_0^a e^{i\pi r^2/(\lambda z)}2\pi r\,dr
=1-e^{i\pi N_F},\qquad
\boxed{I_{\rm ap}/I_{\rm free}=4\sin^2(\pi N_F/2)}.
$$

Odd zone counts reinforce on axis; even counts cancel in this ideal scalar model. An annular opening gives the difference of the corresponding two edge exponentials. A [zone plate](../../physical-optics.md#zone-plate) alternately blocks or phase-shifts zones so that otherwise cancelling contributions reinforce at a focus, with $r_j^2\simeq j\lambda f$ for its principal focal distance.

[Babinet's principle](../../physical-optics.md#babinet-s-principle) gives $U_{\rm disk}=U_{\rm free}-U_{\rm ap}=U_{\rm free}e^{i\pi N_F}$ for [Fresnel diffraction by an opaque disk](../../physical-optics.md#fresnel-diffraction-by-an-opaque-disk). Thus **its ideal on-axis intensity equals the unobstructed intensity**, the [Arago spot](../../physical-optics.md#arago-spot), even within the geometric shadow. This concerns a narrow axial feature, not the whole shadow. Finite source size, imperfect circularity, [bandwidth](../../electrical-engineering.md#bandwidth-signal-processing) and alignment reduce its visibility. When $N_F\ll1$, the circular-aperture far-field pattern becomes the [Airy disk](../../point-spread-function.md#airy-disk) intensity pattern $[2J_1(u)/u]^2$, with $u=ka\sin\theta$ and first minimum near $\theta=1.22\lambda/(2a)$.

<a id="section-d/d13/a/image-original-calculated-circular-fresnel-fabry-perot-and-finite-grating-intensity-patterns-under-their-stated-idealizations"></a>
![](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2-optical-notes.png)

**[Figure 5](#section-d/d13/a/image-original-calculated-circular-fresnel-fabry-perot-and-finite-grating-intensity-patterns-under-their-stated-idealizations). Original calculated circular Fresnel, Fabry–Pérot and finite-grating intensity patterns under their stated idealizations**.

<h4 id="section-d/d13/b">b</h4>

↑ **Parent:** [D13](#section-d/d13)

<h5 id="section-d/d13/b/solution">Solution</h5>

↑ **Parent:** [B](#section-d/d13/b)

Two parallel partially reflecting surfaces in a [Fabry–Pérot interferometer](../../optical-instrument.md#fabry-perot-interferometer) produce a sequence of coherent transmitted beams. For equal lossless mirror intensity [reflectance](../../radiometry.md#reflectance) $\mathcal R$ and round-trip phase $\delta=4\pi nd\cos\theta_t/\lambda$, summing the [geometric series](../../sequence-and-series.md#geometric-series) of amplitudes gives

$$
\frac{E_t}{E_i}=\frac{(1-\mathcal R)e^{i\delta/2}}{1-\mathcal R e^{i\delta}},\qquad
\boxed{\mathcal T=\frac1{1+\mathcal F\sin^2(\delta/2)},\quad
\mathcal F=\frac{4\mathcal R}{(1-\mathcal R)^2}}.
$$

[resonances](../../dynamical-systems.md#resonance) have $2nd\cos\theta_t=m\lambda$ and unit peak transmission in this symmetric lossless model. Varying angle gives concentric equal-inclination rings; changing spacing scans the [resonance](../../dynamical-systems.md#resonance) [wavelengths](../../wave-equation.md#wavelength).

At [normal incidence](../../optics.md#normal-incidence) with negligible dispersion, the [free spectral range](../../physical-optics.md#free-spectral-range) is $\Delta\nu_{\rm FSR}=c/(2nd)$. For high [reflectance](../../radiometry.md#reflectance), the peak full width gives [finesse](../../optical-instrument.md#finesse) and resolving [power](../../energy.md#power)

$$
\boxed{\mathscr F\simeq\frac{\pi\sqrt{\mathcal R}}{1-\mathcal R},\qquad
\frac\nu{\delta\nu}=m\mathscr F}.
$$

The coefficient $\mathcal F$ in the transmission formula and the [finesse](../../optical-instrument.md#finesse) $\mathscr F$ are different quantities. Multiple round trips sharpen a peak, allowing high-resolution spectroscopy, [frequency](../../wave.md#frequency) selection and cavity measurements. Absorption, mirror mismatch, finite angular spread, imperfect parallelism and surface errors reduce usable transmission or [finesse](../../optical-instrument.md#finesse). Adjacent orders can overlap in a broadband measurement, requiring order selection or prior spectral information.

<h4 id="section-d/d13/c">c</h4>

↑ **Parent:** [D13](#section-d/d13)

<h5 id="section-d/d13/c/solution">Solution</h5>

↑ **Parent:** [C](#section-d/d13/c)

For $N$ uniformly illuminated identical slits of a [diffraction grating](../../physical-optics.md#diffraction-grating), with width $b$ and period $d$, the far-field amplitude is a single-slit transform times a finite phasor sum. At [normal incidence](../../optics.md#normal-incidence), write $\beta=\pi d\sin\theta/\lambda$. Then

$$
\boxed{I(\theta)=I_{1,0}\left[\frac{\sin(\pi b\sin\theta/\lambda)}{\pi b\sin\theta/\lambda}\right]^2
\left(\frac{\sin N\beta}{\sin\beta}\right)^2}.
$$

Principal maxima obey $d\sin\theta=m\lambda$ and have $N^2$ times the single-slit intensity at that angle. Nearby first minima are separated from a principal maximum by $\delta\theta\simeq\lambda/(Nd\cos\theta_m)$, so more illuminated slits sharpen each order. The broad single-slit envelope suppresses high angles; an order is missing if its principal maximum coincides with an envelope zero.

Differentiating the [grating equation](../../physical-optics.md#grating-equation) gives angular dispersion $d\theta/d\lambda=m/(d\cos\theta_m)$. Comparing the separation of nearby [wavelengths](../../wave-equation.md#wavelength) with the first-minimum width yields the Rayleigh resolving [power](../../energy.md#power)

$$
\boxed{\lambda/\delta\lambda=|m|N}.
$$

Only propagating orders with $|m\lambda|\leq d$ exist. Different spectral orders can overlap, and finite source-slit width, limited coherence, aberrations and grating errors worsen ideal resolution. A [spectrometer](../../optical-instrument.md#spectrometer) therefore collimates light from an entrance slit and focuses each diffracted direction onto a detector; the slit image width and illuminated grating width must both support the desired spectral separation.

## ↑ Ancestors (11)

1. [2013](../2013.md)
2. [Past exam of the physics A course of the University of Cambridge](../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge.md)
3. [Physics A course of the University of Cambridge](../../university-of-cambridge.md#physics-a-course-of-the-university-of-cambridge)
4. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
