# Equipartition theorem

↑ **Parent:** [Canonical ensemble](canonical-ensemble.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equipartition_theorem)

The [equipartition theorem](equipartition-theorem.md) says that each independent quadratic term in a [Hamiltonian](hamiltonian.md) described by [classical mechanics](classical-mechanics-split.md) has mean [energy](energy.md) $k_BT/2$ in a [canonical ensemble](canonical-ensemble.md). Here $k_B$ is the [Boltzmann constant](boltzmann-constant.md) and $T>0$ the absolute [temperature](temperature.md). Count terms in the [energy](energy.md), rather than vaguely counting everything that can move: one [harmonic oscillator](simple-harmonic-motion.md) has one position [degree of freedom](degree-of-freedom.md) but TWO quadratic terms, one in [momentum](momentum.md) and one in [displacement](displacement.md).

A precise sufficient setting is $H(y,\xi)=ay^2/2+H_0(\xi)$ with $a>0$, where $y$ is one of the [canonical variables](canonical-variables.md), $\xi$ denotes all remaining variables, and the [phase space](phase-space.md) integration measure factors as $dy\,d\xi$. The range of $y$ is the whole [real line](real-line.md), independently of $\xi$; there is no [constraint](constraint-mechanics.md) coupling its allowed values to other variables. The [partition function](canonical-partition-function.md) must be finite, and the relevant [expected values](expected-value.md) must exist. The [Boltzmann factor](boltzmann-factor.md) then gives

$$
\beta=\frac{1}{k_BT},\qquad
\rho_y(y)=\sqrt{\frac{\beta a}{2\pi}}e^{-\beta ay^2/2},\qquad
\left\langle\frac{ay^2}{2}\right\rangle=\frac{k_BT}{2}.
$$

The [probability density function](probability-density-function.md) $\rho_y$ is a [normal distribution](normal-distribution.md) with [variance](variance-split.md) $k_BT/a$. A larger coefficient narrows the fluctuations enough to cancel its greater [energy](energy.md) cost. This is why the mean contribution is independent of [mass](mass.md) or [spring constant](spring-constant.md).[equations 7.124–7.135](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/equipartition-theorem.md)

For a proof outline, the one-variable [Gaussian integral](gaussian-integral.md) is $Z_y=\int_{-\infty}^{\infty}e^{-\beta ay^2/2}\,dy=\sqrt{2\pi/(\beta a)}$, so $-\partial_\beta\ln Z_y=1/(2\beta)$. More generally, [integration by parts](integration-by-parts.md) in a canonical variable gives $\langle y\,\partial_yH\rangle=k_BT$ when its boundary term $[y e^{-\beta H}]$ vanishes and the integrals converge. For $ay^2/2$ this is twice its mean [energy](energy.md). At a finite hard boundary the boundary term need not vanish; [hard-wall correction to harmonic equipartition](hard-wall-correction-to-harmonic-equipartition.md) illustrates the resulting departure. A [constraint](constraint-mechanics.md), a nonquadratic [potential energy](potential-energy.md), or a noncanonical integration measure therefore requires its own calculation. The theorem is an [ensemble average](expected-value.md), not equality of instantaneous [energies](energy.md), and applying it to a recorded trajectory requires equilibration and sufficient sampling.

For a classical one-dimensional [harmonic oscillator](simple-harmonic-motion.md), with positive [mass](mass.md) $m$ and [spring constant](spring-constant.md) $k$,

$$
H=\frac{p^2}{2m}+\frac{kx^2}{2},\qquad
\frac{\langle p^2\rangle}{2m}=\frac{k\langle x^2\rangle}{2}=\frac{k_BT}{2},\qquad
\langle H\rangle=k_BT.
$$

The origin is the [equilibrium](equilibrium-point-of-a-dynamical-system.md) position. Its [heat capacity](heat-capacity.md) is $k_B$ at fixed $m,k$, not $k_B/2$. Although the two mean [energies](energy.md) agree, their measured amplitudes do not: $\langle p^2\rangle=mk_BT$ and $\langle x^2\rangle=k_BT/k$. In a [harmonic optical trap](harmonic-optical-trap.md), the position measurement observes the [potential energy](potential-energy.md) contribution; it does not measure both contributions by observing $x$ alone.[equations 7.136–7.139](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/harmonic-oscillators.md)

