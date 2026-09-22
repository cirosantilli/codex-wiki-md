# Cathode-ray attenuation with finite detector acceptance

↑ **Parent:** [Lenard cathode-ray window experiment](lenard-cathode-ray-window-experiment.md)

An original toy model separates two ways to lose a central [cathode ray](cathode-ray.md) signal. Let $x$ be forward depth into a uniform [gas](gas.md). Normalize the entering [electron](electron.md) population to one. Write $U(x)$ for the fraction still in a narrow forward channel, and $D(x)$ for the fraction diverted into a wider collection channel. Assume constant removal rate $a$ per unit depth in both channels, and constant transfer rate $b$ from $U$ to $D$, with no return. Removal means that an [electron](electron.md) stops or is trapped before reaching the collecting plane; it does not mean that its [electric charge](electric-charge-split.md) disappears. The wide ideal collector accepts all surviving members of both channels. This is a stipulated two-population [differential equation](differential-equation-split.md) model, not a general law of [electron](electron.md) transport:

$$
\frac{dU}{dx}=-(a+b)U,\qquad
\frac{dD}{dx}=bU-aD,\qquad
U(0)=1,\quad D(0)=0.
$$

The first equation gives [exponential decay](exponential-decay.md). Adding the equations gives $W'= -aW$ for $W=U+D$, hence

$$
U(x)=e^{-(a+b)x},\qquad
W(x)=e^{-ax},\qquad
D(x)=e^{-ax}\left(1-e^{-bx}\right).
$$

These formulas also give a conservation check: $U+D+(1-W)=1$. The fraction $1-W$ has been removed before the plane, while $D$ remains present but misses the narrow collector. An exponential fit to the narrow signal therefore measures $a+b$, not the removal rate $a$ by itself. This is an [identifiability](identifiability.md) issue: one declining signal cannot distinguish the two unknown rates.

For a worked example, choose $a=0.15\,\mathrm{cm^{-1}}$ and $b=0.35\,\mathrm{cm^{-1}}$. These are invented teaching inputs, not measured coefficients for air or Lenard's apparatus. At $x=2.00\,\mathrm{cm}$,

$$
U=e^{-1}\simeq0.3679,\qquad
W=e^{-0.3}\simeq0.7408,\qquad
D\simeq0.3729,\qquad
1-W\simeq0.2592.
$$

Thus about $63.2\%$ misses the narrow collector, although only about $25.9\%$ has been removed in this model. Treating the whole narrow-signal deficit as stopping would confuse redistribution with removal.

<a id="image-cathode-ray-attenuation-and-acceptance-model"></a>
![](cathode-ray-attenuation-and-acceptance-model.png)

