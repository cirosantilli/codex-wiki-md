# Beer-Lambert calibration model

↑ **Parent:** [Beer-Lambert law](beer-lambert-law.md)

Choose an ideal absorbing [chemical species](chemical-species.md) with $\varepsilon=8000\,\mathrm{L\,mol^{-1}\,cm^{-1}}$ at a fixed [wavelength](wavelength.md), and a [cuvette](cuvette.md) with geometric [length](length.md) $l=1\,\mathrm{cm}$. These are stipulated model parameters. A micromolar [molar concentration](molar-concentration.md) is $1\,\mu\mathrm M=10^{-6}\,\mathrm{mol\,L^{-1}}$, so each additional $25\,\mu\mathrm M$ gives $\Delta A=8000\times1\times25\times10^{-6}=0.2$. Five chosen standards therefore predict

$$
\begin{array}{c|ccccc}
c\;(\mu\mathrm M)&0&25&50&75&100\\
A&0&0.2&0.4&0.6&0.8\\
T&1&0.63096&0.39811&0.25119&0.15849
\end{array}
$$

The [absorbance](absorbance.md) [graph](graph-split.md) is a [straight line](straight-line.md) of [slope](slope.md) $0.008\,(\mu\mathrm M)^{-1}$, while the [transmittance](transmittance.md) [graph](graph-split.md) shows [exponential decay](exponential-decay.md). Equal increments of [molar concentration](molar-concentration.md) multiply [transmittance](transmittance.md) by $10^{-0.2}\approx0.63096$; they do not subtract a fixed transmitted fraction.

<a id="image-beer-lambert-absorbance-transmission-calibration"></a>
![](beer-lambert-absorbance-transmission-calibration.png)

**[Figure 8](#image-beer-lambert-absorbance-transmission-calibration). Linear absorbance and exponential transmittance describe the same calibration model**. Original exact model curves for $\varepsilon=8000\,\mathrm{L\,mol^{-1}\,cm^{-1}}$ and $l=1\,\mathrm{cm}$; circles mark the five stipulated standards, not measured material data. The highlighted $T=0.40$ reading corresponds to $A=\log_{10}(2.5)$ and $c\approx49.7425\,\mu\mathrm M$. The common horizontal [molar concentration](molar-concentration.md) scale lets the two panels show the same inversion.

Suppose a measurement returns the stipulated blank-normalized reading $T=0.40$ under those same conditions. The inferred [absorbance](absorbance.md) and [molar concentration](molar-concentration.md) are

$$
A=-\log_{10}(0.40)=\log_{10}(2.5)\approx0.3979400,
\qquad
c=\frac{\log_{10}(2.5)}{8000\times1}\,\mathrm{mol\,L^{-1}}
\approx49.7425\,\mu\mathrm M.
$$

This lies slightly below the $50\,\mu\mathrm M$ standard because $0.40$ is slightly above $10^{-0.4}\approx0.39811$. A calibration determined experimentally by [linear regression](linear-regression-split.md) may instead have $A=mc+b$. Then use $c=(A-b)/m$, keeping the [slope](slope.md) $m$ and [intercept](regression-intercept.md) $b$ in their measured units. A nonzero [intercept](regression-intercept.md) calls for checking the [reference blank](reference-blank.md) and sample preparation; it does not uniquely identify the cause.

## ↑ Ancestors (5)

1. [Beer-Lambert law](beer-lambert-law.md)
2. [Absorbance](absorbance.md)
3. [Physical chemistry](physical-chemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
