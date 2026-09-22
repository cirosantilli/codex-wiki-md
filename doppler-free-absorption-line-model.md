# Doppler-free absorption line model

↑ **Parent:** [Doppler-free saturation spectroscopy](doppler-free-saturation-spectroscopy.md)

Construct an original illustrative spectrum using ordinary [frequency](frequency.md) detuning $x=\nu_L-\nu_0$. Write the longitudinal [Doppler shift](doppler-effect.md) in frequency units as $u=v/\lambda_0$, where $\lambda_0=c/\nu_0$. Choose a [normal distribution](normal-distribution.md) with [standard deviation](standard-deviation.md) $\sigma_D$ and a weak-probe [Lorentzian line shape](lorentzian-line-shape.md) with half width at half maximum $\gamma_\nu$:

$$
g(u)=\frac{e^{-u^2/(2\sigma_D^2)}}{\sqrt{2\pi}\sigma_D},\qquad
L(y)=\frac{\gamma_\nu^2}{y^2+\gamma_\nu^2},\qquad
B(x)=\frac{\int_{-\infty}^{\infty}g(u)L(x-u)\,du}
{\int_{-\infty}^{\infty}g(u)L(-u)\,du}.
$$

Thus $B(0)=1$. Choose $\sigma_D=120\ \mathrm{MHz}$ and [natural linewidth](natural-linewidth.md) $\Gamma/(2\pi)=6\ \mathrm{MHz}$, so $\gamma_\nu=3\ \mathrm{MHz}$. The Gaussian-only [full width at half maximum](full-width-at-half-maximum.md) is $2\sqrt{2\ln2}\,\sigma_D\simeq282.58\ \mathrm{MHz}$; the averaged profile also includes the finite [Lorentzian line shape](lorentzian-line-shape.md) width.

Add a deliberately phenomenological [Lamb dip](lamb-dip.md):

$$
A_s(x)=B(x)-\frac{C_s}{1+4x^2/w_s^2},\qquad
C_s=0.24\frac{s}{1+s},\qquad
w_s=\frac{\Gamma}{2\pi}\sqrt{1+s}.
$$

Here $A_s$ is the [absorption coefficient](absorption-coefficient.md) normalized to the pump-off line-centre value. The factor $0.24$ is chosen, not inferred from populations or a fit. The dip's assigned [full width at half maximum](full-width-at-half-maximum.md) $w_s$ borrows the single-atom [power broadening](power-broadening.md) scale purely to illustrate contrast versus width. It is not the preceding overlap integral or a fit to historical spectra. There are no crossover features in this isolated-transition toy spectrum.

For $s=1$, the subtracted dip has depth $0.12$ and width $8.49\ \mathrm{MHz}$; for $s=9$, depth $0.216$ and width $18.97\ \mathrm{MHz}$. Its half-depth points are $x=\pm w_s/2$. Measure that width relative to the curved background $B(x)$, not a horizontal line through the total absorption minimum.

<a id="image-chosen-doppler-envelope-and-phenomenological-lamb-dips"></a>
![](saturation-spectroscopy-chosen-doppler-envelope-and-dip.png)

**[Figure 10](#image-chosen-doppler-envelope-and-phenomenological-lamb-dips). Chosen Doppler envelope and phenomenological Lamb dips**. Original numerical Gaussian velocity average with two explicitly chosen Lorentzian absorption dips. Every numerical setting is illustrative. The right panel magnifies line centre; these curves are not experimental data or fits.

For a chosen cell [optical depth](optical-depth.md) $\tau_s(x)=0.4A_s(x)$, the line-centre pump-off transmission is $e^{-0.4}\simeq0.6703$. At $s=1$ it is $e^{-0.352}\simeq0.7033$. The transmitted probe therefore increases by about $4.92$ percent relative to pump off. Absorption contrast, transmission contrast and spectral width are three different quantities.

## ↑ Ancestors (6)

1. [Doppler-free saturation spectroscopy](doppler-free-saturation-spectroscopy.md)
2. [Laser spectroscopy](laser-spectroscopy.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Lamb dip](lamb-dip.md)
