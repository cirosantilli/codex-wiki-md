# Photocurrent

↑ **Parent:** [Photodiode](photodiode.md)

[Photocurrent](photocurrent.md) is the [electric current](electric-current.md) attributable to illumination. Here $I_{\rm ph}\geq0$ denotes its magnitude after [background subtraction](background-subtraction.md). For a [photodiode](photodiode.md) without internal multiplication, let $P$ be incident [radiant flux](radiant-flux.md) concentrated at [wavelength](wavelength.md) $\lambda$, and let $\eta$ be external [quantum efficiency](quantum-efficiency.md), including losses before collection. An incident [photon](photon.md) has [energy](energy-split.md) $E_\gamma=hc/\lambda$, with [Planck constant](planck-constant.md) $h$ and [speed of light](speed-of-light.md) $c$. Dividing [energy](energy-split.md) per second by [energy](energy-split.md) per [photon](photon.md) gives the incident [photon](photon.md) rate $\Phi_\gamma$. Multiplying by $\eta$ gives the mean collected pair rate $\dot N_{\rm pair}$; multiplying by [elementary charge](elementary-charge.md) $q$ gives

$$
\Phi_\gamma=\frac{P\lambda}{hc},\qquad
\dot N_{\rm pair}=\eta\Phi_\gamma,\qquad
I_{\rm ph}=q\dot N_{\rm pair},\qquad
R(\lambda)=\frac{I_{\rm ph}}P=\frac{\eta q\lambda}{hc}.
$$

The factor is $q$: each collected pair replenishes an [electron](electron.md) at one contact and removes an [electron](electron.md) at the other. A cross-section of the external wire therefore counts one transferred [electron](electron.md) per completed pair, consistent with [charge conservation](charge-conservation.md). The [electron](electron.md) and [electron hole](electron-hole.md) are two internal [charge carriers](charge-carrier.md), not two independent transfers through that wire.

Choose an illustrative [photodiode](photodiode.md) model with $\lambda=650\,\mathrm{nm}$, $\eta=0.75$ and $P=1.00\,\mathrm{\mu W}$. Using the exact SI values $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$, $c=299792458\,\mathrm{m\,s^{-1}}$ and $q=1.602176634\times10^{-19}\,\mathrm C$ gives

$$
\begin{aligned}
E_\gamma&=3.05607055\times10^{-19}\,\mathrm J,\\
\Phi_\gamma&=3.27217577\times10^{12}\,\mathrm{s^{-1}},\\
\dot N_{\rm pair}&=2.45413183\times10^{12}\,\mathrm{s^{-1}},\\
R(650\,\mathrm{nm})&=0.393195267\,\mathrm{A\,W^{-1}},\\
I_{\rm ph}&=0.393195267\,\mathrm{\mu A}.
\end{aligned}
$$

A mean fraction $0.75$ does not require each fourth [photon](photon.md) to be lost in a repeating pattern. It specifies a mean conversion rate. Nor does $0.75$ mean $0.75\,\mathrm{A\,W^{-1}}$: [quantum efficiency](quantum-efficiency.md) is dimensionless, whereas [spectral responsivity](spectral-responsivity.md) compares [electric current](electric-current.md) with [power](power.md).

<a id="image-calculated-spectral-responsivity-photon-rate-and-photocurrent"></a>
![](photodiode-responsivity-and-photon-current.png)

**[Figure 15](#image-calculated-spectral-responsivity-photon-rate-and-photocurrent). Calculated spectral responsivity, photon rate and photocurrent**. Original model, not a measured device spectrum. Left: constant external [quantum efficiency](quantum-efficiency.md) $\eta=0.75$ is assumed only on the displayed [wavelength](wavelength.md) [interval](interval-mathematics.md) $450$–$800\,\mathrm{nm}$. Right: the $650\,\mathrm{nm}$ example at $1\,\mathrm{\mu W}$, with [photon](photon.md) and collected-pair rates distinguished.

At fixed [radiant flux](radiant-flux.md), longer-[wavelength](wavelength.md) [photons](photon.md) have less [energy](energy-split.md), so more arrive per second. This explains the rising [straight line](straight-line.md) when [quantum efficiency](quantum-efficiency.md) is held constant. A real [photodiode](photodiode.md)'s [quantum efficiency](quantum-efficiency.md) varies with [wavelength](wavelength.md); the plotted assumption cannot be extended past its [band gap](band-gap.md) absorption cutoff. At fixed incident [photon](photon.md) rate instead, $I_{\rm ph}=\eta q\Phi_\gamma$ has no additional factor of $\lambda$.

## ↑ Ancestors (7)

1. [Photodiode](photodiode.md)
2. [Photodetector](photodetector.md)
3. [Optical instrument](optical-instrument-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Balanced photodetection](balanced-photodetection.md)
- [Millikan photoelectric experiment](millikan-photoelectric-experiment.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-d/d13/c/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-d/d9/solution.md)
- [Photocurrent](photocurrent.md)
- [Photodiode](photodiode.md)
- [Photoelectric effect](photoelectric-effect.md)
- [Photoelectric saturation current](photoelectric-saturation-current.md)
- [Photoelectric threshold frequency](photoelectric-threshold-frequency.md)
- [Shot noise photocurrent measurement](shot-noise-photocurrent-measurement.md)
- [Siegert relation](siegert-relation.md)
- [Sirius intensity interferometry experiment](sirius-intensity-interferometry-experiment.md)
