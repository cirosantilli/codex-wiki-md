# Thermionic emission

↑ **Parent:** [Electron](physics.md#electron)

Release of [electrons](physics.md#electron) from a heated material; one source of [electrons](physics.md#electron) in an [X-ray tube](electromagnetic-radiation.md#x-ray-tube).

Heating a [metal](chemical-substance.md#metal) gives some [electrons](physics.md#electron) enough [energy](energy.md) to escape its surface. A heated [diode cathode](electrical-circuit.md#diode-cathode) can therefore supply an [electric current](electric-charge.md#electric-current) across a [vacuum](physics.md#vacuum) gap to a collecting [diode anode](electrical-circuit.md#diode-anode). This makes [temperature](temperature.md) a control for the supply of [electrons](physics.md#electron). Conversely, measuring that supply at several [temperatures](temperature.md) lets us estimate the surface [work function](quantum-mechanics.md#work-function): the [energy](energy.md) barrier measured from the [Fermi level](quantum-ideal-gas-statistics.md#fermi-level) to the nearby [vacuum](physics.md#vacuum) level. A [Richardson plot](#richardson-plot) turns the strong [exponential function](calculus.md#exponential-function) dependence into a slope.

Three questions must be kept separate: how many [electrons](physics.md#electron) cross the surface, how many traverse the gap, and how many the collecting [diode anode](electrical-circuit.md#diode-anode) records. The [Richardson-Dushman law](#richardson-dushman-law) answers the first under specified surface assumptions. [Space charge](electric-charge.md#space-charge) can obstruct the second, while incomplete collection can alter the third.

**Table of contents**

- [Richardson-Dushman law](#richardson-dushman-law)
  - [Thermionic Richardson constant](#thermionic-richardson-constant)
  - [Richardson plot](#richardson-plot)
  - [Thermionic tail-flux derivation](#thermionic-tail-flux-derivation)
- [Emission-limited thermionic current](#emission-limited-thermionic-current)
- [Space-charge-limited thermionic current](#space-charge-limited-thermionic-current)
- [Richardson hot-wire emission experiment](#richardson-hot-wire-emission-experiment)

## Richardson-Dushman law

↑ **Parent:** [Thermionic emission](thermionic-emission.md)

The [Richardson-Dushman law](#richardson-dushman-law) models the magnitude of emitted [electric current density](electric-charge.md#current-density) as

$$
J=A T^2\exp\!\left(-\frac{W}{k_BT}\right).
$$

Here $T$ is absolute [thermodynamic temperature](second-law-of-thermodynamics.md#thermodynamic-temperature), $W$ is the [work function](quantum-mechanics.md#work-function), $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant), and $A$ is the [Thermionic Richardson constant](#thermionic-richardson-constant). The signed [electric current density](electric-charge.md#current-density) points opposite to the outgoing [electron](physics.md#electron) motion; $J$ here is positive. For uniform emission over area $S$, the emitted [electric current](electric-charge.md#electric-current) magnitude is $I=SJ$.

The [Richardson-Dushman law](#richardson-dushman-law) assumes an emitter close to [thermal equilibrium](thermal-equilibrium.md), a surface with a well-defined and approximately constant [work function](quantum-mechanics.md#work-function) over the fitted [temperature](temperature.md) range, and predominantly thermal escape over the barrier. Interpreting a measured collector [electric current](electric-charge.md#electric-current) with this law additionally requires an [emission-limited thermionic current](#emission-limited-thermionic-current), known emitting area, and negligible return emission from the collector. Strong [electric fields](electric-field.md) can lower the surface barrier or enable [quantum tunnelling](quantum-mechanics.md#quantum-tunnelling); then this zero-field expression is insufficient.

For a deliberately chosen teaching model, take $W=2.0\,\mathrm{eV}$ and $A=120\,\mathrm{A\,cm^{-2}\,K^{-2}}$, expressing the barrier in [electronvolts](electronegativity.md#electronvolt). These are illustrative parameters, not measured properties of a named material. Using $k_B=8.617333262\times10^{-5}\,\mathrm{eV\,K^{-1}}$, at $1000\,\mathrm K$ the [Boltzmann factor](canonical-ensemble.md#boltzmann-factor) is about $8.33\times10^{-11}$, yet

$$
J(1000\,\mathrm K)\simeq0.00999\,\mathrm{A\,cm^{-2}},
\qquad
J(1200\,\mathrm K)\simeq0.6885\,\mathrm{A\,cm^{-2}}.
$$

A 20 percent increase in [temperature](temperature.md) raises the predicted [electric current density](electric-charge.md#current-density) by about 69 times. For a chosen emitting area $S=0.010\,\mathrm{cm^2}$, these correspond to approximately $0.100\,\mathrm{mA}$ and $6.89\,\mathrm{mA}$ if collection is complete. The small escaping fraction is replenished by the external [electrical circuit](electrical-circuit.md).

The sensitivity is especially clear from the [logarithmic derivative](analytic-number-theory.md#logarithmic-derivative) at fixed $A,W$:

$$
\frac{d\ln J}{dT}=\frac{2}{T}+\frac{W}{k_BT^2}.
$$

In the chosen model at $1000\,\mathrm K$, a $1\,\mathrm K$ rise changes $J$ by about 2.5 percent to first order. Accurate [temperature](temperature.md) measurement matters even when [electric current](electric-charge.md#electric-current) measurement is easy.

### Thermionic Richardson constant

↑ **Parent:** [Richardson-Dushman law](#richardson-dushman-law)

The coefficient $A$ has dimensions of [electric current density](electric-charge.md#current-density) divided by squared [temperature](temperature.md). For ideal [nonrelativistic particles](special-relativity.md#nonrelativistic-particle) with the free [electron mass](physics.md#electron-mass), two [spin](angular-momentum-operator.md#spin) states, a planar uniform surface, and unit escape transmission, the [thermionic tail-flux derivation](#thermionic-tail-flux-derivation) gives

$$
A_0=\frac{4\pi m_e e k_B^2}{h^3}
\simeq1.202\times10^6\,\mathrm{A\,m^{-2}\,K^{-2}}
=120.2\,\mathrm{A\,cm^{-2}\,K^{-2}},
$$

where $e$ is the positive [elementary charge](electric-charge.md#elementary-charge) and $h$ is the [Planck constant](quantum-mechanics.md#planck-constant). The two area units differ by a factor of $10^4$. A fitted $A$ need not equal $A_0$: reflection at the surface, the [electronic band structure](bloch-s-theorem.md#electronic-band-structure), and uncertain emitting area affect the inferred coefficient. A constant escape transmission $\tau$ would give $A=\tau A_0$ in this simple model; an [energy](energy.md)-dependent transmission generally requires an integral instead.

The name joins [Owen Willans Richardson](physicist.md#owen-willans-richardson) with [Saul Dushman](chemistry.md#saul-dushman). Dushman's 1923 paper develops a thermodynamic treatment of [electron](physics.md#electron) emission analogous to [evaporation](critical-phenomenon.md#evaporation) and evaluates the prefactor using quantum ideas.[Abstract, general equation and theoretical evaluation of A](physics-bibliography.md#electron-emission-from-metals-as-a-function-of-temperature-by-saul-dushman)

### Richardson plot

↑ **Parent:** [Richardson-Dushman law](#richardson-dushman-law)

Choose a fixed positive reference $A_{\rm ref}$ with the same units as $A$. Taking the [natural logarithm](calculus.md#natural-logarithm) of a dimensionless ratio gives

$$
x=\frac1T,\qquad
y=\ln\!\left(\frac{J}{A_{\rm ref}T^2}\right)
=\ln\!\left(\frac{A}{A_{\rm ref}}\right)-\frac{W}{k_B}x.
$$

Thus the [Richardson plot](#richardson-plot) is a [straight line](euclidean-geometry.md#straight-line) when $A$ and $W$ are constant, with slope $-W/k_B$ and intercept $\ln(A/A_{\rm ref})$. The familiar notation $\ln(J/T^2)$ silently chooses units; the reference makes that choice explicit. Changing $A_{\rm ref}$ shifts the intercept and leaves the inferred [work function](quantum-mechanics.md#work-function) unchanged. If the horizontal axis instead uses $1000\,\mathrm K/T$, its slope is $-W/(1000\,\mathrm K\,k_B)$.

For the chosen $2.0\,\mathrm{eV}$ example, choose $A_{\rm ref}=120\,\mathrm{A\,cm^{-2}\,K^{-2}}$. Then $y(1000\,\mathrm K)=-23.2090$ and $y(1200\,\mathrm K)=-19.3409$. Their slope is approximately $-23209\,\mathrm K$, giving $W=2.0\,\mathrm{eV}$. Two [temperatures](temperature.md) determine a line algebraically; several [temperatures](temperature.md) allow curvature and drift to be detected. These values are calculated, rather than experimental observations.

<a id="image-one-chosen-emission-model-as-a-temperature-curve-and-a-dimensionless-richardson-plot"></a>
![](thermionic-emission-temperature-richardson-plot.png)

**[Figure 1](#image-one-chosen-emission-model-as-a-temperature-curve-and-a-dimensionless-richardson-plot). One chosen emission model as a temperature curve and a dimensionless Richardson plot**. The marked values are calculations with constant $W=2.0\,\mathrm{eV}$ and $A=A_{\rm ref}=120\,\mathrm{A\,cm^{-2}\,K^{-2}}$. They illustrate the [Richardson-Dushman law](#richardson-dushman-law), rather than a particular material or a historical measurement.

A straight trace alone does not establish a unique surface [work function](quantum-mechanics.md#work-function). [Adsorption](physical-chemistry.md#adsorption), changing [surface coverage](physical-chemistry.md#surface-coverage), or a mixture of regions with different barriers can change the inferred slope. For independent emitting patches with area fractions $f_i$, constant $A_i$ and barriers $W_i$,

$$
J=T^2\sum_i f_i A_i e^{-W_i/(k_BT)},\qquad \sum_i f_i=1.
$$

Lower barriers contribute disproportionately. Even with fixed patches, the slope of the [Richardson plot](#richardson-plot) gives a [temperature](temperature.md)-dependent weighted mean of the $W_i$, rather than their simple area average. If $A$ or $W$ themselves vary with [temperature](temperature.md), the apparent slope-derived barrier becomes

$$
W_{\rm app}=-k_B\frac{dy}{d(1/T)}
=W-T\frac{dW}{dT}+k_BT^2\frac{d\ln A}{dT}.
$$

Check collection, [temperature](temperature.md) calibration, and surface stability before assigning curvature to a new emission mechanism.

### Thermionic tail-flux derivation

↑ **Parent:** [Richardson-Dushman law](#richardson-dushman-law)

Consider a planar surface with outward normal along $z$. For an auxiliary equilibrium [electron gas](physics.md#electron-gas) just outside it, let $n_v$ be the total [number density](statistical-physics.md#number-density), counting both signs of $v_z$. Its [Maxwell-Boltzmann velocity distribution](quantum-ideal-gas-statistics.md#maxwell-boltzmann-velocity-distribution) has normal-component density

$$
f_z(v_z)=\sqrt{\frac{m_e}{2\pi k_BT}}
e^{-m_ev_z^2/(2k_BT)}.
$$

An [electron](physics.md#electron) with $v_z>0$ crosses more area per unit time when it moves faster. The outgoing number flux therefore uses $v_z f_z$, rather than just the probability of $v_z>0$:

$$
\Gamma=n_v\int_0^\infty v_zf_z(v_z)\,dv_z
=n_v\sqrt{\frac{k_BT}{2\pi m_e}}.
$$

This integral contributes only $T^{1/2}$. Holding a classical bulk [number density](statistical-physics.md#number-density) fixed and imposing a normal [kinetic energy](energy.md#kinetic-energy) threshold $W$ would instead give $\Gamma=n\sqrt{k_BT/(2\pi m_e)}e^{-W/(k_BT)}$; that argument alone does not produce $T^2$.

For the ideal surface model, measure external [electron](physics.md#electron) energies from the metal's [chemical potential](chemical-potential.md) $\mu$. A freely propagating external state has $E-\mu=W+p^2/(2m_e)$. When $W\gg k_BT$, its [Fermi-Dirac distribution](quantum-ideal-gas-statistics.md#fermi-dirac-distribution) reduces to the [Maxwell–Boltzmann statistics](quantum-ideal-gas-statistics.md#maxwell-boltzmann-statistics) tail. Counting two [spin](angular-momentum-operator.md#spin) states per [phase space](hamiltonian-mechanics.md#phase-space) cell of volume $h^3$ gives

$$
n_v=\frac{2}{h^3}\int_{\mathbb R^3}
e^{-[W+p^2/(2m_e)]/(k_BT)}\,d^3p
=2\left(\frac{2\pi m_e k_BT}{h^2}\right)^{3/2}
e^{-W/(k_BT)}.
$$

Each of the three [Gaussian integrals](integral.md#gaussian-integral) supplies $T^{1/2}$. Combining this $T^{3/2}$ state count with the $T^{1/2}$ crossing factor gives

$$
J=e\Gamma
=\frac{4\pi m_e e k_B^2}{h^3}\,T^2e^{-W/(k_BT)}.
$$

The auxiliary atmosphere supplies an equilibrium state-counting argument; an operating collector removes the outgoing [electrons](physics.md#electron). It need not maintain a real equilibrium gas throughout the gap. Unit transmission and the ideal free [electron](physics.md#electron) state count are substantive assumptions, so this calculation does not determine an arbitrary real surface's measured $A$.

In particular, [electrons](physics.md#electron) inside a [metal](chemical-substance.md#metal) generally form a degenerate [Fermi gas](quantum-ideal-gas-statistics.md#fermi-gas). A classical distribution for the escaping tail does not imply a classical distribution for the whole interior. Richardson himself emphasized this distinction in his lecture.[Nobel Lectures, Physics 1922–1941; pp. 230–231, internal versus external electron statistics](physics-bibliography.md#nobel-lectures-physics-1922-1941/thermionic-phenomena-and-the-laws-which-govern-them-by-owen-willans-richardson)

## Emission-limited thermionic current

↑ **Parent:** [Thermionic emission](thermionic-emission.md)

An [emission-limited thermionic current](#emission-limited-thermionic-current) is set by the rate at which the heated surface supplies [electrons](physics.md#electron), with nearly complete collection. At fixed [temperature](temperature.md), increasing the attracting [electric potential difference](electric-field.md#electric-potential-difference) then produces an approximate collection plateau. That plateau is the useful regime for fitting the [Richardson-Dushman law](#richardson-dushman-law), provided the [electric field](electric-field.md) has not significantly lowered the surface barrier.

The emitting surface still matters in this regime. [Adsorption](physical-chemistry.md#adsorption) changes the [work function](quantum-mechanics.md#work-function); different crystal faces can have different barriers. Heating may desorb contaminants or change a coating, so repeated measurements at the same [temperature](temperature.md) need not agree unless the surface preparation is controlled. For fixed $A,T$, a barrier change $\Delta W$ multiplies $J$ by $e^{-\Delta W/(k_BT)}$. In the chosen model at $1000\,\mathrm K$, raising the barrier by $0.10\,\mathrm{eV}$ reduces $J$ to about 0.313 of its previous value.

## Space-charge-limited thermionic current

↑ **Parent:** [Thermionic emission](thermionic-emission.md)

A [space-charge-limited thermionic current](#space-charge-limited-thermionic-current) occurs when the negative [space charge](electric-charge.md#space-charge) of emitted [electrons](physics.md#electron) creates an [electric field](electric-field.md) that obstructs further transport across the gap. Raising the emitter [temperature](temperature.md) may then increase the surface supply without producing the corresponding collector [electric current](electric-charge.md#electric-current). The gap geometry and collecting [electric potential difference](electric-field.md#electric-potential-difference) matter even when the surface is stable.

To distinguish this from an [emission-limited thermionic current](#emission-limited-thermionic-current), vary the collecting [electric potential difference](electric-field.md#electric-potential-difference) at fixed emitter [temperature](temperature.md), then repeat at another [temperature](temperature.md). A voltage-dependent transport region followed by a collection plateau separates a gap constraint from a supply constraint. A weak collector [electric current](electric-charge.md#electric-current) alone cannot establish a high [work function](quantum-mechanics.md#work-function). Nor does simply choosing a very large collecting [electric potential difference](electric-field.md#electric-potential-difference) guarantee a valid zero-field measurement: the surface barrier may then change.

## Richardson hot-wire emission experiment

↑ **Parent:** [Thermionic emission](thermionic-emission.md)

In his Nobel lecture, delivered on 12 December 1929 for the 1928 prize, [Owen Willans Richardson](physicist.md#owen-willans-richardson) recalled heating wires for weeks while hand-pumping away gas released by the apparatus. With [platinum](chemical-substance.md#platinum), he found a finite emission per unit area that rose rapidly with [temperature](temperature.md). His initial 1901 formula used $T^{1/2}$; he preferred the $T^2$ form in 1911.[Nobel Lectures, Physics 1922–1941; pp. 224–225 and 229, preparation and chronology](physics-bibliography.md#nobel-lectures-physics-1922-1941/thermionic-phenomena-and-the-laws-which-govern-them-by-owen-willans-richardson)

The early apparatus surrounded a heated [platinum](chemical-substance.md#platinum) wire with a metal cylinder connected to earth through a [galvanometer](electric-charge.md#galvanometer). Wire [electrical resistance](electric-charge.md#electrical-resistance) supplied the [temperature](temperature.md) readout. After checking collection saturation, Richardson measured at a wire potential of $-120\,\mathrm V$, over roughly $1300$–$1600\,\mathrm K$; reversing polarity suppressed the negative discharge.[Histories of the Electron: The Birth of Microphysics edited by Jed Z. Buchwald and Andrew Warwick; pp. 229–231, resistance thermometry and Fig. 7.2, reproducing the 1903 apparatus](physics-bibliography.md#histories-of-the-electron-the-birth-of-microphysics-edited-by-jed-z-buchwald-and-andrew-warwick/o-w-richardson-and-the-electron-theory-of-matter-1901-1916-by-ole-knudsen)

<a id="image-heated-wire-emission-and-separate-collection-and-temperature-measurements"></a>
![](thermionic-emission-hot-wire-collector.png)

**[Figure 2](#image-heated-wire-emission-and-separate-collection-and-temperature-measurements). Heated-wire emission and separate collection and temperature measurements**. Original functional schematic of the measurement principle, with a wire and surrounding collector shown in section. The layout is simplified; no dimensions or instrument performance are asserted.

The inference rests on several controls. A [temperature](temperature.md) sweep probes thermal escape; reversing the collecting [electric field](electric-field.md) tests the sign of the mobile [electric charge](electric-charge.md); varying collection voltage tests whether transport is limiting. Prolonged pumping and heating test whether a transient gas release is responsible. These controls address different alternatives, and none by itself establishes a clean, uniform surface.

For a modern repetition, stabilize each [temperature](temperature.md), measure the collector [electric current](electric-charge.md#electric-current) against collecting [electric potential difference](electric-field.md#electric-potential-difference), and record the pressure and surface preparation. Repeat selected [temperatures](temperature.md) after cooling to reveal drift. Use the collection plateau and the actual emitting area to construct a [Richardson plot](#richardson-plot). The resulting slope estimates the [work function](quantum-mechanics.md#work-function) only within the stated surface and transport assumptions; it does not turn an uncontrolled wire into a reference material.

## ↑ Ancestors (4)

1. [Electron](physics.md#electron)
2. [Subatomic particle](physics.md#subatomic-particle)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Nobel Prize in Physics in 1928](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1928)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2017/paper-1.md#section-a-i/1/i/solution)
- [Shot noise](electrical-engineering.md#shot-noise)
- [X-ray tube](electromagnetic-radiation.md#x-ray-tube)
