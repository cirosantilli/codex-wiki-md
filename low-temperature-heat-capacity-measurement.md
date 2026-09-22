# Low-temperature heat capacity measurement

↑ **Parent:** [Heat capacity](heat-capacity.md)

Low-temperature [calorimetry](calorimetry-split.md) measures a small sample's [heat capacity](heat-capacity.md) by resolving a small [temperature](temperature-split.md) change after a known electrical [energy](energy-split.md) input. The experimental challenge is that the support, heater and [thermometer](thermometer.md) also warm up. Their [calorimeter addenda](calorimeter-addenda.md) must be removed before interpreting the sample's [phonons](phonon.md) or [electronic heat capacity](electronic-heat-capacity.md). The [Debye T-cubed test](debye-t-cubed-test.md) turns the corrected response into a test of the low-[temperature](temperature-split.md) vibrational spectrum.

[Manuel Brando](manuel-brando.md)'s 2009 experiment used a sapphire platform suspended by four alloyed platinum wires from a [copper](copper.md) ring fixed to a cryostat stage. Grease attached the sample; a chip heater and ruthenium-oxide [resistance thermometer](resistance-thermometer.md) served platform PLS-2. A controller stabilized the bath; a lock-in amplifier supplied heating pulses and read the calibrated sensor. The steady rise calibrated [thermal conductance](thermal-conductance.md) as $G=P/\Delta T$. A separate $59.1\,\mathrm{mg}$, $99.99\%$ pure [gold](gold.md) sample, compared with reference [heat capacities](heat-capacity.md), established the [calorimeter addenda](calorimeter-addenda.md). Small pulses limited property variation; imperfect sample contact required a second relaxation time. The platform contribution rose below $1.5\,\mathrm K$, making simple extrapolation unsafe.[Brando, Development of a relaxation calorimeter for temperatures between 0.05 and 4 K, §§II–IV.B, Table I, Figs. 4, 5 and 8: construction, calibration, contact correction and low-temperature platform upturn](development-of-a-relaxation-calorimeter-for-temperatures-between-0-05-and-4-k-by-manuel-brando.md)

For an original idealization, assume sample and platform share one [temperature](temperature-split.md) $T$, the bath remains at $T_b$, and both the total [heat capacity](heat-capacity.md) and the weak-link [thermal conductance](thermal-conductance.md) $G$ are approximately constant across one small pulse. Ignore other [heat transfer](heat-transfer.md) and any [phase transition](phase-transition.md). The [first law of thermodynamics](first-law-of-thermodynamics-split.md) becomes

$$
(C_s+C_a)\frac{dT}{dt}=P(t)-G(T-T_b),\qquad
\tau=\frac{C_s+C_a}{G}.
$$

Here $C_s$ is sample [heat capacity](heat-capacity.md), $C_a$ is [calorimeter addenda](calorimeter-addenda.md), $P$ is deposited electrical [power](power.md) from [Joule heating](joule-heating.md), and $\tau$ is a [time constant](time-constant.md). This is the same balance as [calorimeter heat-loss correction](calorimeter-heat-loss-correction.md), used here with a deliberately weak cryogenic link and a separately subtracted platform. For a constant pulse $P_0$ beginning at bath [temperature](temperature-split.md), then switched off at $t_h$,

$$
T(t)-T_b=\begin{cases}
\dfrac{P_0}{G}(1-e^{-t/\tau}),&0\le t\le t_h,\\
\dfrac{P_0}{G}(1-e^{-t_h/\tau})e^{-(t-t_h)/\tau},&t>t_h.
\end{cases}
$$

The cooling [exponential decay](exponential-decay.md) determines $\tau$, while the heating plateau determines $G=P_0/(T_\infty-T_b)$. Together with [calorimeter addenda](calorimeter-addenda.md), they give $C_s=G\tau-C_a$. Cooling alone determines a ratio, not an absolute [heat capacity](heat-capacity.md). With finite $t_h$, the observed end rise is smaller than the plateau; fit the full response or apply the displayed correction rather than identifying the two.

<a id="image-a-cryogenic-pulse-probes-sample-plus-calorimeter-addenda-through-a-weak-thermal-link"></a>
![](low-temperature-calorimeter-pulse-response.png)

**[Figure 12](#image-a-cryogenic-pulse-probes-sample-plus-calorimeter-addenda-through-a-weak-thermal-link). A cryogenic pulse probes sample plus calorimeter addenda through a weak thermal link**. Original constructed one-[temperature](temperature-split.md) model, not a drawing of Brando's apparatus or measured data. The bath is fixed at $2.000\,\mathrm K$, the heater supplies $2\times10^{-9}\,\mathrm W$ for $100\,\mathrm s$, and the total [heat capacity](heat-capacity.md) is $10^{-6}\,\mathrm{J\,K^{-1}}$. Internal sample-platform [thermal equilibrium](thermal-equilibrium-split.md) is assumed instantaneous; the actual experiment can require two relaxation times.

For the stipulated figure parameters, $G=5.00\times10^{-8}\,\mathrm{W\,K^{-1}}$, $\tau=20.0\,\mathrm s$, and $C_a=2.00\times10^{-7}\,\mathrm{J\,K^{-1}}$ give $C_s=8.00\times10^{-7}\,\mathrm{J\,K^{-1}}$. The asymptotic rise is $0.0400\,\mathrm K$, only $2\%$ of bath [temperature](temperature-split.md). At $100\,\mathrm s$, the rise is $0.0397305\,\mathrm K$. Of $2.00\times10^{-7}\,\mathrm J$ input, only $3.97305\times10^{-8}\,\mathrm J$ remains stored: the other $1.60270\times10^{-7}\,\mathrm J$ has flowed to the bath. Treating this long pulse as an isolated $Q/C$ experiment would overestimate total [heat capacity](heat-capacity.md) by a factor of $5.034$.

Suppose independent [standard uncertainties](standard-uncertainty.md) are $u(G)=0.05\times10^{-8}\,\mathrm{W\,K^{-1}}$, $u(\tau)=0.2\,\mathrm s$ and $u(C_a)=0.10\times10^{-7}\,\mathrm{J\,K^{-1}}$. First-order [propagation of uncertainty](propagation-of-uncertainty.md) gives

$$
u(C_s)^2=\tau^2u(G)^2+G^2u(\tau)^2+u(C_a)^2,
\qquad C_s=(8.00\pm0.17)\times10^{-7}\,\mathrm{J\,K^{-1}}.
$$

The uncertainty is one [standard deviation](standard-deviation.md) under those assumptions, about $2.2\%$ of sample [heat capacity](heat-capacity.md). Shared [thermometer calibration](thermometer-calibration.md) errors can correlate fitted $G$ and $\tau$; then their [covariance](covariance.md) contributes too. Smaller samples amplify the relative influence of [calorimeter addenda](calorimeter-addenda.md). Proposed checks include varying pulse amplitude, repeating with a reference sample, checking sensor self-heating, and comparing single- and two-time-constant fits. A drifting bath, slow internal equilibration or a transition invalidates this simple reduction even if a cooling curve looks smooth.

**Table of contents**

- [Calorimeter addenda](calorimeter-addenda.md)

## ↑ Ancestors (7)

1. [Heat capacity](heat-capacity.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
