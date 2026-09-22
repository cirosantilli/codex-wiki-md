# Amplitude modulation sidebands

↑ **Parent:** [Amplitude modulation](amplitude-modulation.md)

Apply the [product-to-sum formula](product-to-sum-formula.md) to the voltage model:

$$
s(t)=A\cos(\omega_ct)
+\frac{Am}{2}\cos((\omega_c+\Omega)t)
+\frac{Am}{2}\cos((\omega_c-\Omega)t).
$$

The [carrier wave](carrier-wave.md) component has peak voltage [amplitude](wave-amplitude.md) $A$; each AM sideband has peak voltage [amplitude](wave-amplitude.md) $Am/2$. These are temporal [frequency spectrum](frequency-spectrum.md) components, unlike the [spatial sidebands](spatial-sideband.md) used in pattern stability. The separation $\Omega>0$ makes the three positive [angular frequencies](angular-frequency.md) distinct, and $\Omega<\omega_c$ keeps the lower one positive. The span between sidebands is $2\Omega$, or $2f_m$ in [hertz](hertz.md) when $f_m=\Omega/(2\pi)$; this is the single-tone span, not a universal [signal bandwidth](signal-bandwidth.md) for arbitrary messages.

A one-sided [cosine](cosine.md)-[amplitude](wave-amplitude.md) display assigns $A$ to the carrier line. A two-sided complex-exponential expansion instead assigns $A/2$ at each of $\pm\omega_c$, and $Am/4$ at each of the four sideband locations. The signal is identical; confusing the conventions creates a factor-of-two error. An ideal infinite-duration [sinusoid](sinusoid.md) gives a spectral line. A finite recording and finite analyser resolution broaden the displayed peak.

For a voltage applied across an ideal [resistor](resistor.md) of [electrical resistance](electrical-resistance.md) $R>0$, a component of peak voltage $B$ has [root mean square](root-mean-square.md) voltage $B/\sqrt2$ and mean [power](power.md) $B^2/(2R)$ by [Ohm's law](ohm-s-law.md). Thus

$$
P_c=\frac{A^2}{2R},\qquad
P_+=P_-=\frac{A^2m^2}{8R}=\frac{m^2}{4}P_c,\qquad
P_{\mathrm{tot}}=P_c\left(1+\frac{m^2}{2}\right).
$$

The proof of additivity is to average $s(t)^2/R$ over a long time: cross-products of distinct [frequencies](frequency.md) have zero mean. Consequently the whole signal's [root mean square](root-mean-square.md) voltage is $A\sqrt{(1+m^2/2)/2}$, not simply its maximum [wave envelope](envelope-waves.md) divided by $\sqrt2$. The carrier-component $A/\sqrt2$ remains unchanged as $m$ varies.

<a id="image-three-am-spectral-lines-peak-voltage-amplitudes-and-mean-powers"></a>
![](amplitude-modulation-sideband-amplitude-and-power.png)

**[Figure 7](#image-three-am-spectral-lines-peak-voltage-amplitudes-and-mean-powers). Three AM spectral lines: peak voltage amplitudes and mean powers**. Original one-sided spectra at $\omega_c/\Omega=20$, comparing $m=0.5$ and $1.4$. Peak voltages are normalized by $A$; component powers into the same resistor are normalized by $P_c=A^2/(2R)$. Equal-height carrier lines do not mean equal total power. The model has no extra lines when the signed factor changes sign.

With $A=2\,\mathrm V$, $R=50\,\Omega$ and $m=0.5$, the carrier supplies $40\,\mathrm{mW}$ and each $0.5\,\mathrm V$ peak sideband supplies $2.5\,\mathrm{mW}$, giving $45\,\mathrm{mW}$ total. At $m=1.4$ each sideband is $1.4\,\mathrm V$ peak and supplies $19.6\,\mathrm{mW}$, giving $79.2\,\mathrm{mW}$ total. Neither case changes the carrier-component [power](power.md).

The fraction of mean [power](power.md) in the message-bearing sidebands is $m^2/(2+m^2)$. It is $1/9$ at $m=0.5$ and $1/3$ at $m=1$. Conventional [AM](amplitude-modulation.md) spends the remaining [power](power.md) on a carrier that enables an inexpensive [envelope detector](envelope-detector.md). Increasing $m$ beyond $1$ increases this fraction in the linear model but breaks ordinary envelope recovery. Removing the carrier gives [suppressed-carrier amplitude modulation](suppressed-carrier-amplitude-modulation.md) and changes the receiver requirement.

**Table of contents**

- [Fourier filtering of overlapping amplitude-modulation sidebands](fourier-filtering-of-overlapping-amplitude-modulation-sidebands.md)

## ↑ Ancestors (3)

1. [Amplitude modulation](amplitude-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Amplitude modulation](amplitude-modulation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/4/a/solution.md)