For $N$ particles in a three-dimensional classical [monatomic gas](monatomic-gas.md), neglect interactions and thermally accessible internal excitations. Its three translational [momentum](momentum.md) terms give [internal energy](internal-energy.md) $U=3Nk_BT/2$, [heat capacity at constant volume](heat-capacity-at-constant-volume.md) $C_V=3Nk_B/2$, and [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) $C_p=C_V+Nk_B=5Nk_B/2$. Per mole, replace $Nk_B$ by the [molar gas constant](molar-gas-constant.md) $R$. For example, using stipulated $R=8.314\,\mathrm{J\,mol^{-1}\,K^{-1}}$, the [molar heat capacity](molar-heat-capacity.md) at fixed [volume](volume-thermodynamics.md) is $12.471\,\mathrm{J\,mol^{-1}\,K^{-1}}$. These results assume a dilute, nonrelativistic [ideal gas](ideal-gas.md) with classical translational statistics, rather than a [quantum degeneracy](degenerate-energy-levels.md) regime.

For an [ideal gas](ideal-gas.md) of diatomic [molecules](molecule.md), modeled as two [chemical atoms](atom-physics.md) with a bond, there are three translational quadratic terms, two accessible [rotational kinetic energy](rotational-kinetic-energy.md) terms for changes of bond orientation, and one bond-stretching [harmonic oscillator](simple-harmonic-motion.md) with two quadratic terms. Rotation about the bond axis is not an additional active mode in this linear-molecule model. The three familiar limits of [heat capacity at constant volume](heat-capacity-at-constant-volume.md) are

$$
\frac{C_V}{Nk_B}\simeq
\begin{cases}
3/2,&\text{rotations and vibrations frozen},\\
5/2,&\text{rotations active, vibrations frozen},\\
7/2,&\text{rotations and vibrations classical}.
\end{cases}
$$

Corresponding [molar heat capacities](molar-heat-capacity.md) are $3R/2$, $5R/2$ and $7R/2$. Counting the stretching [harmonic oscillator](simple-harmonic-motion.md) only once as $k_BT/2$ would give the wrong last value.[§§2.2.1](statistical-physics-by-david-tong/2-classical-gases.md)

The frozen regimes require [quantum mechanics](quantum-mechanics-split.md). In the simple molecular rotation model, $E_j=k_B\theta_r j(j+1)$ with [state degeneracy](state-degeneracy.md) $2j+1$, $\theta_r=\hbar^2/(2Ik_B)$, and [moment of inertia](moment-of-inertia.md) $I$. For the bond-stretching [quantum harmonic oscillator](quantum-harmonic-oscillator.md), $\theta_v=\hbar\omega/k_B$ with [angular frequency](angular-frequency.md) $\omega$ and $\hbar=h/(2\pi)$ from the [Planck constant](planck-constant.md). When $\theta_r\ll\theta_v$, the three limits above correspond to $T\ll\theta_r$, $\theta_r\ll T\ll\theta_v$, and $T\gg\theta_v$, provided translational motion remains classical. They are smooth crossovers, not abrupt switches. Real [molecules](molecule.md) can have different allowed rotational populations; at high [temperature](temperature.md), [thermal dissociation](thermal-dissociation.md), internal excitations and nonharmonic bond motion can invalidate the fixed-molecule model before its last limit is reached.[§3.4](statistical-physics-by-david-tong/3-quantum-gases.md)

For a [quantum harmonic oscillator](quantum-harmonic-oscillator.md) with fixed $\omega$, put $z=\theta_v/T$. Its exact mean [energy](energy.md) and [heat capacity](heat-capacity.md) are

$$
\langle H\rangle=\frac{\hbar\omega}{2}+\frac{\hbar\omega}{e^z-1},\qquad
\frac{C_{\rm osc}}{k_B}=\frac{z^2e^{-z}}{(1-e^{-z})^2}.
$$

At $T\gg\theta_v$, the mean [energy](energy.md) approaches $k_BT$ and $C_{\rm osc}$ approaches $k_B$. At $T\ll\theta_v$, thermal excitation is exponentially suppressed and $C_{\rm osc}$ tends to zero, although the [zero-point energy](zero-point-energy.md) $\hbar\omega/2$ survives. Frozen thus means little thermal response, not zero motion or zero [energy](energy.md).[equations 7.140–7.155](thermodynamics-and-statistical-mechanics-by-richard-fitzpatrick/harmonic-oscillators.md)

<a id="image-model-heat-capacities-a-quantum-harmonic-oscillator-and-a-diatomic-ideal-gas"></a>
![](equipartition-quantum-heat-capacity.png)