**[Figure 7](#image-cathode-ray-attenuation-and-acceptance-model). Two collecting geometries distinguish redistribution from removal in a toy cathode ray model**. Original calculation with chosen constant rates $a=0.15\,\mathrm{cm^{-1}}$ and $b=0.35\,\mathrm{cm^{-1}}$. Left: fractions in the narrow channel, diverted channel, and removed population sum to one. Right: logarithmic plots of the narrow and wide surviving fractions have different slopes. The marked depth is $2\,\mathrm{cm}$. This model omits [electron](electron.md) slowing and return between channels; neither panel contains historical measurements.

Suppose a calibrated readout is proportional to arriving [electron](electron.md) number with the same response for either channel. Choose an empty-path signal $R_0=1020$ arbitrary units, of which $B=20$ is background; the two collection geometries have the same calibrated reference. The calculated readings at $2\,\mathrm{cm}$ are $R_{\rm n}=20+1000e^{-1}\simeq387.88$ and $R_{\rm w}=20+1000e^{-0.3}\simeq760.82$. After [background subtraction](background-subtraction.md), define $T_j=(R_j-B)/(R_0-B)$ for each geometry. Then the original [inverse problem](inverse-problem-split.md) has the solution

$$
a=-\frac{\ln T_{\rm w}}{x}=0.15\,\mathrm{cm^{-1}},\qquad
b=-\frac{\ln T_{\rm n}}{x}-a=0.35\,\mathrm{cm^{-1}}.
$$

A single narrow reading would instead allow every nonnegative pair with $a+b=0.50\,\mathrm{cm^{-1}}$. Using the raw ratios without subtracting $B$ gives an erroneous narrow rate of about $0.4834\,\mathrm{cm^{-1}}$. In a real [fluorescent screen](fluorescent-screen.md), the assumed response must be tested: deposited [energy](energy-split.md) and conversion to [light](light.md) need not remain constant as [electrons](electron.md) slow. Repeating the comparison at several depths tests the constant slopes, although straight slopes alone do not establish the microscopic mechanism.

Actual [electrons](electron.md) change [kinetic energy](kinetic-energy.md) and direction. [Electron stopping power](electron-stopping-power.md) $S(K)=-dK/ds>0$ describes mean [kinetic energy](kinetic-energy.md) loss per travelled [path length](arc-length.md) $s$; collisional losses include [ionization](ionization.md), while radiative losses include [bremsstrahlung](bremsstrahlung.md). The [continuous slowing-down approximation range](continuous-slowing-down-approximation-range.md) integrates reciprocal total [electron stopping power](electron-stopping-power.md), neglecting fluctuations. It approximates travelled [path length](arc-length.md), not forward penetration depth.[Stopping-Power and Range Tables for Electrons, Protons, and Helium Ions by M. J. Berger and others; Appendix: Significance of Calculated Quantities, collision/radiative/total stopping power, CSDA range, projected range and detour factor](stopping-power-and-range-tables-for-electrons-protons-and-helium-ions-by-m-j-berger-and-others/appendix-significance-of-calculated-quantities.md)

$$
R_{\mathrm{CSDA}}(K_0)=\int_0^{K_0}\frac{dK}{S(K)}.
$$

As a separate original limiting example, stipulate a straight path, constant $S=2\,\mathrm{keV\,cm^{-1}}$, and entering [kinetic energy](kinetic-energy.md) $K_0=6\,\mathrm{keV}$. Then $K(s)=6\,\mathrm{keV}-Ss$ until stopping, and $R_{\mathrm{CSDA}}=3\,\mathrm{cm}$. In that deterministic model every entering [electron](electron.md) reaches each depth below $3\,\mathrm{cm}$ and none crosses a plane beyond it. There is no exponential population tail. Real fluctuations and [electron scattering](electron-scattering.md) make the situation more complicated, but the example already proves that continuous [energy](energy-split.md) loss does not imply constant-rate removal.

The window also changes the entering population: source [kinetic energy](kinetic-energy.md) before the foil need not equal $K_0$ just outside it. For an [electron](electron.md) initially at rest, an ideal static accelerating [electric potential difference](electric-potential-difference.md) $V>0$ supplies electrical [work](work.md) $eV$, where $e$ is the [elementary charge](elementary-charge.md). If losses before and within the foil total $\Delta K\geq0$, a transmitted [electron](electron.md) enters the observation chamber with $K_0=eV-\Delta K\leq eV$. A screen's brightness determines neither $V$ nor $\Delta K$. These formulas specify a modern ideal [work-energy theorem](work-energy-theorem.md) argument; no numerical historical [voltage](voltage.md) or foil thickness is inferred from the diagram.

## ↑ Ancestors (9)

1. [Lenard cathode-ray window experiment](lenard-cathode-ray-window-experiment.md)
2. [Lorentz force](lorentz-force.md)
3. [Electromagnetic field tensor](electromagnetic-field-tensor.md)
4. [Electromagnetic four-potential](electromagnetic-four-potential.md)
5. [Relativistic electromagnetism](relativistic-electromagnetism-split.md)
6. [Electromagnetism](electromagnetism-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)
