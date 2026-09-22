# Debye T-cubed test

↑ **Parent:** [Heat capacity](heat-capacity.md)

The [Debye T-cubed test](debye-t-cubed-test.md) asks whether a bulk three-dimensional [crystal](crystal.md)'s lattice [molar heat capacity](molar-heat-capacity.md) approaches a cubic law well below its [Debye temperature](debye-temperature.md) $T_D$. It tests the low-[frequency](frequency.md) [acoustic phonon branches](acoustic-phonon-branch.md) in the [Debye model](debye-model.md), rather than asserting that every contribution to a real sample's [heat capacity](heat-capacity.md) is cubic. [Peter Debye](peter-debye.md)'s continuum description makes a striking connection: a thermal measurement can reveal the low-[frequency](frequency.md) vibrational [density of states](density-of-states.md) without resolving individual vibrations.[Statistical Physics by David Tong; §3.3.1, The Debye Model: low-temperature heat capacity](statistical-physics-by-david-tong/3-quantum-gases.md)

For a monatomic bulk model, the [Debye model](debye-model.md) has vibrational [density of states](density-of-states.md) $g(\omega)=9N\omega^2/\omega_D^3$ up to the [Debye frequency](debye-frequency.md) $\omega_D$, containing $3N$ [normal modes](normal-mode.md). With $x=\hbar\omega/(k_BT)$, the thermal vibrational [internal energy](internal-energy-split.md) becomes

$$
U_{\rm lattice}=9Nk_BT\left(\frac{T}{T_D}\right)^3
\int_0^{T_D/T}\frac{x^3}{e^x-1}\,dx.
$$

The reduced [Planck constant](planck-constant.md) is $\hbar$, the [Boltzmann constant](boltzmann-constant.md) is $k_B$, and $N$ counts [chemical atoms](atom-physics.md). For $T\ll T_D$, replace the upper limit by infinity. The [integral](integral-split.md) is $\pi^4/15$, as in the [Stefan–Boltzmann law](stefan-boltzmann-law.md) derivation. Differentiating at fixed [volume](volume-thermodynamics.md) gives, per [mole](mole-unit.md) of [chemical atoms](atom-physics.md),

$$
C_{V,\mathrm m}^{\rm lattice}\simeq\beta T^3,
\qquad \beta=\frac{12\pi^4R}{5T_D^3},
\qquad [\beta]=\mathrm{J\,mol^{-1}\,K^{-4}},
$$

where $R$ is the [molar gas constant](molar-gas-constant.md). The cubic exponent comes from three-dimensional [acoustic phonon branches](acoustic-phonon-branch.md) with linear low-[wavevector](wavevector.md) [dispersion relations](dispersion-relation-split.md). The coefficient encodes their propagation speeds. Formula-unit normalization in a compound requires its number of [chemical atoms](atom-physics.md) per formula unit; do not silently substitute moles of formula units for moles of [chemical atoms](atom-physics.md).

For a simple [metal](metal.md) in its nonsuperconducting state, well below both [Debye temperature](debye-temperature.md) and [electron Fermi temperature](electron-fermi-temperature.md), include [electronic heat capacity](electronic-heat-capacity.md):

$$
C_{p,\mathrm m}(T)\simeq\gamma T+\beta T^3,
\qquad \frac{C_{p,\mathrm m}}{T}\simeq\gamma+\beta T^2.
$$

This approximation also requires negligible [difference between constant-pressure and constant-volume heat capacities](difference-between-constant-pressure-and-constant-volume-heat-capacities.md) at the measurement precision, and no significant magnetic, nuclear or [Schottky anomaly](schottky-anomaly.md) contribution in the fit interval. Thus [linear regression](linear-regression-split.md) of $C_{p,\mathrm m}/T$ against $T^2$ separates an electronic intercept from a lattice slope. For an insulating [crystal](crystal.md) with no relevant low-[energy](energy-split.md) magnetic excitations, the electronic term can instead be negligible; a [superconductivity](superconductivity-split.md) transition changes the electronic response.[Statistical Physics by David Tong; §§3.3.1 and 3.6.3: phonon and electronic low-temperature contributions](statistical-physics-by-david-tong/3-quantum-gases.md)