**[Figure 21](#image-model-heat-capacities-a-quantum-harmonic-oscillator-and-a-diatomic-ideal-gas). Model heat capacities: a quantum harmonic oscillator and a diatomic ideal gas**. Original computed equilibrium curves, not measured gas data. Left: $C_{\rm osc}/k_B$ approaches its classical value 1 as $T/\theta_v$ grows. Right: $C_V/(Nk_B)=3/2+C_{\rm rot}/k_B+C_{\rm osc}/k_B$ for stipulated $\theta_v/\theta_r=100$. The rotational [partition function](canonical-partition-function.md) is $\sum_{j=0}^{\infty}(2j+1)e^{-\theta_r j(j+1)/T}$ with every nonnegative integer $j$ allowed; $C_{\rm rot}/k_B$ is the [variance](variance-split.md) of $j(j+1)$ divided by $(T/\theta_r)^2$. No molecular nuclear-spin restrictions, [thermal dissociation](thermal-dissociation.md) or nonharmonic effects are modeled. Horizontal guides mark the three limiting values, not exact plateaus at finite [temperature](temperature.md).

A motivating measurement is [thermal calibration of an optical trap](thermal-calibration-of-an-optical-trap.md). A focused [laser](laser.md) through a microscope objective confines a bead in water; imaging or a quadrant photodetector records a position [time series](time-series-split.md). Gieseler and colleagues describe a polystyrene bead of radius $1.03\,\mathrm{\mu m}$ at $293.15\,\mathrm K$, a $1064\,\mathrm{nm}$ trapping [laser](laser.md), and photodetector acquisition at $10^5\,\mathrm{Hz}$. Their recorded bead continues undergoing [Brownian motion](brownian-motion-split.md); higher trapping power produces a narrower equilibrium position distribution. Infer the centered [variance](variance-split.md), not a squared distance from an arbitrary camera origin:

$$
\sigma_x^2=\left\langle(x-\langle x\rangle)^2\right\rangle,\qquad
k=\frac{k_BT}{\sigma_x^2}.
$$

The [normal distribution](normal-distribution.md) position histogram and agreement with dynamical calibration methods support the local [harmonic optical trap](harmonic-optical-trap.md) interpretation. For a stipulated example, $T=300\,\mathrm K$ and $\sigma_x=20\,\mathrm{nm}$ imply $k\simeq1.04\times10^{-5}\,\mathrm{N/m}=0.0104\,\mathrm{pN/nm}$. This calculated scale is not an experimental reading.[§§2.1–2.2, 3.3; Tables 1–3](optical-tweezers-a-comprehensive-tutorial-from-calibration-to-applications-by-jan-gieseler.md)

Position calibration is essential: if detector output $v$ has conversion $x=s(v-v_0)$, its physical [variance](variance-split.md) is $s^2\operatorname{Var}(v)$. An unknown scale $s$ cannot be determined together with $k$ from that one [variance](variance-split.md). A complementary calibration demonstrated by Tolić-Nørrelykke and colleagues combines the [power spectrum](power-spectrum.md) of thermal motion with the bead response to known sinusoidal motion of a translation stage. The driven response supplies an additional length scale, and their method does not require bead size, liquid [dynamic viscosity](dynamic-viscosity.md) or wall distance as inputs. It still uses a thermal dynamical model; agreement between methods is a consistency check, not a theory-free proof of [equipartition theorem](equipartition-theorem.md).[abstract](calibration-of-optical-tweezers-with-positional-detection-in-the-back-focal-plane-by-simon-f-tolic-norrelykke-and-others.md)

The readout itself can hide fluctuations. Wong and Halvorsen used a $1064\,\mathrm{nm}$ [optical trap](optical-tweezers.md) and adjustable-exposure CCD imaging of a bead in water. They varied exposure and trapping power, held the bead away from the nearest wall, adjusted illumination to maintain comparable images, and measured tracking noise using a stuck bead. The measured [variance](variance-split.md) fell as exposure increased; corrected results agreed with their time-averaging model. For a stationary overdamped [harmonic optical trap](harmonic-optical-trap.md), with [optical trap relaxation time](optical-trap-relaxation-time.md) $\tau$, an exposure of length $W$ measures $\bar x_W=W^{-1}\int_0^W x(t)\,dt$. Its ideal noise-free [variance](variance-split.md) is

$$
\operatorname{Var}(\bar x_W)=\frac{k_BT}{k}S(\alpha),\qquad
\alpha=\frac{W}{\tau},\qquad
S(\alpha)=\frac{2(\alpha-1+e^{-\alpha})}{\alpha^2}.
$$

For $\alpha>0$, $S(\alpha)<1$: using the blurred [variance](variance-split.md) in the uncorrected formula overestimates $k$ by $1/S(\alpha)$. At $W=\tau$, the calculated factor is $e/2\simeq1.36$. Additive tracking noise instead raises the measured [variance](variance-split.md) and biases the inferred $k$ downward if left uncorrected.[equations 15](the-effect-of-integration-time-on-fluctuation-measurements-calibrating-an-optical-trap-in-the-presence-of-motion-blur-by-wesley-p-wong-and-others.md)

<a id="image-equal-mean-quadratic-energies-with-unequal-fluctuations-and-exposure-biased-readout"></a>
![](equipartition-phase-space-readout.png)

**[Figure 22](#image-equal-mean-quadratic-energies-with-unequal-fluctuations-and-exposure-biased-readout). Equal mean quadratic energies with unequal fluctuations, and exposure-biased readout**. Original analytic models, not bead trajectories or measured curves. Left: equal-[energy](energy.md) contours $H/(k_BT)=1/2,2$ in scaled [phase space](phase-space.md), with $Q=x/\sqrt{k_BT/k_0}$, $P=p/\sqrt{mk_BT}$ and $H/(k_BT)=(P^2+\kappa Q^2)/2$, for $\kappa=k/k_0=1,4$. Increasing stiffness narrows position fluctuations but leaves both mean quadratic contributions equal to $k_BT/2$. Right: the exact noise-free exposure reduction $S(W/\tau)$; at $W/\tau=1$, $S=2/e$ and naive inferred stiffness is $e/2$ times true stiffness. The exposure calculation assumes stationary overdamped harmonic [Brownian motion](brownian-motion-split.md) and uniform averaging.

Useful controls are to record over many [optical trap relaxation times](optical-trap-relaxation-time.md), compare blocks for drift, calibrate the position scale, measure fixed-bead noise, vary exposure, and check the position histogram for departures from a [normal distribution](normal-distribution.md). A sparse sequence of accurate instantaneous positions can estimate an equilibrium [variance](variance-split.md); a long exposure averages away motion even if many frames are collected. Flow, appreciable [laser](laser.md) heating, escape from the harmonic region or nonconservative [forces](force.md) can break the assumed [thermal equilibrium](thermal-equilibrium.md). Inferring $k$ by imposing [equipartition theorem](equipartition-theorem.md) is a calibration, whereas testing the relation requires an independently established stiffness and position scale. The beautiful practical connection is that microscopic randomness can set a [force](force.md) scale: once calibrated, a small constant applied [force](force.md) displaces the mean by $f/k$. The same quadratic-term counting predicts macroscopic [heat capacity](heat-capacity.md) and makes microscopic fluctuations useful measurements.

## ↑ Ancestors (5)

1. [Canonical ensemble](canonical-ensemble.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Dulong-Petit law](dulong-petit-law.md)
- [Equipartition theorem](equipartition-theorem.md)
- [Fixed-area capillary spectrum of a circular boundary](fixed-area-capillary-spectrum-of-a-circular-boundary.md)
- [Fixed-volume capillary spectrum of a cylindrical membrane](fixed-volume-capillary-spectrum-of-a-cylindrical-membrane.md)
- [Heat capacity](heat-capacity.md)
- [Heat capacity ratio](heat-capacity-ratio.md)
- [High-force worm-like chain elasticity](high-force-worm-like-chain-elasticity.md)
- [Ideal gas pressure from wall collisions](ideal-gas-pressure-from-wall-collisions.md)
- [Internal energy](internal-energy.md)
- [Maxwell speed distribution](maxwell-speed-distribution.md)
- [Monatomic gas](monatomic-gas.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-71/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-73/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/34d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-74/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-66/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-71/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-75/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-355/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/36a/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/36a/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/35a/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-355/2/solution.md)
- [Rigid-motion-projected thermal covariance of a free filament](rigid-motion-projected-thermal-covariance-of-a-free-filament.md)
- [Spatially varying tension in filament bending](spatially-varying-tension-in-filament-bending.md)
- [Temperature](temperature.md)
- [Thermal calibration of an optical trap](thermal-calibration-of-an-optical-trap.md)
- [Thermal covariance of an elastic filament](thermal-covariance-of-an-elastic-filament.md)
- [Torsion constant](torsion-constant.md)
- [Vector noise normalization in inertial Langevin dynamics](vector-noise-normalization-in-inertial-langevin-dynamics.md)
- [Zero-energy filament mode](zero-energy-filament-mode.md)
