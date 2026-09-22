# Beer-Lambert measurement controls

↑ **Parent:** [Beer-Lambert law](beer-lambert-law.md)

An actual teaching experiment prepares a Kool-Aid stock by weighing powder, transferring it quantitatively into a [volumetric flask](volumetric-flask.md), and filling to the mark with [water](water.md). A Genesys 30 [spectrophotometer](spectrophotometer.md), blanked with [water](water.md) in a [cuvette](cuvette.md), scans for the peak [absorbance](absorbance.md) [wavelength](wavelength.md). A Genesys 10 then measures [absorbance](absorbance.md) at that [wavelength](wavelength.md), with a [water](water.md) [reference blank](reference-blank.md). Each [serial dilution](serial-dilution.md) transfers $50\,\mathrm{mL}$ of the preceding [chemical solution](solution-chemistry.md) to a $100\,\mathrm{mL}$ [volumetric flask](volumetric-flask.md) and fills to the mark; the protocol records the blank and sample readouts and repeats the halving sequence. These are prescribed experimental steps, not a published numerical data set.[Quantitative Analysis of Kool-Aid by Mary Jane Simpson, Procedure: Prepare Kool-Aid Stock Solution; Measure Peak Absorption of Kool-Aid Solution; Measure Absorbance of Solution at Various Concentrations, steps 1–5](quantitative-analysis-of-kool-aid-by-mary-jane-simpson.md)

The experiment tests whether [absorbance](absorbance.md) tracks the prepared [concentration](concentration.md). Its [concentration](concentration.md) is powder [mass](mass.md) per final [volume](volume-thermodynamics.md), so the calibration does not by itself supply a single dye's [molar absorption coefficient](molar-absorption-coefficient.md). The manual identifies loss of discrimination for very concentrated, very dilute, or very similar samples.[Quantitative Analysis of Kool-Aid by Mary Jane Simpson, Background: three limits on distinguishing samples; Procedure: stock preparation and concentration in grams per millilitre](quantitative-analysis-of-kool-aid-by-mary-jane-simpson.md)

To interpret such a calibration, hold [cuvette](cuvette.md) orientation fixed with its clear faces in the [light](light.md) path, keep fingerprints and bubbles out of that path, and keep the geometric [length](length.md) unchanged. Mix each [dilution](dilution.md) completely. Re-read the [reference blank](reference-blank.md) during the sequence and re-read one standard to test drift. A separate preparation of a standard checks errors propagated through [serial dilution](serial-dilution.md); repeating only its instrumental reading does not test the transferred [volumes](volume.md). These controls follow from keeping $P_0$, $l$, and $c$ comparable between readings.

Three mechanisms explain why a [straight line](straight-line.md) can fail. First, [scattering of light](scattering-of-light.md) can divert [radiant power](radiant-flux.md) away from the [photodetector](photodetector.md), so cloudiness can raise apparent [absorbance](absorbance.md) without the intended absorbing [solute](solute.md). A [reference blank](reference-blank.md) removes only losses shared with the sample. Second, [stray light](stray-light.md) reaching the [photodetector](photodetector.md) can make a strongly absorbing sample appear too transmissive. In an original model with extra detected [radiant power](radiant-flux.md) $sP_0$ in both readings,

$$
T_{\rm read}=\frac{10^{-\varepsilon lc}+s}{1+s},\qquad
A_{\rm read}=-\log_{10}T_{\rm read}.
$$

As the ideal [transmittance](transmittance.md) approaches zero, the reported [absorbance](absorbance.md) approaches $\log_{10}((1+s)/s)$ for $s>0$. This finite ceiling is a model prediction, not measured instrument performance.

Third, [chemical equilibrium](chemical-equilibrium.md) can redistribute the absorbing [chemical species](chemical-species.md) when [dilution](dilution.md), [pH](ph.md), or [temperature](temperature-split.md) changes. Even if each [chemical species](chemical-species.md) separately follows the [Beer-Lambert law](beer-lambert-law.md), their combined [absorbance](absorbance.md) is $A=l\sum_i\varepsilon_i c_i$, where $c_i$ is each species' [molar concentration](molar-concentration.md); changing those fractions need not preserve one effective [molar absorption coefficient](molar-absorption-coefficient.md). Thus an unknown should be compared with standards under matching [chemical solution](solution-chemistry.md) conditions, within the tested [concentration](concentration.md) range. A good [linear regression](linear-regression-split.md) alone does not establish chemical selectivity.

**Table of contents**

- [Reference blank](reference-blank.md)

## ↑ Ancestors (5)

1. [Beer-Lambert law](beer-lambert-law.md)
2. [Absorbance](absorbance.md)
3. [Physical chemistry](physical-chemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