After subtracting [calorimeter addenda](calorimeter-addenda.md), Brando's second [gold](gold.md) sample, $72.6\,\mathrm{mg}$, gave a linear $C_{p,\mathrm m}/T$ versus $T^2$ plot in the nonsuperconducting state. The reported electronic intercept was $7.0\times10^{-4}\,\mathrm{J\,mol^{-1}\,K^{-2}}$; deviations from reference [heat capacities](heat-capacity.md) were below $2\%$.[§IV.B and Fig. 9: separate validation sample, molar electronic intercept and reference-comparison inset; plotted temperatures extend to about 3 K](development-of-a-relaxation-calorimeter-for-temperatures-between-0-05-and-4-k-by-manuel-brando.md) This supports the combined linear-plus-cubic description over the plotted interval. Because the platform subtraction used reference [gold](gold.md), it is also an instrument validation with a shared material standard, rather than a wholly independent determination of the [Debye model](debye-model.md) from an uncalibrated instrument.

<a id="image-the-debye-t-cubed-test-in-a-normal-metal-lattice-slope-and-electronic-intercept"></a>
![](debye-normal-metal-intercept-test.png)

**[Figure 13](#image-the-debye-t-cubed-test-in-a-normal-metal-lattice-slope-and-electronic-intercept). The Debye T-cubed test in a normal metal: lattice slope and electronic intercept**. Original constructed model with $\gamma=7.00\times10^{-4}\,\mathrm{J\,mol^{-1}\,K^{-2}}$ and $\beta=4.00\times10^{-4}\,\mathrm{J\,mol^{-1}\,K^{-4}}$. It represents a stipulated monatomic normal [metal](metal.md), not digitized [gold](gold.md) measurements. Solid curves apply only over the chosen $1$–$3\,\mathrm K$ fit interval, with negligible other terms and $C_p-C_V$. Dashed portions illustrate extrapolation; error bars are assigned one-[standard deviation](standard-deviation.md) uncertainties, not scatter measured in the experiment.

For a worked original inference, stipulate values of $y=C_{p,\mathrm m}/T$ equal to $(0.001100,0.002300,0.004300)\,\mathrm{J\,mol^{-1}\,K^{-2}}$ at $T=(1,2,3)\,\mathrm K$. Assign independent $u(y)=0.000020\,\mathrm{J\,mol^{-1}\,K^{-2}}$ and negligible [temperature](temperature-split.md) error. Equal-weight [linear regression](linear-regression-split.md) on $x=T^2$ gives

$$
\gamma=(7.00\pm0.20)\times10^{-4}\,\mathrm{J\,mol^{-1}\,K^{-2}},
\qquad \beta=(4.000\pm0.035)\times10^{-4}\,\mathrm{J\,mol^{-1}\,K^{-4}}.
$$

The points sit exactly on the stipulated line; these [standard uncertainties](standard-uncertainty.md) come from the assigned input precision, not an estimate from zero residual scatter. With $R=8.314462618\,\mathrm{J\,mol^{-1}\,K^{-1}}$, inversion gives

$$
T_D=\left(\frac{12\pi^4R}{5\beta}\right)^{1/3}=169.38\,\mathrm K,
\qquad \frac{u(T_D)}{T_D}=\frac{u(\beta)}{3\beta},
\qquad T_D=(169.4\pm0.5)\,\mathrm K.
$$

At $2\,\mathrm K$, the electronic and lattice [molar heat capacities](molar-heat-capacity.md) are respectively $0.0014$ and $0.0032\,\mathrm{J\,mol^{-1}\,K^{-1}}$. Their equality occurs at $\sqrt{\gamma/\beta}=1.323\,\mathrm K$: even in this clean model, the total [heat capacity](heat-capacity.md) approaches a linear, rather than cubic, law as $T$ tends to zero in the normal state.

A straight line over a narrow interval is a useful diagnostic, not a universal proof. Inspect residuals and repeat the fit over several upper and lower [temperature](temperature-split.md) cutoffs; curvature can signal higher lattice terms, an unremoved [Schottky anomaly](schottky-anomaly.md), or a faulty [calorimeter addenda](calorimeter-addenda.md) subtraction. Correlated [thermometer calibration](thermometer-calibration.md) and sample-amount errors affect both axes and can dominate the illustrative [linear regression](linear-regression-split.md) uncertainty. Low-dimensional samples, additional low-[energy](energy-split.md) excitations and proximity to a [phase transition](phase-transition.md) need other models. The test is valuable precisely because its failures can reveal physics beyond the bulk acoustic approximation.

## ↑ Ancestors (7)

1. [Heat capacity](heat-capacity.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Debye T-cubed test](debye-t-cubed-test.md)
- [Electronic heat capacity](electronic-heat-capacity.md)
- [Low-temperature heat capacity measurement](low-temperature-heat-capacity-measurement.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-2/section-d/d13/a/solution.md)
