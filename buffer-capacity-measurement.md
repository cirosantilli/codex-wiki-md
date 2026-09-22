# Buffer capacity measurement

↑ **Parent:** [Buffer capacity](buffer-capacity.md)

A proposed modern measurement extends the [weak acid dissociation measurement](weak-acid-dissociation-measurement.md) by estimating the local slope of an [acid-base titration](acid-base-titration.md). Transfer a measured sample with a [pipette](pipette.md) into a stirred vessel; clamp a combination [glass electrode](glass-electrode.md)/[reference electrode](reference-electrode.md) clear of the stirring magnet and place a [temperature](temperature.md) probe nearby. A calibrated [burette](burette.md) delivers a [chemical base](base-chemistry.md) of independently standardized [concentration](concentration.md) $c_T$, such as [sodium hydroxide](sodium-hydroxide.md). Record the initial sample [volume](volume-thermodynamics.md) $V_0$, cumulative delivered [volume](volume-thermodynamics.md) $v$, stable [pH](ph.md), and [temperature](temperature.md) after each small addition. Use a separate fresh portion for an acidward series. These are proposed measurement conditions, not reported experimental results.

For the instrument calibration, use fresh standard [buffer solutions](buffer-solution.md) bracketing the measured [pH](ph.md) range, with values appropriate to the actual [temperature](temperature.md). The Hanna manual specifies separate rinse and calibration portions, gentle stirring, and approximately $4\,\mathrm{cm}$ immersion of the probe tip. It calls for stable readings; the sensing bulb and [reference electrode](reference-electrode.md) junction must remain immersed. Rinse between standards and samples and avoid carrying rinse [water](water.md) into the measured portion.[pp. 45–47: calibration portions, bracketing standards, temperature and immersion; pp. 49–50 and 74–75: stable readings, rinsing, junction immersion and drift](hi5221-and-hi5222-instruction-manual-ph-and-mv-and-ise-and-temperature-bench-meters-by-hanna-instruments.md)

The readout pairs each added [amount of substance](amount-of-substance.md) with the measured [pH](ph.md). With negligible added [volume](volume-thermodynamics.md), neighboring readings give the [finite difference](finite-difference-split.md) estimate

$$
\beta\approx\frac{c_T(v_{i+1}-v_i)}{V_0(\mathrm{pH}_{i+1}-\mathrm{pH}_i)},
$$

assigned to the interval's midpoint. High [buffer capacity](buffer-capacity.md) appears as a small change of [pH](ph.md) for a measured reagent dose. Choose increments small enough to resolve changing [buffer capacity](buffer-capacity.md), but large enough that the change of [pH](ph.md) exceeds measurement noise. Repeat with a fresh portion and different increment sizes; remeasure a standard afterward to check drift. A [water](water.md) blank can reveal contamination, but its [pH](ph.md) must not be subtracted from the sample [pH](ph.md). These controls are proposed tests of the measurement and model assumptions.

If additions appreciably increase [volume](volume-thermodynamics.md), even the [analytical concentration](analytical-concentration.md) changes: $C(v)=C_0V_0/(V_0+v)$. Merely dividing the added [moles](mole-unit.md) by the current [volume](volume-thermodynamics.md) does not restore the constant-[volume](volume-thermodynamics.md) [derivative](derivative.md). One alternative is explicitly to report a changing-volume convention. For $c(v)=c_Tv/(V_0+v)$, define

$$
\beta_V=\left|\frac{\mathrm dc}{\mathrm d\mathrm{pH}}\right|=\frac{c_TV_0}{(V_0+v)^2}\left|\frac{\mathrm dv}{\mathrm d\mathrm{pH}}\right|.
$$

This definition includes the reagent's changing [concentration](concentration.md) and differs from the constant-[volume](volume-thermodynamics.md) [buffer capacity](buffer-capacity.md) defined above.[§2, Definition of Dynamic Buffer Capacity, equations (1)–(3): reagent concentration in the combined volume and its derivative](dynamic-buffer-capacity-in-acid-base-systems-by-anna-m-michalowska-kaczmarczyk-and-tadeusz-michalowski.md)

To compare with the constant-[volume](volume-thermodynamics.md) theory, fit the changing-[volume](volume-thermodynamics.md) [chemical equilibrium](chemical-equilibrium.md) model instead of treating the observed slope as $\beta$. In the same ideal [monoprotic acid](monoprotic-acid.md) system, define $S_0=[\mathrm A^-]_0+[\mathrm{OH}^-]_0-[\mathrm H^+]_0$. For baseward additions, the [electric charge](electric-charge.md) balance at each reading is

$$
\frac{S_0V_0+c_Tv}{V_0+v}=\frac{C(v)K_a}{K_a+H}+c^\circ\left(\frac{K_w}{H}-H\right).
$$

Use a minus sign before $c_Tv$ for the corresponding acidward series. From the model parameters, evaluate the constant-[volume](volume-thermodynamics.md) [buffer capacity](buffer-capacity.md) at the chosen [analytical concentration](analytical-concentration.md) and [pH](ph.md). The fit also tests whether one [acid dissociation constant](acid-dissociation-constant.md) describes the observations.

Limitations include incomplete mixing, slow [glass electrode](glass-electrode.md) response, uncertain reagent [concentration](concentration.md), and changes in [temperature](temperature.md) or [ionic strength](ionic-strength.md). Dissolved atmospheric [carbon dioxide](carbon-dioxide.md) introduces an additional [chemical acid](acid-chemistry.md) system; comparable exposure and freshly prepared samples help distinguish it from the intended [monoprotic acid](monoprotic-acid.md) response. Additional reacting [chemical species](chemical-species.md) and nonideal [activity coefficients](activity-coefficient.md) invalidate the simple formula. Especially when [pH](ph.md) increments are tiny, measurement noise can dominate the inferred [derivative](derivative.md); reporting the dose, [pH](ph.md) interval, [volume](volume-thermodynamics.md) convention, and repeatability is part of reporting a meaningful [buffer capacity](buffer-capacity.md).

## ↑ Ancestors (5)

1. [Buffer capacity](buffer-capacity.md)
2. [Buffer solution](buffer-solution.md)
3. [Acid-base chemistry](acid-base-chemistry.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
